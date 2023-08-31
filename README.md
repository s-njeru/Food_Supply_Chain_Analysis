# Food_Supply_Chain_Analysis

## Introduction
In this analysis, we will have a look at how to analyze food prices in difefrent locations, view elements of seasonaity in food prices and possible alternative sources of commodities in the supply chain. 

The analysis analyzes data using libraries in the geospatial space such as Geopandas, Folium, CountryInfo and PyCountry. For viisualization, we're using matplotlib, plotly, and seaborn. 

For analysis purposes, we will look at 1 specific country - Afghanistan, and 1 specific commodity - Retail Wheat. There's a data pipeline at the end that can be used to reproduce the analysis for every counry and/or commodity in the dataset.


## Datasets
The dataset being analyzed is from [Humdata](https://data.humdata.org/dataset/wfp-food-prices).
This dataset contains Global Food Prices data from the World Food Programme covering foods such as maize, rice, beans, fish, and sugar for 76 countries and some 1,500 markets. It is updated weekly but contains to a large extent monthly data. The data goes back as far as 1992 for a few countries, although many countries started reporting from 2003 or thereafter.
Additional datasets include 
- ne_10m_admin_0_countries.shp which has the shape file of the Admin 0 Countries. Each country is coded with a world region that roughly follows the United Nations setup.
- naturalearth_lowres ageopandas dataset 

## Questions
Questions to answer in this analyss include:
1. Of the countries that sell retail wheat, how do their prices compare in the most recent year?
2. For the selected country (Afghanistan) and commodity (Wheat-Retail), what bhavior can be observed?
3. How does the price of the commodity compare to other countries selling it over time?
4. What is an alternative source of the commodity for the select country?
5. What additional information can be helpful to forecast the price of the commodity in the next month? year? 5 years?

## Conclusion

Questions to Answer
1. Of the countries that sell retail wheat, how do their prices compare in the most recent year?
 • *Benin, Guinea-Bissau and Mali had the most expensive rates for retail wheat in 2021 based on how dark the green is.

2. For the selected country (Afghanistan) and commodity (Wheat-Retail), what bhavior can be observed?
• *The price seems to have a general positive linear growth with some spikes and dips in price. The most significant spike happened between 2008 and 2009. From reseach, Afghanistan witnessed several significant developments related to the ongoing conflict, political transitions, and international involvement in this period. Intense fighting continued between Afghan and international coalition forces on one side and various insurgent groups, primarily the Taliban and other militant factions, on the other. The violence escalated in many parts of the country, especially in the southern and eastern provinces. 

3. How does the price of the commodity compare to other countries selling it over time?
• *Guinea Bissau, Benin and Rwanda have the highest prices between 2010 to 2020. Mali soon joined the ranks in 2020 and 2021. The countries with the lowest prices include Zimbabwe, Sudan, Tajikistan, and Ethiopia.

4. What is an alternative source of the commodity for the select country?
• *China

*Hypothesis: Wholesale wheat prices are lower in China due to factors such as local production, transportation costs, trade agreements, or subsidies. Being a boardering country, transport costs from China to Afghanistan will be low.

5. What additional information can be helpful to forecast the price of the commodity in the next month? year? 5 years?
• *To provide a forecast for the next month or the next 12 months using data from 2000 to 2022 December on food prices in countries, you would need the following additional information:

1. Recent Data: Obtain the most up-to-date data available for food prices. Having data for the current month or the past few months will help capture the latest trends and changes in food prices.

2. Economic Indicators: Gather relevant economic indicators that can influence food prices, such as GDP growth, inflation rates, exchange rates, interest rates, and agricultural production data. These indicators provide insights into the macroeconomic conditions and can help identify potential drivers of food price fluctuations.

3. Market-specific Factors: Consider market-specific factors that impact food prices, such as supply and demand dynamics, market competition, transportation costs, storage capacity, and infrastructure. Changes in these factors can affect the availability and cost of food, thus influencing prices.

4. Weather and Climate Data: Collect weather and climate data for the regions or countries involved in the food market. Weather conditions, including rainfall, temperature, droughts, and natural disasters, can significantly impact agricultural production and subsequently affect food prices.

5. Trade Policies and Agreements: Monitor changes in government policies, trade agreements, and regulations related to food imports and exports. Adjustments in tariffs, quotas, subsidies, or trade restrictions can affect food prices by altering the supply-demand balance.

6. Consumer Behavior and Preferences: Analyze consumer behavior, income levels, population growth, dietary shifts, and cultural factors that may impact food consumption patterns. Changes in consumer preferences and purchasing power can influence food prices for specific categories or commodities.

Sources of Uncertainty and Estimating Forecast Uncertainty:

Forecasting food prices involves inherent uncertainty due to various factors. Some sources of uncertainty include:

1. Volatility in Commodities: Food prices can be influenced by the volatility of underlying commodity markets, such as grain prices, oil prices (affecting transportation costs), and other key agricultural inputs. These market fluctuations introduce uncertainty into food price forecasts.

2. Geopolitical Events: Political instability, conflicts, or trade disputes can disrupt food supply chains and impact prices. Geopolitical events are difficult to predict, and their outcomes can introduce considerable uncertainty into food price forecasts.

3. Climate Variability: Weather patterns and natural disasters, such as droughts, floods, or extreme weather events, can significantly affect crop yields and agricultural production. The uncertainty associated with climate variability can make food price forecasts challenging.

4. Unforeseen Events: Unexpected events, such as disease outbreaks (e.g., pandemics affecting labor availability or livestock health), technological disruptions, or policy changes, can introduce uncertainty into food markets and price forecasts.

• To estimate the uncertainty of the forecast, one approach is to use confidence intervals. By applying statistical techniques, you can calculate upper and lower bounds around the forecasted food prices, providing a range of potential outcomes. Confidence intervals provide a measure of uncertainty and indicate the level of confidence in the forecast.

• Additionally, scenario analysis can be employed to assess the uncertainty. By considering different scenarios based on varying assumptions and key factors, you can evaluate a range of potential outcomes and their associated risks. Sensitivity analysis can also help identify the key variables that have a significant impact on the forecasted food prices, allowing for a better understanding of the uncertainty involved.

• It's important to note that the accuracy of the forecasted food prices will depend on the quality of the data, the chosen forecasting models/methods, and the assumptions made. Regularly updating the forecast with new data and monitoring changes in relevant factors will help adapt and refine the forecast as conditions evolve, further reducing uncertainty.
