# CropYieldAnalysisIndia
Analysis of Crop Yield Trends Across Indian States


Introduction:
Agriculture plays an important role in India’s growth and economy,  understanding how crop yields change over time is important for improving food security and promoting sustainable farming. This project, “Analysis of Crop Yield Trends Across Indian States” looks at how different factors like rainfall, temperature, fertilizer and pesticide use, and overall climate affect crop production in various parts of India. By predicting crop yields more accurately, farmers can make better decisions about which crops to grow, how to use resources wisely, and how to avoid losses. It also helps the government create better policies, offer targeted support, and manage food supply more effectively.
With challenges like climate change and uneven use of farming inputs, this project uses data science to study past agricultural data. The goal is to discover patterns, understand what affects crop yields the most, and see how yields vary across states and over time. In the end, the insights from this analysis can help both farmers and policymakers make informed choices, boost productivity for Indian agriculture.

Dataset:
For my project, I have selected three datasets that together provide a full view of how different factors influence crop yields across India.
The first dataset includes all the details about agricultural information from 1997 to 2020, which covers crop types, seasons, states, production, rainfall, fertilizer and pesticide use, and yield. This is the core dataset for analysing trends in crop performance over time.
The second dataset provides historical temperature data from the year 1991 to 2020 which  helps me understand how weather conditions impact crop growth in different regions and years.
The third dataset shows India’s climate zones by state,  which gives me a broader picture of the typical climate in each region. This helps link long-term weather patterns with the kinds of crops grown there.
To combine everything, I merged the agricultural data with the temperature and climate datasets by matching state names. This allowed me to line up crop yield data with the corresponding climate conditions and zone types for each state. As a result, I created a combined dataset that makes it easier to analyse how factors like rainfall, temperature, and input usage (like fertilizers and pesticides) affect crop yields across different temperature and  climate zones.
This integration helps me find meaningful patterns, make comparisons across regions, and better understand what influences crop productivity which supports decision making for both farmers and policymakers.




The core dataset has the following features:

•	Crop: The type of crop that was grown.
•	Crop Year: The year the crop was cultivated.
•	Season: The farming season when the crop was planted, like Kharif, Rabi, or throughout the year.
•	State: The Indian state where the crop was grown.
•	Area: The amount of land (in hectares) used to grow the crop.
•	Production: The total amount of the crop produced (in metric tons).
•	Annual Rainfall: The total rainfall (in millimetres) received in the area where the crop was grown.
•	Fertilizer: The amount of fertilizer (in kilograms) used on the crop.
•	Pesticide: The amount of pesticide (in kilograms) used during cultivation.
•	Yield: The crop output per unit of land—basically, how much crop was produced per hectare.
•	Annual Average Temperature: The average yearly temperature in a region.
•	Climatic Classification: The type of climate a region has based on long-term weather patterns.


Tools:

•	Python
•	Tableau
•	Jupiter Notebook
•	Word

Data Cleaning:

1.	Removed duplicate values to make sure there are no repeated records in the dataset.
2.	Checked for missing values, and found that there were no null values in the dataset.
3.	Applied log transformation to reduce skewness in certain numeric columns like Area, Production, Annual Rainfall, Fertilizer, Pesticide, and Yield.
4.	Saved the cleaned and pre-processed dataset in both CSV and Excel formats for future analysis.
This process has helped to prepare the data for better and more accurate analysis.






Exploratory Data Analysis:

 

Info for the dataset, used for data exploration
 

Checking for null values, output before data cleaning
 

Statistical summary for numerical columns. 

 

 

The histogram graphs show how the data is spread after using a log transformation. Most features, like area, production, rainfall, fertilizer, and pesticide, now have a balanced, bell-shaped curve, which is good for analysis. Also, we can see that the yield graph is a bit left-skewed which means that high yields are more common than low ones.








1.	Which Year has the highest average yield across states and how is the trend of yield from 1997 to 2019?

 

 

Result:

The above graph Average Yield Over the Years shows how the average yield changed from 1997 to 2020 we can see that the year with the highest average yield was 2014, where the yield peaked at 108 which indicates a very productive year across states.

From 1997 to 2014, the average yield generally increased, with some small ups and downs along the way. After reaching its peak in 2014, the yield started to drop slightly, but it remained fairly stable between 2015 and 2019 with values around 74 to 83.








2.	Which state has the most COVID-19 deaths across all years for “All Sexes” and “All Ages”

 

 

Result:

The above bar graph shows average yield by state. We can see that the top 5 states with highest average yield are Goa, Puducherry, Kerala, West Bengal and Tamil Nadu which is ranging from 250-350 production per unit area. We can see that Sikkim, Jammu and Kashmir and Himachal Pradesh has the least yield possibly due to their rocky surface area type and colder climatic conditions.












Hypothesis

1.	What is the percentage contribution of each Indian state to the total crop yield, and which states have the highest and lowest yields over the years?
2.	Is there a strong correlation between annual rainfall and crop yield across different states in India?
3.	How does the use of fertilizers and pesticides affect crop yield across the years?
4.	How does the average crop yield compare across different temperature zones?
5.	Is there a significant difference in crop yield between states with different climatic classifications (e.g., arid, semi-arid, tropical).
6.	How is the yield across various crops in India, which crop has the highest yield and    lowest yield.

Graph-breakthrough-Result

Geographical Map

A geographical map is used to show data based on different places, like states or regions. It helps us easily see patterns or trends by using location points like latitude and longitude.

 


The map visualization is achieved by using geographic states and with their latitude and longitude and ‘Yield’ attribute onto the Text marks and changing the ‘Quick table calculation’ to the ‘Percent of Total’. Furthermore, ‘Yield’ attribute is added to the colour marks and
selected the ‘Sunrise-sunset diverging’ for the colour on the map. And also ‘State’ Attribute is added to Text marks to display the state name.




Result:

The above map visualization depicts the % of the total Yield in every state in India. We can see that the southern states has recorded more yield comparatively than the northern states which may be due to climatic conditions and annual rainfall. We can see that West Bengal has highest yield recorded with18.55% of total, followed by Puducherry, Andhra Pradesh, Assam, Karnataka, Kerala, Goa and Telangana. We can see that Sikkim, Jammu and Kashmir and Himachal Pradesh has recorded lowest yield across states.

Vertical bar Graph:
A vertical bar graph helps compare different categories by displaying data as bars. It makes it easy to see how each category performs in comparison to others.
 
This vertical bar graph visualization is achieved by using states, crop yield and different type of crop categories. I have State names in colour marks filtering all the Indian states, arranged in descending order of crop yield and the filter can be used to filter crop and crop yield by state.

Result:
This chart shows the yield levels of different crops across various states. From the bar graph, we can see that some states consistently have higher yields compared to others for particular crops. We cans see that Sugarcane, Potato, Coconut, Rice and Maize are top 5 crops which had most yield over the years and we can see that certain states are doing better in producing crops like Rice and Wheat, while others have comparatively lower yields and we can see that costal regions have most yield of coconuts and the lowest yielded crop is Cardamom. The overall pattern highlights how yield levels can vary based on factors like climate, soil type, and farming practices in each state. This kind of information can help in focusing improvements on states and crops that need support.

Tree maps:

Tree maps use rectangles to display data, with the size of each rectangle representing a quantity. The colours help show trends or performance, making it easy to compare different parts of a whole.

 


This tree map is achieved by using sum of yield in size marks making the visualisation in square using marks column. I have used yield in colour marks to clearly categorise yield in years. To get clear information from the visualisation, I have put yield attribute in text marks by calculating percentage of total.

Result:
The above tree map visualisation provides information about the total crop yield across different years. The size of each rectangle represents the total yield for that year, we can see  that 2014 which is covering the largest area has 6.57% of the total yiel which makes it the year with the highest contribution. Other years like 2013, 2015, 2016, and 2019 also show significant portions, each contributing over 5% of the total yield.
Years like 1997, 1998, and 1999 have much smaller rectangles which tells that those years have lower yield contributions, with 1997 being the lowest. The colour helps to differentiate between the yield levels, moving from green (lower yield) to dark orange (higher yield) which makes it easy to spot which years performed better in terms of agricultural production.
This tree map highlights how crop yields have varied over the years, with certain years consistently performing better than others. The clear dominance of 2014 suggests favourable farming conditions or policies during that time, while lower-yield years could indicate challenges such as poor weather, pests, or other farming issues. Overall, it provides a quick visual comparison of agricultural productivity over the years.
Line Chart:

A line chart uses points connected by lines to display data, often showing changes over time. It helps track patterns and compare values, with time or categories on the x-axis and data values on the y-axis.

 

This line graph is done using the crop year attribute in the column, the sum of yield attribute in rows, to differentiate different age groups clearly, I have used colour marks for the crop type attribute and to indicate the yield across years.

Result:
This line chart shows how crop yield for various changed over time for different crops. The x-axis represents years, while the y-axis indicates the total crop yield filtering top 5 crops Sugarcane, Potato, Coconut, Rice, Maize. From the graph, it can be seen that  the yield across those crops is growing gradually over the years which tells about improving in farming techniques to grow these crops.









Analysis of crop yield across various crops and their Fertiliser and Pesticide usage across different states of India using dashboard


 


The above visualisation is achieved using the dashboard feature. By using the drag and drop feature, the previously made analysis graphs were placed into a dashboard. To do this, I have selected the sheets which I have made earlier and added them into the dashboard. Then, I have added an action filter for Yield Across States sheets with the other sheets as target. This feature allows us to select any state in the Yield Across States sheet and then automatically Yield across various crops, Pesticide Usage and Fertilizer Usage tabs gets updated with that specific state. This resulting visualisation dashboard gives information on the percentage of total yield yield across various crops and their Fertiliser and Pesticide usage across different states of India.
 


Result:

When I select West Bengal which has highest yield across all other Indian States, we can see that coconut, potato, sugarcane, rice, maize and jute are the top grown crops in the state which has high yield and the below two tabs shows pesticide and fertilizer usage in the state which is 291987 and 291,987 respectively


 


Result:

This dashboard output gives information about the yield across South Indian states like Telangana, Karnataka, Andhra Pradesh, Tamil Nadu, Kerala and Puducherry . From the dashboard, we can see that that Coconut, Sugarcane, Onion, Rice, Tapioca, Potato, Banana, Sweet Potato, Maize and Ragi were the top 10 crops which have the highest yield across these states. The below tabs in the dashboard represents the usage of pesticide and fertilizer across years where the darker shade of blue represents high yield. We can see that Karnataka, Andhra Pradesh, Tamil Nadu, Telangana, Kerala and Puducherry are the states in descending order of fertilizer and pesticide usage. Here Even through Karnataka is using more fertilizer and pesticide for their crops, the crop yield is not as much as Andhra Pradesh, Tamil Nadu and even through Puducherry is using less fertilizer and pesticide, it has more crop yield than any other south Indian state which tells about the climatic conditions and water availability in that region.








Yield Vs Fertilizer and Pesticide Usage Across Years

        


Result:
The graph shows how much fertilizer and pesticide was used over the years, and how it compares to the crop yield. Fertilizer use has slowly gone up every year and is now over 16 billion kilograms. Pesticide use went down until 2008 and was about 8 million kilograms at that time. After 2008, it started going up again and is now more than 35 million kilograms.

Pesticide and Fertilizer Usage

   


Result:
The above graphs shows the Pesticide and Fertilizer usage Across the States, We can see that Utter Pradesh, Madhya Pradesh, Maharashtra, Karnataka and West Bengal were top 5 states which use more Fertilizer and Pesticides, here we can see that even through Utter Pradesh, Madhya Pradesh and Maharashtra is using more fertilizer and pesticides, their yield is comparatively less than other states like Karnataka, Andhra Pradesh, West Bengal and Tamil Nadu who uses less Fertilizers and Pesticides. Which tells that other factors like temperature, rainfall and soil type also contribute to yield.
Yield Across Climatic Classification
The bar graph below gives the log yield value across different states for each climatic classification. India has 7 different climatic conditions which are spread across various states which are:
1.	Tropical Monsoon Climate (Andaman and Nicobar Islands, Goa, Kerala) – These areas get heavy rainfall during the monsoon and have warm temperatures throughout the year. The rain is important for farming.
2.	Tropical Savanna Climate (Andhra Pradesh, Gujarat, Karnataka, etc.) – These places have a wet monsoon season and a dry, hot season. Farming depends on the rainfall during the wet season.
3.	Humid Subtropical Climate (Arunachal Pradesh, Assam, Bihar, etc.) – These regions experience hot summers and mild winters with moderate rainfall. Many types of crops grow here due to good rainfall.
4.	Arid Steppe Climate (Rajasthan, Jammu and Kashmir, Ladakh) – These areas are very dry with little rainfall and big temperature changes. Farmers need to use irrigation to grow crops.
5.	Highland Temperate Climate (Himachal Pradesh, Sikkim, Uttarakhand) – Found in mountains, these regions are cooler with different seasons. Summers are cool, and winters can be very cold.
6.	Mediterranean Climate (Tamil Nadu) – Hot and dry summers with mild, wet winters. It’s good for crops like fruits and vegetables that need a dry season.
7.	Tundra Climate (Ladakh) – Very cold with long winters and short, cool summers. Only hardy plants can grow in this region because of the extreme cold.
 
We can see that areas with Tropical Savanna and Humid Subtropical climates have higher crop yields. In contrast, places with Arid Steppe climates produce about half as much. The other climate types show even lower crop yields.
Rainfall and Yield
   

The above scatter plots shows that states with Humid Subtropical and Tropical Savanna climates receive a medium amount of rainfall, typically between 1250 to 1750 mm per year, and these regions also have the highest crop yields. From the first scatter plot, it is clear that states with very low or extremely high rainfall tend to have lower yields, which could be due to drought in dry regions or flooding in areas with too much rain. States like Telangana, Karnataka, Andhra Pradesh, Tamil Nadu, Kerala, West Bengal, and Puducherry, which receive around 1000 to 2000 mm of annual rainfall, show better crop production compared to others. This suggests that moderate rainfall is ideal for healthy crop growth. When rainfall is either too little or too much, it negatively affects farming. Therefore, balanced climate conditions with rainfall in the range of 1000 to 2000 mm per year appear to be best suited for agriculture in India.








Temperature vs Yield
 
The above scatter plot shows how temperature affects crop yield in India. It is clear that the ideal temperature range for good crop growth is between 20°C and 30°C. States with average temperatures above 25°C, like many in central and southern India, tend to have higher yields. On the other hand, states like Jammu and Kashmir, Sikkim, and Himachal Pradesh, which have lower average temperatures, show lower yields. This suggests that moderate to warm temperatures are better for farming. Extremely cold conditions may not support high crop production.





Discussion
•	West Bengal recorded the highest crop yield contribution at 18.55%, followed by Puducherry, Andhra Pradesh, Assam, Karnataka, Kerala, Goa, and Telangana.
•	States with the lowest crop yields include Sikkim, Jammu and Kashmir, and Himachal Pradesh, likely due to colder temperatures and rocky terrain.
•	Moderate annual rainfall between 1000 mm and 2000 mm is ideal for crop growth, as seen in states like Andhra Pradesh, Telangana, and West Bengal.
•	Very low or extremely high rainfall tends to reduce yield, possibly due to drought or flooding affecting farming conditions.
•	Fertilizer and pesticide usage has increased over the years, but higher usage does not always lead to higher yields, indicating the influence of other environmental factors.
•	States like Tamil Nadu and Puducherry have high yields despite using less fertilizer and pesticides, suggesting favourable climate and water availability.
•	An ideal temperature range for crop growth is between 20°C and 30°C, with warmer states showing higher yields than colder regions.
•	States with Humid Subtropical and Tropical Savanna climates generally show higher yields, whereas Arid Steppe and Tundra regions show lower productivity.
•	Among all crops, Sugarcane, Potato, Coconut, Rice, and Maize have the highest yields across states.
•	Cardamom has the lowest yield, likely due to its limited growing regions and specific climatic requirements.
•	Crop yield trends peaked in 2014, showing the highest productivity, while earlier years like 1997–1999 had much lower outputs.
•	Overall, factors like climate type, temperature, rainfall, and crop variety strongly influence yield more than fertilizer and pesticide use alone.
Conclusion
This project has provided valuable information on the key factors that influence crop yield across different Indian states. Through detailed analysis of historical data, it is clear that climate conditions, especially rainfall and temperature, play a major role in determining crop productivity. From the analysis, we can determine that moderate rainfall and temperatures between 20°C to 30°C were found to be most suitable for higher yields. While fertilizer and pesticide usage has increased over the years, high input levels do not always lead to better output which highlights the importance of balanced farming practices. 

From the analysis, we can see that certain crops like Sugarcane, Potato, Coconut, Rice, and Maize consistently have higher yields, and states with favourable climates like West Bengal, Andhra Pradesh, and Puducherry perform better overall. By understanding these patterns, farmers can plan more effectively, and policymakers can provide better support and resources to areas that need them most. Overall, this project demonstrates how data-driven insights can help improve agricultural planning, promote sustainable farming, and support food security across India.





References:

1.	Agricultural crop yield in Indian States dataset. (2023b, July 17). Kaggle. https://www.kaggle.com/datasets/akshatgupta7/crop-yield-in-indian-states-dataset

2.	India climate zone, weather by month and historical data. (n.d.). https://weatherandclimate.com/india

3.	World Bank Climate Change Knowledge Portal. (n.d.-b). https://climateknowledgeportal.worldbank.org/country/india/climate-data-historical

4.	Wikipedia contributors. (2025, April 18). Agriculture in India. Wikipedia. https://en.wikipedia.org/wiki/Agriculture_in_India






