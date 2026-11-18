---
name: technical-writing-style
description: 'Use when drafting, revising or reviewing technical or explanatory prose — READMEs, design docs, specs, API references, tutorials, runbooks, manuals, reports, proposals, academic writing, emails or agent reports — where correctness, precision, conciseness, audience fit, structure or reader comprehension matter. Distilled from Laplante''s Technical Writing and reader-centred editing practice.'
---

# Technical Writing Style

## Overview

Two principles govern everything below.

1. **Write as if the text will be executed.** Technical writing is any writing where facts must be provable and errors have consequences. A misplaced hyphen lost NASA's Mariner 1. Every statement may be realised in a device, process or action, so verify decimals, signs, units and names character by character, and make every sentence admit exactly one interpretation.
2. **Minimise the reader's effort, not the number of tokens.** Every word must earn its place, but a slightly longer, clearer expression beats a compressed, ambiguous one. Conciseness takes more effort, not less.

When the two principles pull apart, comprehension wins: cut what adds nothing, but never compress a statement into ambiguity.

## When to use

- Writing or editing any technical document: README, design doc, spec, API reference, tutorial, runbook, user manual, report, proposal, email, minutes or presentation.
- Any prose intended for human readers: academic writing, reviews, agent reports, incident reports, complaint letters, insurance or legal responses. Treat it as technical writing even if it "feels" informal.
- Reviewing or grading someone else's writing, or deciding tone, structure and audience treatment for a document.

**When not to use:** marketing or sales copy is the one context that deliberately evokes emotion. The honesty rules below still apply: never advertise features that do not exist.

## Inputs, audience and register

- **Establish the audience and purpose first.** If the audience is missing, infer it from the task, state the assumption and proceed. Ask only when the uncertainty would materially change the result. For mixed audiences, write to the most formal reader (for example, structure an incident report for the regulator who may see it).
- **Establish what must be preserved:** the main message, supporting claims, qualifications, citations, technical terms, requested actions and any length or format constraints. Do not invent missing information.
- **Pick one point of view and hold it:** first person (I/we) for business communication and narratives; second person (you) for procedures, tutorials, runbooks and user guides; third person with anonymised actors (Driver A, Service B) for incident, experiment and postmortem reports.
- **Strip emotion, blame, speculation and accusation** from factual reports. Report observable facts and outcomes in a neutral register.
- **Humour:** never in specs, proposals, safety or failure analyses, résumés, formal customer letters or journals. Discretionary and sparse in manuals, procedures and progress reports. For international or non-native readers, remove humour, slang, metaphors, euphemisms and cultural references entirely.
- **Spell out every acronym exactly once** before first use. Define any term not in a standard dictionary; add a glossary when jargon is unavoidable (construction rules: [reference.md](reference.md) §1b).
- **State reader assumptions explicitly.** In tutorials the two failure modes are over-explaining and skipping "obvious" details.
- **Use British spelling** unless explicitly instructed otherwise: organise, behaviour, colour, centre, licence, catalogue. Keep one dialect throughout.

## The writing process

`brief → structure → draft → revise → edit → verify → publish` — phases blur and loop back.

| Phase | Budget | Rule |
|---|---|---|
| Brief | ~10% | Establish audience, purpose, constraints and what must be preserved. Decide dialect, format and length. |
| Structure | ~15% | Concept-map the document: nodes become headings, and missing nodes reveal coverage gaps. Do not start prose until about 90% of the headings exist. Organise high-level to detailed. |
| Draft | ~35% | Write fearlessly; do not fix grammar yet. Record snippets rather than polished prose where that keeps momentum. |
| Revise | ~20% | Restructure content and logic — a different pass from editing. Do not let the text grow without a comprehension reason. Get two reviewers: one domain expert and one non-technical strong writer; the non-technical reviewer catches logic errors the expert misses. |
| Edit | ~10% | Copy-edit presentation: grammar, word substitution, precision, consistency and citations. |
| Verify | ~5% | Run the verification gate below. Editing can introduce new errors ("many fold" → "manifold"), so every edited version needs one more check. |
| Publish | ~5% | Publishing is permanent. Finish citation, permission and plagiarism checks before this gate. |

Stop revising when you start undoing your own recent changes.

## The 5 Cs (acceptance criteria)

| C | Means | Test |
|---|---|---|
| **Correct** | Grammatically and technically correct | Peer review — spell-checkers catch "kilometres" but not 200 versus 2000 |
| **Clear** | Exactly one interpretation per sentence | Ask "How do I test this?" — ambiguity fails this question |
| **Complete** | Nothing relevant to the reader's needs is missing | Maximum readership is the strongest check; log known gaps for the next version |
| **Consistent** | No self-contradiction; agrees with related documents and standards | Review; use a uniform level of detail per feature |
| **Changeable** | Structure yields to modification | Number sections and requirements; use a common electronic format; track changes with sources and dates |

## Comprehension: diagnose and revise

Treat these signals as review cues, not automatic errors. Check for:

- long gaps between subjects and verbs, or between other closely related words;
- nested clauses that interrupt the main point;
- dense strings of nouns with unclear relationships;
- omitted connecting words that make sentence structure harder to follow;
- unfamiliar word combinations, improvised verbs or strained personification;
- sentences carrying too many distinct ideas.

Then revise:

- Put the main point early.
- Keep related words close together.
- Split overloaded sentences at meaningful boundaries.
- Expand noun strings into explicit relationships.
- Restore words such as "that" where they clarify structure.
- Prefer familiar, precise expressions to compressed novelty.
- Make actors, actions and referents explicit. Prefer the active voice and name the actor when the actor matters and is known; keep the passive when the actor is unknown or irrelevant, or when it preserves topic flow. "The interfaces are tested at the last minute" → "Engineers test the interfaces — if they test them at all."
- Retain necessary technical terminology and explain it for the audience.
- Use headings and lists when they clarify genuine structure.

Do not mechanically remove passive voice, metaphors or complex sentences. Keep them when they serve the meaning and the audience. Worked examples and diagnosis detail are in [reference.md](reference.md) §1c.

## Precision

**Replace vague modifiers with measurements, thresholds or ranges.**

- ❌ "Leakage should be minimal." → ✅ "Leakage should be less than one millilitre per day."
- ❌ "Only a few may be defective." → ✅ "Fewer than ten may be defective."
- "98% shall be within tolerance" beats "a substantial amount within tolerance".

Quantifier mapping when you must approximate:

| Imprecise | A few | Some | Many | Most | All |
|---|---|---|---|---|---|
| Fraction | <10% | 10–20% | 21–50% | 51–99% | 100% |

| Always | Frequently | Often | Sometimes | Rarely | Never |
|---|---|---|---|---|---|
| 100% | 99–75% | 75–50% | 50–25% | 25–1% | 0% |

**Universal claims** ("all", "never", "none", "each") are ∀-quantifiers. Unless demonstrably true, omit them or add the exception explicitly: "All users, except new users, shall…".

**Negatives:** prefer positive verbs — "do not include" → **exclude**; "do not permit" → **forbid**. Use "shall not" only where it is more testable ("shall not permit access to unauthorised users" — you only need unauthorised-user test cases). Never stack negatives ("end brake retarder prohibition"): one negation per statement maximum.

**Hedging** ("likely", "probably", "might be"): replace with a probability or rate when one exists. Hedge only when you have no data, and then say so plainly. "There is no sense in being precise when you don't even know what you're talking about." — von Neumann.

## Conciseness and word choice

Delete any word, sentence or section that adds nothing. Replace two or more words with one where the result stays clear. The full replacement list is in [reference.md](reference.md) §2.

**Delete every "very"** (and really, extremely, massively): use one precise word or a measurement. Better than any synonym is the measured quantity: "the tree is 250 feet tall" beats "very tall".

**Delete filler phrases outright** (list: [reference.md](reference.md) §2).

## Banned language and traps

- Comparative phrases: "better than", "higher quality" (better than what, measured how?).
- Indefinite pronouns with unclear referents: "it", "this", "that".
- Loopholes: "if possible", "as appropriate", "as applicable", "but not limited to".
- Non-verifiable terms: "provide support", "a number of", "as a minimum".
- Superlatives: "best", "most" (usually unverifiable).
- Subjective language: "user friendly", "easy to use", "cost effective".
- **Anthropomorphism:** systems do not feel, want or fail "miserably". ❌ "The system failed miserably" → ✅ "The system failed: <factual detail>."
- **Clichés:** replace with plain meaning (list: [reference.md](reference.md) §2).
- **Malapropisms and heterographs:** sound-alike errors that spell-check never catches; hunt them manually. Full lists are in [reference.md](reference.md) §2.

## Structure and document design

- **Organise hierarchically: high-level to increasingly detailed.** Rarely go beyond a fourth-level heading. Balance externally (roughly uniform counts per level — a pyramid: more low-level than top-level sections) and internally (uniform section lengths). An hourglass shape means missing mid-level detail; a diamond means missing low-level detail.
- **Never ship free-form or stream-of-consciousness organisation.** Reorganise into a logical structure before publishing.
- **Number, caption and call out every figure and table** in the text ("as shown in Figure 3") before it appears. Never end a section on a caption — discuss the figure after it. Number only equations you refer back to, and define every symbol before first use. If a caption needs to be long, the figure is too complex; move detail into the prose.
- **Convert dense numeric prose into a chart**, but normalise the data so the chart cannot mislead, and state in words what a chart hides.
- **Keep tables simple:** no nested columns. When a table is dense, summarise its highlights in words or split it into simpler tables.
- **Put the strongest and most useful material first.** Readers skim and stop early.
- **Write the executive summary last.** Omit empty sections entirely and never leave a header with "none" beneath it.
- **Anticipate FAQs in the document itself** (troubleshooting, Q&A appendix); the document cannot answer back.
- Figure and table detail, including permissions, is in [reference.md](reference.md) §3.

## Special duties: procedures, manuals and email

**Procedures and manuals**

- Assume a novice reader, or document your assumptions. Use exact values ("less than 5 mL"), never vague ones ("minimal").
- Required elements and their order are in the procedure template in [reference.md](reference.md) §1.
- Test procedures and manuals with people who did not write them — experts and novices — under worst-case conditions (fatigued, hurried, surprised), not ideal ones.
- Write the user manual at the end of development; explain why features exist, not just how.
- **Ambiguity in operational text is a correctness failure, not a style nit.** In safety-critical systems, unclear instructions and interfaces can contribute to fatal errors (Therac-25).

**Email**

- Follow the email template in [reference.md](reference.md) §1.
- **Never deliver emotionally loaded news by email.** Talk first, confirm in writing afterwards.

## Honesty and attribution

- **Never exaggerate or claim what you cannot evidence.** Readers test claims, and contradictions are discoverable. Rate proficiency on a fixed scale (proficient, moderately proficient, familiar), per skill — never "expert in everything".
- **Say what you specifically did**, with action verbs, not what "the team" did.
- **Use reliable references.** Prefer named authors to anonymous wiki-style content, balance the reference mix, and do not cite sources more than ten years old for fast-changing technologies.
- **Attribution, permissions and self-plagiarism:** follow the six rules and permission procedure in [reference.md](reference.md) §4.

## Verification gate

Run this before publishing. Do not skip a step because the text "looks fine".

1. **Fidelity diff.** Compare the revision with the source. Are all substantive claims and qualifications preserved? Are causal relationships, uncertainty and scope unchanged? Are citations still attached to the correct claims? Has any ambiguity, unsupported claim or factual change been introduced? Correct any mismatch before proceeding.
2. **5 Cs.** Check every criterion in the table above. Peer review beats automation.
3. **Reader pass.** Read the result in order, without relying on unstated context. Can the reader identify the main point, who or what performs each action, how the ideas relate, and what any requested next step involves?
4. **Mechanical checks.** Spell-check (it misses sound-alike errors and wrong-but-valid words); check citation and reference formatting; run plagiarism and permission checks; clear copyright for reused material.
5. **Stop conditions.** Stop when further changes would be cosmetic or would reduce precision. Do not stop while any of the 5 Cs fails.

## Output

Return the finished text by default. If a review is requested, also give a short account of the most important changes and any unresolved ambiguity.

## Guardrails

- Keep terminology consistent.
- Respect explicit length limits, but do not pursue brevity for its own sake.
- Preserve the author's voice and disciplinary conventions.
- Do not claim that linguistic checks prove comprehension.
- Do not use round-trip translation as an automatic editing step.

## Reference

Templates for more than 20 document types, extended word lists, sentence-level clarity examples, glossary construction, figure and permission guidance, international audiences, publishing and collaboration are in [reference.md](reference.md).
