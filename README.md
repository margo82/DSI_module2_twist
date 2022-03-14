# DSI_module2_twist

# London bike shared analyses

We have 2 years of hourly data of bike shared in London. 
Acknowledge: Contains OS data © Crown copyright and database rights 2016' and Geomni UK Map data © and database rights [2019]

The data has a series of features as below:
- "timestamp" - timestamp field for grouping the data
- "cnt" - the count of a new bike shares
- "t1" - real temperature in C
- "t2" - temperature in C "feels like"
- "hum" - humidity in percentage
- "windspeed" - wind speed in km/h
- "weathercode" - category of the weather
- "isholiday" - boolean field - 1 holiday / 0 non holiday
- "isweekend" - boolean field - 1 if the day is weekend
- "season" - category field meteorological seasons: 0-spring ; 1-summer; 2-fall; 3-winter.

"weathe_code" category description:
- 1 = Clear ; mostly clear but have some values with haze/fog/patches of fog/ fog in vicinity 
- 2 = scattered clouds / few clouds
- 3 = Broken clouds
- 4 = Cloudy
- 7 = Rain/ light Rain shower/ Light rain
- 10 = rain with thunderstorm
- 26 = snowfall
- 94 = Freezing Fog

The data have been loaded into a database (using sqlite3 in python)
We have added hourly data of pollution in London: NO, NO2, NOx, PM10. 

After some Exploratory Data Analysis, we fitted a LSTM model to the data to try to predict the number of bike share hourly.

We have used python widget to plot the data and load them using **voila**. 
Then open a command line and type `voila London_Bike_Dashboard.ipynb` 
