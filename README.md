# Pymaceuticals Inc. Analysis

## Overview

This project involves analyzing the performance of potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer, using data from a recent animal study conducted by Pymaceuticals Inc. The study included 249 mice that were treated with a range of drug regimens over 45 days, and their tumor development was observed and measured.

## Project Structure

The project is organized as follows:

- `Mouse_metadata.csv`: Contains metadata about the mice used in the study.
- `Study_results.csv`: Contains the study results, including tumor volume and treatment regimens.
- `pymaceuticals_starter.ipynb`: The Jupyter Notebook containing the data analysis and visualizations.

## Analysis

### Data Preparation

1. **Data Import and Merging**: The mouse metadata and study results data were merged into a single DataFrame.
2. **Data Cleaning**: Duplicate entries were identified and removed to ensure the data integrity.

### Summary Statistics

- Calculated the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

### Visualizations

1. **Bar Charts**:

   - Total number of timepoints for all mice tested for each drug regimen using Pandas.
   - Total number of timepoints for all mice tested for each drug regimen using Matplotlib.
2. **Pie Charts**:

   - Distribution of unique female versus male mice in the study using Pandas.
   - Distribution of unique female versus male mice in the study using Matplotlib.
3. **Box Plots**:

   - Distribution of the final tumor volume for all mice in each treatment group, highlighting potential outliers.
4. **Line Plot**:

   - Tumor volume versus time point for a single mouse treated with Capomulin.
5. **Scatter Plot**:

   - Mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.
   - Linear regression model plotted on top of the scatter plot to show correlation.

## Findings

1. **Capomulin and Ramicane** were found to be the most effective treatments in reducing tumor volume, as evidenced by the lower mean tumor volumes.
2. **Outliers** were identified in the Infubinol treatment group, indicating variability in its effectiveness.
3. **Correlation Analysis**: There was a positive correlation between mouse weight and average tumor volume for the Capomulin regimen, as shown by the scatter plot and linear regression analysis.

### Analysis Report Document

Bar charts were generated to show the total number of time points for all mice tested for each drug regimen using both Pandas and Matplotlib.

![Analysis Report Document Link](https:/https://github.com/maslla100/mathplothlib/Analysisi%Report.md)

## Instructions

To run the analysis:

1. Clone this repository.
2. Ensure you have all the required dependencies installed (Pandas, Matplotlib, SciPy).
3. Open `pymaceuticals_starter.ipynb` in Jupyter Notebook.
4. Run the cells in the notebook to see the analysis and visualizations.

## Conclusion

This analysis provides insights into the effectiveness of different treatment regimens for SCC in mice, with Capomulin and Ramicane showing the most promise. Further studies and clinical trials would be necessary to confirm these findings and determine their applicability to human patients.

## Contact

For any questions or further information, please contact Luis Llamas at Luis.Llamas@maslla.com

---

This project was completed as part of a data analysis assignment for UT Course. The data was generated by Mockaroo, LLC (2022).
