# Food Plant Experiment & Causal Analysis

## Project Overview

This project focuses on analysing manufacturing data to evaluate whether a production process change improves manufacturing performance at a fictional frozen-food company in Jaipur.

The project uses approximately 300,000 manufacturing records from three production lines. It applies statistical analysis and causal inference techniques to measure the impact of a production change on process yield.

## Project Objectives

- Clean and prepare manufacturing data for analysis.
- Design and analyse an A/B testing experiment.
- Compare Control and Treatment groups.
- Measure treatment effects using confidence intervals and statistical tests.
- Perform Difference-in-Differences analysis.
- Analyse treatment effects across production lines, suppliers, shifts and regions.
- Apply regression adjustment to estimate variance reduction.
- Prepare a final business recommendation based on the results.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Statsmodels
- Jupyter Notebook / Google Colab

## Project Structure

```text
Food-Plant-Experiment-Causal-Analysis/
│
├── data/
│   └── manufacturing_data.csv
│
├── notebooks/
│   └── Food_Plant_Experiment_Analysis.ipynb
│
├── reports/
│   ├── Experiment_Design.docx
│   └── Decision_Memo.docx
│
├── README.md
└── requirements.txt
```

## Dataset Description

The dataset contains approximately 300,000 manufacturing records with information such as:

- Production date and production line
- Region and supplier name
- Shift and machine details
- Raw material quantity
- Process yield and good output
- Wastage percentage
- Quality rejection
- Moisture percentage
- Machine downtime

The project uses simulated manufacturing data for analysis and experimentation.

## Project Methodology

### 1. Data Cleaning and Preparation
Standardized supplier names, converted raw material measurements into kilograms and handled missing moisture readings.

### 2. A/B Testing
Compared Control and Treatment groups to measure the impact of the production change on process yield.

### 3. Difference-in-Differences Analysis
Compared Jaipur (treatment region) and Ajmer (control region) to estimate the impact of the historical production change.

### 4. Segment Analysis
Evaluated treatment effects across production lines, suppliers, shifts and regions.

### 5. Regression Adjustment
Compared original and adjusted treatment effects and estimated variance reduction using available production characteristics.

## Key Findings

- The A/B test showed an estimated process yield improvement of approximately 0.97 percentage points.
- The Difference-in-Differences analysis showed a positive estimated effect.
- Segment analysis indicated positive treatment effects across the analysed groups.
- Regression adjustment estimated approximately 16.76% variance reduction.
- The estimated test duration remained 14 days.

A sample ratio mismatch was also detected during the A/B test. Therefore, the group allocation requires investigation before recommending full implementation.

## Final Recommendation

The project recommends extending the evaluation before full implementation. The company should investigate the sample ratio mismatch, validate the findings using real manufacturing data and monitor process yield, wastage and quality rejection.

## How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```text
notebooks/Food_Plant_Experiment_Analysis.ipynb
```

4. Run the notebook cells sequentially using Jupyter Notebook or Google Colab.

5. Review the analysis outputs, visualizations and final decision memo.

## Project Deliverables

- Manufacturing dataset
- Data analysis Jupyter Notebook
- Experiment Design Report
- Final Decision Memo

## Conclusion

This project demonstrates the use of Python, statistical analysis, A/B testing and causal inference techniques to evaluate manufacturing performance and support data-driven business decisions.
