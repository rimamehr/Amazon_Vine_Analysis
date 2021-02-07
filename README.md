# Amazon_Vine_Analysis

## Overview of the analysis

The purspose of this analysis was to analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers
and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish
a review.

In this project,  we picked a dataset with customer reviews of our product to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance,
and load the transformed data into pgAdmin. Next, we used PySpark to determine if there is any bias toward favorable reviews from Vine members in our dataset. 

## Results 

- We started our analysis with 4,880,466 reviews in our database.
- We then filtered our data to create a DataFrame where there are 20 or more total votes. This narrowed down our count to 107,421.
- We further filtered to create a DataFrame where the percentage of helpful_votes is equal to or greater than 50%. This narrowed down our count to 99,046.
- We then split our DataFrame into two based on if the review was part of the paid vine program or not.
- Our paid vine program DataFrame had 1207 records
- Our unpaid vine program had 97,839 records
- We then counted the number of 5-star reviews for both paid and unpaid program.
- Our final step involved calculating the % of 5-star reviews between the two program.
- Our paid vine program had 509 5-star reviews out of 1207 reviews
- Our unpaid vine program had 45,858 5-star reviews out of 97,839 reivews.

Our Data analysis revealed that;

- Percentage of 5-star reviews for paid Vine program was: 42.170671%
- Percentage of 5-star reviews for unpaid Vine program was: 46.870880%

## Summary

Before our analysis was complete my hypothesis was that a paid vine program would have highest percentage of 5-star reviews but our calculations proved that otherwise. Our unpaid vine program had 46.86% of 5-star reviews in comparison to the paid program that had 42.16%.

We could do some additional filtering of our data and include verified purchase as our criteria to further clean out our data and see if our comparison between paid and unpaid program changes.




