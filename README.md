# BSAN6070_CA05

## The Application

At scale, this would look like recommending products on Amazon, articles on Medium, movies on Netflix, or videos on YouTube. Although, we can be certain they all use more efficient means of making recommendations due to the enormous volume of data they process. However, we could replicate one of these recommender systems on a smaller scale using what we have learned here in this article. Let us build the core of a movies recommender system.

What question are we trying to answer?

Given a movies data set, what are the 5 most similar movies to a movie query?

## The Data

The data contains thirty movies, including data for each movie across seven genres and their IMDB ratings. The labels column values are all zeroes because we aren’t using this data set for classification or regression. You can ignore this column. The implementation assumes that all columns contain numerical data.

Additionally, there are relationships among the movies that will not be accounted for (e.g. actors, directors, and themes) when using the KNN algorithm simply because the data that captures those relationships are missing from the data set. Consequently, when we run the KNN algorithm on our data, similarity will be based solely on the included genres and the IMDB ratings of the movies

## Building Your Own Reccomender System

You are building your own movie recommendation website which uses your Recommendation Engine at the back-end. You are going to build this back-end Recommendation Engine. Imagine a user is navigating your recommendation website, and he/she encounters a movie named “The Post”. The user is not sure if he/she wants to watch it, but its genres intrigue the user; he/she is curious about other similar movies. The user scrolls down to the “More Like This” section to see what recommendations your recommendation website will make, and the back-end algorithmic gears begin to turn.

Your website sends a request to its back-end for the 5 movies that are most similar to The Post. The back- end has a recommendation data set exactly like ours. It begins by creating the row representation (better known as a feature vector) for The Post, then it runs a program similar to the one below to search for the 5 movies that are most similar to The Post, and finally sends the results back to the user at your website.

Following is the genre information about the movie “The Post”:

IMDB Rating = 7.2, Biography = Yes, Drama = Yes, Thriller = No, Comedy = No, Crime = No, Mystery = No, History = Yes

Implement this problem using Python scikit-learn and display the answer within the Notebook with proper narrative / comments.

