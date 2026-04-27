<!-- version: 1 | updated: 2026-04-22 | changelog: توضیحات -->

## Chakra UI Design System

# Chakra UI [v3] FA — Design System Context
# این فایل برای همه پروژه‌هایی که از Chakra UI استفاده می‌کنن مشترکه
# در Claude Code Desktop به عنوان یک Global Skill ذخیره کن

---

## معرفی
- Component Library: Chakra UI v3
- فونت پایه: Vazirmatn (open-source — جایگزین IRANSansX)
- زبان: فارسی / RTL
- همیشه `dir="rtl"` روی root المان

---

## Text Styles

| Style | Font | Size | Weight | Line Height |
|-------|------|------|--------|-------------|
| 2xs/font-normal | Vazirmatn | 10px | 400 | 14px |
| 2xs/font-medium | Vazirmatn | 10px | 500 | 14px |
| 2xs/font-semibold | Vazirmatn | 10px | 700 | 14px |
| 2xs/font-bold | Vazirmatn | 10px | 700 | 14px |
| xs/font-normal | Vazirmatn | 12px | 400 | 16px |
| xs/font-medium | Vazirmatn | 12px | 500 | 16px |
| xs/font-semibold | Vazirmatn | 12px | 700 | 16px |
| xs/font-bold | Vazirmatn | 12px | 700 | 16px |
| sm/font-normal | Vazirmatn | 14px | 400 | 20px |
| sm/font-medium | Vazirmatn | 14px | 700 | 20px |
| sm/font-semibold | Vazirmatn | 14px | 700 | 20px |
| sm/font-bold | Vazirmatn | 14px | 700 | 20px |
| md/font-normal | Vazirmatn | 16px | 400 | 24px |
| md/font-medium | Vazirmatn | 16px | 500 | 24px |
| md/font-semibold | Vazirmatn | 16px | 700 | 24px |
| md/font-bold | Vazirmatn | 16px | 700 | 24px |
| lg/font-normal | Vazirmatn | 18px | 400 | 28px |
| lg/font-medium | Vazirmatn | 18px | 500 | 28px |
| lg/font-semibold | Vazirmatn | 18px | 700 | 28px |
| lg/font-bold | Vazirmatn | 18px | 700 | 28px |
| xl/font-normal | Vazirmatn | 20px | 400 | 30px |
| xl/font-medium | Vazirmatn | 20px | 500 | 30px |
| xl/font-semibold | Vazirmatn | 20px | 700 | 30px |
| xl/font-bold | Vazirmatn | 20px | 700 | 30px |
| 2xl/font-normal | Vazirmatn | 24px | 400 | 32px |
| 2xl/font-medium | Vazirmatn | 24px | 500 | 32px |
| 2xl/font-semibold | Vazirmatn | 24px | 700 | 32px |
| 2xl/font-bold | Vazirmatn | 24px | 700 | 32px |
| 3xl/font-normal | Vazirmatn | 30px | 400 | 38px |
| 3xl/font-medium | Vazirmatn | 30px | 500 | 38px |
| 3xl/font-semibold | Vazirmatn | 30px | 700 | 38px |
| 3xl/font-bold | Vazirmatn | 30px | 700 | 38px |
| 4xl/font-normal | Vazirmatn | 36px | 400 | 44px |
| 4xl/font-medium | Vazirmatn | 36px | 500 | 44px |
| 4xl/font-semibold | Vazirmatn | 36px | 700 | 44px |
| 4xl/font-bold | Vazirmatn | 36px | 700 | 44px |
| 5xl/font-normal | Vazirmatn | 48px | 400 | 60px |
| 5xl/font-medium | Vazirmatn | 48px | 500 | 60px |
| 5xl/font-semibold | Vazirmatn | 48px | 700 | 60px |
| 5xl/font-bold | Vazirmatn | 48px | 700 | 60px |
| 6xl/font-normal | Vazirmatn | 60px | 400 | 72px |
| 6xl/font-medium | Vazirmatn | 60px | 500 | 72px |
| 6xl/font-semibold | Vazirmatn | 60px | 700 | 72px |
| 6xl/font-bold | Vazirmatn | 60px | 700 | 72px |
| 7xl/font-normal | Vazirmatn | 72px | 400 | 92px |
| 7xl/font-medium | Vazirmatn | 72px | 500 | 92px |
| 7xl/font-semibold | Vazirmatn | 72px | 700 | 92px |
| 7xl/font-bold | Vazirmatn | 72px | 700 | 92px |

---

## Shadows — Light Mode

| Token | CSS Value |
|-------|-----------|
| Shadows/light/xs | `box-shadow: 0px 1px 2px 0px rgba(24,24,27,0.1), 0px 0px 1px 0px rgba(24,24,27,0.2)` |
| Shadows/light/sm | `box-shadow: 0px 2px 4px 0px rgba(24,24,27,0.1), 0px 0px 1px 0px rgba(24,24,27,0.3)` |
| Shadows/light/md | `box-shadow: 0px 4px 8px 0px rgba(24,24,27,0.1), 0px 0px 1px 0px rgba(24,24,27,0.3)` |
| Shadows/light/lg | `box-shadow: 0px 8px 16px 0px rgba(24,24,27,0.1), 0px 0px 1px 0px rgba(24,24,27,0.3)` |
| Shadows/light/xl | `box-shadow: 0px 16px 24px 0px rgba(24,24,27,0.1), 0px 0px 1px 0px rgba(24,24,27,0.3)` |
| Shadows/light/2xl | `box-shadow: 0px 24px 40px 0px rgba(24,24,27,0.16), 0px 0px 1px 0px rgba(24,24,27,0.3)` |
| Shadows/light/inner | `box-shadow: inset 0px 2px 4px 0px rgba(0,0,0,0.05)` |

## Shadows — Dark Mode

| Token | CSS Value |
|-------|-----------|
| Shadows/dark/xs | `box-shadow: 0px 1px 1px 0px rgba(0,0,0,0.64), inset 0px 0px 1px 0px rgba(212,212,216,0.2)` |
| Shadows/dark/sm | `box-shadow: 0px 2px 4px 0px rgba(0,0,0,0.64), inset 0px 0px 1px 0px rgba(212,212,216,0.3)` |
| Shadows/dark/md | `box-shadow: 0px 4px 8px 0px rgba(0,0,0,0.64), inset 0px 0px 1px 0px rgba(212,212,216,0.3)` |
| Shadows/dark/lg | `box-shadow: 0px 8px 16px 0px rgba(24,24,27,0.1), inset 0px 0px 1px 0px rgba(212,212,216,0.3)` |
| Shadows/dark/xl | `box-shadow: 0px 16px 24px 0px rgba(0,0,0,0.64), inset 0px 0px 1px 0px rgba(212,212,216,0.3)` |
| Shadows/dark/2xl | `box-shadow: 0px 24px 40px 0px rgba(0,0,0,0.64), inset 0px 0px 1px 0px rgba(212,212,216,0.3)` |

## Focus Ring

| Token | CSS Value |
|-------|-----------|
| FocusRing/teal | `box-shadow: 0px 0px 0px 4px #2dd4bf, 0px 0px 0px 2px #ffffff` |
| FocusRing/blue | `box-shadow: 0px 0px 0px 4px #60a5fa, 0px 0px 0px 2px #ffffff` |
| FocusRing/purple | `box-shadow: 0px 0px 0px 4px #c084fc, 0px 0px 0px 2px #ffffff` |
| FocusRing/pink | `box-shadow: 0px 0px 0px 4px #f472b6, 0px 0px 0px 2px #ffffff` |
| FocusRing/orange | `box-shadow: 0px 0px 0px 4px #fb923c, 0px 0px 0px 2px #ffffff` |
| FocusRing/yellow | `box-shadow: 0px 0px 0px 4px #facc15, 0px 0px 0px 2px #ffffff` |

---

## Color Tokens — Light Mode

### bg
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `bg/default` | `#FFFFFF` | whiteAlpha/0 |
| `bg/subtle` | `#FAFAFA` | gray/50 |
| `bg/muted` | `#F4F4F5` | gray/100 |
| `bg/emphasized` | `#E4E4E7` | gray/200 |
| `bg/inverted` | `#000000` | blackAlpha/0 |
| `bg/panel` | `#FFFFFF` | whiteAlpha/0 |
| `bg/error` | `#FEF2F2` | red/50 |
| `bg/warning` | `#FFF7ED` | orange/50 |
| `bg/success` | `#F0FDF4` | green/50 |
| `bg/info` | `#EFF6FF` | blue/50 |
| `bg/teal` | `#F0FDFA` | teal/50 |

### fg
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `fg/default` | `#000000` | blackAlpha/0 |
| `fg/subtle` | `#A1A1AA` | gray/400 |
| `fg/muted` | `#52525B` | gray/600 |
| `fg/inverted` | `#FAFAFA` | gray/50 |
| `fg/error` | `#EF4444` | red/500 |
| `fg/warning` | `#EA580C` | orange/600 |
| `fg/success` | `#16A34A` | green/600 |
| `fg/info` | `#2563EB` | blue/600 |

### border
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `border/default` | `#E4E4E7` | gray/200 |
| `border/subtle` | `#FAFAFA` | gray/50 |
| `border/muted` | `#F4F4F5` | gray/100 |
| `border/emphasized` | `#D4D4D8` | gray/300 |
| `border/inverted` | `#27272A` | gray/800 |
| `border/error` | `#EF4444` | red/500 |
| `border/warning` | `#F97316` | orange/500 |
| `border/success` | `#22C55E` | green/500 |
| `border/info` | `#3B82F6` | blue/500 |

### text
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `text/fg` | `#000000` | blackAlpha/0 |
| `text/fg_muted` | `#52525B` | gray/600 |
| `text/fg_subtle` | `#A1A1AA` | gray/400 |
| `text/fg_inverted` | `#FAFAFA` | gray/50 |
| `text/fg_error` | `#EF4444` | red/500 |
| `text/fg_warning` | `#CA8A04` | yellow/600 |
| `text/fg_success` | `#16A34A` | green/600 |
| `text/fg_info` | `#2563EB` | blue/600 |

### gray
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `gray/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `gray/fg` | `#27272A` | gray/800 |
| `gray/subtle` | `#F4F4F5` | gray/100 |
| `gray/muted` | `#E4E4E7` | gray/200 |
| `gray/emphasized` | `#D4D4D8` | gray/300 |
| `gray/solid` | `#18181B` | gray/900 |
| `gray/focusRing` | `#A1A1AA` | gray/400 |

### teal
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `teal/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `teal/fg` | `#0C5D56` | teal/700 |
| `teal/subtle` | `#CCFBF1` | teal/100 |
| `teal/muted` | `#99F6E4` | teal/200 |
| `teal/emphasized` | `#5EEAD4` | teal/300 |
| `teal/solid` | `#0D9488` | teal/600 |
| `teal/focusRing` | `#2DD4BF` | teal/400 |

### blue
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `blue/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `blue/fg` | `#173DA6` | blue/700 |
| `blue/subtle` | `#DBEAFE` | blue/100 |
| `blue/muted` | `#BFDBFE` | blue/200 |
| `blue/emphasized` | `#A3CFFF` | blue/300 |
| `blue/solid` | `#2563EB` | blue/600 |
| `blue/focusRing` | `#60A5FA` | blue/400 |

### red
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `red/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `red/fg` | `#991919` | red/700 |
| `red/subtle` | `#FEE2E2` | red/100 |
| `red/muted` | `#FECACA` | red/200 |
| `red/emphasized` | `#FCA5A5` | red/300 |
| `red/solid` | `#DC2626` | red/600 |
| `red/focusRing` | `#F87171` | red/400 |

### green
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `green/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `green/fg` | `#116932` | green/700 |
| `green/subtle` | `#DCFCE7` | green/100 |
| `green/muted` | `#BBF7D0` | green/200 |
| `green/emphasized` | `#86EFAC` | green/300 |
| `green/solid` | `#16A34A` | green/600 |
| `green/focusRing` | `#4ADE80` | green/400 |

### orange
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `orange/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `orange/fg` | `#92310A` | orange/700 |
| `orange/subtle` | `#FFEDD5` | orange/100 |
| `orange/muted` | `#FED7AA` | orange/200 |
| `orange/emphasized` | `#FDBA74` | orange/300 |
| `orange/solid` | `#EA580C` | orange/600 |
| `orange/focusRing` | `#FB923C` | orange/400 |

### purple
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `purple/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `purple/fg` | `#641BA3` | purple/700 |
| `purple/subtle` | `#F3E8FF` | purple/100 |
| `purple/muted` | `#E9D5FF` | purple/200 |
| `purple/emphasized` | `#D8B4FE` | purple/300 |
| `purple/solid` | `#9333EA` | purple/600 |
| `purple/focusRing` | `#C084FC` | purple/400 |

### pink
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `pink/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `pink/fg` | `#A41752` | pink/700 |
| `pink/subtle` | `#FCE7F3` | pink/100 |
| `pink/muted` | `#FBCFE8` | pink/200 |
| `pink/emphasized` | `#F9A8D4` | pink/300 |
| `pink/solid` | `#DB2777` | pink/600 |
| `pink/focusRing` | `#F472B6` | pink/400 |

### cyan
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `cyan/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `cyan/fg` | `#0C5C72` | cyan/700 |
| `cyan/subtle` | `#CFFAFE` | cyan/100 |
| `cyan/muted` | `#A5F3FC` | cyan/200 |
| `cyan/emphasized` | `#67E8F9` | cyan/300 |
| `cyan/solid` | `#0891B2` | cyan/600 |
| `cyan/focusRing` | `#22D3EE` | cyan/400 |

### yellow
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `yellow/contrast` | `#000000` | blackAlpha/0 |
| `yellow/fg` | `#713F12` | yellow/800 |
| `yellow/subtle` | `#FEF9C3` | yellow/100 |
| `yellow/muted` | `#FEF08A` | yellow/200 |
| `yellow/emphasized` | `#FDE047` | yellow/300 |
| `yellow/solid` | `#FDE047` | yellow/300 |
| `yellow/focusRing` | `#FACC15` | yellow/400 |

---

## Color Tokens — Dark Mode

### bg
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `bg/default` | `#000000` | blackAlpha/0 |
| `bg/subtle` | `#111111` | gray/950 |
| `bg/muted` | `#18181B` | gray/900 |
| `bg/emphasized` | `#27272A` | gray/800 |
| `bg/inverted` | `#FFFFFF` | whiteAlpha/0 |
| `bg/panel` | `#111111` | gray/950 |
| `bg/error` | `#1F0808` | red/950 |
| `bg/warning` | `#220A04` | orange/950 |
| `bg/success` | `#03190C` | green/950 |
| `bg/info` | `#0C142E` | blue/950 |
| `bg/teal` | `#021716` | teal/950 |

### fg
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `fg/default` | `#FAFAFA` | gray/50 |
| `fg/subtle` | `#71717A` | gray/500 |
| `fg/muted` | `#71717A` | gray/500 |
| `fg/inverted` | `#000000` | blackAlpha/0 |
| `fg/error` | `#F87171` | red/400 |
| `fg/warning` | `#FDBA74` | orange/300 |
| `fg/success` | `#86EFAC` | green/300 |
| `fg/info` | `#A3CFFF` | blue/300 |

### border
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `border/default` | `#27272A` | gray/800 |
| `border/subtle` | `#111111` | gray/950 |
| `border/muted` | `#18181B` | gray/900 |
| `border/emphasized` | `#3F3F46` | gray/700 |
| `border/inverted` | `#E4E4E7` | gray/200 |
| `border/error` | `#F87171` | red/400 |
| `border/warning` | `#FB923C` | orange/400 |
| `border/success` | `#4ADE80` | green/400 |
| `border/info` | `#60A5FA` | blue/400 |

### text
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `text/fg` | `#FAFAFA` | gray/50 |
| `text/fg_muted` | `#A1A1AA` | gray/400 |
| `text/fg_subtle` | `#71717A` | gray/500 |
| `text/fg_inverted` | `#000000` | blackAlpha/0 |
| `text/fg_error` | `#F87171` | red/400 |
| `text/fg_warning` | `#FDE047` | yellow/300 |
| `text/fg_success` | `#86EFAC` | green/300 |
| `text/fg_info` | `#A3CFFF` | blue/300 |

### gray
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `gray/contrast` | `#000000` | blackAlpha/0 |
| `gray/fg` | `#E4E4E7` | gray/200 |
| `gray/subtle` | `#18181B` | gray/900 |
| `gray/muted` | `#27272A` | gray/800 |
| `gray/emphasized` | `#3F3F46` | gray/700 |
| `gray/solid` | `#FFFFFF` | whiteAlpha/0 |
| `gray/focusRing` | `#A1A1AA` | gray/400 |

### teal
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `teal/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `teal/fg` | `#5EEAD4` | teal/300 |
| `teal/subtle` | `#032726` | teal/900 |
| `teal/muted` | `#114240` | teal/800 |
| `teal/emphasized` | `#0C5D56` | teal/700 |
| `teal/solid` | `#0D9488` | teal/600 |
| `teal/focusRing` | `#2DD4BF` | teal/400 |

### blue
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `blue/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `blue/fg` | `#A3CFFF` | blue/300 |
| `blue/subtle` | `#14204A` | blue/900 |
| `blue/muted` | `#1A3478` | blue/800 |
| `blue/emphasized` | `#173DA6` | blue/700 |
| `blue/solid` | `#2563EB` | blue/600 |
| `blue/focusRing` | `#60A5FA` | blue/400 |

### red
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `red/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `red/fg` | `#FCA5A5` | red/300 |
| `red/subtle` | `#300C0C` | red/900 |
| `red/muted` | `#511111` | red/800 |
| `red/emphasized` | `#991919` | red/700 |
| `red/solid` | `#DC2626` | red/600 |
| `red/focusRing` | `#F87171` | red/400 |

### green
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `green/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `green/fg` | `#86EFAC` | green/300 |
| `green/subtle` | `#042713` | green/900 |
| `green/muted` | `#124A28` | green/800 |
| `green/emphasized` | `#116932` | green/700 |
| `green/solid` | `#16A34A` | green/600 |
| `green/focusRing` | `#4ADE80` | green/400 |

### orange
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `orange/contrast` | `#000000` | blackAlpha/0 |
| `orange/fg` | `#FDBA74` | orange/300 |
| `orange/subtle` | `#3B1106` | orange/900 |
| `orange/muted` | `#6C2710` | orange/800 |
| `orange/emphasized` | `#92310A` | orange/700 |
| `orange/solid` | `#EAB308` | yellow/500 |
| `orange/focusRing` | `#FB923C` | orange/400 |

### purple
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `purple/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `purple/fg` | `#D8B4FE` | purple/300 |
| `purple/subtle` | `#2F0553` | purple/900 |
| `purple/muted` | `#4A1772` | purple/800 |
| `purple/emphasized` | `#641BA3` | purple/700 |
| `purple/solid` | `#9333EA` | purple/600 |
| `purple/focusRing` | `#C084FC` | purple/400 |

### pink
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `pink/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `pink/fg` | `#F9A8D4` | pink/300 |
| `pink/subtle` | `#45061F` | pink/900 |
| `pink/muted` | `#6D0E34` | pink/800 |
| `pink/emphasized` | `#A41752` | pink/700 |
| `pink/solid` | `#DB2777` | pink/600 |
| `pink/focusRing` | `#F472B6` | pink/400 |

### cyan
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `cyan/contrast` | `#FFFFFF` | whiteAlpha/0 |
| `cyan/fg` | `#67E8F9` | cyan/300 |
| `cyan/subtle` | `#072A38` | cyan/900 |
| `cyan/muted` | `#134152` | cyan/800 |
| `cyan/emphasized` | `#0C5C72` | cyan/700 |
| `cyan/solid` | `#0891B2` | cyan/600 |
| `cyan/focusRing` | `#22D3EE` | cyan/400 |

### yellow
| Token | Hex | Global Alias |
|-------|-----|--------------|
| `yellow/contrast` | `#000000` | blackAlpha/0 |
| `yellow/fg` | `#FDE047` | yellow/300 |
| `yellow/subtle` | `#422006` | yellow/900 |
| `yellow/muted` | `#713F12` | yellow/800 |
| `yellow/emphasized` | `#845209` | yellow/700 |
| `yellow/solid` | `#FDE047` | yellow/300 |
| `yellow/focusRing` | `#FACC15` | yellow/400 |

---

## Spacing Tokens
| Token | px |
|-------|----|
| 0_5 | 2px |
| 1 | 4px |
| 1_5 | 6px |
| 2 | 8px |
| 2_5 | 10px |
| 3 | 12px |
| 3_5 | 14px |
| 4 | 16px |
| 4_5 | 18px |
| 5 | 20px |
| 6 | 24px |
| 7 | 28px |
| 8 | 32px |
| 9 | 36px |
| 10 | 40px |
| 11 | 44px |
| 12 | 48px |
| 14 | 56px |
| 16 | 64px |
| 20 | 80px |
| 24 | 96px |

---

## Border Radius
| Token | px | کاربرد |
|-------|----|--------|
| Radii/Semantic/l1 | 2px | خیلی کوچک |
| Radii/Semantic/l2 | 4px | input، button، badge |
| Radii/Semantic/l3 | 6px | dialog، card، panel |
| Radii/lg | 8px | modal، drawer |
| Radii/xl | 12px | بزرگ |
| Radii/full | 9999px | pill، avatar |

---

## Borders
| Token | px |
|-------|----|
| Borders/xs | 0.5px |
| Borders/sm | 1px |
| Borders/md | 2px |

---

## Component Heights
| کامپوننت | ارتفاع |
|----------|--------|
| Input / Button / Select (size md) | 40px |
| Input / Button (size sm) | 32px |
| Input / Button (size lg) | 48px |
| Icon Button | 40×40px |

---

## قوانین کلی
1. همیشه RTL — `dir="rtl"` روی root
2. فونت Vazirmatn برای همه چیز (open-source، قابل loadFontAsync)
3. از Chakra UI v3 components استفاده کن
4. از token ها نه مقادیر hard-coded
5. از text styles آماده استفاده کن (sm/font-normal و غیره)
6. shadow برای dialog: Shadows/light/lg
7. shadow برای card: Shadows/light/sm
8. رنگ primary: teal/solid = #0D9488
