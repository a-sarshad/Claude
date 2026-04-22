<!-- version: 2 | updated: 2026-04-22 | changelog: تصحیح نام و مشخصات تمام کامپوننت ها -->

# Component Inventory — Vitrina
> منبع: DesignBridge-Desktop.md (2026-04-21)
> تمام کامپوننت‌های این فایل **local** هستند (ساخته‌شده در فایل پروژه Vitrina)
> ممکن است داخل هر کامپوننت از Chakra UI DS استفاده شده باشد

---

## راهنمای استفاده برای Claude

- **منبع همه کامپوننت‌ها:** فایل Vitrina (local) — نه DS خارجی
- **برای clone یا جستجو:** از `search_design_system` با نام دقیق Figma استفاده کن
- **نام دقیق Figma:** همان نام ستون «Figma Name» است — variant را با `,` جدا کن
- **اگر component در DS خارجی نیاز بود:** از `search_design_system` در فایل Chakra UI DS جستجو کن

---

## گروه‌بندی کامپوننت‌ها

### ۱. Layout & Navigation

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Navbar** | `Navbar` | `Type=Dashboard \| Website` | 1952×176px | هدر اصلی داشبورد و وبسایت فروشنده |
| **Sidebar** | `Sidebar` | standalone (no variants) | 256×1016px | سایدبار کامل — شامل همه Sidebar-Item‌ها |
| **Sidebar-Item** | `Sidebar-Item` | `Selected=false\|true, State=Default\|Hover\|Disabled` | 256×208px | آیتم پایه منوی سایدبار |
| **Sidebar-Item/Dashboard** | `Sidebar-Item/Dashboard` | `Open=false\|true` | 256×232px | منوی اکوردیون داشبورد در سایدبار |
| **Sidebar-Item/Products** | `Sidebar-Item/Products` | `Open=false\|true` | 256×232px | منوی اکوردیون محصولات در سایدبار |
| **Sidebar-Item/Orders** | `Sidebar-Item/Orders` | `Open=false\|true` | 256×196px | منوی اکوردیون سفارشات در سایدبار |
| **Sidebar-Item/Financial** | `Sidebar-Item/Financial` | `Open=false\|true` | 256×232px / 256×196px | منوی اکوردیون امور مالی در سایدبار |
| **Sidebar-Item/Customers** | `Sidebar-Item/Customers` | `Open=false\|true` | 256×304px | منوی اکوردیون مشتریان در سایدبار |
| **Sidebar-Item/Theme** | `Sidebar-Item/Theme` | `Open=false\|true` | 256×196px | منوی اکوردیون قالب در سایدبار |
| **Sidebar-Item/Setting** | `Sidebar-Item/Setting` | `Open=false\|true` | 256×268px / 256×196px | منوی اکوردیون تنظیمات در سایدبار |
| **SlideMenu-Item** | `SlideMenu-Item` | `Selected=false\|true, State=Default\|Hover` | 256×208px | آیتم منوی slide-out |
| **SubLine** | `SubLine` | `State=Default\|Hover/Select` | 90×54px | زیرمنوی کوچک / tab indicator |
| **Split Menu** | `Split Menu` | `State=Pending\|Canceled\|Processing\|Returned\|Paid\|Sent, Open=false` | 980×68px | منوی تقسیم‌شده وضعیت سفارش |

---

### ۲. Page Structure

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Page-Header** | `Page-Header` | `Size=2xl-24\|xl-20\|l-18` | 1024×232px | هدر صفحات داخلی با عنوان و دکمه‌ها |
| **Title-Bar** | `Title-Bar` | `Size=xl-20\|lg-18\|md-16` | 992×242px | تایتل‌بار بخش‌های داخل صفحه |
| **Button-Footer** | `Button-Footer` | standalone | 960×56px | فوتر ثابت با دکمه‌های submit/cancel |
| **btnScreenSize** | `btnScreenSize` | `Type=maximize\|minimize` | 64×112px | دکمه تغییر اندازه پنجره |

---

### ۳. Product Management

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Product-Card** | `Product-Card` | `State=Default\|Hover\|Selected` | 1066×361px | کارت محصول در لیست محصولات |
| **Product-Status** | `Product-Status` | `Status=Published\|Draft\|Inactive\|Archived` | 100×172px | نشانگر وضعیت انتشار محصول |
| **Product-Amount** | `Product-Amount` | `Type=Number\|Not Available\|Infinity` | 86×134px | نمایش موجودی محصول |
| **Product-TelSale** | `Product-TelSale` | `Enabled=False\|true` | 992×558px | بخش فروش تلفنی محصول |
| **Thumbnail** | `Thumbnail` | `State=Default\|Hover, DefaultImage=true\|false` | 293×257px | تامبنیل تصویر محصول |
| **UploadedImage-Card** | `UploadedImage-Card` | `State=Default\|Hover, isDefault=true\|false` | 342×632px | کارت تصویر آپلودشده در گالری |
| **File-Upload** | `File-Upload` | `Property 1=FileUpload\|Uploaded-File` | 432×344px | کامپوننت آپلود فایل |
| **Currency-Switch** | `Currency-Switch` | `Type=Toman\|Dollar` | 341×175px | سوئیچ واحد پول |
| **Variant-Accordion** | `Variant-Accordion` | `Open=false\|true` | 992×298px | اکوردیون تنوع‌های محصول |
| **Color** | `Color` | `State=Default\|Hover\|Selected` | 134×310px | انتخاب‌گر رنگ محصول |

---

### ۴. Category Management

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Category-Accordion** | `Category-Accordion` | `State=Default\|Hover\|Open, Selected=false\|true` | 1340×432px | اکوردیون دسته‌بندی در انتخاب دسته محصول |
| **Category-Mng Accordion** | `Category-Mng Accordion` | `State=Default\|Hover\|Open, Sub category=Yes\|No` | 1276×558px | اکوردیون مدیریت دسته‌بندی‌ها |
| **SubCategory-Grip** | `SubCategory-Grip` | `State=Default\|Hover` | 600×144px | آیتم زیردسته در اکوردیون |
| **SubCategory-Item** | `SubCategory-Item` (standalone) | — | 94×32px | تگ/چیپ زیردسته |

---

### ۵. Shipping

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Shipping-Local** | `Shipping-Local` | `State=inactive\|active` | 992×457px | بخش ارسال درون‌شهری |
| **Shipping-OutRange** | `Shipping-OutRange` | `State=inactive\|active empty\|active fill` | 992×1392px | بخش ارسال خارج از محدوده |
| **Shipping-Card Custom** | `Shipping-Card Custom` | `State=Default\|Hover\|Disabled` | 504×712px | کارت روش ارسال سفارشی |
| **Shipping-Card System** | `Shipping-Card System` | `State=Default\|Hover\|Disabled\|Comming Soon` | 504×696px | کارت روش ارسال سیستمی |
| **Shipping-Method** | `Shipping-Method` | `Type=Free\|Const\|Weight Based` | 109×124px | نشانگر نوع محاسبه هزینه ارسال |
| **Shipping-Price Item** | `Shipping-Price Item` (standalone) | — | 197×36px | آیتم نمایش قیمت ارسال |

---

### ۶. Order Management

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Order-Status** | `Order-Status` | `Status=Waiting\|Paid\|Payment\|Sent\|Returned\|Canceled` | 124×252px | وضعیت سفارش |
| **Manual-Customer** | `Manual-Customer` | `State=Default\|Hover\|Selected` | 432×300px | انتخاب دستی مشتری در سفارش |
| **Manual-Product** | `Manual-Product` | `State=Default\|Hover\|Selected` | 544×316px | انتخاب دستی محصول در سفارش |
| **Manual-Discount** | `Manual-Discount` | `State=Default\|Hover\|Selected` | 432×342px | انتخاب دستی تخفیف در سفارش |
| **Manual-Shipping** | `Manual-Shipping` | `State=Default\|Hover\|Selected` | 400×424px | انتخاب دستی روش ارسال در سفارش |
| **Sender-Card** | `Sender-Card` | `State=Default\|Hover\|Selected` | 432×288px | کارت انتخاب فرستنده |

---

### ۷. Settings & Account

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Setting-Card** | `Setting-Card` | `State=Default\|Hover\|Disabled` | 537×476px | کارت تنظیمات فروشگاه |
| **Theme-Card** | `Theme-Card` | `isSelected=false\|true, State=Default\|Hover\|Coming Soon` | 734×935px | کارت انتخاب قالب ظاهری |
| **2Factor-Card** | `2Factor-Card` | `State=Default\|Hover\|Selected` | 617×312px | کارت احراز هویت دو مرحله‌ای |
| **Phone-Card** | `Phone-Card` | `State=Default\|Hover` | 504×216px | کارت شماره تلفن |
| **Social-Card** | `Social-Card` | `State=Default\|Hover` | 504×216px | کارت شبکه اجتماعی |
| **Address-Card** | `Address-Card` | `State=Default\|Hover\|Disabled` | 504×1024px | کارت آدرس |

---

### ۸. Auth & Onboarding

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Signup-Accordion** | `Signup-Accordion` | `State=Default\|Hover\|Open, Selected=false\|true` | 1286×324px | اکوردیون مراحل ثبت‌نام |
| **Invitation-Code** | `Invitation-Code` | `Property=Default\|Variant2` | 592×136px | فیلد کد دعوت |

---

### ۹. Misc / Utility

| Component | Figma Name | Variants | Frame Size | کاربرد |
|-----------|------------|----------|------------|--------|
| **Card-Adv** | `Card-Adv` (standalone) | — | 224×136px | کارت تبلیغاتی / بنر کوچک |
| **CommingSoon-Tag** | `CommingSoon-Tag` (standalone) | — | 117×40px | تگ «به زودی» |

---

## آمار کلی

| دسته | تعداد |
|------|-------|
| Variant Sets | 49 |
| Standalone Components | 6 |
| **جمع کل** | **55** |

---