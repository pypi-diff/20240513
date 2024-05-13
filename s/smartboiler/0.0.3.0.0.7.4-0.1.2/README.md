# Comparing `tmp/smartboiler-0.0.3.0.0.7.4.tar.gz` & `tmp/smartboiler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.7.4.tar", last modified: Wed Apr 24 11:22:44 2024, max compression
+gzip compressed data, was "smartboiler-0.1.2.tar", last modified: Mon May 13 10:37:43 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.7.4.tar` & `smartboiler-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:22:44.015111 smartboiler-0.0.3.0.0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-24 11:22:44.015111 smartboiler-0.0.3.0.0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:22:44.015111 smartboiler-0.0.3.0.0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-24 11:22:42.000000 smartboiler-0.0.3.0.0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:22:44.015111 smartboiler-0.0.3.0.0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:22:44.015111 smartboiler-0.0.3.0.0.7.4/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14611 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-24 11:22:41.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:22:44.015111 smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-24 11:22:43.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 11:22:44.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:22:43.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 11:22:43.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 11:22:43.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 11:22:43.000000 smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:37:43.640676 smartboiler-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 10:37:40.000000 smartboiler-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:37:43.640676 smartboiler-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 10:37:42.000000 smartboiler-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32021 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.7.4/src/smartboiler/controller.py` & `smartboiler-0.1.2/src/smartboiler/controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,71 @@
-from pathlib import Path
-from pyexpat import model
-import re, pytz
-
-print("Running" if __name__ == "__main__" else "Importing", Path(__file__).resolve())
-
-###########################################################
-# Masters's thesis                                       #
-# From a dumb boiler to a smart one using a smart socket  #
-# Author: Adam Grünwald                                   #
-# BUT FIT BRNO, Faculty of Information Technology         #
-# 26/6/2021                                               #
-#                                                         #
-# Module that controls a heating of smart boiler.         #
-# Uses module Boiler for computing time needed to heating #
-# of water, module TimeHandler for basic time and date    #
-# operations, WeekPlanner for plan week heating,          #
-# SettingsLoader to load setting from settings file and   #
-# EventChecker which checks events in calendar,           #
-# when the water shouldn't be heated.                      #
-###########################################################
+# Created as a part of Master's Thesis "Using machine learning methods to save energy in a smart home"
+# Faculty of Information Technology, Brno University of Technology, 2024
+# Author: Adam Grünwald
+#
+# This module is used for controlling the boiler with use of the predictions in combination with the smart heating algotithm.
 
 
+from pathlib import Path
+import pytz
 from datetime import datetime, timedelta
-import pandas as pd
-import calendar
-from influxdb import DataFrameClient
-from influxdb import InfluxDBClient
-import os.path
 
-import argparse
+import os.path
 import logging
 import time
 import os
-
 import json
 
 
+from smartboiler.event_checker import EventChecker
 from smartboiler.data_handler import DataHandler
 from smartboiler.fotovoltaics import Fotovoltaics
 from smartboiler.forecast import Forecast
 from smartboiler.boiler import Boiler
 
 
 class Controller:
     """Main class which makes decisions about about heating"""
 
     def __init__(
         self,
         dataHandler: DataHandler,
         boiler: Boiler,
         forecast: Forecast,
+        eventChecker: EventChecker,
         load_model=False,
+        learning=True,
     ):
         """Inits class of Controller. Loads settings from a settings file
 
         Args:
             settings_file (str, optional): [name of json file with settings]. Defaults to 'settings.json'.
         """
-        # TODO - load settings from config file or home assistant
-
-        # self.how_water_flow = settings['how_water_flow']
-        # self.tmp_water_flow = settings['tmp_water_flow']
 
         self.tmp_min = 5
 
         self.start_date = datetime.now()
 
-        # self.Hass = remote.API('localhost', 'smart_boiler01')
         self.dataHandler = dataHandler
         self.boiler = boiler
         self.forecast = forecast
+        self.eventChecker = eventChecker
 
         if load_model:
             print("loading model")
             self.forecast.build_model()
             self.forecast.load_model()
         else:
             print("training model")
             self.forecast.build_model()
             forecast.train_model()
 
         self.last_model_training = datetime.now()
-
-        # #self.EventChecker = EventChecker()
-        # #self.TimeHandler = TimeHandler()
-        # #self.Boiler = Boiler(capacity=boiler_capacity,
-        # #                    wattage=boiler_wattage, set_tmp=boiler_set_tmp)
-
-        # #self.data_db = self._actualize_data()
         self.last_legionella_heating = datetime.now()
 
-        # #self.WeekPlanner = WeekPlanner(self.data_db)
-        self.coef_up_in_current_heating_cycle_changed = False
-        self.coef_down_in_current_heating_cycle_changed = False
-
     def _last_entry(self):
         print("getting last entry")
         last_entry = self.dataHandler.get_actual_boiler_stats()
         print("last entry: {}".format(last_entry))
         return last_entry
 
     def _check_data(self):
@@ -110,83 +78,61 @@
 
     def _learning(self):
         """After one week of only measuring the data starts heating based on historical data.
 
         Returns:
             [boolean]: [True if in learing]
         """
-
-        return (datetime.now() - self.start_date) < timedelta(days=7)
+        if not self.learning:
+            return False
+        return (datetime.now() - self.start_date) < timedelta(days=28)
 
     def actualize_forecast(self):
         self.actual_forecast = self.forecast.get_forecast_next_steps()
 
     def control(self):
         """Method which decides about turning on or off the heating of a boiler."""
 
         time_now = datetime.now().astimezone(pytz.timezone("Europe/Prague"))
         print(f"actual time: {time_now}, controling boiler")
         last_entry = self._last_entry()
 
-        # TODO - heatup events from calendar
-        # # checks whether the water in boiler should be even ready
-        # if self.eventChecker.check_off_event():
-        #     print("naplanovana udalost")
-        #     self.boiler.turn_off()
-        #     time.sleep(600)
-        #     return
+        # checks whether the water in boiler should be even ready
+        if self.eventChecker.check_off_event():
+            print("turning off boiler, event in calendar")
+            self.boiler.turn_off()
+            return
+        # check scheduled heating target event
 
         tmp_measured = last_entry["boiler_case_tmp"]
         is_on = last_entry["is_boiler_on"]
-        boiler_case_last_time_entry = last_entry["boiler_case_last_time_entry"]
-        is_boiler_on_last_time_entry = last_entry["is_boiler_on_last_time_entry"]
-
-        # # in case of too old data, the boiler is turned on
-        # if ( ( time_now.microsecond - (last_entry['boiler_case_last_time_entry']).microsecond)/1000000 > timedelta(minutes=10)):
-        #     print("too old data, turning on")
-        #     boiler.turn_on()
-        #     return
-
-        # # looks for the next heat up event from a calendar
-        # next_calendar_heat_up_event = self.eventChecker.next_calendar_heat_up_event(
-        #     self.Boiler)
 
         # actual tmp of water in boiler
         tmp_act = self.boiler.real_tmp(tmp_measured)
         print(f"actual tmp: {tmp_act}, measured: {tmp_measured}")
 
         if is_on is None:
             print("boiler state is unknown")
             is_on = False
-            
 
         # protection from freezing
         if tmp_act < 5:
             self.boiler.turn_on()
 
-        # if self._learning():
-        #     if tmp_act > 60:
-        #         if is_on:
-        #             self.boiler.turn_off()
-        #     else:
-        #         if tmp_act < 57:
-        #             if not is_on:
-        #                 self.boiler.turn_on()
-
-        #     return
-
-        # # if last entry is older than 10 minutes and not because of high tarif, water in a boiler is heated for sure
-        # time_of_last_entry = last_entry['time_of_last_entry']
-        # if (time_now - time_of_last_entry > timedelta(minutes=10)):
-        #     if not self.weekPlanner.is_in_DTO():
-        #         print("too old last entry ({}), need to heat".format(
-        #             time_of_last_entry))
-        #         if not is_on:
-        #             self.boiler.turn_on()
-        #     return
+        if self._learning():
+            if tmp_act > 60:
+                if is_on:
+                    self.boiler.turn_off()
+            else:
+                if tmp_act < 57:
+                    if not is_on:
+                        self.boiler.turn_on()
+            return
+        else:
+            self._check_data()
 
         # if the boiler is needed to heat up before the next predicted consumption
         is_needed_to_heat, minutes_needed_to_heat = self.boiler.is_needed_to_heat(
             tmp_act, self.actual_forecast
         )
         if is_needed_to_heat:
             print(
@@ -195,54 +141,45 @@
             self.boiler.turn_on()
             time.sleep(minutes_needed_to_heat * 60)
         else:
             print("no need to heat, turning off")
             self.boiler.turn_off()
 
         if self.last_legionella_heating - datetime.now() > timedelta(days=21):
-            print("starting heating for reduce legionella, this occurs every 3 weeks")
             self.boiler.turn_on()
             if tmp_act >= (65):
                 time.sleep(1200)
                 self.last_legionella_heating = datetime.now()
-                print("legionella was eliminated, see you in 3 weeks")
                 self.boiler.turn_off()
                 return
-        # TODO event checker for holidays
 
 
 if __name__ == "__main__":
     logging.info("Starting SmartBoiler Controller")
 
-
-
     OPTIONS_PATH = os.getenv("OPTIONS_PATH", default="/app/options.json")
     options_json = Path(OPTIONS_PATH)
 
     # Read options info
     if options_json.exists():
         with options_json.open("r") as data:
             options = json.load(data)
 
     DATA_PATH = os.getenv("DATA_PATH", default="/app/data/")
 
     data_path = Path(DATA_PATH)
 
-
     start_of_data_measurement = datetime(2023, 10, 1, 0, 0, 0, 0)
 
     hass_url = options["hass_url"]
     home_longitude = options["home_longitude"]
     home_latitude = options["home_latitude"]
-    print(f"home longitude: {home_longitude}, home latitude: {home_latitude}")
-    print(f"home longitude type: {type(home_longitude)}, home latitude type: {type(home_latitude)}")
-    
     device_tracker_entity_id = options["device_tracker_entity_id"]
-    model_path = options["model_path"]
-    scaler_path = options["scaler_path"]
+    device_tracker_entity_id_2 = options["device_tracker_entity_id_2"]
+    model_type = options["model_type"]
     long_lived_token = options["long_lived_token"]
     influxdb_host = options["influxdb_host"]
     influxdb_port: 8086
     influxdb_user = options["influxdb_user"]
     influxdb_pass = options["influxdb_pass"]
     influxdb_name = options["influxdb_name"]
     boiler_socket_switch_id = options["boiler_entidy_id"]
@@ -263,23 +200,31 @@
     one_shower_volume = options["one_shower_volume"]
     boiler_watt_power = options["boiler_watt_power"]
     household_floor_size = options["household_floor_size"]
     household_members = options["household_members"]
     thermostat_entity_id = options["thermostat_entity_id"]
     logging_level = options["logging_level"]
     load_model = options["load_model"]
+    learning = options["learning"]
     hdo = options["hdo"]
     has_fotovoltaics = options["has_fotovoltaics"]
     fve_solax_sn = options["fve_solax_sn"]
     fve_solax_token = options["fve_solax_token"]
     
+    # chosing the model based on size of household
+    if model_type == "smaller_household":
+        model_path = "/app/model_form.weights.h5"
+        scaler_path = "/app/scaler_form.pkl"
+    else:
+        model_path = "/app/model_zuka.weights.h5"
+        scaler_path = "/app/scaler_zuka.pkl"
+
     model_path = Path(model_path)
     scaler_path = Path(scaler_path)
 
-    print(f"Starting SmartBoiler Controller with the following settings: {options}")
     base_url = hass_url
     url = base_url + "/config"
     web_ui = "0.0.0.0"
 
     headers = {
         "Authorization": f"Bearer {long_lived_token}",
         "content-type": "application/json",
@@ -292,67 +237,73 @@
         db_password=influxdb_pass,
         relay_entity_id=boiler_socket_id,
         relay_power_entity_id=boiler_socket_power_id,
         tmp_boiler_case_entity_id=boiler_case_tmp_entity_id,
         tmp_output_water_entity_id=boiler_water_temp_entity_id,
         tmp_output_water_entity_id_2=boiler_water_temp_entity_id_2,
         device_tracker_entity_id=device_tracker_entity_id,
+        device_tracker_entity_id_2=device_tracker_entity_id_2,
         home_longitude=home_longitude,
         home_latitude=home_latitude,
         start_of_data=start_of_data_measurement,
     )
     boiler_switch_entity_id = "switch." + boiler_socket_id
-    
+
     print("inicializing fotovoltaics from controller __main__")
     if has_fotovoltaics:
         fotovoltaics = Fotovoltaics(
             power=100,
             efficiency=0.9,
             token=fve_solax_token,
             sn=fve_solax_sn,
             battery_capacity=10,
             battery_power=5,
         )
     else:
         fotovoltaics = None
-
+    eventChecker = EventChecker()
     print("inicializing boiler from controller __main__")
     boiler = Boiler(
         base_url,
         long_lived_token,
         headers,
         boiler_switch_entity_id=boiler_socket_switch_id,
         dataHandler=dataHandler,
+        eventChecker=eventChecker,
         fotovoltaics=fotovoltaics,
         capacity=boiler_volume,
         wattage=boiler_watt_power,
         set_tmp=boiler_set_tmp,
         min_tmp=boiler_min_operation_tmp,
         average_boiler_surroundings_temp=average_boiler_surroundings_temp,
         boiler_case_max_tmp=boiler_case_max_tmp,
         hdo=hdo,
     )
-    
+
     predicted_columns = ["longtime_mean"]
     print("inicializing forecast from controller __main__   ")
     forecast = Forecast(
         dataHandler=dataHandler,
         start_of_data=start_of_data_measurement,
         model_path=model_path,
         scaler_path=scaler_path,
         predicted_columns=predicted_columns,
-        
     )
     print("inicializing controller from controller __main__")
     controller = Controller(
-        dataHandler=dataHandler, boiler=boiler, forecast=forecast, load_model=load_model
+        dataHandler=dataHandler,
+        boiler=boiler,
+        forecast=forecast,
+        eventChecker=eventChecker,
+        load_model=load_model,
+        learning = learning,
     )
 
     while 1:
         try:
             controller.actualize_forecast()
-            for i in range(0,15):
+            for i in range(0, 15):
                 controller.control()
                 time.sleep(60)
         except Exception as e:
             print(f"Error: {e}")
             time.sleep(60)
```

### Comparing `smartboiler-0.0.3.0.0.7.4/src/smartboiler/data_handler.py` & `smartboiler-0.1.2/src/smartboiler/data_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,64 @@
-from pathlib import Path
+# Created as a part of Master's Thesis "Using machine learning methods to save energy in a smart home"
+# Faculty of Information Technology, Brno University of Technology, 2024
+# Author: Adam Grünwald
+#
+# This module is used for handling the data from the database.
+
+from typing import Optional
 
-print("Running" if __name__ == "__main__" else "Importing", Path(__file__).resolve())
-from operator import le
-from click import group
-from matplotlib.dates import drange
 import pandas as pd
 from influxdb import DataFrameClient, InfluxDBClient
 
-import matplotlib.pyplot as plt
-from datetime import date, datetime, timedelta
+from datetime import datetime, timedelta
 import numpy as np
-import json
-import logging
-from math import dist
+
 import numpy as np
-from geopy.distance import geodesic
 from haversine import haversine
 
 
 class DataHandler:
+    """Class for handling the data from the database."""
+
     def __init__(
         self,
-        influx_id,
-        db_name,
-        db_username,
-        db_password,
-        relay_entity_id,
-        relay_power_entity_id,
-        tmp_boiler_case_entity_id,
-        tmp_output_water_entity_id,
-        tmp_output_water_entity_id_2,
-        device_tracker_entity_id,
-        home_longitude,
-        home_latitude,
-        start_of_data=datetime(2023, 1, 1, 0, 0, 0, 0),
+        influx_id: str,
+        db_name: str,
+        db_username: str,
+        db_password: str,
+        relay_entity_id: str,
+        relay_power_entity_id: str,
+        tmp_boiler_case_entity_id: str,
+        tmp_output_water_entity_id: str,
+        tmp_output_water_entity_id_2: str,
+        device_tracker_entity_id: str,
+        device_tracker_entity_id_2: str,
+        home_longitude: float,
+        home_latitude: float,
+        start_of_data: Optional[datetime] = datetime(2023, 1, 1, 0, 0, 0, 0),
     ):
+        """Init function for the DataHandler class.
+
+        Args:
+            influx_id (str): Influxdb server name.
+            db_name (str): Name of the influxdb database with data for processing.
+            db_username (str): Username for influxdb.
+            db_password (str): Password for influxdb.
+            relay_entity_id (str): Entity ID of shelly relay in home assistant.
+            relay_power_entity_id (str): Entity ID of the shelly relay power in home assistant.
+            tmp_boiler_case_entity_id (str): Entity ID of the boiler case temperature sensor.
+            tmp_output_water_entity_id (str): Entity ID of the output water temperature sensor.
+            tmp_output_water_entity_id_2 (str): Entity ID for the case of two output water temperature sensors.
+            device_tracker_entity_id (str): Entity ID of the first device tracker.
+            device_tracker_entity_id_2 (str): Entity ID of the second device tracker.
+            home_longitude (float):l Longitude of the home.
+            home_latitude (float): atitude of the home.
+            start_of_data (Optional[datetime], optional): Start from when should be the data from db taken. Defaults to datetime(2023, 1, 1, 0, 0, 0, 0).
+        """
+
         self.influx_id = influx_id
         self.db_name = db_name
         self.db_username = db_username
         self.db_password = db_password
         self.group_by_time_interval = "30min"
         self.relay_entity_id = relay_entity_id
         self.relay_power_entity_id = relay_power_entity_id
@@ -46,14 +66,20 @@
         self.tmp_output_water_entity_id = tmp_output_water_entity_id
         self.tmp_output_water_entity_id_2 = tmp_output_water_entity_id_2
 
         self.home_longitude = home_longitude
         self.home_latitude = home_latitude
 
         self.device_tracker_entity_id = device_tracker_entity_id
+        self.device_tracker_entity_id_2 = device_tracker_entity_id_2
+
+        self.start_of_data = start_of_data
+        self.last_time_data_update = datetime.now()
+
+        # initialize clients
         self.dataframe_client = DataFrameClient(
             host=self.influx_id,
             port=8086,
             username=self.db_username,
             password=self.db_password,
             database=self.db_name,
         )
@@ -63,25 +89,33 @@
             username=self.db_username,
             password=self.db_password,
             database=self.db_name,
             retries=5,
             timeout=1,
         )
 
-        self.start_of_data = start_of_data
-        self.last_time_data_update = datetime.now()
-
     def get_actual_boiler_stats(
         self,
-        group_by_time_interval="10m",
-        limit=300,
-        left_time_interval=datetime.now() - timedelta(hours=6),
-        right_time_interval=datetime.now() - timedelta(hours=1),
-    ):
-
+        group_by_time_interval: Optional[str] = "10m",
+        limit: Optional[int] = 300,
+        left_time_interval: Optional[datetime] = datetime.now() - timedelta(hours=6),
+        right_time_interval: Optional[datetime] = datetime.now() - timedelta(hours=1),
+    ) -> dict:
+        # TODO handle correct the timezones
+        """Method to retrieve the actual stats for the boilers. Serves for algorithm of controling the boiler.
+
+        Args:
+            group_by_time_interval (Optional[str], optional): Time interval by which should be the data grouped. Defaults to "10m".
+            limit (Optional[int], optional): Limit of the last N values. Defaults to 300.
+            left_time_interval (Optional[datetime], optional): Left interval in which we are interested. Defaults to datetime.now()-timedelta(hours=6).
+            right_time_interval (Optional[datetime], optional): Right time interval. the -1h is because of the correction of Europe/Prague timezone. Defaults to datetime.now()-timedelta(hours=1).
+
+        Returns:
+            dict: Dictionary of the actual stats for boiler_case_tmp, is_boiler_on, boiler_case_last_time_entry, is_boiler_on_last_time_entry.
+        """
         left_time_interval = f"'{left_time_interval.strftime('%Y-%m-%dT%H:%M:%SZ')}'"
         right_time_interval = f"'{right_time_interval.strftime('%Y-%m-%dT%H:%M:%SZ')}'"
         actual_boiler_stats = {
             "boiler_temperature": {
                 "sql_query": f'SELECT last("value") AS "boiler_case_tmp" FROM "{self.db_name}"."autogen"."°C" WHERE  "entity_id"=\'{self.tmp_boiler_case_entity_id}\' ',
                 "measurement": "°C",
             },
@@ -94,247 +128,398 @@
 
         boiler_case_tmp = data["boiler_case_tmp"].dropna().reset_index()
         is_boiler_on = data["is_boiler_on"].dropna().reset_index()
 
         boiler_case_tmp["index"] = pd.to_datetime(boiler_case_tmp["index"])
         is_boiler_on["index"] = pd.to_datetime(is_boiler_on["index"])
 
+        # last values
         boiler_case_last_time_entry = boiler_case_tmp["index"].iloc[-1]
         boiler_case_tmp = boiler_case_tmp["boiler_case_tmp"].iloc[-1]
         is_boiler_on_last_time_entry = is_boiler_on["index"].iloc[-1]
         is_boiler_on = bool(is_boiler_on["is_boiler_on"].iloc[-1])
 
         return {
             "boiler_case_tmp": boiler_case_tmp,
             "is_boiler_on": is_boiler_on,
             "boiler_case_last_time_entry": boiler_case_last_time_entry,
             "is_boiler_on_last_time_entry": is_boiler_on_last_time_entry,
         }
 
     def get_database_queries(
         self,
-        left_time_interval,
-        right_time_interval,
-    ):
+        left_time_interval: datetime,
+        right_time_interval: datetime,
+    ) -> dict:
+        """Method to create dictionary of queries for the database.
+
+        Args:
+            left_time_interval (datetime): Left time interval.
+            right_time_interval (datetime): Right time interval.
+
+        Returns:
+            dict: Dictionary of queries for the database.
+        """
 
         group_by_time_interval = "1m"
 
         # format datetime to YYYY-MM-DDTHH:MM:SSZ
         left_time_interval = f"'{left_time_interval.strftime('%Y-%m-%dT%H:%M:%SZ')}'"
         right_time_interval = f"'{right_time_interval.strftime('%Y-%m-%dT%H:%M:%SZ')}'"
 
         return {
-        "water_flow": {
-            "sql_query": f'SELECT mean("value") AS "water_flow_L_per_minute_mean" FROM "{self.db_name}"."autogen"."L/min" WHERE time > {left_time_interval} AND time <= {right_time_interval} GROUP BY time({group_by_time_interval}) FILL(0)',
-            "measurement": "L/min",
-        },
-        "water_temperature": {
-            "sql_query": f'SELECT mean("value") AS "water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND ("entity_id"=\'{self.tmp_output_water_entity_id}\' OR "entity_id"=\'{self.tmp_output_water_entity_id_2}\') GROUP BY time({group_by_time_interval}) FILL(0)',
-            "measurement": "°C",
-        },
-        "temperature": {
-            "sql_query": f'SELECT mean("temperature") AS "outside_temperature_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
-            "measurement": "state",
-        },
-        "humidity": {
-            "sql_query": f'SELECT mean("humidity") AS "outside_humidity_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
-            "measurement": "state",
-        },
-        "wind_speed": {
-            "sql_query": f'SELECT mean("wind_speed") AS "outside_wind_speed_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
-            "measurement": "state",
-        },
-        "presence": {
-            "sql_query": f'SELECT count(distinct("friendly_name_str")) AS "device_presence_distinct_count" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "state"=\'home\' GROUP BY time({group_by_time_interval}) FILL(0)',
-            "measurement": "state",
-        },
-        "boiler_water_temperature": {
-            "sql_query": f'SELECT mean("value") AS "boiler_water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.tmp_boiler_case_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
-            "measurement": "°C",
-        },
-        "boiler_relay_status": {
-            "sql_query": f'SELECT last("value") AS "boiler_relay_status" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.relay_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
-            "measurement": "state",
-        },
-        "device_longitude": {
-            "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
-            "measurement": "state",
-        },
-        "device_latitude": {
-            "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
-            "measurement": "state",
-        },
-        
-    } 
+            "water_flow": {
+                "sql_query": f'SELECT mean("value") AS "water_flow_L_per_minute_mean" FROM "{self.db_name}"."autogen"."L/min" WHERE time > {left_time_interval} AND time <= {right_time_interval} GROUP BY time({group_by_time_interval}) FILL(0)',
+                "measurement": "L/min",
+            },
+            "water_temperature": {
+                "sql_query": f'SELECT mean("value") AS "water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND ("entity_id"=\'{self.tmp_output_water_entity_id}\' OR "entity_id"=\'{self.tmp_output_water_entity_id_2}\') GROUP BY time({group_by_time_interval}) FILL(0)',
+                "measurement": "°C",
+            },
+            "temperature": {
+                "sql_query": f'SELECT mean("temperature") AS "outside_temperature_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
+                "measurement": "state",
+            },
+            "humidity": {
+                "sql_query": f'SELECT mean("humidity") AS "outside_humidity_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
+                "measurement": "state",
+            },
+            "wind_speed": {
+                "sql_query": f'SELECT mean("wind_speed") AS "outside_wind_speed_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
+                "measurement": "state",
+            },
+            "presence": {
+                "sql_query": f'SELECT count(distinct("friendly_name_str")) AS "device_presence_distinct_count" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "state"=\'home\' GROUP BY time({group_by_time_interval}) FILL(0)',
+                "measurement": "state",
+            },
+            "boiler_water_temperature": {
+                "sql_query": f'SELECT mean("value") AS "boiler_water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.tmp_boiler_case_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
+                "measurement": "°C",
+            },
+            "boiler_relay_status": {
+                "sql_query": f'SELECT last("value") AS "boiler_relay_status" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.relay_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
+                "measurement": "state",
+            },
+            "device_longitude": {
+                "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+                "measurement": "state",
+            },
+            "device_latitude": {
+                "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+                "measurement": "state",
+            },
+            "device_longitude_2": {
+                "sql_query": f'SELECT mean("longitude") AS "mean_longitude_2" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id_2}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+                "measurement": "state",
+            },
+            "device_latitude_2": {
+                "sql_query": f'SELECT mean("latitude") AS "mean_latitude_2" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id_2}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+                "measurement": "state",
+            },
+        }
+
+    def haversine_dist(self, x1: float, x2: float, y1: float, y2: float) -> float:
+        """Calculates the distance between two coordinates
+
+        Args:
+            x1 (float): X of the first coordinate.
+            x2 (float): X of the second coordinate.
+            y1 (float): Y of the first coordinate.
+            y2 (float): Y of the second coordinate.
+
+        Returns:
+            float: Distance between two coordinates.
+        """
 
-    def haversine_dist(self, x1, x2, y1, y2):
         return haversine((x1, x2), (y1, y2), unit="km")
 
     # Data Processing
 
-    def extract_features_from_longitude_latitude(self, df_old):
-        #drop na in columns mean_latitude and mean_longitude
+    def extract_features_from_longitude_latitude(
+        self, df_old: pd.DataFrame
+    ) -> pd.DataFrame:
+        """Extracts the features from longitude and latitude as speed_towards_home, distance_from_home, heading_to_home_sin, heading_to_home_cos.
+
+        Args:
+            df_old (pd.DataFrame): Incoming dataframe.
+
+        Returns:
+            pd.DataFrame: Dataframe with extracted features.
+        """
+
+        # drop na in columns mean_latitude and mean_longitude
         df = df_old.copy()
-        
+
         df = df.dropna(subset=["mean_latitude", "mean_longitude"])
-        df.loc[:,"distance_from_home"] = np.vectorize(self.haversine_dist)(
+        df.loc[:, "distance_from_home"] = np.vectorize(self.haversine_dist)(
             df["mean_latitude"],
             df["mean_longitude"],
             self.home_latitude,
             self.home_longitude,
         )
 
-        df.loc[:,"heading_to_home"] = np.arctan2(
+        df.loc[:, "heading_to_home"] = np.arctan2(
             df["mean_latitude"] - self.home_latitude,
             df["mean_longitude"] - self.home_longitude,
         )
-        df.loc[:,"heading_to_home_sin"] = np.sin(df["heading_to_home"])
-        df.loc[:,"heading_to_home_cos"] = np.cos(df["heading_to_home"])
+        df.loc[:, "heading_to_home_sin"] = np.sin(df["heading_to_home"])
+        df.loc[:, "heading_to_home_cos"] = np.cos(df["heading_to_home"])
         # resample by 10m mean
-        df.loc[:,"time_stamp"] = df.index
+        df.loc[:, "time_stamp"] = df.index
         # calculate the speed of device
-        df.loc[:,"time_diff"] = (
+        df.loc[:, "time_diff"] = (
             df["time_stamp"].diff().dt.total_seconds() / 3600
         )  # Convert seconds to hours
-        df.loc[:,"distance"] = np.vectorize(self.haversine_dist)(
+        df.loc[:, "distance"] = np.vectorize(self.haversine_dist)(
             df["mean_latitude"],
             df["mean_longitude"],
             df["mean_latitude"].shift(1),
             df["mean_longitude"].shift(1),
         )  # calculate haversine distance
-        # df['hours'] = (df['time_stamp'].astype(int) / 10**9) / 60*60 # convert to seconds
-        # df['time_taken'] = df['hours'] - df['hours'].shift(1) # calculate time difference
 
-        df.loc[:,"speed"] = df["distance"] / df["time_diff"]  # cal speed
+        df.loc[:, "speed"] = df["distance"] / df["time_diff"]  # cal speed
         df.loc[df["speed"] > 200, "speed"] = 0
-        df.loc[:,"speed_towards_home"] = df["speed"] * df["heading_to_home_cos"]
+        df.loc[:, "speed_towards_home"] = df["speed"] * df["heading_to_home_cos"]
+
+        #######
+
+        df = df.dropna(subset=["mean_latitude_2", "mean_longitude_2"])
+        df.loc[:, "distance_from_home_2"] = np.vectorize(self.haversine_dist)(
+            df["mean_latitude_2"],
+            df["mean_longitude_2"],
+            self.home_latitude,
+            self.home_longitude,
+        )
+
+        df.loc[:, "heading_to_home_2"] = np.arctan2(
+            df["mean_latitude_2"] - self.home_latitude,
+            df["mean_longitude_2"] - self.home_longitude,
+        )
+        df.loc[:, "heading_to_home_sin_2"] = np.sin(df["heading_to_home_2"])
+        df.loc[:, "heading_to_home_cos_2"] = np.cos(df["heading_to_home_2"])
+        # resample by 10m mean
+        df.loc[:, "time_stamp_2"] = df.index
+        # calculate the speed of device
+        df.loc[:, "time_diff_2"] = (
+            df["time_stamp_2"].diff().dt.total_seconds() / 3600
+        )  # Convert seconds to hours
+        df.loc[:, "distance_2"] = np.vectorize(self.haversine_dist)(
+            df["mean_latitude_2"],
+            df["mean_longitude_2"],
+            df["mean_latitude_2"].shift(1),
+            df["mean_longitude_2"].shift(1),
+        )  # calculate haversine distance
+
+        df.loc[:, "speed_2"] = df["distance_2"] / df["time_diff_2"]  # cal speed
+        df.loc[df["speed_2"] > 200, "speed_2"] = 0
+        df.loc[:, "speed_towards_home_2"] = df["speed_2"] * df["heading_to_home_cos_2"]
+
         return df
 
-    def get_lowest_area_tmp(
-        self,
-        entity_id,
-        measurement="°C",
-        left_time_interval=datetime.now() - timedelta(days=21),
-        right_time_interval=datetime.now(),
-    ):
-        query = f'SELECT min("value") AS "temperature" FROM "{self.db_name}"."autogen"."{measurement}" WHERE "entity_id"=\'{entity_id}\' ORDER BY "temperature" ASC LIMIT {limit}'
-        result = self.dataframe_client.query(query)
-        return result
+    def get_df_from_queries(self, queries: dict) -> pd.DataFrame:
+        """Get the data from the database based on the queries.
+
+        Args:
+            queries (dict): Dictionary of queries.
+
+        Returns:
+            pd.DataFrame: Result dataframe.
+        """
 
-    def get_df_from_queries(self, queries):
         df_all_list = []
         # iterate over key an value in data
-        for key, value in queries.items():
+        for _, value in queries.items():
 
-            # print(value["sql_query"])
             result = self.dataframe_client.query(value["sql_query"])[
                 value["measurement"]
             ]
             df = pd.DataFrame(result)
             df_all_list.append(df)
 
         df = pd.concat(df_all_list, axis=1)
 
         return df
 
-    def process_kWh_water_consumption(self, df):
+    def process_kWh_water_consumption(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Method to process the data from the database and calculate the consumed heat in kWh
+
+        Args:
+            df (pd.DataFrame): Dataframe with statistics from db.
+
+        Returns:
+            pd.DataFrame: Dataframe with processed data.
+        """
+
+        divide_heat_coefficient = 0.6
+        # resample the data by 1 min as the flow is represended as L/min
         df = df.resample("1min").mean()
-        # df = df.reset_index(drop=True)
+
+        # calculation of consumed kJ
         df["consumed_heat_kJ"] = (
             df["water_flow_L_per_minute_mean"]
             * (df["water_temperature_mean"] - 10)
             * 4.186
-            * 0.6
-        )  
-
+            * divide_heat_coefficient
+        )
+        # extraction of features from device position
         df = self.extract_features_from_longitude_latitude(df)
-        # all value in speed larger than 200 set to 0
+
+        # cleaning the outliners from speed feature
         df.loc[df["speed"] > 200, "speed"] = 0
 
+        # aggregate by 60 minutes
         df = df.groupby(pd.Grouper(freq="60T"))
         df = df.agg(
             {
                 "consumed_heat_kJ": "sum",
                 "water_flow_L_per_minute_mean": "mean",
                 "water_temperature_mean": "mean",
                 "outside_temperature_mean": "mean",
                 "outside_humidity_mean": "mean",
                 "outside_wind_speed_mean": "mean",
-                "device_presence_distinct_count": "mean",
+                "device_presence_distinct_count": "max",
                 "mean_longitude": "mean",
                 "mean_latitude": "mean",
                 "speed": "mean",
                 "speed_towards_home": "mean",
                 "distance_from_home": "mean",
                 "heading_to_home_sin": "mean",
                 "heading_to_home_cos": "mean",
+                "mean_longitude_2": "mean",
+                "mean_latitude_2": "mean",
+                "speed_2": "mean",
+                "speed_towards_home_2": "mean",
+                "distance_from_home_2": "mean",
+                "heading_to_home_sin_2": "mean",
+                "heading_to_home_cos_2": "mean",
             }
         )
+
+        # transform kj to kWh
         df["consumed_heat_kWh"] = df["consumed_heat_kJ"] / 3600
         df = df.drop(columns=["consumed_heat_kJ"])
 
         return df
 
     def get_data_for_training_model(
         self,
-        left_time_interval=None,
-        right_time_interval=datetime.now(),
-        predicted_column="longtime_mean",
-    ):
+        left_time_interval: Optional[datetime] = None,
+        right_time_interval: Optional[datetime] = None,
+    ) -> pd.DataFrame:
+        """Method to retrieve data for training.
+
+        Args:
+            left_time_interval (Optional[datetime], optional): Left time datetime. Defaults to self.start_of_data.
+            right_time_interval (Optional[datetime], optional): Right time datetime. Defaults to datetime.now().
+
+        Returns:
+            pd.DataFrame: Resulting dataframe.
+        """
+
+        # default the intervals if None
         if left_time_interval is None:
             left_time_interval = self.start_of_data
+
+        if right_time_interval is None:
+            right_time_interval = datetime.now()
+
+        left_time_interval = left_time_interval.replace(
+            minute=0, second=0, microsecond=0
+        )
+        right_time_interval = right_time_interval.replace(
+            minute=0, second=0, microsecond=0
+        )
+
+        # retrieve the queries based on the intervals
         queries = self.get_database_queries(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
+        # get the data from the database
         df_all = self.get_df_from_queries(queries)
+        # process the data
         df_all = self.process_kWh_water_consumption(df_all)
-
-        return self.transform_data_for_ml(df_all, predicted_column=predicted_column)
+        # transform for ML
+        return self.transform_data_for_ml(df_all)
 
     def get_data_for_prediction(
         self,
-        left_time_interval=datetime.now() - timedelta(days=5),
-        right_time_interval=datetime.now(),
-    ):
-        
-        left_time_interval = left_time_interval.replace(minute=0, second=0, microsecond=0)
-        right_time_interval = right_time_interval.replace(minute=0, second=0, microsecond=0)
-        
+        left_time_interval: Optional[datetime] = None,
+        right_time_interval: Optional[datetime] = None,
+    ) -> tuple[pd.DataFrame, pd.DatetimeIndex]:
+        """Method to get data for the prediction.
+
+        Args:
+            left_time_interval (Optional[datetime], optional): Left time datetime. Defaults to datetime.now()-timedelta(days=5).
+            right_time_interval (Optional[datetime], optional): Right time datetime. Defaults to datetime.now().
+
+        Returns:
+            tuple[pd.DataFrame, pd.DatetimeIndex]: Tuple with dataframe and datetime index.
+        """
+        # defaulting the intervals if None
+        if left_time_interval is None:
+            left_time_interval = datetime.now() - timedelta(days=5)
+        if right_time_interval is None:
+            right_time_interval = datetime.now()
+
+        # replace the minutes, seconds and microseconds with 0 to get the full hour
+        left_time_interval = left_time_interval.replace(
+            minute=0, second=0, microsecond=0
+        )
+        right_time_interval = right_time_interval.replace(
+            minute=0, second=0, microsecond=0
+        )
+        # get the queries for the database
         queries = self.get_database_queries(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
+        # get the data from the database
         df_all = self.get_df_from_queries(queries)
+
+        # process the data
         df_all = self.process_kWh_water_consumption(df_all)
+
+        # transform the data for ML
         df_all.index = df_all.index.tz_localize(None)
-        df_all, datetimes = self.transform_data_for_ml(df_all, predicted_column="longtime_mean")
+
+        # return the dataframe and the datetimes
+        df_all, datetimes = self.transform_data_for_ml(df_all)
 
         return df_all, datetimes
 
-    def write_forecast_to_influxdb(self, df, measurement_name):
+    def write_forecast_to_influxdb(self, df: pd.DataFrame) -> None:
+        """Method which writes the current forecast to the influxdb.
+
+        Args:
+            df (pd.DataFrame): Dataframe with current prediction.
+        """
         current_time = datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
 
         df.index = df.index.astype(str)
 
         # Create dictionary
         result_dict = df.squeeze().to_dict()
-        print(f'Writing forecast to influxdb: {result_dict}')
         # Create a dictionary
         measurement_dict = {
             "measurement": "prediction",
             "time": current_time,
             "fields": result_dict,
         }
 
+        print(f"Writing forecast to influxdb: {measurement_dict}")
         self.influxdb_client.write_points([measurement_dict])
-        # return measurement_dict
 
-    def get_high_tarif_schedule(self):
-        print("Getting high tarif schedule")
+    def get_high_tarif_schedule(self) -> pd.DataFrame:
+        """Method to retrieve the high tarif schedule from data for the last 14 days.
+
+        Returns:
+            pd.DataFrame: Dataframe with high tarif schedule by hour in each weekday.
+        """
+
         left_time_interval = datetime.now() - timedelta(days=14)
         queries = self.get_database_queries(
             left_time_interval=left_time_interval, right_time_interval=datetime.now()
         )
         df_all = self.get_df_from_queries(queries)
         df_all.index = df_all.index.tz_localize(None)
         data_resampled = df_all.resample("10T").max()
@@ -361,171 +546,200 @@
         df_reset = df_reset.drop(
             columns=["level_0", "level_1", "level_2", "boiler_relay_status"]
         )
 
         return df_reset
 
     def transform_data_for_ml(
-        self, df, days_from_beginning_ignored=0, predicted_column="longtime_mean"
-    ):
-        # read pickles from data/pickles
+        self, df: pd.DataFrame
+    ) -> tuple[pd.DataFrame, pd.DatetimeIndex]:
+        """Method to transform the data for ML model.
+
+        Args:
+            df (pd.DataFrame): Dataframe to transform.
+
+        Returns:
+            tuple[pd.DataFrame, pd.DatetimeIndex]: Transformed dataframe and datetime.
+        """
 
+        # frequency i hours
         freq = 1
-        freq_hour = f"{freq}H"
-
         df.index = pd.to_datetime(df.index)
 
         df.loc[:, "weekday"] = df.index.weekday
         df.loc[:, "hour"] = df.index.hour
-        # df.loc[:, "minute"] = df.index.minute
         df.loc[:, "minute"] = 0
 
-        # delete rows with weekday nan
-        # df = df.dropna(subset=["weekday"])
+        # fill consumed_heat_kWh with 0 if nan
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].fillna(0)
 
         # fill negative values with 0
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].clip(lower=0)
 
-        # fill na in df based on column
+        # ffill na in df based on column
         df["temperature"] = df[f"outside_temperature_mean"].fillna(method="ffill")
         df["humidity"] = df[f"outside_humidity_mean"].fillna(method="ffill")
         df["wind_speed"] = df[f"outside_wind_speed_mean"].fillna(method="ffill")
         df["count"] = df["device_presence_distinct_count"].fillna(method="ffill")
+
         df["mean_longitude"] = df["mean_longitude"].fillna(method="ffill")
         df["mean_latitude"] = df["mean_latitude"].fillna(method="ffill")
         df["speed"] = df["speed"].fillna(0)
         df["speed_towards_home"] = df["speed_towards_home"].fillna(0)
         df["distance_from_home"] = df["distance_from_home"].fillna(method="ffill")
         df["heading_to_home_sin"] = df["heading_to_home_sin"].fillna(method="ffill")
         df["heading_to_home_cos"] = df["heading_to_home_cos"].fillna(method="ffill")
 
-        # add to column 'consumed_heat_kWh' 1,25/6 to each row
-        # df = df.drop(df[df["consumed_heat_kWh"] == 0].sample(frac=0.7).index)
+        df["mean_longitude_2"] = df["mean_longitude_2"].fillna(method="ffill")
+        df["mean_latitude_2"] = df["mean_latitude_2"].fillna(method="ffill")
+        df["speed_2"] = df["speed_2"].fillna(0)
+        df["speed_towards_home_2"] = df["speed_towards_home_2"].fillna(0)
+        df["distance_from_home_2"] = df["distance_from_home_2"].fillna(method="ffill")
+        df["heading_to_home_sin_2"] = df["heading_to_home_sin_2"].fillna(method="ffill")
+        df["heading_to_home_cos_2"] = df["heading_to_home_cos_2"].fillna(method="ffill")
+
+        # adding cooling down to the consumed heat
         df["consumed_heat_kWh"] += 1.25 / (24 // freq)
-        # drop randomly 60 percent of rows where consumed_heat_kWh is 0
-        window = 3
 
+        window = 3
+        # creating a 3 hour rolling window for the mean of the consumed heat for better prediction
         df["longtime_mean"] = (
             df["consumed_heat_kWh"]
             .rolling(window=window, min_periods=1, center=True)
             .mean()
         )
+        # extrahing next features
+        df["last_3_week_mean"] = (
+            df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
+            .rolling(window=3, min_periods=1)
+            .mean()
+            .reset_index(level=[0, 1], drop=True)
+        )
+        df["last_3_week_mean"] = df["last_3_week_mean"].fillna(method="ffill")
 
+        df["last_3_week_std"] = (
+            df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
+            .rolling(window=3, min_periods=1)
+            .std()
+            .reset_index(level=[0, 1], drop=True)
+        )
+        df["last_3_week_std"] = df["last_3_week_std"].fillna(method="ffill")
+
+        df["last_3_week_max"] = (
+            df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
+            .rolling(window=3, min_periods=1)
+            .max()
+            .reset_index(level=[0, 1], drop=True)
+        )
+        df["last_3_week_max"] = df["last_3_week_max"].fillna(method="ffill")
+
+        df["last_3_week_min"] = (
+            df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
+            .rolling(window=3, min_periods=1)
+            .min()
+            .reset_index(level=[0, 1], drop=True)
+        )
+        df["last_3_week_min"] = df["last_3_week_min"].fillna(method="ffill")
+
+        df["last_3_week_skew"] = (
+            df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
+            .rolling(window=3, min_periods=1)
+            .skew()
+            .reset_index(level=[0, 1], drop=True)
+        )
+        df["last_3_week_skew"] = df["last_3_week_skew"].fillna(method="ffill")
+        # fill
+
+        df["last_3_week_median"] = (
+            df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
+            .rolling(window=3, min_periods=1)
+            .median()
+            .reset_index(level=[0, 1], drop=True)
+        )
+        df["last_3_week_median"] = df["last_3_week_median"].fillna(method="ffill")
 
-        # drop consumed_heat_kWh
-        
-        df['last_3_week_mean'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).mean().reset_index(level=[0,1], drop=True)
-        df['last_3_week_mean'] = df['last_3_week_mean'].fillna(method='ffill')
-        
-        df['last_3_week_std'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).std().reset_index(level=[0,1], drop=True)
-        df['last_3_week_std'] = df['last_3_week_std'].fillna(method='ffill')
-        
-        df['last_3_week_max'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).max().reset_index(level=[0,1], drop=True)
-        df['last_3_week_max'] = df['last_3_week_max'].fillna(method='ffill')
-        
-        df['last_3_week_min'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).min().reset_index(level=[0,1], drop=True)
-        df['last_3_week_min'] = df['last_3_week_min'].fillna(method='ffill')
-        
-        df['last_3_week_skew'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).skew().reset_index(level=[0,1], drop=True)
-        df['last_3_week_skew'] = df['last_3_week_skew'].fillna(method='ffill')
-        #fill 
-        
-        df['last_3_week_median'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).median().reset_index(level=[0,1], drop=True)
-        df['last_3_week_median'] = df['last_3_week_median'].fillna(method='ffill') 
-        
-        
-        
         df_reverse = df.iloc[::-1]
 
-        nan_indices = df_reverse[df_reverse['last_3_week_skew'].isna()].index
-
+        # getting nan indices and filling them with rolling mean from the end of the dataframe
+        nan_indices = df_reverse[df_reverse["last_3_week_skew"].isna()].index
         for index in nan_indices:
 
-            rolling_skew = df_reverse.loc[index:, 'consumed_heat_kWh'].rolling(window=3, min_periods=1).skew()
-            rolling_std = df_reverse.loc[index:, 'consumed_heat_kWh'].rolling(window=3, min_periods=1).std()
-            df_reverse.loc[index:, 'last_3_week_skew'] = np.where(df_reverse.loc[index:, 'last_3_week_skew'].isna(), rolling_skew, df_reverse.loc[index:, 'last_3_week_skew'])
-            df_reverse.loc[index:, 'last_3_week_std'] = np.where(df_reverse.loc[index:, 'last_3_week_std'].isna(), rolling_std, df_reverse.loc[index:, 'last_3_week_std'])
-
-        df['last_3_week_skew'] = df_reverse['last_3_week_skew'].iloc[::-1]
-        df['last_3_week_std'] = df_reverse['last_3_week_std'].iloc[::-1]
-        
-        
+            rolling_skew = (
+                df_reverse.loc[index:, "consumed_heat_kWh"]
+                .rolling(window=3, min_periods=1)
+                .skew()
+            )
+            rolling_std = (
+                df_reverse.loc[index:, "consumed_heat_kWh"]
+                .rolling(window=3, min_periods=1)
+                .std()
+            )
+            df_reverse.loc[index:, "last_3_week_skew"] = np.where(
+                df_reverse.loc[index:, "last_3_week_skew"].isna(),
+                rolling_skew,
+                df_reverse.loc[index:, "last_3_week_skew"],
+            )
+            df_reverse.loc[index:, "last_3_week_std"] = np.where(
+                df_reverse.loc[index:, "last_3_week_std"].isna(),
+                rolling_std,
+                df_reverse.loc[index:, "last_3_week_std"],
+            )
+
+        df["last_3_week_skew"] = df_reverse["last_3_week_skew"].iloc[::-1]
+        df["last_3_week_std"] = df_reverse["last_3_week_std"].iloc[::-1]
+
         df = df.drop(columns=["consumed_heat_kWh"])
+
         # transform weekday, minute, hour to sin cos
         df["weekday_sin"] = np.sin(2 * df["weekday"] * np.pi / 7)
         df["weekday_cos"] = np.cos(2 * df["weekday"] * np.pi / 7)
 
         df["hour_sin"] = np.sin(2 * df["hour"] * np.pi / 24)
         df["hour_cos"] = np.cos(2 * df["hour"] * np.pi / 24)
 
         df["minute_sin"] = np.sin(2 * df["minute"] * np.pi / 60)
         df["minute_cos"] = np.cos(2 * df["minute"] * np.pi / 60)
 
+        # result df with features and target variable as a first
         df = df[
             [
                 "longtime_mean",
                 "last_3_week_skew",
                 "last_3_week_std",
                 "distance_from_home",
                 "speed_towards_home",
+                # "distance_from_home_2",
+                # "speed_towards_home_2",
                 "count",
                 "heading_to_home_sin",
                 "heading_to_home_cos",
+                # "heading_to_home_sin_2",
+                # "heading_to_home_cos_2",
                 "temperature",
                 "humidity",
                 "wind_speed",
                 "weekday_sin",
                 "weekday_cos",
                 "hour_sin",
                 "hour_cos",
-
             ]
         ]
-        # df = df[
-        #     [
-        #         predicted_column,
-        #         "weekday_sin",
-        #         "weekday_cos",
-        #         "hour_sin",
-        #         "hour_cos",
-        #         "minute_sin",
-        #         "minute_cos",
-        #         "hea"
-        #     ]
-        # ]
-
-        # df = df.dropna(subset=["longtime_mean", "distance_from_home"])
 
         # extract datetimes from index
         datetimes = df.index
 
         return (df.reset_index(drop=True), datetimes)
 
-    def write_data(self, data):
-        with open(self.data_file, "w") as file:
-            json.dump(data, file)
-
 
 if __name__ == "__main__":
-    # test
 
     dataHandler = DataHandler(
         influx_id="localhost",
         db_name="smart_home_zukalovi",
         db_username="root",
         db_password="root",
         relay_entity_id="shelly1pm_84cca8b07eae",
         relay_power_entity_id="shelly1pm_84cca8b07eae_power",
         tmp_boiler_case_entity_id="esphome_web_c771e8_tmp3",
         tmp_output_water_entity_id="esphome_web_c771e8_ntc_temperature_b_constant_2",
         start_of_data=datetime(2024, 3, 1, 0, 0, 0, 0),
     )
-    # df_from_db = data_handler.get_data_for_training_model()
-    # dropna - remove rows with NaN
-    # result = data_handler.transform_data_for_ml(df_from_db)
-    dataHandler = dataHandler.get_data_for_high_tarif_info()
-
-    # data_handler.get_data_for_prediction()
-    # data_handler.get_actual_data()
-    # data_handler.transform_data_for_ml()
-    # data_handler.write_data()
```

### Comparing `smartboiler-0.0.3.0.0.7.4/src/smartboiler/event_checker.py` & `smartboiler-0.1.2/src/smartboiler/event_checker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,145 +1,150 @@
-##########################################################
-# Bachelor's thesis                                      #
-# From a dumb boiler to a smart one using a smart socket #
-# Author: Adam Grünwald                                  #
-# BUT FIT BRNO, Faculty of Information Technology        #
-# 26/6/2021                                              #
-#                                                        #
-# Module with class used for comunicating with Google    #
-# Calendar API and searching for special events.         #
-##########################################################
+# Created as a part of Master's Thesis "Using machine learning methods to save energy in a smart home"
+# Faculty of Information Technology, Brno University of Technology, 2024
+# Author: Adam Grünwald
+#
+# This module is used for communicating with Google Calendar API and searching for special events.
+
 
 from __future__ import print_function
-import json
-import datetime
-import time
+from datetime import datetime, timezone, timedelta
 import pickle
 import os.path
 import re
-# from googleapiclient.discovery import build
-# from google_auth_oauthlib.flow import InstalledAppFlow
-# from google.auth.transport.requests import Request
 
-from time_handler import TimeHandler
+from google.auth.transport.requests import Request
+from google_auth_oauthlib.flow import InstalledAppFlow
+from googleapiclient.discovery import build
+from google.oauth2.credentials import Credentials
 
+from smartboiler.time_handler import TimeHandler
 
-class EventChecker:
 
-    def __init__(self, token_path='token.pickle', credentials_path='credentials.json'):
+class EventChecker:
+    """Class for communicating with Google Calendar API and searching for special events."""
 
-        self.SCOPES = ['https://www.googleapis.com/auth/calendar.readonly']
+    def __init__(self):
+        """Initialize the class with the scopes for Google Calendar API and TimeHandler class."""
+        self.SCOPES = ["https://www.googleapis.com/auth/calendar.readonly"]
         self.TimeHandler = TimeHandler()
 
-    def load_events(self):
+    def load_events(self) -> list:
         """Loads events from Google Calendar API using credentials of Google Calendar.
 
         Code for communicating with Google Calendar API is inspired by a manual on https://developers.google.com/calendar/
         quickstart/python
 
         Returns:
             [list]: [list of events]
         """
-
-        creds = None
-
-        if os.path.exists('token.pickle'):
-            with open('token.pickle', 'rb') as token:
-                creds = pickle.load(token)
-        if not creds or not creds.valid:
-            if creds and creds.expired and creds.refresh_token:
-                creds.refresh(Request())
-            else:
-                flow = InstalledAppFlow.from_client_secrets_file(
-                    'credentials.json', self.SCOPES)
-                creds = flow.run_local_server(port=0)
-            with open('token.pickle', 'wb') as token:
-                pickle.dump(creds, token)
-
         try:
-            service = build('calendar', 'v3', credentials=creds)
-        except:
-            print("couldn't build service")
-            return
-        now = datetime.datetime.now(datetime.UTC).isoformat() + 'Z'
-        try:
-            events_result = service.events().list(calendarId='primary', timeMin=now,
-                                                  maxResults=1, singleEvents=True,
-                                                  orderBy='startTime').execute()
-            events = events_result.get('items', [])
+
+            creds = None
+            token_file = "/app/token.json"
+            creds_file = "/app/credentials.json"
+            
+            if os.path.exists(token_file):
+                creds = Credentials.from_authorized_user_file(token_file, self.SCOPES)
+            # If there are no (valid) credentials available, let the user log in.
+            if not creds or not creds.valid:
+                if creds and creds.expired and creds.refresh_token:
+                    creds.refresh(Request())
+                else:
+                    flow = InstalledAppFlow.from_client_secrets_file(
+                        creds_file, self.SCOPES
+                    )
+                    creds = flow.run_local_server(port=0)
+                # Save the credentials for the next run
+                with open(token_file, "w") as token:
+                    token.write(creds.to_json())
+
+            service = build("calendar", "v3", credentials=creds)
+
+            now = datetime.now().isoformat() + "Z"
+            
+            events_result = (
+                service.events()
+                .list(
+                    calendarId="primary",
+                    timeMin=now,
+                    maxResults=1,
+                    singleEvents=True,
+                    orderBy="startTime",
+                )
+                .execute()
+            )
+            events = events_result.get("items", [])
             return events
-        except:
-            print("couldn't get events")
+        except Exception as e:
+            print("Error while loading events")
+            print(e)
             return None
 
-    def next_calendar_heat_up_event(self, Boiler):
+    def next_calendar_heat_up_event(self) -> dict:
         """Search next event in a calendar which contains specific words describing the process of heating up.
 
         Args:
-            Boiler ([class]): [class of boiler]
 
         Returns:
             [dict]: [dictionary describing next heating up event]
         """
         events = self.load_events()
-        return_dict = {"hours_to_event": None, "degree_target": None}
+        return_dict = {"minutes_to_event": None, "degree_target": None}
 
         if events:
             for e in events:
-                if re.match('^.*boiler heat up at (\d+) degrees$', e['summary']):
+                if re.match("^.*boiler heat up at (\d+) degrees$", e["summary"]):
                     degree_target = int(
-                        re.split('^.*boiler heat up at (\d+) degrees$', e['summary'])[1])
+                        re.split("^.*boiler heat up at (\d+) degrees$", e["summary"])[1]
+                    )
                     start = self.TimeHandler.date_to_datetime(
-                        e['start'].get('dateTime', e['start'].get('date')))
-                    time_to_event = (start - (datetime.datetime.now() +
-                                     datetime.timedelta(hours=1))) / datetime.timedelta(hours=1)
-
-                    if (time_to_event > 0):
-
-                        return_dict['hours_to_event'] = time_to_event
-                        return_dict['degree_target'] = degree_target
-                    break
-                # if re.match('^.*Prepare (\d+) showers$', e['summary']):
-                #     number_of_showers = int(
-                #         re.split('^.*Prepare (\d+) showers$', e['summary'])[1])
-
-                #     degree_target = Boiler.showers_degrees(
-                #         number_of_showers=number_of_showers)
-
-                #     start = self.TimeHandler.date_to_datetime(
-                #         e['start'].get('dateTime', e['start'].get('date')))
-                #     time_to_event = (start - (datetime.datetime.now() +
-                #                      datetime.timedelta(hours=1))) / datetime.timedelta(hours=1)
-
-                #     if (time_to_event > 0):
-
-                #         return_dict['hours_to_event'] = time_to_event
-                #         return_dict['degree_target'] = degree_target
-                #     break
+                        e["start"].get("dateTime", e["start"].get("date"))
+                    )
+                    end = self.TimeHandler.date_to_datetime(
+                        e["end"].get("dateTime", e["end"].get("date"))
+                    )
+                    time_to_event = (
+                        start - (datetime.now() + timedelta(hours=1))
+                    ) / timedelta(hours=1)
+                    time_to_end_event = (
+                        end - (datetime.now() + timedelta(hours=1))
+                    ) / timedelta(hours=1)
+                    
+                    if time_to_event > 0:
+
+                        return_dict["minutes_to_event"] = time_to_event * 60
+                        return_dict["degree_target"] = degree_target
+
+                        return return_dict
+                    # case in event
+                    elif time_to_end_event > 0:
+                        return_dict["minutes_to_event"] = 0
+                        return_dict["degree_target"] = degree_target
+
+                        return return_dict
 
         return return_dict
 
-    def check_off_event(self):
+    def check_off_event(self) -> bool:
         """Search for an event for turning off the boiler.
 
         Returns:
-            [type]: [description]
+            [bool]: [if the turn offevent is happening now or not]
         """
         events = self.load_events()
-        if not events:
-            return False
-        else:
+        if events:
             for e in events:
 
-                if("#off" in e['summary']):
+                if "#off" in e["summary"]:
                     start = self.TimeHandler.date_to_datetime(
-                        e['start'].get('dateTime', e['start'].get('date')))
+                        e["start"].get("dateTime", e["start"].get("date"))
+                    )
                     end = self.TimeHandler.date_to_datetime(
-                        e['end'].get('dateTime', e['end'].get('date')))
-
+                        e["end"].get("dateTime", e["end"].get("date"))
+                    )
                     return self.TimeHandler.is_date_between(start, end)
-            return False
+        return False
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     e = EventChecker()
-    e.check_event()
+    print(e.next_calendar_heat_up_event())
```

### Comparing `smartboiler-0.0.3.0.0.7.4/src/smartboiler/forecast.py` & `smartboiler-0.1.2/src/smartboiler/forecast.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,129 @@
-from pathlib import Path
+# Created as a part of Master's Thesis "Using machine learning methods to save energy in a smart home"
+# Faculty of Information Technology, Brno University of Technology, 2024
+# Author: Adam Grünwald
+#
+# This module is used for training the model for prediction and creating predictions.
 
-print("Running" if __name__ == "__main__" else "Importing", Path(__file__).resolve())
+from typing import Optional
 from datetime import timedelta, datetime
-from sklearn.preprocessing import MinMaxScaler, RobustScaler
+from sklearn.preprocessing import RobustScaler
 from keras.models import Sequential
 
-# import tensorflow as tf
 from keras.layers import LSTM
-from keras.layers import Dropout
-from keras.models import Model
 from keras.layers import Input, Dense
-from keras.models import load_model
 from keras.callbacks import EarlyStopping, ModelCheckpoint
 import keras.backend as K
 import numpy as np
 import pandas as pd
 from pickle import load
 from pickle import dump
 
 
 from smartboiler.data_handler import DataHandler
 
 
 class Forecast:
+    """Class for training model for prediction and creating predictions"""
+
     def __init__(
         self,
         dataHandler: DataHandler,
         start_of_data: datetime,
-        model_path=None,
-        scaler_path=None,
-        predicted_columns=None,
+        model_path: Optional[str] = None,
+        scaler_path: Optional[datetime] = None,
+        predicted_columns: Optional[list] = None,
     ):
+        """Initialize the class of the forecast.
+
+        Args:
+            dataHandler (DataHandler): Instance of the DataHandler class
+            start_of_data (datetime): Datetime of the start of the data
+            model_path (Optional[str], optional): Path of the model. Defaults to None.
+            scaler_path (Optional[datetime], optional): Path of the scaler. Defaults to None.
+            predicted_columns (Optional[list], optional): List of columns for prediction. Defaults to None.
+        """
         self.batch_size = 16
         self.lookback = 32
-
         self.delay = 1
+        self.step = 1
+
+        self.num_of_features = 14
+
         self.predicted_columns = predicted_columns
         self.dataHandler = dataHandler
         self.scaler = RobustScaler()
         self.start_of_data = start_of_data
 
         self.model_path = model_path
         self.scaler_path = scaler_path
-        # Define the quantiles you want to predict
         self.quantiles = [0.1, 0.3, 0.5, 0.7, 0.9]
 
-
     def train_model(
         self,
-        begin_of_training=None,
-        end_of_training=None,
-        df_training_data=None,
-    ):
+        begin_of_training: Optional[datetime] = None,
+        end_of_training: Optional[datetime] = None,
+        df_training_data: Optional[pd.DataFrame] = None,
+    ) -> None:
+        """Method for training the model
+
+        Args:
+            begin_of_training (_type_, optional): Datetime of beggining of the data for training. Defaults to None.
+            end_of_training (_type_, optional): Datetime of end of the data used for training. Defaults to None.
+            df_training_data (_type_, optional): Dataframe with data for training.
+                                                If not None, this data will be used for training. Defaults to None.
+        """
+
+        # if the data for training is not provided, get the data from the dataHandler
         if df_training_data is None:
             if begin_of_training is None:
                 begin_of_training = self.start_of_data
             if end_of_training is None:
                 end_of_training = datetime.now()
-            print("begin of training: ", begin_of_training)
-            print("end of training : ", end_of_training)
             df_training_data, _ = self.dataHandler.get_data_for_training_model(
                 left_time_interval=begin_of_training,
                 right_time_interval=end_of_training,
-                predicted_columns=self.predicted_columns,
-                dropna=False,
             )
-
+        # get the number of features
         self.num_of_features = len(df_training_data.columns) - 1
+
+        # fit the scaler
         self.df_train_norm = df_training_data.copy()
         self.df_train_norm[df_training_data.columns] = self.scaler.fit_transform(
             df_training_data
         )
+        # save the scaler
         dump(self.scaler, open(self.scaler_path, "wb"))
 
+        # create a train validation generator
         self.train_gen = self.mul_generator(
             dataframe=self.df_train_norm,
             target_names=self.predicted_columns,
-            lookback=self.lookback,
-            delay=self.delay,
             min_index=0,
             max_index=int(df_training_data.shape[0] * 0.8),
-            step=1,
             shuffle=True,
-            batch_size=self.batch_size,
         )
 
         self.valid_gen = self.mul_generator(
             dataframe=self.df_train_norm,
             target_names=self.predicted_columns,
-            lookback=self.lookback,
-            delay=self.delay,
             min_index=int(df_training_data.shape[0] * 0.8),
             max_index=None,
-            step=1,
             shuffle=False,
-            batch_size=self.batch_size,
         )
 
+        # devide validity and train steps
         self.val_steps = int(
             (self.df_train_norm.shape[0] * 0.1 - self.lookback) // self.batch_size
         )
-        # This is how many steps to draw from `train_gen`
-        # in order to see the whole train set:
         self.train_steps = int(
             (self.df_train_norm.shape[0] * 0.9 - self.lookback) // self.batch_size
         )
 
+        # create a callbacks for training of the model
         callbacks = [
             EarlyStopping(
                 monitor="loss",
                 min_delta=0,
                 patience=10,
                 verbose=2,
                 mode="auto",
@@ -119,123 +133,85 @@
                 verbose=1,
                 filepath=self.model_path,
                 save_best_only=True,
                 save_weights_only=True,
             ),
         ]
 
-        print("Start training")
+        # fit the model
         history = self.model.fit(
             self.train_gen,
             steps_per_epoch=self.train_steps,
             epochs=100,
             shuffle=False,
             validation_data=self.valid_gen,
             validation_steps=self.val_steps,
             callbacks=callbacks,
             verbose=2,
         )
 
-        # self.model.save(self.model_path)
-        print("End training")
+        # save the weights of the model
+        self.model.save_weights(self.model_path, overwrite=True)
 
     def load_model(
         self,
-        left_time_interval=datetime.now() - timedelta(days=4),
-        right_time_interval=datetime.now(),
-    ):
-
+    ) -> None:
+        """Load model and scaler from the files"""
         self.scaler = load(open(self.scaler_path, "rb"))
-        self.model.load_weights(self.model_path)
+        self.model.load_weights(self.model_path, skip_mismatch=False)
 
-    def generator(
-        self,
-        dataframe,
-        target_name,
-        lookback,
-        delay,
-        min_index,
-        max_index,
-        shuffle=False,
-        batch_size=128,
-        step=6,
-    ):
-        data_without_target = dataframe.copy()
-        data_without_target = data_without_target.drop(columns=[target_name]).values
-        data_without_target = data_without_target.astype(np.float32)
-
-        data = dataframe.values
-        data = data.astype(np.float32)
-        target_indx = dataframe.columns.get_loc(target_name)
-
-        if max_index is None:
-            max_index = len(data) - delay - 1
-        i = min_index + lookback
-        while 1:
-            if shuffle:
-                rows = np.random.randint(
-                    min_index + lookback, max_index, size=batch_size
-                )
-            else:
-                if i + batch_size >= max_index:
-                    i = min_index + lookback
-                rows = np.arange(i, min(i + batch_size, max_index))
-                i += len(rows)
-
-            samples = np.zeros(
-                (len(rows), lookback // step, data_without_target.shape[-1])
-            )
-            targets = np.zeros((len(rows),))
-
-            for j, row in enumerate(rows):
-                indices = range(rows[j] - lookback, rows[j], step)
-                # samples without column with target
-                samples[j] = data_without_target[indices]
-                targets[j] = data[rows[j] + delay][target_indx]
-            yield samples, targets
-
-    def r2_keras(self, y_true, y_pred):
-        """Coefficient of Determination"""
-        SS_res = K.sum(K.square(y_true - y_pred))
-        SS_tot = K.sum(K.square(y_true - K.mean(y_true)))
-        return 1 - SS_res / (SS_tot + K.epsilon())
-    
-    def mean_absolute_percentage_error(self, y_true, y_pred):
-        epsilon = 1e-10
-        epsilon = K.constant(epsilon, dtype='float32')  # Assuming epsilon is a constant
-        y_true = K.cast(y_true, 'float32')
-        y_pred = K.cast(y_pred, 'float32')
-
-        diff = K.abs((y_true - y_pred) / K.maximum(K.abs(y_true), epsilon))
-        return 100. * K.mean(diff)
-    
-    def quantile_loss(self, q, y_true, y_pred):
-        # Example usage:
-        # Suppose you want to predict the median (q=0.5) and the 90th percentile (q=0.9)
+    def quantile_loss(self, q, y_true, y_pred) -> float:
+        """Quantile loss function used for training the model
 
+        Args:
+            q (float): quantil
+            y_true (float): value of the true data
+            y_pred (float): value of the predicted data
+
+        Returns:
+            float: the loss
+        """
         e = y_true - y_pred
         return K.mean(K.maximum(q * e, (q - 1) * e), axis=-1)
 
+    def build_model(self) -> None:
+        """Method for building the model"""
 
-    def build_model(self):
-
+        # Use the Sequential with LSTM layer with 100 units and Dense layer with 1 unit
         model = Sequential()
-        model.add(Input(shape=(None, 14)))
-
-        # Add LSTM layer
+        model.add(Input(shape=(None, self.num_of_features)))
         model.add(LSTM(100))
         model.add(Dense(1))
 
+        # compile the model with the quantile loss and adam optimizer
         self.model = model
-        self.model.compile(loss=[lambda y_true, y_pred: self.quantile_loss(q, y_true, y_pred) for q in self.quantiles], optimizer="adam")
-        return model
-
-    def add_empty_row(self, df, date_time, predicted_value):
+        self.model.compile(
+            loss=[
+                lambda y_true, y_pred: self.quantile_loss(q, y_true, y_pred)
+                for q in self.quantiles
+            ],
+            optimizer="adam",
+        )
 
+    def add_empty_row(
+        self, df: pd.DataFrame, date_time: datetime, predicted_value: float
+    ) -> pd.DataFrame:
+        """Methot adding an empty row to the dataframe
+
+        Args:
+            df (pd.DataFrame): Dataframe
+            date_time (datetime): Datetime of the new row
+            predicted_value (float): Predicted value from previous step
+
+        Returns:
+            pd.DataFrame: Dataframe with the new row
+        """
+        # get the last row values
         last_row_values = df.iloc[-1].values
+        # get values from previous week
         prev_week_values = df.iloc[-24 * 7].values
 
         new_row_df = pd.DataFrame(
             columns=df.columns,
             data=[
                 [
                     predicted_value,  # longtime_mean
@@ -252,172 +228,190 @@
                     np.sin(2 * np.pi * date_time.weekday() / 7),
                     np.cos(2 * np.pi * date_time.weekday() / 7),
                     np.sin(2 * np.pi * date_time.hour / 24),
                     np.cos(2 * np.pi * date_time.hour / 24),
                 ]
             ],
         )
+
+        # concat the new row to the dataframe
         df = pd.concat([df, new_row_df], ignore_index=True)
         df = df.reset_index(drop=True)
 
         return df
 
     def mul_generator(
         self,
-        dataframe,
-        target_names,
-        lookback,
-        delay,
-        min_index,
-        max_index,
-        shuffle=False,
-        batch_size=128,
-        step=6,
+        dataframe: pd.DataFrame,
+        target_names: list,
+        min_index: int,
+        max_index: int,
+        shuffle: Optional[bool] = False,
+        batch_size=None,
     ):
+        """
+        Method to create a generator for the model.
+        Concept of the generator is taken from the time-series-h2o-automl-example repository.
+        https://github.com/SeanPLeary/time-series-h2o-automl-example by Leary, Sean P.
+
+
+        Args:
+            dataframe (pd.DataFrame): Dataframe with the data
+            target_names (list): Names of the target values
+            min_index (int): Min index of the data
+            max_index (int): Max index of the data
+            shuffle (Optional[bool], optional): Choose if shuffle the data. Defaults to False.
+
+        Yields:
+            _type_: The data for the model
+        """
+        
+        if batch_size is None:
+            batch_size = self.batch_size
         data = dataframe.values
         data = data.astype(np.float32)
 
         data_without_targets = dataframe.copy()
         data_without_targets = data_without_targets.drop(columns="longtime_mean")
         data_without_targets = data_without_targets.values
         data_without_targets = data_without_targets.astype(np.float32)
 
         # Get the column indices for the target names
         target_indices = [
             dataframe.columns.get_loc(target_name) for target_name in target_names
         ]
 
         if max_index is None:
-            max_index = len(data) - delay - 1
-        i = min_index + lookback
+            max_index = len(data) - self.delay - 1
+        i = min_index + self.lookback
         while 1:
             if shuffle:
                 rows = np.random.randint(
-                    min_index + lookback, max_index, size=batch_size
+                    min_index + self.lookback, max_index, size=batch_size
                 )
             else:
                 if i + batch_size >= max_index:
-                    i = min_index + lookback
+                    i = min_index + self.lookback
                 rows = np.arange(i, min(i + batch_size, max_index))
                 i += len(rows)
 
             samples = np.zeros(
-                (len(rows), lookback // step, data_without_targets.shape[-1])
+                (len(rows), self.lookback // self.step, data_without_targets.shape[-1])
             )
 
             # Modify targets array to accommodate multiple target columns
             targets = np.zeros((len(rows), len(target_indices)))
 
             for j, row in enumerate(rows):
-                indices = range(rows[j] - lookback, rows[j], step)
+                indices = range(rows[j] - self.lookback, rows[j], self.step)
                 samples[j] = data_without_targets[indices]
 
                 # Assign values for each target column
                 for k, target_indx in enumerate(target_indices):
-                    targets[j][k] = data[rows[j] + delay][target_indx]
+                    targets[j][k] = data[rows[j] + self.delay][target_indx]
 
             yield samples, targets
 
     def get_forecast_next_steps(
-        self, left_time_interval=None, right_time_interval=None
-    ):
-        # Define the indices for the different predictions and truths
+        self,
+        left_time_interval: Optional[datetime] = None,
+        right_time_interval: Optional[datetime] = None,
+    ) -> pd.DataFrame:
+        """Method for getting the forecast of the consumed heat prediction for the next steps for the next 6 hours.
+
+        Args:
+            left_time_interval (Optional[datetime], optional): Left time datetime of interval. Defaults to None.
+            right_time_interval (Optional[datetime], optional): Right time datetime of interval. Defaults to None.
+
+        Returns:
+            pd.DataFrame: Dataframe with consumed heat prediction for next 6 hours.
+        """
         if left_time_interval is None:
             left_time_interval = datetime.now() - timedelta(days=30)
         if right_time_interval is None:
             right_time_interval = datetime.now()
 
+        # get data for creatig a prediction
         df_all, datetimes = self.dataHandler.get_data_for_prediction(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
 
-        num_targets = len(self.predicted_columns)
-        len_columns = len(df_all.columns)
-        forecast_future = pd.DataFrame()
+        number_of_targets = len(self.predicted_columns)
+        number_of_columns = len(df_all.columns)
+        number_of_features = number_of_columns - number_of_targets
 
+        # dataframe with forecast
+        forecast_future = pd.DataFrame()
 
         current_forecast_begin_date = right_time_interval + timedelta(hours=1)
 
+        # add an empty row to the dataframe
         df_all = self.add_empty_row(df_all, current_forecast_begin_date, 0)
         current_forecast_begin_date += timedelta(hours=1)
 
         # prediction for next 6 hours
         for i in range(0, 6):
 
             df_test_norm = df_all.reset_index(drop=True).copy()
 
             # df_test_norm = df_test_zuka.copy()
             df_test_norm[df_test_norm.columns] = self.scaler.transform(df_test_norm)
 
+            # get data for the last lookback * 4 hours
             df_test_norm = df_test_norm[-self.lookback * 4 :]
+            # create a generator for the model
             test_gen = self.mul_generator(
                 dataframe=df_test_norm,
                 target_names=self.predicted_columns,
-                lookback=self.lookback,
-                delay=self.delay,
+                batch_size=self.batch_size,
                 min_index=0,
                 max_index=None,
-                step=1,
                 shuffle=False,
-                batch_size=self.batch_size,
             )
 
             last_batch = next(test_gen)
 
-            # Step 3: Extract the last batch of features (X_batch) and target values (y_truth_batch)
             (X_batch, y_truth) = last_batch
 
-            # Step 4: Make predictions with your model on the last batch
-            num_targets = len(self.predicted_columns)
-            len_columns = len(df_test_norm.columns)
-            num_features = len_columns - num_targets
-
-            y_truth_concat = np.concatenate(
-                (y_truth, np.zeros((y_truth.shape[0], num_features))), axis=1
-            )
-            y_truth_concat = self.scaler.inverse_transform(y_truth_concat)
-
-            y_truth_inv = y_truth_concat[-1, 0]
-
+            # do the prediction of next step
             y_pred = self.model.predict(X_batch, verbose=0)
+
+            # inverse transform the prediction
             y_pred_inv = np.concatenate(
-                (y_pred, np.zeros((y_pred.shape[0], num_features))), axis=1
+                (y_pred, np.zeros((y_pred.shape[0], number_of_features))), axis=1
             )
-
             y_pred_inv = self.scaler.inverse_transform(y_pred_inv)
+
             # get last predicted value
             y_pred_inv = y_pred_inv[-1, 0]
+
             # y_pred_inv[0] is min 0
             if y_pred_inv < 0:
                 y_pred_inv = 0
 
-            if i == 0:
-                print("y_pred_inv: ", y_pred_inv)
-                print("y_truth_inv: ", y_truth_inv)
-
-            # set last longtimemean value
+            # set last longtime_mean value
             df_all.iloc[-1, df_all.columns.get_loc("longtime_mean")] = y_pred_inv
 
+            # add the prediction to the forecast
             forecast_future = pd.concat(
                 [
                     forecast_future,
                     df_all.iloc[[-1], df_all.columns.get_loc("longtime_mean")],
                 ],
                 axis=0,
             )
             forecast_future = forecast_future.reset_index(drop=True)
-            
+
+            # add an empty row to the dataframe
             df_all = self.add_empty_row(df_all, current_forecast_begin_date, 0)
             current_forecast_begin_date += timedelta(hours=1)
 
         # create a dataframe with forecast and datetime as index
-        self.dataHandler.write_forecast_to_influxdb(
-            forecast_future, "prediction_longtime_mean"
-        )
+        self.dataHandler.write_forecast_to_influxdb(forecast_future)
         return forecast_future
 
 
 if __name__ == "__main__":
     dataHandler = DataHandler(
         "localhost",
         "smart_home_formankovi",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smartboiler-0.0.3.0.0.7.4/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.1.2/src/smartboiler.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 src/smartboiler/boiler.py
 src/smartboiler/controller.py
 src/smartboiler/data_handler.py
 src/smartboiler/event_checker.py
 src/smartboiler/forecast.py
 src/smartboiler/fotovoltaics.py
 src/smartboiler/main.py
-src/smartboiler/retrieve_hass.py
 src/smartboiler/switch.py
 src/smartboiler/time_handler.py
-src/smartboiler/week_planner.py
 src/smartboiler.egg-info/PKG-INFO
 src/smartboiler.egg-info/SOURCES.txt
 src/smartboiler.egg-info/dependency_links.txt
 src/smartboiler.egg-info/entry_points.txt
 src/smartboiler.egg-info/requires.txt
 src/smartboiler.egg-info/top_level.txt
```

