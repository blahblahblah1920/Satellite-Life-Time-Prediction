## Satellite Life-time Estimation using Machine Learning Algorithms 📈

This a group project created as a part of **Discovery and Learning with Big Data** course at **University of North Texas** by:           
[Chandrahaas](https://www.linkedin.com/in/chandrahaas-kalanadhabhatla/),
 [Harshini](https://www.linkedin.com/in/harshini-reddy-chada/),
 [Pranav](https://www.linkedin.com/in/pranav-moses-2142b7154/),
 [Siri Chandana](https://www.linkedin.com/in/cheekoti-siri-chandana-6541a419a/)
and Sai Datta

---

**DATA GATHERING**:

The data set used for this was taken from: (https://www.ucsusa.org/resources/satellite-database) , which had a total of 7553 rows and 29 columns, after studying the dataset, we decided to use 11 features that were efficient in predicting the expected lifetime of the satellite.



**PRE-PROCESSING**:

The data had a significant number of null values which were effectively handled either by removing or replacing them. The data had no linear relationship between each features and the distribution of the data was not uniform so, we used Robust Scalar to scale the data. We also used OneHotEncoding to convert categorical values into readable values for the models. After this process, we were left with 4911 rows and 26 columns.



**MODELLING**:

For modelling, we used the following supervised machine learning models:
1.	Linear Regression (RMSE: 1397.29, R2: -400409.34)
2.	Polynomial Regression (RMSE: 4609286.85, R2: -4357111416313.00)
3.	Random Forest Regressor (RMSE: 0.93, R2: 0.82)
4.	Support Vector Machine Regressor (RMSE: 1.59, R2: 0.49)
5.	K-Nearest Neighbour Regressor (RMSE:1.15, R2: 0.73)



**EVALUATION**:

We can see each models performance represented with RMSE and R2 score.
From the above observation we concluded that the linear models displayed their unsuitability for this dataset due to the non-linear nature of the data. The high value for R2 for the RF, SVM and KNN indicates the strong explanatory power of the model. Both RMSE and R2 scores looked promising for the non-linear models.


