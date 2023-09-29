# Project 4: Analyzing Coastal Sea Level Data - Analytics Avengers

## Team Members
- Bethania Sequera
- Juliana Lima
- Michael Bernstein
- Mohamed Abdelsalam
- Ronda Hinz

## Project Overview
The Analytics Avengers embarked on a project to comprehensively analyze and visualize sea level data from various coastal cities. This README file provides an in-depth overview of the project, its objectives, and the key steps involved.


## Introduction
The project's primary aim is to understand sea level trends in several coastal cities, including San Francisco, San Diego, Key West, Honolulu, Charleston, Boston, and Seattle. This analysis involves the study of mean sea level (MSL) measurements over multiple years and includes predictions for future sea levels.

## Data Processing
The project's data processing pipeline includes the following steps:

### Data Loading and Merging
We began by importing essential libraries, such as Pandas, Matplotlib, and NumPy, for data analysis and visualization. Next, we loaded sea level data for each city from separate CSV files into Pandas DataFrames. These DataFrames contained various columns, including city, region, date, and sea level measurements.

To enable a holistic analysis, we merged these separate DataFrames into one cohesive dataset.

### Data Preprocessing
To simplify the dataset and enhance its usability, we performed several preprocessing tasks:

- We removed unnecessary columns, including 'Time (GMT)', 'Highest', 'MHHW (ft)', 'MTL (ft)', 'MLLW (ft)', 'Lowest (ft)', and 'Inf'.
- Addressed missing values in the 'MHW (ft)' and 'MLW (ft)' columns using appropriate methods.
- Transformed the 'Date' column into datetime format and extracted the year as a new column.

### Annual Averages
To identify long-term trends, we calculated annual averages of mean sea level (MSL) across all cities. These averages were visualized through line plots.

## Data Analysis and Modeling
Our analysis extended to modeling future sea levels using a linear regression approach. Key analysis and modeling tasks included:

### Linear Regression
We implemented a linear regression model to predict future mean sea levels based on historical data. This involved:

- Splitting the data into training and testing sets.
- Training the model and evaluating its performance using mean absolute error (MAE).
- Making predictions for multiple future time periods.

### City-Level Analysis
For a granular analysis, we conducted separate linear regression analyses for each city. This allowed us to visualize historical data and make predictions specific to individual cities.

## Data Visualization
Data visualization played a crucial role in presenting our findings. We employed Matplotlib to create various visualizations, such as line plots, scatter plots, and bar charts, to effectively communicate our results and predictions.

## Animated Bar Chart Race
To offer a simultaneous view of sea level changes over time for all cities, we created an engaging bar chart race animation.

## Data Export
Finally, we exported the processed and transformed data to a CSV file for potential future use or further analysis.

## Results and Conclusion
The project's primary objective was to provide insights into coastal sea level trends, aiding coastal planning, climate research, and environmental monitoring efforts. Through data analysis and modeling, we not only gained valuable insights into historical sea level data but also predicted future sea levels, enhancing our understanding of this critical environmental factor. Feel free to contact the Analytics Avengers team for further information or inquiries about the project.
