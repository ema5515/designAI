**Executive Summary**
The repo expresses a dark, industrial, pixel-grid design language: black surfaces, hard rectangular geometry, high-contrast yellow accents, mono microcopy, and bold grotesk headlines. Evidence comes from global tokens in [globals.css](/Users/emanueledagata/code/v0/boh1/app/globals.css), section composition in [page.tsx](/Users/emanueledagata/code/v0/boh1/app/page.tsx), and repeated component patterns across [Hero.tsx](/Users/emanueledagata/code/v0/boh1/components/Hero.tsx), [Features.tsx](/Users/emanueledagata/code/v0/boh1/components/Features.tsx), [Pricing.tsx](/Users/emanueledagata/code/v0/boh1/components/Pricing.tsx), and [Comparison.tsx](/Users/emanueledagata/code/v0/boh1/components/Comparison.tsx).

The dominant identity is not soft SaaS polish. It is terminal/editor-inspired, precise, gridded, high-density but readable, with deliberate “builder tool” cues: brackets, slashes, uppercase labels, 4px/pixel references, scanlines, rulers, status bars, and token panels. When adapting this style to dashboards or admin screens, preserve square corners, dark layered surfaces, thin borders, yellow active states, mono labels, compact metadata, and strong section rhythm.

The requested support files under `input/` were not present in the repository, so this extraction is based on direct source inspection.

**Identity-Defining Traits**
- **EXPLICIT:** Dark-first system. Body and main surfaces use `#0A0A0A`, with sections alternating through `#050505`, `#060606`, `#080808`, `#0D0D0D`, `#0F0F0F`, and `#111111`.
- **EXPLICIT:** Primary brand color is saturated yellow `#FFD600`; it marks CTAs, active navigation, selected states, important borders, section labels, stat backgrounds, and featured pricing.
- **EXPLICIT:** Secondary accent is orange `#FF6B35`, used sparingly for alternative emphasis, AI/open states, and measurement-style accents.
- **EXPLICIT:** Geometry is mostly square. Buttons, cards, tables, badges, sections, pricing panels, carousel cards, and CTA blocks use no radius.
- **EXPLICIT:** Typography pairs Space Grotesk for bold titles and IBM Plex Mono for labels, metadata, descriptions, navigation, feature lists, and support text.
- **EXPLICIT:** Copy is uppercase, technical, clipped, and command-like.
- **EXPLICIT:** Borders, not shadows, define depth.
- **INFERRED:** The system should feel like a design/dev tool interface more than a conventional marketing site: grid-aware, segmented, inspectable, and precise.

**Design Tokens**
- **Colors, EXPLICIT:** `primary.yellow = #FFD600`; `accent.orange = #FF6B35`; `bg.primary = #0A0A0A`; `text.light = #F5F5F0`; `text.gray = #888888`; `text.muted = #555555`; `text.dim = #444444`; `border.dark = #2D2D2D`; `border.subtle = #1D1D1D`.
- **Additional surfaces, EXPLICIT:** `#050505`, `#060606`, `#080808`, `#0D0D0D`, `#0F0F0F`, `#111111`, `#141414`, `#161616`, `#1A1A1A`, `#1E1E1E`.
- **Additional text, EXPLICIT:** `#CCCCCC` for testimonial/table readable body, `#A0A09A` for included pricing features, `#666666` for paragraph text, `#333333` for disabled/placeholder marks.
- **Positive/support accents, EXPLICIT:** `#4ADE80` and `#60A5FA` appear inside the hero’s design-interface visualization, not as global UI primaries.
- **Background behavior, EXPLICIT:** Full-width horizontal bands alternate near-black values. Bright yellow is reserved for major contrast sections or selected cards, not general backgrounds.
- **Surface behavior, EXPLICIT:** Cards are flat panels with `#0A0A0A`, `#0F0F0F`, or `#111111`, separated by 1-2px borders and 2px gutters.
- **Border treatment, EXPLICIT:** Common borders are `1px solid #2D2D2D`, `2px solid #FFD600` for highlighted items, `2px solid #3D3D3D` for secondary controls, and `1px solid #1D1D1D` for dividers.
- **Radius, EXPLICIT:** Default radius is `0`. Rare exceptions: circular avatar placeholders, mobile active dots, and small SVG mockup `rx=1/2`.
- **Spacing, EXPLICIT:** Mobile section padding commonly `px-6 py-16`; desktop commonly `md:px-[120px] md:py-[100px]`; footer uses `64px`; final CTA uses `120px`.
- **Internal spacing, EXPLICIT:** Cards use `p-8`, `md:p-[32px]`, or `md:p-[40px]`; card gaps are usually `gap-4`, `gap-5`, `gap-6`, `gap-8`.
- **Grid seams, EXPLICIT:** Repeated card groups use `gap-[2px]`, creating pixel-like gutters.
- **Typography, EXPLICIT:** Fonts are Space Grotesk weights `400/500/700` and IBM Plex Mono weights `400/500/700`.
- **Type scale, EXPLICIT:** Hero `clamp(32px,10vw,96px)`; final CTA `44/80`; section title `36/56`; card titles `18`, `20`, `24/28`; stats `40/64`; body/support `10-15`; labels `9-12`.
- **Line height, EXPLICIT:** Headlines use `leading-none`, `1.05`, `1.1`, `1.2`; body text uses `1.5-1.6`.
- **Letter spacing, EXPLICIT:** Labels and CTAs use strong tracking, commonly `1px`, `1.5px`, `2px`, `3px`; large titles use `-1px` or `-2px`.
- **Content widths, EXPLICIT:** Navbar max width `1400px`; hero content `1100px`, subtitle `800px`; section title defaults `700px`, subtitle `600px`; final CTA title `1000px`.
- **Breakpoints, EXPLICIT:** Tailwind `sm` and `md` are used. `md` drives desktop layout, navigation, section padding, card rows, and table display.

**Geometry and Radius System**
- **EXPLICIT:** The dominant radius family is square: `0px`.
- **EXPLICIT:** Brand blocks, CTAs, pricing panels, bento cards, feature cards, table cells, FAQ toggles, carousel cards, and badges are rectangular.
- **EXPLICIT:** Circular geometry is reserved for semantic small objects: avatars, nav active dots, cursor labels/indicators, and SVG status dots.
- **INFERRED:** New product UI should use `0px` radius for containers and primary controls. Use `2px` only for tiny embedded editor/tool glyphs or code-preview affordances. Use `999px` only for avatars, presence dots, status LEDs, and chart points.
- **INFERRED:** Soft 12-24px cards, pill buttons, glassmorphism blobs, and rounded SaaS panels are off-brand.

**Spacing Rhythm**
- **EXPLICIT:** Overall density is balanced-to-spacious at the page level and compact within components.
- **EXPLICIT:** Large sections breathe with `64-100px` vertical padding and `48-64px` header-to-content gaps.
- **EXPLICIT:** Card internals are structured but not airy: `32-40px` padding, `16-24px` vertical gaps, and compact label strips.
- **EXPLICIT:** Multi-card rows use `2px` gutters, making grouped cards feel like one segmented interface.
- **EXPLICIT:** Controls cluster tightly: CTA pairs use `16px` gaps; nav links use `36px`; carousel arrows use `8px`.
- **INFERRED:** In dashboards, keep page padding slightly tighter than marketing: `24px` mobile, `32-48px` desktop shell padding, `24-32px` between dense regions, and `2px` or `1px` seams inside grouped data modules.
- **INFERRED:** Do not turn every widget into an isolated floating card. Prefer segmented panels with shared borders and narrow gutters.

**Visual Priority and Hierarchy**
- **EXPLICIT:** Focal points are established through scale, yellow contrast, and hard-edged framing.
- **EXPLICIT:** Primary content uses Space Grotesk, bold weight, light/yellow color, short uppercase phrases, and tight line height.
- **EXPLICIT:** Supporting content uses IBM Plex Mono, smaller sizes, muted gray, increased tracking, and `1.5-1.6` line height.
- **EXPLICIT:** CTA hierarchy is clear: primary is yellow fill with black text; secondary is black fill with gray/yellow border treatment.
- **EXPLICIT:** Active and selected states use yellow text, yellow border, yellow fill, or a yellow side rail/underline.
- **INFERRED:** Utility screens should establish priority through border weight, surface tone, and yellow state markers before adding decoration.
- **INFERRED:** Use strong emphasis sparingly. The system is high-contrast, but not visually noisy when yellow is rationed.

**Typography as UX**
- **EXPLICIT:** Hero titles are oversized Space Grotesk, bold, uppercase, tight leading, often split across lines.
- **EXPLICIT:** Section headers use a mono eyebrow label like `[01] // FEATURES`, then a bold grotesk title, then optional mono support text.
- **EXPLICIT:** Cards use grotesk titles and mono descriptions, preserving a clear title/body distinction.
- **EXPLICIT:** Metadata uses IBM Plex Mono at `9-12px`, uppercase, wide tracking, bracket/slash syntax.
- **EXPLICIT:** Tables use mono body cells and compact grotesk headers.
- **INFERRED:** Forms and dashboards should keep labels mono and small, values/data mono where precision matters, and primary object names in bold grotesk.
- **INFERRED:** Sentence case would dilute the identity unless the product context demands longer prose; labels, nav, metrics, and controls should remain uppercase.

**Layout System**
- **EXPLICIT:** The page is a vertical stack of full-width sections.
- **EXPLICIT:** Desktop section padding is usually `120px` horizontal; mobile uses `24px`.
- **EXPLICIT:** Section headers precede content blocks, often aligned left; hero and final CTA center their content.
- **EXPLICIT:** Reusable composition is `SectionHeader -> 48/64px gap -> segmented content`.
- **EXPLICIT:** Card rows switch from stacked mobile to horizontal `md:flex-row`.
- **EXPLICIT:** Comparison uses desktop table and a separate mobile card/grid layout.
- **EXPLICIT:** Navbar is fixed at `60px`, transparent initially, then dark translucent with blur and bottom border after scroll.
- **INFERRED:** Product shells should use a fixed top bar or left rail with hard borders. Content should live in full-width panels or segmented grids, not rounded floating islands.
- **INFERRED:** Use 12-column or equal-flex grid logic; the hero visualization explicitly references `GRID: 12 COL`.

**Interaction Model**
- **EXPLICIT:** Hover feedback is simple and crisp: color change, border color change, underline, or small scale on the logo square.
- **EXPLICIT:** Transitions are short: `150-300ms` for nav/hover/drawer, `500ms ease-in-out` for carousel movement.
- **EXPLICIT:** Active navigation uses yellow text and a yellow underline; mobile active nav uses a yellow dot.
- **EXPLICIT:** FAQ selected state turns the toggle square yellow and swaps `+` to `—`.
- **EXPLICIT:** Carousel selected state uses a yellow wider progress segment; inactive dots are gray.
- **EXPLICIT:** Loading/animated behavior uses typewriter/glitch text, blinking cursors, scanlines, pulsing status dots, and moving collaboration cursors.
- **EXPLICIT GAP:** No explicit focus-visible, disabled button, validation, toast, or loading skeleton patterns are implemented.
- **INFERRED:** Focus should be a 2px yellow outline or inset border, square, with no glow except perhaps a very restrained dark shadow for accessibility.
- **INFERRED:** Disabled states should use `#333333/#444444` text, `#1D1D1D` borders, and no yellow.
- **INFERRED:** Validation should be direct and technical: orange for warning/error-adjacent states, yellow for required attention, green only for success/status.

**Explicit Component Patterns**
- **Navbar, EXPLICIT:** Fixed 60px shell, max width `1400px`, transparent-to-blurred black on scroll, mono uppercase links, yellow active underline, square yellow brand mark, square yellow CTA.
- **Hero, EXPLICIT:** Centered content, oversized two-tone headline, mono subheading, paired CTAs, metadata line, and a large bordered editor/design-interface visual.
- **SectionHeader, EXPLICIT:** Mono yellow eyebrow, bold grotesk multiline title, optional muted mono subtitle; default title width `700px`, subtitle width `600px`.
- **Feature/Step/Bento cards, EXPLICIT:** Square panels, `32-40px` padding, `1-2px` borders, `2px` group seams, bold grotesk titles, mono descriptions, small square icon/color blocks.
- **Badges/tags, EXPLICIT:** Rectangular `24-32px` tall, mono uppercase, often bracketed, background `#1A1A1A` or yellow, border matching accent.
- **Stats, EXPLICIT:** Full yellow band, black text, large grotesk numerals, mono labels, hard black dividers.
- **Testimonials, EXPLICIT:** Flat dark panels with a `4px` left accent border, mono quote, small circular avatar placeholder.
- **Comparison table, EXPLICIT:** Dark bordered table, 56px rows, fixed first column, yellow bottom border under header, highlighted PixelCraft column.
- **FAQ, EXPLICIT:** Border-top list rows, 72px desktop trigger height, square 32px toggle, open state uses yellow fill.
- **Pricing, EXPLICIT:** Three square pricing panels, popular tier has yellow border/fill accents, feature list uses `+` and `—`, CTA fills follow tier priority.
- **Footer, EXPLICIT:** Dark segmented footer, square social buttons, mono links, subtle top divider, yellow version stamp.

**Inferred Component Patterns**
- **Buttons, INFERRED:** Primary: yellow fill, black bold grotesk or mono label, 48-64px height, square. Secondary: black/dark fill, 2px gray border, muted mono label, hover border `#888888`. Destructive/urgent: orange border or fill used sparingly.
- **Inputs, INFERRED:** Square dark field `#0F0F0F`/`#111111`, 1px `#2D2D2D` border, 44-48px height, mono 12-13px text, yellow 2px focus border, placeholder `#444444`, error border orange.
- **Selects, INFERRED:** Same as inputs, with square right affordance, mono uppercase selected value, yellow border on open.
- **Dropdowns, INFERRED:** Dark rectangular panel, 1px border, no shadow or minimal black drop shadow, 2px item separators, active item `#1E1E1E` with yellow left rail.
- **Cards, INFERRED:** Use square panels with `1px #2D2D2D` borders, `24-32px` utility padding, `32-40px` marketing padding, no radius, no floating shadow.
- **Tables, INFERRED:** 48-56px rows, mono data, grotesk uppercase headers, subtle row dividers `#1D1D1D`, selected column/row via darker fill plus yellow rail/border.
- **Modals/dialogs, INFERRED:** Centered square panel on `rgba(10,10,10,.88)` overlay, `2px #FFD600` border for critical dialogs or `1px #2D2D2D` default, header with mono eyebrow and grotesk title.
- **Sidebars, INFERRED:** `240-280px` dark rail, right border `#2D2D2D`, mono nav labels, active yellow text plus 2px left rail.
- **Tabs, INFERRED:** Rectangular segmented tabs with 1px borders; active tab yellow text or yellow top/bottom border; no pill tabs.
- **Badges, INFERRED:** 24-28px high, square, mono 9-11px, bracketed labels encouraged.
- **Alerts, INFERRED:** Flat bordered bands. Info uses yellow border, warning uses orange, success uses green only as status accent. Copy should be concise and technical.
- **Empty states, INFERRED:** Use a bordered dark panel, mono status label, bold grotesk headline, one primary yellow action, optional ASCII/bracket motif.
- **Chart containers, INFERRED:** Dark square panels with subtle grid lines, mono axes/legends, yellow primary series, orange secondary series, low-saturation gray comparison series.
- **Page headers, INFERRED:** Mono eyebrow or breadcrumb, bold grotesk title, muted mono description, actions aligned right on desktop.
- **Filters, INFERRED:** Compact toolbar with square fields/buttons, 2px seams, mono labels, selected filters as yellow-bordered tags.
- **Form layouts, INFERRED:** Stacked groups with 16-20px field gaps, 32px section gaps, mono labels above fields, inline validation below in mono 11-12px.

**UX Behavior Patterns**
- **EXPLICIT:** Actions are prioritized by fill strength: yellow fill first, bordered dark second, muted text/link tertiary.
- **EXPLICIT:** Secondary actions are present but visually restrained through gray text, border-only buttons, and hover-only emphasis.
- **EXPLICIT:** Information is grouped into hard-edged sections, card rows, segmented bento grids, and bordered table/list rows.
- **EXPLICIT:** The UI introduces complexity through progressive sections, not dense simultaneous controls.
- **INFERRED:** Dense product screens should preserve the language by using segmented panels, mono metadata, yellow active markers, and strong headers, while reducing marketing-scale type.
- **INFERRED:** Avoid overwhelming dashboards by limiting yellow to active states, primary actions, key metrics, and one selected module per region.

**Constraints and Anti-Drift Rules**
- **EXPLICIT:** Do not introduce light-mode surfaces as defaults; this is dark-first.
- **EXPLICIT:** Do not replace square geometry with rounded SaaS cards or pills.
- **EXPLICIT:** Do not rely on shadows for hierarchy; use borders, seams, contrast, and surface steps.
- **EXPLICIT:** Preserve Space Grotesk plus IBM Plex Mono.
- **EXPLICIT:** Preserve uppercase technical labeling, bracket/slash motifs, and compact metadata.
- **INFERRED:** Avoid gradients, glassmorphism, pastel palettes, soft illustrations, large rounded cards, drop-shadow-heavy elevation, and generic dashboard templates.
- **INFERRED:** Product-context flexibility is allowed in density, table complexity, form controls, and sidebar usage, but not in the core anchors: black surfaces, yellow active/primary states, hard borders, square geometry, mono labels, and grid-like spacing.
- **INFERRED:** To keep CRUD/admin screens on-brand, make them feel like an inspectable control system: bordered regions, precise labels, clear active rails, restrained color, and measured spacing.

**Final Style DNA Summary**
Dark industrial interface language. Square by default. Yellow is the primary signal. Orange is a restrained secondary accent. Borders and 2px seams create structure. Space Grotesk carries command-level hierarchy; IBM Plex Mono carries labels, data, metadata, and body support. Layouts are full-width, gridded, and segmented. Interactions are crisp, minimal, and state-driven. New UI should feel like a production-grade design/dev console, not a generic rounded SaaS dashboard.