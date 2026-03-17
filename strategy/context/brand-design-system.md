---
brand: Embark
version: 1.4
sources:
  - "Brand Guidelines V1.4 (Dec 2023) PDF"
  - "embarkwithus.com live CSS audit (Mar 2026)"
  - "Figma: Embark UI - Resource HP (jSY3ooey3A79x0n81Htoor) MCP extraction"
updated: 2026-03-06
---

# Embark Brand Design System

## Personality

Seriously Happy: professional confidence meets warm optimism. Fun socks with a suit.

Design principles: Happy, Intentional, Bright & bold, Fun socks.
Lead with white space. Bright color as punctuation not wallpaper. Never silly, never corporate-cold.

## Colors

```yaml
brand:
  ink:        { hex: "#000000", use: "logo, headlines, never as background" }
  paper:      { hex: "#FFFFFF", use: "primary background, maximize" }
  bubblegum:  { hex: "#F277C6", use: "floating CTAs, ghost hover accent" }
  sky:        { hex: "#5BC2E7", use: "accent" }
  cherry:     { hex: "#F9423A", use: "accent" }
  spring:     { hex: "#00B74F", use: "accent" }
  sunny:      { hex: "#FEDD00", use: "accent, section backgrounds" }
  fire:       { hex: "#FF8200", use: "accent, floating side CTA" }
  electric:   { hex: "#027FF1", use: "modal/logo-bar backgrounds, NOT buttons" }

functional:
  nav-blue:       { hex: "#0074DD", use: "PRIMARY CTA, nav bar, links, buttons" }
  text-default:   { hex: "#2F3031", use: "body text (not pure black)" }
  text-inverse:   { hex: "#FFFFFF", use: "text on dark backgrounds" }
  text-muted:     { hex: "#8F857B", use: "secondary/caption text" }
  stroke:         { hex: "#BFB6AD", use: "dividers, separators" }
  border-subdued: { hex: "#C9CBCF", use: "subdued borders" }
  border-disabled:{ hex: "#D9DBDD", use: "disabled borders" }
  error-100:      { hex: "#FFCDD2", use: "error background" }

limited:
  sand:   { hex: "#EDE8E3", use: "alternate bg vs white" }
  plum:   { hex: "#6C1D45", use: "illustration accents only" }
  sea:    { hex: "#0047BB", use: "illustration accents, primary btn hover" }
  forest: { hex: "#00573F", use: "illustration accents only" }
  navy:   { hex: "#141B4D", use: "illustration accents only" }

gray:
  g300: "#E0E0E0"
  g600: "#757575"
  g900: "#212121"

hover:
  primary-btn:  "#0047BB"  # sea, darker than nav-blue
  ghost-btn:    "#F277C6"  # bubblegum underline
  secondary-btn: "#0074DD" # fills with nav-blue

overlays: [
  "rgba(0,0,0,0.08)", "rgba(0,0,0,0.25)", "rgba(0,0,0,0.4)",
  "rgba(0,0,0,0.6)", "rgba(0,0,0,0.85)",
  "rgba(255,255,255,0.2-0.7)", "rgba(237,232,227,0.3-0.63)"
]
```

Color rules: use 1-3 bright colors per layout, never all seven. Paper ~20%, Ink ~20%, each bright ~8% max, Sand ~10%. Never pair Cherry+Spring. All digital pairings must meet WCAG AA. Safe body text: Ink on Paper/Sand/Sunny, Paper on NavBlue/Cherry/Spring.

## Typography

```yaml
fonts:
  headline: "'Embark Sans Headline', sans-serif"  # display, H1-H4
  body:     "'Embark Sans', sans-serif"            # body, subtitles, buttons, nav, eyebrows
  fallback: "'DM Sans', sans-serif"                # prototype substitute (bespoke font not public)

# format: [size, line-height, weight]
desktop:
  display:
    D1: [190px, 1, 500, headline]
    D2: [75px, 1, 500, headline]
  headers:
    H1: [60px, 1, 500, headline]
    H2: [48px, 1.1, 500, headline]
    H3: [32px, 1.2, 500, headline]
    H4: [28px, 1.2, 500, headline]
  subtitles:
    S1: [24px, 1.3, 400, body]
    S2: [18px, 1.3, 400, body]
    S3: [18px, 1.3, 400, body]
    S4: [14px, 1.2, 400, body, capitalize]
  body:
    B1: [32px, 1.2, 400, body]
    B2: [22px, 1.4, 400, body]
    B3: [20px, 1.4, 400, body]
    B4: [18px, 1.4, 400, body]
    B5: [14px, 1.4, 400, body]
    B6: [12px, 1.3, 400, body]
  eyebrows:
    E1: [14px, 1.2, 400, body, uppercase]
    E2: [10px, 1.2, 400, body, uppercase]
  nav:
    N1: [16px, 1.3, 400, body]
    N2: [14px, 1.2, 400, body, capitalize]
    N3: [14px, 1.2, 400, body]
    N4: [18px, 1.3, 400, body]
  buttons:
    L:  [20px, 1.1, 400, body]
    M:  [18px, 1.1, 400, body]
    S:  [14px, 1.1, 400, body]
    XS: [12px, 1.0, 400, body]

mobile:
  display:
    D1: [56px, 1, 500, headline]
  headers:
    H1: [44px, 1.2, 500, headline]
    H2: [32px, 1.2, 500, headline]
    H3: [26px, 1.2, 500, headline]
    H4: [20px, 1.2, 500, headline]
  body:
    B1: [32px, 1.2, 400, body]
    B2: [22px, 1.4, 400, body]
    B3: [20px, 1.5, 400, body]
    B4: [18px, 1.4, 400, body]
    B5: [14px, 1.4, 400, body]
    B6: [12px, 1.4, 400, body]
  nav:
    N1: [30px, 1.2, 400, body]
    N2: [18px, 1.2, 400, body]
    N3: [14px, 1.2, 400, body]

letter-spacing:
  display: -2%
  headers: -1%
  subheadings: -0.5%
  body: 0.5%
  eyebrows: 1.25%
```

Type rules: **All titles and headlines must use sentence case** (capitalize first word only, plus proper nouns). Never Title Case. Eyebrows are the sole exception (UPPERCASE). Short sentences. Use contractions. Arrow glyphs only for e,m,b,a,r,k letters, max 2-5 per placement, never in the word "Embark" in copy. Skip arrow glyphs in prototypes unless font files available.

## Buttons

```yaml
# All buttons: font-family body, weight 400, display flex, align-items center
# format: {height, padding, radius, bg, color, font-size, border, hover}

primary:
  L:  { h: 52px, pad: "10px 20px", radius: 100px, bg: "#0074DD", color: "#FFF", size: 20px, hover-bg: "#0047BB" }
  M:  { h: 40px, pad: "10px 20px", radius: 100px, bg: "#0074DD", color: "#FFF", size: 18px, hover-bg: "#0047BB" }
  S:  { h: 32px, pad: "10px 20px", radius: 100px, bg: "#0074DD", color: "#FFF", size: 14px, hover-bg: "#0047BB" }
  XS: { h: 32px, pad: "10px 20px", radius: 100px, bg: "#0074DD", color: "#FFF", size: 12px, hover-bg: "#0047BB" }
  icon: { name: "ic_arrow-embark", size: 16px, gap: 6px }

secondary:
  L:  { h: 52px, pad: "10px 20px", radius: 100px, bg: transparent, color: "#0074DD", size: 20px, border: "2px solid #0074DD" }
  M:  { h: 40px, pad: "10px 20px", radius: 100px, bg: transparent, color: "#0074DD", size: 18px, border: "2px solid #0074DD" }
  S:  { h: 32px, pad: "10px 20px", radius: 100px, bg: transparent, color: "#0074DD", size: 14px, border: "1px solid #0074DD" }
  XS: { h: 24px, pad: "10px 20px", radius: 100px, bg: transparent, color: "#0074DD", size: 12px, border: "1px solid #0074DD" }
  hover: { bg: "#0074DD", color: "#FFF" }
  icon: { name: "ic_arrow-embark", size: 16px, gap: 6px }

ghost:
  all: { pad: "0 0 4px", bg: transparent, color: "#0074DD", border: none }
  sizes: { L: 20px, M: 18px, S: 14px, XS: 12px }
  hover: { border-bottom: "2px solid #F277C6" }
  icon: { name: "ic_arrow-shevron", size: 16px, gap: 4px }

floating:
  active: { h: 44px, pad: "10px 20px", radius: "10px 10px 0 0", bg: "#F277C6", color: "#FFF", size: 20px }
  side:   { h: 44px, pad: "10px 20px", radius: "10px 0 0 10px", bg: "#FF8200", color: "#FFF", size: 20px }
```

## Border Radius

```yaml
tokens:
  none: 0px
  xs: 4px
  sm: 5px
  md: 8px       # inputs
  base: 10px    # cards, nav bottom
  lg: 12px      # containers
  xl: 16px      # large cards
  2xl: 20px     # sections, mobile nav dropdown
  3xl: 24px     # large containers
  4xl: 30px     # feature sections
  5xl: 40px     # hero elements
  pill: 100px   # all buttons
  round: 999px  # circles

asymmetric:
  nav-bottom:       "0 0 10px 10px"
  nav-dropdown:     "0 0 20px 20px"
  section-top:      "20px 20px 0 0"
  float-bottom:     "10px 10px 0 0"
  float-side:       "10px 0 0 10px"
  feature-callout:  "0 40px 40px 40px"
  side-panel:       "44px 0 0 44px"
  section-reveal:   "30px 30px 0 0"
```

## Spacing

```yaml
gaps: [2, 4, 6, 8, 10, 12, 16, 19, 20, 22, 24, 32, 40, 48, 64, 80, 96]
# 2=tight-inline 4=ghost-icon 6=btn-icon 8=small-groups 10=nav-items
# 12=footer-links 16=mobile-nav 20=card-content 24=content-blocks
# 32=form-fields 40=section-internal 48=between-sections
# 64=large-section 80=modal/logo-bar 96=hero

section-padding:
  desktop:      "60px 80px"
  desktop-compact: "40px 80px"
  mobile:       "40px 16px"
  nav-desktop:  "0 30px"
  nav-mobile:   "16px"
  modal-desktop: "40px 40px 80px 81px"

widths:
  desktop: 1440px
  nav: 800px
  mobile: 390px
```

## Shadows

```yaml
sm: "0px 1px 2px 0px rgba(0,0,0,0.05)"
# Embark uses shadows very sparingly. Most cards use bg color contrast.
```

## Strokes

```yaml
weights: { hairline: 0.5px, default: 1px, medium: 1.5px, heavy: 2px, emphasis: 3px, decorative: 4px }
# 1px: small btn borders (S/XS secondary), cards, tables
# 2px: large btn borders (L/M secondary), ghost hover underline
# directional: bottom-only and left-only patterns common
```

## Navigation

```yaml
desktop:
  width: 800px (fixed, centered)
  height: 40px
  layout: row, space-between, center
  padding: "0 30px"
  gap: 10px
  radius: "0 0 10px 10px"
  bg: "#0074DD" or "#FFFFFF"
  text: N3 (14px/1.2, 400)
  logo: 97.92x20px
  search: 12x12px
  items: [Happy Works, What We Do, Who We Serve, Company, Careers, Resources]

mobile:
  width: 390px
  height: 60px
  padding: 16px
  radius: "0 0 10px 10px"
  bg: "#0074DD"
  hamburger: 32x32px
  open-dropdown-radius: "0 0 20px 20px"
  open-nav-font: N1 (30px/1.2, 400)
  floating-cta: { bg: "#F277C6", w: 160px, h: 44px }
```

## Cards & Containers

```yaml
card-standard:
  layout: column, hug
  radius: 10px (default) | 20px (large)
  bg: "#FFFFFF" | "#EDE8E3"
  shadow: "0px 1px 2px 0px rgba(0,0,0,0.05)"
  gap: 20-24px
  padding: 20px (compact) | 32px (spacious)

modal-lets-talk:
  gap: 80px
  padding: "40px 40px 80px 81px"
  width: 1440px
  bg: "#027FF1"

logo-bar:
  layout: row, center
  gap: 80px
  padding: "0 80px"
  width: 1440px
  height: 200px
  bg: "#027FF1"

sunny-section-mobile:
  gap: 22px
  padding: "40px 16px"
  width: 390px
  bg: "#FEDD00"
  radius: "20px 20px 0 0"
```

## Form Inputs

```yaml
# all inputs: radius 8px
sizes:
  S:  { pad: "4px 8px" }
  M:  { pad: "8px 12px" }
  L:  { pad: "10px 15px" }
  XL: { pad: "12px 16px" }
states: [normal, default, hover, focus, error]
```

## Icons

```yaml
button: { ic_arrow-embark: 16px, ic_arrow-shevron: 16px }
nav: { ic_arrow-shevron-right: 24px, ic_arrow-shevron-down: 16px, ic_search: 12px, ic_close: 24px }
ui: { ic_Arrow-Left-Circle: 24px, ic_Arrow-Right-Circle: 24px, ic_email: 16-22px, ic_location: 16-24px, ic_lock: 24px, ic_time: 24px, ic_plus: 24-72px, ic_video: 52px }
social: { all: 18px, youtube: "22x18", linkedin: 16-26px }
```

## Images

```yaml
hero:       { radius: 0px, fit: cover, desktop-size: "659x858", position: absolute-right }
card-thumb: { radius: 10px }
team-photo: { radius: 10-20px, aspect: "square or 3:4" }
mobile-img: { radius: 20px, width: responsive }
illustration: { radius: 0px, fit: fill, use: "decorative background" }
```

## Logo

```yaml
primary-logotype:
  cdn: "https://8725594.fs1.hubspotusercontent-na2.net/hubfs/8725594/Embark2024/images/Embark-Primary%20Logotype-Black.svg"
  figma: "Embark-Primary Logotype-Black"
  variants: [black, white]
  nav-size: "97.92x20px"
  min-desktop: 48px height
  min-mobile: 32px height
  primary-color: "#000000"
  secondary-color: "#FFFFFF (print only)"
  clear-space: "height of lowercase x, all sides"

logomark:
  use: "small spaces only (social profile icons)"
  never: "alongside full logo"
  outlined: "1px stroke #000000, large formats only"
```

## Component Inventory

```yaml
with-variants:
  btn: "Size(L/M/S/XS) x Type(Primary/Secondary/Ghost/floating) x State"
  nav: "type(desktop/Mobile) x state(default/open) x color(blue/white)"
  input: "size(S/M/L/XL) x state(default/error/focus/hover/normal)"
  card-S: "state(default/hover)"
  card-bg-S: "state(default/hover)"
  Cards: "multiple layout variants"
  card-team: "multiple"
  Section-hero: "multiple"
  section-1-4: "layout variants"
  tag: "Size(M/S) x state(default/hover)"
  dropdown: "open/closed"
  Filter: "default/active"
  toggle: "on/off"
  radio-btn: "selected/default"
  list-item: "default/hover/active/selected"
  testimonials: "multiple"
  lets-talk-modal: "desktop/mobile"
  Tooltip-trigger: "Active/Default/Destructive/Focused/Hover/Success"

standalone: [footer, logos, form, map, social-icons, career-awards, Featured-Case-Studies, Featured-insights, bread-crumbs, Label, Helper]
```

## Figma Pages

```yaml
ALL-DESIGNS-FINAL-FOR-DEV: "production-ready desktop + mobile"
Components: "full component library"
Branding-Illustrations: "color palette, illustrations, brand assets"
Updated-Nav: "latest nav iterations"
Hero-carousel: "hero carousel patterns"
Contact-Page-v2: "contact designs"
Home-Page-for-Approval: "approved home page"
Landing-page: "lead gen"
CTA-modal: "CTA modal designs"
Ecommerce-Store: "store pages"
```

## Copy & Tone

Aspirational, warm, witty. Never jargon. Headlines subvert business tropes ("Not business as usual." "Year-over-year happiness."). Short sentences. Contractions. Positive framing only. CTAs direct ("Talk to an advisor", "Download the guide"). Smiles not LOLs. Eyebrows UPPERCASE. All titles/headlines sentence case (never Title Case).

## Anti-Patterns

- Never Ink (#000) as background
- Never all 7 bright colors in one layout
- Never Cherry + Spring together
- Never arrow glyphs in "Embark" in copy
- Never >5 arrow glyphs per placement
- Never stack arrow glyphs vertically
- Never primary logotype next to logomark
- Never all-caps headlines (eyebrows only)
- Never Title Case in headlines or titles (sentence case only: capitalize first word + proper nouns)
- Never stock photography
- Never business jargon
- Never outlined logomark at small sizes
- Never use text placeholders for logos -- use real image assets or omit the section

## CDN Asset Registry

All assets are hosted on Embark's HubSpot CDN. Use these exact URLs in prototypes.

```yaml
# NOTE: The na1 CDN redirects to na2. Both work but use the direct na2 URL to avoid redirect issues.
cdn-base: "https://www.embarkwithus.com/hubfs"
cdn-base-alt: "https://8725594.fs1.hubspotusercontent-na2.net/hubfs/8725594"

embark-logo:
  black-svg: "https://8725594.fs1.hubspotusercontent-na2.net/hubfs/8725594/Embark2024/images/Embark-Primary%20Logotype-Black.svg"
  white-svg: "https://8725594.fs1.hubspotusercontent-na2.net/hubfs/8725594/Embark2024/images/embark_logo.svg"
  black-png: "https://www.embarkwithus.com/hs-fs/hubfs/Embark-Primary%20Logotype-Black-RGB.png?width=338&height=70&name=Embark-Primary%20Logotype-Black-RGB.png"
  # The inline SVG below is the white variant, 98x21 viewBox.
  # Use this as a fallback when the CDN SVG doesn't load.
  inline-svg-white: '<svg width="98" height="21" viewBox="0 0 98 21" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M56.7844 12.7568C56.7844 18.1007 53.7186 20.8851 50.3436 20.8851C48.0935 20.8851 46.0124 19.6476 45.1968 17.2287L44.1842 20.6037H42.3279V0.916016H45.3093V8.2006C46.1811 5.83799 48.0935 4.7131 50.2874 4.7131C53.6906 4.7131 56.7844 7.35674 56.7844 12.7568ZM53.7749 12.7568C53.7749 9.21299 52.1718 7.21622 49.4717 7.21622C46.6873 7.21622 45.0559 9.46622 45.0559 12.8695C45.0559 16.2727 46.6592 18.4101 49.3592 18.4101C52.1435 18.4101 53.7749 16.2726 53.7749 12.7568ZM15.1877 14.6131C15.6096 14.8944 16.0877 15.2882 16.5096 15.6819L16.0877 10.3661L11.5314 13.1786C12.122 13.263 12.6846 13.4317 13.1908 13.6286C10.9407 17.0319 8.80323 18.6912 7.3126 18.6912C5.7376 18.6912 5.00625 17.3976 4.89375 15.9069C9.1126 13.5162 13.2189 10.0569 13.2189 7.0755C13.2189 5.66925 12.094 4.713 10.4345 4.713C7.14385 4.713 2.7 9.63488 2.30625 14.7256C1.51875 15.035 0.73125 15.3162 0 15.5695L0.871979 17.8475C1.37812 17.6506 1.9126 17.4257 2.44698 17.1725C2.95323 19.3101 4.44385 20.8851 7.17198 20.8851C9.73135 20.8851 12.5721 19.1695 15.1877 14.6131ZM10.519 7.10363C10.519 8.59425 8.63448 10.788 5.23135 13.2631C6.3001 10.0569 9.28146 6.82237 10.294 6.82237C10.4345 6.82237 10.519 6.87862 10.519 7.10363ZM18.4781 4.99415V20.6038H18.4782H21.4596V10.3662C21.4596 8.0881 23.0626 7.24425 24.6096 7.24425C26.2971 7.24425 27.4783 8.2006 27.4783 10.31V20.6038H30.4597V10.3662C30.4597 8.0881 32.0627 7.24425 33.6097 7.24425C35.2972 7.24425 36.4784 8.2006 36.4784 10.31V20.6038H39.4598V9.91613C39.4598 6.513 37.3785 4.713 34.6222 4.713C32.6816 4.713 30.769 5.75352 30.1502 7.91925C29.5033 5.80977 27.8158 4.713 25.7065 4.713C23.794 4.713 21.9939 5.7255 21.3751 7.7505L21.2345 4.99415H18.4781ZM72.3092 20.7446V18.5509C72.3092 18.5509 72.0842 18.6072 71.831 18.6072C70.9309 18.6072 70.7059 18.2134 70.7059 17.454V9.66331C70.7059 6.20383 68.0903 4.7132 65.0246 4.7132C61.5932 4.7132 59.1182 6.48508 58.612 9.80383L61.509 10.3382C61.7902 7.91956 63.0558 7.01945 64.9121 7.01945C66.7122 7.01945 67.8091 7.89133 67.8091 9.77581V10.8164C66.2903 10.9007 64.6028 11.0977 63.1121 11.4913C60.8902 12.0538 58.4996 13.2632 58.4996 16.2727C58.4996 18.9446 60.3839 20.8852 63.3371 20.8852C65.5591 20.8852 67.3309 19.7602 67.8091 17.7914C67.8935 19.9008 68.8779 20.8289 70.9873 20.8289C71.7185 20.8289 72.3092 20.7446 72.3092 20.7446ZM67.8091 12.8131V15.2882C67.8091 17.1725 66.4591 18.7195 64.2372 18.7195C62.4371 18.7195 61.3965 17.7351 61.3965 16.1038C61.3965 14.81 62.0433 14.0506 63.5903 13.5162C64.7716 13.0943 66.4591 12.8976 67.8091 12.8131ZM73.8839 20.6038V4.99415H76.6402L76.7808 7.32863C77.3152 5.6129 78.4966 4.713 80.1278 4.713C82.0966 4.713 83.7279 5.97852 83.5309 9.52238L80.8028 9.94435C80.9716 7.638 80.1279 7.04738 79.0309 7.04738C77.9058 7.04738 76.8653 7.83488 76.8653 10.0006V20.6038H73.884H73.8839ZM96.0183 14.6131C95.1463 12.8131 93.937 11.5193 92.4745 11.1256L92.4746 11.1255L97.9309 4.99414H94.4152L88.1715 12.0817V0.916016H85.1901V20.6038H88.1715V13.0943C88.5933 12.785 89.0996 12.6162 89.6902 12.6162C92.6715 12.6162 94.0215 16.582 94.584 20.6038H97.6777C97.4246 18.8601 96.9746 16.5537 96.0183 14.6131Z" fill="white"/></svg>'

client-logos:
  # These are the logos currently uploaded to HubSpot CDN.
  # Use these for the "Trusted by" logo bar on landing pages.
  gamestop:      "https://www.embarkwithus.com/hubfs/FunnelEnvy/logos/gamestop.svg"
  slb:           "https://www.embarkwithus.com/hubfs/FunnelEnvy/logos/slb.svg"
  hellofresh:    "https://www.embarkwithus.com/hubfs/FunnelEnvy/logos/hellofresh.svg"
  aimbridge:     "https://www.embarkwithus.com/hubfs/aimbridge-2.svg"
  tgi-fridays:   "https://www.embarkwithus.com/hubfs/FunnelEnvy/logos/tgi-fridays.svg"
  neiman-marcus: "https://www.embarkwithus.com/hubfs/FunnelEnvy/logos/neiman-marcus.svg"
  daseke:        "https://www.embarkwithus.com/hubfs/FunnelEnvy/logos/daseke.svg"
  # NOTE: Logos for case-study companies (Interstate Batteries, Solo Brands,
  # Helmerich & Payne, Atlas Technical, SecurityScorecard, Ashford Hospitality)
  # are NOT yet uploaded to HubSpot. Use the available logos above instead,
  # or upload new ones to hubfs/FunnelEnvy/logos/ following the same pattern.

icons:
  arrow-up-right:      "https://www.embarkwithus.com/hubfs/arrow-up-right.svg"
  arrow-up-right-blue: "https://www.embarkwithus.com/hubfs/arrow-up-right-blue.svg"
  arrow-up-right-red:  "https://www.embarkwithus.com/hubfs/arrow-up-right-red.svg"
  arrow-up-right-sky:  "https://www.embarkwithus.com/hubfs/arrow-up-right-sky.svg"
  close:               "https://www.embarkwithus.com/hubfs/close_small.svg"
  right-icon:          "https://www.embarkwithus.com/hubfs/right-icon.svg"
  search:              "https://www.embarkwithus.com/hubfs/raw_assets/public/Embark2024/images/search-icon.svg"
  brand-illustration:  "https://8725594.fs1.hubspotusercontent-na2.net/hubfs/8725594/Embark2024/images/Embark%20Brand%20System%20Illustration%204.svg"
  form-arrow:          "https://www.embarkwithus.com/hubfs/2025%20Website/images/arrow.svg"

hero-images:
  homepage: "https://www.embarkwithus.com/hubfs/Frame%20427318829.png"

social:
  linkedin:  "https://www.linkedin.com/company/embarkwithus/"
  youtube:   "https://www.youtube.com/c/EmbarkgroupCo2014/"
  instagram: "https://www.instagram.com/embarkwithus/"
  twitter:   "https://twitter.com/embarkwithus"
  facebook:  "https://www.facebook.com/embarkwithustoday"
```

## Design Agent Instructions

When building landing pages, the design agent MUST:

1. **Use real assets, never placeholders.** The CDN Asset Registry above has every URL needed. Inline the Embark logo SVG as a fallback. Use real client logos from the registry for the social proof bar.
2. **Reference brand-components.html** for ready-to-use HTML/CSS snippets. Compose pages by assembling these components, not building from scratch.
3. **Match embarkwithus.com visual quality.** The live site uses generous whitespace, Sand (#EDE8E3) section backgrounds for warmth, rounded corners on cards (10-20px), pill buttons, and a blue nav bar with bottom-radius. The result should look like a real Embark page, not a wireframe.
4. **Use color strategically.** Sand sections break up white. Electric blue (#027FF1) for bold CTA banners. Sunny (#FEDD00) sparingly for accent sections. Never all-white layouts.
5. **Typography hierarchy matters.** H1 at 60px desktop / 44px mobile. Eyebrows uppercase, 14px, muted. Body at 18px. Big stat numbers at 48-64px in nav-blue.
