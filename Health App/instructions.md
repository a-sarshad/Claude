# instructions | v2 | 2026-04-29

# Health App — Claude Instructions

## زبان
- پاسخ‌ها همیشه **فارسی** — مگر اینکه کاربر خلافش بگوید

---

## طراحی Artifact (HTML/CSS)

چون Chakra UI در artifact پشتیبانی نمی‌شود، از **HTML + CSS خالص یا Tailwind CDN** استفاده کن.

| تنظیم | مقدار |
|-------|-------|
| رنگ Primary | `#0D9488` |
| Background | `#F0FDFA` / `#FFFFFF` |
| Text | `#0F172A` |
| Muted | `#64748B` |
| فونت | Vazirmatn از `https://fonts.googleapis.com/css2?family=Vazirmatn` |
| جهت | همیشه `dir="rtl"` روی `<html>` |
| Layout | Mobile-First — max-width: 390px برای موبایل |

### نام‌گذاری Artifact
- نام artifact: شامل شماره نسخه — مثلاً `health-home-v1`, `health-chat-v2`
- **خط اول داخل کد**: همیشه کامنت مشخصات به این فرمت:

```html
<!-- health-home | v1 | 2026-04-29 -->
```

---

## وقتی صفحه طراحی می‌کنی

1. ساختار کلی را توضیح بده
2. سپس artifact را بساز
3. بعد از artifact برای توضیح بیشتر اول ازم سوال کن — اگر خواستم توضیح بده

---

## وقتی Prompt برای Figma Make / claude.ai/design می‌نویسی

- رنگ‌ها را hex بنویس
- از Chakra UI component name استفاده کن
- layout و spacing و typography را مشخص کن
- RTL را صریح ذکر کن

---

## کد واقعی (Chakra UI v3)

- از `ds-chakra-ui-fa` skill استفاده کن
- RTL حفظ شود
- فونت Vazirmatn
- **هیچ‌وقت props را حدس نزن** — ابتدا مستندات را از `chakra-ui.com/docs` بررسی کن

---

## محدودیت‌های پزشکی (مهم!)

- هرگز توصیه پزشکی قطعی نده
- همیشه disclaimer بده: «این اطلاعات جایگزین مشاوره پزشکی نیست»
- AI باید **empathetic** و **supportive** باشد
