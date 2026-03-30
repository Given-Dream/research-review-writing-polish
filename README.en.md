# Research Review Writing Polish

`research-review-writing-polish` is a Codex skill for research-paper and review-paper language generation and polishing.

It is designed for users who already have research materials, such as outlines, notes, draft paragraphs, literature summaries, figure interpretations, or section drafts, and want those materials turned into publication-style academic prose without changing the scientific meaning.

This skill is not a literature retriever and not a citation fabricator. Its job is to help with drafting, rewriting, condensing, expanding, translating, and polishing while preserving evidential limits.

## What it does

- drafts sections from outlines or notes
- rewrites rough prose into cleaner academic language
- polishes near-final sections for clarity and reviewer readability
- condenses sections for word limits
- expands sparse notes into cautious manuscript-ready prose
- turns citation-heavy review text into synthesis-oriented review writing
- supports both research papers and review papers

## Methodology basis

This skill is grounded mainly in Adrian Wallwork's _English for Writing Research Papers_.

The skill borrows several core principles from that book:

- each section has a distinct rhetorical job
- writing should be reader-facing and referee-aware
- clarity and concision matter more than inflated style
- contribution should be shown with evidence, not hype words
- literature review and review-paper writing should be organized and synthetic, not paper-stacking
- Methods should be reproducible and orderly
- Results should highlight the meaningful findings rather than repeat tables
- Discussion should interpret without overclaiming
- Conclusions should add perspective rather than repeat earlier sections
- final polishing should emphasize readability, consistency, and reviewer trust

## Directory structure

```text
research-review-writing-polish/
|-- SKILL.md
|-- README.md
|-- README.en.md
|-- .gitignore
|-- agents/
|   `-- openai.yaml
|-- references/
    |-- section-patterns.md
    |-- review-synthesis-patterns.md
    |-- academic-tone-checklist.md
    `-- revision-output-templates.md
`-- examples/
    `-- ...
```

## Files

### `SKILL.md`

The main skill definition.
It defines trigger conditions, task classification, non-negotiables, section guidance, and default workflow.

### `references/section-patterns.md`

Section-by-section patterns for:

- title
- abstract
- introduction
- literature review
- review-paper body
- methods
- results
- discussion
- conclusions

Use this when the main need is section structure and section function.

### `references/review-synthesis-patterns.md`

Patterns for review writing and literature synthesis.

Use this when the draft is too citation-heavy, too catalogue-like, or lacks comparison and synthesis.

### `references/academic-tone-checklist.md`

A reviewer-facing checklist for:

- clarity
- concision
- precision
- contribution visibility
- evidential discipline
- readability
- consistency

Use this when the draft needs language polishing without changing meaning.

### `references/revision-output-templates.md`

Recommended output shapes for:

- polishing
- structural rewrite
- expansion from notes
- condensation
- review synthesis rewrite
- methods rewrite
- results rewrite
- discussion rewrite
- conclusion rewrite
- translation plus polishing

Use this when you want stable output formatting.

### `examples/`

Input/output examples for common tasks such as:

- generating a Discussion paragraph from notes
- turning literature notes into review synthesis
- condensing an abstract to a target length

## Best-fit use cases

This skill works best when the user already has one or more of the following:

- a section outline
- rough bullet points
- a Chinese or English draft
- literature notes
- review notes that need synthesis
- figure or table interpretation notes
- a section that is logically weak but factually usable

## Non-fit use cases

This skill is not the right first tool when the main need is:

- paper retrieval
- reference verification
- fact checking against the web
- data analysis
- experimental design from scratch
- fabricated citation or result generation

## Installation

Place this folder inside your Codex skills directory.

Typical layout:

```text
$CODEX_HOME/skills/research-review-writing-polish/
```

If you are managing skills manually, copy the whole folder rather than only `SKILL.md`, because the skill depends on the `references/` files and `agents/openai.yaml`.

## Example prompts

```text
Use $research-review-writing-polish to rewrite my introduction draft in more formal academic English without changing the scientific meaning.
```

```text
Use $research-review-writing-polish to turn my literature notes into a synthesis paragraph for a review paper rather than a paper-by-paper list.
```

```text
Use $research-review-writing-polish to condense this abstract to 200 words while preserving the contribution and limitations.
```

```text
Use $research-review-writing-polish to generate an English Discussion from my Chinese notes, but keep the claims conservative and limitation-aware.
```

## Authoring notes

This repository currently focuses on the language-generation and polishing layer.

It does not yet include:

- custom scripts
- icons
- evaluation examples
- sample assets

Those can be added later if you want this skill to become a more fully packaged public repository.
