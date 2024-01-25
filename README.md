# Data Visualization in Biycle Renting

Some kind of experiments for data visualization purposes. The aim is to draw meaningful conclusions from data using visualization techniques. Bicycle rental data was used for this. After using some data manipulation techniques, the data was visualized both with various graphs and on the map.

## Prerequisites

All you need to run is described in the jpynb file. They are also shared below:

```python
import pandas as pd
import geopandas as gpd
import matplotlib.pyplot as plt
from shapely.geometry import Point, LineString
from matplotlib.lines import Line2D
import folium
```

## Dataset

[Main source](https://www.kaggle.com/datasets/benhamner/sf-bay-area-bike-share) have four datasets, but I used just three of them:

1. Data_trip (Contains data about individual bike trips. Such as starting station id, ending
station id, date and time, duration, bike id.)
2. Data_stations (Contains data that represents a station where users can pickup or return
bikes. Most important one of the features of data is location information of stations.)
3. Data_weather (Contains data about the weather on a specific day for certain zip codes.
Such as temperature, event (rainy, foggy, etc.), dew point)
4. Data_status (Contains data about the number of bikes and docks available for given
station and minute. I didn’t use this data.)

[Data source of map](https://geodata.ucdavis.edu/gadm/gadm4.1/json/gadm41_USA_2.json.zip)