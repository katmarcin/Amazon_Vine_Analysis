# Amazon_Vine_Analysis

## Overview of the Analysis

The purpose of this project is to analyze Amazon reviews written by members of a paid Amazon Vine program and unpaid reviewers in order to determine if there is any bias toward favorable reviews. Specifically, the dataset we used contains reviews on products categorized into "beauty". The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. 
As part of the ETL process, PySpark was used to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. We are then able to determine if there is any bias toward favorable reviews from Vine members in the dataset and if having a paid Vine review makes a difference in the percentage of 5-star reviews.


### Data-source:

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Beauty_v1_00.tsv.gz

### Tools:

Amazon Web Services (AWS), S3, RDS, Google Colab, Apache Spark, PySpark Machine Learning (ML) library, mrjob library, pgAdmin, PostgreSQL, SQL language


## Results

* Paid Vine Program

  * 647 total reviews
  * 229 5-star reviews
  * 35.4% of vine reviews were 5-star

* Unpaid Reviews (non-Vine Program)

  * 74,113 total reviews
  * 43,217 5-star reviews
  * 58.3% of unpaid reviews were 5-star

* How many Vine reviews and non-Vine reviews were there?

<img src="images/Screen Shot 2022-04-10 at 11.50.47 PM.png" alt="Alt text" title="Optional title" width="500" height="250"/>

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

<img src="images/Screen Shot 2022-04-10 at 11.50.55 PM.png" alt="Alt text" title="Optional title" width="500" height="250"/>

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

<img src="images/Screen Shot 2022-04-11 at 12.13.57 AM.png" alt="Alt text" title="Optional title" width="500" height="250"/>


## Summary


Made evident by our last result, there isn't a positivity bias for reviewers in the Vine program. 58% of unpaid reviewers gave 5-star reviews and only 35% of paid reviewers gave positive ratings. This might indicate that paid reviewers take their critiquing more seriously and unpaid reviewers might not be doing in-depth analyses on their own reviews. It is worth noting that there are far less Vine reviewers than regular non-Vine reviewers so there might not be enough data to solidify this claim. However, if we were to perform an additional analysis to support the statement, it would be beneficial to examine the distirubution of star-ratings amongst the two groups to see if there are any trends worth noting. This can be done by running a measure of central tendency on only star-rating column in our table. By doing so, we can see the most common rating (mode) and the average rating (mean) for the dataset. This would support our statement in that there isn't any positivity bias from reviewers in the Vine program. From a business standpoint, it might not be useful at all for a company such asSellBy

Made evident by our last result, there isn't a positivity bias for reviewers in the Vine program. 58% of unpaid reviewers gave 5-star reviews and only 35% of paid reviewers gave positive ratings. This might indicate that paid reviewers take their critiquing more seriously and unpaid reviewers might not be doing in-depth analyses on their own reviews. It is worth noting that there are far less Vine reviewers than regular non-Vine reviewers so there might not be enough data to solidify this claim. However, if we were to perform an additional analysis to support the statement, it would be beneficial to examine the distribution of star-ratings amongst the two groups to see if there are any trends worth noting. This can be done by running a measure of central tendency on only star-rating column in our table. By doing so, we can see the most common rating (mode) and the average rating (mean) for the dataset. This would support our statement in that there isn't any positivity bias from reviewers in the Vine program. From a business standpoint, it might not be useful for a company to invest in and use Amazon Vine's services if their goal is to encourage positive reviews. Nonetheless, from a data science standpoint, it would be more beneficial to collect more data on reviewers before drawing bias conclusions.
