# DS5500-HW2

# Problem 1:
Manvita Markala
Bishishta Mukherjee
Konanki Sai Charan
Romil Rathi

# Problem 2:
I have chosen the below visualization for comparison:
https://github.com/Omairss/ds5500_hw1/blob/master/Homework1.ipynb

Describe the visualization:
Visualization uses heatmap for countries to represent the trend of income over the years. This is an interesting visualization and it can provide required insights, but one thing that could have been improved here is to make it a bit clear, as there are very huge number of countries, each country's name has been represented using a 3 letter word. It can be difficult to move from country to country and at the same time understand the change of pattern through years. But, I really liked the use of heatmaps in this case.

how it is similar and/or different from yours:
I have used a chloropleth map that changes through the timeline, the dynamic chloropleth map could be more easy to interpret in some cases.

Is it easy to interpret? Does it effectively visualize what is being asked? Why or why not?
Use of heatmaps helps us in extracting insights, but at the same time due to the existence of large number of countries, the takeaway might not be simple as we need to identify the country codes and then unedrstand how the behavior changes. The 2nd stacked line chart is a very good idea, but it could have been more useful if cuts like country or continent had been provided, and the legend axes could be more explanatory.

# Problem 3:
I have chosen the below visualization for comparison:
https://github.com/nanavatirutu/DS5500

Describe the visualization:
Here, Rutu has plotted GDP, life expectancy and child mortality over time, best thing about these plots is how simple they are, this helps in easily getting the takeaway without much complexity, this graphs are easily interpretable. 

how it is similar and/or different from yours:
My approach is very similar to what has been done by Rutu, I have used continents as the split while Rutu used countries.

Is it easy to interpret? Does it effectively visualize what is being asked? Why or why not?
Yes, these graphs are very easy to interpret and are suitable for this use case. But a improvement would be to use multi axis plots. Multi axis plots help in keeping all the required data in the same graph thus help us in interpretting the graphs easily. But, with multi axis plots the graphs could get clumsy with increase in number of variables that are being displayed.


# Problem 4:

![1](/41.JPG)

Here, we would like to quantify the relation between gdp per capita and life expectancy over time. Using the available datasets we build a master dataset that contains both gdp and life expectancy, using this dataset we try to understand the relation and quantify it using graphs and modeling techniques. 

From the 1st graph we can say that there is close to linear relationship between gdp per capita and life expectancy, using the gdp and life expectancy variables we create a scatter plot, using this we can interpret that there exists a relation between the variables, this can be quantified using further analysis.

![2](/42.JPG)

By building a simple linear regression model using log of gdp per capita, life expectancy, and time. By further understanding the results of this model we can quantify the relationship. R squared of the model is ~0.8, by which we can say that using logarithmic value of gdp, the linear model that has been built can explain relation between all these variables. We can observe from the model that p values of log(gdp) and time are significant.


![4](/44.JPG)
From the above code snippet we can understand that rmse values obtained for train and test datasets are 7.46 and 7.5 respectively, which is an acceptable error value.


![3](/43.JPG)
From the above 3d plot we can see the distribution of actual and predicted values, a good takeaway from this visualization is that there is a good overlap between actual and predicted values.

How does autocorrelation impact our analysis:
Auto correlation is correlation of a signal with a delayed copy of itself as a function of delay, it is similarity of between observations as a function of time lag between them, Underlying assumption of linear regression is that the data has no auto correlation, hence, if auto correlation exists we get inaacurate evaluation metrics like R^2, rmse, coefficients. Hence, if auto correlation exists there is a high probability that values obtaines are totally wrong.

# Problem 5:

![1](/51.JPG)
Here, we would like to quantify the relation between gdp per capita and child mortality. Using the available datasets we build a master dataset that contains both gdp and child mortality, using this dataset we try to understand the relation and quantify it using graphs and modeling techniques. 

From the 1st graph we can say that there is no evident linear relation between gdp per capita and life expectancy, using the gdp and child mortality variables we create a scatter plot, using this we can interpret that linear relation does not exist between the variables, this can be quantified using further analysis. Hence, we could use log transform of gdp per capita to check if this could help us in getting better results.

![1](/52.JPG)
By building a simple linear regression model using log of gdp per capita, child mortality, and time. By further understanding the results of this model we can quantify the relationship. R squared of the model is ~0.63, by which we can say that using logarithmic value of gdp, the linear model that has been built can explain relation between all these variables, but this relation is not strong enough. We can observe from the model that p values of log(gdp) and time are significant.


![1](/53.JPG)
We can observe from the code snippet that RMSE values for train and test datasets are 47.5 and 49 respectively, these values can be further improved


![1](/54.JPG)
From the above 3d plot we can see the distribution of actual and predicted values, a good takeaway from this visualization is that there exits an overlap between actual and predicted values but the overlap is not completely efficient.

How does autocorrelation impact our analysis:
Auto correlation is correlation of a signal with a delayed copy of itself as a function of delay, it is similarity of between observations as a function of time lag between them, Underlying assumption of linear regression is that the data has no auto correlation, hence, if auto correlation exists we get inaacurate evaluation metrics like R^2, rmse, coefficients. Hence, if auto correlation exists there is a high probability that values obtaines are totally wrong.
