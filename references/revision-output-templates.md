# Revision Output Templates

This file defines output formats for drafting, rewriting, polishing, condensing, and review synthesis.
It is based on Wallwork's section-function logic, his emphasis on clarity and referee usability, and his warnings about generic AI text.

## Goal

Return outputs that are immediately useful in manuscript work.

Prefer outputs that:
- preserve the user's scientific meaning
- make the section function clearer
- expose unsupported areas instead of inventing content
- keep revision notes short and high-value

## General output rule

Unless the user requests otherwise, return:
1. the revised text
2. a short note on the main changes
3. one short block of unresolved risks, only if necessary

Do not overwhelm the user with editing commentary.

## Template 1: Polish only

Use when the user has a workable paragraph or section and mainly wants language improvement.

### Output format

#### Revised text
[polished paragraph or section]

#### Main changes
- improved clarity and sentence flow
- reduced redundancy
- adjusted tone to a more academic register
- preserved original claim scope

#### Risks or gaps
- only include if a claim is unclear, unsupported, or internally inconsistent

## Template 2: Structural rewrite

Use when the paragraph is logically disordered or the section is not doing its job.

### Output format

#### Revised text
[rewritten text]

#### Structural changes
- opening sentence now states the paragraph's function
- supporting material reordered for clearer progression
- result and interpretation separated more cleanly
- contribution/limitation made more explicit

#### Remaining issue
- [only if essential information is missing]

## Template 3: Expand from notes

Use when the user provides bullet points, figure notes, or outline fragments.

### Output format

#### Draft text
[expanded section or paragraph]

#### What was inferred from the notes
- paragraph function
- likely logical order
- conservative connective wording where detail was missing

#### Missing inputs
- [only the smallest missing items needed for a stronger version]

## Template 4: Condense for word limit

Use when the user needs a tighter section, abstract, or conclusion.

### Output format

#### Condensed version
[shorter text]

#### What was compressed
- background trimming
- repeated claims merged
- low-value modifiers removed
- table/figure description shortened in favor of interpretation

#### Watch point
- [only if compression forced a sharper or more cautious phrasing choice]

## Template 5: Review synthesis rewrite

Use when the user provides literature notes or citation-heavy draft text.

### Output format

#### Synthesis version
[rewritten review paragraph or subsection]

#### Synthesis moves applied
- grouped related studies
- reduced paper-by-paper listing
- foregrounded comparison or trend
- made the section-level takeaway explicit

#### Gap notice
- [only if the literature pool is too thin for the claim being made]

## Template 6: Methods rewrite

Use when the user needs a clearer procedure description.

### Output format

#### Revised methods text
[rewritten methods]

#### Improvements made
- chronological/logical order clarified
- ambiguity reduced
- unnecessary detail cut or referenced
- tense and voice normalized

#### Replication risk
- [only if a required methodological detail appears missing]

## Template 7: Results rewrite

Use when the user needs findings reported more clearly.

### Output format

#### Revised results text
[rewritten results]

#### Improvements made
- prioritized the most relevant findings
- changed table/figure repetition into interpretation-supporting prose
- clarified which findings are primary vs secondary
- preserved negative or contradictory results where relevant

#### Boundary note
- [only if interpretation is drifting into discussion]

## Template 8: Discussion rewrite

Use when the user needs stronger interpretation but controlled claims.

### Output format

#### Revised discussion text
[rewritten discussion]

#### Improvements made
- foregrounded the key finding
- clarified relation to prior work
- separated evidence from interpretation
- added or sharpened limitation-aware wording

#### Overclaim check
- [only if the original draft exceeded the evidence]

## Template 9: Conclusion rewrite

Use when the user's conclusion is repetitive or vague.

### Output format

#### Revised conclusion
[rewritten conclusion]

#### Improvements made
- reduced repetition from earlier sections
- clarified take-home message
- made implications more specific
- kept future directions realistic

#### Caution
- [only if the conclusion still depends on unsupported broad implications]

## Template 10: Translation plus polishing

Use when the user provides Chinese source material for English academic prose, or the reverse.

### Output format

#### Polished translation
[translated and polished text]

#### Translation choices
- academic rather than literal wording
- preserved technical meaning
- retained caution and scope markers
- normalized sentence flow for the target language

#### Check needed
- [only if a technical term or field-specific phrase is ambiguous]

## Short fallback template

Use when the user asks for a very fast answer.

### Output format

#### Revised text
[text]

#### One-line note
- tightened language and preserved scientific meaning

## When not to give detailed revision notes

Do not add long notes when:
- the user only asked for a clean rewrite
- the revision is minor
- the output itself makes the change obvious

## When to surface a warning

Surface a warning only if one of these is true:
- the source text contains factual inconsistency
- the claim is stronger than the evidence
- essential detail is missing
- the section function is fundamentally misassigned
- the user appears to be asking for fabricated or unattributed content

## Final check before returning output

Ask:
- Is the revised version immediately usable?
- Is the section function clearer now?
- Did I preserve meaning and evidential limits?
- Did I remove generic AI-sounding phrasing?
- Did I avoid bloating the response with unnecessary commentary?
