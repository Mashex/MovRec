# MovRec

## Summary 

A Movie Recommender system trained on the Movie Lens 1 Million Dataset Using a Restricted Boltzmann Machine (RBM) in PyTorch. RBM uses collaborative filtering and recommends items by trying to find users that are similar to each other based on their item ratings in this case movie review rating.

RBM is a Generative model that assigns a probability to each possible state and then using this probability we can predict similar items. 

Requirements
Python 3.6 and above
Tensorflow 1.6.0 and above
NumPy
Pandas
Matplotlib

# Dataset
The dataset used is MovieLens 1M Dataset acquired by Grouplens contains movies, users and movie ratings by these users.

## Model Description
Our model works in the following manner :-

The hidden layer is used to learn features from the information fed through the input layer.
The input is going to contain X neurons, where X is the amount of movies in our dataset.
Each of these neurons will possess a normalized rating value varying from 0 to 1: 0 meaning that a user has not watched that movie and the closer the value is to 1, the more the user likes the movie that neuron's representing.
These normalized values will be extracted and normalized from the ratings dataset.
After passing in the input, we train the RBM on it and have the hidden layer learn its features.
These features are used to reconstruct the input, which will predict the ratings for movies that the input hasn't watched, which is what we can use to recommend movies!

## References
[Restricted Boltzmann Machines — Simplified](https://towardsdatascience.com/restricted-boltzmann-machines-simplified-eab1e5878976)
[Restricted Boltzmann Machine Creation as Recommendation System](https://towardsdatascience.com/restricted-boltzmann-machine-how-to-create-a-recommendation-system-for-movie-review-45599a406deb)
[DeepLearning.net](http://deeplearning.net/tutorial/rbm.html)
