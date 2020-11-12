# Loan-Approval-Prediction

# Table of Content
<ul>
 <li>Introduction
  <ul><li>Problem Description</li>
   <li>Data Understanding</li></ul>
 </li>
 <li>Data Acquisition/Cleaning </li> 
 <li>Modeling</li>
 <li>Conclusion</li>
</ul>

<br>
<h1>Introduction</h1>
<h2>Problem Description</h2>

<p>Loan eligibility is primarily dependent on the income and repayment capacity of the individual(s). There are other factors that determine the eligibility of loan such as age, financial position, credit history, credit score, and other financial duty. </p>
<p>Loan Approval Prediction is automate loan eligibility process from customer details. These details are Gender, Marital status, Education, Number of dependents, Self-employed, Monthly income, Loan Application amount and Credit history. In this process identify the customer segmentation and those are eligible for the loan amount.</p>

<h2> Data Understanding </h2>

### Data Sets
	Range Index: 614 entries (0 to 613) <br> Data columns: 13 columns
  
  
<h2>Data Acquisition/Cleaning</h2>
  First downloaded the data from source and find the data information, description and shape of the data in after analysis. There were missing values from dataset, because of lack of record keeping. And also lot of data is object type. It is trouble to feature prediction. So we change the datatype from object to numeric values.
	
  Data set has to several problems, so start the cleaning of data. First, there were lot of missing values. There are Gender, Married, Dependents, Self_Employed, LoanAmount, Loan_Amount_Term and Credit_History. These missing values replace from zero to mean and some kind of categorical values are contain missing values replace to ‘Undefined or other’ categorical value. For example, we consists of columns are Gender, Married, Dependents, Self_Employed. These are categorical values, so that missing value of these columns replace to another categorical values like, undefined or others.
  
  Second, data has lot of data is object data type, so encode the data. Encoding is used to change the values from object to numeric. The columns are Gender, Married, Dependents, Self_Employed and Property_Area. These are categorical values, so encode that data. For example, we consists of columns are Gender. It has two values are Male and Female. These values are change in male (0) and female (1). It is purpose easy to implement predictive modelling.       
  
  After fixing these problems, I checked for outliers in the data. I found there were some extreme outliers, mostly caused by some types of small sample size problem.
  
## Predictive Modelling
Predictive modelling uses statistics to predict outcomes. It is the general concept of building a model that capable of making predictions. Typically, such a model includes a machine learning algorithm that learns certain properties from a training dataset in order to make those predictions.

### Models
Models can use one or more classiﬁers in trying to determine the probability of a set of data belonging to another set. There are two types of models, Regression and Classification. 
Regression is Supervised Learning task where output is having continuous value. The goal here is to predict a value as much closer to actual output value as our model can and then evaluation is done by calculating error value. The smaller the error the greater the accuracy of our regression model.
		 Classification is a Supervised Learning task where output is having deﬁned labels (discrete value). The goal here is to predict discrete values belonging to a particular class and evaluate on the basis of accuracy. It can be either binary or multi class classiﬁcation. In binary classiﬁcation, model predicts either 0 or 1; yes or no but in case of multi class classiﬁcation, model predicts more than one class.
		In this project target value is categorical type (discrete value). So I choose classification model.

### Applying standard Classification algorithms 
Classiﬁcation in machine learning and statistics is a supervised learning approach in which the computer program learns from the data given to it and make new observations or classiﬁcations. A classiﬁcation model attempts to draw some conclusion from observed values. Given one or more inputs a classiﬁcation model will try to predict the value of one or more outcomes. Outcomes are labels that can be applied to a dataset.
		There are a number of classiﬁcation models. Classiﬁcation models include K nearest neighbour and Naive Bayes, Logistic regression, Decision tree, and Random forest.

## Performance of Models
Model evaluation metrics are required to quantify model performance. I choose the model evaluation metrics depends on our machine learning task such as classification algorithms. In precision – recall are useful for multiple tasks. 
The Classification metrics include classification accuracy, confusion matrix, log loss and f – measure.


I applied some classification metrics for model evaluation. There are Classification accuracy and Confusion matrix. Classification accuracy is the number of correct prediction made as a ratio of all predictions made. Confusion matrix provide a more detailed breakdown of correct and incorrect classification for each class. And also fine Actual and predicted values (True and False).
		It estimated performance of a model tells as how well it preform on unseen data. And also I find best classifier on this problem based on the table, it is decision tree. It has to high accuracy and better result on confusion matrix. In table explain performance of different models (Table 1.1).


## Conclusion:
Finally, I predicted the severity of the collision based on further analysis. I achieved above 80% accuracy in classification algorithms. That is helps to identify the eligibility of loan. And also analysis of major features, it used to get better result of this problem. 
Purpose of this project was to predict the Loan Approval. Company wants to automate the loan eligibility process based on customer details. These details are Gender, Marital status, Education, Number of dependents, Self-employed, Monthly income, Loan Application amount and Credit history. In this process identify the customer segmentation and those are eligible for the loan amount.

  
