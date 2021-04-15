# Data Investigation

The purpuse of this analysis is to onvestigate a dataset. For my project I choose Suicide Data Analysis (Suicide Rates per Country from 1990 to 2016 and GDP, gini-index and cell phone use).

#### Introduction

Suicide is a global phenomenon and occurs throughout the lifespan. Close to 800 000 people die due to suicide every year, which is one person every 40 seconds (source: WHO). For this project, I am analyzing global suicide data from 1990 to 2016. In particular I am interested in finding trends amongst countries with the most and the least suicide per 100,000 people and how those countries differ in GDP, Gini-index (inequality index) and cell-phone use.

#### Data used

For my analysis I choose datasets form Gapminder World (https://www.gapminder.org/data/). 

- Population Dataset (pop_df) -> <i>number of people</i>
- Cell Phone Usage Dataset (cell_df) -> <i>numbers of subscriptions</i>
- Suicide Dataset (suic_df) -> <i>suicide total deaths</i>
- GDP Dataset (gdp_df) -> <i>GDP per capita</i>
- Gini Index (gini_df) -> <i>(inequality index)</i>


#### Questions for Analysis
<b>1. SUICIDE TREND AND GDP: Is GDP associated with suicide rate per country?</b><br />
        - what is the overall suicide trend globally?<br />
        - what is the overall suicide trend for top 10 countries\*?<br/>
        - what is the overall suicide trend for bottom 10 countries\*?<br/>
        - what is GDP (gross domestic product) in top or bottom 10 countries?<br/>
        - which countries are in top 10?<br />
        - which countries are in bottom 10?<br />

<b>2. SUICIDE TREND AND GINI INDEX: Is Gini Index associated with suicide rate per country</b><br />
        - is gini index associated with suicide rate?
        
*Top and bottom 10 countries were defined by most/least number of suicides per capita (per 100,000).       
        
*Gross domestic product is a monetary measure of the market value of all the final goods and services produced in a specific time period. Source: wikipedia*

*In economics, the Gini coefficient, sometimes called the Gini index or Gini ratio, is a measure of statistical dispersion intended to represent the income inequality or wealth inequality within a nation or any other group of people. A Gini coefficient of zero expresses perfect equality, where all values are the same (for example, where everyone has the same income). A Gini coefficient of one (or 100%) expresses maximal inequality among values (e.g., for a large number of people where only one person has all the income or consumption and all others have none, the Gini coefficient will be nearly one) Source: wikipedia*

#### Description for investigation
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
