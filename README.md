
# Data Visualisation using Python Seaborn

This motivation for this project is to find patterns in data by using seaborn for data visualisation.

## What is Seaborn ?

 Seaborn is Python data visualisation tool that is based on matplotlib. It facilitates an interface which is used in creating informative graphs. While matplotlib works best for visualising data frames and arrays, seaborn effectively handles data frames. Seaborn is useful for exploratory data analysis and statistical graphics.

## About the dataset
 
 The dataset consists of 14454 rows and 14 columns ('date_time', 'is_holiday', 'air_pollution_index', 'humidity','wind_speed','wind_direction', 'visibility_in_miles', 'dew_point','temperature', 'rain_p_h','snow_p_h','clouds_all','weather_type','weather_description'). 

## Assumptions
 The dataset under consideration is a large dataset with over 14k rows. Before beginning the process of data visualisation, let's try to perform some on the surface analysis of the dataset to get a general idea of the patterns.
 1. There seems to be no correlation between the temperature and weather type
 2. There seems to be no correlation between the air_pollution_index and temperature
 3. The visibilty_in_miles may be affected to the weather_type


## Data Visualisation on the weather dataset
 Seaborn can be used to perform univariate and bivariate analysis on the dataset. Univariate analysis is the simplest statistical analysis where only one variable is involved. Bivariate analysis involves analysis of two variables with the motive of finding empirical relationship between them.

 ### Univariate analysis using Seaborn
  1. Histogram : Histogram is used to display the distribution of data by forming bins along the range of data. The bars of histogram depict the observations that fall under each bin.

  2. Distplot : Distplot depicts the distribution of data for continuous variables. It basically shows the histogram with line on it.

  3. Box plot : Boxplot, also known as box and whisker diagram, makes use of quartiles to depict the numerical distribution of data. Boxplot provides a five-point summary : min,max,median,lower quartile(Q1),upper quartile(Q3). It is also used to detect the outliers in the data.

  4. Countplot : Countplot is used to depict the distribution of categorial variables. It shows the number of times the categorical variable occur in the dataset

 ### Bivariate analysis using Seaborn

 1. Scatterplot  : Scatterplot is used to derive the correlation between two numerical variables.

 2. lineplot : Lineplot is used to derive the correlation between two numerical variables using a line.

 3. regplot : regplot is essentially a scatterplot with a reression line through it.

 4. Barplot(Categorial variables) : Barplot aggregates categorial variables of the dataset based on summary static such as mean. The static can be changed to min, max, median using the estimator attribute. The length of each bar depicts the value of the static being calculated. The error bars give an indication of uncertainity around the estimate.

 5. Pointplot : Pointplot makes use of scatterplot and visualises the central tendency for the categorical variable. By default, pointplot gives indication of the mean, along with the error bars that depict the uncertainity.

 6. Jointplot : Jointplot comprises of 3 plot : one bivariate plot that depicts the relationship between the two variables and two univariate plots that depict the distribution of the two variables.

 7. Pairplot : Pairplot depicts pairwise relationships in the datasets. It creates a axes wherein each continous variable is shared acorss the x-axis and y-axis. The diagonal plots are the univariate distributions of the variable, while the rest depict the bivariate distribution.

## Conclusions/helpful findings from the project:
 The main aim of the project was to derive insights from the weather dataset. From the data visualisation, following findings were found:
 1. The temperature is the highest in cloudy weather, while Hazy and clear weather have the lowest temperatures on an average
 2. The air_pollution_index does not affect the temperature.
 3. Rainy weather has the lowest visibility in miles, while hazy weather has highest visibility.
 4. The visibilty in miles is not affected by the temperature.
 5. The air_pollution_index does not affect the temperature.

## References:

 1. The weather data used in the project is sourced from Kaggle.com
 2. https://seaborn.pydata.org/index.html


