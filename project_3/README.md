# Josh Slizinov Project 3

## Problem statement

Something is wrong with the reddit servers. New posts are being posted to random subreddits! Until the servers are fixed, reddit employees have to manually direct posts to the correct subreddit! It’s taking too long! I’ve decided to offer my pro-bono services to reddit in exchange for a data science job upon graduation.

Model success will be evaluated using accuracy score.

## Description of data

The primary data used for the modeling in this project is 10000 rows × 11651 columns. The columns all represent words in the respective document. The only column I added was 'from_sub' which represents teh subreddit from which the text came from.


## Model performance on training/test data

I fit 2 total models: Random Forest Classifier and KNNClassifier. Their respective accuracy scores were as follows:

Random Forest training: 0.9148
Random Forest testing: 0.902

KNN training: 0.9244
KNN testing: 0.8612


The model that will be used is the Random Forest model because it has the highest accuracy on the test set and does not seem to be overfit on the train set.


## Primary findings/conclusions/recommendations

I found that a random forest classifier model and a knn calssifier model can predict the subreddit which text belongs to very well. The top word analysis was very helpful in distinguishing whether or not this model would be successful. Something to consider is that two subreddits with very similar top words may notbe classified as well. The sentiment analysis that was doen for this project was either kind of useless or I was not able to find an appropriate use for it.

Because this random forest model IS able to predict, with high accuracy, the classification of subreddit posts based on text, I recommend that reddit employees use this model to assist them in classifying their subreddit posts until they can fix their servers.


## Next steps

The random forest model already has a very high accuracy, but something that could be improved is more feature engineering, better outlier maintenance, and more narrowed down features. Additionally, I would like to test more models and use GridSearch to tune the models. Finally, testing the model on 2 similar subreddits or multiple subreddits would really put it to the test.

Thanks for reading!