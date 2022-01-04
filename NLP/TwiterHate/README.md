# Twitter Combat Hate Speech Using NLP and Machine Learning

Dataset Details: 
Attached

id: identifier number of the tweet
Label: 0 (non-hate) /1 (hate)
Tweet: the text in the tweet


DESCRIPTION
Using NLP and ML, make a model to identify hate speech (racist or sexist tweets) in Twitter.

Problem Statement:  
Twitter is the biggest platform where anybody and everybody can have their views heard. Some of these voices spread hate and negativity. Twitter is wary of its platform being used as a medium  to spread hate. 

You are a data scientist at Twitter, and you will help Twitter in identifying the tweets with hate speech and removing them from the platform. You will use NLP techniques, perform specific cleanup for tweets data, and make a robust model.

Domain: Social Media

Analysis done: Clean up tweets and build a classification model by using NLP techniques, cleanup specific for tweets data, regularisation and hyper-parameter tuning using stratified k-fold and cross validation to get the best model.

Steps Performed:

1. Tweets into a list for easy text cleanup and manipulation.
2. Cleanup: 
	a. Normalize the casing.
	b. Using regular expressions, user handles are removed which begins with '@’.
	c. Using regular expressions to remove URLs.
	d. Using TweetTokenizer from NLTK to tokenize the tweets into individual terms.
	e. Remove stop words and ‘#’ symbols from the tweet while retaining the term.
	f. Extra cleanup by removing terms with a length of 1.

3. Perform train_test_split using sklearn.
4. Using TF-IDF values for the terms as a feature to get into a vector space model.
5. Logistic Regression from sklearn with default parameters.
6. Model evaluation: Accuracy, recall, and f_1 score.
7. Adjust the appropriate class in the LogisticRegression model.
8. Evaluate the predictions on the train set: accuracy, recall, and f_1 score.
9. GridSearch and StratifiedKFold because of class imbalance.
10. Predict and evaluate using the best estimator.
