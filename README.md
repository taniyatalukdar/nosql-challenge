# nosql-challenge

# nosql-challenge

The NoSQL_setup.ipynb sets up and updates the database. 
The queries NoSQL_analysis.ipynb analyses the data and converts the results into Pandas DataFrame. Used the command: mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json from the establishments.json to create the DB.

Database and Jupyter Notebook Set Up
Importing the data in establishments.json and converted it into a dataframe using crowdfunding_info_df = pd.read_excel('Resources/crowdfunding.xlsx') and check the datatypes.
Libraries imported were: pandas as pd, numpy as np, pd.set_option('max_colwidth', 400) and re.
After creating an instanse of mongodb, we listed the: database, collections and documents. 

Update the Database
1. Inserted the information of the new restaurant provided on Canvas.
2. Looked up BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
3. Updated the BusinessTypeId.
4. Checked and removed establihment from Dover Local Aut - hority.
5. Converted dtatypes from string to ints/ floats for numeric values.


Exploratory Analysis
Used NoSQL_analysis_starter.ipynb for this section of the challenge.
1. Which establishments have a hygiene score equal to 20? - 41
2. Which establishments in London have a RatingValue greater than or equal to 4? - There are 33 establishments in London that have a RatingValue greater than or equal to 4 from the uk_food dataset.
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"? -  The top 5 establishments with a RatingValue of '5' sorted by lowest hygiene score nearest to "Penang Flavours" are: "Volunteer", "Plumstead Manor Nursery", "Atlantic Fish Bar", "Iceland", and "Howe and Co Fish and Chips - Van 17".
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas. - There are 55 rows in the DataFrame. This is the preview of the first 10 rows:

![alt text](https://github.com/taniyatalukdar/nosql-challenge/tree/main/Images.png?raw=true)
