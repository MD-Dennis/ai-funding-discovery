# V2 Improved Prompt — Exploratory Evaluation

**Project:** AI Funding Discovery and Matching  
**Prompt version:** V2.0  
**Test organisation:** GreenHarvest Innovations Ltd (fictional)  
**Dataset:** GreenHarvest Synthetic Funding Discovery Test Dataset v4.1  
**Evaluation rubric:** AI Funding Discovery Evaluation Rubric v1.0  
**Evaluation mode:** Controlled synthetic evaluation — no live web research

**Evaluation status: Exploratory; not a formal benchmark.**

This report documents an initial evaluation of the V2 funding-discovery prompt against the GreenHarvest Synthetic Test Dataset v4.1. The run was conducted in controlled synthetic mode without live web research. The provisional score reflects one exploratory assessment and should not be interpreted as a validated performance result or evidence that V2 outperforms V1. The evaluator answer key was available in the broader evaluation context, so this was not a clean, blind run. A formal comparison requires identical inputs and settings, multiple runs where feasible, retained raw outputs, and independent scoring against the frozen rubric.

## 1. Evaluation setup and limitations

I retrieved the V2 prompt, synthetic dataset, evaluator answer key, and evaluation rubric.

The run below applies V2 to the 19 synthetic opportunity records, A–S, with J1 and J2 treated as separate records. It preserves the fictional status of every funder and programme and does not treat any opportunity as a real-world funding lead. The dataset itself states that all organisations, funders, sources, dates, and the N2 exchange rate are fictional. greenharvest-synthetic-test-dat…

**Important limitation:** The answer key was available in the broader evaluation context while preparing this run. Consequently, this is a useful **exploratory evaluation, but not a clean, blind model run**. The output should not be represented as independent benchmark evidence. A formal evaluation should be repeated with only the prompt and model-facing dataset supplied to the model, while the answer key remains evaluator-only.

---

# Part 1 — V2 exploratory run

## 2. Executive summary

GreenHarvest Innovations Ltd is a fictional early-stage B2B agritech and climate-technology venture seeking **US$150,000 in total external funding over 6–12 months**. Grants and equity are preferred; debt is conditional on suitable terms and affordability.

Its legal registration status is unknown in the general profile. The organisation's revenue, financial statements, matching-fund availability, founder characteristics, and quantified climate-impact results are also unknown.

The most important conclusion is that **the Kenya Seed Innovation Grant (P) is the strongest candidate in the supplied evidence**. Its record explicitly satisfies the relevant eligibility requirements for the P control scenario.

Other opportunities warrant different levels of attention:

- **Prepare or pursue conditionally:** B, A, F, J1, H, I and N2.
- **Investigate before making a financing decision:** C, D, J2 and N1.
- **Monitor for a future opening:** S.
- **Do not pursue in the current state:** E, G, K, L, M, Q and R.

These categories reflect the supplied fictional evidence, not real-world funding availability.

### Profile facts and unresolved information

| Dimension | Finding | Evidence status |
|---|---|---|
| Sector | Agritech and climate technology | Supplied |
| Business model | B2B | Supplied |
| Stage | Seed/early stage; prototype and limited pilots | Supplied |
| Legal registration | Intends to register in Kenya; actual registration not established in the general profile | Unknown |
| Funding target | US$150,000 total over 6–12 months | Supplied |
| Preferred financing | Grants and equity; debt only if suitable | Supplied |
| Planned uses | Product development, pilots, customer acquisition and expansion | Supplied |
| Matching funds | Availability unknown | Unknown |
| Revenue and repayment capacity | Not supplied | Unknown |
| Founder and team eligibility characteristics | Not supplied | Unknown |

**Important exception:** Record P includes its own explicit profile addendum confirming Kenyan legal registration on 12 August 2026 and a prototype with two documented pilot deployments. These facts apply to record P only; they must not be generalised to other records.

## 3. Ranked conditional shortlist

The ranking below reflects practical priority, not a guarantee of eligibility or funding. A high position does not override unresolved conditions.

| Rank | Record and opportunity | Eligibility assessment | Status in synthetic dataset | Maximum award | Funding gap or limitation | Immediate action |
|---:|---|---|---|---|---|---|
| 1 | **P — Kenya Seed Innovation Grant** | Appears eligible under the supplied P-specific facts | Open; deadline 12 Dec 2026 | US$150,000 | US$0 at maximum award | Prioritise application preparation and confirm required submission materials. |
| 2 | **B — Regional FarmTech Microgrant** | Requires preparation; relevant requirements remain outstanding | Rolling; reviewed monthly | US$40,000 | US$110,000 nominal gap | Prepare the two-page pilot plan and confirm a local pilot partner. |
| 3 | **A — East Africa Climate Innovation Grant** | Conditional; legal registration is a mandatory unresolved gate | Open; deadline 30 Nov 2026 | US$100,000 | US$50,000 nominal gap | Confirm and document legal registration in an eligible country before investing heavily in the application. |
| 4 | **F — Climate Seed Catalyst** | Requires eligibility confirmation; current programme details are supported by conflicting sources | Open in the newer official guidelines; deadline 15 Nov 2026 | US$80,000 | US$70,000 nominal gap | Use the 15 Sep 2026 official guidelines as the primary reference, document the older conflicting claim, and confirm eligibility. |
| 5 | **J1 — African AgriScale Fund – Seed Window** | Potential equity fit; terms and other conditions remain unknown | Rolling | US$250,000 | Award range covers the target; actual investment and terms are unknown | Request the official term sheet and review dilution, governance rights and portfolio conflicts. |
| 6 | **N2 — Umoja County Resilience Grant — FX Test Copy** | Potentially relevant; local eligibility details need confirmation | Open in synthetic dataset; deadline 28 Nov 2026 | KES 13,000,000 | US$50,000 nominal gap using the supplied synthetic rate | Confirm geographic and programme eligibility; use the supplied fictional exchange rate only for this test. |
| 7 | **H — Farm Futures Support Package** | Partial funding fit; cash and in-kind components must be assessed separately | Open; deadline 25 Nov 2026 | US$10,000 cash plus US$20,000 in-kind | US$140,000 cash gap | Determine whether the restricted equipment/services are useful and budget them only against permitted costs. |
| 8 | **I — Resilient Agriculture Matching Grant** | Conditional on ability to provide a 1:1 cash match | Open; deadline 5 Dec 2026 | US$75,000 | US$75,000 nominal gap, plus matching requirement | Confirm whether the required cash match can be committed before contracting. |

**How to interpret this shortlist:** P is the only record whose supplied evidence explicitly establishes all the listed eligibility conditions for GreenHarvest. Several other records are worth preparing for or investigating, but they are not confirmed eligible merely because they appear relevant.

The award maximum is not the same as funding secured. The US$150,000 target is a total funding requirement, not a minimum that every individual funder must meet. Award stacking must not be assumed.

## 4. Opportunities requiring verification

These opportunities should not be treated as confirmed recommendations until the relevant questions are resolved.

| Record | Opportunity | Main issue | Recommended next step |
|---|---|---|---|
| C | AgriGrowth Working Capital Facility | Debt terms, repayment capacity, and eligibility of product R&D are unknown. | Request the full term sheet and assess interest, fees, collateral, tenor, repayment schedule, underwriting criteria and permitted uses. |
| D | Pan-African Food Systems Challenge | An invitation code or nomination from a listed partner is required; no invitation is established. | Determine whether an eligible partner can nominate GreenHarvest before preparing a full application. |
| J2 | AgriScale Africa Seed Investments | It may be the same investment opportunity as J1, but the identity is unresolved. | Compare the newsletter details with J1's official fund identity. Do not count both as separate confirmed opportunities. |
| N1 | Umoja County Resilience Grant | Award is KES 13,000,000, but no exchange rate is supplied. Local eligibility requirements need clarification. | Preserve the amount in KES and establish a defensible dated conversion rate only if USD comparison is required. |

### Special case: F and conflicting evidence

The dataset contains two different claims for Climate Seed Catalyst:

- Official fictional guidelines dated **15 September 2026**: awards of US$20,000–US$80,000, with applications closing 15 November 2026.
- Secondary fictional article dated **10 February 2025**: awards up to US$120,000 and an earlier application window.

The newer official guidelines should be the primary basis for the current award range and deadline. The older article should be recorded as conflicting historical information rather than silently combined with the newer details.

### Special case: J1 and J2

J1 and J2 must not be counted as two confirmed investment options until their identities are resolved.

The names and source types differ, but the investment ranges, geography and sector are similar. The correct conclusion is **possible duplicate**, not confirmed duplicate and not definitely separate opportunities.

## 5. Excluded and non-actionable opportunities

| Record | Opportunity | Classification | Reason |
|---|---|---|---|
| E | Harvest Futures Prize | Closed | The supplied deadline was 31 August 2026, and no reopening notice is included. |
| G | GreenTech Launch Award | Unverified opportunity | Only a third-party blog claim is supplied; no official funder page, guidelines, legal entity or verifiable application route is provided. |
| K | Northern Plains Agricultural Innovation Fund | Ineligible on the supplied profile | Requires US registration and primary US operations, neither of which is established for GreenHarvest. |
| L | Frontier Hardware Scale Facility | Poor stage and amount fit | Minimum ticket is US$500,000, and the programme targets post-revenue manufactured hardware scale-up. |
| M | Digital Finance for Agriculture Grant | Sector/product mismatch | It supports regulated agricultural finance products, not the general farm-management and irrigation technology described in the profile. |
| Q | Early Farm Robotics Research Fellowship | Material use-of-funds mismatch | It funds university-affiliated academic research, not commercial company product delivery. University affiliation is unknown, but that uncertainty does not remove the stated commercial-use mismatch. |
| R | AgriWorks Equipment Voucher | Paused | The newer official update says applications are paused. The older brochure does not establish that applications have reopened. |

These records should not be included in the recommended funding shortlist. They can remain in the report to document the screening decisions.

## 6. Upcoming opportunity

| Record | Opportunity | Status | Award | Immediate action |
|---|---|---|---|---|
| S | Regional Soil Health Challenge | Upcoming; expected opening 15 Nov 2026 and closing 15 Jan 2027 | Up to US$90,000 | Review the full guidelines when published. Do not assert eligibility before the mandatory requirements are available. |

S has potential thematic relevance, but its detailed eligibility rules are not yet supplied. The correct action is to monitor the opening and assess the published requirements—not to treat it as an open grant today.

---

## 7. Financial calculations

The calculations below use the US$150,000 total funding target and the award information supplied in the synthetic dataset. They are nominal comparisons, not predictions of award success.

| Record | Award or amount | Calculation | Nominal funding gap |
|---|---|---|---:|
| A | Up to US$100,000 | US$150,000 − US$100,000 | US$50,000 |
| B | Up to US$40,000 | US$150,000 − US$40,000 | US$110,000 |
| C | US$50,000–US$200,000 debt facility | Range includes US$150,000; terms unknown | Not a simple fixed gap |
| D | US$75,000 grant | US$150,000 − US$75,000 | US$75,000 |
| E | Up to US$60,000 | US$150,000 − US$60,000 | US$90,000; closed |
| F | Up to US$80,000 | US$150,000 − US$80,000 | US$70,000 |
| G | Claimed US$100,000 | Amount is unverified | Not established |
| H | US$10,000 cash + US$20,000 in-kind | US$150,000 − US$10,000 cash | **US$140,000 cash gap** |
| I | Up to US$75,000 | US$150,000 − US$75,000 | US$75,000, plus required match |
| J1 | US$50,000–US$250,000 equity | Range includes US$150,000; terms unknown | Not a simple fixed gap |
| J2 | US$50,000–US$250,000 equity | Possible duplicate of J1 | Do not count separately |
| L | Minimum US$500,000 | US$500,000 − US$150,000 | Minimum exceeds target by US$350,000 |
| N1 | KES 13,000,000 | No exchange rate supplied | USD gap cannot be calculated |
| N2 | KES 13,000,000 | KES 13,000,000 ÷ 130 | US$100,000 converted amount; US$50,000 gap |
| P | Up to US$150,000 | US$150,000 − US$150,000 | US$0 at maximum |
| S | Up to US$90,000 | US$150,000 − US$90,000 | US$60,000 |

### Currency conversion for N2

The supplied fictional rate is:

**US$1 = KES 130**, dated 16 October 2026.

Therefore:

KES 13,000,000 ÷ 130 = **US$100,000**.

This is a synthetic test calculation, not a live exchange-rate quote.

For N1, no conversion is justified from the supplied evidence. Its amount should remain **KES 13,000,000**.

### Financial interpretation

- **H:** Only US$10,000 is cash. The US$20,000 in-kind component cannot be treated as unrestricted cash or used to reduce the cash funding gap.
- **I:** The nominal gap is US$75,000 at the maximum award, but GreenHarvest must also satisfy the 1:1 cash-match requirement. The availability of matching funds is unknown.
- **C:** Although the facility's range includes the funding target, its repayment terms and GreenHarvest's repayment capacity are unknown. A debt facility should not be treated as equivalent to a grant.
- **J1:** The investment range includes the funding target, but the amount invested, dilution and other terms are unknown.
- **P:** A zero nominal gap is possible only at the maximum award of US$150,000. It does not mean the funding has been awarded.
- **Award stacking:** No combined total should be presented as available funding unless compatibility and stacking rules are established.

---

## 8. V2 scoring demonstration

V2 requires seven component ratings, weighted points, and a final calculation. The weights are:

| Dimension | Weight |
|---|---:|
| Sector and activity alignment | 20% |
| Geographic eligibility alignment | 15% |
| Development-stage alignment | 15% |
| Funding amount and financial fit | 15% |
| Use-of-funds alignment | 15% |
| Financing-instrument compatibility | 10% |
| Timing and application practicality | 10% |

Weighted points are calculated as:

**Dimension weight × (rating ÷ 4)**

The ratings below are exploratory judgements based on the synthetic records. They are not externally validated measures of funding success.

### Record P — Kenya Seed Innovation Grant

| Dimension | Weight | Rating | Weighted points | Reason |
|---|---:|---:|---:|---|
| Sector and activity alignment | 20 | 4 | 20.00 | Agritech and climate-tech eligibility is explicit. |
| Geographic eligibility alignment | 15 | 4 | 15.00 | Kenyan registration is confirmed for this control scenario, and Kenya is eligible. |
| Development-stage alignment | 15 | 4 | 15.00 | Seed-stage ventures with prototypes or pilots are eligible. |
| Funding amount and financial fit | 15 | 4 | 15.00 | Award range reaches the US$150,000 target. |
| Use-of-funds alignment | 15 | 4 | 15.00 | Product development and field pilots are permitted. |
| Financing compatibility | 10 | 4 | 10.00 | Grant financing is preferred, and no matching funds are required. |
| Timing and application practicality | 10 | 4 | 10.00 | Open in the fixture, with a stated deadline of 12 December 2026. |
| **Total** | **100** | | **100.00/100** | |

**Exploratory interpretation:** Strongest candidate. The supplied facts support pursuing the application, subject to preparing the required materials. This does not mean the fictional opportunity is real or that an award has been secured.

### Record B — Regional FarmTech Microgrant

| Dimension | Weight | Rating | Weighted points | Reason |
|---|---:|---:|---:|---|
| Sector and activity alignment | 20 | 4 | 20.00 | Agritech pilots are accepted. |
| Geographic eligibility alignment | 15 | 4 | 15.00 | Kenya is explicitly eligible. |
| Development-stage alignment | 15 | 4 | 15.00 | Pilot work and product refinement are accepted. |
| Funding amount and financial fit | 15 | 3 | 11.25 | The maximum award is below the total funding target, leaving a gap. |
| Use-of-funds alignment | 15 | 4 | 15.00 | Field testing and product refinement fit the planned uses. |
| Financing compatibility | 10 | 4 | 10.00 | Grant financing aligns with the preference. |
| Timing and application practicality | 10 | 3 | 7.50 | Rolling applications are available, but required materials and partner evidence are missing. |
| **Total** | **100** | | **93.75/100** | |

**Exploratory interpretation:** Strong thematic and practical fit. The next step is to prepare the required pilot plan and confirm a local pilot partner.

### Record A — East Africa Climate Innovation Grant

| Dimension | Weight | Rating | Weighted points | Reason |
|---|---:|---:|---:|---|
| Sector and activity alignment | 20 | 4 | 20.00 | Climate/agritech ventures are accepted. |
| Geographic eligibility alignment | 15 | Not assessable | — | Mandatory legal registration is not confirmed in the general profile. |
| Development-stage alignment | 15 | 4 | 15.00 | Pre-seed to seed ventures are eligible. |
| Funding amount and financial fit | 15 | 3 | 11.25 | The maximum award is US$100,000, leaving a nominal gap. |
| Use-of-funds alignment | 15 | 4 | 15.00 | Product development and field pilots are permitted. |
| Financing compatibility | 10 | 4 | 10.00 | Grant financing aligns with the preference. |
| Timing and application practicality | 10 | 3 | 7.50 | The deadline is 30 November 2026, but the registration gate remains unresolved. |
| **Assessable subtotal** | **85 assessable points** | | **78.75/85** | |

**Exploratory interpretation:** Conditional opportunity. The partial subtotal must not be compared directly with a fully assessed score of 100. Registration must be verified before GreenHarvest can be described as eligible.

### Record J1 — African AgriScale Fund – Seed Window

| Dimension | Weight | Rating | Weighted points | Reason |
|---|---:|---:|---:|---|
| Sector and activity alignment | 20 | 4 | 20.00 | Seed-stage agritech is explicitly targeted. |
| Geographic eligibility alignment | 15 | 4 | 15.00 | Kenya is included. |
| Development-stage alignment | 15 | 4 | 15.00 | Seed-stage ventures are targeted. |
| Funding amount and financial fit | 15 | 4 | 15.00 | The investment range includes the funding target. |
| Use-of-funds alignment | 15 | Not assessable | — | Specific permitted uses are not supplied. |
| Financing compatibility | 10 | 3 | 7.50 | Equity is preferred, but dilution and governance terms are unknown. |
| Timing and application practicality | 10 | 4 | 10.00 | Rolling applications are specified, although investment terms remain unresolved. |
| **Assessable subtotal** | **85 assessable points** | | **82.50/85** | |

**Exploratory interpretation:** Potential equity fit, but this partial score is not directly comparable with a fully assessed score. Request the term sheet before treating it as a practical financing option.

### Scoring limitation identified

The numeric scores are useful for showing how V2 applies its scoring rules, but the results also expose a weakness in the prompt: **it does not define a fully standardised method for comparing opportunities when some dimensions are unassessable.**

The prompt says to disclose scoring coverage, which is helpful, but it does not define a common normalisation method or a minimum coverage threshold for ranking. As a result, two partial scores can look similar while being based on different amounts of evidence.

For this exploratory run, I would not assign a definitive comparable numeric score to every candidate. That limitation should be documented rather than hidden.

---

# Part 2 — Evaluation of V2 against the rubric

## 9. Rubric scoring

The rubric scores the **quality of the output**, not the number of opportunities shortlisted. A correct rejection can demonstrate good performance.

The following is a provisional evaluator assessment of this exploratory output.

| Criterion | Weight | Rating / 4 | Points | Rationale |
|---|---:|---:|---:|---|
| R1. Factual integrity and non-fabrication | 20 | 4 | 20.00 | The output treats the dataset as fictional and does not invent real-world funders or URLs. |
| R2. Evidence quality and source traceability | 15 | 3 | 11.25 | It identifies the supplied evidence, dates, and source conflicts, but does not provide claim-level references or URLs. No URLs were supplied in the dataset. |
| R3. Eligibility and hard constraints | 15 | 4 | 15.00 | It preserves the registration gate for A, excludes K and M, and recognises the P control. |
| R4. Application status and deadline accuracy | 10 | 4 | 10.00 | It distinguishes closed, paused, rolling, invitation-only, open, and upcoming records. |
| R5. Profile interpretation and uncertainty | 10 | 4 | 10.00 | It preserves unknown legal status and other missing profile facts, while applying the P-specific addendum only to P. |
| R6. Financing and use-of-funds compatibility | 10 | 4 | 10.00 | It distinguishes debt, equity, grants, matching funds, and cash versus in-kind support. |
| R7. Financial calculations and funding gap | 5 | 4 | 5.00 | The stated nominal gaps and N2 conversion are correct; N1 is not converted without a rate. |
| R8. Scoring and ranking consistency | 5 | 2 | 2.50 | Some scoring is demonstrated, but unassessable dimensions make comparisons incomplete and the scoring method needs clearer calibration. |
| R9. Actionability and decision support | 5 | 4 | 5.00 | The output gives specific next actions and verification steps. |
| R10. Completeness, clarity, and output compliance | 5 | 4 | 5.00 | The report covers the required major sections and explains important limitations. |
| **Total** | **100** | | **93.75/100** | |

### Provisional result: 93.75/100 — Excellent band

**Critical-failure review:** No confirmed critical failure was identified in this exploratory output.

This is a provisional score assigned by one evaluator to one non-blind exploratory run. It is not a formal benchmark result, a validated measure of V2's performance, or evidence that V2 outperforms V1.

The high score should also be interpreted in context: V2 includes detailed instructions for most of the dimensions assessed, and the evaluation was prepared with the answer key available in the broader context. A clean, independent run could produce a different result.

## 10. Critical-failure checklist

| Failure | Finding | Reason |
|---|---|---|
| CF1 — Fabricated real-world opportunity | Not confirmed | All opportunities are explicitly treated as fictional test records. |
| CF2 — Fabricated source or URL | Not confirmed | No source URL or application route is invented. |
| CF3 — False eligibility assurance | Not confirmed | A is conditional; K and M are excluded; P is assessed using its specific addendum. |
| CF4 — False open status | Not confirmed | E remains closed, R remains paused, and S remains upcoming. |
| CF5 — Financing misrepresentation | Not confirmed | Debt, equity, grants, cash and in-kind support are distinguished. |
| CF6 — False verification claim | Not confirmed | No live source checks are claimed. |
| CF7 — Material financial misrepresentation | Not confirmed | The stated calculations are consistent with the supplied synthetic figures. |

---

# Part 3 — Findings and recommended improvements

## 11. What V2 handled well

### 1. Eligibility is separate from strategic fit

The output does not assume that a relevant sector is enough to establish eligibility. A's registration requirement remains unresolved, while K and M are excluded for material mismatches.

### 2. The P control is recognised

The output identifies P as the strongest candidate because its record explicitly satisfies the relevant conditions. This is important: an overly cautious assistant might incorrectly mark every opportunity as uncertain.

### 3. Status handling is specific

The output does not collapse every opportunity into a generic Open/Closed classification. It preserves rolling, invitation-only, paused and upcoming statuses.

### 4. Financial calculations are transparent

The output correctly distinguishes cash from in-kind support and does not invent a conversion rate for N1.

### 5. The recommendations are actionable

The output specifies what GreenHarvest should do next, rather than merely listing opportunity names and award amounts.

## 12. What needs improvement

| Issue | Why it matters | Recommended improvement |
|---|---|---|
| Incomplete scoring standardisation | Partial scores are not directly comparable with fully assessed scores. | Define a standard treatment for unassessable dimensions and a minimum evidence-coverage threshold before ranking by score. |
| No explicit opportunity-by-opportunity evidence ledger | A reader may find it difficult to trace every eligibility or status claim back to a specific record. | Require a compact evidence table with record ID, supplied source title/date, claim supported, and unresolved limitation. |
| Ranking can look more definitive than the evidence warrants | A ranked list can imply that all candidates are equally ready to pursue. | Separate *application readiness* from *strategic fit* and flag conditional candidates prominently. |
| Financing terms need an explicit decision gate | A large debt or equity range may look attractive even when the terms are unknown. | Require a “terms verified?” field and prohibit a firm financing recommendation until material terms are reviewed. |
| The output can become lengthy | Detailed scoring and evidence for every record may make the report difficult to use. | Put the executive shortlist first, followed by compact scoring and detailed exclusions. Keep the full audit trail in an appendix when appropriate. |

## 13. Recommended next steps

I recommend the following order:

1. **Keep V2 as a candidate prompt.** Do not label it a validated improvement.
2. **Record the exploratory findings.** Preserve the provisional score, scoring rationale, critical-failure checklist, and the limitation that the run was not blind.
3. **Consider a targeted V2.1 revision.** The highest-priority improvement is a reproducible scoring policy for unassessable dimensions and evidence coverage.
4. **Freeze the evaluation materials.** Keep the dataset, profile, prompt versions and rubric fixed for the comparison.
5. **Run a clean evaluation.** Supply the model with only the tested prompt and model-facing dataset; keep the answer key separate.
6. **Run V1 and V2 under comparable settings.** Use at least three runs per prompt where feasible, retain unedited outputs, and score each independently.
7. **Compare the results only after scoring.** Report observed scores, critical failures, consistency and limitations without assuming V2 is better.

## Final conclusion

**V2 is a promising candidate prompt, but its effectiveness has not yet been established.** This exploratory run suggests that it can structure a careful funding analysis, preserve important uncertainties, distinguish financing types and produce actionable recommendations. It also reveals a scoring-standardisation issue worth addressing.

The next defensible claim should come from a clean, controlled comparison against V1 using the same dataset and evaluation rubric—not from the exploratory score alone.
