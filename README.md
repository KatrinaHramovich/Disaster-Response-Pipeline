# Disaster-Response-Pipeline
## Project Description
In this project, we will build a model to classify messages that are sent during disasters. There are 36 pre-defined categories, and examples of these categories include Aid Related, Medical Help, Search And Rescue, etc. By classifying these messages, we can allow these messages to be sent to the appropriate disaster relief agency. This project will involve the building of a basic ETL and Machine Learning pipeline to facilitate the task. This is also a multi-label classification task, since a message can belong to one or more categories. We will be working with a data set provided by Figure Eight containing real messages that were sent during disaster events.

Finally, this project contains a web app where you can input a message and get classification results.
![](https://github.com/KatrinaHramovich/Disaster-Response-Pipeline/blob/main/app_web.PNG)

## File Description
        disaster_response_pipeline
          |-- app
                |-- templates
                        |-- go.html
                        |-- master.html
                |-- run.py
          |-- data
                |-- disaster_message.csv
                |-- disaster_categories.csv
                |-- DisasterResponse.db
                |-- process_data.py
          |-- models
                |-- classifier.pkl
                |-- train_classifier.py
          |-- Preparation
                |-- categories.csv
                |-- ETL Pipeline Preparation.ipynb
                |-- ETL_Preparation.db
                |-- messages.csv
                |-- ML Pipeline Preparation.ipynb
                |-- README
          |-- README

## Installation
Must runing with Python 3 with libraries of numpy, pandas, sqlalchemy, re, NLTK, pickle, Sklearn, plotly and flask libraries.

## File Descriptions
App folder including the templates folder and "run.py" for the web application
Data folder containing "DisasterResponse.db", "disaster_categories.csv", "disaster_messages.csv" and "process_data.py" for data cleaning and transfering.
Models folder including "classifier.pkl" and "train_classifier.py" for the Machine Learning model.
README file
Preparation folder containing 6 different files, which were used for the project building. (Please note: this folder is not necessary for this project to run.

## Instructions

1 Run the following commands in the project's root directory to set up your database and model.

a) To run ETL pipeline that cleans data and stores in database python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db

b) To run ML pipeline that trains classifier and saves python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl

2 Run the following command in the app's directory to run your web app. python run.py

3 Go to http://0.0.0.0:3001/

          
