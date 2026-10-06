# 来源保真与章节映射

制作内容映射或修改事实性文字时读取；所有原始来源保护约束持续生效。

### Source Fidelity and Protected Terms

Treat visual transformation as a change of presentation form, not a license to rewrite the source's facts, entities, or meaning.

- Before drafting, create an internal protected-source register containing every source-provided project or document title; customer, company, organization, and department name; case customer and case project name; product, platform, system, module, technology, standard, certification, and location name; date, version, quantity, amount, percentage, and other decision-relevant value; plus scope, status, condition, responsibility, commitment, attribution, and acceptance wording that affects interpretation.
- Preserve protected names exactly as written in the source in visible copy and accessibility metadata, including `alt`, `aria-label`, `title`, captions, navigation, and footer text. Do not translate, abbreviate, expand, rename, beautify, normalize, or replace them with a similar term. If the source provides both a full name and an abbreviation, use only those supplied forms. Line wrapping is allowed; truncation or silent shortening is not.
- Preserve anonymization, masking, placeholders, and disclosure boundaries exactly. Do not infer or restore an omitted customer, project, or organization name.
- Keep every case internally consistent. Do not rename a case, merge multiple cases, split one case into invented sub-cases, transfer facts or outcomes between cases, change the relationship between the customer and project, or turn a generic scenario into a named case.
- Preserve the source's meaning, attribution, scope, sequence, certainty, conditions, responsibilities, commitments, and conclusions. Do not turn a plan into a delivered capability, a possibility into a commitment, a pilot into full scope, an observation into a verified result, or one party's responsibility into another party's responsibility.
- Allow only meaning-preserving transformations: remove exact repetition, shorten redundant connective prose, split paragraphs into bullets, move an intact fact block to a more suitable page, or change a table into a relationship-appropriate visual structure. Keep the source wording when a rewrite could change domain meaning or factual nuance.
- When content does not fit, add a continuation page, stack the layout, or retain a compact table. Do not solve space pressure by dropping protected information, weakening qualifiers, or substituting shorter invented wording.
- If the source is ambiguous or internally inconsistent, preserve the relevant wording and mark it as needing confirmation. Do not silently correct, reconcile, or complete it.
- Maintain an internal traceability map from each protected term and decision-relevant source block to its output page and visible element. Any omission of protected or unique decision-relevant content requires explicit user approval and must be recorded as `user-approved omission`.

### Chapter Mapping and Synthesis

When a proposal, brief, or other source attachment is provided, use **source-faithful executive-summary mode** by default. The goal is an executive-grade paged presentation: every source chapter is visibly covered, logically adjacent chapters may be combined, and wording may be condensed only when the protected terms, unique facts, meaning, attribution, scope, conditions, and conclusions remain unchanged.

- Map every top-level source chapter to one or more HTML presentation pages. One page may combine multiple logically adjacent source chapters only when they support the same takeaway. Do not silently omit a top-level source chapter.
- In a combined section, retain a visible sub-heading, label, card group, or other identifiable content block for each merged source chapter. A generic chapter heading may be editorially rewritten only when its purpose remains unchanged; preserve every protected project, customer, case, product, platform, system, and module name inside a heading exactly as written.
- Treat source H3 sections as compact sub-blocks, cards, steps, evidence, or continuation pages inside their parent chapter unless the user requests one independent page per H3.
- Before writing HTML, create an internal map with: `source chapter`, `page number / anchor`, `page thesis`, `presentation form`, `coverage status`, and `protected terms / source blocks carried forward`.
- For each source chapter, write one clear takeaway and condense only redundant explanatory prose. Prefer three to six concise points when they can retain every unique decision-relevant fact. Preserve protected terms, named products or modules, named cases, delivery items, customer responsibilities, acceptance concerns, confirmation items, qualifiers, and attribution exactly enough to keep the source meaning unchanged.
- Treat source tables as source material, not as mandatory HTML tables. Extract their information relationship, then select a more suitable structure: a response matrix, comparison strip, card set, timeline, capability map, evidence list, or compact table. Do not reproduce a table row-for-row when grouping, short labels, or visual hierarchy communicate the same information more clearly.
- When table rows are repetitive, group them by their shared conclusion and retain the differentiating facts. Do not collapse rows that carry different commitments, owners, acceptance criteria, cases, products, or next actions.
- Preserve source-provided industry observations, competitive references, products, and cases as source-provided content. Keep their names, attribution, scope, status, and evidence relationships unchanged. Do not add external comparison claims or facts.
- Use visual transformation to improve readability, not to create a Word-to-HTML copy. “Chapter coverage” requires a distinct page or identifiable sub-block; it does not require copied prose or a duplicate table layout.

Before creating separate pages, apply a **meeting-compression pass**:

- merge requirement-response material into one page when its rows share one operating conclusion; group the content into two or three storylines such as efficiency, governance, and evidence instead of reproducing every row;
- merge implementation stages into one roadmap page when objectives, deliverables, cooperation, and acceptance can remain legible at the verified desktop sizes;
- combine next actions and confirmation items when they support the same meeting decision, using a compact action strip plus grouped decision themes;
- split only when unique commitments, owners, acceptance conditions, evidence, or source density cannot remain legible. Never add pages merely because the source uses separate headings or tables.

Create a **presentation-form inventory** in the internal page map, recording each page's primary relationship, form, and reason. Choose among thesis, operating storyline, response lanes, layered architecture, scenario loop, evidence narrative, timeline, action strip, or comparison according to real information. There is no minimum count or consecutive-repeat limit; consistent forms can support comparison. Keep tables for exact stable-field cross-reference, not as the automatic rendering of source tables.

### Delivery Modes

Select the delivery mode explicitly before drafting:

- **source-faithful executive-summary mode (default):** cover every top-level source chapter in an independent or combined HTML section; condense redundant prose while preserving all protected terms, unique decision-relevant facts, attribution, scope, conditions, and conclusions;
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
