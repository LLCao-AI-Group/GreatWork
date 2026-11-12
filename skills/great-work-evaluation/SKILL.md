---
name: great-work-evaluation
description: Evaluate a research, product or start-up proposal (or an early experiment report) against Paul Graham's "How to Do Great Work" standard. Scores five dimensions on a -1 / 0 / +1 scale (true and new, honesty and rigor, generality, quality of the question, first step and value of failure), searches for the closest existing work, checks the strongest simple baseline, and fact-checks the author's own answers on scope, curiosity and "why you". Use this skill whenever someone asks to review, score, critique or get feedback on a proposal, project idea, paper plan, grant draft or early report, asks whether an idea is novel or worth pursuing, or mentions "great work", even if they do not name the skill.
---

# Great Work Evaluation

Give an author specific, honest feedback on a proposal, measured against Paul Graham's essay *How to Do Great Work* (https://paulgraham.com/greatwork.html). His working definition: great work means doing something important so well that you expand people's ideas of what is possible. The essay covers research, products and start-ups alike, and so does this skill.

## What this skill does and does not decide

A proposal is judged on eight dimensions in two groups.

- **The author's three questions belong to the author and their advisor.** They are scope and ambition, curiosity, and "why you". These ask whether the direction and the person are worth a bet. A document rarely shows them, so the author answers each in one or two sentences at the top of the proposal. The three form a hierarchy: each only matters if the one before it holds, a clear failure at any level stops the project, and at least one must stand out. That decision is made by the author together with their advisor. Do not score these three and do not give an overall go / no-go verdict.
- **The five feedback dimensions are yours.** They are: true and new; honesty and rigor; generality; the question; first step and the value of failure. Score each one and give feedback the author can act on.

You also **fact-check the author's three answers**. You read the whole document and search the literature, so you can see things the author cannot, such as a paper published last month that already does the same thing. Report what you find and leave the judgment to people.

The reader is the author, and often their advisor. Write for someone who wants to know what to do next. Give clear judgments with evidence. Polite, balanced-sounding filler helps nobody.

## Inputs

- **The proposal.** A file path, pasted text, or a link. Read all of it, including tables, setup sections and appendices. Flaws tend to sit in the setup.
- **The author's top section**, if present: one paragraph on the project, then answers on scope and ambition, curiosity, and why you. If it is missing, say so, skip the fact-check, and suggest the author add it.
- **Reference material**, if the user supplies any. Treat it as a point of comparison for you, not as a list the proposal should have cited.

## Before scoring: three preparation steps

These steps decide the quality of everything that follows. Most of the useful findings come from them.

### 1. Restate the core idea in one plain sentence

Strip every acronym and fashionable term and say what the proposal actually claims. New names make old ideas look new. Once the names are gone you can see what the idea is, and you can search for it.

### 2. Find the closest existing work yourself

Do not rely on the proposal's reference list. Authors tend to cite the last two years of a hot topic. Search with your plain-sentence restatement and look for two things in particular:

- **The oldest ancestor of the idea.** It may be ten or twenty years old, in another subfield, under another name.
- **Other teams (or companies) doing the same thing now**, and how far ahead they are.

List the 3–5 closest items. For each, say in one sentence what the proposal adds or lacks relative to it. "Nothing" is a valid and common answer. Give each item's date and whether it came before or after the proposal was written.

Existing work is used only for comparison. What matters is whether the idea is true and new relative to what exists, not whether the reference list is complete. A missing citation is not a fault in itself. If a prior work already covers the core idea, the problem is "the idea is not new", not "you did not cite it".

State how well you verified each item: read the paper, read only the abstract or a search snippet, or recalled from memory without checking. If you cannot search, say plainly that the list is from memory and unverified. Never imply a check you did not do.

Check the proposal's own citations and sort them into three lists: not findable; findable but the content does not match how the proposal describes it (the most serious kind); findable and consistent. List coined terms and acronyms that have no source. Mark vendor-reported numbers that nobody has reproduced. If there are too many citations to check, check the ones that carry the core claims and mark the rest "not verified".

Keep the author's name, institution and other personal details out of search queries. Search on the technical ideas only.

### 3. Find the strongest simple baseline

Ask: in this proposal's own setting, is there an answer that needs no new method at all? If so, the proposed method has to beat it before it means anything. Three concrete checks:

- Does the information the method already uses (labels, for example) make the target quantity directly computable?
- Do the success examples actually show what the proposal says they show? A proposal may claim to find hard cases while its showcase example is an easy one.
- Does the randomness in an experiment come from a distribution that is already known? If so, the result can be computed exactly and the sampling only adds noise.

If the proposal contains numbers, recompute the key ones. If it has no experimental numbers of its own, check three things instead: whether quoted numbers are accurate; whether its own estimates (cost, latency, time) are internally consistent; and whether the planned evaluation set is large enough to separate the expected gain from noise.

For a product or start-up proposal, the same three steps apply: the "closest existing work" includes products and companies, and the "simple baseline" is what users do today without the product.

## The five dimensions

Score each dimension on three levels and quote **evidence from the proposal's own text**.

- **−1** — a problem that must be fixed. Pair every −1 with a specific suggestion.
- **0** — no serious flaw and no highlight. The level of a competent, ordinary paper.
- **+1** — done well even by the standard of the best work. Say what is good about it.

Most dimensions of most proposals are 0. Give −1 or +1 only with concrete evidence. If the text gives no basis for a judgment, write "insufficient evidence" and do not guess.

A proposal written before any experiment has been run cannot yet show that its claims hold. Score that as "insufficient evidence", not −1, and say which experiment would settle it. Missing evidence is normal at that stage. Keep −1 for things that are wrong on the page: a core idea that existing work already covers, estimates that contradict each other, a source described incorrectly, or a conclusion stated as settled when nothing supports it.

Refer to the dimensions by name, never by number. The sections of your output are numbered, and dimension numbers would be confused with them.

A dimension gets one score even when it covers several things. When the parts differ, say so in the reason. For example, under "true and new" state separately whether the idea is new and whether the claims hold, since the fixes are different.

These scores are feedback. They are not summed or averaged, and they are not an overall verdict.

### True and new

Compare the core idea with the work you found. Compare the idea itself, regardless of whom the proposal cites.

- **Is the gap real?** Has nobody done this, or has somebody? Can the author say precisely what everyone else overlooks? If not, the claim reduces to "they don't get it".
- **New.** What exactly is new relative to the closest work: a new question or viewpoint, or a change of dataset, modality or one module?
- **True.** Does the core claim hold? Check whether the setup makes the problem trivial, whether the evidence supports the conclusion, whether the evaluation can separate success from noise, and whether the method beats the strongest simple baseline from step 3. If there are no experiments yet, this part is "insufficient evidence".
- Graham's test: a good idea tends to look both novel and obvious. Be wary of an idea that only looks new because it is complicated.

### Honesty and rigor

Graham doubts that great work is possible without intellectual honesty, because there is no margin for self-deception.

- Are unfavourable results, limits and failure cases reported?
- Do the conclusions match the evidence? Read the headline claims in the title and abstract, not only the body.
- Does the proposal say what result would prove it wrong?
- Is the author stricter than others: do they follow up the things that look slightly off, or step around them?

### Generality

Great work is often tool-like: others build on it.

- Does the core idea hold apart from one specific model, dataset or checkpoint?
- Can it be said in one sentence or one formula? Is it a derived principle, or a set of thresholds found by trial?
- Once it works, does it expose new questions that others can go on to answer?

### The question

Graham observes that the insight in a big idea is often in the question, not the answer. The other dimensions judge the answer. This one judges the question.

- Is the question specific enough to be answered wrong? What result would show the idea is mistaken?
- Could the answer surprise the author? A question of the form "how can we build X" can only end in "we built it". A question about how something works can end in a discovery.
- Does answering it lead to a larger question? The best questions grow in the answering.

When this dimension is weak, propose a sharper version of the question. That is usually the single most useful piece of feedback, because a better question changes everything downstream.

### First step and the value of failure

Graham's advice is to begin with the simplest thing that could possibly work and then make successive versions.

- What is the smallest first version that gives a result in a week or two?
- Which result means continue, and which means change direction?
- If the project fails in the end, what is left: data, a tool, a negative result worth knowing, a better question?

High risk is good when the expected value is high. It is a problem when failure leaves nothing behind. If the proposal has no small first step, design one and write it down.

If the document is a report on a first step already taken, judge two things instead: whether that step was small and informative, and whether the next step is equally small, with a stated result that would mean stopping.

## Fact-check of the author's three answers

Do not score these. For each answer, give one of three findings with evidence:

- **Supported** — the proposal or the facts you found back the statement.
- **Contradicted** — say where. The most important case is scope: if the author writes that nobody has done this, or that others cannot go around the result, and you found work that covers the core idea, name the work and its date. The advisor needs this more than anything else in the review.
- **Cannot tell from the document** — for example "I have wanted to know this for years". Say so plainly and do not guess.

Useful things to check:

- **Scope:** whether the result would be one more paper or something others cannot go around depends on existing work and other teams. Compare the answer with your search results.
- **Curiosity:** if the answer mentions a surprise or a failure the author chased, does the proposal contain it?
- **Why you:** do the stated advantages (data, tools, first results) appear in the proposal? Do the stated resource needs match the plan?

If the document reads mostly as the output of a search tool or an AI survey, say so. Such a text reflects the tool more than the author, and the three answers then need confirming in person.

## Output format

Write in the language the user is writing in. Be brief and lead with findings. The main body should take about five minutes to read. Long verification lists go in the appendix.

1. **Core idea in one plain sentence.**
2. **Closest existing work** — 3–5 items; what the proposal adds or lacks relative to each; date; how well you verified it.
3. **Scores** — a table of the five dimensions, listed by name, with the level (−1 / 0 / +1 / insufficient evidence), a one-sentence reason, and the evidence from the text.
4. **What must be fixed** — one entry per problem, labelled with the name of its dimension; a dimension scored −1 may have several. Mark each as *fixable* (an experimental flaw, thin evidence, a missing baseline, no closed loop) or *not fixable without changing the idea* (the core idea is already covered, the problem is too small), and say concretely what to do. For recomputed numbers, say here only whether they matched and name any that did not or could not be recomputed; the detail goes in the appendix.
5. **What is done well** — one entry per +1. If there is none, say so.
6. **The thread most worth keeping** — the part of the proposal most likely to grow into something new, if any. If the core idea does not hold, this is where to describe the way out.
7. **Fact-check of the three answers** — supported / contradicted / cannot tell, with evidence. If the proposal has no top section with the three answers, keep this heading, say the section is missing, and ask the author to add it.
8. **The one next step** — the single most important thing to do, small enough to start this week.
9. **Appendix** — the three citation lists, the recomputation detail, and other verification notes.

Do not give an overall recommendation. Do not invent strengths or weaknesses for the sake of balance. If a finding is negative, state it directly, and then say what the author can do about it.
