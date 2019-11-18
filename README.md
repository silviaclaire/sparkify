# Using Spark to Predict Churn
A binary classification problem solved with Spark and Spark's MLlib.
[Medium Post](https://medium.com/@claireyan/using-spark-to-predict-churn-c69e675272bf)

## Project Motivation
This project serves as an exploration of how to make a churn-prediction model using Spark, with the following steps included:

- explore and manipulate our dataset
- engineer relevant features for our problem
- split data into train and test sets by sampling churn
- build binary classifier models with Spark’s DataFrame-based MLlib
- select and fine-tune the final model with Spark’s ML Pipelines and a StratifiedCrossValidator

## Dependencies
- python==3.7.3
- pyspark==2.4.4
- spark-stratifier==0.1.5
- numpy
- pandas
- matplotlib
- seaborn
- jupyterlab

## Files Explanation
- Sparkify.ipynb
  - A notebook contains all the analysis codes.
- requirements.txt
  - A file specifies what python packages are required to run this project.
- .gitignore
  - A file tells git which files/patterns it should ignore.

## Analysis Results
- Best model: `LogisticRegression(msxIter=10)`
- Best f1-score: 0.75 among 62 test samples
- Top feature importances:
  - days after registration
  - setting-checking events per hour
  - upgrade-related events per hour
  - ads watched per hour
  - songs played per hour
