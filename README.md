# Movies ETL
## Purpose

### Extract -
In this exercise we read in (or extracted) movie data from different sources: wikipedia.json and kaggle(movie lens - movie metadata.csv and ratings data.csv).

### Transform -  
Once the files were read into pyton we cleaned each data set using data and column examination, eliminating duplicate rows and columns and getting data within columns to be a consistent datatype.  For much of the data we used regular expressions or regex as a way to filter the data.  For example, changing box office to represent a number in consistent format throughout all records.  Once cleaned we merged the files to create dataframe (movies_df).

Once merged we then did another round of cleaning to get rid of duplicate columns and make decisions on which data set was best and in some cased determined one was better but we used the 2nd data to fill in gaps in the best data.  

### Load - 
Once these steps were completed we imported (or loaded) the data to postresql from python.  That is we created code in python to import the data.  For the ratings database which is a very large file we displayed elapsed time to give us feedback on the status of the data as it is loaded to sql.  We do this to let us know at what stage the loading process is.
