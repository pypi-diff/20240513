# Comparing `tmp/icad_tone_detection-0.8.tar.gz` & `tmp/icad_tone_detection-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icad_tone_detection-0.8.tar", last modified: Tue Apr 16 05:21:29 2024, max compression
+gzip compressed data, was "icad_tone_detection-0.9.tar", last modified: Mon May 13 05:53:44 2024, max compression
```

## Comparing `icad_tone_detection-0.8.tar` & `icad_tone_detection-0.9.tar`

### file list

```diff
@@ -1,25 +1,20 @@
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/.github/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/.github/workflows/
--rw-rw-r--   0 ian       (2000) ian       (2000)     1301 2024-03-18 00:28:15.000000 icad_tone_detection-0.8/.github/workflows/python-package.yml
--rw-rw-r--   0 ian       (2000) ian       (2000)     3084 2024-03-14 21:16:01.000000 icad_tone_detection-0.8/.gitignore
--rw-rw-r--   0 ian       (2000) ian       (2000)      555 2024-03-17 23:53:26.000000 icad_tone_detection-0.8/LICENSE
--rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/PKG-INFO
--rw-rw-r--   0 ian       (2000) ian       (2000)      457 2024-03-18 00:11:11.000000 icad_tone_detection-0.8/README.md
--rw-rw-r--   0 ian       (2000) ian       (2000)      627 2024-04-16 04:52:45.000000 icad_tone_detection-0.8/detect_test.py
--rw-rw-r--   0 ian       (2000) ian       (2000)      779 2024-04-16 04:42:10.000000 icad_tone_detection-0.8/pyproject.toml
--rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/setup.cfg
--rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-03-18 00:11:11.000000 icad_tone_detection-0.8/setup.py
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/src/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/src/icad_tone_detection/
--rw-rw-r--   0 ian       (2000) ian       (2000)       57 2024-03-14 20:41:31.000000 icad_tone_detection-0.8/src/icad_tone_detection/__init__.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     2599 2024-03-18 01:16:38.000000 icad_tone_detection-0.8/src/icad_tone_detection/audio_loader.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     5855 2024-03-12 18:45:10.000000 icad_tone_detection-0.8/src/icad_tone_detection/frequency_extraction.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     2977 2024-04-16 05:12:10.000000 icad_tone_detection-0.8/src/icad_tone_detection/main.py
--rw-rw-r--   0 ian       (2000) ian       (2000)    13039 2024-04-16 05:05:49.000000 icad_tone_detection-0.8/src/icad_tone_detection/tone_detection.py
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/
--rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/PKG-INFO
--rw-rw-r--   0 ian       (2000) ian       (2000)      536 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)        1 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)       59 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/requires.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)       20 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/top_level.txt
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-05-13 05:53:44.222995 icad_tone_detection-0.9/
+-rw-rw-r--   0 ian       (2000) ian       (2000)      555 2024-05-13 05:04:31.000000 icad_tone_detection-0.9/LICENSE
+-rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-05-13 05:53:44.222995 icad_tone_detection-0.9/PKG-INFO
+-rw-rw-r--   0 ian       (2000) ian       (2000)      457 2024-05-13 05:04:31.000000 icad_tone_detection-0.9/README.md
+-rw-rw-r--   0 ian       (2000) ian       (2000)      779 2024-05-13 05:05:45.000000 icad_tone_detection-0.9/pyproject.toml
+-rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-05-13 05:53:44.222995 icad_tone_detection-0.9/setup.cfg
+-rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-05-13 05:04:31.000000 icad_tone_detection-0.9/setup.py
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-05-13 05:53:44.222995 icad_tone_detection-0.9/src/
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-05-13 05:53:44.222995 icad_tone_detection-0.9/src/icad_tone_detection/
+-rw-rw-r--   0 ian       (2000) ian       (2000)       57 2024-05-13 05:04:31.000000 icad_tone_detection-0.9/src/icad_tone_detection/__init__.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     2599 2024-05-13 05:04:31.000000 icad_tone_detection-0.9/src/icad_tone_detection/audio_loader.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     6330 2024-05-13 05:33:18.000000 icad_tone_detection-0.9/src/icad_tone_detection/frequency_extraction.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     2977 2024-05-13 05:04:31.000000 icad_tone_detection-0.9/src/icad_tone_detection/main.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     6397 2024-05-13 05:50:00.000000 icad_tone_detection-0.9/src/icad_tone_detection/tone_detection.py
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-05-13 05:53:44.222995 icad_tone_detection-0.9/src/icad_tone_detection.egg-info/
+-rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-05-13 05:53:44.000000 icad_tone_detection-0.9/src/icad_tone_detection.egg-info/PKG-INFO
+-rw-rw-r--   0 ian       (2000) ian       (2000)      473 2024-05-13 05:53:44.000000 icad_tone_detection-0.9/src/icad_tone_detection.egg-info/SOURCES.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)        1 2024-05-13 05:53:44.000000 icad_tone_detection-0.9/src/icad_tone_detection.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)       59 2024-05-13 05:53:44.000000 icad_tone_detection-0.9/src/icad_tone_detection.egg-info/requires.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)       20 2024-05-13 05:53:44.000000 icad_tone_detection-0.9/src/icad_tone_detection.egg-info/top_level.txt
```

### Comparing `icad_tone_detection-0.8/LICENSE` & `icad_tone_detection-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.8/PKG-INFO` & `icad_tone_detection-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 0.8
+Version: 0.9
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-0.8/pyproject.toml` & `icad_tone_detection-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icad_tone_detection"
-version = "0.8"
+version = "0.9"
 authors = [
   {name = "TheGreatCodeholio", email = "ian@icarey.net"},
 ]
 description = "A Python library for extracting scanner radio tones from scanner audio."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `icad_tone_detection-0.8/src/icad_tone_detection/audio_loader.py` & `icad_tone_detection-0.9/src/icad_tone_detection/audio_loader.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.8/src/icad_tone_detection/frequency_extraction.py` & `icad_tone_detection-0.9/src/icad_tone_detection/frequency_extraction.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,38 +39,52 @@
         Extracts frequencies from the audio data using STFT.
 
         Returns:
             list: A list of tuples, each containing the start time and a list of matching frequencies, or None if an error occurs.
         """
         try:
             window = 'hann'
-            n_fft = 2048  # Number of FFT points
+            n_fft = 2048  # Number of FFT points, smaller values may be considered if finer time resolution is needed
 
             # Calculate hop_length based on the desired time resolution
-            hop_length = int(self.frame_rate * self.time_resolution_ms / 1000)
+            hop_length = max(1, int(self.frame_rate * self.time_resolution_ms / 1000))
 
             # Perform the STFT
-            frequencies, _, zxx = stft(self.samples, self.frame_rate, window=window, nperseg=n_fft,
-                                       noverlap=n_fft - hop_length)
+            frequencies, time_samples, zxx = stft(self.samples, self.frame_rate, window=window, nperseg=n_fft, noverlap=n_fft - hop_length)
             amplitude = np.abs(zxx)  # Get the magnitude of the STFT coefficients
 
             # Convert amplitude to decibels
             amplitude_db = self.amplitude_to_decibels(amplitude, np.max(amplitude))
 
             # Detect the frequency with the highest amplitude at each time step
             detected_frequencies = frequencies[np.argmax(amplitude_db, axis=0)]
 
-            matching_frequencies = self.match_frequencies(detected_frequencies.tolist())
+            matching_frequencies = self.match_frequencies(detected_frequencies.tolist(), time_samples)
 
             return matching_frequencies
 
         except Exception as e:
             print(f"Error extracting frequencies: {e}")
             return None
 
+    def dynamic_threshold(self, frequencies, index):
+        """
+        Calculates a dynamic threshold based on the frequency changes.
+        """
+        base_frequency = frequencies[max(0, index - 1)]
+        return base_frequency * self.matching_threshold / 100
+
+    def calculate_times(self, start_index, end_index, time_samples):
+        """
+        Calculates accurate start and end times for frequency matches.
+        """
+        start_time = round(time_samples[start_index], 3)
+        end_time = round(time_samples[end_index - 1], 3)
+        return start_time, end_time
+
     @staticmethod
     def amplitude_to_decibels(amplitude, reference_value):
         """
         Converts amplitude to decibels relative to a reference value.
 
         Parameters:
             amplitude (np.array): The amplitude of the frequencies.
@@ -79,51 +93,50 @@
         Returns:
             np.array: The amplitude in decibels.
         """
         # Ensure the reference is not zero to avoid division by zero
         reference_value = np.maximum(reference_value, 1e-20)
         return 20 * np.log10(np.maximum(amplitude, 1e-20) / reference_value)
 
-    def match_frequencies(self, detected_frequencies):
+    def match_frequencies(self, detected_frequencies, time_samples):
         """
-        Identifies and groups matching frequencies from a list of detected frequencies based on the matching threshold.
-        Each group's start time, end time, and the matching frequencies are returned.
+            Identifies and groups matching frequencies from a list of detected frequencies based on the matching threshold.
+            Each group's start time, end time, and the matching frequencies are returned.
 
-        Parameters:
-            detected_frequencies (list of float): The detected frequencies from the audio sample.
+            Parameters:
+                detected_frequencies (list of float): The detected frequencies from the audio sample.
+                time_samples (np.array): Array of times corresponding to each frequency sample.
 
-        Returns:
-            list of tuples: Each tuple contains the start time, end time, and a list of matching frequencies.
+            Returns:
+                list of tuples: Each tuple contains the start time, end time, and a list of matching frequencies.
         """
+
         if not detected_frequencies:
             return []
 
         try:
             frequencies = [round(f, 1) for f in detected_frequencies]
             matching_frequencies = []
             current_match = [frequencies[0]]
-            start_index = 0  # Initialize start index for the first frequency
+            start_index = 0
 
             for i in range(1, len(frequencies)):
-                threshold = frequencies[i - 1] * self.matching_threshold / 100
+                threshold = self.dynamic_threshold(frequencies, i)
                 if abs(frequencies[i] - frequencies[i - 1]) <= threshold:
                     current_match.append(frequencies[i])
                 else:
                     if len(current_match) >= 2:
-                        # Calculate start and end times for the current match
-                        start_time = round(start_index * self.duration_seconds / len(frequencies), 3)
-                        end_time = round(i * self.duration_seconds / len(frequencies), 3)
-                        matching_frequencies.append((start_time, end_time, current_match))
+                        start_time, end_time = self.calculate_times(start_index, i, time_samples)
+                        freq_length = round((end_time - start_time) + .1, 2)
+                        matching_frequencies.append((start_time, end_time, freq_length, current_match))
                     current_match = [frequencies[i]]
-                    start_index = i  # Update start index for the new match
+                    start_index = i
 
-            # Handle the last group of matching frequencies
             if len(current_match) >= 2:
-                start_time = round(start_index * self.duration_seconds / len(frequencies), 3)
-                end_time = round(len(frequencies) * self.duration_seconds / len(
-                    frequencies), 3)  # End time for the last frequency
-                matching_frequencies.append((start_time, end_time, current_match))
+                start_time, end_time = self.calculate_times(start_index, len(frequencies), time_samples)
+                freq_length = round((end_time - start_time) + .1, 2)
+                matching_frequencies.append((start_time, end_time, freq_length, current_match))
 
             return matching_frequencies
         except Exception as e:
             print(f"Error matching frequencies: {e}")
-            return []
+            return []
```

### Comparing `icad_tone_detection-0.8/src/icad_tone_detection/main.py` & `icad_tone_detection-0.9/src/icad_tone_detection/main.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.8/src/icad_tone_detection.egg-info/PKG-INFO` & `icad_tone_detection-0.9/src/icad_tone_detection.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: icad_tone_detection
-Version: 0.8
+Name: icad-tone-detection
+Version: 0.9
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

