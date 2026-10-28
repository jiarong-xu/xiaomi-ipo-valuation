# Xiaomi IPO: Business Analysis and Valuation

**Author:** Jiarong Xu  
**Context:** CNAC.F215 — Introduction to Asset Pricing, undergraduate coursework  
**Status:** Portfolio draft; original calculations are being reviewed. No revised fair-value conclusion is presented yet.

## Project Overview

I originally developed this case study as part of my undergraduate Introduction to Asset Pricing coursework to evaluate Xiaomi's business model, cost of capital and valuation around its 2018 Hong Kong IPO. I am revisiting the project to make the analysis and supporting Excel calculations easier to follow in a public portfolio.

The central question is whether Xiaomi's HK$17 IPO price was justified by its business fundamentals and risks. The analysis considers how its smartphone, Internet of Things (IoT) and lifestyle products, and internet services businesses should be valued, rather than assuming that one industry label adequately describes the whole company.

This was originally a group assignment. I was the primary writer and analyst and contributed substantially across the report and supporting calculations. This portfolio edition reorganizes the original work and will identify any substantive corrections or newly added analysis separately from the original coursework.

## Case Background

The case places the investor immediately before Xiaomi's Hong Kong trading debut on 9 July 2018. Xiaomi priced its offering at HK$17 per share, the bottom of an indicative HK$17–22 range, amid concerns about its valuation, weaker market conditions and the postponement of its proposed Chinese Depository Receipt (CDR) offering.

Xiaomi's business combined relatively low-margin hardware with higher-margin internet services. Hardware generated most of its revenue, while internet services contributed disproportionately to gross profit. This created a valuation question: should investors compare Xiaomi with hardware manufacturers, internet companies, or value its businesses separately?

The case also raises questions about founder control under a dual-class share structure, access to mainland investors and support from cornerstone investors. These factors provide context for the financial analysis without independently establishing a fair share price.

**Historical perspective:** The economic decision examined is the 2018 IPO. However, the supplied teaching case is a later publication and includes peer data accessed in March 2019. Calculations based on those exhibits are a retrospective coursework exercise, not a reconstruction using exclusively information available before the IPO. Current Xiaomi results and subsequent share-price performance are outside this draft's scope.

## Five Analytical Questions

The following questions organize this portfolio. They summarize the case issues and the structure of my original report; they are not a verbatim, numbered question sheet from the case publisher.

| Question | Analytical objective | Supporting work |
| --- | --- | --- |
| 1. Which factors affected Xiaomi's valuation at IPO? | Assess dual-class governance, the postponed CDR offering, potential Stock Connect participation and cornerstone investors. | Qualitative business and capital-markets analysis. |
| 2. How should Xiaomi's business model be classified for valuation? | Compare the revenue mix, margins and economics of its different businesses; assess a segment-based approach. | Business-model analysis and peer-selection rationale. |
| 3. What is an appropriate WACC for Xiaomi? | Review peer betas and capital structures, unlever and relever beta, and estimate the cost of equity through CAPM and the after-tax cost of debt. | Original WACC workbooks; assumptions and formulas pending review. |
| 4. What value is implied by relative valuation? | Apply appropriate peer multiples to segment measures, distinguish enterprise value from equity value, and assess whether the results are economically meaningful. | Original relative-valuation workbook; earnings adjustments and units pending review. |
| 5. Was HK$17 per share an attractive IPO price? | Compare a defensible per-share valuation with the offer price and explain the principal risks and limitations. | Final synthesis to be revised after the models are checked. |

## 1. Factors Affecting Valuation

### Dual-class shareholding structure

Xiaomi's Class A shares carried ten votes each, compared with one vote for Class B shares. Founder control could support strategic continuity and long-term investment in research, the IoT ecosystem and international expansion. However, it also limited ordinary shareholders' influence and could make management harder to hold accountable. The valuation effect therefore depends on the balance between the benefits of continuity and the risks of entrenchment and conflicts of interest. Stable control should not automatically be treated as lower operating risk. *(Case, pp. 2–3.)*

### Postponement of the CDR offering

The proposed CDR offering would have given mainland investors another channel to invest in Xiaomi. Its postponement reduced the immediate scope of the planned offering and added uncertainty about regulatory acceptance and valuation. The case reports that Xiaomi subsequently reduced the valuation discussed with cornerstone investors from US$100 billion to US$55–70 billion. This sequence does not isolate the delay's causal effect: business-model concerns and broader market conditions also mattered. Any effect on operating value would depend on whether financing constraints changed Xiaomi's investment opportunities. *(Case, pp. 4–5.)*

### Potential participation in Stock Connect

Stock Connect enabled mainland investors to purchase eligible Hong Kong-listed shares; it did not require Xiaomi to have a separate mainland listing. Participation could broaden the investor base and support liquidity, conditional on eligibility and investor demand. The case records Xiaomi's intention to participate, rather than establishing that access was already available at the IPO. Secondary-market share purchases would not themselves raise new capital for Xiaomi. *(Case, p. 7.)*

### Cornerstone investors

Seven cornerstone investors subscribed for approximately 10% of the shares offered. Qualcomm and China Mobile had existing commercial relationships with Xiaomi. Their commitments supported part of the offering and could provide a credibility signal to other investors. Nevertheless, strategic investors may have objectives beyond financial returns, and their participation did not establish that the offer price was fair or guarantee subsequent performance. Valuation still required an assessment of operating prospects, cash flows and risk. *(Case, p. 5.)*

### Implication for the valuation

These factors affect governance, financing flexibility and investor demand through different channels. They inform the risk assessment surrounding the IPO, while the next stages examine the business mix and the financial assumptions needed to support a valuation conclusion.

## Methods and Skills Demonstrated

- Business-model and corporate-governance analysis.
- Comparable-company selection and segment-based valuation.
- Beta unlevering and relevering, CAPM and WACC calculations.
- Excel formulas linking inputs, intermediate calculations and valuation outputs.
- Interpretation of accounting earnings and the distinction between enterprise and equity value.

The files recovered for this project do not yet establish a completed DCF model, automated Excel/VBA implementation, or sensitivity analysis. Those capabilities are not claimed as deliverables of this repository draft.

## Repository Structure to Prepare

The following is a proposed structure, not a list of files already included with this draft. Links should be added only once the corresponding files have been prepared and reviewed.

| Planned path | Purpose | Current stage |
| --- | --- | --- |
| `README.md` | Project context, analytical questions, contribution and navigation. | This draft. |
| `report/Xiaomi_IPO_Valuation_Report.pdf` | Revised analysis with references and clear limitations. | Original report recovered; revision pending. |
| `models/Xiaomi_WACC.xlsx` | Reviewed WACC inputs, formulas and result. | Multiple original versions recovered. |
| `models/Xiaomi_Relative_Valuation.xlsx` | Reviewed segment valuation and equity-value bridge. | Original workbook recovered; revision pending. |
| `notes/Revision_Notes.md` | Distinguish original assumptions from later corrections and additions. | To prepare during model review. |

## Review Status and Limitations

- Two recovered WACC copies have identical populated cell values and formulas; one can be used as the working base while originals are preserved privately.
- The revised WACC copies include a tax-shield calculation whose cached result is approximately 5.335%. This is an original-workbook output, not an independently validated estimate.
- Peer identities and suitability, interest-bearing debt versus total liabilities, tax assumptions, units, and the basis for segment weights require review.
- The teaching case itself supplies an unusually large IoT EBITDA figure. Its presence in the workbook is not, by itself, evidence of a transcription error; its economic plausibility still needs assessment.
- Negative reported earnings require careful treatment before applying P/E multiples. A negative mechanical output is not a meaningful fair-value conclusion on its own.
- The supplied case includes DCF guidance, but a completed DCF model has not been recovered in the current project files.

## Sources and Publication Scope

Primary teaching source: Hameed, Allaudeen; Tan, Ruth; Zhang, Weina; and Too, Marshall. *Xiaomi Corporation: Initial Public Offering*. Case GC-18-001-CE, dated 30 June 2019. National University of Singapore case authors; relevant rights administered through CEIBS/ChinaCases.Org as stated in the supplied document.

Relevant materials within the case are the IPO narrative (pp. 1–7), income statements (Exhibit 1, p. 8), balance sheet (Exhibit 2, p. 9), peer data (Exhibit 3, p. 10), precedent transactions (Exhibit 4, pp. 11–12), and valuation guidance (Exhibit 5, pp. 13–14).

The original teaching-case PDF is excluded from the planned public repository because it carries reproduction restrictions. This portfolio uses an original summary, attribution and analysis. Any case-derived data intended for publication should be checked for permitted use; citing the source does not itself authorize redistribution of its tables or exhibits. Publicly accessible original company disclosures can be used as replacement sources where appropriate, with dates and substitutions documented.

The original coursework files remain private working materials until personal information has been removed and publication scope checked. New explanatory text and corrections in this portfolio edition should not be represented as unchanged original coursework.
