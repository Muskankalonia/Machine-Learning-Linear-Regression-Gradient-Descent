# Machine-Learning-Linear-Regression-Gradient-Descent

#Machine Learning Course Coursera By Andrew NG

It contains the vectorized implementaion of the linear regression and gradient descent with single as well as multi variable . It also includes solution through Normal Equation method.


#Regression 
A regression problem is the one which has it output values over an interval.
Like : We have an inventory of 1000's of item and want to predict how many of these items will sell over the next 3 months .


#Cost Function: 
It helps us to figure out the best possible fit to our data .
represented by J(theta(0),theta(1)...).
  h(x) = theta(0) + theta(1) + theta(2).... where theta(i) are parameters 
The idea is to choose theta(i) (where i = 1,2,3,...n) so that h(x) is close to y (which is the output of the training example).
  thus , (h(x)-y)^2 must be less
(Implementation of cost function is seprately written in the code)

#Gardient Descent
It is an algorithm to slowly minimise the cost function and reach the best possible hypothesis h(x) to fit the data 


#Normal Equation 
In contrast to gradient descent normal equation gives us a simple analytical method to get the output in one go it is best suited for datasets with less rows and columns 
  theta = pinv(X'*X)*(X'*y)
(pinv is pseudoinverse of the matrix )


##So how to navigate through code file??
- Data1.txt file contains the dataset for linear regression with one variable. The first column is the population of a city and the second column is the profit of a food truck in that city. A negative value for profit indicates a loss. 

- plotData.m includes plotting the data in matlab on scatter plot

- gradientDescent.m includes vectorly implemented gradient descent on the dataset

- computeCost.m includes computing the cost function

- data2.txt contains training set of housing price . The first column is the size of the house (in square feet), the second column is the number of bedrooms, and the third column is the price of the house.

- featureNormalise.m includes implementation of feature normalisation so as to produce better results

- gradientDescentMulti.m and computeCostMulti.m for implementing gradient descent for multiVariate regression problem
