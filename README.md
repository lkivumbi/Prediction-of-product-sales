___
# Prediction-of-product-sales
___
## Item sales for a particular product in a particular store given different features
___
## Author `LUKE KIVUMBI`
## Business Problem:
The goal of this project was to predict the sales of a given item in a particular store given the following features
1. Product ID
2. weight of the product
3. Fat content
4. Item visibility in the store
5. Item category
6. Maximum retail price of the product
7. store ID &
8. Outlet type

## Data:
This dataset had twelve features including our target and 8523 entries with some missing value. The data is a mixture of float and object datatypes
# Method
___
1. This data was first checked for duplicates and null values so as to enable cleaning and preparation for Machine Learning.
2. The data was also checked for inconsistent values and wrong datatypes which were identified and corrected.
3. custom Exploratory Data Analysis functions were used to to do Exploratory Data Analysis and visualisation of the features.
4. Further the preprocessing object was identified for each class: numeric, ordinal and nominal and taken through a model pipeline where a linear regression model was used at first.
5. the second model chosen was a Random Forest Regression which was modified using GridSearchCV to identify the best version

# Results
___
 Preview 
- Heatmap of correlation relationship between numerical features in the data


![readme2](https://github.com/lkivumbi/Prediction-of-product-sales/assets/161327455/7ccdbf7f-ceba-48df-9296-ebfba95c842e)



- Barplot of Item Identifier on Item Outlet Sales colored according to Outlet size


![outlet indentifier](https://github.com/lkivumbi/Prediction-of-product-sales/assets/161327455/338be1a2-2999-4a26-8ea5-68ffb8bd3a92)

# Model
- The final model chosen for this project was a Random Forest Regressor after doing a Gridsearch of the best parameters and using the best estimators on the dataset.
- The best parameters identified were
-- max_features: 3
-- min_samples_leaf: 2
-- n_estimators: 500

- Thees parameters when used with our Random Forest Model gave the best predictions when fit on the training and test set. the resultant model was not over fit and gave the best balance with bias as compared to the default Random Forest Regression and or the linear model.
- The r2 score of the training data came in at 0.77 and that of the test data came in at 0.568.
- The Mean Squared error for this model was also the lowest amongest the model tried.
- This model therefore proved to be the best predictor of the target as it would give the most correct predictions and even where it fell off, it wouldn't be as bad as the other models.

# Recommendations:
___
I would recommend that focus would be put on the Item Maximum retail price as this showed the greatest positive correlation with item outlet sales and also focus to be put on the item visibility as it also showed some negative relationship with the outlet sales.

# Limitations and next Step
___
The dictionary wasn't descriptive enough and the missing values were not explained well to determing the best way to deal with them.

## For further information
For any additional questions, please contact me @kivumbimluke@gmail.com
