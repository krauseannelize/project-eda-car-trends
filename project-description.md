# Project Description | Car Dataset

## Intro

Welcome to the project sprint where you are about to start working with an interesting dataset about cars! You’ll have a chance to practice everything in this course! If it sounds exciting, let’s start with the dataset description. The data itself is available for downloading via [this link](/notebooks/s06_project/car-data.csv).

## 🚗 Dataset Description

You are given a car dataset with the following columns:

- **Make**: The manufacturer of the car (e.g., Toyota, Ford, BMW).
- **Model**: The specific model name of the car.
- **Year**: The production year of the car.
- **Engine Fuel Type**: Type of fuel the car uses (e.g., gas, diesel, electric, hybrid).
- **Engine HP**: The horsepower of the car's engine.
- **Engine Cylinders**: The number of cylinders in the car's engine.
- **Transmission Type**: The type of transmission in the car (e.g., automatic, manual).
- **Driven_Wheels**: The type of drivetrain (e.g., front-wheel drive, rear-wheel drive, all-wheel drive).
- **Number of Doors**: Number of doors the car has (e.g., 2, 4).
- **Market Category**: The market segment the car belongs to (e.g., SUV, sedan, luxury).
- **Vehicle Size**: The size category of the car (e.g., compact, mid-size, large).
- **Vehicle Style**: The style of the vehicle (e.g., coupe, convertible, hatchback).
- **highway MPG**: The estimated miles per gallon on the highway.
- **city mpg**: The estimated miles per gallon in the city.
- **Popularity**: A numerical value indicating how popular the car is in the market.
- **MSRP**: The Manufacturer's Suggested Retail Price of the car.

Your goal is to **clean, transform, and analyze the data** by performing the tasks below.

## 🛠️ Tasks

### 1. Data Cleaning

#### 1.1 Handle Missing Data

- Identify if there are missing values
- Decide how to handle missing data for each column (e.g., fill with appropriate values, drop rows, etc.).

#### 1.2 Data Type Conversion

- Ensure that columns are of the correct data type for analysis (e.g., ensure that `Year` is an integer or float).

#### 1.3 Filter Data

- Filter the dataset to only include cars **from the year 1995 and later**.

#### 1.4 String Operations

- Standardize text entries by converting these columns' entries to lowercase:
  - `Vehicle Style`
  - `Market Category`

### 2. Feature Engineering

#### 2.1 Create New Columns

- Create a column called `Total MPG` that is the **average of `city mpg` and `highway MPG`**.
- Create a column called `Price per HP` calculated as:
  - `MSRP / Engine HP`.

### 3. Exploratory Data Analysis (EDA)

#### 3.1 Descriptive Statistics

- Calculate summary statistics (mean, median, standard deviation) for the following columns:
  - `Engine HP`
  - `MSRP`
  - `Popularity`
  - `highway MPG`
  - `city mpg`

#### 3.2 Group Analysis

- Group the data by the following columns and calculate the **average `MSRP` and `Popularity`** for each group:
  - `Driven_Wheels`
  - `Vehicle Size`
  - `Engine Cylinders`

#### 3.3 Visualizations

- Generate the following visualizations:
  - A **histogram** that shows a distribution for the `city mpg` column.
  - A **bar chart** showing the average `MSRP` for each category in `Vehicle Size`.
  - A **scatter plot** showing the relationship between `Engine HP` and `MSRP`.
  - A **boxplot** showing the distribution of `MSRP` for each category in `Driven_Wheels`.
  - A **line plot** showing trends in average `city mpg` and `highway MPG` for different `Transmission Type`.

#### **3.4 Correlation Analysis:**

- Investigate the correlation between the following variables:
  - `Engine HP`
  - `MSRP`
  - `Popularity`
  - `highway MPG`
  - `city mpg`

## 📊 Deliverables

- A **cleaned dataset** with all missing data addressed, data types fixed, and filters applied.
- All new features (columns) created as described in the feature engineering section.
- Visualizations that answer the following questions:
  - What trends exist in pricing (`MSRP`) and market size (`Vehicle Size`)?
  - How does horsepower (`Engine HP`) relate to price (`MSRP`)?
  - Is there a significant difference in price (`MSRP`) for different drivetrains (`Driven_Wheels`)?
  - How do MPG (`city mpg` and `highway MPG`) trends change with transmission type (`Transmission Type`)?
- A short written summary (1-2 paragraphs) outlining:
  - Insights derived from the analysis.
  - Patterns or trends identified from visualizations.
