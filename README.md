# Wealth vs. Happiness: A Global Data Analysis Study  
**Created by:** Harsheta Sharma  

## 📖 Overview  
**"Wealth_Happiness_Global_DataAnalysis_Study"** explores one of the most debated questions in social science: *Does money buy happiness?*  

This project takes a **data analytics** approach, comparing **GDP per capita** (as a measure of national wealth) with **happiness scores** across countries from 2005–2024 using data from the **World Happiness Report**. The analysis was conducted at the **country level** to uncover broader economic and social patterns, rather than individual perceptions.

---

## 🎯 Project Objectives  
- Investigate whether a country's **GDP per capita** directly affects the **overall happiness** of its citizens.  
- Lay the groundwork for future exploration of other happiness factors such as **freedom, generosity, and social support**.
![Price of Joy dashboard](dashboard.png)
---

## 🧠 Methodology  

### 1. Data Acquisition  
- **Dataset:** [World Happiness Report (2005–2024)](https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated/data)  
- **Tools:**  
  - `kaggle` API for direct, scalable data imports.  
  - `kagglehub` for programmatic access and automatic dataset updates.

### 2. Data Processing (`Logic.py`)  
- **Libraries:** `pandas`, `numpy`  
- **Steps Performed:**  
  - Extracted and loaded CSV data into Pandas DataFrames.  
  - Cleaned and renamed columns using dictionaries for semantic clarity.  
  - Transformed the `Life_Ladder` column into a percentage format for improved readability.  
  - Saved the preprocessed data to a new dataset using `to_excel()` for visualization.

**Key Columns Used:**  

| Column | Description |
|---------|--------------|
| `Log GDP per capita` | Natural log of GDP per person (PPP-adjusted). |
| `Life_Ladder` | Happiness score derived from the Cantril Ladder scale (0–10). |

---

## 📊 Visualizations (`app.py`)  

The web app was built using **Dash** and **Plotly**, with **Bootstrap** for a responsive layout.  

### Visual Components  
1. **Scatter Plot:**  
   - Shows the relationship between GDP and Happiness.  
   - Displays a positive correlation — higher GDP values generally align with higher happiness levels.

2. **Line Graph:**  
   - Tracks happiness trends over time.  
   - Useful for observing changes year-to-year but requires contextual data (e.g., global events).

3. **Bubble Chart:**  
   - Visual variation of GDP vs. Happiness, incorporating bubble size to represent additional variables.  
   - Reinforces findings from the scatter plot.

### Dash Components Used  
- `dash_core_components` (Graphs, Markdown, Interactivity)  
- `dash_html_components` (Layout Elements)  
- `dash_bootstrap_components` (Navigation and Styling)  
- `@app.callback` decorators for interactive behavior between charts and pages  

---

## 🚀 How to Run the Project  

### Prerequisites  
Make sure you have **Python 3.9+** and the following libraries installed:  
```
pip install pandas plotly dash dash-bootstrap-components kaggle kagglehub
```

### Launch Instructions  
1. Clone the project repository:  
   ```
   git clone https://github.com/HARSHEE04/Wealth_Happiness_Global_DataAnalysis_Study.git
   cd Wealth_Happiness_Global_DataAnalysis_Study
   ```  
2. Run the Dash app:  
   ```
   python app.py
   ```  
3. Click on the generated local URL to open the web interface.  

---

## 📈 Insights & Findings  
- **Positive correlation** observed between GDP per capita and happiness scores.  
- Countries with higher wealth indices tend to report higher levels of life satisfaction.  
- However, GDP alone doesn’t account for all variance — secondary factors like **social support, generosity, and freedom** likely influence overall happiness.

---

## 🧩 Future Enhancements  
- Integrate additional variables (e.g., **freedom, corruption perception, social trust**) into multivariate visualizations.  
- Conduct **regression modeling** to quantify variable influence.  
- Build **filter-based interactivity** for continent or year-based exploration.  
- Deploy a **public-hosted version** using Heroku or Render for live demos.



