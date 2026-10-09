# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across different product categories.

The objective is to uncover insights into:

- Customer spending patterns
- Product preferences
- Customer segments
- Subscription behavior
- Discount usage
- Revenue trends

The project follows an end-to-end data analytics workflow using **Python, SQL, Power BI, and Gamma**.

---

## Dataset

The dataset contains **3,900 rows and 18 columns**.

### Key Features

- **Customer Demographics:** Age, Gender, Location, Subscription Status
- **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
- **Shopping Behavior:** Discount Applied, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

The dataset initially contained **37 missing values in the Review Rating column**.

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python** | Data loading, cleaning, EDA & feature engineering |
| **Pandas** | Data manipulation and analysis |
| **PostgreSQL / MySQL / SQL Server** | SQL-based business analysis |
| **Power BI** | Interactive dashboard and visualization |
| **Gamma** | Project presentation / PPT |
| **GitHub** | Project documentation and version control |

---

## Project Workflow

### 1. Data Loading & Exploration — Python

The dataset was loaded into Python using Pandas.

Initial analysis included:

- Checking dataset structure using `df.info()`
- Generating descriptive statistics using `df.describe()`
- Checking for missing values
- Understanding customer and purchase attributes

### 2. Data Cleaning

The dataset was prepared for analysis by:

- Handling missing values
- Imputing missing **Review Rating** values using the median rating of each product category
- Standardizing column names using `snake_case`
- Checking data consistency and redundancy

The `promo_code_used` column was removed after identifying redundancy with `discount_applied`.

### 3. Feature Engineering

New analytical features were created, including:

- `age_group`
- `purchase_frequency_days`

These features helped support customer segmentation and demographic analysis.

### 4. SQL Analysis

The cleaned dataset was loaded into **PostgreSQL** for structured business analysis.

Key SQL analyses included:

1. Revenue by gender
2. High-spending discount users
3. Top 5 products by rating
4. Standard vs. Express shipping comparison
5. Subscribers vs. non-subscribers
6. Products with the highest percentage of discounted purchases
7. Customer segmentation
8. Top 3 products by category
9. Repeat buyers and subscription behavior
10. Revenue by age group

### 5. Power BI Dashboard

An interactive **Power BI dashboard** was created to visualize the key findings and make the analysis easier to interpret for business users.

The dashboard focuses on customer behavior, revenue, product performance, discounts, subscriptions, and customer segments.

### 6. Report & Presentation

The analytical findings were documented in a project report and converted into a presentation using **Gamma** for clear business communication.

---

## Dashboard

The Power BI dashboard provides an interactive view of:

- Customer demographics
- Revenue performance
- Product performance
- Subscription behavior
- Discount usage
- Customer segments
- Age-group revenue contribution
- Shipping behavior

---

## Key Results & Business Recommendations

The analysis produced several actionable recommendations:

- **Boost Subscriptions:** Promote exclusive benefits for subscribers.
- **Customer Loyalty:** Reward repeat buyers and encourage movement into the Loyal segment.
- **Review Discount Policy:** Balance discount-driven sales with margin control.
- **Product Positioning:** Promote highly rated and best-selling products.
- **Targeted Marketing:** Focus marketing efforts on high-revenue age groups and express-shipping users.

---

## How to Run

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd customer-shopping-behavior-analysis
```

### 2. Install Python Dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

### 3. Run the Python Analysis

Open the Jupyter Notebook or Python script and run the data loading, EDA, cleaning, and feature engineering steps.

### 4. Set Up the SQL Database

Create a database in **PostgreSQL, MySQL, or SQL Server** and import the cleaned dataset.

Update the database connection details in the Python/SQL files according to your environment.

### 5. Run SQL Queries

Execute the provided SQL queries to reproduce the business analysis and generate the required results.

### 6. Open the Power BI Dashboard

Open the `.pbix` file in Power BI Desktop and refresh the data connection if required.

### 7. View the Report & Presentation

The project report and Gamma presentation are included in the repository for documentation and presentation of the findings.

---

## Project Structure

```text
customer-shopping-behavior-analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── notebooks/
│   └── customer_behavior_analysis.ipynb
│
├── sql/
│   └── customer_behavior_analysis.sql
│
├── powerbi/
│   └── customer_behavior_dashboard.pbix
│
├── report/
│   └── project_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
└── README.md
```

---

## Skills Demonstrated

- Data Cleaning & Preprocessing
- Exploratory Data Analysis
- Python & Pandas
- SQL Querying
- PostgreSQL Database Integration
- Feature Engineering
- Customer Segmentation
- Business Analysis
- Data Visualization
- Power BI Dashboard Development
- Business Reporting
- Data Storytelling

---

## Conclusion

This project demonstrates an end-to-end approach to transforming raw customer transaction data into actionable business insights using **Python, SQL, Power BI, and presentation tools**.
