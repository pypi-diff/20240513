# Comparing `tmp/business_duration-0.66.tar.gz` & `tmp/business_duration-0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\business_duration-0.66.tar", last modified: Wed Jan 19 17:24:14 2022, max compression
+gzip compressed data, was "business_duration-0.67.tar", last modified: Mon May 13 16:10:19 2024, max compression
```

## Comparing `business_duration-0.66.tar` & `business_duration-0.67.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-01-19 17:24:14.006115 business_duration-0.66/
--rw-rw-rw-   0        0        0     4410 2022-01-19 17:24:14.006115 business_duration-0.66/PKG-INFO
--rw-rw-rw-   0        0        0     3096 2022-01-19 17:18:14.000000 business_duration-0.66/README.rst
-drwxrwxrwx   0        0        0        0 2022-01-19 17:24:14.006115 business_duration-0.66/business_duration/
--rw-rw-rw-   0        0        0    12543 2022-01-19 17:15:23.000000 business_duration-0.66/business_duration/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-19 17:24:14.006115 business_duration-0.66/business_duration.egg-info/
--rw-rw-rw-   0        0        0     4410 2022-01-19 17:24:13.000000 business_duration-0.66/business_duration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2022-01-19 17:24:13.000000 business_duration-0.66/business_duration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-19 17:24:13.000000 business_duration-0.66/business_duration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-04-11 19:44:44.000000 business_duration-0.66/business_duration.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2022-01-19 17:24:13.000000 business_duration-0.66/business_duration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-01-19 17:24:14.006115 business_duration-0.66/setup.cfg
--rw-rw-rw-   0        0        0      578 2022-01-19 17:16:37.000000 business_duration-0.66/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:10:19.134436 business_duration-0.67/
+-rw-rw-rw-   0        0        0     3631 2024-05-13 16:10:19.132438 business_duration-0.67/PKG-INFO
+-rw-rw-rw-   0        0        0     3096 2022-01-19 17:18:14.000000 business_duration-0.67/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-13 16:10:19.094206 business_duration-0.67/business_duration/
+-rw-rw-rw-   0        0        0    12543 2022-01-19 17:15:23.000000 business_duration-0.67/business_duration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:10:19.128420 business_duration-0.67/business_duration.egg-info/
+-rw-rw-rw-   0        0        0     3631 2024-05-13 16:10:18.000000 business_duration-0.67/business_duration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-13 16:10:19.000000 business_duration-0.67/business_duration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:10:18.000000 business_duration-0.67/business_duration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2018-04-11 19:44:44.000000 business_duration-0.67/business_duration.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2024-05-13 16:10:18.000000 business_duration-0.67/business_duration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 16:10:18.000000 business_duration-0.67/business_duration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-13 16:10:19.138422 business_duration-0.67/setup.cfg
+-rw-rw-rw-   0        0        0      621 2024-05-13 16:01:46.000000 business_duration-0.67/setup.py
```

### Comparing `business_duration-0.66/PKG-INFO` & `business_duration-0.67/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,111 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: business_duration
-Version: 0.66
+Version: 0.67
 Summary: Calculates business duration in days, hours, minutes and seconds by excluding weekends, public holidays and non-business hours
 Home-page: https://github.com/gnaneshwar441/Business_Duration
 Author: Gnaneshwar G
 Author-email: gnaneshwar441@gmail.com
 License: MIT
-Description: Business\_Duration
-        ==================
-        
-        Calculates business duration in days, hours, minutes and seconds by
-        excluding weekends, public holidays and non-business hours
-        
-        How to install the package
-        ==========================
-        
-        pip install business-duration
-        
-        Example 1
-        =========
-        
-        .. code:: python
-        
-            from business_duration import businessDuration
-            import pandas as pd
-            import holidays as pyholidays
-            from datetime import time
-        
-            #Start date must be in standard python datetime format
-            start_date = pd.to_datetime('2017-07-01 02:02:00')
-        
-            #Start date must be in standard python datetime format
-            end_date = pd.to_datetime('2017-07-07 04:48:00')
-        
-            #Business open hour must be in standard python time format-Hour,Min,Sec
-            biz_open_time=time(7,0,0)
-        
-            #Business close hour must be in standard python time format-Hour,Min,Sec
-            biz_close_time=time(17,0,0)
-        
-            #US public holidays
-            US_holiday_list = pyholidays.US(state='CA')
-        
-            #Business duration can be 'day', 'hour', 'min', 'sec'
-            unit_hour='hour'
-        
-            #Printing output
-            print(businessDuration(startdate=start_date,enddate=end_date,starttime=biz_open_time,endtime=biz_close_time,holidaylist=US_holiday_list,unit=unit_hour))
-        
-            #Result
-            #30.0
-        
-            #Result is 30 hours because July 1st, 2nd are weekends and 4th is US public holiday. So 3 days remains with 10 business hours per day. 3 days*10 hours = 30 Hours
-        
-        Example 2
-        =========
-        
-        .. code:: python
-        
-            from business_duration import businessDuration
-            from datetime import datetime
-        
-            start_date = datetime.strptime("2018-01-01","%Y-%m-%d").date()
-            end_date = datetime.strptime("2018-03-31","%Y-%m-%d").date()
-        
-            print(businessDuration(startdate=start_date,enddate=end_date,unit='day'))
-        
-            #Result
-            65.0
-        
-        Example 3
-        =========
-        
-        .. code:: python
-        
-            from business_duration import businessDuration
-            import pandas as pd
-            import holidays as pyholidays
-            from datetime import time,datetime
-        
-            #Reading input file
-            inputdata = pd.read_excel('Sample.xls')
-        
-            #Converting to standard Python datetime format
-            inputdata.sys_created_on=pd.to_datetime(inputdata.sys_created_on,format='%Y-%m-%d %H:%M:%S')
-            inputdata.resolved_at=pd.to_datetime(inputdata.resolved_at,format='%Y-%m-%d %H:%M:%S')
-        
-            #Business open hour
-            biz_open_time = time(8,0,0)
-        
-            #Business close time
-            biz_close_time = time(17,0,0)
-        
-            #Weekend list. 5-Sat, 6-Sun
-            weekend_list = [5,6]
-        
-            #Custom US holidays
-            US_holiday_list = {datetime(2018,1,1).date():"New Year's Day",datetime(2018,5,28).date():"Memorial Day",datetime(2018,7,4).date():"Independence Day",datetime(2018,9,3).date():"Labor Day",datetime(2018,11,22).date():"Thanksgiving",datetime(2018,12,25).date():"Christmas Day"}
-        
-            #Business duration 'day','hour','min','sec'
-            unit_hour='hour'
-        
-            #Applying the function to entire dataframe
-            from itertools import repeat
-            inputdata['Biz_Hour'] = list(map(businessDuration,inputdata.sys_created_on,inputdata.resolved_at,repeat(biz_open_time),repeat(biz_close_time),repeat(weekend_list),repeat(US_holiday_list),repeat(unit_hour)))
-        
-        
 Keywords: business,duration,time,hour,day,working
-Platform: UNKNOWN
+Requires-Dist: numpy
+Requires-Dist: pandas
+
+Business\_Duration
+==================
+
+Calculates business duration in days, hours, minutes and seconds by
+excluding weekends, public holidays and non-business hours
+
+How to install the package
+==========================
+
+pip install business-duration
+
+Example 1
+=========
+
+.. code:: python
+
+    from business_duration import businessDuration
+    import pandas as pd
+    import holidays as pyholidays
+    from datetime import time
+
+    #Start date must be in standard python datetime format
+    start_date = pd.to_datetime('2017-07-01 02:02:00')
+
+    #Start date must be in standard python datetime format
+    end_date = pd.to_datetime('2017-07-07 04:48:00')
+
+    #Business open hour must be in standard python time format-Hour,Min,Sec
+    biz_open_time=time(7,0,0)
+
+    #Business close hour must be in standard python time format-Hour,Min,Sec
+    biz_close_time=time(17,0,0)
+
+    #US public holidays
+    US_holiday_list = pyholidays.US(state='CA')
+
+    #Business duration can be 'day', 'hour', 'min', 'sec'
+    unit_hour='hour'
+
+    #Printing output
+    print(businessDuration(startdate=start_date,enddate=end_date,starttime=biz_open_time,endtime=biz_close_time,holidaylist=US_holiday_list,unit=unit_hour))
+
+    #Result
+    #30.0
+
+    #Result is 30 hours because July 1st, 2nd are weekends and 4th is US public holiday. So 3 days remains with 10 business hours per day. 3 days*10 hours = 30 Hours
+
+Example 2
+=========
+
+.. code:: python
+
+    from business_duration import businessDuration
+    from datetime import datetime
+
+    start_date = datetime.strptime("2018-01-01","%Y-%m-%d").date()
+    end_date = datetime.strptime("2018-03-31","%Y-%m-%d").date()
+
+    print(businessDuration(startdate=start_date,enddate=end_date,unit='day'))
+
+    #Result
+    65.0
+
+Example 3
+=========
+
+.. code:: python
+
+    from business_duration import businessDuration
+    import pandas as pd
+    import holidays as pyholidays
+    from datetime import time,datetime
+
+    #Reading input file
+    inputdata = pd.read_excel('Sample.xls')
+
+    #Converting to standard Python datetime format
+    inputdata.sys_created_on=pd.to_datetime(inputdata.sys_created_on,format='%Y-%m-%d %H:%M:%S')
+    inputdata.resolved_at=pd.to_datetime(inputdata.resolved_at,format='%Y-%m-%d %H:%M:%S')
+
+    #Business open hour
+    biz_open_time = time(8,0,0)
+
+    #Business close time
+    biz_close_time = time(17,0,0)
+
+    #Weekend list. 5-Sat, 6-Sun
+    weekend_list = [5,6]
+
+    #Custom US holidays
+    US_holiday_list = {datetime(2018,1,1).date():"New Year's Day",datetime(2018,5,28).date():"Memorial Day",datetime(2018,7,4).date():"Independence Day",datetime(2018,9,3).date():"Labor Day",datetime(2018,11,22).date():"Thanksgiving",datetime(2018,12,25).date():"Christmas Day"}
+
+    #Business duration 'day','hour','min','sec'
+    unit_hour='hour'
+
+    #Applying the function to entire dataframe
+    from itertools import repeat
+    inputdata['Biz_Hour'] = list(map(businessDuration,inputdata.sys_created_on,inputdata.resolved_at,repeat(biz_open_time),repeat(biz_close_time),repeat(weekend_list),repeat(US_holiday_list),repeat(unit_hour)))
+
```

### Comparing `business_duration-0.66/README.rst` & `business_duration-0.67/README.rst`

 * *Files identical despite different names*

### Comparing `business_duration-0.66/business_duration/__init__.py` & `business_duration-0.67/business_duration/__init__.py`

 * *Files identical despite different names*

### Comparing `business_duration-0.66/business_duration.egg-info/PKG-INFO` & `business_duration-0.67/business_duration.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,111 @@
-Metadata-Version: 1.0
-Name: business-duration
-Version: 0.66
+Metadata-Version: 2.1
+Name: business_duration
+Version: 0.67
 Summary: Calculates business duration in days, hours, minutes and seconds by excluding weekends, public holidays and non-business hours
 Home-page: https://github.com/gnaneshwar441/Business_Duration
 Author: Gnaneshwar G
 Author-email: gnaneshwar441@gmail.com
 License: MIT
-Description: Business\_Duration
-        ==================
-        
-        Calculates business duration in days, hours, minutes and seconds by
-        excluding weekends, public holidays and non-business hours
-        
-        How to install the package
-        ==========================
-        
-        pip install business-duration
-        
-        Example 1
-        =========
-        
-        .. code:: python
-        
-            from business_duration import businessDuration
-            import pandas as pd
-            import holidays as pyholidays
-            from datetime import time
-        
-            #Start date must be in standard python datetime format
-            start_date = pd.to_datetime('2017-07-01 02:02:00')
-        
-            #Start date must be in standard python datetime format
-            end_date = pd.to_datetime('2017-07-07 04:48:00')
-        
-            #Business open hour must be in standard python time format-Hour,Min,Sec
-            biz_open_time=time(7,0,0)
-        
-            #Business close hour must be in standard python time format-Hour,Min,Sec
-            biz_close_time=time(17,0,0)
-        
-            #US public holidays
-            US_holiday_list = pyholidays.US(state='CA')
-        
-            #Business duration can be 'day', 'hour', 'min', 'sec'
-            unit_hour='hour'
-        
-            #Printing output
-            print(businessDuration(startdate=start_date,enddate=end_date,starttime=biz_open_time,endtime=biz_close_time,holidaylist=US_holiday_list,unit=unit_hour))
-        
-            #Result
-            #30.0
-        
-            #Result is 30 hours because July 1st, 2nd are weekends and 4th is US public holiday. So 3 days remains with 10 business hours per day. 3 days*10 hours = 30 Hours
-        
-        Example 2
-        =========
-        
-        .. code:: python
-        
-            from business_duration import businessDuration
-            from datetime import datetime
-        
-            start_date = datetime.strptime("2018-01-01","%Y-%m-%d").date()
-            end_date = datetime.strptime("2018-03-31","%Y-%m-%d").date()
-        
-            print(businessDuration(startdate=start_date,enddate=end_date,unit='day'))
-        
-            #Result
-            65.0
-        
-        Example 3
-        =========
-        
-        .. code:: python
-        
-            from business_duration import businessDuration
-            import pandas as pd
-            import holidays as pyholidays
-            from datetime import time,datetime
-        
-            #Reading input file
-            inputdata = pd.read_excel('Sample.xls')
-        
-            #Converting to standard Python datetime format
-            inputdata.sys_created_on=pd.to_datetime(inputdata.sys_created_on,format='%Y-%m-%d %H:%M:%S')
-            inputdata.resolved_at=pd.to_datetime(inputdata.resolved_at,format='%Y-%m-%d %H:%M:%S')
-        
-            #Business open hour
-            biz_open_time = time(8,0,0)
-        
-            #Business close time
-            biz_close_time = time(17,0,0)
-        
-            #Weekend list. 5-Sat, 6-Sun
-            weekend_list = [5,6]
-        
-            #Custom US holidays
-            US_holiday_list = {datetime(2018,1,1).date():"New Year's Day",datetime(2018,5,28).date():"Memorial Day",datetime(2018,7,4).date():"Independence Day",datetime(2018,9,3).date():"Labor Day",datetime(2018,11,22).date():"Thanksgiving",datetime(2018,12,25).date():"Christmas Day"}
-        
-            #Business duration 'day','hour','min','sec'
-            unit_hour='hour'
-        
-            #Applying the function to entire dataframe
-            from itertools import repeat
-            inputdata['Biz_Hour'] = list(map(businessDuration,inputdata.sys_created_on,inputdata.resolved_at,repeat(biz_open_time),repeat(biz_close_time),repeat(weekend_list),repeat(US_holiday_list),repeat(unit_hour)))
-        
-        
 Keywords: business,duration,time,hour,day,working
-Platform: UNKNOWN
+Requires-Dist: numpy
+Requires-Dist: pandas
+
+Business\_Duration
+==================
+
+Calculates business duration in days, hours, minutes and seconds by
+excluding weekends, public holidays and non-business hours
+
+How to install the package
+==========================
+
+pip install business-duration
+
+Example 1
+=========
+
+.. code:: python
+
+    from business_duration import businessDuration
+    import pandas as pd
+    import holidays as pyholidays
+    from datetime import time
+
+    #Start date must be in standard python datetime format
+    start_date = pd.to_datetime('2017-07-01 02:02:00')
+
+    #Start date must be in standard python datetime format
+    end_date = pd.to_datetime('2017-07-07 04:48:00')
+
+    #Business open hour must be in standard python time format-Hour,Min,Sec
+    biz_open_time=time(7,0,0)
+
+    #Business close hour must be in standard python time format-Hour,Min,Sec
+    biz_close_time=time(17,0,0)
+
+    #US public holidays
+    US_holiday_list = pyholidays.US(state='CA')
+
+    #Business duration can be 'day', 'hour', 'min', 'sec'
+    unit_hour='hour'
+
+    #Printing output
+    print(businessDuration(startdate=start_date,enddate=end_date,starttime=biz_open_time,endtime=biz_close_time,holidaylist=US_holiday_list,unit=unit_hour))
+
+    #Result
+    #30.0
+
+    #Result is 30 hours because July 1st, 2nd are weekends and 4th is US public holiday. So 3 days remains with 10 business hours per day. 3 days*10 hours = 30 Hours
+
+Example 2
+=========
+
+.. code:: python
+
+    from business_duration import businessDuration
+    from datetime import datetime
+
+    start_date = datetime.strptime("2018-01-01","%Y-%m-%d").date()
+    end_date = datetime.strptime("2018-03-31","%Y-%m-%d").date()
+
+    print(businessDuration(startdate=start_date,enddate=end_date,unit='day'))
+
+    #Result
+    65.0
+
+Example 3
+=========
+
+.. code:: python
+
+    from business_duration import businessDuration
+    import pandas as pd
+    import holidays as pyholidays
+    from datetime import time,datetime
+
+    #Reading input file
+    inputdata = pd.read_excel('Sample.xls')
+
+    #Converting to standard Python datetime format
+    inputdata.sys_created_on=pd.to_datetime(inputdata.sys_created_on,format='%Y-%m-%d %H:%M:%S')
+    inputdata.resolved_at=pd.to_datetime(inputdata.resolved_at,format='%Y-%m-%d %H:%M:%S')
+
+    #Business open hour
+    biz_open_time = time(8,0,0)
+
+    #Business close time
+    biz_close_time = time(17,0,0)
+
+    #Weekend list. 5-Sat, 6-Sun
+    weekend_list = [5,6]
+
+    #Custom US holidays
+    US_holiday_list = {datetime(2018,1,1).date():"New Year's Day",datetime(2018,5,28).date():"Memorial Day",datetime(2018,7,4).date():"Independence Day",datetime(2018,9,3).date():"Labor Day",datetime(2018,11,22).date():"Thanksgiving",datetime(2018,12,25).date():"Christmas Day"}
+
+    #Business duration 'day','hour','min','sec'
+    unit_hour='hour'
+
+    #Applying the function to entire dataframe
+    from itertools import repeat
+    inputdata['Biz_Hour'] = list(map(businessDuration,inputdata.sys_created_on,inputdata.resolved_at,repeat(biz_open_time),repeat(biz_close_time),repeat(weekend_list),repeat(US_holiday_list),repeat(unit_hour)))
+
```

### Comparing `business_duration-0.66/setup.py` & `business_duration-0.67/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup
 
 with open('README.rst') as f:
     readme = f.read()
 	
 setup(name='business_duration',
-	version='0.66',
+	version='0.67',
 	description='Calculates business duration in days, hours, minutes and seconds by excluding weekends, public holidays and non-business hours',
 	long_description=readme,
 	url='https://github.com/gnaneshwar441/Business_Duration',
 	author='Gnaneshwar G',
 	author_email='gnaneshwar441@gmail.com',
 	license='MIT',
 	packages=['business_duration'],
 	keywords = ['business', 'duration', 'time', 'hour', 'day', 'working'],
+    install_requires=['numpy', 'pandas'],
 	zip_safe=False)
```

