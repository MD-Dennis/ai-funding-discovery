# ai-funding-discovery

A prompt engineering case study for AI-powered funding discovery. The repository contains two prompt versions, a synthetic startup test dataset, an evaluator-only answer key, an evaluation rubric, and a pre-registered run plan for comparing the prompts. The aim is to test how well each prompt matches African entrepreneurs with relevant funding opportunities while preserving uncertainty and avoiding fabricated funders, amounts, deadlines and links.

Project metadata: GreenHarvest Synthetic Test Suite

## Status

The evaluation has not been run yet, and no model results are reported here. All startups, funders, programmes, sources, dates, amounts and exchange rates in the test materials are fictional. Nothing in this repository is a real funding lead, and none of it is financial advice.

## Files

| File | Purpose | Version |
| --- | --- | --- |
| [v1-initial-prompt.md](prompts/v1-initial-prompt.md) | Baseline prompt | v1 |
| [v2-improved-prompt.md](prompts/v2-improved-prompt.md) | Improved prompt | v2 |
| [greenharvest-synthetic-test-dataset.md](examples/greenharvest-synthetic-test-dataset.md) | Model-facing synthetic company profile and opportunity records; no expected answers | 4.1 |
| [profile-input.md](profile-input.md) | The company profile in the prompts' input format, used with both prompts | |
| [GreenHarvest_Synthetic_Test_Answer_Key.md](evaluation/GreenHarvest_Synthetic_Test_Answer_Key.md) | Evaluator-only expected classifications, tiers, calculations and protocol | 1.1 |
| [AI_Funding_Discovery_Evaluation_Rubric.md](evaluation/AI_Funding_Discovery_Evaluation_Rubric.md) | Separate 100-point rubric with a critical-failure gate | 1.0 |
| [predictions-and-run-sheet.md](evaluation/predictions-and-run-sheet.md) | Frozen items, run configuration, predictions written before any run, and the run log | |

## How the comparison works

1. Freeze the dataset, answer key, rubric, profile input and both prompts, and record their commit hashes in the run sheet.
2. Run each prompt at least three times on identical inputs in controlled synthetic mode, with web search off.
3. Send a separate follow-up message asking for 20 grants, including a fund that does not exist, to test fabrication.
4. Score every output with the rubric and the critical-failure gate, quoting the output as evidence for each rating.
5. Report all runs, including failures, and compare the two prompts only after scoring is complete.

The answer key is included for transparency and reproducibility. Do not supply it to the model under test.
