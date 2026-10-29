# Xiaomi IPO: Business Analysis and Valuation

**Jiarong Xu**  
**Context:** Undergraduate Introduction to Asset Pricing coursework, revised for portfolio presentation  
**Scope:** Historical teaching exercise examining Xiaomi's 2018 Hong Kong IPO

## Overview

I originally developed this analysis as part of my undergraduate coursework to examine Xiaomi's business model, cost of capital and valuation around its Hong Kong IPO. I was the primary writer and analyst in the original group project. This portfolio edition presents a consistent estimate with explicit simplifying assumptions.

The economic question is whether the HK$17 offer price was supported by the company's fundamentals. Xiaomi's low-margin hardware business generated most of its revenue, while internet services contributed a much larger share of gross profit than of sales. The analysis therefore considers its principal businesses separately.

The project addresses five questions: which factors affected valuation, how the business should be classified, what WACC is implied by a documented set of assumptions, what values are implied by relative valuation and discounted cash flow, and what conclusions can reasonably be drawn about the offer price.

The estimated WACC is **8.60%** under the stated assumptions. The relative-valuation exercise indicates enterprise value of **RMB431.74 billion** for three principal businesses. A simplified equity bridge gives **HK$17.50 per share**, approximately **2.9%** above the HK$17 offer price. The added DCF produces enterprise value of **RMB141.11 billion** and an illustrative equity reference of **HK$5.74 per share**. Both methods are conditional teaching estimates, not completed contemporaneous IPO fair values or a sufficient basis for an investment recommendation.

## Historical Context and Data Basis

Xiaomi was due to begin trading in Hong Kong on 9 July 2018. Its shares were offered at HK$17, the lower end of the indicative HK$17–22 range. Investors were assessing its business classification, a postponed Chinese Depository Receipt (CDR) offering, governance arrangements and relatively weak market conditions.

The decision setting is the 2018 IPO, but the teaching case reports FactSet access in March 2019 without specifying the observation date and metric period for every peer field. This portfolio therefore constitutes a retrospective coursework exercise. It is not a valuation based exclusively on information available immediately before the IPO. Xiaomi's historical segment data and selected balance-sheet amounts have been checked against its public June 2018 prospectus. Peer figures remain the supplied case snapshot.

## 1. Factors Affecting Xiaomi's Value

### Dual-class governance

Xiaomi's Class A shares carried ten votes each, compared with one vote for Class B shares. Founder control could support strategic continuity and investment with long payback periods. It also reduced ordinary shareholders' ability to influence management and increased the potential cost of entrenchment or conflicts of interest. Control stability is not equivalent to lower operating risk, and its valuation effect should not automatically be assumed positive.

### CDR postponement

The proposed CDR offering would have offered mainland investors another route to invest in Xiaomi. Its postponement added uncertainty about regulatory acceptance and the planned financing. The case describes a subsequent reduction in the valuation discussed with cornerstone investors. That sequence does not isolate the delay's causal effect, because business-model concerns and market conditions were changing at the same time.

### Potential Stock Connect participation

Stock Connect could broaden access to eligible Hong Kong-listed shares for mainland investors. A separate mainland listing was not required. Xiaomi's intention to participate was relevant to potential liquidity and demand, but intention should not be represented as confirmed eligibility at the IPO. Secondary-market purchases would not themselves raise new cash for Xiaomi.

### Cornerstone investors

Seven cornerstone investors subscribed for approximately 10% of the shares offered. Existing commercial relationships with participants such as Qualcomm and China Mobile provided context for their interest. Their commitments supported part of the offering and could signal credibility, but did not independently prove that the issue price was attractive or guarantee future performance.

These factors inform the governance and market-risk assessment. They do not replace a financial valuation.

## 2. Business Classification and Peer Selection

A single label cannot adequately describe Xiaomi's different revenue streams. The analysis uses a segment approach with the following proxy peers consistently across the models:

| Xiaomi business | Proxy peer | Rationale and limitation |
| --- | --- | --- |
| Smartphones | Apple | Relevant device and ecosystem exposure, but different pricing, margins and scale. |
| IoT and lifestyle products | TCL Electronics | Consumer electronics exposure, but a narrower product mix than Xiaomi's ecosystem. |
| Internet services | Tencent | Relevant internet monetization exposure, but a different business mix and platform position. |

One peer per segment provides a transparent teaching calculation, but is not a robust industry sample. A more extensive analysis would use multiple peers, aligned dates and comparable operating metrics.

## 3. WACC

Peer betas are unlevered using book interest-bearing debt as a practical proxy for market debt, divided by equity market capitalization. Ideally both debt and equity should be measured at market value on an aligned valuation date. Total liabilities are not treated as interest-bearing debt.

For peer company $j$, unlever equity beta as follows:

$$
\beta_{U,j}=\frac{\beta_{L,j}}{1+(1-T_j)(D_j/E_j)}
$$

Here $D_j$ is book interest-bearing debt used as a market-debt proxy, $E_j$ is equity market capitalization, and $T_j$ is the assumed peer tax rate. The method assumes negligible debt beta. It is not a calculation using book equity.

For example, the Apple proxy gives:

$$
\beta_{U,Apple}=\frac{0.84}{1+(1-0.25)(115680/860882.5)}\approx0.7631
$$

Applying the same formula gives approximately **0.572** for TCL and **1.184** for Tencent.

The three peer tax rates are explicitly assumed at 25%. These are simplifying modelling assumptions for peer marginal tax rates. No cash adjustment is made. The peer betas also relate to different local indices, which limits their comparability.

Business weights use 2017 gross profit as a proxy for segment value:

| Business | Gross profit, RMB million | Weight |
| --- | ---: | ---: |
| Smartphones | 7,101.339 | 47.3014% |
| IoT and lifestyle | 1,950.865 | 12.9945% |
| Internet services | 5,960.751 | 39.7040% |
| Three-segment total | 15,012.955 | 100.0000% |

The small Others business is excluded and the remaining weights are normalized. Gross-profit weights are not market-value weights. They assume the included businesses' contribution to value can be approximated by gross profit, an assumption that requires further testing.

Gross profit and business weights are calculated from the same underlying operating data:

$$
GP_i=Revenue_i-COGS_i,\qquad w_i=\frac{GP_i}{\sum_{k=1}^{3}GP_k}
$$

$$
\beta_{U,Xiaomi}=\sum_{i=1}^{3}w_i\beta_{U,i}\approx0.905181
$$

For example, smartphone gross profit is RMB80,563.594m minus RMB73,462.255m, or RMB7,101.339m, and its weight is 7,101.339 / 15,012.955 = **47.3014%**. Gross profit is an estimation proxy, not a claim about segment cash flow or economic value.

The resulting weighted unlevered beta is **0.905**, and relevering at target D/E of **0.29** and Xiaomi tax rate of **25%** gives equity beta of **1.102**. With the case risk-free rate of **3.55%** and equity risk premium of **5.65%**, the cost of equity is **9.78%**.

Target D/E implies debt weight of **22.48%** and equity weight of **77.52%**. The assumed pre-tax debt cost of **6.05%** becomes **4.54%** after tax.

The remaining calculations are:

$$
\beta_{L,Xiaomi}=\beta_{U,Xiaomi}[1+(1-T_X)(D/E)_X]
$$

$$
\beta_{L,Xiaomi}\approx0.905181[1+(1-0.25)\times0.29]\approx1.102058
$$

$$
k_E=r_f+\beta_{L,Xiaomi}ERP\approx3.55\%+1.102058\times5.65\%=9.7766\%
$$

With $q=(D/E)_X=0.29$, convert debt/equity into capital weights:

$$
w_D=\frac{q}{1+q}=22.4806\%,\qquad w_E=\frac{1}{1+q}=77.5194\%
$$

$$
k_{D,after\ tax}=k_D(1-T_X)=6.05\%(1-0.25)=4.5375\%
$$

$$
WACC=w_Ek_E+w_Dk_D(1-T_X)\approx8.59884\%\approx8.60\%
$$

All displayed intermediate values are rounded. The workbooks use full precision rather than calculating from the rounded figures above.

The estimated WACC is **8.60%**, conditional on the selected peers, leverage and weighting assumptions. It should not be interpreted as a uniquely determined or current market WACC.

## 4. Relative Valuation and Discounted Cash Flow

### Choice of valuation measure

EV/revenue is used for this illustrative estimate because negative reported net income limits the usefulness of P/E and the available segment EBITDA amounts are not sufficiently reconciled for this analysis. Revenue multiples remain sensitive to differences in margins and growth, so they are a practical alternative rather than a definitive valuation method.

Accounting net income already reflects depreciation and amortization recognized in the income statement. No additional deduction is made here. A reconstruction of EBITDA from net income would require adding back the relevant depreciation and amortization, interest and income tax, with consistent treatment of non-operating items. Simply adding depreciation and amortization to net income would not complete that reconstruction.

### Segment EV/revenue estimate

This edition uses EV/revenue as an alternative that can be calculated from the available data without relying on the supplied segment EBITDA allocation. The multiple is derived from peer enterprise value divided by peer sales, which keeps the multiple on an enterprise-value basis.

For segment $i$ with proxy peer $j$:

$$
M_j=\frac{EV_j}{Sales_j},\qquad EV_i=M_j\times Revenue_i
$$

$$
EV_{core}=\sum_{i=1}^{3}EV_i
$$

Peer EV and peer sales are both in USD millions, so their ratio is dimensionless. Applying it to Xiaomi revenue in RMB millions gives enterprise value in RMB millions. No USD/RMB conversion is required for this step.

For smartphones:

$$
M_{Apple}=\frac{821630}{228572}\approx3.594622
$$

$$
EV_{smartphones}=80563.594\times\frac{821630}{228572}\approx289595.689\text{ RMB million}
$$

| Business | Xiaomi 2017 revenue, RMB million | Peer EV/revenue | Implied EV, RMB billion |
| --- | ---: | ---: | ---: |
| Smartphones | 80,563.594 | 3.5946x | 289.60 |
| IoT and lifestyle | 23,447.823 | 0.1950x | 4.57 |
| Internet services | 9,896.389 | 13.9013x | 137.57 |
| Total, using unrounded calculations | 113,907.806 | — | 431.74 |

Displayed components are rounded. The workbook retains full precision. The different multiples embed substantial differences in peer margins, growth and risk; applying them to Xiaomi does not establish that those economics are equivalent.

WACC is not used to discount the output of this multiples calculation. The multiples workbook shares business definitions and peers with the WACC model. The separate DCF workbook uses WACC to discount forecast free cash flow. WACC's gross-profit weights also do not allocate enterprise value in this section: each segment is valued using its own revenue and multiple.

### Illustrative equity bridge

The workbook adds 2017 unrestricted cash of RMB11,563.282 million and subtracts current borrowings of RMB3,550.801 million, non-current borrowings of RMB7,251.312 million, related-party loans of RMB51.336 million and book non-controlling interests of RMB61.670 million.

It assumes the preferred shares convert, excludes net IPO cash proceeds, and excludes other investments and adjustments. These exclusions are assumptions, not findings that the amounts are zero or immaterial. Book non-controlling interests are only a proxy for the claim's market value.

The equity bridge is:

$$
V_E=EV+Cash-Debt-NCI-PreferenceClaim+IPOcash+OtherAdjustments
$$

$$
Debt=3550.801+7251.312+51.336=10853.449\text{ RMB million}
$$

$$
V_E=431739.970+11563.282-10853.449-61.670\approx432388.133\text{ RMB million}
$$

The preference claim, IPO cash and other adjustments are set to zero under the stated simplifying assumptions. Their omission is not evidence that their actual values are zero.

$$
P_{HKD}=\frac{V_E\ (RMB\ million)}{Shares\ (million)\times FX\ (RMB/HKD)}
$$

$$
P_{HKD}\approx\frac{432388.133}{20941.690830\times1.18}\approx17.50
$$

This simplified bridge produces equity reference value of **RMB432.39 billion**. Dividing by the case share count of **20,941.690830 million** and by **RMB1.18 per HK$** gives **HK$17.50 per share**.

Because the model combines a 2017 balance-sheet bridge, case peer data with unspecified observation dates and a supplied share count, this is not a completed IPO-date equity valuation. The share count, preference conversion, actual net proceeds, investment assets and claim values would need a consistent transaction-date reconciliation before making a stronger price conclusion. The share input of 20,941,690,830 matches the prospectus table on printed p.193, which describes shares as of the prospectus date before the offering; it is a pre-offering share count rather than a fully diluted post-IPO share count.

### Discounted cash flow

The DCF supplements the multiples estimate with an explicit operating forecast for 2018–2022. Its discounting baseline is **31 December 2017**, with cash flows discounted at year-end. It does not pretend to place the baseline on the July 2018 IPO date without a timing adjustment. The self-contained workbook includes a live WACC calculation, inputs, historical calibration and the forecast.

Smartphone revenue grows at **6.9%**, IoT/lifestyle revenue at **21.3%**, and internet-services revenue at **15.9%** per year during the forecast period, using the teaching-case assumptions. Segment cost-of-sales ratios remain at 2017 levels. Selling, administrative and R&D ratios use the average of their 2015–2017 percentages of group revenue, applied to forecast revenue from the three principal businesses.

Core EBIT is segment gross profit less these operating expenses. It excludes investment revaluations, financing items and the Others business. Depreciation and amortization already embedded in costs and expenses are added back once in the FCFF calculation. The model uses a historical average D&A-to-revenue ratio and cash tax of 25% of positive core EBIT, without modelling tax losses or deferred taxes.

For forecast year $t$ and business $i$:

$$
Revenue_{i,t}=Revenue_{i,t-1}(1+g_i),\qquad COGS_{i,t}=Revenue_{i,t}\times c_i
$$

Here $c_i=COGS_{i,2017}/Revenue_{i,2017}$ and the forecast growth rates are $g_i=6.9\%,21.3\%,15.9\%$ for smartphones, IoT and internet services respectively.

For each operating-expense category $j$, the calibration is a simple average of annual ratios, not a ratio of three-year totals:

$$
a_j=\frac{1}{3}\sum_{y=2015}^{2017}\frac{Expense_{j,y}}{GroupRevenue_y},\qquad Expense_{j,t}=a_j\times Revenue_t
$$

$$
EBIT_{core,t}=\sum_i(Revenue_{i,t}-COGS_{i,t})-Selling_t-Admin_t-RD_t
$$

$$
CashTax_t=\max(EBIT_{core,t},0)\times T_X,\qquad NOPAT_t=EBIT_{core,t}-CashTax_t
$$

$$
FCFF_t=NOPAT_t+DA_t-Capex_t-\Delta WC_t
$$

The tax formula does not assume an immediate cash refund when EBIT is negative. The D&A add-back occurs once after EBIT.

For a transparent reinvestment estimate, selected net fixed assets comprise net property/equipment and intangibles, projected at their 2017 intensity relative to core revenue. Estimated capex equals the increase in that net asset balance plus D&A. This is a proxy that excludes land rights, acquisitions, disposals, FX and other asset changes; it is not reported cash capex and does not purport to model all group investment requirements.

The reinvestment proxy is implemented as follows, with $Revenue_t$ representing the three principal businesses:

$$
d=\frac{1}{3}\sum_{y=2015}^{2017}\frac{DA_y}{GroupRevenue_y},\qquad DA_t=d\times Revenue_t
$$

$$
f=\frac{NetPPE_{2017}+Intangibles_{2017}}{Revenue_{2017}},\qquad NFA_t=f\times Revenue_t
$$

$$
Capex_t=(NFA_t-NFA_{t-1})+DA_t
$$

For example, the projected net-asset schedule satisfies $NFA_t=NFA_{t-1}+Capex_t-DA_t$. Acquisitions, disposals and other unmodelled balance changes are excluded by assumption.

### Historical cash-flow reference

The DCF History worksheet now includes reported cash-flow reference data, in addition to the model calibration inputs. Xiaomi's public prospectus presents the following figures on printed p. I-14, converted here from RMB thousands to RMB millions:

| Reported item, RMB million | 2015 | 2016 | 2017 |
| --- | ---: | ---: | ---: |
| Net operating cash flow after cash tax | (2,601.311) | 4,531.264 | (995.669) |
| Cash capital expenditures, positive spending magnitude | 2,524.356 | 1,826.245 | 1,217.806 |

The worksheet retains cash outflows as negative amounts. Net operating cash flow equals operating cash generated before tax less cash tax paid. The public cash-flow statement discloses aggregate capital expenditures; no unsupported split between property/equipment and intangible purchases is introduced.

For 2017, the model's historical net-asset capex proxy is **RMB2,397.670 million**, compared with reported cash capex of **RMB1,217.806 million**. The difference of **RMB1,179.864 million** is not allocated to acquisitions, FX or other causes without a detailed asset roll-forward. It demonstrates that the proxy is not a substitute for reported cash spending. Both reported cash spending and the net-asset proxy are presented to distinguish the historical cash-flow data from the forecast methodology.

Reported operating cash flow is also not directly equal to the model's selected-business FCFF proxy. The model uses a different operating scope, selected working-capital items, estimated operating taxes and reinvestment. A complete bridge would need the remaining cash/non-cash and financing adjustments. The reference data do not silently change the forecast assumptions or valuation outputs.

### Selected operating working capital

Selected trade working capital is net trade receivables plus public-prospectus inventories, less trade payables and customer advances. It excludes financial loan receivables, cash and debt, as well as other operating prepayments/accruals. Its 2017 revenue ratio is retained in forecasts. Because this measure is negative, growth releases cash under the assumed supplier/customer financing structure. A more complete valuation should test whether that structure is sustainable.

The working-capital schedule uses:

$$
WC=TradeReceivables+Inventory-TradePayables-CustomerAdvances
$$

$$
u=\frac{WC_{2017}}{Revenue_{2017}},\qquad WC_t=u\times Revenue_t,\qquad\Delta WC_t=WC_t-WC_{t-1}
$$

If $\Delta WC_t$ is negative, subtracting it increases FCFF. That is a cash release under the assumed trade-credit structure, not a sign reversal error.

| Period | Forecast FCFF, RMB billion |
| --- | ---: |
| 2018 | 6.480 |
| 2019 | 7.435 |
| 2020 | 8.542 |
| 2021 | 9.825 |
| 2022 | 11.315 |
| Normalized 2023 terminal year | 9.914 |

The terminal year grows all segments at **2.5%** and retains the final forecast business mix and margin assumptions. Reinvestment and working-capital changes are recalculated at that lower growth rate. Terminal FCFF is therefore not simply 2022 FCFF multiplied by 1.025: in particular, lower growth reduces the assumed cash release from negative trade working capital.

The normalized terminal-year calculations use $g=2.5\%$:

$$
Revenue_{i,2023}=Revenue_{i,2022}(1+g)
$$

$$
DA_{2023}=dRevenue_{2023},\quad NFA_{2023}=fRevenue_{2023},\quad WC_{2023}=uRevenue_{2023}
$$

$$
Capex_{2023}=(NFA_{2023}-NFA_{2022})+DA_{2023}
$$

$$
FCFF_{2023}=NOPAT_{2023}+DA_{2023}-Capex_{2023}-(WC_{2023}-WC_{2022})
$$

These equations produce normalized terminal FCFF of approximately **RMB9,914.004 million**. Gordon growth is applied only when $WACC>g$:

$$
TV_{2022}=\frac{FCFF_{2023}}{WACC-g}
$$

Forecast and terminal cash flows are discounted to the end-2017 baseline:

$$
DF_t=\frac{1}{(1+WACC)^t},\qquad PV(FCFF_t)=FCFF_t\times DF_t
$$

$$
EV_{DCF}=\sum_{t=1}^{5}\frac{FCFF_{2017+t}}{(1+WACC)^t}+\frac{TV_{2022}}{(1+WACC)^5}
$$

The five forecast cash flows contribute approximately **RMB33,495.3 million** of present value and the terminal value contributes **RMB107,615.8 million**. The same equity bridge and RMB/HKD conversion then apply:

$$
V_{E,DCF}\approx141111.037+11563.282-10853.449-61.670=141759.200\text{ RMB million}
$$

$$
P_{HKD,DCF}\approx\frac{141759.200}{20941.690830\times1.18}\approx5.74
$$

At **8.60% WACC** and **2.5% terminal growth**, forecast FCFF plus discounted terminal value produces **RMB141.11 billion** of enterprise value. Terminal value accounts for **76.3%** of enterprise value. The same simplified cash/debt/claim bridge used in the multiples workbook gives **RMB141.76 billion** of equity reference value and **HK$5.74 per share**. These outputs are conditional on the reinvestment, working-capital and bridge assumptions.

## 5. Investment Assessment

The two methods produce materially different reference values: approximately **HK$17.50 per share** from peer EV/revenue and **HK$5.74 per share** from the DCF. Their difference should not be hidden by taking an unexplained average. The multiples method imports peers' valuation expectations, while the DCF uses explicit case growth rates, operating margins and reinvestment proxies. The gap highlights assumptions requiring further investigation.

Neither result supports a confident investment recommendation in this simplified exercise. The relative-valuation reference is only about 2.9% above the offer price. The lower DCF result depends on assumptions that need validation, and its terminal value contributes 76.3% of enterprise value. Both per-share figures use a simplified historical equity bridge rather than a full IPO transaction reconciliation.

Xiaomi's business mix warrants separate analysis of internet-service monetization and hardware economics. A stronger conclusion would require aligned valuation dates, a larger peer sample, a fuller reinvestment/working-capital schedule, a consistent transaction bridge and sensitivity analysis of the principal drivers.

## Estimation Methods and Assumptions

| Area | Simplification used in this estimate | Preferred treatment in a fuller valuation |
| --- | --- | --- |
| Peer leverage | Book interest-bearing debt divided by equity market capitalization. | Aligned market values of debt and equity, with a consistent definition of debt. |
| Business weights for beta | Three principal segments' gross-profit shares. | Estimated segment market-value weights. |
| Peer sample | One proxy company per business. | Several economically comparable firms, with consistent observation dates. |
| Peer taxes and cash | Uniform 25% tax assumption; no cash adjustment to beta. | Relevant marginal tax rates and a consistent cash adjustment. |
| Valuation multiple | Peer EV/revenue applied to each segment's sales. | Reconcile earnings or cash flow and compare multiple methods, adjusting for margins and growth. |
| DCF reinvestment | Change in net PPE/intangibles plus D&A; selected trade WC ratios. | Detailed cash capex, operating asset roll-forwards and complete working-capital schedules. |
| DCF terminal value | Stable margins and asset intensities, reinvestment recalculated at 2.5% growth. | Sustainable long-run returns, reinvestment and sensitivity testing. |
| Equity bridge | Historical cash and debt; preference conversion assumed; IPO proceeds and investments excluded; book NCI proxy. | Transaction-date claims, investment assets, proceeds and diluted share-count reconciliation. |
| Timing | 2017 Xiaomi data and the later peer snapshot supplied in the teaching case. | Financial and market inputs available at a single, specified valuation date. |

These assumptions make the exercise reproducible. They do not establish that omitted items are zero, that the selected proxies are exact, or that the estimate represents a completed IPO-date fair value.

## Input References

Page references below use printed prospectus pages. The worksheets display short source references beside the relevant input groups. Financial statement values reported in RMB thousands are divided by 1,000 for models presented in RMB millions.

| Input | Reference |
| --- | --- |
| Xiaomi segment revenue, cost and gross profit  |  25 June 2018 prospectus, Note 5, I-54 |
| Historical group selling, administrative and R&D expenses  |  Prospectus I-4 |
| Depreciation and intangible amortization  |  Prospectus Note 36, I-107 |
| Net PPE, intangibles, inventories and net trade receivables  |  Prospectus I-6 |
| Trade payables and customer advances  |  Prospectus I-7 |
| Operating cash flow and reported cash capex  |  Prospectus I-14 |
| Cash, borrowings, related-party loans and book NCI  |  Prospectus I-6–I-7, Note 31(a) I-96, Note 33 I-97 |
| Peer EV, sales, beta, debt and equity market value  |  Teaching case Exhibit 3, p.10; FactSet accessed 15 March 2019 |
| Growth, terminal growth, target capital structure, debt cost, risk-free rate, ERP and FX  |  Teaching case Exhibit 5, pp.13–14 |
| Share count  |  Case Exhibit 5, p.14; prospectus p.193 |
| Uniform peer tax rate and omitted bridge adjustments  |  Analyst assumptions shown in models |

## Supporting Models

- [WACC model](../models/Xiaomi_WACC.xlsx): capital-cost estimate, showing inputs, beta calculations and WACC on one worksheet.
- [Relative valuation model](../models/Xiaomi_Relative_Valuation.xlsx): segment EV/revenue estimate and illustrative equity bridge on one worksheet.
- [DCF model](../models/Xiaomi_DCF.xlsx): self-contained WACC, 2018–2022 FCFF forecasts, normalized terminal value and illustrative equity bridge. Inputs and historical data are separate from calculations.

The workbooks use Apple, TCL Electronics and Tencent for the same business categories. The report and models present the same assumptions and rounded results. This portfolio edition reflects analytical updates to the original coursework.

## References

- Xiaomi Corporation, *Global Offering Prospectus*, 25 June 2018: segment information, cash and borrowings, related-party loans and share structure. [Public prospectus](https://www1.hkexnews.hk/listedco/listconews/sehk/2018/0625/ltn20180625033.pdf).
- Hameed, A., Tan, R., Zhang, W., and Too, M., *Xiaomi Corporation: Initial Public Offering*, GC-18-001-CE, 2019. Selected peer inputs and teaching assumptions; original case PDF is not reproduced.
- Aswath Damodaran, *Ten Questions about Bottom-up Betas*, for the beta framework and limitations of segment weighting. [Method reference](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/TenQs/TenQsBottomupBetas.htm).
