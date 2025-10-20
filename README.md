# 🌍 Happiness Drivers Analysis  
*What makes people happy? Can you find Dytopia?*  

---

## 📘 Introduction  
The **World Happiness Report** is a landmark global survey that measures how people evaluate their lives in over **150 countries**.  
It provides deep insights into how **economic**, **social**, and **institutional** factors influence subjective well-being.  

This project explores **global happiness trends** and the **key drivers** — such as GDP per capita, social support, freedom of choice, generosity, health, and corruption perception.  
It investigates how these relationships evolved **before**, **during**, and **after the COVID-19 crisis**, highlighting which factors became more (or less) important for happiness over time.

> 🧭 *“The true measure of progress is not wealth or power, but the happiness of the people.”*

<p align="center">
  <img src="https://allthatsinteresting.com/wordpress/wp-content/uploads/2016/03/giphy-4.gif" width="720" alt="Animated globe showing happiness around the world">
</p>

---

## 🎯 Goals of the Research  
- Identify which factors most strongly influence happiness  
- Explore how happiness changed across the **Pre-COVID**, **COVID**, and **Post-COVID** phases  
- Visualize and compare trends across **continents and years (2017–2023)**  
- Quantify the **unique importance** of each driver using **Fixed Effects** and **Shapley R²** analysis  

---

## ❓ Research Question  
> **How did the key drivers of happiness change before, during, and after the COVID-19 crisis?**  

Do economic, health, and social factors contribute to happiness in a stable way across time and regions —  
or did the pandemic **reweight** the importance of these drivers, shifting well-being from **wealth-based** to **relationship-based** determinants?


## 📊 Dataset Overview  

The **World Happiness Report**, published annually by the **United Nations Sustainable Development Solutions Network (SDSN)**,  
uses data from the **Gallup World Poll (2013–2023)** to rank nations based on citizens’ perceived life satisfaction.  

### 🪜 How the Data Is Collected  
Respondents answer the *Cantril Ladder* question:  
> “Imagine a ladder with steps from 0 (worst possible life) to 10 (best possible life).  
> On which step do you personally feel you stand today?”

Their average response forms each country’s **Happiness Score**.

---

### 💡 Key Indicators Influencing Happiness  

| **Indicator** | **Meaning** |
|----------------|-------------|
| `Overall_rank` | Global ranking position |
| `Country` | Country or region name |
| `Year` | Survey year (2013–2023) |
| `Happiness_Score` | National average life evaluation (0–10) |
| `GDP_per_capita` | Log GDP per capita — economic prosperity |
| `Healthy_life_expectancy` | Average healthy life expectancy (0–1) |
| `Social_support` | Strength of social and institutional networks |
| `Freedom_to_make_life_choices` | Perceived personal freedom (0–1) |
| `Generosity` | Willingness to help others (0–1) |
| `Perceptions_of_corruption` | Confidence in public institutions (inverse of corruption) |

---

### 📚 Data Source  
Data derived from:  
- 🌐 [World Happiness Report Website](https://worldhappiness.report/data/)  
- 📊 [Kaggle: World Happiness Report Dataset](https://www.kaggle.com/datasets/unsdsn/world-happiness)

**Citation:**  
> Helliwell, J. F., Layard, R., Sachs, J., & De Neve, J.-E. (Eds.).  
> *World Happiness Report 2013–2023.* Sustainable Development Solutions Network (SDSN).

---

## Tools & Libraries  
- **Python:** Pandas, NumPy, Matplotlib, Plotly, Statsmodels, Folium, GeoPandas  
- **Jupyter Notebook:** used for analysis and visualization  
- Optional: Shapley-based dominance analysis for variable importance  

---

## 📂 Repository Structure  

| Folder | Description |
|--------|--------------|
| `/data/` | Raw and processed World Happiness datasets |
| `/notebooks/` | Step-wise analysis notebooks (01–08) |
| `/results/` | CSV exports and model outputs |
| `/images/` | Saved charts and figures |
| `/src/` | Optional helper scripts (data cleaning, plotting) |

**Main Notebook:**  
📓 `happiness_drivers_analysis_project.ipynb` — runs the full workflow (Steps 1–8)

---

## ⚙️ Getting Started  

```bash
# Clone the repository
git clone https://github.com/nishaverma24/happiness-drivers-analysis.git
cd happiness-drivers-analysis

# Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate      # (Windows: .venv\Scripts\activate)

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter lab
