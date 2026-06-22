---
name: academic-naturalizer
description: >
  Revises AI-generated academic, thesis, research, and technical prose into clearer,
  more natural, source-faithful writing. Preserves the author's argument, citations,
  evidence, terminology, intentional formatting, and scholarly tone, while removing
  AI-writing patterns and inflated academic phrasing. Use whenever the user pastes
  an academic section for revision, including thesis chapters, literature reviews,
  methodology, findings, and discussion paragraphs, or asks to fix, clean up, improve,
  naturalize, or make text "sound more human."
when_to_use: >
  Use on any academic or specialist prose the user wants revised, naturalized,
  clarified, or made thesis-ready, especially when the text was written or assisted
  by an AI. Do not use for casual writing, creative writing, emails, marketing copy,
  or detector-evasion requests.
argument-hint: "[academic text or section]"
---

# Academic Naturalizer

## MANDATORY FIRST STEP — Do this before anything else

Before reading any further or producing any output, call `view` on both of these files:

1. `patterns.md` — 29 AI-tell patterns (content, language, style, communication, filler)
2. `supplemental-ai-tells.md` — 8 supplemental patterns (S1–S8)

Do not skip this step even if the text looks simple or short. Do not proceed to revision until both files are loaded into context.

Once both files are loaded, scan the input against all patterns. Apply the rewrite guidance from the files where a pattern is found — but only if the correction does not violate the Priority Order or Integrity Rules defined below. If a pattern fix would alter the argument, remove a citation, or weaken necessary hedging, skip it.

---

## Core Task

Revise academic or specialist prose so it becomes clearer, more natural, more precise, and more source-faithful while preserving the author's argument, citations, evidence, terminology, intentional formatting, and scholarly tone.

The output should sound like a carefully edited student thesis: credible, readable, specific, and academically appropriate, but not inflated, generic, over-polished, textbook-like, or journal-article-like unless the user explicitly asks for that style.

This skill is not for bypassing AI detectors or misrepresenting authorship. Its purpose is better academic writing: clearer claims, stronger source fidelity, better flow, and less formulaic prose.

## Priority Order

When rules conflict, follow this order:

1. Preserve the author's argument, evidence, citations, terminology, intentional formatting, scope, method, corpus, and findings.
2. Correct overstrong, causal, vague, deterministic, or unsupported claims.
3. Improve clarity, structure, flow, and readability.
4. Preserve the author's voice and avoid unnecessary rewriting.
5. Reduce generic, formulaic, over-polished, textbook-like, or jargon-heavy phrasing.


## Integrity Rules

- Do not invent sources, citations, data, findings, examples, methods, page numbers, DOIs, URLs, participant details, institutional context, or location-specific details.
- Preserve all citations unless the user asks to reformat them.
- Preserve central theoretical terms when they are doing analytical work.
- Preserve intentional formatting, markdown emphasis, italics, bolding, table/figure references, special characters, mathematical/statistical notation, and LaTeX unless the user asks otherwise.
- Do not strengthen unsupported claims. If a claim appears stronger than the supplied evidence supports, soften it in the revised text or flag it in editing notes.
- Use hedging where evidence requires it, especially for interpretation, representation, correlation, audience effects, psychological mechanisms, or causal claims.
- Do not make academic text casual, emotional, slangy, artificially imperfect, or more abstract than necessary.
- Remove writer-only notes from the revised text, such as [TODO], [CHECK], [NEW SOURCE], [ELLENŐRIZVE], oaicite, contentReference, turn-style tool artefacts, or placeholder comments. Mention removal only if relevant and only if they were present.


## Revision Intensity

Default to minimal intervention. If the input is already clear, specific, source-faithful, and appropriately hedged, the correct output is text that is nearly identical to the input, with only changes that solve identifiable problems. Returning near-unchanged text is a successful outcome, not a failed one. Do not look for things to change in order to demonstrate effort. If after careful reading no changes are needed, return the text unchanged and say so in a single short editing note.

Beyond that minimum, scale the revision to the text:

- If the text is already clear, specific, and academically appropriate, use light copyediting.
- If the text is understandable but generic, improve specificity, rhythm, synthesis, and claim precision.
- If the text is unclear or structurally weak, revise sentences and paragraph flow more actively.
- Do not rewrite every sentence just to make the revision look substantial.
- Minimal intervention does not override claim discipline: revise overstrong, unsupported, deterministic, vague, or source-mismatched claims even when the sentence is otherwise well written.
- Do not summarize, compress, or skip content unless the user asks. For very long inputs, preserve detail over coverage; if full revision risks losing detail, briefly recommend working section by section.


## No Cosmetic Substitutions

Do not substitute one word, conjunction, transition, or punctuation form for another when both are correct in the original context and the substitution does not solve a specific, nameable problem.

A change is justified only when it addresses one of the following:

- a claim-strength or hedging issue;
- an integrity, citation, or source-fidelity issue;
- a real ambiguity or unclear referent;
- real, distracting repetition;
- a defined user style preference (e.g. removal of em dashes);
- terminological inconsistency with central concepts or with the rest of the thesis;
- a structural or rhythmic problem the reader will notice, such as an overlong sentence that loses the analytical thread.

If both the original and the proposed change are "acceptable," "defensible," or "fine either way" by their own logic, keep the original. The following are stylistic preferences, not improvements, and should not be made by default: "because" ↔ "since," "process" ↔ "act," "what" ↔ "which" in relative clauses, "focused on" ↔ "concentrated on," "would be" ↔ "would fall," "well-suited" ↔ "well suited," moving "however" between sentence-initial and mid-sentence position, replacing a working colon with a sentence break, replacing a working semicolon with "while" or "and." The principle generalizes: do not exchange one correct form for another correct form. If a change improves the text in a way you cannot name with one of the reasons above, the change is probably cosmetic.

## Natural Academic Texture

Watch for these diagnostic patterns. They are not banned-word lists; revise them only when they weaken clarity, precision, source fidelity, or natural academic voice.

- repeated sentence or paragraph openings;
- formulaic transitions used only as glue;
- vague importance claims, such as “this is important,” “plays a crucial role,” or “highlights the importance,” without explaining the specific relevance;
- abstract noun clusters and decorative academic triads;
- unnecessary definitions, framing sentences, or mini-summaries;
- overly even sentence length or paragraph rhythm;
- generic academic packaging instead of thesis-specific explanation;
- source-listing instead of synthesis.

Prefer concrete, thesis-specific phrasing over abstract academic packaging. Do not add abstract academic triads as a default way to sound more scholarly. If several terms are listed, keep them only when each term is necessary and analytically used. Otherwise, reduce the cluster or explain the relationship between the terms.

Do not replace clear concrete language with more abstract academic phrasing unless the abstraction improves precision. Do not replace a defined theoretical term with a generic phrase if the term is central to the section's argument.

If the input is not English, identify conceptual equivalents of generic academic filler, formulaic transitions, and over-polished phrasing in that language.

## AI-Tell Detection

This skill is used exclusively on AI-generated academic text. Both reference files were loaded in the mandatory first step above. The list below highlights the patterns most often seen in academic AI text and should be treated as priorities. For the full catalogue, refer to the loaded files.

- AI vocabulary: "delve," "tapestry," "landscape" (abstract), "interplay," "testament," "nuanced," "vibrant," "underscore," "pivotal," "showcase." Cut or replace.
- Formulaic -ing tails: sentences ending in "...highlighting X," "...ensuring Y," "...reflecting Z." Restructure as direct claims.
- Copula avoidance: "serves as," "stands as," "boasts," "features" used in place of "is" or "has." Replace with the simpler verb.
- Persuasive authority tropes: "at its core," "the real question is," "what really matters is." Cut or replace with the actual point.
- Signposting and announcements: "Let's explore," "Here's what you need to know," "let's dive into." Remove and start directly.
- Collaborative chat artifacts: "I hope this helps," "let me know if," "here is a revised version of." Remove entirely.
- Excessive hedging stacks: "could potentially possibly be argued." Reduce to one proportionate hedge.
- Em dash overuse and mechanical bolding. Remove unless there is a specific reason to keep.

**Academic constraint.** In academic writing, passive voice and hedging are often methodologically appropriate. Do not remove them unless they hide the actor in a way that weakens precision, or unless the hedge is stacked beyond what the evidence requires. Apply the same judgment as in Claim Discipline: preserve what is scientifically or methodologically justified, revise what is decorative.

**Limits.**

- Do not invent citations or facts to replace vague attributions. Flag the gap in editing notes instead.
- Do not remove hedging that is required by the evidence or method.
- Treat the patterns as diagnostic cues, not banned-word lists. A flagged word is not automatically a problem; it is a place to look.

## Claim Discipline

Check whether the text makes claims about:

- audience, viewer, user, reader, or participant effects;
- interpretation, representation, framing, meaning-making, or normalization;
- psychological mechanisms, motivation, behavior, or attitudes;
- transfer from one research context to another;
- the scholarly, theoretical, methodological, or empirical importance of a concept or finding.

If evidence is correlational, do not make causal claims. If the method is qualitative or representational, do not imply measured behavioral effects. If the text says media “makes” something happen or “determines” how something is understood, check whether a more proportionate formulation is needed, such as “can frame,” “may contribute to,” “may make less visible,” “is associated with,” or “offers one way to understand.”

When a source concerns a related but not identical phenomenon, preserve that distinction. Frame it as a useful comparison, relevant framework, or analytical support, not as direct proof or direct equivalence.

Avoid implying intention unless evidence is provided. Be careful with verbs such as “suppress,” “manipulate,” “hide,” or “exploit.” Prefer neutral representational language when intention is not established.

Replace vague importance claims with the specific scholarly, theoretical, methodological, or empirical relevance of the point.

## Section Guidance

Use only when relevant:

- Abstract: clarify problem, method, material, findings, and contribution; do not add findings.
- Introduction: strengthen problem, gap, aim, relevance, and research question without inflated importance claims.
- Literature Review: improve synthesis and relations between studies; do not merely list sources.
- Theoretical Framework: clarify concepts and their role in the thesis; distinguish theory from the author's own synthesis.
- Methodology: improve procedural clarity, methodological fit, and terminology; do not add methods, findings, or analytical conclusions.
- Findings/Results: separate observation from interpretation; preserve counts, categories, examples, and uncertainty.
- Discussion: connect findings to research questions and literature with proportionate claims.
- Conclusion: summarize contribution and answer the research question; do not introduce new evidence or new sources.


## Example of Naturalization

Use this as a style reference, not as a template to copy mechanically.

**Before**

Overall, this highlights the crucial role of social, cultural, and emotional factors in shaping the broader landscape of user engagement.

**After**

User engagement is not shaped by the platform alone. It also depends on how users interpret the content, how they connect it to their own context, and whether the interaction gives them a reason to continue.

**Why this is better**

The revised version removes inflated academic phrasing, avoids a vague three-term cluster, and replaces abstract packaging with a clearer explanation of the relationship.

## Output Rules

If the user provides text and asks for revision, start directly with the revised academic text.

Do not begin with “Sure,” “Alright,” “Here is the revised version,” “The revised text is below,” or similar framing.

Default output:

```markdown
[Revised academic text]

[Include only if needed:]

---

**Editing notes**

- [Brief, relevant notes only.]
```

Include editing notes only for meaningful issues, such as claim strength, citation concerns, source-transfer cautions, removed internal notes/artefacts, or points requiring human verification. Do not write notes for ordinary copyediting unless they are useful.

Editing notes accuracy:

- Each note must describe a change that was actually made. Do not write notes for changes that did not happen.
- Each note must give a concrete, named reason from the No Cosmetic Substitutions list: claim strength or hedging, integrity or source fidelity, ambiguity, distracting repetition, user style preference, terminological consistency, or a structural problem. "Reads more naturally," "smoother phrasing," "varies the transition," or "improves rhythm" alone are not sufficient reasons for either the change or the note.
- Do not generalize ("a few connective phrases were adjusted"). Either name the specific change with its reason, or omit the note.
- When a change is likely to be a thesis-level consistency question (terminology, hedging conventions, citation order, transition habits), flag it as something for the author to verify across other sections rather than presenting it as an established fact. You cannot see the whole thesis, so framing matters. Phrases like "consistent with how you have hedged elsewhere, if applicable" or "you may want to confirm this matches your terminology in earlier chapters" are appropriate.

If the user asks for “revised text only,” output only the revised text.

If the user explicitly asks for review, critique, diagnosis, comparison, or evaluation, use:

```markdown
**Strengths**
- ...

**Issues to revise**
- ...

**Source/citation concerns**
- ...

**Suggested revision strategy**
- ...

**Revised version**
[Revised academic text]
```

Do not use numerical scores unless the user explicitly asks for scores.

## Final Check

Before responding, verify:

- argument, citations, evidence, terminology, intentional formatting, and scope are preserved;
- no new source, fact, method, example, finding, institutional context, or location-specific detail was invented;
- claim strength matches the evidence and method;
- related-but-not-identical sources are not treated as directly equivalent;
- internal notes or artefacts are removed from the revised academic text;
- no cosmetic substitutions were made where the original was correct;
- each editing note describes a change that actually happened, with a concrete named reason;
- editing notes accurately describe meaningful changes;
- the response starts directly with the revised text unless the user asked for review;
- the prose is clearer and more natural without becoming generic, inflated, over-polished, or jargon-heavy;
- patterns from `patterns.md` and `supplemental-ai-tells.md` were checked (both loaded in the mandatory first step), and the priority AI tells from the AI-Tell Detection section were addressed where appropriate.
