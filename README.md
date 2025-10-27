# Car Trends EDA

Exploratory data analysis of car features to uncover pricing, performance, and efficiency trends.

## Tools & Skills Used

![Python](https://img.shields.io/badge/Python-EDA-%233776AB)
![Python](https://img.shields.io/badge/Python-Data%20Wrangling-%233776AB)
![Python](https://img.shields.io/badge/Python-pandas-%233776AB)
![Python](https://img.shields.io/badge/Python-numpy-%233776AB)
![Python](https://img.shields.io/badge/Python-seaborn-%233776AB)
![Python](https://img.shields.io/badge/Python-matplotlib-%233776AB)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter%20Notebook-Interactive%20Analysis-%23C35817)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Cloud%20Analysis-%23F9AB00)

## Quick Access

- [Jupyter Notebook](/car_trends_eda.ipynb)
- [Colab Notebook](https://colab.research.google.com/drive/1HnPDu1C6ZsQrizWcOqGHg2S1SAXgWlsf?usp=sharing)
- [Project Description](/project-description.md)
- [Car Trends Metadata](/car-trends-metadata.md)
- [Car Trends Dataset](/car-trends.csv)
- [Cleaned Dataset](/car-trends-clean.csv)

## Project Overview

This project, completed as part of the Masterschool Data Science program, demonstrates the full data analysis workflow to uncover insights about vehicle pricing, efficiency, and performance. I cleaned, prepared, explored, visualized, and summarized car data to identify key trends and relationships.

## Objectives

- What trends exist in pricing (`MSRP`) and market size (`Vehicle Size`)?
- How does horsepower (`Engine HP`) relate to price (`MSRP`)?
- Do different drivetrains (`Driven_Wheels`) show significant price differences?
- How do MPG trends vary by transmission type?

## Methodology

1. **Data Cleaning**  

   - Converted data types, standardized text, removed duplicate rows, and handled missing values.
   - Filtered dataset to cars from 1995 onward.

2. **Feature Engineering**  

   - **Total MPG**: average of `city mpg` and `highway MPG`.  
   - **Price per HP**: `MSRP` divided by `Engine HP`.  
   - **MSRP (K)**: scaled version of `MSRP` for improved readability.
   - Produced a cleaned dataset with engineered features (`car-trends-clean.csv`).

3. **Exploratory Data Analysis**

   - Generated descriptive statistics and grouped summaries.  
   - Built visualizations: histogram, bar chart, scatter plot, boxplot, line plot.  
   - Conducted correlation analysis across key variables.

## Key Findings

- Vehicle size, horsepower, and drivetrain all influence pricing.  
- Horsepower showed the strongest association with MSRP.  
- Larger and performance‑oriented cars generally command higher prices.  
- Drivetrain type influenced efficiency patterns, while city vs. highway usage showed weaker correlations.  

Overall, horsepower emerged as the most important driver of price, while drivetrain type shaped efficiency patterns.

## Assessment

- **Grade:** 98%
- **Instructor Feedback Highlights:**  

  - Went beyond expectations in feature engineering by adding a `MSRP (K)` column for readability.  
  - Visualizations were polished, clear, and stakeholder‑friendly with custom palettes, flipped axes and thoughtful layouts.  
  - Notebook was clean, logically structured, and well‑documented.  
  - Correlation analysis was not only presented but meaningfully interpreted.  

## Areas of Improvement

- Consider applying filtering or log transformation on `MSRP` to reduce the impact of extreme outliers.  
- Enforce consistent data types with `.astype()` to ensure robustness after imputation.  
- Add histogram commentary on skewness to highlight distribution properties.
