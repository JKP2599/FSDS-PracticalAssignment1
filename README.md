# Housing Price Prediction - Linear Regression

This ML web app uses a linear regression model trained on the Boston Housing Prices dataset to predict the price of a house based on user input values. The model takes into account several variables including number of rooms, crime rate, per capita income by town, and more.

The linear regression model was implemented using the scikit-learn library, and to achieve better generalization, we also used regularization techniques such as Lasso, Ridge, and ElasticNet. These regularization techniques help to prevent overfitting of the model and improve its ability to generalize to new data.

With this app, users can input the values for the various variables of a hypothetical house, and the model will predict the expected price based on its training data.

### Check Out the App
[Boston Housing Price Prediction](https://boston-housing-price-prediction.onrender.com)

### Dataset Description

The Boston house-price data of Harrison, D. and Rubinfeld, D.L. 'Hedonic prices and the demand for clean air', J. Environ. Economics & Management, vol.5, 81-102, 1978. Used in Belsley, Kuh & Welsch, 'Regression diagnostics ...', Wiley, 1980. N.B. Various transformations are used in the table on pages 244-261 of the latter.

 Variables in order:
 - CRIM     per capita crime rate by town
 - ZN       proportion of residential land zoned for lots over 25,000 sq.ft.
 - INDUS    proportion of non-retail business acres per town
 - CHAS     Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
 - NOX      nitric oxides concentration (parts per 10 million)
 - RM       average number of rooms per dwelling
 - AGE      proportion of owner-occupied units built prior to 1940
 - DIS      weighted distances to five Boston employment centres
 - RAD      index of accessibility to radial highways
 - TAX      full-value property-tax rate per $10,000
 - PTRATIO  pupil-teacher ratio by town
 - B        1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
 - LSTAT    % lower status of the population
 - MEDV     Median value of owner-occupied homes in $1000's

Due to the future deprecation warning for the boston dataset, the data is loaded from a local csv instead of the scikitlearn library

### Input Variables required for the prediction
'CRIM', 'ZN', 'CHAS', 'NOX', 'RM', 'DIS', 'RAD', 'TAX', 'PT', 'B', 'LSTAT'

**MEDV** is the target variable

Stastistical Analysis of the dataset reveals that INDUS and AGE contribute little to the target variable.
Hence these are not considered for the prediction.
