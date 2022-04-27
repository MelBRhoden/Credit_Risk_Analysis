# Credit_Risk_Analysis
Supervised Machine Learning and Credit Risk

# Overview of the loan prediction risk analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques were used to train and evaluate models with unbalanced classes. Various libraries and algorithms were used to build and evaluate models using resampling including:

* imbalanced-learn
* scikit-learn
* RandomOverSampler
* SMOTE algorithms
* ClusterCentroids algorithm
* SMOTEENN algorithm
* BalancedRandomForestClassifier (bias reduction model)
* EasyEnsembleClassifier (bias reduction model)

# Purpose:
* Explain how a machine learning algorithm is used in data analytics.
* Create training and test groups from a given data set.
* Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
* Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
* Compare the advantages and disadvantages of each supervised learning algorithm.
* Determine which supervised learning algorithm is best used for a given data set or scenario.
* Use ensemble and resampling techniques to improve model performance.

# Results:
The results for the six machine learning models including their respective balanced accuracy, precision, and recall scores are as follows:

<b>Naive Random Oversampling</b> </br>
![image](https://user-images.githubusercontent.com/95143562/165646441-db644e8c-6c9d-4fc1-aba8-e2971c0357ff.png)
* Balanced Accuracy: 0.6612700484668286
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low risk = .66/.67

<b>SMOTE Oversampling</b></br>
![image](https://user-images.githubusercontent.com/95143562/165646520-316406cd-0888-4711-8697-c005b8a7c6d4.png)
* Balanced Accuracy: 0.6303296388959394
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low risk = .62/.64

<b>Undersampling</b></br>
![image](https://user-images.githubusercontent.com/95143562/165646596-8366d3f9-ea48-4851-9537-7667ee5e0143.png)
* Balanced Accuracy: 0.6303296388959394
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low risk = .63/.40

<b>Combination Under-Over Sampling</b></br>
![image](https://user-images.githubusercontent.com/95143562/165646695-c3730f82-c00d-47b1-bcbd-0505b7d83dc2.png)
* Balanced Accuracy: 0.5173713090878325
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low risk = .70/.57

<b>Balanced Random Forest Classifier</b></br>
![image](https://user-images.githubusercontent.com/95143562/165646755-2c867721-bdd0-43ff-89c8-5d4b1dda1c8d.png)
* Balanced Accuracy: 0.7877672625306695
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low risk = .67/.91

<b>Easy Ensemble AdaBoost Classifier</b></br>
![image](https://user-images.githubusercontent.com/95143562/165646840-aad14a35-60be-4150-a7e0-1a96b6934e17.png)
* Balanced Accuracy: 0.925427358175101
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low risk = .91/.94

# Summary:
When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model. For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy. The other models were below .80 balanced accuracy. The precision for all models were similar and within an appropriate range. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the final best machine learning model to choose for further credit card analysis.
