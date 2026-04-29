---
title: "DESIGN.md — Vitrina"
generated: "2026-04-21"
generator: "DesignOps Tools: DesignBridge v2.0"
source_file: "Vitrina"
purpose: "AI-ready design system specification"
---

# DESIGN.md — Vitrina

> **AI AGENT INSTRUCTIONS — READ FIRST, APPLY TO ALL OUTPUT**
>
> This file is the complete visual specification for **"Vitrina"**.
> Apply every rule below to every line of UI, HTML, CSS, JSX, or component code you generate.
>
> 1. **Colours** — Use only exact hex values or `var(--token)` names from this file. No substitutions.
> 2. **Typography** — Match font family, weight, size, line-height exactly.
> 3. **Spacing** — Use only values from the spacing/sizing token tables.
> 4. **Border radius** — Use only the defined radius tokens.
> 5. **Components** — Mirror defined structures. Honour variant property names exactly.
> 6. **Shadows** — Apply defined elevation styles. Do not invent shadows.
> 7. **Unknowns** — If a visual decision is not defined here, ask before inventing it.

## How to Use

| Platform | Instructions |
|----------|-------------|
| **Google Stitch** | Upload via *Design System → DESIGN.md* |
| **Claude Code** | Place in project root, reference as `@DESIGN.md` |
| **Cursor / Windsurf** | Add to context, prompt: *"Follow @DESIGN.md for all visual decisions"* |
| **Antigravity** | Import via *Design System settings* |
| **OpenAI Codex** | Paste as system context before UI tasks |
| **Any LLM** | Paste at top of session as system context |

```
You have the design system for "Vitrina" in DESIGN.md. Follow it precisely for ALL visual decisions. No deviations.
```

## Design System Summary

- **Source**: Vitrina · Generated: 2026-04-21
- **Generator**: DesignOps Tools: DesignBridge — [designops.tools](https://designops.tools)
- **Spacing / size tokens**: 6
- **Component sets**: 49
- **Standalone components**: 6

## Spacing Tokens

> Apply these values for all margins, padding, and gaps.

### Screen

| Token | Value |
|-------|-------|
| `Size/Navbar` | `512px` |
| `Size/Main` | `512px` |
| `Content Column/Start` | `0px` |
| `Content Column/Middle` | `512px` |
| `Content Column/End` | `0px` |
| `Size/Screen` | `1920px` |

## String Tokens

### Tokens

- `Products/Currency/Currency`: `تومانء`

## Components

> Replicate structures exactly. Honour variant property names for interactive states.

### Variant Sets

#### btnScreenSize
- **Total variants**: 2
- **Frame size**: 64 × 112px
- **Variant properties**:
  - `Type: maximize | minimize`
- **Sample variant names**: `Type=maximize` · `Type=minimize`

#### Navbar
- **Total variants**: 2
- **Frame size**: 1952 × 176px
- **Variant properties**:
  - `Role: Seller`
  - `Type: Website | Dashboard`
- **Sample variant names**: `Role=Seller, Type=Dashboard` · `Role=Seller, Type=Website`

#### Title-Bar
- **Total variants**: 3
- **Frame size**: 992 × 242px
- **Variant properties**:
  - `Size: xl-20 | lg-18 | md-16`
- **Sample variant names**: `Size=xl-20` · `Size=lg-18` · `Size=md-16`

#### Sidebar-Item
- **Total variants**: 4
- **Frame size**: 256 × 208px
- **Variant properties**:
  - `Selected: false | true`
  - `State: Default | Hover | Disabled`
- **Sample variant names**: `Selected=false, State=Default` · `Selected=false, State=Hover` · `Selected=false, State=Disabled` · `Selected=true, State=Default`

#### Sidebar-Item/Dashboard
- **Total variants**: 2
- **Frame size**: 256 × 232px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Products
- **Total variants**: 2
- **Frame size**: 256 × 232px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Orders
- **Total variants**: 2
- **Frame size**: 256 × 196px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Financial
- **Total variants**: 2
- **Frame size**: 256 × 232px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Financial
- **Total variants**: 2
- **Frame size**: 256 × 196px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Customers
- **Total variants**: 2
- **Frame size**: 256 × 304px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Theme
- **Total variants**: 2
- **Frame size**: 256 × 196px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Setting
- **Total variants**: 2
- **Frame size**: 256 × 268px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Sidebar-Item/Setting
- **Total variants**: 2
- **Frame size**: 256 × 196px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### SubLine
- **Total variants**: 2
- **Frame size**: 90 × 54px
- **Variant properties**:
  - `State: Default | Hover/Select`
- **Sample variant names**: `State=Default` · `State=Hover/Select`

#### Page-Header
- **Total variants**: 3
- **Frame size**: 1024 × 232px
- **Variant properties**:
  - `Size: 2xl-24 | xl-20 | l-18`
- **Sample variant names**: `Size=2xl-24` · `Size=xl-20` · `Size=l-18`

#### Invitation-Code
- **Total variants**: 2
- **Frame size**: 592 × 136px
- **Variant properties**:
  - `Property: Default | Variant2`
- **Sample variant names**: `Property =Default` · `Property =Variant2`

#### Signup-Accordion
- **Total variants**: 6
- **Frame size**: 1286 × 324px
- **Variant properties**:
  - `State: Default | Hover | Open`
  - `Selected: false | true`
- **Sample variant names**: `State=Default, Selected=false` · `State=Open, Selected=false` · `State=Open, Selected=true` · `State=Hover, Selected=false` · `State=Hover, Selected=true` · `State=Default, Selected=true`

#### Category-Mng Accordion
- **Total variants**: 6
- **Frame size**: 1276 × 558px
- **Variant properties**:
  - `State: Default | Hover | Open`
  - `Sub category: Yes | No`
- **Sample variant names**: `State=Default, Sub category=No` · `State=Default, Sub category=Yes` · `State=Hover, Sub category=No` · `State=Hover, Sub category=Yes` · `State=Open, Sub category=No` · `State=Open, Sub category=Yes`

#### SubCategory-Item
- **Total variants**: 2
- **Frame size**: 600 × 144px
- **Variant properties**:
  - `State: Default | Hover`
- **Sample variant names**: `State=Default` · `State=Hover`

#### Product-Status
- **Total variants**: 4
- **Frame size**: 100 × 172px
- **Variant properties**:
  - `Status: Published | Draft | Inactive | Archived`
- **Sample variant names**: `Status=Published` · `Status=Draft` · `Status=Inactive` · `Status=Archived`

#### Product-Amount
- **Total variants**: 3
- **Frame size**: 86 × 134px
- **Variant properties**:
  - `Type: Number | Not Available | Infinity`
- **Sample variant names**: `Type=Infinity` · `Type=Not Available` · `Type=Number`

#### Product-Card
- **Total variants**: 3
- **Frame size**: 1066 × 361px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Selected`

#### Thumbnail
- **Total variants**: 4
- **Frame size**: 293 × 257px
- **Variant properties**:
  - `State: Default | Hover | State3 | State4`
  - `Default: true | false`
- **Sample variant names**: `State=Default, Default=false` · `State=State4, Default=true` · `State=Hover, Default=false` · `State=State3, Default=true`

#### Currency-Switch
- **Total variants**: 2
- **Frame size**: 341 × 175px
- **Variant properties**:
  - `Type: Toman | Dollar`
- **Sample variant names**: `Type=Toman` · `Type=Dollar`

#### UploadedImage-Card
- **Total variants**: 4
- **Frame size**: 342 × 632px
- **Variant properties**:
  - `State: Default | Hover`
  - `isDefault: true | false`
- **Sample variant names**: `State=Default, isDefault=false` · `State=Default, isDefault=true` · `State=Hover, isDefault=false` · `State=Hover, isDefault=true`

#### Product-TelSale
- **Total variants**: 2
- **Frame size**: 992 × 558px
- **Variant properties**:
  - `Enabled: False | true`
- **Sample variant names**: `Enabled=False` · `Enabled=true`

#### Variant-Accordion
- **Total variants**: 2
- **Frame size**: 992 × 298px
- **Variant properties**:
  - `Open: false | true`
- **Sample variant names**: `Open=false` · `Open=true`

#### Shipping-Local
- **Total variants**: 2
- **Frame size**: 992 × 457px
- **Variant properties**:
  - `State: inactive | active`
- **Sample variant names**: `State=inactive` · `State=active`

#### Shipping-OutRange
- **Total variants**: 3
- **Frame size**: 992 × 1392px
- **Variant properties**:
  - `State: inactive | active empty | active fill`
- **Sample variant names**: `State=inactive` · `State=active empty` · `State=active fill`

#### Shipping-Card Custom
- **Total variants**: 3
- **Frame size**: 504 × 712px
- **Variant properties**:
  - `State: Default | Disabled | Hover`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Disabled`

#### Shipping-Card System
- **Total variants**: 4
- **Frame size**: 504 × 696px
- **Variant properties**:
  - `State: Default | Hover | Disabled | Comming Soon`
- **Sample variant names**: `State=Default` · `State=Comming Soon` · `State=Hover` · `State=Disabled`

#### Shipping-Method
- **Total variants**: 3
- **Frame size**: 109 × 124px
- **Variant properties**:
  - `Type: Free | Const | Weight Based`
- **Sample variant names**: `Type=Free` · `Type=Const` · `Type=Weight Based`

#### Phone-Card
- **Total variants**: 2
- **Frame size**: 504 × 216px
- **Variant properties**:
  - `State: Default | Hover`
- **Sample variant names**: `State=Default` · `State=Hover`

#### Social-Card
- **Total variants**: 2
- **Frame size**: 504 × 216px
- **Variant properties**:
  - `State: Default | Hover`
- **Sample variant names**: `State=Default` · `State=Hover`

#### Address-Card
- **Total variants**: 3
- **Frame size**: 504 × 1024px
- **Variant properties**:
  - `State: Default | Hover | Disabled`
- **Sample variant names**: `State=Default` · `State=Disabled` · `State=Hover`

#### Category-Accordion
- **Total variants**: 6
- **Frame size**: 1340 × 432px
- **Variant properties**:
  - `State: Default | Hover | Open`
  - `Selected: false | true`
- **Sample variant names**: `State=Default, Selected=false` · `State=Open, Selected=false` · `State=Open, Selected=true` · `State=Hover, Selected=false` · `State=Hover, Selected=true` · `State=Default, Selected=true`

#### Theme-Card
- **Total variants**: 5
- **Frame size**: 734 × 935px
- **Variant properties**:
  - `isSelected: false | true`
  - `State: Default | Hover | Coming Soon`
- **Sample variant names**: `isSelected=false, State=Default` · `isSelected=false, State=Hover` · `isSelected=true, State=Hover` · `isSelected=true, State=Default` · `isSelected=false, State=Coming Soon`

#### SlideMenu-Item
- **Total variants**: 3
- **Frame size**: 256 × 208px
- **Variant properties**:
  - `Selected: false | true`
  - `State: Default | Hover`
- **Sample variant names**: `Selected=false, State=Default` · `Selected=false, State=Hover` · `Selected=true, State=Default`

#### Color
- **Total variants**: 3
- **Frame size**: 134 × 310px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Selected` · `State=Hover`

#### Setting-Card
- **Total variants**: 3
- **Frame size**: 537 × 476px
- **Variant properties**:
  - `State: Default | Hover | Disabled`
- **Sample variant names**: `State=Default` · `State=Disabled` · `State=Hover`

#### File-Upload
- **Total variants**: 2
- **Frame size**: 432 × 344px
- **Variant properties**:
  - `Property 1: FileUpload | Uploaded-File`
- **Sample variant names**: `Property 1=FileUpload` · `Property 1=Uploaded-File`

#### 2Factor-Card
- **Total variants**: 3
- **Frame size**: 617 × 312px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Selected`

#### Prd/Status
- **Total variants**: 6
- **Frame size**: 124 × 252px
- **Variant properties**:
  - `Status: Waiting | Paid | Payment | Sent | Returned | Canceled`
- **Sample variant names**: `Status=Waiting` · `Status=Paid` · `Status=Payment` · `Status=Sent` · `Status=Returned` · `Status=Canceled`

#### Split Menu
- **Total variants**: 6
- **Frame size**: 980 × 68px
- **Variant properties**:
  - `State: Pending | Canceled | Processing | Returned | Paid | Sent`
  - `Open: false`
- **Sample variant names**: `State=Canceled, Open=false` · `State=Returned, Open=false` · `State=Sent, Open=false` · `State=Processing, Open=false` · `State=Paid, Open=false` · `State=Pending, Open=false`

#### Manual-Customer
- **Total variants**: 3
- **Frame size**: 432 × 300px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Selected`

#### Manual-Product
- **Total variants**: 3
- **Frame size**: 544 × 316px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Selected`

#### Manual-Discount
- **Total variants**: 3
- **Frame size**: 432 × 342px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Selected`

#### Manual-Shipping
- **Total variants**: 3
- **Frame size**: 400 × 424px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Selected`

#### Sender-Card
- **Total variants**: 3
- **Frame size**: 432 × 288px
- **Variant properties**:
  - `State: Default | Hover | Selected`
- **Sample variant names**: `State=Default` · `State=Hover` · `State=Selected`

### Standalone Components

#### Card-Adv
- **Size**: 224 × 136px

#### ‌Button-Footer
- **Size**: 960 × 56px

#### Sidebar
- **Size**: 256 × 1016px

#### SubCategory-Item
- **Size**: 94 × 32px

#### CommingSoon / Tag
- **Size**: 117 × 40px

#### Shipping-Price Item
- **Size**: 197 × 36px

## Design Rules — Mandatory for AI Agents

| Category | Rule |
|----------|------|
| Colours | Use only tokens defined above. Always output as `var(--token)`. Never hard-code. |
| Typography | Match family, weight, size, line-height exactly from the table above. |
| Spacing | Use only spacing token values. No arbitrary numbers. |
| Radius | Use only border-radius tokens. No arbitrary values. |
| Shadows | Use only defined elevation/effect styles. |
| Components | Replicate structures. Honour variant property names. |
| HTML | Output semantic HTML5 with ARIA roles. All components responsive by default. |
| Unknowns | If a decision is not defined here: ask the user, do not invent. |

## CSS Custom Properties

```css
:root {

  /* ── Spacing ────────────────────────── */
  --size-navbar: 512px;
  --size-main: 512px;
  --content-column-start: 0px;
  --content-column-middle: 512px;
  --content-column-end: 0px;
  --size-screen: 1920px;
}
```

## Tailwind Configuration

```javascript
// tailwind.config.js
module.exports = { theme: { extend: {

  spacing: {
    'size-navbar': '512px',
    'size-main': '512px',
    'content-column-start': '0px',
    'content-column-middle': '512px',
    'content-column-end': '0px',
    'size-screen': '1920px',
  },
}}};
```

---

*Generated on 2026-04-21 by **DesignOps Tools: DesignBridge v2.0** from "Vitrina".*
*[designops.tools](https://designops.tools) — Bridge your Figma design system to any AI tool.*