# Amazon Vine Analysis

## Overview
* The purpose of this project to to analyze reviews written by members of the Amazon Vine Program. Specifically, we will try to determine if there is evidence of bias towards favorable reviews by Vine members for SellBy, a company that sells on Amazon. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

## Resources
* Data source: amazon_reviews_us_Automotive_v1_00.tsv.gz
* Software: PySpark, PostgreSQL 11.16, Amazon AWS, Amazon S3

## Results
* We determined that there were a total of 3,514,942 total reviews in our dataset. Of these reviews, Amazon Vine members only account for 5,925 of these reviews. The vast majority of reviews are provided by non-Vine users who account for 3,508,784.
* ![total_reviews](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/total_reviews.png)
* ![total_vine_reviews](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/total_vine_reviews.png)
* ![total_non_vine_reviews](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/total_non_vine_reviews.png)

* Additionally, we calculated the total number of 5 Star reviews, the highest possible rating. There was a total of 2,300,587 5 star reviews out of the 3,514,942 total reviews. Vine members produced 2,743 5 star reviews where as non-Vine users produced 2,297,844. 
* ![total_5star_reviews](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/total_5star_reviews.png)
* ![vine_5star_reviews](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/vine_5star_reviews.png)
* ![non_vine_5star_reviews](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/non_vine_5star_reviews.png)

* What we were able to determine from this analysis is that Amazon Vine members gave a 5 star rating 46.3% of the time and non-Vine users gave 5 star ratings 65.49% of the time.
* ![vine_5star_percent](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/vine_5star_percent.png)
* ![non_vine_5star_percent](https://github.com/BryantKlewer/Amazon_Vine_Analysis/blob/main/Screen_shots/non_vine_5star_percent.png)

## Summary

### Positivity bias?
* From the data gathered, it is not indicated that there is a bias towards positivity in the reviews in this data set. As shown in the results of the analysis, only 46.3% of Amazon Vine members gave a 5 star review where as 65.49% of non-Vine users gave a 5 star review. What the data indicates is actually the opposite, it stands to reason that Vine members may actually hold a higher standard for their products and therefore may be harsher in their reviews.

### Recommendations
* Further analysis of the Vine program would be recommended in order to determine if there are similar findings. Only one of fifty product categories' data was utilized during this analysis. Given enough time and resources, it would be recommended to replicate this analysis at scale for the additional 49 categories. At a minimum, a random sampling of at least 50% of the product categories should be completed. Furthermore, including 4 star reviews in the analysis could be another alternative in order to determine if they have bearing on overall positivity bias. 
