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

<b>Data Footnotes</b>
As laws differ a lot from territory to territory, especially relating to whom is protected by minimum wage laws, the following footnotes are located throughout the data in Footnote to add more context to the minimum wage. The original footnotes can be found here.

(a) - under the Federal Fair Labor Standards Act (FLSA), the two rates shown in 1968, 1970, and 1976 reflect the former multiple-track minimum-wage system in effect from 1961 to 1978. The lower rate applied to newly covered persons brought under the act by amendments, whose rates were gradually phased in. A similar dual-track system was also in effect in certain years under the laws in Connecticut, Maryland, and Nevada.

(b) - For the years indicated, the laws in Arizona, Arkansas, California, Colorado, Kentucky, Minnesota, Ohio, Utah, and Wisconsin applied only to women and minors.

[c] - Rates applicable to employers of four or more.

(d) - Rates applicable to employers of six or more. In West Virginia, applicable to employers of six or more in one location.

(e) - Rates applicable to employers of two or more.

(f) - For the years 1988 to 1990, Minnesota had a two tier schedule with the higher rate applicable to employers covered by the FLSA and the lower rate to employers not covered by the FLSA.

(g) - Minnesota sets a lower rate for enterprises with annual receipts of less than $500,000 ($4.90, January 1, 1998-January 1, 2005). The dollar amount prior to September 1, 1997 was $362,500 ($4.00 - January 1, 1991-January 1, 1997); Montana sets a lower rate for businesses with gross annual sales of $110,000 or less ($4.00 - January 1, 1992-January 1, 2005); Ohio sets a lower rate for employers with gross annual sales from $150,000 to $500,000 ($3.35 - January 1, 1991-January 1, 2005) and for employers with gross annual sales under $150,000 ($2.50 - January 1, 1991-January 1, 2005); Oklahoma sets a lower rate for employers of fewer than 10 full-time employees at any one location and for those with annual gross sales of less than $100,000 ($2.00, January 1, 1991-January 1, 2005); and the U.S. Virgin Islands sets a lower rate for businesses with gross annual receipts of less than $150,000 ($4.30, January 1, 1991-January 1, 2005).

(h) - In the District of Columbia, wage orders were replaced by a statutory minimum wage on October 1, 1993. A $5.45 minimum rate remained in effect for the laundry and dry cleaning industry as the result of the grandfather clause.

(i) - In Puerto Rico, separate minimum rates are in effect for almost 350 non-farm occupations by industry Mandatory Decrees. Rates are higher than those in the range listed in effect in a few specific occupations. (i2) - The rate is 5.08/hour for those employees not covered by the Fair Labor Standards Act.

(j) - In the U.S. Virgin Islands, implementation of an indexed rate, which was to have started January 1, 1991, was delayed.
