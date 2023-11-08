# Lin-Reg-YES Bank
**Introduction**
Yes Bank is a banking company founded in 2004 that offers a wide range of financial products for corporate and retail customers. As a publicly traded company, it provides an opportunity for individuals to invest and become shareholders. However, this also means that the company's valuation is influenced by public opinion, making stock prices susceptible to various factors. In this documentation, we focus on utilizing a dataset related to Yes Bank's stock prices to build an efficient machine learning regression model for predicting the closing price. This project aims to understand the dynamics of stock prices and to assess the impact of external events, such as the 2018 fraud case involving Rana Kapoor, on stock price movements.

**Approach**
The approach to analyzing and predicting Yes Bank's stock prices involves several steps:

**Data Loading and Observation:** The dataset contains 185 rows and five features, including Date, Open, High, Low, and Close. The first step is to load the data and explore its contents.

**Data Understanding:** The features in the dataset include:

**Date:** Denotes the date of the investment (in month-year format).
**Open:** The opening price of the stock.
**High:** The highest price within the given time period.
**Low:** The lowest price within the same time period.
**Close:** The closing price of the stock at the end of the considered time period.

**Data Preprocessing:**

**Converting the 'Date' column from the month-year format to the YYYY-MM-DD date format.**
**Handling null values** (though the dataset is already devoid of null values).
**Visualizing data relationships, identifying and addressing outliers, and conducting univariate, multivariate, and bivariate analyses.**

**Feature Engineering:**
**Addressing multicollinearity** among the independent features by creating a new feature that represents the mean of all independent features.
**Train-Test Split: **Dividing the dataset into training and testing sets for model development and evaluation.

**Model Building:** Implementing various regression models, including:

**Linear Regression
Lasso Regression with Grid Search CV
Ridge Regression with Grid Search CV
Elastic Net Regression**

I achieved an accuracy of 97.5% with these models. Further variations, such as log transformation, introducing lags, or using advanced regression models like Random Forest Regressor, XGBoost Regressor, and Support Vector Regressor, offer potential for even higher accuracy but must be monitored for overfitting.

**Conclusion**
In conclusion, I found that the closing stock price of YES Bank is influenced by factors like the opening price, highest price, and lowest price during the trading period. The dataset, although small, offered insights into stock price dynamics and revealed some potential outliers.

These outliers mirror the real-world scenario where stock prices can fluctuate significantly overnight due to various external factors. 

To address multicollinearity among independent features, feature engineering was employed.

Our machine learning models, including Linear Regression, Lasso, Ridge, and Elastic Net, achieved an accuracy of 97.5%. Further exploration, such as log transformation and the use of advanced regression models, could potentially enhance accuracy but need to be monitored for overfitting.

**The impact of the 2018 fraud case involving Rana Kapoor is clearly visible in the dataset**, with a significant decline in stock prices during that period. While our model performs well on this test data, its real-world applicability should be assessed on larger datasets to validate its performance in practical scenarios.

