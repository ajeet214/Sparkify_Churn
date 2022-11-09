# Sparkify Churn Prediction

## Installed Libraries
 - NumPy
 - Pandas
 - Seaborn
 - Matplotlib
 - PySpark SQL
 - PySpark ML 
 
No additional installations beyond the Anaconda distribution of Python and Jupyter notebooks.

## Project Overview
This is one of the parts of the capstone project in Udacity's data science Nanodgeree program. There is a virtual start-up company named Sparkify(similar to Spotify) that offers music streaming services to users in the USA. Many users stream their favorite songs every day either using the basic free tier that places advertisements between the songs or the premium subscription model, where they stream the music for free but pay a monthly flat rate. Users can upgrade, downgrade, or cancel their service at any time. So, it is crucial to make sure the users love the service. Every time a user interacts with the service such as playing songs, logging out, liking a song with a thumps-up, hearing an Ad, or downgrading their service, it generates data. All this data contains key insides for keeping the users happy and helping Sparkify’s business thrive. It is our job on the data team to predict which users are at risk to churn either downgrading from premium to free tier or canceling their service altogether. If we can accurately identify these users before they leave, Sparkify can offer them discounts and incentives, potentially saving the business millions in revenue.

Sparkify keeps a Log file with 18 fields for every user interaction (e.g., userId, name of the song played, length of a song played, name of artist). Soon, the log file data volume exceeded the available memory space on standard desktop computers, and the company opted for using the distributed file system Apache Spark™. Udacity™ provides the full dataset with 12GB on AWS™ S3, and you can run a Spark cluster on the cloud using AWS or IBM™ Cloud to analyse the large amount of data.

## Project Motivation
The problem is to create a machine learning solution that can predict the user's intent to unsubscribe (Called customers' churn) before it happens in order to minimize the churn rate and provide better customer services.

The project involved:
 - Loading and cleaning a small subset (128MB) of a full dataset available (12GB) 
 - Conducting Exploratory Data Analysis(EDA) to understand the data and what features are useful for predicting churn
 - Feature Engineering to create features that will be used in the modeling process
 - Modelling using machine learning algorithms such as Logistic Regression, Random Forest, Gradient Boosted Trees, Linear SVM, Naive Bayes 

## File Descriptions
 - Sparkify.ipynb : The main jypyter notebook script file to work in Udacity workspace.
 - Sparkify.html : an HTML file for the jupyter workbook
 - README.md : this file

## Medium Blog Post 
The main findings of the code can be found in the Medium Blog post available [here](https://stephirvine.medium.com/predicting-churn-with-pyspark-4c8edc8a19e0) explaining the technical details of my project.
A Random Forest Classifier was chosen to be the best model by evaluating the F1 score and accuracy metrics. The final model achieved an F1 and an Accuracy score of 0.88. 

## Licensing, Authors, Acknowledgements, etc.
I'd like to acknowledge Udacity for the project idea and workspace.
