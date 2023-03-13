# Data Modeling with Cassandra

---
A UDACITY Data Engineering Nanodegree Project
2nd project.

## About The Project

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what, when and how users are playing songs on the company's music app. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions. The task is to create a database for this analysis. 

In this project, you'll be :

-   Modeling the data with Cassandra
-   Creating an ETL pipeline using Python

## Project structure

1.  **event_data**  
folder nested at the home of the project, where all needed data reside.
2.  **Project_1B_ Project_Template.ipynb**  
a notebook contains the code itself.
3.  **event_datafile_new.csv** 
 a smaller event data csv file that will be used to insert data into the Apache Cassandra tables.
4.  **images**  
a screenshot of what the denormalized data should appear like in the event_datafile_new.csv.
5.  **README.md**  
current file, provides discussion on my project.

## How to Use

Just run the  **Project_1B_ Project_Template.ipynb**  notebook to process the **event_data** files, create **event_datafile_new.csv** file like the above, create the schema, load the tables, run some analytics queries, and finally close the connection.

## Datasets

For this project, you'll be working with one dataset:  `event_data`. The directory of CSV files partitioned by date. Here are examples of file paths to two files in the dataset:
````
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
````

### Analytics tables
1. **song_info_by_session**
		sessionId, itemInSession, artist, song, length.
		
2. **song_and_user_info_by_userid_and_session**
		userId, sessionId, itemInSession, artist, song, firstName, lastName.
		
3. **username_by_song_title**
		song, userId, firstName, lastName.

