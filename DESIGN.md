---
name: Obsidian Cyan Scientific
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#b9cac3'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#83948e'
  outline-variant: '#3a4a45'
  surface-tint: '#00e0bb'
  primary: '#ffffff'
  on-primary: '#00382d'
  primary-container: '#00ffd5'
  on-primary-container: '#00725e'
  inverse-primary: '#006b58'
  secondary: '#43f3d7'
  on-secondary: '#00372f'
  secondary-container: '#00d6bb'
  on-secondary-container: '#00574c'
  tertiary: '#fefffd'
  on-tertiary: '#00382e'
  tertiary-container: '#37fdd8'
  on-tertiary-container: '#00715f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#00ffd5'
  primary-fixed-dim: '#00e0bb'
  on-primary-fixed: '#002019'
  on-primary-fixed-variant: '#005142'
  secondary-fixed: '#50fbdf'
  secondary-fixed-dim: '#1bdec4'
  on-secondary-fixed: '#00201b'
  on-secondary-fixed-variant: '#005046'
  tertiary-fixed: '#38fdd8'
  tertiary-fixed-dim: '#00dfbd'
  on-tertiary-fixed: '#00201a'
  on-tertiary-fixed-variant: '#005143'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: 80px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  container-max: 1440px
  gutter: 32px
  section-padding: 120px
  card-padding: 40px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

This design system is engineered for high-stakes scientific storytelling, blending a premium luxury aesthetic with futuristic technical precision. It targets a sophisticated audience of investors, researchers, and global stakeholders within the sustainable materials industry.

The design style is a hybrid of **Apple-inspired Minimalism** and **High-Tech Glassmorphism**. It utilizes a deep, multi-layered obsidian background to create a "void" where data and imagery feel suspended. Key characteristics include:
- **Cinematic immersion:** Heavy use of high-resolution imagery and full-bleed transitions.
- **Glassmorphism:** UI components appear as frosted, translucent biological panes, reflecting the bioplastic subject matter.
- **Luminescent accents:** Primary colors are treated as light sources (neon) rather than flat fills, evoking a sense of laboratory precision and energy.

## Colors

The palette is anchored in a monochromatic obsidian foundation to maximize the "pop" of the cyan and emerald bioluminescent accents.

- **Primary (#00FFD5):** Used for critical data points, active states, and primary calls to action. It should always feel like it is emitting light.
- **Secondary/Tertiary:** Used for data visualization gradients and subtle atmospheric glows behind glass layers.
- **Surfaces:** Utilize the Deep Teal Navy (#08131A) for card containers. Deep Forest Cyan (#0B1F1F) is reserved for hovering states or secondary section backgrounds to provide subtle depth without breaking the dark-mode immersion.

## Typography

Typography balances technical rigor with editorial elegance. 

- **Headlines:** Space Grotesk provides a geometric, futuristic skeleton. Display sizes should use tight letter-spacing to emphasize the modern, scientific feel.
- **Body:** Inter is used for its high legibility in technical descriptions. Maintain generous line heights to ensure readability against dark backgrounds.
- **Labels:** JetBrains Mono (monospaced) is introduced for data labels, scientific notation, and metadata to reinforce the research-driven narrative.

## Layout & Spacing

The layout philosophy follows a **Cinematic Grid** model. It uses expansive margins and white space (or "dark space") to create a sense of importance and focus.

- **Desktop:** A 12-column grid with wide 32px gutters. Content should be centered with a 1440px max-width to maintain focus.
- **Sections:** Vertical rhythm is exaggerated; use 120px to 160px of padding between major sections to allow the "bioplastic" imagery to breathe.
- **Responsive:** On mobile, margins reduce to 20px, and the grid collapses to a single column. Section padding should be halved to 60px to maintain momentum on smaller screens.

## Elevation & Depth

Elevation is achieved through translucency and light refraction rather than traditional shadows.

- **Glass Layers:** All floating containers use a background blur of 24px and a semi-transparent background color (White at 5% opacity).
- **Borders:** "Ghost" borders are used on all glass elements—1px solid White at 10% opacity.
- **Luminescence:** Use `box-shadow` only as a "glow" effect for active elements (e.g., `0 0 20px rgba(0, 255, 213, 0.3)`).
- **Z-Index:** Content is layered such that data overlays sit on top of blurred organic shapes, creating a "microscope lens" depth effect.

## Shapes

The design uses a **Pill-shaped** language to echo the organic nature of bioplastics while maintaining a modern, high-end tech feel. 

- **Primary Elements:** Buttons and tags use `rounded-full` (capsule) shapes.
- **Containers:** Research cards and data modules use `rounded-xl` (24px - 48px) to soften the technical data and make it feel more approachable and fluid.

## Components

### Buttons
- **Primary:** Rounded-full, glass backdrop, 1px Primary color border. On hover, the border glow expands and the background fill increases in opacity (15% to 25%).
- **Ghost:** No border, primary color text, subtle 10% background fill on hover.

### Research Cards
- **Structure:** 24px blur background, 1px White/10 border. Padding is generous (40px). 
- **Content:** Headline-md at the top, Label-caps for category, and Body-md for research summary.

### Interactive Gallery
- Elements should use horizontal scrolling with a snapping effect. Each slide is a full-height glass pane with high-contrast scientific photography.

### Data Inputs & Checkboxes
- Inputs are glass-based with bottom-only borders (1px White/20). On focus, the bottom border transitions to the Primary neon color with a subtle glow.

### Chips / Tags
- Small capsule shapes used for material properties (e.g., "Biodegradable"). Background is 10% Primary color, text is 100% Primary color.