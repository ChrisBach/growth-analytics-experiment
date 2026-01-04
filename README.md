# Growth Analytics Experiment — GMV Uplift Analysis

## Overview
- End-to-end growth analytics project simulating a randomized experiment to evaluate GMV impact using transactional data
- Dataset: https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset?select=online_retail.csv

## Key Skills Demonstrated
- SQL-style data aggregation with pandas
- Experiment design (control vs treatment, pre/post)
- Difference-in-differences analysis
- Bootstrap-based statistical validation
- Business-focused interpretation of results

## Project Structure
data/
  - raw # Original transaction data from Kaggle/        
  - processed # Cleaned and aggregated datasets/  

notebooks/
  - 01_metrics_and_experiment_setup.ipynb/
  - 02_experiment_analysis.ipynb/
  - 03_statistical_validation.ipynb/

## Key Findings
- Positive GMV uplift observed in treatment group
- Statistical validation confirms robustness of results
- Growth driven primarily by order frequency

## Tools
Python, pandas, NumPy, SciPy, Matplotlib, Seaborn

## Author
Cuong Hai Bach
