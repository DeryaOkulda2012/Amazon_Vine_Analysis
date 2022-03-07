# Amazon_Vine_Analysis

## Overview

### Analyzing Amazon reviews written by members of the paid Amazon Vine program.

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I picked the Amazon dataset for toys, then performed ETL on this data using AWS, Google Colaboratory, PostgreSQL, and PySpark. After that, I took a closer look at one of the tables made during the ETL phase regarding the vine reviews to determine if there was any bias for positivity in the reviews in the Vine Program.

## Results

The Toys product category data set was used for this analysis.

There were 1,266 Vine (Paid) reviews and 62,028 non-vine reviews for a total of 63,294 reviews.
- Total Vine reviews: 1,266
- Total non-Vine reviews: 62,028

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- 5-star Vine reviews: 432
- 5-star non-Vine reviews: 29,982

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- % of 5-star Vine reviews: 34.12322%
- % of 5-star Non-Vine reviews: 48.33624%

- % of all reviews that were 5-star: 48.05195%

The table below shows the results of the analysis:

| | Paid Review (Vine) | Unpaid Review (Not Vine) | Total |
| ------------: | -------------: | ------------: | ------------: |
| 5 Star | 432  | 29,982 |  30,414 |
| Less than 5 Star | 834 | 32,046 | 32,880 |
| Total  | 1,266 | 62,028 | 63,294 |
| 5-Star Percentage | 34.12% | 48.34% | 48.05% |



