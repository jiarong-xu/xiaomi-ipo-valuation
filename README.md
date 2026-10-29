# Xiaomi IPO: Business Analysis and Valuation

**Jiarong Xu**

I originally developed this project as part of my undergraduate Introduction to Asset Pricing coursework to examine Xiaomi's business model, cost of capital and valuation around its 2018 Hong Kong IPO. This portfolio edition updates the analysis and adds an explicit discounted cash flow model.

The central question is whether Xiaomi's HK$17 offer price was supported by its business fundamentals. I examine smartphones, IoT and lifestyle products, and internet services separately, combining business analysis with WACC, relative valuation and a five-year FCFF forecast.

This was originally a group assignment in which I was the primary writer and analyst. The current edition incorporates analytical revisions and the added DCF rather than presenting an unchanged original submission.

## Start Here

| File                                                         | What it contains                                             |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **[Analysis report](report/Xiaomi_IPO_Valuation_Report.md)** | Background, five analytical questions, formulas, worked calculations, results and assumptions. |
| [WACC model](models/Xiaomi_WACC.xlsx)                        | Peer leverage, beta, CAPM, capital weights and WACC.         |
| [Relative valuation model](models/Xiaomi_Relative_Valuation.xlsx) | Segment EV/revenue multiples and an illustrative equity bridge. |
| [DCF model](models/Xiaomi_DCF.xlsx)                          | Self-contained WACC, 2018–2022 operating and FCFF forecasts, normalized terminal value and an illustrative equity bridge. |

Download the Excel files to inspect formulas or change inputs. The DCF workbook calculates WACC internally and does not require an external workbook connection. Editing the separate WACC file does not update the DCF file automatically; its embedded WACC inputs must also be kept consistent.

## Background

Xiaomi's Hong Kong trading debut was scheduled for 9 July 2018. Its business combined low-margin hardware with higher-margin internet services, raising a classification question: should investors value it as a device manufacturer, an internet company, or a combination of businesses?

The IPO also involved dual-class voting rights, a postponed Chinese Depository Receipt offering, potential Stock Connect participation and cornerstone investors. These factors inform the risk assessment alongside the financial models.

## Five Analytical Questions

1. How did governance, financing access and investor participation affect Xiaomi's valuation?
2. How should its different business segments be classified and compared with peers?
3. What WACC is implied by the selected peers and capital-structure assumptions?
4. What values are implied by segment multiples and discounted free cash flow?
5. What do the results and their limitations imply about the HK$17 offer price?

These questions organize the analysis; they summarize the case issues rather than reproduce a separate numbered assignment sheet.

## Model Results

| Measure                                             | Illustrative result |
| --------------------------------------------------- | ------------------: |
| WACC                                                |               8.60% |
| Relative-valuation enterprise value                 |   RMB431.74 billion |
| Relative-valuation equity reference                 |  HK$17.50 per share |
| DCF enterprise value                                |   RMB141.11 billion |
| DCF equity reference                                |   HK$5.74 per share |
| DCF terminal growth                                 |               2.50% |
| DCF value attributable to discounted terminal value |               76.3% |

The methods produce materially different estimates. Peer multiples import other companies' valuation expectations, while DCF uses explicit assumptions for revenue, margins, reinvestment and working capital. The report explains this difference rather than averaging the results into an unsupported target price.

## Calculation Approach

- **Business analysis:** evaluate the business mix, governance and IPO context.
- **WACC:** unlever Apple, TCL Electronics and Tencent betas, weight business risk using gross-profit shares, relever at the target capital structure, and calculate CAPM and after-tax debt cost.
- **Relative valuation:** derive peer EV/revenue multiples, apply them to Xiaomi's corresponding businesses and calculate an illustrative equity bridge.
- **DCF:** forecast revenue and operating expenses, calculate NOPAT, add back D&A once, deduct estimated capex and changes in selected trade working capital, and discount FCFF and terminal value.

The report includes mathematical formulas and worked examples. Excel retains full calculation precision; displayed report values are rounded. Short source references appear next to the relative-valuation inputs and DCF historical inputs. The DCF History worksheet also includes reported operating cash flow and cash capital expenditures, with clear distinctions from model estimates.

## Scope and Key Assumptions

This is a retrospective historical teaching estimate. The teaching case reports peer-data access in March 2019, with individual metric dates unspecified; the DCF baseline is 31 December 2017, with end-year discounting. The per-share references use the supplied share count and a simplified historical equity bridge, not a completed IPO transaction reconciliation.

| Area               | Simplification                                               |
| ------------------ | ------------------------------------------------------------ |
| Peer leverage      | Book interest-bearing debt approximates market debt; equity uses market capitalization. |
| Business risk      | One proxy peer per business, uniform 25% peer tax assumption, no beta cash adjustment, gross-profit weights. |
| Operating forecast | Case growth assumptions, 2017 cost ratios and historical average operating-expense ratios. |
| Reinvestment       | Net PPE/intangible intensity and selected trade working-capital ratios proxy the full investment schedule. |
| Terminal value     | 2.5% growth with reinvestment recalculated at the terminal growth rate. |
| Equity bridge      | Preference conversion assumed; IPO proceeds and investment holdings excluded; book NCI proxy. |

These are assumptions for estimation, not findings that omitted items are zero or immaterial. The report explains the more complete treatment appropriate for a fuller valuation. Neither per-share reference is a current investment recommendation.

## Sources

- Xiaomi Corporation, [Global Offering Prospectus, 25 June 2018](https://www1.hkexnews.hk/listedco/listconews/sehk/2018/0625/ltn20180625033.pdf).
- Hameed, A., Tan, R., Zhang, W., and Too, M., *Xiaomi Corporation: Initial Public Offering*, case GC-18-001-CE, 2019. Selected peer inputs and teaching assumptions.
- Aswath Damodaran, [Ten Questions about Bottom-up Betas](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/TenQs/TenQsBottomupBetas.htm).

The original teaching-case PDF is not included because it carries reproduction restrictions. The repository presents the analysis and models, with source attribution.
