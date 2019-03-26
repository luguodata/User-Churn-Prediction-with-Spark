# User Churn Prediction with Spark

# Sparkify Project


**Project Overview:**  <br>
This project is about building a churn prediction model on Sparkify, a Digital music service, like Spotify or Pandora. Spark will be used to manipulate the user log information ,do data exploratory and build machine learning models for predict monthly churn.

A subset of full data will be used for this analysis.

**Project Purpose:**  <br>
Churn prevention is a hot and challenging problem in almost every product and service company. If the risk of users disconnecting service could be predicted, then company could take actions to save customers before they leaving. In this sepecific case for Sparkify, what I do is to predict users at risk to cancel their services or downgrading from premium to free tier altogether. More sepecifically, I will use the monthly user-product interations along with user demographic information to predict next month churn. If we could get good model performance and make it into production, company would benefit a lot.

**Project Evaluation**  <br>
Since customer churn or not is a binary outcome, the classification models will be built on the processed dataset.
Churn or stay group is imblanced, F1 score, AUC score will be as the evalution metrics inteading of accuracy.



## Project Outline

`1.` Load and Clean Dataset <br>
`2.` Feature Engineering. <br>
`3.` Build Data Processing and ML Pipeline. <br>
`4.` Model Training and Prediction


## Files
Churn_Prediction_with_Spark.ipynb -- Data Exploratory and Model Constructing on a small subset.


## Project Results

In this project, digital music service user log data has been explicitly explored by using Spark. A lot work been done such as data cleaning, churn defining, data transformation, exploratory between churn/stay groups. At last, we built data processing and machine learning piplines. Using several algorithms and parameter tuning to train churn model and got fine predicted results on test set. Finally, we got pretty good model performance. The AUC score of random forest and Logistic Regression predictions on test set are both above 0.8.  F1 score of logistic Regression is abot 0.91. However, due to the limited size of this dataset , the result might be unstable if we change train, test dataset.

* Ways to Improve
1. Re-analyze the whole process on the full size dataset. The whole dataset user log scenario might be very different with the small one.
2. Set spark cluster on AWS EMR, which allow to access the full dataset in S3 and alos could boost calculation speed.
3. Continue to extract more useful features and try more algorithms and parameter tunings.


## Blog Post

I posted the whole analysis process into Medium. Link is here:
https://medium.com/@lguodata/user-churn-prediction-with-spark-a2e6abb39fb


## Required packages
`pyspark` <br>
`pandas` <br>
`numpy` <br>
`datetime` <br>
`matplotlib` <br>
`seaborn` <br>



## Reference
Level changes for each user along time: <br>
 https://fle.github.io/detect-value-changes-between-successive-lines-with-postgresql.html <br>
Replace space in column names with _ : <br> https://stackoverflow.com/questions/41655158/dynamically-rename-multiple-columns-in-pyspark-dataframe <br>
Proportion distributions of a variable: <br>
https://stackoverflow.com/questions/1823599/calculating-percentage-within-a-group <br>
Data processing and ML Pipeline building: <br>
https://docs.databricks.com/spark/latest/mllib/binary-classification-mllib-pipelines.html <br>
https://blog.usejournal.com/tutorial-on-pyspark-transformations-and-mlib-7ed289a9e843 <br>

Setting up spark cluster on AWS EMR: <br>
https://www.perfectlyrandom.org/2018/08/11/setup-spark-cluster-on-aws-emr/
