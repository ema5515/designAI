---
name: Warm Fintech Minimalism
description: Generate warm, premium operational UI with cream canvas, forest green hierarchy, lime accents, rounded cards, and calm data density.
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

- Root: `/Users/emanueledagata/code/v0/boh2`
- Detected hints: Next.js, Tailwind CSS, shadcn/ui, Charts, Radix/Lucide
- Total indexed files: 92
- Relevant UI/design files: 89

## Key dependencies

- @radix-ui/react-dialog: 1.1.15
- @radix-ui/react-dropdown-menu: 2.1.16
- @radix-ui/react-select: 2.2.6
- @radix-ui/react-tabs: 1.1.13
- class-variance-authority: ^0.7.1
- clsx: ^2.1.1
- lucide-react: ^0.564.0
- next: 16.1.6
- react: 19.2.4
- react-dom: 19.2.4
- recharts: 2.15.0
- tailwind-merge: ^3.3.1
- tailwindcss: ^4.2.0

## Key analysis goals

- Extract the source design language from the repository.
- Identify explicit and inferred design-system rules.
- Preserve radius, spacing character, hierarchy, typography roles, and interaction tone.
- Produce a reusable design skill for generating new UI categories consistently.
- Prevent style drift when adapting to dashboards, forms, CRUD, or utility-heavy interfaces.


# Final Design Skill

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

# Structured Style Profile

```json
{
  "style_name": "Warm Fintech Minimalism",
  "visual_identity": {
    "tone": "Premium, calm, optimistic fintech with a tactile wallet-app feel.",
    "density": "Balanced-compact: mobile screens use tight finance-app rhythm while preserving touch targets and breathing room.",
    "corner_style": "Large rounded geometry dominates; rounded-2xl and rounded-3xl are the visible brand shapes, with pills for avatars, dots, and nav accents.",
    "elevation_style": "Low elevation inside the app: mostly shadow-sm, light borders, and color contrast. Strong shadows are reserved for demo device/browser chrome.",
    "contrast_profile": "Warm cream canvas, white surfaces, deep forest primary content, lime signature accents, and semantic green/red for financial values.",
    "mood": "Trustworthy, soft, modern, financially precise, and lightly expressive without feeling playful.",
    "notes": [
      "EXPLICIT: app/globals.css defines cream, forest, lime, white card, muted, border, ring, chart, and radius tokens.",
      "EXPLICIT: components/finance/* repeatedly use bg-cream, bg-white, bg-forest, bg-lime, rounded-2xl, rounded-3xl, shadow-sm, compact labels, and bold financial values.",
      "EXPLICIT: app/layout.tsx uses Plus Jakarta Sans with weights 400, 500, 600, 700, and 800.",
      "INFERRED: new product areas should preserve wallet-app tactility and avoid generic gray/blue SaaS styling."
    ]
  },
  "identity_traits": {
    "non_negotiable_traits": [
      "Cream page background instead of generic gray or pure white app canvas.",
      "Forest green as primary text, navigation, and high-emphasis action color.",
      "Lime as the signature accent for constructive actions, active highlights, rings, dots, and key chart bars.",
      "Large soft radii for visible surfaces and controls: 16px-24px as the normal brand range.",
      "Compact finance hierarchy: short labels, muted metadata, extra-bold totals, right-aligned amounts, and semantic positive/negative colors.",
      "Subtle interaction feedback: restrained hover fills, lime focus rings, light scale on major CTAs, and minimal shadow escalation."
    ],
    "adaptable_traits": [
      "Tables and forms may become more structured for CRUD workflows if they stay card-contained, rounded, and low-divider.",
      "Primitive shadcn radii may remain smaller for dense internal controls, but branded surfaces should use larger finance radii.",
      "Forest and lime hero cards may be used selectively; not every card should be saturated.",
      "Secondary accent colors may appear in avatars or charts, but they should not overtake the forest/lime identity.",
      "Desktop sidebars and page headers can become more utilitarian if active states remain forest/lime and surfaces remain cream/white."
    ],
    "source_type": "Explicit repo evidence plus conservative inference from finance screens and shadcn/ui primitives.",
    "adaptation_notes": [
      "Treat finance screens as stronger identity evidence than generic shadcn primitives.",
      "When primitive defaults conflict with custom finance screens, prefer the finance screen visual language for branded product UI.",
      "For missing branded implementations, infer only from token roles, radius system, spacing rhythm, and observed UX patterns."
    ]
  },
  "tokens": {
    "colors": {
      "primary": "oklch(0.28 0.07 145) / var(--forest), observed hex #1B3A2D; use for primary text, active navigation, major CTAs, dark cards.",
      "secondary": "oklch(0.96 0.03 100) / var(--secondary) and oklch(0.93 0.025 100) / var(--cream-dark); use for soft grouped surfaces and rows.",
      "accent": "oklch(0.88 0.22 120) / var(--lime), observed hex #C8E63A; use for constructive actions, highlights, rings, active dots, and chart-1.",
      "neutral": [
        "background: oklch(0.97 0.015 100) / var(--cream)",
        "surface: oklch(1 0 0) / white card surfaces",
        "muted: oklch(0.94 0.02 100) / var(--muted)",
        "border/input: oklch(0.90 0.02 100)",
        "demo chrome gradient only: #4a8fa8, #3d7a8a, #2d6070"
      ],
      "success": "Tailwind green utilities are explicit for positive values: text-green-600 and text-green-500; use for income, verified, success, and positive deltas.",
      "warning": "No dedicated warning token; amber #F59E0B appears as an avatar color only. Infer amber for warnings sparingly, with cream/white containment.",
      "danger": "oklch(0.577 0.245 27.325) / var(--destructive), plus text-red-500 and bg-red-50 for negative values and destructive actions.",
      "background": "oklch(0.97 0.015 100) / var(--background), var(--cream); main app canvas.",
      "surface": "oklch(1 0 0) / var(--card); cards, lists, popovers, nav bars.",
      "text": {
        "primary": "oklch(0.18 0.04 145) / var(--foreground) and var(--forest); headings, labels, nav, icons.",
        "secondary": "Forest at reduced opacity or secondary-foreground; row labels and less dominant content.",
        "muted": "oklch(0.52 0.03 145) / var(--muted-foreground); captions, metadata, helper text.",
        "inverse": "oklch(0.98 0 0) / primary-foreground or white; text on forest cards and dark demo chrome."
      },
      "border": "oklch(0.90 0.02 100) / var(--border); also border-white/10, border-forest/20, and dashed border-border for add/empty actions."
    },
    "spacing": {
      "density": "Balanced-compact, optimized for finance dashboards and mobile wallet screens.",
      "section_gap": [
        "mobile primary stack: space-y-4",
        "desktop grids: gap-4",
        "onboarding/marketing-like panels: mb-8, mb-10, mt-12, pt-8",
        "major desktop page padding: p-6"
      ],
      "card_gap": [
        "compact list rows: space-y-2 or space-y-3",
        "card internals: gap-2, gap-2.5, gap-3",
        "horizontal carousels/actions: gap-3 or gap-4",
        "desktop multi-card dashboards: gap-4"
      ],
      "control_gap": [
        "icon-label controls: gap-2 or gap-2.5",
        "tight metadata: gap-0.5 to gap-1.5",
        "button groups/view switchers: p-1 container with gap-1",
        "action rows: justify-around or compact flex gap"
      ],
      "grouping_pattern": "Group information into digestible modules: balance, cards, actions, quick send, transactions, chart, settings rows. Prefer spacing and soft background shifts over many dividers.",
      "adaptation_rule": "For new utility screens, use 24px page padding, 16px grid gaps, 20px card padding, 12px list-row padding, and compact filter chips rather than large form panels by default."
    },
    "radius": {
      "control": "12px-16px for compact controls; 16px for branded primary buttons and action tiles.",
      "container": "22px-24px for major cards and panels; rounded-3xl is the common finance card shape.",
      "overlay": "16px in generic shadcn dialogs, inferred 24px for branded finance dialogs/sheets.",
      "pill": "9999px / rounded-full for avatars, nav dots, progress dots, home indicators, chart bars, and circular icon wells.",
      "dominant_family": "Soft rounded-xl, rounded-2xl, rounded-3xl, rounded-full.",
      "sharp_allowed": "Only for tiny decorative elements, chart internals, table grid internals, or demo/browser chrome details; not for primary user-facing cards or buttons.",
      "style_rule": "Visible branded surfaces should default to large radii. Primitive rounded-md may remain for dense low-emphasis internals but should not define the page character."
    },
    "shadows": [
      "shadow-sm for standard white cards, transaction rows, icon buttons, and active segmented controls.",
      "shadow-md only as a subtle hover escalation on some profile/stat rows.",
      "shadow-lg for the central mobile QR action and important floating CTAs.",
      "Large custom shadows are explicit on phone/browser demo frames only and should not be copied into normal app surfaces."
    ],
    "typography": {
      "font_families": [
        "Plus Jakarta Sans via next/font/google and --font-plus-jakarta",
        "Geist Mono only as theme mono fallback"
      ],
      "scale": [
        "caption/card microcopy: text-[8px] to text-[10px]",
        "metadata/supporting: text-xs",
        "body/list rows/buttons: text-sm",
        "mobile titles/section emphasis: text-base to text-xl",
        "desktop page titles: text-2xl",
        "financial totals: text-3xl to text-4xl"
      ],
      "font_weights": [
        "400 body copy",
        "500 labels and subdued controls",
        "600 buttons, rows, important labels",
        "700 section titles and mobile titles",
        "800 page titles and financial totals",
        "font-black only for compact brand/card-network marks"
      ],
      "line_heights": [
        "leading-none for labels and primitive controls",
        "leading-tight for headings and totals",
        "leading-relaxed for longer body/onboarding copy"
      ]
    },
    "widths": [
      "mobile phone demo: 300px wide, 620px high",
      "desktop demo/content shell: max-w-5xl",
      "desktop sidebar observed: w-56 / 224px in finance app",
      "generic sidebar primitive: 16rem desktop, 18rem mobile, 3rem icon-collapsed",
      "mobile content padding: px-4 and px-5 headers",
      "onboarding content panel: px-7 mobile, px-14 py-12 desktop"
    ],
    "breakpoints": [
      "sm and md responsive classes in primitives and screens",
      "container-query behavior in sidebar primitives",
      "mobile: bottom navigation and vertical stack",
      "desktop: sidebar plus content, 3-column and 5-column grids"
    ]
  },
  "hierarchy": {
    "primary_focus_pattern": "Lead with one strong financial anchor per view: a large balance, forest/lime hero card, active navigation state, or primary CTA. Use weight and color before heavy decoration.",
    "secondary_content_pattern": "Secondary content appears as white cards, rounded list rows, muted metadata, small labels, and soft cream grouped surfaces.",
    "cta_hierarchy": "Primary CTAs use forest fill with white text or lime fill with forest text. Secondary actions use white/cream surfaces with light borders or muted text. Tertiary actions are small icon-only or text links.",
    "emphasis_rules": [
      "Reserve lime for signature actions, active indicators, chart highlights, and key positive moments.",
      "Use forest for authority: headings, selected nav, primary text, dark summary cards, and secure/major actions.",
      "Use extra-bold type for balances, totals, and page-level metrics; avoid making every label large.",
      "Use semantic green/red only for financial meaning, not general decoration.",
      "Use color blocks sparingly so one card or action remains dominant in a section."
    ],
    "grouping_rules": [
      "Prefer card/list modules over dense raw grids.",
      "Represent transactions as rows with icon well, primary label, secondary metadata, right-aligned amount, and category.",
      "Use rounded icon wells to make action groups scannable.",
      "Use dashed rounded containers for add/new/empty actions.",
      "Keep dividers sparse; use spacing, background, and radius to separate groups."
    ],
    "contrast_usage": "High contrast for primary numbers and active actions; low-noise contrast for metadata, borders, and hover states. Avoid low-contrast long text blocks."
  },
  "typography_roles": {
    "page_title": "Desktop: text-2xl font-extrabold text-forest. Mobile: text-base to text-xl font-bold, usually short location labels such as Transactions, My Cards, Profile.",
    "section_title": "text-sm or text-xs font-bold text-forest with tight margins; labels such as Quick Send, Recent Transactions, Actions.",
    "body": "text-sm or text-xs, forest or foreground, medium/semibold in rows; concise product copy rather than long explanations.",
    "supporting_text": "text-xs or text-[10px] text-muted-foreground; used for dates, subtitles, helper copy, categories, descriptions.",
    "label": "text-xs to text-sm font-medium or font-semibold; controls and finance labels use compact leading and forest/muted color.",
    "caption": "text-[8px] to text-[10px], muted or opacity-reduced, especially on payment cards and transaction metadata.",
    "scanning_behavior": "Users scan by large totals first, then bold section labels, row names, right-aligned amounts, muted dates/categories, and compact action icons."
  },
  "interaction": {
    "hover": "Restrained hover feedback: hover:bg-cream, hover:bg-cream-dark, hover:bg-white/20, hover:text-forest, and occasional hover:shadow-md on rows/cards.",
    "focus": "Use lime-aligned focus: focus-visible:ring-ring/50, focus-visible:ring-[3px], border/ring tokens from app/globals.css; avoid blue default focus.",
    "active": "Major CTAs may use hover:scale-[1.02] and active:scale-[0.98]; screen transitions slide horizontally over 320ms cubic-bezier(0.4,0,0.2,1).",
    "selected": "Selected nav uses forest fill with white text and lime dot, or active forest icon/text in bottom nav. Segmented controls use white active surface and shadow-sm.",
    "disabled": "Generic primitives use disabled:pointer-events-none and disabled:opacity-50. Preserve subdued disabled states without changing layout.",
    "loading": "Skeleton primitive uses bg-accent animate-pulse rounded-md; inferred branded loading should use cream/lime-tinted rounded placeholders.",
    "validation": "Primitive invalid states use destructive border/ring and aria-invalid styling; errors should be concise, red, and not visually louder than the form context unless destructive.",
    "feedback_style": "Calm, crisp, touch-friendly, and low-drama. Use quick color/opacity/scale changes rather than glow, bounce, or heavy shadow."
  },
  "layout": {
    "page_shell": "Cream app canvas with mobile vertical shell or desktop sidebar/content shell. Demo wrapper uses teal gradient browser/phone chrome but app surfaces remain cream and white.",
    "page_width_strategy": "Constrain app/demo content around max-w-5xl; desktop app uses fixed presentation frame and sidebar. For real pages, infer max-w-5xl to max-w-6xl with 24px padding.",
    "header_pattern": "Title/subtitle or profile row on left, compact actions/avatar/filters on right. Mobile headers are compact; desktop headers can include page actions and filters.",
    "section_spacing": "Mobile sections stack with space-y-4 and px-4. Desktop sections use p-6 and gap-4. Onboarding can use more relaxed spacing.",
    "grid_rules": [
      "Mobile: one-column stack with horizontal carousels where needed.",
      "Desktop dashboard: 3-column grid with important balance/summary card spanning 2 columns.",
      "Transactions desktop: 5-column layout with chart spanning 2 columns and list spanning 3 columns.",
      "Cards/settings/profile modules: white rounded panels with compact rows.",
      "Use overflow-x carousels for cards and quick-send contacts on mobile."
    ],
    "navigation_patterns": [
      "Mobile bottom nav: white surface, top border, compact labels, active forest state, central floating lime QR action.",
      "Desktop sidebar: white on cream, logo header, grouped nav, active forest pill with lime dot, footer user/balance/action area.",
      "Top demo toolbar: dark translucent segmented view switcher, white active state, lime logo dot; treat as presentation chrome."
    ],
    "responsive_rules": [
      "Bottom nav on mobile, sidebar on desktop.",
      "Maintain touch-friendly icon wells around 36px-48px.",
      "Avoid collapsing hierarchy by making desktop too sparse; keep gap-4 dashboard rhythm.",
      "Use cards/lists before table grids on small screens.",
      "Filters should become chips or sheet/dialog controls on narrow viewports."
    ]
  },
  "components": {
    "buttons": {
      "explicit": true,
      "source_basis": "Explicit shadcn button primitive plus finance screen buttons in components/finance/home-screen.tsx, nav-bar.tsx, onboarding-screen.tsx, cards-screen.tsx.",
      "confidence": "high",
      "rules": {
        "purpose": "Primary progression, financial actions, navigation actions, icon actions, and secondary text links.",
        "appearance": "Primary: forest fill with white text or lime fill with forest text. Secondary: white/cream with light border. Ghost/link: muted or forest text. Icon buttons often white with border and shadow-sm.",
        "spacing": "Primitive sizes h-8, h-9, h-10; finance CTAs use py-4, px-4, w-9/h-9 to w-12/h-12 icon wells, gap-2.",
        "radius": "Primitive uses rounded-md; branded finance buttons use rounded-xl, rounded-2xl, or rounded-full.",
        "border": "Light border-border on secondary/icon buttons; no heavy outlines. Dashed border for add actions.",
        "shadow": "shadow-sm for white/icon buttons, shadow-lg for floating QR CTA, minimal otherwise.",
        "typography": "text-sm font-medium in primitive; finance buttons use text-xs to text-sm with font-semibold or font-bold.",
        "states": "Hover uses cream/white tint or lime-dark/forest-dark; active may scale to 0.98; disabled opacity 50%; focus lime ring.",
        "variants": [
          "forest-primary",
          "lime-primary",
          "white-secondary",
          "cream-ghost",
          "icon-round",
          "icon-rounded-2xl",
          "dashed-add",
          "text-link"
        ]
      }
    },
    "inputs": {
      "explicit": true,
      "source_basis": "Generic shadcn input primitive exists, but branded finance screens use forms lightly; brand adaptation is inferred from tokens and visible control geometry.",
      "confidence": "medium",
      "rules": {
        "purpose": "Text entry for forms, filters, search, and account/card workflows.",
        "appearance": "White or transparent-on-white field, forest text, muted placeholder, light border, lime/forest focus.",
        "spacing": "Primitive h-9 px-3 py-1; inferred branded input h-10 or h-11 with px-3/px-4 and gap-2 when icon-led.",
        "radius": "Primitive rounded-md; inferred branded visible inputs should use rounded-xl or rounded-2xl.",
        "border": "border-input by default; focus should strengthen ring/border in lime or forest.",
        "shadow": "No default shadow; use shadow-sm only when an input appears as a standalone filter chip/control.",
        "typography": "text-sm for value, text-xs helper/description, label font-medium or semibold.",
        "states": "Focus-visible ring-ring/50 ring-[3px]; invalid destructive border/ring; disabled opacity and cursor states from primitive.",
        "variants": [
          "text",
          "search",
          "icon-leading",
          "filter-chip-input",
          "invalid",
          "disabled"
        ]
      }
    },
    "selects": {
      "explicit": true,
      "source_basis": "shadcn/Radix select primitive exists; finance filter pills such as Monthly provide brand direction.",
      "confidence": "medium",
      "rules": {
        "purpose": "Compact filtering, period selection, account/card selection, and form options.",
        "appearance": "White or cream rounded trigger with forest text, muted placeholder, chevron, and white popover surface.",
        "spacing": "Compact triggers should use h-9/h-10, px-3, gap-2; popover items use compact row padding.",
        "radius": "Primitive rounded-md; branded selects should use rounded-xl or rounded-2xl for visible filters.",
        "border": "Light border-border/input; selected/open state may use forest border or lime ring.",
        "shadow": "Popover shadow-md; active local filter may use shadow-sm.",
        "typography": "text-sm trigger text; item labels text-sm with muted descriptions only where needed.",
        "states": "Open/focus uses lime ring; selected item uses cream background and forest text; disabled uses opacity 50%.",
        "variants": [
          "form-select",
          "period-pill",
          "filter-select",
          "account-select",
          "compact-select"
        ]
      }
    },
    "dropdowns": {
      "explicit": true,
      "source_basis": "shadcn/Radix dropdown-menu, context-menu, menubar, command, and popover primitives exist; row-level overflow actions are implied by MoreHorizontal icons.",
      "confidence": "medium",
      "rules": {
        "purpose": "Overflow actions, account menus, row actions, command-style choices, and contextual operations.",
        "appearance": "White popover/menu with light border, compact rounded rows, forest text, muted shortcuts, red destructive rows.",
        "spacing": "Menu item rows should stay compact with px-2/px-3, py-1.5/py-2, and gap-2.",
        "radius": "Primitive rounded-md; branded larger menus can use rounded-xl or rounded-2xl.",
        "border": "Light border and subtle separator only for grouping.",
        "shadow": "shadow-md or shadow-lg on floating menu surfaces.",
        "typography": "text-sm item labels; shortcuts and descriptions muted text-xs.",
        "states": "Hover/active bg-cream or bg-muted; destructive hover should remain pale red; focus follows Radix item focus styling.",
        "variants": [
          "overflow-menu",
          "account-menu",
          "row-actions",
          "command-menu",
          "context-menu",
          "destructive-action"
        ]
      }
    },
    "cards": {
      "explicit": true,
      "source_basis": "Strong explicit evidence across components/finance/*: balance cards, payment cards, stat cards, transaction rows, connect-card banner, profile/settings panels.",
      "confidence": "high",
      "rules": {
        "purpose": "Primary grouping for balances, cards, charts, transactions, actions, settings, onboarding panels, and metric summaries.",
        "appearance": "White rounded cards on cream; forest hero cards with lime highlights; lime payment/action cards with forest text; cream-dark secondary group cards.",
        "spacing": "Mobile rows p-3; standard cards p-4/p-5; major desktop cards p-6; internal gaps 2-4.",
        "radius": "rounded-2xl for rows/secondary cards; rounded-3xl for major cards and panels.",
        "border": "Usually none or light border-border; border-forest/20 for tinted surfaces; dashed border for add/empty card actions.",
        "shadow": "shadow-sm for standard white cards; hover:shadow-md only for interactive rows; saturated cards often rely on color instead of shadow.",
        "typography": "Small bold section titles, extra-bold financial totals, muted captions, right-aligned amounts.",
        "states": "Hover bg-cream for rows, subtle shadow escalation, selected/focal cards use forest/lime contrast.",
        "variants": [
          "white-standard",
          "forest-hero",
          "lime-highlight",
          "payment-card",
          "transaction-row-card",
          "settings-row",
          "dashed-add-card",
          "chart-card"
        ]
      }
    },
    "tables": {
      "explicit": true,
      "source_basis": "components/ui/table.tsx exists with generic table styles; finance-specific data is represented as list rows rather than tables.",
      "confidence": "medium",
      "rules": {
        "purpose": "Structured dense data when list cards are insufficient, especially desktop CRUD or audit views.",
        "appearance": "Card-contained table on white rounded surface; minimal dividers, muted headers, forest primary cells, semantic amount/status colors.",
        "spacing": "Primitive cells p-2; inferred branded rows h-12 to h-14 with px-3/px-4 and compact header spacing.",
        "radius": "The table container should be rounded-3xl; internal cells can remain square for grid alignment.",
        "border": "Use sparse row borders or separators; avoid dense full grid lines.",
        "shadow": "Container may use shadow-sm; rows should use hover fill rather than raised shadows.",
        "typography": "Header text text-xs font-semibold muted; body text text-sm; important values font-bold.",
        "states": "Row hover bg-muted/50 or bg-cream; selected bg-muted/cream; status badges compact and rounded.",
        "variants": [
          "card-contained-table",
          "transaction-table",
          "audit-table",
          "responsive-list-fallback"
        ]
      }
    },
    "modals": {
      "explicit": true,
      "source_basis": "Dialog, alert-dialog, drawer, sheet primitives exist; branded finance modal pattern is inferred because custom finance screens do not show many modals.",
      "confidence": "medium",
      "rules": {
        "purpose": "Focused confirmation, creation/edit forms, advanced filters, QR/payment flows, and irreversible action confirmation.",
        "appearance": "White modal over black overlay, forest title, muted description, rounded finance geometry, primary lime/forest action.",
        "spacing": "p-6 modal body; footer gap-2/gap-3; use compact form spacing inside.",
        "radius": "Primitive rounded-lg; inferred branded modals should use rounded-3xl where product-facing.",
        "border": "Light border-border; destructive confirmations may use pale red accents.",
        "shadow": "shadow-lg on modal surface; overlay handles separation.",
        "typography": "Title text-lg/text-xl font-bold or extrabold forest; description text-sm muted.",
        "states": "Overlay fade, content zoom/slide from primitives; focus trap and focus-visible lime ring.",
        "variants": [
          "confirmation",
          "form-modal",
          "advanced-filter",
          "destructive-confirmation",
          "qr-payment-modal"
        ]
      }
    },
    "dialogs": {
      "explicit": true,
      "source_basis": "components/ui/dialog.tsx and alert-dialog.tsx define Radix dialog patterns; brand adaptation inferred from finance identity.",
      "confidence": "medium",
      "rules": {
        "purpose": "Dialog-level decisions, small forms, confirmation, and alert flows.",
        "appearance": "White surface, black overlay, forest heading, muted description, lime or forest primary action.",
        "spacing": "p-6 content; footer flex gap-2; descriptions and titles stacked compactly.",
        "radius": "Primitive rounded-lg; branded dialog should move to rounded-2xl/3xl for visible product dialogs.",
        "border": "Light border and focus-managed content.",
        "shadow": "shadow-lg on dialog content.",
        "typography": "Dialog title font-semibold/bold; finance title can be text-xl font-extrabold text-forest.",
        "states": "Open/closed animation from Radix data-state; close icon subdued hover opacity; invalid fields destructive.",
        "variants": [
          "standard-dialog",
          "alert-dialog",
          "form-dialog",
          "destructive-dialog"
        ]
      }
    },
    "sidebars": {
      "explicit": true,
      "source_basis": "components/ui/sidebar.tsx primitive plus explicit desktop finance sidebar/navigation in components/finance/desktop-views.tsx.",
      "confidence": "high",
      "rules": {
        "purpose": "Desktop primary navigation, account context, balance summary, QR/action entry, and user footer.",
        "appearance": "White sidebar on cream page, light right border, logo header, active forest nav pill with white text and lime dot, muted inactive rows.",
        "spacing": "Finance sidebar observed w-56, p-4/p-6 patterns, nav row px-3 py-2.5, grouped vertical gaps.",
        "radius": "Active nav rows rounded-2xl; logo well rounded-xl; footer cards rounded-2xl/3xl.",
        "border": "Border-right or light surface separation; internal dividers sparse.",
        "shadow": "Avoid heavy sidebar shadow; rely on white/cream contrast and border.",
        "typography": "Nav labels text-sm font-semibold; footer/user metadata text-xs muted.",
        "states": "Inactive hover bg-cream and text-forest; active forest fill; collapsed primitive supports icon width 3rem.",
        "variants": [
          "desktop-finance-sidebar",
          "collapsible-sidebar",
          "icon-sidebar",
          "footer-balance-sidebar"
        ]
      }
    },
    "tabs": {
      "explicit": true,
      "source_basis": "components/ui/tabs.tsx primitive and explicit demo view switcher/segmented controls in finance-app.tsx.",
      "confidence": "medium",
      "rules": {
        "purpose": "View switching, local filters, segmented modes, and high-level content categories.",
        "appearance": "Muted/cream or translucent pill container; active segment white with forest text and shadow-sm, or forest fill for high-level active state.",
        "spacing": "Container p-1 gap-1; segments px-3/px-4 py-2, text-sm.",
        "radius": "Container rounded-2xl; active item rounded-xl or rounded-2xl.",
        "border": "Usually borderless; optional light border when on white surface.",
        "shadow": "shadow-sm for active segment only.",
        "typography": "text-sm font-semibold for segment labels; icons 14px-16px when present.",
        "states": "transition-all duration-200; inactive text muted with hover stronger; selected uses white or forest active treatment.",
        "variants": [
          "segmented-view-switcher",
          "local-filter-tabs",
          "high-level-tabs",
          "icon-tabs"
        ]
      }
    },
    "badges": {
      "explicit": true,
      "source_basis": "components/ui/badge.tsx exists; finance screens use small pills/dots/trust badges and semantic transaction colors.",
      "confidence": "medium",
      "rules": {
        "purpose": "Status, trust, category, filter count, notification, chart legend, and compact finance metadata.",
        "appearance": "Compact rounded labels using cream, lime/forest, semantic green/red, or muted backgrounds; notification dots are red or lime.",
        "spacing": "px-2 py-0.5 or tiny dot sizes 2px-8px; keep text concise.",
        "radius": "rounded-lg, rounded-full, or small pill shape.",
        "border": "Optional light border for outline/neutral badges; semantic badges can use tint backgrounds.",
        "shadow": "No shadow by default.",
        "typography": "text-[9px] to text-xs, font-medium or font-semibold.",
        "states": "Interactive badges hover cream/forest; selected badges may use forest fill or lime fill.",
        "variants": [
          "status",
          "category",
          "trust",
          "notification-dot",
          "chart-legend",
          "filter-count",
          "destructive"
        ]
      }
    },
    "alerts": {
      "explicit": true,
      "source_basis": "components/ui/alert.tsx exists; destructive and negative patterns are present, but custom finance alerts are inferred.",
      "confidence": "medium",
      "rules": {
        "purpose": "Informational messages, validation summaries, destructive warnings, and financial risk confirmations.",
        "appearance": "Calm card-like alert with icon well, short title, muted explanation; destructive uses red text/pale red background.",
        "spacing": "p-4 to p-5, gap-3 between icon and copy, compact action footer if needed.",
        "radius": "Primitive rounded-lg; branded alerts should use rounded-2xl.",
        "border": "Light border; destructive border can be red-tinted but not saturated.",
        "shadow": "Usually no shadow or shadow-sm if floating in a panel.",
        "typography": "Title text-sm font-semibold/bold; description text-xs/text-sm muted.",
        "states": "No flashy animation; dismiss/secondary action hover follows cream/forest pattern.",
        "variants": [
          "info",
          "success",
          "warning",
          "destructive",
          "validation-summary",
          "inline-alert"
        ]
      }
    },
    "empty_states": {
      "explicit": true,
      "source_basis": "components/ui/empty.tsx exists and finance Add Card/Add contact patterns explicitly use dashed rounded controls.",
      "confidence": "medium",
      "rules": {
        "purpose": "No cards, no transactions, no results, add-new slots, and first-run setup prompts.",
        "appearance": "Dashed rounded container or white rounded card with muted icon, concise title, muted copy, one lime/forest action.",
        "spacing": "p-5/p-6 for empty panels; compact add slots can be w-8/h-8 or larger rounded tiles.",
        "radius": "rounded-2xl for small add controls; rounded-3xl for panel empty states.",
        "border": "border-2 border-dashed border-border for add/new; light border for full empty panels.",
        "shadow": "No heavy shadow; optional shadow-sm for white panel.",
        "typography": "Title text-sm/base font-bold forest; description text-xs/sm muted.",
        "states": "Hover bg-cream or border-forest/20; primary action follows lime/forest CTA rules.",
        "variants": [
          "dashed-add",
          "no-results",
          "first-run",
          "empty-transactions",
          "empty-cards"
        ]
      }
    },
    "charts_containers": {
      "explicit": true,
      "source_basis": "app/globals.css chart tokens, components/ui/chart.tsx, and desktop finance chart/list patterns.",
      "confidence": "high",
      "rules": {
        "purpose": "Spending trends, balances, income/expense comparison, compact analytics summaries.",
        "appearance": "White rounded-3xl card or forest/lime summary card; rounded bars; forest/lime first; tiny muted legends/axis labels.",
        "spacing": "Card p-5/p-6; chart and summary gaps around 3-4; labels compact.",
        "radius": "Container rounded-3xl; bars rounded-full or rounded tops where possible.",
        "border": "Usually none or light border; avoid dense chart grid borders.",
        "shadow": "shadow-sm container; chart internals flat.",
        "typography": "Summary numbers font-extrabold; legends text-[10px]/text-xs muted; labels compact.",
        "states": "Tooltips use white/cream popover with border/shadow; active datapoint should use forest/lime emphasis.",
        "variants": [
          "bar-chart-card",
          "summary-chart",
          "forest-chart-card",
          "lime-highlight-chart",
          "tooltip-container"
        ]
      }
    },
    "page_headers": {
      "explicit": true,
      "source_basis": "Finance mobile headers/profile rows and desktop views show title/action patterns; generic page header primitive is absent.",
      "confidence": "medium",
      "rules": {
        "purpose": "Orient the user, expose page-level actions, filters, notifications, and profile context.",
        "appearance": "Left title/subtitle or profile identity; right compact icon buttons/avatar/filter chips; forest text on cream canvas.",
        "spacing": "Mobile px-4/px-5 and compact vertical padding; desktop p-6 with flex justify-between and gap-4.",
        "radius": "Header itself unframed; contained actions use rounded-full, rounded-xl, or rounded-2xl.",
        "border": "No header border by default; nav bars may use top/bottom border-border.",
        "shadow": "No header shadow; icon buttons may use shadow-sm.",
        "typography": "Desktop title text-2xl font-extrabold forest; mobile title text-base-xl font-bold; subtitle text-sm muted.",
        "states": "Header action hover bg-cream/cream-dark; notification dot red; active filters forest/lime.",
        "variants": [
          "mobile-profile-header",
          "desktop-page-header",
          "title-action-header",
          "filter-header"
        ]
      }
    },
    "filters": {
      "explicit": true,
      "source_basis": "Explicit compact filter controls appear in finance transactions/desktop views; select/dropdown primitives support inferred advanced filters.",
      "confidence": "medium",
      "rules": {
        "purpose": "Period, category, status, account, search, and transaction narrowing.",
        "appearance": "Compact chips/pills, white or cream surface, light border, muted label, forest selected state, chevron for dropdown filters.",
        "spacing": "px-3/px-4 py-2, h-9/h-10, gap-2; page-level filters sit in header right or above list.",
        "radius": "rounded-xl, rounded-2xl, or rounded-full depending chip density.",
        "border": "Light border-border; selected can use forest fill or lime/forest border.",
        "shadow": "shadow-sm only for active white segment or floating popover.",
        "typography": "text-xs/text-sm font-semibold; helper count text-xs muted.",
        "states": "Hover bg-cream; selected forest fill or white active with shadow-sm; advanced filters open sheet/dialog.",
        "variants": [
          "period-pill",
          "category-chip",
          "search-filter",
          "status-chip",
          "advanced-filter-sheet",
          "header-filter"
        ]
      }
    },
    "form_layouts": {
      "explicit": true,
      "source_basis": "components/ui/form.tsx and field primitives exist; custom finance form screens are not prominent, so layout adaptation is inferred.",
      "confidence": "medium",
      "rules": {
        "purpose": "Account setup, transfer creation, card management, profile settings, and advanced filters.",
        "appearance": "White rounded-3xl grouped panels on cream canvas, forest labels, muted descriptions, lime/forest primary actions.",
        "spacing": "One-column mobile forms with gap-4; desktop two-column groups where useful; panel p-5/p-6; field helper spacing compact.",
        "radius": "Form panels rounded-3xl; fields rounded-xl/2xl when branded; buttons rounded-2xl.",
        "border": "Light panel/field borders; invalid destructive border/ring; avoid dense section dividers.",
        "shadow": "Panel shadow-sm; no heavy elevation.",
        "typography": "Labels text-sm font-medium/semibold; descriptions text-xs muted; errors text-xs destructive.",
        "states": "Validation via aria-invalid destructive styles; focus lime ring; disabled opacity 50%.",
        "variants": [
          "mobile-single-column",
          "desktop-two-column",
          "grouped-card-form",
          "inline-filter-form",
          "destructive-confirm-form"
        ]
      }
    }
  },
  "ux_patterns": {
    "cta_hierarchy": "Primary page/action CTAs are visually isolated and use lime or forest. Secondary actions are compact white/cream buttons or text links. Tertiary actions are icon-only, muted, or hidden behind overflow menus.",
    "information_grouping": "Group financial information into modules: balance, cards, actions, quick-send people, transactions, charts, settings. Use rounded white cards and rows on cream rather than full-page grids.",
    "filter_placement": "Place common filters in the page header or just above the affected list as compact chips/selects. Put advanced filters in a sheet/dialog instead of expanding dense inline panels.",
    "form_structure": "Use short labels, one-column mobile forms, two-column desktop grouping only when it improves scanning, and rounded white form cards for related fields.",
    "validation_behavior": "Use inline destructive text and destructive border/ring states; keep wording concise and avoid large saturated alert blocks except for irreversible financial actions.",
    "table_detail_strategy": "Prefer transaction/list cards for primary workflows. Use card-contained tables for dense desktop data, with minimal dividers, muted headers, semantic badges, and responsive list fallback on mobile.",
    "loading_error_empty_states": "Use rounded skeletons, calm card-like alerts, and dashed rounded empty/add states. Preserve forest/lime CTAs for resolution actions.",
    "action_placement": "Primary action in header or dominant card; row actions at the right or overflow; mobile primary actions can be full-width or floating only when central to the workflow.",
    "notes": [
      "Progressive disclosure is explicit through See all, Filter, Monthly, balance visibility toggles, onboarding skip, and row/icon actions.",
      "Dense CRUD screens should still preserve rounded rows, muted metadata, semantic amounts/status, and forest/lime active states.",
      "Avoid representing financial data as raw spreadsheet grids unless task requirements demand it."
    ]
  },
  "constraints": [
    "Do not replace the cream canvas with generic gray or pure white page defaults.",
    "Do not replace forest/lime brand states with blue SaaS defaults.",
    "Do not make sharp rectangular cards, square primary buttons, or hard-edged panels the dominant geometry.",
    "Do not overuse heavy shadows; most app surfaces should remain shadow-sm or flat.",
    "Do not make every card saturated; use one forest or lime focal surface per major section.",
    "Do not create divider-heavy admin tables as the default for financial data.",
    "Do not use large bodies of low-contrast explanatory text; keep copy short, direct, and task-oriented.",
    "Do not let generic shadcn rounded-md primitives visually dominate branded finance screens.",
    "Do not use lime for arbitrary decoration; reserve it for action, brand, selection, and meaningful highlights.",
    "Do not obscure hierarchy by giving all tiles equal visual weight."
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
