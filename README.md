## 1 Gradient Descent with Python and NumPy

From a Jupyter notebook in Python, extract two time series of your choice from the CryptoCompare API, calling one xt and the other yt.

You do not have to use the CryptoCompare API (for example you can use the Nasdaq Data Link API). Depending on availability, choose your own frequency and time period, making sure that you can analyse both time series by treating
them each as a one dimensional array of the same length, and make sure they are reasonably long (more than 100 observations). Use the numpy library to Önd OLS estimates of  and  and in the following speciÖcation, where et is an assumed white noise error:

yt = α+β+ xt + et

·Analytically from standard OLS formulae

·By trial and error Machine Learning with a Gradient Descent (GD) Algorithm

One challenge you may encounter is obtaining convergence, depending on the underlying data. In words, describe why convergence to a Loss Function minimum may be di¢ cult to obtain in practice, and how this might be overcome.

## 2 Time Series Forecasting with Regularisation

Create a Python notebook that produces a time series forecast of a Önancial
time series of your choice. Pick one single Önancial time series that you are
interested in (eg the Bitcoin price in Sterling), and conduct your analysis in
stages:
1. In the Örst stage, you must describe why you have chosen the series, and
what factors you think a§ect it. Where relevant, describe any general
trends, speciÖc events, and what variables you think may drive it. Distinguish between variables that you should be able to obtain, versus those
you cannot.
2. Extract the relevant time series (you could use the cryptocompare API
calls already used, or any other).
3. Conduct analysis. You must reduce a larger model with many variables
(more than 10) down to a smaller model by applying L1/L2 Regularisation.
Scikit learn has examples of implementing the combination of L1 and
L2 called elastic nets. Pay attention to stationarity, and use the Scikit
learn implementation that uses cross validation (CV) to pin down the
hyper parameters (weights on L1 and L2). Also, for the purposes of CV
it is important to split time series appropriately by using Scikit learnís
TimeSeriesSplit procedure.
