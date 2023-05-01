# Comparing `tmp/mbta-gtfs-sqlite-0.1.3.tar.gz` & `tmp/mbta-gtfs-sqlite-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.1.3.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.9.0.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.1.3.tar` & `mbta-gtfs-sqlite-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       68 2023-04-30 02:24:02.217122 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     1203 2023-04-30 02:31:00.196926 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0      164 2023-04-30 03:32:59.636399 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/config.py
--rw-r--r--   0        0        0     4336 2023-04-30 03:37:17.361560 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6505 2023-04-30 03:27:20.093974 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      299 2023-04-30 02:17:41.015128 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1437 2023-04-30 02:21:50.513446 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2209 2023-04-30 02:22:46.094390 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     1865 2023-04-30 02:22:59.207780 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1503 2023-04-29 22:18:11.002315 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-04-30 02:20:52.918874 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      491 2023-04-30 03:39:09.415472 mbta-gtfs-sqlite-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      794 2023-04-30 03:39:22.657925 mbta-gtfs-sqlite-0.1.3/setup.py
--rw-r--r--   0        0        0      573 2023-04-30 03:39:22.658203 mbta-gtfs-sqlite-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-01 19:07:59.003673 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-01 19:40:06.198381 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0     2368 2023-05-01 20:08:17.551242 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/build.py
+-rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0     2917 2023-05-01 19:08:24.868631 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6281 2023-05-01 18:28:34.679685 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      300 2023-05-01 19:08:24.816733 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1452 2023-05-01 18:55:03.550890 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2222 2023-05-01 19:08:24.872868 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     1866 2023-05-01 19:08:24.861186 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/indexes.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      454 2023-05-01 20:05:02.693316 mbta-gtfs-sqlite-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-05-01 20:10:01.191046 mbta-gtfs-sqlite-0.9.0/setup.py
+-rw-r--r--   0        0        0      494 2023-05-01 20:10:01.191297 mbta-gtfs-sqlite-0.9.0/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/ingest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from sqlalchemy.orm import Session
-from typing import Dict, Any, Callable, List, Union, Type, Iterable
+from typing import Dict, Any, Callable, List, Type, Iterable
 
-from .archive import GtfsFeed
+from .build import GtfsFeedDownloadResult
+from .reader import GtfsReader
 from .utils.time import date_from_string, seconds_from_string
 from .utils.decorators import listify
+from .utils.indexes import bucket_by
 from .models.base import Base
 from .models.calendar_attributes import CalendarAttribute
 from .models.calendar_dates import CalendarServiceException
 from .models.calendar import CalendarService
 from .models.feed_info import FeedInfo
 from .models.lines import Line
 from .models.route_patterns import RoutePattern
@@ -37,29 +39,14 @@
 ) -> Dict[str, Any]:
     return {
         key: (transforms[key](value) if transforms.get(key) else value)
         for key, value in row_dict.items()
     }
 
 
-def bucket_by(
-    items: List[any],
-    key_getter: Union[str, Callable[[Any], str]],
-) -> Dict[str, List[any]]:
-    res = {}
-    if isinstance(key_getter, str):
-        key_getter_as_str = key_getter
-        key_getter = lambda dict: dict[key_getter_as_str]
-    for item in items:
-        key = key_getter(item)
-        res.setdefault(key, [])
-        res[key].append(item)
-    return res
-
-
 @listify
 def get_trip_rows_with_extra_time_fields(
     trip_rows: List[Dict[str, str]],
     stop_time_rows: List[Dict[str, str]],
 ) -> List[Dict[str, str]]:
     stop_times_by_trip_id = bucket_by(stop_time_rows, "trip_id")
     for trip_row in trip_rows:
@@ -70,25 +57,29 @@
         yield {
             **trip_row,
             "start_time": stop_times_for_trip[0]["arrival_time"],
             "end_time": stop_times_for_trip[-1]["arrival_time"],
         }
 
 
-def ingest_feed_info(session: Session, feed: GtfsFeed) -> FeedInfo:
+def ingest_feed_info(
+    session: Session,
+    download: GtfsFeedDownloadResult,
+    reader: GtfsReader,
+) -> FeedInfo:
     num_feed_infos = session.query(FeedInfo).count()
     next_id = 1 + num_feed_infos
-    feed_info_dict_raw = next(feed.reader.read_feed_info())
+    feed_info_dict_raw = next(reader.read_feed_info())
     feed_info_dict = transform_row_dict(
         {
             **feed_info_dict_raw,
             "id": next_id,
             "feed_info_id": next_id,
-            "retrieved_from_url": feed.url,
-            "zip_md5_checksum": feed.zip_md5_checksum,
+            "retrieved_from_url": download.url,
+            "zip_md5_checksum": download.zip_md5_checksum,
         },
         {
             "feed_start_date": date_from_string,
             "feed_end_date": date_from_string,
         },
     )
     feed_info = FeedInfo(**feed_info_dict)
@@ -115,17 +106,20 @@
     if individually:
         for mapping in mappings:
             session.add(model(**mapping))
     else:
         session.bulk_insert_mappings(model, mappings)
 
 
-def ingest_gtfs_csv_into_db(session: Session, feed: GtfsFeed):
-    reader = feed.reader
-    feed_info = ingest_feed_info(session, feed)
+def ingest_gtfs_csv_into_db(
+    session: Session,
+    download: GtfsFeedDownloadResult,
+    reader: GtfsReader,
+):
+    feed_info = ingest_feed_info(session, download, reader)
     stop_times = list(reader.read_stop_times())
     trips = list(reader.read_trips())
     trip_rows = get_trip_rows_with_extra_time_fields(trips, stop_times)
     ingest_rows(
         session=session,
         model=CalendarService,
         feed_info=feed_info,
```

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     service_schedule_name: Mapped[str] = mapped_column(String)
     service_schedule_type: Mapped[str] = mapped_column(String)
     service_schedule_typicality: Mapped[TServiceScheduleTypicality] = mapped_column(
         gtfs_enum_type(ServiceScheduleTypicality)
     )
     rating_start_date: Mapped[date] = mapped_column(Date, nullable=True)
     rating_end_date: Mapped[date] = mapped_column(Date, nullable=True)
-    rating_description: Mapped[str] = mapped_column(String)
+    rating_description: Mapped[str] = mapped_column(String, nullable=True)
```

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stops.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,21 @@
     stop_lat: Mapped[float] = mapped_column(Float, nullable=True)
     stop_lon: Mapped[float] = mapped_column(Float, nullable=True)
     zone_id: Mapped[str] = mapped_column(String)
     stop_address: Mapped[str] = mapped_column(String, nullable=True)
     stop_url: Mapped[str] = mapped_column(String, nullable=True)
     level_id: Mapped[str] = mapped_column(String, nullable=True)
     location_type: Mapped[TLocationType] = mapped_column(
-        gtfs_enum_type(LocationType), 
+        gtfs_enum_type(LocationType),
         nullable=True,
     )
     parent_station: Mapped[str] = mapped_column(String, index=True)
     wheelchair_boarding: Mapped[TWheelchairBoardingType] = mapped_column(
         gtfs_enum_type(WheelchairBoardingType),
         nullable=True,
     )
     municipality: Mapped[str] = mapped_column(String, nullable=True)
     on_street: Mapped[str] = mapped_column(String, nullable=True)
     at_street: Mapped[str] = mapped_column(String, nullable=True)
-    vehicle_type: Mapped[TRouteType] = mapped_column(gtfs_enum_type(RouteType), nullable=True)
+    vehicle_type: Mapped[TRouteType] = mapped_column(
+        gtfs_enum_type(RouteType), nullable=True
+    )
```

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/trips.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     bikes_allowed: Mapped[TBikesAllowed] = mapped_column(
         gtfs_enum_type(BikesAllowed),
         nullable=True,
     )
     # start_time and end_time are not part of GTFS but they're useful information to have
     # in smaller versions of the database without StopTimes
     start_time: Mapped[int] = mapped_column(Integer)
-    end_time: Mapped[int] = mapped_column(Integer)
+    end_time: Mapped[int] = mapped_column(Integer)
```

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 class GtfsReader:
     def _reader_by_file_name(self, name: str):
         file_path = path.join(self.root, name + ".txt")
 
         def load():
             try:
                 with open(file_path, "r") as file:
-                    print(f"Reading {file_path}...")
                     dict_reader = DictReader(file)
                     for row in dict_reader:
                         yield row
             except FileNotFoundError:
-                print(f"File {file_path} not found. Skipping.")
                 yield from []
-                
+
         return load
 
     def __init__(self, root: str):
         self.root = root
         self.read_calendar = self._reader_by_file_name("calendar")
         self.read_calendar_attributes = self._reader_by_file_name("calendar_attributes")
         self.read_calendar_dates = self._reader_by_file_name("calendar_dates")
```

### Comparing `mbta-gtfs-sqlite-0.1.3/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.3/setup.py` & `mbta-gtfs-sqlite-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 packages = \
 ['mbta_gtfs_sqlite', 'mbta_gtfs_sqlite.models', 'mbta_gtfs_sqlite.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['SQLAlchemy>=2.0.7,<3.0.0',
- 'boto3>=1.26.123,<2.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'tqdm>=4.65.0,<5.0.0']
+['SQLAlchemy>=2.0.7,<3.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.1.3',
+    'version': '0.9.0',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

