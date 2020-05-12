# Disaster Response Pipeline Project
This project is to classify disaster response messages through machine learning. 

## Content
- Data
  - process_data.py: reads in the data, cleans and stores it in a SQL database. Basic usage is python process_data.py MESSAGES_DATA CATEGORIES_DATA NAME_FOR_DATABASE
  - disaster_categories.csv and disaster_messages.csv (dataset)
  - DisasterResponse.db: created database from transformed and cleaned data.
- Models
  - train_classifier.py: includes the code necessary to load data, transform it using natural language processing, run a machine learning model using GridSearchCV and train it. Basic usage is python train_classifier.py DATABASE_DIRECTORY SAVENAME_FOR_MODEL  
- App
  - run.py: Flask app and the user interface used to predict results and display them.
  - templates: folder containing the html templates

## Example:
> python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db

> python train_classifier.py ../data/DisasterResponse.db classifier.pkl

> python run.py

## Screenshots
This is the frontpage:
![Alt text](https://github.com/janierkkilae/Disaster-Response-Pipelines/blob/master/Screenshot1.PNG?raw=true "Screenshot1")

By inputting a word, you can check its category:
![Alt text](https://github.com/janierkkilae/Disaster-Response-Pipelines/blob/master/Screenshot2.PNG?raw=true "Screenshot2")

## About
This project was prepared as part of the Udacity Data Scientist nanodegree programme. The data was provided by Figure Eight. 
