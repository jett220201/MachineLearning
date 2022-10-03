# Classification of survivors of the Titanic accident by age, gender and class on the ship

## By: Juan Esteban Torres Tamayo

## Dataset available in:  https://www.kaggle.com/c/titanic

## Description: 
Testing and performance comparison between 3 Machine Learning classifiers: Logistic Regression (LR), K nearest neighbors (KNN) and Support Vector Machine (SVM) for the problem of determining the survival of a person in the Titanic accident from his age, gender and the class in which the person travels by ship. 

For the adequacy of the Dataset we analyzed the empty data (NaN) and its feasibility of elimination, determining that it was not a good practice, I opted for the filling of these (Age). Given that the standard deviation of this variable is very high, two options were formulated: to use the mean despite the risk due to the standard deviation, or to perform a regression using a trained percetron with the other age data.

For its development, Hold-Out validation is used and an iteration of hyperparameters is performed until the best combination of these is obtained according to the Matthews Correlation Coefficient (MCC) metric.

*ToDo:
- Include more features as number of siblings (SibSp) or fare (Fare).
