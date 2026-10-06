# 分页视觉与验收

仅按当前制作、图示或验收阶段读取对应小节；不加载其他风格种子。

### Brand Palette Lock

The user may specify one of the following brands:

1. 彩讯科技 / Richinfo
- primary: #FF642A
- accent: #FFC000

2. 中国移动
- primary: #1184CF
- accent: #8DC222

3. 中国银行
- primary: #BC260D
- accent: #D4AF37

If the user does not specify a brand, use 彩讯科技 / Richinfo by default.

Once a brand is selected, use the selected palette for primary accents, labels, buttons, diagrams, flow nodes, architecture highlights, and visual emphasis. Do not invent a new primary color direction.

Reference HTML files may influence layout, cards, labels, tables, spacing, and page rhythm, but must not override the selected brand palette.

### No Invented Logos

Do not create, invent, redraw, approximate, imitate, or synthesize any company logo.

If an official logo image file is provided, use that exact file.

If no official logo file is provided, use plain text only, such as:
- 彩讯科技 Richinfo
- 中国移动
- 中国银行

Do not add abstract marks, geometric symbols, initials, badges, seals, or colored blocks that could be mistaken for an official logo.

### Header Navigation

When a page contains three or more Chinese navigation labels, make each item visibly distinct at desktop width. Use a literal, visible text delimiter such as `·` or `/` between labels, or an equally legible rendered divider. Do not rely only on flex gap, whitespace, or low-contrast CSS pseudo-elements.

Use a presentation-page anchor for every navigation item and verify that its target ID exists. Keep navigation readable at the requested desktop width; hide or replace it with an appropriate mobile treatment only at smaller breakpoints.

### Presales Page Position

The output should feel like an executive-grade digital proposal presented one page at a time, not a literal Word-to-HTML report, a continuously scrolling article, or a consumer-style marketing landing page.

Preserve the solution logic from the provided content, but transform it into a web presentation with a strong hero thesis, structured sections, cards, labels, diagrams, architecture views, scenario blocks, lightweight tables, and clear visual rhythm.

In all delivery modes, cover every top-level source chapter. Combine adjacent chapters only when every protected term and unique source block remains intact, individually visible, and traceable; otherwise use adjacent continuation pages.

Do not invent unsupported customer names, project facts, statistics, commitments, certifications, cases, product functions, or commercial claims.

### Hero Illustration Boundary

The hero illustration must be visually self-contained.

All lines, curves, paths, nodes, arrows, SVG strokes, and decorative elements must stay inside the illustration container or a clearly controlled boundary.

Do not let hero illustration elements spill into the title, summary, navigation, action buttons, or lower information blocks.

If using flowing lines or data paths, they must terminate inside the frame, connect to visible nodes, or be clipped cleanly by the container.

### Structure Rules

Choose visual structures according to content relationships:

- parallel capabilities: card grid;
- staged implementation: timeline;
- business flow: process diagram;
- continuous improvement: closed-loop diagram;
- system relationship or explicit architecture chapter: layered capability architecture;
- requirement response: dual-lane storyline or concern-to-outcome flow by default; matrix only for irreducible cross-row comparison;
- before and after: side-by-side comparison;
- key metrics: metric cards;
- detailed lists: lightweight tables.

Do not make every section look like the same card grid. Do not use arrows, numbers, dividers, or labels unless they encode real information.

Avoid large-area black, near-black, or charcoal fills by default. Do not use a dark page, half-page frame, dominant card group, or wide rectangular emphasis band merely to create contrast. Use white, light gray, and pale brand tints for page and major-panel backgrounds. A deep neutral may appear in a compact callout, diagram node, or footer, but should normally occupy no more than roughly one quarter of the visible page. Use a full dark page only when the user explicitly requests it or the source provides a strong visual reason.
### Layered Capability Architecture (Mandatory)

When the source has a chapter such as `总体架构` / `总体架构说明`, or explicitly describes business, analysis, knowledge, governance, data, system, or other layers, render that chapter as a **layered capability architecture diagram**. Do not reduce it to a text-heavy table, a list of prose rows, generic cards, or one paragraph per layer.

At desktop width, use one bordered architecture container with repeated layer rows:

- left column: layer name plus one concise statement of its role;
- right column: one visible capability chip for each decision-relevant source item in that layer;
- rows: use dividers to communicate hierarchy; distinguish business-entry and intelligent-analysis chips with the selected brand primary/accent, and keep knowledge, governance, and data/system chips neutral but readable;
- preserve each source-provided layer and its named capabilities. Do not collapse a layer into a sentence when its individual capabilities are known;
- use responsive wrapping for chips and stack the label above the chips only at smaller breakpoints.

The architecture title should express the source's actual organizing thesis. The diagram must remain self-contained, legible, and based only on the source content.


### Final Check

Before finishing, check:
- when a source attachment was provided, every factual statement, case, data point, function, and commitment comes from that attachment;
- the protected-source register is complete, and every project, customer, organization, case, product, platform, system, module, technology, standard, certification, location, date, version, quantity, and amount visible in the output matches the source exactly;
- every protected name also matches the source in image `alt` text, `aria-label`, `title`, captions, navigation, and footer metadata;
- no case has been renamed, merged, split, reassigned, supplemented from another case, or given an invented customer, project name, scope, outcome, or evidence relationship;
- every content transformation preserves the source's meaning, attribution, scope, sequence, certainty, conditions, responsibilities, commitments, and conclusions;
- the internal traceability map links every protected term and unique decision-relevant source block to a visible output element, with omissions limited to items explicitly approved by the user;
- when a source attachment was provided, every top-level source chapter has one or more HTML presentation pages and is either an independent page or an identifiable sub-block on a combined page; every source H3 is represented within its parent chapter pages or documented as a compact sub-block;
- every source chapter has a clear takeaway plus sufficient source-backed evidence, without copied paragraphs or row-for-row table duplication by default;
- source tables have been deliberately recast for their information relationship, and repeated table styles are not used by default;
- the internal page map records each page's relationship, form, and reason; repeated forms support comparison or common tasks, and no minimum count forces artificial variety;
- all decision-shaping named products, modules, cases, industry observations, delivery items, customer responsibilities, acceptance concerns, and confirmation items are visibly represented in source-faithful executive-summary and full-coverage modes;
- each source chapter is recorded internally as `complete`, `synthesized`, or `user-approved omission` before delivery;
- visible copy states its intended conclusion directly; habitual “不是 A，而是 B” / “not A, but B” contrasts have been rewritten as direct affirmative statements, except for necessary source-grounded corrections or boundaries;
- the deliverable is one HTML file with inline CSS, inline interaction JavaScript, and no external dependency or network URL;
- exactly one presentation page is visible at rest, and every page is reachable through keyboard, wheel, touch, navigation anchors, and direct hashes;
- the internal page counter is accurate, no floating page control appears, one wheel gesture does not skip multiple pages, and `prefers-reduced-motion` removes animated transitions;
- no desktop page clips or internally scrolls at `1440×900` and `1366×768`; dense content is split into continuation pages instead of shrunk below the type limits;
- every visible text element is at least 14px, body text uses a 16px baseline, and the main title does not exceed 60px;
- at desktop widths, the hero title has intentional semantic wrapping with no accidental orphan fragment; short titles may remain on one line. Apply the smallest fitting correction and re-render without changing source meaning;
- selected brand palette is consistent;
- no invented logo or brand mark appears;
- hero illustration does not overflow;
- each desktop navigation label is visibly separated and every navigation anchor resolves to an existing presentation page;
- page does not look like Word converted to HTML;
- section layouts are not overly repetitive;
- no full-page, half-page, dominant card group, or wide emphasis frame uses black, near-black, or charcoal by default; major emphasis areas use pale selected-brand tints, with deep neutral limited to compact local elements unless explicitly requested;
- side-by-side blocks are semantic peers with reasonably balanced rendered heights; when one column is materially taller or contains a long table/list, stack the blocks vertically instead of leaving a large empty area under the shorter column;
- diagrams match the actual solution logic;
- when the source contains an explicit architecture chapter or layered architecture content, that chapter is rendered as a layered capability architecture diagram with visible layer labels and capability chips, not as prose rows or a text-only table;
- no unsupported content is invented;
- print rules expand every presentation page with a page break after it;
- no external network resources are required.

Verify the exact output file, not a draft or cached copy. If a rendered visual check is unavailable, complete structural checks and state that visual verification could not be completed; do not claim visual QA that did not occur.

## 设计复核证据

按 [design-review](design-review.md) 将设计计划与实际画面对照：先检查整体焦点和层次，再检查阅读尺寸、中文断行、装饰的信息作用与移动顺序。记录执行的文件、尺寸、问题和修正；未实际完成的视觉或交互项目标注为未验证。
