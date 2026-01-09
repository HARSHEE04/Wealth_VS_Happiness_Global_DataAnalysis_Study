# Wealth VS Happiness Global Data Analysis Study

## Overview

While economic growth is often one of the primary goals of national policy, it is unclear if increasing a nation's wealth directly translates to the well-being of its citizens. This project addresses the gap between macroeconomic output and human sentiment to determine if GDP per capita is a reliable predictor of a population's happiness and answer the question: **"Does Money Buy Happiness?"**

This end-to-end data analysis project explores the relationship between a country's wealth (measured by Log GDP per Capita) and its citizens' happiness (measured by the Life Ladder score from the World Happiness Report). Through data visualization and analysis, we investigate whether higher economic output correlates with greater subjective well-being.

## Methodology

1. **Data Acquisition**: Downloaded the World Happiness Report 2024 dataset from Kaggle using the Kaggle API and kagglehub library for programmatic access.

2. **Data Extraction**: Extracted the contents from the downloaded zip file to access the CSV data.

3. **Data Loading and Exploration**:
   - Loaded the CSV file using Pandas with ISO-8859-1 encoding to handle special characters.
   - Explored the dataset structure, including column names, data types, and value distributions for key variables such as country, year, Life Ladder, GDP, freedom, generosity, social support, and life expectancy.

4. **Data Transformation**:
   - Renamed columns for clarity and ease of use (e.g., 'Country name' to 'country_name', 'Life Ladder' to 'life_ladder').
   - Converted the Life Ladder score to a percentage by scaling it from its original scale.

5. **Data Export**: Saved the cleaned and transformed data to an Excel file (`World Happiness_Final.xlsx`) for further analysis or backup.

6. **Visualization and Analysis**: Utilized Dash and Plotly to create interactive visualizations, including scatter plots, line graphs, and bubble charts, to analyze the relationship between GDP and happiness scores across countries and over time.

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
- **Pandas**: For data manipulation, cleaning, and analysis
- **Kaggle & KaggleHub**: For downloading datasets programmatically
- **Zipfile**: For extracting archived data
- **Dash**: Framework for building the interactive web dashboard
- **Plotly**: Library for creating interactive charts and graphs
- **Dash Bootstrap Components**: For styling the dashboard with Bootstrap themes

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/HARSHEE04/Wealth_VS_Happiness_Global_DataAnalysis_Study.git
   cd Wealth_VS_Happiness_Global_DataAnalysis_Study
   ```

2. Install the required Python packages:
   ```bash
   pip install dash dash-bootstrap-components plotly pandas kaggle kagglehub
   ```

3. Configure Kaggle API: Ensure `kaggle.json` is in the appropriate directory and authenticated for dataset downloads.

## Usage

1. Run the data processing script to download, extract, and clean the data:
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
