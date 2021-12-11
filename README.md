# CPSC481_EmpHappinessMonitoring

PROBLEM STATEMENT:
Mental Health is one of the important keys for the growth of an individual as well as an organization. The project will allow the employers to know the mental health status of their respective employees. 

There are various factors affecting the same as mentioned below:
a.	Working Duration in a company
b.	Gender
c.	Type of Company, e.g.: Product or Service
d.	Work From Home is available or not
e.	Designation
f.	Resource Allocation
g.	Mental Fatigue, etc.

The project will focus on computing the above-mentioned factors and derive the proper metric score for happiness of the employees. This will provide the data to the organization to take steps for employee’s mental health.
The end goal is to create the system for daily monitoring the employee’s health status and maintain the positive and stress-free work environment in any industry.

APPROACH:
![image](https://user-images.githubusercontent.com/71597613/145694626-1f15fd5d-dbaf-4c97-af91-064ea3f49445.png) 

•	Above mentioned factors are used to train the model.
•	Test Input Data is given to the trained model.
•	Output is evaluated.


DESCRIPTION OF THE SOFTWARE:
•	Code Flow:
o	Creating new column [HappyCond] using below condition: 
![image](https://user-images.githubusercontent.com/71597613/145694638-01192aa4-2207-4dcc-a94e-dfe7dde816e9.png)

o	Creating new column [tenure] from ‘Date of Joining’. 
o	Drop those rows where [happiness] is empty.
o	Impute remaining missing values with medians. 
o	Train a Gaussian Naive Bayes classifier on the training set.
o	Test the model using test.csv.

•	Programming Language: Python 
o	Numpy
o	Pandas
o	Scikit Learn Library
	Gaussian Naïve Bayes Classifier

•	Gaussian Naïve Bayes Classifier:
o	Classifies the output in two classes: 0 and 1
o	0 refers to Unhappy Class and 1 refers to Happy Class.
o	Probability of Happy and Unhappy is calculated and updated in both the classes.
o	If the Happy rate > Unhappy rate=> Employee is happy, else Unhappy.
