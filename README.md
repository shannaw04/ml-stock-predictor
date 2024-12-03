# **Stock Price Prediction Model**
COSC 325 Course Project  
Fall 2024
### Members:
  * John Paul Saia  
  * Riley Taylor  
  * Shanna Wallace  

### Objective: 
Create a machine learning model to predict the stock's closing price in 7 days. 

### The Data:
**Data set:** Berkshire Hathaway daily stock price and volume traded from 2015-01-02 to 2024-07-29  
**Format:** .csv file  

#### Target and features:

| Target | Description |
| :- | :- | 
| Close 7 Days | Closing price 7 days from the trading day |

<br>

  | Features | Description |
  | :- | :- | 
  | Date | The day the price data is from (yyyy-mm-dd) |
  | Open | Opening price | 
  | High | Highest price |
  | Low | Lowest price |
  | Close | Closing price |
  | Adj Close | Closing price after adjustments for applicable splits and dividend distributions |
  | Volume | Total number of shares traded that day |

### Feature Selection:
* Calculate correlation coefficients to evaluate correlation between the features, and between the features and the target. 
* Use MDI to compare the importance of the features. 

### The Baseline Model:
* Create baseline linear regression model using 1 feature
* Use Scikit Learn's default OLS linear regressor


### The Ensemble Model:
* Use K-Folds Cross Validation to select optimal max depth.
* Use MDI to evaluate relevant importance of all features.


### Model Evaluation and Comparison:
* Calculate R2, MAE, RMSE for both models and compare performance to select the model that provides the most accurate results. 
