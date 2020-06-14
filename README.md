#                               FordGoBike Data(2018) Analysis
### by Nishu Jain

## Dataset

__Bay Wheels__ (previously known as Ford GoBike) is a regional public bicycle sharing system in the San Francisco Bay Area,
Bay Wheels is the first regional and large-scale bicycle sharing system deployed in California and on the West Coast of the United States. It was established as Bay Area Bike Share in August 2013. As of January 2018, the Bay Wheels system had over 2,600 bicycles in 262 stations across San Francisco, East Bay and San Jose. On June 28, 2017, the system officially re-launched as Ford GoBike in a partnership with Ford Motor Company. After Motivate's acquisition by Lyft, the system was subsequently renamed to Bay Wheels in June 2019. The system is expected to expand to 7,000 bicycles around 540 stations in San Francisco, Oakland, Berkeley, Emeryville, and San Jose.

Ford GoBike, like other bike share systems, consists of a fleet of specially designed, sturdy and durable bikes that are locked into a network of docking stations throughout the city. The bikes can be unlocked from one station and returned to any other station in the system, making them ideal for one-way trips. People use bike share to commute to work or school, run errands, get to appointments or social engagements and more. It's a fun, convenient and affordable way to get around.

![alt text](https://github.com/nishujain95/FordGoBike_Data_Analysis/blob/master/bikebay.jpg "Logo Title Text 1")

You can download the dataset from [baywheels-data](https://s3.amazonaws.com/baywheels-data/index.html)

## Data Wrangling Process

- There are missing values in columns(start_station_id, start_station_name, end_station_id, end_station_name)
- Incorrect data types in following column names:
  - start_time should be of datetime format
  - end_time should be of datetime format
  - start_station_id should be of object type
  - end_station_id should be of object type
  - bike_id should be of object type
  - user_type should be of category type
  - bike_share_for_all_trip should be of category type
- Add new columns (start_month,start_month_num,start_weekday,start_hour,end_hour,duration_min)

## Project Findings

- We have observed an analysis on user types with respect to hour,day,month of travel.  
- We got to note that on weekends we can see a more variation in trips throughout the day.  
- We can see that the customers have the higher average trip duration as compared to the subscribers.

## Resources 

- [pandas documentation](https://pandas.pydata.org/docs/)
- [matplotlib tutorials](https://matplotlib.org/tutorials/index.html)
- [seaborn tutorial](https://seaborn.pydata.org/tutorial.html)
- [glob](https://docs.python.org/3/library/glob.html)
- [stackoverflow](https://stackoverflow.com/questions/)
- [Data Visualization](https://blog.insightdatascience.com/data-visualization-in-python-advanced-functionality-in-seaborn-20d217f1a9a6)
- [color palettes](https://seaborn.pydata.org/tutorial/color_palettes.html)
