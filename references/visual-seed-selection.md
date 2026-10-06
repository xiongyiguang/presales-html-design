# Visual Seed Selection

Select one primary seed only after mapping every top-level source chapter to presentation pages. The seeds are paged structural and runtime references, not fill-in-the-blank templates. Brand, factual boundaries, source coverage, accessibility, and responsive behavior always remain authoritative.

## Available Seeds

| Seed | Status | Best fit | Structural character |
|---|---|---|---|
| `richinfo-executive-seed.html` | Default | Executive technical exchange, concise solution narrative, limited major chapters, one clear thesis | Short paged deck, strong cover mechanism, synthesized response lanes, pale-tint thesis, layered architecture, asymmetric scenarios, editorial value evidence, concise roadmap and grouped next steps |
| `richinfo-linear-evidence-seed.html` | Optional | Long or evidence-heavy proposal with independent products, industry observations, cases, detailed implementation, or many decision points | Longer evidence deck, quiet gray/white/pale-brand rhythm, independent evidence pages, varied relationship-specific forms, detailed roadmap and grouped confirmation themes |

## Selection Heuristic

Use **Executive Technical Brief** unless the source strongly benefits from a longer evidence-page sequence.

Choose **Linear Evidence Brief** when at least two of the following are true:

- the source has eight or more decision-relevant top-level chapters;
- products or capability combinations need a dedicated section rather than a compact matrix;
- industry observations contain multiple concrete facts that need room for date, impact, response, and source;
- customer or project cases need a dedicated evidence chapter;
- implementation phases require work items, deliverables, customer cooperation, and acceptance criteria;
- the final section requires detailed confirmation responsibilities, inputs, or decision status that may need a dedicated page.

Do not select the linear seed merely because the Markdown file is long. Select it because the information relationships deserve independent presentation pages.

## Adaptation Rules

- Rebuild the page sequence and navigation from the current source. Do not force a fixed page count.
- Split any page whose content does not fit at the verified desktop sizes. Label continuation pages and keep them adjacent.
- Preserve the source's actual number of layers, scenarios, products, cases, phases, and confirmation items.
- Never copy visible sample wording, placeholder text, customer type, business domain, or numerical values from a seed.
- Reuse the selected seed's runtime and component grammar while rebuilding its page compositions around the source. Borrow another seed's component only when it fits the relationship and remains consistent with the selected brand and shell.
- Run a meeting-compression pass before deciding page count. Shared requirement-response conclusions, implementation phases, and next-step decisions should normally be synthesized onto one page when legible.
- Record each page's primary relationship, presentation form, and selection reason. Forms have no minimum count; comparable evidence or repeated tasks may use the same form across consecutive pages.
- Treat tables as optional exact-comparison tools, not seed defaults. Prefer response lanes, storylines, scenario loops, capability maps, evidence narratives, timelines, action strips, and grouped decision themes.
- Keep page and major-panel backgrounds white, light gray, or pale selected-brand tints. Do not copy a dominant near-black page from any reference; deep neutral is limited to compact local elements unless the user explicitly requests otherwise.
- If the user supplies a reference page or explicitly names a seed, follow that direction unless it conflicts with factual, brand, accessibility, or delivery constraints.

## Prompt Overrides

Users may select a seed explicitly with language such as:

- `视觉种子 = Executive Technical Brief`
- `视觉种子 = Linear Evidence Brief`
- `参考第一套，偏管理层技术交流`
- `参考第二套，偏章节化证据翻页演示`

When no selection is provided, make the choice silently using the heuristic above and state the selected visual direction in the brief delivery note.
