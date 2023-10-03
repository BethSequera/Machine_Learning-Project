**UCB Data Analysis Group Project 4**
# Sea Level Rise Predictions: Gaining Insight with Predictive Analytics

---------------
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

### Data Export
The processed and transformed data was exported to a CSV file for further analysis via neural network.

### Annual Averages
We calculated annual averages of mean sea level (MSL) on all historic sea level data for all cities combined.

## Data Analysis and Modeling
Our analysis extended to modeling future sea levels with regression modeling. Key analysis and modeling tasks included:

### Linear Regression / Polynomial Regression
We implemented a linear regression model to predict future mean sea levels based on historical data. This involved:

- Grouping data by month (and subsequently by year) and city.
- Splitting the data into training and testing sets.
- Training the model and evaluating its performance using R-squared value.
- Plotting real values as scatter plot with regression line showing real and predicted values.

Disappointed in the r-squared values for regression grouped by month, the data was further summarized by year with much healthier resulting R-squared values.
Finding that the linear regression model was overly rigid, we then applied a polynomial regression model on the data grouped by year. This model succeeded in accurately visualizing the accelerated sea level rise for all cities. 

### Neural Network
In the Neural Network phase, we employed TensorFlow and Keras to construct a powerful neural network model. This model, with carefully tuned hyperparameters, delved into complex relationships within the sea level data. It learned intricate patterns and trends, enhancing our sea level predictions by capturing the nuances in environmental factors and sea level changes. This advanced model contributed significantly to refining our predictions and gaining deeper insights into coastal sea level rise.

#### Data PRocessing
- Target:
  - MSL (ft)

- Feature:
  - Years
 
### Compiling, Training and Evaluating the Model
 - The model consit of one hidden layer with total for with 5 nodes run for 100 epochs was used to create the model and activation method *relu* . After compling the model it accuracy score 95%.
 - The model at the beginning gave 100% accuracy but after using the *Standard Scaling* method the accuray was 95%.

## Data Visualization
Data visualization played a crucial role in presenting our findings. We employed Matplotlib to create various visualizations, such as line plots, scatter plots, and bar charts, to effectively communicate our results and predictions.

A featured visualization included an engaging bar chart race animation to offer a simultaneous view of sea level changes over time for all cities.

## Results and Conclusion
The project's primary objective was to provide insights into coastal sea level trends, aiding coastal planning, climate research, and environmental monitoring efforts. Through data analysis and modeling, we not only gained valuable insights into historical sea level data but also predicted future sea levels, enhancing our understanding of this critical environmental factor.  

While this analysis resulted in an accurate sea rise prediction model, the human impact on climate has greatly accelerated global warming which significantly complicates the processes impacting ice-shelf calving and overall sea level rise.

--------------
--------------
#### Contents of Repository:
- Code Scripts
  - 2 x .ipynb python notebooks (SeaLevel_Project_4.ipynb, Neural_Model.ipynb)
- Media Files
  - 1 x .gif image (MSL_race.gif)
  - 1 x .pdf document, converted PowerPoint presentation (Predicting Future Sea Level Changes_presentation.pdf)
- Data Files
  - 1 x .csv data file, code export (reduced_data.csv)
  - 7 x .csv data files, import data (Analytics_Avengers-Boston_MA_Sea_Levels.csv, same for Charleston_SC, Honolulu_HI, Key_West_FL, SF_CA, San_Diego_CA, Seattle_WA)
- 1 x README file

-------------------
#### Contributors:
- Bethania Sequera
- Juliana Lima
- Michael Bernstein
- Mohamed Abdelsalam
- Ronda Hinz

------------------
#### License:
[MIT](https://choosealicense.com/licenses/mit/)
