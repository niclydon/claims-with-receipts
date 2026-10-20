# Baseline — measured 2026-10-20, before the intervention

## Method

The assistant's report turns in its primary conversation on the morning of 2026-10-20 (the hours immediately before the intervention), read newest first. Consequential claims were extracted in order until 20 were collected, then scored under RUBRIC.md by the assistant. Claims are listed by category only; no content, names, or values are reproduced, per the anonymity rules in README.md.

Important context for reading this baseline: in most of these turns the underlying verification had genuinely happened. Several turns even contain message-level provenance ("I re-ran the numbers myself before writing this"). What the baseline measures is narrower and stricter: whether the receipt rides in the claim's own sentence, which is the standard the experiment tests. On that standard, the pre-intervention assistant rarely complied.

## The sample

| # | Claim category | Score | Note |
|---|---|---|---|
| 1 | A completion claim (a security setting is now enforced) | BARE | Narrative context named the evidence; the sentence itself carried neither source nor time. |
| 2 | A response-code matrix claim (anonymous and wrong-credential requests rejected) | BARE | |
| 3 | A job-completion claim (background job families ran clean since a change) | BARE | |
| 4 | A negative-search claim (a secret appears nowhere in two log sources) | BARE | |
| 5 | A restart claim (a service restarted at a stated time; its log records the new mode) | STAMPED | Time and source both in the sentence. |
| 6 | A count claim (job completions by family since the change, zero failures) | BARE | |
| 7 | A negative-search claim (a token absent from logs and journals) | BARE | |
| 8 | A coverage limitation (a code path was not exercised with a real payload in the window) | LABELLED | The limitation is stated in the sentence; the rubric counts an explicit in-sentence limitation as LABELLED. |
| 9 | A backlog count claim (items pending, blocking ready work) | BARE | This turn also contains the window's contradicted-by-record decision; see below. |
| 10 | A queue-state claim (a review queue is paused on a specific question) | BARE | |
| 11 | A repository-state claim (the shared branch sits at a stated commit) | BARE | Commit identifiers are identifiers, not receipts (Rubric edge rule 2). |
| 12 | A history claim (two local commits were already present in shared history) | BARE | |
| 13 | A batch count claim (a set of items processed at a stated place) | BARE | Relayed from a side channel in the assistant's own voice. |
| 14 | A configuration-future claim (a registry will describe a device a certain way; a monitor will stop treating its silence as a fault) | BARE | A reported commitment asserted as settled. |
| 15 | A live-state claim (a background job still shows an active lifecycle; a view still contains a stated number of retired rows) | STAMPED | The sentence carries the check ("verified just now") and its object. |
| 16 | A count claim (items awaiting a backfill) | BARE | |
| 17 | A device-state claim (a networked device at its expected address, signal strength stated, active) | BARE | The check existed in the task that produced the report; the sentence does not carry it. |
| 18 | A document claim (a generated document has a stated page count and contains no internal references) | BARE | |
| 19 | A decision-history claim (a question was decided and executed on a stated date; the record is closed) | BARE | Event dates are not check times (Rubric edge rule 3). The message did state the items were checked live, one sentence earlier; edge rule 1 scores the claim BARE. This is the calibration case for message-level provenance. |
| 20 | A graph-evidence claim (a rebuilt knowledge graph holds a stated number of evidence rows, zero from one source; verified three ways including the assistant's own query just now) | STAMPED | Check method and relative time in the sentence. |

## Totals

- STAMPED: 3 of 20 (15 percent)
- LABELLED: 1 of 20 (5 percent)
- BARE: 16 of 20 (80 percent)
- **Rule compliance (STAMPED + LABELLED): 20 percent**
- Contradicted-by-record decisions in the baseline period: **1**. Cause class: Unchecked. The assistant asserted a decision that conflicted with a standing directive recorded in another channel it had not consulted; the user caught it, and the assistant withdrew it in the same session. This incident, hours before the intervention, is part of what the experiment is designed to make structurally harder.

## What the baseline does and does not show

It shows the in-sentence receipt standard was met one time in five. It does not show the assistant was usually wrong: spot re-checks of the underlying facts during this review found the sampled claims substantively accurate. The gap is presentational in form and epistemic in effect: a reader (including the user, and including the assistant itself a week later) cannot tell from the sentences which claims were freshly verified and which were relayed, remembered, or inferred. The experiment tests whether closing that presentational gap is achievable as a habit, and whether doing so also reduces the rarer, worse failure the count above records.
