# Project 4 DEND Datalakes

## Description

Sparkify is a music streaming startup with a growing user base and song database.

Their user activity and songs metadata data resides in json files in S3. The goal of the current project is to build an ETL pipeline that extracts their data from S3, processes them using Spark, and loads the data back into S3 as a set of dimensional tables. This will allow their analytics team to continue finding insights in what songs their users are listening to.

## How to run

1. To run this project you will need to fill the following information, and save it as *dl.cfg* in the project root folder.

```

[AWS]
AWS_ACCESS_KEY_ID= 
AWS_SECRET_ACCESS_KEY= 

```


2. Follow the steps:
 
a) Create a S3 Bucket in AWS. Ensure the iam role is created that has full S3 access.
b) Run etl.py from terminal. (A Smaller Data Set can be used to test as it takes a long time to process the data given in Udacity S3)
c) AWS Athena can be used to query the data in the S3 location where the files are created. 


## Structure

This project includes five script files:

- etl.py is reads data from S3, transforms it using Spark and then loads it back to S3.
- dl.cfg has secret key and id of IAM Role that has access to the S3 bucket created.
- README.md is current file.
- test.ipynb is a notebook that you can use to test whether SPARK is able to read a file in S3 location.



# dend-project4
