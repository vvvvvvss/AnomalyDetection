# Anomaly Detection

Anomaly detection simply means outlier detection. It is necessary to remove the outliers for better accuracy of a model. 
Anomaly is a deviation from the expected or normal behavior or pattern.
Anomaly Detection is the technique of identifying rare events or observations which can raise suspicions by being statistically different from the rest of the observations.

An anomaly can be broadly categorized into three categories –   

Point Anomaly: A tuple in a dataset is said to be a Point Anomaly if it is far off from the rest of the data.     
Contextual Anomaly: An observation is a Contextual Anomaly if it is an anomaly because of the context of the observation.   
Collective Anomaly: A set of data instances help in finding an anomaly.  


Anomaly detection can be done using the concepts of Machine Learning. It can be done in the following ways –  
 

### Supervised Anomaly Detection: 
This method requires a labeled dataset containing both normal and anomalous samples to construct a predictive model to classify future data points. 
The most commonly used algorithms for this purpose are **supervised Neural Networks, Support Vector Machine learning, K-Nearest Neighbors Classifier**, etc. 
### Unsupervised Anomaly Detection: 
This method does require any training data and instead assumes two things about the data, i.e., only a small percentage of data is anomalous and any anomaly is statistically different from the normal samples. 
Based on the above assumptions, the data is then clustered using a similarity measure and the data points which are far off from the cluster are considered to be anomalies.

## Local Outlier Factor (LOF) algorithm
One of the most widely used algorithms for anomaly detection is the Local Outlier Factor (LOF) algorithm. 
This algorithm uses the local density of points in a dataset to identify anomalies. 
The basic idea is that, in most datasets, the density of points is relatively uniform, with only a few points having significantly lower or higher densities than the rest. 
The LOF algorithm uses this property to identify points that have a significantly lower density than their neighbors, which are likely to be anomalies.
