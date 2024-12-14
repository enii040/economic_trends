## Analyzing Inflation and Economic Trends: A Comparative Data Analysis of U.S. and German CPI, GDP, and Inflation Across Presidential and Chancellor Tenures 
<div align="center">
  Eneida Likaj
</div>

<div align="center">
Val Hoxha & Eneida Likaj
  <p><a href="https://colab.research.google.com/drive/1owGzEK4yEnB7BBwD5_JwS8etEzIckTPT?usp=sharing" target="_blank">Google Collab</a></p>
</div>

#Introduction
The primary aim of this project is to conduct a comparative analysis of inflation and economic trends in the U.S. and Germany across different political leadership periods. 
We focus on the Consumer Price Index (CPI), Inflation, GDP, and GDP Deflator data from 2009 to 2023, analyzing how these economic indicators vary under different U.S. presidencies (Obama, Trump, Biden) and German chancellor ships (Merkel and Scholz). 
Specifically, we seek to understand how inflationary trends and overall economic performance have been influenced by changes in political leadership in both countries.

#Data and Data Sources
Consumer Price Index (CPI) - United States & Germany: The CPI dataset measures changes in the cost of a fixed basket of goods and services, offering insights into the cost of living and inflation. This dataset covers 1960-2023 for 265 countries and regions. We filtered this dataset to get the information only for the United States and Germany. 
Data source: World Bank (API_FP.CPI.TOTL_DS2_en_csv_v2_63937.csv)
Inflation (Annual %) - United States & Germany: This dataset tracks inflation as the percentage change in the cost of goods and services based on the CPI. It enables comparing price changes over time from 1960 to 2023 for 265 countries and regions.
Data source: World Bank (API_FP.CPI.TOTL.ZG_DS2_en_csv_v2_77.csv)
Inflation (Based on GDP Deflator) - United States & Germany: This dataset measures inflation as the annual percentage change in the GDP deflator, which reflects the overall rate of price changes in the entire economy. It allows for a broader view of inflation beyond just consumer goods and services. The data covers the period from 1960 to 2023 for 265 countries and regions.
Data source: World Bank (API_NY.GDP.DEFL.KD.ZG_DS2_en_csv_v2_63918.csv)
GDP (Current US$) - United States & Germany: This dataset provides the GDP at purchaser's prices from 1960 to 2023 for 265 countries and regions, measuring the total production value added by all resident producers. It gives a broader perspective on inflationary effects within the entire economy.
Data source: World Bank (API_NY.GDP.MKTP.CD_DS2_en_csv_v2_2.csv)
GDP Deflator (Base Year Varies by Country) - United States & Germany (2010 base year): The GDP deflator is the ratio of nominal GDP to real GDP, which provides an economy-wide price measure. This dataset shows the percentage change in the GDP deflator, using a base year of 2010 for both the United States and Germany. The data covers 1960 to 2023 and includes 265 countries and regions.
Data source: World Bank (API_NY.GDP.DEFL.ZS_DS2_en_csv_v2_3767.csv)

#Research Questions
How do inflation trends (both CPI and GDP deflator) differ across different political tenures in the U.S. and Germany?
How do changes in economic indicators like GDP reflect shifts in leadership policies and their impact on the overall economy?
What are the similarities and differences between inflationary trends in the U.S. and Germany during different political periods?

#Overview of Analysis Approach
Our approach is to analyze CPI, inflation, and GDP data for both the U.S. and Germany across different political tenures. We will compare the CPI-based inflation and GDP deflator-based inflation to evaluate their relationship and differences, and how they change under different political leadership in both countries. This analysis will use visualizations and statistical analysis to interpret the trends.

#Methods & Results
##Data Preparation
The datasets were obtained from the World Bank, covering economic indicators such as the Consumer Price Index (CPI), Inflation (based on CPI and GDP Deflator), and GDP for both the United States and Germany from 1960 to 2023.
We first focused on slicing the data to only include the relevant rows for the United States and Germany and filtered the columns to only include data from 2009 to 2023. This ensured that our analysis was limited to the most recent periods, which were relevant for our comparative analysis. This step was crucial to maintain consistency and relevance in our comparison, as the political leadership in both countries changed during this time, affecting economic conditions.
We then transposed the datasets to make the year column the index, ensuring that it would be easier to plot and analyze the data over time. The datasets were cleaned to handle missing or inconsistent data points, which were minimal but addressed by interpolation when necessary.

##Data Issues & Concerns
The data for both countries had some discrepancies, particularly in terms of different base years for the GDP deflator. We took these differences into account during our analysis, ensuring that the comparisons made were contextually relevant.
Due to missing data points for some countries, especially those outside the U.S., we focused on Germany, which had complete and reliable data for the period of interest. This allowed us to maintain consistency and ensure a meaningful comparison in our analysis.

##Analysis and Visualizations
After preparing the datasets, we analyzed the data based on two main axes: the U.S. Presidential Terms and the German Chancellor Terms which both aligned perfectly (2009-2013, 2013-2017, 2017-2021, 2021-2023). Shaded regions were used to highlight the periods of different U.S. presidencies and German chancellorships, making it easier to visualize the impacts of leadership changes. We plotted each dataset over these political tenures to explore how the leadership affected the economic indicators.
Graphing for Each Indicator (Points 1-8): For each of the following points, we created separate graphs for the U.S. and Germany to visualize and compare the trends:
Consumer Price Index (CPI): We visualized the CPI for both countries to see how the cost of consumer goods has evolved from 2009 to 2023.




