# Comparing `tmp/weatherly-0.5.0.tar.gz` & `tmp/weatherly-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherly-0.5.0.tar", last modified: Sun Apr 30 21:53:06 2023, max compression
+gzip compressed data, was "weatherly-0.5.1.tar", last modified: Mon May  1 20:54:00 2023, max compression
```

## Comparing `weatherly-0.5.0.tar` & `weatherly-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.542178 weatherly-0.5.0/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1076 2023-04-14 20:22:17.000000 weatherly-0.5.0/LICENSE
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2996 2023-04-30 21:53:06.542178 weatherly-0.5.0/PKG-INFO
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1929 2023-04-30 21:48:52.000000 weatherly-0.5.0/README.rst
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       38 2023-04-30 21:53:06.542178 weatherly-0.5.0/setup.cfg
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1919 2023-04-27 19:25:17.000000 weatherly-0.5.0/setup.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.534179 weatherly-0.5.0/weatherly/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)      783 2023-04-30 21:49:20.000000 weatherly-0.5.0/weatherly/__init__.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    21660 2023-04-30 21:31:00.000000 weatherly-0.5.0/weatherly/abc.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.542178 weatherly-0.5.0/weatherly/api/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1227 2023-04-30 21:49:39.000000 weatherly-0.5.0/weatherly/api/__init__.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    19278 2023-04-30 21:37:57.000000 weatherly-0.5.0/weatherly/api/client.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2657 2023-04-23 19:24:58.000000 weatherly-0.5.0/weatherly/api/core.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     4488 2023-04-16 21:05:46.000000 weatherly-0.5.0/weatherly/enums.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     3905 2023-04-30 21:01:53.000000 weatherly-0.5.0/weatherly/errors.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    31591 2023-04-30 21:45:33.000000 weatherly-0.5.0/weatherly/responses.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2798 2023-04-27 19:47:53.000000 weatherly-0.5.0/weatherly/utils.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.538179 weatherly-0.5.0/weatherly.egg-info/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2996 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/PKG-INFO
--rw-rw-r--   0 konrad    (1000) konrad    (1000)      383 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/SOURCES.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)        1 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/dependency_links.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       90 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/requires.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       10 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/top_level.txt
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-01 20:54:00.023852 weatherly-0.5.1/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1076 2023-04-14 20:22:17.000000 weatherly-0.5.1/LICENSE
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2996 2023-05-01 20:54:00.015852 weatherly-0.5.1/PKG-INFO
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1929 2023-04-30 21:48:52.000000 weatherly-0.5.1/README.rst
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)       38 2023-05-01 20:54:00.023852 weatherly-0.5.1/setup.cfg
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1919 2023-04-27 19:25:17.000000 weatherly-0.5.1/setup.py
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-01 20:53:59.995852 weatherly-0.5.1/weatherly/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)      783 2023-05-01 20:51:14.000000 weatherly-0.5.1/weatherly/__init__.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)    15796 2023-05-01 20:30:07.000000 weatherly-0.5.1/weatherly/abc.py
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-01 20:54:00.015852 weatherly-0.5.1/weatherly/api/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1227 2023-04-30 21:49:39.000000 weatherly-0.5.1/weatherly/api/__init__.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)    19278 2023-04-30 21:37:57.000000 weatherly-0.5.1/weatherly/api/client.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2657 2023-04-23 19:24:58.000000 weatherly-0.5.1/weatherly/api/core.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     4488 2023-04-16 21:05:46.000000 weatherly-0.5.1/weatherly/enums.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     3905 2023-04-30 21:01:53.000000 weatherly-0.5.1/weatherly/errors.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)    23321 2023-05-01 20:47:09.000000 weatherly-0.5.1/weatherly/responses.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2798 2023-04-27 19:47:53.000000 weatherly-0.5.1/weatherly/utils.py
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-01 20:54:00.011852 weatherly-0.5.1/weatherly.egg-info/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2996 2023-05-01 20:53:59.000000 weatherly-0.5.1/weatherly.egg-info/PKG-INFO
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)      383 2023-05-01 20:53:59.000000 weatherly-0.5.1/weatherly.egg-info/SOURCES.txt
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)        1 2023-05-01 20:53:59.000000 weatherly-0.5.1/weatherly.egg-info/dependency_links.txt
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)       90 2023-05-01 20:53:59.000000 weatherly-0.5.1/weatherly.egg-info/requires.txt
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)       10 2023-05-01 20:53:59.000000 weatherly-0.5.1/weatherly.egg-info/top_level.txt
```

### Comparing `weatherly-0.5.0/LICENSE` & `weatherly-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/PKG-INFO` & `weatherly-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatherly
-Version: 0.5.0
+Version: 0.5.1
 Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
 Home-page: https://github.com/konradsic/weatherly
 Author: konradsic
 License: MIT
 Project-URL: Issues, https://github.com/konradsic/weatherly/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `weatherly-0.5.0/README.rst` & `weatherly-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/setup.py` & `weatherly-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/weatherly/__init__.py` & `weatherly-0.5.1/weatherly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 :license: MIT license, see LICENSE for details
 """
 
 __title__ = 'weatherly'
 __author__ = 'konradsic'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present konradsic'
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 from typing import NamedTuple, Literal
 
 from .api import *
 from .errors import *
 from .enums import *
 from .responses import *
@@ -25,10 +25,10 @@
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     release_type: Literal["alpha", "beta", "candidate", "final"]
     
-version_info = VersionInfo(major=0, minor=5, micro=0, release_type="final")
+version_info = VersionInfo(major=0, minor=5, micro=1, release_type="final")
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `weatherly-0.5.0/weatherly/abc.py` & `weatherly-0.5.1/weatherly/abc.py`

 * *Files 16% similar despite different names*

```diff
@@ -286,16 +286,16 @@
         Chance of rain as percentage
     chance_of_snow: :class:`int`
         Chance of snow as percentage
     gust_mph: :class:`float`
         Wind gust in miles per hour
     gust_kph: :class:`float`
         Wind gust in kilometer per hour
-    uv: :class:`float`
-        UV Index
+    uv: Optional[:class:`float`]
+        UV Index. Can be ``None`` when this class is returned from Future API 
     aqi: Optional[:class:`AirQuality`]
         Air Quality data. See :class:`AirQualityData` for more info.
     """
     time_epoch: int
     time: str
     temp_c: float
     temp_f: float
@@ -325,15 +325,15 @@
     is_day: bool
     vis_km: float
     vis_miles: float
     chance_of_rain: int
     chance_of_snow: int
     gust_mph: float
     gust_kph: float
-    uv: float
+    uv: Optional[float]
 
     aqi: Optional[AirQuality]
     
 
 class ForecastDayModel(ResponseModel):
     """
     An ABC defining a base forecast day model from WeatherAPI
@@ -369,16 +369,16 @@
         Total precipitation in inches
     avgvis_km: :class:`float`
         Average visibility in kilometer
     avgvis_miles: :class:`float`
         Average visibility in miles
     avghumidity: :class:`int`
         Average humidity as percentage
-    uv: :class:`int`
-        UV Index
+    uv: Optional[:class:`float`]
+        UV Index. Can be ``None`` when returned from Future API
     condition_text: :class:`str`
         Weather condition text
     condition_icon: :class:`str`
         Weather condition icon
     condition_code: :class:`int`
         Weather condition code
     hour_data: List[:class:`ForecastHourModel`]
@@ -421,15 +421,15 @@
 
     totalprecip_mm: float
     totalprecip_in: float
 
     avgvis_km: float
     avgvis_miles: float
     avghumidity: int
-    uv: int
+    uv: Optional[float]
 
     condition_text: str
     condition_icon: str
     condition_code: int
     # astro data
     sunrise: Optional[str]
     sunset: Optional[str]
@@ -508,239 +508,25 @@
         A list of forecast days
     alerts: List[:class:`AlertModel`]
         A list of alerts, this list can be empty
     """
     location: LocationModel
     forecast_days: List[ForecastDayModel]
     alerts: List[AlertModel]
-
-class FutureHourModel(ResponseModel):
-    """
-    An ABC defining a base future hour model from WeatherAPI
-
-    The following classes implement this ABC:
-    - :class:`~weatherly.FutureHour`
-
-    Attributes
-    -------------
-    time_epoch: :class:`int`
-        Time as epoch
-    time: :class:`str`
-        Date and time
-    temp_c: :class:`float`
-        Temperature in celsius
-    temp_f: :class:`float`
-        Temperature in fahrenheit
-    condition_text: :class:`str`
-        Weather condition text
-    condition_icon: :class:`str`
-        Weather condition icons
-    condition_code: :class:`int`
-        Weather condition code
-    wind_mph: :class:`float`
-        Maximum wind speed in miles per hour
-    wind_kph: :class:`float`
-        Maximum wind speed in kilometer per hour
-    wind_degree: :class:`int`
-        Wind direction in degrees
-    wind_dir: :class:`str`
-        Wind direction as 16 point compass. e.g.: NSW
-    pressure_mb: :class:`float`
-        Pressure in millibars
-    pressure_in: :class:`float`
-        Pressure in inches
-    precip_mm: :class:`float`
-        Precipitation amount in millimeters
-    precip_in: :class:`float`
-        Precipitation amount in inches
-    humidity: :class:`int`
-        Humidity as percentage
-    cloud: :class:`int`
-        Cloud cover as percentage
-    feelslike_c: :class:`float`
-        Feels like temperature as celcius
-    feelslike_f: :class:`float`
-        Feels like temperature as fahrenheit
-    windchill_c: :class:`float`
-        Windchill temperature in celcius
-    windchill_f: :class:`float`
-        Windchill temperature in fahrenheit
-    headindex_c: :class:`float`
-        Heat index in celcius
-    headindex_f: :class:`float`
-        Heat index in fahrenheit
-    dewpoint_c: :class:`float`
-        Dew point in celcius
-    dewpoint_f: :class:`float`
-        Dew point in fahrenheit
-    will_it_rain: :class:`bool`
-        Will it will rain or not
-    will_it_snow: :class:`bool`
-        Will it will snow or not
-    is_day: :class:`bool`
-        Whether to show day condition icon or night icon
-    vis_km: :class:`float`
-        Visibility in kilometer
-    vis_miles: :class:`float`
-        Visibility in miles
-    chance_of_rain: :class:`int`
-        Chance of rain as percentage
-    chance_of_snow: :class:`int`
-        Chance of snow as percentage
-    gust_mph: :class:`float`
-        Wind gust in miles per hour
-    gust_kph: :class:`float`
-        Wind gust in kilometer per hour
-    """
-    time_epoch: int
-    time: str
-    temp_c: float
-    temp_f: float
-    condition_text: str
-    condition_icon: str
-    condition_code: int
-    wind_mph: float
-    wind_kph: float
-    wind_degree: int
-    wind_dir: str
-    pressure_mb: float
-    pressure_in: float
-    precip_mm: float
-    precip_in: float
-    humidity: int
-    cloud: int
-    feelslike_c: float
-    feelslike_f: float
-    windchill_c: float
-    windchill_f: float
-    headindex_c: float
-    headindex_f: float
-    dewpoint_c: float
-    dewpoint_f: float
-    will_it_rain: bool
-    will_it_snow: bool
-    is_day: bool
-    vis_km: float
-    vis_miles: float
-    chance_of_rain: int
-    chance_of_snow: int
-    gust_mph: float
-    gust_kph: float
     
 
-class FutureDayModel(ResponseModel):
-    """
-    An ABC defining a base future day model from WeatherAPI
-
-    The following classes implement this ABC:
-    - :class:`~weatherly.FutureDay`
-
-    Attributes
-    -------------
-    date: :class:`str`
-        Future date
-    date_epoch: :class:`int`
-        Future date as unix time.
-    maxtemp_c: :class:`float`
-        Maximum temperature in celsius for the day.
-    maxtemp_f: :class:`float`
-        Maximum temperature in fahrenheit for the day
-    mintemp_c: :class:`float`
-        Minimum temperature in celsius for the day
-    mintemp_f: :class:`float`
-        Minimum temperature in fahrenheit for the day
-    avgtemp_c: :class:`float`
-        Average temperature in celsius for the day
-    avgtemp_f: :class:`float`
-        Average temperature in fahrenheit for the day
-    maxwind_mph: :class:`float`
-        Maximum wind speed in miles per hour
-    maxwind_mph: :class:`float`
-        Maximum wind speed in kilometer per hour
-    totalprecip_mm: :class:`float`
-        Total precipitation in milimeter
-    totalprecip_in: :class:`float`
-        Total precipitation in inches
-    avgvis_km: :class:`float`
-        Average visibility in kilometer
-    avgvis_miles: :class:`float`
-        Average visibility in miles
-    avghumidity: :class:`int`
-        Average humidity as percentage
-    condition_text: :class:`str`
-        Weather condition text
-    condition_icon: :class:`str`
-        Weather condition icon
-    condition_code: :class:`int`
-        Weather condition code
-    hour_data: List[:class:`FutureHourModel`]
-        A list of :class:`FutureHourModel` objects representing hourly weather data.
-    sunrise: :class:`str`
-        Sunrise time
-    sunset: :class:`str`
-        Sunset time
-    moonrise: :class:`str`
-        Moonrise time
-    moonset: :class:`str`
-        Moonset time
-    moon_phase: :class:`str`
-        Moon phases. Value returned:
-        * New Moon
-        * Waxing Crescent
-        * First Quarter
-        * Waxing Gibbous
-        * Full Moon
-        * Waning Gibbous
-        * Last Quarter
-        * Waning Crescent
-    moon_illumination: :class:`float`
-        Moon illumination as %
-    """
-    date: str
-    date_epoch: int
-    # day
-    maxtemp_c: float
-    maxtemp_f: float
-    mintemp_c: float
-    mintemp_f: float
-    avgtemp_c: float
-    avgtemp_f: float
-
-    maxwind_mph: float
-    maxwind_mph: float
-
-    totalprecip_mm: float
-    totalprecip_in: float
-
-    avgvis_km: float
-    avgvis_miles: float
-    avghumidity: int
-
-    condition_text: str
-    condition_icon: str
-    condition_code: int
-    # astro data
-    sunrise: Optional[str]
-    sunset: Optional[str]
-    moonrise: Optional[str]
-    moonset: Optional[str]
-    moon_phase: Optional[str]
-    moon_illumination: Optional[float]
-
-    hour_data: List[FutureHourModel]
-
 class FutureModel(ResponseModel):
     """
     An ABC defining a base response from Future API. Similiar to :class:`weatherly.ForecastModel`
 
     The following classes implement this ABC:
     - :class:`~weatherly.FutureData`
     
     Attributes
     -------------
     location: :class:`LocationModel`
         Location of the forecast data.
-    forecast_days: :class:`FutureDayModel`
+    day: :class:`ForecastDayModel`
         Day data
     """
     location: LocationModel
-    day: FutureDayModel
+    day: ForecastDayModel
```

### Comparing `weatherly-0.5.0/weatherly/api/__init__.py` & `weatherly-0.5.1/weatherly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/weatherly/api/client.py` & `weatherly-0.5.1/weatherly/api/client.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/weatherly/api/core.py` & `weatherly-0.5.1/weatherly/api/core.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/weatherly/enums.py` & `weatherly-0.5.1/weatherly/enums.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/weatherly/errors.py` & `weatherly-0.5.1/weatherly/errors.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/weatherly/responses.py` & `weatherly-0.5.1/weatherly/responses.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,16 +26,14 @@
     CurrentWeather, 
     LocationModel, 
     AirQuality, 
     ForecastDayModel, 
     ForecastHourModel, 
     ForecastModel,
     AlertModel,
-    FutureDayModel,
-    FutureHourModel,
     FutureModel
 )
 from typing import (
     Dict,
     Any,
     Union,
     Optional,
@@ -47,16 +45,14 @@
     "CurrentWeatherData",
     "LocationData",
     "AirQualityData",
     "ForecastData",
     "ForecastDay",
     "ForecastHour",
     "AlertData",
-    "FutureDay",
-    "FutureHour",
     "FutureData",
 )
 
 
 GB_DEFRA_BAND = ("Low", "Low", "Low", "Moderate", "Moderate", "Moderate", "High", "High", "High", "Very High")
 
 class CurrentWeatherData(CurrentWeather):
@@ -217,19 +213,19 @@
         HTTP status of the response. 200 is OK, and is the most common status.
     code: Optional[:class:`int`]
         Response code. In some cases this can be ``None``
     co: :class:`float`
         Carbon Monoxide (μg/m3)
     o3: :class:`float`
         Ozone (μg/m3)
-    no2: :class`float`	
+    no2: :class:`float`	
         Nitrogen dioxide (μg/m3)
     so2: :class:`float`
         Sulphur dioxide (μg/m3)
-    pm2_5: :class`float`
+    pm2_5: :class:`float`
         PM2.5 (μg/m3)
     pm10: :class:`float`
         PM10 (μg/m3)
     us_epa_index: :class:`int`
         US - EPA standard.
         * 1 means Good
         * 2 means Moderate
@@ -243,16 +239,17 @@
         +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
         | Index  | 1    | 2     | 3     | 4        | 5        | 6        | 7     | 8     | 9     | 10         |
         +========+======+=======+=======+==========+==========+==========+=======+=======+=======+============+
         | Band   | Low  | Low   | Low   | Moderate | Moderate | Moderate | High  | High  | High  | Very High  |
         +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
         | µgm^-3 | 0-11 | 12-23 | 24-35 | 36-41    | 42-47    | 48-53    | 54-58 | 59-64 | 65-70 | 71 or more |
         +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
+    
     gb_defra_band: :class:`str`
-        A band corresponding to the :ref:`gb_defra_index`
+        A band corresponding to the :py:attr:`~gb_defra_index`
     """
     def __init__(
         self,
         raw: Dict[str, Any],
         status: int,
         code: Optional[int]
     ) -> None:
@@ -410,16 +407,16 @@
         Chance of rain as percentage
     chance_of_snow: :class:`int`
         Chance of snow as percentage
     gust_mph: :class:`float`
         Wind gust in miles per hour
     gust_kph: :class:`float`
         Wind gust in kilometer per hour
-    uv: :class:`float`
-        UV Index
+    uv: Optional[:class:`float`]
+        UV Index. Can be ``None`` when this class is returned from Future API
     aqi: Optional[:class:`AirQualityData`]
         Air Quality data. See :class:`AirQualityData` for more info.
     """
     def __init__(
         self,
         raw: Dict[str, Any],
         status: int,
@@ -459,15 +456,15 @@
         self.is_day = bool(raw["is_day"])
         self.vis_km = raw["vis_km"]
         self.vis_miles = raw["vis_miles"]
         self.chance_of_rain = raw["chance_of_rain"]
         self.chance_of_snow = raw["chance_of_snow"]
         self.gust_mph = raw["gust_mph"]
         self.gust_kph = raw["gust_kph"]
-        self.uv = raw["uv"]
+        self.uv = raw.get("uv")
         
         if raw.get("air_quality"): self.aqi = AirQualityData(raw["air_quality"], status, code)
         else: self.aqi = None
     
 class ForecastDay(ForecastDayModel):
     """
     A forecast day, element of :class:`ForecastData`
@@ -506,16 +503,16 @@
         Total precipitation in inches
     avgvis_km: :class:`float`
         Average visibility in kilometer
     avgvis_miles: :class:`float`
         Average visibility in miles
     avghumidity: :class:`int`
         Average humidity as percentage
-    uv: :class:`int`
-        UV Index
+    uv: Optional[:class:`float`]
+        UV Index. Can be ``None`` when this class is returned from Future API
     condition_text: :class:`str`
         Weather condition text
     condition_icon: :class:`str`
         Weather condition icon
     condition_code: :class:`int`
         Weather condition code
     hour_data: List[:class:`ForecastHour`]
@@ -567,15 +564,15 @@
         self.maxwind_mph = raw["maxwind_mph"]
         self.maxwind_kph = raw["maxwind_kph"]
         self.totalprecip_in = raw["totalprecip_in"]
         self.totalprecip_mm = raw["totalprecip_mm"]
         self.avgvis_km = raw["avgvis_km"]
         self.avgvis_miles = raw["avgvis_miles"]
         self.avghumidity = raw["avghumidity"]
-        self.uv = raw["uv"]
+        self.uv = raw.get("uv")
         self.condition_text = raw["condition"]["text"]
         self.condition_icon = raw["condition"]["icon"]
         self.condition_code = raw["condition"]["code"]
         if raw.get("air_quality"): self.aqi = AirQualityData(raw["air_quality"], status, code)
         else: self.aqi = None
         
         raw = before_raw
@@ -646,253 +643,14 @@
             A generator object you can iterate over made of :class:`ForecastHour`
         """
 
         for day in self.forecast_days:
             for hour in day.hour_data:
                 yield hour
 
-class FutureHour(FutureHourModel):
-    """
-    Future hour, an element of :class:`FutureDay`
-    
-    Attributes
-    -------------
-    raw: Dict[:class:`str`, Any]
-        Raw response in a JSON-like format (converted to a python dictionary)
-    status: :class:`int`
-        HTTP status of the response. 200 is OK, and is the most common status.
-    code: Optional[:class:`int`]
-        Response code. In some cases this can be ``None``
-    time_epoch: :class:`int`
-        Time as epoch
-    time: :class:`str`
-        Date and time
-    temp_c: :class:`float`
-        Temperature in celsius
-    temp_f: :class:`float`
-        Temperature in fahrenheit
-    condition_text: :class:`str`
-        Weather condition text
-    condition_icon: :class:`str`
-        Weather condition icons
-    condition_code: :class:`int`
-        Weather condition code
-    wind_mph: :class:`float`
-        Maximum wind speed in miles per hour
-    wind_kph: :class:`float`
-        Maximum wind speed in kilometer per hour
-    wind_degree: :class:`int`
-        Wind direction in degrees
-    wind_dir: :class:`str`
-        Wind direction as 16 point compass. e.g.: NSW
-    pressure_mb: :class:`float`
-        Pressure in millibars
-    pressure_in: :class:`float`
-        Pressure in inches
-    precip_mm: :class:`float`
-        Precipitation amount in millimeters
-    precip_in: :class:`float`
-        Precipitation amount in inches
-    humidity: :class:`int`
-        Humidity as percentage
-    cloud: :class:`int`
-        Cloud cover as percentage
-    feelslike_c: :class:`float`
-        Feels like temperature as celcius
-    feelslike_f: :class:`float`
-        Feels like temperature as fahrenheit
-    windchill_c: :class:`float`
-        Windchill temperature in celcius
-    windchill_f: :class:`float`
-        Windchill temperature in fahrenheit
-    headindex_c: :class:`float`
-        Heat index in celcius
-    headindex_f: :class:`float`
-        Heat index in fahrenheit
-    dewpoint_c: :class:`float`
-        Dew point in celcius
-    dewpoint_f: :class:`float`
-        Dew point in fahrenheit
-    will_it_rain: :class:`bool`
-        Will it will rain or not
-    will_it_snow: :class:`bool`
-        Will it will snow or not
-    is_day: :class:`bool`
-        Whether to show day condition icon or night icon
-    vis_km: :class:`float`
-        Visibility in kilometer
-    vis_miles: :class:`float`
-        Visibility in miles
-    chance_of_rain: :class:`int`
-        Chance of rain as percentage
-    chance_of_snow: :class:`int`
-        Chance of snow as percentage
-    gust_mph: :class:`float`
-        Wind gust in miles per hour
-    gust_kph: :class:`float`
-        Wind gust in kilometer per hour
-    """
-    def __init__(
-        self,
-        raw: Dict[str, Any],
-        status: int,
-        code: Optional[int]
-    ) -> None:
-        self.raw = raw
-        self.status = status
-        self.code = code
-
-        self.time_epoch = raw["time_epoch"]
-        self.time = raw["time"]
-        self.temp_c = raw["temp_c"]
-        self.temp_f = raw["temp_f"]
-        self.condition_text = raw["condition"]["text"]
-        self.condition_icon = raw["condition"]["icon"]
-        self.condition_code = raw["condition"]["code"]
-        self.wind_mph = raw["wind_mph"]
-        self.wind_kph = raw["wind_kph"]
-        self.wind_degree = raw["wind_degree"]
-        self.wind_dir = raw["wind_dir"]
-        self.pressure_mb = raw["pressure_mb"]
-        self.pressure_in = raw["pressure_in"]
-        self.precip_mm = raw["precip_mm"]
-        self.precip_in = raw["precip_in"]
-        self.humidity = raw["humidity"]
-        self.cloud = raw["cloud"]
-        self.feelslike_c = raw["feelslike_c"]
-        self.feelslike_f = raw["feelslike_f"]
-        self.windchill_c = raw["windchill_c"]
-        self.windchill_f = raw["windchill_f"]
-        self.heatindex_c = raw["heatindex_c"]
-        self.heatindex_f = raw["heatindex_f"]
-        self.dewpoint_c = raw["dewpoint_c"]
-        self.dewpoint_f = raw["dewpoint_f"]
-        self.will_it_rain = bool(raw["will_it_rain"])
-        self.will_it_snow = bool(raw["will_it_snow"])
-        self.is_day = bool(raw["is_day"])
-        self.vis_km = raw["vis_km"]
-        self.vis_miles = raw["vis_miles"]
-        self.chance_of_rain = raw["chance_of_rain"]
-        self.chance_of_snow = raw["chance_of_snow"]
-        self.gust_mph = raw["gust_mph"]
-        self.gust_kph = raw["gust_kph"]
-
-class FutureDay(FutureDayModel):
-    """
-    A future day, element of :class:`FutureData`
-
-    Attributes
-    -------------
-    raw: Dict[:class:`str`, Any]
-        Raw response in a JSON-like format (converted to a python dictionary)
-    status: :class:`int`
-        HTTP status of the response. 200 is OK, and is the most common status.
-    code: Optional[:class:`int`]
-        Response code. In some cases this can be ``None``
-    date: :class:`str`
-        Forecast date
-    date_epoch: :class:`int`
-        Forecast date as unix time.
-    maxtemp_c: :class:`float`
-        Maximum temperature in celsius for the day.
-    maxtemp_f: :class:`float`
-        Maximum temperature in fahrenheit for the day
-    mintemp_c: :class:`float`
-        Minimum temperature in celsius for the day
-    mintemp_f: :class:`float`
-        Minimum temperature in fahrenheit for the day
-    avgtemp_c: :class:`float`
-        Average temperature in celsius for the day
-    avgtemp_f: :class:`float`
-        Average temperature in fahrenheit for the day
-    maxwind_mph: :class:`float`
-        Maximum wind speed in miles per hour
-    maxwind_kph: :class:`float`
-        Maximum wind speed in kilometer per hour
-    totalprecip_mm: :class:`float`
-        Total precipitation in milimeter
-    totalprecip_in: :class:`float`
-        Total precipitation in inches
-    avgvis_km: :class:`float`
-        Average visibility in kilometer
-    avgvis_miles: :class:`float`
-        Average visibility in miles
-    avghumidity: :class:`int`
-        Average humidity as percentage
-    condition_text: :class:`str`
-        Weather condition text
-    condition_icon: :class:`str`
-        Weather condition icon
-    condition_code: :class:`int`
-        Weather condition code
-    hour_data: List[:class:`FutureHour`]
-        A list of :class:`FutureHour` objects representing hourly weather data.
-    sunrise: :class:`str`
-        Sunrise time
-    sunset: :class:`str`
-        Sunset time
-    moonrise: :class:`str`
-        Moonrise time
-    moonset: :class:`str`
-        Moonset time
-    moon_phase: :class:`str`
-        Moon phases. Value returned:
-            * New Moon
-            * Waxing Crescent
-            * First Quarter
-            * Waxing Gibbous
-            * Full Moon
-            * Waning Gibbous
-            * Last Quarter
-            * Waning Crescent
-    moon_illumination: :class:`float`
-        Moon illumination as %
-    """
-    def __init__(
-        self,
-        raw: Dict[str, Any],
-        status: int,
-        code: Optional[int]
-    ) -> None:
-        self.raw = raw
-        self.status = status
-        self.code = code
-        self.date = raw["date"]
-        self.date_epoch = raw["date_epoch"]
-        
-        before_raw = raw.copy()
-        raw = raw["day"]
-        
-        self.maxtemp_c = raw["maxtemp_c"]
-        self.maxtemp_f = raw["maxtemp_f"]
-        self.mintemp_c = raw["mintemp_c"]
-        self.mintemp_f = raw["mintemp_f"]
-        self.avgtemp_c = raw["avgtemp_c"]
-        self.avgtemp_f = raw["avgtemp_f"]
-        self.maxwind_mph = raw["maxwind_mph"]
-        self.maxwind_kph = raw["maxwind_kph"]
-        self.totalprecip_in = raw["totalprecip_in"]
-        self.totalprecip_mm = raw["totalprecip_mm"]
-        self.avgvis_km = raw["avgvis_km"]
-        self.avgvis_miles = raw["avgvis_miles"]
-        self.avghumidity = raw["avghumidity"]
-        self.condition_text = raw["condition"]["text"]
-        self.condition_icon = raw["condition"]["icon"]
-        self.condition_code = raw["condition"]["code"]
-        
-        raw = before_raw
-        self.hour_data = list([
-            FutureHour(elem, status, code) for elem in raw["hour"]
-        ])
-        self.sunrise = raw["astro"]["sunrise"]
-        self.sunset = raw["astro"]["sunset"]
-        self.moonrise = raw["astro"]["moonrise"]
-        self.moonset = raw["astro"]["moonset"]
-        self.moon_phase = raw["astro"]["moon_phase"]
-        self.moon_illumination = raw["astro"]["moon_illumination"]
 
 class FutureData(FutureModel):
     """
     Forecast data returned from Future API
     
     Attributes
     -------------
@@ -900,22 +658,22 @@
         Raw response in a JSON-like format (converted to a python dictionary)
     status: :class:`int`
         HTTP status of the response. 200 is OK, and is the most common status.
     code: Optional[:class:`int`]
         Response code. In some cases this can be ``None``
     location: :class:`LocationData`
         Location of the forecast data.
-    day: :class:`FutureDay`
+    day: :class:`ForecastDay`
         Day data for the requested future date.
     """
     def __init__(
         self,
         raw: Dict[str, Any],
         status: int,
         code: Optional[int]
     ) -> None:
         self.raw = raw
         self.status = status
         self.code = code
         
         self.location = LocationData(raw["location"], status, code)
-        self.day = FutureDay(raw["forecast"]["forecastday"][0], status, code)
+        self.day = ForecastDay(raw["forecast"]["forecastday"][0], status, code)
```

### Comparing `weatherly-0.5.0/weatherly/utils.py` & `weatherly-0.5.1/weatherly/utils.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.5.0/weatherly.egg-info/PKG-INFO` & `weatherly-0.5.1/weatherly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatherly
-Version: 0.5.0
+Version: 0.5.1
 Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
 Home-page: https://github.com/konradsic/weatherly
 Author: konradsic
 License: MIT
 Project-URL: Issues, https://github.com/konradsic/weatherly/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

