<!-- version: 2 | updated: 2026-04-22 | changelog: توضیحات -->

# Page Templates — Vitrina Dashboard
> همیشه همراه با `component-inventory.md` و `project-context.md` استفاده شود

---

## مشخصات کلی

| مشخصه | مقدار |
|--------|-------|
| عرض canvas (desktop base) | 1920px |
| عرض Sidebar | 256px — ثابت |
| جهت | RTL |

---

## ساختار لایه‌بندی استاندارد

```
Page
├── Navbar                          ← fill container | محتوا max 1920px
└── Body  [horizontal auto layout]
    ├── Main  [vertical auto layout]
    │   │   width: fill container
    │   │   padding: 16px
    │   │   gap: 16px
    │   ├── Page-Header (component - اگر از قبل در صفحه موجود بود نیازی به ساخت مجدد نیست)
    │   └── Content  [horizontal auto layout]
    │       │   padding: 24px
    │       │   gap: 40px
    │       ├── Start   ← ستون راست (RTL — اول رندر می‌شود)
    │       ├── Middle  ← ستون مرکزی
    │       └── End     ← ستون چپ
    └── Sidebar (component)         ← width: 256px — fixed
```

### قوانین نام‌گذاری ستون‌ها در RTL

| نام | موقعیت | توضیح |
|-----|---------|-------|
| **Start** | راست | در RTL، شروع از راست — اول رندر می‌شود |
| **Middle** | مرکز | ستون اصلی محتوا |
| **End** | چپ | در RTL، انتها سمت چپ |

> این نام‌گذاری با CSS logical properties هم‌خوانی دارد.
> در صورت تبدیل به LTR، فقط ترتیب رندر عوض می‌شود — نام‌ها ثابت می‌مانند.

---

## Responsive Behavior

| المان | canvas = 1920px | canvas < 1920px | tablet/mobile |
|-------|----------------|----------------|---------------|
| **Navbar** | fill container — محتوا max 1920px | fill container — کوچک می‌شه | fill container |
| **Sidebar** | 256px fixed | 256px fixed | hamburger در Navbar — hidden |
| **Main** | fill container | fill container — کوچک می‌شه | fill container |
| **Middle column** | max-width خاص هر template | fill container — کوچک می‌شه | fill container |

---

## Spacing

### Main Frame
| مشخصه | مقدار |
|--------|-------|
| width | fill container |
| padding | 16px (همه طرف) |
| gap | 16px |

### Content Frame
| مشخصه | مقدار |
|--------|-------|
| width | fill container |
| padding | 24px (همه طرف) |
| gap | 40px |

### عرض‌های محاسبه‌شده در canvas 1920px
| لایه | محاسبه | نتیجه |
|------|--------|-------|
| Body | 1920 − 256 (Sidebar) | 1664px |
| Main | 1664 − 16×2 (padding) | 1632px |
| Content | 1632 − 24×2 (padding) | 1584px |

---

## Template ها

> ابعاد و سایز ستون‌ها ممکن است در برخی صفحات متفاوت باشد — در داکیومنت آن صفحه مشخص می‌شود.

---

### 1. 1 Column Fill
> **Figma:** https://www.figma.com/design/CfbQjlet5WMabrTfZt46iL/Vitrina?node-id=1984-27376&t=MC27TP1VjEnFONmR-11

```
Content (1584px)
└── Middle — fill container
```

| ستون | width | sizing |
|------|-------|--------|
| Middle | fill container | max 1584px در canvas 1920 |

**کاربرد:** لیست محصولات، جداول داده، داشبورد اصلی

---

### 2. 1 Column Center
> **Figma:** https://www.figma.com/design/CfbQjlet5WMabrTfZt46iL/Vitrina?node-id=281-5698&t=MC27TP1VjEnFONmR-11

```
Content (1584px)
└── Middle — max 960px | fill در canvas کوچک‌تر
```

| ستون | width | sizing |
|------|-------|--------|
| Middle | 960px max | fill container در canvas کوچک‌تر |

**کاربرد:** فرم‌های تک‌ستونه، تنظیمات، ثبت اطلاعات

> **default** — اگه template مشخص نشد از این استفاده کن

---

### 3. 2 Column Right Center
> **Figma:** https://www.figma.com/design/CfbQjlet5WMabrTfZt46iL/Vitrina?node-id=281-5732&t=MC27TP1VjEnFONmR-11

```
Content (1584px)
├── Start  — 256px fixed     ← راست
└── Middle — max 960px fill  ← مرکز
```

| ستون | موقعیت | width | sizing |
|------|---------|-------|--------|
| Start | راست | 256px | fixed |
| Middle | مرکز | 960px max | fill در canvas کوچک‌تر |

**کاربرد:** پنل اطلاعات جانبی (راست) + محتوای اصلی (مرکز)

---

### 4. 2 Column Right Fill
> **Figma:** https://www.figma.com/design/CfbQjlet5WMabrTfZt46iL/Vitrina?node-id=281-5708&t=MC27TP1VjEnFONmR-11

```
Content (1584px)
├── Start  — 256px fixed  ← راست
└── Middle — fill         ← مرکز/چپ
```

| ستون | موقعیت | width | sizing |
|------|---------|-------|--------|
| Start | راست | 256px | fixed |
| Middle | مرکز | fill container | max ~1288px در canvas 1920 |

**کاربرد:** محتوای گسترده + پنل کوچک جانبی راست

---

### 5. 3 Column
> **Figma:** https://www.figma.com/design/CfbQjlet5WMabrTfZt46iL/Vitrina?node-id=281-5719&t=MC27TP1VjEnFONmR-11

```
Content (1584px)
├── Start  — 288px fixed     ← راست
├── Middle — max 960px fill  ← مرکز
└── End    — 256px fixed     ← چپ
```

| ستون | موقعیت | width | sizing |
|------|---------|-------|--------|
| Start | راست | 288px | fixed |
| Middle | مرکز | 960px max | fill در canvas کوچک‌تر |
| End | چپ | 256px | fixed |

**کاربرد:** ناوبری/فیلتر (Start-راست) + محتوای اصلی (Middle) + اطلاعات جانبی (End-چپ)

---

## خلاصه مقایسه‌ای

| Template | Start (راست) | Middle (مرکز) | End (چپ) | Sidebar |
|----------|-------------|--------------|---------|---------|
| 1 Column Fill | — | fill (max 1584px) | — | 256px |
| 1 Column Center | — | fill (max 960px) | — | 256px |
| 2 Column Right Center | 256px | fill (max 960px) | — | 256px |
| 2 Column Right Fill | 256px | fill | — | 256px |
| 3 Column | 288px | fill (max 960px) | 256px | 256px |

---

## نکات مهم برای Claude

1. **همه frame ها Auto Layout** — هیچ frame معمولی استفاده نکن
2. **Main و Content همیشه fill container** — عرض ثابت نده
3. **Start = راست / End = چپ** در RTL
4. **ترتیب رندر در Content:** Start → Middle → End (از راست به چپ)
5. **Sidebar در tablet/mobile** hidden می‌شود — hamburger در Navbar جای آن را می‌گیرد
6. **ابعاد ستون‌ها** ممکن است در برخی صفحات متفاوت باشد — داکیومنت آن صفحه را چک کن
7. اگه template مشخص نشد → **1 Column Center** به عنوان default
