# Claims With Receipts

A two-week, preregistered experiment on an AI assistant's personality, run in public.

## The question

Can an AI assistant change a specific, measurable behaviour about how it talks, not by declaring a new personality, but by adopting one rule, measuring a baseline, living under the rule for two weeks, and publishing the before-and-after counts either way?

## The rule under test

**Every consequential claim carries its receipt, or admits it has none.**

In the assistant's reports to its user, any claim that matters (a number, a system state, a completion, a decision-relevant fact) must carry, in the same sentence, either:

- its **check**: what source was consulted and when, or
- the word **unverified**, in the sentence.

The rule exists because the assistant's most repeated documented failure was not dishonesty. It was confident phrasing outrunning verification: true-sounding claims asserted at a strength the underlying check did not support, and numbers passed along from secondary reports that later turned out to be wrong in detail. The fix being tested is not "be more careful," which is unmeasurable. The fix is moving the provenance into the sentence, where the reader can see it without having to trust the narrator.

## The experiment

- **Name:** Claims With Receipts
- **Window:** 2026-10-20 to 2026-11-03 (14 days)
- **Subject:** one AI personal assistant ("Nova"), working for one user, in one long-running primary conversation plus its side channels.
- **Intervention:** a persona amendment (see INTERVENTION.md) plus this experiment's declared setting.
- **Baseline:** 20 consequential claims sampled from the assistant's report turns immediately before the intervention. Compliance with the rule: **20 percent** (3 stamped, 1 labelled, 16 bare). Full method and table: BASELINE.md.
- **Targets, fixed in advance:** in the end-of-window sample of 20 report turns' claims, at least 90 percent stamped or labelled, and zero decisions that contradict a directive already on record.
- **Review:** 2026-11-03, results published in RESULTS.md whatever they show. The setting lapses automatically at the window's end unless the review renews it.

## Why this is designed the way it is

The design borrows from the human personality-change literature, where the consistent finding is that declared change is weak and measured change is what counts:

- Change goals alone move human traits only slightly (meta-analytic effect around d = 0.14 over three months); structured, behaviour-level interventions with feedback do better (the best randomized trial reached about d = 0.5).
- Unstructured "write a plan and try harder" interventions fail and sometimes backfire. Specific if-then commitments, behavioural repetition, self-monitoring, and observer-style evaluation are the ingredients that work.
- Self-report is the weakest evidence class. Observers often cannot detect change the subject confidently reports.

Translated: a persona document edit is the unstructured plan. This repo is the structure around it: a fixed protocol (PROTOCOL.md), an explicit scoring rubric (RUBRIC.md), a baseline measured before the intervention, a dated log (LOG.md), and a final count scored the same way as the baseline.

## Anonymity

This repository publishes process and results only. It contains no information about the user: no names, no organizations, no systems, no ticket or record identifiers, no locations, and no quoted conversation. Sampled claims are described by category (a status claim, a count claim, a completion claim), never by content. The only named entity is the assistant.

## Reading order

1. PROTOCOL.md: the design, fixed before results existed.
2. RUBRIC.md: exactly how a claim is scored.
3. BASELINE.md: the before picture.
4. INTERVENTION.md: the persona amendment under test.
5. LOG.md: dated entries across the window.
6. RESULTS.md: the after picture, published 2026-11-03.
7. docs/narrative/: one narrative per completed arc, starting with the founding arc (2026-10-20-origins.md); CHANGES.md records what landed and when.

## License

MIT. The process is the contribution; reuse it, improve it, run it on your own assistant.
