# Data Modeling with Postgres

## Summary
As part of the "Data Modeling with Postgres" project, I have created a relational database schema and performed ETL (Extract, Transform, Load) processes using PostgreSQL. The main objective of this project is to design a database for a fictional music streaming service called Sparkify, enabling efficient analysis of user activity and song data.

## How to Run the Python Scripts
To run the project, follow these steps:

1. Install PostgreSQL if you haven't already.
2. Create a new PostgreSQL database for the project.
3. Update the database connection details in the `create_tables.py` and `etl.py` scripts to match your database configuration.
4. Run the `create_tables.py` script to drop and create the necessary tables in the database.
5. Run the `etl.py` script to perform the ETL process, which involves extracting data from JSON files, transforming it, and loading it into the PostgreSQL database.
6. Open and run the cells in the `test.ipynb` Jupyter Notebook to verify that the tables were created and filled with data.

## Files in the Repository
The project repository contains the following files:

1. `create_tables.py`: This script is responsible for dropping and creating the tables defined in the `sql_queries.py` file. Running this script is a prerequisite before executing the ETL process.
2. `etl.py`: This script performs the ETL process by extracting data from JSON files, transforming it, and loading it into the PostgreSQL database. It connects to the Sparkify database and processes the `log_data` and `song_data` to populate the five tables.
3. `sql_queries.py`: This file contains the SQL queries used by the other scripts. It includes queries for creating tables, inserting data, and performing other database operations.
4. `test.ipynb`: This Jupyter Notebook provides a way to test the database and query the tables to ensure that the ETL process was successful. It can be used to verify that the five tables were created and filled with data.
5. `data/`: This directory contains sample data in JSON format that is used for the ETL process.

## Comments and Docstrings
Throughout the project, I have made effective use of comments to explain the purpose and functionality of the code. Each function in the scripts has a docstring that provides a brief description of the function, its parameters, and its return value. These comments and docstrings enhance the readability and maintainability of the code.
