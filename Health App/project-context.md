# project-context | v1 | 2026-04-29

# Health & Wellness App — Project Context

## معرفی پروژه

یک اپلیکیشن هوشمند در حوزه بهداشت و سلامت که به‌عنوان **دستیار شخصی AI** عمل می‌کند. هدف اصلی کمک به کاربران برای بهبود کیفیت زندگی از طریق راهنمایی‌های شخصی‌سازی‌شده است.

- **پلتفرم**: PWA (در آینده: Native App)
- **زبان هدف**: فارسی (RTL)
- **مخاطب**: تمام سنین

---

## Tech Stack

| لایه | تکنولوژی |
|------|-----------|
| Frontend | React + TypeScript |
| UI Library | Chakra UI v3 (RTL + Vazirmatn) |
| AI Engine | Anthropic Claude API (`claude-sonnet-4-20250514`) |
| Platform | PWA → Native |

---

## Design System

| ویژگی | مقدار |
|-------|-------|
| رنگ اصلی | `#0D9488` (Teal) |
| پس‌زمینه | `#FFFFFF` / `#F0FDFA` |
| متن اصلی | `#0F172A` |
| متن فرعی | `#64748B` |
| خطا | `#DC2626` |
| موفقیت | `#16A34A` |
| فونت | Vazirmatn |
| جهت | RTL |
| مود | Light (پیش‌فرض) + Dark آماده |

---

## ماژول‌های اصلی

### 1. 🎭 Daily Mood Tracking
- Emotion Check-ins
- Mood Patterns Analysis
- Trigger Identification — AI می‌پرسد چه چیزی باعث این احساس شد
- Progress Visualization

### 2. 💬 Conversational Interface (AI Chat)
- Voice Interaction
- Video Interaction
- Text Chat Option
- Natural Language Processing
- Personalized Questions

### 3. 🤖 AI Feedback System
- Voice Tone Analysis
- Facial Expression Recognition
- Sentiment Detection
- Behavioral Insights

### 4. 🏋️ Virtual Exercise Coach
- Personalized Workouts
- Form Correction
- Progress Tracking
- Adaptive Difficulty

### 5. 👤 User Profile
- Personal Info
- Notifications
- Partnership

### 6. 📱 Smart Device Integration
- Heart Rate Monitoring *(Native)*
- Sleep Quality Data *(Native)*
- Step Counter *(Native)*
- Blood Pressure *(Native)*
- Muscle Mass *(Partner)*
- Body Fat *(Partner)*
- Calorie Tracking *(Partner)*

### 7. 🧠 Mental Health Support
- AI Feedback
- Stress Management Tips
- Meditation Guides
- Breathing Exercises
- Therapy Resources

### 8. 🥗 Nutrition Guidance
- Meal Suggestions
- Hydration Reminders
- Caloric Intake *(Partner)*
- Dietary Preferences
- Suggestion Based on Data

### 9. 📊 Health Reports
- Medical File (EHR)
- Goal Achievement (مثل: کاهش وزن)
- Recommendations
- Physical Prediction
- Doctor Sharing Option

---

## صفحات (Screens)

| # | صفحه | اولویت |
|---|------|--------|
| 1 | Onboarding | 🔴 بالا |
| 2 | Home / Dashboard | 🔴 بالا |
| 3 | AI Chat | 🔴 بالا |
| 4 | Mood Check-in | 🔴 بالا |
| 5 | Exercise | 🟡 متوسط |
| 6 | Nutrition | 🟡 متوسط |
| 7 | Mental Health | 🟡 متوسط |
| 8 | Health Reports | 🟡 متوسط |
| 9 | Device Integration | 🟠 پایین |
| 10 | Profile & Settings | 🟠 پایین |

---

## نکات Partner Features

فیچرهایی با برچسب **(Partner)** از طریق شریک تجاری ارائه می‌شوند. در طراحی با badge یا آیکون متمایز نشان داده شوند.
