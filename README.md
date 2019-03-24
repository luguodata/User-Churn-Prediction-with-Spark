# Sparkify-Project---User-Churn-Prediction
This project is about building a churn prediction model on Sparkify, a Digital
music service, like Spotify or Pandora. Spark on AWS EMR cluster will be used to
manipulate the large user log information and build machine learning models.


This project is from Udacity Data Science Nano-Degree. Full raw data is about 12 GB.

## Project Outline

* Data Exploratory and Model Constructing in a small Subset. <br>
`1.` Load and Clean Dataset <br>
`2.` Feature Engineering. <br>
`3.` Build Data Processing and ML Pipeline. <br>
`4.` Model Training and Prediction

* Run compiled data processing scripts on AWS EMR cluster with full size dataset.


## Files
Sparkify_Exploratary.ipynb -- Data Exploratory and Scripts Constructing on a small subset.
Sparkify_Scripts.ipynb -- Scripts of data Loading, feature processing and model predition on AWS EMR cluster.

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
