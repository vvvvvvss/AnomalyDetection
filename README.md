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

## Isolation Forest algorithm
Another popular algorithm for anomaly detection is the Isolation Forest algorithm
This algorithm uses decision trees to identify anomalies, by isolating points that are difficult to reach in the decision tree. 
The basic idea is that, in most datasets, the majority of points can be reached in the decision tree with only a few splits. 
Anomalies, on the other hand, are typically isolated from the rest of the data, requiring many splits to reach them in the decision tree. 
The Isolation Forest algorithm uses this property to identify anomalies by isolating points that are difficult to reach in the decision tree.

## Support Vector Machines (SVMs)
One-class Support Vector Machines (SVMs) are another popular approach to anomaly detection. This algorithm uses support vector machines to learn a decision boundary that separates the majority of the data from the anomalies. 
The basic idea is that, in most datasets, the majority of points belong to a single cluster, while anomalies form a separate cluster. 
The One-class SVM algorithm uses this property to learn a decision boundary that separates the majority of the data from the anomalies, and uses this boundary to identify points that are likely to be anomalies.

## Elliptic Envelope algorithm 
Elliptic Envelope algorithm is another approach to anomaly detection that assumes that the data is normally distributed. 
This algorithm fits an ellipse around the data, and identifies points that fall outside of the ellipse as anomalies. 
The basic idea is that, in a normally distributed dataset, most of the points will fall within the ellipse, while anomalies will fall outside of it. 
The Elliptic Envelope algorithm uses this property to identify anomalies by fitting an ellipse around the data and identifying points that fall outside of it.
