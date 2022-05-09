# Amazon_Vine_Analysis
#### *Analysis on Amazon's vine review program using PySpark and AWS RDS with PostgreSQL*

## Overview

Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

##Background
*US Apparel product reviews* from Amazon was used in this project. The goal: to analyze if it would be worth it to subscribe to a Vine program if we were to sell similar products through their platform. The vine review program is an incentive model in which customers are gifted free gifts to write good reviews. PySpark was used to extract, transform, and load (ETL) the data to a AWS *RDS* created and connected to a PostgreSQL server to be able to query it and extract finished tables from there. Pandas was used to further manipulate the data to extract information. 



## Resources
- Datasets:
  - [US Apparel dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

- Technologies used:
  - Google Colab (to run PySpark)
  - Jupyter Notebook
  - AWS S3 and RDS 
  - PostgreSQL


## Results
- Paid Vine Program
  - 33 total reviews
  - 15 5-star reviews
  - ***45.5%*** of vine reviews were 5-star

- Unpaid reviews
  - 45,388 total reviews
  - 23,733 5-star reviews
  - ***52.3%*** of unpaid reviews were 5-star


## Summary

In conclusion, the vine program might not be worth it for the apparel category. There weren't many helpful reviews that made part of it (total of 33), and only around half of them were 5-star rated (45%) which was similar to unpaid reviews (52%). Even though the percentages may be misleading as the volume of reviews in the vine and non-vine programs are very different, this itself is a sign that the vine program is not very popular in this category. It may not be worth paying for incentivizing the people to write better reviews. 

Further analysis got the average star rating for vine and non-vine reviews (4.09, 3.87 respectively). While 5 stars is much more desired, psycologically 4 is acceptable while the 3 range is not. Maybe further incentives to get more people to give higher reviews may be worth it from that standpoint, put a cost-benefit analysis is needed to determine if it truly is worth it the cost to profit potential. 



