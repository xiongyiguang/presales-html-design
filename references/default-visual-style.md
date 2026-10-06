# Richinfo Executive Technical Brief

This is the shared visual-language and quality reference for daily presales paged HTML presentations. Use `visual-seed-selection.md` to choose the primary page structure and `paged-presentation-runtime.md` for interaction behavior. Keep the selected brand palette authoritative.

## 1. Positioning

Create an executive technical-exchange presentation: calm, structured, evidence-led, and easy to scan in a meeting. It should look like a designed digital proposal, not a marketing landing page, a converted Word document, a continuously scrolling article, or a dashboard.

The visual character is:

- white and light-gray foundations;
- restrained warm brand tints for scope, caution, and next-step areas;
- pale selected-brand thesis, value, and action bands for emphasis; do not use black, near-black, or charcoal for a large rectangular page, half-page frame, dominant card group, or wide emphasis band; deep neutral is primarily a text color and may be used only in compact local callouts and the footer;
- strong message-style headings, compact body copy, thin dividers, and limited shadow;
- varied structures selected by information relationship, not repeated card grids.

## 2. Default Tokens

Use these proportions unless the source or viewport requires adjustment:

| Token | Default |
|---|---|
| Desktop page ratio | compose near `16:9`, adapt to the available viewport without distortion |
| Content width | approximately `1200px` inside the page safe area |
| Desktop page gutter | `24px` or more on each side |
| Persistent header | `56–68px`; include it in viewport sizing |
| Page safe area | normally `40–64px` vertical and `24–48px` horizontal |
| Section heading layout | `180–210px` kicker column + flexible heading column |
| Body text | `16px` baseline |
| Supporting text | never below `14px` |
| Main title | `42–58px`, never above `60px` |
| Section heading | `31–43px` |
| Card heading | `20–24px` |
| Divider | cool gray, approximately `#E1E4E7` |
| Geometry | square or subtle radius; avoid pill-heavy consumer styling |

For Richinfo use:

- primary `#FF642A`;
- accent `#FFC000`;
- deep neutral around `#24282D` for text, rules, and small callouts rather than large backgrounds;
- light gray around `#F5F7F8`;
- warm orange tint around `#FFF2E9`;
- warm yellow tint around `#FFF9E8`.

Use the primary color for section labels, important headings, flow nodes, and high-priority chips. Use the accent for cautions, conditions, selected intelligent capabilities, and decision points. Do not fill large areas with both colors.

## 3. Default Slide Rhythm

Map the current source first. Use the following as a preferred rhythm, not a fixed chapter list:

1. **Cover page** — plain-text brand, project thesis and necessary metadata; select a conclusion, source-grounded mechanism, approved evidence, comparison, or true path opening according to the meeting task.
2. **Project understanding / customer concerns page** — message heading plus an operating storyline, shift map, or synthesized response lanes.
3. **Solution thesis / design principles page** — one pale primary-tint thesis block paired with a white principle grid.
4. **Overall architecture page or page sequence** — light-gray canvas containing the mandatory layered capability architecture; split into overview/detail pages when it cannot remain legible on one page.
5. **Core scenario page sequence** — one dominant scenario or a small group of true peers per page; continue on a second page when the evidence does not fit.
6. **Products or capability combination page** — compact role/capability/condition matrix.
7. **Industry observation pages** — evidence cards containing date, fact, customer impact, solution response, and source.
8. **Value and case pages** — an editorial evidence page on a pale brand tint, followed by clearly bounded case-evidence pages when needed.
9. **Implementation page** — staged roadmap; preserve the source's actual number of phases and split detailed deliverables into continuation pages.
10. **Next steps and confirmation page** — warm-tint canvas with an action strip and grouped decision themes, or two consecutive pages when exact owners and inputs require more room.
11. **References / closing page** — compact source list, plain-text brand, version, and confidentiality information.

Combine adjacent source chapters on one page when this improves the story, but retain a visible label or sub-block for every merged top-level chapter. If the source does not contain a listed relationship, omit that page structure rather than inventing content.

### Paged Canvas

- Show one page at a time inside the available viewport. Keep the header, progress line, and optional footer inside the viewport budget.
- Treat the viewport as persistent presentation chrome around a page canvas:
  - header: white, approximately `56–68px`, with the plain-text brand at left and compact chapter navigation at right;
  - stage: quiet cool gray around `#EEF1F3`, giving the page canvas a visible boundary without competing with content;
  - page canvas: one large centered white/light-gray/pale-brand frame, thin cool-gray border, restrained shadow, square or nearly square corners, and a consistent safe area;
  - page number: inside the canvas at the upper right, two-digit `current / total` formatting, current number in the selected primary color, separator and total in muted gray, tabular numerals, at least `14px`;
  - footer: compact deep-neutral band, plain-text brand at left, source-grounded project/document metadata at right, with white and cool-gray text.
- Keep the header brand treatment typographically direct. For Richinfo without an official logo, render `彩讯股份` or the source-provided Chinese brand name in deep neutral bold text and `Richinfo` in `#FF642A`; do not recolor the Chinese name orange or render `RICHINFO` in all caps unless the user/source requests it.
- Render navigation labels in deep neutral, bold enough for meeting projection, with low-contrast gray `/` separators. Use the current source's chapter names and valid anchors; do not inherit labels from a reference file.
- Keep the page frame dimensions and outer margins stable from page to page. Change only the frame's internal background/tint and content composition when the story requires it.
- On mobile, hide or compact the chapter navigation and footer when needed, reduce the outer stage margin, and retain the framed-page boundary plus internal page counter. Do not let the chrome consume the reading area.
- Give each page one dominant conclusion. A page is not a container for an entire chapter regardless of density.
- Prefer approximately three to six proof points, one diagram, one compact matrix, or one tightly related card group per page.
- Split before shrinking. At desktop sizes, never hide overflow, clip a table, or require internal scrolling to preserve a nominal page count.
- Use the page number inside the canvas as the only visible numeric page indicator. Keep it quiet but always visible; do not render a floating lower-right page control or previous/next arrows. A thin non-interactive progress line may remain as part of the paged runtime.
- Let page changes be crisp and restrained. Do not add 3D flips, parallax, or decorative transitions unless the user explicitly requests them.

## 4. Component Rules

### Header

- Use plain text for the company name when no official logo file is supplied.
- Keep navigation compact and place literal `/` or `·` separators between Chinese labels.
- Verify that every anchor target exists.
- Keep the Chinese brand name deep neutral and the English Richinfo wordmark in the selected primary color for the default Richinfo direction; use `14–16px`, heavy weight, and restrained letter spacing.

### Hero

- Use a two-column thesis-and-mechanism cover when a real governing mechanism benefits from visual explanation; stack it on mobile. Other openings are equally valid: a text-led conclusion, approved evidence, same-dimension comparison, or a true sequence. Select by meeting task and source, not seed appearance.
- State a clear source-grounded project thesis in the primary reading area.
- For a mechanism opening, use one source-grounded SVG loop, flow, or relationship diagram. Do not invent nodes or links to occupy an empty column.
- An engineering grid is optional for a mechanism diagram when it helps the technical reading. Keep title and outer padding plain; if used, confine the grid to the diagram viewport.
- Build the grid with two `1px` perpendicular cool-gray lines at roughly `6–9%` opacity. Use a cell size around `44–52px` on desktop and `32–40px` on mobile. The grid must remain quieter than diagram nodes, labels, paths, and borders.
- Keep SVG lines, arrows, nodes, and labels within a coherent visual area. Use a border only when it clarifies grouping; a frame is not required for every opening.
- Include project stage and scope boundaries when they affect interpretation.

#### Hero Heading Line Control

- Compose the desktop hero heading with intentional semantic breaks when needed; a short title can stay on one line. Determine the number of lines from wording, width, and page balance rather than a fixed two- or three-line rule.
- Avoid orphan lines containing only one to three Chinese characters or punctuation, especially a trailing word or punctuation fragment split from the preceding line.
- For chosen semantic breaks, use explicit line spans if needed. Avoid fixed nowrap rules that overflow at the verified widths; allow responsive wrapping while preserving meaning.
- When a line misses by only one or two characters, first reduce the heading size by approximately `3–8%` while keeping the desktop title within the normal `42–58px` range. If needed, make a small adjustment to the hero column ratio, inter-column gap, or negative letter spacing. Do not rewrite or delete source meaning merely to fit.
- Verify the real heading at `1366px` and `1440px` desktop widths, plus any user-specified target width. Count the rendered lines visually; do not treat the absence of horizontal overflow as proof that the title wrapping is good.

### Requirement Response

- Default to a dual-lane response, concern-to-outcome flow, grouped response themes, or operating storyline.
- Synthesize repetitive rows around a shared conclusion while preserving different commitments, impacts, owners, and confirmation conditions.
- Use a compact matrix only when the meeting requires exact cross-row comparison. If a table is necessary on mobile, keep it inside an internal horizontal scroll container; do not let the page itself overflow.

### Thesis and Principles

- Use a pale selected-brand tint for one strong statement and one supporting boundary or decision rule.
- Use the adjacent light grid for three to six principles.
- Avoid turning every principle into a large decorative card.

### Layered Architecture

- Use one bordered white container on a light-gray section.
- Each row has a layer label/role on the left and capability chips on the right.
- Use warm primary/accent tints for business-entry and intelligent-analysis capabilities.
- Keep integration, governance, and data/system chips neutral.
- Preserve every named source layer and decision-relevant capability.

### Scenario Layout

- Use an asymmetric grid only when one scenario is genuinely primary.
- A recommended desktop pattern is `7/5` for the first row and equal thirds for supporting scenarios.
- Include role, task, mechanism, and confirmation condition where the source provides them.
- On mobile, stack all scenarios in source order.

### Capability Combination

- Prefer a compact three-part row: role/priority, capability and purpose, inclusion condition.
- Distinguish core, foundation, pilot, combination, and future capabilities when the source makes that distinction.
- Never visually imply that an optional capability is committed scope.

### Industry Observations

- Use evidence cards with a visible date or status line.
- Each card must contain: specific fact, customer impact, solution response, and source.
- Do not use decorative trend cards containing only generic claims.

### Value and Cases

- Use an editorial evidence narrative, proof ladder, or pale-tint value strip when value proof is important.
- Use three or four concise value arguments with evidence-oriented wording; do not default to another equal card grid.
- Keep named cases in a separate bounded block and preserve disclosure cautions.
- Preserve exact case names in visible labels, captions, image `alt` text, and other accessibility metadata; do not substitute a descriptive or similar project name.

### Roadmap

- Use the source's exact stage names and actual number of stages.
- Each stage should show objective, work or deliverable, and acceptance/attention focus when available.
- Use restrained colored top rules rather than oversized step numbers.
- Keep the source's stages on one horizontal or stepped roadmap page when all objectives, deliverables, cooperation, and acceptance gates remain legible; split only for real density.

### Next Steps

- Use a warm-tint section to signal action and unresolved decisions.
- Separate recommended next actions from confirmation items.
- Keep confirmation items complete enough to support the next customer meeting.
- Use side-by-side columns only when the two blocks are semantic peers and their rendered heights are reasonably balanced. As a default check, a height difference greater than roughly `20–25%` indicates that the composition should be reconsidered.
- When the confirmation block contains a long list and the action block is much shorter, stack them vertically: place a compact full-width action strip first and the grouped confirmation themes below it. Use a matrix only when exact owner/input/status comparison is essential.
- Do not stretch a short card to imitate the height of a long table, and do not accept a large blank area below the shorter column as intentional whitespace.

## 5. Adaptation Rules

Always adapt the template to the current source:

- derive the opening form from the meeting task and supported thesis, mechanism, evidence, comparison, or sequence;
- derive page count and order from the source chapters and their content density;
- preserve the source's number of layers, scenarios, products, cases, and phases;
- let content density determine whether to use a table, cards, a flow, or a timeline;
- rewrite only generic display headings as message-style conclusions; keep any source heading containing a protected project, chapter, case, layer, scenario, phase, product, or organization name unchanged;
- keep every factual statement traceable to the provided source.
- inventory each page's relationship, form, and selection reason; repeat a form for comparable evidence or common tasks, and change it when information shape changes;
- keep white, light gray, and pale brand tints dominant. Do not use a dark half-page frame, dominant card group, or wide rectangular emphasis band merely to create contrast. Deep neutral fills should normally occupy no more than roughly one quarter of a page and should not become a full-page background unless the user explicitly requests a dark direction.

User-supplied visual references may override this layout rhythm. They may not override the selected brand palette, factual constraints, source coverage, accessibility, responsiveness, or self-contained delivery requirements.

## 6. Anti-patterns

Do not:

- copy the seed's visible sample text;
- force an eight-section or three-phase structure;
- use large gradients, glassmorphism, floating blobs, or consumer-style CTA sections by default;
- use a full-page, half-page, dominant card group, or wide rectangular emphasis area in black, near-black, or charcoal by default;
- reproduce source tables row-for-row when a storyline, flow, capability map, timeline, evidence narrative, or action strip preserves every distinct source row more clearly; retain the table when row identity, ownership, conditions, acceptance criteria, or confirmation status require exact comparison;
- repeat the same card grid for every chapter;
- use excessive rounded corners, shadows, badges, or decorative numbers;
- place generic AI trend slogans in the industry section;
- omit a source chapter to preserve the template's preferred page count;
- merge, rename, or summarize away a named case, source phase, layer, scenario, or confirmation item;
- force an entire dense chapter onto one page, clip content, or shrink text to avoid a continuation page;
- expose adjacent pages at rest or rely on free continuous body scrolling;
- shrink captions or SVG labels below `14px`;
- add a grid merely to resemble the seed, extend it across the whole hero, or make it compete with the diagram;
- leave an accidental one-to-three-character orphan line in the desktop hero heading or force semantic text into a preset line count;
- place a short summary card beside a materially taller table or list when the resulting empty lower column has no semantic purpose;
- use external fonts, images, scripts, CSS, or CDN dependencies.

## 7. Final Visual QA

Check the exact final HTML at `1440×900`, `1366×768`, and `390×844`:

- no page-level horizontal overflow;
- exactly one presentation page visible at rest, with no adjacent-page edge showing;
- stable white header, quiet gray stage, one bordered/shadowed page frame, internal two-digit page number, and compact deep-neutral footer at desktop widths;
- an accurate current-page/total-page number inside the frame and no floating lower-right page control;
- every page reachable by keyboard, wheel, touch, navigation anchors, and direct hash;
- no desktop page clipping or internal scroll; split dense pages instead;
- body baseline `16px`, every visible label at least `14px`, title at most `60px`;
- the selected opening communicates the source thesis; any mechanism diagram is source-grounded and contained;
- any engineering grid remains subtle, confined to a diagram viewport, and justified by the visual task;
- desktop hero heading has intentional wrapping at `1366px` and `1440px`, with no accidental orphan fragments or forced line count;
- side-by-side content blocks have comparable rendered heights; if one block is more than about `20–25%` taller, either justify the asymmetry through a deliberate sticky/supplementary role or convert the layout to stacked blocks;
- architecture rows readable and complete;
- navigation anchors valid and separators visible on desktop;
- pale brand-tint emphasis areas used intentionally, with any deep-neutral element kept compact;
- no full-page, half-page, dominant card group, or wide emphasis frame uses black, near-black, or charcoal by default; pale selected-brand tints carry emphasis, with deep neutral limited to compact elements unless explicitly requested;
- presentation forms and repetition match the actual information relationships; no minimum form count drives gratuitous modules;
- source chapters visibly covered;
- protected project, chapter, case, layer, scenario, phase, and confirmation wording matches the source in visible text and accessibility metadata;
- browser console free of errors and warnings;
- reduced-motion changes pages without animation, and print output expands one presentation page per printed page;
- no external runtime resources required.
