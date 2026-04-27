---
name: ds-chakra-ui-fa
description: "Use for ALL UI design and code tasks in Vitrina project that involve colors, typography, spacing, components, or tokens. Load automatically when working with Chakra UI design system, writing JSX/CSS, or making any visual decisions in Vitrina."
---

<!-- version: 2 | updated: 2026-04-24 | changelog: اضافه شدن بخش Chakra UI MCP fallback و web_fetch strategy -->

# Chakra UI [v3] FA — Rules
> نسخه فشرده برای استفاده در Skill
> داده‌های کامل (color tokens، text styles، shadows) در `chakra-ui-v3-fa.md` موجود است

---

## قوانین پایه — همیشه اعمال کن

1. **RTL** — همیشه `dir="rtl"` روی root المان
2. **فونت** — فقط `Vazirmatn` (open-source، قابل `loadFontAsync`)
3. **Token** — هیچ‌وقت مقدار hard-coded نده — همیشه از token name استفاده کن
4. **Component** — از Chakra UI v3 components استفاده کن

---

## رنگ‌های کلیدی پروژه

| کاربرد | Token | Hex |
|--------|-------|-----|
| Primary | `teal/solid` | `#0D9488` |
| خطا | `red/solid` | `#DC2626` |
| موفقیت | `green/solid` | `#16A34A` |
| هشدار | `orange/solid` | `#EA580C` |
| پس‌زمینه | `bg/default` | `#FFFFFF` (light) |
| متن اصلی | `fg/default` | `#000000` (light) |
| متن فرعی | `fg/muted` | `#52525B` (light) |
| بوردر | `border/default` | `#E4E4E7` (light) |

---

## Typography — قوانین انتخاب سایز

| موقعیت | Text Style |
|--------|-----------|
| body / فرم | `sm/font-normal` — 14px/400 |
| label / caption | `xs/font-medium` — 12px/500 |
| عنوان بخش | `md/font-semibold` — 16px/700 |
| عنوان صفحه | `xl/font-semibold` — 20px/700 |
| عنوان بزرگ | `2xl/font-bold` — 24px/700 |

> جدول کامل text styles در `chakra-ui-v3-fa.md`

---

## Spacing — قوانین استفاده

| کاربرد | Token | مقدار |
|--------|-------|-------|
| فاصله کوچک (icon gap) | `2` | 8px |
| padding داخلی کوچک | `3` | 12px |
| padding استاندارد | `4` | 16px |
| فاصله بین المان‌ها | `6` | 24px |
| فاصله بین بخش‌ها | `10` | 40px |

> جدول کامل spacing در `chakra-ui-v3-fa.md`

---

## Border Radius — قوانین انتخاب

| المان | Token | مقدار |
|-------|-------|-------|
| Badge / Tag | `Radii/Semantic/l2` | 4px |
| Input / Button | `Radii/Semantic/l2` | 4px |
| Card / Panel | `Radii/Semantic/l3` | 6px |
| Modal / Drawer | `Radii/lg` | 8px |
| Avatar / Pill | `Radii/full` | 9999px |

---

## Shadow — قوانین انتخاب

| المان | Token |
|-------|-------|
| Card | `Shadows/light/sm` |
| Dialog / Modal | `Shadows/light/lg` |
| Dropdown | `Shadows/light/md` |
| Tooltip | `Shadows/light/xs` |

---

## Component Size — استاندارد

| کامپوننت | size | ارتفاع |
|----------|------|--------|
| Input / Button / Select | `md` | 40px |
| Input / Button | `sm` | 32px |
| Input / Button | `lg` | 48px |
| Icon Button | `md` | 40×40px |

> اگه size مشخص نشد → `md` به عنوان default

---

## قوانین رنگ بر اساس وضعیت

| وضعیت | رنگ border | رنگ bg | رنگ text |
|-------|-----------|--------|---------|
| default | `border/default` | `bg/default` | `fg/default` |
| focus | `teal/solid` + focus ring | — | — |
| error | `border/error` | `bg/error` | `fg/error` |
| success | `border/success` | `bg/success` | `fg/success` |
| disabled | `border/muted` | `bg/muted` | `fg/subtle` |

---

## Chakra UI MCP — استراتژی دسترسی به مستندات

### وضعیت MCP
Chakra UI MCP server (`@chakra-ui/react-mcp`) یک **stdio-based** server است و فقط در Claude Code / Cursor / VS Code قابل استفاده‌ست — **در claude.ai در دسترس نیست**.

### جایگزین: web_fetch از مستندات رسمی

هر بار که component ای ناشناخته بود یا props آن مبهم بود، **قبل از حدس زدن** از web_fetch استفاده کن:

| نیاز | URL برای fetch |
|------|---------------|
| لیست همه components | `https://chakra-ui.com/docs/components/concepts/overview` |
| props یک component خاص | `https://chakra-ui.com/docs/components/[component-name]` |
| design tokens کامل | `https://chakra-ui.com/docs/theming/overview` |
| مثال کد یک component | `https://chakra-ui.com/docs/components/[component-name]#usage` |

### الگوی URL ها

```
Button    → https://chakra-ui.com/docs/components/button
Input     → https://chakra-ui.com/docs/components/input
Select    → https://chakra-ui.com/docs/components/select
Table     → https://chakra-ui.com/docs/components/table
Dialog    → https://chakra-ui.com/docs/components/dialog
Drawer    → https://chakra-ui.com/docs/components/drawer
Badge     → https://chakra-ui.com/docs/components/badge
Tag       → https://chakra-ui.com/docs/components/tag
Tabs      → https://chakra-ui.com/docs/components/tabs
```

### قانون استفاده

1. اگه component در `chakra-ui-v3-fa.md` موجود بود → همان را استفاده کن
2. اگه component ناشناخته یا props مبهم بود → `web_fetch` از URL مربوطه
3. **هیچ‌وقت props را حدس نزن** — اشتباه در props باعث کد غیرقابل اجرا می‌شود

---

## یادآوری‌های مهم

- داده‌های کامل color tokens → `chakra-ui-v3-fa.md`
- اگه token نامشخص بود → از PK سرچ کن، مقدار حدس نزن
- dark mode tokens جدا هستند — پیش‌فرض light mode است مگر خلافش گفته شود
- اگه component ناشناخته بود → web_fetch از chakra-ui.com/docs قبل از هر اقدام
