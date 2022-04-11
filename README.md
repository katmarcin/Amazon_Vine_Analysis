# Amazon_Vine_Analysis

## Overview of the Analysis

The purpose of this analysis is to analyze Amazon reviews written by members of a paid Amazon Vine program in order to determine if there is any bias toward favorable reviews from Vine members towards beauty products.  The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. PySpark was used to intitiate and perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. We used PySpar, again to determine if there is any bias toward favorable reviews from Vine members in the dataset. Ultimately, the goal is to determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.


### Data-source:

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Beauty_v1_00.tsv.gz

### Tools:

Amazon Web Services (AWS), S3, RDS, Google Colab, Apache Spark, PySpark Machine Learning (ML) library, mrjob library, pgAdmin, PostgreSQL, SQL language


## Results


Results: Using bulleted lists and images of DataFrames as support, address the following questions:

How many Vine reviews and non-Vine reviews were there?
How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

<img src=“https://github.com/katmarcin/Amazon_Vine_Analysis/blob/77eee94897700251c90d71576548c239183b9361/images/Screen%20Shot%202022-04-10%20at%2011.50.47%20PM.png" width="350" height="320"/>

<img src="https://github.com/katmarcin/MechaCar_Statistical_Analysis/blob/8d842ea7cae9d201f0605488c1ef41b1533ed108/images/ttest_all.png" width="350" height="250"/>

<img src=“https://github.com/katmarcin/Amazon_Vine_Analysis/blob/77eee94897700251c90d71576548c239183b9361/images/Screen%20Shot%202022-04-10%20at%2011.50.55%20PM.png">

<img src=“https://github.com/katmarcin/Amazon_Vine_Analysis/blob/77eee94897700251c90d71576548c239183b9361/images/Screen%20Shot%202022-04-10%20at%2011.51.10%20PM.png" height="320"/>

There is a bulleted list that addresses the three questions for unpaid and paid program reviews (7 pt

## Summary


Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

The summary states whether or not there is bias, and the results support this statement 
An additional analysis is recommended to support the statement 
