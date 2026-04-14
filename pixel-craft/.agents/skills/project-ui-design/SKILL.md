---
name: Project UI Design
description: Generate UI consistent with the existing product style, structure, and UX rules.
---

# Usage

Use this skill whenever you need to generate new UI, pages, components, flows, or product screens consistent with the existing application style.

Priority rules:
1. Preserve the source design identity at the level of geometry, spacing character, hierarchy, typography roles, and interaction tone.
2. Extend the current patterns conservatively.
3. Adapt to the functional context without drifting into a generic style family.
4. Prefer clarity, consistency, and product readiness over novelty.
5. When explicit patterns are missing, infer conservatively from the source design language.

# Project Summary

# Repository Summary

- Root: `/Users/emanueledagata/code/v0/boh1`
- Detected hints: Next.js, Tailwind CSS
- Total indexed files: 30
- Relevant UI/design files: 27

## Key dependencies

- next: 15.1.9
- react: ^19.0.0
- react-dom: ^19.0.0
- tailwindcss: ^4.0.0

## Key analysis goals

- Extract the source design language from the repository.
- Identify explicit and inferred design-system rules.
- Preserve radius, spacing character, hierarchy, typography roles, and interaction tone.
- Produce a reusable design skill for generating new UI categories consistently.
- Prevent style drift when adapting to dashboards, forms, CRUD, or utility-heavy interfaces.


# Final Design Skill

# PixelCraft UI Design Skill

## Purpose

Use this skill to generate new UI screens, components, product flows, and interface states that feel native to the existing PixelCraft application.

The goal is not to copy existing sections literally. The goal is to preserve the application’s design logic: dark industrial surfaces, squared geometry, strict spacing, high-contrast yellow emphasis, restrained orange accents, border-led structure, terminal-like metadata, and bold product hierarchy.

## AI Role

Act as a product UI/UX designer and interface system builder.

You are responsible for producing professional, production-ready software interfaces that are coherent with the source product’s current visual language, geometry, hierarchy, spacing character, typography roles, interaction tone, and component behavior.

You must think like both a designer and a system maintainer: every new screen should look like it belongs to the same product, and every new component should be reusable without weakening the design language.

## Design Philosophy

PixelCraft uses an industrial, dark-first, precision-oriented interface language. It feels like a design system, code editor, production console, and product marketing surface merged into one coherent system.

The visual identity is defined by:

- Dark layered surfaces: `#050505`, `#080808`, `#0A0A0A`, `#0D0D0D`, `#0F0F0F`, `#111111`, `#1A1A1A`
- Bright yellow primary emphasis: `#FFD600`
- Orange secondary accent: `#FF6B35`
- Off-white primary text: `#F5F5F0`
- Muted gray support text: `#888888`, `#666666`, `#555555`, `#444444`
- Thin technical borders: `#1D1D1D`, `#2D2D2D`, `#3D3D3D`
- Mostly square geometry with almost no radius
- Tight internal component gutters, large page-level spacing, and explicit grid rhythm
- Bold uppercase headlines paired with small mono labels, indexes, tags, and system copy
- Functional motion and state feedback rather than decorative animation

The UX should prioritize clarity, visual priority, fast scanning, obvious interaction affordances, and consistent system behavior.

## Non-Negotiable Style Traits

### Radius And Geometry Family

Use square, rectilinear geometry as the default.

- Default radius: `0px`
- Component frames, cards, buttons, tables, panels, dialogs, alerts, filters, and form fields should be square.
- Use `1px` or `2px` radius only for tiny technical SVG/editor details if unavoidable.
- Use fully rounded shapes only for avatars, cursor dots, status dots, or intentionally circular indicators.
- Do not introduce soft cards, rounded pills, floating blobs, or generic SaaS radius unless the source identity explicitly evolves.

### Spacing Character

Preserve the spacious-but-mechanical rhythm.

- Page sections use large vertical padding: mobile around `64px`, desktop around `80px` to `120px`.
- Desktop horizontal section padding commonly uses `120px`.
- Mobile horizontal padding commonly uses `24px`.
- Component interiors commonly use `32px` or `40px`.
- Repeated card grids use very tight `2px` gutters to create an industrial tiled system.
- Use a 4px base grid. Prefer spacing values divisible by 4.

### Emphasis Discipline

Only a few things may be loud at once.

- Yellow is the main emphasis color and should identify primary actions, active states, selected sections, key metrics, and featured cards.
- Orange is secondary and should mark warnings, AI/open/advanced states, special accents, or alternate highlights.
- Most supporting content stays muted gray.
- Do not make every border, icon, and label yellow. Preserve contrast by keeping most UI quiet.

### Hierarchy Style

Hierarchy is built through scale, weight, color, borders, and spatial separation.

- Large headlines carry the primary story.
- Mono labels establish section, state, metadata, sequence, and controls.
- Borders define structure instead of shadows.
- Selected or primary regions get stronger borders, yellow fills, or yellow text.
- Secondary content remains muted and compact.

### Typography Roles

Use typography as a UX system, not decoration.

- `Space Grotesk` is for headings, brand marks, large numbers, primary buttons, strong card titles, and structural labels.
- `IBM Plex Mono` is for metadata, subtitles, descriptions, navigation, form hints, table data, badges, technical copy, tags, and secondary controls.
- Copy is commonly uppercase, concise, and technical.
- Large headings use tight line-height and slight negative tracking.
- Metadata uses small sizes, uppercase, letter spacing, and restrained color.

### Interaction Tone

Interactions should feel precise, fast, technical, and predictable.

- Use color shifts, border changes, underline growth, active indicators, simple disclosure, and direct state changes.
- Avoid playful springiness, excessive easing, floating hover effects, or ornamental motion.
- Motion should clarify state or navigation, not decorate.

## Core UI/UX Principles

- Clarity: every screen needs one obvious primary task and one dominant visual focus.
- Hierarchy: guide the eye from section label to title to primary action to supporting data.
- Visual priority: high emphasis belongs only to the most important action, active state, selected item, or metric.
- Consistency: reuse spacing, color roles, typography roles, border weights, and control shapes.
- Task completion: prioritize direct paths, visible actions, clear feedback, and minimal decision overhead.
- Accessibility: preserve contrast, keyboard focus, readable type sizes, and non-color-only state communication.
- Scalability: components must handle longer labels, empty states, loading states, errors, and responsive layouts.
- Progressive disclosure: reveal advanced detail only when it helps completion.

## Project-Specific Style Rules

### Color Usage Rules

Use the project palette with explicit roles:

- Page background: `#050505`, `#080808`, `#0A0A0A`
- Section variation: `#0D0D0D`, `#0F0F0F`
- Card and panel surfaces: `#0A0A0A`, `#0F0F0F`, `#111111`
- Raised or active technical surface: `#1A1A1A`
- Primary action and active state: `#FFD600`
- Secondary accent: `#FF6B35`
- Primary text: `#F5F5F0`
- Secondary readable text: `#CCCCCC`, `#AAAAAA`, `#888888`
- Muted metadata: `#666666`, `#555555`, `#444444`
- Disabled text or inactive marks: `#333333`, `#3D3D3D`
- Borders: `#1D1D1D`, `#2D2D2D`, `#3D3D3D`

Never use soft pastel palettes, gradients, translucent glass cards, beige themes, blue-purple SaaS gradients, or decorative color systems unrelated to the source identity.

### Typography Rules

- Use bold `Space Grotesk` for primary headings and strong product terms.
- Use `IBM Plex Mono` for descriptions, labels, status, navigation, table cells, badges, and helper copy.
- Prefer uppercase copy for UI labels and marketing-style product copy.
- Use short, scannable phrases.
- Maintain strong contrast between heading scale and body scale.
- Common heading sizes:
  - Hero: `clamp(32px, 10vw, 96px)`, line-height `1`
  - Section title: `36px` mobile, `56px` desktop, line-height around `1.05`
  - Card title: `18px` to `28px`, line-height `1.1` to `1.2`
  - Metrics: `40px` to `64px`
- Common mono sizes:
  - Labels and badges: `9px` to `12px`
  - Descriptions: `11px` to `13px`
  - Hero/support copy: `13px` to `15px`
- Letter spacing is part of the identity: use `1px` to `3px` for mono labels and small uppercase controls.

### Spacing Rules

- Use a 4px grid.
- Use tight repeated gutters: `2px` between tiled cards, comparison rows, bento blocks, and dense component groups.
- Use `16px`, `20px`, `24px`, `32px`, `40px`, `48px`, `64px`, `80px`, `100px`, `120px` as primary spacing values.
- Page sections should feel spacious, not cramped.
- Internal component spacing should feel mechanical and deliberate.
- Do not collapse generous marketing spacing into generic dense admin spacing when adapting to dashboards or utility screens.

### Radius Rules

- Default all containers and controls to square corners.
- Buttons, cards, dialogs, filters, inputs, table wrappers, alerts, and panels should use `0px` radius.
- Keep geometry sharp and modular.
- Only use roundness for semantic dots, avatars, cursors, and tiny indicators.

### Shadow And Elevation Rules

- Do not rely on shadows for hierarchy.
- Use borders, surface contrast, yellow/orange accent borders, and layout position instead.
- If depth is necessary, use subtle surface layering rather than drop shadows.
- Avoid soft floating panels.

### Hierarchy Rules

- Start major screens with a mono section label or contextual system label.
- Pair labels with large bold headings or compact page titles.
- Use yellow for the current section, active selection, primary CTA, featured metric, or dominant state.
- Use borders and surface contrast to group content.
- Use muted gray text for secondary detail.
- Use numbered markers like `[01]`, `01`, `01 / 04`, or bracketed tags when sequencing matters.

### Visual Priority Rules

- Each screen should have one primary action.
- Secondary actions should use dark backgrounds with gray or accent borders.
- Danger, warning, or special states may use orange, but sparingly.
- Tables and dashboards should highlight the active product/entity column or key result in yellow.
- Empty and loading states should remain quiet unless an action is required.

### Interaction State Rules

- Hover:
  - Primary yellow buttons may shift to `#e6c200` or `#F5F5F0`.
  - Secondary buttons should usually strengthen border color from `#3D3D3D` to `#888888`.
  - Links may move from muted gray to off-white or yellow.
- Active/selected:
  - Use yellow text, yellow border, yellow fill, or a small yellow indicator.
  - Keep active indicators geometric: underlines, left bars, square dots, or top borders.
- Focus:
  - Provide clear keyboard focus with yellow outline, yellow border, or high-contrast ring.
- Disabled:
  - Use `#333333` or `#3D3D3D` text/border, with no hover emphasis.
- Loading:
  - Use terminal-style indicators, skeleton rows, scanline-style progress, or compact mono status text.
- Error:
  - Use orange or a clear high-contrast error treatment with concise mono explanation.
- Success:
  - Prefer yellow or restrained green only if the app already uses it for live/system status.

## Visual Priority And Hierarchy Rules

For every generated screen, define the hierarchy before placing components:

1. Primary task: what the user came to do.
2. Primary object: project, component, workflow, account, metric, dataset, or setting.
3. Primary action: the one action that advances the task.
4. Secondary actions: navigation, filtering, export, edit, duplicate, archive, or details.
5. Supporting metadata: status, timestamps, counts, plan limits, technical labels, IDs.

Translate that hierarchy into the PixelCraft visual language:

- Primary task gets a strong title and enough space.
- Primary action gets yellow fill.
- Secondary actions get dark fill and border.
- Metadata gets mono type and muted color.
- Structural groups get borders, not shadows.
- Dense data gets table/grid structure with strong separators.

## Typography As UX Rules

Use typography to control reading order.

- Use `Space Grotesk` when the text should be seen first.
- Use `IBM Plex Mono` when the text should be scanned, compared, or treated as system data.
- Use uppercase for controls, labels, tags, and concise product statements.
- Do not make long paragraphs fully dominant. Keep prose short and structured.
- For long-form settings or help content, use mono sparingly for metadata and use readable spacing to avoid fatigue.
- Maintain line-height around `1.5` to `1.6` for supporting copy.
- Use negative tracking only on large bold headings or numbers.

## Interaction Rules

Generate interactions that are direct and low-friction.

- Navigation should clearly show current location through yellow text, underline, left bar, or square indicator.
- Disclosure controls should use square plus/minus buttons or border-based toggles.
- Carousels and paginated areas should use square controls and simple position indicators.
- Filters should feel like technical controls: bordered groups, compact mono labels, square chips, clear selected states.
- Form validation should appear near the field, use concise mono text, and include visible border/state changes.
- Destructive actions require confirmation through a dialog or inline confirmation when risk is meaningful.
- Avoid hidden gestures, novelty interactions, decorative cursor effects in utility screens, and animation that slows completion.

## Layout And Page Composition Rules

- Use full-width dark page sections or app surfaces.
- Keep main content aligned to a clear grid.
- Use `24px` mobile side padding and around `120px` desktop side padding for page-like compositions.
- For app dashboards, use a fixed or collapsible square-edged sidebar/topbar if useful, but preserve the same typography, border, and color logic.
- Use tight `2px` gaps for tiled modules when the screen should feel systematic.
- Use larger gaps like `48px` to `64px` between major screen regions.
- Prefer simple flex/grid structures with explicit widths, stable heights, and predictable breakpoints.
- On mobile, stack columns vertically and keep controls full-width when needed.
- Tables may transform into compact card rows or simplified grids on mobile.
- Do not place the primary product experience inside decorative outer cards unless the frame is functional.

## Component Rules

### Dashboards

Create dashboards as dark, border-defined systems.

- Use a strong page header with mono context label, title, primary action, and optional metadata.
- Use metric tiles with large `Space Grotesk` numbers and mono labels.
- Use yellow for the most important metric or selected time range.
- Use tiled cards with `2px` gaps or bordered panels with `32px` to `40px` padding.
- Use charts with restrained colors: yellow primary series, orange secondary series, muted gray gridlines.
- Avoid generic soft analytics cards with shadows.

### Settings Pages

Settings should feel precise and structured.

- Use section groups with top borders or square bordered panels.
- Use mono labels for setting names, descriptions, state, and technical metadata.
- Use clear save/cancel hierarchy: yellow primary save, dark bordered cancel.
- Use segmented navigation, sidebar groups, or tabs with yellow active states.
- Keep forms spacious and readable.

### CRUD Pages

CRUD flows should be task-first.

- List views use strong headers, filters, table/list body, and clear primary create action.
- Detail views use bordered sections, metadata rows, and direct edit/archive/delete actions.
- Create/edit pages use stacked forms with clear section labels.
- Use dialogs only for quick, bounded actions. Use dedicated pages for complex editing.

### Forms

- Inputs should be square, dark, bordered, and aligned to the grid.
- Labels use mono uppercase or compact system case.
- Field height should commonly be `48px` to `56px`.
- Use `#1A1A1A` or `#0F0F0F` backgrounds with `#2D2D2D` or `#3D3D3D` borders.
- Focus state should visibly shift to yellow.
- Validation text should be concise and placed directly beneath the field.
- Group related fields with spacing and borders, not decorative cards.

### Tables

- Tables should be technical, high-scan, and border-led.
- Header rows use `#111111` or `#1A1A1A`.
- Important headers or active columns may use yellow bottom borders.
- Row height commonly around `56px`.
- Cells use mono text for data and `Space Grotesk` for strong labels only when necessary.
- Use alternating subtle dark surfaces only when it improves scanability.
- Keep empty, loading, selected, and error row states explicit.

### Analytics Blocks

- Use large numeric hierarchy with muted mono labels.
- Use yellow for primary values, orange for exceptional secondary signals.
- Pair metrics with small trend, period, or status metadata.
- Keep visualizations minimal, bordered, and dark.
- Avoid colorful chart palettes that weaken the identity.

### Dialogs

- Dialogs are square, dark, bordered panels.
- Use a strong title, compact mono description, and clear action row.
- Use yellow primary action, dark bordered secondary action.
- For destructive confirmations, use orange border/text and require explicit confirmation when risk is high.
- Avoid rounded modal shells and shadow-heavy overlays.

### Navigation

- Use uppercase mono nav labels.
- Active nav uses yellow text, underline, left bar, square dot, or yellow border.
- Desktop nav can be horizontal or sidebar depending on product area.
- Mobile nav should collapse into a square-edged drawer with dark surface and border separators.
- Keep navigation concise and stable.

### Cards

- Cards are square modules with dark surfaces and `1px` or `2px` borders.
- Use `32px` or `40px` padding for substantial cards.
- Use `2px` gaps for tiled systems.
- Use yellow border/fill only for featured or selected cards.
- Do not use soft rounded cards or shadow cards.

### Empty States

- Empty states should be direct and useful.
- Use a mono bracketed label like `[EMPTY]`, `[NO RESULTS]`, or `[NO PROJECTS]`.
- Use a clear title, short explanation, and one primary action when possible.
- Use a bordered dark panel or table body region.
- Avoid illustrations unless they are geometric, functional, and aligned with the technical identity.

### Alerts

- Alerts should be square, concise, and border-led.
- Info/default: dark surface with gray border.
- Important/active: yellow border or yellow label.
- Warning/error: orange border or orange label.
- Success: restrained yellow or green only when semantically appropriate.
- Include clear action when the alert requires user response.

### Filters

- Filters should behave like technical controls.
- Use compact mono labels, square chips, bordered selects, and dark inputs.
- Selected filters use yellow text, yellow border, or yellow fill with dark text.
- Keep filter groups aligned with the table/list they control.
- Provide clear reset behavior using a muted secondary action.

## Derived Component Rules

When generating components that do not exist in the original repository, derive them conservatively from the existing system.

Use this derivation process:

1. Identify the closest existing pattern:
   - Cards from feature, bento, pricing, testimonial, and showcase modules.
   - Tables from comparison rows.
   - Navigation from navbar and mobile drawer.
   - Disclosure from FAQ.
   - Metrics from stats.
   - Actions from hero, final CTA, carousel controls, and pricing buttons.
2. Preserve the same design primitives:
   - Square geometry
   - Dark surfaces
   - Thin borders
   - Yellow primary emphasis
   - Orange secondary emphasis
   - Mono metadata
   - Bold grotesk titles
   - 4px grid
   - Spacious page rhythm
3. Adapt function before aesthetics:
   - A dashboard is not a landing page, but it should still use the same geometry, typography roles, surface layering, and emphasis discipline.
   - A settings screen should be calmer than a hero, but still recognizably PixelCraft.
   - A table should be denser than a marketing section, but not generic or cramped.
4. Extend the system using existing logic:
   - New status chips should look like existing tags.
   - New panels should look like bento/pricing cards.
   - New data rows should look like comparison rows.
   - New buttons should follow CTA and carousel button rules.
   - New sidebars should follow navbar typography and active indicators.

Do not invent a different visual family to solve a new UI category.

## Constraints

Never:

- Introduce rounded SaaS geometry into this square source language.
- Flatten the spacious spacing character into a cramped generic admin layout.
- Break the 4px spacing rhythm or the `2px` tiled-gutter pattern where modules repeat.
- Create inconsistent hierarchy where every element competes equally.
- Use decorative elements without functional value.
- Add gradients, floating blobs, bokeh, glassmorphism, soft shadows, or ornamental illustrations.
- Overcomplicate interactions with unnecessary animation or hidden behavior.
- Invent unsupported component patterns without grounding them in the source identity.
- Use yellow everywhere.
- Replace mono metadata with generic body text styling.
- Use shadows as the primary grouping mechanism.
- Make primary and secondary actions visually equal.
- Create screens that look like a different product category template.

## Anti-Drift Rules

To avoid style drift over time:

- Start every new screen by restating the source identity: dark industrial, square, border-led, mono metadata, bold grotesk hierarchy, yellow primary emphasis.
- Reuse existing token roles before adding new colors.
- Reuse existing spacing values before adding new spacing.
- Reuse existing typography roles before inventing new type treatments.
- Reuse existing interaction states before adding new behavior.
- Compare every new component against at least one source-derived pattern.
- If a new component feels too soft, rounded, pastel, shadowed, generic, or decorative, revise it toward the PixelCraft system.
- Keep dashboards and utility screens less theatrical than the landing page, but not visually neutralized.
- Keep marketing screens more expressive than utility screens, but still governed by the same geometry and emphasis discipline.
- Prefer conservative extension over novelty.
- Do not let one-off components introduce new radii, shadows, color roles, or typography roles.

## Conservative Adaptation Rule

A portfolio, marketing page, or landing-page design language may be adapted into dashboards, CRUD tools, settings pages, admin flows, and utility screens.

When adapting PixelCraft into those categories, preserve the defining traits:

- Square geometry
- Dark layered surfaces
- Border-led structure
- Spacious page rhythm
- Tight tiled module gutters
- Yellow primary emphasis
- Orange secondary accent
- Bold grotesk titles
- Mono metadata and system copy
- Clear visual priority
- Direct, technical interaction tone

The new screen does not need to look like a marketing page, but it must still be recognizably PixelCraft.

## Final Operating Instructions

When generating UI for this project:

1. Produce product-ready interface designs, not abstract style descriptions.
2. Reuse existing patterns wherever possible.
3. Extend the system conservatively when a needed component does not exist.
4. Preserve the source design identity across every UI category.
5. Make hierarchy, visual priority, and task completion explicit.
6. Use typography, spacing, color, borders, and interaction states with discipline.
7. Justify key design decisions through clarity, hierarchy, visual priority, consistency, task completion, accessibility, and scalability.
8. Ensure every generated component feels native to the existing PixelCraft design language.

# Structured Style Profile

```json
{
  "style_name": "Industrial Pixel Terminal",
  "visual_identity": {
    "tone": "technical, industrial, builder-focused, direct, all-caps product language",
    "density": "high information density with compact labels, tight control copy, large section rhythm, and dense component grids",
    "corner_style": "predominantly square and rectilinear; most UI surfaces and controls use 0px radius, with rare circular dots/avatars only",
    "elevation_style": "flat layered surfaces separated by hard borders, 2px seams, color bands, and occasional accent rails; shadows are essentially absent except cursor effects",
    "contrast_profile": "dark-first high contrast: near-black backgrounds, off-white primary text, muted gray metadata, bright yellow primary emphasis, orange secondary accent",
    "mood": "precision tool, terminal/editor inspired, pixel-grid, unapologetically mechanical",
    "notes": [
      "Evidence: app/globals.css defines yellow, orange, near-black background, off-white text, muted grays, and border tokens.",
      "Evidence: components use repeated bg-[#0A0A0A]/[#0D0D0D]/[#111111], border-[#2D2D2D], and bright #FFD600 accents.",
      "Evidence: Navbar, Hero, Features, Bento, Comparison, Pricing, FAQ, Showcase, and FinalCTA use uppercase labels, bracket syntax, monospace metadata, and square controls."
    ]
  },
  "identity_traits": {
    "non_negotiable_traits": [
      "Dark-first base with near-black page shell and section bands.",
      "Primary accent is #FFD600 yellow; use it for active state, primary CTA, key borders, stats bands, and selected emphasis.",
      "Use hard rectangular geometry: default radius 0px and border-driven separation.",
      "Use Space Grotesk for bold display/product headings and IBM Plex Mono for labels, metadata, body support, nav, and data rows.",
      "Preserve all-caps technical copy, bracketed labels, slash separators, and short declarative phrases.",
      "Use dense 2px seams between repeated cards, grids, pricing tiers, and comparison rows."
    ],
    "adaptable_traits": [
      "Secondary orange #FF6B35 can mark special capabilities, enterprise actions, or secondary accents.",
      "Green #4ADE80 and blue #60A5FA appear mainly in the hero/editor visual and cursor affordances; use sparingly for system/status detail.",
      "Section background can alternate among #050505, #060606, #080808, #0A0A0A, #0D0D0D, #0F0F0F, and #111111 to create depth without shadow.",
      "Animations may use quick color transitions, smooth scroll, typewriter/glitch reveal, carousel translation, and subtle scan/cursor motion."
    ],
    "source_type": "direct repo evidence with conservative inference for missing categories",
    "adaptation_notes": [
      "The supplied input/*.md and outputs/02-design-extraction.md files were not present in the workspace, so this profile is derived directly from app and component source files.",
      "Missing component categories are marked explicit=false and use low-confidence inferred rules only when consistent with the observed visual system."
    ]
  },
  "tokens": {
    "colors": {
      "primary": "#FFD600",
      "secondary": "#FF6B35",
      "accent": "#FFD600",
      "neutral": [
        "#050505",
        "#060606",
        "#080808",
        "#0A0A0A",
        "#0D0D0D",
        "#0F0F0F",
        "#111111",
        "#1A1A1A",
        "#1D1D1D",
        "#2D2D2D",
        "#3D3D3D",
        "#444444",
        "#555555",
        "#666666",
        "#888888",
        "#CCCCCC",
        "#F5F5F0"
      ],
      "success": "#4ADE80",
      "warning": "#FEBC2E",
      "danger": "#FF5F57",
      "background": "#0A0A0A",
      "surface": "#111111",
      "text": {
        "primary": "#F5F5F0",
        "secondary": "#888888",
        "muted": "#555555",
        "inverse": "#0A0A0A"
      },
      "border": "#2D2D2D"
    },
    "spacing": {
      "density": "compact controls inside large section bands; 4px grid language is explicit in product copy and stats",
      "section_gap": [
        "48px mobile vertical section gap",
        "64px desktop section gap",
        "py-16 px-6 mobile section padding",
        "md:py-[100px] md:px-[120px] common desktop section padding",
        "FinalCTA uses md:p-[120px]"
      ],
      "card_gap": [
        "2px repeated-card seam gap",
        "20px internal card content gap",
        "24px showcase card content gap",
        "32px mobile card padding",
        "40px desktop card padding"
      ],
      "control_gap": [
        "8px icon/dot/button group gaps",
        "10px mobile nav CTA stack gap",
        "12px avatar/social/brand gaps",
        "14px desktop nav CTA gap",
        "16px CTA and small row gap",
        "32px logo/section spacer rhythm"
      ],
      "grouping_pattern": "sections stack vertically; repeated cards sit in flex/grid rows with 2px seams; internal content stacks with 16-40px gaps; metadata badges sit above titles",
      "adaptation_rule": "Prefer multiples of 4px; use 24px horizontal padding on mobile, 120px on desktop, 32-40px card padding, and 2px seams for dense component groups."
    },
    "radius": {
      "control": "0px default",
      "container": "0px default",
      "overlay": "0px inferred default",
      "pill": "9999px only for dots/avatars/active markers; not for badges or CTAs",
      "dominant_family": "square brutalist rectangles",
      "sharp_allowed": "required for most buttons, cards, badges, tables, pricing panels, and navigation controls",
      "style_rule": "Use hard corners by default; only use circular radius for semantic dots, avatars, cursor markers, or tiny status indicators."
    },
    "shadows": [
      "No standard card/surface shadows in repo.",
      "Use borders and background shifts for elevation.",
      "Cursor visuals use drop-shadow(0 2px 6px rgba(0,0,0,0.7)) and name tags use box-shadow 0 2px 8px rgba(0,0,0,0.5)."
    ],
    "typography": {
      "font_families": [
        "Space Grotesk via next/font for headings, brand, primary CTA labels, and large numerals",
        "IBM Plex Mono via next/font for nav, labels, metadata, body support text, tables, pricing features, and captions"
      ],
      "scale": [
        "9-12px micro labels and metadata",
        "11-13px nav/body/caption mono text",
        "14-16px FAQ and small headings",
        "18-20px card headings",
        "24-28px bento/pricing headings",
        "36px mobile section titles",
        "44px mobile final CTA title",
        "48px pricing numbers and step numbers",
        "56px desktop section titles",
        "64px desktop stats",
        "80px desktop final CTA title",
        "clamp(32px,10vw,96px) hero title"
      ],
      "font_weights": [
        "400 regular",
        "500 available but rarely used",
        "700 dominant for headings, labels, CTAs, values"
      ],
      "line_heights": [
        "leading-none for hero and large numerals",
        "1.05 for section titles",
        "1.1 for bento titles",
        "1.2 for card/FAQ titles",
        "1.5 for step body",
        "1.6 for paragraphs/supporting text"
      ]
    },
    "widths": [
      "max-w-[480px] FAQ header",
      "max-w-[600px] section subtitle/showcase title",
      "max-w-[700px] default section title and final subtitle",
      "max-w-[800px] hero subtitle and bento title",
      "max-w-[1000px] final CTA title",
      "max-w-[1100px] hero title and design interface",
      "max-w-[1400px] navbar inner shell"
    ],
    "breakpoints": [
      "sm used for CTA row changes and footer bottom row; Tailwind default inferred at 640px",
      "md used as primary desktop switch for sections, nav, cards, carousel, tables, and typography; Tailwind default inferred at 768px"
    ]
  },
  "hierarchy": {
    "primary_focus_pattern": "large bold Space Grotesk headlines, often multiline and all caps, paired with yellow accent words, bands, borders, or badges",
    "secondary_content_pattern": "IBM Plex Mono captions and support text in #666666/#888888 with tracking and 1.5-1.6 line height",
    "cta_hierarchy": "primary CTA is yellow fill with black text; secondary CTA is dark fill with 2px gray or orange border; text links are muted gray until hover or active yellow",
    "emphasis_rules": [
      "Use yellow fill or yellow text for the highest-priority state or plan.",
      "Use orange border/text for secondary special features or enterprise emphasis.",
      "Use border width 2px for selected/featured/primary containers and 1px for normal surfaces.",
      "Use black-on-yellow inverse text for stats bands, primary CTAs, and featured pricing badges.",
      "Use bracketed numeric labels like [01] and section prefixes like [06] // VS. THE REST for scanning."
    ],
    "grouping_rules": [
      "Group repeated items edge-to-edge with 2px gaps rather than isolated floating cards.",
      "Separate data-heavy rows with 1px #1D1D1D/#2D2D2D borders.",
      "Use alternating section backgrounds to structure long pages.",
      "Keep action groups adjacent to header/title blocks, generally right-aligned on desktop or full-width stacked on mobile."
    ],
    "contrast_usage": "High contrast is reserved for primary actions and highlighted sections; most supporting text and inactive states remain deliberately low contrast in gray."
  },
  "typography_roles": {
    "page_title": "Space Grotesk, 700, clamp(32px,10vw,96px), tracking -1px, leading none, centered, all caps; yellow may be used for the emphasized line",
    "section_title": "Space Grotesk, 700, 36px mobile / 56px desktop, tracking -1px, leading 1.05, all caps, often whitespace-pre-line",
    "body": "IBM Plex Mono, 11-13px, tracking 1px, leading 1.5-1.6, gray/off-white depending emphasis, uppercase copy",
    "supporting_text": "IBM Plex Mono, 10-14px, #555555/#666666/#888888, tracking 0.5-2px, often centered in hero/CTA and left-aligned in cards",
    "label": "IBM Plex Mono, 9-12px, 700 when important, #FFD600 or muted gray, tracking 1.5-3px, bracket/slash syntax",
    "caption": "IBM Plex Mono, 10-11px, #444444/#555555/#666666, tracking 1-2px",
    "scanning_behavior": "users scan by yellow section labels, huge multiline titles, 2px card seams, bracket tags, and hard row dividers"
  },
  "interaction": {
    "hover": "color-only or border-only transitions: yellow CTAs darken to #e6c200, secondary controls shift border from #3D3D3D to #888888, muted links brighten to #CCCCCC/#F5F5F0, logo mark scales to 110%",
    "focus": "not explicitly implemented; infer visible 2px yellow outline or border treatment should be added for accessibility while preserving square geometry",
    "active": "nav active state uses #FFD600 text plus a 1.5px yellow underline; mobile nav uses yellow text and yellow dot; FAQ open state uses yellow square toggle with black glyph; carousel active dot expands from 8px to 32px",
    "selected": "selected/featured panels use yellow border/fill, 2px border, dark inverse text, or a left/top accent rail; hero editor selection uses dashed yellow outline and handles",
    "disabled": "not explicitly implemented; inferred pattern is #333333/#3D3D3D text or marks with no hover elevation, matching excluded pricing features and comparison negative states",
    "loading": "no generic loader; explicit motion vocabulary includes typewriter/glitch text reveal, blinking cursor, scanline, pulse, and carousel transition",
    "validation": "not present; infer inline monospace message, square border state, yellow/orange for attention, green #4ADE80 for success, red #FF5F57 for error if needed",
    "feedback_style": "immediate mechanical feedback through color, border, underline, expanded indicator bars, and plus/minus glyph changes rather than soft animation or shadow"
  },
  "layout": {
    "page_shell": "Next.js single landing page with fixed 60px navbar, full-width vertical sections, bg #0A0A0A, overflow-x hidden",
    "page_width_strategy": "sections are full-bleed color bands with inner horizontal padding px-6 mobile and md:px-[120px]; navbar has max-w-[1400px]; hero media/title max at 1100px",
    "header_pattern": "fixed transparent-to-blurred dark navbar; 60px height; desktop nav centered with active underline; desktop login/CTA on right; mobile burger opens dark blurred drawer",
    "section_spacing": "common pattern: py-16 px-6 gap-12 on mobile, md:py-[100px] md:px-[120px] gap-[64px] on desktop; smaller bands use py-[48px] or py-[80px]",
    "grid_rules": [
      "Cards use flex-col on mobile and md:flex-row on desktop.",
      "Repeated cards/tables/pricing use gap-[2px] to create pixel seams.",
      "Stats use two-column mobile grid and desktop flex row with hard dividers.",
      "Comparison uses desktop table and separate compact mobile grid.",
      "Showcase uses mobile single-card and desktop horizontal carousel with fixed 560px cards.",
      "Bento uses two stacked rows of three equal columns on desktop."
    ],
    "navigation_patterns": [
      "Smooth-scroll section links.",
      "IntersectionObserver active section tracking.",
      "Mobile drawer expands via max-height from 0 to 400px.",
      "Active section communicates through yellow text, underline/dot, and muted inactive text."
    ],
    "responsive_rules": [
      "Mobile first: stack CTAs, cards, pricing, footer, FAQ actions, and showcase cards.",
      "Use md breakpoint for major layout shift to horizontal rows and desktop table/carousel.",
      "Use sm breakpoint for CTA pairs and footer bottom alignment.",
      "Use max-width constraints on long title/subtitle blocks to preserve readable line length."
    ]
  },
  "components": {
    "buttons": {
      "explicit": true,
      "source_basis": "Navbar, Hero, Showcase, Pricing, FAQ, FinalCTA, and Footer implement buttons/links with square geometry, fixed heights, yellow fill or bordered dark variants, hover color/border transitions.",
      "confidence": "high",
      "rules": {
        "purpose": "primary actions, secondary actions, carousel controls, FAQ toggles, nav buttons, social buttons",
        "appearance": "square rectangular controls; primary #FFD600 fill with #0A0A0A text; secondary #0A0A0A/#111111 fill with 2px #3D3D3D border; icon toggles use 32-48px square blocks",
        "spacing": "heights 36px, 48px, 56px, or 64px; horizontal padding 18px for nav CTA, full-width on mobile, fixed 200-260px CTA widths on sm+",
        "radius": "0px except small circular status dots not actual buttons",
        "border": "primary often borderless; secondary 2px #3D3D3D; social 1px #2D2D2D; featured states #FFD600 or #FF6B35",
        "shadow": "none",
        "typography": "Space Grotesk 11-13px bold for primary/brand actions; IBM Plex Mono 10-12px for secondary, nav, and utility actions; tracking 1.5-2px",
        "states": "hover changes fill to #e6c200/#F5F5F0 or border to #888888; active nav uses yellow text and underline; FAQ open uses yellow fill and black minus; no explicit focus or disabled styling",
        "variants": [
          "primary-yellow",
          "secondary-bordered-dark",
          "nav-text",
          "icon-square",
          "faq-toggle",
          "carousel-arrow",
          "social-square",
          "text-link"
        ]
      }
    },
    "inputs": {
      "explicit": false,
      "source_basis": "No form input components found; inferred from buttons, table cells, badges, and editor visual language only.",
      "confidence": "low",
      "rules": {
        "purpose": "data entry or search should follow terminal/editor aesthetic if added",
        "appearance": "dark #0A0A0A/#111111 field, square corners, 1-2px #2D2D2D/#3D3D3D border, mono text, yellow caret/accent",
        "spacing": "height likely 48-56px; px 16-18px; gap 8-12px for labels/help",
        "radius": "0px",
        "border": "default #2D2D2D, hover #888888, focus #FFD600 inferred",
        "shadow": "none",
        "typography": "IBM Plex Mono 12-13px with tracking near 1px; labels 10-12px bold uppercase",
        "states": "inferred hover border brightens, focus yellow outline/border, disabled #333333 text, validation red/green border if needed",
        "variants": [
          "text-field-inferred",
          "search-field-inferred",
          "textarea-inferred"
        ]
      }
    },
    "selects": {
      "explicit": false,
      "source_basis": "No native select/listbox components found; inferred from square controls and dropdown-like nav/menu logic.",
      "confidence": "low",
      "rules": {
        "purpose": "single-choice selection should use compact terminal rows",
        "appearance": "dark square trigger, mono uppercase value, right glyph, hard border",
        "spacing": "48px height, px 16, option rows 40-48px inferred",
        "radius": "0px",
        "border": "#2D2D2D default; #FFD600 active/focus inferred",
        "shadow": "none",
        "typography": "IBM Plex Mono 11-12px, tracking 1-2px",
        "states": "selected option yellow text/dot; hover muted text brightens; disabled dim gray",
        "variants": [
          "single-select-inferred",
          "compact-filter-select-inferred"
        ]
      }
    },
    "dropdowns": {
      "explicit": true,
      "source_basis": "Navbar mobile drawer is an explicit collapsible dropdown panel with blurred near-black background and section buttons.",
      "confidence": "medium",
      "rules": {
        "purpose": "mobile navigation menu and inferred compact menu surfaces",
        "appearance": "full-width dark drawer, rgba(10,10,10,0.97), blur(14px), border-bottom #1E1E1E, stacked rows with border dividers",
        "spacing": "px-6 py-5 drawer, row py-[14px], gap 0, CTA stack gap 10px",
        "radius": "0px",
        "border": "bottom border #1E1E1E on open; row border #141414",
        "shadow": "none",
        "typography": "IBM Plex Mono 12px uppercase, tracking 1.5-2px",
        "states": "open max-height 400px; active row yellow text and yellow dot; inactive #666; close on link click",
        "variants": [
          "mobile-nav-drawer",
          "inferred-menu-panel"
        ]
      }
    },
    "cards": {
      "explicit": true,
      "source_basis": "FeatureCard, StepCard, TestimonialCard, Bento panels, PricingCard, and Showcase cards define repeated panel rules.",
      "confidence": "high",
      "rules": {
        "purpose": "feature explanation, process steps, testimonials, capability tiles, pricing tiers, showcase projects",
        "appearance": "dark rectangular surfaces with 1px or 2px borders, no radius, no shadow; highlighted cards use yellow fill, yellow/orange border, or left accent rail",
        "spacing": "p-8 mobile, md:p-[32px] or md:p-[40px]; content gap 16-32px; card rows gap-[2px]",
        "radius": "0px",
        "border": "#2D2D2D default; #FFD600 primary highlight; #FF6B35 secondary highlight; testimonial uses border-left-4 accent",
        "shadow": "none",
        "typography": "Space Grotesk bold 18-28px headings; IBM Plex Mono 11-13px support text; labels/tags 10-11px mono",
        "states": "mostly static; carousel active chooses current card; featured pricing uses stronger border/fill; no hover state on cards",
        "variants": [
          "feature-card",
          "step-card",
          "testimonial-card",
          "bento-tile",
          "pricing-card",
          "showcase-card",
          "accent-filled-card",
          "left-rail-card"
        ]
      }
    },
    "tables": {
      "explicit": true,
      "source_basis": "Comparison implements desktop table and mobile comparison grid with headers, rows, borders, and emphasized PixelCraft column.",
      "confidence": "high",
      "rules": {
        "purpose": "feature comparison and structured data display",
        "appearance": "square bordered table, dark header #111111, yellow 2px header divider, #1A1A1A highlighted product column, hard cell dividers",
        "spacing": "desktop rows h-[56px], px-[32px]; first column w-[400px]; mobile grid px 2-3 and py 3-4",
        "radius": "0px",
        "border": "outer #2D2D2D; row separators #1D1D1D; column dividers #2D2D2D; active header border #FFD600",
        "shadow": "none",
        "typography": "headers Space Grotesk 9-11px bold tracking 1-2px; cells IBM Plex Mono 9-14px tracking 1px",
        "states": "static; positive cells yellow for PixelCraft, competitor positives muted #444444, negatives/dashes dim #3D3D3D/#444444",
        "variants": [
          "desktop-comparison-table",
          "mobile-comparison-grid"
        ]
      }
    },
    "modals": {
      "explicit": false,
      "source_basis": "No modal component found; inferred cautiously from drawer/cards/table surface language.",
      "confidence": "low",
      "rules": {
        "purpose": "blocking overlays should be rare and utilitarian",
        "appearance": "near-black square panel, 2px #FFD600 or #2D2D2D border, mono labels, no rounded corners",
        "spacing": "p 32-40px inferred; action row gap 16px",
        "radius": "0px",
        "border": "2px accent for critical/active modal, 1px #2D2D2D for neutral",
        "shadow": "none or very subtle black overlay only inferred",
        "typography": "Space Grotesk title; IBM Plex Mono body/actions",
        "states": "focus trap and yellow focus ring should be added if implemented; no repo evidence",
        "variants": [
          "modal-inferred"
        ]
      }
    },
    "dialogs": {
      "explicit": false,
      "source_basis": "No dialog/alert dialog component found; inferred from FAQ toggles, pricing cards, and CTA controls.",
      "confidence": "low",
      "rules": {
        "purpose": "confirmation or short decision UI",
        "appearance": "compact square dark panel with hard border and yellow/orange action emphasis",
        "spacing": "p 24-32px inferred; stacked on mobile, inline actions on sm+",
        "radius": "0px",
        "border": "#2D2D2D default, #FFD600 for primary decision",
        "shadow": "none",
        "typography": "Space Grotesk 20-28px title; IBM Plex Mono 12-13px message/actions",
        "states": "primary yellow action, secondary bordered dark action, no explicit repo state",
        "variants": [
          "confirm-dialog-inferred"
        ]
      }
    },
    "sidebars": {
      "explicit": true,
      "source_basis": "Hero SVG contains explicit left LAYERS and right INSPECT side panels; mobile nav drawer is also side/drawer-adjacent but vertical top panel.",
      "confidence": "medium",
      "rules": {
        "purpose": "editor side panels for layers, inspect properties, and token lists",
        "appearance": "#111111 panel on #0F0F0F canvas, 1px #2D2D2D separators, 36px darker header bars, yellow section labels",
        "spacing": "200px left panel, 201px right panel in SVG; 36px headers; property rows spaced 26-32px",
        "radius": "0px; tiny SVG swatches may use rx 1px",
        "border": "1px #2D2D2D vertical separators and header dividers",
        "shadow": "none",
        "typography": "monospace 8-9px labels and values with 0.5-2px tracking",
        "states": "active layer uses #1E1E1E row fill and 2px yellow left rail; selected tool uses yellow square",
        "variants": [
          "layers-sidebar",
          "inspect-sidebar",
          "mobile-nav-drawer"
        ]
      }
    },
    "tabs": {
      "explicit": false,
      "source_basis": "No tab component found; carousel dots and nav active underline provide only related selection patterns.",
      "confidence": "low",
      "rules": {
        "purpose": "section switching or compact segmented navigation if needed",
        "appearance": "mono uppercase labels, square hit areas, active yellow text plus 1.5-2px underline or yellow block indicator",
        "spacing": "desktop gap 32-36px inferred from nav; compact tabs 8-16px gaps inferred",
        "radius": "0px",
        "border": "active underline #FFD600; optional bottom border #1D1D1D",
        "shadow": "none",
        "typography": "IBM Plex Mono 10-12px tracking 1.5-2px",
        "states": "active yellow, inactive #555/#666, hover #F5F5F0, focus yellow outline inferred",
        "variants": [
          "underline-tabs-inferred",
          "segmented-square-tabs-inferred"
        ]
      }
    },
    "badges": {
      "explicit": true,
      "source_basis": "Hero badge, FinalCTA badge, Feature tags, Bento tags, Pricing tier labels, and Showcase tags share compact rectangular badge rules.",
      "confidence": "high",
      "rules": {
        "purpose": "section status, tags, tier labels, capability labels, project categories",
        "appearance": "small square rectangular chips with dark or yellow fill, optional 1-2px accent border, all-caps bracket text",
        "spacing": "height 24-32px; px 10-16px; internal dot gap 8px",
        "radius": "0px",
        "border": "1px or 2px #FFD600/#FF6B35/#3D3D3D; transparent border for filled badges",
        "shadow": "none",
        "typography": "IBM Plex Mono 9-11px, often bold, tracking 1-2px",
        "states": "static; active/featured badges invert to yellow fill with black text",
        "variants": [
          "section-badge",
          "tag-chip",
          "tier-badge",
          "status-chip",
          "dot-badge"
        ]
      }
    },
    "alerts": {
      "explicit": false,
      "source_basis": "No alert component found; color/status vocabulary exists in badges, pricing inclusion marks, and hero SVG status dots.",
      "confidence": "low",
      "rules": {
        "purpose": "system feedback should be terse and label-like",
        "appearance": "square dark strip or panel with left accent rail or 2px border; monospace uppercase message",
        "spacing": "p 16-24px inferred; gap 8-12px for icon/label",
        "radius": "0px",
        "border": "yellow for notice, orange for warning, green #4ADE80 for success, red #FF5F57 for destructive/error inferred from SVG tokens",
        "shadow": "none",
        "typography": "IBM Plex Mono 11-13px tracking 1px, bold label prefix",
        "states": "static; dismiss control should be square bordered button if needed",
        "variants": [
          "notice-inferred",
          "warning-inferred",
          "success-inferred",
          "error-inferred"
        ]
      }
    },
    "empty_states": {
      "explicit": true,
      "source_basis": "Showcase placeholder panels use [SCREENSHOT] in muted mono text inside bordered dark blocks; hero editor also uses placeholder-like grid/canvas states.",
      "confidence": "medium",
      "rules": {
        "purpose": "placeholder media, unavailable preview, or empty editor/data region",
        "appearance": "#1A1A1A dark block with 1px #2D2D2D border and centered bracketed mono text in #333333",
        "spacing": "showcase placeholders h-[160px] mobile and h-[200px] desktop; centered flex alignment",
        "radius": "0px",
        "border": "1px #2D2D2D",
        "shadow": "none",
        "typography": "IBM Plex Mono 11px, tracking 2px, muted #333333",
        "states": "static; can pair with yellow CTA or link below for recovery",
        "variants": [
          "media-placeholder",
          "canvas-placeholder-inferred"
        ]
      }
    },
    "charts_containers": {
      "explicit": true,
      "source_basis": "Hero DesignInterfaceSVG implements dashboard/editor-like chart/code/canvas containers, token panels, rulers, code lines, and status bars.",
      "confidence": "medium",
      "rules": {
        "purpose": "visual product demo, analytics/editor panels, token displays, code/canvas regions",
        "appearance": "dark editor canvas with side panels, rulers, grid dots, code blocks, status bars, selection handles, and dashed yellow selection frame",
        "spacing": "large fixed SVG viewBox 1100x580; 36px toolbar/panel headers; 16-32px panel rows; code lines spaced 16px",
        "radius": "0px dominant; SVG mini swatches and toolbar buttons may use rx 1-2px",
        "border": "1px #2D2D2D grid/panel borders; dashed #FFD600 selected frame; orange/blue measurement lines",
        "shadow": "none in container; only external collaboration cursors have drop shadows",
        "typography": "monospace 6-9px for editor labels, properties, rulers, and tokens",
        "states": "animated scanline, blinking cursor, pulsing status dot, selected tool yellow fill, active layer left rail",
        "variants": [
          "editor-canvas",
          "inspect-panel",
          "code-block",
          "token-list",
          "status-bar",
          "selected-frame"
        ]
      }
    },
    "page_headers": {
      "explicit": true,
      "source_basis": "SectionHeader is shared by most sections; Hero and FinalCTA define larger page-level header variants.",
      "confidence": "high",
      "rules": {
        "purpose": "section introduction, hero headline, conversion headline",
        "appearance": "stacked label, large multiline title, optional mono subtitle; label in yellow, title off-white or yellow emphasis",
        "spacing": "SectionHeader gap 16px; section-to-content gap usually 48px mobile / 64px desktop; hero uses 32-64px explicit spacers",
        "radius": "none",
        "border": "none directly; nearby section badges may carry borders",
        "shadow": "none",
        "typography": "label IBM Plex Mono 10-12px bold tracking 1.5-3px; title Space Grotesk 36/56px or larger; subtitle IBM Plex Mono 10-15px leading 1.6",
        "states": "GlitchText/typewriter reveal on many labels/titles/subtitles; no interactive states",
        "variants": [
          "section-header",
          "hero-header",
          "final-cta-header",
          "compact-left-header"
        ]
      }
    },
    "filters": {
      "explicit": false,
      "source_basis": "No filters found; inferred from nav links, badges, carousel dots, and comparison controls.",
      "confidence": "low",
      "rules": {
        "purpose": "filtering lists or project categories should use chip/button controls",
        "appearance": "rectangular dark chips with 1px border; active chip yellow fill or yellow border/text",
        "spacing": "height 28-36px, px 10-16px, gap 8px inferred from badges and carousel controls",
        "radius": "0px",
        "border": "#2D2D2D default; #FFD600 active; #FF6B35 special category",
        "shadow": "none",
        "typography": "IBM Plex Mono 10-11px uppercase tracking 1-2px",
        "states": "active yellow, hover border/text brighten, disabled dim #333333 inferred",
        "variants": [
          "chip-filter-inferred",
          "dot-filter-inferred"
        ]
      }
    },
    "form_layouts": {
      "explicit": false,
      "source_basis": "No forms found beyond pricing actions; inferred layout follows stacked labels/controls and full-width mobile CTA behavior.",
      "confidence": "low",
      "rules": {
        "purpose": "forms should be utilitarian and mono-labeled",
        "appearance": "single-column dark form sections with hard borders and square controls",
        "spacing": "field stack gap 16-24px; form padding 24-40px; action gap 16px; full-width buttons on mobile",
        "radius": "0px",
        "border": "section border #2D2D2D; focused field #FFD600 inferred",
        "shadow": "none",
        "typography": "IBM Plex Mono labels 10-12px uppercase; Space Grotesk form title if present",
        "states": "inline validation below fields in mono text; success/error colors inferred from SVG status tokens",
        "variants": [
          "stacked-form-inferred",
          "inline-action-form-inferred"
        ]
      }
    }
  },
  "ux_patterns": {
    "cta_hierarchy": "Hero and FinalCTA establish paired CTAs: yellow filled primary first, dark bordered secondary second; navbar repeats small yellow primary CTA plus muted login link.",
    "information_grouping": "Long landing page groups content into numbered sections, each with a yellow mono label, big title, and a dense grid/table/card block; repeated items sit edge-to-edge with 2px seams.",
    "filter_placement": "No filters implemented; inferred placement is above data/card regions or as compact chip rows aligned with section headers, matching carousel dots below showcase content.",
    "form_structure": "No forms implemented; inferred structure is single-column, mono labels, square bordered inputs, and full-width mobile action buttons.",
    "validation_behavior": "No validation implemented; inferred behavior should use border color and terse mono helper text, with green success, red error, orange warning, and yellow attention states.",
    "table_detail_strategy": "Desktop comparison table prioritizes first feature column and highlighted product column; mobile switches to compact grid with abbreviated competitor headers and fewer visible columns.",
    "loading_error_empty_states": "Loading is expressed as typewriter/glitch text, blinking cursor, scanline, pulse, and carousel transitions; empty media uses a bordered placeholder with bracketed muted mono label.",
    "action_placement": "Primary actions appear immediately after hero/final CTA copy, pricing details, or top-right section controls; secondary text links appear at section footers or next to support copy.",
    "notes": [
      "Interaction design favors instant state changes through color, border, underline, and glyph swaps over depth or motion-heavy feedback.",
      "The system is intentionally low-radius and low-shadow; introducing soft cards or rounded controls would conflict with the repo identity.",
      "Several accessibility states, especially focus-visible and disabled, are not explicitly coded and should be added if this design system is productized."
    ]
  },
  "constraints": [
    "Use valid Next.js/Tailwind-compatible tokens and preserve current font pair: Space Grotesk and IBM Plex Mono.",
    "Avoid rounded cards/buttons; radius should normally be 0px.",
    "Avoid shadows for layout elevation; prefer hard borders, color bands, and 2px seams.",
    "Do not dilute #FFD600 as primary accent; use it sparingly but decisively for key hierarchy and active states.",
    "Keep copy uppercase, terse, and technical when extending existing sections.",
    "Respect mobile stacking and md desktop row/table/carousel switches.",
    "Focus states are under-specified in the repo; any implementation should add accessible visible focus without changing the core square visual language.",
    "The requested context files under input/ and outputs/ were absent, so this profile is based on direct source inspection of app/ and components/."
  ]
}

```

# Reference Files

- `input/repo-summary.md`
- `input/repo-file-map.txt`
- `input/relevant-files.md`
- `input/design-extraction-schema.json`
- `input/design-extraction-output-schema.json`
- `outputs/01-ui-ux-foundation.md`
- `outputs/02-design-extraction.md`
- `outputs/02-design-extraction.json`
- `outputs/03-final-skill.md`

# Operating Notes

- Reuse existing component conventions before proposing new ones.
- Treat radius, spacing, hierarchy, typography roles, and interaction feedback as design anchors.
- When a screen category is missing in the source repo, derive it from the source identity rather than inventing a new visual system.
- A dashboard may be denser than a portfolio, but it must still retain the source geometry, spacing character, and emphasis style.