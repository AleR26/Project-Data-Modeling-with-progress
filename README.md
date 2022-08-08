# Project: Data Modeling with Postgres

In this project we work with a JSON files provided by startup called Sparkify, we create a ETL pipeline for that first:
1. Create a database with 5 tables.
2. Extract information from JSON files.
3. Use pandas library to transform data
4. Insert the data in SQL tables

You can see how this project works if you runs the python scripts for that is necessary:
- Open the terminal
- Run the create_tables.py file to create the database and the tables for that is necessary write the next statement:
    - python create_tables.py
- Run etl.py file in this file we connect to the database and insert the information that we need in our database, for that is necessary write the next statement:
    - python etl.py
    

## Files in the repository:
- data folder: Contains the JSON files 
- create_tables.py: In this file you are going to find the functions to: create the database, create tables and drop tables.
- sql_querys.py: This file contains every query and sql statement to: drop tables, create tables, insert data, and select data.
- elt.ipynb: This is the jupyter notebook where contains the ETL process for each of the tables we can run step by step in the notebook!
- etl.py: Function for the ETL process in this project.
- README.md: this document containts the information for the project.
- test.ipybn: Jupyther notebook to check the database.

State and justify your database schema design and ETL pipeline.
## Schema design
I use a star schema for the database because we need 4 dimension tables and 1 fact table to store the data. With this schema is time efficient and allow us to query data and create joins more easily.

## ETL pipeline
Steps in the ETL pipeline:
1. First we read the song_data JSON file then insert the data in song and artist tables.
2. Convert the log_data JSON file in a dataframe
3. Transforme data and insert into time and users tables
4. Finally we create a join to insert into songplay fact table





