# Aggregating-Algorithm for Quasi-Sums -- Weather Data Collection
This repository contains the code which has been used to create the experimental plots in the publication "An Axiomatical Approach to Loss Aggregation in Online Learning and an Adapted Aggregating Algorithm".

We run a tabular classification task on weather data collection. The data is curated and provided by the DWD (German Weather Agency). The data collections are publicly available at [DWD](https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/daily/kl/historical/}).
The jupyter notebook first cleans the data collection to be able to train 9 simple (probabilistic) classification models on the first 80% (in temporal order) of the data collection:  logistic regression (LR), gaussian naive bayes (NB), support vector machine (SVC), linear model with stochastic gradient descent (SGD), decision tree (DT), k-nearest neighbors (KNN), random foreast (RF), bagging on decision trees (BAGGING), gradient boosting on decision trees (GB).

Then we apply the predictors on the remaining 20%. We aggregate the prediction via aggregating algorithm using different aggregations but holding fix the log-loss. Finally, we plot the loss profiles for different aggregations.
