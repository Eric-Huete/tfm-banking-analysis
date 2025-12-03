# Banking Analytics & Product Propensity Model  
### *Nuclio Digital School — Final Master's Project (TFM)*

This project analyzes the data of a fictitious banking company to uncover business insights and build a machine learning model that predicts which clients are most likely to purchase specific financial products.

It includes:

- A Power BI dashboard with KPIs on clients, sales, and product profitability  
- Full data cleaning & preparation  
- Exploratory data analysis (EDA)  
- Customer segmentation via clustering  
- A propension-to-buy ML model  

---

Data Availability

The raw datasets used in this project exceed GitHub's file size limits (25MB per file).  
For this reason, only sample processed datasets are included in `/data/processed/`.

If you need access to the full dataset for validation or review, feel free to contact me.

---

## Project Structure

```
tfm-banking-analysis
│
├── notebooks/
│   ├── Tarea 1 - Data cleaning.ipynb
│   ├── Tarea 2 - Modelo Propensión a Compra.ipynb
│   ├── Tarea 3 - Clustering.ipynb
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── initial KPIs report - PowerBI/
│   ├── PowerBI final.pbix
│   ├── dashboard_images/
│
├── requirements.txt
└── README.md
```

---

# Data Cleaning  

**Notebook:** *Tarea 1 - Data cleaning.ipynb*

Main tasks:

- Removed duplicates and inconsistent entries  
- Imputed missing values  
- Standardized product labels and categories  
- Engineered new features (age groups, product families, customer activity)  
- Merged all tables into final clean datasets  

The cleaned datasets is stored in `/data/processed/`.

---

# Exploratory Data Analysis (EDA)

The EDA revealed major behavior patterns across clients, regions, sales, and profitability.

### Customer Insights

- Largest age segment: **20–30 years old (~300k clients)**  
- Top regions: **Madrid (29.6%)**, **Barcelona (13.9%)**, **Valencia (8.4%)**  
- Multiple filters available: gender, active status, new vs. existing clients  

### New Customers

- New client acquisition shows strong **seasonality**  
- Monthly range: **11k → 94k**  
- Peaks in **August–October** consistently  

### Product Insights  

- **Most sold:** em_account (basic bank account), debit_card, pension_plan, payroll  
- **Least sold:** long_term_deposit, securities, funds, loans, mortgage  
- **Most profitable:** pension_plan, em_account  

### Sales & Benefits Summary  

- Monthly views of units sold and total benefits  
- Profit peaks:  
  - March 2018 → **14.5M€**  
  - July 2018 → **12.3M€**  
  - November 2018 → **10.5M€**  
- Slight downward trend through 2018–2019  

---

# Power BI Dashboard (KPIs)

Includes:

- Client demographics  
- New customers (monthly & yearly)  
- Most/least sold products  
- Product profitability  
- Sales to new customers  
- Global summary view  

Location:  
`/initial KPIs report/`

---

# Propensity-to-Buy Model (Machine Learning)

**Notebook:** *Tarea 2 - Modelo Propensión a Compra.ipynb*

### Workflow:

- Feature engineering  
- Encoding and scaling  
- Train/test split  
- Models trained:  
  - Logistic Regression  
  - Random Forest  
  - Gradient Boosting  

### Output  
Assigns a **purchase probability** for each product and each client.

---

# Customer Segmentation (Clustering)

**Notebook:** *Tarea 3 - Clustering.ipynb*

### Steps:

- PCA dimensionality reduction  
- K-Means clustering  
- Silhouette analysis  
- Final customer profiles:  
  - High-value frequent users  
  - Young digital-first clients  
  - Low-engagement inactive customers  
  - Long-term investment-oriented users  

---

# Business Recommendations

- **Invest in high-profit products**  
- **Focus customer acquisition in Aug–Oct**  
- **Target younger clients for entry-level products**  
- **Use the ML model for targeted marketing**  

---

# How to Run the Project

### Clone the repo

```bash
git clone https://github.com/Eric-Huete/tfm-banking-analysis.git
cd tfm-banking-analysis
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the notebooks

```bash
jupyter notebook
```

### Open the dashboard  
Located in `/initial KPIs report/`.

---

# Technologies Used

- Python (pandas, numpy, sklearn, matplotlib, seaborn)  
- Machine Learning (Logistic Regression, Random Forest, Gradient Boosting)  
- Power BI  
- Jupyter Notebooks  

---

# About the Project

This project was developed as the **Final Master Project (TFM)** for the **Nuclio Digital School — Master in Data Science & AI**.

It replicates a realistic end-to-end banking analytics workflow.
