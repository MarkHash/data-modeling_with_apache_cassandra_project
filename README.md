# Introduction

## Purpose of this project

Startup company, Sparkify, launched their new streaming app and collected song and user activities in JSON format. This project is to create a Apache Cassandra database with queries to provide the insight of app's usage for analytics team.

# Database modeling

## Apache Cassandra Database

This project uses Apache Cassandra Database to provide the following data 

1. Provide the artist, song title and song's length in the music app history that was heard during  sessionId = 338, and itemInSession  = 4
2. Provide only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
3. Provide every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

## ETL pipeline

Sparkify has one type of dataset (event_data). This project creates two ETL piple for each dataset.

1. Creates a list of filepath for event_data
2. Reads data from each event_data file
3. Creates a new csv file named `event_datafile_new.csv` to load data into tables

# Files and instructions

## Files in this repository

- `Project_1B_Project_Template.ipynb` reads and processes event_data files and loads them into tables
- `event_datafile_new.csv` collects data from event_data files
- `README.md` discusses this project

## Run instructions

1. Run `Project_1B_Project_Template.ipynb` to process event_data and load to tables