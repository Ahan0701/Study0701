# Computer Science

### Linear Regression
Linear Regression is a linear equation used for predicting a value of something when there are multiple data sets with a different rate of change. Regression analysis stems from the idea that given data have a certain tendency. The main purpose of regression analysis is to explain the tendency among variables. When expressed mathematically, the regression model is divided into a part that shows a trend and a part that shows an uncontrollable error. The equation has the form Y= a + bX, where Y is the dependent variable, X is the independent variable, b is the slope of the line, and a is the y-intercept.
[logo]: https://miro.medium.com/max/1400/1*Cw5ZSYDkIFpmhBwr-hN84A.png "Linear Regression"

### Derivative
A derivative represents the slope of the tangent line at a specific point on the curve. In the case of a straight line, the slope does not change even if x changes because it continues to extend in the same direction. But, because the slope changes depending on what the value of x is on a curved line, we differentiate to find the value of the slope that changes according to the value of x. The equation obtained by differentiating the cubic function is the equation for the slope. You just need to find two x-values where the value at that time is 0 and draw a graph around that value. This point is specifically called the inflection point, and the y-value at this point is called the extreme point. Extreme points are places where a function takes on an extreme value, a value that is especially small or especially large compared to other nearby values of the function. When the slope is a negative number, the graph is convex up. In this case, the top tip of this convex is the extreme point. When the slope is a positive number, it is convex down. In this case, the bottom tip of this convex is the extreme point. 
[logo]: https://www.mathfactory.net/wp-content/uploads/%EC%88%98%ED%95%99-%EA%B3%B5%EC%8B%9D-%ED%8F%89%EA%B7%A0%EB%B3%80%ED%99%94%EC%9C%A8-%EB%AF%B8%EB%B6%84%EA%B3%84%EC%88%98-02.png "Linear Regression"

### a b
y^i=axi+b
∑ei^2=∑(yi-axi-b)^2

partial derivative for b: 
∂∑ei^2/∂b=2∑(-1)(yi-axa-b)

When this equation is 0: 
0=∑yi-a∑xi-nb

nb=∑yi-a∑xi

b=∑yi-a∑xi/n

When average if yi=￣y:

b=￣y-a(￣x)
	
Partial derivative for ∑R:

y∑∂i^2/∂i= (-1)2∑(yi-axi-b)(xi)
	
0=-2{∑yi-xi-a∑(xi^2)-b∑xi}

a∑(xi^2)=∑(yi)xi-b∑xi	

a{∑(xi^2)-￣∑xi}=∑yi(xi)-￣yxi

a=∑ti(xi)-￣y∑xi/∑(xi^2)-￣x∑xi


### MSE and RMSE
MSE=1/n∑(y-y^)^2

RMSE=√mse=√∑(y^-y)^2/n

MSE represents the difference between the original and predicted values extracted by squaring the mean difference over a data set. MSE is the measure of how close the fitted line is to the actual data points. The closer the fit is to the data set if the smaller the mean squared error. MSE has units squared on the vertical axis. RMSE is the error rate by the square root of MSE. RMSE is the easiest statistic to interpret because it has the same units as the values shown on the vertical or y-axis. It is a better measure of goodness of fit than correlation coefficient because RMSE can be interpreted directly as a unit of measure. 

### R^2
R^2=1-RSS/TSS

R^2 is the coefficient of determination. Let's look at the coefficient of determination (R^2). This is what is commonly called R squared.  R^2 is a measure of how well the estimated linear model fits the given data. The proportion of the variance of the response variable (y) can be explained by the fitted model. The coefficient of determination is an indicator of how much the independent variable explains the dependent variable in a regression model. Also called explanatory power. 

A higher coefficient of determination means that the independent variable explains more of the dependent variable and this coefficient increases as the number of independent variables increases. In fact, it is somewhat problematic to judge the usefulness of a regression model with only the coefficient of determination because it increases even if a variable that does not explain the dependent variable well is added. 

## Skyline Implementation

### Code
