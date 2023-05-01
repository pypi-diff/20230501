# Comparing `tmp/navigation-utilities-0.1.2.tar.gz` & `tmp/navigation-utilities-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigation-utilities-0.1.2.tar", last modified: Wed Mar 15 17:52:15 2023, max compression
+gzip compressed data, was "navigation-utilities-0.2.0.tar", last modified: Mon May  1 12:11:55 2023, max compression
```

## Comparing `navigation-utilities-0.1.2.tar` & `navigation-utilities-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-15 17:52:15.516889 navigation-utilities-0.1.2/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1073 2023-03-13 17:51:45.000000 navigation-utilities-0.1.2/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      704 2023-03-15 17:52:15.516889 navigation-utilities-0.1.2/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       96 2023-03-13 18:04:41.000000 navigation-utilities-0.1.2/README.md
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      697 2023-03-15 17:51:56.000000 navigation-utilities-0.1.2/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-03-15 17:52:15.516889 navigation-utilities-0.1.2/setup.cfg
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-15 17:52:15.516889 navigation-utilities-0.1.2/src/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-15 17:52:15.516889 navigation-utilities-0.1.2/src/navigation_utilities/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-13 18:05:21.000000 navigation-utilities-0.1.2/src/navigation_utilities/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1440 2023-03-15 16:54:10.000000 navigation-utilities-0.1.2/src/navigation_utilities/coordinate.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3748 2023-03-15 17:12:26.000000 navigation-utilities-0.1.2/src/navigation_utilities/nmea.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2734 2023-03-15 16:54:12.000000 navigation-utilities-0.1.2/src/navigation_utilities/oxts.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-15 17:52:15.516889 navigation-utilities-0.1.2/src/navigation_utilities/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1914 2023-03-13 17:47:26.000000 navigation-utilities-0.1.2/src/navigation_utilities/utils/time.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-15 17:52:15.516889 navigation-utilities-0.1.2/src/navigation_utilities.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      704 2023-03-15 17:52:15.000000 navigation-utilities-0.1.2/src/navigation_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      405 2023-03-15 17:52:15.000000 navigation-utilities-0.1.2/src/navigation_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-03-15 17:52:15.000000 navigation-utilities-0.1.2/src/navigation_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       21 2023-03-15 17:52:15.000000 navigation-utilities-0.1.2/src/navigation_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1073 2023-03-28 18:04:54.000000 navigation-utilities-0.2.0/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      522 2023-04-03 09:41:32.000000 navigation-utilities-0.2.0/README.md
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      697 2023-05-01 12:11:43.000000 navigation-utilities-0.2.0/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/setup.cfg
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.208311 navigation-utilities-0.2.0/src/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/src/navigation_utilities/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-28 18:04:54.000000 navigation-utilities-0.2.0/src/navigation_utilities/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1455 2023-05-01 12:01:13.000000 navigation-utilities-0.2.0/src/navigation_utilities/coordinate.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4187 2023-05-01 12:01:01.000000 navigation-utilities-0.2.0/src/navigation_utilities/gngga.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1936 2023-05-01 11:56:39.000000 navigation-utilities-0.2.0/src/navigation_utilities/nmea.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2749 2023-05-01 11:56:49.000000 navigation-utilities-0.2.0/src/navigation_utilities/oxts.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/src/navigation_utilities/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2515 2023-05-01 12:01:32.000000 navigation-utilities-0.2.0/src/navigation_utilities/utils/time.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      439 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       21 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/top_level.txt
```

### Comparing `navigation-utilities-0.1.2/LICENSE` & `navigation-utilities-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.1.2/pyproject.toml` & `navigation-utilities-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools",
   "numpy>=1.24.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "navigation-utilities"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Pablo Dorrio Vazquez", email="pablo.dorrio.vazquez@gmail.com" },
 ]
 description = "Collection of utilities for driverless navigation systems and gnss tools"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `navigation-utilities-0.1.2/src/navigation_utilities/coordinate.py` & `navigation-utilities-0.2.0/src/navigation_utilities/coordinate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Container module for the Coordinate class.
 
 Author:
-    Pablo Dorrio Vazquez
+    Pablo Dorrio Vazquez (@pablodorrio)
 """
 
 
 class Coordinate:
     """This class represents a bidimensional coordinate.
     
     Attributes:
```

### Comparing `navigation-utilities-0.1.2/src/navigation_utilities/nmea.py` & `navigation-utilities-0.2.0/src/navigation_utilities/gngga.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,139 @@
-"""Container module for NMEA data format classes.
+"""Container module for NMEA($GNGGA) data format class.
 
 Author:
-    Pablo Dorrio Vazquez
+    Pablo Dorrio Vazquez (@pablodorrio)
 """
 
-from .oxts import Oxts
 from .coordinate import Coordinate
+from .nmea import Nmea, NmeaError
+from .oxts import Oxts
 from .utils.time import Time
 
 
-class Nmea:
-    """This class represents a NMEA sentence.
+class Gngga(Nmea):
+    """This class represents a NMEA($GNGGA) sentence.
 
     Attributes:
         latitude (str): Latitude of the location.
         longitude (str): Longitude of the location.
+        time (TIme): Time of the location.
     """
 
-    def __init__(self, latitude: str, longitude: str) -> None:
-        """Initialize the NMEA sentence.
+    def __init__(self, sentence: str) -> None:
+        """Initialize the NMEA($GNGGA) sentence.
 
         Args:
-            latitude (str): Latitude of the location.
-            longitude (str): Longitude of the location.
-        """
-        self.__latitude = latitude
-        self.__longitude = longitude
-
-    @property
-    def latitude(self) -> str:
-        """Get the latitude of the location.
-
-        Returns:
-            str: Latitude of the location.
-        """
-        return self.__latitude
-
-    @property
-    def longitude(self) -> str:
-        """Get the longitude of the location.
+            sentence (str): NMEA($GNGGA) sentence.
 
-        Returns:
-            str: Longitude of the location.
+        Raises:
+            NmeaError: If the sentence is not a NMEA($GNGGA) sentence.
         """
-        return self.__longitude
-
-    def __str__(self) -> str:
-        """Get the string representation of the NMEA sentence.
-
-        Returns:
-            str: String representation of the NMEA sentence.
-        """
-        return f"{self.__latitude}, {self.__longitude}"
-
-
-class Gpgga(Nmea):
-    """This class represents a NMEA(GPGGA) sentence.
-    
-    Attributes:
-        latitude (str): Latitude of the location.
-        longitude (str): Longitude of the location.
-        time (Time): Time of the location.
-    """
-
-    def __init__(self, latitude: str, longitude: str, time: Time=None) -> None:
-        """Initialize the NMEA(GPGGA) sentence.
 
-        Args:
-            latitude (float): Latitude of the location.
-            longitude (float): Longitude of the location.
-            time (Time): Time of the location.
+        if sentence.strip().split(",")[0] != "$GNGGA":
+            raise NmeaError("Error: invalid $GNGGA sentence.")
+        else:
+            self.sentence = sentence.strip()
 
-        NMEA (GPGGA) latitude format: "DDMM.MMMMMMMC"
-        NMEA (GPGGA) longitude format: "DDDMM.MMMMMMM"
+        latitude = self.__parse_latitude()
+        longitude = self.__parse_longitude()
+        time = self.__parse_time()
 
-        Example:    latitude = "4217.8161502N"
-                    longitude = "00748.0032395W"
-        """
-        super().__init__(latitude, longitude)
-        self.__time = time
+        super().__init__(latitude, longitude, time)
 
     def to_oxts(self) -> Oxts:
-        """Transform the latitude and longitude from NMEA (GPGGA)
+        """Transform the latitude and longitude from NMEA ($GNGGA)
         to decimal degrees.
 
         Returns:
-            OxTS: OXTS sentence whit the latitude and longitude in decimal degrees.
+            Oxts: OxTS sentence with the latitude and longitude in decimal degrees.
         """
 
-        lat_dir = super().latitude[-1]  # North or south
         lat_deg = int(super().latitude[:2])  # Degrees
         lat_min = float(super().latitude[2:-1])  # Minutes
 
-        lon_dir = super().longitude[-1]  # East or west
         lon_deg = int(super().longitude[:3])  # Degrees
         lon_min = float(super().longitude[3:-1])  # Minutes
 
         lat_dec = lat_deg + (lat_min / 60)
         lon_dec = lon_deg + (lon_min / 60)
 
-        if lat_dir == 'S':
+        if super().latitude[-1] == "S":  # North or south
             lat_dec *= -1
-        if lon_dir == 'W':
+        if super().longitude[-1] == "W":  # East or west
             lon_dec *= -1
 
         return Oxts(lat_dec, lon_dec)
 
     def to_coordinate(self, lat_0: float, lon_0: float) -> Coordinate:
-        """Transform the latitude and longitude from NMEA (GPGGA)
+        """Transform the latitude and longitude from NMEA($GNGGA)
         to a bidimensional (x, y) coordinate.
 
         Args:
             lat_0 (float): Latitude of the origin in decimal degrees.
             lon_0 (float): Longitude of the origin in decimal degrees.
 
         Returns:
             Coordinate: Bidimensional (x, y) coordinate of the location.
         """
         oxts = self.to_oxts()
         return oxts.to_coordinate(lat_0, lon_0)
 
+    def __parse_latitude(self) -> str:
+        """Parse the latitude from the NMEA($GNGGA) sentence.
+
+        NMEA ($GNGGA) latitude format: "DDMM.MMMMMMMC"
+            Example: "4217.8161502N"
+
+        Returns:
+            str: Latitude of the location.
+        """
+        if self.sentence.split(",")[2] == "" or self.sentence.split(",")[3] == "":
+            latitude = None
+        else:
+            latitude = self.sentence.split(",")[2] + self.sentence.split(",")[3]
+
+        return latitude
+
+    def __parse_longitude(self) -> str:
+        """Parse the longitude from the NMEA($GNGGA) sentence.
+
+        NMEA ($GNGGA) longitude format: "DDDMM.MMMMMMM"
+            Example: "00748.0032395W"
+
+        Returns:
+            str: Longitude of the location.
+        """
+        if self.sentence.split(",")[4] == "" or self.sentence.split(",")[5] == "":
+            longitude = None
+        else:
+            longitude = self.sentence.split(",")[4] + self.sentence.split(",")[5]
+
+        return longitude
+
+    def __parse_time(self) -> Time:
+        """Parse the time from the NMEA($GNGGA) sentence.
+
+        Returns:
+            Time: Time of the location.
+        """
+        if self.sentence.split(",")[1] == "":
+            time = None
+        else:
+            not_parsed_time = self.sentence.split(",")[1]
+
+            hours = int(not_parsed_time[:2])
+            mins = int(not_parsed_time[2:4])
+            secs = int(not_parsed_time[4:6])
+            msecs = int(not_parsed_time[7:])
+
+            time = Time(hours, mins, secs, msecs)
+
+        return time
+
     def __str__(self) -> str:
-        """Get the string representation of the NMEA(GPGGA) sentence.
+        """Get the string representation of the NMEA($GNGGA) sentence.
 
         Returns:
-            str: String representation of the NMEA(GPGGA) sentence.
+            str: String representation of the NMEA($GNGGA) sentence.
         """
-        return f"{self.__time}, {super().__str__()}"
+        return f"{super().__str__()}"
```

### Comparing `navigation-utilities-0.1.2/src/navigation_utilities/oxts.py` & `navigation-utilities-0.2.0/src/navigation_utilities/oxts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Container module for the Oxts class.
 
 Author:
-    Pablo Dorrio Vazquez
+    Pablo Dorrio Vazquez (@pablodorrio)
 """
 
 import numpy as np
 
 from .coordinate import Coordinate
 
 EARTH_RADIUS = 6371000
```

### Comparing `navigation-utilities-0.1.2/src/navigation_utilities/utils/time.py` & `navigation-utilities-0.2.0/src/navigation_utilities/utils/time.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-"""This module contains the Time class."""
+"""This module contains the Time class.
+
+Author:
+    Pablo Dorrio Vazquez (@pablodorrio)
+"""
 
 
 class Time:
     """This class represents a time in the format hh:mm:ss.
-    
+
     Attributes:
         hours (int): Hours.
         minutes (int): Minutes.
         seconds (int): Seconds.
+        miliseconds (int): Miliseconds.
     """
 
-    def __init__(self, hours: int, minutes: int, seconds: int) -> None:
+    def __init__(
+        self, hours: int, minutes: int, seconds: int, miliseconds: int
+    ) -> None:
         """Initialize the time sentence.
 
         Args:
             hours (int): Hours.
             minutes (int): Minutes.
             seconds (int): Seconds.
         """
         self.__hours = hours
         self.__minutes = minutes
         self.__seconds = seconds
+        self.__miliseconds = miliseconds
 
     @property
     def hours(self) -> int:
         """Get the hours of the time.
 
         Returns:
             int: Hours."""
@@ -71,14 +79,32 @@
         """Set the seconds of the time.
 
         Args:
             seconds (int): Seconds.
         """
         self.__seconds = seconds
 
+    @property
+    def miliseconds(self) -> int:
+        """Get the miliseconds of the time.
+
+        Returns:
+            int: Miliseconds.
+        """
+        return self.__miliseconds
+
+    @miliseconds.setter
+    def miliseconds(self, miliseconds: int) -> None:
+        """Set the miliseconds of the time.
+
+        Args:
+            miliseconds (int): Miliseconds.
+        """
+        self.__miliseconds = miliseconds
+
     def __str__(self) -> str:
         """Get the time representation of time in the format "hh:mm:ss".
 
         Returns:
             str: String representation of time.
         """
-        return f"{self.__hours}:{self.__minutes}:{self.__seconds}"
+        return f"{self.__hours}:{self.__minutes}:{self.__seconds}:{self.__miliseconds}"
```

