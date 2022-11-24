# Facebool Prophet
## [Project Summary](https://nbviewer.org/github/davidefilosa/Facebook-Prophet/blob/master/Facebook%20Prophet.ipynb)


## Predicting Homeless Shelter Entry

In this project we will try to predict the number of people who will need shelter.

Intuitively we can imagine that the number of people who need a refuge depends on the weather, therefore on the season, on the holidays: so it seems like a perfect problem to solve with Facebook Prophet.

Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.

The framework that typically applies to time series analysis is the structural time series which simply means decomposing the time series into trend, seasonality, and exogenus events.

Facebook Prophet follows a similar approach. 

The formula is: $$y(t) = c(t) + s(t) + h(t) + x(t) + ε$$ 

How to read this formula:

- c(t) is the trend component 
- s(t) is the sesosonality 

then we have the exogenus events that are split into two:

- h(t) is the Holiday Effects
- x(t) is the external regressors that can be any other event

finally we have

- ε is the error term, everithing that can not be explained by the model
