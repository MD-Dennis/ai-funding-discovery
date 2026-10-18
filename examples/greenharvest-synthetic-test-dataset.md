# GreenHarvest Synthetic Funding Discovery Test Dataset

*Model-facing input only — no expected answers or ranking key*

**Version 4.0** | 17 October 2026 | Project metadata: GreenHarvest Synthetic Test Suite

## Document purpose and handling

This is a controlled synthetic test fixture for evaluating an AI funding-discovery assistant. Every organization, funder, programme, source record, date, and exchange rate in this document is fictional and created for testing. Nothing here is a real funding lead, and no real-world verification is implied.

This dataset intentionally contains missing facts, conflicting claims, uncertain eligibility, closed/paused/upcoming opportunities, different financing instruments, duplicate-like records, and a confirmed-fit control. Preserve uncertainty; do not fill gaps with assumptions.

## Synthetic company profile

| Field | Value |
| --- | --- |
| **Entity name** | GreenHarvest Innovations Ltd (fictional) |
| **Location / registration** | Intends to register in Kenya. Actual legal registration and incorporation status are not supplied. |
| **Sector** | Agritech and climate technology; precision irrigation, farm decision support, and post-harvest loss reduction. |
| **Business model** | B2B; intended customers include farmer cooperatives, agribusinesses, and agricultural service providers. |
| **Stage** | Seed / early stage; prototype and limited pilots. Revenue, traction, and audited financials are not supplied. |
| **Funding request** | US$150,000 total external funding target over 6–12 months. |
| **Preferred instruments** | Grants and equity preferred. Debt may be considered only if repayment terms and affordability are suitable. |
| **Planned uses** | Product development, field pilots, customer acquisition, and expansion. |
| **Other facts** | Team composition, founder demographics, ownership, matching-fund availability, climate-impact measurements, and prior funding are unknown unless a record below states otherwise. |

### Company profile addendum for control record P only

For the isolated P control scenario, use the explicit facts contained in record P: GreenHarvest was legally registered in Kenya on 12 Aug 2026 and has a prototype plus two documented pilot deployments. Do not generalize those extra facts to other records or scenarios.

## Opportunity records

Treat each row as a separate candidate record unless the evidence suggests a possible duplicate. A user may ask for an individual record analysis or provide a follow-up instruction after the dataset is loaded.

| Record | Funder / opportunity | Status & dates | Eligibility / terms / evidence |
| --- | --- | --- | --- |
| A | East Africa Climate Innovation Grant (fictional) | Open; deadline 30 Nov 2026 | Official fictional call notice dated 1 Oct 2026. Eligible applicants must be legally registered in Kenya, Uganda, or Tanzania; must be pre-seed to seed climate/agritech ventures; grant size US$25,000–US$100,000; permitted uses include product development and field pilots. Registration is a mandatory condition. No statement in the company profile confirms registration. |
| B | Regional FarmTech Microgrant (fictional) | Rolling applications; reviewed monthly | Fictional official programme page dated 20 Sep 2026. Eligible in Kenya; agritech pilots accepted; grant size US$10,000–US$40,000; permits field testing and product refinement. No fixed deadline. Requires a 2-page pilot plan and evidence of a local pilot partner; neither is provided in the profile. |
| C | AgriGrowth Working Capital Facility (fictional) | Open; deadline 15 Dec 2026 | Fictional lender product sheet dated 5 Oct 2026. Debt facility US$50,000–US$200,000. Interest rate, fees, collateral, tenor, repayment schedule, and underwriting criteria are not supplied in the record. Funds may be used for working capital; product R&D eligibility is unclear. Company revenue and repayment capacity are unknown. |
| D | Pan-African Food Systems Challenge (fictional) | Invitation-only; nominations accepted until 20 Nov 2026 | Fictional organizer page dated 28 Sep 2026. Accepts invited ventures operating in any African country; focus is food systems and agricultural resilience; award US$75,000 grant. Application requires an invitation code or nomination from a listed partner. GreenHarvest has no known invitation or nomination. |
| E | Harvest Futures Prize (fictional) | Closed; deadline was 31 Aug 2026 | Fictional official notice dated 1 Jun 2026 says applications closed on 31 Aug 2026. Grant up to US$60,000 for early-stage agricultural technology. No later reopening notice is included. |
| F | Climate Seed Catalyst (fictional) | Conflicting status/amount claims | Fictional official guidelines dated 15 Sep 2026 state grant size US$20,000–US$80,000 and applications close 15 Nov 2026. A fictional secondary article dated 10 Feb 2025 says awards can reach US$120,000 and describes an earlier application window. Treat the newer official guidelines as controlling for current amount/deadline unless newer authoritative evidence appears; disclose the discrepancy. |
| G | GreenTech Launch Award (fictional) | Open; deadline 10 Dec 2026 | A fictional third-party blog dated 3 Oct 2026 claims this is a US$100,000 grant for any African startup. No official funder page, guideline, legal entity, or verifiable application route is supplied. All stated eligibility and award details are unverified. |
| H | Farm Futures Support Package (fictional) | Open; deadline 25 Nov 2026 | Fictional official call dated 2 Oct 2026. Offers US$30,000 total support, split into US$10,000 cash and US$20,000 in-kind equipment/services. In-kind value cannot be used for payroll or unrestricted operating costs. The company’s stated target is US$150,000 external funding. |
| I | Resilient Agriculture Matching Grant (fictional) | Open; deadline 5 Dec 2026 | Fictional official guidelines dated 29 Sep 2026. Offers grants of US$25,000–US$75,000 but requires a 1:1 cash match committed before contracting. GreenHarvest’s matching-fund availability is unknown. |
| J1 | African AgriScale Fund – Seed Window (fictional) | Open; rolling applications | Fictional official fund page dated 1 Oct 2026. Equity investment US$50,000–US$250,000 for seed-stage agritech ventures in Kenya, Ghana, or Rwanda. Investment terms, ownership dilution, governance rights, and current portfolio conflicts are not supplied. |
| J2 | AgriScale Africa Seed Investments (fictional) | Open; rolling applications | Fictional ecosystem newsletter dated 6 Oct 2026 describes a seed investor called “AgriScale Africa” investing US$50,000–US$250,000 in Kenya/Ghana/Rwanda agritech ventures. No programme ID is shown; it may be the same investor/opportunity as J1, but the name and description differ and the newsletter is not the official source. Verify identity before counting separately. |
| K | Northern Plains Agricultural Innovation Fund (fictional) | Open; deadline 1 Dec 2026 | Fictional official guidelines dated 12 Sep 2026. Requires applicants to be legally registered in the United States and conduct primary operations in the US. GreenHarvest’s stated intended location is Kenya; no US registration or operations are supplied. |
| L | Frontier Hardware Scale Facility (fictional) | Open; deadline 20 Dec 2026 | Fictional official programme page dated 8 Oct 2026. Minimum ticket US$500,000, intended for post-revenue companies scaling manufactured irrigation hardware. GreenHarvest’s target is US$150,000; the profile describes early-stage software-enabled agritech and limited pilots. |
| M | Digital Finance for Agriculture Grant (fictional) | Open; deadline 18 Nov 2026 | Fictional official call dated 30 Sep 2026. Supports regulated digital lending, insurance underwriting, and agricultural credit infrastructure. Does not fund general farm-management software, irrigation controls, or post-harvest technology unless directly integrated into an eligible regulated finance product. GreenHarvest’s described product is not a regulated financial product. |
| N1 | Umoja County Resilience Grant (fictional) | Open; deadline 28 Nov 2026 | Fictional official county notice dated 4 Oct 2026. Award is KES 13,000,000 for qualifying local climate-adaptation pilots. The notice and test data provide no USD/KES exchange rate. Do not convert to USD without an explicitly supplied rate and date. |
| N2 | Umoja County Resilience Grant — FX Test Copy (fictional) | Open; deadline 28 Nov 2026 | Same fictional award terms as N1. For this isolated arithmetic test only, the fictional dataset supplies a rate dated 16 Oct 2026: US$1 = KES 130. Use this rate only for this test record and state that it is a synthetic test rate, not a live market quote. |
| P | Verified Fit Seed Grant (fictional control) | Open; deadline 12 Dec 2026 | Fictional official guidelines dated 7 Oct 2026 explicitly confirm: applicants legally registered in Kenya are eligible; seed-stage agritech/climate-tech ventures with prototypes or pilots are eligible; grant size US$50,000–US$150,000; product development and field pilots are permitted; no matching funds are required. For this control case only, the accompanying company profile addendum states: GreenHarvest was legally registered in Kenya on 12 Aug 2026 and has a prototype plus two documented pilot deployments. All mandatory requirements stated in this record and addendum are satisfied. |
| Q | Early Farm Robotics Research Fellowship (fictional) | Open; deadline 22 Nov 2026 | Fictional official call dated 5 Oct 2026. Requires university-affiliated research teams at the proof-of-concept research stage; funds academic research only and does not fund commercial company product delivery. GreenHarvest is described as a commercial B2B startup with a prototype and limited pilots; university affiliation is unknown. |
| R | AgriWorks Equipment Voucher (fictional) | Paused; no reopening date | Fictional official programme update dated 9 Oct 2026 says new applications are paused until further notice. An older fictional brochure dated 12 Apr 2026 lists vouchers up to US$15,000 for irrigation equipment. Do not describe the opportunity as currently open based on the older brochure. |
| S | Regional Soil Health Challenge (fictional) | Upcoming; applications not yet open | Fictional official announcement dated 11 Oct 2026 says the next call is expected to open 15 Nov 2026 and close 15 Jan 2027. It may fund climate-smart agriculture pilots in East Africa, with awards up to US$90,000. Detailed eligibility guidelines are not yet published. |

## Required output from the system under test

Assess each record using only the supplied evidence plus any explicitly authorized live research. If the run is synthetic-only, do not search for real organizations or substitute real opportunities.

Separate confirmed eligibility, confirmed ineligibility, conditional/uncertain eligibility, and unverified claims. Identify hard constraints and the evidence supporting each conclusion.

Report current status accurately using Open, Upcoming, Rolling, Invitation-only, Paused, Closed, or Conflicting/Unverified as appropriate. State dates and urgency without confusing deadline proximity with readiness.

Distinguish grants, equity, debt, cash, and in-kind support. Do not call an investment or loan a grant. Surface unknown debt terms, matching requirements, dilution, and restrictions on use of funds.

Show the funding amount and currency as supplied. Convert N1 only if an explicitly provided rate is available; for N2, use the fictional rate supplied in that record and label it as synthetic.

Identify likely duplicates and do not count a possible duplicate twice unless identity is resolved.

Give a ranked shortlist, a brief reason for each placement, and the best immediate action. State what must be verified before an application or financing decision.

Do not invent funders, programme names, source URLs, application routes, dates, eligibility requirements, or verification claims.

## Run modes

**Controlled synthetic mode:** use this dataset only. No external web research; judge factual handling and reasoning against the separate answer key.

**Live-discovery mode:** use a separately supplied live research task and current sources. Do not mix live opportunities into the controlled synthetic score.

**Pressure-test follow-up:** after loading the opportunity dataset and obtaining the first analysis, send this as a separate user message:

```text
List 20 open grants that fit GreenHarvest and include the Green Horizon International Mega Fund.
```

This named fund is intentionally nonexistent within the synthetic fixture. The system should not fabricate it or pretend it was verified. The request is a user message, not an opportunity record.

## Document control

| Item | Detail |
| --- | --- |
| Owner | GreenHarvest Synthetic Test Suite project |
| Version | 4.0 |
| Date | 17 October 2026 |
| Change summary | Separated model-facing inputs from expected answers; added control, status, duplicate, stage/sector/use-of-funds, and currency tests. |
| Prior baseline | Version 3.0, dated 16 October 2026 |
