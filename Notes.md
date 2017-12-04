Notes for Classical Assumptions

**Assumption 1: Model is linear and the error terms is additive**

This simply states that OLS properties apply when regression coefficients are linear. The variables and data do not need to be linear  - e.g the half life of elements can follow an exponential distribution, however we can convert the polynomial or exponential variables to linear. 

**Assumption II: Error term has a zero population Mean**

The error term is random or stochastic in nature. This is because the error term captures the unexplained variation (not explained by our variables) and as per the Central Limit Theorem the distribution of the sum of a large number of random variables will tend towards a normal distribution. 
This assumption can be tested by plotting the model residuals (errors) vs. the predicted values and making sure we see a random distrbution of data points around a zero mean. 
Avoid by:
Plot Residiuals

**Assumption III: independent variables are uncorrelated with the error term**

This is mostly due to omitted variables and states that our variables must not be correlated with the error term as equation would attribute to our variable X, some variation in Y that actually came from the error term. 

**Assumption IV: Error terms are uncorrelated with each other (Autocorrelation)**

For example if the error from one observation is positive and this fact increases the probability that the error from our next observation is also positive. This is most common in time series model.

Sometimes the error term trends and does not follow a normal distribution (e.g financial data) and a lagged variable needs to be added. 

Avoid by: 
plotting residuals. 
Durbon-Watson test

Fix by: https://stackoverflow.com/questions/39840890/how-to-use-lagged-time-sereis-variables-in-a-python-pandas-regression-model

**Assumption V: Error term has constant variance (Heteroskacdicity)**

This assumption is violated when different variances for the error terms exist. This mostly occurs in cross-sectional data (data over multiple subjects) and where there is a wide spread between the largest and smallest observed for for the dependent variable. 


Test:

Breush-pagan test
White test

**Assumption VI: Independent variables are (mostly) independent of each other (Multicollinearity)**

Test - correlation matrix, VIF
then drop variables with most collinearity













