# Executive Summary

Source note: the requested `input/` support files are not present in this checkout, so the extraction is based on the active app source: `app/globals.css`, `app/layout.tsx`, `components/finance/*`, and `components/ui/*`.

**EXPLICIT:** This repository expresses a soft, premium mobile-finance design language: warm cream backgrounds, deep forest green content, sharp lime highlights, large rounded geometry, compact information density, and subdued surface separation.

**EXPLICIT:** The strongest identity anchors are:
- Cream app canvas instead of pure white.
- Forest green as the dominant text, brand, navigation, and high-emphasis surface color.
- Lime as the signature action/accent color.
- Large rounded cards and controls, especially `rounded-2xl` and `rounded-3xl`.
- Compact finance-app typography with strong numeric emphasis.
- White cards on cream backgrounds with light borders or `shadow-sm`.
- Calm, quick transitions: `transition-colors`, `transition-all`, subtle scale on primary CTAs.

**INFERRED:** When adapted to a different product area, preserve the cream/forest/lime system, large soft radii, compact but friendly spacing, strong numeric hierarchy, and low-noise interaction feedback. Avoid turning it into a generic admin UI with gray slabs, square controls, dense divider grids, or blue SaaS defaults.

# Identity-Defining Traits

- **EXPLICIT:** The product identity is fintech, not neutral SaaS. It uses money-card gradients, account stats, transaction rows, privacy controls, and banking-style trust badges.
- **EXPLICIT:** The UI favors rounded physical objects: phone shell, cards, stat tiles, avatars, icon wells, nav items, CTA buttons, and chart bars are all rounded.
- **EXPLICIT:** Content feels compact but not cramped. Mobile screens use `px-4`, `space-y-4`, `p-3`, `p-4`; desktop views use `p-6`, `gap-4`, and 3-column grids.
- **EXPLICIT:** Visual emphasis is created through color contrast and weight, not heavy shadow or complex borders.
- **EXPLICIT:** The app uses real imagery only for onboarding/profile hero imagery; product surfaces are mostly tokenized UI shapes.
- **INFERRED:** New screens should feel like a wallet app: tactile, rounded, calm, financially precise, and optimistic without looking playful.

# Design Tokens

## Color Roles

| Role | Status | Value / Pattern | Usage |
|---|---:|---|---|
| App background | EXPLICIT | `--background: oklch(0.97 0.015 100)`, `--cream` | Main app canvas |
| Primary text | EXPLICIT | `--foreground: oklch(0.18 0.04 145)`, `--forest` | Headings, labels, nav, icons |
| Primary surface | EXPLICIT | `--card: oklch(1 0 0)` | Cards, lists, popovers |
| Primary action | EXPLICIT | `--primary`, `--forest`, hardcoded `#1B3A2D` | Main CTA, active nav, dark finance cards |
| Accent action | EXPLICIT | `--accent`, `--lime`, hardcoded `#C8E63A` | QR CTA, highlights, positive brand emphasis |
| Secondary background | EXPLICIT | `--secondary`, `--cream-dark` | Soft grouped rows, action tiles |
| Muted text | EXPLICIT | `--muted-foreground: oklch(0.52 0.03 145)` | Captions, metadata, support copy |
| Border | EXPLICIT | `--border: oklch(0.90 0.02 100)` | Card edges, top/bottom bars, controls |
| Ring/focus | EXPLICIT | `--ring: oklch(0.88 0.22 120)` | Focus ring, lime-aligned |
| Destructive | EXPLICIT | `--destructive`, red utilities | Sign out, negative transaction values |
| Chart colors | EXPLICIT | `--chart-1` lime, `--chart-2` forest, plus green range | Finance analytics |

Additional observed hardcoded palette:
- **EXPLICIT:** Lime card/accent: `#C8E63A`, darker lime `#b5d42a`.
- **EXPLICIT:** Forest card/text: `#1B3A2D`, secondary forest `#2d5c44`.
- **EXPLICIT:** Teal demo shell gradient: `#4a8fa8`, `#3d7a8a`, `#2d6070`.
- **EXPLICIT:** Positive/negative finance values use Tailwind greens and reds: `text-green-600`, `text-red-500`, `bg-red-50`, `text-green-500`.

## Background And Surface Behavior

- **EXPLICIT:** Main app screens use `bg-cream`; primary content cards use `bg-white`.
- **EXPLICIT:** Elevated summaries can invert to `bg-forest` with white/lime text or use `bg-lime` with forest text.
- **EXPLICIT:** Soft secondary group surfaces use `bg-cream-dark`, `bg-cream`, `bg-white/25`, `bg-white/30`, `bg-white/10`.
- **INFERRED:** For dashboards, use cream page background, white cards, forest/lime hero cards, and subtle tinted rows. Avoid large neutral gray backgrounds.

## Text Hierarchy

- **EXPLICIT:** Large financial values use `text-3xl` to `text-4xl`, `font-extrabold`, often `tracking-tight`.
- **EXPLICIT:** Desktop page titles use `text-2xl font-extrabold text-forest`.
- **EXPLICIT:** Mobile screen titles use `text-base` to `text-xl`, `font-bold`.
- **EXPLICIT:** Card section titles use `text-sm font-bold text-forest`.
- **EXPLICIT:** Metadata and captions use `text-[9px]`, `text-[10px]`, `text-xs`, `text-muted-foreground`, or reduced opacity.
- **INFERRED:** New product screens should keep titles short, use weight more than size, and reserve large type for balances, totals, and primary metrics.

## Border And Divider Treatment

- **EXPLICIT:** Borders are very light: `border-border`, `border-white/10`, `border-forest/20`, `border-white/8`.
- **EXPLICIT:** Borders often appear with white cards and controls, but major cards frequently rely on color or shadow instead.
- **EXPLICIT:** Dashed borders indicate add/new/empty actions.
- **INFERRED:** Dividers should be sparse. Prefer spacing and soft background changes over table-like grid lines.

## Radius System

- **EXPLICIT:** Active app token sets `--radius: 1rem`.
- **EXPLICIT:** Theme radii: `sm = 10px`, `md = 12px`, `lg = 16px`, `xl = 22px`.
- **EXPLICIT:** Implemented finance screens repeatedly use `rounded-xl`, `rounded-2xl`, `rounded-3xl`, `rounded-full`.
- **EXPLICIT:** Device shell uses very large custom radii: `42px`, `44px`, `46px`.
- **INFERRED:** Primary brand radius is `24px` for major cards and `16px` for controls. Sharp rectangles are off-brand except tiny decorative card-chip squares.

## Spacing System

- **EXPLICIT:** Mobile page padding: `px-4`, headers `px-5`, onboarding content `px-7`.
- **EXPLICIT:** Desktop page padding: `p-6`, onboarding panel `px-14 py-12`.
- **EXPLICIT:** Common gaps: `gap-1`, `gap-1.5`, `gap-2`, `gap-2.5`, `gap-3`, `gap-4`.
- **EXPLICIT:** Card padding: compact rows `p-2.5`/`p-3`, standard cards `p-4`/`p-5`, major desktop cards `p-6`.
- **INFERRED:** Utility-heavy layouts should use `gap-4` grids, `p-5` cards, `p-3` rows, and avoid bloating density beyond the existing finance-dashboard rhythm.

## Shadows And Elevation

- **EXPLICIT:** Most app cards use `shadow-sm`; nav QR uses `shadow-lg`; profile/stat rows sometimes use `hover:shadow-md`.
- **EXPLICIT:** Device/browser demo shells use strong external shadows, but those are presentation chrome, not app surfaces.
- **INFERRED:** App UI elevation should stay low. Use color, radius, and spacing before shadows.

## Typography

- **EXPLICIT:** Active app font is Plus Jakarta Sans via `next/font/google`.
- **EXPLICIT:** Weights loaded: `400`, `500`, `600`, `700`, `800`.
- **EXPLICIT:** UI primitives use `text-sm font-medium` defaults; finance screens lean `font-bold`, `font-extrabold`, `font-black` for brand/numbers.
- **EXPLICIT:** Body copy uses `leading-relaxed`; headings use `leading-tight`; labels often use compact `leading-none`.
- **INFERRED:** Use `400` for body, `500` for labels, `600` for rows/buttons, `700` for section titles, `800` for metrics and page titles, `900`-like `font-black` only for brand/card network text.

## Content Widths And Breakpoints

- **EXPLICIT:** Demo toolbar/browser frame caps at `max-w-5xl`.
- **EXPLICIT:** Desktop app content is fixed presentation height `640px`; sidebar width is `w-56`.
- **EXPLICIT:** UI sidebar primitive uses `16rem` desktop, `18rem` mobile, `3rem` icon collapsed width.
- **EXPLICIT:** Tailwind responsive classes appear through `md`, `sm`, and container queries in primitives.
- **INFERRED:** Real app pages should cap content around `max-w-5xl` to `max-w-6xl`, with 3-column desktop grids, 1-column mobile stacks, and sidebar at 224-256px.

# Geometry And Radius System

- **EXPLICIT:** The dominant shape language is rounded and pill-like.
- **EXPLICIT:** Major dashboard cards: `rounded-3xl`.
- **EXPLICIT:** Secondary cards, action tiles, nav items, feature pills: `rounded-2xl`.
- **EXPLICIT:** Small icon wells and controls: `rounded-xl`.
- **EXPLICIT:** Avatars, notification dots, chart bars, pagination dots: `rounded-full`.
- **EXPLICIT:** Generic shadcn primitives still define smaller `rounded-md` and `rounded-lg`, but the custom finance UI visually overrides them with larger radii.
- **INFERRED:** For new branded product UI, upgrade primitive defaults where visible:
  - Buttons: `rounded-2xl` for primary, `rounded-xl` for compact.
  - Inputs/selects: `rounded-xl` or `rounded-2xl`.
  - Cards/dialogs: `rounded-3xl`.
  - Badges: `rounded-lg` or pill.
- **INFERRED:** Sharp corners are only acceptable for tiny decorative details, chart ticks, table grid internals, or browser/device chrome. They should not define user-facing surfaces.

# Spacing Rhythm

- **EXPLICIT:** Overall density is balanced-compact. Mobile screens fit many financial actions without feeling cramped.
- **EXPLICIT:** Main mobile vertical rhythm uses `space-y-4`; transaction rows use `space-y-2` or `space-y-3`.
- **EXPLICIT:** Desktop dashboard grids use `gap-4`, not wide marketing spacing.
- **EXPLICIT:** Large onboarding uses more relaxed spacing: `mb-8`, `mb-10`, `mt-12`, `pt-8`.
- **EXPLICIT:** Controls pair icon and label with `gap-2` or `gap-2.5`; compact metadata uses `gap-0.5` to `gap-1.5`.
- **INFERRED:** Dashboard adaptation:
  - Keep page padding at `24px`.
  - Keep card grids at `16px` gap.
  - Use `20px` card padding for normal cards and `24px` for hero metric cards.
  - Use `12px` padding for list rows.
  - Use grouped controls in soft cream/white containers rather than adding many separate floating controls.

# Visual Priority And Hierarchy

- **EXPLICIT:** Focal points are established by:
  - Large numeric values.
  - Forest/lime color blocks.
  - Gradient payment cards.
  - Centered or top-aligned page headers.
  - Floating QR action in mobile nav.
- **EXPLICIT:** Primary content is separated from supporting content through color and weight, not heavy dividers.
- **EXPLICIT:** CTA hierarchy:
  - Primary: forest background with white text or lime background with forest text.
  - Secondary: muted text link or white/cream button with border.
  - Tertiary: icon-only, low opacity, hover color change.
- **EXPLICIT:** Metadata uses small text, muted color, opacity, and sometimes right alignment.
- **EXPLICIT:** The project uses subtle emphasis most of the time, with strong emphasis reserved for balances, primary cards, and active nav states.
- **INFERRED:** For admin screens, preserve hierarchy by making only one card/metric/action visually dominant per section. Do not make every tile equally saturated.

# Typography As UX

- **EXPLICIT:** Titles act as location markers: “Transactions”, “My Cards”, “Profile”.
- **EXPLICIT:** Large account values are the strongest scanning anchors.
- **EXPLICIT:** Section titles are short, bold, and small: “Quick Send”, “Recent Transactions”, “Actions”.
- **EXPLICIT:** Rows use a two-line pattern: primary label in forest/semibold, supporting date/category in muted small text.
- **EXPLICIT:** Captions and labels are intentionally tiny in financial cards: `text-[8px]` to `text-[10px]`.
- **EXPLICIT:** Transaction amounts are right-aligned, bold, and color-coded by sign.
- **INFERRED:** Form-heavy screens should use labels as primary scan anchors, helper text as muted secondary copy, and errors in destructive red. Avoid verbose explanatory copy inside controls.

# Layout System

- **EXPLICIT:** App shell supports mobile phone and desktop browser presentations.
- **EXPLICIT:** Mobile layout is vertical: status/header, scrollable content, bottom nav.
- **EXPLICIT:** Desktop layout is sidebar plus content.
- **EXPLICIT:** Desktop dashboard uses 3-column and 5-column grids:
  - 3-column dashboard with large balance card spanning 2 columns.
  - 5-column transactions layout with chart spanning 2 and list spanning 3.
- **EXPLICIT:** Cards and horizontal carousels use overflow scrolling with hidden scrollbars.
- **EXPLICIT:** Sidebar has logo header, nav group, user/balance card, and QR CTA footer.
- **EXPLICIT:** Headers place title/subtitle left and actions/avatar/filters right.
- **INFERRED:** New page layout recipe:
  - Cream canvas.
  - Header with title, short subtitle, and 1-2 actions.
  - 3-column responsive grid for summary cards.
  - White rounded content panels below.
  - Dense lists inside panels with hover cream rows.
  - Sidebar or bottom nav depending viewport.

# Interaction Model

- **EXPLICIT:** Hover feedback is restrained: `hover:bg-cream`, `hover:bg-cream-dark`, `hover:bg-white/20`, `hover:text-forest`.
- **EXPLICIT:** Primary CTA hover may scale slightly: `hover:scale-[1.02]`; active press uses `active:scale-[0.98]`.
- **EXPLICIT:** Screen transitions slide horizontally over `320ms cubic-bezier(0.4,0,0.2,1)`.
- **EXPLICIT:** Dots and toggles animate width/color with `duration-300`.
- **EXPLICIT:** Focus feedback in primitives uses `focus-visible:ring-ring/50 focus-visible:ring-[3px]`.
- **EXPLICIT:** Disabled primitives use `disabled:pointer-events-none disabled:opacity-50`.
- **EXPLICIT:** Selected nav states use forest fill + white text + lime dot, or active forest icon/text in bottom nav.
- **EXPLICIT:** Loading skeletons use `bg-accent animate-pulse rounded-md`.
- **EXPLICIT:** Validation uses destructive border/ring and text.
- **INFERRED:** Interaction feel is calm, crisp, premium, and touch-friendly. Avoid dramatic animations, neon glow, or noisy hover elevation.

# Explicit Component Patterns

## Buttons

- **EXPLICIT:** Generic primitive variants: default, destructive, outline, secondary, ghost, link.
- **EXPLICIT:** Primitive sizes: `h-8`, `h-9`, `h-10`, icon `size-8/9/10`.
- **EXPLICIT:** Finance primary buttons use larger radius: `rounded-2xl`, `py-4`, `font-semibold/bold`.
- **EXPLICIT:** Icon buttons often use `w-9 h-9` or `w-10 h-10`, white background, border, `shadow-sm`, rounded-full or rounded-2xl.
- **EXPLICIT:** CTA active state uses slight press scale.

## Navigation

- **EXPLICIT:** Mobile bottom nav uses white surface, top border, compact labels, active forest state.
- **EXPLICIT:** Central QR action floats above nav with lime fill, rounded-2xl, shadow-lg.
- **EXPLICIT:** Desktop sidebar active item uses forest fill, white text, and a small lime dot.
- **EXPLICIT:** Inactive sidebar items are muted and become cream/forest on hover.

## Cards

- **EXPLICIT:** Major finance cards use `rounded-3xl`, `p-5/p-6`, often no border.
- **EXPLICIT:** Standard white cards use `bg-white rounded-3xl shadow-sm`.
- **EXPLICIT:** List rows use `bg-white rounded-2xl p-3 shadow-sm` on mobile, or hoverable `p-2.5 rounded-2xl` rows inside desktop cards.
- **EXPLICIT:** Payment cards use diagonal gradients and high contrast typography.

## Transaction Rows

- **EXPLICIT:** Row structure: icon well/avatar, primary name, secondary date, right-aligned amount, category.
- **EXPLICIT:** Positive values green, negative values red.
- **EXPLICIT:** Merchant icons are circular or rounded-2xl colored blocks with initials.

## Charts

- **EXPLICIT:** Charts are simple bar charts with rounded bars, forest/lime colors, tiny muted labels.
- **EXPLICIT:** Chart cards include compact summaries and legends.
- **EXPLICIT:** Recharts primitive support exists with token-driven chart colors and tooltip/legend components.

## Profile And Settings Rows

- **EXPLICIT:** Profile uses avatar with lime ring, centered identity, stats card, then white menu rows.
- **EXPLICIT:** Settings rows use left icon well, title, subtitle, optional chevron.
- **EXPLICIT:** Danger items use red icon/text and omit the chevron in mobile profile.

## Onboarding

- **EXPLICIT:** Mobile onboarding uses full image hero plus bottom content panel.
- **EXPLICIT:** Desktop onboarding uses split image/content panel, feature pills, progress dots, trust badges.
- **EXPLICIT:** Onboarding CTA is prominent and rounded; skip is a muted text action.

## Forms And Inputs

- **EXPLICIT:** Generic input primitive exists: `h-9`, `rounded-md`, border, transparent background, focus ring.
- **EXPLICIT:** Form primitives provide labels, descriptions, messages, invalid state, and field grouping.
- **EXPLICIT:** These are not used heavily in finance screens, so their base look is generic shadcn rather than fully brand-adapted.

## Tables

- **EXPLICIT:** Table primitive exists with `text-sm`, row borders, hover `bg-muted/50`, selected `bg-muted`, `p-2` cells.
- **EXPLICIT:** No brand-specific finance table implementation appears; transactions are represented as cards/list rows instead.

## Dialogs, Sheets, Dropdowns, Selects, Tabs

- **EXPLICIT:** Radix/shadcn primitives exist.
- **EXPLICIT:** Dialogs use centered modal, black overlay, rounded-lg, border, `p-6`, `shadow-lg`.
- **EXPLICIT:** Sheets slide from screen edges with overlay and border.
- **EXPLICIT:** Dropdowns/selects use popover surfaces, `rounded-md`, border, shadow, compact item rows.
- **EXPLICIT:** Tabs use muted pill list with active background and shadow.

# Inferred Component Patterns

## Buttons

- **INFERRED:** Use lime fill with forest text for constructive primary actions in dashboards: “Add Card”, “Create Transfer”, “Apply Filter”.
- **INFERRED:** Use forest fill with white text for major flow progression or security-sensitive actions.
- **INFERRED:** Use cream/white ghost buttons for secondary actions, with hover `bg-cream` and text forest.
- **INFERRED:** Radius should be `16px`; compact toolbar buttons may use `12px`.

## Inputs

- **INFERRED:** Brand inputs should evolve from primitive defaults to `h-10` or `h-11`, `rounded-xl`, white background, light border, forest text, muted placeholder.
- **INFERRED:** Focus should use lime ring with forest border, not blue.
- **INFERRED:** Helper text should be `text-xs text-muted-foreground`; errors use destructive red and avoid aggressive alert styling.

## Selects And Dropdowns

- **INFERRED:** Use white popovers with `rounded-2xl` for larger menus and `rounded-xl` for compact filters.
- **INFERRED:** Selected items should use cream background and forest text; destructive items red.
- **INFERRED:** Filter selects can look like existing “Monthly” pills: white or translucent surface, rounded-full/2xl, compact text, chevron.

## Cards

- **INFERRED:** Dashboard cards should be either:
  - White `rounded-3xl p-5 shadow-sm`.
  - Forest hero `rounded-3xl p-6` with lime highlights.
  - Lime highlight `rounded-3xl p-5` with forest content.
- **INFERRED:** Use borders only when surfaces are similar in color; otherwise use shadow or background contrast.

## Tables

- **INFERRED:** Prefer card-contained tables over full-width grid tables.
- **INFERRED:** Header text should be `text-xs font-semibold text-muted-foreground`; row text `text-sm`.
- **INFERRED:** Rows should be `h-12` to `h-14`, hover cream, minimal horizontal dividers.
- **INFERRED:** Important cells such as amounts/status should use bold forest, green, red, or small rounded badges.

## Modals And Dialogs

- **INFERRED:** Brand dialogs should use `rounded-3xl`, `p-6`, white background, light border/shadow, black overlay at 40-50%.
- **INFERRED:** Titles should be `text-xl font-extrabold text-forest`; descriptions muted.
- **INFERRED:** Footer actions should include lime/forest primary and ghost secondary.

## Sidebars

- **INFERRED:** Use white sidebar on cream page, border-right, logo row, grouped nav, active forest pill with lime dot.
- **INFERRED:** Footer can contain a compact user/balance card and a lime action button.
- **INFERRED:** Avoid dark sidebars except for marketing/demo chrome.

## Tabs

- **INFERRED:** Use cream pill container with active white or forest segment.
- **INFERRED:** For high-level tabs, active state can be forest fill; for local filters, active can be white with shadow.

## Badges

- **INFERRED:** Finance/status badges should be compact, rounded-lg, `text-[9px]` to `text-xs`, semibold.
- **INFERRED:** Use semantic tints: green for income/verified, red for failed/danger, lime/forest for brand statuses, cream for neutral.

## Alerts

- **INFERRED:** Alerts should be calm and card-like: rounded-2xl, light border, icon well, short title, muted explanation.
- **INFERRED:** Destructive alerts should use red text and pale red background, not large saturated red blocks unless confirming irreversible financial action.

## Empty States

- **INFERRED:** Use dashed rounded-3xl containers, centered icon well, concise title, muted text, one primary action.
- **INFERRED:** Empty states should resemble “Add New Card”: dashed border, muted icon, soft hover.

## Chart Containers

- **INFERRED:** Charts should sit in white rounded-3xl cards or lime/forest summary cards.
- **INFERRED:** Bars should be rounded; legends tiny and muted; avoid dense axes.
- **INFERRED:** Use forest and lime as first chart colors, then controlled semantic colors.

## Page Headers

- **INFERRED:** Use title/subtitle left, actions right.
- **INFERRED:** Title: `text-2xl font-extrabold text-forest`.
- **INFERRED:** Subtitle: `text-sm text-muted-foreground`.
- **INFERRED:** Actions should be limited to 1 primary plus 1-2 compact secondary controls.

## Filters

- **INFERRED:** Filters should be compact chips/buttons, not full form panels by default.
- **INFERRED:** Use rounded-xl/2xl, white background, light border, muted label, forest selected state.
- **INFERRED:** Advanced filters can open a sheet/dialog rather than expanding a dense inline panel.

## Form Layouts

- **INFERRED:** Use one-column forms on mobile, two-column grouped forms on desktop.
- **INFERRED:** Group related fields inside white rounded-3xl cards with `gap-4` or `gap-6`.
- **INFERRED:** Use field descriptions sparingly. The style favors directness.

# UX Behavior Patterns

- **EXPLICIT:** Primary actions are visually isolated: floating QR button, lime “Add Card”, full-width onboarding CTA.
- **EXPLICIT:** Secondary actions are small text buttons or subdued icon controls.
- **EXPLICIT:** Information is grouped into digestible modules: balance, cards, actions, quick send, transactions.
- **EXPLICIT:** Dense data is represented as cards/lists, not spreadsheet grids.
- **EXPLICIT:** Progressive disclosure appears through “See all”, “Filter”, “Monthly”, balance visibility toggles, and onboarding skip.
- **INFERRED:** Utility-heavy screens should introduce controls in layers:
  - Page-level primary action in header.
  - Compact filters as chips.
  - Row-level actions hidden behind hover/menu icons.
  - Advanced controls in dialogs/sheets.
- **INFERRED:** Denser CRUD screens should still preserve the source language by using rounded cards, muted metadata, spacious row height, and brand-colored active states.

# Constraints And Anti-Drift Rules

- **EXPLICIT:** Do not replace the cream canvas with generic gray.
- **EXPLICIT:** Do not replace forest/lime with blue SaaS defaults.
- **EXPLICIT:** Do not make all cards white-on-white without contrast; use forest/lime hero surfaces for key metrics.
- **EXPLICIT:** Do not overuse heavy shadows; app surfaces mostly use `shadow-sm`.
- **EXPLICIT:** Do not make sharp rectangular cards or square buttons.
- **EXPLICIT:** Do not create dense divider-heavy admin tables as the default representation for financial data.
- **EXPLICIT:** Do not use large bodies of low-contrast text; the app uses short labels and strong hierarchy.
- **INFERRED:** New UI must preserve:
  - Cream page background.
  - Forest primary text/action.
  - Lime accent/CTA.
  - Large radii.
  - Compact finance-card density.
  - Subtle interaction feedback.
- **INFERRED:** Product context can flex:
  - More tables/forms are acceptable.
  - Slightly smaller radii are acceptable inside dense controls.
  - White cards can carry more structured data.
  - Sidebars and filters can become more utilitarian.
- **INFERRED:** To prevent generic dashboard drift:
  - Start every page with a branded metric or action surface.
  - Use rounded list rows instead of raw table rows where possible.
  - Keep semantic colors tied to financial meaning.
  - Make active/selected states forest or lime.
  - Keep copy short and task-oriented.

# Final Style DNA Summary

**EXPLICIT:** FinFlow’s style DNA is warm fintech minimalism: cream background, forest authority, lime optimism, soft tactile geometry, compact financial hierarchy, and quiet interaction feedback.

**INFERRED:** A consistent new screen should feel like this:

- Cream canvas.
- White rounded-3xl cards.
- One forest or lime focal surface per major section.
- Plus Jakarta Sans with bold, compact labels and extra-bold numbers.
- `16px` to `24px` radii as the default geometry.
- `16px` grid gaps and `20px` card padding.
- Muted metadata and high-contrast primary values.
- Subtle hover fills, lime focus rings, light shadows.
- Product controls introduced as chips, sheets, cards, and rounded rows rather than dense generic admin chrome.