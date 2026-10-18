# V1 Initial Prompt — Exploratory Evaluation

**Project:** AI Funding Discovery for African Entrepreneurs  
**Test suite:** GreenHarvest Synthetic Test Suite  
**Baseline prompt:** `prompts/v1-initial-prompt.md`  
**Dataset:** `examples/greenharvest-synthetic-test-dataset.md` (v4.1)  
**Evaluation rubric:** `evaluation/AI_Funding_Discovery_Evaluation_Rubric.md` (v1.0)  
**Answer key:** `evaluation/GreenHarvest_Synthetic_Test_Answer_Key.md` (v1.1)  
**Evaluation status:** Exploratory review — controlled evaluation pending

## 1. Purpose

This review examines the initial funding-discovery prompt (V1) to identify its strengths, weaknesses, and potential failure modes before developing an improved version.

The objective is to establish an evidence-based improvement process rather than rewrite the prompt based on assumptions about what a better version should contain.

V1 is intended to help African entrepreneurs identify and prioritize funding opportunities using business-profile information, eligibility requirements, funding criteria, source evidence, and practical next steps.

The evaluation focuses on whether the prompt encourages the model to produce recommendations that are accurate, relevant, transparent, financially consistent, and actionable.

## 2. Evaluation methodology

The exploratory review uses the GreenHarvest synthetic dataset, which contains fictional funding opportunities designed to test eligibility decisions, evidence handling, application-status interpretation, financing compatibility, financial calculations, and duplicate detection.

The planned controlled evaluation will use:

- The original V1 prompt without modifications.
- The standardized GreenHarvest business profile.
- Synthetic dataset version 4.1.
- Evaluation rubric version 1.0.
- The evaluator-only answer key version 1.1.

External web research is disabled in controlled synthetic mode. The model must reason from the supplied fixture without substituting real funding programmes or inventing supporting evidence.

The planned procedure is to execute V1 at least three times using identical inputs and settings, preserve every raw output, score each run independently, and record any critical failures.

The answer key is reserved for evaluation and must not be included in the model-facing input.

### Current evaluation limitations

This document records an exploratory review of one output generated in the current conversation. It is not the result of three completed, controlled runs.

The review is also not blind because the answer key was already present in the conversation context. The current findings should therefore be treated as preliminary observations, not definitive evidence of reproducible model performance.

No claims of accuracy improvement, benchmark superiority, or production readiness are made.

## 3. Summary of exploratory findings

The reviewed output demonstrated several useful behaviours, including preserving important unknowns, distinguishing financing instruments, identifying conditional eligibility requirements, and recommending practical next steps.

However, it also exposed weaknesses that should be investigated during controlled testing.

| Evaluation area | Preliminary finding | Potential impact |
|---|---|---|
| Factual integrity | The reviewed output did not invent source URLs or claim to have performed live verification. | Positive initial signal, but repeated testing is needed. |
| Evidence traceability | Source descriptions were included, but claims were not consistently connected to specific supporting evidence. | Makes independent verification more difficult. |
| Eligibility handling | Most mandatory conditions and material unknowns were identified. | Some classifications may still require more explicit decision rules. |
| Application status | Closed, paused, upcoming, and invitation-only opportunities were distinguished. | The approach should be tested for consistency across repeated runs. |
| Financing compatibility | Grants, equity, debt, cash, and in-kind support were generally distinguished. | Additional safeguards may be needed for restrictions, matching requirements, and financing terms. |
| Financial calculations | Funding gaps were calculated for some opportunities but not consistently reported across all applicable records. | Incomplete comparisons can lead to poor funding decisions. |
| Ranking consistency | Preliminary fit scores were assigned, but the calculations were not fully demonstrated. | Rankings may vary between runs. |
| Duplicate detection | A possible duplicate was identified, but the two records remained separately ranked. | Duplicate opportunities could be counted more than once. |
| Output completeness | The report contained the major requested sections and covered the dataset. | Some financial and evidence fields remained incomplete. |
| Self-evaluation | The output assigned itself relatively high quality ratings with limited supporting evidence. | Self-assessment may create unjustified confidence. |

These findings describe the reviewed output only. They have not yet been established as consistent behaviours of V1.

## 4. Strengths to preserve

The following aspects of V1 should be retained during future prompt development.

### 4.1 Explicit handling of missing information

The prompt instructs the model not to invent missing business details and to identify information that could materially affect its recommendations.

This is important because registration status, revenue, traction, ownership, matching funds, and financing preferences can determine whether an opportunity is appropriate.

### 4.2 Emphasis on evidence and non-fabrication

V1 prioritizes official sources, requires disclosure of uncertainty, and prohibits inventing funders, funding amounts, deadlines, eligibility conditions, and application URLs.

These instructions establish a useful foundation for a trustworthy funding-discovery system.

### 4.3 Distinction between financing instruments

The prompt recognizes that grants, equity investments, and debt facilities have different implications for a business.

This distinction should be preserved and strengthened, particularly when assessing repayment obligations, equity dilution, matching requirements, and restricted in-kind support.

### 4.4 Practical recommendations

The required output includes a funding strategy, prioritized action plan, and verification checklist.

These elements help translate funding research into decisions a founder can act on.

### 4.5 Separation of fit and evidence confidence

V1 instructs the model to distinguish opportunity relevance from the confidence supported by available evidence.

This is an important principle: an opportunity can appear strategically suitable while remaining unverified or inaccessible.

## 5. Potential weaknesses identified

### 5.1 Scoring methodology may be under-specified

V1 provides weighted criteria for calculating a preliminary fit score out of 100. However, the prompt does not define detailed scoring anchors for each criterion.

Consequently, different runs may assign different scores to the same opportunity without a clearly identifiable reason.

**Investigation:** Determine whether explicit scoring anchors and a requirement to show the component scores improve ranking consistency.

### 5.2 Funding-gap calculations are not sufficiently explicit

The prompt considers whether a funding amount aligns with the entrepreneur's requirements, but it does not explicitly require a funding-gap calculation for every applicable opportunity.

The exploratory output therefore calculated gaps for some records but omitted others.

**Investigation:** Test whether a structured financial comparison improves completeness and arithmetic accuracy. The calculation must distinguish the total funding target from the amount available from a single source.

### 5.3 Evidence traceability could be stronger

V1 requests official sources and supporting evidence. However, the reviewed output did not consistently associate each important claim with its supporting record or source.

**Investigation:** Determine whether a structured evidence field containing the claim, supporting source, source date, verification status, and remaining uncertainty improves traceability.

In controlled synthetic mode, the model must not imply that a fictional source was independently accessed or live-verified.

### 5.4 Duplicate detection is not explicitly required

The dataset includes two differently named records that may refer to the same investment opportunity.

The exploratory output recognized the possible duplication but continued to rank both records separately.

**Investigation:** Test whether explicit duplicate-detection instructions prevent double-counting while preserving uncertainty about identity.

### 5.5 Application status and opportunity fit could be more clearly separated

An opportunity can be relevant to a business but unavailable for immediate application.

For example, a programme may be closed, paused, upcoming, or invitation-only despite having an otherwise suitable sector or award range.

**Investigation:** Test whether separate fields for fit, eligibility, application status, and evidence confidence produce more reliable recommendations.

### 5.6 Self-evaluation may not provide sufficient assurance

V1 asks the model to evaluate its own output against several quality criteria.

The exploratory output assigned itself relatively high ratings, but those ratings did not fully reflect the omissions identified in the independent review.

**Investigation:** Assess whether evidence-linked self-review is useful, while keeping final scoring independent and governed by the separate evaluation rubric.

## 6. Preliminary rubric assessment

The exploratory output received the following provisional assessment.

| Criterion | Weight | Provisional rating | Weighted points |
|---|---:|---:|---:|
| R1. Factual integrity and non-fabrication | 20 | 3/4 | 15.00 |
| R2. Evidence quality and source traceability | 15 | 2/4 | 7.50 |
| R3. Eligibility and hard constraints | 15 | 3/4 | 11.25 |
| R4. Application status and deadline accuracy | 10 | 3/4 | 7.50 |
| R5. Profile interpretation and uncertainty | 10 | 4/4 | 10.00 |
| R6. Financing and use-of-funds compatibility | 10 | 3/4 | 7.50 |
| R7. Financial calculations and funding gap | 5 | 2/4 | 2.50 |
| R8. Scoring and ranking consistency | 5 | 2/4 | 2.50 |
| R9. Actionability and decision support | 5 | 4/4 | 5.00 |
| R10. Completeness, clarity, and output compliance | 5 | 3/4 | 3.75 |
| **Total** | **100** | | **72.50/100** |

**Interpretation:** This is a provisional score for the reviewed output, not an established V1 baseline score.

The result suggests that financial completeness, evidence traceability, and scoring consistency deserve particular attention. These areas must be reassessed across controlled runs before conclusions are finalized.

### Critical-failure review

No critical failure was confirmed in the reviewed output.

This does not establish that V1 is free of critical failures. The remaining controlled runs must independently assess all seven categories defined in the evaluation rubric.

## 7. Relationship to the pre-registered predictions

The project includes predictions about V1's expected behaviour before evaluation.

These predictions must remain unchanged. After each controlled run, the evaluator should classify each prediction as supported, not supported, or inconclusive and cite the output evidence.

The exploratory observations may inform the investigation, but they must not replace the planned run log or be presented as results from repeated trials.

## 8. Implications for the next prompt version

The findings suggest several areas to investigate when developing V2:

1. More explicit scoring anchors and component-level score calculations.
2. Consistent funding-gap calculations and clear financial assumptions.
3. Stronger claim-level evidence traceability.
4. Explicit duplicate-detection and consolidation rules.
5. Separate reporting of fit, eligibility, application status, and evidence confidence.
6. More evidence-based quality checks.

These are **candidate improvements**, not yet validated changes.

V2 should be developed after the controlled V1 evaluation is completed. Each material change should be linked to an observed weakness, and the revised prompt should be tested against the same frozen inputs and rubric.

## 9. Next steps

- [ ] Freeze the exact versions of all evaluation inputs.
- [ ] Record file hashes or the relevant Git commit.
- [ ] Confirm the model, configuration, tool settings, and evaluation date.
- [ ] Execute at least three controlled V1 runs.
- [ ] Save each complete, unedited model output.
- [ ] Score every run using criteria R1–R10.
- [ ] Check critical-failure categories CF1–CF7 independently.
- [ ] Evaluate the pre-registered predictions without modifying them.
- [ ] Compare run-to-run consistency and investigate recurring failures.
- [ ] Finalize the V1 evaluation report.
- [ ] Develop V2 based on the documented findings.
- [ ] Evaluate V2 using the same controlled test cases.

## 10. Conclusion

The exploratory review suggests that V1 provides a useful starting point for funding discovery, particularly through its emphasis on evidence, uncertainty, financing compatibility, and practical recommendations.

However, the reviewed output also highlights potential weaknesses in scoring reproducibility, financial completeness, source traceability, and duplicate handling.

The next objective is to determine whether these weaknesses persist across controlled runs. Only after that evaluation should the project move to V2.

**No performance improvement is claimed at this stage.** Any improvement claim must be supported by recorded outputs and comparative evaluation results.

---
