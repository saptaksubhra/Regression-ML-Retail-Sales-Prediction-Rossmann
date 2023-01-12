# Regression-ML-Retail-Sales-Prediction-Rossmann
Regression ML Project

![image](https://user-images.githubusercontent.com/95517916/209662166-bf1d0ebb-4a17-4d5f-9cd2-06467364a8e6.png)

📖 Introduction :

A major challenge for large retailers is to address the reqirements of the consumers more effectively on a local level, while maintaining the efficiencies of central distribution simultaneously. As the demand for mass customization by consumers grows, methods focused on store level optimization increase in value. Prediction of sales is an important implementation of machine learning in the retail space. Given accurate predictions, retailers can manage dynamic pricing, staff rostering and inventory so as to maximize profit and improve the customers' experience.

An accurate forecast of sales allows retail outlets to answer questions such as:

* Can we use dynamic pricing to maximize our profit?
* Do we have enough stock to satisfy demand without being overstocked?
* What are the most important factors that affect sales, and how can we optimize them?

📖 Approaches Used :

* Loading our dataset and importing all the useful libraries : We have two datasets. One is Sales dataset and other is Stores dataset. Loading of those two datasets with proper commands and importing required libraries to perform various operations have been executed at the outset of the project.

* Data preprocessing and Feature Engineering : Lot of techniques ( Such as : describe, info, unique values and many more ) havee been applied to get the ins of outs from both (Sales and Stores ) datasets as far as the data preprocessing is concerned. As to Feature Engineering, handling outliers, handling and counting of missing values have been accomplished in case of both Sales and Stores datasets.

* Scaling numeric features to a (0,1) range : Some features are converted into boolean numbers. For example, 'StateHoliday' column has been converted into Boolean variable in Sales dataset. The value of type a, b , c are converted into 1 and others into 0.

* Date Extraction : There is a need to extract 'Date' column in Sales dataset. So, 'Date' column has been extracted into 'Day', 'Month', 'Year', 'Week', 'Quarter', 'WeekOfYear'. Now, as 'Date' column has been extracted, so, there is no need of 'Date' column and it has been deleted from Sales dataset.

* Exploratory Data Analysis (On Individual Datasets and Merged Dataset) : EDA analysis has been performed on various features throuh beautiful data visualizations. Libraries like Seaborn , Matplotlib have been utilised for better data visualizations. Various plots or graphs have been used. Barplot, histplot, violinplot, boxplot, pairplot, distribution plot, jointplot are the examples of different data visualization graphs to describe correlations between different features. Such as : 'Sales vs SchoolHoliday', 'Sales vs Promo', 'Customers vs Promo', 'Customers vs StateHoliday', 'Sales vs StateHoliday', 'Customers vs SchoolHoliday', 'Sales vs Assortment', 'Sales vs StoreType' and many more. 

* Merging of Datasets : Both Sales and Stores datset have been merged for the sake better analysis and visualizations. Another EDA has been perfromed for better satisfaction and implenetation of different ML models on merged dataset. Some specific categorical variables will be analyzed with the target variable 'Sales'.

* Feature Selection of Regression Models : There are various factors while performing feature selection of regression models. This project is based on regression which is a parametric approach. So there are various things to keep in mind. Those are :
There should be a linear and additive relationship between dependent and independent variables. 
There should be no correlation between residual terms.

* One Hot Encoding : One hot encoding algorithm is an encoding system of Sci-kit learn library. It is used to convert numerical categorical variables into binary vectors. Before applying this algorithm we need to be sure that the categorical values must be label encoded as one hot encoding takes only numerical categorical values. One Hot Encoding has been applied in the merged dataset here by get_dummies method. 

* Machine Learning Data Modeling ( For Prediction ) : For prediction some additional steps have been executed in connection with ML data modeling. Those are :
Correlation Heatmap
Correlation Matrix : Correlation is a statistical term used to measure the degree in which two variables move in relation to each other. A perfect positive correlation means that the correlation coefficient is exactly 1. This implies that as one variable moves, either up or down, the other moves in the same direction. A perfect negative correlation means that two variables move in opposite directions, while a zero correlation implies no linear relationship at all. This correlation heatmap is here to visualize correlation amongst variables.

Selection and Final selection of Independent Variables : The selection of independent variables has been done prior to model building based on regression algorithms.

Train-Test Split: Here, the merged dataset has been split into training and testing dataset. The model has been trained with the help of training set and then testing set has been used to test or evaluate the model.

* Importance of Features : The importance of features in the merged dataset has been calculated here. 'Customers' is found out to be the most important feature with almost 72% of share of importance.

* Calculation of Train Score and Test Score : Train score and test score of different regression models have been calculated in this section. Out of these regression methods, Random Forest proved to be the most accurate, achieving a R2_Score of 0.968566, MAE of 2.0359620872115216. MSE of 7.6529574439377015 and RMSE of 2.7663979185825203.

📖 Algorithms Used :

* Linear Regression

* Lasso Regression or L1 Regularization

* Ridge Regression or L2 Regularization

* Elastic Net Regression

* Decision Tree Regressor

* Random Forest Regressor

* XGBoost Regressor

* AdaBoost Regressor

* GradientBoost Regressor
