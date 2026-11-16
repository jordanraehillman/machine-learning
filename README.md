# Customer Segmentation Using K-Means Clustering

### Unsupervised Machine Learning | Python | Scikit-learn

## Project Overview

This project applies unsupervised machine learning to identify customer segments based on income and spending behavior.

Using Python and K-Means clustering, customers are grouped according to similarities in their financial and purchasing characteristics. The resulting clusters are analyzed to identify patterns in customer demographics and spending behavior.

The project demonstrates how machine learning can transform customer data into meaningful insights that support business decision-making.

## Tools & Technologies

- **Python** – Data analysis and machine learning
- **Pandas** – Data manipulation and aggregation
- **NumPy** – Numerical operations
- **Scikit-learn** – Data standardization and K-Means clustering
- **Matplotlib** – Data visualization
- **Jupyter Notebook** – Interactive analysis and documentation

## Dataset

The project uses `mallcustomers.csv`, containing customer demographic and spending information.

Key variables include:

| Variable | Description |
|---|---|
| CustomerID | Unique customer identifier |
| Gender | Customer gender |
| Age | Customer age |
| Income | Customer income |
| SpendingScore | Customer spending behavior score |

## Methodology

### 1. Data Preparation

- Loaded the dataset using Pandas.
- Reviewed data types and sample records.
- Cleaned the Income field by removing commas and currency labels.
- Removed CustomerID from the analysis.
- Standardized Income and SpendingScore using `StandardScaler`.

### 2. Determining the Optimal Number of Clusters

Applied the **Elbow Method** to evaluate K-Means models with 1 through 10 clusters.

Within-Cluster Sum of Squares (WCSS) was calculated to evaluate clustering performance.

Based on the analysis, **K = 5** was selected.

### 3. K-Means Clustering

Applied K-Means clustering using standardized Income and SpendingScore values.

Customers were assigned to one of five clusters based on similarities in these characteristics.

The resulting clusters were visualized using a scatter plot showing customer groups and cluster centroids.

### 4. Customer Segment Identification

The five clusters were assigned descriptive names:

| Customer Segment | Description |
|---|---|
| Average Customers | Moderate income and spending |
| Higher Income High Spend | Higher-income customers with high spending scores |
| Lower Income High Spend | Lower-income customers with high spending scores |
| Higher Income Low Spend | Higher-income customers with low spending scores |
| Lower Income Low Spend | Lower-income customers with low spending scores |

### 5. Demographic Analysis

Each customer segment was further analyzed using:

- Number of customers
- Percentage of total customers
- Average age
- Gender distribution
- Average normalized income
- Average normalized spending score

A consolidated summary table was created to compare customer segments and their demographic characteristics.

## Results & Insights

The analysis demonstrates how K-Means clustering can identify distinct groups of customers based on income and spending patterns.

By combining cluster assignments with demographic analysis, the project provides a more complete understanding of customer characteristics.

Potential business applications include:

- Targeted marketing strategies
- Customer segmentation
- Personalized promotions
- Resource allocation
- Customer behavior analysis

**Note:** Cluster labels describe the relative characteristics of groups within this dataset. Income and spending values were standardized before clustering.

## Repository Contents

```text
customer-segmentation-kmeans/
│
├── README.md
├── LICENSE
├── .gitignore
├── unsupervisedHW 2026.ipynb
└── mallcustomers.csv
```

## How to Run

1. Clone or download this repository.
2. Install Python and Jupyter Notebook.
3. Install the required libraries:

```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

4. Ensure `mallcustomers.csv` is located in the same directory as the notebook.
5. Open `unsupervisedHW 2026.ipynb` in Jupyter Notebook.
6. Run the notebook cells sequentially.

## Skills Demonstrated

- Data cleaning and preprocessing
- Feature scaling and normalization
- Unsupervised machine learning
- K-Means clustering
- Elbow Method for model selection
- Data visualization
- Customer segmentation
- Demographic analysis
- Data aggregation and reporting

*Written with assistance from AI
