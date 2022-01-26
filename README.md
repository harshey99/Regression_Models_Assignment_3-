# Regression_Models_Assignment_3


Machine Learning Assignment 3 DescriptionMachine Learning Assignment 3 Description
Date posted: Tuesday 16 November 2021.
Due date: Sunday 28 November 2021 Monday 3 January 2022 by 23:55.
The goal of this assignment is for you to gain practical experience of performing regression on a real world dataset, using a machine learning package of your choice.
To complete this assignment, you will train two different regression models and prepare a short report. This report will describe the methodology followed, and analyse the performance of the models that were trained.
Here are the steps to be documented in your report (with the maximum marks for each aspect of your work):
Select an appropriate ML package to use for this regression task. Your report should briefly introduce your chosen package and your reasons for selecting it. [2 marks max.]
Document any steps which you followed to prepare the data for input into the ML package [1 mark max.]
In the ML package, select two different regression algorithms that you will apply to the dataset to learn two different regression models. Here are some possible choices, though other appropriate algorithms are fine too: linear regression, multi-layer perceptron, decision trees, k-nearest neighbours, support vector machines, etc. In your report, include a brief, clear description of both algorithms. Ensure that you acknowledge all of your sources of information. [2x2 = 4 marks max.]
Describe the process you followed while developing each model. Be sure to include and justify final the values selected for all parameter settings, and describe the process you followed while searching through possible parameter settings. Describe each of the models, using graphics if appropriate. [2x3 = 6 marks max]
Discuss how you divided the dataset into test/training sets and monitored for possible overfitting or underfitting. [3 marks max.]
Evaluate the performance of the two regression models using appropriate metrics (e.g., RMSE, MAE, R, R2 etc.). Discuss whether the two models give very similar or significantly different results, and why. [4 marks max.]
The dataset for this assignment in a file called "galway_rentals.txt". Columns are separated by tabs and rows are separated by newlines. Each row describes one individual instance in the dataset. The attributes are in columns in the following order: 
price_per_month, distance_eyre_square, distance_salthill , distance_nuig, distance_gmit, num_bedrooms, num_bathrooms, type, ber, balcony, floor, heating
The goal of this regression task is to predict price_per_month based on the values of the other attributes.
Your report should not exceed four A4 pages in total. Therefore, take care to ensure that it is succinct and informative, and not overly superficial. This is an individual assignment. As you are all postgraduate students, we will treat any plagiarism (from another student or other sources) very seriously.
You must submit your report as a single PDF file in Blackboard, on or before the due date. Ensure your name, class and student ID are on it.Your assignment will be marked out of 20, with the breakdown shown above. If any aspect of your work is plagiarised or is otherwise dishonest, you will receive 0 for the full assignment.

- Prof. Michael Madden & Dr. Patrick Mannion.
Guidance on handling categorical attributes in this dataset
In this dataset, some of the attributes are categorical and others are continuous. It will be necessary to encode the categorical attributes as numeric values using ordinal encoding or one-hot encoding before applying your chosen regression algorithms.
The categorical attributes are:
type - the type of property. The possible values of this attribute do not have a natural ordering. Possible values: studio, apartment, house, townhouse.
ber - the energy rating of the property. The possible values of this attribute have a natural ordering. Possible values (ordered from most desirable to least desirable): a, b1, b2, b3, c1, c2, c3, d1, d2, e1, e2, f, g, exempt.
balcony - whether the property has a balcony. Possible values: yes, no. This is a Boolean variable that could be encoded with values 1 and 0.
floor - the floor that the property is on. The possible values of this attribute have a natural ordering. Possible values (ordered from most desirable to least desirable): third, second, first, ground.
heating - the type of heating system in the property. The possible values of this attribute do not have a natural ordering. Possible values: central, electric, NA
For a further information on how to encode categorical variables, you may wish to consult the following free online resources:
Ordinal and One-Hot Encodings for Categorical Data, a blog post by Jason Brownlee (2020), https://machinelearningmastery.com/one-hot-encoding-for-categorical-data/
Chapter 5 Encoding Categorical Predictors from the book Feature Engineering and Selection: A Practical Approach for Predictive Models by Max Kuhn and Kjell Johnson (2019). Free HTML version available at http://www.feat.engineering/encoding-categorical-predictors.html
