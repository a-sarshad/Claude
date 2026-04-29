# Health & Wellness App — Project Brief v2

## توضیح پروژه

یک اپلیکیشن هوشمند در حوزه بهداشت و سلامت که به‌عنوان یک **دستیار شخصی AI** عمل می‌کند. هدف اصلی کمک به کاربران برای بهبود کیفیت زندگی از طریق راهنمایی‌های شخصی‌سازی‌شده است. این اپ روی هوش مصنوعی بنا شده و ابزارهایی برای پایش جسم، ذهن، تغذیه، ورزش و سلامت روان ارائه می‌دهد.

**پلتفرم**: PWA (در آینده: Native App)  
**زبان هدف**: فارسی (RTL)  
**مخاطب**: تمام سنین

---

## Tech Stack

- **Frontend**: React + TypeScript
- **UI Library**: Chakra UI v3 (RTL + Vazirmatn)
- **AI Engine**: Anthropic Claude API (`claude-sonnet-4-20250514`)
- **Platform**: PWA → Native

---

## Design Direction

| ویژگی | انتخاب |
|-------|--------|
| سبک | Modern Medical + Warm Tech |
| رنگ اصلی | Teal `#0D9488` |
| فونت | Vazirmatn |
| جهت | RTL |
| مود | Light (پیش‌فرض) + Dark آماده |
| لحن | دوستانه، حرفه‌ای، انگیزه‌بخش |

---

## ماژول‌های اصلی (از MindMap)

### 1. 🎭 Daily Mood Tracking
ردیابی روزانه حال و هوای کاربر با هوش مصنوعی

| Feature | توضیح |
|---------|-------|
| Emotion Check-ins | ثبت احساسات روزانه |
| Mood Patterns Analysis | تحلیل الگوهای خلقی در طول زمان |
| Trigger Identification | شناسایی محرک‌های احساسی — AI می‌پرسد: «چه چیزی باعث این احساس شد؟» |
| Progress Visualization | نمایش گرافیکی پیشرفت خلقی |

---

### 2. 💬 Conversational Interface (AI Chat)
رابط مکالمه‌ای چندوجهی با دستیار هوشمند

| Feature | توضیح |
|---------|-------|
| Voice Interaction | مکالمه صوتی با AI |
| Video Interaction | تعامل ویدیویی |
| Text Chat Option | چت متنی ساده |
| Natural Language Processing | پردازش زبان طبیعی فارسی |
| Personalized Questions | سوالات شخصی‌سازی‌شده بر اساس پروفایل |

---

### 3. 🤖 AI Feedback System
سیستم بازخورد هوشمند چندحسی

| Feature | توضیح |
|---------|-------|
| Voice Tone Analysis | تحلیل لحن صدای کاربر |
| Facial Expression Recognition | تشخیص حالت چهره |
| Sentiment Detection | تشخیص احساسات از متن |
| Behavioral Insights | بینش‌های رفتاری بلندمدت |

---

### 4. 🏋️ Virtual Exercise Coach
مربی ورزشی مجازی شخصی‌سازی‌شده

| Feature | توضیح |
|---------|-------|
| Personalized Workouts | برنامه تمرینی اختصاصی |
| Form Correction | تصحیح فرم حرکات ورزشی |
| Progress Tracking | ردیابی پیشرفت ورزشی |
| Adaptive Difficulty | تنظیم خودکار سختی تمرین‌ها |

---

### 5. 👤 User Profile
پروفایل جامع کاربر

| Feature | توضیح |
|---------|-------|
| Personal Info | اطلاعات پایه (سن، وزن، قد، جنسیت، هدف) |
| Notifications | تنظیم یادآورها و اعلان‌ها |
| Partnership | ارتباط با شریک/ارائه‌دهنده خدمات |

---

### 6. 📱 Smart Device Integration
اتصال به دستگاه‌های هوشمند

| Feature | نوع | توضیح |
|---------|-----|-------|
| Heart Rate Monitoring | Native | پایش ضربان قلب |
| Sleep Quality Data | Native | داده‌های کیفیت خواب |
| Step Counter | Native | شمارش قدم‌ها |
| Blood Pressure | Native | فشار خون |
| Muscle Mass | Partner | از طریق شریک تجاری |
| Body Fat | Partner | از طریق شریک تجاری |
| Calorie Tracking | Partner | از طریق شریک تجاری |

---

### 7. 🧠 Mental Health Support
حمایت از سلامت روان

| Feature | توضیح |
|---------|-------|
| AI Feedback | بازخورد هوشمند وضعیت روانی |
| Stress Management Tips | راهکارهای مدیریت استرس |
| Meditation Guides | راهنمای مدیتیشن گام‌به‌گام |
| Breathing Exercises | تمرین‌های تنفسی |
| Therapy Resources | منابع و معرفی متخصص |

---

### 8. 🥗 Nutrition Guidance
راهنمای تغذیه هوشمند

| Feature | نوع | توضیح |
|---------|-----|-------|
| Meal Suggestions | Native | پیشنهاد وعده غذایی |
| Hydration Reminders | Native | یادآور آب خوردن |
| Caloric Intake | Partner | محاسبه کالری (شریک) |
| Dietary Preferences | Native | ثبت ترجیحات غذایی |
| Suggestion Based on Data | Native | پیشنهاد بر اساس داده‌های کاربر |

---

### 9. 📊 Health Reports
گزارش‌های جامع سلامت

| Feature | توضیح |
|---------|-------|
| Medical File (EHR) | پرونده پزشکی الکترونیک |
| Goal Achievement | پیشرفت در اهداف (مثل: کاهش وزن) |
| Recommendations | توصیه‌های شخصی‌سازی‌شده |
| Physical Prediction | پیش‌بینی وضعیت جسمی آینده |
| Doctor Sharing Option | اشتراک‌گذاری گزارش با پزشک |

---

## صفحات (Screens) و اولویت‌بندی

| # | صفحه | ماژول‌های مرتبط | اولویت |
|---|------|-----------------|--------|
| 1 | Onboarding | User Profile | 🔴 |
| 2 | Home / Dashboard | همه | 🔴 |
| 3 | AI Chat | Conversational Interface | 🔴 |
| 4 | Mood Check-in | Daily Mood Tracking | 🔴 |
| 5 | Exercise | Virtual Exercise Coach | 🟡 |
| 6 | Nutrition | Nutrition Guidance | 🟡 |
| 7 | Mental Health | Mental Health Support | 🟡 |
| 8 | Health Reports | Health Reports | 🟡 |
| 9 | Device Integration | Smart Device Integration | 🟠 |
| 10 | Profile & Settings | User Profile | 🟠 |

---

## Instructions برای Claude (این پروژه)

### زبان
- پاسخ‌ها همیشه **فارسی** — مگر اینکه کاربر خلافش بگوید

### طراحی Artifact (HTML/CSS)
- چون Chakra UI در artifact پشتیبانی نمی‌شود، از **HTML + CSS خالص یا Tailwind CDN** استفاده کن
- رنگ‌ها: Primary `#0D9488`, Background `#F0FDFA` / `#FFFFFF`, Text `#0F172A`, Muted `#64748B`
- فونت: `Vazirmatn` از `https://fonts.googleapis.com/css2?family=Vazirmatn`
- همیشه `dir="rtl"` روی `<html>` یا root
- طراحی **Mobile-First** (max-width: 390px برای موبایل)
- نام artifact: همیشه متفاوت، مثلاً `health-home-v1`, `health-chat-v2`

### وقتی صفحه طراحی می‌کنی
1. ساختار کلی را توضیح بده
2. سپس artifact را بساز
3. بعد از artifact توضیح دهی از المان‌های کلیدی بده

### وقتی Prompt برای Figma Make / claude.ai/design می‌نویسی
- رنگ‌ها را hex بنویس
- از Chakra UI component name استفاده کن
- layout و spacing و typography را مشخص کن
- RTL را صریح ذکر کن

### کد واقعی (Chakra UI v3)
- از `ds-chakra-ui-fa` skill استفاده کن
- RTL حفظ شود
- فونت Vazirmatn
- هیچ‌وقت props را حدس نزن — ابتدا مستندات را بررسی کن

### محدودیت‌های پزشکی (مهم!)
- هرگز توصیه پزشکی قطعی نده
- همیشه disclaimer: «این اطلاعات جایگزین مشاوره پزشکی نیست»
- AI باید empathetic و supportive باشد

### Partner Features
فیچرهایی که با برچسب **(Partner)** مشخص شده‌اند (Muscle Mass، Body Fat، Caloric Intake، Calorie Tracking) از طریق شریک تجاری ارائه می‌شوند — در طراحی با badge «Partner» یا آیکون متفاوت نشان بده.

---

## نکات فنی PWA

```
manifest.json
Service Worker (offline support)
Responsive: 320px → 1440px
CSS Custom Properties برای theming
Lazy loading برای صفحات
Push Notifications برای یادآورها
```
