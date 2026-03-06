# Outlier Analysis, Research Frontiers Assignment



### Outlier Analysis

There are three main types of outliers that we covered in this course, which are global, contextual, and collective outlier.

##### ➣ Global Outlier
Starting off with global outlier, which is a single data point that is extremely different from the rest of the data. One way to detect this type of outlier is by using distance based methods like k-nearest neighbors aka kNN.For example, in banks statement, if someone typically does purchases to $400 maximum usually and then suddenly there is a $50000 purchase, that would  be considered a global outlier, since the transaction is very different from the usual spending. Here we would mesaurse the distance between normal spending and that global outlier because it will appear far away from the normal data points.

##### ➣ Contextual Outlier
Next we will look into contextual outlier, which is when a value is only abnormal in a certain context. This type of outlier can be detected using time series analysis or other context-based methods that compare a value with similar time periods or environmental conditions. One specific way to do this is to separate the data into context attributes and behavior attributes. Then the behavior of a data point is compared only with other points that share the same context. If the behavior is very different from the others in that context, it can be identified as a contextual outlier. For example, a temperature of 5°F is normal during the winters of the midwest, but it would be unusual during August. So for many data the value must be anaylzed within context (time, location, situation) because the meaning could change even if the value itself isn’t abnomarl.

##### ➣ Collective Outlier
Finally we will look at collective outlier, which is when a group of data points together looks unusual, even though each individual point may seem normal on its own in that group. This kind of outlier can be detected using clustering methods or sequence analysis, since these approaches can detect unusual patterns in groups of data. In the course, one specific way to detect this was to first combine the related data points into a super object, which will be treated as one unit, and then detect that super object as a global outlier. We can use another example of weather, where in mid August of the midwest there is a super rare artic blast that bring the average temperate to 20°F, 30°F, 25°F, 21°F, 30°F, 45°F and 35°F for a week when the average temperatures are usually 85°F. When looking at just one temperature by itself might not seem strange at first, but when the whole sequence of temperatures is considered together, it clearly shows an abnormal pattern and this group of unusual temperatures would be considered a collective outlier.


### Research Frontiers


### Referance:
Symbols: https://coolsymbol.com/

Research: Tian, Z., Zhuo, M., Liu, L., Chen, J., & Zhou, S. (2023). Anomaly detection using spatial and temporal information in multivariate time series. Scientific Reports, 13, 4400. https://doi.org/10.1038/s41598-023-31193-8
https://www.nature.com/articles/s41598-023-31193-8
