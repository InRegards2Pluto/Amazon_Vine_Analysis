# Amazon Vine Analysis

## Overview
This analysis is part of a mock analysis of Amazon video game reviews written by members of the paid Amazon Vine program. PySpark is used to perform the ETL process on a dataset retrieved from an AWS RDS instance. PySpark analyses were originally conducted within Google Colab. Transformed data frames are loaded into pgAdmin.The following metrics were assessed for both paid and unpaid Vine reviews:
- Total reviews
- Number of 5-star reviews
- Percentage of total reviews that were 5-star

## Results
- Paid Vine Reviews
  - Total reviews: <b>94</b>
  - 5-star reviews: <b>48</b>
  - Percentage of reviews that were 5-stars: <b>51%</b>
- Unpaid Vine Reviews
  - Total reviews: <b>40,471</b>
  - 5-star reviews: <b>15,663</b>
  - Percentage of reviews that were 5-stars: <b>39%</b> 
## Summary
## Resources
Data:
- [Amazon Video Game Review Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
    - [Metadata](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
- Software:
  - [Google Colab](https://research.google.com/colaboratory/)
- Scripts
  - [Amazon_Reviews_ETL.ipynb](./Amazon_Reviews_ETL.ipynb)
  - [Vine_Review_Analysis.ipynb](./Vine_Review_Analysis.ipynb)
