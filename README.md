# Superstore Sales & Profitability Analysis

An end-to-end exploratory business analysis of Superstore transactional data using **Python, Pandas, and Matplotlib**.

The project investigates sales performance, profitability, discount behavior, product categories, geographic performance, and customer segments to identify the main drivers of profit and loss.
---

## Results at a Glance

| KPI | Result |
|---|---:|
| Total Sales | $2.30M |
| Total Profit | $286.4K |
| Overall Profit Margin | 12.47% |
| Transaction Lines | 9,994 |
| Loss-Making Transaction Rate | 18.72% |

The analysis identified discounting, low-margin Furniture products, and geographic concentration of losses as major profitability issues.
----
## Live Kaggle Notebook

The complete executable version of this project, including outputs and visualizations, is available on Kaggle:

[View the analysis on Kaggle](https://www.kaggle.com/code/aierajahassan/superstore-sales-profitability-analysis)

## Project Objectives

The analysis answers the following questions:

- Which categories and sub-categories generate the highest sales and profits?
- Which areas of the business are generating losses?
- How are discounts associated with profitability?
- Which regions and states perform best and worst?
- How does profitability differ across customer segments?
- Where should management focus to improve business margins?

## Dataset

The project uses the **Super Store** dataset available on Kaggle.


**Dataset Source:** [Superstore Dataset on Kaggle](https://www.kaggle.com/datasets/itssuru/super-store)

The dataset contains **9,994 transaction records** covering:

- Ship Mode
- Customer Segment
- State and Region
- Product Category and Sub-Category
- Sales
- Quantity
- Discount
- Profit

The dataset itself is not included in this repository.

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Kaggle

## Analysis Workflow

1. Data loading and inspection
2. Data quality audit
3. Data cleaning and preparation
4. Feature engineering
5. Executive KPI analysis
6. Category and sub-category analysis
7. Discount analysis
8. Regional and state analysis
9. Customer segment analysis
10. Data visualization
11. Business recommendations

## Key KPIs

| KPI | Result |
|---|---:|
| Total Sales | $2,297,199.86 |
| Total Profit | $286,394.05 |
| Overall Profit Margin | 12.47% |
| Transaction Lines | 9,994 |
| Loss-Making Transaction Rate | 18.72% |

## Key Findings

- **Technology** is the strongest category, generating approximately **17.4% profit margin**.
- **Office Supplies** also performs strongly with approximately **17.0% margin**.
- **Furniture** generates substantial revenue but only approximately **2.5% margin**.
- **Tables** are the largest loss-making sub-category, losing approximately **$17.7K**.
- Bookcases and Supplies are also loss-making.
- Transactions with **no discount** generate approximately **29.5% margin**.
- Profitability deteriorates substantially as discount levels increase.
- Discount bands above approximately **20%** are associated with negative aggregate profitability.
- The **Central region** has the weakest regional profitability.
- Texas, Ohio, Pennsylvania, and Illinois are among the largest state-level loss contributors.
- Furniture losses are particularly concentrated in Texas and Illinois.
- The Consumer segment generates the highest absolute sales and profit, while Home Office achieves the strongest overall segment margin.

## Business Recommendations

1. Review discount policies, particularly discounts exceeding 20%.
2. Investigate pricing and cost structures for Tables and Bookcases.
3. Prioritize corrective action in major loss-making states such as Texas and Illinois.
4. Protect and expand profitable Technology and Office Supplies sales.
5. Track profit margin together with revenue rather than evaluating performance on sales alone.
6. Improve future transaction-level data collection by including Order ID, Customer ID, Product ID, and transaction dates.
----

## Limitations

- The dataset represents historical transactional data and does not contain a complete time-series structure for forecasting.
- Important identifiers such as Order ID, Customer ID, and Product ID are not available in the analyzed version of the dataset.
- Observed relationships between discounts and profitability represent associations rather than causal effects.
- The analysis focuses on descriptive and exploratory analytics rather than predictive modelling.
- Business costs, operating expenses, and customer acquisition costs are not included.
---  

## Project Structure

```text
superstore-sales-profitability-analysis/
│
├── .gitignore
├── README.md
└── superstore_sales_profitability_analysis.ipynb
```

---

## Author

**Raja Hassan**

Electrical Engineer transitioning into Data Science & AI, applying Python and analytics to engineering and general business problems.

GitHub: [RajaHassan6](https://github.com/RajaHassan6)

