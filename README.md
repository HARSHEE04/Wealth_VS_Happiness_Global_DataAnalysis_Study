# Wealth VS Happiness Global Data Analysis Study

## Overview

While economic growth is often one of the primary goals of national policy, it is unclear if increasing a nation's wealth directly translates to the well-being of its citizens. This project addresses the gap between macroeconomic output and human sentiment to determine if GDP per capita is a reliable predictor of a population's happiness and answer the question: **"Does Money Buy Happiness?"**

This end-to-end data analysis project explores the relationship between a country's wealth (measured by Log GDP per Capita) and its citizens' happiness (measured by the Life Ladder score from the World Happiness Report). Through data visualization and analysis, we investigate whether higher economic output correlates with greater subjective well-being.

## Features

- **Interactive Dashboard**: A web-based application built with Dash for exploring visualizations.
- **Data Visualizations**:
  - Scatter Plot: GDP vs. Life Ladder Score
  - Line Graph: Happiness trends over time by country
  - Bubble Chart: Enhanced scatter plot with size representing happiness levels
- **Data Processing**: Custom logic in Python for cleaning and preparing the dataset.

## Data Sources

- **World Happiness Report 2024**: Dataset sourced from Kaggle, containing happiness scores, GDP data, and other socio-economic indicators for various countries over multiple years.
- Key files:
  - `World-happiness-report-2024.csv`
  - `World-happiness-report-updated_2024.csv`
  - `World Happiness_Final.xlsx`
  - `WorldHappy.zip` (archived additional data)

## Technologies Used

- **Python**: Core programming language
- **Dash**: Framework for building the interactive web dashboard
- **Plotly**: Library for creating interactive charts and graphs
- **Dash Bootstrap Components**: For styling the dashboard with Bootstrap themes
- **Pandas**: For data manipulation and analysis (used in `Logic.py`)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/HARSHEE04/Wealth_VS_Happiness_Global_DataAnalysis_Study.git
   cd Wealth_VS_Happiness_Global_DataAnalysis_Study
   ```

2. Install the required Python packages:
   ```bash
   pip install dash dash-bootstrap-components plotly pandas
   ```

3. (Optional) If you need to access Kaggle datasets, ensure `kaggle.json` is configured properly.

## Usage

1. Run the data processing script (if needed):
   ```bash
   python Logic.py
   ```

2. Launch the dashboard:
   ```bash
   python app.py
   ```

3. Open your web browser and navigate to `http://127.0.0.1:8050/` to interact with the visualizations.

## Dashboard Preview

![Dashboard Preview](dashboard.png)

## Key Findings

*(Note: Add your analysis results here after running the analysis. For example:)*
- There is a positive correlation between GDP per capita and happiness scores, but the relationship is not linear.
- Other factors like social support, health, and freedom may play significant roles in overall well-being.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Data provided by the World Happiness Report (Gallup World Poll).
- Inspired by discussions on economic policy and human development.
