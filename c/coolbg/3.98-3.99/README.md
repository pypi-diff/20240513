# Comparing `tmp/coolbg-3.98.tar.gz` & `tmp/coolbg-3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolbg-3.98.tar", last modified: Tue May 24 05:20:18 2022, max compression
+gzip compressed data, was "coolbg-3.99.tar", last modified: Tue May 31 10:57:10 2022, max compression
```

## Comparing `coolbg-3.98.tar` & `coolbg-3.99.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 05:20:18.823513 coolbg-3.98/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-24 05:20:18.823513 coolbg-3.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-24 05:20:08.000000 coolbg-3.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 05:20:18.823513 coolbg-3.98/bgeditor/
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 05:20:18.823513 coolbg-3.98/bgeditor/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/common/image_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 05:20:18.823513 coolbg-3.98/bgeditor/dao/
--rw-r--r--   0 runner    (1001) docker     (121)    28876 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/Component.py
--rw-r--r--   0 runner    (1001) docker     (121)     9405 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/FFmpeg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/Lyric.py
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/LyricStatic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/Matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     8130 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/MusicHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/RenderHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/Summon.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-24 05:20:08.000000 coolbg-3.98/bgeditor/dao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 05:20:18.823513 coolbg-3.98/coolbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-24 05:20:18.000000 coolbg-3.98/coolbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-05-24 05:20:18.000000 coolbg-3.98/coolbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-24 05:20:18.000000 coolbg-3.98/coolbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-24 05:20:18.000000 coolbg-3.98/coolbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-24 05:20:18.000000 coolbg-3.98/coolbg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-24 05:20:18.823513 coolbg-3.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-05-24 05:20:08.000000 coolbg-3.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 10:57:10.318823 coolbg-3.99/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-31 10:57:10.318823 coolbg-3.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-31 10:57:01.000000 coolbg-3.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 10:57:10.314823 coolbg-3.99/bgeditor/
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 10:57:10.314823 coolbg-3.99/bgeditor/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/common/image_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 10:57:10.314823 coolbg-3.99/bgeditor/dao/
+-rw-r--r--   0 runner    (1001) docker     (121)    29748 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/Component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9405 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/FFmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/Lyric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/LyricStatic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/Matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8130 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/MusicHelper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/RenderHelper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/Summon.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 10:57:01.000000 coolbg-3.99/bgeditor/dao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 10:57:10.318823 coolbg-3.99/coolbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-31 10:57:10.000000 coolbg-3.99/coolbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-05-31 10:57:10.000000 coolbg-3.99/coolbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 10:57:10.000000 coolbg-3.99/coolbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-31 10:57:10.000000 coolbg-3.99/coolbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-31 10:57:10.000000 coolbg-3.99/coolbg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-31 10:57:10.318823 coolbg-3.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-05-31 10:57:01.000000 coolbg-3.99/setup.py
```

### Comparing `coolbg-3.98/bgeditor/__init__.py` & `coolbg-3.99/bgeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/common/utils.py` & `coolbg-3.99/bgeditor/common/utils.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/dao/Component.py` & `coolbg-3.99/bgeditor/dao/Component.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,24 +72,33 @@
         utils.remove(tmp_path_composite_outro)
         audio_compilation.close()
         create_video_audio(final_clip_path, outro_sound, path_video)
     except:
         path_video = None
         pass
     return path_video
-def create_image(list_comp_data,path_img, t=0):
+def create_image(list_comp_data, path_img, t=0):
     arr_comps = []
     for comp_data in list_comp_data:
         comp_data["job_id"] = 1
         comp_data["mf_server"] = "http://api-magicframe.automusic.win/"
-        if comp_data['type'] == "compilation" or comp_data['type'] == "lyric" :
+        if comp_data['type'] == "video":
+            comp_data['c_type'] = 'image'
+        if comp_data['type'] == "compilation" or comp_data['type'] == "lyric":
             continue
-        arr_comps.append(Component.convert(comp_data).make())
 
-    CompositeVideoClip(arr_comps).save_frame(path_img,t)
+        arr_comps.append(Component.convert(comp_data))
+    arr_comps_maked=[]
+    for comp in arr_comps:
+        arr_comps_maked.append(comp.make())
+    CompositeVideoClip(arr_comps_maked).save_frame(path_img, t)
+    for compm in arr_comps_maked:
+        compm.close()
+    for comp in arr_comps:
+        comp.delete_res()
     return path_img
 
 def create_video(list_comp_data, path_video, job_id, mf_server):
     print('get list')
     intro_time=10
     intro_time_real=0
     arr_comps=[]
@@ -326,14 +335,21 @@
         print('setup')
     def order(self):
         print('order')
     def get_clip(self):
         print('get clip')
     def set_bg_clip(self,bg_clip):
         print('set bg clip')
+    def delete_res(self):
+        if hasattr(self,'audio_path') and self.audio_path:
+            utils.remove(self.audio_path)
+        if hasattr(self,'video_path') and self.video_path:
+            utils.remove(self.video_path)
+        if hasattr(self,'image_path') and self.image_path:
+            utils.remove(self.image_path)
     def get_audio(self):
         self.audio_path=None
         self.audio_moviepy=None
         if self.audio_url and self.audio_ext:
             self.audio_path = download_file(self.audio_url, ext=self.audio_ext)
             if self.audio_loop:
                 self.audio_path = create_loop_audio(self.audio_path, self.duration)
@@ -534,22 +550,28 @@
         self.md5 = json_data['md5']
         self.opacity = json_data['opacity']
         self.real_duration=0
         self.is_canva = json_data['isCanva']
         self.kind = "video"
         self.is_intro=False
         self.is_outro=False
+        self.c_type='video' #type get clip
+        if "c_type" in json_data:
+            self.c_type = json_data['c_type']
         if "is_intro" in json_data:
             self.is_intro = json_data['is_intro']
         if "is_outro" in json_data:
             self.is_outro = json_data['is_outro']
         if self.is_canva:
             self.kind = "canva"
     def get_clip(self):
-        if self.isLoop and self.isSmoothLoop and self.ext != "gif" and not self.is_intro and not self.is_outro and self.md5!="tiktok":
+        if self.c_type == 'image':
+            self.isLoop = False
+            self.isSmoothLoop = False
+        if self.isLoop and self.isSmoothLoop and self.ext != "gif" and not self.is_intro and not self.is_outro and self.md5 != "tiktok":
             obj = requests.get(self.mf_server+"resource/get-md5/"+self.kind+"/"+self.md5).json()
             if "id" in obj:
                 if "loop_link" in obj and obj['loop_link'] is not None and "gdrive" in obj['loop_link']:
                     self.video_path = download_file(obj['loop_link'], ext=self.ext)
                 else:
                     self.video_path = download_file(self.video_url, ext=self.ext)
                     path_loop = create_suource_can_loop_path(self.video_path, True, ext=self.ext)
@@ -568,15 +590,15 @@
             else:
                 has_mask = True
                 self.video_path = FFmpeg.convert_gif(self.video_path)
         if self.ext == "mov":
             has_mask = True
         rs = VideoFileClip(self.video_path, audio=not self.isMute, has_mask=has_mask)
         self.real_duration = rs.duration
-        if (self.index == 0 or self.isLoop) and rs.duration < 600: #max 20 mins loop
+        if ((self.index == 0 or self.isLoop) and self.c_type=='video') and rs.duration < 600: #max 20 mins loop
             rs.close()
             self.video_path = create_loop(self.video_path, 600)
             rs = VideoFileClip(self.video_path, audio=not self.isMute, has_mask=has_mask)
         if self.isMask:
             rs = mask_color.mask_color(rs, self.maskColor, thr=150, s=5)
         if self.opacity < 1.0:
             rs = rs.set_opacity(self.opacity)
```

### Comparing `coolbg-3.98/bgeditor/dao/FFmpeg.py` & `coolbg-3.99/bgeditor/dao/FFmpeg.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/dao/Lyric.py` & `coolbg-3.99/bgeditor/dao/Lyric.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/dao/LyricStatic.py` & `coolbg-3.99/bgeditor/dao/LyricStatic.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/dao/Matrix.py` & `coolbg-3.99/bgeditor/dao/Matrix.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/dao/MusicHelper.py` & `coolbg-3.99/bgeditor/dao/MusicHelper.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/dao/RenderHelper.py` & `coolbg-3.99/bgeditor/dao/RenderHelper.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/bgeditor/dao/Summon.py` & `coolbg-3.99/bgeditor/dao/Summon.py`

 * *Files identical despite different names*

### Comparing `coolbg-3.98/setup.py` & `coolbg-3.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='coolbg',
-    version='3.98',
+    version='3.99',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of coolbg",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/vtandroid/dokr",
     packages=setuptools.find_packages(),
```

