# Professional Software UI/UX Foundations (Style‑Agnostic)

## Purpose
Enable an AI agent to design professional software interfaces that are clear, accessible, consistent, and product‑ready, while remaining agnostic to visual style. This skill defines foundational UX/UI rules, layout and component guidance, decision heuristics, and output behaviors. A project‑specific style guide may later bind tokens (color, type, radius, shadows) to these rules.

## Design philosophy
- Clarity over cleverness; purpose over decoration.
- Predictability, learnability, and efficiency drive decisions.
- Start from user tasks and constraints; adopt progressive disclosure.
- Prefer semantic roles and tokens over hardcoded visuals.
- Consistency creates speed: reuse patterns before inventing new ones.
- Accessibility is non‑negotiable; inclusivity by default.
- Small, intentional variations; every deviation must earn its keep.

## UX fundamentals
- Clarity
  - Use plain language; avoid jargon. Labels name actions (“Invite user”), not technologies.
  - Pair icons with text where meaning isn’t universally recognized.
  - One clear primary action per view; make its outcome obvious.
- Usability
  - Minimize steps, scrolling, and precision clicks. Targets ≥44×44 logical px.
  - Inline, real‑time validation; do not punish reversible mistakes.
  - Offer sensible defaults; remember last chosen options when safe.
- Visual hierarchy
  - Emphasize by position, size, weight, and contrast (in that order).
  - Group related items via proximity and shared containers.
  - Limit concurrent emphasis: 1 primary, a few secondary, most tertiary.
- Accessibility
  - Text contrast: ≥4.5:1 (normal), ≥3:1 (large). Do not rely on color alone.
  - Full keyboard navigation; visible focus states; logical tab order.
  - Provide ARIA/semantic structure; announce dynamic updates.
  - Descriptive error messages, not codes; include suggestions to fix.
- Consistency
  - One spacing scale, one type scale, one radius scale, shared state model.
  - Reuse patterns across views; avoid near‑duplicate components.
  - Terminology and microcopy stay consistent across the product.
- Feedback states
  - Show immediate acknowledgment (press, loading, success, error, empty).
  - Use skeletons for content loads and progress for process loads.
  - Non‑blocking toasts for minor events; inline messages for contextual issues.
- Cognitive load reduction
  - Chunk tasks; reveal advanced options on demand.
  - Replace long forms with steps and smart defaults.
  - Prefer examples and helper text over lengthy documentation.
- Task‑oriented design
  - Optimize for the top tasks’ happy paths; make recovery easy.
  - Place next best action near the object of work.
  - Allow safe exploration; make destructive actions intentional and reversible.
- Responsiveness
  - Layouts adapt fluidly; prioritize content order on narrow screens.
  - Touch and pointer affordances are both first‑class.
  - Respect safe areas, dynamic type preferences, and system themes if available.
- Information density management
  - Offer density modes (comfortable/compact) without breaking alignment.
  - Use whitespace to create rhythm; avoid cramming more than 9–12 items per visual group.
  - Truncate with tooltips for long strings; allow column toggles in data‑heavy views.

## UI fundamentals
- Spacing systems
  - Use a single modular scale (e.g., 4/8‑pt). Apply to padding, gaps, margins.
  - Define container paddings (page, section, card) and inter‑component spacing tokens.
  - Maintain vertical rhythm; avoid arbitrary one‑off offsets.
- Typography hierarchy
  - Semantic levels (Page title, Section title, Subhead, Body, Caption, Code).
  - Limit to 5–6 text styles; control line length (45–75 chars body).
  - Set line‑height for readability (≈1.4–1.6 body; tighter for headings).
- Component consistency
  - Standard sizes (S/M/L) per control family; shared state model across components.
  - Inputs align label, helper, error consistently; identical hit areas per size.
- Layout rhythm
  - Work on a column grid with consistent gutters and margins.
  - Align content blocks to grid; keep consistent header and section spacing.
- Alignment
  - Left align text and form labels; right align numeric table cells; center sparingly.
  - Align controls and icons to text baselines or optical centers.
- Contrast management
  - Use role‑based color tokens (text/primary/secondary/muted/border/surface/background).
  - Elevation and borders are for separation; avoid low‑contrast “ghost” controls.
- State design
  - Define states: default, hover, focus (always visible), active/pressed, selected, disabled, loading, success, warning, error.
  - Transitions: subtle (100–200ms) with consistent easing; no gratuitous motion.
- Icon usage
  - Prefer simple, universal metaphors; pair with labels unless truly obvious.
  - Consistent stroke/fill style and sizes mapped to text sizes.
  - Do not convey meaning by color alone; ensure contrast and labeling.
- Border radius logic
  - One radius scale (e.g., 0, XS, S, M, L, pill). Map by component class.
  - Larger containers get larger radii than inner elements; avoid nesting conflicting radii.
- Shadow usage
  - Use a small set of elevation levels; subtle, color‑aware shadows for separation.
  - Increase elevation to indicate interactivity or overlay hierarchy; avoid multiple stacked shadows.
- Color role assignment
  - Semantic roles: primary, secondary, destructive; status: success, warning, danger, info.
  - Surfaces: background, surface, raised, overlay; text: high, medium, low emphasis; borders: subtle/strong.
  - Map brand later via tokens; never hardcode palette in foundational guidance.

## Layout rules
- Grids and containers
  - Define page max‑widths; use responsive columns (e.g., 4/8/12) with fixed gutters.
  - Keep primary content within the central container; utilities in side rails.
- Multi‑column layouts
  - Mobile: single column; Tablet: 2 columns; Desktop: 3–4 columns as content allows.
  - Avoid splitting related content across columns; maintain reading order.
- Page archetypes
  - Dashboards
    - Above‑the‑fold summary; cards with clear titles, primary metric, trend/context.
    - Prioritize scannability (consistent card headers, aligned baselines).
    - Personalization allowed within safe bounds (reorder, hide, density).
  - Forms
    - One clear purpose per form; group by topic; multi‑step for 7+ fields or complexity.
    - Labels persist above inputs; helper text below; inline validation on blur/change.
    - Primary action fixed at bottom/top on long forms; include keyboard submit.
  - Settings pages
    - Left navigation for categories; right content area for controls.
    - Use toggles for binary, selects for finite sets, text inputs sparingly.
    - Show “Saved” feedback inline; provide “Reset to defaults” and “Audit notes” where needed.

## Component rules
- Data tables
  - Use when items share uniform attributes; support sorting, filtering, and column control.
  - Sticky header; optional sticky first column; zebra or subtle row separators.
  - Row density toggle; inline actions on hover/focus; bulk actions above table.
  - Empty, loading (skeleton rows), and error states defined and consistent.
- Cards
  - Use for heterogeneous or summary content; consistent structure (media/metric → title → meta → actions).
  - Clickable region is the whole card only when the card represents a single destination; otherwise isolate actions.
- Navigation
  - Global nav exposes top‑level IA; highlight current location; provide search entry.
  - Secondary nav (tabs/left rail) for section scoping; breadcrumbs for depth >2.
  - Collapse to hamburger or “More” only when necessary; preserve key items.
- Modals
  - For small, focused tasks (≤2 decisions) or confirmations; never for multi‑step flows or navigation.
  - Trap focus; restore focus on close; provide clear primary and safe secondary actions.
- Empty states
  - Explain “why empty,” “what to do,” and “how to start.” Offer primary action and optional sample data or import.
- Alerts
  - Severity‑mapped visuals (info/success/warning/danger). Inline for local issues; banners for page‑level; toasts for ephemeral success.
  - Include action to resolve; ensure dismissibility rules are consistent by severity.
- Filters
  - Place near data source (lists/tables/maps). Support quick chips for common filters; advanced panel/drawer for complex.
  - Summarize active filters as tokens; allow one‑click clear; persist on navigation when appropriate.

## Decision heuristics
- Card vs table
  - Choose table when comparing many items across consistent attributes, enabling sort/filter/bulk actions.
  - Choose card when items are few, attributes vary, or storytelling/preview matters (media, rich metrics).
- Modal vs dedicated page
  - Use modal for single decision, quick confirm, or minor create/edit with ≤2 inputs.
  - Use page for multi‑step tasks, heavy context, or actions requiring discovery, help, or preview.
- Tabs vs accordion
  - Tabs when categories are peers requiring quick comparison/switching; limit to 2–6 labels.
  - Accordion when content is long, independent, and scan‑then‑expand suits the task; avoid nesting.
- Sidebar vs top navigation
  - Sidebar for many sections or deep IA requiring persistent context and secondary actions.
  - Top nav for shallow IA and frequent cross‑section switching; add secondary nav within pages as needed.
- Dense vs spacious layout
  - Dense for expert, data‑heavy workflows and high frequency tasks; keep legibility and hit targets intact.
  - Spacious for discovery, learning, and infrequent tasks; emphasize guidance and context.
- High emphasis vs subtle emphasis
  - High emphasis for primary next action, critical alerts, or key KPIs; only one primary per view.
  - Subtle emphasis for supportive actions, secondary info, or non‑blocking notices.

## Anti‑patterns
- Decorative UI without purpose
- Inconsistent spacing
- Too many accent colors
- Weak visual hierarchy
- Inaccessible contrast
- Overdesigned controls
- Poor grouping
- Excessive shadows or gradients
- Unclear CTA hierarchy

## Final behavioral rules for the AI
- Prioritize clarity over novelty; explain choices in plain language.
- Keep screens coherent: one primary goal, minimal emphasis points.
- Avoid unnecessary variation; reuse established patterns and components.
- Justify layout and component choices based on task, density, and accessibility needs.
- Maintain a product‑ready feel: complete states (empty/loading/error/success), keyboard focus, and responsive behavior.
- Use semantic roles and tokens (colors, spacing, type, radius, shadows) rather than hardcoded values; defer visual style to the project style guide.
- Provide defaults and options safely: compact/comfortable density, column visibility, and non‑destructive undo where applicable.
- When uncertain, choose the simpler, more consistent pattern and document the tradeoff.