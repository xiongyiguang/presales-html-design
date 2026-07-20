---
name: presales-html-design
description: Generate enterprise Chinese presales solution HTML presentations that show one full-screen page at a time, with brand-locked visual style, source-grounded content, keyboard/wheel/touch navigation, and a self-contained single-file runtime.
license: Complete terms in LICENSE.txt
---

# Presales HTML Design

Approach this as the design lead at a small studio known for giving every client a visual identity that could not be mistaken for anyone else's. This client has already rejected proposals that felt templated, and is paying for a distinctive point of view: make deliberate, opinionated choices about palette, typography, and layout that are specific to this brief, and take one real aesthetic risk you can justify.

## Ground it in the subject

If the brief does not pin down what the product or subject is, pin it yourself before designing: name one concrete subject, its audience, and the page's single job, and state your choice. If there's any information in your memory about the human's preferences, context about what they're building, or designs you've made before – use that as a hint. The subject's own world, its materials, instruments, artifacts, and vernacular, is where distinctive choices come from. Build with the brief's real content and subject matter throughout.

## Design principles

For web designs, the hero is a thesis. Open with the most characteristic thing in the subject's world, in whatever form makes sense for it: a headline, an image, an animation, a live demo, an interactive moment. Be deliberate with your choice: a big number with a small label, supporting stats, and a gradient accent is the template answer, only use if that's truly the best option.

Typography carries the personality of the page. Pair the display and body faces deliberately, not the same families you would reach for on any other project, and set a clear type scale with intentional weights, widths, and spacing. Make the type treatment itself a memorable part of the design, not a neutral delivery vehicle for the content.

Structure is information. Structural devices, numbering, eyebrows, dividers, labels, should encode something true about the content, not decorate it. Many generic designs use numbered markers (01 / 02 / 03), but that's only appropriate if the content actually is a sequence - like a real process or a typed timeline where order carries information the reader needs. Question if choices like numbered markers actually make sense before incorporating them.

Leverage motion deliberately. Think about where and if animation can serve the subject: a page-load sequence, a scroll-triggered reveal, hover micro-interactions, ambient atmosphere. An orchestrated moment usually lands harder than scattered effects; choose what the direction calls for. However, sometimes less is more, and extra animation contributes to the feeling that the design is AI-generated.

Match complexity to the vision. Maximalist directions need elaborate execution; minimal directions need precision in spacing, type, and detail. Elegance is executing the chosen vision well.

Consider written content carefully. Often a design brief may not contain real content, and it's up to you to come up with copy. Copy can make a design feel as templated as the design itself. See the below section on writing for more guidance.

## Process: brainstorm, explore, plan, critique, build, critique again

For calibration: AI-generated design right now clusters around three looks: (1) a warm cream background (near #F4F1EA) with a high-contrast serif display and a terracotta accent; (2) a near-black background with a single bright acid-green or vermilion accent; (3) a broadsheet-style layout with hairline rules, zero border-radius, and dense newspaper-like columns. All three are legitimate for some briefs, but they are defaults rather than choices, and they appear regardless of subject. Where the brief pins down a visual direction, follow it exactly — the brief's own words always win, including when it asks for one of these looks. Where it leaves an axis free, don't spend that freedom on one of these defaults. Just like a human designer who's hired, there's often a careful balance between doing what you're good at and taking each project as a chance to experiment and learn.

Work in two passes. First, brainstorm a short design plan based on the human's design brief: create a compact token system with color, type, layout, and signature. Color: describe the palette as 4–6 named hex values. Type: the typefaces for 2+ roles (a characterful display face that's used with restraint, a complementary body face, and a utility face for captions or data if needed). Layout: a layout concept, using one-sentence prose descriptions and ASCII wireframes to ideate and compare. Signature: the single unique element this page will be remembered by that embodies the brief in an appropriate way.

Then review that plan against the brief before building: if any part of it reads like the generic default you would produce for any similar page (work through a similar prompt to see if you arrive somewhere similar) rather than a choice made for this specific brief — revise that part, say what you changed and why. Only after you've confirmed the relative uniqueness of your design plan should you start to write the code, following the revised plan exactly and deriving every color and type decision from it.

When writing the code, be careful of structuring your CSS selector specificities. It's easy to generate CSS classes that cancel each other out (especially with a type-based selector like .section and a element-based selector like .cta). This can happen often with paddings/margins between sections.

Try to do a lot of this planning and iteration in your thinking, and only show ideas to the user when you have higher confidence it'll delight them.

## Restraint and self-critique

Spend your boldness in one place. Let the signature element be the one memorable thing, keep everything around it quiet and disciplined, and cut any decoration that does not serve the brief. Not taking a risk can be a risk itself! Build to a quality floor without announcing it: responsive down to mobile, visible keyboard focus, reduced motion respected. Critique your own work as you build, taking screenshots if your environment supports it – a picture is worth 1000 tokens. Consider Chanel's advice: before leaving the house, take a look in the mirror and remove one accessory. Human creators have memory and always try to do something new, so if you have a space to quickly jot down notes about what you've tried, it can help you in future passes.

## More on writing in design

Words appear in a design for one reason: to make it easier to understand, and therefore easier to use. They are design material, not decoration. Bring the same intentionality to copy that you would bring to spacing and color. Before writing anything, ask what the design needs to say, and how it can best be said to help the person navigate the experience.

Write from the end user's side of the screen. Name things by what people control and recognize, never by how the system is built. A person manages notifications, not webhook config. Describe what something does in plain terms rather than selling it. Being specific is always better than being clever.

Use active voice as default. A control should say exactly what happens when it's used: "Save changes," not "Submit." An action keeps the same name through the whole flow, so the button that says "Publish" produces a toast that says "Published." The vocabulary of an interface is the signposting for someone navigating the product. Cohesion and consistency are how people learn their way around.

Treat failure and emptiness as moments for direction, not mood. Explain what went wrong and how to fix it, in the interface's voice rather than a person's. Errors don't apologize, and they are never vague about what happened. An empty screen is an invitation to act.

Keep the register conversational and tuned: plain verbs, sentence case, no filler, with tone matched to the brand and the audience. Let each element do exactly one job. A label labels, an example demonstrates, and nothing quietly does double duty.

## Presales HTML Extension

When this skill is used to generate daily presales solution HTML presentations, keep the distinctive frontend design quality, but follow the constraints below.

### Default Visual Template

For daily presales paged HTML presentations, use the **Richinfo Executive Technical Brief** as the default visual system unless the user explicitly supplies or requests another visual direction.

Before planning or writing HTML:

1. Read `references/default-visual-style.md` completely.
2. Read `references/visual-seed-selection.md` completely and select one primary seed after mapping the source chapters.
3. Read `references/paged-presentation-runtime.md` completely and use its interaction, viewport, overflow, accessibility, and verification contract.
4. Use the selected seed only as visual, structural, and runtime calibration when code structure or component proportions are useful. Do not treat either seed as a copy-and-replace template.

Use **Richinfo Executive Technical Brief** (`references/richinfo-executive-seed.html`) by default. Select **Richinfo Linear Evidence Brief** (`references/richinfo-linear-evidence-seed.html`) when the source is long and evidence-heavy, with several independent chapters such as product combinations, industry observations, cases, implementation details, or confirmation matrices that deserve separate sections.

Choose one primary skeleton. Do not mechanically merge both seeds in the same page. Borrow at most one component pattern from the other seed when the source relationship clearly justifies it.

Apply this priority order:

1. The user's explicit visual instructions and supplied reference page.
2. The selected brand palette and all factual/source constraints in this skill.
3. `references/default-visual-style.md` as the default visual language and quality bar.
4. `references/visual-seed-selection.md` as the structural selection rule.
5. The selected sanitized seed file as optional implementation guidance.

The default style should normally include:

- a restrained white/light-gray/warm-tint section rhythm;
- a full-screen paged canvas that shows one explicit presentation page at a time;
- a two-column hero with a source-grounded inline SVG thesis diagram on a restrained light engineering-grid canvas;
- numbered section kickers aligned beside message-style headings;
- pale primary/accent-tint emphasis areas for requirement response, thesis, value, and next-step content; reserve deep neutral fills for text, rules, or a compact local callout rather than a full-page or half-page background;
- a layered capability architecture, response storyline, asymmetric scenario composition, capability map, staged roadmap, and warm final confirmation area when the source supports them;
- a maximum content width around 1200px, disciplined dividers, limited shadows, square or subtly rounded geometry, and high information density without visual crowding.

Do not force the seed's sample chapter count, number of scenarios, number of phases, wording, customer type, or business domain onto the source. Rebuild the chapter mapping from the current source every time. Never copy visible seed text into a deliverable. Never retain placeholders from the seed.

### Default Delivery Constraints

Apply these constraints by default. The user does not need to repeat them in each prompt.

- When a proposal, brief, or other source attachment is provided, treat it as the only factual source. Do not browse for, infer, or add external customers, cases, data, functions, commitments, certifications, or project facts unless the user explicitly authorizes it.
- Deliver one self-contained HTML file. Put all CSS in an inline `<style>` block and all interaction JavaScript in inline `<script>` blocks. Do not depend on external fonts, images, scripts, stylesheets, slide frameworks, CDNs, network URLs, or other local files. Use inline SVG only when needed for a diagram or illustration.
- Keep every visible text element at 14px or larger. Use 16px as the body-text baseline. Keep the main page title at 60px or smaller, and maintain a clear, proportionate type hierarchy.

### Paged Presentation Contract

- Use a deck container whose direct child `<section>` elements are explicit presentation pages. Show exactly one page at rest; do not deliver a continuous long page by default.
- Map every source chapter to one or more pages before writing HTML. Give each page one clear takeaway and split dense chapters into labeled continuation pages instead of shrinking or clipping content.
- Provide visible previous/next controls plus a current-page/total-page indicator. Support keyboard, one-page mouse-wheel, touch-swipe, navigation-anchor, and direct-hash access.
- Prevent one wheel gesture from skipping multiple pages. Respect `prefers-reduced-motion`, preserve keyboard focus, and do not intercept typing controls.
- Keep desktop pages free of internal scrolling at the verified presentation sizes. Allow controlled internal scrolling on narrow mobile pages only when the information relationship cannot be split cleanly.
- Include print rules that expand all pages and apply a page break after each page.
- Follow `references/paged-presentation-runtime.md` for the complete runtime and QA requirements. Use the selected seed's runtime as the implementation baseline instead of rewriting navigation behavior from scratch.

### Chapter Mapping and Synthesis

When a proposal, brief, or other source attachment is provided, use **executive-summary mode** by default. The goal is an executive-grade paged presentation: every source chapter is visibly covered, while logically adjacent chapters may be combined and their content distilled for presentation.

- Map every top-level source chapter to one or more HTML presentation pages. One page may combine multiple logically adjacent source chapters only when they support the same takeaway. Do not silently omit a top-level source chapter.
- In a combined section, retain a visible sub-heading, label, card group, or other identifiable content block for each merged source chapter. A chapter heading may be editorially rewritten, but it must retain the source chapter's purpose.
- Treat source H3 sections as compact sub-blocks, cards, steps, evidence, or continuation pages inside their parent chapter unless the user requests one independent page per H3.
- Before writing HTML, create an internal map with: `source chapter`, `page number / anchor`, `page thesis`, `presentation form`, and `coverage status`.
- For each source chapter, write one clear takeaway and select the smallest set of facts, examples, rows, or bullets that proves it. Prefer three to six concise points over copied paragraphs. Preserve decision-shaping facts, named products or modules, named cases, delivery items, customer responsibilities, acceptance concerns, and confirmation items.
- Treat source tables as source material, not as mandatory HTML tables. Extract their information relationship, then select a more suitable structure: a response matrix, comparison strip, card set, timeline, capability map, evidence list, or compact table. Do not reproduce a table row-for-row when grouping, short labels, or visual hierarchy communicate the same information more clearly.
- When table rows are repetitive, group them by their shared conclusion and retain the differentiating facts. Do not collapse rows that carry different commitments, owners, acceptance criteria, cases, products, or next actions.
- Preserve source-provided industry observations, competitive references, products, and cases as source-provided content. Do not add external comparison claims or facts.
- Use visual transformation to improve readability, not to create a Word-to-HTML copy. “Chapter coverage” requires a distinct page or identifiable sub-block; it does not require copied prose or a duplicate table layout.

Before creating separate pages, apply a **meeting-compression pass**:

- merge requirement-response material into one page when its rows share one operating conclusion; group the content into two or three storylines such as efficiency, governance, and evidence instead of reproducing every row;
- merge implementation stages into one roadmap page when objectives, deliverables, cooperation, and acceptance can remain legible at the verified desktop sizes;
- combine next actions and confirmation items when they support the same meeting decision, using a compact action strip plus grouped decision themes;
- split only when unique commitments, owners, acceptance conditions, evidence, or source density cannot remain legible. Never add pages merely because the source uses separate headings or tables.

Create a **presentation-form inventory** in the internal page map. For a deck of six or more pages, normally use at least four relationship-specific forms across the deck, for example: thesis diagram, operating storyline, dual-lane response, layered architecture, scenario loop, capability constellation, evidence narrative, timeline, action strip, or grouped confirmation themes. Do not use the same form on more than two consecutive pages. A table is a last-resort form for exact cross-reference, not the default representation of source tables.

### Delivery Modes

Select the delivery mode explicitly before drafting:

- **executive-summary mode (default):** cover every top-level source chapter in an independent or combined HTML section; distill each into its thesis and strongest supporting information;
- **full-coverage mode:** cover every top-level source chapter and retain all unique, decision-relevant factual details, while still redesigning prose and tables for the web;
- **presentation mode:** organize selected chapters around a meeting storyline. Obtain user approval before omitting a top-level source chapter.

All three content modes use the same paged HTML presentation runtime. The modes change content coverage, not whether the output is paginated.

Use appropriate web structures for each relationship:

- project metadata and thesis: hero / project brief;
- background and customer concerns: narrative, shift map, or operating storyline;
- requirement response: dual-lane response, concern-to-outcome flow, grouped response themes, or a compact matrix only when exact row comparison matters;
- products and modules: capability constellation, business-trunk-and-enablers map, role map, or compact capability matrix when inclusion conditions require exact comparison;
- industry observations and positioning: landscape or positioning section;
- values and highlights: editorial evidence narrative, proof ladder, value strip, or evidence list;
- named cases: case-reference table or case cards;
- implementation: phased roadmap including objectives, work, deliverables, customer cooperation, and acceptance focus;
- confirmation items: grouped decision themes, action strip plus confirmation groups, or a compact matrix only when owner/input/status comparison is essential.

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

In all delivery modes, cover every top-level source chapter. Combine adjacent chapters when doing so improves the storyline, and use identifiable sub-blocks plus synthesis to preserve their purpose, scanability, and visual rhythm.

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

Avoid large-area near-black or charcoal fills by default. Use white, light gray, and pale brand tints for page and major-panel backgrounds. A deep neutral may appear in a compact callout, diagram node, or footer, but should normally occupy no more than roughly one quarter of the visible page. Use a full dark page only when the user explicitly requests it or the source provides a strong visual reason.
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
- when a source attachment was provided, every top-level source chapter has one or more HTML presentation pages and is either an independent page or an identifiable sub-block on a combined page; every source H3 is represented within its parent chapter pages or documented as a compact sub-block;
- every source chapter has a clear takeaway plus sufficient source-backed evidence, without copied paragraphs or row-for-row table duplication by default;
- source tables have been deliberately recast for their information relationship, and repeated table styles are not used by default;
- the internal page map includes a presentation-form inventory; decks of six or more pages normally use at least four distinct relationship-specific forms and do not repeat one form on more than two consecutive pages;
- all decision-shaping named products, modules, cases, industry observations, delivery items, customer responsibilities, acceptance concerns, and confirmation items are visibly represented in executive-summary and full-coverage modes;
- each source chapter is recorded internally as `complete`, `synthesized`, or `user-approved omission` before delivery;
- the deliverable is one HTML file with inline CSS, inline interaction JavaScript, and no external dependency or network URL;
- exactly one presentation page is visible at rest, and every page is reachable through visible controls, keyboard, wheel, touch, navigation anchors, and direct hashes;
- the page counter is accurate, one wheel gesture does not skip multiple pages, and `prefers-reduced-motion` removes animated transitions;
- no desktop page clips or internally scrolls at `1440×900` and `1366×768`; dense content is split into continuation pages instead of shrunk below the type limits;
- every visible text element is at least 14px, body text uses a 16px baseline, and the main title does not exceed 60px;
- at desktop widths, the hero title uses two or three intentional semantic lines, with no accidental orphan line containing only one to three Chinese characters or punctuation; when a line misses by only one or two characters, apply the smallest fitting correction and re-render;
- selected brand palette is consistent;
- no invented logo or brand mark appears;
- hero illustration does not overflow;
- each desktop navigation label is visibly separated and every navigation anchor resolves to an existing presentation page;
- page does not look like Word converted to HTML;
- section layouts are not overly repetitive;
- no full-page or dominant near-black background is used by default; major emphasis areas use pale selected-brand tints, with deep neutral limited to compact local elements unless explicitly requested;
- side-by-side blocks are semantic peers with reasonably balanced rendered heights; when one column is materially taller or contains a long table/list, stack the blocks vertically instead of leaving a large empty area under the shorter column;
- diagrams match the actual solution logic;
- when the source contains an explicit architecture chapter or layered architecture content, that chapter is rendered as a layered capability architecture diagram with visible layer labels and capability chips, not as prose rows or a text-only table;
- no unsupported content is invented;
- print rules expand every presentation page with a page break after it;
- no external network resources are required.

Verify the exact output file, not a draft or cached copy. If a rendered visual check is unavailable, complete structural checks and state that visual verification could not be completed; do not claim visual QA that did not occur.
