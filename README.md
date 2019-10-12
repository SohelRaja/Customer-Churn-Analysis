# Customer-Churn-Analysis

Implementation of Decision Tree Classifier, Esemble Learning, Association Rule Mining and Clustering models(Kmodes & Kprototypes) for Customer attrition analysis of bank to identify the cause and conditions of the churn.

## Project Summary:

### Collecting Data:
We used this telecom service customer churn dataset for this particular project- [WA_Fn-UseC_-Telco-Customer-Churn.csv](https://github.com/arghac14/Customer-Churn-Analysis/blob/master/Decision%20Tree/WA_Fn-UseC_-Telco-Customer-Churn.csv)

### Data preprocessing:
We cleaned the dataset and took dummy datas in the form of categorical datas for our classification purpose.
Here is the new dataset- [new_telco.csv](https://github.com/arghac14/Customer-Churn-Analysis/blob/master/Decision%20Tree/new_telco.csv)

### Initial classification:
First of all, we did an initial classification by Implementing Decision Tree classifier using all the features of our dataset.
We got an **accuracy** of **79.83%** at depth=5 for Decision Tree Entropy technique.
[See the notebook](https://github.com/arghac14/Customer-Churn-Analysis/blob/master/Decision%20Tree/Decision_Tree_Customer_Churn_v3.ipynb)
Here is the graph-

### Implementation of Clustering models:
We implemented Kmodes and Kprototype clustering to get the clusters and centroids for each feature of our dataset. It will be used to find the best features of our dataset.
[See the notebook](https://github.com/arghac14/Customer-Churn-Analysis/tree/master/Clustering)

### Associtaion Rule Mining:
We implemented apriori algorithm(association rule miining) to get the rules of features, depending on which we will find the best features of our dataset.
[See the notebooks](https://github.com/arghac14/Customer-Churn-Analysis/tree/master/Association%20Rule%20Mining)

### Finding the best features:
Comparing the results of Decisiton Tree classifier, Clustering and Association Rule mining, we get the following best features-
**'tenure'**,**'InternetService'**,**'PhoneService'**.

### Implementing other classifiers:
We implemented other classifiers like K-nearest Neighbors, Logistic Regression, Support Vector Machine, Random Forest and Naive Bayes Classifiers taking all the feauters and then taking the best features of the dataset. Then we compared the accuracy of the different models.
[See the notebooks](https://github.com/arghac14/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers)

### Implementing Voting Classifier (Ensemble Leaning):
We implemeted Voting Classifier that combines several classifier models in order to produce one optimal predictive model and improves the model performance.
[See the notebook](https://github.com/arghac14/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Voting%20Classifier)

## Final Result:
