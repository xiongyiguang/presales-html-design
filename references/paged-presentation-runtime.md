# Paged HTML Presentation Runtime

Use this contract for every default deliverable created by `presales-html-design`. The selected visual seed supplies the reference implementation.

## Output Model

- Deliver a single self-contained HTML presentation, not a continuously scrolling long page.
- Treat every direct child `<section>` of the deck container as one explicit presentation page.
- Show exactly one page at a time. Do not expose the top or bottom edge of an adjacent page at rest.
- Keep the document body from scrolling. Put controlled page navigation on the deck container.
- Keep CSS, interaction JavaScript, diagrams, and required SVG inline. Do not load a slide framework or any external runtime.

## Story and Page Planning

- Map each top-level source chapter to one or more pages before writing HTML.
- Give every page one message-style conclusion and only the evidence needed to support that conclusion.
- Split dense material into continuation pages instead of shrinking type, clipping content, or turning a page into a miniature report.
- Repeat the source-chapter label on continuation pages and mark the relationship clearly, for example `总体架构 · 2/2`.
- Keep page order meaningful. Use page numbers for real presentation order, not as decoration.
- A source chapter may share a page with another chapter only when both support the same conclusion and each remains visibly identifiable.

## Required Interaction

- Provide visible previous/next controls and a current-page/total-page indicator.
- Render the controls as a quiet utility: use a compact neutral surface, small low-contrast text and icons, minimal shadow, and no large dark control block. Reveal stronger contrast or the selected brand color only on hover and keyboard focus.
- Support `ArrowLeft`, `ArrowUp`, `PageUp`, `ArrowRight`, `ArrowDown`, `PageDown`, `Home`, `End`, and `Space` navigation.
- Support one-page-at-a-time mouse-wheel navigation with gesture throttling so one wheel gesture does not skip several pages.
- Support vertical touch swipe on mobile.
- Keep navigation anchors synchronized with page IDs and update the URL hash for the active page when possible.
- Do not intercept keys while the user is typing in an input, textarea, select, button, or editable region.

## Viewport and Overflow Rules

- Use `100dvh`/flex sizing so the header, page canvas, controls, and optional footer fit within the viewport.
- Compose desktop pages for presentation screens, normally around `16:9`, while allowing the canvas to fill other desktop ratios without distortion.
- Keep a safe content area on every page. Headings, diagrams, cards, and tables must not collide with controls or browser edges.
- At desktop verification widths, do not rely on internal page scrolling. Split the page when content does not fit.
- On narrow mobile screens, a page may use a controlled internal scroll region only when splitting would destroy the information relationship. Preserve the explicit page boundary and do not allow body-level continuous scrolling.
- Use `scroll-snap` as a resilient baseline, but include explicit controls and JavaScript navigation rather than relying on scroll snapping alone.

## Accessibility and Fallbacks

- Use semantic `<section>` pages with stable IDs and an accessible label or heading.
- Give controls visible keyboard focus and useful `aria-label` text.
- Expose the page counter through an `aria-live="polite"` region.
- Respect `prefers-reduced-motion`; page changes must become immediate rather than animated.
- Add print rules that expand all pages and apply `break-after: page` so the presentation can be printed or exported without clipped pages.

## Verification

Check the exact final file at minimum at `1440×900`, `1366×768`, and `390×844`:

- only one page is visible at rest;
- every page is reachable by controls, keyboard, wheel, touch, and direct hash navigation;
- no wheel gesture skips multiple pages;
- the current-page indicator is accurate;
- every navigation target exists;
- no desktop page clips or internally scrolls;
- mobile internal scrolling, if any, stays inside the active page;
- browser console has no errors or warnings;
- reduced-motion and print behavior work;
- the file has no external runtime dependency.
