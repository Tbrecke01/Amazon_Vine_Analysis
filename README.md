# Amazon_Vine_Analysis

## Overview
The purpose of this project wast to use Google collab, PySpark, Postgres/PgAdmin and SQL to analyze customer reviews from Amazon's Vine Program, a service that pays individuals to review certain products, to determine if there is a bias between paid Vine members and unpaid non-members. I chose to focus my analysis on reviews in the 'electronics' category, whose reviews had 20+ votes and were 50%+ 'helpful' in nature. I then calculated the total number of reviews, and the total number of 5 star reviews for Vine and non-Vine members.

## Results
With over 3M reviews recorded, I first filtered the list down to a more manageable number. I did this by filtering the list down to those revies who had 20+ ratings, and where over 50% of the ratings indicated the review had been 'helpful' which led to the below list (by review ID):
![Review_ID](https://github.com/Tbrecke01/Amazon_Vine_Analysis/blob/main/Images/review_id_df.png)
 
From here, I divided the list between Vine and non-Vine reviews, the total number of 5-star reviews, and the calculated the percent of 5-star reviews for each Vine and non-Vine members. This showed the following results:
![Vine_vs_nonVine](https://github.com/Tbrecke01/Amazon_Vine_Analysis/blob/main/Images/vine_review_compare.png)
 
From this we can see that the vast majority of reviews(~50k non-Vine vs ~450 Vine) are posted by non-vine members and that, while Vine does tend to have slightly more 5-star reviews than non-Vine members (46% for Vine vs 42% for non-Vine), the number is far from substantial and can be explained by the sheer size discrepency between the two groups causing Vine reviews to be artificially inflated.
    
## Summary
From the data above it can be concluded that there is a minor to no preference for 5-star reviews between Vine and non-Vine members. However that is not to say that no bias exists between the groups. To accurately determine this, I would recommend further analysis to determine which group submits more positive reviews (say 3 or 4 star reviews and up) than the other, and additional analysis across all product segments, not just electronics.
