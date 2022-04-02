# Collaborative Filtering Recommendation System

Collaborative filtering is a highly effective recommendation system and popularlized through the Netflix Prize competition in 2009. The basic intuition behind collaborative filtering is that if User1 and User2 both like items A, B, C, then if User1 also likes item D we would expect that User2 would like it as well. Bilinear prediction of the target variable (i.e. like, rating) is a simple parametric method that has been highly successful. Of particular interest, this is independent of any features associated with the specified items.

While the Netflix data provides an example of explicit ratings (input directly by the user), it is also possible to use implicit feedback. Examples of implicit ratings could be coding a "1" for movies that were stopped within the first quarter of the movie and never finished, or perhaps a "4" or "5" could be coded if a movie was watched until the end and the user then watched a similar movie. 

Collaborative filtering recommendation systems can suffer from a "cold start" problem referring to the fact that new users and new products/content will not have any pre-existing data from which to draw and there is no way to calculate similarity to other items. This can be overcome through (i) solicitation of initial ratings for new users, and/or (ii) supplementation of content-based recommender systems. 


## Conclusions

* Collaborative filtering models are an effective way to recommend content based upon user behavior (and utilize this data)
* Explicit data can be utilized (user ratings), though features can also be calculated with implicit data (e.g. did someone stop watching a movie after 5 minutes?)
* Collaborative filtering can be used to make recommendations for a given user or based on a single product
* The collaborative filtering model used in this notebook is based upon singular value decomposition
* "Surprise", a Python scikit, is a very useful and efficient tool for building recommender systems, even with particularly large, sparse matrices
