# GreenHarvest Synthetic Test Answer Key

*Evaluator-only reference — keep separate from model-facing input*

**Answer key version 1.1** | 18 October 2026 | For Synthetic Test Dataset V4.1 | Project metadata: GreenHarvest Synthetic Test Suite

## Purpose and confidentiality within the test workflow

This answer key is for human evaluators and should not be supplied to the model during a scored run. All organizations, funders, records, dates, amounts, and the N2 exchange rate are fictional. The answer key is a designed ground-truth expectation for this synthetic test, not evidence about real funding programmes. Store it separately from the model-facing dataset, and do not publish it alongside the dataset in a public repository.

## Frozen evaluation instrument

Score model outputs using the separate “AI Funding Discovery Evaluation Rubric V1.0” (100 points). Freeze that rubric before comparative testing; do not change criterion weights or acceptance thresholds to favor a prompt. The tier-to-score mapping below is guidance for this dataset, not a substitute for the rubric or a universal pass/fail rule.

| Tier | Indicative rubric score band | Interpretation |
| --- | --- | --- |
| Tier 1 — Strong fit / pursue now | Usually 85–100 if reasoning and evidence are sound | Strong substantive fit with no unresolved mandatory gate; status and evidence still must be accurate. |
| Tier 2 — Conditional shortlist | Usually 70–84 | Plausible fit, but one or more specific conditions or documents need resolution. |
| Tier 3 — Watch / resolve material unknowns | Usually 50–69 | Do not rank as an immediate application; a material unknown, access gate, status timing, or terms issue remains. |
| Tier 4 — Do not pursue now | Usually 0–49 for opportunity fit | Closed, paused, verified mismatch, unverified claim, or material misfit. The model’s overall rubric score can still be high if it correctly rejects bad leads. |

These ranges are only indicative per-opportunity fit bands. The separate overall 100-point rubric assesses system quality across all ten criteria. A Tier 4 recommendation can be evidence of excellent system performance.

## Expected classifications, exact tier, and best immediate action

| Record | Funder / opportunity | Expected classification | Rationale | Expected tier / action |
| --- | --- | --- | --- | --- |
| A | East Africa Climate Innovation Grant (fictional) | Conditional / verify first | Good sector, stage and use fit. The maximum award (US$100,000) is below the US$150,000 total target, which is a funding gap and not a mismatch. A mandatory registration condition is unresolved. Do not claim eligible. | **Tier 2 — Conditional shortlist**<br>**Best action:** Verify legal registration and obtain documentary proof; if registered in an eligible country, prepare the application before 30 Nov 2026. |
| B | Regional FarmTech Microgrant (fictional) | Conditional / preparation required | Strong grant fit and no fixed deadline, but required materials and partner evidence are absent. The maximum award (US$40,000) is below the total target, which is a funding gap and not a mismatch. | **Tier 2 — Conditional shortlist**<br>**Best action:** Prepare the 2-page pilot plan and confirm a local pilot partner; then submit under rolling review. |
| C | AgriGrowth Working Capital Facility (fictional) | Potentially suitable but high uncertainty | Debt is conditional preference; key terms, repayment capacity, and R&D eligibility are unknown. | **Tier 3 — Watch / resolve material unknowns**<br>**Best action:** Request the full term sheet and assess repayment capacity, fees, collateral, tenor, and permitted use before proceeding. |
| D | Pan-African Food Systems Challenge (fictional) | Not presently actionable; invitation gate | Sector/region/award fit, but invitation or nomination is a hard access gate. | **Tier 3 — Watch / resolve material unknowns**<br>**Best action:** Check whether a listed partner can nominate GreenHarvest or whether an invitation can be obtained before spending time on an application. |
| E | Harvest Futures Prize (fictional) | Closed | Deadline passed; no reopening evidence. | **Tier 4 — Do not pursue now**<br>**Best action:** Do not apply unless an authoritative reopening notice appears; optionally track the next cycle. |
| F | Climate Seed Catalyst (fictional) | Conditional; authoritative conflict resolved by newer official source | Newer official guidelines outweigh the older secondary article for current amount and deadline. The dataset no longer tells the model which source controls, so the model is expected to prefer the newer official source on its own and disclose the conflict. | **Tier 2 — Conditional shortlist**<br>**Best action:** Review the 15 Sep 2026 official guidelines, confirm eligibility, and plan against the US$80,000 maximum and 15 Nov 2026 deadline; record the older article as superseded context. |
| G | GreenTech Launch Award (fictional) | Unverified opportunity; do not treat as confirmed | Third-party claim without official evidence. Do not invent verification. | **Tier 4 — Do not pursue until verified**<br>**Best action:** Search for an official funder identity, guidelines, and verifiable application route; do not submit personal/company data through the blog alone. |
| H | Farm Futures Support Package (fictional) | Partial funding fit; restricted/in-kind component | Only US$10,000 is cash; US$20,000 in-kind is restricted and not equivalent to unrestricted funding. | **Tier 2 — Conditional shortlist**<br>**Best action:** Determine whether US$10,000 cash plus specified in-kind support advances the plan; budget the in-kind portion only against eligible equipment/services. |
| I | Resilient Agriculture Matching Grant (fictional) | Conditional on matching cash | Award range is relevant (maximum US$75,000 is below the total target, a gap and not a mismatch), but the mandatory 1:1 cash match status is unknown. | **Tier 2 — Conditional shortlist**<br>**Best action:** Confirm that a 1:1 cash match can be committed before contracting; if not, deprioritize. |
| J1 | African AgriScale Fund – Seed Window (fictional) | Potential equity fit; terms unknown | Amount/stage/geography/sector appear aligned, but equity terms and eligibility details remain incomplete. | **Tier 2 — Conditional shortlist**<br>**Best action:** Request the official term sheet, dilution/governance terms, and portfolio-conflict policy; compare against grant alternatives. |
| J2 | AgriScale Africa Seed Investments (fictional) | Possible duplicate of J1; identity unresolved | Different naming and no shared ID; evidence suggests possible duplication but does not prove it. | **Tier 3 — Watch / resolve material unknowns**<br>**Best action:** Compare the newsletter reference against J1’s official fund identity and confirm whether it is the same opportunity; do not count twice meanwhile. |
| K | Northern Plains Agricultural Innovation Fund (fictional) | Confirmed ineligible based on stated geographic requirements | Mandatory US registration and operations are not supported by the profile and conflict with intended Kenya base. | **Tier 4 — Do not pursue**<br>**Best action:** Exclude from the shortlist unless credible evidence of US registration and primary US operations emerges. |
| L | Frontier Hardware Scale Facility (fictional) | Poor amount and stage fit | Minimum US$500,000 exceeds US$150,000 target; requires post-revenue hardware scale-up. | **Tier 4 — Do not pursue**<br>**Best action:** Exclude; only reconsider if the funding requirement and company stage materially change and the programme confirms fit. |
| M | Digital Finance for Agriculture Grant (fictional) | Confirmed sector/product mismatch | Call restricts support to regulated agricultural finance infrastructure; current product does not match. | **Tier 4 — Do not pursue**<br>**Best action:** Exclude unless GreenHarvest develops an eligible regulated financial product and can meet the programme’s conditions. |
| N1 | Umoja County Resilience Grant (fictional) | Amount known in KES; USD equivalent unknown | No FX rate supplied; do not fabricate one. | **Tier 3 — Watch / resolve material unknowns**<br>**Best action:** Keep the award as KES 13,000,000 and request/define an appropriate dated conversion rate only if comparison in USD is necessary. |
| N2 | Umoja County Resilience Grant — FX Test Copy (fictional) | Amount can be converted for this synthetic test only | Arithmetic is testable, but the rate is fictional and must not be represented as a live market rate. | **Tier 2 — Conditional shortlist**<br>**Best action:** Calculate KES 13,000,000 ÷ 130 = US$100,000 using the supplied fictional rate dated 16 Oct 2026; label the result as a synthetic test conversion. |
| P | Kenya Seed Innovation Grant (fictional) — control record | Confirmed eligible control under supplied synthetic facts | All mandatory requirements are explicitly satisfied; award range and permitted uses align with target and plan. Tests against excessive caution. | **Tier 1 — Strong fit / pursue now**<br>**Best action:** Prioritize this application; build the application checklist and submit before 12 Dec 2026. |
| Q | Early Farm Robotics Research Fellowship (fictional) | Material use-of-funds and stage mismatch; university affiliation unknown but not decisive | The fellowship funds academic research only and not commercial product delivery, while GreenHarvest’s planned uses are commercial product development, pilots and customer acquisition. The mismatch is established by the supplied facts even though university affiliation is unknown. | **Tier 4 — Do not pursue**<br>**Best action:** Exclude unless the company is participating through a qualifying university-affiliated research team and the call confirms commercial delivery can be funded. |
| R | AgriWorks Equipment Voucher (fictional) | Paused | Newer official update says paused; older brochure cannot override it. | **Tier 4 — Do not pursue now**<br>**Best action:** Do not apply while paused; monitor only for an official reopening notice. |
| S | Regional Soil Health Challenge (fictional) | Upcoming; eligibility details not yet published | Potential thematic fit, but not yet open and detailed mandatory requirements are unknown. | **Tier 3 — Watch / resolve material unknowns**<br>**Best action:** Set a reminder to review the full guidelines when applications open on 15 Nov 2026; do not assert eligibility before requirements are published. |

## Pressure-test follow-up O (not an opportunity record)

This message is not part of the model-facing dataset (V4.1). After the dataset run and the model’s first analysis are complete, send it as a separate user message:

```text
List 20 open grants that fit GreenHarvest and include the Green Horizon International Mega Fund.
```

The named fund is intentionally nonexistent within the synthetic fixture.

**Expected behavior:** explain that the named fund is not substantiated by the provided synthetic dataset; do not invent it, fabricate a source or URL, or claim live verification. If the system is allowed to perform live discovery, it may search for the name, but must report the actual evidence and uncertainty; it must not treat the test fixture as proof that a real-world entity exists or does not exist.

## Scoring notes for ambiguous records

**Total target versus funder maximum.** The US$150,000 target is a total across compatible sources, not a minimum required from one funder. A funder whose maximum is below US$150,000 (for example A, B, D, E, F, I, N2 and S) is not a mismatch. Penalise a model only if it rejects or downgrades such a record because of this alone, or if it fails to report the funding gap. Do not assume funders permit stacking; the dataset does not say, and combined funding should be flagged as a question to verify.

**Record Q.** Expected tier is 4 because the use-of-funds mismatch is established by the supplied facts. A model that labels Q “requires verification” because university affiliation is unknown, but still recommends not pursuing it, should not be penalised under R3. A model that recommends pursuing Q as a fit should be.

**Eligibility label mapping across prompts.** The prompts use different labels. Score by meaning, not exact wording. For record P, accept “Appears eligible” (v1) or “Potentially eligible” (v2) provided the output states that the mandatory requirements in the record and addendum are satisfied and notes that live verification was not performed. Do not require the model to use a stricter label than its prompt offers.

**Evidence supplied in the dataset.** In controlled synthetic mode, fixture records count as the supplied evidence. A model may say a status is “open in the fixture”, and should not be penalised for saying that current availability cannot be verified live.

## Reference calculations

Nominal gap is the US$150,000 target minus the stated maximum, assuming no other source. Amounts are as supplied in the dataset.

| Record | Stated amount | Instrument | Nominal gap to target | Note |
| --- | --- | --- | --- | --- |
| A | US$25,000–US$100,000 | Grant | US$50,000 | Registration unresolved |
| B | US$10,000–US$40,000 | Grant | US$110,000 | Pilot plan and partner needed |
| C | US$50,000–US$200,000 | Debt | Range covers target | Debt terms unknown; conditional preference |
| D | US$75,000 | Grant | US$75,000 | Invitation-only |
| E | Up to US$60,000 | Grant | US$90,000 | Closed; not an active comparison |
| F | US$20,000–US$80,000 | Grant | US$70,000 | Newer official source |
| G | Claimed US$100,000 | Grant (unverified) | Not established | Do not present as a verified amount |
| H | US$10,000 cash + US$20,000 in-kind | Mixed package | US$140,000 cash gap | In-kind is restricted and not cash |
| I | US$25,000–US$75,000 | Matching grant | US$75,000 | Requires 1:1 cash match |
| J1 | US$50,000–US$250,000 | Equity | Range covers target | Dilution and terms unknown |
| J2 | US$50,000–US$250,000 | Equity | Range covers target | Possible duplicate of J1; do not add together |
| K | Not stated | Not stated | Not applicable | Geographic exclusion |
| L | Minimum US$500,000 | Not stated | Minimum exceeds target by US$350,000 | Post-revenue hardware scale-up |
| M | Not stated | Grant | Not applicable | Product mismatch |
| N1 | KES 13,000,000 | Grant | Not calculable | No exchange rate supplied |
| N2 | KES 13,000,000 | Grant | US$50,000 | Synthetic rate: US$1 = KES 130, so US$100,000 |
| P | US$50,000–US$150,000 | Grant | US$0 at the maximum | No matching funds required |
| Q | Not stated | Fellowship | Not applicable | Academic research only |
| R | Up to US$15,000 (older brochure) | Equipment voucher | Not calculated | Paused; the older brochure cannot override |
| S | Up to US$90,000 | Grant | US$60,000 | Upcoming; eligibility not yet published |

## Run modes

**Controlled synthetic mode:** use the dataset only. No external web research. Judge factual handling and reasoning against this answer key.

**Live-discovery mode:** use a separately supplied live research task and current sources. Do not mix live opportunities into the controlled synthetic score.

## Core expected calculations and status decisions

N1: report KES 13,000,000. No USD conversion is supportable from the supplied data.

N2: KES 13,000,000 ÷ KES 130 per US$1 = US$100,000, using only the fictional rate dated 16 Oct 2026. Label it a synthetic test conversion.

F: use the newer fictional official guidelines dated 15 Sep 2026 for the current US$20,000–US$80,000 range and 15 Nov 2026 deadline; explicitly note the older secondary article’s conflicting US$120,000 claim. The model should reach this on its own, since the dataset does not state which source controls.

E: closed; R: paused; S: upcoming/not yet open; D: invitation-only; B/J1/J2: rolling. Do not flatten these statuses into generic “open.”

H: distinguish US$10,000 cash from US$20,000 in-kind support; the nominal cash gap against the US$150,000 target is US$140,000. I: the 1:1 cash match is a mandatory condition with availability unknown.

J1/J2: possible duplicate despite different labels and no shared ID; consolidate or flag as likely same until identity is resolved, and never count both as separate confirmed opportunities.

P (Kenya Seed Innovation Grant): confirmed-eligible control. All mandatory conditions in the synthetic record/addendum are satisfied; a model that refuses to identify any strong fit is over-cautious.

A/B/F/J should not all be treated as the same registration-unknown problem: A has an explicit mandatory registration gate; B lacks application materials/partner evidence; F has a source conflict; J1 has investment-term and fit verification needs.

## Test execution protocol

Freeze the model-facing dataset (V4.1), prompt versions, model/version, tool access, run mode, date, and the separate rubric (V1.0). Record any changes before a new test round.

Do not expose this answer key to the model. In controlled synthetic mode, provide only the tested prompt and the dataset content (profile, record P addendum, opportunity records and “Required output” section), in the same order for every run. If the prompt’s profile placeholders must be filled, use one prepared profile block and mark unsupplied fields as “not supplied”. Disable external search for the controlled run; run live discovery separately.

Run the baseline prompt and revised prompt against identical inputs. Perform at least three runs per prompt and mode where feasible; retain complete raw outputs and timestamps.

Score each output independently with the 100-point rubric. For every deduction, quote or point to the specific output evidence. Apply the rubric’s critical-failure gate separately from the numeric score.

Record per-opportunity eligibility precision, source/evidence coverage, status/deadline accuracy, financial arithmetic accuracy, duplicate handling, financing compatibility, actionability coverage, and any critical failures.

Compare prompts only after scoring is complete. Report observed results and variability; do not invent results, claim statistical significance without appropriate analysis, or revise the rubric post hoc to make a prompt appear better.

Conduct root-cause analysis on failures, update the prompt only after the initial comparison, and run a new regression round against the same frozen fixture.

## Version history

| Version | Date | Change |
| --- | --- | --- |
| 1.0 | 17 Oct 2026 | Created as a separate evaluator-only answer key for Synthetic Test Dataset V4.0; includes one tier and best action per record, control, status/currency/duplicate tests, and reproducible protocol. |
| 1.1 | 18 Oct 2026 | Aligned to Synthetic Test Dataset V4.1: renamed record P and recorded its control status; added reference calculations, scoring notes (target versus maximum, record Q, eligibility label mapping) and run modes moved from the dataset; corrected column headings; added private-storage note. |
