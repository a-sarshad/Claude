---
name: vitrina-project-context
description: "Use for ALL tasks related to Vitrina project — variables, local styles, feature flags, and project-specific settings. Load automatically for any Vitrina design or development task."
---

<!-- version: 1 | updated: 2026-04-22 | changelog: توضیحات -->

# 
# این فایل فقط مختص پروژه Vitrina است


## معرفی پروژه
- نام: Vitrina
- Component Library: Chakra UI v3 (فارسی‌شده)
- زبان: فارسی / RTL
- DS پایه: Chakra UI [v3] FA (موجود در Project Knowledge)

---

## Grid System

### Main Grid
- Pattern: 12 ستون
- Gutter: 16px
- Margin: 16px

### Card 10 Stretch Grid
- Pattern: 10 ستون
- Gutter: 16px
- Margin: 24px

---

## Breakpoints (Screen Collection)

| نام | عرض | Size/Screen |
|-----|-----|-------------|
| Mobile | 480px | 1920px canvas |
| Desktop | 1440px | 1440px |
| Wide | 1920px | 1920px |

### Layout در هر Breakpoint

| متغیر | 480 | 1440 | 1920 |
|--------|-----|------|------|
| Size/Navbar | 512px | 1440px | 1920px |
| Size/Main | 512px | 1184px | 1664px |
| Content Column/Start | 0 | 256px | 256px |
| Content Column/Middle | 512px | 808px | 960px |
| Content Column/End | 0 | 236px | 288px |

---

## Boolean Variables (Feature Flags)

| Variable | مقدار پیش‌فرض | کاربرد |
|----------|----------------|--------|
| Theme/Light | true | حالت روشن |
| Theme/Dark | false | حالت تاریک |
| Theme/isChecked | false | وضعیت تاگل تم |
| Products/Show Discount | false | نمایش تخفیف |
| Products/Show Selected-Prd CTA | true | نمایش CTA محصول انتخابی |
| Products/Currency/Show Currency-Alert | false | نمایش هشدار ارز |
| Badge | true | نمایش badge |
| btnScreen/Show Maximize | false | دکمه maximize |
| btnScreen/Show Minimize | true | دکمه minimize |

---

## String Variables

| Variable | مقدار | کاربرد |
|----------|-------|--------|
| Products/Currency/Currency | تومان | واحد پول نمایش محصولات |

---

## نکات مهم پروژه
1. سه breakpoint اصلی: 480 (موبایل)، 1440 (دسکتاپ)، 1920 (وایدسکرین)
2. Navbar عرض کامل صفحه رو می‌گیره
3. Content area در 1440 و 1920 از سمت راست شروع می‌شه (256px offset)
4. محصولات دارای سیستم discount و currency جداگانه‌ان
5. پشتیبانی از Dark/Light mode از طریق boolean variables