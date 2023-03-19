# Amazon_Vine_Analysis

> For this project you'll be partnering with Jennifer, an account manager at BigMarket. SellBy, your client, loves to talk about the power of big data, but Jennifer isn't a data expert. So you start off the project by giving her a quick overview of what big data actually is.

> Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

Language: python
IDE: Google Colaboratory 
Library: PySpark

## Overview of the analysis of the Vine program:

SellBy wants to harness the power of big data to analyze product review data.  BigMarket is a company dedicated to allowing customers to use big data to help make educated business decisions. 
In this case, BigMarket can provide review and Amazon Vine data for a cost.  The job of Jennifer and I is to analyze the Amazon review data provided for our customer SellBy.

## Results:

- How many Vine reviews and non-Vine reviews were there?

    - There is a total of 94 Amazon Vine reviews and 40471 non-Vine reviews. 

![Quantity of Vine versus Non-Vine Reviews](/images/number_of_views.png)

Figure 1: Quantity of Vine versus Non-Vine Reviews

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
    - There is 48 Amazon Vine review that were rated 5 stars.  
    - There was 15663 non-Vine reviews that were rated 5 stars. 

![Quantity of Vine versus Non-Vine 5 stars](/images/number_of_5stars.png)

Figure 2: Quantity of Vine versus Non-Vine 5 stars


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
    - There was a 51.1% of Amazon Vine reviews that were rated 5 stars.
    - There was a 38.7% of non-Vine reviews that were rated 5 stars.

![Quantity of Vine versus Non-Vine Percentage 5 stars](/images/percentage_of_5stars.png)

Figure 3: Quantity of Vine versus Non-Vine Percentage 5 stars


## Summary:

Based on the analyses, half of the Amazon Vine reviews are rated as five stars versus the thirty nine percent of non-vine reviews rated as five stars.  Based on that information, there is at least some bias in this dataset.  The Amazon Vine program sends free products to customers for them to review.  This is an example of an incentivized review program.  Amazon states that people enrolled in the Vine program are recommended to provide accurate and informative reviews.  There are 48 people who could have rated it 5 stars; because, it was free product.  As someone who uses Amazon frequently, I'm always cautious of the five star reviews from Amazon Vine participants. You can't be sure that the reviewer is not influenced by the fact the product was free or not. I would recommend performing a t test with subsets of the mean for Vine reviews versus non-Vine reviews.  This would tell us if the means were statistically similar or not.  If the means are similar, the impact of the bias could be considered negligible.  If the data is to be published, it should be stated to inform the reader of the possible source of bias. 