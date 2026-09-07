# Data

The raw Superstore dataset is intentionally not committed to this repository.

Dataset source:

- Kaggle: https://www.kaggle.com/datasets/itssuru/super-store
- File used in the analysis: `SampleSuperstore.csv`

The analyzed dataset contains 9,994 transaction-line records and the following fields:

- Ship Mode
- Segment
- Country
- City
- State
- Postal Code
- Region
- Category
- Sub-Category
- Sales
- Quantity
- Discount
- Profit

Important limitation: this version of the dataset does not contain Order ID, Customer ID, Product ID, or transaction dates. The analysis is therefore performed at the available record level rather than unique-order, customer, product, or time-series level.

For the fully executable hosted notebook, use the Kaggle version linked in the project README.
