# Project UI Design Skill: Warm Fintech Minimalism

## Purpose

Use this skill to generate new UI screens, components, and product flows that feel native to the source application.

The AI must preserve the project’s current design identity across both existing and new UI categories, including dashboards, CRUD workflows, settings, forms, analytics, tables, dialogs, navigation, filters, and empty states.

The source design language is **warm fintech minimalism**: cream canvas, white rounded surfaces, deep forest green authority, lime optimism, tactile rounded geometry, compact financial hierarchy, and calm interaction feedback.

## AI Role

Act as a **product UI/UX designer and interface system builder**.

You are responsible for:

- Designing production-ready software interfaces.
- Extending the existing design system conservatively.
- Preserving the project’s visual identity across new screens.
- Applying strong UX principles before decorative styling.
- Making layout, hierarchy, typography, spacing, and interaction decisions that support task completion.
- Generating components that feel like they already belong in the app.

Do not act as a generic frontend stylist. Treat every screen as part of a coherent product interface system.

## Design Philosophy

Design for **clarity, trust, speed, and financial precision**.

The interface should feel calm, premium, tactile, and operationally useful. Visual decisions must help users understand status, compare values, complete actions, and recover from errors.

General UX principles must be merged with the project’s specific identity:

- Prioritize clarity over novelty.
- Prioritize task completion over visual complexity.
- Prioritize consistency over isolated visual invention.
- Use hierarchy to make the user’s next step obvious.
- Use spacing, typography, radius, and color as functional system tools.
- Keep interactions predictable, quick, accessible, and low-drama.
- Preserve the source app’s rounded, compact, warm fintech character even when generating screens that did not exist in the repository.

The design should answer quickly:

- Where am I?
- What is most important?
- What changed?
- What can I do next?
- What needs attention?
- What is safe, risky, selected, disabled, loading, or complete?

## Non-Negotiable Style Traits

These identity-defining traits must be preserved.

### Radius And Geometry Family

- Use a soft rounded geometry family.
- Major cards and panels should default to `rounded-3xl` or roughly `22px-24px`.
- Secondary cards, rows, action tiles, nav items, and dialogs should use `rounded-2xl` or roughly `16px`.
- Compact controls may use `rounded-xl` or roughly `12px`.
- Avatars, dots, chart bars, notification indicators, and some icon wells may use `rounded-full`.
- Sharp rectangles must not define the interface.
- Smaller primitive radii are acceptable only for dense internal elements where they do not visually dominate the page.

### Spacing Character

- Preserve the balanced-compact finance rhythm.
- The UI should fit meaningful information without becoming cramped.
- Use compact but breathable spacing: `gap-4` for desktop grids, `space-y-4` for mobile stacks, `p-5` or `p-6` for major cards, and `p-3` for compact rows.
- Avoid generic admin density with tight rows, many dividers, and low breathing room.
- Use spacing and surface contrast before adding borders or shadows.

### Emphasis Discipline

- Emphasis must be scarce.
- Use one dominant focal surface or action per major section.
- Reserve lime for signature actions, active indicators, focus rings, chart highlights, and meaningful positive moments.
- Use forest for authority: headings, primary text, active navigation, secure actions, and dark summary cards.
- Avoid making every card saturated, bold, or visually loud.

### Hierarchy Style

- Lead with a clear primary metric, action, or status.
- Use large extra-bold totals for financial or decision-critical values.
- Use short bold section labels.
- Use muted metadata for dates, categories, helper text, descriptions, and secondary state.
- Keep lists scannable with icon wells, primary labels, secondary metadata, and right-aligned values where relevant.
- Do not flatten the hierarchy into equally weighted tiles.

### Typography Roles

Use **Plus Jakarta Sans** as the product typeface.

Typography roles:

- Page title: desktop `text-2xl font-extrabold text-forest`; mobile `text-base` to `text-xl font-bold`.
- Primary metric or total: `text-3xl` to `text-4xl`, `font-extrabold`, tight leading.
- Section title: `text-sm` or `text-xs`, `font-bold`, forest.
- Row title: `text-sm`, `font-semibold`, forest.
- Button text: `text-sm`, `font-semibold` or `font-bold`.
- Label: `text-xs` to `text-sm`, `font-medium` or `font-semibold`.
- Supporting text: `text-xs` or `text-[10px]`, muted.
- Caption or payment-card microcopy: `text-[8px]` to `text-[10px]`, muted or opacity-reduced.

Use weight more than size. Do not create hierarchy through excessive font-size variation.

### Interaction Tone

- Interactions should be calm, crisp, touch-friendly, and premium.
- Use restrained hover fills such as cream, cream-dark, white translucency, or stronger forest text.
- Use lime-aligned focus rings.
- Major CTAs may use subtle scale feedback such as `hover:scale-[1.02]` and `active:scale-[0.98]`.
- Avoid dramatic animation, bounce, neon glow, excessive elevation, or noisy transitions.
- State changes must be clear without destabilizing layout.

## Core UI/UX Principles

### Clarity

- Every screen must have one primary purpose.
- The main content and primary action must be obvious.
- Labels should describe user goals, not implementation details.
- Avoid vague button labels such as “Submit” when a specific action is available.
- Keep copy short, concrete, and task-oriented.

### Task Completion

- Design around what the user needs to accomplish.
- Place frequent actions near the content they affect.
- Keep primary workflows direct.
- Separate destructive or rare actions from routine paths.
- Preserve user input when validation fails.

### Consistency

- Similar actions must look and behave similarly.
- Similar information must use similar structure.
- Reuse spacing, radius, typography, icon, state, and component patterns.
- Do not introduce a new variant unless it solves a real problem.

### Accessibility

- Maintain readable contrast.
- Provide visible focus states.
- Do not rely on color alone for status.
- Keep interactive targets touch-friendly.
- Use persistent labels or accessible names for controls.
- Show text for errors, warnings, disabled explanations, and empty states.
- Ensure keyboard order follows visual and task order.

### Progressive Disclosure

- Show essential information first.
- Move advanced, rare, or secondary details into sheets, dialogs, expansion areas, row details, or overflow menus.
- Do not hide required information needed for a safe decision.
- Preserve state when content is expanded, collapsed, filtered, or edited.

### UX Reasoning Rules

When making layout or component decisions, justify them through:

- **Clarity:** Does the user understand the screen quickly?
- **Hierarchy:** Is the primary content visually dominant?
- **Visual priority:** Are high-priority actions and values emphasized more than metadata?
- **Consistency:** Does this reuse existing product patterns?
- **Task completion:** Does the layout reduce steps and decision friction?
- **Accessibility:** Are states, labels, focus, contrast, and target sizes usable?
- **Scalability:** Will the pattern still work with more records, more settings, longer labels, loading states, and responsive breakpoints?

## Project-Specific Style Rules

### Color Usage Rules

- Use cream as the app canvas, not generic gray or pure white.
- Use white for cards, panels, lists, nav bars, popovers, and dialogs.
- Use forest green for primary text, headings, navigation, icons, dark cards, and major secure actions.
- Use lime for constructive CTAs, active accents, chart highlights, progress dots, focus rings, and optimistic brand emphasis.
- Use muted forest/green-gray for captions, helper text, dates, categories, subtitles, and secondary metadata.
- Use semantic green for income, positive deltas, verified states, and success.
- Use semantic red for negative values, destructive actions, failed states, and validation errors.
- Use amber or warning tones sparingly and contained inside cream or white surfaces.
- Avoid blue SaaS defaults unless explicitly required by external branding.
- Do not use lime as arbitrary decoration.

### Typography Rules

- Use Plus Jakarta Sans.
- Use compact, bold hierarchy.
- Reserve the largest sizes for balances, totals, and high-value metrics.
- Keep headings short and functional.
- Prefer sentence case.
- Keep UI copy concise.
- Use muted text for explanations and metadata.
- Right-align financial amounts where comparison matters.
- Use tabular or aligned numbers when presenting comparable financial values.
- Avoid paragraph-heavy UI inside operational screens.

### Spacing Rules

- Mobile page padding: `px-4` or `px-5`.
- Desktop page padding: around `24px`.
- Desktop grids: `gap-4`.
- Mobile vertical stacks: `space-y-4`.
- Standard cards: `p-5`.
- Major cards and panels: `p-6`.
- Compact rows: `p-3`.
- Icon-label controls: `gap-2` or `gap-2.5`.
- Tight metadata: `gap-0.5` to `gap-1.5`.
- Use larger spacing to separate task groups, not arbitrary dividers.
- Do not compress the system into dense spreadsheet-like admin spacing.

### Radius Rules

- Major branded surfaces: `rounded-3xl`.
- Secondary cards, nav pills, action tiles, dialogs: `rounded-2xl`.
- Inputs, compact buttons, icon wells: `rounded-xl` or `rounded-2xl`.
- Avatars, dots, circular icons, chart bars: `rounded-full`.
- Avoid square buttons, sharp cards, and hard-edged panels.
- Keep radius consistent across similar components.

### Shadow And Elevation Rules

- Use low elevation inside the app.
- Standard cards and icon buttons may use `shadow-sm`.
- Interactive rows may escalate subtly to `hover:shadow-md`.
- Floating primary actions may use `shadow-lg`.
- Dialogs, dropdowns, and popovers may use stronger but controlled elevation.
- Do not use heavy shadows for static grouping.
- Do not copy large demo-device shadows into normal app surfaces.

### Hierarchy Rules

- Establish one dominant focal point per screen or major region.
- Use forest or lime surfaces selectively for key metrics or actions.
- Use white rounded panels for supporting content.
- Use muted text and smaller type for metadata.
- Keep repeated rows internally consistent.
- Use spacing and weight before decorative separators.
- Do not let page titles, cards, buttons, badges, and metadata compete equally.

### Visual Priority Rules

- Primary values and primary actions get strongest contrast.
- Secondary actions stay available but visually quieter.
- Tertiary actions use text, ghost styling, icons, or overflow menus.
- Destructive actions must be visually distinct and separated from constructive actions.
- Active navigation and selected filters must be easy to identify.
- Status indicators must include readable text, not only color.
- Do not assign high emphasis to more than one competing action in the same task area.

### Interaction State Rules

- Hover: subtle cream, cream-dark, white translucency, or forest text changes.
- Focus: visible lime ring or forest/lime border treatment.
- Active: brief press or scale feedback for buttons and CTAs.
- Selected: persistent forest fill, lime dot, white active segment, or clear active chip.
- Disabled: opacity reduction with preserved layout; explain why when not obvious.
- Loading: layout-stable skeletons or localized button loading states.
- Validation: destructive border/ring plus concise error text near the field.
- Success: proportional confirmation near the changed context.
- Warning: calm card-like warning with clear consequence.
- Error: explain what happened and how to recover.

### Layout Rules

- Use cream canvas with white rounded content modules.
- Use mobile bottom navigation and desktop sidebar patterns when appropriate.
- Use sidebar widths around `224px-256px` for desktop app navigation.
- Use max content widths around `max-w-5xl` to `max-w-6xl` for full product pages.
- Use a header with title/subtitle on the left and compact actions/filters on the right.
- Use 1-column mobile stacks.
- Use 3-column desktop dashboard grids.
- Use 5-column desktop analytics/list combinations when a chart and list share a page.
- Keep primary actions visible in predictable places.
- Avoid placing unrelated controls in the same toolbar.

### Responsiveness Rules

- Mobile: stack content, preserve primary actions, use bottom nav, use cards/lists before tables.
- Desktop: use sidebar plus content, multi-column grids, card-contained tables, and header-level actions.
- Keep touch targets roughly `36px-48px` where possible.
- Allow horizontal scrolling only for intentionally wide data tables or carousels.
- Convert dense tables into list rows or cards on small screens when comparison is not the main task.
- Move advanced filters into sheets or dialogs on narrow viewports.
- Preserve hierarchy across breakpoints instead of merely shrinking everything.

## Visual Priority And Hierarchy Rules

Before generating a screen, determine hierarchy in this order:

1. Primary user task.
2. Primary content needed for that task.
3. Primary action.
4. Secondary actions.
5. Status, risk, validation, or feedback.
6. Supporting metadata.
7. Optional or advanced details.

Apply visual weight accordingly:

- High priority: strong contrast, larger or heavier type, dominant placement, or forest/lime surface.
- Medium priority: clear but quieter controls, white/cream surfaces, semibold text.
- Low priority: muted metadata, smaller type, reduced opacity, tertiary placement.
- Risk priority: destructive or warning styling only when consequences justify it.

For this project, the ideal hierarchy often feels like:

- Cream canvas.
- One forest or lime focal surface.
- White rounded content panels.
- Bold compact section labels.
- Strong numbers or names.
- Muted metadata.
- Soft hover and focus states.

## Typography As UX Rules

Typography must guide scanning and reduce cognitive effort.

- Use page titles as location markers.
- Use section titles as scan anchors.
- Use large extra-bold values only for important totals, balances, or metrics.
- Use concise row titles with secondary metadata beneath.
- Use helper text only when it prevents mistakes.
- Use error text that tells the user how to fix the problem.
- Use action labels that state the result, such as “Add card,” “Save changes,” “Invite member,” or “Apply filters.”
- Avoid long explanations inside cards, tables, forms, and settings rows.
- Do not use all caps for hierarchy unless matching an existing compact label pattern.
- Keep terminology consistent across navigation, headers, buttons, empty states, and alerts.

## Interaction Rules

The interaction model is restrained, precise, and accessible.

### Buttons

- One primary button per task area.
- Forest primary for secure, major, or high-authority actions.
- Lime primary for constructive, optimistic, add/create, or signature actions.
- White or cream secondary buttons with light borders.
- Ghost or text buttons for low-priority actions.
- Destructive buttons only for destructive actions.
- Use loading states on the button that initiated the action.
- Preserve layout during hover, active, disabled, and loading states.

### Links

- Use links for navigation.
- Use buttons for actions.
- Avoid styling a destructive action as a casual link unless it is clearly separated and labeled.

### Menus

- Use menus for overflow actions.
- Keep menu items compact and readable.
- Use red only for destructive menu items.
- Do not hide essential primary actions only in menus.

### Focus

- Every interactive element needs a visible focus state.
- Focus should use the app’s lime/forest focus language, not browser-blue defaults.
- Focus order must match visual and task order.

### Motion

- Use quick color, opacity, shadow, or subtle scale transitions.
- Screen transitions may slide over roughly `320ms` with a standard ease.
- Avoid bounce, large transforms, parallax, animated decoration, or motion that distracts from tasks.

## Layout And Page Composition Rules

### Page Recipe

Use this default structure for new product screens:

1. Cream canvas.
2. Header with short title, muted subtitle, and 1 primary action plus optional compact filters.
3. Dominant metric, status, or action surface when useful.
4. White rounded panels for main content.
5. Compact rounded rows, cards, or table containers.
6. Muted metadata and restrained secondary actions.
7. Complete empty, loading, error, selected, disabled, and responsive states.

### Dashboard Composition

- Lead with decision-relevant metrics.
- Use one forest or lime hero card per major dashboard region.
- Use white rounded-3xl metric cards for supporting stats.
- Use rounded chart bars and forest/lime chart colors first.
- Group metrics by user question, not arbitrary card count.
- Avoid decorative charts that do not support decisions.
- Provide clear drill-down paths.

### CRUD Composition

- List pages should include search, filters, create action, records, empty/loading/error states, and row actions.
- Detail pages should show identity, status, key metadata, primary actions, related records, and destructive actions separated.
- Create/edit pages should use grouped white rounded form panels.
- After create/update/delete, show clear feedback and preserve useful context.
- Prefer rounded rows and card-contained tables over raw grid-heavy layouts.

### Settings Composition

- Group settings by user mental model.
- Use white rounded cards containing compact settings rows.
- Each row should have an icon well, title, optional subtitle, current value/status, and chevron or control.
- Separate dangerous settings into their own lower-emphasis or red-accent section.
- Make save behavior obvious.
- Show unsaved changes when relevant.

### Forms Composition

- Use one-column forms on mobile.
- Use two-column desktop grouping only when it improves scanning.
- Group related fields in white rounded-3xl panels.
- Use visible labels, concise helper text, and inline errors.
- Use lime or forest submit actions.
- Keep cancel/destructive actions visually separated from submit.
- Use dedicated pages instead of modals for long or complex forms.

### Table Composition

- Use tables only when precise comparison across shared attributes matters.
- Place tables inside white rounded-3xl card containers.
- Use muted compact headers.
- Use `text-sm` body cells and bold important values.
- Keep row height readable, roughly `h-12` to `h-14`.
- Use sparse dividers and cream hover states.
- Use semantic compact badges for status.
- Provide responsive list fallback on mobile when possible.

## Component Rules

### Dashboards

- Use a cream page background.
- Start with a hero metric or status card when the page needs a strong anchor.
- Use forest/lime for the most important card only.
- Use white rounded support cards.
- Keep charts simple, rounded, and readable.
- Include trends, comparison, or thresholds when a number alone is not meaningful.
- Avoid disconnected card grids with no user question.

### Settings Pages

- Use sectioned white rounded panels.
- Use compact rows with icon wells.
- Use muted subtitles for consequences or current state.
- Use toggles for immediate on/off settings.
- Use chevrons for navigational settings.
- Place destructive or security-sensitive settings separately.
- Do not bury critical billing, permissions, or security settings.

### CRUD Pages

- Use header-level create action.
- Place common filters near the list.
- Use compact filter chips/selects.
- Use rounded rows or card-contained tables.
- Use overflow menus for secondary row actions.
- Separate destructive actions.
- Include empty, filtered-empty, loading, and error states.

### Forms

- Use white rounded form cards on cream.
- Use forest labels and muted helper text.
- Use branded rounded inputs, ideally `rounded-xl` or `rounded-2xl`.
- Use lime focus rings and destructive invalid states.
- Use clear field grouping.
- Preserve input after validation errors.
- Prefer specific submit labels.

### Tables

- Use card-contained tables.
- Avoid dense full grid lines.
- Keep headers muted and compact.
- Use semantic badges and right-aligned numbers.
- Use cream row hover.
- Use row expansion or detail drawers for secondary metadata.
- Convert to list cards on mobile when precise comparison is less important.

### Analytics Blocks

- Use white rounded-3xl chart cards or forest/lime summary cards.
- Use forest and lime as first chart colors.
- Use rounded bars and minimal axes.
- Use tiny muted legends.
- Avoid dense chart grids.
- Pair every chart with a clear summary or decision point.
- Keep analytics visually calm and financially precise.

### Dialogs

- Use dialogs for short focused tasks, confirmations, lightweight creation, and destructive confirmation.
- Use white surfaces, black overlay, forest title, muted description, and rounded-3xl branded geometry.
- Use lime or forest primary action.
- Use ghost/white secondary action.
- Use pale red accents for destructive confirmations.
- Do not use dialogs for complex multi-step workflows.

### Navigation

- Mobile navigation: white bottom bar, compact labels, active forest state, optional central lime action.
- Desktop navigation: white sidebar on cream, light border, logo/header, grouped nav, active forest pill with lime dot.
- Inactive items should be muted and hover to cream/forest.
- Keep primary navigation stable.
- Do not mix navigation, filters, and destructive actions without clear separation.

### Cards

- Major cards: white, forest, or lime, rounded-3xl.
- Standard cards: white rounded-3xl with `shadow-sm`.
- Secondary rows/cards: rounded-2xl.
- Payment or financial cards may use strong forest/lime contrast and compact typography.
- Cards should have one clear purpose.
- Do not put cards inside cards unless the nested card is a distinct repeated object.

### Empty States

- Use dashed rounded containers for add/new/first-use states.
- Use white rounded panels for larger empty states.
- Include muted icon well, concise title, short explanation, and one primary action.
- For filtered empty states, provide clear reset or search adjustment.
- Avoid decorative emptiness with no next step.

### Alerts

- Use calm card-like alerts.
- Include an icon well, short title, and concise explanation.
- Use pale red for destructive alerts, not large saturated red blocks unless the action is irreversible.
- Use inline alerts near the affected content when possible.
- Avoid stacking multiple alerts without priority.

### Filters

- Use compact chips, pills, selects, or search controls.
- Place filters near the data they affect.
- Show active filters visibly.
- Provide clear reset behavior.
- Use advanced filters in a sheet or dialog.
- Selected filters should use forest fill, lime/forest border, or a clear active chip style.
- Do not hide active constraints inside menus without visible summary.

## Derived Component Rules

When generating a component that does not exist in the source repository, derive it from the source system instead of inventing a new style family.

Use this derivation process:

1. Identify the component’s job.
2. Match it to the closest existing source pattern.
3. Preserve source tokens: cream, white, forest, lime, muted, semantic green/red.
4. Preserve source geometry: rounded-xl, rounded-2xl, rounded-3xl, rounded-full.
5. Preserve source spacing: compact but breathable.
6. Preserve source hierarchy: strong numbers/names, short labels, muted metadata.
7. Preserve source interaction tone: subtle hover, lime focus, low elevation.
8. Add only the minimum new behavior required by the task.

Examples:

- A kanban board should use cream canvas, white rounded columns, rounded task cards, forest labels, muted metadata, and lime/forest selected or primary states.
- A permissions matrix should be card-contained, low-divider, rounded, and compact, with clear role/status badges.
- A billing page should use a forest or lime focal summary card, white rounded invoice/payment panels, compact rows, and semantic amount colors.
- A search results page should use rounded white result rows/cards, compact filters, muted snippets, and forest/lime selected states.
- An audit log should use a card-contained table or timeline with sparse dividers, muted timestamps, rounded status badges, and restrained emphasis.

Derived components may become more utilitarian, but they must remain visibly part of the same warm fintech system.

## Constraints

The AI must never:

- Replace the cream canvas with generic gray or pure white page defaults.
- Replace forest/lime brand states with blue SaaS defaults.
- Introduce sharper geometry when the source uses rounded language.
- Make sharp rectangular cards, square primary buttons, or hard-edged panels dominant.
- Flatten or neutralize the spacious compact rhythm into cramped generic admin UI.
- Break spacing rhythm with arbitrary gaps and padding.
- Create inconsistent hierarchy where all cards, actions, and labels compete equally.
- Use decorative elements without functional value.
- Overuse heavy shadows, glassmorphism, glow, gradients, or ornamental effects.
- Make every card saturated or visually loud.
- Use dense divider-heavy tables as the default representation for financial or operational data.
- Use large bodies of low-contrast explanatory text.
- Let generic primitive defaults visually dominate branded product screens.
- Use lime for arbitrary decoration.
- Overcomplicate interactions with unnecessary flows, hidden controls, or novelty patterns.
- Invent unsupported component patterns without grounding them in source identity.
- Hide essential actions or information behind hover-only behavior.
- Use color-only status communication.
- Place destructive actions beside constructive primary actions without separation.
- Use modals for complex workflows that need dedicated pages.

## Anti-Drift Rules

Use these rules to prevent style drift over time.

- Start every new screen from the source identity: cream canvas, forest authority, lime accent, white rounded surfaces, compact hierarchy.
- Compare every new component against an existing pattern before creating a new one.
- Prefer finance-screen patterns over generic shadcn defaults when they conflict.
- Keep visible branded surfaces in the large-radius family.
- Preserve the balanced-compact spacing rhythm.
- Keep one dominant visual anchor per section.
- Use forest/lime active and primary states consistently.
- Keep metadata muted and concise.
- Use semantic colors only for semantic meaning.
- Avoid adding new colors unless the role is necessary and reusable.
- Avoid adding new radii unless the component has a distinct system role.
- Avoid adding new shadows unless there is a real elevation layer.
- Avoid adding new interaction behavior unless it improves task completion.
- Review new UI against the non-negotiable traits before finalizing.
- If a screen begins to look like a generic admin template, reintroduce the project DNA through radius, spacing, color hierarchy, and compact financial-style information grouping.

## Final Operating Instructions

When generating UI for this project:

- Prefer product-ready interface design over conceptual mockups.
- Reuse existing patterns first.
- Extend the system instead of reinventing it.
- Preserve the source design identity across all UI categories.
- Generate components that feel native to the existing app.
- Make key decisions explainable through clarity, hierarchy, visual priority, consistency, task completion, accessibility, and scalability.
- Include complete states for hover, focus, active, selected, disabled, loading, empty, error, validation, and responsive behavior when relevant.
- Use conservative adaptation when translating the design language into new product areas.

A portfolio, marketing page, or landing style may be adapted into dashboards, CRUD pages, settings, and utility screens, but the defining traits must remain recognizable: **soft rounded geometry, warm cream canvas, forest/lime hierarchy, compact spacing character, disciplined emphasis, bold financial typography, and calm interaction tone**.