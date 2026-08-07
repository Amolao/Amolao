---
name: Liquid Glass GitHub Profile
description: A quiet bilingual developer profile expressed as one adaptive liquid-glass calling card.
colors:
  canvas-ice: "#f7f9fc"
  canvas-mist: "#e8eef7"
  canvas-night: "#090d16"
  canvas-night-raised: "#111827"
  ink-primary: "#101828"
  ink-secondary: "#526070"
  text-on-night: "#f6f8fb"
  text-muted-on-night: "#a9b5c5"
  refraction-blue: "#2997ff"
  refraction-cyan: "#5ac8fa"
  refraction-violet: "#bf5af2"
  refraction-purple: "#af52de"
  availability-green: "#34c759"
  glass-light: "rgba(255, 255, 255, 0.38)"
  glass-dark: "rgba(255, 255, 255, 0.20)"
typography:
  display-zh:
    fontFamily: '-apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans SC", "Microsoft YaHei", sans-serif'
    fontSize: "76px"
    fontWeight: 650
    lineHeight: 1
    letterSpacing: "-2.2px"
  display-en:
    fontFamily: '-apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
    fontSize: "69px"
    fontWeight: 650
    lineHeight: 1
    letterSpacing: "-2.1px"
  subtitle:
    fontFamily: '-apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans SC", "Microsoft YaHei", sans-serif'
    fontSize: "25px"
    fontWeight: 450
    lineHeight: 1
    letterSpacing: "0.4px"
  status:
    fontFamily: '-apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans SC", "Microsoft YaHei", sans-serif'
    fontSize: "13px"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "1.2px"
rounded:
  status-pill: "19px"
  glass-panel: "28px"
  hero-frame: "32px"
  orb: "50%"
spacing:
  hero-frame-inset: "58px"
  hero-copy-inset: "112px"
  status-inline: "21px"
  contact-gap: "0.5em"
components:
  profile-hero:
    backgroundColor: "{colors.canvas-ice}"
    textColor: "{colors.ink-primary}"
    rounded: "{rounded.hero-frame}"
    width: "100%"
    size: "1280px 520px"
  readme-navigation:
    textColor: "{colors.ink-primary}"
    padding: "0"
    width: "100%"
---

# Design System: Liquid Glass GitHub Profile

## Overview

**Creative North Star: "The Refractive Calling Card"**

The profile behaves like one digital glass object catching the color of its environment. Its mood is quiet, precise, cool, and professionally optimistic: a restrained ice-white or ink-black field carries blue-violet refraction, while the content remains sparse enough for the student Unity developer identity to register immediately.

The hero is the identity, not a container for a collection of widgets. Apple-like reduction appears through generous emptiness, exact hairlines, system typography, and adaptive light/dark material rather than imitation interface chrome. The surrounding Markdown stays deliberately plain so the glass artwork owns the visual voice and the language/contact actions remain obvious.

**Key Characteristics:**

- One continuous liquid-glass hero, never a dashboard of cards.
- Ice-white and ink-black theme adaptation with blue-violet refracted light.
- Precise translucent edges, soft ambient depth, and restrained geometry.
- System-native bilingual typography with matching Chinese and English hierarchy.
- Minimal README navigation that moves from identity to direct contact.

## Colors

The palette is nearly neutral until refracted blue and violet light crosses the glass; a single green signal communicates availability.

### Primary

- **Refractive Blue:** `{colors.refraction-blue}` supplies the brightest environmental light and the cool face of the Unity prism.
- **Refractive Violet:** `{colors.refraction-violet}` balances the blue glow and marks the prism's warmer face.

### Secondary

- **Optical Cyan:** `{colors.refraction-cyan}` softens blue into translucent halos and edge highlights.
- **Optical Purple:** `{colors.refraction-purple}` extends violet into the lowest ambient bloom.
- **Availability Green:** `{colors.availability-green}` is reserved for the small open-to-opportunities signal.

### Neutral

- **Ice Canvas / Mist Canvas:** `{colors.canvas-ice}` and `{colors.canvas-mist}` form the light-theme environmental gradient.
- **Night Canvas / Raised Night:** `{colors.canvas-night}` and `{colors.canvas-night-raised}` form the dark-theme counterpart.
- **Primary / Secondary Ink:** `{colors.ink-primary}` and `{colors.ink-secondary}` establish the light-theme text hierarchy; `{colors.text-on-night}` and `{colors.text-muted-on-night}` mirror it in dark mode.
- **Adaptive Glass:** `{colors.glass-light}` becomes `{colors.glass-dark}` under the system dark preference so the panel remains translucent rather than turning opaque.

**The Refracted-Only Rule.** Saturated blue and violet belong to environmental light, optical edges, and the prism; they do not become broad text fills or decorative badges.

**The One Green Signal Rule.** Green identifies opportunity status only. Its rarity preserves meaning.

## Typography

**Display Font:** Apple system stack, with Segoe UI and Chinese system fallbacks  
**Body Font:** GitHub's rendered Markdown font stack  
**Label Font:** Apple system stack, with Segoe UI and Chinese system fallbacks

**Character:** The type is neutral, compact, and native to the viewer's operating system. Weight and spacing—not a branded display face—create the hierarchy, allowing the optical material to carry personality.

### Hierarchy

- **Chinese Display:** `{typography.display-zh}` is used once for the hero's profession title.
- **English Display:** `{typography.display-en}` compensates for the longer English title while preserving the same visual weight.
- **Subtitle:** `{typography.subtitle}` identifies the student role and repeats the developer direction in a quieter register.
- **Status Label:** `{typography.status}` uses compact semibold type with open tracking; the English counterpart reduces slightly to fit its longer phrase.
- **README Body and Links:** Native GitHub Markdown typography remains unstyled and centered, keeping the supporting copy quieter than the SVG hero.

**The One Display Line Rule.** Each language gets one dominant profession line; supporting identity and availability never compete at display scale.

## Layout

The README follows a strict vertical reading path: a right-aligned language switch, a centered full-width hero, one centered identity sentence, then a centered contact row. The profile hero uses a fixed `1280 × 520` viewBox and scales uniformly to `100%` width, preserving its composition and rounded silhouette at every GitHub-rendered width.

Inside the hero, a single inset glass panel sits within the outer canvas. Copy occupies the left side in a status-title-subtitle stack; a large glass orb containing the abstract Unity cube anchors the right side. The two language variants preserve this geometry, changing only text widths and their measured type sizes.

The contact row is intentionally linear: actionable email first, followed by dot-separated inactive placeholders for the website and Bilibili. There is no bespoke mobile rearrangement in the current implementation; the SVG scales as a whole and the Markdown host controls wrapping.

## Elevation & Depth

Depth is optical rather than interactive. The inner glass sheet re-samples and displaces the environmental light beneath it, the orb applies a tighter second refraction pass, and blue-violet spectral edges reveal the material thickness. Broad offset shadows lift both lenses while localized white caustics clarify curvature. No hover elevation or motion is implemented.

### Shadow Vocabulary

- **Glass Ambient:** `feDropShadow(0 26px 24px rgba(7, 17, 31, 0.18))` lifts the continuous inner sheet without producing a hard card edge.
- **Orb Ambient:** `feDropShadow(0 28px 22px rgba(8, 16, 30, 0.30))` gives the optical sphere denser local depth.
- **Environmental Bloom:** `feGaussianBlur(34px)` diffuses the colored ellipses and light ribbon behind the glass.
- **Panel Refraction:** low-frequency displacement at `34px` bends the repeated backdrop inside the panel while a small blur keeps the result lens-like.
- **Orb Refraction:** a tighter `52px` displacement produces stronger curvature inside the circular lens.

**The Ambient-Only Rule.** Shadows describe translucent material and spatial separation; they never indicate a clickable card or hover state.

## Shapes

The form language pairs large continuous curves with exact crystalline geometry. The outer hero uses `{rounded.hero-frame}`, the inset sheet uses `{rounded.glass-panel}`, and the status capsule uses `{rounded.status-pill}`. The right-side orb is a true circle containing a three-faced isometric cube; narrow gradient strokes and translucent highlights keep both forms optical rather than illustrative.

**The Continuous Surface Rule.** Rounded rectangles may define the outer canvas, inner glass sheet, and status capsule only; do not subdivide the profile into additional floating panels.

## Components

### Navigation

The README language/contact navigation is native Markdown by design. The language switch sits alone at the top right. Below the hero, the contact row is centered and ordered as email, website placeholder, then Bilibili placeholder. Only valid destinations are anchors; unavailable destinations remain plain text with an explicit “coming soon” state. No custom button styling, hover effects, or faux-disabled links are introduced.

### Profile Hero

The signature component is a bilingual, adaptive SVG calling card. It combines the environmental canvas, one refractive liquid-glass sheet, a smaller opportunity lens, profession title, student subtitle, and an abstract Unity prism inside a spherical glass lens. The panel and sphere each duplicate and distort the environmental light so transparency reads as physical refraction rather than a pale overlay. Chinese and English variants mirror geometry and semantics. The SVG provides `role="img"`, a localized title and description, and switches its canvas, glass, text, and edge values through `prefers-color-scheme: dark`.

## Do's and Don'ts

### Do:

- **Do** preserve the one-hero reading path: language, identity artwork, short identity sentence, then contact.
- **Do** keep Chinese and English geometry, facts, accessibility labels, and hierarchy equivalent.
- **Do** adapt the glass, canvas, text, and edge contrast together when supporting light and dark themes.
- **Do** use plain text for destinations that are not yet available.
- **Do** let translucent material and refracted light supply distinction while supporting copy stays quiet.

### Don't:

- **Don't** add statistics cards, skill badges, technology stacks, activity widgets, or decorative card grids.
- **Don't** invent projects, links, credentials, personal claims, a real name, or a username.
- **Don't** turn the blue-violet refraction palette into loud filled controls or rainbow decoration.
- **Don't** split the hero into multiple glass cards or add unrelated UI component families.
- **Don't** style unavailable website or Bilibili placeholders as working links.
