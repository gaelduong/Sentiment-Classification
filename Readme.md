
## Sentiment Classification

We will design a sentiment classifier for classifying the sentiment of the
reviews. This is a Natural Language Processing (NLP) task where the input is a natural
language text and output is the sentiment label. We will consider two different review
datasets: yelp reviews for restaurants and IMDB reviews for movies.

### YELP dataset

The Yelp dataset consists of 7000 reviews in the training set, 1000 reviews in the validation
set, and 2000 reviews in the test set. This is a 5 class problem where each review is classified
into one of the five ratings with rating-5 being the best score and rating-1 being the worst
score.

### IMDB dataset

IMDB dataset consists of 15000 reviews in training set, 10000 reviews in validation set, and
25000 reviews in test set. This is a 2 class problem with class 1 being positive sentiment and
class 0 being negative sentiment.

### Approach

- Define the vocabulary for each dataset (10000 most common words for each dataset)
- Convert the dataset (reviews) in binary-bag-of-words (BBOW) representation and frequency-bag-of-words (FFOB) representation.
- Train and tune Naive Bayes, Decision Tree, SVM model on both representations (BBOW and FBOW) to classify the sentiments of the new reviews and compare the performances of the models.
- F1 is used as the evaluation metric.
