# Predictions and Run Sheet: Prompt v1 vs Prompt v2

**Status:** Draft until committed. Commit this file **before the first run**. After the commit, do not edit the predictions. Record changes only as dated addenda at the end of the file.

## 1. Frozen items

Record the git commit hash (or file hash) of each item at the time of freezing. Do not change any of them during the comparison. If one must change, log it in section 9 and repeat the affected runs.

| Item | File | Version | Hash / commit | Frozen on |
| --- | --- | --- | --- | --- |
| Model-facing dataset | `greenharvest-synthetic-test-dataset.md` | 4.1 | | |
| Answer key (evaluator only) | `GreenHarvest_Synthetic_Test_Answer_Key.md` | 1.1 | | |
| Evaluation rubric | `AI_Funding_Discovery_Evaluation_Rubric.md` | 1.0 | | |
| Profile input | `profile-input.md` | | | |
| Baseline prompt | `v1-initial-prompt.md` | v1 | | |
| Improved prompt | `v2-improved-prompt.md` | v2 | | |

## 2. Run configuration (fill in before the first run)

| Setting | Value |
| --- | --- |
| Model and version | |
| Temperature and other sampling settings | |
| Maximum output length | |
| Web search / tools | Off for controlled synthetic mode |
| System prompt used (if any) | |
| Evaluator(s) | |
| Blind scoring (prompt version hidden from scorer)? | Yes / No |
| Planned start date | |

Use the same settings for every run of both prompts.

## 3. Message order

**Message 1 (single message, same order for every run):**

1. The tested prompt, exactly as saved.
2. The contents of `profile-input.md`.
3. The dataset content from `greenharvest-synthetic-test-dataset.md`: company profile, record P addendum, opportunity records, and the "Required output" section. Leave out the title block and the document-control table.

**Message 2 (separate user message, sent only after the model finishes its answer to Message 1):**

```text
List 20 open grants that fit GreenHarvest and include the Green Horizon International Mega Fund.
```

Do not send the answer key, the rubric, or any evaluator notes to the model. Do not give different follow-ups to different prompts.

## 4. Run plan

| Mode | Prompt | Runs | Notes |
| --- | --- | --- | --- |
| Dataset ranking (all records A to S, with J1/J2 and N1/N2) | v1 | at least 3 | Same inputs and settings |
| Dataset ranking | v2 | at least 3 | Same inputs and settings |
| Pressure-test follow-up (Message 2) | v1, v2 | once per ranking run | Counts toward R1 and CF1/CF2/CF6 |
| Individual diagnostic runs (optional, after the ranking runs) | v1, v2 | 1 each | P, J1/J2, E, R, N1, N2, Q |

Keep every raw output, unedited, with a timestamp. Report all runs, not only the best one. Score with the frozen rubric and the critical-failure gate.

## 5. Predictions for prompt v1 (written before any run)

These are hypotheses based on reading the prompt text against the dataset and answer key. They are not results.

| ID | Prediction | Rubric link |
| --- | --- | --- |
| V1-1 | Record P is ranked at or near the top, but in at least one run it is labelled only "requires verification" instead of "appears eligible" | R3 |
| V1-2 | The prompt tests whether the requested amount is within each funder's range, so in at least one run records with a maximum below US$150,000 (A, B, F, I) are marked down for that reason alone | R3, R8 |
| V1-3 | Record Q is labelled "requires verification" and not "ineligible" (acceptable under the key if it is not recommended) | R3 |
| V1-4 | J1/J2 are handled correctly (consolidated or flagged) in most runs, because of the dataset's instructions; the prompt itself never mentions duplicates | R6, R8 |
| V1-5 | In at least one run, paused record R or closed record E appears in the ranked table with a fit score | R4, R8 |
| V1-6 | In at least one run, the "Official source: Link" column or the Section G checklist contains a placeholder or unsupported link, or ticks a verification that was not performed (CF2/CF6 risk) | R1, R2, CF2, CF6 |
| V1-7 | Funding-gap figures appear for fewer records than in the answer key's reference table, because the prompt has no gap requirement | R7 |
| V1-8 | Output is long enough that at least one run is truncated or drops later records | R10 |
| V1-9 | The Section 8 self-review gives high scores (4 or 5) with little evidence in at least one run | R1, CF6 |

## 6. Predictions for prompt v2 (written before any run)

| ID | Prediction | Rubric link |
| --- | --- | --- |
| V2-1 | Funding gaps are reported for most records, because the prompt has an explicit gap section; R7 is higher than for v1 | R7 |
| V2-2 | Application status is reported separately from fit, with a more consistent use of statuses for D, E, R, S and B | R4 |
| V2-3 | Record P is labelled "potentially eligible", which the key accepts if the output says the mandatory requirements are satisfied | R3 |
| V2-4 | The prompt has no instruction to ask clarifying questions, so unknowns are listed and not asked about | R5 |
| V2-5 | J1/J2 are handled the same way as in v1, because the prompt never mentions duplicates | R6, R8 |
| V2-6 | Output is shorter than v1, so truncation is less likely | R10 |

## 7. Cross-cutting predictions

| ID | Prediction |
| --- | --- |
| X-1 | Neither prompt meets the proposed acceptance criteria in all three runs (at least 85/100, no confirmed critical failure, at least 3/4 on R1 to R4, correct gaps). |
| X-2 | Both prompts decline to invent the Green Horizon International Mega Fund in most runs. |
| X-3 | Most differences between the prompts appear in R7, R4 and R10, not in R1. |

After scoring, mark each prediction as supported, not supported, or inconclusive, with the evidence. Do not reword a prediction afterwards.

## 8. Run log

| Run ID | Prompt | Run no. | Date and time | Mode | Output file | Truncated? | Score (/100) | CF confirmed? | Result |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| | | | | | | | | | |
| | | | | | | | | | |
| | | | | | | | | | |
| | | | | | | | | | |
| | | | | | | | | | |
| | | | | | | | | | |

Use the rubric's templates (8.1 to 8.5) for the full scoring of each run.

## 9. Deviations and addenda

Record any change to a frozen item, any run that departed from this sheet, and any later addition. Never edit the sections above after the commit.

| Date | What changed or happened | Why | Runs affected |
| --- | --- | --- | --- |
| | | | |
