# Restaurant_Recommendation_System

## A Restaurant Recommendation System using Matrix Factorization

Recommendation systems provide consumers with individualized, relevant recommendations and have been utilized in a variety of environments, including shopping, movies, and so on. Currently, Yelp, the world's largest publisher of local business reviews, does not offer recommendations. Instead, users must filter, sort, and read reviews to see if a company can give them what they require. A personalized recommendation system would improve the user experience by encouraging users to review and rate more restaurants in exchange for better restaurant recommendations, which will provide Yelp with additional data to improve the recommendation system.
We created a restaurant recommendation system for individuals and groups based on Yelp business and Yelp reviews datasets. We developed a matrix factorization with a collaborative filtering model with features for each of the 10k Yelp users. Food preferences and dietary restrictions, as well as cuisine style, services offered, ambiance, noise level, and average rating, and so on.
As an alternative to conventional group recommendation systems that select the most frequently recommended restaurant among individual users, this method selects the most generally recommended restaurant across a group of users.


## Methodology:
This project is based on the public opinion of restaurants. The datasets was extracted from the Kaggle (provided the link below). This was acquired on July, 2021. The extracted reviews and business datasets contained 10,000 unique comments/compliments from multiple users around the world and 10 columns each.
1. https://www.kaggle.com/datasets/omkarsabnis/yelp-reviews-dataset
2. https://www.kaggle.com/datasets/tanyadixit/yelp-business-dataset


## Steps Involved:

Get data on restaurants and reviews of those restaurants.

Identify rows by customer’s ids and restaurant id's.

Preprocess the text of the reviews - remove stop words from the stop words library and normalize all text to text without punctuation.

Splitting datasets into test and train datasets in the 85:15 ratio.

Process data to train and test datasets by customer’s ids and their reviews, and restaurants ids and their reviews.

Tokenize the text of the reviews using TFID Vectorizer for easier NLP processing.

Create a value matrix of ratings, and convert it to NumPy arrays.

Matrix Factorization.



## Predictions:

We input what we desire to eat to the recommendation system, and it gives us the top 5 recommendations based on what we want to eat.

## Visualizations:

Review count by star ratings, review text length by star ratings, the number of reviews per star rating, reviews word cloud for the 1-star rating, and a 5-star rating.
