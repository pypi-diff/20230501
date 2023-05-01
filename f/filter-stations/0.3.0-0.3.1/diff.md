# Comparing `tmp/filter_stations-0.3.0.tar.gz` & `tmp/filter_stations-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.0.tar", last modified: Sat Apr 29 12:06:19 2023, max compression
+gzip compressed data, was "filter_stations-0.3.1.tar", last modified: Mon May  1 20:36:30 2023, max compression
```

## Comparing `filter_stations-0.3.0.tar` & `filter_stations-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:06:19.743750 filter_stations-0.3.0/
--rw-rw-rw-   0        0        0     3488 2023-04-29 12:06:19.741482 filter_stations-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3182 2023-03-12 12:07:13.000000 filter_stations-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 12:06:19.697460 filter_stations-0.3.0/filter_stations/
--rw-rw-rw-   0        0        0    25062 2023-04-29 11:36:52.000000 filter_stations-0.3.0/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:06:19.734594 filter_stations-0.3.0/filter_stations.egg-info/
--rw-rw-rw-   0        0        0     3488 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 12:06:19.744752 filter_stations-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-29 12:02:47.000000 filter_stations-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:36:30.372008 filter_stations-0.3.1/
+-rw-rw-rw-   0        0        0    39900 2023-05-01 20:36:30.369020 filter_stations-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    39594 2023-05-01 20:35:50.000000 filter_stations-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 20:36:30.267863 filter_stations-0.3.1/filter_stations/
+-rw-rw-rw-   0        0        0    33665 2023-05-01 19:30:40.000000 filter_stations-0.3.1/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:36:30.357811 filter_stations-0.3.1/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0    39900 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:36:30.373007 filter_stations-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-05-01 20:36:19.000000 filter_stations-0.3.1/setup.py
```

### Comparing `filter_stations-0.3.0/filter_stations/__init__.py` & `filter_stations-0.3.1/filter_stations/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,23 +14,15 @@
 import base64
 import json
 from folium.plugins import MeasureControl
 import os
 import datetime
 import gc
 
-# try:
-#     # Load json cofig file
-#     with open('config.json') as f:
-#         conf = json.load(f)
-
-#     apiKey = conf['apiKey']
-#     apiSecret = conf['apiSecret']
-# except FileNotFoundError:
-#     raise("Please create a config.json file with your API key and secret")
+
 # Constants
 API_BASE_URL = 'https://datahub.tahmo.org'
 API_MAX_PERIOD = '365D'
 
 endpoints = {'VARIABLES': 'services/assets/v2/variables', # 28 different variables
              'STATION_INFO': 'services/assets/v2/stations',
              'WEATHER_DATA': 'services/measurements/v2/stations', # Configured before requesting
@@ -69,34 +61,57 @@
         )
         if apiRequest.status_code == 200:
             return apiRequest.json()
         else:
             return self.__handleApiError(apiRequest)
     
     def get_stations_info(self, station=None, multipleStations=[], countrycode=None):
+        """
+        Retrieves information about weather stations from an API endpoint and returns relevant information based on the parameters passed to it.
+
+        Args:
+            station (str, optional): Code for a single station to retrieve information for. Defaults to None.
+            multipleStations (list, optional): List of station codes to retrieve information for multiple stations. Defaults to [].
+            countrycode (str, optional): Country code to retrieve information for all stations located in the country. Defaults to None.
+
+        Returns:
+            pandas.DataFrame: DataFrame containing information about the requested weather stations.
+
+        """
+        # Make API request and convert response to DataFrame
         response = self.__request(endpoints['STATION_INFO'], {'sort':'code'})
         info = pd.json_normalize(response['data']).drop('id', axis=1)
+        
+        # Filter DataFrame based on parameters
         if station:
             return info[info['code'] == station.upper()]
         elif len(multipleStations) >= 1:
             return info[info['code'].isin(multipleStations)]
         elif countrycode:
             info = info[info['location.countrycode'] == f'{countrycode.upper()}']
             return info.drop(labels=info['code'][info.code.str.contains('TH')].index, axis=0)
         else:
             return info
+
         
-    # retrieve available variables
     def get_variables(self):
+        """
+        Retrieves information about available weather variables from an API endpoint.
+
+        Returns:
+            dict: Dictionary containing information about available weather variables, keyed by variable shortcode.
+        """
+        # Make API request and create dictionary of variables
         response = self.__request(endpoints['VARIABLES'], {})
         variables = {}
         if 'data' in response and isinstance(response['data'], list):
             for element in response['data']:
                 variables[element['variable']['shortcode']] = element['variable']
         return variables
+
     
      # Split date range into intervals of 365 days.
     def __splitDateRange(self, inputStartDate, inputEndDate):
         try:
             startDate = dateutil.parser.parse(inputStartDate)
             endDate = dateutil.parser.parse(inputEndDate)
         except ValueError:
@@ -113,34 +128,75 @@
         df.loc[0, 'start'] = pd.Timestamp(startDate)
         df['end'].iloc[-1] = pd.Timestamp(endDate)
         return df
     
     def raw_measurements(self, station, startDate=None, endDate=None, variables=None):
         return self.get_measurements(station, startDate=startDate, endDate=endDate, variables=variables, dataset='raw')
     
-    # A dictionary of neighbouring stations
     def k_neighbours(self, station, number=5):
-        '''
-        Pass in a station - return the longitude and latitude from get stations info
-        '''
+        """
+        Returns a dictionary of the nearest neighbouring stations to the specified station.
+
+        Args:
+            station (str): Code for the station to find neighbouring stations for.
+            number (int, optional): Number of neighbouring stations to return. Defaults to 5.
+
+        Returns:
+            dict: Dictionary containing the station codes and distances of the nearest neighbouring stations.
+        """
+        # Get latitude and longitude of specified station
         lon, lat = self.get_stations_info(station)[['location.longitude', 'location.latitude']].values[0]
+        
+        # Calculate distances to all other stations and sort by distance
         infostations = self.get_stations_info()
         infostations['distance'] = infostations.apply(lambda row: hs.haversine((lat, lon), (row['location.latitude'], row['location.longitude'])), axis=1)
         infostations = infostations.sort_values('distance')
-        return  dict(infostations[['code', 'distance']].head(number).values[1:])
+        
+        # Create dictionary of nearest neighbouring stations and their distances
+        return dict(infostations[['code', 'distance']].head(number).values[1:])
+
     
-    # Pure aggregates
     def aggregate_variables(self, dataframe):
+        """
+        Aggregates a pandas DataFrame of weather variables by summing values across each day.
+
+        Args:
+            dataframe (pandas.DataFrame): DataFrame containing weather variable data.
+
+        Returns:
+            pandas.DataFrame: DataFrame containing aggregated weather variable data, summed by day.
+        """
+        # Reset index and rename columns
         dataframe = dataframe.reset_index()
-        dataframe.rename(columns = {'index':'Date'}, inplace = True)
-        return dataframe.groupby(pd.Grouper(key='Date', axis=0, 
-                        freq='1D')).sum()
+        dataframe.rename(columns={'index':'Date'}, inplace=True)
+        
+        # Group by date and sum values
+        return dataframe.groupby(pd.Grouper(key='Date', axis=0, freq='1D')).sum()
+
     
     # Get the variables only
     def get_measurements(self, station, startDate=None, endDate=None, variables=None, dataset='controlled', aggregate=False):
+            """
+            Get measurements for a specified station and time period.
+
+            :param station: The station ID for which to retrieve measurements.
+            :type station: str
+            :param startDate: The start date of the time period for which to retrieve measurements.
+            :type startDate: datetime or str, optional
+            :param endDate: The end date of the time period for which to retrieve measurements.
+            :type endDate: datetime or str, optional
+            :param variables: A list of variable shortcodes to retrieve measurements for. If None, all variables are retrieved.
+            :type variables: list or None, optional
+            :param dataset: The dataset to retrieve measurements from. Default is 'controlled'.
+            :type dataset: str, optional
+            :param aggregate: Whether to aggregate variables by sensor ID. Default is False.
+            :type aggregate: bool, optional
+            :return: A Pandas DataFrame containing the requested measurements.
+            :rtype: pandas.DataFrame
+            """
             #print('Get measurements', station, startDate, endDate, variables)
             endpoint = 'services/measurements/v2/stations/%s/measurements/%s' % (station, dataset)
 
             dateSplit = self.__splitDateRange(startDate, endDate)
             series = []
             seriesHolder = {}
 
@@ -252,14 +308,31 @@
             if aggregate:
                 return self.aggregate_variables(df)
             else:
                 return df
     
     # retrieve data from multiple at a time
     def multiple_measurements(self, stations_list, csv_file, startDate, endDate, variables, dataset='controlled'):
+        """
+        Retrieves measurements for multiple stations and saves the aggregated data to a CSV file.
+
+        Parameters:
+            stations_list (list): A list of strings containing the names of the stations to retrieve data from.
+            csv_file (str): The name of the CSV file to save the data to.
+            startDate (str): The start date for the measurements, in the format 'yyyy-mm-dd'.
+            endDate (str): The end date for the measurements, in the format 'yyyy-mm-dd'.
+            variables (list): A list of strings containing the names of the variables to retrieve.
+            dataset (str): The name of the dataset to retrieve the data from. Default is 'controlled'.
+
+        Returns:
+            df (pandas.DataFrame): A DataFrame containing the aggregated data for all stations.
+
+        Raises:
+            ValueError: If stations_list is not a list.
+        """
         error_dict = dict()
         if isinstance(stations_list, list):
             df_stats = []
             
             for station in stations_list:
                 print(stations_list.index(station))
                 try:
@@ -290,14 +363,27 @@
         super().__init__(apiKey, apiSecret)
     
     def get_stations_info(self, station=None, multipleStations=[], countrycode=None):
         return super().get_stations_info(station, multipleStations, countrycode)
         
     # Get the centre point of the address
     def getLocation(self, address):
+        """
+        This method retrieves the latitude and longitude coordinates of a given address using the Nominatim API.
+        
+        Parameters:
+        -----------
+        address : str
+            The address of the location you want to retrieve the coordinates for.
+            
+        Returns:
+        --------
+        Tuple (float, float)
+            The latitude and longitude coordinates of the location.
+        """
         url = 'https://nominatim.openstreetmap.org/search/' + urllib.parse.quote(address) +'?format=json'
         return requests.get(url).json()[0]['lat'], requests.get(url).json()[0]['lon']
 
     # Get the new radius of the address
     def calculate_new_point(self, lat, lon, distance, bearing):
         """
         Calculate a new point given a starting point, distance, and bearing.
@@ -330,27 +416,51 @@
         lon2 = math.degrees(lon2)
         
         return lat2, lon2
     
 
     # Get the bounding box of the address
     def compute_filter(self, lat, lon, distance):
+        """
+        Calculates the bounding box coordinates for a given location and distance.
+
+        Parameters:
+        lat (float): The latitude of the location.
+        lon (float): The longitude of the location.
+        distance (float): The distance from the location, in kilometers, to the edge of the bounding box.
+
+        Returns:
+        A tuple containing four floats representing the bounding box coordinates: (min_lat, min_lon, max_lat, max_lon).
+        """
         points = []
         g1 = []
         for i in range(0, 360, 45):
             points.append(self.calculate_new_point(lat, lon, distance, i))
         g1 = [min(p[0] for p in points), min(p[1] for p in points)]
         g2 = [max(p[0] for p in points), max(p[1] for p in points)]
         # print(g1, '\n', g2)
         return g1[0], g1[1], g2[0], g2[1]
 
     # Get the minimum and maximum latitude and longitude of the address
 
 
-    def filterStations(self, address, distance, startDate=None, endDate=None, csvfile='KEcheck3.csv'):     
+    def filterStations(self, address, distance, startDate=None, endDate=None, csvfile='KEcheck3.csv'):
+        """
+        This method filters weather station data within a certain distance from a given address.
+        
+        Parameters:
+        address (str): Address to center the bounding box around.
+        distance (float): The distance (in kilometers) from the center to the edge of the bounding box.
+        startDate (str): The start date for filtering the weather station data in the format 'YYYY-MM-DD'.
+        endDate (str): The end date for filtering the weather station data in the format 'YYYY-MM-DD'.
+        csvfile (str): The name of the csv file containing the weather station data.
+        
+        Returns:
+        pandas.DataFrame: The filtered weather station data within the bounding box.
+        """     
         lat, lon = self.getLocation(address)
         min_lat, min_lon, max_lat, max_lon = self.compute_filter(float(lat), float(lon), distance)
         stations = super().get_stations_info()
         bounds = list(stations['code'][(stations['location.longitude'] >= min_lon)
                                         & (stations['location.longitude'] <= max_lon)
                                         & (stations['location.latitude'] >= min_lat)
                                             & (stations['location.latitude'] <= max_lat)])
@@ -370,27 +480,48 @@
             ke_chec = ke_chec.set_index('Date')
 
             return ke_chec[[col for bbox in bounds for col in ke_chec if bbox in col]]
         else:
             ke_chec = ke_chec.set_index('Date')
             return ke_chec[[col for bbox in bounds for col in ke_chec if bbox in col]]
 
+
     # A list of filtered stations
     def filterStationsList(self, address, distance=100):
+        """
+        Filters stations based on their proximity to a given address and returns a list of station codes that fall within the specified distance.
+        
+        Args:
+            address (str): Address to filter stations by.
+            distance (float, optional): Maximum distance (in kilometers) between the stations and the address. Default is 100 km.
+        
+        Returns:
+            List of station codes that fall within the specified distance from the given address.
+        """
         return list(set([i.split('_')[0] for i in self.filterStations(f'{address}', distance).columns if i.split('_')[-1] != 'clogFlag']))
 
     
 
 # A different class for visualisations
 class Interactive_maps(retreive_data):
     # inherit from retrieve_data class
     def __init__(self, apiKey, apiSecret):
         super().__init__(apiKey, apiSecret)
 
     def draw_map(self, map_center):
+        """
+        Creates a Folium map centered on the specified location and adds markers for each weather station in the area.
+
+        Args:
+            map_center: a tuple with the latitude and longitude of the center of the map
+
+        Returns:
+            A Folium map object
+        """
+
         #  retrieve the stations data
         stations = super().get_stations_info()[['code', 'location.longitude', 'location.latitude']]
         # create a map centered on a specific location
 
         my_map = folium.Map(location=map_center, min_zoom=5, max_zoom=30, zoom_start=12, tiles='cartodbpositron')
         for _, row in stations.iterrows():
             folium.Marker([row['location.latitude'], row['location.longitude']], tooltip=row['code']).add_to(my_map)
@@ -402,16 +533,25 @@
 
         # display the map
         return my_map
 
 
     def create_animation(self, data, valid_sensors, day=100, T=10, interval=500):
         '''
-        T days giving the range 
-        valid sensors
+        Creates an animation of pollutant levels for a given range of days and valid sensors.
+
+        Parameters:
+        data (DataFrame): A pandas DataFrame containing pollution data.
+        valid_sensors (list): A list of valid sensor names.
+        day (int): The starting day of the animation (default is 100).
+        T (int): The range of days for the animation (default is 10).
+        interval (int): The interval between frames in milliseconds (default is 500).
+
+        Returns:
+        HTML: An HTML object containing the animation.
         '''
         
         data1 = np.array(data[valid_sensors].iloc[day:day+1]).T
         data1 /= np.max(data1)
         # Create figure and axis
         fig, ax = plt.subplots()
 
@@ -432,25 +572,26 @@
         # Create animation
         ani = animation.FuncAnimation(fig, update, frames=range(T), interval=interval, blit=False)
         plt.close()
 
         return HTML(ani.to_jshtml())
 
 
-    '''
-    1. Get the stations information
-    2. From the points given get the map center
-    3. Get a max and min zoom for the map
-    4. Place the data in a map with a certain colour
-    5. a different marker for a different subset of the data
-    6. Pass an argument for the start and end date
-    7. Generate plots for each station for the given date range and add them to the map as a popup on click
-    8. Create a slider to change the day on the plots 
-    '''
     def plot_station(self, ws, df_rainfall):
+        """
+        Plot the rainfall data for a specific weather station.
+
+        Args:
+        - ws: string, the code of the weather station to plot
+        - df_rainfall: DataFrame, a pandas DataFrame with rainfall data
+
+        Returns:
+        - None if no data is available for the specified station
+        - a Matplotlib figure showing rainfall data for the specified station otherwise
+        """
         # filter columns based on station code and type (sensor or clog flag)
         sensors = [x for x in list(df_rainfall.keys()) if ws in x and 'clog' not in x]
         clog_flags = [x for x in list(df_rainfall.keys()) if ws in x and 'clog' in x]
 
         # check if any data is present
         if not sensors and not clog_flags:
             return None
@@ -476,14 +617,24 @@
         plt.suptitle('Rainfall data for sensors and clog flags at station {}'.format(ws))
         plt.close()
         return fig
 
 
     # Encode the image
     def encode_image(self, ws, df_rainfall):
+        """
+        Encodes a station's rainfall data plot as a base64-encoded image.
+
+        Args:
+        - ws (str): the code for the station to encode the image for
+        - df_rainfall (pandas.DataFrame): a DataFrame containing the rainfall data for all stations
+        
+        Returns:
+        - str: a string containing an HTML image tag with the encoded image data, or a message indicating no data is available for the given station
+        """
         figure = self.plot_station(ws, df_rainfall)
         if figure is not None:
             figure.tight_layout()
             buf = BytesIO()
             figure.savefig(buf, format='png')
             plt.close() # close the figure object to remove the subplot
             buf.seek(0)
@@ -492,14 +643,45 @@
             return '<img src="data:image/png;base64,{}">'.format(image_data)
         else:
             return 'No data available for station {}'.format(ws)
 
 
 
     def get_map(self, subset_list, start_date=None, end_date=None, data_values=False, csv_file='KEcheck3.csv', min_zoom=8, max_zoom=11, width=850, height=850, png_resolution=300):
+        """
+        Creates a Folium map showing the locations of the weather stations in the given subsets.
+
+        Parameters:
+        -----------
+        subset_list : list of lists of str
+            List of subsets of weather stations, where each subset is a list of station codes.
+        start_date : str, optional
+            Start date in the format YYYY-MM-DD, default is None.
+        end_date : str, optional
+            End date in the format YYYY-MM-DD, default is None.
+        data_values : bool, optional
+            If True, the map markers will display a plot of rainfall data, default is False.
+        csv_file : str, optional
+            The name of the CSV file containing the rainfall data, default is 'KEcheck3.csv'.
+        min_zoom : int, optional
+            The minimum zoom level of the map, default is 8.
+        max_zoom : int, optional
+            The maximum zoom level of the map, default is 11.
+        width : int, optional
+            The width of the map in pixels, default is 850.
+        height : int, optional
+            The height of the map in pixels, default is 850.
+        png_resolution : int, optional
+            The resolution of the PNG image if data_values is True, default is 300.
+
+        Returns:
+        --------
+        my_map : folium.folium.Map
+            A Folium map object showing the locations of the weather stations in the given subsets.
+        """
         # Read the csv file 
         df_rainfall = pd.read_csv(csv_file)
         df_rainfall['Date'] = pd.to_datetime(df_rainfall['Date'])
         df_rainfall= df_rainfall.set_index('Date')
         if start_date and end_date:
             df_rainfall = df_rainfall[start_date:end_date]
```

### Comparing `filter_stations-0.3.0/setup.py` & `filter_stations-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

