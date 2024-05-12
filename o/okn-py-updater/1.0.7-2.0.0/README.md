# Comparing `tmp/okn_py_updater-1.0.7.tar.gz` & `tmp/okn_py_updater-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okn_py_updater-1.0.7.tar", last modified: Mon May  6 22:36:41 2024, max compression
+gzip compressed data, was "okn_py_updater-2.0.0.tar", last modified: Sun May 12 23:24:54 2024, max compression
```

## Comparing `okn_py_updater-1.0.7.tar` & `okn_py_updater-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.233960 okn_py_updater-1.0.7/
--rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3706 2024-05-06 22:36:41.232953 okn_py_updater-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-1.0.7/README.md
--rw-rw-rw-   0        0        0      657 2024-05-06 22:36:30.000000 okn_py_updater-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 22:36:41.233960 okn_py_updater-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.209179 okn_py_updater-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.213701 okn_py_updater-1.0.7/src/okn_py_updater/
--rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-1.0.7/src/okn_py_updater/__init__.py
--rw-rw-rw-   0        0        0    18323 2024-05-06 22:35:43.000000 okn_py_updater-1.0.7/src/okn_py_updater/okn_py_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.231443 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/
--rw-rw-rw-   0        0        0     3706 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 23:24:54.963801 okn_py_updater-2.0.0/
+-rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3706 2024-05-12 23:24:54.962821 okn_py_updater-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.0/README.md
+-rw-rw-rw-   0        0        0      657 2024-05-12 23:24:34.000000 okn_py_updater-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 23:24:54.963801 okn_py_updater-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 23:24:54.932371 okn_py_updater-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 23:24:54.944342 okn_py_updater-2.0.0/src/okn_py_updater/
+-rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.0/src/okn_py_updater/__init__.py
+-rw-rw-rw-   0        0        0    17497 2024-05-12 23:23:21.000000 okn_py_updater-2.0.0/src/okn_py_updater/okn_py_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:24:54.961803 okn_py_updater-2.0.0/src/okn_py_updater.egg-info/
+-rw-rw-rw-   0        0        0     3706 2024-05-12 23:24:54.000000 okn_py_updater-2.0.0/src/okn_py_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-12 23:24:54.000000 okn_py_updater-2.0.0/src/okn_py_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 23:24:54.000000 okn_py_updater-2.0.0/src/okn_py_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-12 23:24:54.000000 okn_py_updater-2.0.0/src/okn_py_updater.egg-info/top_level.txt
```

### Comparing `okn_py_updater-1.0.7/LICENSE` & `okn_py_updater-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `okn_py_updater-1.0.7/PKG-INFO` & `okn_py_updater-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 1.0.7
+Version: 2.0.0
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `okn_py_updater-1.0.7/README.md` & `okn_py_updater-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `okn_py_updater-1.0.7/pyproject.toml` & `okn_py_updater-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "okn_py_updater"
-version = "1.0.7"
+version = "2.0.0"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for OKN Data Updater"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `okn_py_updater-1.0.7/src/okn_py_updater/okn_py_updater.py` & `okn_py_updater-2.0.0/src/okn_py_updater/okn_py_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import collections
 import numpy as np
 import math
-from scipy.signal import medfilt
+# from scipy.signal import medfilt
+import statistics
 
 
 def live_dispatch_function(filter_config_info, data_dict_input):
     match_item = filter_config_info["function"]
     # print(f"Dispatched function name: {match_item}")
     if match_item == 'cdp_direction':
         # t = data_dict_input[filter_config_info["input"]]
@@ -16,124 +17,124 @@
         print(f"{match_item} will be coming soon.")
 
     elif match_item == 'reduce':
         print(f"{match_item} will be coming soon.")
         # print('reduce')
 
     elif match_item == 'dwnsample':
-        # target_data = data_dict_input[filter_config_info["input"]]
-        # target_samplerate = filter_config_info["target_samplerate"]
-        # if len(target_data) > target_samplerate:
-        #     diff_mean = np.nanmean(np.diff(target_data))
-        #     estimated_samplerate = 1 / diff_mean
-        #     approximated_reduction = math.log(math.floor(estimated_samplerate / target_samplerate), 2)
-        # else:
-        #     approximated_reduction = 0
-        #
-        # # print(f"Target samplerate       =  {target_samplerate}")
-        # # print(f"Estimated samplerate    =  {estimated_samplerate}")
-        # # print(f"Approximated reductions =  {approximated_reduction}")
-        #
-        # if approximated_reduction == 0:
-        #     return data_dict_input
-        #
-        # p = dwnsample(data_dict_input, approximated_reduction)
-        # data_dict_input = p
-        # return data_dict_input
+        # Implement as data drop rate in live updater
         pass
 
     elif match_item == 'detectblinkV':
-        x1 = data_dict_input[filter_config_info["input"][0]]
-        x2 = data_dict_input[filter_config_info["input"][1]]
-        x1 = medfilt(x1, 3)
-        x2 = medfilt(x2, 3)
-
-        # print(f"x1: {x1}")
-        # print(f"x2: {x2}")
+        # x1 = data_dict_input[filter_config_info["input"][0]]
+        # x2 = data_dict_input[filter_config_info["input"][1]]
+        # x1 = medfilt(x1, 3)
+        # x2 = medfilt(x2, 3)
+        # Not tested in live updater
+        pass
 
     elif match_item == 'deblinker2':
-        x0 = data_dict_input[filter_config_info["input"][0]]
-        y0 = data_dict_input[filter_config_info["input"][1]]
-        th = filter_config_info["threshold"]
-
-        i = deblinker2(x0, y0, th)
-        data_dict_input[filter_config_info["output"]] = i
+        # x0 = data_dict_input[filter_config_info["input"][0]]
+        # y0 = data_dict_input[filter_config_info["input"][1]]
+        # th = filter_config_info["threshold"]
+        #
+        # i = deblinker2(x0, y0, th)
+        # data_dict_input[filter_config_info["output"]] = i
+        # Not tested in live updater
+        pass
 
     elif match_item == 'passthrough':
         f = data_dict_input[filter_config_info["input"]]
         output_column = filter_config_info["output"]
         data_dict_input[output_column] = f
         # print(f"{output_column} column has been added to output data.")
 
     elif match_item == 'dshift':
-        f = data_dict_input[filter_config_info["input"][0]]
-        data_dict_input[filter_config_info["output"]] = dshift(f)
+        # f = data_dict_input[filter_config_info["input"][0]]
+        # data_dict_input[filter_config_info["output"]] = dshift(f)
+        # Not tested in live updater
+        pass
 
     elif match_item == 'tidy':
-        f = data_dict_input[filter_config_info["input"][0]]
-        n = filter_config_info["value"]
-        thicken = filter_config_info["thicken"]
-
-        is_tracking = data_dict_input[filter_config_info["input"][1]]
-        data_dict_input[filter_config_info["output"]] = tidy(f, n, thicken, np.logical_not(is_tracking))
+        # f = data_dict_input[filter_config_info["input"][0]]
+        # n = filter_config_info["value"]
+        # thicken = filter_config_info["thicken"]
+        #
+        # is_tracking = data_dict_input[filter_config_info["input"][1]]
+        # data_dict_input[filter_config_info["output"]] = tidy(f, n, thicken, np.logical_not(is_tracking))
+        # Not tested in live updater
+        pass
 
     elif match_item == 'wavelet':
-        f = data_dict_input[filter_config_info["input"][0]]
-        if are_all_elements_nan(f):
-            data_dict_input[filter_config_info["output"]] = f
-            return
-
-        level_for_reconstruction = np.array(filter_config_info["levelForReconstruction"])
-        wavelet_type = filter_config_info["type"]
-        level = filter_config_info["Level"]
-        data_dict_input[filter_config_info["output"]] = waveleter(f, level_for_reconstruction, wavelet_type, level)
+        # f = data_dict_input[filter_config_info["input"][0]]
+        # if are_all_elements_nan(f):
+        #     data_dict_input[filter_config_info["output"]] = f
+        #     return
+        #
+        # level_for_reconstruction = np.array(filter_config_info["levelForReconstruction"])
+        # wavelet_type = filter_config_info["type"]
+        # level = filter_config_info["Level"]
+        # data_dict_input[filter_config_info["output"]] = waveleter(f, level_for_reconstruction, wavelet_type, level)
+        # Not tested in live updater
+        pass
 
     elif match_item == 'spikeRemover':
-        print(f"{match_item} will be coming soon.")
+        # Not tested in live updater
+        pass
 
     elif match_item == 'deblinker':
-        print(f"{match_item} will be coming soon.")
+        # Not tested in live updater
+        pass
 
     elif match_item == 'shiftSignal':
-        print(f"{match_item} will be coming soon.")
+        # Not tested in live updater
+        pass
 
     elif match_item == 'medianFilter':
         input_column = filter_config_info["input"][0]
         f = data_dict_input[input_column]
         n = filter_config_info["npoint"]
+        if n <= 1:
+            raise ValueError("Median Filter: kernel value n must be greater than 1.")
+        elif n % 2 == 0:
+            raise ValueError("Median Filter: kernel value n must be odd number.")
         if len(f) >= n:
             last_n_number_array = f[-n:]
-            mean_value = np.nanmean(last_n_number_array)
-            f[-1] = mean_value
+            median_value = statistics.median(last_n_number_array)
+            f[-1] = median_value
             data_dict_input[filter_config_info["output"]] = f
         else:
             data_dict_input[filter_config_info["output"]] = f
 
     elif match_item == 'replaceNanBy':
         input_column = filter_config_info["input"][0]
         input_array = data_dict_input[input_column]
         pointer = filter_config_info["pointer"]
         data_dict_input[filter_config_info["output"]] = replace_nan_by(data_dict_input, input_array, pointer)
 
     elif match_item == 'applymask':
-        print(f"{match_item} will be coming soon.")
+        # Not tested in live updater
+        pass
 
     elif match_item == 'detrender':
-        print(f"{match_item} will be coming soon.")
+        # Not tested in live updater
+        pass
 
     elif match_item == 'detectblinkV':
-        print(f"{match_item} will be coming soon.")
+        # Not tested in live updater
+        pass
 
     elif match_item == 'gradient':
-        related_column_name_array = filter_config_info["input"]
-        f = data_dict_input[related_column_name_array[1]]
-        t = data_dict_input[related_column_name_array[0]]
-        output_column = filter_config_info["output"]
-        data_dict_input[output_column] = grad(f, t)
-        # print(f"{output_column} column is added to the output data by using gradient.")
+        # related_column_name_array = filter_config_info["input"]
+        # f = data_dict_input[related_column_name_array[1]]
+        # t = data_dict_input[related_column_name_array[0]]
+        # output_column = filter_config_info["output"]
+        # data_dict_input[output_column] = grad(f, t)
+        # Not tested in live updater
+        pass
 
     else:
         print(f"Function:{match_item} is not found")
 
     return data_dict_input
 
 
@@ -147,15 +148,14 @@
 
 # def detectblinkV(t, V, fps, varargin):
 #     pass
 
 
 def dwnsample(dict_input, number_of_reduction):
     f = len(dict_input[next(iter(dict_input))])
-    print("********************", f)
     number_of_reduction = int(number_of_reduction)
     if isinstance(number_of_reduction, int):
         loop_count = 0
         while loop_count < number_of_reduction:
             loop_count += 1
             for key in dict_input:
                 temp_array = dict_input[key]
@@ -279,30 +279,14 @@
         return 0
 
 
 def cdp_direction(logs, fname, t):
     return t
 
 
-# def medfilt1(x, k):
-#     # Apply a length-k median filter to a 1D array x.
-#     # Boundaries are extended by repeating endpoints.
-#     assert k % 2 == 1, "Median filter length must be odd."
-#     assert x.ndim == 1, "Input must be one-dimensional."
-#     k2 = (k - 1) // 2
-#     data_dict_input = np.zeros((len(x), k), dtype=x.dtype)
-#     data_dict_input[:, k2] = x
-#     for i in range(k2):
-#         j = k2 - i
-#         data_dict_input[j:, i] = x[:-j]
-#         data_dict_input[:j, i] = x[0]
-#         data_dict_input[:-j, -(i + 1)] = x[j:]
-#         data_dict_input[-j:, -(i + 1)] = x[-1]
-#     return np.median(data_dict_input, axis=1)
-
 def are_all_elements_nan(input_array):
     for ele in input_array:
         if not np.isnan(ele):
             return False
     return True
 
 
@@ -353,48 +337,52 @@
         self.config = config
         self.filter_config = filter_config
         self.circular_buffer = collections.deque(maxlen=circular_buffer_length)
         self.buffer_max_length = circular_buffer_length
         self.header_array = header_array
         self.out_header_array = get_out_header_array(header_array, filter_config)
         self.data_drop_rate = drop_rate
+        self.currently_working_function = ['passthrough', 'medianFilter', 'replaceNanBy']
+        for filter_info in self.filter_config:
+            if filter_info["Enabled"]:
+                function_name = filter_info["function"]
+                if function_name not in self.currently_working_function:
+                    if function_name == 'dwnsample':
+                        print(f"The function \"dwnsample\" is implemented as drop rate in live updater.")
+                    else:
+                        print(f"The function \"{function_name}\" is not available in live updater.")
+            else:
+                pass
         self.count = 0
 
     def update(self, data_input):
         if self.data_drop_rate == 0:
             self.circular_buffer.append(data_input)
             data_dict = {}
-            output_header_array = [header for header in self.header_array]
             output_data = []
-            for filter_info in self.filter_config:
-                if filter_info["Enabled"]:
-                    try:
-                        output_header = filter_info["output"]
-                    except KeyError:
-                        output_header = None
-                    if output_header and output_header not in output_header_array:
-                        output_header_array.append(output_header)
             for header in self.header_array:
                 data_dict[header] = []
             for data in self.circular_buffer:
                 for header_index, header_string in enumerate(self.header_array):
                     data_dict[header_string].append(float(data[header_index]))
 
             # if len(self.circular_buffer) >= 3:
             for filter_info in self.filter_config:
                 if filter_info["Enabled"]:
                     data_dict = live_dispatch_function(filter_info, data_dict)
                 else:
                     pass
 
-            for index in range(len(data_dict[output_header_array[0]])):
+            for index in range(len(data_dict[self.out_header_array[0]])):
                 temp_array = []
-                for header in output_header_array:
+                for header in self.out_header_array:
                     try:
                         temp_array.append(data_dict[header][index])
+                    except KeyError:
+                        temp_array.append(0)
                     except TypeError:
                         temp_array.append(0)
                 output_data.append(temp_array)
                 # len_diff = len(output_header_array) - len(self.header_array)
                 # for data in self.circular_buffer:
                 #     temp_array = [ele for ele in data]
                 #     temp_array.extend(len_diff * [0])
@@ -405,34 +393,35 @@
             #     print(d)
             # print("end")
             return output_data[-1]
         else:
             if self.count == 0:
                 self.circular_buffer.append(data_input)
                 data_dict = {}
-                output_header_array = self.out_header_array
                 output_data = []
                 for header in self.header_array:
                     data_dict[header] = []
                 for data in self.circular_buffer:
                     for header_index, header_string in enumerate(self.header_array):
                         data_dict[header_string].append(float(data[header_index]))
 
                 # if len(self.circular_buffer) >= 3:
                 for filter_info in self.filter_config:
                     if filter_info["Enabled"]:
                         data_dict = live_dispatch_function(filter_info, data_dict)
                     else:
                         pass
 
-                for index in range(len(data_dict[output_header_array[0]])):
+                for index in range(len(data_dict[self.out_header_array[0]])):
                     temp_array = []
-                    for header in output_header_array:
+                    for header in self.out_header_array:
                         try:
                             temp_array.append(data_dict[header][index])
+                        except KeyError:
+                            temp_array.append(0)
                         except TypeError:
                             temp_array.append(0)
                     output_data.append(temp_array)
                     # len_diff = len(output_header_array) - len(self.header_array)
                     # for data in self.circular_buffer:
                     #     temp_array = [ele for ele in data]
                     #     temp_array.extend(len_diff * [0])
```

### Comparing `okn_py_updater-1.0.7/src/okn_py_updater.egg-info/PKG-INFO` & `okn_py_updater-2.0.0/src/okn_py_updater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 1.0.7
+Version: 2.0.0
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

