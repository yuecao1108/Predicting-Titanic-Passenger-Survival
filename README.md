# Predicting Titanic Passenger Survival

This is a machine learning project in Python inspired by a Kaggle competition, [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic).

The aim of this project is to utilize machine learning models to predict the survival for Titanic passengers. Since the outcome of interest is binary, the problem at hand is a binary classification task.

To prepare the data for analysis, variables with substantial missing values were excluded, while variables with only slight amounts of missing data were filled in using data imputation methods.

Exploratory data analysis revealed that females had a higher likelihood of survival compared to males, as evidenced by the chart below.

![image](https://user-images.githubusercontent.com/25331292/227840555-210409cd-aadd-4551-a9cf-3f8abcd7d39f.png)

Additionally, a correlation heatmap illustrated that variables such as 'Pclass', 'Sex_Code', and 'FareBin_Code' had higher correlations with the outcome variable 'Survived' than other variables.

![image](https://user-images.githubusercontent.com/25331292/227841015-26cc561a-1479-461c-9e3d-58a6faac7e38.png)

The dataset was then subjected to a Random Forest algorithm, which is an ensemble machine learning method rooted from decision trees. For this classification problem, the output of the Random Forest algorithm was the class selected by the majority of trees. The mean of cross-validated test scores was 81.23%, indicating that the model was able to accurately predict survival outcomes for over 80% of the inputs, based on a 10-fold cross validation result.
