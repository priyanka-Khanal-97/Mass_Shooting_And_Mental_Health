# Mass Shooting in United States (1982-2019)

With the increase in mass shooting in United States, there has been a political debate in the country about possible factor in this increased number. Some people argue that the main reason is openly available firearms and some argue that it is because of lack of proper background check. There are several other factors that come into play as well.

For this project, I am mainly focusing on the if the alleged prior mental health signs affect the total number of victims. The dataset used in this project extracted from Mother Jones'. 

Initial exporation and data cleaning was performed in the dataset. The dataset chosen has 110 data entries with total of 24 rows.  6 rows were removed for cleaning purposes because they were never going to use those rows for analysis.

Link of the repository: https://github.com/44-599-machine-learning-S19/machine-learning-project-priyanka-khanal/blob/master/shooting.csv


## Analysis

### Linear Regression

Linear regression was performed on the dataset. Total victims was used as  X and prior_signs_mental_health_issues as Y. The r-sqaured value was wound 0.03 which means the model deosn't fit the data. After adding weapons_obtained_legally as Y the r-sqaured value improved to 0.02. When regression was performed in test set, the r-squared value was 0.01 which is better. The r-squared value was lower but it also might be because the dataset chosen was smaller. 

Link to the repo: https://github.com/44-599-machine-learning-S19/machine-learning-project-priyanka-khanal/blob/master/Linear_regression_shooting.ipynb

### Classification

#### Decision Tree

Decision tree was used for classification of  data. The data set was split in 70% training set and 30% for test set. The training set has and accuracy of 68% whereas the F1-Score is 68%. The test set has the accuracy of 42% whereas the F1-score is 43%. SVM was then used to perform classification.The accuracy of training set is 65% and the F1-score is 58%. The test set has the accuracy of 78% whereas the F1-score is 76%. 

#### SVM Classifier

The accuracy and F1 score using SVM is better than using tree classifier. The accuracy of the test set is 42% using decision tree whereas the accuracy of test set using SVM is 78%. The same way, f1 score using decision tree for the test set is 43% where as f1 score using 76%.

### Clustering

There was no k-means clusters found between the features weapons obtained legally and prior signs of mental health.

Link to Classification and Clustering: https://github.com/44-599-machine-learning-S19/machine-learning-project-priyanka-khanal/blob/master/classification.ipynb

# Conclusion: 

The r-sqaured and MSE of the features were very very low which usually means there is no relationship between total victims and prior signs of mental health. So, blaming the mental health if the shooter is not an appropriate conclusion based on the database.
Along with that, accuracy and F1-score of these features was also not high. This also solidifies the previous conclusion drawn from the linear regression.
One more algorithm was performed in the project which was finding clusters between legal obtaining of weapon and mental health signs. There is no clusters found. This again proves that just blaming mental health of the shooters is not the correct conclusion for blaming this mass shooting.



### References
https://www.motherjones.com/politics/2012/12/mass-shootings-mother-jones-full-data/ 