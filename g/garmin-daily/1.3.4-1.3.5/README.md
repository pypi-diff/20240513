# Comparing `tmp/garmin-daily-1.3.4.tar.gz` & `tmp/garmin_daily-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garmin-daily-1.3.4.tar", last modified: Thu Jan 25 05:33:47 2024, max compression
+gzip compressed data, was "garmin_daily-1.3.5.tar", last modified: Mon May 13 12:51:58 2024, max compression
```

## Comparing `garmin-daily-1.3.4.tar` & `garmin_daily-1.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 05:33:47.099887 garmin-daily-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-01-25 05:33:47.099887 garmin-daily-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-25 05:33:47.099887 garmin-daily-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 05:33:47.091887 garmin-daily-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 05:33:47.095887 garmin-daily-1.3.4/src/garmin_daily/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/src/garmin_daily/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/src/garmin_daily/columns_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/src/garmin_daily/garmin_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/src/garmin_daily/google_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/src/garmin_daily/snake_to_camel.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/src/garmin_daily/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 05:33:47.095887 garmin-daily-1.3.4/src/garmin_daily.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-01-25 05:33:47.000000 garmin-daily-1.3.4/src/garmin_daily.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-25 05:33:47.000000 garmin-daily-1.3.4/src/garmin_daily.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 05:33:47.000000 garmin-daily-1.3.4/src/garmin_daily.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-25 05:33:47.000000 garmin-daily-1.3.4/src/garmin_daily.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-25 05:33:47.000000 garmin-daily-1.3.4/src/garmin_daily.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-25 05:33:47.000000 garmin-daily-1.3.4/src/garmin_daily.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 05:33:47.095887 garmin-daily-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/tests/test_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/tests/test_columns_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/tests/test_garmin_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/tests/test_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-25 05:33:39.000000 garmin-daily-1.3.4/tests/test_snake_to_camel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:51:58.922750 garmin_daily-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-13 12:51:58.922750 garmin_daily-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 12:51:58.922750 garmin_daily-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:51:58.914750 garmin_daily-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:51:58.918750 garmin_daily-1.3.5/src/garmin_daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/src/garmin_daily/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/src/garmin_daily/columns_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/src/garmin_daily/garmin_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/src/garmin_daily/google_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/src/garmin_daily/snake_to_camel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/src/garmin_daily/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:51:58.918750 garmin_daily-1.3.5/src/garmin_daily.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-13 12:51:58.000000 garmin_daily-1.3.5/src/garmin_daily.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-13 12:51:58.000000 garmin_daily-1.3.5/src/garmin_daily.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:51:58.000000 garmin_daily-1.3.5/src/garmin_daily.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 12:51:58.000000 garmin_daily-1.3.5/src/garmin_daily.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 12:51:58.000000 garmin_daily-1.3.5/src/garmin_daily.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 12:51:58.000000 garmin_daily-1.3.5/src/garmin_daily.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:51:58.918750 garmin_daily-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/tests/test_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/tests/test_columns_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/tests/test_garmin_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/tests/test_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-13 12:51:50.000000 garmin_daily-1.3.5/tests/test_snake_to_camel.py
```

### Comparing `garmin-daily-1.3.4/LICENSE.txt` & `garmin_daily-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/PKG-INFO` & `garmin_daily-1.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-daily
-Version: 1.3.4
+Version: 1.3.5
 Summary: Aggregate data from Garmin Connect daily.
 Home-page: https://andgineer.github.io/garmin-daily/en/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: Garmin Connect Health Google Sheets
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,23 +14,21 @@
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: gspread
 Requires-Dist: markdownify
 Requires-Dist: click
 Requires-Dist: rich-click
 Requires-Dist: garminconnect
-Requires-Dist: click
 Requires-Dist: pandas
 Provides-Extra: test
 Requires-Dist: lazydocs; extra == "test"
 Requires-Dist: mkdocs-material; extra == "test"
 Requires-Dist: pymdown-extensions; extra == "test"
 Requires-Dist: mkdocs-awesome-pages-plugin; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
-Requires-Dist: mkdocs-awesome-pages-plugin; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: freezegun; extra == "test"
 Requires-Dist: twine; extra == "test"
 Requires-Dist: pip-tools; extra == "test"
```

### Comparing `garmin-daily-1.3.4/README.md` & `garmin_daily-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/setup.py` & `garmin_daily-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/src/garmin_daily/columns_mapper.py` & `garmin_daily-1.3.5/src/garmin_daily/columns_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Map fields to columns using spreadsheet header row."""
+
 from enum import Enum, IntEnum
 from typing import Dict, List, Optional, Type, Union
 
 
 class GarminCol(IntEnum):
     """Columns of the Garmin daily data spreadsheet."""
```

### Comparing `garmin-daily-1.3.4/src/garmin_daily/garmin_aggregations.py` & `garmin_daily-1.3.5/src/garmin_daily/garmin_aggregations.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,17 +160,20 @@
             self.sleep_rem_time,
         ) = self.get_sleep()
         self.vo2max = self.get_vo2max()
         self.activities = self.aggregate_activities()
 
     def get_vo2max(self) -> float:
         """Get VO2 max."""
-        return self.api.get_training_status(self.date_str)["mostRecentVO2Max"][  # type: ignore
-            "generic"
-        ]["vo2MaxValue"]
+        try:
+            return self.api.get_training_status(self.date_str)["mostRecentVO2Max"][  # type: ignore
+                "generic"
+            ]["vo2MaxValue"]
+        except Exception:  # pylint: disable=broad-except
+            return 0.0
 
     def get_hr(self) -> Tuple[Optional[int], Optional[int], Optional[int], Optional[int]]:
         """Set HR attrs.
 
         Returns (min, max, average, rest)
         """
         hr_data = self.api.get_heart_rates(self.date_str)
```

### Comparing `garmin-daily-1.3.4/src/garmin_daily/google_sheet.py` & `garmin_daily-1.3.5/src/garmin_daily/google_sheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Export Garmin data to Google Sheet."""
+
 import locale
 import sys
 import time
 from datetime import date, datetime, timedelta
 from enum import IntEnum
 from functools import lru_cache
 from typing import Dict, List, Optional, Tuple, Union
 
 import gspread
 import gspread.exceptions
 import pandas as pd
 import rich_click as click
+from gspread.utils import ValueInputOption
 
 from garmin_daily import SPORT_STEP_LENGTH_KM, WALKING_SPORT, Activity, GarminDaily
 from garmin_daily.columns_mapper import ColumnsMapper, GarminCol
 from garmin_daily.version import VERSION
 
 SHEET_NAME_DEFAULT = "05 Fitness"
 
@@ -81,15 +83,15 @@
     help="Gym training duration, minutes.",
     nargs=1,
 )
 @click.option(
     "--gym-location",
     "-l",
     "gym_location",
-    default="The classic Bulevar Oslobođenja",
+    default="No Limit Gym",
     show_default=True,
     help="Gym training duration, minutes.",
     nargs=1,
 )
 @click.option(
     "--force",
     "-f",
@@ -181,15 +183,15 @@
             )
             rows = [
                 localized_csv_raw(columns.map(fields)) for fields in rows_fields  # type: ignore
             ]
             search_missed_steps_in_sheet(fitness, rows, columns)
             for row in rows:
                 print("; ".join(row))
-            fitness.insert_rows(rows, row=2, value_input_option="USER_ENTERED")
+            fitness.insert_rows(rows, row=2, value_input_option=ValueInputOption.user_entered)
         if batch < batches_num - 1:  # do not pause on last iteration
             time.sleep(API_DELAY)  # pause to prevent robot protection from Garmin API
 
 
 @lru_cache(maxsize=None)
 def fitness_df(fitness: gspread.Worksheet) -> pd.DataFrame:
     """Load the Google Sheet as Pandas DataFrame.
@@ -323,41 +325,47 @@
         )
     rows_fields: List[Dict[GarminCol, Optional[Union[str, int, float]]]] = [
         {
             GarminCol.LOCATION: activity.location_name,
             GarminCol.SPORT: activity.sport,
             GarminCol.DURATION: round(activity.duration / 60) if activity.duration else "",
             GarminCol.DATE: day.strftime("%Y-%m-%d"),
-            GarminCol.DISTANCE: round(activity.distance / 1000, 2)
-            if activity.distance
-            else (
-                f"=({activity.steps}"
-                f"-{activity.non_walking_steps if activity.non_walking_steps else 0})"
-                f"*{SPORT_STEP_LENGTH_KM[activity.sport]:.2n}"
-            )
-            if activity.sport in SPORT_STEP_LENGTH_KM
-            else "",
-            GarminCol.STEPS: f"={activity.steps}-{activity.non_walking_steps}"
-            if activity.non_walking_steps
-            else f"={activity.steps}"
-            if activity.sport == WALKING_SPORT
-            else "",
+            GarminCol.DISTANCE: (
+                round(activity.distance / 1000, 2)
+                if activity.distance
+                else (
+                    (
+                        f"=({activity.steps}"
+                        f"-{activity.non_walking_steps if activity.non_walking_steps else 0})"
+                        f"*{SPORT_STEP_LENGTH_KM[activity.sport]:.2n}"
+                    )
+                    if activity.sport in SPORT_STEP_LENGTH_KM
+                    else ""
+                )
+            ),
+            GarminCol.STEPS: (
+                f"={activity.steps}-{activity.non_walking_steps}"
+                if activity.non_walking_steps
+                else f"={activity.steps}" if activity.sport == WALKING_SPORT else ""
+            ),
             GarminCol.COMMENT: activity.comment,
             GarminCol.WEEK: week_num(day),
             GarminCol.HOURS: round(activity.duration / 60 / 60, 1) if activity.duration else 0,
             GarminCol.WEEKDAY: sheet_week_day(day),
-            GarminCol.HR_REST: round(gday.hr_rest, 1)
-            if activity.sport == WALKING_SPORT and gday.hr_rest
-            else "",
-            GarminCol.SLEEP_TIME: round(gday.sleep_time, 1)
-            if activity.sport == WALKING_SPORT and gday.sleep_time
-            else "",
-            GarminCol.VO2_MAX: gday.vo2max
-            if activity.sport == WALKING_SPORT and gday.vo2max
-            else "",
+            GarminCol.HR_REST: (
+                round(gday.hr_rest, 1) if activity.sport == WALKING_SPORT and gday.hr_rest else ""
+            ),
+            GarminCol.SLEEP_TIME: (
+                round(gday.sleep_time, 1)
+                if activity.sport == WALKING_SPORT and gday.sleep_time
+                else ""
+            ),
+            GarminCol.VO2_MAX: (
+                gday.vo2max if activity.sport == WALKING_SPORT and gday.vo2max else ""
+            ),
         }
         for activity in gday.activities
     ]
     return rows_fields
 
 
 def localized_csv_raw(row: List[Optional[Union[str, int, float]]]) -> List[str]:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `garmin-daily-1.3.4/src/garmin_daily/snake_to_camel.py` & `garmin_daily-1.3.5/src/garmin_daily/snake_to_camel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convert names from Python (snake-name) to Java (camelName) name convention and vice-versa."""
+
 import re
 
 
 def snake_to_camel(snake_case_name: str) -> str:
     """Convert snake_case_names to camelCase."""
     words = snake_case_name.split("_")
     return words[0].lower() + "".join(word.title() for word in words[1:])
```

### Comparing `garmin-daily-1.3.4/src/garmin_daily.egg-info/PKG-INFO` & `garmin_daily-1.3.5/src/garmin_daily.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-daily
-Version: 1.3.4
+Version: 1.3.5
 Summary: Aggregate data from Garmin Connect daily.
 Home-page: https://andgineer.github.io/garmin-daily/en/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: Garmin Connect Health Google Sheets
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,23 +14,21 @@
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: gspread
 Requires-Dist: markdownify
 Requires-Dist: click
 Requires-Dist: rich-click
 Requires-Dist: garminconnect
-Requires-Dist: click
 Requires-Dist: pandas
 Provides-Extra: test
 Requires-Dist: lazydocs; extra == "test"
 Requires-Dist: mkdocs-material; extra == "test"
 Requires-Dist: pymdown-extensions; extra == "test"
 Requires-Dist: mkdocs-awesome-pages-plugin; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
-Requires-Dist: mkdocs-awesome-pages-plugin; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: freezegun; extra == "test"
 Requires-Dist: twine; extra == "test"
 Requires-Dist: pip-tools; extra == "test"
```

### Comparing `garmin-daily-1.3.4/src/garmin_daily.egg-info/SOURCES.txt` & `garmin_daily-1.3.5/src/garmin_daily.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/tests/test_activity.py` & `garmin_daily-1.3.5/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/tests/test_columns_mapper.py` & `garmin_daily-1.3.5/tests/test_columns_mapper.py`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/tests/test_garmin_day.py` & `garmin_daily-1.3.5/tests/test_garmin_day.py`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/tests/test_main.py` & `garmin_daily-1.3.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/tests/test_sheet.py` & `garmin_daily-1.3.5/tests/test_sheet.py`

 * *Files identical despite different names*

### Comparing `garmin-daily-1.3.4/tests/test_snake_to_camel.py` & `garmin_daily-1.3.5/tests/test_snake_to_camel.py`

 * *Files identical despite different names*

