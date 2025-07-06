# 🔍 Electric Vehicles Price Analysis 

This is a learning project that focuses on exploring and modeling the prices of electric vehicles (EVs) using real-world listings data from [Edmunds.com](https://www.edmunds.com/).
---

## Project Objective

To analyze and model the price of electric vehicles using machine learning methods and identify the relationship between key features and final listing price.

---

##  Data Collection

- Scraped from Edmunds.com using a custom web scraper.
- Used Python libraries:
  - `requests` – for HTTP requests
  - `beautifulsoup4` – for HTML parsing
  - `csv` – for saving data
  - `tqdm` – for a progress bar during loops

> ✅ Each car listing includes multiple technical and performance attributes, making it ideal for ML modeling.

---

## Contents

| Section | Description |
|--------|-------------|
| 📦 Data Collection | Web scraping logic and raw dataset creation |
| 🧹 Data Cleaning | Handling missing values, formatting |
| 📈 Exploratory Analysis | Correlation heatmaps, price distribution |
| 📊 Feature Engineering | Preparing categorical/numerical data |
| 🤖 ML Modeling | Regression models to predict prices |
| 🖼️ Visualization | Charts and plots to show insights |

---
## ❓Questions

**Q: Does mileage affect the resale value of EVs?**
While **mileage does tend to reduce resale price**, the relationship is **not strong nor consistent** across years. Other factors (year, brand, efficiency) likely have a stronger influence.

> Correlation ≈ **-0.3197** globally, indicating a **weak but present negative relationship** between usage and price.
![download (2)](https://github.com/user-attachments/assets/06516ff2-4951-44fb-9b19-67135ef9b4cb)


**Q: Does longer charging time (EPA Time to Charge) reduce EV resale value?**

This result is **counterintuitive** — we expect shorter charging time to increase value. However:
- Vehicles with **larger batteries** (e.g., long-range or luxury EVs) usually take longer to charge.
- These models also have **higher prices**, which explains the **positive correlation**.
- In this context, **longer charge time is a proxy for higher battery capacity**, not inefficiency.

> Longer charging time **does not reduce** price — it often correlates with premium or long-range EVs.
![download (3)](https://github.com/user-attachments/assets/1b138393-ce2e-4855-a9fa-0f21d8b56ad1)

---
##  Self-Evaluation

What went well:
- Real-world dataset from Edmunds listings was collected manually via scraping, giving the project a practical foundation.
- Basic EDA and hypothesis testing were completed, with visualizations supporting key assumptions (e.g., mileage vs. price, year vs. price).
- Use of regression plots and Pearson correlations added credibility to findings.

What needs serious improvement:

| Area                     | Critique                                                                                                                                                       |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Depth of analysis     | The project **scratches the surface**. Many insights are **descriptive** rather than analytical or explanatory.                                                |
| Visualizations        | Plots are basic and not always interpretable without strong labeling or annotations. There's **no use of multivariate plots** or feature interaction analysis. |
| Modeling              | Despite importing machine learning libraries, **no model was trained, validated, or interpreted**. The “ML” claim in the objective remains **unfulfilled**.    |
| Statistical rigor     | There is **no discussion of significance, confidence, or variance**, nor any diagnostic tests for outliers or data imbalance.                                  |
| Reusability           | The code lacks modularization (e.g., functions or pipeline structure), making it **not reusable or scalable**.                                                 |
| File structure        | There is **no structured project layout** (e.g., data/ vs. notebook/ vs. images/), reducing professionalism.                                                   |
| Insight communication | Many insights are **obvious (e.g., newer cars are more expensive)** and lack **business or market context** to be impactful.                                   |

**What to improve next**

Train actual regression models and compare their performance (e.g., Linear Regression, XGBoost).
Include feature importance charts, especially to evaluate the weight of each variable.
Use residual plots or cross-validation to validate model quality.\
Add multivariate analysis: e.g., Price ~ Year + Mileage + Brand (as categorical).
Explore NLP on car descriptions or sentiment from reviews to expand insights.
Apply interactive dashboards (Streamlit/Plotly) to make the project portfolio-ready.


> This project shows good data handling basics but falls short of being an end-to-end data analysis pipeline. It’s an incomplete MVP (minimum viable project) with potential — but must go deeper to truly impress in a data analyst or data science portfolio.




