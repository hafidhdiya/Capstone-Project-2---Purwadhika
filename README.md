# <H1><center>**Capstone Project 2 - NYC TLC Trip Record**
# <H4><center>**By Hafidh Diya Ulhaqi Dewantoro**
---
---

# <H2> **BACKGROUND**
The New York City Taxi and Limousine Commission (TLC), created in 1971, is the agency responsible for licensing and regulating New York City's Medallion (Yellow) taxi cabs, for-hire vehicles (community-based liveries, black cars and luxury limousines), commuter vans, and paratransit vehicles.

The company is dedicated on expanding its taxi service user base. Through a targeted business strategy, tailored to the characteristics of taxi users, the aim is to attract a larger audience and solidify the company's position in the transportation industry.

To achieve this goal, understanding customer behavior is crucial. Analyzing the travel records will help bridge the gap in the company's knowledge about the characteristics and preferences of green taxi users. By delving into this dataset, the company can unveil patterns and extract valuable insights that will inform a targeted and effective business strategy.

The company aims to enhance its understanding of taxi user behavior to formulate effective business strategies that will lead to an increase in the number of taxi users. In the transportation industry, optimizing operations and increasing profitability hinges on satisfying customers by comprehending their demand patterns, time and area preferences, and the benefits (specifically, comfortability) provided to them.


## **Problem Statement**
Exploratory Questions:

1. Demand Variability:

    - Pick-up Time:
        - What are the peak hours of demand for taxi services?
        - How does demand fluctuate during different times of the day?

    - Pick-up Zone and Preferences:
        - Which areas exhibit the highest demand for taxi services?
        - Are there specific pick-up zones preferred by users?
        - How do user preferences influence demand patterns?


2. Revenue by Travel Zones and Routes:

    - Travel Zones:
        - What are the revenue trends across different travel zones?
        - Are there particular zones that contribute significantly to overall revenue?
    
    - Routes:
        - Which routes are most profitable for the company?
        - Are there certain routes that attract higher fares and more users?


3. Factors Influencing Tip Amount:

    - User Experience:
        - How does the level of comfort provided influence the amount of tip given?
        - Are there specific aspects of the service that correlate with higher tips?

## **Goals**
Our goal is delivering strategies to stakeholders in helping them increasing profitability by:

1. Optimizing vehicle distribution based on the customer's demands for operational cost efficiency.

2. Understanding and fulfilling customer's needs and preferences in increasing their loyalty and satisfaction.

3. Maximizing revenue through strategic travel zone and route exploration.

## **Project Assumptions and Limitations:**
1. One trip represents one different person

2. Do not enter trips under 0.2mill or 60seconds (Limit is charged per meter)

3. There is no age limit for people using taxis

4. Upper taxi speed limit is 40 mph.

5. Using recorded data in January 2023

6. Taxi operates in NYC Borough and outside the city.

## **Summary of Data Cleaning**

The data cleaning process has been carried out by doing:

1. Handling the missing/Null values
    
    - Dropping unrelevant and unuseful columns (`ehail_fee` and `store_and_fwd_flag`) to the analysis

    - Filling the missing values 

2. Adjusting the data types

    - Changing the `lpep_pickup_datetime` and `lpep_dropoff_datetime` data type to the datetime type

    - Changing `passenger_count` data type to integer type

3. Handling the outliers

    - Dropping the negative data, which is the duplicate of the positive data, by seeing the recorded data in date and location columns.

    - Dropping 3 rows contained negative values in mta_tax, improvement_surcharge, and total_amount column.

    - Limiting data to Janury 2023 only for analysis.
    
    - Handling outliers in `passenger_count`, `RatecodeID`, `trip_distance`, `fare_amount`, `trip_duration_minute`, `vehicle_speed`, `tip_amount` by referring to the regulatioins.

Note : All the assumptions for the data cleaning process refers to NYC government regulations and conditions.

The results of the data cleaning process left **65781** data by cutting **3.56%** from the initial data.

## **Analysis Highlights**

1. Demand Variability:

Pick-up Zone and Preferences:

Identify areas with the highest demand for taxi services by analyzing historical data and user patterns.
Explore if there are specific pick-up zones that users prefer, and if so, strategize to optimize service in those areas.

Pick-up Time:

Determine the peak hours of demand for taxi services to allocate resources efficiently.
Study how demand fluctuates during different times of the day to enhance operational planning and meet user needs effectively.

2. Revenue by Travel Zones and Routes:

Travel Zones:

Examine revenue trends across various travel zones to identify potential growth areas and areas that may need additional marketing efforts.
Identify specific zones that significantly contribute to overall revenue, allowing for targeted business strategies.

Routes:

Analyze profitability on different routes to optimize resource allocation and potentially adjust service offerings based on high-demand routes.

3. Tipping Patterns:

By Time (Day and Hour) within a Week:

Investigate tipping patterns to understand user behavior and preferences.
Analyze tipping data based on both the day of the week and specific hours, providing insights for drivers and the company to enhance service during peak tipping times.

Explore the interactive Tableau dashboard ([Here](https://www.nyc.gov/assets/tlc/downloads/pdf/driver_education_study_guide.pdf](https://public.tableau.com/app/profile/hafidh.diya/viz/CapstoneProject2_17071212301240/Story1)https://public.tableau.com/app/profile/hafidh.diya/viz/CapstoneProject2_17071212301240/Story1))
