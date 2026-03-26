# DAS-Group-16
# Project 16 - Measles Susceptibility in Edinburgh

This project examines measles susceptibility among primary school children in Edinburgh, focusing on whether the retraction of the 1998 Wakefield study influenced the susceptibility rates. The data is drawn from 101 intermediate zones (IZs) in Edinburgh, covering the period from 1998 to 2012. The dataset contains information on the total number of pre-school children (𝑁), the number of susceptible children (𝑌), and the year of data collection.

## Objective

The primary goals of this project are to:
1. Investigate whether Edinburgh experienced a change in measles susceptibility following the retraction of the controversial Wakefield article.
2. Determine if this change, if any, occurred specifically in 2004, the year of the article's retraction.

## Dataset

The dataset used in this analysis is stored in the file `DAProject16.csv` and includes the following columns:
- **Y**: The number of pre-school children susceptible to measles in a given IZ.
- **N**: The total number of pre-school children in a given IZ.
- **Year**: The year in which the data was collected.

### Summary of Key Variables:
- **Y**: Number of susceptible children in each intermediate zone.
- **N**: Total number of children in each intermediate zone.
- **Year**: Year of the data collection.

## Methods

### 1. Exploratory Data Analysis (EDA)
The exploratory analysis begins by calculating the susceptibility proportion (𝑌 / 𝑁) for each intermediate zone. Descriptive statistics and graphical visualizations (e.g., box plots and trends over time) were used to identify patterns in measles susceptibility and to highlight any shifts around the time of the article’s retraction.

### 2. Statistical Modeling
#### Model 1: Temporal Trend
A logistic regression model was used to analyze the temporal trend in measles susceptibility across the years. The model tested whether susceptibility had changed over time, taking into account the year of data collection.

#### Model 2: Change Post-2004
A second model was employed to assess whether there was a noticeable change in measles susceptibility after the retraction of Wakefield’s article in 2004. This model included an indicator variable (Post2004) to capture any additional change after the retraction.

### 3. Model Comparison
A likelihood ratio test was conducted to compare the models and determine if the inclusion of the Post2004 variable improved the model fit. The results confirmed that the model with the Post2004 indicator provided a significantly better fit to the data.

## Key Findings

- **Temporal Trends**: The analysis revealed a consistent downward trend in measles susceptibility over time, with the odds of susceptibility decreasing by approximately 4.8% per year on average.
- **Impact of the Wakefield Retraction**: The introduction of the Post2004 variable showed that while the overall trend remained negative, there was a statistically significant shift in susceptibility levels post-2004. The odds of susceptibility increased by approximately 19% for data collected after 2004 compared to the expected trend.
  
## Conclusion

The results of the temporal trend model confirmed a significant reduction in susceptibility over the study period. The inclusion of the post-2004 indicator revealed a structural shift in measles susceptibility following the retraction of the Wakefield article, highlighting its potential impact on public health behaviors. This analysis underscores the complex dynamics of public health trends and the importance of addressing misinformation in shaping public health outcomes.

Further research could explore regional variations in susceptibility across Edinburgh’s intermediate zones, and analyze factors such as vaccination rates and health interventions that may have contributed to these changes in susceptibility.

## Files in This Repository

- **`DAProject16.csv`**: The dataset containing measles susceptibility data from 1998 to 2012.
- **`Group_16_Analysis.qmd`**: Quarto file containing the full analysis, statistical models, and results.

## Authors

Group 16: 2889642, 2888928, 2960701, 2896766
