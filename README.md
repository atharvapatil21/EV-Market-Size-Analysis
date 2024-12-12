# EV-Market-Size-Analysis
Market size analysis is a crucial aspect of market research that determines the potential sales volume within a given market. It helps businesses understand the magnitude of demand, assess market saturation levels, and identify growth opportunities.
## Project Overview : 
The Electric Vehicles Market Size Analysis project will involve collecting, cleaning, and analyzing data to understand the current and projected market size of electric vehicles. The analysis will cover global, regional, and country-specific markets, identifying key trends, growth drivers, and strategic opportunities. The final deliverables will include a detailed report with actionable recommendations and a series of visualizations to communicate findings effectively.

## Tools and Technologies : 
- Python: For data analysis and visualization.
- Pandas and NumPy: For data manipulation and analysis.
- Matplotlib, Seaborn, and Plotly: For creating visualizations.
-  Jupyter Notebooks: For interactive data analysis and reporting.

## Dataset Description : 
We will use this dataset for the analysis:  Electric_Vehicle_Population_Data.csv

### EV Population Data: 
- Dataset Name: Electric Vehicle Population Data
- Source: User-uploaded dataset containing detailed information about electric vehicles, including their make, model, year, type, electric range, and location.
- Citation: This dataset is provided by the user and includes data on various attributes of electric vehicles, such as VIN, county, city, state, postal code, model year, make, model, electric vehicle type, clean alternative fuel vehicle eligibility, electric range, base MSRP, legislative district, DOL vehicle ID, vehicle location, electric utility, and 2020 census tract.

### Problem statements : 
1. Define whether the analysis is global, regional, or focused on specific countries.
2. Gather information from industry associations, market research firms (e.g., BloombergNEF, IEA), and government publications relevant to the EV market.
3. Use historical data to identify trends in EV sales, production, and market.
4. Analyze the market size and growth rates for different EV segments.
5. Based on the market size analysis, provide strategic recommendations for businesses looking to enter or expand in the EV market.

## Step-by-Step Analysis
•	Importing Necessary Libraries and Loading Data - Begin by importing essential libraries such as pandas, matplotlib, seaborn, numpy, and the curve fit function from scipy.optimize. Load the dataset to start the analysis.



•	Data Cleaning - Ensure the dataset is clean by handling missing values and verifying appropriate data types. This step is crucial for accurate analysis.






 #### For the task of market size of electric vehicles analysis, we can explore the following areas:

- EV Adoption Over Time: Analyze the growth of the EV population by model year.
- Geographical Distribution: Understand where EVs are most commonly registered (e.g., by county or city).
- EV Types: Breakdown of the dataset by electric vehicle type (BEV, etc.).
- Make and Model Popularity: Identify the most popular makes and models among the registered EVs.
- Electric Range Analysis: Analyze the electric range of vehicles to see how EV technology is progressing.
- Estimated Growth in Market Size: Analyze and find the estimated growth in the market size of electric vehicles.

#### Let’s start with analyzing the EV Adoption Over Time by visualizing the number of EVs registered by model year. It will give us an insight into how the EV population has grown over the years


![3](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/7a0a7c95-3fe5-40bf-86dc-64cc65f3df9a)

From the above bar chart, it’s clear that EV adoption has been increasing over time, especially noting a significant upward trend starting around 2016. The number of vehicles registered grows modestly up until that point and then begins to rise more rapidly from 2017 onwards. The year 2023 shows a particularly sharp increase in the number of registered EVs, with the bar for 2023 being the highest on the graph, indicating a peak in EV adoption.

#### Now, let’s start by selecting the top 3 counties based on EV registrations and then analyze the distribution of EVs within the cities of those counties:

![4](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/cdc509e1-a48f-461b-add5-e01ebfe1ecad)

The above graph compares the number of electric vehicles registered in various cities within three counties: King, Snohomish, and Pierce. The horizontal bars represent cities, and their length corresponds to the number of vehicles registered, colour-coded by county. Here are the key findings from the above graph:

Seattle, which is in King County, has the highest number of EV registrations by a significant margin, far outpacing the other cities listed.
Bellevue and Redmond, also in King County, follow Seattle with the next highest registrations, though these are considerably less than Seattle’s.
Cities in Snohomish County, such as Kirkland and Sammamish, show moderate EV registrations.
Tacoma and Tukwila, representing Pierce County, have the fewest EV registrations among the cities listed, with Tacoma slightly ahead of Tukwila.
The majority of cities shown are from King County, which seems to dominate EV registrations among the three counties.
Overall, the graph indicates that EV adoption is not uniform across the cities and is more concentrated in certain areas, particularly in King County.

#### Next, let’s explore the types of electric vehicles represented in this dataset. Understanding the breakdown between different EV types, such as Battery Electric Vehicles (BEV) and Plug-in Hybrid Electric Vehicles (PHEV), can provide insights into consumer preferences and the adoption patterns of purely electric vs. hybrid electric solutions. So, let’s visualize the distribution of electric vehicle types to see which categories are most popular among the registered vehicles:



 ![5](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/1273e006-d3d0-4f4b-bc80-8713f08eae3a)

The above graph shows that BEVs are more popular or preferred over PHEVs among the electric vehicles registered in the United States.

Let’s now focus on the popularity of electric vehicle manufacturers and models among the registered vehicles. This analysis will help us identify which manufacturers and specific models dominate the EV market, potentially indicating consumer preferences, brand loyalty, and the success of various manufacturers’ strategies in promoting electric mobility.

#### So, let’s have a look at the most popular manufacturers and then drill down into the most popular models within those manufacturers:

# analyzing the popularity of EV manufacturers

![6](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/39ff8b9e-53d2-4967-8932-fe2c03655961)

The above chart shows that:

TESLA leads by a substantial margin with the highest number of vehicles registered.
NISSAN is the second most popular manufacturer, followed by CHEVROLET, though both have significantly fewer registrations than TESLA.
FORD, BMW, KIA, TOYOTA, VOLKSWAGEN, JEEP, and HYUNDAI follow in decreasing order of the number of registered vehicles.

#### Next, let’s drill down into the most popular models within these top manufacturers to get a more detailed understanding of consumer preferences at the model level:


![7](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/dc020512-f6ff-4b2b-a042-89bbdffd9fea)

The above graph shows the distribution of electric vehicle registrations among different models from the top three manufacturers: TESLA, NISSAN, and CHEVROLET. Here are the findings:

TESLA’s MODEL Y and MODEL 3 are the most registered vehicles, with MODEL Y having the highest number of registrations.
NISSAN’s LEAF is the third most registered model and the most registered non-TESLA vehicle.
TESLA’s MODEL S and MODEL X also have a significant number of registrations.
CHEVROLET’s BOLT EV and VOLT are the next in the ranking with considerable registrations, followed by BOLT EUV.
NISSAN’s ARIYA and CHEVROLET’s SPARK have the least number of registrations among the models shown.

#### Next, we’ll explore the electric range of vehicles, which is a critical factor for analyzing the market size of electric vehicles. The electric range indicates how far an EV can travel on a single charge, and advancements in battery technology have been steadily increasing these ranges over the years. So, let’s look at the distribution of electric ranges in the dataset and identify any notable trends, such as improvements over time or variations between different vehicle types or manufacturers:


![8](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/2b59e36d-4066-4e4c-b02d-0ae8a61131a8)

The above graph shows the mean electric range. Key observations from the graph include:

There is a high frequency of vehicles with a low electric range, with a significant peak occurring just before 50 miles.
The distribution is skewed to the right, with a long tail extending towards higher ranges, although the number of vehicles with higher ranges is much less frequent.
The mean electric range for this set of vehicles is marked at approximately 58.84 miles, which is relatively low compared to the highest ranges shown in the graph.
Despite the presence of electric vehicles with ranges that extend up to around 350 miles, the majority of the vehicles have a range below the mean.
It suggests that while there are EVs available with high electric ranges, the average range is skewed lower due to a substantial number of vehicles with shorter ranges.

Now, let’s delve into the trend of electric ranges over model years, which can provide insights into how advancements in battery technology and vehicle design have influenced the electric range capabilities of electric vehicles over time. A positive trend in this analysis would indicate continuous improvements, offering consumers EVs with longer driving ranges and potentially addressing one of the major concerns regarding the EV market (range anxiety):


![9](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/61e82194-1253-4cd7-8304-314b3234201e)

The above graph shows the progression of the average electric range of vehicles from around the year 2000 to 2024. Key findings from the graph:

There is a general upward trend in the average electric range of EVs over the years, indicating improvements in technology and battery efficiency.
There is a noticeable peak around the year 2020 when the average range reaches its highest point.
Following 2020, there’s a significant drop in the average range, which could indicate that data for the following years might be incomplete or reflect the introduction of several lower-range models.
After the sharp decline, there is a slight recovery in the average range in the most recent year shown on the graph.
The data suggest that while there have been fluctuations, the overall trend over the last two decades has been toward increasing the electric range of EVs.

Next, let’s explore how electric ranges vary among the top manufacturers and models. This analysis can reveal how different manufacturers are addressing the crucial aspect of electric range and highlight which models stand out for their superior range capabilities:



![10](https://github.com/aniket3096/Electric_Vehicles_Market/assets/164318183/9bdd5099-568d-4232-a84c-ed33b93e08b7)

The TESLA ROADSTER has the highest average electric range among the models listed. TESLA’s models (ROADSTER, MODEL S, MODEL X, and MODEL 3) occupy the majority of the top positions, indicating that on average, TESLA’s vehicles have higher electric ranges. The CHEVROLET BOLT EV is an outlier among the CHEVROLET models, having a substantially higher range than the VOLT and S-10 PICKUP from the same maker. NISSAN’s LEAF and CHEVROLET’s SPARK are in the lower half of the chart, suggesting more modest average ranges.

#### Estimated Market Size Analysis of Electric Vehicles in the United States
Now, let’s move forward towards finding the estimated market size of electric vehicles in the United States. I’ll first count the number of EVs registered every year:



![WhatsApp Image 2024-07-25 at 3 10 35 PM](https://github.com/user-attachments/assets/d50193e6-e4fb-4bd9-98ef-7c0758c5b9e6)

The dataset provides the number of electric vehicles registered each year from 1997 through 2024. However, the data for 2024 is incomplete as it only contains the data till March. Here’s a summary of EV registrations for recent years:

In 2021, there were 19,063 EVs registered.
In 2022, the number increased to 27708 EVs.
In 2023, a significant jump to 57,519 EVs was observed.
For 2024, currently, 7,072 EVs are registered, which suggests partial data.
To forecast the total number of EVs expected to be registered in 2024, we can use a growth rate based approach from previous complete years.

We’ll calculate the Compound Annual Growth Rate (CAGR) between a recent year with complete data (2023) and an earlier year to project the 2024 figures. Additionally, using this growth rate, we can estimate the market size for the next five years. Let’s proceed with these calculations:



![WhatsApp Image 2024-07-25 at 3 14 38 PM](https://github.com/user-attachments/assets/1f52f081-27f9-427c-a583-2a2abba4bc5b)

Now, let’s plot the estimated market size data:


![WhatsApp Image 2024-07-25 at 3 17 33 PM](https://github.com/user-attachments/assets/5dd7aced-cdb1-4421-abef-210805e0f371)

From the above graph, we can see:

The number of actual EV registrations remained relatively low and stable until around 2010, after which there was a consistent and steep upward trend, suggesting a significant increase in EV adoption.
The forecasted EV registrations predict an even more dramatic increase in the near future, with the number of registrations expected to rise sharply in the coming years.
Given the growing trend in actual EV registrations and the projected acceleration as per the forecast data, we can conclude that the EV market size is expected to expand considerably. The steep increase in forecasted registrations suggests that consumer adoption of EVs is on the rise, and this trend is likely to continue. Overall, the data point towards a promising future for the EV industry, indicating a significant shift in consumer preferences and a potential increase in related investment and business opportunities.

### Summary :
So, market size analysis is a crucial aspect of market research that determines the potential sales volume within a given market. It helps businesses understand the magnitude of demand, assess market saturation levels, and identify growth opportunities. From our market size analysis of electric vehicles, we found a promising future for the EV industry, indicating a significant shift in consumer preferences and a potential increase in related investment and business opportunities.

### Thank you 

