## Movies-ETL
![ALT Text](https://user-images.githubusercontent.com/30667001/153760764-7c974de6-e3da-4b4b-968b-e3e80ff7b674.png)

The purpose of the Extract, Transform, Load process is to read data from multiple sources (extract), clean the data to create a consistent structure (transform), then write the data into a database for storage (load). For this project, an automated ETL pipeline was created to load differing movie data into existing tables of a PostgreSQL database for use in an Amazing Prime hackathon. 

## Resources
- Data Sources: wikipedia-movies.json, Kaggle movies_metadata.csv, MovieLens ratings.csv
- Software: Python 3.7.6, Jupyter Notebook 6.4.5, PostgreSQL 11.14-1, pgAdmin4
- Libraries: Pandas, NumPy, json, RegEx, time


## Project
Pipeline creation steps included:
* Writing an ETL function to read in the three data files and creating three separate dataframes.
* Extracting and transforming Wikipedia data to filter out unnecessary data, group data as needed and format to a consistent expression.
* Extracting and transforming Kaggle data as performed previously.
* Creating the movie database by merging Wikipedia and Kaggle dataframes on pre-determined bases, filling in missing data, combining the results with the MovieLens dataframe, and loading all work into the PostgreSQL movie_data database "movies" and "ratings" tables.

     ![CmpData](https://user-images.githubusercontent.com/30667001/153760793-075ea9ae-4751-4760-b3a3-70c5f8adc39c.png)

![PostregSQL](https://user-images.githubusercontent.com/30667001/153760779-409d472c-139c-48a0-9179-24d537cba8db.png)

## Summary
This project required the extraction of disparate data, multiple iterations to clean the data with techniques such as list comprehension to filter data, lambda and regular expression (regex) use to convert values, a comparison of Wikipedia and Kaggle data to determine best use, and the application of the time module to identify the time-related task of loading work in order to produce the final product.

