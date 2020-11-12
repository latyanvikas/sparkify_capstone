# sparkify_capstone

### Table of Contents

1. [Project Overview](#overview)
2. [Project Motivation](#motivation)
3. [Solutions Steps](#solution)
4. [Libraries Used](#library)
5. [Files](#files)
6. [Results](#results)
7. [Installation](#installation)
8. [Licensing, Authors, Acknowledgements](#final)


# Project Overview <a name="overview"></a>
I have picked sparkify as my final project for data science nano-degree capstone where we will be predicting the customer’s churn. Sparkify is a digital music service platform where we have free and paid users streaming the music online. In a simple term, we will be using various machine learning algorithm using spark MLlib to predict the customers who are most likely to cancel their subscription in future.

# Project Motivation <a name="motivation"></a>
We will be predicting the churn for the customers those are using sparkify streaming services. We have been provided with a large data sets of 12 GB for the users who have been using sparkify, however, I will be using a subset of this data.

* Essential skills that I have learned through this project are
* Load large datasets into Spark and manipulate them using Spark SQL and Spark Data frames
* Use the machine learning APIs within Spark ML to build and tune models
* Integrate the skills you’ve learned in the Spark course and the Data Scientist Nanodegree program

Initially it was quite challenging to build ML algorithms using spark as I was doing it for the first time. I have been using spark from quite some time, I found it was easy to the feature engineering. This project has given me further insights as how we can do complex data engineering tasks and build the ML algorithms using spark. It’s going to be really useful for me as I don’t have depend on scikit-learn to implement ML algorithms.

# ibraries Used <a name="library"></a>

In order to build the sparkify churn model, I have used followin libraries

* pyspark.sql
* pyspark.ml
* pyspark.mllib
* import seaborn as sns
* import matplotlib.pyplot as plt

# Solutions Steps <a name="solution"></a>

1. Loading and Cleaning the data
2. Exploratory data analysis
    * Defining Churn
    * Exploring the data
3. Feature Engineering - Building number of features form given dataset
4. Modelling — Test out several of the machine learning algorithm

# Files <a name="files"></a>

This repo has following files
* README.md - Overview of the sparkify_capstone project
* Sparkify.ipynb - The Jupyter Notebook called Sparkify.ipynb have all the solution steps mentioned above.

# Installation <a name="installation"></a>

To clone the git repository:
```
git clone https://github.com/latyanvikas/sparkify_capstone.git
```

# Results <a name="results"></a>

As an objective of this project, we have successfully used spark to load the data, clean the data, performing EDA and feature engineering the data for implementing machine learning algorithms. We have designed a scalable solution and made use of module so that this solution can be implemented on full size data.

As we can see Random Forest has the precision of .78 but the lower AUC of .32. Gradient Boosted Trees is having lower precision of .65, however the higher AUC of .59. SVM & Logistic regression model is performing on the similar lines as Random forest when we look into the precision, however, SVM has higher AUC of .43 than others. I am recommending Support Vector Machine model as it has higher precision, F1 score and AUC compare to others.

Support Vector Machine -> PR AUC: 0.43934267486899065
Support Vector Machine
 | precision = 0.782608695652174
 | recall = 0.782608695652174
 | F1-Score = 0.782608695652174


The main findings of the code can be found at the post available [here](https://vikaslatyan.medium.com/sparkify-churn-model-3a1046bcebec).

# Licensing, Authors, Acknowledgements <a name="final"></a>

I would like to say thanks to [Udacity](https://www.udacity.com/) for providing me this platform and opportunity to learn the advance techniques in data science space. They have high quality of nano-degree course and provides you detailed review of your work. Stack overflow was really helpful to solve the problems I was facing during coding of this project. I have also referred other sources online and please feel free to use the code here as you would like!
