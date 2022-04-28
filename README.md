# House_Price_Prediction (Using XGBoost Regression) 

### Problem Statement: 
In this project, we will evaluate the performance and predictive power of a model that has been trained and tested on data collected from homes.  A XGBoost regression model trained on this data that is seen as a good fit could then be used to make certain predictions about a home's monetary value.

### About Dataset
This dataset is imported from sklearn. The dataset consists of 506 observations and 14 variables. 

### Data Exploration:
- After checking first few rows of the data and shape, I did statistical measurement on the data.
- Before applying any machine learning model, it is important to remove or impute NA values, So I checked NA  values but this dataset does'nt have any NA values.


### Feature Observation:

To dive a bit deeper int our data, we are using three features from the dataset: 'RM', 'LSTAT', and 'PTRATIO'. For each data point (neighborhood):

'RM' is the average number of rooms among homes in the neighborhood.

'LSTAT' is the percentage of homeowners in the neighborhood considered "lower class" (working poor).

'PTRATIO' is the ratio of students to teachers in primary and secondary schools in the neighborhood.

Without building a model, let's try to figure out if an increase in the value of a feature would lead to an increase in the value of 'price' or a decrease in the value of 'price'.

'RM': An increase in the value of this feature will lead to an increase in the value of 'price'. This is because for you'd expect a home with a higher number of rooms to be more expensive that a home with lower number of rooms.

'LSTAT': An increase in the value of this feature will lead to a decrease in the value of 'price'. A lower class homeowner might not be able to afford expensive houses, so you'd expect them to leave in a cheaper home. A higher percentage of such people could correlate to cheaper homes in an area, and thus, a lower 'price' value.

'PTRATIO': An increase in the value of this feature will lead to an decrease in the value of 'price'. A low student to teacher ration is typically associated with better education level of a school, as a teacher is able to focus on individual students better (than if there were more students). So, due to the presence of better quality schools, people might be willing to pay more to live in those areas, to provide their children with better education, and the prices might be higher.

I built scatterplots to see if my intuition is correct.

