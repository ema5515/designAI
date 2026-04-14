# Professional Software UI/UX Foundation

## Purpose

This skill teaches an AI agent how to design professional software interfaces using strong UI and UX fundamentals.

It is intentionally style-agnostic. It does not prescribe a specific aesthetic, color palette, density, radius scale, typography family, or visual trend. It defines reusable product design judgment that can be combined with a project-specific style guide, existing design system, or codebase-derived visual language.

Use this foundation whenever generating, reviewing, or improving software interfaces such as dashboards, admin tools, SaaS products, internal tools, data products, settings areas, CRUD workflows, and form-heavy applications.

## Design Philosophy

Professional software UI should help users complete tasks clearly, confidently, and efficiently.

Prioritize clarity over novelty. A screen is successful when users can understand what matters, what they can do, what changed, and what to do next without unnecessary explanation.

Good interface design is not decoration. Every layout, visual treatment, interaction state, and component choice should support usability, hierarchy, comprehension, or task completion.

When a project-specific style guide exists, follow it. When no style guide exists, establish consistent local rules and reuse them throughout the interface.

## UX Fundamentals

### Clarity

- Make the primary purpose of each screen immediately understandable.
- Put the most important task, decision, or status in the strongest visual position.
- Use plain, specific labels instead of vague or clever language.
- Avoid making users infer what a control does from iconography alone unless the icon is universally understood.
- Prefer explicit status, ownership, dates, amounts, and actions over ambiguous summaries.

### Usability

- Optimize for the user’s next likely action.
- Make common tasks easy to find and complete.
- Keep destructive, irreversible, or high-risk actions visually and spatially distinct.
- Place actions close to the content they affect.
- Avoid hiding essential functionality behind hover-only behavior.

### Consistency

- Reuse layout patterns, component structures, spacing, labels, and interaction behavior once established.
- Similar things should look and behave similarly.
- Different things should be visually distinct for a clear reason.
- Do not introduce new button styles, card styles, shadows, radii, or spacing patterns unless the interface needs a new semantic level.

### Feedback And State Visibility

- Every user action should produce visible feedback.
- Show loading, saving, success, warning, error, disabled, selected, focused, and empty states.
- Make system status visible when latency, validation, permissions, or background processing affect the user.
- Confirm completed changes when the outcome is not obvious.
- Show progress for multi-step or long-running processes.

### Cognitive Load Reduction

- Reduce the number of competing decisions on screen.
- Group related information and controls.
- Use progressive disclosure for advanced, rare, or secondary options.
- Prefer recognition over recall by showing context, labels, examples, and current values.
- Avoid dense layouts where users must scan unrelated elements to complete a single task.

### Accessibility

- Maintain sufficient contrast for text, icons, borders, focus indicators, and semantic states.
- Do not communicate meaning through color alone.
- Ensure all interactive elements have visible focus states.
- Use clear labels, helper text, and error messages.
- Preserve keyboard navigation order that matches visual reading order.
- Keep hit targets large enough for comfortable interaction.
- Avoid relying on hover as the only way to reveal important content.

### Responsiveness

- Design layouts that adapt to available space without hiding core tasks.
- On narrow screens, preserve task order and reading order.
- Collapse secondary navigation, filters, metadata, or low-priority columns before primary actions.
- Prevent text overflow, clipped controls, and unstable layout shifts.
- Tables, forms, dashboards, and navigation should each have responsive behavior planned, not left accidental.

### Task-Oriented Design

- Start from what the user is trying to accomplish, not from available data alone.
- Each screen should have a clear primary task or a clear set of related tasks.
- Remove or demote information that does not support the current task.
- Use page titles, section labels, and action labels that reflect user goals.
- Avoid building pages that are only collections of components without workflow logic.

### Progressive Disclosure

- Show essential information first.
- Reveal details, configuration, advanced controls, and secondary actions when needed.
- Use accordions, expandable rows, drill-down pages, popovers, or secondary panels only when they reduce initial complexity.
- Do not hide critical errors, required fields, primary actions, or safety information.

### Predictable Interaction Behavior

- Controls should behave according to platform and product conventions.
- Buttons perform actions. Links navigate. Tabs switch peer views. Accordions reveal nested content. Checkboxes allow independent selection. Radios select one option from a set.
- Avoid using components in ways that contradict user expectations.
- Keep interaction patterns stable across similar screens.

## UI Fundamentals

### Visual Hierarchy

- Create a clear order of importance using size, weight, placement, spacing, contrast, and grouping.
- The primary content should be visually dominant.
- Secondary content should support the primary content without competing with it.
- Avoid screens where every card, heading, button, and badge has equal visual weight.

### Visual Priority

- Assign priority before styling.
- Primary actions should stand out more than secondary actions.
- Current status should be easier to find than historical details.
- Required decisions should be more prominent than optional configuration.
- Use emphasis sparingly so emphasized elements remain meaningful.

### Spacing Rhythm

- Use a consistent spacing scale.
- Related elements should be closer together than unrelated elements.
- Section gaps should be larger than gaps within a section.
- Control groups should have predictable internal spacing.
- Avoid arbitrary margins that make the interface feel uneven or improvised.

### Typography Hierarchy

- Use typography to establish reading order.
- Headings, labels, body text, helper text, metadata, and captions should each have distinct roles.
- Larger or heavier text should indicate importance, not decoration.
- Avoid too many type sizes or weights in a single screen.
- Keep line length readable, especially for descriptions, help text, and settings pages.

### Typography As A UX Tool

- Use headings to answer “Where am I?”
- Use labels to answer “What is this?”
- Use helper text to answer “How should I decide?”
- Use error text to answer “What went wrong and how do I fix it?”
- Use metadata styling to make secondary information scannable without overpowering primary content.
- Align typography choices with scanning behavior: users often scan headings, labels, values, and actions before reading full descriptions.

### Grouping And Alignment

- Align elements to reveal relationships.
- Use consistent left edges, column alignment, and baseline rhythm.
- Group controls with the content they affect.
- Avoid floating controls that are visually disconnected from their context.
- Use dividers, spacing, background shifts, or containers only when they clarify structure.

### Component Consistency

- Components should have consistent anatomy, sizing, spacing, states, and behavior.
- A button should not change radius, shadow, typography, or padding arbitrarily between screens.
- Cards, tables, inputs, filters, navigation items, and modals should follow reusable patterns.
- If variants exist, each variant needs a semantic purpose.

### Contrast Management

- Use contrast to guide attention, not merely to decorate.
- Primary actions and key data need enough contrast to be found quickly.
- Secondary elements should remain readable without dominating the screen.
- Disabled states should look inactive while still being legible when necessary.
- Semantic colors for success, warning, and error must be distinguishable by more than hue.

### Border Radius Logic

- Border radius should follow a defined system.
- Similar components should share the same radius unless their role differs.
- Inputs, buttons, cards, tags, modals, and panels may use different radius values only if the distinction is intentional and consistent.
- Avoid arbitrary radius changes to create visual interest.
- Large radius values should not reduce clarity, alignment, density, or perceived precision.

### Shadow And Elevation Discipline

- Use shadows to communicate elevation, layering, or active surfaces.
- Do not use shadows as generic decoration.
- Keep elevation levels limited and consistent.
- Modals, popovers, dropdowns, sticky bars, and raised panels may use elevation when they sit above other content.
- Avoid stacking multiple shadow styles without a clear depth model.

### Emphasis Control

- Not everything can be important at once.
- Limit high-emphasis treatments to primary actions, urgent statuses, active navigation, selected items, and critical information.
- Use subtle emphasis for supporting content.
- Reduce visual noise by avoiding unnecessary badges, borders, fills, icons, shadows, and colored backgrounds.

## Visual Priority And Hierarchy Rules

- Identify the primary user task before laying out the screen.
- Place primary content and primary actions where users naturally scan first.
- Use one dominant focal point per screen or section.
- Separate page-level hierarchy from component-level hierarchy.
- Use whitespace as structure, not empty decoration.
- Make important values, statuses, and actions easier to scan than labels and explanations.
- Avoid giving equal weight to navigation, filters, content, and actions.
- Reduce emphasis on repeated UI chrome so actual content can stand out.
- Use alignment and spacing before adding borders or backgrounds.
- When everything feels too loud, reduce contrast, size, color, or container treatment on secondary elements.

## Typography As UX Rules

- Use typography to create a clear reading path from page title to section title to content to action.
- Keep headings concise and specific.
- Pair labels with values consistently.
- Use sentence case or title case according to the project style guide, then apply it consistently.
- Avoid long all-caps labels except for very small metadata categories.
- Use body text for explanation, not headings.
- Use helper text only when it reduces uncertainty.
- Error messages should be specific, actionable, and placed near the field or action that caused them.
- Numeric data should align consistently and use formatting that supports comparison.
- In dense UIs, typography must improve scanning through size, weight, spacing, and alignment.

## Interaction State Rules

### Hover

- Hover states should indicate interactivity.
- Use hover to clarify affordance, not to reveal essential information exclusively.
- Hover changes should be noticeable but not disruptive.
- Avoid layout shifts on hover.

### Focus

- Focus states must be visible and accessible.
- Keyboard users should always know where they are.
- Focus styling should work on light, dark, and mixed backgrounds.
- Do not remove default focus behavior unless replacing it with an equally clear custom state.

### Active Or Pressed

- Active states should confirm that a control is being pressed or activated.
- Use active feedback for buttons, toggles, menu items, and interactive rows.
- The pressed state should feel connected to the default and hover states.

### Selected

- Selected states should be persistent and clearly distinguishable from hover.
- Use selected states for tabs, navigation items, filters, rows, cards, options, and toggles.
- Selected items should remain understandable without relying only on color.

### Disabled

- Disabled controls should communicate that an action is unavailable.
- When the reason is not obvious, provide helper text, tooltip text, or inline explanation.
- Disabled controls should not look like loading controls.
- Avoid disabling primary actions without explaining what is required.

### Loading

- Use loading states when data, validation, submission, or processing takes time.
- Prefer skeletons for content loading and spinners for short isolated actions.
- Preserve layout stability during loading.
- For submissions, prevent duplicate actions and show whether the system is saving, processing, or retrying.

### Success, Warning, And Error

- Success states confirm completion.
- Warning states identify risk before damage occurs.
- Error states explain what failed and how to recover.
- Use semantic styling consistently.
- Place feedback close to the relevant action or content.

### Empty States

- Empty states should explain what is missing and what the user can do next.
- Provide a primary action when there is a clear next step.
- Avoid decorative empty states that do not help the user proceed.
- Distinguish between first-use empty states, filtered empty states, error empty states, and permission-limited empty states.

### Validation Feedback

- Validate as close to the source of input as practical.
- Show field-level errors near fields.
- Show form-level errors when submission fails for cross-field or system reasons.
- Preserve user input after validation errors.
- Use clear messages that tell users how to fix the issue.

## Layout Rules

### Dashboards

- Dashboards should prioritize monitoring, comparison, and action.
- Put the most important metrics, alerts, or work queues first.
- Avoid filling dashboards with decorative charts that do not support decisions.
- Use consistent card and chart sizing.
- Provide time ranges, filters, and definitions when metrics may be ambiguous.
- Make anomalies, trends, and required actions easier to find than static totals.

### Data-Heavy Pages

- Optimize for scanning, sorting, filtering, comparison, and bulk action.
- Use tables for structured records with repeated attributes.
- Keep important identifiers and statuses visible.
- Provide meaningful empty, loading, error, and filtered states.
- Avoid hiding essential data behind excessive card layouts.
- Support density controls when users have different scanning needs.

### CRUD Pages

- Separate list, detail, create, edit, and delete flows clearly.
- Use list views for finding records.
- Use detail pages for reviewing a record and its related data.
- Use forms for creating or editing.
- Confirm destructive actions and explain consequences.
- Keep primary record actions consistent across similar resources.

### Settings Pages

- Group settings by user mental model, not implementation model.
- Use clear section titles and descriptions.
- Show current values and consequences of changes.
- Save behavior must be obvious: immediate save, explicit save, or staged changes.
- Dangerous settings should be separated from routine configuration.

### Forms

- Group related fields into clear sections.
- Place labels close to inputs.
- Mark required and optional fields consistently.
- Use helper text for constraints, examples, or consequences.
- Put primary submit actions where users expect them after completing the form.
- Preserve data and show actionable errors after failed submission.
- Avoid multi-column forms when fields need a strong reading sequence.

### Tables

- Use tables when users compare many records across shared attributes.
- Align column content consistently.
- Keep headers visible or easy to reference in large tables.
- Prioritize columns based on task importance.
- Use row actions consistently.
- Avoid excessive badges, icons, or controls in every cell unless they support scanning or action.
- Provide sorting, filtering, pagination, or virtualization when data volume requires it.

### Cards

- Use cards for distinct objects, summaries, previews, or grouped actions.
- A card should have a clear subject and purpose.
- Avoid cards inside cards unless the inner card represents a truly distinct repeated item.
- Keep card actions predictable and visually connected to the card content.
- Do not use cards as a default replacement for all layout structure.

### Navigation

- Navigation should reflect product structure and user tasks.
- Keep labels short, specific, and consistent.
- Show current location clearly.
- Group navigation items logically.
- Avoid mixing unrelated destinations at the same hierarchy level.
- Preserve predictable navigation placement across the product.

### Modals And Sheets

- Use modals for focused tasks that interrupt the current flow intentionally.
- Use sheets for contextual editing, inspection, or secondary workflows when preserving background context helps.
- Avoid modals for complex multi-step tasks, deep editing, or content that needs full-page space.
- Always provide clear close, cancel, and primary action behavior.
- Prevent accidental destructive actions inside modals.

### Alerts And Inline Feedback

- Use alerts for important system-level or page-level messages.
- Use inline feedback for field-level, row-level, or component-level issues.
- Avoid persistent alert banners for low-importance information.
- Alerts should explain the issue and provide recovery when applicable.
- Use semantic severity consistently.

### Filters And Search Areas

- Put filters close to the data they affect.
- Make active filters visible.
- Provide clear reset behavior.
- Use search for keyword matching and filters for structured refinement.
- Avoid hiding commonly used filters behind advanced controls.
- Collapse rare filters only when the active state remains visible.

## Component Rules

- Buttons need clear hierarchy: primary, secondary, tertiary, destructive, and disabled.
- Primary buttons should represent the main intended action in the current context.
- Secondary buttons should support alternative actions without competing.
- Destructive buttons should be visually distinct and paired with confirmation when risk is high.
- Inputs should include labels, values, placeholders only when helpful, helper text when needed, and validation states.
- Selects, comboboxes, radios, and checkboxes should be chosen according to option count and selection behavior.
- Tabs should switch between peer views without changing the overall task context.
- Accordions should reveal optional or secondary content within the same page.
- Badges should communicate compact status or category, not decorate headings.
- Tooltips should clarify small uncertainties, not contain essential instructions.
- Icons should support labels and scanning; avoid icon-only controls unless space or convention justifies them.
- Cards should group coherent content and actions.
- Tables should support comparison and data operations.
- Modals should focus attention on a bounded task.
- Toasts should confirm transient outcomes, not replace persistent error handling.

## Decision Heuristics

### Card Vs Table

Use a card when each item is a distinct object, summary, preview, or content unit with variable structure.

Use a table when users need to compare many records across the same attributes, scan rows, sort columns, filter data, or perform bulk actions.

Choose a table for operational data. Choose cards for discovery, summaries, galleries, or object previews.

### Modal Vs Dedicated Page

Use a modal for short, focused, reversible tasks that depend on the current context.

Use a dedicated page for complex forms, multi-step workflows, deep review, heavy content, collaboration, or tasks users may need to bookmark, revisit, or share.

Do not force complex creation or editing flows into modals when users need space and context.

### Tabs Vs Accordion

Use tabs for switching between peer sections at the same hierarchy level.

Use accordions for revealing or hiding sections within a single flow.

Tabs imply separate views. Accordions imply expandable content on the same view.

Avoid tabs when users need to compare all sections at once.

### Sidebar Vs Top Navigation

Use a sidebar when the product has many persistent sections, nested destinations, or admin-style workflows.

Use top navigation when the product has a small number of primary areas or benefits from a broader content canvas.

Do not use both heavily unless each has a distinct role.

### Spacious Vs Compact Layout

Use spacious layouts for onboarding, low-frequency decisions, complex comprehension, marketing-adjacent product areas, or workflows where confidence matters more than speed.

Use compact layouts for expert tools, dashboards, dense data, repeated operations, and high-frequency workflows.

Do not make dense workflows spacious at the cost of scanning efficiency. Do not make complex decisions cramped.

### High Emphasis Vs Subtle Emphasis

Use high emphasis for primary actions, critical states, selected navigation, dangerous warnings, and essential data.

Use subtle emphasis for secondary metadata, supporting controls, optional information, and repeated structure.

If too many elements need high emphasis, revisit the screen hierarchy.

### Dense Information View Vs Progressive Disclosure

Use dense information views when users need comparison, monitoring, or expert scanning.

Use progressive disclosure when users need guidance, when information is optional, or when too much detail would slow the primary task.

Do not hide information that is required to make a correct decision.

## Anti-Patterns

- Decorative UI without functional purpose.
- Visual novelty that makes tasks harder to understand.
- Flat hierarchy where every element competes equally.
- Inconsistent spacing between similar elements.
- Weak CTA hierarchy where primary and secondary actions look equally important.
- Multiple unrelated primary actions in the same visual area.
- Inaccessible contrast for text, icons, borders, or states.
- Weak or missing keyboard focus feedback.
- Interaction states that rely only on color.
- Arbitrary border radius changes across similar components.
- Arbitrary shadow changes without an elevation model.
- Overdesigned controls that distract from the workflow.
- Cramped grouping that makes unrelated elements feel connected.
- Excessive containers, borders, cards, and dividers.
- Cards used where a table would better support comparison.
- Modals used for complex workflows that need a full page.
- Tabs used for non-peer content.
- Accordions used to hide essential information.
- Hover-only actions with no keyboard or touch equivalent.
- Disabled actions with no explanation.
- Error messages that describe failure but not recovery.
- Empty states that are only decorative.
- Inconsistent loading behavior across similar actions.
- Inconsistent labels for the same concept.
- Icons used without labels when meaning is not obvious.
- Layout shifts caused by hover, loading, validation, or dynamic content.

## Final Behavioral Rules For The AI

- Prioritize clarity over novelty.
- Design around the user’s task, not around visual decoration.
- Create clear focal points on every screen.
- Establish visual hierarchy before adding detail.
- Maintain consistent spacing rhythm.
- Use typography intentionally to guide reading order and scanning.
- Group related information and actions.
- Reuse established patterns once they exist.
- Keep interaction states complete and predictable.
- Make feedback visible for user actions and system changes.
- Choose components based on usability, not aesthetic preference.
- Justify layout choices through task flow, density, comparison needs, and user risk.
- Prefer accessible, readable, resilient interfaces.
- Avoid arbitrary radius, shadow, color, spacing, or typography decisions.
- Keep screens production-ready, responsive, and state-complete.
- When combined with a project-specific style guide, preserve these UX principles while adopting the project’s visual language.