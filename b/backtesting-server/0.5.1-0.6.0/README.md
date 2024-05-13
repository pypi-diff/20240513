# Comparing `tmp/backtesting_server-0.5.1.tar.gz` & `tmp/backtesting_server-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtesting_server-0.5.1.tar", max compression
+gzip compressed data, was "backtesting_server-0.6.0.tar", max compression
```

## Comparing `backtesting_server-0.5.1.tar` & `backtesting_server-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.5.1/LICENSE
--rw-r--r--   0        0        0      628 2024-05-08 20:54:54.193183 backtesting_server-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.5.1/README.md
--rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.5.1/src/backtesting_server/__init__.py
--rw-r--r--   0        0        0    27243 2024-05-08 20:54:36.406102 backtesting_server-0.5.1/src/backtesting_server/main.py
--rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.6.0/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-12 13:36:16.558091 backtesting_server-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.6.0/README.md
+-rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.6.0/src/backtesting_server/__init__.py
+-rw-r--r--   0        0        0    29714 2024-05-12 13:36:02.145416 backtesting_server-0.6.0/src/backtesting_server/main.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.6.0/PKG-INFO
```

### Comparing `backtesting_server-0.5.1/LICENSE` & `backtesting_server-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.5.1/pyproject.toml` & `backtesting_server-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backtesting-server"
-version = "0.5.1"
+version = "0.6.0"
 description = "Package to interact with MySQL server, recording results of the backtesting."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `backtesting_server-0.5.1/README.md` & `backtesting_server-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.5.1/src/backtesting_server/main.py` & `backtesting_server-0.6.0/src/backtesting_server/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -518,25 +518,27 @@
           df.set_index("Datetime",inplace=True)
           # Updating previous timestamp.
           previous_timestamps[instrument.epic] = instrument.ticker.timestamp
 
           # Uploading data.
           self.upload_instrument(instrument,dataset=df)
 
-  def get_historical_data(self, instrument: ig_package.Instrument, start_datetime: str = None, end_datetime: str = None) -> pd.DataFrame:
+  def get_historical_data(self, instrument: ig_package.Instrument, resolution: str = None, start_datetime: str = None, end_datetime: str = None) -> pd.DataFrame:
     """ Getting historical data stored on the Backtesting Server.
       
       Parameters
       ----------
       instrument: ig_package.Instrument
         Instrument to get historical data for.
+      resolution: str
+        OPTIONAL Resolution of historical data candlesticks e.g. SECOND, MINUTE, MINUTE_15, HOUR, HOUR_4 and DAY.
       start_datetime: str
-        Start datetime of data e.g. yyyy-mm-dd HH:MM:SS.
+        OPTIONAL Start datetime of data e.g. yyyy-mm-dd HH:MM:SS.
       end_datetime: str
-        End datetime of data e.g. yyyy-mm-dd HH:MM:SS.
+        OPTIONAL End datetime of data e.g. yyyy-mm-dd HH:MM:SS.
       
       Returns
       -------
       pd.DataFrame
         DataFrame containing historical data, e.g columns = ['Datetime', 'Open', 'High', 'Low', 'Close']"""
     # Getting start datetime object.
     if start_datetime:
@@ -553,14 +555,17 @@
     new_name = instrument.name.replace(" ","_")
     self.cursor.execute("SELECT * FROM {}_HistoricalDataset WHERE DatetimeIndex > '{}' AND DatetimeIndex < '{}';".format(new_name,str(start_datetime_obj),str(end_datetime_obj)))
     results = self.cursor.fetchall()
     
     # Creating dataframe.
     df = pd.DataFrame(results, columns=['Datetime', 'Open', 'High', 'Low', 'Close'])
     df.set_index("Datetime",inplace=True)
+    if resolution:
+      # Filtering data.
+      df = self._filter_candles(df,resolution)
     return df
 
   def get_uploaded_instruments(self, ig: ig_package.IG) -> list[ig_package.Instrument] | None:
     """ Getting all instruments uploaded to the Backtesting Server.
       
       Parameters
       ----------
@@ -580,14 +585,74 @@
       for epic in results:
         instruments.append(ig_package.Instrument(epic[0],ig))
       return instruments
     except:
       logger.info("Could not get uploaded instruments from the server.")
       return None
 
+  def _filter_candles(self, dataframe: pd.DataFrame, resolution: str) -> pd.DataFrame:
+    """ Filter candlesticks for a specific resolution.
+    
+      Parameters
+      ----------
+      dataframe: pd.DataFrame
+        Historical data in dataframe.
+      resolution: str
+        Resolution e.g. SECOND, MINUTE, MINUTE_15, HOUR, HOUR_4 and DAY.
+        
+      Returns
+      -------
+      pd.DataFrame
+        Dataframe of candles with Open, High, Low and Close."""
+    # Resolutions.
+    resolution_dict = {
+      "SECOND":1,
+      "MINUTE":60,
+      "MINUTE_15":15*60,
+      "HOUR":60*60,
+      "HOUR_4":4*60*60,
+      "DAY":24*60*60
+    }
+    results = []
+    resolution_factor = resolution_dict[resolution]
+    # Getting starting time.
+    open_datetime = dataframe.index[0].to_pydatetime()
+    open_epoch = (open_datetime.timestamp() // resolution_factor) * resolution_factor
+    previous_epoch = 0
+    # Filtering data.
+    for index, row in dataframe.iterrows():
+      # Getting row datetime.
+      current_datetime = row.name.to_pydatetime()
+      current_epoch = current_datetime.timestamp()
+
+      if ((current_epoch) // resolution_factor) * resolution_factor > ((previous_epoch) // resolution_factor) * resolution_factor:
+        # Setting previous candle.
+        if previous_epoch != 0:
+          single_candle = (datetime.fromtimestamp(((previous_epoch) // resolution_factor) * resolution_factor),open_value,high_value,low_value,close_value)
+          results.append(single_candle)
+        # Setting open values.
+        open_value = row["Open"]
+        low_value = row["Open"]
+        high_value = row["Open"]
+      else:
+        # Checking low and high.
+        if row["Open"] < low_value:
+          low_value = row["Open"]
+        elif row["Open"] > high_value:
+          high_value = row["Open"]
+        # Setting close value and previous epoch.
+        close_value = row["Open"]
+      # Setting previous epoch.
+      previous_epoch = current_epoch
+    
+    # Creating dataframe.
+    df = pd.DataFrame(results, columns=['Datetime', 'Open', 'High', 'Low', 'Close'])
+    df.set_index("Datetime",inplace=True)
+    return df
+
 # - - - - - - - - - - - - - -
 
 class InstrumentGroup():
   """ Class for representing a group of instruments on the Backtesting Server. These instruments can have entire actions performed on them, allowing for easy management of specific instruments."""
 
   def __init__(self, name:str, cursor:pymysql.cursors.Cursor) -> None:
     self.name: str = name
```

### Comparing `backtesting_server-0.5.1/PKG-INFO` & `backtesting_server-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtesting-server
-Version: 0.5.1
+Version: 0.6.0
 Summary: Package to interact with MySQL server, recording results of the backtesting.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

