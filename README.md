# CreditCardFraud-KNN_Tree_Classification-
Data link: https://www.kaggle.com/mlg-ulb/creditcardfraud
In this project we classify whether or not a given transaction is fraudulent or not. Credit fraud is a big problem in the modern world, and many banks have come up with programs to immediately detect if a given transaction is fraudulent.

The original dataset contained 284,807  instances with 28 columns labeled V1-V28. Of these 284,807 instances, 492 were fraudulent. The original column names contained classified information, which is why they have been given generic names. Each field will be used to help us determine whether the transaction represented was fraudulent or not.

Every column’s data type is a 64-bit float, except the “Class” column, which only contains binary integers (1 or 0).

We utilized both a Decision Tree Classifier and a K-Nearest Neighbors algorithm to interpret our dataset. With the Decision Tree Classifier, we split the 284,807 instances into  80-20% training to test and and 60-40% training to test set.

Due to the large imbalance of positive and negative instances, it was necessary to utilize a 60-40 train/test split to upscale the amount of fraudulent instances in our test set. 

80/20 accuracy = 99.89 | 60/40 accuracy = 99.99

When utilizing the 60/40 split on a Decision Tree Classifier, our test set accuracy was 99.992%. The confusion matrix of our test results showed that our model only predicted 57 cases out of 56,962 wrong.

We also ran a K-Nearest Neighbors algorithm on our dataset, and got worse results, with only 99.833% accuracy, which is a significant difference when you consider the size of our dataset. 

In conclusion, both our Tree Classifier and K-Nearest Neighbors models seem to do a good job of detecting fraudulent transactions given our high accuracy metrics. Therefore, we can conclude that the predictors in our model (V1-V28) do a decent job of detecting fraudulent transactions.
