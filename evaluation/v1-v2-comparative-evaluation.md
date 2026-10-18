# V1 vs V2 Comparative Evaluation: AI Funding Discovery and Matching

> [!IMPORTANT]
> This is an **exploratory comparison, not a validated benchmark.** Both assessments were single-run and non-blind, and the evaluator answer key was available in the broader evaluation context.

## Table of Contents

1. [Evaluation objective](#1-evaluation-objective)
2. [Methodology and limitations](#2-methodology-and-limitations)
3. [Comparative results](#3-comparative-results)
4. [Comparative performance analysis](#4-comparative-performance-analysis)
5. [Critical-failure review](#5-critical-failure-review)
6. [Overall interpretation](#6-overall-interpretation)
7. [Conclusion](#7-conclusion)

## 1. Evaluation objective

This evaluation compares the reviewed outputs produced using two prompt versions for the GreenHarvest AI funding-discovery case study. GreenHarvest Innovations Ltd and the funding records in the test dataset are fictional. The evaluation therefore measures performance on a controlled synthetic task, not real-world funding availability.

The purpose is to assess how well each output handles factual integrity, evidence traceability, eligibility, application status, profile uncertainty, financing compatibility, financial calculations, ranking consistency, actionability, and completeness.

## 2. Methodology and limitations

Both outputs were assessed against the same ten-criterion evaluation rubric. Each criterion is rated from 0 to 4, with weighted points calculated as:

**Weighted points = criterion weight × (rating ÷ 4)**

The scores below are provisional evaluator judgments based on one exploratory review of each output. Both assessments were **single-run, exploratory, and non-blind**. The evaluator answer key was available in the broader evaluation context, so these results are not a clean blind benchmark. No multi-run consistency analysis or independent inter-rater agreement result is available.

## 3. Comparative results

| Evaluation criterion | Weight | V1 rating | V1 points | V2 rating | V2 points |
|---|---:|---:|---:|---:|---:|
| R1: Factual integrity and non-fabrication | 20 | 3/4 | 15.00 | 4/4 | 20.00 |
| R2: Evidence and source traceability | 15 | 2/4 | 7.50 | 3/4 | 11.25 |
| R3: Eligibility accuracy | 15 | 3/4 | 11.25 | 4/4 | 15.00 |
| R4: Application status and deadlines | 10 | 3/4 | 7.50 | 4/4 | 10.00 |
| R5: Profile accuracy and uncertainty | 10 | 4/4 | 10.00 | 4/4 | 10.00 |
| R6: Financing compatibility | 10 | 3/4 | 7.50 | 4/4 | 10.00 |
| R7: Financial calculations | 5 | 2/4 | 2.50 | 4/4 | 5.00 |
| R8: Ranking consistency | 5 | 2/4 | 2.50 | 2/4 | 2.50 |
| R9: Actionability | 5 | 4/4 | 5.00 | 4/4 | 5.00 |
| R10: Completeness | 5 | 3/4 | 3.75 | 4/4 | 5.00 |
| **Total** | **100** |  | **72.50/100** |  | **93.75/100** |

The reviewed V2 output scored **21.25 points higher** than the reviewed V1 output. This is a descriptive difference between the two reviewed outputs; it is not, by itself, evidence of statistical significance or a validated improvement.

## 4. Comparative performance analysis

### 4.1 Factual integrity and evidence traceability

**V1:** The output disclosed that live verification had not been performed and did not have a confirmed critical failure identified. However, evidence traceability and the explanation of how claims supported recommendations could have been more systematic.

**V2:** The output more explicitly distinguished evidence-supported findings from unknowns and conflicting information. It also made the limits of the synthetic exercise clearer. Traceability still could be improved through a compact evidence ledger linking each decision to its supporting record and source details.

**Comparative finding:** V2 was assessed more favorably for factual integrity and traceability in the reviewed output. Because the assessments were not blind, this should be interpreted as a provisional evaluator judgment.

### 4.2 Eligibility and application status

**V1:** The output generally handled unknowns and eligibility considerations, but the distinctions between eligibility, strategic fit, application status, and evidence confidence were not as consistent.

**V2:** The output more clearly separated these dimensions, kept confirmed exclusions out of the recommended shortlist, and identified records that required verification. It also accounted for conflicting status evidence in the synthetic records.

**Comparative finding:** The reviewed V2 output showed stronger eligibility and status discipline. No confirmed critical eligibility or false-open-status failure was identified in either reviewed output.

### 4.3 Financial calculations and financing compatibility

**V1:** The output recognised that grants, equity, debt, and in-kind support are different, but its funding-gap calculations were incomplete across the records.

**V2:** The output calculated the principal funding gaps more consistently and distinguished cash from in-kind support. It did not convert the N1 amount without a supplied exchange rate; for N2, it used the dataset's fictional exchange rate of KES 130 per US dollar. It also identified the possible duplicate relationship between J1 and J2 rather than automatically counting them as separate opportunities.

**Comparative finding:** Financial calculations were the clearest rubric-level difference: V1 received 2/4 for R7, while V2 received 4/4. This finding applies to the reviewed synthetic output and does not establish financial accuracy in real-world research.

### 4.4 Ranking consistency

Both outputs received **2/4** for ranking consistency. This indicates that the relationship between scores, evidence confidence, eligibility, unresolved requirements, and final ordering remained an area for improvement.

A numerical fit score should not be treated as a definitive ranking when key eligibility facts are unknown. Recommendations should make their provisional nature clear and explain the deciding factors when opportunities have similar scores.

### 4.5 Actionability and completeness

Both outputs received **4/4** for actionability. V1 already provided practical next steps, while V2 retained this strength and gave a more structured account of exclusions, verification needs, and financial considerations.

V2 received 4/4 for completeness compared with V1's 3/4, reflecting the more explicit coverage of scoring, financial gaps, duplicate handling, and quality-control considerations in the reviewed output.

## 5. Critical-failure review

| Critical-failure category | V1 reviewed output | V2 reviewed output |
|---|---|---|
| Fabricated funding opportunity | None confirmed | None confirmed |
| Fabricated source or URL | None confirmed | None confirmed |
| False eligibility assurance | None confirmed | None confirmed |
| False open-status claim | None confirmed | None confirmed |
| Financing misrepresentation | None confirmed | None confirmed |
| False verification claim | None confirmed | None confirmed |
| Material financial misrepresentation | None confirmed; calculation coverage was incomplete | None confirmed |

> [!NOTE]
> "None confirmed" means no such failure was identified in the reviewed output. It does not mean that every claim was independently verified or that either prompt is proven free of critical failures.

## 6. Overall interpretation

The provisional scores were:

- **V1:** 72.50/100
- **V2:** 93.75/100
- **Observed difference:** +21.25 points for V2

Within these exploratory reviews, V2 showed stronger results in factual-integrity assessment, evidence traceability, eligibility handling, status classification, financing compatibility, financial calculations, and completeness. Profile accuracy and uncertainty, actionability, and ranking consistency did not change in the rubric scores.

The most important remaining weakness was ranking consistency, which scored 2/4 for both versions. The evidence also remains insufficient to determine how stable these results would be across repeated runs or independent evaluators.

## 7. Conclusion

The reviewed outputs suggest that V2 is a more explicit and promising prompt design for the GreenHarvest synthetic funding-discovery task. Its provisional score was **93.75/100**, compared with **72.50/100** for V1. The strongest observed difference was in financial calculations, with additional improvements in evidence handling, eligibility, application status, financing compatibility, and completeness.

> [!WARNING]
> The result should be described as an **exploratory comparison, not a validated benchmark**. Each version was assessed in a single non-blind review, and the evaluator answer key was available in the broader context. The 21.25-point difference does not establish statistical significance or prove that V2 will perform better across repeated runs or real-world funding research.
