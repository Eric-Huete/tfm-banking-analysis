# Banking Analytics & Product Propensity Model  
### *Nuclio Digital School — Final Master's Project (TFM)*

End-to-end analytics project for a fictitious banking company, covering data cleaning, exploratory analysis, customer segmentation, a product-sales-propensity ML model, and a Power BI dashboard for executives.

---

## Highlights

- Built a **Propensity-to-Buy model** to predict which products clients are likely to purchase  
- Performed **EDA** on customer behavior, product sales, and profitability  
- Segmented clients using **K-Means clustering** + PCA  
- Delivered a complete **Power BI dashboard** with KPIs  
- Produced actionable **business recommendations** for the CEO  

---

## Project Structure

```
notebooks/           → all Jupyter analysis (cleaning, ML, clustering)
data/                → raw + processed datasets
initial KPIs report/ → PowerBI final.pbix + images
requirements.txt
```

---

## Data Preparation

- Removed duplicates, corrected inconsistencies  
- Engineered new features (age groups, product families, activity flags)  
- Unified all sources into a clean analytical dataset  

---

## Main Insights (EDA)

- Largest client segment: **ages 20–30 (~300k)**  
- Top regions: **Madrid, Barcelona, Valencia**  
- New clients peak in **Aug–Oct**  
- **Most sold:** em_account (basic bank account), debit_card, pension_plan  
- **Most profitable:** pension_plan, em_account  

---

## Propensity Model (ML)

Trained and evaluated:

- Logistic Regression  
- Random Forest  
- Gradient Boosting  

**Output:** predicted probability of product purchase for each client → supports targeted marketing.

---

## Customer Segmentation

Using PCA + K-Means, identified:

- High-value frequent users  
- Young digital-first clients  
- Low-engagement customers  
- Long-term investment profiles  

---

## Power BI Dashboard

Includes:

- Client demographics  
- New client trends  
- Product sales & profitability  
- Benefits over time  
- Executive summary  

Dashboard files in:  
`/initial KPIs report/`

---

## Key Business Recommendations

- Invest in **high-profit** products (pension plans, deposits)  
- Focus acquisition campaigns during **seasonal peaks**  
- Target younger clients with entry-level products  
- Use the ML model for **personalized marketing**  

---

## Tech Stack

**Python**, **Pandas**, **Scikit-learn**, **Power BI**, **Jupyter**, **Git/GitHub**

---

## About

Developed as the **Final Master Project (TFM)** for the *Nuclio Digital School Master in Data Science & AI*, simulating a real banking data scientist's job.