# Project1_Group5

Data used:
1. Minimum wage Data:

Source: https://www.kaggle.com/lislejoem/us-minimum-wage-by-state-from-1968-to-2017
This formed the inspiration for our data exploration where the cleaned minimum wage data was pulled from a kaggle file. This data includes historical rate for 40 years (1968 to 2017). 

2. Unemployment data
Source: http://www.ncsl.org/research/labor-and-employment/2012-state-unemployment-rates.aspx
This let us extract the unemployment data from 2009 - 2017. We merged and cleaned this data to find the total unemployment rate for each states individually for all the years

3. Crime Data
Source: https://www.ucrdatatool.gov/Search/Crime/State/RunCrimeStatebyState.cfm

Extracting the latest 15 years' data available in FBI UCRA tool for state by state crime in United States. The data has categorized crime data, which if time permits will let us diagnose the type of crime which picked up/ dropped. 
The year range for this data is 2000 - 2014 for our purposes. 

Since we do not have years beyond those, we will be using unemployment years as the master years and merge all datasets into those.  

<b>Description of Data of unemployment</b>

The values in the dataset are as follows:

<b>Year</b>: The year of the data.

<b>State</b>: The state or territory of the data.

<b>Table_Data</b>: The scraped value from the source.

<b>Footnote</b>: The footnote associated with the Table_Data. See more below.

<b>High.Value</b>: As there were some values in Table_Data that had multiple values (usually associated with footnotes), this is the higher of the two values in the table. It could be useful for viewing the proposed minimum wage, because in most cases, the higher value meant that all persons protected under minimum wage laws eventually had minimum wage set at that value.

<b>Low.Value</b>: This is the same as High.Value, but has the lower of the two values. This could be useful for viewing the effective minimum wage at the year of setting the minimum wage, as peoples protected under such minimum wage laws made that value during that year (although, in most cases, they had a higher minimum wage after that year).

<b>CPI.Average</b>: This is the Consumer Price Index associated with that year. It was used to calculate 2018-equivalent values.

<b>High.2018</b>: This is the 2018-equivalent dollars for High.Value.

<b>Low.2018</b>: This is the 2018-equivalent dollars for Low.Value.

Summary
---
  * The debate about the effect increases in the minimum wage have on employment is ongoing.
  * Some studies find either no or only a small effect while others find significant effects 
  * A study recently published in the American Economic Association provides new evidence that increases in minimum wage reduce employment in the long run (click here for review)
  * The goal of this research is to review 8 years of historic data across the entire United States and come up with our own understanding of the impacts of minimum wage on the overall economic profile of our country. 

Hypothesis:
---
We are set out to test three related hypotheses regarding the United States economy: 
  * Higher minimum wage has the potential to increase unemployment rates over time
  * Higher minimum wage has short term positive impact on CPI which eventually levels off as unemployment rises
  * Because of increased unemployment, crime rates will also go up over time
  
Questions: 
---
  * What is the relationship between unemployment and crime
  * Does that relationship vary by state, region, or is it consistent across the entire United States
  * Did minimum wage increase, decrease, or remain the same across the time frame of our dataset
  * Did changes in minimum wage impact employment and subsequently crime?

Summary of Findings: 
---
  * Overall, as unemployment decreases, we see a decrease in crime rates across all states
  * 2014 demonstrates the biggest drop in unemployment rates which is consistent with the tail end of the great recession from 2009
  * In the same period of time, 2009 – 2014, crime rates were consistent (slightly downward trending) but in 2014 there is a noticeable drop in crime which is consistent with the drop in the average unemployment index
  * In general, Crime and Unemployment move in the same direction though not proportionally which leads us to believe that though the two events may happen simultaneously, there is more than one factor that drive crime rates – this is especially evident as we break up our data at a more granular level (by state).
  * In the short term, increases in minimum wage did not drive unemployment and seemed to lower crime rates especially in areas with historically high crime.

Unanticipated Findings: 
---
  * By state, we expected to see that states which stood out as having higher than average unemployment rates would also see high crime instances. 
  * We found that not to be the case at the individual state level but rather on the aggregate (across the country). In other words, on average, as unemployment rises, so does crime, however that is not consistent in state by state comparisons. 
  * States with historically high crime rates see bigger drops in crime as unemployment decreases compared to states with historically lower crime rates. This could indicate that there are other (potentially more impactful) factors on crime than unemployment. 
  * Within the 8 year time frame we studied, increases in minimum wage did not seem to have an adverse (negative) effect on unemployment. Unemployment dropped noticeably and consistently YOY while minimum wage rates remained the same and increased slightly

Discussion:
---
  * One of our initial hypotheses was that because of increased unemployment, crime rates will also go up over time
  * After analyzing our data, we determined that indeed crime rate and unemployment move in the same direction consistently where as unemployment decreases crime rates also decrease. 
  * However, we don’t have enough supporting evidence to establish causality. We would reframe the hypothesis to emphasize that though there is a positive relationship between the two, crime is not necessarily depended upon or determined by  unemployment 
  * In states with historically high crime rates, the effect of decreased unemployment on crime is much more noticeable than in states with lower crime
  * Minimum wage did not change drastically in the selected time period however, unemployment decreased drastically which had a positive impact on CPI
  * Our findings are heavily impacted by the recessions and post recession dynamics of the selected time-period
  
Post Mortem:
---
  * A challenges we faced was in formatting the data and making it ready for merging (creating the final data set)
  * We focused on finding single year data per category– Crime, Unemployment, Minimum Wage
  * We cleaned each year individually and formatted it the same way for each year
  * We then stacked each year per group (Crime, Unemployment, Minimum Wage) to create three large data-sources for the same time period 
  * Finally, we merged the data together to create one final large dataset to be used for exploration and analysis





