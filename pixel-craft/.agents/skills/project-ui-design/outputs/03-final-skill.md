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