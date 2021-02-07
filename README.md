# Amazon_Vine_Analysis

## Overview of the analysis

The purspose of this analysis was to analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers
and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish
a review.

In this project,  we picked a dataset with customer reviews of our product to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance,
and load the transformed data into pgAdmin. Next, we used PySpark to determine if there is any bias toward favorable reviews from Vine members in our dataset. 
