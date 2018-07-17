THIS IS ONE OF THE FINAL PROJECTS OF MIPT & YANDEX MACHINE LEARNING COURSERA COURSE


Forecasting of a time series on a geographic map

The task of this project is to learn how to predict the number of trips for the next few hours in each district of 
New York. In order to solve it, raw data must be aggregated by hours and areas. Aggregated data will be the hourly time 
series with the number of trips from each district. Similar tasks arise in practice, if you need to forecast sales of 
a large number of products in a large number of stores, the amount of cash withdraw in the ATM network, site traffic etc.

The New York Taxi and Limousine Commission (TLC) provides detailed anonymous data on customer travel since 2009. Yellow 
cars are given permission to take passengers on the streets in any of the five boroughs of the city. 

Raw data on trips in a yellow taxi can be found on the TLC website: 
www.nyc.gov/html/tlc/html/about/trip_record_data.shtml 
This data is divided into files by months. Each file contains the following information about trips:

• start time of the trip
• end time of the trip
• Longitude and latitude of the starting point of the trip
• Longitude and latitude of the end point of the trip
• number of passengers
• distance over the counter
• type of tariff (one of six categories)
• payment method (one of six categories)
• cost of the trip by the meter
• tax on the counter
• surcharge for trips during peak hours and at night
• surcharge for tolls on toll roads
• fare paid for each trip from January 2015
• size of tips
• total cost of the trip
• Data provider (one of two categories)
• A binary flag indicating whether the train data was received immediately after its completion, or for some time was 
  stored in the vehicle's memory.

More information: http://www.nyc.gov/html/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf

The task of the project is to learn how to predict the number of trips in the next few hours in every district of New 
York; for simplicity, we define rectangular regions. In order to solve it, raw data must be aggregated by hours and 
areas. Aggregated data will be the hourly time series with the number of trips from each district.
The task of predicting such series can be solved using autoregressive models, predicting each series independently. 
The series clearly have a complex seasonality - daily, weekly and yearly, so to model them you will need to use the 
ARIMA model with an additional regression to external characteristics.

To improve this model, you can try to take into account:

• relationships between series
• additional travel parameters that can be calculated from the source data
• external calendar and geographical signs

In the course of the project, you will learn:

• work with location data
• predict time series of a complex structure
• build and customize regression models that make joint predictions for a large number of interconnected series

Similar tasks arise in practice, if you need to forecast sales of a large number of goods in a large number of stores,
the amount of cash withdraw in the ATM network, site traffic etc.

You will have the freedom to choose which analysis tools, libraries and models to use. 
Also note that for its successful accomplishment you will need to download and process from 10 to 200 gigabytes of 
raw data.
