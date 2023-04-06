# project2

 

This project will be focusing on the  Bank Marketing Data Set from Kaggle described below.

1) Source of data
Source:
[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014
2) Brief description of data
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.
There are four datasets: 1) bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014] 2) bank-additional.csv with 10% of the examples (4119), randomly selected from 1), and 20 inputs. 3) bank-full.csv with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs). 4) bank.csv with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs). The smallest datasets are provided to test more computationally demanding machine learning algorithms (e.g., SVM).
3) What is the target?
The goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).
4) Is this a classification or regression problem?
This is a classification Problem 5) How many features?
17 Features
6) How many rows of data.
4521
7) What, if any, challenges do your foresee in cleaning, exploring, or modeling with this dataset?
Cleaning
None
Exploring
Correlation
Visualization
Preprocessing
Scaling
OneHotEncoding of Nominal Features


# Relevant insights from the data.


![alt text](https://github.com/gatimo256/project2/blob/58ba4abe8868a2775c10ef72999525d5db015bca/Corr.png)
Most of the features have weak correlations with one another apart from pdays and previous outcome which have a moderate positive correlation with one another.

-- insert box plot
From the Visualization above we can see that distribution of Age from different Job types.
* As expected,most customers who are retired are between 60 and 70 years
* Customers in Management are within 30 and 50 years of age.


-- insert graphy of duration

Longer Call durations had a higher success rate from the previous campaign

-- insert percentage yes/no
From the visualization above we can see that the customers who said yes to the Previous Campain had a higher percentange of saying yes to the Current Term Deposit Campaign

-- insert pie charts

From the above visualization we can make the following observiations
* 85 percent of customers don't have a personal loan
* We do not know the previous outcome of the previous campaign for 82 percent of the customers
* 57% of the Customers have a Housing Loan
* The most common job type for our customers is Blue Collar and Managemnt Jobs with 21%


Machine Learning

The Machine Learning Models used were as follows
- Logistic Regression Model
- Random Forrest Classifier
- XGB Classifier
- KNN Classifier


All the models seemed to perform poorly on the data, probably because the target data was quite imbalanced. 

The Model that performed the best  with an f1-score with 0.22 ( before tuning) was the Logistic regression Model. 
Not only did it perform better but it had the fastest run time out of all the 4 learning models used. 

This was was chosen as the final regression model and with further Hyper Parameter tuning, the f1-score was improved to 0.32. A significant improvement but still not good for a production model. 

Proposed future activities
- With the imbalanced data, I will perform some DataSampling Techniques(oversampling, undersampling) to introduce some balance to the target data. Maybe then the Learning Model will perform better than than it is now. 

