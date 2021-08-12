# Data Investigation - Suicide Data Analysis

### Project Overview

The purpuse of this analysis is to investigate a dataset. For my project I choose Suicide Data Analysis (Suicide Rates per Country from 1990 to 2016 and GDP, gini-index and cell phone use). 

***For detailed data investigation please see the [jupiter notebook report](Investigate_a_Dataset_Report_Udacity_Andreja_Ho.ipynb) where one can follow complete steps of data investigation, accompanied with charts and explanation.***


### Introduction

Suicide is a global phenomenon and occurs throughout the lifespan. Close to 800 000 people die due to suicide every year, which is one person every 40 seconds (source: WHO). For this project, I am analyzing global suicide data from 1990 to 2016. In particular I am interested in finding trends amongst countries with the most and the least suicide per 100,000 people and how those countries differ in GDP, Gini-index (inequality index) and cell-phone use.

### Data used

For my analysis I choose datasets form [Gapminder World](https://www.gapminder.org/data/). 

- Population Dataset (pop_df) -> <i>number of people</i>
- Cell Phone Usage Dataset (cell_df) -> <i>numbers of subscriptions</i>
- Suicide Dataset (suic_df) -> <i>suicide total deaths</i>
- GDP Dataset (gdp_df) -> <i>GDP per capita</i>
- Gini Index (gini_df) -> <i>(inequality index)</i>


### Questions for Analysis
<b>1. SUICIDE TREND AND GDP: Is GDP associated with suicide rate per country?</b><br/>
        - what is the overall suicide trend globally?<br/>
        - what is the overall suicide trend for top 10 countries\*?<br/>
        - what is the overall suicide trend for bottom 10 countries\*?<br/>
        - what is GDP (gross domestic product) in top or bottom 10 countries?<br/>
        - which countries are in top 10?<br/>
        - which countries are in bottom 10?<br/>

<b>2. SUICIDE TREND AND GINI INDEX: Is Gini Index associated with suicide rate per country</b><br />
        - is gini index associated with suicide rate?
        
*Top and bottom 10 countries were defined by most/least number of suicides per capita (per 100,000).       
        
*Gross domestic product is a monetary measure of the market value of all the final goods and services produced in a specific time period. Source: wikipedia*

*In economics, the Gini coefficient, sometimes called the Gini index or Gini ratio, is a measure of statistical dispersion intended to represent the income inequality or wealth inequality within a nation or any other group of people. A Gini coefficient of zero expresses perfect equality, where all values are the same (for example, where everyone has the same income). A Gini coefficient of one (or 100%) expresses maximal inequality among values (e.g., for a large number of people where only one person has all the income or consumption and all others have none, the Gini coefficient will be nearly one) Source: wikipedia*

### Description for investigation
In order to investigate those question I did the following:
- Download the data from Gapminder World.
- Examine dataset and handle missing values.
- Merge and reshape the data.
- Calculate suicide per 100,000 people and cell phone use per 100,000 people.
- Check the trends and correlations between variables.
- Group countries in two categories for comparison - top 10 countries with most suicide per capita and bottom 10 countries with least suicide per capita.
- Check summary statistics.
- Plot histogram for GDP in those two groups.
- Explore suicide trends in those two groups.
- Group Gini index into 3 categories in order to see which group has more suicide per capita.

### Conclusions
In this analysis, I focused on the global suicide trend from 1990 to 2016 and explore the potential association with GDP, Gini-index and cell phone use.
Regarding cell phone use I cannot draw any meaningful conclusions since the idea is beyond this dataset. I wanted to see if there is any trend or association between cell phone use and suicide. For example: in 1990 the cell phone became more and more popular and it might have an impact on the suicide rate. Next, smartphones became popular around the year 2010 and wanted to see if there is any association. Unfortunately, this dataset is not suitable for this kind of research and more detailed data is needed. For example suicide data per age, smartphone sales, etc.

From the line chart, I learned about the suicide trends, globally, for the top 10 countries with the most suicide per capita and the bottom 10 countries with the least suicide per capita. From the line chats, I can see an overall decreasing trend with a slight increase in 2014. This trend is similar for the top 10 countries. The bottom 10 countries' suicide rate has a positive trend, which is the opposite of the top 10 countries. The mean for the top 10 countries is 33.93 suicide per 100,000 while the mean for the bottom 10 countries is 2.37 per 100,000 people.*

From the summary statistics, we can see that GDP values in the top 10 countries are much more spread out than in the bottom 10 countries. The histogram showed that the top 10 countries have GDP between 5,000 and 30,000 whereas the top and bottom countries have GDP values more spread out ranging from 10,000 to 55,000.

Grouping the Gini index into three categories showed that countries with a lower inequality rate have more suicide than countries with a higher inequality rate.

Limitations This dataset has few limitations. Gini-index null values were filled with the mean of the Gini index for a specific country throughout the years. The original dataset had a lot of missing values and filling null values this way could cause the results to be too general. Another improvement could be done to add more variables to the dataset. For example suicide per age group, gender and smartphone sales in the 2000s.
