# Titanic-survival-challenge
Using a dataset with different information about every passenger from the Titanic. I made an AI model which tried to predict whether a certain passenger survived the sinking of the Titanic or not. 
# Cleaning the Dataset
We begin by cleaning the dataset. It is important that all the data in the dataset is represented in an integer so our computer can read it and make accurate mathematical predictions. It is also necessary to scan the data and make sure all data being fed o the computer is relevant to making a prediction. If something is not relevant we can drop the column using the .drop() function which was used with various columns. Most of the data that was dropped was mainly because it included integers along with letters such as the cabin and the ticket number. We also must make sure to get rid of any null values in the datset.
# Analysis
After we have cleaned and simplified the data. We begin to implement our models. In this code, I imported 3 models from scikit learn--LogisticRegression, KNN, and Decision Tree. After a lot of experimentation with the models, I came to the conclusion that Logistic Regression would get me the best accuracy in predicting the survival of different people on the Titanic. However, for a basic model, the decision tree classifier did fairly well in its predictions, scoring an almost identical score to the Logistic Regression, consistently scoring above 80% accuracy.
# Conclusion
Since I used a random_state = None classifier, the results for each run-through were different but the trends were mostly the same. As mentioned before, the Logistic Regression and Decision Tree Classifiers consistently scored with over 80% accuracy on the test set after being trained with the training set. However, the KNN Classifier was consistently in the low 70% range despite changing parameters multiple times. Although an 80% accuracy is not bad, it is not the greatest either. In order to increase the accuracy, we could try various things including, incorporating more data in the training process. Earlier we dropped a lot of aspects of the datasets because it was not in integer form, for example, the cabin. The cabin could be a key part of predicting whether or not the person survived because it indicates their placement on the ship. If I could find a way to convert the cabin to a numerical value and include it in the dataset, I could expect the accuracy to jump for all three models. 

Credits Code inspiration YT: Aladdin Persson https://www.youtube.com/watch?v=pUSi5xexT4Q
