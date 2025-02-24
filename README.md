# London Bike Analysis

## Overview

This project analyzes London bike rental data to explore usage patterns, the impact of weather conditions, and seasonal trends using **Python** (Jupyter Notebook) and **Tableau**. It involves data gathering, exploration, manipulation, and the creation of an interactive dashboard for data-driven decision-making.

## Dataset

- **Raw Data:** `london_bikes_raw.csv` – Original unprocessed data downloaded from Kaggle.
- **Cleaned Data:** `london_bikes_final.xlsx` – Cleaned and structured data used for analysis.

## Tools & Technologies

- **Python (Jupyter Notebook)**
  - **Data Gathering and Preparation**
      - Extracted the CSV file from the downloaded zip file using the `zipfile` library.
    - **Data Exploration and Manipulation with `pandas`:**
      - Loaded the CSV data into a pandas DataFrame.
      - Explored the data using `info()`, `shape`, and viewing sample rows.
      - **Counting Unique Values:**
        - Counted unique values in the `weather_code` and `season` columns to understand data distribution.
      - **Renaming Columns:**
        - Created a dictionary (`new_cols_dict`) with preferred column names.
        - Renamed columns for clarity using `DataFrame.rename()`.
      - **Adjusting Humidity Values:**
        - Converted humidity values to actual percentages by dividing by 100.
      - **Mapping Codes to Descriptive Labels:**
        - Created dictionaries (`season_dict` and `weather_dict`) to map numerical codes to meaningful categories.
        - Applied mappings using the `map()` function.
    - **Data Export:**
      - Exported the cleaned DataFrame to an Excel file (`london_bikes_final.xlsx`) for use in Tableau.

- **Tableau**
  - **Data Analysis and Visualization**
    - Created interactive visualizations to depict rental patterns.
    - Implemented filters and interactive elements for deeper insights.
    - Visualization types include moving average charts, heatmaps, and bar charts.
  - **Dashboard Creation**
    - Built an interactive dashboard to display key metrics and trends.
    - Applied formatting techniques to enhance visual appeal.

## Key Insights & Outcomes

- **Peak Rental Times**
  - Identified peak usage periods aligned with commuting hours and weekends.
- **Weather Impact**
  - Discovered correlations between weather conditions and bike usage trends.
  - Noted decreased rentals during adverse weather conditions.
- **Seasonal Trends**
  - Observed higher rental counts during warmer months.
- **Interactive Dashboard**
  - Developed for enhanced operational planning and decision-making.

## How to Use

1. **Data Cleaning with Jupyter Notebook:**
   - Open `scripts/data_cleaning.ipynb` in Jupyter Notebook.
   - Run all cells to process the raw data (`data/london_bikes_raw.csv`).
   - The cleaned data `london_bikes_final.xlsx` will be saved in the `data` folder.

2. **Explore the Cleaned Data:**
   - Open `london_bikes_final.xlsx` to review the prepared data.

3. **Load the Tableau Dashboard:**
   - Open `London_Bike_Rentals.twb` using **Tableau Desktop**.

4. **Interact with the Dashboard:**
   - Use filters to explore different aspects of the data.
   - Analyze trends and patterns in rental usage.

## Acknowledgments

- This project was inspired by **Mo Chen**, a data analyst in the financial sector. His YouTube tutorial, ["Data Analyst Portfolio Project | Build an Awesome Tableau Dashboard Step by Step"](https://www.youtube.com/watch?v=nl9eZl1IOKI), guided me through the process of data visualization and dashboard creation in Tableau.






