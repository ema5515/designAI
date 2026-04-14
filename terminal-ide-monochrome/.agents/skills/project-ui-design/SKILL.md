---
name: Terminal IDE Monochrome
description: Generate terminal-native product UI with black/navy surfaces, monospaced typography, hard borders, compact command workflows, and restrained semantic color.
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

- Root: `/Users/emanueledagata/code/v0/boh3`
- Detected hints: Next.js, Tailwind CSS, shadcn/ui, Charts, Radix/Lucide
- Total indexed files: 83
- Relevant UI/design files: 81

## Key dependencies

- @radix-ui/react-dialog: 1.1.4
- @radix-ui/react-dropdown-menu: 2.1.4
- @radix-ui/react-select: 2.1.4
- @radix-ui/react-tabs: 1.1.2
- class-variance-authority: ^0.7.1
- clsx: ^2.1.1
- lucide-react: ^0.454.0
- next: 15.2.6
- react: ^19
- react-dom: ^19
- recharts: 2.15.4
- tailwind-merge: ^2.5.5
- tailwindcss: ^4.1.9

## Key analysis goals

- Extract the source design language from the repository.
- Identify explicit and inferred design-system rules.
- Preserve radius, spacing character, hierarchy, typography roles, and interaction tone.
- Produce a reusable design skill for generating new UI categories consistently.
- Prevent style drift when adapting to dashboards, forms, CRUD, or utility-heavy interfaces.


# Final Design Skill

# Terminal IDE Monochrome Product UI Design Skill

## Purpose

Use this skill to generate new UI screens, components, and product flows that feel native to this project’s existing interface language. The output must preserve the source application’s terminal-native identity while applying strong product UI/UX judgment for clarity, hierarchy, accessibility, task completion, and scalability.

The source design language is **Terminal IDE Monochrome**: black backgrounds, gray terminal panels, white text, monospaced typography, hard borders, command-style controls, compact expert workflows, crisp hover states, and restrained semantic color.

## AI Role

Act as a **product UI/UX designer and interface system builder**.

You design production-ready software interfaces, not decorative mockups. You translate product requirements into coherent layouts, component structures, interaction states, responsive behavior, and reusable design patterns that preserve the project’s visual identity.

You must behave like a design systems architect: reuse existing patterns first, extend them conservatively when needed, and keep every new screen consistent with the source system’s geometry, spacing, typography, emphasis, and interaction tone.

## Design Philosophy

Design interfaces that feel like a polished developer terminal expanded into a complete product UI.

Prioritize clarity over novelty. The interface should help users understand where they are, what matters, what they can do, what changed, and what to do next.

The project’s style is technical, precise, terminal-native, developer-focused, and utilitarian. Good UI in this system is not soft SaaS decoration. It is structured control-surface design: bordered panels, command rows, status metadata, compact controls, white-on-black contrast, and restrained functional color.

Use general UX best practices through the project’s identity:

- Use hierarchy to make task priority obvious.
- Use spacing to reveal relationships.
- Use typography to support scanning.
- Use borders before shadows.
- Use color as signal, not decoration.
- Use interaction feedback that feels crisp, local, and technical.
- Use shadcn/Radix primitives for accessibility and state logic, but visually bias them toward the terminal-console identity.

## Non-Negotiable Style Traits

### Radius And Geometry Family

- Preserve the sharp, rectangular terminal geometry.
- Default custom product surfaces to `rounded-none` or very small radius, roughly `0px` to `4px`.
- Use `rounded-md`, `rounded-lg`, or stock shadcn radius only for accessibility-heavy primitives such as inputs, selects, dialogs, popovers, switches, and tooltips.
- Use `rounded-full` only for status dots, switches, progress tracks, and similar functional indicators.
- Do not make large rounded SaaS cards the default container shape.

### Spacing Character

- Preserve medium-dense product spacing: broad page gutters, compact panel interiors, tight command/control rows, and clear section grouping.
- Use `p-4` to `p-6` for most panels.
- Use `gap-2`, `gap-3`, and `gap-4` for controls and dense groups.
- Use `gap-6`, `gap-8`, or `space-y-6/8` for major product sections.
- Avoid flattening the interface into a cramped generic admin layout. Dense does not mean crowded.

### Emphasis Discipline

- Use strong emphasis rarely.
- Primary emphasis is white text, white fill, stronger border, or active terminal status.
- Secondary content belongs in gray text and lower-contrast borders.
- Semantic color is reserved for state: green for success/active, yellow for warning/pending, red for destructive/error, blue only for terminal path/link semantics.
- Do not make multiple actions look equally primary.

### Hierarchy Style

- Establish hierarchy through contrast, alignment, border strength, spacing, typography weight, and panel structure.
- Page-level hierarchy must be stronger than component-level hierarchy.
- Use one dominant focal point per screen or section.
- Make primary values, statuses, and actions easier to scan than labels and supporting text.

### Typography Roles

- Preserve monospaced or code-adjacent typography as a core identity trait.
- Use mono for headings, labels, commands, stats, IDs, timestamps, navigation, filters, and compact product UI.
- Sans text may support longer prose only when mono harms readability.
- Use `text-sm` as the product UI default.
- Use `text-xs` for metadata and status labels.
- Use `text-lg` to `text-xl` for card and section titles.
- Use larger headings sparingly for page orientation or marketing-adjacent moments.

### Interaction Tone

- Interactions should feel crisp, calm, technical, and local.
- Hover states should brighten borders/text or shift dark backgrounds to `gray-900`.
- Focus states must remain visible and accessible.
- Loading should use terminal-native patterns such as blinking cursors, skeletons, spinners, processing labels, pulse status dots, or command-like progress.
- Avoid playful, bouncy, or decorative interaction unless it reinforces terminal behavior.

## Core UI/UX Principles

- Start from the user task before choosing layout or components.
- Make the primary purpose of each screen immediately clear.
- Group related information and actions.
- Keep common actions easy to find.
- Make destructive or irreversible actions distinct and confirmed.
- Show loading, empty, error, success, disabled, hover, focus, selected, and active states.
- Maintain accessible contrast and keyboard-visible focus.
- Do not rely on color alone for meaning.
- Preserve layout stability during loading, validation, hover, and dynamic updates.
- Prefer recognition over recall with labels, current values, helper text, and clear status.

## Project-Specific Style Rules

### Color Usage

- Base background: black.
- Main surfaces: `gray-950`, `gray-900`, and black.
- Main text: white.
- Supporting text: `gray-300`, `gray-400`, and `gray-500`.
- Low-priority metadata: `gray-600` or `gray-700`.
- Primary CTA: white fill, black text, strong border.
- Default borders: `gray-800` or `gray-700`.
- Hover/active borders: `gray-600`, `gray-500`, or white.
- Keep 85-90% of the interface black, gray, and white.
- Use green, yellow, red, and blue only for status, validation, terminal semantics, charts, or links.

### Typography Rules

- Use mono as the default product identity font.
- Headings are bold and concise.
- Labels are small, direct, and close to their controls.
- Helper text is gray and used only when it reduces uncertainty.
- Error text must explain what failed and how to recover.
- IDs, commands, values, metrics, timestamps, and technical metadata should use mono/tabular treatment.
- Avoid too many sizes or weights in one screen.

### Spacing Rules

- Use wide outer page gutters such as `px-6` and `lg:px-12`.
- Use constrained max widths for reading-heavy content.
- Use wider content areas for dashboards, tables, and operational views.
- Product page header to content spacing should usually be `24px` to `32px`.
- Panel grid gaps should usually be `16px` to `24px`.
- Table rows should usually be `40px` to `48px`.
- Form field gaps should usually be `12px` to `16px`.
- Field group gaps should usually be around `24px`.

### Radius Rules

- Terminal panels, command rows, cards, tables, page sections, and custom CTAs should usually be square.
- Form controls may use shadcn `rounded-md`.
- Dialogs and overlays may use `rounded-lg`.
- Do not mix arbitrary radii for visual interest.
- Radius differences must correspond to component role or primitive constraints.

### Shadow And Elevation Rules

- Borders are the primary separation mechanism.
- Shadows are secondary and sparse.
- Use shadows for terminal windows, active CTAs, dialogs, popovers, dropdowns, and raised overlays.
- If using glow, keep it white-tinted and subtle.
- Do not use soft card stacks as the main structure.

### Hierarchy Rules

- White text and stronger borders indicate priority.
- Gray text and weaker borders indicate support.
- Active navigation uses `bg-gray-900`, stronger border, and white text.
- Destructive actions use red only when the action is truly destructive.
- Status badges should be compact and semantic.
- Repeated chrome should be quiet so content can stand out.

### Visual Priority Rules

- Identify the screen’s primary task before styling.
- Place primary actions near the content they affect.
- Use one clear primary action per decision area.
- Make important values scannable before explanations.
- Use compact metadata rows for secondary information.
- Do not allow filters, nav, badges, or decorative elements to compete with the main task.

### Interaction State Rules

- Hover: brighten text, border, or dark surface; avoid layout shift.
- Focus: use visible ring or border treatment that works on black and gray surfaces.
- Active: use stronger border/background and persistent white text.
- Selected: distinguish from hover with persistent state, not color alone.
- Disabled: use opacity plus explanation when the reason is not obvious.
- Loading: preserve layout with skeletons, spinners, terminal labels, or processing states.
- Success: use local green feedback when possible.
- Warning: use yellow sparingly with clear text.
- Error: use red border/text and actionable recovery guidance.

### Layout Rules

- Use black full-page shells.
- Prefer sticky top nav, persistent left sidebar, or local page header depending on product complexity.
- Use terminal-like panels with header/body/footer structure for grouped workflows.
- Use command bars above data for search, filters, and actions.
- Use bordered sections instead of floating decorative cards.
- Avoid cards inside cards unless the inner item is a truly repeated object.
- Keep controls visually connected to the content they affect.

### Responsiveness Rules

- Preserve task order on narrow screens.
- Stack CTAs and controls vertically on mobile when needed.
- Collapse sidebars into off-canvas navigation on small screens.
- Keep command strings readable with wrapping or `break-all`.
- Hide or collapse secondary columns before primary identifiers, statuses, or actions.
- Tables should support horizontal scroll, responsive column priority, or alternate row detail views.
- Do not let text overflow, clip, or cause layout shifts.

## Visual Priority And Hierarchy Rules

Every generated screen must answer:

- What is the user trying to do?
- What is the most important information?
- What action should happen next?
- What is secondary, historical, optional, or metadata?
- What state is the system currently in?

Use hierarchy in this order:

1. Layout position.
2. Grouping and spacing.
3. Typography size and weight.
4. Text and border contrast.
5. Surface contrast.
6. Semantic color.
7. Motion or animation.

Do not solve hierarchy primarily with color, decoration, or excessive badges.

## Typography As UX Rules

Use typography to guide comprehension:

- Page title answers: where am I?
- Section title answers: what is this group?
- Label answers: what is this control or value?
- Helper text answers: how should I decide?
- Metadata answers: what is the supporting context?
- Error text answers: what went wrong and how do I fix it?
- Action label answers: what will happen if I click?

Keep headings short, specific, and product-facing. Avoid vague labels like “Overview” when a task-specific title is possible.

## Interaction Rules

- Buttons perform actions.
- Links navigate.
- Tabs switch peer views.
- Accordions reveal secondary content in the same flow.
- Dialogs interrupt for bounded decisions.
- Forms preserve user input after errors.
- Filters stay close to the data they affect.
- Copy actions should show immediate local feedback.
- Advanced or rare options may use progressive disclosure, but critical actions and errors must remain visible.
- Do not hide essential functionality behind hover-only behavior.

## Layout And Page Composition Rules

### Page Shells

Use a terminal control-surface shell:

- Black page background.
- Gray-950 navigation/sidebar.
- Gray-800 dividers.
- White primary text.
- Gray support text.
- Compact command/action areas.
- Bordered panels for content groups.

### Page Headers

Use page headers with:

- White title.
- Short gray description.
- Optional status/version/timestamp metadata.
- Right-aligned command-like primary action.
- Secondary actions as outline, dashed, ghost, or text controls.

### Product Dashboards

Dashboards must feel like terminal monitoring surfaces, not generic SaaS metric grids.

Use:

- Compact metric panels with white values and gray labels.
- Status dots and sparse semantic color.
- Bordered chart containers with muted gridlines.
- Command bar filters for time range, environment, status, or scope.
- Alerts/work queues above static vanity metrics when action is required.

### Data And CRUD Pages

Use list/detail/create/edit/delete separation.

- Lists use tables or dense rows for operational data.
- Detail pages use panels, property lists, command blocks, and related-record sections.
- Create/edit flows use grouped forms in bordered panels.
- Delete flows require confirmation and consequence text.
- Primary record actions stay consistent across resources.

### Settings Pages

Group settings by user mental model.

- Use clear section titles.
- Show current values.
- Explain consequences of risky changes.
- Separate dangerous settings from routine configuration.
- Make save behavior explicit: immediate, explicit, or staged.

## Component Rules

### Dashboards

- Use bordered metric panels with compact typography.
- Use white values, gray labels, and mono/tabular numerals.
- Use green/yellow/red only for actual state.
- Place filters and time ranges in compact command bars.
- Avoid decorative charts that do not support monitoring, comparison, or action.

### Settings Pages

- Use stacked bordered sections.
- Use compact labels, descriptions, and current values.
- Use inline status and save feedback.
- Keep dangerous actions isolated with stronger warning language.

### CRUD Pages

- Use tables for scanning and comparison.
- Use details panels for record inspection.
- Use forms for create/edit.
- Use confirmation dialogs for destructive actions.
- Keep row actions compact and predictable.

### Forms

- Use grouped fieldsets inside bordered panels.
- Use full-width controls in narrow contexts.
- Place labels close to controls.
- Use helper text for constraints or consequences.
- Use red destructive text and border treatment for errors.
- Put submit actions after the form content or in a sticky/local footer for long forms.

### Tables

- Use full-width tables inside bordered containers.
- Use compact `text-sm` rows.
- Use muted column headers.
- Use row dividers instead of heavy card separation.
- Use hover `bg-gray-900`.
- Use selected state with stronger background or border.
- Keep identifiers, statuses, and primary actions visible.
- Use horizontal scroll or responsive column priority on mobile.

### Analytics Blocks

- Use dark bordered chart panels.
- Use muted axes, gridlines, and labels.
- Use mono values in tooltips.
- Use chart colors sparingly and semantically.
- Keep charts subordinate to the insight or decision they support.

### Dialogs

- Use black or gray-950 content with gray border.
- Use `bg-black/50` overlay.
- Use compact `p-6`.
- Use white title and gray description.
- Align actions right on desktop and stack appropriately on mobile.
- Avoid colorful modal headers.
- Use destructive styling only for destructive confirmations.

### Navigation

- Use terminal chrome, gray-950 backgrounds, and gray borders.
- Use white active labels.
- Use gray inactive labels.
- Use active state with `bg-gray-900` and stronger border.
- Use compact icon plus label rows.
- Use nested indentation where needed.
- Mobile navigation may slide off-canvas with a black overlay.

### Cards

- Use cards as bordered terminal panels, not soft elevated tiles.
- Use black or gray-950 fill.
- Use `p-4` to `p-6`.
- Use square or tiny radius.
- Use white titles and gray descriptions.
- Use hover border brightening for interactive cards.
- Do not use card grids where a table better supports comparison.

### Empty States

- Use dashed bordered terminal panels.
- Use a short white title.
- Use gray explanatory text.
- Provide one clear command-style action when there is a next step.
- Distinguish first-use, filtered-empty, permission-empty, and error-empty states.

### Alerts

- Use bordered callout panels.
- Keep fill changes subtle.
- Use semantic color only for severity.
- Explain the issue and recovery action.
- Prefer inline feedback for field-level or row-level problems.

### Filters

- Place filters directly above the data they affect.
- Use a compact command-bar row.
- Combine search, select filters, status chips, and reset behavior.
- Show active filters clearly.
- Hide rare advanced filters behind a dropdown, drawer, or expandable region only when active filters remain visible.

## Derived Component Rules

When creating components that do not exist in the original repository, derive them from the source identity instead of inventing a new style family.

Use this derivation process:

1. Identify the closest existing source pattern: terminal window, command row, docs panel, sidebar item, shadcn primitive, table row, dialog, badge, or empty state.
2. Preserve the dominant traits: black/gray surfaces, mono typography, hard borders, compact spacing, restrained color, and crisp state changes.
3. Choose component anatomy based on user task, not visual novelty.
4. Use existing radius and spacing behavior unless the component’s function requires a primitive-specific exception.
5. Use semantic variants only when they represent actual state or risk.
6. Add new variants only when they have a clear reusable purpose.

Examples:

- A calendar should look like a bordered terminal grid with compact mono dates, gray inactive days, white selected day, and green/yellow/red only for availability or risk.
- A kanban board should use dark bordered columns, compact cards, white titles, gray metadata, and status dots instead of colorful column backgrounds.
- A billing screen should use property panels, command-like plan actions, compact invoices table, and restrained semantic status badges.
- A profile editor should use grouped bordered form panels, mono labels, gray helper text, and explicit save feedback.
- A notification center should use dense rows with timestamps, status dots, muted descriptions, and border/hover state instead of illustrated feed cards.

## Constraints

Never:

- Introduce broad new color families, pastel palettes, glassmorphism, blobs, or colorful decorative gradients.
- Replace the terminal identity with generic bright SaaS styling.
- Use decorative elements without functional value.
- Use soft shadows as the primary layout separator.
- Use large rounded cards as the default surface.
- Introduce sharper geometry if adapting a source system that is rounded; for this project, preserve the existing sharp terminal geometry.
- Flatten or neutralize the spacious/dense rhythm into a cramped generic admin style.
- Break spacing rhythm between similar groups.
- Create inconsistent hierarchy where every card, badge, button, or metric competes equally.
- Overuse semantic colors.
- Hide critical actions, errors, or required fields behind progressive disclosure.
- Use hover-only actions without keyboard or touch equivalents.
- Overcomplicate interactions when a direct action, table, form, or dialog is clearer.
- Invent unsupported component patterns without grounding them in the source identity.
- Add illustrations, mascots, playful icons, or decorative animations unless they directly support terminal/product comprehension.

## Anti-Drift Rules

Use these checks before finalizing any generated UI:

- Does the screen still read as a terminal/IDE control surface?
- Is the palette still mostly black, gray, and white?
- Are semantic colors used only for state, validation, or terminal semantics?
- Are panels bordered before they are shadowed?
- Are custom product surfaces mostly square?
- Is mono typography still visible in core product elements?
- Are spacing choices consistent with compact expert UI?
- Is there one clear primary action per area?
- Are supporting elements gray and quieter than primary content?
- Are hover, focus, active, selected, disabled, loading, empty, and error states defined?
- Are new components derived from existing source patterns?
- Would this screen feel native beside the landing page, docs page, terminal panels, command rows, and sidebar?

If the answer is no, revise toward the source identity. Remove decorative color, soften hierarchy conflicts, tighten spacing, strengthen borders, restore mono roles, and reduce unsupported component novelty.

## Conservative Adaptation Rule

A portfolio, marketing page, landing page, or documentation style may be adapted into dashboards, settings, CRUD flows, forms, analytics, or utility screens.

The adaptation must preserve the recognizable traits of the source system:

- Geometry remains sharp, rectangular, and terminal-like.
- Hierarchy remains high-contrast but disciplined.
- Spacing remains broad at page level and compact inside controls.
- Emphasis remains sparse and purposeful.
- Typography remains mono/code-adjacent in core UI roles.
- Interaction remains crisp, local, and technical.
- Components feel like extensions of terminal windows, command rows, docs panels, and shadcn primitives rather than a different product family.

## Final Operating Instructions

When generating UI for this project:

1. Start with the user task and screen purpose.
2. Select the closest existing source pattern.
3. Build the layout using black shells, gray panels, hard borders, compact controls, and mono hierarchy.
4. Reuse shadcn/Radix primitives for accessible behavior where appropriate.
5. Style primitives to align with the terminal identity.
6. Define responsive behavior and all important interaction states.
7. Justify key layout and component decisions using clarity, hierarchy, visual priority, consistency, task completion, accessibility, and scalability.
8. Prefer product-ready UI over conceptual styling.
9. Extend the system conservatively instead of reinventing it.
10. Preserve the Terminal IDE Monochrome identity across every new screen category.

# Structured Style Profile

```json
{
  "style_name": "Terminal IDE Monochrome",
  "visual_identity": {
    "tone": "technical, terminal-native, developer-focused",
    "density": "medium-dense with compact controls, large hero moments, and high information density in docs",
    "corner_style": "dominantly sharp and square in product surfaces; shadcn library components retain rounded-md/lg defaults",
    "elevation_style": "border-led elevation with sparse shadows, glow-on-hover, and offset duplicate-border CTA treatment",
    "contrast_profile": "high contrast black/white base with gray hierarchy and limited semantic status color",
    "mood": "command-line, IDE chrome, cyber-terminal, precise",
    "notes": [
      "Requested context files under input/ and outputs/ were not present in the checkout; profile is based on direct inspection of app/page.tsx, app/docs/page.tsx, app/globals.css, styles/globals.css, components.json, and components/ui/*.",
      "Landing and docs pages use bg-black text-white font-mono directly, overriding the more general shadcn neutral token system.",
      "Visual signature comes from ASCII art, terminal panels, window-control dots, command snippets, matrix characters, scan/glow animation, and monochrome borders."
    ]
  },
  "identity_traits": {
    "non_negotiable_traits": [
      "black or near-black page background",
      "monospace product UI for terminal/CLI surfaces",
      "white primary text with gray secondary hierarchy",
      "rectangular bordered panels",
      "hover states brighten borders/text rather than introducing new color families",
      "green/red/yellow reserved for terminal status and window controls"
    ],
    "adaptable_traits": [
      "shadcn components may use rounded-md/lg defaults when outside bespoke terminal surfaces",
      "accent gradients are allowed only as white-to-gray text or subtle gray panel backplates",
      "blue may appear in shell prompt/path text but should not become a primary brand color",
      "animations may be pulsing, blinking, scanning, typing, or matrix-like when they reinforce the terminal metaphor"
    ],
    "source_type": "direct repository inspection",
    "adaptation_notes": [
      "Prefer page-level terminal aesthetic over default shadcn styling for product-facing screens.",
      "Where a component exists only in components/ui and is not used by pages, confidence is lower and source_basis states library implementation."
    ]
  },
  "tokens": {
    "colors": {
      "primary": "white / text-white / bg-white for primary CTA",
      "secondary": "gray-400 for secondary text and navigation",
      "accent": "gray-900, gray-800, gray-700, gray-600 border/surface accents",
      "neutral": [
        "black",
        "gray-950",
        "gray-900",
        "gray-800",
        "gray-700",
        "gray-600",
        "gray-500",
        "gray-400",
        "gray-300",
        "white"
      ],
      "success": "green-400 / green-500 for status dots, copied state, active availability",
      "warning": "yellow-500 for terminal window dot and pending status",
      "danger": "red-500 for terminal window dot; shadcn destructive token oklch(0.577 0.245 27.325)",
      "background": "bg-black; token --background defaults to oklch(1 0 0) light and oklch(0.145 0 0) dark",
      "surface": "bg-gray-950, bg-gray-900, bg-black, bg-gray-950/95, bg-gray-950/30",
      "text": {
        "primary": "text-white",
        "secondary": "text-gray-400",
        "muted": "text-gray-500 / text-gray-600 / text-gray-700",
        "inverse": "text-black on bg-white CTA"
      },
      "border": "border-gray-800 primary section dividers; border-gray-700 panels; border-gray-600/500 hover; border-white active CTA"
    },
    "spacing": {
      "density": "medium-dense",
      "section_gap": [
        "py-16",
        "py-20",
        "mb-12",
        "mb-16"
      ],
      "card_gap": [
        "gap-4",
        "gap-6",
        "space-y-6",
        "space-y-8"
      ],
      "control_gap": [
        "gap-2",
        "gap-3",
        "gap-4",
        "px-3 py-1.5",
        "px-4 py-2",
        "px-6 py-4"
      ],
      "grouping_pattern": "large centered sections with max-width containers; terminal panels use header/body split; docs use fixed sidebar plus content stack",
      "adaptation_rule": "Use p-6 for panels/cards, px-6 lg:px-12 for page gutters, max-w-7xl for landing sections, max-w-4xl/5xl for terminal and docs content."
    },
    "radius": {
      "control": "product CTAs and command blocks are square; shadcn controls default rounded-md",
      "container": "product panels/cards are mostly square; shadcn Card default rounded-xl",
      "overlay": "Dialog and AlertDialog use rounded-lg",
      "pill": "only status indicators use rounded-full",
      "dominant_family": "sharp/square terminal geometry",
      "sharp_allowed": "yes; preferred for product-facing terminal surfaces",
      "style_rule": "Default to no radius for terminal panels, code blocks, cards, and CTAs; allow rounded-md/lg only when using stock shadcn primitives or status dots."
    },
    "shadows": [
      "shadow-xl",
      "shadow-2xl",
      "shadow-lg group-hover:shadow-white/20",
      "group-hover:shadow-xl group-hover:shadow-white/10",
      "shadow-sm/shadow-md/shadow-lg in shadcn overlays",
      "custom terminal-window glow rgba(255,255,255,0.1-0.2)"
    ],
    "typography": {
      "font_families": [
        "Geist",
        "Geist Mono",
        "font-mono on product pages",
        "Courier New / Monaco / Menlo for terminal-text utility"
      ],
      "scale": [
        "text-xs",
        "text-sm",
        "text-base",
        "text-lg",
        "text-xl",
        "text-2xl",
        "text-3xl",
        "text-4xl",
        "text-5xl",
        "text-6xl"
      ],
      "font_weights": [
        "font-medium",
        "font-semibold",
        "font-bold"
      ],
      "line_heights": [
        "leading-none for ASCII/title glyphs",
        "leading-tight for hero headings",
        "leading-relaxed for supporting copy",
        "text-sm/relaxed in empty descriptions"
      ]
    },
    "widths": [
      "max-w-7xl page/nav sections",
      "max-w-5xl CTA section",
      "max-w-4xl terminal/docs content",
      "max-w-3xl hero copy",
      "w-80 docs mobile sidebar",
      "16rem shadcn sidebar width",
      "18rem shadcn mobile sidebar width",
      "3rem shadcn collapsed sidebar width"
    ],
    "breakpoints": [
      "sm",
      "md",
      "lg",
      "desktop sidebar at lg",
      "mobile menu below md/lg depending page"
    ]
  },
  "hierarchy": {
    "primary_focus_pattern": "centered hero with ASCII masthead, large bold headline, install CTA, and live terminal simulator",
    "secondary_content_pattern": "terminal-window sections with command headers, rows, status metadata, and centered section headers",
    "cta_hierarchy": "primary: white filled offset install command; secondary: dashed outline documentation link; tertiary: inline command copy rows/text links",
    "emphasis_rules": [
      "Use white for active/primary content.",
      "Use gray-400 for explanatory copy and inactive navigation.",
      "Use gray-500/600 for metadata and low-priority terminal chrome.",
      "Use border brightness changes for hover/selection.",
      "Use green only for success/online/copied/active status."
    ],
    "grouping_rules": [
      "Terminal panels group content with gray-900 header, gray-700 divider, and black body.",
      "Docs content groups each topic in bg-gray-950 border-gray-800 p-6 blocks.",
      "Repeated command rows are black bordered strips with copy affordance on the right.",
      "Feature cards use numbered square markers and command snippets as anchors."
    ],
    "contrast_usage": "Very high contrast for foreground and CTAs; gray hierarchy distinguishes metadata, descriptions, inactive items, and borders."
  },
  "typography_roles": {
    "page_title": "text-4xl lg:text-6xl font-bold leading-tight on landing; text-4xl font-bold in docs",
    "section_title": "text-3xl/lg:text-4xl or text-4xl/lg:text-5xl font-bold with centered alignment on landing; text-2xl font-bold in docs panels",
    "body": "text-lg or text-xl for landing explanatory copy; text-gray-400 body copy in docs",
    "supporting_text": "text-sm/text-xs gray-400/500 for metadata, descriptions, status labels, and command hints",
    "label": "font-medium or font-bold, often text-white; sidebar labels use text-sm and active border/background",
    "caption": "text-xs gray-500 for terminal status, version, availability, command metadata",
    "scanning_behavior": "Users scan from white headings to gray descriptions to bordered command blocks; monospace rows and bracketed numbers support quick terminal-like parsing."
  },
  "interaction": {
    "hover": "text gray-400 to white, border gray-700/600 to gray-500/white, subtle gray background, shadow-white glow, and occasional translate offset reset",
    "focus": "shadcn primitives use focus-visible:border-ring and focus-visible:ring-ring/50 ring-[3px]; dialogs close button uses focus:ring-2 ring-offset",
    "active": "docs active sidebar items use bg-gray-900 border-gray-600 text-white; selected shadcn rows/items use data-state styles",
    "selected": "selected rows/items use bg-muted or bg-gray-900 with stronger border; select/menu items show check/circle indicators",
    "disabled": "shadcn controls use disabled:pointer-events-none disabled:opacity-50; select adds disabled:cursor-not-allowed",
    "loading": "terminal simulator uses bouncing dots, Processing text, blinking cursor, pulsing status dots, and timed command/output sequences",
    "validation": "form/input/select/button primitives support aria-invalid:border-destructive and destructive ring; FormMessage renders text-destructive text-sm",
    "feedback_style": "copy actions swap Copy icon to green Check for 2 seconds; success terminal lines render green; hover feedback is immediate via transition-colors/transition-all"
  },
  "layout": {
    "page_shell": "black full-height shell with sticky top nav and terminal/matrix background on landing; docs shell uses sticky nav, left sidebar, and content main",
    "page_width_strategy": "max-w-7xl for broad landing content, max-w-4xl for terminal/docs reading, max-w-5xl for CTA section, centered mx-auto containers",
    "header_pattern": "sticky bg-gray-950/95 nav with border-b, backdrop-blur-sm, logo/window dots, hidden desktop links, and command/install action",
    "section_spacing": "landing sections use px-6 py-16/20 lg:px-12 with border-t dividers; docs uses p-6 lg:p-12 content padding",
    "grid_rules": [
      "feature cards use grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6",
      "IDE list uses grid-cols-2 md:grid-cols-3 gap-4",
      "docs default cards use md:grid-cols-2 gap-6",
      "matrix background uses custom grid-cols-25 increasing at md/lg"
    ],
    "navigation_patterns": [
      "desktop landing nav shows inline anchors with underline-on-hover",
      "mobile landing shows hamburger icon only",
      "docs mobile uses off-canvas sidebar with overlay",
      "docs desktop sidebar is fixed/static left navigation with nested items"
    ],
    "responsive_rules": [
      "CTAs stack flex-col on mobile and become sm:flex-row.",
      "Long command text uses break-all on small screens where needed.",
      "Sidebar is translated offscreen on mobile and static on lg.",
      "Landing terminal/list footers switch from column to row at md."
    ]
  },
  "components": {
    "buttons": {
      "explicit": true,
      "source_basis": "components/ui/button.tsx plus custom CTA div/button patterns in app/page.tsx and app/docs/page.tsx",
      "confidence": "high",
      "rules": {
        "purpose": "trigger install/copy/navigation/actions",
        "appearance": "stock Button is rounded-md with variants; product CTAs are square bordered blocks, often offset over a secondary border layer",
        "spacing": "stock h-8/h-9/h-10 px-3/4/6; product CTAs use px-6 to px-16 and py-2 to py-5",
        "radius": "rounded-md in stock component; no radius in product CTAs",
        "border": "primary product CTA uses border-white; secondary uses border-2 border-dashed gray-400/600; hover strengthens to white",
        "shadow": "stock outline has shadow-xs; product hover uses shadow-lg/shadow-white/20",
        "typography": "text-sm font-medium stock; font-bold monospace product CTA",
        "states": "hover background/border/text transitions, disabled opacity-50 in stock, focus-visible ring in stock, copied state swaps icon to Check",
        "variants": [
          "default",
          "destructive",
          "outline",
          "secondary",
          "ghost",
          "link",
          "terminal-filled",
          "terminal-dashed",
          "command-copy"
        ]
      }
    },
    "inputs": {
      "explicit": true,
      "source_basis": "components/ui/input.tsx",
      "confidence": "high",
      "rules": {
        "purpose": "text/file input primitive for forms and sidebar search contexts",
        "appearance": "transparent bg, border-input, shadow-xs, placeholder muted, full width",
        "spacing": "h-9 px-3 py-1; md:text-sm",
        "radius": "rounded-md",
        "border": "border-input with focus-visible:border-ring and aria-invalid:border-destructive",
        "shadow": "shadow-xs",
        "typography": "text-base on mobile, md:text-sm",
        "states": "focus-visible ring-[3px], disabled opacity-50 cursor-not-allowed, invalid destructive ring/border",
        "variants": [
          "default",
          "file input support"
        ]
      }
    },
    "selects": {
      "explicit": true,
      "source_basis": "components/ui/select.tsx",
      "confidence": "high",
      "rules": {
        "purpose": "compact option selection with Radix Select",
        "appearance": "transparent bordered trigger, popover content with bg-popover border shadow-md",
        "spacing": "trigger h-9 px-3 py-2 default, h-8 sm; content p-1; item py-1.5 pl-2 pr-8",
        "radius": "rounded-md trigger/content, rounded-sm items",
        "border": "border-input trigger; content border",
        "shadow": "shadow-xs trigger, shadow-md content",
        "typography": "text-sm; label text-xs muted",
        "states": "focus-visible ring-[3px], disabled opacity-50, invalid destructive, open/closed fade/zoom/slide animations, selected item check indicator",
        "variants": [
          "default",
          "sm",
          "popper"
        ]
      }
    },
    "dropdowns": {
      "explicit": true,
      "source_basis": "components/ui/dropdown-menu.tsx",
      "confidence": "high",
      "rules": {
        "purpose": "menus, checkbox/radio menu items, nested submenus, shortcuts",
        "appearance": "bg-popover text-popover-foreground bordered menu with compact item rows",
        "spacing": "content p-1 min-w-8rem; items px-2 py-1.5 gap-2",
        "radius": "rounded-md content, rounded-sm items",
        "border": "content border; separators use bg-border",
        "shadow": "shadow-md",
        "typography": "text-sm items/labels; shortcut text-xs tracking-widest muted",
        "states": "focus:bg-accent, data-state=open accent on subtrigger, disabled opacity-50, destructive item variant, open/closed fade/zoom/slide animations",
        "variants": [
          "item",
          "checkbox",
          "radio",
          "sub",
          "destructive",
          "inset"
        ]
      }
    },
    "cards": {
      "explicit": true,
      "source_basis": "components/ui/card.tsx plus terminal/product panels in app/page.tsx and docs page topic blocks",
      "confidence": "high",
      "rules": {
        "purpose": "group related content, terminal windows, docs topics, feature steps",
        "appearance": "product cards/panels are bg-gray-950 or bg-black with gray borders; stock Card uses bg-card rounded-xl border shadow-sm",
        "spacing": "stock py-6 gap-6 px-6 inner parts; product p-6 with gap-4/6 and section mb-12/16",
        "radius": "product cards square; stock cards rounded-xl",
        "border": "border-gray-800/700 product; stock border token",
        "shadow": "terminal panels shadow-xl/2xl; feature cards hover shadow-white/10; stock shadow-sm",
        "typography": "card titles font-bold/semibold; descriptions gray-400 text-sm",
        "states": "hover:border-white or gray-500, hover:bg-gray-900, hover shadow/glow, optional slight transform/backplate rotation",
        "variants": [
          "terminal-window",
          "docs-topic",
          "feature-step",
          "stock-card"
        ]
      }
    },
    "tables": {
      "explicit": true,
      "source_basis": "components/ui/table.tsx",
      "confidence": "medium-high",
      "rules": {
        "purpose": "responsive tabular data primitive",
        "appearance": "full-width table inside overflow-x-auto container, border-separated rows via border-b",
        "spacing": "head h-10 px-2; cells p-2",
        "radius": "none",
        "border": "row border-b; footer border-t",
        "shadow": "none",
        "typography": "text-sm, head font-medium, caption text-muted-foreground",
        "states": "row hover:bg-muted/50 and data-state=selected:bg-muted",
        "variants": [
          "header",
          "body",
          "footer",
          "caption",
          "selected row"
        ]
      }
    },
    "modals": {
      "explicit": true,
      "source_basis": "components/ui/dialog.tsx",
      "confidence": "high",
      "rules": {
        "purpose": "general modal content over overlay",
        "appearance": "centered bg-background panel over bg-black/50 overlay",
        "spacing": "gap-4 p-6, close button top-4 right-4",
        "radius": "rounded-lg content; rounded-xs close",
        "border": "content border",
        "shadow": "shadow-lg",
        "typography": "title text-lg font-semibold leading-none; description text-sm muted",
        "states": "open/closed fade and zoom animations, close hover opacity-100, focus ring, disabled pointer-events-none",
        "variants": [
          "default",
          "with close button",
          "without close button"
        ]
      }
    },
    "dialogs": {
      "explicit": true,
      "source_basis": "components/ui/alert-dialog.tsx",
      "confidence": "high",
      "rules": {
        "purpose": "confirmation/destructive decision dialogs",
        "appearance": "same modal shell as Dialog with action/cancel buttons",
        "spacing": "content gap-4 p-6; footer gap-2 column-reverse on mobile, row at sm",
        "radius": "rounded-lg",
        "border": "content border",
        "shadow": "shadow-lg",
        "typography": "title text-lg font-semibold; description text-sm muted",
        "states": "open/closed fade and zoom animations; actions inherit Button states",
        "variants": [
          "action",
          "cancel",
          "destructive via button variant when supplied"
        ]
      }
    },
    "sidebars": {
      "explicit": true,
      "source_basis": "app/docs/page.tsx docs sidebar and components/ui/sidebar.tsx",
      "confidence": "high",
      "rules": {
        "purpose": "documentation navigation and reusable collapsible app navigation",
        "appearance": "docs sidebar bg-gray-950 border-r gray-800; reusable sidebar uses bg-sidebar text-sidebar-foreground",
        "spacing": "docs width w-80 p-6, section gaps space-y-6, item p-2/p-3; reusable width 16rem, mobile 18rem, icon 3rem",
        "radius": "docs sidebar square; reusable floating variant rounded-lg",
        "border": "border-r gray-800 docs; reusable border-sidebar-border for floating/side borders",
        "shadow": "floating reusable sidebar shadow-sm; docs no shadow",
        "typography": "section labels text-white font-medium; nested items text-sm gray-400",
        "states": "mobile translate-x open/closed, overlay on mobile, active bg-gray-900 border-gray-600, hover border-gray-700 bg-gray-900, keyboard shortcut support in reusable provider",
        "variants": [
          "docs fixed/offcanvas",
          "sidebar",
          "floating",
          "inset",
          "offcanvas",
          "icon collapsed"
        ]
      }
    },
    "tabs": {
      "explicit": true,
      "source_basis": "components/ui/tabs.tsx",
      "confidence": "medium-high",
      "rules": {
        "purpose": "segmented content switching",
        "appearance": "inline bg-muted tab list with active trigger bg-background and optional shadow",
        "spacing": "root gap-2; list h-9 p-[3px]; trigger px-2 py-1 gap-1.5",
        "radius": "rounded-lg list, rounded-md trigger",
        "border": "transparent trigger border; active dark border-input",
        "shadow": "active trigger shadow-sm",
        "typography": "text-sm font-medium",
        "states": "data-state=active background/text/shadow, focus-visible ring-[3px], disabled opacity-50",
        "variants": [
          "default"
        ]
      }
    },
    "badges": {
      "explicit": true,
      "source_basis": "components/ui/badge.tsx and inline docs model tags",
      "confidence": "high",
      "rules": {
        "purpose": "compact status/category labels",
        "appearance": "stock badge rounded-md border px-2 py-0.5; docs tags use bg-gray-800 text-gray-300 px-2 py-1",
        "spacing": "px-2 py-0.5 stock; gap-1; docs px-2 py-1",
        "radius": "rounded-md stock; docs tags appear square unless class adds radius",
        "border": "transparent for filled variants; outline variant keeps border",
        "shadow": "none",
        "typography": "text-xs font-medium",
        "states": "anchor badges hover background, focus-visible ring, invalid destructive support",
        "variants": [
          "default",
          "secondary",
          "destructive",
          "outline",
          "terminal-tag"
        ]
      }
    },
    "alerts": {
      "explicit": true,
      "source_basis": "components/ui/alert.tsx",
      "confidence": "medium-high",
      "rules": {
        "purpose": "inline messages and destructive notices",
        "appearance": "bordered rounded panel using bg-card text-card-foreground; optional icon grid",
        "spacing": "px-4 py-3 gap-x-3 gap-y-0.5",
        "radius": "rounded-lg",
        "border": "default border with destructive text variant",
        "shadow": "none",
        "typography": "text-sm; title font-medium tracking-tight; description text-sm muted",
        "states": "destructive variant changes text/icon/description color",
        "variants": [
          "default",
          "destructive"
        ]
      }
    },
    "empty_states": {
      "explicit": true,
      "source_basis": "components/ui/empty.tsx",
      "confidence": "medium-high",
      "rules": {
        "purpose": "centered no-content or setup prompts",
        "appearance": "flex column centered, text-balance, optional icon media",
        "spacing": "gap-6 p-6 md:p-12; content gap-4; header gap-2",
        "radius": "rounded-lg container/media icon",
        "border": "border-dashed on container",
        "shadow": "none",
        "typography": "title text-lg font-medium tracking-tight; description text-sm/relaxed muted",
        "states": "links in description underline and hover:text-primary",
        "variants": [
          "default",
          "icon media"
        ]
      }
    },
    "charts_containers": {
      "explicit": true,
      "source_basis": "components/ui/chart.tsx",
      "confidence": "medium-high",
      "rules": {
        "purpose": "Recharts responsive chart wrapper and tooltip/legend styling",
        "appearance": "aspect-video flex container with muted axes/grid and tokenized series colors",
        "spacing": "tooltip px-2.5 py-1.5 gap-1.5; chart container fills responsive area",
        "radius": "tooltip rounded-lg; indicators rounded-[2px]",
        "border": "tooltip border-border/50; grid uses stroke-border/50",
        "shadow": "tooltip shadow-xl",
        "typography": "text-xs chart/tooltip, font-medium labels",
        "states": "tooltip renders only when active payload exists; indicator supports dot/line/dashed",
        "variants": [
          "dot tooltip indicator",
          "line tooltip indicator",
          "dashed tooltip indicator",
          "themed series colors"
        ]
      }
    },
    "page_headers": {
      "explicit": true,
      "source_basis": "app/page.tsx hero/section headers and app/docs/page.tsx content headers",
      "confidence": "high",
      "rules": {
        "purpose": "orient page/section and establish primary message",
        "appearance": "large white bold headings, centered on landing and left-aligned in docs content",
        "spacing": "mb-4/6/8 after titles; header groups mb-12/16",
        "radius": "none",
        "border": "section headers often sit above bordered terminal blocks; no direct border",
        "shadow": "ASCII/terminal glow classes available but headings mostly unshadowed",
        "typography": "landing h1 text-4xl lg:text-6xl; section h2 text-3xl to text-5xl; docs h1 text-4xl",
        "states": "some emphasized words animate-pulse or use white-to-gray text gradient",
        "variants": [
          "hero ASCII masthead",
          "centered landing section",
          "docs content header"
        ]
      }
    },
    "filters": {
      "explicit": false,
      "source_basis": "inferred from available Input, Select, DropdownMenu, Tabs, and Table primitives; no dedicated filter component or product filter UI observed",
      "confidence": "low",
      "rules": {
        "purpose": "filter rows should refine lists/tables without leaving terminal aesthetic",
        "appearance": "transparent or black controls with gray borders, monospace labels, compact rows",
        "spacing": "gap-2/3 controls, h-9 controls, p-4 wrapper if framed",
        "radius": "square for product pages; rounded-md only if using stock primitives directly",
        "border": "border-gray-700 default, border-gray-500/white hover/focus",
        "shadow": "none unless dropdown/select popover uses shadow-md",
        "typography": "text-sm font-mono with muted labels",
        "states": "active filter should use bg-gray-900 border-gray-600 text-white; disabled opacity-50",
        "variants": [
          "search input",
          "select filter",
          "tab filter",
          "dropdown filter"
        ]
      }
    },
    "form_layouts": {
      "explicit": true,
      "source_basis": "components/ui/form.tsx with Input/Select validation conventions",
      "confidence": "high",
      "rules": {
        "purpose": "structured field composition with accessible descriptions and errors",
        "appearance": "grid-based field stacks with labels, controls, muted descriptions, destructive messages",
        "spacing": "FormItem grid gap-2; descriptions/messages directly under controls",
        "radius": "inherits from controls",
        "border": "inherits control border and invalid destructive border",
        "shadow": "inherits control shadow-xs",
        "typography": "label inherits Label; description text-sm muted; message text-sm destructive",
        "states": "aria-describedby and aria-invalid wired through FormControl; label data-error true turns destructive",
        "variants": [
          "field",
          "description",
          "message",
          "controlled input"
        ]
      }
    }
  },
  "ux_patterns": {
    "cta_hierarchy": "Make the install command the strongest action: white filled, black text, offset border, copy feedback. Documentation/navigation actions use dashed or plain outline. Inline command rows act as tertiary copy actions.",
    "information_grouping": "Group content into terminal-like panels with a chrome header, command body, status footer, and gray border. Docs group topics as stacked bordered blocks with headings, copyable commands, and option lists.",
    "filter_placement": "No explicit filter UI observed. If added, place filters above the affected list/table as compact monospace control rows, not as detached cards.",
    "form_structure": "Use FormItem grid gap-2 with label, control, optional muted description, and destructive message. Keep controls compact and full-width in narrow contexts.",
    "validation_behavior": "Use aria-invalid destructive border/ring, destructive label/message, and preserve accessible describedby wiring from form primitives.",
    "table_detail_strategy": "Tables should be horizontally scrollable, compact, row-hover highlighted, and selected rows use muted background; detail actions should appear as command-style rows or inline terminal links.",
    "loading_error_empty_states": "Loading should feel terminal-native: blinking cursor, bouncing dots, Processing text, pulse status dots. Empty states use centered dashed bordered containers. Errors should use destructive alert/form variants but avoid expanding the palette.",
    "action_placement": "Primary actions appear near section starts or terminal headers; copy actions sit at the right edge of command rows; docs navigation actions live in the left sidebar and close it on mobile.",
    "notes": [
      "The product UI favors direct manipulation of command snippets over conventional form-heavy flows.",
      "Animations are part of the identity but should remain low-amplitude and terminal-relevant.",
      "Use borders and text contrast as the main hierarchy tools; avoid colorful fills except semantic status indicators."
    ]
  },
  "constraints": [
    "Do not introduce broad new color families; preserve monochrome terminal identity.",
    "Do not round terminal/product panels unless intentionally using stock shadcn primitives.",
    "Do not use card elevation without borders; borders are the primary containment device.",
    "Keep interactive feedback visible through text, border, icon, or transform changes.",
    "Maintain responsive command readability; allow wrapping/breaking for long terminal strings on mobile.",
    "Treat components/ui as reusable library evidence and app/page.tsx plus app/docs/page.tsx as product visual evidence."
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
