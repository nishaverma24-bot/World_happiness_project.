# Technical Documentation — Happiness Drivers Analysis
## 1. Objective
This project investigates global happiness trends and the key factors influencing well-being such as GDP per capita, social support, freedom of choice, generosity, healthy life expectancy, and corruption perception.  
The analysis spans 2015–2023 using data from the **World Happiness Report**.

---

## 2. Workflow Overview

| Step | Notebook | Description |
|------|-----------|--------------|
| 1 | `1_DataCollection.ipynb` | Load datasets (World Happiness, GDP, and regional indicators) |
| 2 | `2_Cleaning.ipynb` | Clean missing values, rename columns, and standardize countries |
| 3 | `3_EDA.ipynb` | Explore trends, distributions, and correlations |
| 4 | `4_DriverAnalysis.ipynb` | Perform regression & Shapley R² analysis |
| 5 | `5_Trends_COVID.ipynb` | Compare happiness levels Pre-, During-, and Post-COVID |
| 6 | `6_Final_Visuals.ipynb` | Generate final visualizations and maps |

---

## 3. Data Sources
- World Happiness Report (2015–2023) – [https://worldhappiness.report/](https://worldhappiness.report/)
- World Bank Indicators (GDP per capita, life expectancy)
- Freedom House Index
- Transparency International – Corruption Perceptions Index

---

## 4. Analytical Methods
1. **Descriptive Statistics:** Mean, median, and variation of happiness score.  
2. **Correlation Analysis:** Pearson correlation among drivers.  
3. **Fixed-Effects Regression:** Controls for country-specific influences.  
4. **Shapley R² Analysis:** Quantifies relative importance of each driver.  
5. **Trend Analysis:** Year-over-year comparison across continents.

---

## 5. Outputs
- CSV files: Cleaned datasets in `clean_data/`  
- Visuals: Charts and maps in `images/`  
- Final report: Key findings and insights summarized in `README.md`  

---

## 6. Version Control
All major updates are tracked in GitHub commits.  
Each notebook has clear markdown cells for transparency and reproducibility.
