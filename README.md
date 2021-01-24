# Amazon Vine Analysis

## Overview

The purpose of this analysis is to determine if there is any evidence to support a claim that being a member of the Amazon Vine program will bias the vine member to produce a more positive review of a product.

## Results

A random dataset of product reviews was pulled from AWS S3 buckets and broken down into total reviews, total 5-star reviews, 5-star reviews by Vine members, and 5-star reviews by non-members. The following is a discussion of the results: 

![total reviews](https://github.com/MattK1454/Amazon_Vine_Analysis/blob/main/Resources/images/total_reviews.png)

After filtering the table for reviews where at least 50% people who voted on the review found it helpful, the total number of reviews remaining was 25,557.

![total 5-star reviews](https://github.com/MattK1454/Amazon_Vine_Analysis/blob/main/Resources/images/five_star_reviews.png)

Of the 25,557 reviews, 12,235 reviews had a 5-star rating.

![5-star reviews by Vine members](https://github.com/MattK1454/Amazon_Vine_Analysis/blob/main/Resources/images/vine_member_5reviews.png)

The 12,235 were then filtered for 5-star reviews posted by Vine members. Of the 12,235 5-star reviews, 202 of them came from Vine program members.

![5-star reviews by non-members](https://github.com/MattK1454/Amazon_Vine_Analysis/blob/main/Resources/images/nonvine_member_5reviews.png)

The 12,235 reviews were also filtered for 5-star reviews posted by non-Vine members. Of the 12,235 5-star reviews, 12,033 of them were posted by non-Vine members.

This data shows 98.35% of 5-star reviews came from non-vine members versus the 1.65% of reviews posted by Vine members.

Results Summary:

- Total reviews: 25,557
- Total 5-star reviews: 12,235
- 202 (1.65%) of 5-star reviews were posted by Vine members
- 12,033 (98.35%) of 5-star reviews were posted by Vine members

## Summary

1.65% (202) of the total, helpful, 5-star reviews were posted by Vine members. The overwhelming majority of 98.35% (12,033) of 5-star reviews were posted by non-Vine members.  It would be resonable to argue a bias exists if an overwhelming majority of the positive reviews came from the Vine members. Since this dataset shows no clear evidence of a majority of 5-star reviews were posted by non-Vine members we can state there is no positivity bias in the Vine program for this dataset.

Suggested analysis:

- It might be of benifit to statistically analyze the distribution of reviews among Vine members to determine if someone is in the Vine program, are the reviews randomly distributed or is there a tendency toward a higher or lower level review revealing an implicit bias by being in the Vine program. This test could be performed using an ANOVA statistical test.

## References

1. Module 16 Challenge. Retrieved January 23, 2021, from https://courses.bootcampspot.com/courses/453/assignments/6458
