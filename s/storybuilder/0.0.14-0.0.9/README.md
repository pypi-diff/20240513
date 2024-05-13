# Comparing `tmp/storybuilder-0.0.14-py3-none-any.whl.zip` & `tmp/storybuilder-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 13943 bytes, number of entries: 12
+Zip file size: 13537 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      112 b- defN 24-May-13 03:49 storybuilder/__init__.py
--rw-r--r--  2.0 unx     4732 b- defN 24-May-13 09:16 storybuilder/characterpostures.py
--rw-r--r--  2.0 unx     1601 b- defN 24-May-13 06:39 storybuilder/cosuploader.py
+-rw-r--r--  2.0 unx     1601 b- defN 24-May-13 03:38 storybuilder/cosuploader.py
 -rw-r--r--  2.0 unx     5305 b- defN 24-May-13 04:00 storybuilder/speechsynthesizer.py
--rw-r--r--  2.0 unx    30823 b- defN 24-May-13 09:18 storybuilder/storybuilder.py
--rw-r--r--  2.0 unx     4715 b- defN 24-May-13 06:21 storybuilder/storyprofiles.py
+-rw-r--r--  2.0 unx    31502 b- defN 24-May-13 05:58 storybuilder/storybuilder.py
+-rw-r--r--  2.0 unx     4715 b- defN 24-May-12 15:23 storybuilder/storyprofiles.py
 -rw-r--r--  2.0 unx     2631 b- defN 24-May-13 04:01 storybuilder/storyvoicebuilder.py
--rw-r--r--  2.0 unx     1062 b- defN 24-May-13 09:24 storybuilder-0.0.14.dist-info/LICENSE
--rw-r--r--  2.0 unx      700 b- defN 24-May-13 09:24 storybuilder-0.0.14.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 09:24 storybuilder-0.0.14.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-13 09:24 storybuilder-0.0.14.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1021 b- defN 24-May-13 09:24 storybuilder-0.0.14.dist-info/RECORD
-12 files, 52807 bytes uncompressed, 12217 bytes compressed:  76.9%
+-rw-r--r--  2.0 unx     1062 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      699 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      926 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/RECORD
+11 files, 48658 bytes uncompressed, 11963 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,13 +1,10 @@
 Filename: storybuilder/__init__.py
 Comment: 
 
-Filename: storybuilder/characterpostures.py
-Comment: 
-
 Filename: storybuilder/cosuploader.py
 Comment: 
 
 Filename: storybuilder/speechsynthesizer.py
 Comment: 
 
 Filename: storybuilder/storybuilder.py
@@ -15,23 +12,23 @@
 
 Filename: storybuilder/storyprofiles.py
 Comment: 
 
 Filename: storybuilder/storyvoicebuilder.py
 Comment: 
 
-Filename: storybuilder-0.0.14.dist-info/LICENSE
+Filename: storybuilder-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: storybuilder-0.0.14.dist-info/METADATA
+Filename: storybuilder-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: storybuilder-0.0.14.dist-info/WHEEL
+Filename: storybuilder-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: storybuilder-0.0.14.dist-info/top_level.txt
+Filename: storybuilder-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: storybuilder-0.0.14.dist-info/RECORD
+Filename: storybuilder-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## storybuilder/storybuilder.py

```diff
@@ -4,15 +4,14 @@
 import uuid
 import copy
 import re
 import xml.etree.ElementTree as ET
 from PIL import Image
 
 from .storyprofiles import CHARACTER_FIGURE_ACCESSORY_KEYS, STORY_SCENARIO_STYLES
-from .characterpostures import CHARACTER_FIGURES
 
 class Story:
     
     @staticmethod
     def retrieveSvgSize(image_path):
         # Load the SVG file
         tree = ET.parse(image_path) 
@@ -52,49 +51,77 @@
                     height = dim2[1]
             elif '.jpg' in file_path[-4:] or '.jpeg' in file_path[-5:] or '.png' in file_path[-4:] or '.gif' in file_path[-4:]:
                 width, height = Story.retrievePixelSize(file_path)
         except:
                 print('retrieve image file size error =========', file_path)
         return width, height
 
+    def _loadStoryDataDefaults(self, filename, key='defaultCharacters'):
+        with open(filename) as f:
+            data = f.read()
+    
+        pattern = r'export const (\w+) = (.*?)(;)'
+        flags = re.DOTALL | re.MULTILINE
+    
+        matches = re.finditer(pattern, data, flags=flags)
+    
+        # Replace export const with key:
+        matched = {key:None}
+        for one_match in matches:
+            if one_match.group(1) == key:
+                cleaned_string = one_match.group(2).strip().replace('\n', '').replace(',]', ']')
+                matched[key] = json.loads(cleaned_string)
+        
+        return matched
+
+    
     def __init__(self, title, storyId=None, style="shinkai_makoto", **kwargs):
         self.title = title
         self.storyId = storyId if storyId!=None else uuid.uuid4()
         self.styles = STORY_SCENARIO_STYLES[style]
         self.locale = kwargs["locale"] if "locale" in kwargs else "cn"
         self.narrator = kwargs["narrator"] if "narrator" in kwargs else "M"
         self.pages = []
 
         self._cosUploader = kwargs["uploader"] if "uploader" in kwargs else None
         self._synthesizer = kwargs["synthesizer"] if "synthesizer" in kwargs else None
         
-        self._defaultCharacters = CHARACTER_FIGURES
+        self._defaultCharacters = None
+        # 需要提供defaultdata.tsx源文件所在项目根路径
+        figureSource = kwargs["figureSource"] if "figureSource" in kwargs else None
+        if figureSource != None:
+            print("Load default character figure info at", figureSource)
+
+            self._defaultCharacters = self._loadStoryDataDefaults(figureSource, key='defaultCharacters')['defaultCharacters']
+        else:
+            print("No source file for default character figure loaded, please input number for posture variable.")
 
         print("New story Id", self.storyId)
 
     def getUserPostureId(self, actor, postures, keyScenario = 'stand', excludeAccessories=True):
         if type(postures) is int:
             return postures
         if type(postures) is list and type(postures[0]) is int:
             return postures[0]
         if self._defaultCharacters == None:
             return 0
 
-        currentActorFigures = self._defaultCharacters[actor]
+        currentActorFigures = self._defaultCharacters[actor]['figure']
         availableFigures = []
         for j, figure in enumerate(currentActorFigures):
+            fullFigure = figure['source'].split('/')[-1]
             skip = False
             if excludeAccessories:
                 for accessory in CHARACTER_FIGURE_ACCESSORY_KEYS:
-                    if accessory in figure:
+                    if accessory in fullFigure:
                         skip = True
             if skip:
                 continue
-            if keyScenario in figure and all(keyWord in figure for keyWord in postures):
-                availableFigures.append({'index':j, 'figure':figure})
+            if keyScenario in fullFigure and all(keyWord in fullFigure for keyWord in postures):
+                availableFigures.append({'index':j, 'figure':fullFigure.split('.')[0]})
         if len(availableFigures) > 0:
             return random.choice(availableFigures)['index']
         else:
             return 0
 
     def appendPage(self, page):
         self.pages.append(page)
@@ -214,18 +241,15 @@
         locale = self.locale if locale == None else locale
         if len(self.subscripts) > 0 and scriptId < len(self.subscripts):
             if text != None:
                 self.subscripts[scriptId]['subscript'][locale] = text 
             if actor != None:
                 self.subscripts[scriptId]['narrator'] = actor
             if alternativeText != None:
-                if 'alternative' not in self.subscripts[scriptId]:
-                    self.subscripts[scriptId]['alternative'] = {locale: alternativeText}
-                else:
-                    self.subscripts[scriptId]['alternative'][locale] = alternativeText 
+                self.subscripts[scriptId]['alternative'][locale] = alternativeText 
         else:
             scriptId = scriptId - len(self.subscript)
             if len(self.narrations) > 0 and scriptId < len(self.narrations):
                 if text != None:
                     self.narrations[scriptId]['subscript'][locale] = text 
                 if actor != None:
                     self.narrations[scriptId]['narrator'] = actor
@@ -307,15 +331,15 @@
             "text": ""
           },
           "actor": self._getUserId("exam"),
           "type": "talk"
         })
 
         # 正确答案行为 onResult: 由所有正确答案id计算所得
-        if self.correctAnswerId > 0:
+        if self.answerId > 0:
             self.questionInteractions.append({
               "start": "",
               "duration": "",
               "onResult": self.correctAnswerId,
               "content": {
                 "popup": 2,
                 "text": ""
@@ -344,15 +368,15 @@
         if  self.story._cosUploader != None:
             target_path = kwargs["targetPath"] if "targetPath" in kwargs else None
             source = self.story._cosUploader.local2cos(source, self.story.storyId, target_path)    
         
         self.board["contentList"].append({
             "caption": {self.locale: kwargs["caption"]} if "caption" in kwargs else "",
             "rect": rect,
-            "image": {self.locale : source}
+            "image": {"cn" : source}
           })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outSubscripts = self.subscripts + self.questionSubscripts
         outInteractions = self.interactions + self.questionInteractions
 
         interactionOffset = len(self.interactions)
@@ -450,15 +474,15 @@
 ##### 黑板页面 #####
 class BlackboardPage(Page):
     def __init__(self, storyInstance, source, rect=[0,0,1,1]):
         assert len(rect)>=4 and type(rect) is list
         super().__init__("blackboard", storyInstance)
         self.scene = self.story.styles["scenarios"]["blackboard"]
         self.board = {
-            "content": {"image": {self.locale: source}},
+            "content": {"image": source},
             "rect": rect
         }
 
     def addNarration(self, text, narrator=None, alternativeText=None):
         if alternativeText != None:          
             self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
                                 "subscript":{self.locale: text}, 
@@ -477,20 +501,14 @@
                 "voice": len(self.subscripts)-1,
                 "text": {self.locale: text}
             },
             "actor": self._getUserId(narrator if narrator!=None else self.narrator),
             "type": "talk"
         })
 
-    def updateImage(self, source=None, rect=None, locale=None):
-        if source != None:
-            self.board["content"]["image"][locale if locale != None else self.locale] = source
-        if rect != None:
-            self.board["content"]["rect"] = rect
-
     def export(self, voiceOffset=0, pageId=0.0):
         outInteractions = copy.deepcopy(self.interactions)
         for i, interaction in enumerate(outInteractions):
             if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
                 outInteractions[i]["content"]["voice"] += voiceOffset
         return {
             "voices": self.subscripts,
@@ -565,15 +583,15 @@
 ##### 首页页面 #####
 class CoverPage(Page):
     def __init__(self, storyInstance, source, rect=[0,0,1,1]):
         assert len(rect)>=4 and type(rect) is list
         super().__init__("cover", storyInstance)
         self.scene = self.story.styles["scenarios"]["cover"]
         self.board = {
-            "content": {"image": {self.locale: source}},
+            "content": {"image": source},
             "rect": rect
         }
     
     def addNarration(self, text, narrator=None, alternativeText=None):            
         if alternativeText != None:
             self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
                                     "subscript":{self.locale: text}, 
@@ -676,15 +694,15 @@
             source = self.story._cosUploader.local2cos(source, self.story.storyId, target_path)
 
         self.board = {
             "content": {
                 "caption": kwargs["caption"] if "caption" in kwargs else "",
                 "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else "24px",
                 "fontColor": kwargs["fontColor"] if "fontColor" in kwargs else "white",
-                "image": {self.locale : source},
+                "image": {"cn" : source},
                 "magnify": True,
                 "border": self.story.styles["frame"]
             },
             "rect": rect
         }
         self.hasImage = True
 
@@ -698,15 +716,15 @@
                 rect[0] = 0.9 - rect[3]
             
         self.board = {
             "content": {
                 "caption": kwargs["caption"] if "caption" in kwargs else "",
                 "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else "24px",
                 "fontColor": kwargs["fontColor"] if "fontColor" in kwargs else "white",
-                "src": {self.locale: source},
+                "src": source,
                 "border": self.story.styles["frame"]
             },
             "rect": rect
         }
         if "videoType" in kwargs:
             self.board["content"]["videoType"] = kwargs["videoType"].lower()
         self.hasImage = True
```

## storybuilder/storyprofiles.py

```diff
@@ -138,15 +138,15 @@
             "blackboard": {"bgColor": "#98A698"},
             "concentrak": {"index": "0bd6c33e-31eb-4083-8dd8-ee07837bc975", "bgColor": "#C1D0BA"},
         },
         "frame": "10px solid #843C0C",
         "positions": {
             "left": [0.2, 0.05],
             "right": [0.8, 0.05],
-            "right-bottom": [0.85, -0.05],
+            "right_bottom": [0.85, -0.05],
         },
         "popup": 11,
         "scale": 1
     },
     "close_up": {
         "scenarios": {
             "cover": "5cdab8ba-c028-45ea-87cc-b0d75dd81e10",
@@ -165,13 +165,13 @@
             "blackboard": "e183c517-cbb7-4831-bcf6-efd310ee8790",
             "concentrak": {"index": "0bd6c33e-31eb-4083-8dd8-ee07837bc975", "bgColor": "#9BB9BF"},
         },
         "frame": "10px solid #843C0C",
         "positions": {
             "left": [0.2, -0.25],
             "right": [0.8, -0.25],
-            "right-bottom": [0.8, 0.05],
+            "right_bottom": [0.8, 0.05],
         },
         "popup": 10,
         "scale": 2
     }
 }
```

## Comparing `storybuilder-0.0.14.dist-info/LICENSE` & `storybuilder-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `storybuilder-0.0.14.dist-info/METADATA` & `storybuilder-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storybuilder
-Version: 0.0.14
+Version: 0.0.9
 Summary: A Python toolkit to build story meta.
 Author-email: Kelvin Xu <xxk59@hotmail.com>
 Project-URL: Homepage, https://github.com/xxk59/StoryBuilder
 Project-URL: Issues, https://github.com/xxk59/StoryBuilder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `storybuilder-0.0.14.dist-info/RECORD` & `storybuilder-0.0.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 storybuilder/__init__.py,sha256=DQYLSoMI3B4vfOI8Bbg_mnKlZJKvHhpgQMneo5cwErQ,112
-storybuilder/characterpostures.py,sha256=vmwMQ0seA8wR_8JGGoVJQwM2YgqtxpURybyIJbqrqfk,4732
 storybuilder/cosuploader.py,sha256=rejv5x0Am6axxOo4ewmmh7V2rB-K_rAETbpUh3kaW44,1601
 storybuilder/speechsynthesizer.py,sha256=mE6auE0vCfj7tnbcfcglpsWTOKYVnWA9jp1g-4bePL8,5305
-storybuilder/storybuilder.py,sha256=FLXekZg99qDENC-fSz0As5vbkgp-KQW01_HfIrZeC1s,30823
-storybuilder/storyprofiles.py,sha256=SA70Q4FEC-rQpaG8Awu4x1a__bx_11itzkKbHjN6Q6w,4715
+storybuilder/storybuilder.py,sha256=4SZu6EueY_Ddg09kdTJdVLZEvQQacYaxrO4W96U0wQk,31502
+storybuilder/storyprofiles.py,sha256=Eh04qKkQQd-jFJXKJ5H_R9gSXr4PTJY44kdjoP0mdEw,4715
 storybuilder/storyvoicebuilder.py,sha256=7EYGLloFaWWSqHKZ8MoLaWDQnIK41I_GAFQh6FOKoEk,2631
-storybuilder-0.0.14.dist-info/LICENSE,sha256=g0NNrixMENLCdfFk30AZvIBxy-oC-iGVvOO3ZeR54lw,1062
-storybuilder-0.0.14.dist-info/METADATA,sha256=zoVUO5zR4j8iU8Pqdm1EXNECogQ9bOLMWi8orPn3ZTo,700
-storybuilder-0.0.14.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-storybuilder-0.0.14.dist-info/top_level.txt,sha256=W-M011nO1TCCB8iNHIGxuaZupqBTafrvcqJPcoQiOSc,13
-storybuilder-0.0.14.dist-info/RECORD,,
+storybuilder-0.0.9.dist-info/LICENSE,sha256=g0NNrixMENLCdfFk30AZvIBxy-oC-iGVvOO3ZeR54lw,1062
+storybuilder-0.0.9.dist-info/METADATA,sha256=cZaeGnfSsQxjAf5i1Vl6IaKOXbdZfbxYya4-ANQad7I,699
+storybuilder-0.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+storybuilder-0.0.9.dist-info/top_level.txt,sha256=W-M011nO1TCCB8iNHIGxuaZupqBTafrvcqJPcoQiOSc,13
+storybuilder-0.0.9.dist-info/RECORD,,
```

