# Comparing `tmp/jzchatbot-59.83.96.tar.gz` & `tmp/jzchatbot-59.83.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.96.tar", last modified: Sun May 12 09:59:12 2024, max compression
+gzip compressed data, was "jzchatbot-59.83.97.tar", last modified: Sun May 12 10:06:12 2024, max compression
```

## Comparing `jzchatbot-59.83.96.tar` & `jzchatbot-59.83.97.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 09:59:12.120389 jzchatbot-59.83.96/
--rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.96/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-12 09:59:12.118642 jzchatbot-59.83.96/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.96/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 09:59:12.101419 jzchatbot-59.83.96/jzchatbot/
--rw-rw-rw-   0        0        0     5664 2024-05-12 09:58:55.000000 jzchatbot-59.83.96/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 09:59:12.117632 jzchatbot-59.83.96/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-12 09:59:12.000000 jzchatbot-59.83.96/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 09:59:12.120389 jzchatbot-59.83.96/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-12 09:59:06.000000 jzchatbot-59.83.96/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:06:12.180890 jzchatbot-59.83.97/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.97/LICENSE
+-rw-rw-rw-   0        0        0      343 2024-05-12 10:06:12.178787 jzchatbot-59.83.97/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.97/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 10:06:12.159952 jzchatbot-59.83.97/jzchatbot/
+-rw-rw-rw-   0        0        0     5955 2024-05-12 10:05:47.000000 jzchatbot-59.83.97/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:06:12.176406 jzchatbot-59.83.97/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 10:06:12.180890 jzchatbot-59.83.97/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-12 10:05:32.000000 jzchatbot-59.83.97/setup.py
```

### Comparing `jzchatbot-59.83.96/LICENSE` & `jzchatbot-59.83.97/LICENSE`

 * *Files identical despite different names*

### Comparing `jzchatbot-59.83.96/jzchatbot/__init__.py` & `jzchatbot-59.83.97/jzchatbot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,37 +113,41 @@
         self.engine.say(text)
         self.engine.runAndWait()
 
     def load_conversations(self, file_path):
         with open(file_path, 'r') as file:
             return json.load(file)
 
+    def run(self):
+        while True:
+            user_input = input("You: ")  # Wait for user to input command
+            if user_input.lower() == '/m on':
+                self.listen_for_input()  # Start listening for speech input
+            elif user_input.lower() == 'exit':
+                break
+            else:
+                bot_response = self.generate_response(user_input)
+                print(f"{self.name}: {bot_response}")
+                self.speak(bot_response)
+
     def listen_for_input(self):
         recognizer = sr.Recognizer()
         with sr.Microphone() as source:
             print("Listening...")
             recognizer.adjust_for_ambient_noise(source)  # Adjust microphone for ambient noise
             audio = recognizer.listen(source)  # Listen for audio input
 
         try:
             print("Recognizing...")
             user_input = recognizer.recognize_google(audio)  # Recognize speech using Google Speech Recognition
-            print("You:", user_input)
-            return user_input
+            print("You:", user_input)  # Print "You: " before the recognized user input
+            # Process the recognized user input here
+            bot_response = self.generate_response(user_input)
+            print(f"{self.name}: {bot_response}")
+            self.speak(bot_response)
         except sr.UnknownValueError:
             print("JZ: Sorry, I could not understand your speech.")
-            return ""
         except sr.RequestError as e:
             print("JZ: Speech recognition request failed:", e)
-            return ""
 
-    def run(self):
-        while True:
-            user_input = self.listen_for_input()  # Listen for user speech input
-            if user_input.lower() == 'exit':
-                break
-            if user_input:
-                bot_response = self.generate_response(user_input)
-                print(f"{self.name}: {bot_response}")
-                self.speak(bot_response)
```

### Comparing `jzchatbot-59.83.96/setup.py` & `jzchatbot-59.83.97/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.96", 
+	version="59.83.97", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

