## Supervised Learning Techniques for Sentiment Analytics

[1]: http://ai.stanford.edu/~amaas/data/sentiment/
[2]: http://thinknook.com/twitter-sentiment-analysis-training-corpus-dataset-2012-09-22/

Classify tweets or movie reviews as either positive or negative. Used logistic regression as well as a Naive Bayes classifier from python’s well regarded machine learning package scikit-learn. As a point of
reference, Stanfords Recursive Neural Network code produced an accuracy of 51.1% on the IMDB dataset and 59.4% on the Twitter data.

## Approaches
1. A more traditional NLP technique where the features are simply “important” words and the feature vectors are simple binary vectors.
2. Doc2Vec technique where document vectors are learned via artificial neural networks

## Requirements
Python packages that you will need for this project are **scikit-learn, nltk, and gensim**. To install these, simply use the pip installer `sudo pip install X` or, if you are using Anaconda, `conda install X`, where X is the package name.


## Datasets
The IMDB reviews and tweets can be found in the data folder. These have already been divided
into train and test sets.

1. The IMDB dataset, originally found [here][1], that contains 50,000 reviews split evenly into 25k train and 25k test sets. Overall, there are 25k pos and 25k neg reviews. In the labeled train/test sets, a negative review has a score <= 4 out of 10, and a positive review has a score >= 7 out of 10. Thus reviews with more neutral ratings are not included in the train/test sets.

2. The Twitter Dataset, taken from [here][2], contains 900,000 classified tweets split into 750k train and 150k test sets. The overall distribution of labels is balanced (450k pos and 450k neg).

## How to run
`python sentiment.py <folder> <approach>`

1. <folder> can be `data/imdb/` or `data/twitter/` 
2. <approach> can be `0` or `1` as mentioned in approaches.
