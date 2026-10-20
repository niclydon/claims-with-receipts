# Scoring rubric

Applied identically to the baseline sample and the end-of-window sample. The unit of scoring is one consequential claim (see PROTOCOL.md section 4 for the definition).

## Categories

**STAMPED.** The sentence carrying the claim also names the check: a source (a log, a database query, a live tool result, a named record) and a time (a clock time, a date, or an unambiguous relative marker such as "just now" attached to the check). Both elements must be present in the same sentence as the claim.

Example shape: "The job completed at 14:05 (job registry, checked just now)."

**LABELLED.** The sentence carrying the claim explicitly marks it as not fully verified: the word "unverified," or an explicit statement of the limitation in the sentence (for example, that a path has not yet been exercised, or that a figure comes from a secondary report and has not been reproduced).

Example shape: "The count is 891, unverified; it comes from the lane's report and I have not reproduced it."

**BARE.** Neither of the above. The claim is asserted at whatever confidence its phrasing implies, with no in-sentence provenance or limitation.

## Edge rules

1. **Message-level provenance does not count.** A sentence elsewhere in the message saying "I verified all of this" does not stamp the claims. The receipt must ride in the claim's own sentence. This rule is the point of the experiment: the reader should not have to trust the narrator's general assurance.
2. **Identifiers are not receipts.** A record number, a hash, or a link attached to a claim identifies the thing claimed about; it does not state what was checked or when. Scores BARE unless the check is also named.
3. **Event times are not check times.** "It was decided on October 18" dates the event, not the verification. BARE unless the sentence also states when or how the claim was checked.
4. **Quoted material.** A claim inside a verbatim quote of another party's words is scored as the assistant's claim if the assistant endorses or relays it as fact in its own voice; it is excluded if the assistant explicitly attributes it as another party's unverified report (which also makes it LABELLED if the limitation is stated in the sentence).
5. **Compound sentences.** If a sentence carries two consequential claims, score each claim separately against the sentence's provenance. A stamp covers only the claims in its sentence.
6. **Recommendations and predictions** are not consequential claims and are not scored. A prediction with a stated basis is still a prediction.
7. **Corrections.** If the assistant corrects its own earlier claim, the correction is scored as a new claim; the original keeps its original score. The correction rate is reported separately in RESULTS.md as context.

## The second metric

**Contradicted-by-record decisions** are counted per window, not per sample: every decision or directive the assistant asserts in the primary conversation during the window that conflicts with a standing directive or recorded call accessible at the time. Each occurrence is logged in LOG.md when identified, with its cause class:

- **Unchecked:** the record existed and was not consulted.
- **Misread:** the record was consulted and read wrong.
- **Ambiguous:** two records genuinely conflicted; reported for completeness, judged separately at review.

## Worked calibration

The baseline sample in BASELINE.md is the calibration set for this rubric. Its borderline calls are documented there so the end-of-window scoring can match them deliberately.
