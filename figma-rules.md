---
name: vitrina-figma-rules
description: "Vitrina figma rules as Skills"
---

<!-- version: 2 | updated: 2026-04-22 | changelog: ایجاد تغییرات در فایل ایجاد شده توسط claude -->

# Figma Rules — Vitrina
> قوانین اجباری برای طراحی صفحات در فیگما
> این فایل را همیشه قبل از هر کار در فیگما بخوان

---

## ۱. قوانین پایه — هیچ‌وقت نقض نکن

1. **همیشه Auto Layout** — هیچ Frame معمولی (بدون Auto Layout) نساز و اگر نیاز شد مگر برای موارد خاص
2. **هیچ مقدار hard-coded** — همیشه از design system tokens استفاده کن
3. **فونت فقط Vazirmatn** — قبل از هر text node: `await figma.loadFontAsync({family: "Vazirmatn", style: "..."})`
4. **جهت RTL** — همه Auto Layout ها `layoutDirection: "HORIZONTAL"` با `RTL` در نظر بگیر
5. **قبل از ساخت، جستجو کن** — از `search_design_system` یا inspect موجود برای یافتن component استفاده کن

---

## ۲. نام‌گذاری

### لایه‌ها
- **زبان:** انگلیسی
- **فرمت:** `PascalCase` برای frame/group — `kebab-case` برای component جدید
- **مثال‌های درست:**

```
Page
├── Navbar
└── Body
    ├── Main
    │   ├── Page-Header
    │   └── Content
    │       ├── Start
    │       ├── Middle
    │       └── End
    └── Sidebar
```

### Components جدید
- **فرمت:** `Kebab-Case` با خط تیره
- **مثال:** `Product-Card`، `Order-Status`، `Shipping-Method`
- **Variant properties:** `PascalCase` — مثال: `State`، `Selected`، `IsDefault`
- **Variant values:** `PascalCase` — مثال: `Default`، `Hover`، `Disabled`

---

## ۳. Sizing — Fill / Hug / Fixed

| المان | Horizontal | Vertical |
|-------|-----------|---------|
| Page | Fixed (1920px) | Hug |
| Body | Fill | Fill |
| Main | Fill | Fill |
| Content | Fill | Hug |
| ستون‌های Start/End (fixed) | Fixed | Fill |
| ستون Middle | Fill (با max-width) | Hug (معمولاً) |
| Sidebar | Fixed (256px) | Fill |
| Navbar | Fill | Fixed |
| Component داخلی | Fill | Hug (معمولاً) |

**قانون مهم:** `layoutSizingHorizontal/Vertical = 'FILL'` را فقط **بعد از** `parent.appendChild(child)` تنظیم کن — قبلش error می‌ده.

---

## ۴. ساختار صفحه

همیشه از template های تعریف‌شده در `page-template.md` استفاده کن:

| Template | Start | Middle | End | Sidebar |
|----------|-------|--------|-----|---------|
| 1 Column Fill | — | fill | — | 256px |
| 1 Column Center | — | max 960px | — | 256px |
| 2 Column Right Center | 256px | max 960px | — | 256px |
| 2 Column Right Fill | 256px | fill | — | 256px |
| 3 Column | 256px | max 960px | 288px | 256px |

**Spacing داخل صفحه:**
- Main: `padding: 16px` — `gap: 16px` - `flow: vertical`
- Content: `padding: 24px` — `gap: 40px` - `flow: horizontal`

> اگه template مشخص نشد → **1 Column Center** به عنوان default

---

## ۵. Component سازی

**چه موقع component بساز:**
- یه element چندین بار در صفحه تکرار می‌شه
- element نیاز به states مختلف داره (Hover، Selected، Disabled)

**ساختار variant set:**
```
Component-Name (COMPONENT_SET)
├── State=Default
├── State=Hover
├── State=Selected
└── State=Disabled
```

**قوانین:**
- همیشه `combineAsVariants` برای ساخت variant set استفاده کن
- حداقل `State=Default` و `State=Hover` داشته باش
- Boolean properties: `IsDefault`، `IsSelected`، `IsOpen` (با `Is` شروع کن)

---

## ۶. رنگ و استایل

- **هیچ‌وقت** hex مستقیم نده — از variable binding استفاده کن
- رنگ‌ها از `chakra-ui-v3-fa.md` یا `project-context.md`
- برای text: `node.textStyleId` را با style از DS ست کن
- برای shadow: `node.effectStyleId` را با effect style از DS ست کن
- برای fill/stroke: از `setBoundVariableForPaint` استفاده کن

---

## ۷. کار با کامپوننت‌های موجود

**اولویت استفاده:**
1. **Local components** (فایل Vitrina) ← از `component-inventory.md` نام دقیق را پیدا کن
2. **DS components** (Chakra UI) ← از `search_design_system` جستجو کن
3. **ساخت جدید** ← فقط اگه در هیچ‌کدام نبود

**Clone کردن:**
```js
// همیشه اول import، بعد clone
const component = await figma.importComponentByKeyAsync(key);
const instance = component.createInstance();
parent.appendChild(instance);
// بعد از appendChild، sizing را تنظیم کن
instance.layoutSizingHorizontal = 'FILL';
```

---

## ۸. قوانین Plugin API — خلاصه حیاتی

```js
// ✅ درست — رنگ 0 تا 1
node.fills = [{type: 'SOLID', color: {r: 0.05, g: 0.58, b: 0.53}}]

// ✅ درست — font قبل از text
await figma.loadFontAsync({family: "Vazirmatn", style: "Regular"});
node.characters = "متن";

// ✅ درست — FILL بعد از appendChild
parent.appendChild(child);
child.layoutSizingHorizontal = 'FILL';

// ✅ درست — page switch
await figma.setCurrentPageAsync(page);

// ❌ اشتباه — هرگز
figma.notify()          // throw می‌ده
console.log()           // برنمی‌گرده
figma.currentPage = p   // کار نمی‌کنه
```

**همیشه return کن:**
```js
return { createdNodeIds: [...], mutatedNodeIds: [...] }
```

---

## ۹. Workflow طراحی صفحه جدید

```

اگر لینک frame ستون middle در template صفحه جدید رو بهت دادم یک راست برو به شماره ۴
اگر لینک رو ندادم اول سوال کن و اگر ندادم از شماره ۱ شروع کن و اگر دادم از شماره ۴ شروع کن

۱. template را از page-template.md انتخاب کن
۲. تو Figma، template مناسب را clone کن
۳. لینک frame ستون Middle (یا Start/End) را بگیر
۴. داکیومنت صفحه را بخوان
۵. کامپوننت‌های لازم را از component-inventory.md شناسایی کن
۶. هر section را جداگانه بساز (یه use_figma call = یه section)
۷. بعد از هر section با get_screenshot validate کن
۸. پس از پایان برای screenshot ازم سوال کن و اگر اوکی دادم screenshot کامل صفحه را چک کن
```

---

## ۱۰. چک‌لیست قبل از هر use_figma

- [ ] فونت load شده؟ (`loadFontAsync` قبل از هر text)
- [ ] رنگ‌ها 0-1 هستند؟ (نه 0-255)
- [ ] `FILL` بعد از `appendChild` تنظیم شده؟
- [ ] page switch با `setCurrentPageAsync` انجام شده؟
- [ ] همه node IDs در `return` هستند؟
- [ ] از token استفاده شده؟ (نه hex مستقیم)
- [ ] نام‌گذاری لایه‌ها انگلیسی و با convention درسته؟
