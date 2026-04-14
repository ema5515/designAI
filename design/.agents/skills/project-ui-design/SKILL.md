---
name: Project UI Design
description: Generate UI consistent with the existing product style and UX rules.
---

# Usage

Use this skill whenever you need to generate new UI, pages, components, flows, or product screens consistent with the existing application style.

Priority rules:
1. Preserve the existing design system.
2. Extend the current patterns conservatively.
3. Prefer clarity, consistency, and product readiness over novelty.
4. Do not invent a new visual language unless explicitly requested.

# Project Summary

# Repository Summary

- Root: `/Users/emanueledagata/code/v0/portfolio_disegno`
- Detected hints: Next.js, Tailwind CSS, shadcn/ui, Charts, Radix/Lucide
- Total indexed files: 68
- Relevant UI/design files: 64

## Key dependencies

- @radix-ui/react-dialog: 1.1.4
- @radix-ui/react-dropdown-menu: 2.1.4
- @radix-ui/react-select: 2.1.4
- @radix-ui/react-tabs: 1.1.2
- class-variance-authority: ^0.7.1
- clsx: ^2.1.1
- lucide-react: ^0.454.0
- next: 15.5.9
- react: 19.1.0
- react-dom: 19.1.0
- recharts: 2.15.4
- tailwind-merge: ^2.5.5
- tailwindcss: ^4.1.9

## Key analysis goals

- Extract design tokens already present in the repository.
- Infer layout and component rules from shared files and pages.
- Produce a reusable design skill for future UI generation.
- Preserve style consistency and avoid design drift.


# Final Design Skill

# Product UI/UX Design Skill — “Paperfolio X” System

## Purpose
Create new product interfaces that look and feel native to the existing Next.js app, uphold strong UX principles, and are ready for production without visual or behavioral drift.

## AI Role
You are a product UI/UX designer and interface system builder. You extend the application’s design language by generating coherent screens, components, and flows that reuse established tokens, patterns, and behaviors while scaling to new use cases.

## Design Philosophy
- Marry clarity and utility with the app’s bold “paper card” aesthetic: high-contrast black outlines, offset shadows, friendly radii, and vibrant accent chips.
- Favor simple, legible typography (Onest 500/700) and generous spacing to maintain approachable, professional tone.
- Build with real-world constraints: responsive grids, accessible states, keyboard flows, and production-ready code patterns that match the repo’s Tailwind v4 + Radix UI + shadcn-style primitives.

## Core UI/UX Principles
- Clarity: One clear primary action per view; obvious visual grouping; scannable content.
- Hierarchy: Typographic scale, spacing, and contrast create a single dominant heading and well-ordered secondary content.
- Consistency: Reuse tokens, radii, border weights, shadow styles, and interaction states across all components and pages.
- Task Completion: Reduce steps, keep actions within reach, and place confirmations inline where possible.
- Accessibility: Provide focus-visible rings, sufficient contrast, semantic structure, and keyboard-friendly flows.
- Scalability: Use modular cards, grids, and primitives that extend to more data and features without redesigns.

## Project-Specific Style Rules
- Color tokens (light mode defaults):
  - Background: `#FFFFFF`; Foreground: `#0A0A0A` (primary text).
  - Primary: `#0A0A0A` on `#FAFAFA` foreground.
  - Secondary/muted/accent surfaces: light neutrals (`#F5F5F5`) with `#171717` foreground.
  - Destructive: `#E7000B` (dark mode variant available).
  - Ring: `#A1A1A1`; Border: black on light (`#0A0A0A`).
  - Accent “chips” used in hero and cards: Blue `#2F81F7`, Yellow `#FFC224`, Pink `#FF6B7A`, Indigo `#6366F1`. Use these sparingly to highlight keywords, tags, and callouts—not as base surfaces.
  - Dark mode has paired tokens; use tokens, not raw colors, except for the sanctioned accent chips above.
- Typography:
  - Family: Onest (weights 500, 700). Sans for UI; Mono only when essential (code, metrics alignment).
  - Scale guidance:
    - Display/H1: 42–72 px responsive
    - H2: 32–52 px responsive
    - H3: 24–28 px
    - Body: 16–18 px; Lead: 18–20 px
    - Overline/Tag: 12–14 px, semi-bold
  - Line-height: Tight for headings, comfortable for paragraphs (approx. 1.3–1.6).
- Spacing:
  - Base rhythm: multiples of 4; common blocks use 16/24/32 px vertical spacing; sections often 64–96 px (`py-16`/`py-24`).
  - Grid gaps typically 6/8/12 (Tailwind `gap-6/8/12`).
  - Page gutters: `container mx-auto px-4`; content max-width commonly `max-w-7xl`.
- Radius:
  - Token `--radius: 1rem` for general UI (inputs, small buttons).
  - Larger surfaces use friendly radii: `rounded-xl` / `rounded-3xl` / `rounded-[32px]`.
  - Avatars, badges: `rounded-full`.
- Borders:
  - Use bold black outlines on white cards: `border-[3px]` or `border-4 border-black`.
  - Inputs and small elements: `border` with `border-input` token; focus ring provides emphasis.
- Shadows:
  - Signature “paper” shadow: crisp offset black, e.g., `shadow-[6px_6px_0_0_rgba(0,0,0,1)]` or `8px` variant.
  - Shadows are decorative emphasis on interactive surfaces (cards, nav) rather than soft blurs.
- Layout:
  - Section scaffold: `container mx-auto px-4 py-16 md:py-24`, content constrained to `max-w-7xl`.
  - Grid: 1–2 columns on small/medium; 3+ on large for dense content. Maintain generous gaps.
- Component Behavior:
  - Buttons: shadcn + CVA variants. Primary is filled dark on light; outline variant uses black border on white; ghost only for subtle, low-risk actions.
  - Inputs: use focus-visible ring (`ring-[3px] ring-ring/50`) and `aria-invalid` red ring/border.
  - Pills/Tags: small, bold, often on black or accent chip; `rounded-full`, tight padding.
- State Styling:
  - Hover: subtle color/translate deltas; never remove the black outline.
  - Focus-visible: ring + maintain border (do not swap to outline-only).
  - Active/pressed: small inward translation; keep legibility.
  - Disabled: lower opacity and disable pointer events.
  - Validation: `aria-invalid` applies red ring/border using tokens; messages sit beneath fields with consistent spacing.
- Responsiveness:
  - Always define responsive typography and spacing (`md:` and `lg:` steps).
  - Collapse multi-column layouts to single column; action areas remain visible and tappable.

## Layout and Page Composition Rules
- Page shell:
  - Top-level: `min-h-screen`, light background by default.
  - Content container: `container mx-auto px-4`, vertical rhythm via `py-*`.
  - Primary header region: page title (H1) + primary actions on the right; secondary actions grouped.
- Grids and grouping:
  - Use cards for discrete information units; group related cards in 2–3 column grids on desktop.
  - Maintain consistent card padding (`p-6`/`p-8`), border weight, and shadow style per page.
- Visual emphasis:
  - Use accent chip backgrounds to highlight small in-line phrases, tags, or hero keywords.
  - Avoid large accent-color fills for whole pages; the base canvas remains neutral.

## Component Rules
- Dashboards:
  - Header: Title + date/filter + primary action button (filled dark).
  - Content: Analytics cards in 2–3 columns; cards use black border (3–4 px), white surface, offset black shadow.
  - Quick insights: small stacked KPI blocks; consistent number formatting and labels.
- Settings Pages:
  - Left: simple section nav (list or tabs). Right: content panel.
  - Form groups in white cards with black border; save/cancel in a sticky footer or header within the card.
  - Use help text under fields, not tooltips, for persistent guidance.
- CRUD Pages:
  - Index/List: Toolbar (search, filters, create) above a table or card list.
  - Create/Edit: One column form; multi-step only when necessary. Confirmation uses inline toast or success alert card.
  - Read/Details: Summary card(s) at top; metadata in two columns; actions grouped in a sticky area.
- Forms:
  - Inputs: `h-9`/`h-10`, rounded-md; labels always visible; required `*`.
  - Validation: on blur and submit; show concise messages beneath fields; never use only color to indicate error.
  - Primary submit is filled dark; secondary is outline.
- Tables:
  - Container card with black border and subtle offset shadow.
  - Header row bold; zebra striping optional; row hover uses light neutral background, not color fills.
  - Sort icons aligned right in header cells; pagination persists at bottom with clear size and spacing.
- Analytics Blocks:
  - Use Recharts; legend/text in foreground color; axis/grid light neutral.
  - Respect chart tokens; if color needed, use approved accent chips in small amounts for series.
  - Cards include concise title, trend pill (+/−), and last updated timestamp.
- Dialogs:
  - Radix Dialog primitives; surface: white with black border (3 px), friendly radius (`rounded-xl`), and slight offset shadow.
  - Overlay: semi-opaque dark (`bg-black/50`); trap focus; close via ESC and explicit buttons.
- Navigation:
  - Top nav: white bar with black border/shadow; center-aligned links on desktop; condensed on mobile.
  - Active link uses bold text/underline; CTA button uses filled dark or “chip” accent sparingly.
- Cards:
  - Always `bg-white border-[3px] border-black rounded-3xl` (or `[32px]` where featured) with offset black shadow.
  - Inside: strong title, medium description (`text-[#393939]`), and a clear action link/button.
- Empty States:
  - Centered icon/illustration; short headline; one supportive sentence; primary action button.
  - Avoid decorative overload; keep the paper aesthetic via border/shadow, not color floods.
- Alerts:
  - Inline card with black border; use small colored chip for state: info (blue), warning (yellow), error (destructive red).
  - Include title, brief message, and clear dismiss/action area.

## UX Behavior Rules
- Focus management: On open (dialogs/sheets), focus the first actionable element. Restore focus on close.
- Keyboard: Tab order follows visual order; all interactive components keyboard-operable.
- Feedback: Use toasts or inline confirmations; destructive actions require confirmation.
- Performance: Progressive rendering for large tables/lists; skeletons instead of spinners when possible.
- Copy: Short, action-oriented labels; sentence case; avoid jargon; keep body text ~60–80 chars per line.

## Constraints (Never Do)
- Do not introduce new color families beyond tokens and sanctioned accent chips.
- Do not break spacing rhythm (stick to multiples of 4; reuse established paddings/gaps).
- Do not create conflicting hierarchy (multiple primary actions or multiple H1s).
- Do not add decorative flourishes that don’t support comprehension or action.
- Do not overcomplicate interactions (avoid unnecessary wizards, nested modals, or hidden actions).
- Do not invent component patterns not supported by existing primitives (stay within buttons, inputs, cards, tables, dialogs, tabs, etc. using Radix + shadcn-style structure).

## Anti-Drift Rules
- Token-first: Always reference design tokens (color, radius, ring, input, border). If a value is not in tokens, prefer the closest existing token or skip.
- Outline and shadow: Surfaces keep black border (3–4 px) and the signature offset shadow; never replace with soft box-shadows.
- Typography guardrails: Onest only; size within the documented ranges; headings remain bold; body remains 16–18 px.
- Accent restraint: Accent chips are localized highlights (inline words, small tags, tiny badges). Never apply as page-wide backgrounds or large sections.
- Component reuse: Start from existing button/input patterns (CVA variants, focus-visible ring, aria-invalid). Extend variants only when necessary and consistent.
- Review checklist before finalizing:
  - Borders match weight and color
  - Radii consistent with surface size
  - Focus-visible present on all interactive elements
  - Spacing follows 4px multiples and section rhythm
  - Dark mode respects tokens
  - No raw arbitrary colors except the approved chip accents

## Final Operating Instructions
- When generating screens:
  - Start with page shell: `container mx-auto px-4`, `py-16` (or `py-24`), `max-w-7xl`.
  - Define a clear H1 and a single primary action; group secondary actions.
  - Compose content with white cards with black borders and offset shadows; choose `rounded-xl` or `rounded-3xl/[32px]` based on prominence.
  - Apply typography and spacing per the rules; ensure responsive steps with `md:` and `lg:`.
  - Use existing button/input patterns (focus-visible rings, states). Prefer outline buttons for secondary actions.
  - For data: pick tables or card grids; use the same card/container styling, pagination, and sort affordances.
  - For analytics: place in card modules with concise titles and optional trend chips; use approved series colors sparingly.
- When generating components:
  - Define variants and sizes with CVA-like structure; align with existing `button` and `input` patterns.
  - Provide full interaction states (hover, focus-visible, active, disabled, invalid).
  - Include accessibility attributes/labels and keyboard semantics (Radix primitives where applicable).
- Always justify key layout choices in your response using:
  - Clarity (why this structure), Hierarchy (how prominence is conveyed), Consistency (which tokens/patterns), Task Completion (how it accelerates the goal), Accessibility (focus/contrast/labels), Scalability (how it adapts to more data).

By following this skill, every new dashboard, settings area, CRUD flow, or marketing-to-product bridge will look and behave like it shipped with the app from day one—bold, clear, accessible, and unmistakably “Paperfolio X.”

# Structured Style Profile

```json
{
  "style_name": "shadcn new-york (with custom Paperfolio styling)",
  "visual_identity": {
    "tone": "bold, high-contrast, playful (inferred)",
    "density": "spacious; large paddings and generous whitespace",
    "corner_style": "rounded; base radius 1rem with large radii (e.g., 32px, full)",
    "elevation_style": "hard offset drop-shadows (e.g., 8px_8px_0 rgba(0,0,0,1)); minimal soft blur",
    "contrast_profile": "very high contrast (black/white) with bright accent blocks",
    "mood": "neo‑brutalist, friendly, editorial (inferred)",
    "notes": [
      "Tokens sourced from app/globals.css; layout imports this file.",
      "Multiple ad‑hoc accent colors used in components (e.g., #FF6B7A, #2F81F7, #FFC224, #6366F1, #FDB927).",
      "components.json declares style \"new-york\"; implementation looks more neo‑brutalist than stock preset."
    ]
  },
  "tokens": {
    "colors": {
      "primary": "#0a0a0a",
      "secondary": "#f5f5f5",
      "accent": "#f5f5f5",
      "neutral": [
        "#ffffff",
        "#fafafa",
        "#f5f5f5",
        "#e5e5e5",
        "#a1a1a1",
        "#717171",
        "#525252",
        "#404040",
        "#383838",
        "#262626",
        "#171717",
        "#0a0a0a"
      ],
      "success": "unknown",
      "warning": "unknown",
      "danger": "#e7000b",
      "background": "#ffffff",
      "surface": "#ffffff",
      "text": {
        "primary": "#0a0a0a",
        "secondary": "#171717",
        "muted": "#717171",
        "inverse": "#fafafa"
      },
      "border": "#0a0a0a"
    },
    "spacing": [
      "0.75rem",
      "1rem",
      "1.25rem",
      "1.5rem",
      "1.75rem",
      "2rem",
      "3rem",
      "4rem",
      "6rem",
      "8rem"
    ],
    "radius": [
      "var(--radius)=1rem",
      "radius-sm=calc(var(--radius)-4px)",
      "radius-md=calc(var(--radius)-2px)",
      "radius-lg=var(--radius)",
      "radius-xl=calc(var(--radius)+4px)",
      "rounded-xl",
      "rounded-3xl",
      "rounded-full",
      "rounded-[10px]",
      "rounded-[12px]",
      "rounded-[16px]",
      "rounded-[29px]",
      "rounded-[32px]"
    ],
    "shadows": [
      "shadow-xs",
      "shadow-[4px_4px_0px_0px_rgba(0,0,0,1)]",
      "shadow-[6px_6px_0px_0px_rgba(0,0,0,1)]",
      "shadow-[8px_8px_0px_0px_rgba(0,0,0,1)]",
      "shadow-[-8px_8px_0px_0px_rgba(0,0,0,1)]"
    ],
    "typography": {
      "font_families": [
        "Onest",
        "JetBrains Mono"
      ],
      "scale": [
        "text-sm",
        "text-base",
        "text-lg",
        "text-xl",
        "text-2xl",
        "text-3xl",
        "text-4xl",
        "text-5xl",
        "text-6xl",
        "16px",
        "18px",
        "20px",
        "22px",
        "28px",
        "42px",
        "52px",
        "72px"
      ],
      "font_weights": [
        500,
        600,
        700
      ],
      "line_heights": [
        "leading-tight",
        "leading-relaxed",
        "20px",
        "28px",
        "30px",
        "32px",
        "34px",
        "40px",
        "50px",
        "60px",
        "85px",
        "1.3"
      ]
    },
    "widths": [
      "max-w-7xl",
      "max-w-5xl",
      "max-w-2xl",
      "max-w-md",
      "max-w-lg",
      "min-w-[200px]",
      "min-w-[240px]",
      "min-w-[400px]",
      "min-w-[480px]"
    ],
    "breakpoints": [
      "sm",
      "md",
      "lg"
    ]
  },
  "layout": {
    "page_shell": "Landing page with stacked sections inside centered container",
    "page_width_strategy": "container mx-auto with max-w-7xl and section paddings",
    "header_pattern": "Top navigation bar centered; thick black border, rounded, offset shadow; right-aligned icon CTA",
    "section_spacing": "Vertical rhythm ~py-16 base, md:py-24/32",
    "grid_rules": [
      "grid md:grid-cols-2",
      "md:grid-cols-[0.9fr_1.1fr]",
      "lg:grid-cols-3"
    ],
    "navigation_patterns": [
      "Inline link group centered on md+",
      "Primary icon CTA at right",
      "Hidden link group on small screens (no alt menu present)"
    ],
    "responsive_rules": [
      "Typography scales up at md",
      "Single column → two columns at md",
      "Buttons widen on small screens (min-w constraints on sm+)"
    ]
  },
  "components": {
    "buttons": {
      "variants": [
        "default",
        "destructive",
        "outline",
        "secondary",
        "ghost",
        "link"
      ],
      "sizes": [
        "default (h-9, px-4)",
        "sm (h-8, px-3)",
        "lg (h-10, px-6)",
        "icon (size-9)",
        "icon-sm (size-8)",
        "icon-lg (size-10)"
      ],
      "focus": "focus-visible:border-ring + ring-[3px] using --ring token",
      "shape": "rounded-md by default; sections use larger custom radii",
      "notes": [
        "Primary treatment often overrides to solid black with white text.",
        "Outline variant uses 3–4px black borders in sections."
      ]
    },
    "inputs": {
      "field_height": "h-9 default; newsletter uses h-14/h-16",
      "style": "border-input, bg-transparent, rounded-md, text-base, shadow-xs",
      "focus": "focus-visible:border-ring + ring-[3px] (--ring)",
      "validation": "aria-invalid adds red destructive ring and border",
      "states": [
        "disabled: opacity-50 and no pointer events"
      ]
    },
    "selects": {},
    "dropdowns": {},
    "cards": {
      "style": "white surface, black border [3px–4px], large radius (≈32px), hard offset shadows on hover",
      "content_patterns": [
        "media top with rounded inner corners",
        "title + description + link/CTA"
      ]
    },
    "tables": {},
    "modals": {},
    "dialogs": {},
    "sidebars": {},
    "tabs": {},
    "badges": {
      "style": "rounded-full, text-xs, px-4 py-1.5",
      "variants": [
        "black bg with white text (portfolio tag)"
      ]
    },
    "alerts": {},
    "empty_states": {},
    "charts_containers": {},
    "page_headers": {
      "hero": "Large headline with colored highlight chips; split 2-col at md; illustrated card with offset shadow"
    },
    "filters": {},
    "form_layouts": {
      "newsletter": "Inline input with absolute CTA button inside bordered rounded container"
    }
  },
  "ux_patterns": {
    "cta_hierarchy": "Primary: solid black on white; Secondary: white with 3–4px black border; Icon CTA in nav",
    "information_grouping": "Large bordered cards with clear media/title/description blocks",
    "filter_placement": "none observed",
    "form_structure": "Simple single-field forms; prominent CTA; inline in footer",
    "validation_behavior": "ARIA-invalid triggers destructive ring/border on inputs",
    "table_detail_strategy": "not present",
    "loading_error_empty_states": "not present",
    "action_placement": "Section-level CTAs at ends; global CTA in header right",
    "notes": [
      "Bright color highlight chips used to emphasize words within headings.",
      "Hover scales images inside cards; cards lift with offset shadow."
    ]
  },
  "constraints": [
    "Success and warning colors are not defined in app/globals.css.",
    "Spacing scale is not explicitly customized; Tailwind defaults implied.",
    "Accent brand colors are applied ad‑hoc in components, not tokenized.",
    "Two global styles exist; only app/globals.css is imported by layout."
  ]
}

```

# Reference Files

- `input/repo-summary.md`
- `input/repo-file-map.txt`
- `input/relevant-files.md`
- `input/design-extraction-schema.json`
- `outputs/01-ui-ux-foundation.md`
- `outputs/02-design-extraction.md`
- `outputs/02-design-extraction.json`
- `outputs/03-final-skill.md`

# Operating Notes

- Reuse existing component conventions before proposing new ones.
- When a screen is not directly represented in the current codebase, extrapolate conservatively from similar patterns.
- Keep spacing, radius, shadow, typography, and interaction rules aligned with the extracted system.