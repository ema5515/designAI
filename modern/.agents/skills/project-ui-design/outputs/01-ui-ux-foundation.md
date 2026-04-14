# Professional Software Interface Design Foundation

## Purpose

This skill teaches an AI agent how to design professional software interfaces with strong UI and UX fundamentals before applying any project-specific visual style.

Use this foundation when designing, reviewing, or improving software interfaces such as dashboards, admin tools, SaaS products, internal tools, data-heavy applications, settings screens, forms, tables, workflows, and CRUD experiences.

This skill is intentionally style-agnostic. It does not prescribe a brand, color palette, aesthetic direction, component library, or visual trend. It defines durable product design principles that can later be combined with a project-specific design system or style guide extracted from a real codebase.

## Design Philosophy

Design software interfaces for comprehension, action, and trust.

A professional interface should make the user’s next step clear, reduce unnecessary decisions, expose system state, prevent avoidable errors, and support efficient task completion. Visual design should serve usability before decoration.

Core philosophy:

- Prioritize clarity over novelty.
- Prioritize task completion over visual complexity.
- Prioritize consistency over one-off cleverness.
- Prioritize accessible, predictable behavior over subtle effects.
- Prioritize reusable patterns over isolated screen design.
- Use visual hierarchy to explain importance.
- Use spacing, typography, alignment, and state feedback as functional tools.
- Make the interface feel intentional even before a visual style is applied.

A good software UI should answer these questions quickly:

- Where am I?
- What is most important?
- What can I do next?
- What changed?
- What requires my attention?
- What happens if I take this action?
- How do I recover if something goes wrong?

## UX Fundamentals

### Clarity

Clarity means the user can understand the screen, its purpose, and available actions without unnecessary interpretation.

Rules:

- Every screen should have a clear primary purpose.
- The main action should be obvious without relying only on color.
- Labels should describe the user’s goal, not the implementation detail.
- Avoid vague actions like “Submit” when a specific verb is available, such as “Create invoice,” “Save changes,” or “Invite user.”
- Use plain language over internal terminology unless the product domain requires specialized terms.
- Avoid making multiple unrelated tasks compete for attention on the same screen.
- If a user must make a decision, provide enough context to make that decision confidently.

### Usability

Usability means the interface supports efficient, accurate task completion.

Rules:

- Put frequent actions close to the content they affect.
- Put destructive or rare actions away from primary task paths.
- Use familiar interaction patterns unless there is a strong product reason not to.
- Reduce unnecessary steps in common workflows.
- Preserve user input when validation fails.
- Provide clear recovery paths for errors.
- Do not require users to remember information across screens when it can be shown in context.
- Optimize first for the primary user flow, then support secondary flows without cluttering the main path.

### Consistency

Consistency reduces learning cost and increases user confidence.

Rules:

- Similar actions should look and behave similarly.
- Similar information should be structured similarly.
- Reuse spacing, typography, component variants, icon behavior, and state patterns once established.
- Do not introduce a new component variation unless it solves a real interaction or information problem.
- Keep action placement predictable across similar pages.
- Keep terminology consistent across navigation, page titles, buttons, forms, empty states, and alerts.

### Feedback And State Visibility

Users need to know what the system is doing and what changed.

Rules:

- Show loading states for actions that are not immediate.
- Show success feedback after important changes.
- Show validation feedback near the field or control that needs correction.
- Show selected, active, disabled, and focused states clearly.
- Show unsaved changes when leaving a form could cause data loss.
- Show progress for multi-step or long-running operations.
- Do not leave users wondering whether a click, save, upload, or filter action worked.

### Cognitive Load Reduction

Reduce the amount of information the user must hold in memory.

Rules:

- Group related controls and content.
- Break complex workflows into clear sections or steps.
- Use progressive disclosure for advanced, rare, or optional details.
- Prefer recognition over recall by showing available options.
- Avoid presenting every possible action at once.
- Use defaults, examples, summaries, and contextual help when they prevent confusion.
- Keep visual hierarchy strong enough that users can scan before reading deeply.

### Accessibility

Accessibility is a baseline requirement, not an enhancement.

Rules:

- Text and interactive elements must meet appropriate contrast requirements.
- Focus states must be visible and not rely on color alone.
- Interactive targets must be large enough for pointer and touch use.
- Form fields must have persistent labels or accessible names.
- Error states must include text, not only color or icons.
- Disabled controls should explain why they are unavailable when the reason is not obvious.
- Keyboard users must be able to reach and operate all interactive controls.
- Screen-reader order should match visual reading order.
- Do not use placeholder text as the only label.
- Avoid interactions that depend only on hover.

### Responsiveness

Responsive design means the interface adapts without losing usability.

Rules:

- Preserve task priority across viewport sizes.
- Collapse secondary navigation before hiding primary actions.
- Stack related content in a logical reading order on smaller screens.
- Keep primary actions reachable on mobile.
- Avoid horizontal scrolling except for intentionally wide data tables.
- Ensure text wraps gracefully without truncating essential meaning.
- Use compact density only when readability and target size remain acceptable.
- Test layouts at narrow, medium, wide, and content-heavy states.

### Task-Oriented Design

Design around what users need to accomplish, not around component inventory.

Rules:

- Start each screen by identifying the primary task.
- Rank content and actions by task importance.
- Keep the main workflow visible and direct.
- Move supporting metadata, history, advanced options, and secondary actions into lower-emphasis areas.
- Avoid decorative sections that do not help the user decide, understand, or act.
- Prefer “what the user is trying to do” over “what the system can display.”

### Progressive Disclosure

Progressive disclosure reveals complexity only when it becomes useful.

Rules:

- Show essential information first.
- Hide advanced controls behind expandable areas, secondary panels, detail views, or explicit actions.
- Do not hide required information needed to make a safe decision.
- Use disclosure for optional configuration, detailed metadata, audit history, advanced filters, and rare actions.
- Make disclosed content predictable: the label should clearly describe what will appear.
- Preserve state when users expand, collapse, or return to a disclosed section.

### Predictable Interaction Behavior

Users should be able to predict what an interaction will do.

Rules:

- Buttons should perform actions.
- Links should navigate.
- Checkboxes should allow multiple independent selections.
- Radio buttons should select one option from a visible set.
- Tabs should switch between peer views, not submit data.
- Accordions should reveal content, not navigate unexpectedly.
- Destructive actions should require clear confirmation when consequences are significant.
- Interactions should not move controls unexpectedly after hover, focus, or validation.

## UI Fundamentals

### Visual Hierarchy

Visual hierarchy guides the user through the screen in order of importance.

Rules:

- Establish one dominant focal point per screen or region.
- Use size, weight, spacing, alignment, position, and contrast to create hierarchy.
- Primary content should be visually stronger than supporting content.
- Primary actions should be more prominent than secondary actions.
- Metadata should not compete with titles, values, or task-critical labels.
- Avoid flat layouts where every element has similar size, weight, color, and spacing.

### Visual Priority

Visual priority determines what the user notices first, second, and third.

Rules:

- Assign priority before styling.
- High-priority elements may use stronger weight, clearer placement, greater contrast, or more surrounding space.
- Low-priority elements should remain readable but visually quieter.
- Avoid giving high emphasis to too many elements at once.
- Use visual priority to support task order, not decoration.
- If everything is emphasized, nothing is emphasized.

### Spacing Rhythm

Spacing creates structure and improves scanning.

Rules:

- Use a consistent spacing scale.
- Use tighter spacing for closely related elements.
- Use larger spacing to separate groups, sections, or task areas.
- Avoid arbitrary one-off spacing values.
- Keep spacing rhythm consistent across similar components.
- Do not use borders or shadows to compensate for weak spacing.
- Crowded interfaces should first improve grouping and hierarchy before reducing font size.

### Typography Hierarchy

Typography should communicate structure and reading order.

Rules:

- Use a limited set of text roles: page title, section title, item title, body text, label, helper text, metadata, caption, and button text.
- Larger or heavier type should correspond to higher information importance.
- Labels should be concise and scannable.
- Body text should be readable at normal distances.
- Metadata should be visually subordinate but still legible.
- Avoid using too many font sizes or weights.
- Do not rely on all caps for hierarchy unless the design system already uses it carefully.

### Typography As A UX Tool

Typography helps users scan, compare, and act.

Rules:

- Put the most meaningful words first in labels and headings.
- Use predictable text patterns across repeated items.
- Use line length that supports reading, especially for descriptions and help text.
- Align numeric data consistently for comparison.
- Use tabular or aligned numbers where precise comparison matters.
- Avoid center alignment for dense, operational, or data-heavy content.
- Use truncation only when full content is available through expansion, tooltip, detail view, or responsive layout.

### Grouping And Alignment

Grouping tells users what belongs together.

Rules:

- Align related elements along clear edges.
- Keep labels close to the fields or values they describe.
- Group controls with the content they affect.
- Use section headings when groups need names.
- Avoid floating controls with unclear scope.
- Use consistent alignment for repeated content.
- Prefer strong layout structure over decorative dividers.

### Component Consistency

Components should behave as part of a system.

Rules:

- Use the same component for the same job.
- Use variants intentionally: primary, secondary, tertiary, destructive, disabled, selected, and loading should each have clear meaning.
- Do not create visual variants only for novelty.
- Keep icon placement, button height, input styling, table density, and card structure consistent.
- Component changes should reflect state, hierarchy, or function.

### Contrast Management

Contrast controls readability and emphasis.

Rules:

- Maintain accessible contrast for text and important controls.
- Use stronger contrast for primary information and actions.
- Use lower contrast for secondary metadata, but never so low that it becomes hard to read.
- Do not use color alone to communicate status.
- Avoid high-contrast noise in dense screens.
- Use background contrast to separate major regions only when spacing and hierarchy are insufficient.

### Border Radius Logic

Border radius should be systematic.

Rules:

- Use a consistent radius scale.
- Similar components should share similar radius.
- Large containers, small controls, inputs, badges, and overlays may use different radii only if the system defines that logic.
- Do not vary radius arbitrarily across cards, buttons, inputs, and panels.
- Avoid excessive rounding when it conflicts with dense professional software UI.
- Radius should support component identity, not act as decoration.

### Shadow And Elevation Discipline

Elevation should communicate layering, not visual flair.

Rules:

- Use shadows only when an element is above another surface or needs separation.
- Modals, popovers, dropdowns, floating toolbars, and sticky elements may need elevation.
- Static cards and sections often do not need heavy shadows.
- Avoid stacking multiple shadow styles without a clear elevation system.
- Do not use shadows as the primary method of grouping.
- Elevation should be subtle, consistent, and functional.

### Emphasis Control

Emphasis must be scarce and intentional.

Rules:

- Use high emphasis for primary actions, urgent statuses, active navigation, and task-critical information.
- Use medium emphasis for secondary actions and important supporting content.
- Use low emphasis for metadata, optional context, and repeated secondary details.
- Do not emphasize decorative labels, redundant icons, or non-actionable content.
- Reduce emphasis when a screen feels noisy before adding more styling.

## Visual Priority And Hierarchy Rules

When generating a screen, determine hierarchy in this order:

1. Identify the primary user task.
2. Identify the primary content needed for that task.
3. Identify the primary action.
4. Identify secondary actions.
5. Identify status, feedback, or risk information.
6. Identify metadata and supporting details.
7. Assign visual weight based on this order.

Practical rules:

- The page title should orient the user, not compete with the main task area.
- The primary action should be easy to find but not overwhelm the content.
- Destructive actions should be visually distinct from primary positive actions.
- Repeated items should have a consistent internal hierarchy.
- Empty, loading, and error states should preserve the same hierarchy as the loaded state when possible.
- Dense pages need stronger grouping, not more decoration.
- Important values should be visually stronger than their labels.
- Warnings and errors should interrupt only when user attention is required.

## Typography As UX Rules

Use typography to create a clear reading path.

Rules:

- Use headings to establish structure, not to decorate sections.
- Use short headings that match user intent.
- Use labels that remain visible after input.
- Use helper text only when it prevents mistakes or clarifies constraints.
- Keep error text direct and actionable.
- Use sentence case unless the project style guide specifies otherwise.
- Use consistent terminology for the same object and action.
- Avoid paragraph-heavy UI; convert instructions into concise labels, hints, steps, or inline feedback.
- Keep button labels action-oriented.
- Avoid ambiguous verbs such as “Process,” “Proceed,” or “Confirm” when a specific action is available.
- In data views, prioritize names, statuses, dates, owners, amounts, and actions according to the user’s task.

## Interaction State Rules

### Hover

Hover should indicate interactivity.

Rules:

- Use hover for interactive elements only.
- Hover should not be the only way to reveal essential actions.
- Hover changes should be subtle and layout-stable.
- Do not shift size, position, or surrounding layout on hover.
- In dense tables, row hover may help show action scope.

### Focus

Focus is required for keyboard navigation and accessibility.

Rules:

- Every interactive element must have a visible focus state.
- Focus should be at least as visible as hover.
- Focus indicators must not rely on color alone if contrast is weak.
- Do not remove browser focus behavior unless replacing it with an accessible equivalent.
- Focus order must follow the visual and task order.

### Active And Pressed

Active states confirm immediate interaction.

Rules:

- Buttons, toggles, menu items, and tabs should visibly respond when pressed.
- Active feedback should be brief and not confused with selected state.
- Pressed states should not imply success; success requires its own feedback when relevant.

### Selected

Selected state indicates a persistent choice.

Rules:

- Selected items must be visually distinct from hover and focus.
- Selected navigation should clearly show the current location.
- Selected filters should be easy to review and clear.
- Multi-select states should show count and available batch actions when useful.

### Disabled

Disabled state indicates an unavailable action.

Rules:

- Use disabled only when the action is truly unavailable.
- If the reason is not obvious, explain it through helper text, tooltip, inline message, or permission notice.
- Disabled controls must remain legible.
- Do not hide unavailable actions when seeing them helps users understand permissions, requirements, or workflow state.

### Loading

Loading states should preserve context.

Rules:

- Use skeletons for content areas where shape is predictable.
- Use spinners for short, localized actions.
- Use progress indicators for long-running or multi-step operations.
- Keep layout stable while loading.
- Disable repeated submissions when an action is in progress.
- Show loading state on the control that initiated the action when possible.

### Success, Warning, And Error

Status feedback should be clear, contextual, and proportional.

Rules:

- Success confirms completion of important actions.
- Warnings indicate risk, dependency, or caution before failure.
- Errors explain what went wrong and how to recover.
- Use inline errors for field-specific issues.
- Use page-level or alert errors for system-wide failures.
- Use destructive styling only for destructive or critical states.
- Do not overuse success alerts for trivial actions.

### Empty States

Empty states should help users move forward.

Rules:

- Explain what is missing.
- Explain why it matters when helpful.
- Provide the best next action.
- Avoid decorative emptiness that does not help the user.
- For first-use empty states, guide setup.
- For filtered empty states, offer filter clearing or search adjustment.
- For permission-based empty states, explain access limits.

### Validation Feedback

Validation should prevent and correct errors.

Rules:

- Validate as early as useful, but avoid interrupting before the user has had a chance to complete input.
- Show errors near the relevant field.
- Preserve entered data.
- Explain the required fix.
- Use examples for complex formats.
- Summarize errors at the top for long forms while keeping field-level messages.
- Do not rely only on red borders.

## Layout Rules

### General Layout

Rules:

- Start with the user’s primary task and build the layout around it.
- Use a clear page structure: header, primary content, supporting content, actions, feedback.
- Keep related information visually grouped.
- Keep primary actions in predictable locations.
- Avoid placing unrelated controls in the same toolbar or section.
- Use whitespace to separate meaningfully different areas.
- Avoid full-width content when narrower line lengths improve readability.
- Use full-width layouts when comparing data across columns or managing dense operational workflows.

### Dashboards

Dashboards should summarize status and guide investigation.

Rules:

- Lead with the most decision-relevant metrics, alerts, or trends.
- Avoid turning dashboards into collections of disconnected cards.
- Group metrics by user question or operational area.
- Show comparison, trend, or threshold when a number alone is not meaningful.
- Make drill-down paths obvious.
- Use charts only when they improve understanding.
- Avoid excessive decorative charts that do not support decisions.
- Keep dashboard actions secondary unless the dashboard is also a control surface.

### Data-Heavy Pages

Data-heavy pages should support scanning, comparison, filtering, and action.

Rules:

- Prioritize columns by task relevance.
- Put identifiers, names, statuses, dates, owners, and key metrics where users expect them.
- Use alignment to support comparison.
- Use density intentionally; compact layouts still need readable text and clear targets.
- Keep filters visible when they are central to the task.
- Provide saved views, sorting, column control, or bulk actions when data complexity requires them.
- Use progressive disclosure for row details, histories, logs, and secondary metadata.
- Avoid card layouts when users need to compare many records precisely.

### CRUD Pages

CRUD experiences should make create, read, update, and delete actions predictable.

Rules:

- List pages should support finding, filtering, sorting, viewing, and creating records.
- Detail pages should show the record identity, status, metadata, primary actions, and related data.
- Create and edit pages should clearly distinguish new unsaved data from existing data.
- Destructive actions should be separated and confirmed.
- After create, update, or delete, show clear feedback and navigate to the most useful next context.
- Preserve user context when returning from detail or edit pages.

### Settings Pages

Settings pages should be calm, structured, and easy to verify.

Rules:

- Group settings by user mental model, not backend schema.
- Use clear section names.
- Explain settings with consequences or dependencies.
- Save behavior must be obvious: auto-save, section save, or page save.
- Show unsaved changes when relevant.
- Separate dangerous settings from routine configuration.
- Use defaults and current values clearly.
- Avoid burying critical permissions, billing, or security settings.

### Forms

Forms should reduce effort and prevent mistakes.

Rules:

- Ask only for information needed for the task.
- Group fields by meaning.
- Use one clear label per field.
- Mark required and optional fields consistently.
- Use helper text for constraints, examples, or consequences.
- Keep validation close to the relevant field.
- Align actions with the form completion path.
- Place destructive or cancel actions away from the primary submit action.
- Use multi-step forms only when sections are meaningfully distinct or the form is too complex for one page.
- Preserve input on errors and navigation interruptions when possible.

### Tables

Tables are for comparison, scanning, and structured records.

Rules:

- Use tables when rows share the same attributes.
- Keep column names short and clear.
- Align text, numbers, dates, statuses, and actions consistently.
- Keep row actions scoped and predictable.
- Use sticky headers or columns only when they solve a real navigation problem.
- Provide empty, loading, filtered, and error states.
- Use row expansion for secondary detail when it supports scanning.
- Do not overload tables with unrelated actions, nested controls, or excessive badges.

### Cards

Cards are for grouped summaries, objects, or choices.

Rules:

- Use cards when each item benefits from visual grouping or variable content.
- Keep card structure consistent across repeated cards.
- Make the main click target clear.
- Do not place too many competing actions inside a card.
- Use cards for dashboards, summaries, resources, previews, or object collections where comparison is loose.
- Avoid cards for dense tabular comparison.
- Do not put cards inside cards unless the nested card is a distinct repeated object with a clear reason.

### Navigation

Navigation should orient users and support predictable movement.

Rules:

- Navigation labels should match user goals and product objects.
- Active location must be visible.
- Keep primary navigation stable.
- Do not mix global navigation, local navigation, and filters without clear separation.
- Use breadcrumbs for deep hierarchies or detail pages.
- Use sidebar navigation for many persistent destinations.
- Use top navigation for fewer top-level destinations or broad product areas.
- Keep destructive or transactional actions out of primary navigation.

### Modals And Sheets

Modals and sheets should interrupt only when the task requires focused attention.

Rules:

- Use modals for focused, short tasks, confirmations, lightweight creation, or blocking decisions.
- Use dedicated pages for complex forms, multi-step workflows, deep editing, or tasks requiring reference context.
- Keep modal titles specific.
- Keep modal actions clear and limited.
- Make dismissal behavior predictable.
- Warn users before losing unsaved modal changes.
- Use sheets when users need to keep some parent context visible while editing or inspecting related detail.

### Alerts And Inline Feedback

Feedback should appear where users need it.

Rules:

- Use inline feedback for field-level or section-level issues.
- Use alerts for page-level, system-level, or workflow-level messages.
- Keep alert language concise and actionable.
- Do not stack many alerts without priority.
- Avoid persistent success messages for minor actions.
- Warnings should explain risk before the user commits.
- Errors should provide recovery steps.

### Filters And Search Areas

Filters and search should help users narrow information quickly.

Rules:

- Place filters close to the data they affect.
- Make active filters visible.
- Provide clear reset behavior.
- Distinguish search from filters.
- Use default filters only when they match user expectations.
- Use advanced filters for less common criteria.
- Show filtered empty states that help users recover.
- Avoid hiding active constraints in menus without visible summary.

## Component Rules

### Buttons

Rules:

- One primary button per task area.
- Use secondary buttons for alternative actions.
- Use tertiary or text buttons for low-emphasis actions.
- Use destructive buttons only for destructive actions.
- Button labels should describe the action result.
- Keep button order consistent across the product.
- Loading buttons should prevent duplicate submission.

### Inputs

Rules:

- Labels must be visible or programmatically available.
- Placeholder text should provide examples, not replace labels.
- Input width should match expected content when practical.
- Required, optional, disabled, error, and success states should be clear.
- Use appropriate input types for dates, numbers, currency, passwords, URLs, and search.

### Selects, Comboboxes, And Dropdowns

Rules:

- Use select controls for known option sets.
- Use comboboxes when search is needed within options.
- Use menus for actions, not form values.
- Keep option labels clear and scannable.
- Show selected values clearly.
- Avoid long dropdowns without search or grouping.

### Toggles, Checkboxes, And Radio Buttons

Rules:

- Use toggles for immediate on/off settings.
- Use checkboxes for independent multi-select choices.
- Use radio buttons for mutually exclusive choices where options should be visible.
- Label controls by the state or choice they represent.
- Explain consequences for settings that affect behavior or access.

### Badges And Status Indicators

Rules:

- Use badges for compact status, category, or count information.
- Status labels must be text-readable, not color-only.
- Use a consistent status vocabulary.
- Avoid badge overload in dense lists.
- Do not style decorative labels like critical statuses.

### Icons

Rules:

- Icons should clarify, not replace, important labels unless the meaning is universally understood.
- Use consistent icon style and size.
- Provide accessible names for icon-only controls.
- Avoid using multiple icon metaphors for the same action.
- Do not use icons as decoration in operational UI unless they support scanning.

## Decision Heuristics

### Card Vs Table

Use a table when:

- Users need to compare many records across shared attributes.
- Sorting, filtering, scanning, or bulk actions are important.
- Precise values, dates, statuses, owners, or amounts matter.
- Density and consistency are more important than visual storytelling.

Use cards when:

- Items have variable content or need summary presentation.
- Users are browsing or choosing rather than comparing precisely.
- Each item benefits from a preview, description, image, or grouped actions.
- The collection is small or medium-sized.

Default heuristic: if users ask “which records match these conditions?” use a table. If users ask “which option or object should I open?” cards may work.

### Modal Vs Dedicated Page

Use a modal when:

- The task is short and focused.
- The user should remain in the parent context.
- The action is confirmatory or lightweight.
- Required inputs are minimal.

Use a dedicated page when:

- The task is complex, long, or multi-step.
- Users need reference information while working.
- The workflow has significant consequences.
- The screen requires deep validation, collaboration, or navigation.

Default heuristic: if the task may grow, require careful review, or include many fields, use a page.

### Tabs Vs Accordion

Use tabs when:

- Sections are peer-level views.
- Users switch between categories of content.
- Only one section should be viewed at a time.
- The first-level structure is stable and limited.

Use accordions when:

- Users may need to scan several sections in one flow.
- Content is optional or progressively disclosed.
- Sections are part of a longer page.
- Multiple sections may be opened for comparison or reference.

Default heuristic: tabs change views; accordions reveal details.

### Sidebar Vs Top Navigation

Use sidebar navigation when:

- There are many destinations.
- The app has persistent operational sections.
- Users frequently switch between areas.
- Navigation labels need more horizontal room.

Use top navigation when:

- There are few top-level destinations.
- The product is simpler or content-led.
- The main layout benefits from more horizontal content space.
- Navigation represents broad product areas rather than many tools.

Default heuristic: complex applications usually benefit from sidebar navigation; simpler products can use top navigation.

### Spacious Vs Compact Layout

Use spacious layout when:

- The task requires careful reading or decision-making.
- The page has forms, settings, onboarding, or explanatory content.
- The user needs confidence more than speed.
- The screen is used infrequently.

Use compact layout when:

- Users work with high-volume data.
- Scanning and comparison are primary.
- Users are experienced and repeat tasks often.
- More visible rows or controls improve efficiency.

Default heuristic: compactness is earned by task frequency and data density, not by aesthetic preference.

### High Emphasis Vs Subtle Emphasis

Use high emphasis when:

- The element is the primary action.
- The message is urgent or blocking.
- The value is task-critical.
- The item represents current location or selected state.

Use subtle emphasis when:

- The element is secondary, repeated, metadata, or optional.
- The user only needs it after initial scanning.
- Too much emphasis would create noise.

Default heuristic: high emphasis should be rare enough to remain meaningful.

### Dense Information View Vs Progressive Disclosure

Use dense information views when:

- Users need to compare, monitor, or operate quickly.
- Information is structured and repeatable.
- The user is likely to be experienced.
- Hiding details would slow the task.

Use progressive disclosure when:

- Information is optional, advanced, rare, or secondary.
- The screen would otherwise overwhelm users.
- Users need a guided path.
- Details are useful only after selecting or expanding an item.

Default heuristic: show what users need to decide now; disclose what they need after choosing.

## Anti-Patterns

Avoid these patterns:

- Decorative UI that does not improve comprehension, navigation, action, or feedback.
- Flat hierarchy where titles, metadata, buttons, cards, and alerts all compete equally.
- Inconsistent spacing that makes grouping unclear.
- Weak CTA hierarchy where primary, secondary, destructive, and tertiary actions look too similar.
- Inaccessible contrast or focus states that are hard to see.
- Arbitrary radius changes between similar components.
- Arbitrary shadow changes without elevation logic.
- Overdesigned controls that hide standard behavior.
- Cramped grouping where unrelated elements appear connected.
- Excessive dividers used to compensate for weak layout.
- Cards used for data that should be compared in tables.
- Modals used for complex workflows.
- Hidden required information behind progressive disclosure.
- Disabled actions without explanation.
- Hover-only actions that are essential to the task.
- Error states that only use color.
- Form placeholders used as labels.
- Confirmation dialogs for harmless actions.
- Destructive actions placed next to primary positive actions without separation.
- Multiple primary buttons in the same task area.
- Inconsistent interaction states across similar components.
- Loading states that cause layout shifts.
- Empty states that explain nothing and offer no next step.
- Filters with hidden active criteria.
- Navigation labels based on internal architecture instead of user goals.
- Dense pages made smaller instead of better organized.
- Visual novelty that makes behavior less predictable.

## Final Behavioral Rules For The AI

When designing software UI, the AI must:

- Prioritize clarity over novelty.
- Start from the user’s task, not from visual decoration.
- Create clear focal points on every screen.
- Maintain strong visual hierarchy.
- Maintain consistent spacing rhythm.
- Use typography intentionally to guide reading order and scanning.
- Use contrast to support readability and priority.
- Reuse patterns once established.
- Keep interaction states complete and accessible.
- Make hover, focus, active, selected, disabled, loading, success, warning, error, empty, and validation states explicit.
- Justify layout choices through usability.
- Prefer familiar patterns unless there is a strong product reason to diverge.
- Keep primary actions visible and secondary actions available without competing.
- Separate destructive actions from routine actions.
- Use progressive disclosure to manage complexity without hiding required context.
- Choose tables, cards, modals, pages, tabs, accordions, sidebars, and top navigation based on task needs.
- Avoid arbitrary radius, shadow, spacing, color, and component changes.
- Avoid decorative elements that do not serve comprehension or action.
- Ensure layouts work across responsive breakpoints.
- Ensure controls are accessible by keyboard and readable by assistive technology.
- Preserve user input and provide recovery paths.
- Keep screens production-ready, systematic, and coherent.
- When a project-specific style guide exists, apply it on top of these fundamentals without violating usability, accessibility, hierarchy, or consistency.