# Twitter-Buzz-Prediction

This data-set contains examples of buzz events from Twitter.

CLASSIFICATION TASK
In the classification task you will be provided with time-windows showing an upward trend. The objective of this task is to determine whether or not these time-windows are followed by buzz events. 
In this task:
Each example matches an upward window. Such an example is a multivariate time-series ranging from t to t+β.
 The labeling (ie. buzz; non-buzz) of an example, as well as the upward detection, are performed considering an univariate time-series. This time series (Y, the target feature, presented bellow) is meant to reflect the popularity of a topic.
 There is two ways to label examples: Absolute labeling and Relative labeling. The first one labels as buzz any example which is “sufficiently” popular between t+β+1 to t+β+δ while the second one is based on the increment of popularity level before and after β
 For both of these labeling methods, the threshold value σ varies in order to qualify buzz of distinct magnitude. Concretely σ = 500 implies that an example is labeled as a buzz if:
(Absolute labeling) the sum of Y’s values ranging from t+β+1 to t+β+δ is greater than 500
(Relative labeling) the difference between (a) the Y’s mean value between t+β+1 and t+β+δ and (b) the Y’s mean value between between t to t+β is greater than 500


REGRESSION TASK
As in the classification task you will be provided only with upward-windows. The value to be predicted will be the value of the time-series used to determine the popularity of a topic (Y, as presented before)



