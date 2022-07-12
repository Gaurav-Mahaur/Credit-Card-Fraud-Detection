# Credit-Card-Fraud-Detection-Machine-Learning-Project

* Project Name : Credit Card Fraud Detection using Machine Learning Algorithms
* Skills : Data Visualisation , Exploratory Data Analysis , Data Science , Machine Learning Algorithms
* Tools :  Google Colab , Jupyter Notebooks , Python , Numpy , Pandas , Matplotlib , Seaborn , Sklearn

##  Motivation And Objective

When we make any transaction while purchasing any product online — a good amount of people prefer credit cards. The credit limit in credit cards sometimes helps us me making purchases even if we don’t have the amount at that time. but, on the other hand, these features are misused by Cyber attackers. One of the most common way these attackers exploit the system is doing a fraudulent transaction.

To tackle this problem we need a system that can detect anomaly in the transaction if it finds fishy.
Here, comes the need for a system that can track the pattern of all the transactions and if any pattern is
abnormal then the transaction should be aborted.

 So,I used 4 inbuilt machine learning algorithms from sklearn toolkit library to model the data.
1. Logistic Regression
2. Support Vector Machine
3. Random Forest Classifier
4. Decision Tree Classifier


To handle imbalanced nature of data, we took that into consider in the testing set, by using *proper evaluation metrics* like Accuracy and F1-Score and *k-fold cross-validation*.

## The Dataset:

The data was taken from Kaggle site : [Dataset Link](https://www.kaggle.com/mlg-ulb/creditcardfraud)

The Columns do not have physical significance directly visible since as per the source (Kaggle) , the data was compressed using Principle Component Analysis (PCA) 
in order to protect the privacy of the individuals while making a realistic secnario dataset availaible to public 

## Data Preprocessing And Visualisation

**Data Save in the form of dataframe**
![data_take](https://user-images.githubusercontent.com/93429968/178411050-190de9b9-a879-4606-a0a9-c9a7af461ddc.png)

**Class Imbalance in Dataset:**

![separatin_fraud](https://user-images.githubusercontent.com/93429968/178411586-433d943e-367c-4b08-8841-4d137a7b2a56.png)


This shows that we have way way less data for fraud cases than for non fraud cases , which is expected from the dataset .

To cure imbalance , we can use undersampling or oversampling . Here , I have decided to use SMOTE to counter the class imbalance in the dataset .

**Correlation:**

![correlation](https://user-images.githubusercontent.com/93429968/178411829-1559d4bc-d274-4d2f-8cb2-0e39e3421b84.png)

The columns do not seem to have correlations with each other , and seem to have great correlation with the Class and time variables , hence being a great indicator that simple models would be helpful here , and neural networks wont be needed hopefully .

## Training of Models And Results:

I have trained model for different algorithms and check cross validation score of the model. 

**Logistics Regression**

![training](https://user-images.githubusercontent.com/93429968/178412318-5a128977-615e-4a4b-bd0e-1c0a70eb238e.png)
![logistics](https://user-images.githubusercontent.com/93429968/178412456-d24ca490-1703-4ea2-be93-2bf107a6fb16.png)


This is the results of training of model for Logistics Regression.In the similar way i have trained models for rest of the algorithms i used.


### **Support Vector Machine(SVM) Results**

![svm](https://user-images.githubusercontent.com/93429968/178412868-fa16e8ee-6c2a-42a4-8388-1afed033a6d7.png)

### **Random Forest Results**

![random forest](https://user-images.githubusercontent.com/93429968/178412952-a785b6a2-8f9d-48c8-a48e-c019edc151c4.png)

### **Decision Tree Results**

![desiciontree](https://user-images.githubusercontent.com/93429968/178413054-fbb87d51-3ac9-4fff-8ada-78e368d54a6a.png)



**From all the results, we finally conclude that Decision Tree Classifier gives the best accuracy and F1-score amongst the 4 models used. While, SVM also shows good results to train and test**







