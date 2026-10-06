# Paged HTML Presentation Runtime

Use this contract for every default deliverable created by `presales-html-design`. The selected visual seed supplies the reference implementation.

## Output Model

- Deliver a single self-contained HTML presentation, not a continuously scrolling long page.
- Treat every direct child `<section>` of the deck container as one explicit presentation page.
- Show exactly one page at a time. Do not expose the top or bottom edge of an adjacent page at rest.
- Keep the document body from scrolling. Put controlled page navigation on the deck container.
- Keep CSS, interaction JavaScript, diagrams, and required SVG inline. Do not load a slide framework or any external runtime.

## Persistent Presentation Chrome

- Reserve viewport space for a stable header and optional compact footer; keep them outside the scrolling deck so page changes do not move the chrome.
- Put every desktop presentation page inside one centered frame on a quiet stage. The direct child `<section>` remains the page boundary; its immediate content frame owns the border, shadow, safe-area padding, internal background, and overflow behavior.
- Generate one internal page-number element per section after the final slide list is known. Use two-digit `current / total` text, expose it as decorative when the accessible section label already announces the same count, and keep the current number visually distinct from the muted separator/total.
- Do not render a floating previous/next or numeric-page control. The page number inside the frame is the only visible numeric page indicator; keep a visually hidden live status for assistive technology. A thin non-interactive progress line may remain.
- Keep header brand text, navigation labels, footer metadata, and page-number placement stable across pages. Derive their visible text from the current source and selected brand; do not hard-code seed project labels.

## Story and Page Planning

- Map each top-level source chapter to one or more pages before writing HTML.
- Give every page one message-style conclusion and only the evidence needed to support that conclusion.
- Split dense material into continuation pages instead of shrinking type, clipping content, or turning a page into a miniature report.
- Repeat the source-chapter label on continuation pages and mark the relationship clearly, for example `总体架构 · 2/2`.
- Keep page order meaningful. Use page numbers for real presentation order, not as decoration.
- A source chapter may share a page with another chapter only when both support the same conclusion and each remains visibly identifiable.

## Required Interaction

- Provide a current-page/total-page indicator inside every page frame. Do not render any floating lower-right page control.
- Generate every internal page number and the hidden accessible page-status message from the same computed slide list; never maintain totals manually in page markup.
- Render header navigation as a quiet utility with legible labels and visible keyboard focus. Use the selected brand color for a meaningful active state, not a large dark control block.
- Support `ArrowLeft`, `ArrowUp`, `PageUp`, `ArrowRight`, `ArrowDown`, `PageDown`, `Home`, `End`, and `Space` navigation.
- Support one-page-at-a-time mouse-wheel navigation with gesture throttling so one wheel gesture does not skip several pages.
- Support vertical touch swipe on mobile.
- Keep navigation anchors synchronized with page IDs and update the URL hash for the active page when possible.
- Do not intercept keys while the user is typing in an input, textarea, select, button, or editable region.

## Viewport and Overflow Rules

- Use `100dvh`/flex sizing so the header, page canvas, progress line, and optional footer fit within the viewport.
- Compose desktop pages for presentation screens, normally around `16:9`, while allowing the canvas to fill other desktop ratios without distortion.
- Keep a safe content area on every page. Headings, diagrams, cards, and tables must not collide with controls or browser edges.
- At desktop verification widths, do not rely on internal page scrolling. Split the page when content does not fit.
- On narrow mobile screens, a page may use a controlled internal scroll region only when splitting would destroy the information relationship. Preserve the explicit page boundary and do not allow body-level continuous scrolling.
- Use `scroll-snap` as a resilient baseline, together with header navigation and JavaScript keyboard, wheel, touch, and hash navigation; do not rely on scroll snapping alone.

## Accessibility and Fallbacks

- Use semantic `<section>` pages with stable IDs and an accessible label or heading.
- Give header navigation anchors visible keyboard focus and useful labels.
- Expose the active page position through one visually hidden `aria-live="polite"` status region. Do not make the repeated page-number elements live regions.
- Respect `prefers-reduced-motion`; page changes must become immediate rather than animated.
- Add print rules that expand all pages and apply `break-after: page` so the presentation can be printed or exported without clipped pages.

## Verification

Check the exact final file at minimum at `1440×900`, `1366×768`, and `390×844`:

- only one page is visible at rest;
- every page is reachable by keyboard, wheel, touch, navigation anchors, and direct hash navigation;
- no wheel gesture skips multiple pages;
- the frame's current-page indicator is accurate and no floating page control appears;
- every page frame contains the correct two-digit internal page number, and the active position agrees with the hidden accessible status;
- every navigation target exists;
- no desktop page clips or internally scrolls;
- mobile internal scrolling, if any, stays inside the active page;
- browser console has no errors or warnings;
- reduced-motion and print behavior work;
- the file has no external runtime dependency.
