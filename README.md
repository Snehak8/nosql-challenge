# nosql-challenge

Database and Jupyter Notebook Set Up:

Imported the data from the establishments.json file into MongoDB.
Created a database named "uk_food" and a collection named "establishments".
Imported necessary libraries including PyMongo and pprint.
Created an instance of the MongoClient.
Confirmed the database creation and data loading by listing databases and collections, and displaying one document from the establishments collection using pprint.
Update the Database:

Added a new restaurant named "Penang Flavours" with specific information to the establishments collection.
Found the BusinessTypeID for "Restaurant/Cafe/Canteen" and updated the new restaurant with this BusinessTypeID.
Checked the number of documents containing the Dover Local Authority, removed any establishments within this authority, and confirmed the deletion.
Converted number values stored as strings to numeric values using update_many for latitude, longitude, and RatingValue fields.
Exploratory Analysis:

Answered specific questions using count_documents, find_one, and displaying results as DataFrames:
Identified establishments with a hygiene score equal to 20.
Identified establishments in London with a RatingValue greater than or equal to 4.
Found the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score and nearest to the new restaurant "Penang Flavours".
Determined the number of establishments in each Local Authority area with a hygiene score of 0, sorted the results, and displayed the top ten local authority areas
