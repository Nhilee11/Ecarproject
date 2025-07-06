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
## ❓ Research Questions

This project aims to answer:

1. What car attributes are most correlated with price in the EV segment?
2. Do newer EVs with longer EPA range or better efficiency command a premium?
3. Which brands dominate the high-end and low-end price spectrum?


## 📷  Visualizations

**Does mileage affect resale value of EVs?**
#### ✅ Conclusion:
While **mileage does tend to reduce resale price**, the relationship is **not strong nor consistent** across years. Other factors (year, brand, efficiency) likely have stronger influence.

> Correlation ≈ **-0.3197** globally, indicating a **weak but present negative relationship** between usage and price.


---
##  Self-Evaluation

What went well:
- Successfully collected real-world data via web scraping.
- Gained hands-on experience in EDA and correlation analysis.

What could be improved:
- Could have added price prediction models and compared performance.
- More visualizations (e.g., price vs. battery capacity, brand frequency).
- Include a clearer interpretation of insights after each visualization.

Next steps:
- Apply regression models (e.g., Linear, XGBoost) to predict price.
- Deploy via Streamlit or Flask for an interactive demo.


