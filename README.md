# Movies-ETL
Resources:

    - Jupyter notebook
    - SQL:  
        - postgreSQL
        - pgadmin 4
    - csv+json data files:
        - wikipedia-movies.json, web-scraped
        - movies.csv, Kaggle
        - ratings.csv, Kaggle

## Overview

This project travels through the data extract, transform, and load pipeline known as ETL.  We received web-scraped wikipedia data for a list of movies in JSON format and movie database csv files.  Each file is loaded into a jupyter notebook, then code written and executed to clean, transform, and merge the data into a usable format.  Lastly, the clean data is loaded into a postgreSQL database using a connection engine and to_sql() method for use in pgadmin 4.  In other jupyter notebook files, code is refactored so that the cleaning and loading can be performed daily and automatically as new data is received.

## Repository Contents

**wiki_movies.ipynb** - performs entire ETL process start to finish.  First Draft.

**ETL_function_test.ipynb** - tests a function to load files and create Pandas DataFrames

**ETL_clean_wiki_movies.ipynb** - refactored wiki_movies.ipynb code to write functions automating and transforming wikipedia data

**ETL_clean_kaggle_data.ipynb** - refactored wiki_movies.ipynb code to write functions automating and transforming kaggle data then merging wikipedia dataframe

**ETL_create_database.ipynb** - performs all of the above operations (with the exception of returning dataframes) and loads data to SQL database

![Screen Shot 2022-05-13 at 2 39 56 PM](https://user-images.githubusercontent.com/100544761/168378434-aaba82ad-51b8-4827-b8a4-2fc68eb71475.png)


## Conclusion

A successful completion of the ETL process has resulted in usable movie data from multiple sources and is ready for analysis.

### Contact

Email:  mrmileyy@gmail.com