# UK Food Standards Agency Food Hygiene Rating - Data Analysis

## Project Overview

In this project, I were contracted by the editors of a food magazine, Eat Safe, Love, to evaluate the food hygiene rating data provided by the UK Food Standards Agency.

I used ***NoSQL (MongoDB)*** to store and manipulate the data and Jupyter Notebook to perform exploratory analysis on the data.

I made modifications to the database as per the editors' requirements and answered specific questions to help them decide where to focus future articles.

## Prerequisites
To run this project, I will need the following:

Python,
Jupyter Notebook,
PyMongo, and
Pandas

I will also need to have access to the establishments.json file provided.

## Database and Jupyter Notebook Set Up

***Import Data***

* Import the data provided in the establishments.json file from Terminal.
* Name the database ***uk_food*** and the collection ***establishments***.

***Import Libraries***

* Import the libraries needed for data analysis: PyMongo and Pretty Print (pprint).
* Create an instance of the Mongo Client.

***Confirm Database and Data Loaded Properly***

* List the databases in MongoDB and confirm that ***uk_food*** is listed.
* List the collection(s) in the database to ensure that ***establishments*** is there.
* Find and display one document in the ***establishments*** collection using ***find_one*** and display with ***pprint***.
* Assign the ***establishments*** collection to a variable to prepare the collection for use.

## Update the Database
The magazine editors have requested some modifications to the database before performing any queries or analysis for them.

1- An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked me to include it in my analysis.

2- Find the ***BusinessTypeID*** for "Restaurant/Cafe/Canteen" and return only the ***BusinessTypeID*** and ***BusinessType fields***.

3- Update the new restaurant with the ***BusinessTypeID*** I found.

4- The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.

5- Some of the number values are stored as strings, when they should be stored as numbers. Use ***update_many*** to convert latitude and longitude to decimal numbers.

## Exploratory Analysis
Eat Safe, Love has specific questions they want answered, which will help them find the locations they wish to visit and avoid. Use the following questions to explore the database, and find the answers.

***Questions and Analysis***

For each question, use ***count_documents*** to display the number of documents contained in the result,

display the first document in the results using ***pprint***,

convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.

1- Which establishments have a hygiene score equal to 20?

2- Which establishments in London have a RatingValue greater than or equal to 4?

3- What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

4- How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

## Conclusion
In this project, I demonstrated how to work with ***NoSQL databases***( MongoDB) to store and manipulate data.

I also showed how to use Jupyter Notebook to perform exploratory analysis on the data and answer specific questions. By making modifications to the database as per the editors' requirements and answering their questions, I provided insights that could help them decide where to focus future articles. This project showcases the power of NoSQL databases in storing and processing large datasets and the flexibility they offer in handling unstructured data.

