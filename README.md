# Superstore Sales & Profitability Analysis

An end-to-end exploratory business analysis of Superstore transactional data using **Python, Pandas, Matplotlib, Jupyter Notebook, and Kaggle**.

The project evaluates sales performance, profitability, discount behavior, product categories, customer segments, and geographic performance to identify the main drivers of profit and loss and translate them into management actions.

---

## Project Status

| Component | Status |
|---|---|
| Data inspection and quality audit | **Complete** |
| Data cleaning and feature preparation | **Complete** |
| Product/category analysis | **Complete** |
| Discount analysis | **Complete** |
| Regional/state analysis | **Complete** |
| Customer-segment analysis | **Complete** |
| Executive summary and recommendations | **Complete** |
| GitHub portfolio packaging | **Complete** |

---

## Results at a Glance

| KPI | Result |
|---|---:|
| Total Sales | **$2,297,199.86** |
| Total Profit | **$286,394.05** |
| Overall Profit Margin | **12.47%** |
| Transaction Lines | **9,994** |
| Loss-Making Transaction Rate | **~18.7%** |

The analysis shows that the business is profitable overall, but profitability is highly uneven across products, discount levels, and geographic markets.

---

## Business Questions

The analysis answers the following questions:

- Which categories and sub-categories generate the strongest sales and profit?
- Which product areas are destroying value?
- How are discounts associated with profitability?
- Which regions and states perform best and worst?
- How does profitability differ across customer segments?
- Where should management focus to improve margins?

---

## Key Findings

### Category Performance

| Category | Sales | Profit | Profit Margin |
|---|---:|---:|---:|
| Technology | ~$836.2K | ~$145.5K | **17.4%** |
| Office Supplies | ~$719.0K | ~$122.5K | **17.0%** |
| Furniture | ~$742.0K | ~$18.5K | **2.5%** |

**Technology** is the strongest category by profit and margin. **Office Supplies** also performs strongly, while **Furniture** generates substantial revenue but very weak profitability.

### Loss-Making Sub-Categories

- **Tables** generate approximately **$207K in sales** but lose about **$17.7K**, with an aggregate margin of roughly **-8.6%**.
- **Bookcases** lose approximately **$3.5K**.
- **Supplies** is the only loss-making Office Supplies sub-category.
- Tables and Bookcases both carry relatively high average discounts.
- Machines remain profitable but operate at a very low margin despite substantial sales.

### Discount Effect

- Transactions with **no discount** generate approximately **29.5% profit margin**.
- Profitability deteriorates sharply as discount intensity increases.
- Discount levels above approximately **20%** are associated with negative aggregate profitability.

This relationship is descriptive and should not be interpreted as proof of causality.

### Geographic Performance

- The **Central region** has the weakest regional profitability, with an aggregate margin of approximately **7.9%**, and also carries the highest average discount.
- **Texas, Illinois, Pennsylvania, and Ohio** are among the largest state-level loss contributors.
- Furniture losses are particularly concentrated in **Texas and Illinois**.

### Customer Segments

- **Consumer** generates the highest absolute sales and profit.
- **Home Office** achieves the strongest overall segment profit margin.

---

## Business Recommendations

1. **Review discount policy** — require stronger commercial justification for discounts above 20%.
2. **Address Furniture profitability** — review pricing, product cost, discounting, and regional selling practices for Tables and Bookcases.
3. **Investigate high-loss states** — prioritize Texas, Illinois, Pennsylvania, and Ohio for corrective action.
4. **Protect profitable growth areas** — continue expanding Technology and Office Supplies while monitoring margin quality.
5. **Track margin with revenue** — sales alone should not be treated as a sufficient performance measure.
6. **Improve transaction-level data collection** — future datasets should include Order ID, Customer ID, Product ID, and transaction dates.

---

## Dataset

The project uses the **Super Store** dataset available on Kaggle.

**Dataset source:** https://www.kaggle.com/datasets/itssuru/super-store

The analyzed dataset contains **9,994 transaction-line records** with fields covering:

- Ship Mode
- Customer Segment
- State and Region
- Product Category and Sub-Category
- Sales
- Quantity
- Discount
- Profit

The dataset itself is intentionally not committed to this repository.

### Dataset Limitation

The analyzed version does **not** include Order ID, Customer ID, Product ID, or transaction dates. For that reason:

- exact duplicate rows cannot be confirmed as erroneous transactions;
- order-level KPIs cannot be calculated reliably;
- customer-level and repeat-purchase analysis is not possible;
- product-level analysis is limited to sub-category level;
- time-series analysis and forecasting are not possible.

Seventeen exact duplicate records were identified, but they were retained because no unique transaction identifier exists to prove they are invalid duplicates.

---

## Analysis Workflow

```text
Raw dataset
    ↓
Initial inspection
    ↓
Data quality audit
    ↓
Data cleaning and column standardization
    ↓
Executive KPI analysis
    ↓
Category and sub-category analysis
    ↓
Discount analysis
    ↓
Regional and state analysis
    ↓
Customer-segment analysis
    ↓
Visualizations
    ↓
Business recommendations
```

The notebook concludes with a final validation check confirming:

- **9,994 rows** in the working dataset;
- **0 missing values**;
- **$2.30M total sales**;
- **$286.4K total profit**;
- **12.47% overall profit margin**.

---

## Live Kaggle Notebook

The fully executable version of the analysis, including notebook outputs and visualizations, is hosted on Kaggle:

**[View the analysis on Kaggle](https://www.kaggle.com/code/aierajahassan/superstore-sales-profitability-analysis)**

The GitHub notebook is retained as the portfolio copy of the analysis.

---

## Repository Structure

```text
superstore-sales-profitability-analysis/
│
├── data/
│   └── README.md
│
├── .gitignore
├── LICENSE
├── README.md
├── requirements.txt
└── superstore_sales_profitability_analysis.ipynb
```

---

## Local Setup

Clone the repository:

```bash
git clone https://github.com/RajaHassan6/superstore-sales-profitability-analysis.git
cd superstore-sales-profitability-analysis
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

**Windows**

```bash
.venv\Scripts\activate
```

**macOS / Linux**

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### Running Locally

The notebook currently references the Kaggle dataset path used in the hosted Kaggle environment. For local execution, download `SampleSuperstore.csv` from the dataset source and change the notebook `file_path` to the local CSV location.

For zero-configuration execution, use the linked Kaggle notebook.

---

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Kaggle
- Git
- GitHub

---

## Skills Demonstrated

**Data Analysis:** data inspection, cleaning, aggregation, grouping, KPI calculation, descriptive analytics.

**Business Analytics:** profitability analysis, margin analysis, discount analysis, product performance, customer segmentation, geographic performance.

**Data Visualization:** bar charts, comparative plots, state-level profitability views, discount-performance analysis.

**Analytical Judgment:** duplicate-record assessment, metric interpretation, association-versus-causality distinction, business recommendation development.

**Portfolio Engineering:** GitHub documentation, dependency management, dataset documentation, repository licensing.

---

## Limitations

- The dataset represents historical transaction-line data and lacks a usable time-series structure.
- Order, customer, product, and date identifiers are absent from the analyzed version.
- Discount-profit relationships are associations rather than causal estimates.
- The project focuses on descriptive/exploratory analytics rather than predictive modeling.
- Operating expenses, acquisition costs, and other full business-cost components are not available.

---

## Future Improvements

With a richer source dataset, the project could be extended to include:

- monthly and quarterly sales trends;
- customer lifetime value and repeat-purchase analysis;
- product-level profitability;
- cohort analysis;
- market-basket analysis;
- sales and profit forecasting;
- predictive modeling for loss-making transactions;
- interactive Power BI or Tableau dashboards.

---

## Key Takeaway

The Superstore business is profitable overall, but revenue alone masks substantial margin weakness. The main management priorities are **discount discipline, Furniture profitability, and targeted intervention in high-loss states**.

This project demonstrates the complete transition from raw transactional data to management-oriented business insight using Python analytics.

---

## License

This project is released under the **MIT License**. See `LICENSE` for details.

---

## Author

**Raja Hassan**

GitHub: https://github.com/RajaHassan6
