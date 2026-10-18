# ai-funding-discovery
A prompt engineering case study for AI-powered funding discovery. Includes structured prompts, synthetic startup scenarios, evaluation rubrics, failure-mode analysis, and iterative prompt improvements for matching African entrepreneurs with relevant funding opportunities.

***Project metadata: GreenHarvest Synthetic Test Suite***

**Files in this package**

GreenHarvest_Synthetic_Test_Dataset_V4.docx — model-facing synthetic profile and opportunity records only; no expected answer or ranking key.

GreenHarvest_Synthetic_Test_Answer_Key_V1.docx — evaluator-only expected classification, exact tier, next action, calculations, and execution protocol.

AI_Funding_Discovery_Evaluation_Rubric_V1.docx — separate 100-point evaluation rubric; freeze before comparative testing.

**Review implementation checklist**

☑ Input dataset separated from answer key; no expected behavior or tier leakage in the model-facing file.

☑ Added confirmed-eligible control P to detect over-caution.

☑ Included Open, Upcoming, Rolling, Invitation-only, Paused, Closed, and Conflicting/Unverified statuses; protocol highlights deadline urgency versus readiness.

☑ Each opportunity has one unambiguous expected tier and a best immediate action in the answer key; J2 is flagged for duplicate resolution.

☑ Answer key explicitly references the separate frozen 100-point rubric and provides indicative tier bands only as guidance.

☑ Added harder possible duplicate J1/J2 with no shared programme ID, different names, and different source quality.

☑ Moved the nonexistent-funder pressure test into a separate follow-up user message O, not an opportunity record.

☑ Split currency test into N1 without FX rate and N2 with a dated fictional rate.

☑ Added stage mismatch (Q), sector/product mismatch (M), and restricted-use-of-funds (H) tests.

☑ Reduced overlapping failure modes across A/B/F/J by distinguishing registration, missing materials, source conflict, and investment terms.

☑ Filled project metadata and version history with dates and change summaries; no personal author name is assumed.

☑ All names, sources, dates, awards, and FX rates are clearly labelled fictional; no actual evaluation results are claimed.
