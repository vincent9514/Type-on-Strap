---
layout: post
title: Shoprunner Repurchasing Analysis
tags: [E-commerce, Survial Analysis]
---

*   **Student Group**: Northwestern University Master of Science in Analytics (MSiA)    
*   **Team Members**: Vincent, Daniel, Chris, Phyllis, Zili

![Image of Shoprunner Project]({{ site.baseurl }}/assets/img/pexels/Shoprunner.png)


### 1. Purpose and Objectives

*   Analyze the factors that affect repurchasing behavior.
*   Explore the impact of the shoprunner network on its individual retailers.
*   Focal Retailers: a focal retailer is any retailer that a customer has already made a purchase from. 


### 2. Dataset

*   36000 customers
*   12000 repeat customers
*   Purchase Dates
*   Spend
*   Store Information

### 3. Impact

*   33% customer repurchase 
*   82% sales revenue comes from repurchasers

### 4. Model 

*   Discrete Time Survival Model with logistic regression


### 5. Possible factors for repurchases

1.	Focal Retailer:
    *   How many purchases did a customer make at focal retailer
    *   How many month since a customer’s last purchase at the focal retailer
2.	Shoprunner Network:
    *   How many times did a customer shop at a retailer category different from the retailer than their focal retailer
    *   How many times did a customer shop at the same retailer category as their focal retailer
3.	Control:
    *   Is it a holiday season


### 6. Feature Creation

1.	Aggregated by Month
    *   Recency: The amount of time since a focal purchase
    *   Frequency: 
        1.	Cumulative number of focal purchases
        2.	Cumulative number of non-focal purchases
        3.	Discretized continuous variable (buckets)
    *   Monetary: Cumulative average dollar amount spent by a customer 
2.	Over Time
    *   Customer lifetime (number of months since joining ShopRunner) --- T
    *   Entropy: Cumulative number of unique retailers purchased from
    *   Is a referred member or not 
    *   Impact of the network effect on focal repurchases
3.	Interactions between: Entropy & Frequency

### 7. Shoprunner Network Effect

Participating in the shoprunner network does not cannibalize customers and in many case healthy competition boosts repurchasing.


### 8. What effects repurchasing

1.	The longer it’s been since your last purchase, the less likely you are to make another purchase
2.	As you make more purchases with ShopRunner, you are more likely to make another purchases
3.	Holiday shopping has an positive effect on repurchasing for most retailers
4.	Frequent shoppers who made recent purchases are more likely to repurchase
5.	Average sales dollars and referral status do not impact repurchase much
6.	Network effect helps or it doesn’t hurt


### 9. Next Steps

1.	External marketing to shoppers:
    *   Opportunistic window to bump up frequency level for more repurchases
2.	Data Science Analysis:
    *   Investigate on more retailers
3.	External Marketing to Retailers:
    *   Sell the network effects
    *   Sell the fit-for-all Image


