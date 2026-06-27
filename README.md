# Used_Car_Price_Prediction
I have created a Machine Learning model using Random Forest Regression model which predict the price of a used car by its specifications like, model, years used, max power, max torque etc.

Source code - 
The notebook is available in the 'notebook/' folder of this repository.

Google Colab:
https://colab.research.google.com/drive/1Te4sznRmn7JB3zTdAfJ743IJW2n4Hqxs?usp=sharing#scrollTo=zEN7rUsckTc4


Dataset link -
https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho?


Report - 


Title -
Used Car Price Prediction using Random Forest Regression


Problem Statement -
The objective is to predict the selling price of a used car using a Random Forest Regression machine learning model. It helps in determining the best value price for a car based on its model, features etc. It helps both the seller and buyer to get the best price.


Dataset description -
Dataset contains 2059 rows and 20 columns, which means there are 19 features for each car by which we will predict the target column ‘Price’.
It contains different features like model, brand, kilometers driven, max power, max torque, seating capacity etc.


Data preprocessing steps -
We can do 2 things in this -
Remove the null values which will led to remove the rows containing null values.
Change the null values with the median in case of numerical values nd with mode in caseof classified objects.
When I did 1st, it results in deleting around 185 rows that is not appropriate as it will result in deleting the essential data, so I will go with te second method.
I will also check if there’s any duplicate rows in the given dataset
Also the values of Engine, Max Torque nd Max Power is in object type, so I will convert it into float values to enhance my model.


Exploratory Data Analysis -
Firstly, we will analyze the structure nd the data types of all the features given nd analyze where the missing or null values are, what steps we have to take etc.
Before preprocessing, we will analyze the data, that which features contains null values, is there any duplicate row, nd after training the model, what features contribute the most, nd which one the least, etc.


Model used -
I am using Random Forest regression model for this.
Random Forest is an ensemble learning algorithm which use multiple decision trees to mak ethe prediction. Using multiple trees will improve the model nd reduce overfitting which leads to better prediction. Also it works better on regression models that have complex relationships with features.


Training Process -
The dataset is splitted into training nd test dataset using train_test_split() nd will split the data into 80% training data nd 20% test data. Training data would be used to train the model nd then predictions would be made using the test data.



Evaluation metrics nd Results -
The following evaluation metrics were used:
Mean Absolute Error (MAE): 301631.49
Mean Squared Error (MSE): 1269981654709.88
Root Mean Squared Error (RMSE): 1126934.63
R² Score: 0.8182
R² score indicates that the model gives 81.82% of the variation in used car prices, demonstrating good predictive performance. 


Conclusion -
In this Minor project, a machine learning model is made using random Forest Regression.
Dataset was preprcessed by handling the missing values, checking for duplicate rows, cleaning the numerical features, etc. Then dataset is splitted into 2 sets, training nd testing data nd then training the model by training data then predicting the values by test data.
Project demonstrates how machine learning can be used to estimate used car prices accurately based on various vehicle characteristics. 


References-
Scikit-learn Documentation: https://scikit-learn.org/
Pandas Documentation: https://pandas.pydata.org/
NumPy Documentation: https://numpy.org/
Matplotlib Documentation: https://matplotlib.org/
Dataset Source: Dataset Link

Google doc file -
https://docs.google.com/document/d/1V7KXfXo6Om6KsTAAgpX6o1AFGxZWMGz94WwxAJJLZVY/edit?usp=sharing