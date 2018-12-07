# Project 2 - Projecting Country by Country Suicide Statistics Using Linear Regression

The goal of this project was to build a regression model to predict the combined male and female suicide rate for any country.
We gathered data on the 2016 world suicide statistics using the World Health Organization API. After doing some research into the previous work done on the subject, we collected data on the following independent variables which we believed would help to build our model.
Those variables are:
1. Depression rate
2. Anxiety rate
3. Bipolar Disorder
4. Eating Disorder
5. Alcohol Use Disorder
6. Drug Use Disorder
7. GDP
8. Health Spending per Capita
9. Unemployment Rate
9. Percentage of Population Living in Cities with > 100k People
10. Percentage of Population with Internet Access
11. Categorical data concerning level of Religous Observance
12. Schizophrenia rate

After gathering and cleaning all the data, we scaled the independent variables. We then compared each of the variables collinearity through a SeaBorn Correlation Heatmap and by plotting pair plots of each independent variable's correlation to our target. We began building our Linear Regression by adding on polynomial features to our data. We then used a combination of Recursive Feature Elimination and Cross Validation to pick the model with the optimal feature selection. 

After selecting the features we wanted to use, we split our data into training and testing data (20% was for testing). We fit our regression using the training data and checked its accuracy on the test data. 
The following graphs demonstrate the accuracy of our model:
![](https://github.com/Botafogo1894/Project2/blob/master/screenshots/Screen%20Shot%202018-12-07%20at%201.24.48%20PM.png)

The following bar chart demonstrates the weight of the selected features:

![](https://github.com/Botafogo1894/Project2/blob/master/screenshots/download.png)
