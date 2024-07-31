A. The ZIP file contains a Jupyter notebook and an assignment. The tasks performed in the Jupyter notebook are as follows:
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
1.A DataFrame was created using the day.csv file.
2.Seaborn's pairplot was utilized to visualize the data and extract insights.
3.Seaborn's boxplot was employed to visualize categorical variables.
4.Dummy variables for weathersit and season were created using pd.get_dummies.
5.The dteday column was removed due to approximately 306 null values out of 510, and the instant column was dropped as it served only as a record index.
6.The data was split into training and test datasets using train_test_split.
7.Scaling was performed on the training data using MinMaxScaler() with scaler.fit_transform.
8.Correlation was analyzed using sns.heatmap.
9.Training datasets y_train and X_train were created.
10.A constant was added using sm.add_constant, and a model was constructed with sm.OLS(y_train, X_train_sm). The model was then fitted using lr.fit(), and a summary was obtained with lr_model.summary() to retrieve p-values and other statistical information.
11.The Variance Inflation Factor (VIF) was computed using [variance_inflation_factor(X_train.values, i) for i in range(X_train.shape[1])].
12.P-values and VIFs were analyzed to identify and remove unnecessary variables.
13.Predictions were made using lr_model.predict(X_train_sm), residuals were calculated by subtracting y_train_pred from y_train, and a residual analysis was performed using sns.distplot(res).
14.Predictions and evaluations were carried out using the test dataset.
15.Finally, the R-squared score for the test set was compared with the R-squared score for the training set, which was 0.7639, confirming that the model is effective.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
B. Additionally, there is an assignment PDF file in which I have addressed model-related questions and other queries.
