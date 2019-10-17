# ETL_Project_comic


Project Report
Contributors :  Eric Kleppen and Bimi Bisht.

The purpose of this project was to create a relational database in MySQL to store data about Marvel and DC comic book characters and their superpowers. We transformed the data and loaded it using Python. We also checked the relation between eye color and good/bad characters.

Extract:

Original Data Sources include:
1. FiveThirtyEight Comic Characters Dataset from Kaggle.com
2. API pull from comicvine.gamespot.com/api/

The superpowers were extracted from the API using a for loop nested within a for loop due to the way the JSON data was structured. Because of API limits, we pulled only the first 100 superpowers from the API.

Transform 

The data was reviewed, and the irrelevant columns were dropped. The clean data was then used to create data frames that matched the relational schema we designed. We created separate dataframes for the characters and character attributes to maintain a relationship. The real names and the character names were split into separate columns so the characters could later be matched to the superpowers dataset. 

Load 

Each dataframe was loaded into its corresponding table in our schema. We loaded the following datasets:
•	Characters
•	Character attributes
•	Powers
•	Character Powers
Once the data was loaded, tests were run to validate that the data was loaded and available for data analysis. Database comic_db was created.

Analysis: We did not have information about the superpowers of all the comic characters so we chose this particular topic. MySQL database is easy to use and even though we had a large data to process it was easily loaded and was available to use.





