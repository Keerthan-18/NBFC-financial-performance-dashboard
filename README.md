# NBFC Financial Performance Dashboard
**Comparative analysis of Tata Capital, Bajaj Finance & Manappuram Finance | FY2024–FY2025**

An interactive Power BI dashboard benchmarking three leading Indian NBFCs on profitability, efficiency, capital adequacy, and asset quality — built from audited standalone financial statements.

---

## 🎯 Objective

NBFCs are frequently compared using surface-level metrics like AUM growth, but real credit and equity analysis depends on ratio-level benchmarking — NIM, ROA, ROE, capital adequacy, and asset quality. This project builds that analysis from primary sources for three structurally different NBFCs:

- **Tata Capital** — diversified lender (retail, wealth, housing finance)
- **Bajaj Finance** — India's largest diversified retail NBFC
- **Manappuram Finance** — gold-loan specialist

## 📊 Key Insights

| Finding | Detail |
|---|---|
| **Bajaj Finance leads on profitability and asset quality** | ROE 18.93%, GNPA 1.18%, NNPA 0.57% (FY25) — best-in-class across all three peers |
| **Manappuram commands the highest interest margin** | NIM 11.12% (FY25), reflecting the short-tenure, high-frequency nature of gold loans |
| **Manappuram carries the weakest asset quality despite the strongest capital buffer** | GNPA 2.71%, NNPA 2.38%, yet CRAR 30.91% — a counterintuitive combination worth investigating further (possible drivers: gold-price volatility affecting LTV breaches, slower recovery cycles) |
| **Tata Capital's FY25 figures are not fully comparable YoY** | FY25 includes the merger of Tata Motors Finance Ltd., inflating balance sheet growth versus organic performance |

## 🧮 Ratios Calculated

Net Interest Margin (NIM) · Return on Assets (ROA) · Return on Equity (ROE) · Net Profit Margin · Debt-to-Equity · Capital Adequacy Ratio (CRAR) · Gross NPA % · Net NPA %

## 🛠️ Methodology

1. **Data sourcing** — pulled standalone Balance Sheet, P&L, and RBI-mandated disclosure notes (Asset Classification, Capital Adequacy) directly from each company's FY2024-25 Annual Report / Investor Presentation — not secondary aggregator sites.
2. **Data modeling (Excel)** — structured 100+ line items into a tidy long-format table (Company × FY × Metric × Value), with a source citation for every figure, enabling full traceability back to the original filing.
3. **Ratio engine (Excel)** — built SUMIFS-based formulas to calculate all 8 ratios per company per year, validated by hand before moving to Power BI.
4. **Dashboard build (Power BI)** — imported the tidy dataset, reshaped it via Power Query (pivot), and rebuilt all 8 ratios natively as DAX measures for a fully interactive, refreshable model.
5. **Insight synthesis** — cross-referenced ratio patterns against each company's business model to explain *why* the numbers diverge, not just *that* they diverge.

## 🖥️ Dashboard Pages

1. **NIM Comparison** — interest margin across companies and years
2. **Full Ratio Table** — all 8 ratios, all companies, both years, side by side
3. **ROE Comparison** — profitability trend by company
4. **Asset Quality (GNPA/NNPA) Comparison** — credit risk benchmarking

## 📁 Files in This Repository

| File | Description |
|---|---|
| `NBFC_Financial_Analysis_Master.xlsx` | Source data model + Excel-native ratio calculations |
| `NBFC_Dashboard.pbix` | Power BI file with DAX measures and all visuals |
| `NBFC_Dashboard.pdf` | Static export of the dashboard (viewable without Power BI installed) |
| `/screenshots` | PNG exports of each dashboard page |

## 🔧 Tools Used

Power BI Desktop (Power Query, DAX) · Microsoft Excel (SUMIFS, financial modeling) · Public company disclosures (Annual Reports, RBI-mandated NBFC disclosures)

## 📌 Data Sources

- Tata Capital Ltd. — Annual Report 2024-25 (Standalone Financial Statements)
- Bajaj Finance Ltd. — Annual Report 2024-25 (Standalone Financial Statements)
- Manappuram Finance Ltd. — Annual Report 2024-25 (Standalone Financial Statements)

*All figures are standalone (not consolidated) to ensure like-for-like comparability across companies.*

---

## 👤 Author

**Vijay Keerthan**
MBA Finance & Fintech | [LinkedIn](https://linkedin.com/in/vijay-keerthan-a28680413) | [GitHub](https://github.com/Keerthan-18)
