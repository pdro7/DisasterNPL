# Disaster Response Pipeline Project
<p align="center">
  <img width="560" height="400" src="https://www.tetratech.com/en/images/emergency-management-and-disaster-recovery-mk14-204-3-650.jpg?blobheader=image/jpeg">
</p>

In this project we are using data from the company Figure eight, they provide to pre-labeled text and twit messages from real life messages, the goal of the project is to prepare the data with a ETL pipeline and then buil a MLP (Machine Learning Pipeline) to  classifies disaster messages.

The project include a web app where an emergency worker can input a new message and get classification results in several categories. The web app will also display visualizations of the data.

Following a disaster a lot of messages are received through different channels, sms, tweets, social media and so on. It is important to identify the purpose of every message in an automatic way to help the organizations involved in helping people affected by a disaster. 

<p align="center">
  <img  src="https://i.ibb.co/WHf9PKd/disaster.png">
</p>

<p align="center">
  <img  src="https://i.ibb.co/9q20N0R/disaster-images.png)">
</p>

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/
