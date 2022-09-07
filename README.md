![airbnb](https://user-images.githubusercontent.com/102264298/186799347-d7ea854f-8468-4c05-b0ba-84d27bad17b3.png)

# Hawaii_Airbnb_Data_Analysis
## Why invest in Aribnb Hawaii
Hawaii is one of the premiere destinations on the Planet. According to Hawaii's Department of Business, Economic Development and Tourism(DBEDT), the State of Hawaii received a total of 842,927 visitors during the month of June 2022. Tourism plays a significant role in the Hawaii's economy and investing in Airbnb Hawaii can be a financial windfall for residents and non-residents alike. There are more and more people considering purchasing a second house or investment property to rent out to tourists as an Airbnb business.  

## Overview
The purpose of this analysis is to facilitate decision making on consideration for running a short term rental property in the area.  Short term rentals offer a unique alternative to traditional hotel/motel stays and present the opportunity for a property owner to generate income from an otherwise unoccupied residence or room.  Utilizing several datasets taken from Inside Airbnb (http://insideairbnb.com/get-the-data) for Hawaii, the goal is to answer several questions pertinent to entry into the short term rental business model.

### Questions to answer:
1. Which neighborhoods have the most rental properties, and which neighborhoods generate the most revenue?
2. Which property/room type is booked most often?
3. What are the most influential factors (amenities) for drawing rentals and commanding a higher pricepoint?
4. When is the peak season for rentals, and when can maintenance and repairs be performed?

### Methods utilized:
1. Data cleaning and preprocessing - Pandas, Jupyter Notebook
2. Data storage and queries - PGAdmin, SQL, AWS
3. Modeling and Learning - Simple Linear Regression
4. Visualizations - Tableau, Wordcloud

### External Links

[Interactive Tableau Dashboard1](https://public.tableau.com/authoring/hawaii_airbnb/HawaiiAirbnb#1)

[Interactive Tableau Dashboard2](https://public.tableau.com/app/profile/sharon3357/viz/HawaiiAirbnb_16623379982290/HawaiiAirbnb)

[Link to Google Slides](https://docs.google.com/presentation/d/1k1sqCg5IGoMQEcSsKaAKfR8khjJH_nL3eLUeeSi4Bgk/edit?usp=sharing)](https://docs.google.com/presentation/d/1r6uzFeajACkauZkifVMawIDFXFesPJ2sTc0j8t99m_A/edit?usp=sharing)


### Data Exploration
* Raw data from four csv files and one geoJSON file from the Inside Airbnb source
  * Listings.csv.gz with Detailed Listings data
  * Calendar.csv.gz with Detailed Calendar data
  * Reviews.csv.gz with Detailed Review data
  * Neighbourhoods.csv as a list for geo filter sourced from open source GIS files
  * Neighbourhoods.geojson as a GeoJSON file of selected neighborhoods
* Utilized Pandas with Jupyter Notebook to clean and preprocess data
  * Dropped repetitive and non-contextual columns
  * Replaced or eliminated null values
  * Generated csv files from the cleaned DataFrames
  * Imported csv files to PGAdmin to populate tables for SQL 

### Data Analysis
* Plotted GeoJSON file with geopandas
  * Plotted scatter of listings on top with lat/long
* Grouped neighborhoods and plotted bar chart of most popular neighborhoods in bar chart
* Grouped room types and plotted pie chart of most popular room types
* Generated word clouds of amenities listings and review mentions frequency
* Grouped reviews by month with count to plot bar chart of bookings per month

## Results

* Which neighborhoods have the most rental properties, and which neighborhoods generate the most revenue?

  Primary Urban Center contains the most rental properties, followed by Lahaina and Kihei-Makena areas. 
  
![neighbourhoods](https://user-images.githubusercontent.com/102264298/186802324-d686e9e2-ad33-4333-b241-1cc350ad1d2b.png)

* Which property/room type is booked most often?

  Entire home/apt is the most often booked room type. 
  
![room_type](https://user-images.githubusercontent.com/102264298/186802332-7e835d95-4502-44d6-a80c-f00d191087a4.png)

* What are the most influential factors (amenities) for drawing rentals and commanding a higher pricepoint?
  
  From the wordcloud picture, it shows that hot water, long-term stay, free parking, smoke alarm, are most influential amenities when customers seeking a rental home.   
  
![amenities_wordcloud](https://user-images.githubusercontent.com/102264298/186802347-52045096-ef60-4d07-917d-b4636caab7f3.png)

* When is the peak season for rentals, and when can maintenance and repairs be performed?

  From the bar chart, we can see that there is not significant difference between each month. As a result, Hawaii is good for rental all year around.  Maintenance  and repairs can be performed in February. 

![month booking](https://user-images.githubusercontent.com/102264298/186802318-f3fba198-1726-42ae-a0c9-59424b0c1244.png)


## ML Model Diagram
![ML_diagram](https://user-images.githubusercontent.com/102084269/186306268-c0643af7-7124-4ae7-a29f-c00225032c66.png)

## ML Overview
Regression model with "Price" as the target.  Features include Bedrooms, Number of Reviews, Review Scores Rating, Availability, Neighborhood Group, Neighborhood, and Rental Type.
![Screen Shot 2022-08-27 at 5 43 15 PM](https://user-images.githubusercontent.com/98665941/187050523-a44f4dc7-a646-4f13-bb8d-0b9dbcca0de9.png)

Scaled data and utilized PCA

![Screen Shot 2022-08-27 at 5 46 55 PM](https://user-images.githubusercontent.com/98665941/187050590-209dca57-867a-4817-952d-ee5160d4cf3e.png)

Determined K clusters of 4 with an Elbow Curve

![Screen Shot 2022-08-27 at 5 49 37 PM](https://user-images.githubusercontent.com/98665941/187050636-349f0749-d9ff-4bcb-824d-6174d08b2b8b.png)

Predicted clusters and added predicted classes

![Screen Shot 2022-08-27 at 6 12 03 PM](https://user-images.githubusercontent.com/98665941/187051067-407b20a1-234f-4c50-94e5-c95c3ed91f38.png)

![Screen Shot 2022-08-27 at 6 15 51 PM](https://user-images.githubusercontent.com/98665941/187051159-9f2c371f-a9e2-4a36-bcf8-2d16a74e5fb6.png)



