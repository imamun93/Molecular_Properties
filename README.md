# Predicting Molecular Properties

Data from Kaggle competition [Predicting Molecular Properties](https://www.kaggle.com/c/champs-scalar-coupling?utm_medium=email&utm_source=intercom&utm_campaign=champs-email-launch). All data can be found there. Due to git size limitation, all data were ignored from this repo.


Finished basic EDA and found out which features are important at the [SNS and LGB file](https://github.com/imamun93/Molecular_Properties/blob/master/SNS%20and%20LGB%20EDA.ipynb). Thorugh EDA and lgbm modelling, I leanred that fc, pso, sd and dso play a more important weighted role in predicting the Scalar Constant.

Finished working on creating a simple Linear Regression and then a more complex linear regression at the [Linear Regression Notebook](https://github.com/imamun93/Molecular_Properties/blob/master/LinearRegression.ipynb). This result failed. I do not see the point with moving forward with OLS type model.

I also did quick work on a Ridge as well as Lasso model. They are at the [Ridge Lasso Notebook](https://github.com/imamun93/Molecular_Properties/blob/master/RidgeLasso.ipynb). Although it showed promising results at first, the end result was still disappointing.

Since I never worked with a Random Forest Linear Regression, I decided to try it out. That notebook is [Random Forest](https://github.com/imamun93/Molecular_Properties/blob/master/RandomForest.ipynb). It gave me a 99% accuracy using CV. But this was rather on a smaller scale.


However, that gave me a great idea. I realized that since my data were all over the place, I decided to take a bigger sample size and normalized the data. Then ran different variations of Linear, Ridge and Lasso. That notebook is [Normalized Regression](https://github.com/imamun93/Molecular_Properties/blob/master/NormalizedRegression.ipynb). This time I used a larger data set. This did give me the desire results. Both ridge and lasso showed a 99% accuracy. Even a smaller randomforest regression tree gave me 99% accuracy. However, when I attempted it with a higher tuned parameter, my computer crashed after 48 hours.



The [Neural Network file](https://github.com/imamun93/Molecular_Properties/blob/master/SimpleNeuralNetwork.ipynb) is currently stopped and will resume after I have established a baseline model that works accurately.
