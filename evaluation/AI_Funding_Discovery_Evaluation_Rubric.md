# AI Funding Discovery Evaluation Rubric

**Version 1.0** | General-purpose quality assessment

*Designed for controlled test fixtures and real-world funding discovery*

## 1. Purpose and scope

This rubric provides a consistent, evidence-based way to evaluate AI outputs for funding discovery and opportunity matching. It assesses factual integrity, source quality, eligibility handling, status and deadline accuracy, uncertainty, financing compatibility, calculations, ranking, actionability, and output completeness.

It can be applied to controlled synthetic test fixtures or to live discovery runs involving real funding opportunities. Keep the test data, source evidence, and actual model output available to evaluators. This rubric does not itself establish whether an opportunity is real, open, or suitable; those determinations require evidence.

## 2. Scoring overview

Score ten dimensions for a total of 100 possible points. Each dimension receives one integer rating from 0 to 4, then is converted to weighted points.

| Dimension | Weight | Rating | Maximum points |
| --- | --- | --- | --- |
| **R1. Factual integrity and non-fabrication** | 20% | 0–4 | 20 |
| **R2. Evidence quality and source traceability** | 15% | 0–4 | 15 |
| **R3. Eligibility and hard constraints** | 15% | 0–4 | 15 |
| **R4. Application status and deadline accuracy** | 10% | 0–4 | 10 |
| **R5. Profile interpretation and uncertainty** | 10% | 0–4 | 10 |
| **R6. Financing and use-of-funds compatibility** | 10% | 0–4 | 10 |
| **R7. Financial calculations and funding gap** | 5% | 0–4 | 5 |
| **R8. Scoring and ranking consistency** | 5% | 0–4 | 5 |
| **R9. Actionability and decision support** | 5% | 0–4 | 5 |
| **R10. Completeness, clarity, and output compliance** | 5% | 0–4 | 5 |
| **TOTAL** | 100% | — | 100 |

**Weighted-points formula:** Dimension points = dimension weight × (rating ÷ 4). For example, a rating of 3 on a 20-point dimension earns 15 points. Add all ten dimension scores for a total out of 100.

The numeric score is diagnostic, not a substitute for the critical-failure gate in Section 5. A confirmed critical failure makes the overall result FAIL regardless of the numeric score.

## 3. Common rating scale

| Rating | Label | General anchor |
| --- | --- | --- |
| **4** | Excellent | Fully meets the dimension; accurate, complete, well-supported, and no material issue found. |
| **3** | Good | Meets the core requirement with only minor omissions or presentation issues that do not materially affect the decision. |
| **2** | Partially satisfactory | Mixed performance; a meaningful omission, ambiguity, or limited error remains, but the output is not wholly unusable. |
| **1** | Poor | Major weakness or error undermines reliability or usefulness for this dimension. |
| **0** | Failed | Dimension is absent, fundamentally incorrect, or unusable; or the output directly violates a core requirement. |

Evaluators should cite the exact output passage and relevant source or test record supporting each rating. Do not assign a score based only on impression.

## 4. Dimension-specific scoring anchors

### R1. Factual integrity and non-fabrication

**Weight: 20 points**

- **4 —** Material claims are accurate against the available evidence; no invented funders, opportunities, amounts, deadlines, eligibility rules, contacts, URLs, or verification claims.
- **3 —** No material fabrication; only minor imprecision that does not change the funding decision.
- **2 —** One or more unsupported or inaccurate non-critical claims, but the main shortlist remains broadly interpretable.
- **1 —** Multiple material inaccuracies or unsupported assertions meaningfully distort the shortlist.
- **0 —** Confirmed fabrication or false claim materially misleads the user; apply the critical-failure gate where applicable.

### R2. Evidence quality and source traceability

**Weight: 15 points**

- **4 —** Material claims are traceable to appropriate sources; source identity, URL, access/check date, and claim supported are clear; authoritative/current sources are prioritized.
- **3 —** Most material claims have usable sources; small gaps in dates or claim-level linkage remain.
- **2 —** Sources are present but incomplete, uneven, weak, or not clearly tied to individual claims.
- **1 —** Important claims lack supporting evidence, or low-quality sources are relied on without caveat.
- **0 —** Evidence is absent or unusable for the material claims, or sources are falsely represented as having been checked.

### R3. Eligibility and hard constraints

**Weight: 15 points**

- **4 —** Applies hard exclusions before ranking; distinguishes confirmed eligible, likely but unverified, potentially eligible pending clarification, ineligible, and unknown; explains decisive requirements.
- **3 —** Eligibility is generally handled correctly, with minor gaps in explanation or classification.
- **2 —** Some requirements are recognized, but unknowns and exclusions are not handled consistently.
- **1 —** Ranking or recommendation ignores important eligibility conditions or implies eligibility without adequate basis.
- **0 —** Verified-ineligible candidates are represented as eligible or hard exclusions are fundamentally disregarded; apply the critical-failure gate where applicable.

### R4. Application status and deadline accuracy

**Weight: 10 points**

- **4 —** Open/closed/upcoming/rolling/invitation-only/paused/unknown status and deadlines match current evidence; dates are explicit and checked where possible.
- **3 —** Status and deadlines are correct, with a minor citation or clarity gap.
- **2 —** Some status information is uncertain or incompletely sourced but uncertainty is disclosed.
- **1 —** Status/deadline is unreliable, stale, or presented with unjustified certainty.
- **0 —** A verified-closed opportunity is falsely presented as open, or a material deadline/status claim is fabricated; apply the critical-failure gate where applicable.

### R5. Profile interpretation and uncertainty

**Weight: 10 points**

- **4 —** Correctly interprets the user profile, preserves unknowns, distinguishes user-reported information from verified facts, and asks for or flags decisive missing information.
- **3 —** Profile is interpreted well with minor omissions in uncertainty handling.
- **2 —** Some assumptions or missing details are handled inconsistently, but major uncertainties are visible.
- **1 —** Makes unsupported assumptions about registration, revenue, founder attributes, traction, readiness, or capacity that materially affect recommendations.
- **0 —** The profile is fundamentally misread or material unknowns are routinely presented as established facts.

### R6. Financing and use-of-funds compatibility

**Weight: 10 points**

- **4 —** Correctly distinguishes grants, equity, debt, prizes, accelerators, in-kind support, and mixed packages; checks permitted uses and surfaces dilution, repayment, collateral, or matching conditions when relevant.
- **3 —** Financing type and use-of-funds fit are accurate, with minor omissions in caveats.
- **2 —** Some distinctions or conditions are missed, but the basic financing structure remains understandable.
- **1 —** Material financing terms or use restrictions are overlooked or obscured.
- **0 —** Financing type or cash value is materially misrepresented, such as calling a loan a grant; apply the critical-failure gate where applicable.

### R7. Financial calculations and funding gap

**Weight: 5 points**

- **4 —** Amounts, currency, cash/in-kind split, arithmetic, and nominal funding gaps are correct and assumptions are stated.
- **3 —** Calculations are correct with a minor presentation or assumption-labeling issue.
- **2 —** Small arithmetic or interpretation issue that is unlikely to materially alter the decision.
- **1 —** Material calculation error, unclear currency, or misleading comparison of award amounts.
- **0 —** Major financial misrepresentation, including treating in-kind support as cash or materially misstating available funding; apply the critical-failure gate where applicable.

### R8. Scoring and ranking consistency

**Weight: 5 points**

- **4 —** Ranking follows stated criteria consistently; hard eligibility is handled separately; fit and evidence confidence are distinct; score rationale is explainable.
- **3 —** Ranking is broadly consistent, with minor unexplained ordering choices.
- **2 —** Scores are present but weakly calibrated, partially inconsistent, or insufficiently explained.
- **1 —** Rankings conflict with the stated criteria or materially favor weaker matches without explanation.
- **0 —** Scores are arbitrary, internally contradictory, or used to imply an unsupported probability of winning.

### R9. Actionability and decision support

**Weight: 5 points**

- **4 —** Provides prioritized next steps, specific verification questions, document-preparation guidance, and practical follow-up actions.
- **3 —** Clear next steps are included but some could be more specific or prioritized.
- **2 —** Advice is generally relevant but generic or incomplete.
- **1 —** Little usable guidance for deciding or taking action.
- **0 —** No meaningful next steps, or advice encourages action based on materially false premises.

### R10. Completeness, clarity, and output compliance

**Weight: 5 points**

- **4 —** All required fields are present; concise, organized, understandable, and compliant with the requested output format.
- **3 —** Mostly complete and clear, with minor omissions or formatting issues.
- **2 —** Several fields are missing or the structure makes comparison difficult.
- **1 —** Major omissions or confusing presentation impair use.
- **0 —** Output fails to address the task or is unusable for comparison or follow-up.

## 5. Critical-failure gate

Before assigning the final outcome, review the output for the critical failures below. A confirmed critical failure makes the overall result FAIL regardless of the weighted score. Keep the numerical score for diagnostic purposes and record the evidence for the failure.

| Failure ID | Definition |
| --- | --- |
| **CF1 — Invented real-world opportunity** | The output presents a fabricated or unsupported opportunity as a verified real funding option. Do not trigger this solely because an evaluator is unfamiliar with a program; investigate the evidence first. |
| **CF2 — Fabricated source or application URL** | The output invents a source, official page, contact, or application URL, or falsely attributes information to a source. |
| **CF3 — False eligibility assurance** | The output assures or materially implies eligibility despite a verified exclusion or failed mandatory requirement. |
| **CF4 — False open status** | The output presents an opportunity as open when reliable evidence verifies that the relevant call is closed. |
| **CF5 — Material financing misrepresentation** | The output materially mislabels the financing type, such as describing a loan as a grant or equity as non-dilutive funding. |
| **CF6 — False verification claim** | The output claims to have checked or verified a source, deadline, eligibility condition, or status when it did not. |
| **CF7 — Material financial misrepresentation** | The output materially misstates the award amount, currency, cash component, matching requirement, or funding calculation in a way that could mislead a decision. |

### Critical-failure recording requirements

- Record the exact output passage and the relevant source, test record, or authoritative evidence.
- Explain why the issue is material and which critical-failure definition applies.
- Mark the failure as confirmed, not confirmed, or unresolved pending evidence.
- If unresolved, do not label it confirmed; document the additional verification needed.
- A confirmed critical failure results in overall FAIL even if the numeric score is high.

## 6. Performance bands and proposed acceptance criteria

| Weighted score | Performance band | Interpretation |
| --- | --- | --- |
| **90–100** | Excellent | Strong performance; minor refinements may remain. |
| **80–89** | Good | Generally reliable, with targeted improvements recommended. |
| **70–79** | Acceptable with revisions | Usable only with meaningful corrections and retesting. |
| **60–69** | Weak | Substantial improvement is needed before relying on outputs. |
| **0–59** | Poor | Output quality is not adequate for the intended use. |
| **Any score with a confirmed critical failure** | FAIL | Critical-failure gate overrides the numeric performance band. |

**Proposed prototype acceptance criteria (not industry standards):** A prototype may be considered ready for the next controlled iteration if it scores at least 85/100, has no confirmed critical failures, scores at least 3/4 on R1–R4, calculates funding gaps correctly, does not present verified-ineligible opportunities as eligible, does not fabricate real funders/sources/URLs, and explicitly discloses unresolved material requirements. These are proposed project thresholds, not validated industry benchmarks.

A passing score does not prove the system is safe for unattended use, that opportunities are comprehensive, or that an applicant will receive funding.

## 7. Evaluation procedure

1. Define the evaluation mode: (A) controlled matching against a fixed reference dataset, or (B) live discovery of real opportunities. Keep the two modes separate.
2. Freeze the input profile, prompt version, model and configuration, tool access, date/time, and reference dataset or source snapshot.
3. Establish expected outcomes and known facts before reviewing the model output. Do not use the model’s own answer as ground truth.
4. Run the prompt and retain the complete unedited output and source material actually accessed.
5. Score R1–R10 independently. For every dimension, record the rating, weighted points, evidence, and a concise rationale.
6. Check each critical-failure condition separately and document any confirmed or unresolved issue.
7. Apply the critical-failure gate, then assign the performance band based on the numeric score.
8. Perform root-cause analysis for each error: prompt ambiguity, missing profile data, weak source, retrieval failure, stale information, reasoning/calculation error, or output-format failure.
9. Revise the prompt or workflow, rerun the same cases, and compare the results. Use a separate holdout set when possible to reduce overfitting.
10. Report observed results only. Do not invent scores, accuracy rates, or claims of improvement.

## 8. Evaluation record templates

### 8.1 Run information

| Field | Record |
| --- | --- |
| **Evaluation/run ID** |  |
| **Date and time** |  |
| **Evaluator(s)** |  |
| **Prompt version / hash** |  |
| **Model and configuration** |  |
| **Evaluation mode** | Controlled fixture / Live discovery |
| **Input profile / dataset version** |  |
| **Sources or snapshot date** |  |
| **Output file or record location** |  |

### 8.2 Scoring sheet

| ID | Dimension | Weight | Rating | Points | Evidence / rationale |
| --- | --- | --- | --- | --- | --- |
| **R1** | Factual integrity and non-fabrication | 20 | ___ / 4 | |  |
| **R2** | Evidence quality and source traceability | 15 | ___ / 4 | |  |
| **R3** | Eligibility and hard constraints | 15 | ___ / 4 | |  |
| **R4** | Application status and deadline accuracy | 10 | ___ / 4 | |  |
| **R5** | Profile interpretation and uncertainty | 10 | ___ / 4 | |  |
| **R6** | Financing and use-of-funds compatibility | 10 | ___ / 4 | |  |
| **R7** | Financial calculations and funding gap | 5 | ___ / 4 | |  |
| **R8** | Scoring and ranking consistency | 5 | ___ / 4 | |  |
| **R9** | Actionability and decision support | 5 | ___ / 4 | |  |
| **R10** | Completeness, clarity, and output compliance | 5 | ___ / 4 | |  |
| **TOTAL** | | 100 | — | ___ / 100 |  |

### 8.3 Critical-failure record

| Field | Record |
| --- | --- |
| **Failure ID (CF1–CF7)** |  |
| **Status** | Confirmed / Not confirmed / Unresolved |
| **Exact output passage** |  |
| **Supporting evidence / source** |  |
| **Why material** |  |
| **Required correction** |  |

### 8.4 Test-case result record

| Field | Record |
| --- | --- |
| **Test-case ID / title** |  |
| **Expected behavior (predefined)** |  |
| **Observed model behavior** |  |
| **Result** | Pass / Partial pass / Fail / Not tested |
| **Evidence and notes** |  |
| **Root cause / follow-up** |  |

### 8.5 Final assessment

| Field | Record |
| --- | --- |
| **Weighted score** | ___ / 100 |
| **Performance band** |  |
| **Critical failure confirmed?** | Yes / No / Unresolved |
| **Overall result** | PASS / FAIL / NEEDS REVISION |
| **Top strengths** |  |
| **Top failure modes** |  |
| **Required changes before retest** |  |
| **Retest date / version** |  |

## 9. Additional metrics to track

These metrics complement the rubric; they do not replace human review or the critical-failure gate. Define the denominator consistently and retain examples behind each reported metric.

| Metric | Suggested definition |
| --- | --- |
| **Eligibility precision** | Correctly classified eligible opportunities ÷ all opportunities classified as eligible. Requires a reliable reference determination. |
| **Evidence coverage** | Material claims supported by appropriate evidence ÷ total material claims assessed. |
| **Critical error rate** | Runs with one or more confirmed critical failures ÷ total evaluated runs. |
| **Deadline/status accuracy** | Correctly reported status/deadline assessments ÷ status/deadline assessments with a verifiable reference. |
| **Funding-gap accuracy** | Correct funding-gap calculations ÷ calculations assessed, with cash/in-kind and currency treatment checked. |
| **Duplicate rate** | Duplicate opportunity records retained in final shortlist ÷ total shortlisted records, using a documented duplicate definition. |
| **Eligibility disqualification recall** | Known ineligible cases correctly flagged as ineligible ÷ all known ineligible cases in the reference set. |
| **Financing compatibility** | Cases where the financing type and material conditions are represented correctly ÷ cases assessed. |
| **Actionability coverage** | Shortlisted opportunities with a specific, relevant next action ÷ total shortlisted opportunities. |

## 10. Comparing baseline and improved prompts

- Run the baseline and improved prompt on the same fixed inputs, with the same source evidence and comparable tool access.
- Compare total score, each dimension, critical failures, and task-specific metrics. A higher total score should not conceal a new critical failure.
- Use the same rating anchors and record evidence for both versions.
- Where feasible, use two independent evaluators, then reconcile differences with written reasons. Small samples should be interpreted cautiously; transparent disagreement analysis is more useful than overstated statistical certainty.
- Use a separate holdout set for final checks when possible. Do not keep modifying the prompt only to pass a small set of known cases.
- Publish only actual observed results and disclose the number and type of cases tested, the evaluation date, and the limitations.

## 11. Limitations

This rubric is a proposed evaluation instrument for a funding-discovery prototype. Its weights, thresholds, and anchors should be calibrated as real evaluation evidence accumulates. A score reflects performance on the cases and evidence reviewed; it does not guarantee complete coverage of funding programs, legal eligibility, successful applications, or funding awards. Live opportunity information changes over time, so current status and deadline claims must be checked against current sources.

AI Funding Discovery Evaluation Rubric | Version 1.0
