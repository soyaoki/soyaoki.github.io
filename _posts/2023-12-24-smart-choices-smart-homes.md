---
layout: post
title: "Smart Choices, Smart Homes: A Data-Driven Approach to Home Purchases in Ames"
date: 2023-12-23 09:00:00
---

For those considering purchasing a home in Ames, Iowa...

# Introduction

The purchase of a home is, for most people, the biggest purchase of their lives. With housing prices rising in recent years, it is natural to want to make a purchase that you will not regret. The answers to the following questions, for example, may help you make a good choice when purchasing a home.

- Q.1 What are the main factors influencing housing prices in Ames, Iowa?
- Q.2 Is there any seasonality in the real estate market?
- Q.3 How does renovation or remodeling affect housing prices?


To answer the above questions, we analyzed the [Ames Housing dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview) and present the insights gained on this page.

# Q.1 What are the main factors influencing housing prices in Ames, Iowa?

The top three variables that positively affected prices were `PoolQC_EX`, `BsmtCond_Gd`, and `BsmtCond_TA`, while the top three variables that negatively affected prices were `Heating_Grav`, `Neighborhood_MeadowV` and `Functional_Maj2`. It should be understood that properties with pools and basements in good condition will be priced higher. Also, if you are satisfied with the conditions of Gravity furnace and near Meadow Village, you may be able to live in a cheap house.

![](https://github.com/soyaoki/soyaoki.github.io/blob/main/_posts/img/2023-12-24-feature-importance.png)

# Q.2 Is there any seasonality in the real estate market?

If you are purchasing a home, we recommend that you purchase in March. Also, since the prices tend to rise every year, we recommend that you purchase as soon as possible.The number of purchases is higher in April ~ July, and purchase prices tend to soar in November ~ February and June, although there are no major fluctuations.The average home (with a `BsmtCond` of TA and a `TotalBsmtSF` between 950 and 1030) has seen an increase in average price each year, although the number of purchases has decreased slightly each year.

## Yealy Trend
![](https://github.com/soyaoki/soyaoki.github.io/blob/main/_posts/img/2023-12-24-Count-of-PurchasingHouse-yearly.png)
![](https://github.com/soyaoki/soyaoki.github.io/blob/main/_posts/img/2023-12-24-SalePrice-yearly.png)

## Monthly Trend
![](https://github.com/soyaoki/soyaoki.github.io/blob/main/_posts/img/2023-12-24-Count-of-PurchasingHouse-monthly.png)
![](https://github.com/soyaoki/soyaoki.github.io/blob/main/_posts/img/2023-12-24-SalePrice-monthly.png)

# Q.3 How does renovation or remodeling affect housing prices?

Basically, the SalePrice decreases over time, but the decrease tends to be reset by remodeling.

![](https://github.com/soyaoki/soyaoki.github.io/blob/main/_posts/img/2023-12-24-Age-Remod-and-NoRemod.png)
![](https://github.com/soyaoki/soyaoki.github.io/blob/main/_posts/img/2023-12-24-Age-from-Build-and-Remod.png)


# Conclusion

In our Ames Housing market analysis, we've uncovered key insights for smart home purchasing decisions:

- **Influential Factors:** Features like `PoolQC_EX` and well-maintained basements positively impact prices, while factors like specific neighborhoods and functionalities can have a negative influence.

- **Seasonal Trends:** Purchase in March for favorable prices, and act promptly due to annual increases. Peaks in purchases occur from April to July, with price fluctuations in November-February and June.

- **Renovation Impact:** While property age may lead to a price decrease, remodeling efforts can reset this decline, emphasizing the importance of renovation potential.

By adopting a data-driven approach, prospective homebuyers can navigate the Ames real estate market more intelligently, making well-informed choices for their future homes. For further details, refer to [my notebook](https://github.com/soyaoki/DSND-Writing-a-Data-Scientist-Blog-Post). Happy home hunting!



# References
- [House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview)
- [My Notebook](https://github.com/soyaoki/DSND-Writing-a-Data-Scientist-Blog-Post)
