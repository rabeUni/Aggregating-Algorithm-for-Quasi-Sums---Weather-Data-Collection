# Aggregating-Algorithm for Quasi-Sums -- Weather Data Collection
This repository contains the code which has been used to create the experimental plots in the publication "An Axiomatical Approach to Loss Aggregation in Online Learning and an Adapted Aggregating Algorithm".

We run a tabular classification task on weather data collection. The data is curated and provided by the DWD (German Weather Agency). The data collections are publicly available at [DWD](https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/daily/kl/historical/}).
The jupyter notebook first cleans the data collection to be able to train 9 simple (probabilistic) classification models on the first 80% (in temporal order) of the data collection:  logistic regression (LR), gaussian naive bayes (NB), support vector machine (SVC), linear model with stochastic gradient descent (SGD), decision tree (DT), k-nearest neighbors (KNN), random foreast (RF), bagging on decision trees (BAGGING), gradient boosting on decision trees (GB).

Then we apply the predictors on the remaining 20%. We aggregate the prediction via aggregating algorithm using different aggregations but holding fix the log-loss. Finally, we plot the loss profiles for different aggregations.


Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
