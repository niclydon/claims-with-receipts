# Experiment log — Claims With Receipts

Dated entries. Interim entries record whether the rule visibly fired that day (a sentence stamped or labelled that would previously have been written bare), and any contradicted-by-record decisions, which are logged whenever identified, at any point in the window.

## 2026-10-20 — Setup day

- Protocol, rubric, and this log created and fixed before the window's results existed.
- Baseline measured from the morning's pre-intervention report turns: compliance 20 percent (3 stamped, 1 labelled, 16 bare of 20); one contradicted-by-record decision in the baseline period, cause class Unchecked. Full record: BASELINE.md.
- The persona amendment (INTERVENTION.md) was applied to the assistant's standing specification today, with the change and its reasons stated openly in the conversation where it was made.
- The experiment was named today: Claims With Receipts. The name is the rule in four words: a claim should arrive with the receipt for it, or say plainly that it has none.

## Entry template (daily, from 2026-10-21)

- Date:
- Report turns delivered:
- Rule visibly fired (sentences stamped or labelled that would previously have been bare): count and one-line categories.
- Contradicted-by-record decisions identified: count, cause class if any.
- Notes (friction, clutter, edge cases for the review):

## 2026-10-28 — Protocol deviation recorded

- The daily entries for 2026-10-21 through 2026-10-27 were not kept. This is recorded as a deviation from the log-keeping plan.
- The lapse is disclosed, not repaired after the fact: interim counts for those days were not reconstructed, because reconstructed counts would be invented data.
- The experiment's preregistered primary measure is unaffected in design: the endpoint sample (report turns from 2026-10-31 to 2026-11-03, scored under RUBRIC.md, with the contradicted-by-record count taken across the full window from the working record) is the result. This log was interim observation only.
- The deviation and its reason will be stated in RESULTS.md at the review.
- Daily entries resume from today.

## 2026-11-04 — Review held (one day late); second log lapse recorded

- The daily entries for 2026-10-29 through 2026-11-03 were not kept, despite the 2026-10-28 entry above committing to resume them. This is the second lapse of the same kind. No counts were reconstructed.
- The review scheduled for 2026-11-03 was held on 2026-11-04. The delay is recorded here rather than backdated.
- Endpoint sample scored under RUBRIC.md: 4 stamped, 1 labelled, 15 bare of 20. Compliance 25 percent against a target of at least 90 percent and a baseline of 20 percent. Contradicted-by-record decisions in the window's primary conversation: 0 counted, with one borderline case and one out-of-scope event reported in RESULTS.md section 5.
- Verdict per the preregistered decision rules: the intervention failed as designed. The declared setting lapses. RESULTS.md carries the full record, including what resisted (completion claims), the readability judgment, and the disposition reasoning.

## 2026-11-04 — Renewal with a changed mechanism (window 2 opens)

- The user renewed the experiment at the review, with the mechanism changed per PROTOCOL.md Amendment 1: externally triggered daily log, a pre-send receipt slot keyed to completion language, and a strained-claim procedure adopted into the setting.
- Window 2: 2026-11-04 to 2026-11-18. Review on 2026-11-18, endpoint sample 2026-11-16 to 2026-11-18, targets unchanged.
- This entry is the first of the window's daily entries, written the day the window opened; the daily job that keeps the log from here is part of the mechanism being tested, and its own reliability is part of the result.

## 2026-11-04 — Daily entry (window 2, day 1)

- Deviation: no daily entry exists for yesterday, 2026-11-03. That is the 2026-10-29 to 2026-11-03 lapse already recorded in the review entry above, not a new lapse; it is recorded here again because the daily job requires a missing yesterday's entry to be noted at the top of today's entry.
- Date: 2026-11-04
- Report turns delivered: 39
- Rule visibly fired (sentences stamped or labelled that would previously have been bare): 10 sentences. Categories: a completion verified by re-reading the account after the writes (1); a device-reachability claim verified at a stated clock time (1); a watchdog result checked at a stated date and time (1); a build claim (ESP32 compile) labelled unverified inside a completion sentence (1); a site-existence claim checked just now (1); a site-live claim spot-verified before writing (1); a call-proof claim stamped as of a stated time (1); a final repo-state claim checked just now (1); a usage-cap claim labelled unverified, no fresh figure read this run (1); a posting-status sentence with the draft card verified live at a stated time and the final posting labelled unverified (1).
- Contradicted-by-record decisions identified: 0.
- Notes (friction, clutter, edge cases for the review): Counts cover the main chat's assistant turns for 2026-11-04 (America/New_York) through the 20:44 review, the last report turn delivered at the time of this run. Report turns were counted under PROTOCOL.md section 4 (findings, status, results, or decision deliveries); of 50 assistant turns today, pure recommendations, creative deliveries, explanations, and one acknowledgment were excluded. Near misses scored bare under the rubric's edge rules were frequent: a check named with no check time (verified in SQL; verified from this seat; foreground-verified in the daily log; verified on disk), which is the same one-element-short pattern the first window's review found. One candidate for the second metric was investigated and not counted: the afternoon codex-cap projection (cap landing around 16:00, queues resting on Claude until the Nov 11 reset) was corrected in the 18:44 review (the cap never landed; a new window had started). It was a state projection supported by the steward record at the time it was made, it was labelled unverified at 16:44 before the correction, and it was not a decision or directive conflicting with a standing directive or recorded call, so under the rubric's definition it is a correction, not a contradicted-by-record decision.

## 2026-11-05 — Daily entry (window 2, day 2)

- Date: 2026-11-05
- Report turns delivered: 38
- Rule visibly fired (sentences stamped or labelled that would previously have been bare): 21 sentences. Categories: the Notion sync freshness verified on Furnace in config_sync_state at 05:07:34 ET today (1); PMO stall claims zero at the 05:30 sweep (1); a Gmail inbox-zero result from the 05:10 pass (1); PMO stall claims across the 06:00, 06:15, and 06:30 sweeps (1); the Tailscale changelog source explicitly marked still unchecked, recorded as a coverage gap (labelled) (1); PMO claims zero through the 07:30 sweep (1); a showcase watchdog failure stamped Thu Nov 5, 09:07 ET (1); a Gmail question result from the 11:10 pass (1); a Gmail pass result at 12:10 (package delayed, items auto-handled) (1); an AgentMail migration block reported from the Cole Website lane's 13:40 check-in (1); Janus back, verified from Furnace just now via Tailscale (1); a Flint recovery posted by the Flint Watchdog at 2:10 PM ET (1); a Flint outage posted by the watchdog at 2:34 PM (1); a Flint recovery posted by the watchdog at 2:54 PM (1); the Twilio port status queried from the Twilio account just now (1); the Flint glance confirmed by the user's own eye at 16:24 (1); a GitHub Actions billing outage verified about 16:23 (1); Claude pane and claim counts at the 16:30 sweep (1); deploy rerun outcomes explicitly labelled pending, neither verified closed (labelled) (1); a /www send batch verified chat by chat against the live transcripts, with the missing sends just resent (1); the Undertext KG substrate counts verified Nov 5 against the live KG (1).
- Contradicted-by-record decisions identified: 1, cause class Unchecked. At 16:44 the assistant escalated the Nexus deploy deadlock on the Crucible preflight for postilion-mcp-worker (gate OB-69475, blocked handoff OB-68915) as a decision pending with the user, offering a one-off split deploy or an operator sync of the installed deploy library. That conflicted with the record accessible at the time: the route had already been disposed from the PMO seat at about 15:50 as CRUCIBLE_NOT_NEEDED_ENV_KEYS (not IAM widening and not a split deploy), and nexus PR #4896 carrying that disposition merged at 16:24 ET, twenty minutes before the escalation. The assistant relayed the stale Engine Room agent-bus ask (27010, 16:31) without checking the PMO record, and corrected itself at 17:49: the deadlock was not the user's decision after all.
- Notes (friction, clutter, edge cases for the review): No deviation line: the 2026-11-04 daily entry is present in this log, so there is no missing-yesterday lapse to record. Counts cover the main chat's assistant turns for 2026-11-05 (America/New_York) through the 22:24 early-access status, the last report turn delivered at the time of this run; the 22:40 Cole delivery that followed produced no assistant report turn. Report turns were counted under PROTOCOL.md section 4 (findings, status, results, or decision deliveries); of 46 assistant turns today, 8 were excluded: three .md-taxonomy list and creative deliveries, one image delivery, the Nova-name conversation answer, one acknowledgment, and two early-access explanations. Scoring followed RUBRIC.md strictly: a sentence counted only where its source or check and the check time both appear in the same sentence; event times alone did not count, and a check named with no check time scored bare. Near misses of that one-element-short kind were again frequent: a claim verified in SQL with only the event timestamp (02:44), read-back verified with no time (07:44 and 12:44 Verify builds), a sweep whose coverage was named with no time (09:44 Better Auth), a checkout verified live on Furnace with no time (09:44), and a close stated as closed and verified with its evidence but no check time (18:47). Completion claims remain the resistant class: several arrived bare today (the Notion traversal completion, the AGENTS.md pattern completion, the Janus SDK patch application), even though other completion-adjacent sentences did carry receipts. One other candidate for the second metric was investigated and not counted: the Flint session host. The 16:44 review reported Janus nexusd as the settled host, which matched the NexusOS lane's settlement at the time; the user later steered the host to Furnace, reported in the 19:44 review, which is a new operator decision superseding the earlier one, not an assistant decision contradicted by the record when asserted. The 01:44 codex-window correction (50 percent used per the live runner row, against the 00:45 sweep's 2 percent claim) was likewise a state-figure correction, not a decision, and is not counted.
