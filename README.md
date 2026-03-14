# Healthcare Financial Analytics Dashboard

An interactive Power BI dashboard analyzing financial performance and uncompensated care burdens across US hospitals from 2019 to 2023, built using CMS Hospital Cost Report Information System (HCRIS) data.

---

## Overview

This project visualizes hospital financial data across four analytical pages — providing a comprehensive view of uncompensated care costs, financial health, and rural vs urban disparities across thousands of US hospitals over a five-year period.

**Key questions this dashboard answers:**
- Which states carry the highest uncompensated care burden?
- How have hospital finances trended from 2019 to 2023?
- Are rural hospitals more financially distressed than urban ones?
- How does hospital ownership type (Non-Profit, For-Profit, Government) affect financial outcomes?

---

## Dashboard Pages

| Page | Description |
|------|-------------|
| **National Overview** | KPI cards, state-level bar chart, year trend line, rural vs urban donut |
| **Uncompensated Care** | Charity care vs bad debt trends, cost scatter plot, filled state map, breakdown by ownership |
| **Financial Health** | Net income trends, profitability scatter, % hospitals with negative income |
| **Rural vs Urban** | Side-by-side comparisons, dual-line trend chart, top states by rural hospital count |

---

## Data Source

- **Source:** [CMS Hospital Provider Cost Report (HCRIS)](https://www.cms.gov/Research-Statistics-Data-and-Systems/Downloadable-Public-Use-Files/Cost-Reports/Hospital-2010-form)
- **Years:** 2019 – 2023
- **Records:** 22,745 hospital-year observations
- **Columns:** 27 features including financial metrics, hospital identifiers, and geographic attributes

### Key Fields

| Field | Description |
|-------|-------------|
| `Cost of Uncompensated Care` | Primary metric — care provided without payment |
| `Cost of Charity Care` | Care given to patients unable to pay |
| `Total Bad Debt Expense` | Unpaid bills written off by the hospital |
| `Net Income` | Hospital profitability |
| `Rural Versus Urban` | R = Rural, U = Urban |
| `Type of Control` | Hospital ownership type (see lookup table) |

---

## Files in This Repository

```
healthcare-financial-analytics-dashboard/
│
├── README.md
├── HealthcareFinancialDashboard.pbix       # Power BI dashboard file
│
├── data/
│   ├── cleaned_hospital_data.csv           # Main cleaned dataset
│   ├── type_of_control_lookup.csv          # Ownership type labels
│   └── provider_type_lookup.csv            # Provider type labels
│
└── screenshots/
    ├── page1_national_overview.png
    ├── page2_uncompensated_care.png
    ├── page3_financial_health.png
    └── page4_rural_vs_urban.png
```

---

## How to Use

1. Clone or download this repository
2. Open `HealthcareFinancialDashboard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
3. If prompted to refresh data, point the data source to the `data/` folder
4. Use the slicers on each page to filter by Year, State, Rural/Urban, and Ownership Type

---

## Tools & Technologies

- **Power BI Desktop** — dashboard development
- **Python (pandas)** — data cleaning and preparation
- **CMS HCRIS** — raw data source

---

## Author

**Atharva**   
[GitHub Profile](https://github.com/)  
[LinkedIn](https://linkedin.com/)

---

## Acknowledgements

Data sourced from the Centers for Medicare & Medicaid Services (CMS) public use files. This project was built as part of a healthcare analytics portfolio.

