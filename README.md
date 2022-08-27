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

### Communication protocols:
We worked on the project as a group during class, and updated the status of the project through Slack and weekend zoom meetups. 
#### Team member role: 
* Ryan: Created the flowchart for the Machine Learning Model, generated a wordcloud for reviews, edit the README.
* James: Cleaned the inicial CSV file and created wordcloud and neiborhood notebook, and edit the README.
* John: Stored the database in SQL and created tables in PGAdmin using CSVs and edit the README.
* Sharon: Created github branch for each team member and cleaned the dataframe, converted approriate datatype and edit the README.

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
