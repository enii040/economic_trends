
## Analyzing Inflation and Economic Trends: A Comparative Data Analysis of U.S. and German CPI, GDP, and Inflation Across Presidential and Chancellor Tenures 


<div align="center">
Val Hoxha & Eneida Likaj
  <p><a href="https://colab.research.google.com/drive/1owGzEK4yEnB7BBwD5_JwS8etEzIckTPT?usp=sharing" target="_blank">Google Collab</a></p>
</div>


## **Introduction**

The primary aim of this project is to conduct a comparative analysis of inflation and economic trends in the U.S. and Germany across different political leadership periods. We focus on the **Consumer Price Index (CPI)**, **Inflation, GDP**, and **GDP Deflator** data from 2009 to 2023, analyzing how these economic indicators vary under different U.S. presidencies (Obama, Trump, Biden) and German chancellorships (Merkel and Scholz). Specifically, we seek to understand how inflationary trends and overall economic performance have been influenced by changes in political leadership in both countries.

### **Data and Data Sources**

1. **Consumer Price Index (CPI) \- United States & Germany**: The CPI dataset measures changes in the cost of a fixed basket of goods and services, offering insights into the cost of living and inflation. This dataset covers 1960-2023 for 265 countries and regions. We filtered this dataset to get the information only for the United States and Germany.   
   * Data source: World Bank (API\_FP.CPI.TOTL\_DS2\_en\_csv\_v2\_63937.csv)  
2. **Inflation (Annual %) \- United States & Germany**: This dataset tracks inflation as the percentage change in the cost of goods and services based on the CPI. It enables comparing price changes over time from 1960 to 2023 for 265 countries and regions.  
   * Data source: World Bank (API\_FP.CPI.TOTL.ZG\_DS2\_en\_csv\_v2\_77.csv)  
3. **Inflation (Based on GDP Deflator) \- United States & Germany:** This dataset measures inflation as the annual percentage change in the GDP deflator, which reflects the overall rate of price changes in the entire economy. It allows for a broader view of inflation beyond just consumer goods and services. The data covers the period from 1960 to 2023 for 265 countries and regions.  
   * Data source: World Bank (API\_NY.GDP.DEFL.KD.ZG\_DS2\_en\_csv\_v2\_63918.csv)  
4. **GDP (Current US$) \- United States & Germany**: This dataset provides the GDP at purchaser's prices from 1960 to 2023 for 265 countries and regions, measuring the total production value added by all resident producers. It gives a broader perspective on inflationary effects within the entire economy.  
   * Data source: World Bank (API\_NY.GDP.MKTP.CD\_DS2\_en\_csv\_v2\_2.csv)  
5. **GDP Deflator (Base Year Varies by Country) \- United States & Germany (2010 base year):** The GDP deflator is the ratio of nominal GDP to real GDP, which provides an economy-wide price measure. This dataset shows the percentage change in the GDP deflator, using a base year of 2010 for both the United States and Germany. The data covers 1960 to 2023 and includes 265 countries and regions.  
   * Data source: World Bank (API\_NY.GDP.DEFL.ZS\_DS2\_en\_csv\_v2\_3767.csv)


### **Research Questions**

* How do inflation trends (both CPI and GDP deflator) differ across different political tenures in the U.S. and Germany?  
* How do changes in economic indicators like GDP reflect shifts in leadership policies and their impact on the overall economy?  
* What are the similarities and differences between inflationary trends in the U.S. and Germany during different political periods?


### **Overview of Analysis Approach**

Our approach is to analyze CPI, inflation, and GDP data for both the U.S. and Germany across different political tenures. We will compare the **CPI-based inflation** and **GDP deflator-based inflation** to evaluate their relationship and differences, and how they change under different political leadership in both countries. This analysis will use visualizations and statistical analysis to interpret the trends.


## **Methods & Results**

### **Data Preparation**

The datasets were obtained from the World Bank, covering economic indicators such as the **Consumer Price Index (CPI)**, **Inflation (based on CPI and GDP Deflator)**, and **GDP** for both the United States and Germany from 1960 to 2023\.

We first focused on **slicing the data** to only include the relevant rows for the **United States** and **Germany** and filtered the columns to **only include data from 2009 to 2023**. This ensured that our analysis was limited to the most recent periods, which were relevant for our comparative analysis. This step was crucial to maintain consistency and relevance in our comparison, as the political leadership in both countries changed during this time, affecting economic conditions.

We then **transposed** the datasets to make the year column the index, ensuring that it would be easier to plot and analyze the data over time. The datasets were cleaned to handle missing or inconsistent data points, which were minimal but addressed by interpolation when necessary.


### **Data Issues & Concerns**

* The data for both countries had some discrepancies, particularly in terms of different base years for the GDP deflator. We took these differences into account during our analysis, ensuring that the comparisons made were contextually relevant.  
* Due to missing data points for some countries, especially those outside the U.S., we focused on Germany, which had complete and reliable data for the period of interest. This allowed us to maintain consistency and ensure a meaningful comparison in our analysis.


### **Analysis and Visualizations**

After preparing the datasets, we analyzed the data based on **two main axes**: the **U.S. Presidential Terms** and the **German Chancellor Terms** which both aligned perfectly **(2009-2013, 2013-2017, 2017-2021, 2021-2023)**. Shaded regions were used to highlight the periods of different U.S. presidencies and German chancellorships, making it easier to visualize the impacts of leadership changes. We plotted each dataset over these political tenures to explore how the leadership affected the economic indicators.


- **Graphing for Each Indicator (Points 1-8):** For each of the following points, we created **separate** graphs for the U.S. and Germany to visualize and compare the trends:


**1. Consumer Price Index (CPI)**: We visualized the **CPI** for both countries to see how the cost of consumer goods has evolved from 2009 to 2023\.

<iframe src="Consumer Price Index (2010 100) - United States.html" width="100%" height="600" frameborder="0"></iframe>
<iframe src="Consumer Price Index (2010 100) - Germany.html" width="100%" height="600" frameborder="0"></iframe>

\
**2. Inflation, Consumer Prices (Annual %)** :  
   We plotted the **annual inflation rates** based on **CPI** for the U.S. and Germany to compare how the yearly inflation percentage has fluctuated across both countries\.
   
 <iframe src="Inflation(Consumer Prices) - United States.html" width="100%" height="600" frameborder="0"></iframe>
 <iframe src="Inflation(Consumer Prices) - Germany.html" width="100%" height="600" frameborder="0"></iframe>

\
**3. CPI and Inflation Graph**:  
   We combined **CPI** and **Inflation** data on a single graph for both countries, allowing a direct comparison of these two key indicators\.

 <iframe src="Consumer Price Index (CPI) and Inflation in the US (2009-2023).html" width="100%" height="600" frameborder="0"></iframe>
 <iframe src="Consumer Price Index (CPI) and Inflation in Germany (2009-2023).html" width="100%" height="600" frameborder="0"></iframe>

\
**4. Inflation, GDP deflator (Annual %)**:  
   We created graphs showing inflation based on the **GDP deflator**, which offers a broader view of inflation by measuring price changes in the economy as a whole\.

 <iframe src="Inflation(GDP deflator) - United States.html" width="100%" height="600" frameborder="0"></iframe>
 <iframe src="Inflation(GDP deflator) - Germany.html" width="100%" height="600" frameborder="0"></iframe>

\
**5. GDP (Current US$)**:  
   We visualized the **Gross Domestic Product (GDP)** data for both countries to analyze the overall economic output and growth over the years.\

 <iframe src="GDP - United States.html" width="100%" height="600" frameborder="0"></iframe>
 <iframe src="GDP - Germany.html" width="100%" height="600" frameborder="0"></iframe>

\
**6. GDP Deflator (2010 \= 100\)**:  
   The **GDP deflator** was plotted for both countries, showing the changes in the price level of all goods and services produced domestically, relative to the base year 2010\.
   
 <iframe src="GDP Deflator - United States.html" width="100%" height="600" frameborder="0"></iframe>
 <iframe src="GDP Deflator - Germany.html" width="100%" height="600" frameborder="0"></iframe>

\
**7. Economic Indicators \- GDP Deflator and Inflation (based on GDP Deflator)**:  
   These graphs combined the **GDP deflator** and **Inflation (based on GDP deflator)** for the U.S. and Germany to examine the relationship between these two indicators during the specified period in each country.\

 <iframe src="USA Economic Indicators - GDP Deflator and Inflation (based on GDP Deflator).html" width="100%" height="600" frameborder="0"></iframe>
 <iframe src="Germany Economic Indicators - GDP Deflator and Inflation (based on GDP Deflator).html" width="100%" height="600" frameborder="0"></iframe>

\
**8. Inflation Comparison: GDP Deflator vs CPI**:  
   We compared **GDP deflator-based inflation** and **CPI-based inflation** on a single graph for each country to analyze the differences in these two inflation measures over time\.

 <iframe src="Inflation Comparison_ GDP Deflator vs CPI - USA (2009-2023).html" width="100%" height="600" frameborder="0"></iframe>
 <iframe src="Inflation Comparison_ GDP Deflator vs CPI - Germany (2009-2023).html" width="100%" height="600" frameborder="0"></iframe>

\
**9. Cross-Country Comparison of CPI and Inflation in the US and Germany**:  
   We analyzed and compared the CPI and inflation trends between the US and Germany to identify differences in price stability and inflationary pressures over time\.

 <iframe src="Cross-Country Comparison of CPI and Inflation in the US and Germany.html" width="100%" height="600" frameborder="0"></iframe>


 
## **Conclusions**

Referring to the Methods section, we successfully analyzed inflation and economic trends in both the **United States** and **Germany** across different political leadership periods. We focused on a comparative analysis of **Consumer Price Index (CPI)**, **GDP deflator**, and **Gross Domestic Product (GDP)** for the years **2009-2023**. Using visualizations and statistical analysis, we explored how these economic indicators varied under different **U.S. presidencies** (Obama, Trump, Biden) and **German chancellorships** (Merkel, Scholz).


### **Key Findings**

* **CPI and GDP Deflator Trends**: We found that inflation, as measured by the CPI, showed similar trends between the U.S. and Germany, though Germany's CPI was generally lower throughout the analysis period. The GDP deflator in the U.S. exhibited greater volatility compared to Germany, suggesting broader economic shifts.  
* **Impact of Political Leadership**: The changes in inflation rates across U.S. presidential terms (Obama, Trump, and Biden) reflected the differences in economic policies, particularly during times of economic crisis (e.g., the COVID-19 pandemic) and recovery periods. Similarly, Germany’s inflationary trends under Merkel and Scholz indicated shifts in fiscal policy and economic strategy, especially in response to the global economic shifts caused by the pandemic.


### **Limitations**

* **Data Sources**: We first encountered limitations as we believed that there were differences in database years for the GDP deflator between the U.S. and Germany, which could have led to some inconsistencies in cross-country comparisons. However, we spoon realized that the data statistics had the same base year (2010 \= 100\)  
* **External Factors**: Our analysis is confined to data from 2009 to 2023, and external events (such as the COVID-19 pandemic) may have disproportionately impacted economic trends during this period.





## **References**

“Consumer Price Index (2010 \= 100).” *World Bank Open Data*, International Monetary Fund, International Financial Statistics and data files., data.worldbank.org/indicator/FP.CPI.TOTL?end=2023\&locations=US\&start=1960. Accessed 7 Dec. 2024\. 

“Inflation, Consumer Prices (Annual %).” *World Bank Open Data*, International Monetary Fund, International Financial Statistics and data files., https://data.worldbank.org/indicator/FP.CPI.TOTL.ZG?end=2023\&locations=US\&start=1960. Accessed 7 Dec. 2024\. 

“Inflation, GDP deflator (annual %).*”* *World Bank Open Data*, International Monetary Fund, International Financial Statistics and data files., https://data.worldbank.org/indicator/NY.GDP.DEFL.KD.ZG?locations=US. Accessed 7 Dec. 2024\. 

“GDP (Current US$).” *World Bank Open Data*, International Monetary Fund, International Financial Statistics and data files., https://data.worldbank.org/indicator/NY.GDP.MKTP.CD?locations=US. Accessed 7 Dec. 2024\. 

“GDP deflator (2010 \= 100).” *World Bank Open Data*, International Monetary Fund, International Financial Statistics and data files., https://data.worldbank.org/indicator/NY.GDP.DEFL.ZS?locations=US. Accessed 7 Dec. 2024\. 
