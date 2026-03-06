# Outlier Analysis, Research Frontiers Assignment



### Outlier Analysis

There are three main types of outliers that we covered in this course, which are global, contextual, and collective outlier.

##### ➣ Global Outlier
Starting off with global outlier, which is a single data point that is extremely different from the rest of the data. One way to detect this type of outlier is by using distance based methods like k-nearest neighbors aka kNN.For example, in banks statement, if someone typically does purchases to $400 maximum usually and then suddenly there is a $50000 purchase, that would  be considered a global outlier, since the transaction is very different from the usual spending. Here we would measure the distance between normal spending and that global outlier because it will appear far away from the normal data points.

##### ➣ Contextual Outlier
Next we will look into contextual outlier, which is when a value is only abnormal in a certain context. This type of outlier can be detected using time series analysis or other context-based methods that compare a value with similar time periods or environmental conditions. One specific way to do this is to separate the data into context attributes and behavior attributes. Then the behavior of a data point is compared only with other points that share the same context. If the behavior is very different from the others in that context, it can be identified as a contextual outlier. For example, a temperature of 5°F is normal during the winters of the Midwest, but it would be unusual during August. So for many data the value must be analyzed within context (time, location, situation) because the meaning could change even if the value itself isn’t abnormal.

##### ➣ Collective Outlier
Finally we will look at collective outlier, which is when a group of data points together looks unusual, even though each individual point may seem normal on its own in that group. This kind of outlier can be detected using clustering methods or sequence analysis, since these approaches can detect unusual patterns in groups of data. In the course, one specific way to detect this was to first combine the related data points into a super object, which will be treated as one unit, and then detect that super object as a global outlier. We can use another example of weather, where in mid August of the Midwest there is a super rare arctic blast that bring the average temperate to 20°F, 30°F, 25°F, 21°F, 30°F, 45°F and 35°F for a week when the average temperatures are usually 85°F. When looking at just one temperature by itself might not seem strange at first, but when the whole sequence of temperatures is considered together, it clearly shows an abnormal pattern and this group of unusual temperatures would be considered a collective outlier.


### Research Frontiers
One issue from the course that I found interesting is spatial temporal anomaly detection, which focused on finding unusual patterns by looking at both location and time together, instead of only one of them. This is a super important concept because in real life when data mining and looking at data patterns because something might seem normal if you only look at the time or only look at the place, but it can look abnormal when both are considered together. For example, a certain temperature might be normal in one area but strange in another, or it might be normal in one season but unusual in a different one. This is really useful in areas like remote sensing, environmental monitoring, and industrial sensor systems, where detecting unusual changes early can help prevent bigger problems. One paper I found interesting on this topic is a paper called Anomaly detection using spatial and temporal information in multivariate time series by Tian published in the Nature journal in 2023, which explains that this is especially important for multivariate time series data from connected sensors, because many older methods do not fully use both the spatial relationships between sensors and the temporal patterns over time. Their model, called STADN, combines a graph attention network to learn spatial relationships and an LSTM to learn temporal patterns, then uses prediction error to detect anomalies. The paper showed that using both kinds of information together can improve anomaly detection compared to methods that only focus on one side.

### Reference:
Symbols: https://coolsymbol.com/

Research: Tian, Z., Zhuo, M., Liu, L., Chen, J., & Zhou, S. (2023). Anomaly detection using spatial and temporal information in multivariate time series. Scientific Reports, 13, 4400. https://doi.org/10.1038/s41598-023-31193-8
https://www.nature.com/articles/s41598-023-31193-8

Spell Check: Spell Right by Bartosz Antosik for vscode
