# FIFA 21 Messy Dataset Analysis

## Overview

This repository contains a Jupyter Notebook that cleans and explores a raw, messy dataset of FIFA 21 players, scraped from [sofifa.com](https://sofifa.com/). Unlike typical clean datasets on Kaggle, this one is intentionally unpolished, making it an excellent resource for practicing data cleaning and exploratory data analysis (EDA).

- **Dataset Source**: Scraped from sofifa.com by yagunnersya, hosted on [Kaggle](https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring).
- **Size**: 18,979 players, 77 columns.
- **Purpose**: Learn data cleaning, transformation, and visualization with real-world messy data.

## Dataset Description

The dataset includes player details such as names, nationalities, ages, heights, weights, market values, wages, clubs, and in-game stats. It’s raw and unprocessed, featuring challenges like mixed units, special characters, and inconsistent formats—perfect for honing data wrangling skills.

## Notebook Contents

The Jupyter Notebook (`fifa_21_analysis.ipynb`) walks through the following steps:

1. **Data Loading**: Import and initial inspection of the messy dataset.
2. **Cleaning**: 
   - Convert `'Height'` and `'Weight'` to numerical values (e.g., cm, kg).
   - Remove newline characters (`\n`) and stars (`★`) from relevant columns.
   - Transform `'Value'`, `'Wage'`, and `'Release Clause'` from strings to numbers (e.g., €103.5M → 103,500,000).
   - Parse `'Contract'` and `'Joined'` for structured insights.
3. **Exploration**: Univariate, bivariate, and multivariate analyses (e.g., age distribution, OVA vs. wage).
4. **Outlier Handling**: Cap extreme values using the IQR method.
5. **Visualization**: Static (histograms, scatter plots) and interactive (Plotly choropleths, treemaps) plots.
6. **Insights**: Identify undervalued players, efficient clubs, and young talents with growth potential.
7. **Bonus**: Radar chart of top 10 players’ skill profiles.

## Key Features

- **Data Cleaning Challenges**: Mixed units (cm, feet, kg, lbs), currency strings, and inconsistent text formats.
- **Objectives Achieved**:
  - Players with >10 years at a club.
  - High-value, low-wage players via scatter plots.
  - Skill comparisons for top players.
- **Tools Used**: Pandas, NumPy, Matplotlib, Seaborn, Plotly.

## Installation

To run the notebook locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/oscarcurtog/fifa_21_notebook_EDA.git
   cd fifa_21_notebook_EDA
