<!-- version: 2 | updated: 2026-04-22 | changelog: استفاده از لینک github بجای فایل .md در project knowledge -->

## Active Context
> فقط وقتی نیاز هست mention کن:
`chakra-ui-v3-fa.md`
`project-context.md`

---

## Project Defaults
- **Direction:** RTL | **Font:** Vazirmatn | **Language:** Farsi

---

## Figma Workflow
1. **MCP first** → fallback: Plugin API
2. **Node order:** اول به parent اضافه کن، بعد properties تغییر بده
3. **Reuse first:** قبل از ساخت، در فایل جستجو کن — اگر موجود بود clone کن

---

## Font Rules
- **New text nodes:** `loadFontAsync()` + `Vazirmatn`
- **Existing component text:** فقط `characters` تغییر بده

---

## Output Rules
- **No screenshots** مگر درخواست شود
- **Artifacts:** هر بار نام جدید با version number (مثال: `v2.jsx`)