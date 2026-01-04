# Growth Analytics Experiment — GMV Uplift Analysis

## Overview
- End-to-end growth analytics project simulating a randomized experiment to evaluate GMV (Gross Mechandise Value) impact using transactional data
- Dataset: https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset?select=online_retail.csv

1. Problem Framing
The objective of this project was to evaluate the impact of a product or marketing change on GMV. The focus was on designing a realistic end-to-end experiment workflow rather than optimizing model complexity.
2. Data Understanding & Assumptions
The dataset represents transactional e-commerce data. Each invoice corresponds to an order, with potential multiple items per order. 
Negative quantities were treated as returns and separated to avoid contaminating GMV metrics.
3. Metric Definition
Primary metric: GMV. Supporting metrics included order count and average order value. Metrics were aggregated at the order level to avoid item-level bias.
4. Experiment Design
Customers were randomly assigned to control and treatment groups using deterministic hashing. A pre/post split based on the 70th percentile of time ensured balanced data and avoided arbitrary calendar bias.
5. Analysis Approach
Difference-in-differences was used to isolate treatment effects from baseline trends. Visual inspection was performed before statistical testing to detect data issues early.
6. Statistical Validation
Bootstrap resampling was chosen due to skewed GMV distributions. Welch’s t-test was used as a secondary robustness check.
7. Business Interpretation
Results were translated into actionable insights, focusing on whether GMV changes were driven by order frequency or basket size.
8. Outcome
The project demonstrates ownership of the full analytics lifecycle: problem framing, data preparation, experimentation, validation, and executive-ready insights.


## Key Skills Demonstrated
- SQL-style data aggregation with pandas
- Experiment design (control vs treatment, pre/post)
- Difference-in-differences analysis
- Bootstrap-based statistical validation
- Business-focused interpretation of results

## Project Structure
data
  - raw # Original transaction data from Kaggle      
  - processed # Cleaned and aggregated datasets  

notebooks
  - 01_metrics_and_experiment_setup.ipynb
  - 02_experiment_analysis.ipynb
  - 03_statistical_validation.ipynb

## Key Findings
- Positive GMV uplift observed in treatment group
- Statistical validation confirms robustness of results
- Growth driven primarily by order frequency

## Tools
Python, pandas, NumPy, SciPy, Matplotlib, Seaborn

## Author
Cuong Hai Bach
