

# Pymaceuticals Inc. Analysis Report

## Introduction

This report presents an analysis of the potential treatments for squamous cell carcinoma (SCC) in mice, conducted by Pymaceuticals Inc. SCC is a commonly occurring form of skin cancer. The study included 249 mice treated with various drug regimens, with tumor development observed and measured over 45 days. The goal of this analysis is to evaluate the effectiveness of these treatments.

## Data Preparation and Cleaning

### Data Import

The analysis began by importing two datasets:

- `Mouse_metadata.csv`: Contains metadata about the mice used in the study.
- `Study_results.csv`: Contains the study results, including tumor volume and treatment regimens.

### Merging Datasets

The datasets were merged into a single DataFrame to facilitate a comprehensive analysis.

### Data Cleaning

Duplicate entries were identified and removed to ensure data integrity. Specifically, mouse ID `g989` was found to have duplicate time points and was excluded from the analysis.

## Summary Statistics

Summary statistics were calculated for each drug regimen, including mean, median, variance, standard deviation, and standard error of the mean (SEM) for the tumor volume.

| Drug Regimen | Mean Tumor Volume | Median Tumor Volume | Tumor Volume Variance | Tumor Volume Std. Dev. | Tumor Volume Std. Err. |
| ------------ | ----------------- | ------------------- | --------------------- | ---------------------- | ---------------------- |
| Capomulin    | 40.68             | 41.56               | 24.95                 | 4.99                   | 0.33                   |
| Ceftamin     | 52.59             | 51.78               | 39.29                 | 6.27                   | 0.47                   |
| Infubinol    | 52.88             | 51.82               | 43.13                 | 6.57                   | 0.49                   |
| Ketapril     | 55.24             | 53.70               | 68.55                 | 8.28                   | 0.60                   |
| Naftisol     | 54.33             | 52.51               | 66.17                 | 8.13                   | 0.60                   |
| Placebo      | 54.03             | 52.29               | 61.17                 | 7.82                   | 0.58                   |
| Propriva     | 52.32             | 50.45               | 43.85                 | 6.62                   | 0.54                   |
| Ramicane     | 40.22             | 40.67               | 23.49                 | 4.85                   | 0.32                   |
| Stelasyn     | 54.23             | 52.43               | 59.45                 | 7.71                   | 0.57                   |
| Zoniferol    | 53.24             | 51.82               | 48.53                 | 6.97                   | 0.52                   |

## Visualizations

### Bar Charts

Bar charts were generated to show the total number of time points for all mice tested for each drug regimen using both Pandas and Matplotlib.

![Bar Chart](/Pymaceuticals/images/barplot.png)

### Pie Charts

Pie charts were created to show the distribution of unique female versus male mice in the study using both Pandas and Matplotlib.

![Pie Chart](/Pymaceuticals/images/piechart.png)

### Box Plots

Box plots were generated to show the distribution of the final tumor volume for all mice in each treatment group. Outliers were identified and highlighted.

![Box Plot](/Pymaceuticals/images/boxplot.png)

### Line Plot

A line plot was created to show the tumor volume versus time point for a single mouse treated with Capomulin.

![Line Plot](/Pymaceuticals/images/lineplot.png)

### Scatter Plot

A scatter plot was generated to show the relationship between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen. A linear regression model was plotted on top of the scatter plot to show the correlation.

![Scatter Plot](/Pymaceuticals/images/scatterplot.png)

## Analysis and Findings

### Effectiveness of Treatments

- **Capomulin and Ramicane** were the most effective treatments in reducing tumor volume, as evidenced by the lower mean tumor volumes.
- **Outliers** were identified in the Infubinol treatment group, indicating variability in its effectiveness.

### Correlation Analysis

- There was a positive correlation between mouse weight and average tumor volume for the Capomulin regimen, suggesting that heavier mice tend to have larger tumors.

## Conclusion

This analysis provides valuable insights into the effectiveness of various treatment regimens for SCC in mice. Capomulin and Ramicane show the most promise in reducing tumor volume. Further studies and clinical trials are necessary to confirm these findings and determine their applicability to human patients.

## Instructions for Reproduction

To reproduce this analysis:

1. Clone the repository from GitHub.
2. Ensure you have all the required dependencies installed (`Pandas`, `Matplotlib`, `SciPy`).
3. Open `pymaceuticals_starter.ipynb` in Jupyter Notebook.
4. Run the cells in the notebook to see the analysis and visualizations.

## Contact

For any questions or further information, please contact Luis Llamas at Luis.Llamas@maslla.com
