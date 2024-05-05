# Eat Safe, Love Data Analysis

## Overview

This project involves analyzing food hygiene ratings data provided by the UK Food Standards Agency. I was contracted by the editors of a food magazine, Eat Safe, Love, to evaluate the ratings data in order to assist their journalists and food critics in deciding where to focus future articles.

## Instructions

### Part 1: Database and Jupyter Notebook Set Up

1. Import Data: I imported the data provided in the `establishments.json` file from my Terminal and named the database `uk_food` and the collection `establishments`.

2. Library Import: Within my notebook, I imported the necessary libraries: PyMongo and Pretty Print (pprint).

3. Mongo Client: I created an instance of the Mongo Client.

4. Database Confirmation: I confirmed that I created the database and loaded the data properly by listing the databases and collections, and displaying one document from the `establishments` collection.

5. Collection Assignment: I assigned the `establishments` collection to a variable to prepare it for use.

### Part 2: Update the Database

1. Modifications: The magazine editors requested modifications to the database before performing any queries or analysis. I made the following changes to the `establishments` collection:
   - Added a new halal restaurant in Greenwich to the database.
   - Found the `BusinessTypeID` for "Restaurant/Cafe/Canteen" and updated the new restaurant with the `BusinessTypeID`.
   - Removed establishments within the Dover Local Authority from the database.
   - Converted latitude and longitude to decimal numbers.
   - Converted `RatingValue` to integer numbers.

### Part 3: Exploratory Analysis

1. Data Exploration: Using `NoSQL_analysis_starter.ipynb`, I answered specific questions to assist Eat Safe, Love magazine:
   - Identified establishments with a hygiene score equal to 20.
   - Found establishments in London with a `RatingValue` greater than or equal to 4.
   - Determined the top 5 establishments with a `RatingValue` of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours".
   - Calculated the number of establishments in each Local Authority area with a hygiene score of 0, sorted the results from highest to lowest, and printed out the top ten local authority areas.



