<!-- version: 1 | updated: 2026-04-22 | changelog: توضیحات -->

# Context
[محتوای chakra-ui-ds-context-v2.md]
[محتوای vitrina-project-context.md]

---

# درخواست طراحی صفحه جدید

## اطلاعات پایه
- نام صفحه: [مثلاً: لیست محصولات]
- هدف صفحه: [کاربر می‌خواد چیکار کنه — یه جمله]
- Breakpoint هدف: [480 / 1440 / 1920]

## Layout مرجع
از template خالی Vitrina استفاده کن:
https://www.figma.com/design/CfbQjlet5WMabrTfZt46iL/Vitrina?node-id=281-5698

ساختار ثابت (دست نزن):
- Navbar: 64px — full width
- Sidebar: 256px — سمت راست
- Main: 1664px
- Middle column (محل محتوا): 960px — با offset 336px از چپ
- Page Header: شامل breadcrumb + عنوان + دکمه CTA اختیاری

## محتوای صفحه
بخش‌هایی که باید در Middle column طراحی بشن:

### بخش ۱: [نام]
- هدف: [چی نشون میده]
- محتوا: [چه المان‌هایی داره]
- Component پیشنهادی Chakra: [اگه می‌دونی]

### بخش ۲: [نام]
- هدف: ...
- محتوا: ...

## قوانین خاص این صفحه
- [مثلاً: جدول باید قابلیت sort داشته باشه]
- [مثلاً: هر ردیف باید دکمه Edit و Delete داشته باشه]
- [مثلاً: state خالی باید نمایش داده بشه]

## خروجی مورد نیاز
لطفاً به ترتیب بده:
1. ساختار لایه‌های پیشنهادی (مثل همان متادیتای Figma)
2. Component های Chakra UI که باید استفاده بشن با props اصلی
3. Spacing و sizing دقیق بر اساس DS tokens
4. State های مختلف که باید طراحی بشن (empty، loading، error)
5. نکات UX مهم برای این صفحه