# project2

This Project is proposing two possible data sets to work with. 

The first Dataset is Bank Marketing

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

The Second is Fertility Data Set

1) Source of data
David Gil, dgil '@' dtic.ua.es, Lucentia Research Group, Department of Computer Technology, University of Alicante
2) Brief description of data
100 volunteers provide a semen sample analyzed according to the WHO 2010 criteria. Sperm concentration are related to socio-demographic data, environmental factors, health status, and life habits
3) What is the target?
Diagnosis normal (N), altered (O)
4) Is this a classification or regression problem?
This is Classificatio Problem
5) How many features?
10
6) How many rows of data.
100
7) What, if any, challenges do your foresee in cleaning, exploring, or modeling with this dataset?
Cleaning
Renaming Columns
Exploring
Correlation
Visualization
Preprocessing
Scaling
