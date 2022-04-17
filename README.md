# Amazon Vine Analysis

## Overview
This repository contains an analysis of Amazon video game reviews written by members of the paid Amazon Vine program. PySpark is used to perform the ETL process on a dataset retrieved from an AWS RDS instance. PySpark analyses were originally conducted within [Google Colab](https://research.google.com/colaboratory/) and the code script is located in the [Amazon_Reviews_ETL.ipynb file](./Amazon_Reviews_ETL.ipynb). Transformed data frames are loaded into pgAdmin. Analysis of Vine reviews were executed in a [second Colab notebook](./Vine_Review_Analysis.ipynb). The following metrics were assessed for both paid and unpaid Vine reviews:
- Total reviews
- Number of 5-star reviews
- Percentage of total reviews that were 5-star

## Results
- <u>Paid Vine Reviews</u>
  - Total reviews: <b>94</b>
  - 5-star reviews: <b>48</b>
  - Percentage of reviews that were 5-stars: <b>51%</b>
- <u>Unpaid Vine Reviews</u>
  - Total reviews: <b>40,471</b>
  - 5-star reviews: <b>15,663</b>
  - Percentage of reviews that were 5-stars: <b>39%</b> 
## Summary
Results of the Vine review analysis suggests that <u>there is a positivity bias in paid Vine reviews </u>. The percentage of paid Vine reviews that were 5-stars is 51% compared to the 39% of unpaid Vine reviews. Granted, the total number of paid reviews (i.e. 94) is dwarfed by the number of unpaid reviews (i.e. 40,471). It's possible that the positivity bias is in part due to the limited sample size of paid reviewers. If the number paid reviews more comparable to the number of unpaid reviews, the difference in percentages may decrease.

To understand if reviews statistics would be more comparable if the sample sizes were similar, an additional analysis could be done where the same statistics were run on a random sample of 150 unpaid Vine reviews instead of the full dataset. Another, more industrious additional analysis could involve running statistics on paid Vine reviews of multiple product categories, not just video games.
## Resources
Data:
- [Amazon Video Game Review Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
    - [Metadata](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
- Software:
  - [Google Colab](https://research.google.com/colaboratory/)
- Scripts
  - [Amazon_Reviews_ETL.ipynb](./Amazon_Reviews_ETL.ipynb)
  - [Vine_Review_Analysis.ipynb](./Vine_Review_Analysis.ipynb)
