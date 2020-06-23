# Udacity Data Engineering Nanodegree
# Project 1b: Data Modeling with Cassandra

This project is a mockup for a fictional music streaming service, Sparkify, which wants to analyze the data they've collected on user activity.

# Source Data

The source data is event_data broken into multiple JSON formatted files.  Event data includes items such as userId, sessionId, user first/last names, and the song played on the event

# Queries

The primary queries supported by this database are:

* Get artist, song title, and song length for a given sessionId and itemInSession
* Get artist, song title, and user first/last names for a given userId and sessionId (sorted by itemInSession)
* Get user first/last names for users that have listend to a given song title

To support these operations, tables have been generated for each query.  In setting the clustering columns, some assumptions have been made on whether downstream users would want sorted results.
    
# Repository Contents

Included in the repository are:

* event data files in ./event_data
* all project work in Project_1B_Project_Template.ipynb
    * Definition of create/insert/drop/select queries
    * Sample ETL and query code
* event_datafile_new.csv
    * This file is a concatenation of all event_data.  It is generated by Project_1B_Project_Template.ipynb, but included in the repo as a sample