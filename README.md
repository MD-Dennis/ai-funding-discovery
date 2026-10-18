# ai-funding-discovery

A prompt-engineering case study evaluating AI-powered funding discovery for African entrepreneurs. This repository compares two prompt versions using a fictional company profile and a synthetic funding-opportunity dataset. The goal is to assess how well the prompts identify relevant opportunities while preserving uncertainty, applying eligibility rules, calculating funding gaps, and avoiding fabricated funders, amounts, deadlines, sources, and links.

**Project metadata:** GreenHarvest Synthetic Test Suite

## Evaluation status

The project has completed initial exploratory reviews of both prompt versions:

| Prompt version | Provisional score | Review status |
|---|---:|---|
| V1: Initial prompt | **72.50/100** | Single exploratory review |
| V2: Evidence-grounded prompt | **93.75/100** | Single exploratory review |

> [!IMPORTANT]
> These scores are **provisional, not a formal benchmark**. The reviews were single-run and non-blind; the evaluator answer key was available in the broader evaluation context. The 21.25-point difference is an observed difference between the reviewed outputs, not proof of a validated improvement or statistical significance. The results should not be presented as evidence that V2 will necessarily perform better across repeated runs or in real-world funding research.

All startups, funders, programmes, sources, dates, amounts, and exchange rates in the test materials are fictional. Nothing in the synthetic dataset is a real funding lead, and this project is not financial advice.

## Repository contents

| File | Purpose |
|---|---|
| [`prompts/v1-initial-prompt.md`](prompts/v1-initial-prompt.md) | V1 baseline funding-discovery prompt |
| [`prompts/v2-improved-prompt.md`](prompts/v2-improved-prompt.md) | V2 evidence-grounded funding-discovery prompt |
| [`examples/greenharvest-synthetic-test-dataset.md`](examples/greenharvest-synthetic-test-dataset.md) | Synthetic company and funding-opportunity records used for testing |
| [`profile-input.md`](profile-input.md) | GreenHarvest company profile formatted for use with the prompts |
| [`evaluation/v1-exploratory-review.md`](evaluation/v1-exploratory-review.md) | Exploratory review of the V1 output |
| [`evaluation/V2 Exploratory Evaluation — AI Funding Discovery and Matching.md`](evaluation/V2%20Exploratory%20Evaluation%20%E2%80%94%20AI%20Funding%20Discovery%20and%20Matching.md) | Exploratory review of the V2 output |
| [`evaluation/v1-v2-comparative-evaluation.md`](evaluation/v1-v2-comparative-evaluation.md) | Side-by-side comparison of the V1 and V2 exploratory results |
| [`evaluation/predictions-and-run-sheet.md`](evaluation/predictions-and-run-sheet.md) | Pre-registered predictions, run configuration, and evaluation log |
| [`rubrics/AI_Funding_Discovery_Evaluation_Rubric.md`](rubrics/AI_Funding_Discovery_Evaluation_Rubric.md) | Ten-criterion, 100-point evaluation rubric and critical-failure conditions |
| [`evaluation/GreenHarvest_Synthetic_Test_Answer_Key.md`](evaluation/GreenHarvest_Synthetic_Test_Answer_Key.md) | Evaluator-only expected classifications and calculations; do not provide to the model under test |

## What the evaluation examines

The rubric assesses:

- Factual integrity and non-fabrication.
- Evidence and source traceability.
- Eligibility accuracy.
- Application status and deadlines.
- Accuracy of the supplied company profile and handling of unknowns.
- Financing compatibility.
- Funding-gap calculations.
- Ranking consistency.
- Actionability.
- Completeness.

Critical failures can result in a fail regardless of the numerical score, according to the rubric.

## Evaluation materials and handling

The synthetic dataset and `profile-input.md` are model-facing test materials. The answer key is for evaluators only.

> [!CAUTION]
> **Do not include the answer key in the prompt, model context, or model-facing files during a test**, because exposing expected answers undermines the validity of the evaluation.

The run sheet records the intended evaluation procedure and should be used to document actual run settings and results. Keep raw model outputs unchanged and distinguish exploratory observations from results obtained in any later controlled evaluation.

## Limitations

- The current V1 and V2 scores each reflect one exploratory review.
- The reviews were not blind, and the answer key was available in the broader evaluation context.
- Multiple-run consistency and independent inter-rater agreement have not been established.
- The synthetic records do not establish real-world funding availability.
- The current score difference should not be described as a statistically significant or validated performance improvement.

These limitations should remain visible whenever the results are presented or cited.
