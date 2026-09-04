---
name: Proof Agent
description: Direct technical documentation for independent AI code verification.
colors:
  verification-red: "#dc3545"
  pass-green: "#198754"
  pass-green-text: "#157347"
  partial-orange: "#fd7e14"
  partial-orange-text: "#b84e00"
  ink: "#212529"
  text-secondary: "#6c757d"
  text-muted: "#adb5bd"
  surface: "#fefefe"
  surface-raised: "#f8f9fa"
  border: "#e9ecef"
typography:
  display:
    fontFamily: "JetBrains Mono, monospace"
    fontSize: "clamp(2.25rem, 5vw, 3.75rem)"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "-0.03em"
  body:
    fontFamily: "Inter Tight, -apple-system, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "normal"
  label:
    fontFamily: "JetBrains Mono, monospace"
    fontSize: "0.875rem"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "normal"
rounded:
  sm: "6px"
  md: "8px"
spacing:
  xs: "8px"
  sm: "12px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  2xl: "48px"
  3xl: "64px"
components:
  resource-link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    padding: "12px 0"
  code-block:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.surface}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: "24px"
  documentation-panel:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "32px"
---

# Design System: Proof Agent

## 1. Overview

**Creative North Star: "The Verification Bench"**

Proof Agent should feel like a compact workbench used to inspect a change, not a campaign built to sell one. Neutral surfaces carry dense technical content while verification red marks attention, failure, and primary paths. Green and orange retain their literal verdict roles.

The composition is asymmetric and practical: explanation and evidence occupy the main reading column, while runnable usage paths stay visible in a dedicated technical panel. It explicitly rejects generic SaaS landing pages, excessive card grids, decorative grid backgrounds, inflated AI claims, and unrelated visual spectacle.

**Key Characteristics:**
- Compact technical rhythm with clear section breaks
- Monospace for commands, labels, and high-signal headings
- Flat surfaces separated by tone and rules instead of decorative shadow
- Direct links to every supported usage path

## 2. Colors

The palette is neutral and high-contrast, with semantic accents reserved for verification states.

### Primary
- **Verification Red** (#dc3545): Primary links, section rules, focus, and FAIL states.

### Secondary
- **Pass Green** (#198754): PASS states and positive operational notices.
- **Pass Green Text** (#157347): Accessible PASS labels on light surfaces.
- **Partial Orange** (#fd7e14): PARTIAL states and experimental warnings.
- **Partial Orange Text** (#b84e00): Accessible PARTIAL labels on light surfaces.

### Neutral
- **Ink** (#212529): Primary text and code surfaces.
- **Secondary Text** (#6c757d): Supporting prose on white or near-white surfaces.
- **Muted Text** (#adb5bd): Short tertiary labels only, never body copy.
- **Surface** (#fefefe): Main page background.
- **Raised Surface** (#f8f9fa): Technical panels and grouped process content.
- **Border** (#e9ecef): Dividers and resource rows.

### Named Rules
**The Semantic Accent Rule.** Red, green, and orange must retain verification meaning; never use them as interchangeable decoration.

## 3. Typography

**Display Font:** JetBrains Mono (with monospace fallback)  
**Body Font:** Inter Tight (with system sans-serif fallback)  
**Label/Mono Font:** JetBrains Mono

**Character:** The pairing reads like a technical report with a human editing hand. Monospace establishes mechanism and verdicts; the condensed sans keeps documentation compact.

### Hierarchy
- **Display** (600, clamp(2.25rem, 5vw, 3.75rem), 1): Product name only.
- **Headline** (600, 1.25rem, 1.3): Major documentation sections.
- **Title** (600, 1rem, 1.4): Usage paths and process steps.
- **Body** (400, 1rem, 1.6): Explanatory copy, capped at 72ch.
- **Label** (600, 0.875rem, normal case): Resource links, commands, and verdict names.

### Named Rules
**The Mechanism First Rule.** Use monospace where the text names a command, path, verdict, or system boundary, not as decoration.

## 4. Elevation

The system uses no shadows. Depth comes from tonal surface changes, full-width rules, and spacing. Interactive feedback uses color and a small translation without implying floating cards.

### Named Rules
**The Flat Bench Rule.** Surfaces stay flat at rest; never pair a border with a wide decorative shadow.

## 5. Components

### Buttons
- **Shape:** Resource actions are text links with a full-row 44px minimum target, not filled buttons.
- **Primary:** Ink text with a red directional marker.
- **Hover / Focus:** Red text on hover; a 2px red outline on focus-visible.

### Cards / Containers
- **Corner Style:** Small radius (8px maximum).
- **Background:** White for content, raised surface for setup and process groups.
- **Shadow Strategy:** None.
- **Border:** Horizontal dividers only where rows need separation.
- **Internal Padding:** 24px to 32px.

### Navigation
- Resource links form a compact ruled list on desktop and remain full-width touch targets on mobile.

### Verdict Row
- Verdicts use semantic text and compact rows rather than three interchangeable cards. The label and supporting consequence remain readable as one unit.

## 6. Do's and Don'ts

### Do:
- **Do** keep body copy between 45ch and 72ch.
- **Do** use the 8px, 12px, 16px, 24px, 32px, 48px, and 64px spacing scale.
- **Do** preserve direct links to the repository, GitHub Action, and Grok Bot in the hero and experimental-tool resources.
- **Do** keep mobile content in a single logical reading order without horizontal scrolling.

### Don't:
- **Don't** turn the site into a generic SaaS landing page.
- **Don't** use excessive card grids or decorative grid backgrounds.
- **Don't** use inflated AI claims or unrelated visual spectacle.
- **Don't** use a colored border-left or border-right wider than 1px as an accent.
- **Don't** hide operational details behind marketing language.
