# Comparing Household Income in Baltimore, MD and Nassau County, NY with Opportunity Atlas Data
## Background

The metric of household income is an important contributor to many different aspects of life. An [editorial by the Baltimore Sun](https://www.baltimoresun.com/opinion/editorial/bs-ed-0207-baltimore-poverty-20190205-story.html) provided arguments for how a focus on poverty in Baltimore could possibly solve a wide array of the issues in the city. The article mentions that multiple issues in the city can be correlated to poverty. For instance, people may turn to crimes like burglary at a higher rate if they have less economic security, and feel the need to engage in it for financial reasons. Moreover, The Baltimore City Health Department that poverty has been correlated with health issues as well. The article states that “people in low-income neighborhoods such as Upton Druid Heights consistently have more health problems … than people in wealthier areas such as Roland Park.” The fact that household income has such far reaching consequences beyond what one may initially think makes this a very important metric.

Additionally, according to an [article in the New York Times](https://www.nytimes.com/2015/05/04/upshot/an-atlas-of-upward-mobility-shows-paths-out-of-poverty.html), household income could be affected by the location of the individual when they were a child. It provides information on the notion that location plays a role in the American dream. According to a study in the article, it “f[ound] that poor children who grow up in some cities and towns have sharply better odds of escaping poverty than similar poor children elsewhere.” 

A deeper look into the household incomes of vastly different location could provide greater insights for a potential Baltimore-centric solution. An analysis of Nassau County, NY and Baltimore, MD, two locations with very different socioeconomic scenes, will allow the ability to analyze how location may affect the financial status of children. Having grown up in Nassau County for most of my life, I had not understood the relative wealthiness of where I lived. Resting around 50 minutes outside New York City, it has a median household income of [$116,304](https://datausa.io/profile/geo/nassau-county-ny).On the other hand, Baltimore has a median household income of $76,182. Throughout my three years in Baltimore, I had definitely felt the stark contrast. It would be interesting to me to be able to potentially find Baltimore-centric solutions by comparing my personal home to my college home.

A look into Open Data from [Opportunity Atlas](https://www.opportunityatlas.org/) for household income will provide the means to explore how the financial trajectory of individuals in adulthood may be correlated with their parents' income and location at which they grew up.

## Business Question
___How can Baltimore better target their considerable problem of poverty, and how can the different metrics affect the financial position of children in adulthood?___

## Open Data 
1.	__Opportunity Insights:__ this research group found the average household income from the 2014-2015 Census.
- [Nassau County household income for those with parents' income in bottom 25th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p25%20(11).csv)
- [Nassau County household income for those with parents' income in middle 50th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p50%20(7).csv)
- [Nassau County household income for those with parents' income in 75th percentile or higher](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p75%20(2).csv)
- [Baltimore household income for those with parents' income in bottom 25th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p25%20(12).csv)
- [Baltimore household income for those with parents' income in middle 50th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p50%20(8).csv)
- [Baltimore household income for those with parents' income in 75th percentile or higher](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p75%20(3).csv)


## Data Analysis 
Microsoft Excel was used to help further provide color on the problem and potential avenues to solving it.

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupoverty.png)
![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/baltimorepoverty.png)

No one who grew up in Nassau County, regardless of the income of the parents, were living in poverty in adulthood. According to my data, Baltimore only had very small levels of poverty for those who grew up with parents with incomes higher than the 25th percentile. However, for those with parents' income in the 25th percentile or less, 75% ended up in poverty when they were adults. This demonstrates that getting parents in the 50th percentile made a big difference for those in Baltimore. Looking at how to get more people at that level could help result in lower percentages of adults in poverty. 
![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/meanmedian.png)
Upon looking at the combined bar graph, you can see that the both the mean and median are higher in Nassau than in Baltimore. Sometimes the values for a mean can be skewed by outliers, but the fact that both the mean and median here are higher in Nassau than in Baltimore demonstrates its consistency. It highlights the need for reform, and how looking into some of the initiatives and opportunities that are created by living in Nassau could help develop Baltimore-centric solutions for the issue of poverty.

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupivot.png)

Both pivot charts show that there are pockets in both locations where household income is lower across all parent income distributions. This provides a direction of where to potentially concentrating resources for maximum benefit in the future. 

## Summary
Overall household income is higher for those who live in Nassau, regardless of parents' income. Thus, location plays role. Given the importance of household income in different aspects of life, including health and future security, the analysis provides a direction for which to start to combat poverty.

Based on my analysis, focusing on different pockets of Baltimore that are more significantly lower in terms of household income could be an efficient method of target issues of poverty. Furthermore, determining what Nassau might do or have that could result in higher household incomes could be another way of figuring out Baltimore-centric solutions. Finally, focusing on getting people within the middle 50th percentile in terms of income could help with future issues of poverty.

Some additional data on the specific pockets in both Nassau and Baltimore that seem to have lower household incomes relative to other towns in the area would be helpful.

This is important for me because throughout my 3 years at Hopkins, I have definitely felt the difference in wealth between the Baltimore and Nassau County. I would hope that I might want to make sure that I make sure to base any solutions on hard metrics and data that I find in order to more adequately be able to monitor my own biases while developing some sort of solution for Baltimore.
