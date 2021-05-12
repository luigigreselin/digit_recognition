# Digit Recognition

MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. 
Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. 
In this competition, the goal was to correctly identify digits from a dataset of tens of thousands of handwritten images.

# Statistical analysis with ''traditional'' classifiers

I compared random Nayve Baesyan classifier, logistic regression, KNN, decision tree, SVC, random forest and XGboost.
Logistic regession, SVC, KNN and XGboost required too much time to be trained (Logistic regression failed multiple times to converge), due
to the large anount of features (28*28 pixels per image). Random forest proved to be the best on training dataset, with an accuracy of
96% on the cross validation score.

# Statistical analysis with Keras CNN
I created a CNN composed by two CL and 2 final dense layers. I added then 2 dropout layers inbetween the CL to reduce overfitting. In this
second case I obtained an accuracy of 98.8 in my test dataset.

# Data
Data can be found [here](https://www.kaggle.com/c/digit-recognizer) 