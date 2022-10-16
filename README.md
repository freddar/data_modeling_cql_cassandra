# Project 2: Data Modeling with Apache Cassandra

This project creates an __Apache Cassandra database__ for a music app called __Sparkify__.

The aim of this NoSQL database is to answer questions on song play data. 

The data model offers a __DENORMALIZED DATASET__ with which a table for each of the following queries is included in the new database:

* Give the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
* Give only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
* Give every user name (first and last) in the music app history who listened to the song 'All Hands Against His Own'

## Dataset

The dataset with which this project is carried out is called __event_data__. It is a directory of CSV files partitioned by date.

## ETL Pipeline

* Iterate through each event file in __event_data__
* Process and create a new CSV file in __Python__
* Create __Apache Cassandra tables__ 
* Load processed records into the relevant tables
* Run __SELECT__ statements to query the database and answer the three given questions
