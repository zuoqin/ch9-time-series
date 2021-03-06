# Time series

Example code for chapter nine, [Clojure for Data Science](https://www.packtpub.com/big-data-and-business-intelligence/clojure-data-science).

## Data

This chapter makes use of two datasets: the [Longley](http://www.itl.nist.gov/div898/strd/lls/data/LINKS/i-Longley.shtml) dataset and the Airline dataset from Box & Jenkins (1976).

Both datasets are included with the Incanter library.

### Fitting curves with a linear model

1. Add the year squared as a parameter, in addition to the year
2. The curve fits the data quite well, with an R2 of over 0.97. However, it should come as no surprise to you now to discover that we are overfitting the data. The model we have built is unlikely to have very much forecasting power. In fact, if we extend the range of the chart to the right, as we do with ex-9-8 to show predictions into the future, we obtain that just two-and-a-half years after the last measured data point, our model is predicting that the military will grow more than 500 percent

### Time series decomposition

1. Trend
2. Seasonality
3. Cycles

### De-trending and differencing

### Discrete time models

### Autoregressive models

### Determining autocorrelation in AR models

### Moving-average models

### Combining the AR and MA models

### Calculating partial autocorrelation

The partial autocorrelation function (PACF) aims to address the issue of spotting cyclic components in a hybrid ARMA model. It's defined as the correlation coefficient between yt and yt+k given all the in-between observations. In other words, it's the autocorrelation at lag k that isn't already accounted for by lags 1 through k-1.

### Autocovariance

### PACF with Durbin-Levinson recursion


### Removing seasonality with differencing

### Maximum likelihood estimation

### Estimating the maximum likelihood

The number of parameters to our ARMA model is large, and so to determine the maximum likelihood we're going to use an optimization method that performs well in high-dimensional spaces. The method is called the Nelder-Mead, or simplex,
method.

### Nelder-Mead optimization with [Apache Commons Math](http://commons.apache.org/proper/commons-math/userguide/optimization.html) Apache Commons Math

### Identifying better models with Akaike Information Criterion

### Time series forecasting

### Forecasting with Monte Carlo simulation

The Monte Carlo method was developed and used systematically during the Manhattan Project, the American World War II effort to
develop nuclear weapons. John Von Neumann and Stanislaw Ulam suggested it as a means to investigate properties of neutron travel through radiation shielding and named the method after the Monte Carlo Casino in Monaco.