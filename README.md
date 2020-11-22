# Comparing Household Income in Baltimore, MD and Nassau County, NY with Opportunity Atlas Data
## Background

The metric of household income is an important contributor to many different aspects of life. An [editorial by the Baltimore Sun](https://www.baltimoresun.com/opinion/editorial/bs-ed-0207-baltimore-poverty-20190205-story.html) provided arguments for how a focus on poverty in Baltimore could solve a wide array of the issues in the city. The article mentions that multiple issues in the city can be correlated to poverty. For instance, people may turn to crimes like burglary at a higher rate if they have less economic security, and feel the need to engage in it for financial reasons. Moreover, The Baltimore City Health Department that poverty has been correlated with health issues as well. The article states that “people in low-income neighborhoods such as Upton Druid Heights consistently have more health problems … than people in wealthier areas such as Roland Park.” The fact that household income has consequences beyond what one may initially think, like health and crime rates, makes this a very important and interesting metric to delve into.

Additionally, according to an [article in the New York Times](https://www.nytimes.com/2015/05/04/upshot/an-atlas-of-upward-mobility-shows-paths-out-of-poverty.html), household income could be affected by the location of the individual when they were a child. It provides information on the notion that location plays a role in the American dream. According to a study in the article, it “f[ound] that poor children who grow up in some cities and towns have sharply better odds of escaping poverty than similar poor children elsewhere.” Thus, a deeper look into the household incomes of vastly different location could provide greater insights for a potential Baltimore-centric solution. 

An analysis of Nassau County, NY and Baltimore, MD, two locations with very different socioeconomic scenes, allows the ability to analyze how location may affect the financial status of children. Having grown up in Nassau County for most of my life, I had not understood the relative wealthiness of where I lived. Resting around 50 minutes outside New York City on Long Island, NY, it has a median household income of [$116,304](https://datausa.io/profile/geo/nassau-county-ny).Throughout my three years in Baltimore, I had definitely felt the stark contrast. It would be interesting to me to be able to potentially find Baltimore-centric solutions by comparing my personal home to my college home to find ways to alleviate percentage of people in poverty.

A look into Open Data from [Opportunity Atlas](https://www.opportunityatlas.org/) for household income will provide the means to explore how the financial trajectory of individuals in adulthood may be correlated with their parents' income and location at which they grew up.

## Business Question
___How can Baltimore better target their considerable problem of poverty, and what different metrics affect the financial position of children in adulthood?___

## Open Data 
1.	__Opportunity Insights:__ this research group found the average household income from the 2014-2015 Census. A full data dictionary of column variables can be found [here.](https://github.com/skang06/baltimore-nassau-county/blob/master/glossary.txt)
- [Nassau County household income for those with parents' income in bottom 25th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p25%20(11).csv):this dataset contains the original data source
- [Nassau County household income for those with parents' income in middle 50th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p50%20(7).csv):this dataset contains the original data source
- [Nassau County household income for those with parents' income in 75th percentile or higher](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p75%20(2).csv):this dataset contains the original data source
- [Baltimore household income for those with parents' income in bottom 25th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p25%20(12).csv):this dataset contains the original data source
- [Baltimore household income for those with parents' income in middle 50th percentile](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p50%20(8).csv):this dataset contains the original data source
- [Baltimore household income for those with parents' income in 75th percentile or higher](https://github.com/skang06/baltimore-nassau-county/blob/master/shown_tract_kfr_rP_gP_p75%20(3).csv):this dataset contains the original data source


## Excel Data Analysis 
Microsoft Excel was used to help further provide color on the problem and potential avenues for solutions.

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/meanmedian.png)

Upon looking at the combined bar graph, you can see that the both the mean and median are higher in Nassau than in Baltimore. Sometimes the values for a mean can be skewed by outliers, but the fact that both the mean and median here are higher in Nassau than in Baltimore demonstrates its consistency. It highlights the need for reform, and how looking into some of the initiatives and opportunities that are created by living in Nassau could help develop Baltimore-centric solutions for the issue of poverty.

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupoverty.png)
![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/baltimorepoverty.png)

No one who grew up in Nassau County, regardless of the income of the parents, were living in poverty in adulthood. According to my data, Baltimore only had very small levels of poverty for those who grew up with parents with incomes higher than the 25th percentile. However, for those with parents' income in the 25th percentile or less, around 60% ended up in poverty when they were adults. This demonstrates that getting parents in the 50th percentile made a big difference for those in Baltimore. Looking at how to get more people at that level could help result in lower percentages of adults in poverty. 

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupivot1.png)
![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/baltimorepivot2.png)

Both pivot charts show that there are pockets in both locations where household income is lower across all parent income distributions. This provides a direction of where to potentially concentrate resources in a Baltimore-centric solution for maximum benefit in the future. 

## Python Notebooks
Used Python and Google colaboratory to conduct analysis
- __Baltimore-Nassau-sunwookang.ipynb:__ a Google Colaboratory notebook to aggregate data and make data visualizations [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/11teRC-rjrv8kMtpNIDOyBTZdIYh9PQTe#scrollTo=tbo5tE9SR066).

## Python Data Analysis

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/Screen%20Shot%202020-11-21%20at%208.42.09%20PM.png)
![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/Screen%20Shot%202020-11-21%20at%208.41.53%20PM.png)
Python was used to measure how many people were below/above the poverty level for each income bracket. This produced almost identical results to the Excel data analysis, further supporting the conclusion that there were much more people above poverty in Baltimore across the income percentiles. Moreover, getting people in the 50th percentile made a big difference in lowering the amount below poverty in Baltimore. Additionally, Nassau had barely any below poverty. The slight error in getting some people below poverty in Nassau although the Excel data analysis did not, was that the in my Excel analysis, I realized had filtered out those with blank inputs for the different income percentiles because I had been able to see it clearly since I saw the data set all on one page. Howevver, using Python, I wasn't able to catch that.

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/Screen%20Shot%202020-11-21%20at%208.31.17%20PM.png)
![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/Screen%20Shot%202020-11-21%20at%208.31.28%20PM.png)
Python was used to recreate the pivot charts that compared the different household incomes for those who came from differing household income backgrounds in the different neighborhoods of Baltimore. As demonstrated in the two graphs, they are both showing that there are pockets in both locations where household income is lower across all parent income distributions, as the Excel Data Analysis did. 

Python was also used to calculate the aggregated mean and median for the differing household incomes. Although the mean and median for Baltimore were lower than Nassau for all income percentiles, supporting the original analysis, the analysis produced slightly different values for some of the mean and median values. As mentioned earlier, there were some data points that I had not included from the Excel analysis since I had seen empty inputs, but hadn't in my python analysis.

In conclusion, Python provided further support for my analysis as I receive the virtually the same mean, median, above/below poverty calculations and pivot charts. Therefore, I was able to able provide credibility to my original analysis. 

## Python vs Excel

Overall, Python did help in this analysis in that it involved commands that performed steps that would have otherwise required the use of multiple clicks. Thus, it was faster. Moreover, since it does not involve as many steps, there is less room for error. Not to mention, Python immediately tells you if something went wrong with an explanation as to why it went wrong. For Excel, it is a bit harder to figure out why something might not be going right. There is also the ability to embed comments of what you did to clarify an analysis.

Nonetheless, Python made the analysis a bit difficult in that it was not as intuitive as Excel. I did not have much prior experience using Excel, and so it made forming certain graphs more difficult and took longer. Additionally, since I could not see all of the data set at once as I was going through all of the analysis for Python, it made it harder to catch some discrepancies in the data.

In the future, Python is an efficient method of analysis if one is experienced with using it. It often accomplishes tasks with only a couple steps, minimizing the chance for error. Additionally, it tells you why something might not be working. Both can be used to provide checks against each other, if time allows, as I mentioned earlier, sometimes they provide different answers that one can catch using the different methods.


## Importance of Findings and Next Steps
Overall household income is higher for those who live in Nassau County, regardless of parents' income. The findings are important for the Baltimore City Government as the issue of household income has far-reaching effects, in terms of health and crime, as well as the tendency of it to cycle and continue in the future. Baltimore City can look into what initiatives and opportunities Nassau made available to its residents in order to figure out Baltimore-centric solutions to decrease rates of poverty. Based on my analysis, focusing on different pockets of Baltimore that are more significantly lower in terms of household income could be an efficient method to target issues of poverty. Finally, focusing on getting people within the middle 50th percentile in terms of income could help with future issues of poverty. 

Some additional data on the specific pockets in both Nassau County and Baltimore that seem to have lower household incomes relative to other towns in the area would be helpful. Further analysis on possible similarities and differences between those towns with relatively lower household incomes can provide further solutions for the Baltimore City Government.
