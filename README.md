# Cardiovascular Risk Prediction
In the given problem statement, we were asked to predict whether the patient has a 10-year risk of future coronary heart disease (CHD and for that, we looked into the heart disease dataset. The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The dataset provides the patients’ information. It includes 3390 records and 17 attributes. There are demographic, behavioural and medical risk factors. From that dataset we derived various insights that helped us know the weightage of each feature and how they are interrelated but our sole aim is to detect whether the person will be affected by a coronary heart problem or not.
## We followed the following sequence of steps to achieve this goal:
* Understanding the dataset, doing some basic inspection on the raw data to check the number of columns, understanding distribution of data and checking statistics of the data in each variable. Checking for and handling missing values, Visualizing the distributions and boxplots of each variable to handle the outliers, Cleaning the data.
* Feature engineering: After getting some insights from the dataset we created some new features, altered the existing features so that they can move forward for the model building phase.
* EDA & Data insight: As mentioned earlier we worked with the heart disease detection dataset and we put out interesting inferences from the data to derive some meaningful results by doing univariate, bivariate and correlation analysis.
* After EDA we to visualize the severity of multicollinearity. Removed multicollinearity based on VIF factor. Scaled the data and started experimenting different algorithms. First, we started with simple models like Logistic Regression and Naïve Bayes algorithm then to enhance the accuracy we tried some complex algorithms too.
* Model building: In this phase, we built our Machine learning model for heart disease detection, evaluated on different metrics compared the results, tuned the hyperparameters of models to get the best performance, we also had a rough idea on feature importance.

## We observed following results after completing the task:
* If we want to completely avoid any situations where the patient has heart disease, a high recall is desired. Whereas if we want to avoid treating a patient with no heart diseases a high precision is desired.
* Assuming that in our case the patients who were incorrectly classified as suffering from heart disease are equally important since they could be indicative of some other ailment, so we want a balance between precision and recall and a high f1 score is desired.
* Since we have added synthetic datapoints to handle the huge class imbalance in training set, the data distribution in train and test are different so the high performance of models in the train set is due to the train-test data distribution mismatch and not due to overfitting.
* We tuned the hyperparameters to get optimal model performance and evaluated the models.Best performance of Models on test data based on evaluation metrics for class 1:
    * Recall – SVC
    * Precision - Naive Bayes Classifier
    * F1 Score - Logistic Regression, XGBoost
    * Accuracy - Naive Bayes Classifier
### Support vector classifier gave the best Recall of 71%.
