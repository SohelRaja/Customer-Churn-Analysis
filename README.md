
# Customer-Churn-Analysis

Implementation of Decision Tree Classifier, Esemble Learning, Association Rule Mining and Clustering models(Kmodes & Kprototypes) for Customer attrition analysis of telecommunication company to identify the cause and conditions of the churn.

### Contributers: [Arghadip Chakraborty](https://github.com/arghac14), [Sohel Raja Molla](https://github.com/SohelRaja), [Disha Sinha](https://github.com/disha2sinha), [Shankhadeep Giri](https://github.com/shankha2018). 

## Project Summary:
Finding the best features of the dataset by comparing the rules obtained from Decision Tree Classifier, Clustering Models(Kmodes and Kprototypes) and Assocication Rule Mining(Apriori algorithm) and then implementing Voting Classifiers(Ensemble Learning) with other classifier models, taking the best features with other classifier models to see if there is a boost in accuracy of prediction or not.

## Workflow:
![](https://github.com/SohelRaja/Customer-Churn-Analysis/blob/master/Snapshots/workflow.jpg)

### Collecting Data:
We used this telecom service customer churn dataset for this particular project- [WA_Fn-UseC_-Telco-Customer-Churn.csv](https://github.com/arghac14/Customer-Churn-Analysis/blob/master/Decision%20Tree/WA_Fn-UseC_-Telco-Customer-Churn.csv)

### Data preprocessing:
We cleaned the dataset and took dummy datas in the form of categorical datas for our classification purpose.
Here is the new dataset- [new_telco.csv](https://github.com/SohelRaja/Customer-Churn-Analysis/blob/master/Decision%20Tree/new_telco.csv)

### Initial classification using Decison Tree Classifier:
First of all, we did an initial classification by Implementing Decision Tree classifier using all the features of our dataset.
We got an **accuracy** of **79.83%** at depth=5 for Decision Tree Entropy technique.
[See the notebook](https://github.com/SohelRaja/Customer-Churn-Analysis/blob/master/Decision%20Tree/Decision_Tree_Customer_Churn_v3.ipynb)
![](https://github.com/SohelRaja/Customer-Churn-Analysis/blob/master/Snapshots/ID3graph.JPG)

### Implementation of Clustering models:
We implemented Kmodes and Kprototype clustering to get the clusters and centroids for each feature of our dataset. It will be used to find the best features of our dataset.
[See the notebook](https://github.com/arghac14/Customer-Churn-Analysis/tree/master/Clustering)

### Associtaion Rule Mining:
We implemented apriori algorithm(association rule miining) to get the rules of features, depending on which we will find the best features of our dataset.
[See the notebooks](https://github.com/arghac14/Customer-Churn-Analysis/tree/master/Association%20Rule%20Mining)

##### Most important frqeuent items when Churn=0:
![](https://github.com/arghac14/Customer-Churn-Analysis/blob/master/Snapshots/apriori1.JPG)

##### Most important frqeuent items when Churn=1:
![](https://github.com/arghac14/Customer-Churn-Analysis/blob/master/Snapshots/apriori2.JPG)

### Finding the best features:
Comparing the results of Decisiton Tree classifier, Clustering and Association Rule mining, we get the following best features-
**'tenure'**,**'InternetService'**,**'PhoneService'**.

### Implementing other classifiers:
We implemented other classifiers like K-nearest Neighbors, Logistic Regression, Support Vector Machine, Random Forest and Naive Bayes Classifiers taking all the feauters and then taking the best features of the dataset. Then we compared the accuracy of the different models.
[See the notebooks](https://github.com/SohelRaja/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers)
* [Decision Tree](https://github.com/SohelRaja/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers/Decision%20Tree)
* [KNN](https://github.com/disha2sinha/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers/KNN)
* [Logistic Regression](https://github.com/shankha2018/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers/Logistic%20Regression)
* [Naive Bayes](https://github.com/shankha2018/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers/Naive%20Bayes)
* [Random Forest](https://github.com/SohelRaja/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers/Random%20Forest)
* [SVM](https://github.com/disha2sinha/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Other%20Classifiers/SVC)
#### Accuracy report-
With all features:

![](https://github.com/disha2sinha/Customer-Churn-Analysis/blob/master/Snapshots/otherClassifiers1.png)

With best features:

![](https://github.com/SohelRaja/Customer-Churn-Analysis/blob/master/Snapshots/other%20classifiers.JPG)

### Implementing Voting Classifier (Ensemble Leaning):
We implemeted Voting Classifier that combines several classifier models in order to produce one optimal predictive model and improves the model performance.
[See the notebook](https://github.com/arghac14/Customer-Churn-Analysis/tree/master/Ensemble%20Learning/Voting%20Classifier)

## Final Result:
![](https://github.com/SohelRaja/Customer-Churn-Analysis/blob/master/Snapshots/voting.JPG)

![](https://github.com/SohelRaja/Customer-Churn-Analysis/blob/master/Snapshots/accc.JPG)


   


