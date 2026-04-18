# 🎮 Video Game Industry Analysis: Market Trends & Predictive Insights

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-white.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange.svg)
![Statistical_Testing](https://img.shields.io/badge/Stats-T--Test-green.svg)

## 📋 Project Overview
This project performs a comprehensive historical analysis of the video game industry to identify patterns that determine a game's success. Using a dataset from 2016, I developed a data pipeline to clean, process, and analyze sales and ratings across different regions (NA, EU, JP), providing a strategic outlook for the 2017 market.

**Key Objective:** Identify the "winners" (platforms and genres) and validate how expert and user reviews impact global sales through statistical rigor.

---

## 🛠️ Technical Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scipy (Stats), Matplotlib, Seaborn.
* **Techniques:** Data Imputation, Regex Pattern Matching, Exploratory Data Analysis (EDA), Hypothesis Testing (T-test).

---

## 🔍 Data Engineering & Cleaning
A significant portion of this project focused on **Data Quality**. As an engineer, I prioritized data integrity over simply deleting missing values:
* **Year Recovery:** Used **Regex** to extract years from titles (e.g., "FIFA 2006") and cross-referenced platforms to fill `year_of_release`.
* **Intelligent Imputation:** Missing scores were filled using **median** values to account for outliers, while categorical data (Ratings) used the **mode**.
* **TBD Handling:** Managed "To Be Determined" values by coercing them into numeric types to facilitate statistical operations.

---

## 📊 Key Insights & EDA
### 1. Platform Lifecycles
I identified that platforms have a peak lifecycle of **7 to 10 years**. For the 2017 strategy, the analysis focused on **PS4** and **Xbox One** as the current leaders, while noting the decline of legacy consoles like the Wii and PS3.

### 2. The "Review" Impact
* **Professional Critics:** Show a moderate positive correlation with sales (~0.40).
* **User Reviews:** Interestingly, show almost zero correlation with sales in some platforms, suggesting that marketing and brand loyalty often outweigh casual player ratings.

### 3. Regional Profiling
* **NA & EU:** Dominated by Action and Shooter genres.
* **Japan:** A distinct outlier where **Role-Playing (RPG)** is the king of the market.

---

## 🧪 Hypothesis Testing
I applied the scientific method to validate business assumptions:
* **Hypothesis 1:** "Are Xbox One and PC user ratings the same?"
    * *Method:* Independent T-Test.
    * *Result:* Failed to reject H0 (No significant difference found).
* **Hypothesis 2:** "Are Action and Sports genre ratings different?"
    * *Method:* Independent T-Test.
    * *Result:* Rejected H0 (Significant difference confirmed).

---

## 🚀 Installation & Setup

Follow these steps to set up the project and the local environment:

### 1. Clone the Repository
```bash
git clone [git@github.com:JManuelCR/video-games-sales-data-analysis.git](git@github.com:JManuelCR/video-games-sales-data-analysis.git)
cd video-game-analysis