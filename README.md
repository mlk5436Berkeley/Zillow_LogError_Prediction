# Zillow LogError Prediction
The Zestimate was created to give consumers as much information as possible about homes and the housing market, marking the first time consumers had access to this type of home value information at no cost.

“Zestimates” are estimated home values based on 7.5 million statistical and machine learning models that analyze hundreds of data points on each property. And, by continually improving the median margin of error (from 14% at the onset to 5% today), Zillow has since become established as one of the largest, most trusted marketplaces for real estate information in the U.S. and a leading example of impactful machine learning.

The goal of this project is to build a machine learning model that improve the accuracy of the Zestimate even further by prediction the log-error between their Zestimate and the actual sale price, given all the features of a home.

### Logerror

logerror = log(Zestimate/SalePrice)

For the logerror to be negative, we need Zestimate to be less than Sale Price, resulting in a ratio less than 1. 
This means the Zestimate is underestimating the actual Sale Price. 

If Zestimate is significantly smaller than Sale Price, the logerror will have a larger negative value. 
On the other hand, if Zestimate is close to actual Sale Price., the logerror will approach zero.

### Data
The data contain the full list of real estate properties in three counties (Los Angeles, Orange and Ventura, California) data in 2016.
The train data has all the transactions before October 15, 2016, plus some of the transactions after October 15, 2016. 
The data can be downloaded at https://www.kaggle.com/competitions/zillow-prize-1/data
