# Viz_Project_Data_Wizards
## Data Visualizations on NYC dataset
### Garima Garg (garimag2@illinois.edu), Paulami Ray(paulami2@illinois.edu), Kumkum Yadav(kumkumy2@illinois.edu)

The data represents the list of Citi Bikers in New York. It tells us when do they ride, how far do they go, which stations are the most popular and also what days of the week are the most rides taken on. For more information on the dataset columns please refer file : Dataset_Part1.
The dataset is uploaded here as a .zip file.
You can obtain the dataset from https://s3.amazonaws.com/tripdata/index.html. The name of the dataset on that site is 201712-citibike-tripdata.csv.zip. It is an open source data the data policy can be seen here : https://www.citibikenyc.com/data-sharing-policy .

## File size
The file size of this dataset is 155,622 Kb. The number of rows in this dataset are 889,968. The number of columns are 15 which have been defined above.

## Tools Used:
Python has been used to analyze the dataset and visualize the plots.

## Libraries Used :
1) matplotlib
2) ipywidgets
3) bokeh
4) folium maps
5) vincent
6) haversine
7) bqplot

## Files explanation:
The dataset has 3 important files:
1) Cleaned.files is used to clean the dataset from the site. Perform various operations like 
a) convert column with dates into datetime format
b) replaces na values in the birth year column with the mode of the column
c) more columns like day, hour and age were added
d) calculated speed and distance using haversine. 
2) Understanding the dataset : We have made many plots to understand the basic nature of the dataset. Some of the plots are mentioned below:
a) Population of bike riders by Gender
b) Population of bike riders by Usertype whether they are Subscribers or Customers
c) Number of trips per day
d) Number of trips per station
e) Number of bikes leaving a station id
f) Number of trips with a given end date (interactive graph)
g) Added HandDraw, Panzoom, FastIntervalSelector, IndexSelector, BrushIntervalSelector, MultiSelector and None.
h) Distance covered by age and gender
i) Average biker speed by age and gender
j) Number of trips per hour corresponding to start station
k) Number of trips per hour corresponding to start and end station
3) Interactive Maps on the Biker data: Here we used the folium package to provide some insights into the dataset. The maps drwan are :
a) Trips density of each station based on arrival and departure by hour.
b) Interactive map using start and end stations with hours and tiles option
c) Heat Map using Speed and Day of the Week
