# Movies-ETL

## Overview of Project
Extract Transform Load (ETL)

The goal of this project was to create an automated pipeline for a company Amazing Prime that is hosting a hackathon. The topic is about movies, the data is information about movies from 1990 to 2018 and combining the information from the new data from the data listed in the data sources under the resource section. Then performing the suitable transformations on the data. Merge the parsed data sets and load the data into an existing PostgreSQL database for the Amazing Prime Hackathon.

---

## Resource:

Data Sources: movies_metadata.csv, ratings.csv, wikipedia-movies.json

Software: pgAdmin 4  v6.8, Visual Studio Code v1.67.2, Anaconda 4.13.0, Jupyter Notebook 6.4.11, Python v3.8.9

Dependences: SQLAlchemy, Psycopg2, time, pandas, json, numpy, regular expressions

---
## Results:
ETL_function_test.ipynb
    
* The data is extracted in JSON and CSV formats and is transformed into Pandas Dataframes.

* The JSON file requires the file first to be loaded and then transformed into Dataframes.

ETL_clean_wiki_movies.ipynb
    
* The clean_movies function combines scatted data of alternative languages into one column ‘alt_titles’ and the sub-function change_column_name arranges column names into regular pattern.

* The extract_transform_load function is the begins the process of transforming the wiki movie data, using Python list comprehensions, the apply(), map() methods with lambda functions and regular expressions (RegEx).

ETL_clean_kaggle_data.ipynb
    
* The extract_transform_load function is updated to clean the Kaggle data, by changing datatypes using astype(), pd.to_numeric, comparison operator method.
	 
* The missing values were filled and unneeded columns were removed.

* Using the method pd_merge the Dataframes were merge.

ETL_create_database.ipynb
    
* The sqlalchemy library and to_sql method is the last step to connect the database and complete the ETL process using the extract_transform_load function call.


---

## Summary:


---
