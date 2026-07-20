# Richinfo Executive Technical Brief

This is the shared visual-language and quality reference for daily presales paged HTML presentations. Use `visual-seed-selection.md` to choose the primary page structure and `paged-presentation-runtime.md` for interaction behavior. Keep the selected brand palette authoritative.

## 1. Positioning

Create an executive technical-exchange presentation: calm, structured, evidence-led, and easy to scan in a meeting. It should look like a designed digital proposal, not a marketing landing page, a converted Word document, a continuously scrolling article, or a dashboard.

The visual character is:

- white and light-gray foundations;
- restrained warm brand tints for scope, caution, and next-step areas;
- pale selected-brand thesis, value, and action bands for emphasis; deep neutral is primarily a text color and may be used only in compact local callouts;
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

1. **Cover page** — plain-text brand, project thesis, project metadata, and a self-contained inline SVG showing the source's central mechanism.
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

- Show one page at a time inside the available viewport. Keep the header, page controls, and footer inside the viewport budget.
- Give each page one dominant conclusion. A page is not a container for an entire chapter regardless of density.
- Prefer approximately three to six proof points, one diagram, one compact matrix, or one tightly related card group per page.
- Split before shrinking. At desktop sizes, never hide overflow, clip a table, or require internal scrolling to preserve a nominal page count.
- Keep the current-page indicator quiet but always visible. Previous/next buttons must remain discoverable and keyboard focusable.
- Let page changes be crisp and restrained. Do not add 3D flips, parallax, or decorative transitions unless the user explicitly requests them.

## 4. Component Rules

### Header

- Use plain text for the company name when no official logo file is supplied.
- Keep navigation compact and place literal `/` or `·` separators between Chinese labels.
- Verify that every anchor target exists.

### Hero

- Use a two-column layout on desktop and stack it on mobile.
- Make the left side a clear project thesis, not a generic slogan.
- Use the right side for one source-grounded SVG mechanism, loop, flow, or relationship diagram.
- Render the diagram region on a restrained light engineering-grid canvas by default. Keep the title strip and outer padding plain white; start the grid below the title divider and confine it to the diagram viewport.
- Build the grid with two `1px` perpendicular cool-gray lines at roughly `6–9%` opacity. Use a cell size around `44–52px` on desktop and `32–40px` on mobile. The grid must remain quieter than diagram nodes, labels, paths, and borders.
- Put all SVG lines, arrows, nodes, and labels inside a bordered visual container.
- Include project stage and scope boundaries when they affect interpretation.

#### Hero Heading Line Control

- Compose the desktop hero heading into two or three intentional semantic lines. Do not rely on uncontrolled browser wrapping for the final result.
- Avoid orphan lines containing only one to three Chinese characters or punctuation, especially a trailing word or punctuation fragment split from the preceding line.
- Prefer explicit block line spans after choosing the semantic breaks. Keep those spans `white-space: nowrap` at the verified desktop widths, and relax wrapping only at responsive breakpoints where the two-column hero has already stacked.
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

### Roadmap

- Use the source's actual number of stages.
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

- derive the hero diagram from the project's actual mechanism;
- derive page count and order from the source chapters and their content density;
- preserve the source's number of layers, scenarios, products, cases, and phases;
- let content density determine whether to use a table, cards, a flow, or a timeline;
- rewrite headings as message-style conclusions while retaining chapter purpose;
- keep every factual statement traceable to the provided source.
- inventory the presentation form selected for every page; for decks of six or more pages, normally use at least four distinct relationship-specific forms and avoid repeating one form on more than two consecutive pages.
- keep white, light gray, and pale brand tints dominant. Deep neutral fills should normally occupy no more than roughly one quarter of a page and should not become a full-page background unless the user explicitly requests a dark direction.

User-supplied visual references may override this layout rhythm. They may not override the selected brand palette, factual constraints, source coverage, accessibility, responsiveness, or self-contained delivery requirements.

## 6. Anti-patterns

Do not:

- copy the seed's visible sample text;
- force an eight-section or three-phase structure;
- use large gradients, glassmorphism, floating blobs, or consumer-style CTA sections by default;
- use a full-page or dominant near-black background by default;
- reproduce source tables row-for-row when a storyline, flow, capability map, timeline, evidence narrative, action strip, or grouped confirmation themes communicate the relationship more clearly;
- repeat the same card grid for every chapter;
- use excessive rounded corners, shadows, badges, or decorative numbers;
- place generic AI trend slogans in the industry section;
- omit a source chapter to preserve the template's preferred page count;
- force an entire dense chapter onto one page, clip content, or shrink text to avoid a continuation page;
- expose adjacent pages at rest or rely on free continuous body scrolling;
- shrink captions or SVG labels below `14px`;
- omit the default light grid from the hero diagram canvas, extend the grid across the whole hero, or use a dark/high-contrast grid that competes with the diagram;
- leave a one-to-three-character orphan line in the desktop hero heading, or accept an accidental fourth line when a small type or column adjustment would produce a deliberate two- or three-line composition;
- place a short summary card beside a materially taller table or list when the resulting empty lower column has no semantic purpose;
- use external fonts, images, scripts, CSS, or CDN dependencies.

## 7. Final Visual QA

Check the exact final HTML at `1440×900`, `1366×768`, and `390×844`:

- no page-level horizontal overflow;
- exactly one presentation page visible at rest, with no adjacent-page edge showing;
- visible previous/next controls and an accurate current-page/total-page indicator;
- every page reachable by keyboard, wheel, touch, navigation anchors, and direct hash;
- no desktop page clipping or internal scroll; split dense pages instead;
- body baseline `16px`, every visible label at least `14px`, title at most `60px`;
- hero diagram contained;
- hero diagram uses a subtle light grid inside the diagram viewport only, with nodes and labels clearly dominant;
- desktop hero heading uses two or three intentional lines at `1366px` and `1440px`, with no one-to-three-character orphan line;
- side-by-side content blocks have comparable rendered heights; if one block is more than about `20–25%` taller, either justify the asymmetry through a deliberate sticky/supplementary role or convert the layout to stacked blocks;
- architecture rows readable and complete;
- navigation anchors valid and separators visible on desktop;
- pale brand-tint emphasis areas used intentionally, with any deep-neutral element kept compact;
- no dominant near-black page or major panel appears by default; pale selected-brand tints carry emphasis, with deep neutral limited to compact elements unless explicitly requested;
- decks of six or more pages use at least four distinct relationship-specific presentation forms, with no single form repeated on more than two consecutive pages;
- source chapters visibly covered;
- browser console free of errors and warnings;
- reduced-motion changes pages without animation, and print output expands one presentation page per printed page;
- no external runtime resources required.
