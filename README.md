# Indian Import Trend Analysis

## Project Overview

The **Indian Import Trend Analysis** project explores India's import
trade data using Python. It examines import patterns across commodities,
countries, Indian states, and years to identify major import categories,
important trading partners, and changes in import values over time.

The analysis is performed in a Jupyter Notebook using data cleaning,
preprocessing, exploratory data analysis (EDA), statistical summaries,
and visualizations.

## Problem Statement

India imports a wide range of commodities from different countries to
meet consumer and industrial demand. Because of the volume and variety
of import transactions, identifying high-value commodities, key trading
partners, and regional import patterns can be difficult.

This project uses data analytics and visualization to uncover these
patterns and generate insights that can support market research and
data-driven import planning.

## Objectives

* Perform data cleaning and preprocessing to improve data quality.
* Explore the dataset using descriptive statistics.
* Analyze import trends across different years and states.
* Identify top-performing states and commodity categories.
* Examine relationships between quantity, dollar value, and INR value.
* Generate informative visualizations to support data-driven insights.
* Summarize findings and provide meaningful business insights.

---

## Data Preprocessing

Several preprocessing techniques were applied to ensure data quality and consistency:

* Checked dataset dimensions and structure.
* Identified and handled missing values.
* Removed duplicate records.
* Converted date columns into datetime format.
* Extracted year information from date fields.
* Verified and corrected data types.
* Formatted numerical values for better readability.
* Created derived features for analysis.

---

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand the dataset and discover hidden patterns.

### Univariate Analysis

* Distribution of import quantities.
* Distribution of import values.
* Commodity category frequency analysis.
* State-wise import distribution.

### Bivariate Analysis

* Relationship between quantity and import value.
* Comparison of imports across states.
* Commodity category versus import value.

### Multivariate Analysis

* Correlation analysis among numerical variables.
* State, commodity, and import value relationships.
* Multi-dimensional trend analysis.

---

## Dataset

-   **Dataset:** Imports at Principal Commodity Level
-   **Source:** [India Data Portal](https://indiadataportal.com/)
-   **Discovery:** Google Dataset Search
-   **File used in the notebook:**
    `imports-at-principal-commodity-level.csv`

The notebook works with the following fields:

  Column            Description
  ----------------- ------------------------------------------------
  `id`              Unique identifier for each import transaction
  `date`            Date of the import transaction
  `state_name`      Indian state associated with the import
  `state_code`      Code corresponding to the state
  `country`         Country from which the commodity was imported
  `port`            Port through which the commodity entered India
  `pc_code`         Principal commodity classification code
  `commodity`       Imported commodity name
  `units`           Unit of measurement
  `quantity`        Quantity imported
  `dollars_value`   Import value in US dollars
  `inr_value`       Import value in Indian rupees

## Technologies and Libraries

-   Python
-   Jupyter Notebook
-   Pandas
-   NumPy
-   Matplotlib
-   Seaborn

## Project Workflow

1.  **Data loading and initial inspection** -- load the CSV file and
    examine its structure.
2.  **Data preprocessing**
    -   Check and handle missing values.
    -   Replace missing values in `units` with `Unknown`.
    -   Check for duplicate records.
    -   Convert `date` to datetime format.
    -   Extract the year from the date.
    -   Review numerical fields such as quantity and import values.
    -   Group commodities into broader business categories.
3.  **Exploratory Data Analysis**
    -   Univariate analysis of numerical and categorical columns.
    -   Bivariate analysis across commodity categories, countries,
        states, quantity, and import value.
    -   Multivariate analysis using pivot tables.
    -   Correlation analysis of numerical variables.
4.  **Data visualization** -- create charts to explore import values,
    category shares, country contributions, state-level patterns, and
    yearly trends.
5.  **Insight generation** -- summarize the main patterns observed in
    the analysis.

## Visualizations

The notebook includes the following visual analyses:

-   Top 10 import commodities
-   Year-wise import trend
-   Import share by commodity category
-   Quantity versus import value scatter plot
-   Distribution of import values
-   Import value by commodity category (box plot)
-   Correlation heatmap
-   Import share of top countries (donut chart)
-   Country versus commodity category (stacked bar chart)
-   Yearly import trend by commodity category (stacked area chart)
-   Top 10 states by import value

## Key Findings

The notebook reports the following findings from its analysis:

-   Energy & Fuels, Oil & Seeds, and Electronics are among the major
    commodity categories by import value.
-   Import values vary across commodities, countries, states, and years.
-   China is identified in the notebook as a major import partner.
-   Gujarat, Maharashtra, and Tamil Nadu are identified among the
    leading states by import value.
-   The notebook describes an overall increase in import value from 2018
    to 2024, with a decline in 2020 followed by recovery.
-   Dollar value and INR value show a strong correlation, while quantity
    does not show a similarly strong linear relationship with import
    value.

### State-wise Import Analysis

* Gujarat emerged as the leading state in terms of total import value.
* Maharashtra and Tamil Nadu also contributed significantly to overall imports.
* Import activities are concentrated in a few major industrial and port-based states.

### Commodity Analysis

* Certain commodity categories dominate India's import expenditure.
* Energy, chemicals, and industrial raw materials account for a substantial share of imports.
* Commodity demand varies significantly across states.

### Value Analysis

* Import values exhibit a highly skewed distribution with several large transactions.
* A small number of transactions contribute disproportionately to the total import value.
* Significant outliers were observed in both quantity and value metrics.

### Correlation Analysis

* Strong positive relationships exist between quantity, dollar value, and INR value.
* Higher import quantities generally correspond to higher import values.
* Currency-converted values closely follow dollar-based import values.

### Time-based Analysis

* Import activity varies across years.
* Some years recorded significantly higher import values, indicating growth in trade volume.
* Temporal analysis helps identify periods of increased import demand.

---
These are findings recorded in the notebook and should be interpreted in
the context of the dataset and analysis performed.

## Repository Structure

A suggested GitHub structure for this project is:

``` text
indian-import-trend-analysis/
│
├── Indian Import trend Analysis .ipynb
├── imports-at-principal-commodity-level.csv
├── README.md
└── requirements.txt
```

If the dataset is distributed as an archive, extract it and place the
CSV file in the project root (or update the file path in the notebook).

## How to Run the Project

### 1. Clone the repository

``` bash
git clone <your-github-repository-url>
cd indian-import-trend-analysis
```

### 2. Create and activate a virtual environment (optional)

On Windows:

``` bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install dependencies

``` bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 4. Open Jupyter Notebook

``` bash
jupyter notebook
```

Open `Indian Import trend Analysis .ipynb` and run the cells in order.

Make sure `imports-at-principal-commodity-level.csv` is available at the
path specified in the notebook.

## Output

During preprocessing, the notebook saves the processed dataset,
including the derived year and commodity category fields, as:

``` text
imports-at-principal-commodity-level.csv
```

## Visualizations Created

The project includes a variety of visualizations to better understand the data:

1. Bar Chart
2. Line Chart
3. Pie Chart
4. Scatter Plot
5. Histogram
6. Box Plot
7. Correlation Heatmap
8. Donut Chart
9. Stacked Bar Chart
10. Stacked Area Chart

Each visualization highlights different aspects of import activity and helps uncover significant trends and patterns.

---

## Business Impact

The insights generated from this analysis can help:

* Understand regional import concentration.
* Identify high-value import sectors.
* Support trade and logistics planning.
* Assist policymakers in evaluating import patterns.
* Enable businesses to identify major importing regions and commodities.


## Future Enhancements

-   Build an interactive dashboard using Power BI or Plotly.
-   Add monthly and quarterly trend analysis.
-   Develop forecasting models for import values.
-   Explore commodity-wise and country-wise import dependency in greater
    detail.
-   Automate data updates when a refreshed dataset becomes available.

## Conclusion

This project successfully demonstrates the application of data analytics techniques to real-world trade data. Through comprehensive data cleaning, exploratory analysis, and visualization, valuable insights were derived regarding India's import activities. The findings reveal state-wise dominance, commodity-level contributions, and strong relationships among key import metrics. Overall, the project provides a data-driven understanding of import trends and showcases practical skills in Python, data analysis, and visualization.

## Author

** SARANYA CHANDRAN S **

------------------------------------------------------------------------

*This project was developed for learning and demonstrating Python-based
data analysis and visualization using Indian import trade data.*
