# News_Recommendor_System
Problem Statement
iPrint is an upcoming media house in India that offers media and information services to the people. The company’s business extends across a wide range of media, including news and information services on sports, weather, education, health, research, stocks and healthcare. Over the years, through its online application, iPrint has been efficiently delivering news and information to the common people. However, with time and technological advancements, several new competitors of iPrint have emerged in the market. Hence, it has decided to begin providing a more personalised experience to its customers.

The problem statement can be divided into two parts.

Recommend new top 10 relevant articles to a user when he visits the app at the start of the day
Recommend top 10 similar news articles that match the ones clicked by the user.
You have to ensure that the system does not recommend any news article that has been pulled out from the app or has already been seen by the user. In addition, only the articles that are written in the English language must be considered for content-based recommendations. The final generated list must contain the names of the recommended articles, along with their IDs.

Exploratory data analysis

Explore the various features present in the data set for their distribution and any meaningful inferences.
Check the distribution of interaction type, consumer location/country, producer country/location, item type and so on.
Check the most common language and most popular country that consumes the articles on the platform.

Recommendation techniques

You may want to use the ‘consumer_interaction’ data set for building the ALS, user-based and item-based collaborative filtering models and ‘platform_content’ data to build a content-based recommendation model.


User-based collaborative filtering

Create user-item matrix using the rating values.
Find the user-similarity matrix based on a similarity measure.
Generate predicted ratings for all the user-item pairs.
Item-based collaborative filtering

Find the item-similarity matrix based on a similarity measure.
Generate the top 10 similar and relevant items based on the similarity scores.
Content-based filtering

Use text processing to analyse the ‘keywords’ feature in the data set.
Recommend similar items based on the TF-IDF scores.

ALS

Create Compressed Sparse user-item and item-user matrices. 
Train the ALS model and generate recommendations for a user. Try experimenting with the hyperparameters.
Hybrid recommendation system

Normalise the scores for content and collaborative filtering and combine them with an appropriate weightage to build a hybrid model.
Try out hybrids of different types of models that can help recommend items similar to a particular item. For example, Content+Item-based collaborative model, ALS+Item-based collaborative model, ALS+Content-based model, etc.
Model evaluation

Use appropriate evaluation metrics, such as RMSE, MAE and precision@k, to evaluate the recommendations generated for a user as mentioned in the first part of the problem statement and use global precision@k to assess the overall performance of the recommendation system.
