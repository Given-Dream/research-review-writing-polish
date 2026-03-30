---
name: research-review-writing-polish
description: Use when the user is drafting or revising a research paper or review paper and wants Codex to generate, rewrite, expand, condense, translate, or polish academic prose from outlines, notes, literature summaries, figure interpretations, or draft text while preserving scientific meaning and evidential boundaries.
---

# Research Review Writing Polish

This skill turns research materials into publication-style academic prose.

Its job is not to invent content. Its job is to preserve the scientific meaning of the user's materials while improving logic, flow, clarity, concision, and academic register.

## Use when

- The user is writing or revising a research paper or review paper.
- The user wants section drafting, paragraph generation, rewriting, polishing, expansion, condensation, restructuring, or academic translation.
- The user provides outlines, notes, bullet points, literature summaries, figure/table interpretations, Chinese source materials, English drafts, or section drafts.
- The user asks for clearer, more formal, more concise, more logical, or more journal-appropriate academic prose.

## Do not use when

- The user mainly needs literature retrieval, paper download, citation verification, fact checking, or data analysis.
- The user wants fabricated references, invented results, or unsupported claims.
- The user only wants a normal paper summary rather than writing help.

## Core objective

- Preserve scientific meaning.
- Improve logic and readability.
- Increase formality and section-level fitness.
- Keep claims within evidential bounds.
- Produce text that a reviewer can read quickly and trust.

## First classify the task

Identify which writing operation the user actually needs:

- drafting from outline or notes
- rewriting rough prose
- polishing near-final prose
- condensing for word limit
- expanding a subsection
- restructuring for logic
- translating into academic Chinese or academic English
- synthesizing review prose from multiple literature notes

Do not treat all requests as simple polishing.

## Then classify the section function

Identify the paragraph or section role before rewriting:

- title
- abstract
- introduction
- literature review
- review-paper body
- methods
- results
- discussion
- conclusion
- figure/table commentary
- cover letter or response text, only if the user explicitly asks

The rewrite should match the function of the section, not just improve sentence quality in isolation.

## Use references progressively

- For section function and expected content, read [references/section-patterns.md](references/section-patterns.md).
- For review-paper synthesis and citation-heavy material, read [references/review-synthesis-patterns.md](references/review-synthesis-patterns.md).
- For tone, readability, and reviewer-facing polish, read [references/academic-tone-checklist.md](references/academic-tone-checklist.md).
- For output shape, use [references/revision-output-templates.md](references/revision-output-templates.md).

Load only what is needed for the current request.

## Non-negotiables

- Do not fabricate data, citations, experiments, results, or methods.
- Do not overstate novelty, significance, causality, certainty, or generality.
- Do not change the scientific meaning unless the user explicitly asks for content-level revision.
- Preserve limitations, uncertainty, scope conditions, contrast markers, and exception conditions.
- Keep terminology, abbreviations, variables, named methods, and quantitative values consistent.
- If the source support is weak, use conservative wording.
- If critical information is missing, either ask for the smallest missing item or produce a clearly conservative version.

## Journal alignment

If the user provides a target journal, field, or section guideline:

- align tone, density, and section conventions to that context
- follow user-provided word limits or structure requirements
- respect whether the field prefers stronger or more cautious rhetorical style

If no journal is given, default to a clear, moderately conservative academic style.

## Default workflow

1. Identify the output language, task type, and section function.
2. Extract the facts and claims that must not change.
3. Identify the paragraph's job:
- context
- gap
- aim
- method
- finding
- interpretation
- limitation
- implication
4. Rebuild the logic so the text has a clear opening, development, and close.
5. Rewrite in the register required by the section.
6. Run a final boundary check:
- no invented content
- no inflated claims
- no broken logic
- no fabricated citations
7. Return the output in the form the user needs.

## Section guidance

### Title

- Be specific, readable, and information-dense.
- Prefer clarity over cleverness.
- Avoid empty hype words such as novel, innovative, remarkable, or groundbreaking unless clearly justified by the user's materials.

### Abstract

- State topic, problem, aim, approach, main finding, and contribution.
- Keep only the information needed to understand the study.
- Avoid unsupported implications or exaggerated claims.
- If the abstract is for a review paper, make the scope, organizing logic, and synthesis outcome visible.

### Introduction

- Move from context to gap to objective to contribution.
- Keep background selective rather than encyclopedic.
- Make clear why the problem matters and what this paper adds.
- If useful, end with a brief roadmap of the paper.

### Literature review / review-paper body

- Synthesize rather than stack references.
- Group studies by theme, method, period, question, or debate.
- Highlight agreements, conflicts, blind spots, and trends.
- Do not produce one-paper-one-sentence catalogues unless the user explicitly wants an inventory.
- Keep the author's evaluative and organizing line visible.

### Methods

- Prioritize precision, reproducibility, and sequence clarity.
- Describe only what is needed for the reader to understand and evaluate the procedure.
- Avoid promotional language.
- Keep tense, voice, and terminology consistent.

### Results

- Report findings directly.
- Foreground the patterns, comparisons, or contrasts that matter.
- Do not interpret beyond what belongs in results, unless the target genre merges results and discussion.
- Align figure/table commentary with the actual claim being made.

### Discussion

- Interpret the results, compare with prior work, explain meaning, and delimit scope.
- Distinguish clearly between:
- what the data show
- what the author infers
- what remains uncertain
- Include limitations where relevant.
- Avoid repeating the results section without added interpretation.

### Conclusion

- Restate the main contribution without repeating the entire abstract.
- End on implication, usefulness, limitation-aware significance, or future work.
- Keep the tone measured.

## Review-paper specific rules

- Make the organizing framework explicit.
- Synthesize across studies instead of paraphrasing each paper in isolation.
- Define comparison dimensions before using them.
- Identify research gaps conservatively.
- If the source notes are thin, prefer a scoped synthesis over a sweeping field-level claim.
- Do not let the prose collapse into citation stacking with no argument.

## Language and style rules

- Prefer direct, formal, compact sentences.
- Remove redundancy, filler, and vague boosters.
- Keep paragraph openings functional.
- Use transitions to show contrast, cause, addition, boundary, and limitation.
- Prefer precise verbs over noun-heavy phrasing when meaning is preserved.
- If translating from Chinese to English or English to Chinese, prioritize academic naturalness over literal mirroring.
- Preserve all numbers, units, citations, equations, and named methods exactly unless the user asks otherwise.
- If the source wording is awkward but scientifically important, preserve the claim and improve only the expression.

## Output modes

When the user does not specify a format, default to one of these:

- clean rewritten text
- polished text plus a short list of major revisions
- expanded subsection
- condensed version
- two alternative versions: more concise / more formal

## What to do when material is incomplete

- Do not fill gaps with invented facts.
- If a full draft would be risky, say what is missing in one short block.
- If the user still wants a draft, produce the most conservative usable version.
- When helpful, keep the claim narrower rather than broader.
- If a citation would normally be needed but none is provided, do not invent one.

## Common failure patterns to avoid

- changing the scientific claim while polishing the language
- turning cautious results into strong causal claims
- stuffing review prose with citation stacks but no synthesis
- repeating the same idea in multiple sentences
- mixing results with discussion without clear signaling
- using vague evaluative adjectives without explaining why
- flattening important contrasts, exceptions, or limitations
- making the prose sound polished but less accurate

## Default outputs

Prefer outputs that can be used immediately in a manuscript:

- polished paragraph
- revised subsection
- abstract rewrite
- introduction rewrite
- review synthesis paragraph
- methods/results/discussion/conclusion rewrite
- concise version for word-limit reduction
- rewrite plus revision notes

## Example prompts

- Use `research-review-writing-polish` to rewrite my introduction draft in more formal academic English without changing the meaning.
- Use `research-review-writing-polish` to expand these bullet points into a discussion subsection for a research paper.
- Use `research-review-writing-polish` to turn my literature notes into a synthesis paragraph for a review paper, not a paper-by-paper list.
- Use `research-review-writing-polish` to condense this abstract to 200 words while preserving the contribution and limitations.
- Use `research-review-writing-polish` to turn my rough review paragraph into journal-style prose without inventing citations.
- Use `research-review-writing-polish` to generate an English Discussion from my Chinese notes without overstating the conclusion.
- Use `research-review-writing-polish` to make this Results section clearer without turning it into Discussion.
