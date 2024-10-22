# AQI Analysis - Exploring Probability Distributions

## Project Overview

This project focuses on performing an **exploratory analysis of air quality data** with a particular emphasis on carbon monoxide levels. By utilizing statistical methods, we aim to assess the distribution of AQI readings, calculate z-scores, and detect outliers to understand air quality trends and identify areas needing improvement.

Through this analysis, we will employ log transformations to normalize skewed data and ensure that our findings are robust and meaningful.

## Table of Contents

- [Introduction](#introduction)
- [Tools Used](#tools-used)
- [Project Structure](#project-structure)
- [Data Analysis Steps](#data-analysis-steps)
  - [Step 1: Imports and Data Loading](#step-1-imports-and-data-loading)
  - [Step 2: Data Exploration](#step-2-data-exploration)
  - [Step 3: Statistical Tests](#step-3-statistical-tests)
  - [Step 4: Outlier Detection](#step-4-outlier-detection)
- [Key Insights](#key-insights)
- [Conclusion](#conclusion)
- [How to Run](#how-to-run)
- [References](#references)

## Introduction

Air quality is a critical public health issue, and understanding the factors that influence it is essential for policy-making and intervention. This project analyzes a dataset from the United States Environmental Protection Agency (EPA), focusing on air quality indicators, particularly carbon monoxide levels.

The analysis seeks to answer the following questions:

- How does the distribution of AQI readings behave?
- Are there any significant outliers in the data?
- What insights can we derive about air quality improvements based on the analysis?

## Tools Used

- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization.
- **SciPy**: For statistical analysis.

## Project Structure

This analysis is divided into the following sections:

- **Step 1: Imports and Data Loading**: Import relevant libraries and load the dataset.
- **Step 2: Data Exploration**: Explore the dataset characteristics and visualize the distribution.
- **Step 3: Statistical Tests**: Apply the empirical rule to assess normality.
- **Step 4: Outlier Detection**: Identify potential outliers using z-scores.

## Data Analysis Steps

### Step 1: Imports and Data Loading

We begin by importing the necessary libraries and loading the dataset into a Pandas DataFrame to start the analysis process.

### Step 2: Data Exploration

- **Visualizing Data**: Create a histogram of the AQI readings to assess their distribution.
- **Log Transformation**: Apply log transformation to the AQI data to normalize skewed distributions and stabilize variance.

### Step 3: Statistical Tests

- **Empirical Rule**: Assess the normality of the data by applying the empirical rule, which states that:
  - 68% of the data falls within 1 standard deviation of the mean
  - 95% of the data falls within 2 standard deviations of the mean
  - 99.7% of the data falls within 3 standard deviations of the mean

Define the mean and standard deviation, then verify how closely the data adheres to these expectations.

### Step 4: Outlier Detection

- **Identifying Outliers**: Utilize the z-score approach to detect outliers in the AQI data. A value is considered an outlier if its z-score exceeds 3 in absolute value. Compute the z-scores for the AQI readings and identify any significant outliers.

## Key Insights

- The distribution of AQI readings appears approximately normal after applying log transformation.
- Statistical tests confirm the presence of a few potential outliers, notably at the West Phoenix site, indicating areas that require further investigation for air quality improvement.
- The analysis illustrates the importance of understanding data distribution and outlier detection in environmental assessments.

## Conclusion

This project emphasizes the significance of exploring probability distributions and detecting outliers in air quality data. By systematically analyzing the data, we have gained valuable insights that can inform decisions related to air quality management and policy-making.

## How to Run

1. **Clone the repository**:

    ```bash
    git clone <https://github.com/MahmoudKhaled98/AQI-Analysis-Exploring-Probability-Distributions.git>
    ```

2. **Install the required dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Jupyter notebook**:

    ```bash
    jupyter notebook
    ```

## References

- US EPA, OAR. 2014, July 8. [Air Data: Air Quality Data Collected at Outdoor Monitors Across the US](https://www.epa.gov/outdoor-air-quality-data).
- [Pandas Documentation](https://pandas.pydata.org/)
- [NumPy Documentation](https://numpy.org/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [SciPy Documentation](https://www.scipy.org/)
