# Restaurant_Recommendation_System

## A Restaurant Recommendation System using Matrix Factorization

Recommendation systems provide consumers with individualized, relevant recommendations and have been utilized in a variety of environments, including shopping, movies, and so on. Currently, Yelp, the world's largest publisher of local business reviews, does not offer recommendations. Instead, users must filter, sort, and read reviews to see if a company can give them what they require. A personalized recommendation system would improve the user experience by encouraging users to review and rate more restaurants in exchange for better restaurant recommendations, which will provide Yelp with additional data to improve the recommendation system.
We created a restaurant recommendation system for individuals and groups based on Yelp business and Yelp reviews datasets. We developed a matrix factorization with a collaborative filtering model with features for each of the 10k Yelp users. Food preferences and dietary restrictions, as well as cuisine style, services offered, ambiance, noise level, and average rating, and so on.
As an alternative to conventional group recommendation systems that select the most frequently recommended restaurant among individual users, this method selects the most generally recommended restaurant across a group of users.


## Theory:
When we consider factorization, we can compare it to the concept of three times nine equaling twenty-seven. Although twenty-seven is a large number, we can represent it as a product of two small numbers, three and nine, allowing us to break down a large number into two small ones. Matrix Factorization is based
On a similar notion. Recommendation systems are mainly classified into two categories.
Content-Based System
Collaborative Filtering (CF) System
Entirely based on past interactions between the customer and the product. Thus, the primary input for Collaborative filtering (CF) is historical data relating to all transactions between user interactions with targeted products. Matrix is used to store data, where rows are customers and columns, are products. This technique is purely dependent on historical data and nothing more, such as current trends and cultures. At the deepest level, CF can be classified into memory-based and pattern-based methods. The memory-based method is the simplest method that tracks only historical data with a simple distance
measurement. The model-driven approach used a model to fit possible outcomes.
A recommendation system is a data filtering system that attempts to forecast the user's rating of an item (in this case a restaurant). We can divide the huge matrix of user and item ratings into two smaller user-feature and item-feature matrixes. For instance, if user A enjoys hotdogs but despises pizza, and restaurant P serves excellent hotdogs, we multiply the matrices using the dot product, and the result is the ratings (in the example above will be 11).
In order to use the text for the matrix factorization recommendation system, we will follow the architecture below to extract the features from the review text.
For each user, combine all reviews into one paragraph. After combining everything, apply the TFIDF vectorizer to extract features from the text. Each restaurant should take a similar approach and specify max_feature to match the dimensions of the matrix.


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
