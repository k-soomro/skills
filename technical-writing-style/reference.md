# Technical Writing Style — Reference

Heavy reference for [SKILL.md](SKILL.md): compact document templates, extended word lists, worked clarity examples and domain guidance. Distilled from Phillip A. Laplante, *Technical Writing: A Practical Guide for Engineers, Scientists, and Nontechnical Professionals* (CRC Press), with reader-centred editing practice.

---

## 1. Document Templates

### Technical report (overview / product survey / trend forecast)
1. Introduction: technology history and context. 2. Body: numbered lines of research, product innovations or a taxonomy with gaps. 3. Per line: current state plus a few relevant references. 4. Comprehensive conclusion. 5. Short glossary. (A primer: you organise the state of affairs; no invention is required.)

### Tutorial / primer / user manual
Textbook-excerpt feel: narrative + figure + table; no long runs of sentences. State the reader-assumption level explicitly (failure modes: over-explaining versus skipping "obvious" details). Use more reviewers than for other document types.

### Experimentation-based report (5 steps)
1. Background and need. 2. Methodology: exact versions, build settings and hardware. 3. Results (graphs and tables; introduce every table in the text before showing it). 4. Interpretation. 5. Recommendations and conclusions. **Include enough detail for someone else to repeat the experiment.** Express algorithms in **pseudocode**, never in a specific language.

### Survey-of-the-field research report (for experts)
Organise by research questions, historical trends or taxonomy — not dry paper-by-paper summaries. Gap analysis: ① cluster papers into a taxonomy → ② analyse the distribution → ③ propose research for the quantified gaps ("8% compression, <1% remote sensing").

### Survey-based report
1. Need and context. 2. Administration (URL, question count, invitations, reminders, population). 3. Questions in a table. 4. Response statistics (invited versus completed; cut-off policy). 5. Results charts, each labelled with the respondent count ("n = 191").

### Journal/conference paper review (8 points; ① and ⑧ mandatory)
1. Hook in the first sentence. 2. Context: why the work matters and how it fits related work. 3. Salient findings. 4. Shortcomings and improvements. 5. Future research areas. 6. Who benefits (researcher, practitioner, novice, expert). 7. Further reading. 8. Final assessment. Quick test: What is the conclusion? Is it so (supported)? So what (significant)?

### Book review
Theme-led narrative, not a chapter-by-chapter litany. Highlight a few chapters, not all. No platitudes, trivia or per-section template paragraphs ("In section x…").

### Incident/accident/outage report
Point of view: see [SKILL.md](SKILL.md) (Inputs, audience and register). Sequence: date and time with time zone → factual sequence → observable outcomes → no cause speculation and no blame. Write for the most formal reader who may see it (regulators, lawyers).

### Requirements/spec fragment
One numbered statement per requirement; apply the precision and testability rules in [SKILL.md](SKILL.md); track changes with sources and dates.

### Procedure / runbook / recipe (base pattern)
name → serves/scope → purpose → safety information → preconditions → performer qualifications → materials list → tools → numbered single-action steps → postconditions → troubleshooting → FAQ. Materials list: items first, then details per item (not detail-all-at-once). Order steps by immediacy; handle variations explicitly ("if multiple attackers…, if a weapon…").

### User manual
Cover → quick-start guide → table of contents → list of figures → installation/assembly → features (each described in detail) → maintenance → FAQ → troubleshooting → contact information → glossary.

### Bug / problem report
Problem name · product ID · detailed description · date discovered · who discovered · **conditions under which it occurred** · **expected results** · **actual results** · severity · contact. Consistent terminology is critical: duplicates and mislabels prevent maintainers from recognising them. (Careful reports often reveal that the "bug" was your own misunderstanding — write it before filing.)

### Grant / R&D proposal
Title → Problem Statement (cite evidence) → Hypotheses/Objective → Scope and Limitations (exclusions explicit) → Definition of Terms → Abbreviations → Background → **Uniqueness of the Research (most important)** → Potential Contribution → Direct Application → Technology Transfer → Methods and Procedures (phased) → **Success Criteria (measurable)** → Team Qualifications → Deliverables/Schedule → Estimated Cost (best case, worst case and contingency) → Other Funding → References. **Proposals are commitments and legal documents.** Do not overstate ability; winning work you cannot deliver is the worst outcome.

### Consulting proposal (numbered clauses)
Preamble → Deliverables (with dates) → Client Obligations (facilities, documents, personnel, insurance) → Consultant Obligations → Payment Terms (amount, timing, method, early/late terms) → Changes/Cancellation → Interpretation (entire agreement, governing law, arbitration).

### Strategic plan / roadmap
**Executive summary (write last)** → Mission statement (a compact decision guidepost: "How does this activity serve the mission?" Develop it BEFORE planning and do not reopen it mid-planning) → SWOT (2×2: internal/external × positive/negative; bullets elaborated in narrative) → Competitive market analysis → **Mission —→ Goals (broad, enduring) —→ Objectives (measurable) —→ Strategies** (mission-consistent, actionable, measurable, persistent, embraceable, each with a metric) → Appendix: performance indicators and budget.

### Memo
`To / From / Date / Subject` → purpose → details and tables → summary plus the actions you will take. The subject line should be a memorable handle for the topic.

### Meeting invitation / agenda / minutes
Invitation: purpose, participant's role, where and when, logistics, why this recipient, call to action and response deadline. Agenda: topics with a **lead person and time allotted** for each. Minutes: attendees, per-topic summaries, action items **by owner**, adjournment; use the agenda as an outline; **send a draft to all attendees before general distribution**.

### Press release
Persuasive title, concise news description, official point of contact. **Neutral tone** — anything that reads like advertising gets discarded.

### Presentation / slide content
Minimal text, more graphics; slides are a contextual map, never a copy of the speech; detail lives in speaker notes. Revision passes: verbose → succinct bullets → pictorial layouts with icons. Track the slide-to-time ratio (about 3 minutes per slide); size the deck to the slot.

### Résumé / CV / capability statement
One page ideal, two maximum. Reverse chronological, action verbs, *your specific contribution* ("Wrote software acceptance test scripts and conducted acceptance testing for…", not "Part of a team that developed…"). Include a summary only if it differentiates you. Lead with education (little experience) or experience (no degree). No GPA, hobbies, photos, humour, gimmicks or "References available upon request". Echo the audience's stated requirements with evidence, never with parroted adjectives.

### Letter of reference / endorsement
(1) Who you are and why you are writing. (2) How you know the candidate and for how long. (3) Strengths AND weaknesses. (4) Suitability for THIS job. (5) Summary recommendation. Customised beats generic ("Dear Mr Jones" beats "To Whom It May Concern"). **Rule of silence: the absence of positive comment on an attribute is equivocation** — anything less than glowing reads as lukewarm. If you do not know the candidate well enough, decline.

### Transmittal / cover letter
State the purpose briefly ("Please find attached X in response to Y") → why you fit → call to action → thank-you. No embellishments, no gimmicks.

### E-mail
Keywords in the subject line · one screen · call to action with a deadline · plain language · "urgent" and receipt confirmation used sparingly · no emoticons in official communication (if you need one to soften a message, fix the message).

### Online course / tutorial site
Adult learners: assume motivation and independence, but still write simply. High structure and navigation; interaction and feedback loops; a short assessment per module (1–2 learning checks); graphics, videos and simulations over recorded lectures; distil into very short bites; expect low completion.

### Vignette: non-technical versus technical register (same accident)
❌ "This idiot runs a stop sign and T-bones my car… Stupid jerk was probably drunk…"
✅ "On 1 October 2017 at approximately 10 AM, Driver A was proceeding on Valley Road… Driver B proceeded through the stop sign…, colliding with the passenger side of Driver A's vehicle. The driver's airbag deployed. There were no injuries. Driver A's vehicle needed to be towed."

---

## 1b. Glossary Construction

- Short glossaries: a `Term | Definition` table; longer ones: `Term: one-sentence definition.` entries, alphabetical.
- Gloss any word unfamiliar to someone *outside your specialty*; when unsure, gloss it.
- Every glossary-defined term that itself uses jargon needs its own entry. Define noun and verb forms separately where both are used (interface/interfacing); use "see" and "see also" cross-references; resist embedding a dictionary.
- Example entry: "Binary search: A divide-and-conquer technique in which the range of the search is halved each time."

---

## 1c. Sentence-Level Clarity: Worked Examples

The rules are in [SKILL.md](SKILL.md) (Comprehension). These examples show the revision moves in practice.

### Subject–verb gap
❌ "The validation routine, which runs after every import and which checks each field against the schema defined by the data team, rejects malformed records."
✅ "The validation routine rejects malformed records. It runs after every import and checks each field against the schema defined by the data team."

### Noun string
❌ "Update the user account permission validation routine."
✅ "Update the routine that validates permissions for user accounts."

### Omitted connective
❌ "The sample was heated. The pressure rose."
✅ "The pressure rose when the sample was heated." (or "because the sample was heated", if causation is the point)

### Overloaded sentence
❌ "The controller logs the fault, restarts the service and notifies the operator, which reduces downtime but can also mask intermittent failures unless the log is reviewed daily."
✅ "The controller logs the fault, restarts the service and notifies the operator. This sequence reduces downtime, but it can mask intermittent failures unless the log is reviewed daily."

### Improvised verb
❌ "The team leveraged the data to action the findings."
✅ "The team used the data to act on the findings."

### Worked example: preserving qualifications and scope
Source: "The prototype reduced average latency by about 30% in our tests, although the result was not statistically significant and did not hold under peak load."

A faithful revision keeps four things: the **claim** (about 30% reduction), the **qualification** (not statistically significant), the **scope** (average latency, in our tests), and the **exception** (did not hold under peak load). A revision that drops "not statistically significant" or "under peak load" is a factual change, not an edit.

---

## 2. Extended Word Lists

### Concise replacements
a substantial amount of redesign → substantial redesign · available out there → available · fire up the engine → start the engine · go along with each unit → accompany each unit · many fold → numerous · put off by → unimpressed by · really strong odour → powerful odour · software tie-in → software connection · tying in together → attaching · stretched thin → overextended · on the fly → contemporaneously · write down → record · day to day → ordinary · came out → appeared · comprised of → comprise · which may not integrate according to expectations → that might not integrate as expected · "This situation is entirely due to the lack of X" → "because the industry lacks X".

### Malapropisms to hunt
beets/beat · contingency/contingent · costumers/customers · destiny/density · eros/errors · etymology/entomology · examples/samples · floundered/foundered · ingratiate/integrate · object-orientated/object-oriented · spoon/spawn · typing point/tipping point · wretched set/ratchet set.

### Heterographs (sound-alike, spell-check-proof)
compliment/complement · course/coarse · facts/fax · fourth/forth · hire/higher · hole/whole · knew/new · real/reel · sheer/shear · their/there/they're · two/too/to · its/it's · discrete/discreet · principal/principle.

### "Very" replacements
very clear → transparent · very loud → deafening · very new → pristine · very often → frequently · very old → ancient · very quiet → muted · very strong → mighty · very weak → feeble · very fast → sudden · very simple → basic · very small → tiny · very large → enormous · very heavy → weighty · very clean → spotless.

### Clichés → plain meaning
bite the bullet → sacrifice · in this day and age → today · ins and outs / nitty gritty → details · only time will tell → eventually · no mean feat → difficult · drop in the bucket → tiny · feather in your cap → accolade · whets the appetite → invites.

### Filler to delete outright
as a matter of fact · for what it is worth · all in all · that being said · in fact · that, in itself · I personally think that.

### British/US dialect pairs
metre/meter · colour/color · stabilise/stabilize · different from (UK)/different than (US) · aerial/airplane · trolley/cart · mobile phone/cell phone · defence/defense · lift/elevator · expiry date/expiration date · torch/flashlight · petrol/gas · earth wire/ground wire · maths/math · programme/program · spanner/wrench. Beware same-word-different-meaning ("rubber").

---

## 3. Figures, Tables, Equations, Dynamic Content

- Diagrams beat prose for complex **behaviour** (state machines, flowcharts), but only if the reader has the domain knowledge; stipulate symbols and conventions before the diagram.
- Research: papers gain about two citations per diagram; equations and photos slightly *reduce* citations. Diagrams illustrating an original idea beat quantitative dump-figures.
- A caption must state the encoding and cite data sources even for a figure you drew yourself (Minard's map: line width = troop count; the caption states the encoding and sources).
- Permissions: an original figure is yours; a copyrighted figure reused needs permission plus the required credit line; a substantially redrawn figure needs a citation, not permission; public domain is jurisdiction-dependent, so verify before publishing; your own published figures may have transferred copyright.
- Dynamic content: embed video or animation electronically, or link a hosted simulation with a pointer figure.
- Ambiguity worked example (car manual): "three consecutive error-free cold starts… followed by several minutes of either highway or city driving" is uninterpretable. Spell out exact sequences, counts and conditions.
- Ambiguity worked example (smart-home spec, exposed by "How do I test this?"): "record any show" (anywhere? pay-per-view?) · "make storage expandable" (how much?) · "provide search feature" (by name? time?) · "store X episodes" (natural number? integer?).

---

## 4. Plagiarism & Permissions (six rules)

1. Verbatim text → cite AND set it off (quotes, font change or indentation). 2. Any idea from a source → cite it, even if reworded substantially. 3. Large text portions (about 50–200 words) in commercial works → written permission. 4. Your own previously transferred work → permission, unless the agreement grants reuse. 5. Unaltered figures → cite; commercial use → permission. 6. Redrawn figures → cite. Permission exists only when written confirmation arrives: silence means no. Quoting copyrighted poetry or lyrics always requires permission, no matter how short.

**Self-plagiarism:** never reuse your own prior work without attribution. Cite it so reviewers can tell new material from repurposed material. After copyright transfer, request permission; for co-authored material, obtain permission and acknowledge co-authors; when in doubt, cite.

**Detection:** repository and web-crawl matching AND style fingerprinting (Flesch–Kincaid: words per sentence, syllables per word). A sudden metric shift between paragraphs signals pasted text, so keep style metrics uniform across sections. Plagiarised sources often plagiarise others: never assume your source was original. Run a detection check before submitting to any supervisor, client or publication. Never use paper generators; as a reviewer, grammatical but nonsensical text means rejection — verify substance, not structure. Flag every pasted fragment in a draft and verify attribution at publication.

Permission request skeleton: identify your work, publisher and date → list exactly what will be reused → describe how it will be used → ask what else is needed → thank the representative.

---

## 5. International & Cultural Audiences

- Hofstede's six dimensions (power distance, individualism, masculinity index, uncertainty avoidance, long-term orientation, indulgence): a high power-distance audience means never write something that could embarrass a superior. Consult country metrics before writing for a specific country.
- Verify domain terminology across domains (to a courier, a "truck" is a long-haul vehicle; the delivery van is a "package car").
- Use simple language and a glossary for mixed or novice audiences (the home medical device pattern).

---

## 6. Publishing, Reviews, Rejection

- Match the material to the venue FIRST: the wrong venue guarantees rejection. Archival, long-lived content belongs in slow peer-reviewed venues (months to two or more years); fast-moving content belongs in fast venues (magazines, newsletters, blogs) or it is stale on arrival. Conferences sit in between.
- Administrative rejection: out of scope, writing too poor to review, length out of specification, obviously poor quality. Expect editorial advice and possibly an invitation to resubmit.
- Formal review: editor-in-chief → two to five reviewers → two to eighteen months → accept / minor changes / major changes / rewrite and resubmit / reject.
- Handling rejection: thank the reviewers politely, mine the reviews for fixes, improve the work and resubmit elsewhere. Never reply angrily or defensively: communities are small, and civility buys goodwill. Persistence beats talent (Carrie was rejected 30 times, Gone with the Wind 38 times, Harry Potter 9 times). Diagnose repeated rejections honestly: poor writing, an incomplete prior-work analysis or insufficient data are your fault. About 20% of papers never find a home, so know when to cut losses.
- Succeeding: volunteer to review (you learn what the venue wants), keep multiple works in the pipeline, seek a unique contribution, and remember that editors reject good research that is badly written.
- Open access models: Green (self-archived after embargo), Gold (author pays an article processing charge of about $1–2k) and Hybrid. Vanity press: the author pays $5–10k and the quality bar is low; online self-publishing is easy, but marketing is the hard problem.

---

## 7. Collaborative Writing

- Collaboration cost grows as n(n−1)/2: manage egos and share credit.
- Homogenisation: multi-author documents read as multiple voices. Measure Flesch–Kincaid per section, investigate dramatic shifts, and edit until section statistics are similar (within about 20%). Use circular revision (each author takes a full-document pass) or a unified pass by a non-author.
- **One co-author must hold final authority.** Democratic editing invites stalemate.
- Author order reflects actual contribution, never rank or alphabetical tricks.
- Large contributed works: partition into areas with an area editor each → terms list → definitions → cross-check within areas → cross-check across areas → compile → review → final proofread.
- Tuckman: forming → storming → norming → performing. Teams do not automatically reach performing.

---

## 8. Writer's Block (for long-form projects)

Write something daily · schedule and honour writing sessions · alternate writing and editing · shelve the stuck section and work where progress is possible · read unrelated material, then return · exercise · remove distractions · change environment. Being blocked is not being broken. Always impose a completion goal even when nobody else does. Ship at "good enough and verified", not "perfect".
