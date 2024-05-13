# Comparing `tmp/rendercat-1.0.0.dev0.tar.gz` & `tmp/rendercat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendercat-1.0.0.dev0.tar", last modified: Sat May 11 21:18:02 2024, max compression
+gzip compressed data, was "rendercat-1.0.1.tar", last modified: Mon May 13 18:48:16 2024, max compression
```

## Comparing `rendercat-1.0.0.dev0.tar` & `rendercat-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 21:18:02.768236 rendercat-1.0.0.dev0/
--rw-rw-rw-   0        0        0      918 2024-05-11 20:32:22.000000 rendercat-1.0.0.dev0/LICENSE
--rw-rw-rw-   0        0        0      612 2024-05-11 21:18:02.768236 rendercat-1.0.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-05-11 20:32:22.000000 rendercat-1.0.0.dev0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 21:18:02.760904 rendercat-1.0.0.dev0/RenderCat/
--rw-rw-rw-   0        0        0     2843 2024-05-11 21:16:40.000000 rendercat-1.0.0.dev0/RenderCat/__init__.py
--rw-rw-rw-   0        0        0     2163 2024-05-11 20:05:31.000000 rendercat-1.0.0.dev0/RenderCat/camera.py
--rw-rw-rw-   0        0        0      475 2024-05-09 19:51:38.000000 rendercat-1.0.0.dev0/RenderCat/light.py
--rw-rw-rw-   0        0        0      408 2024-05-09 11:16:33.000000 rendercat-1.0.0.dev0/RenderCat/loadobject.py
--rw-rw-rw-   0        0        0      284 2024-05-09 19:22:12.000000 rendercat-1.0.0.dev0/RenderCat/mesh.py
--rw-rw-rw-   0        0        0     3922 2024-05-09 20:18:35.000000 rendercat-1.0.0.dev0/RenderCat/model.py
--rw-rw-rw-   0        0        0     2074 2024-05-09 19:49:21.000000 rendercat-1.0.0.dev0/RenderCat/scene.py
--rw-rw-rw-   0        0        0      784 2024-05-09 20:10:30.000000 rendercat-1.0.0.dev0/RenderCat/scene_renderer.py
--rw-rw-rw-   0        0        0     7344 2024-05-11 21:11:58.000000 rendercat-1.0.0.dev0/RenderCat/shader_program.py
--rw-rw-rw-   0        0        0     2718 2024-05-09 19:43:02.000000 rendercat-1.0.0.dev0/RenderCat/texture.py
--rw-rw-rw-   0        0        0     2087 2024-05-11 20:32:22.000000 rendercat-1.0.0.dev0/RenderCat/vao.py
--rw-rw-rw-   0        0        0     4799 2024-05-11 20:32:22.000000 rendercat-1.0.0.dev0/RenderCat/vbo.py
-drwxrwxrwx   0        0        0        0 2024-05-11 21:18:02.766268 rendercat-1.0.0.dev0/rendercat.egg-info/
--rw-rw-rw-   0        0        0      612 2024-05-11 21:18:02.000000 rendercat-1.0.0.dev0/rendercat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-05-11 21:18:02.000000 rendercat-1.0.0.dev0/rendercat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 21:18:02.000000 rendercat-1.0.0.dev0/rendercat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-11 21:18:02.000000 rendercat-1.0.0.dev0/rendercat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-11 21:18:02.000000 rendercat-1.0.0.dev0/rendercat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 21:18:02.769047 rendercat-1.0.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0      944 2024-05-11 21:17:27.000000 rendercat-1.0.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:48:16.892121 rendercat-1.0.1/
+-rw-rw-rw-   0        0        0      918 2024-05-11 20:32:22.000000 rendercat-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      661 2024-05-13 18:48:16.892121 rendercat-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2024-05-13 15:46:23.000000 rendercat-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 18:48:16.885682 rendercat-1.0.1/RenderCat/
+-rw-rw-rw-   0        0        0     2666 2024-05-11 21:27:49.000000 rendercat-1.0.1/RenderCat/__init__.py
+-rw-rw-rw-   0        0        0     2163 2024-05-11 20:05:31.000000 rendercat-1.0.1/RenderCat/camera.py
+-rw-rw-rw-   0        0        0      475 2024-05-09 19:51:38.000000 rendercat-1.0.1/RenderCat/light.py
+-rw-rw-rw-   0        0        0      408 2024-05-09 11:16:33.000000 rendercat-1.0.1/RenderCat/loadobject.py
+-rw-rw-rw-   0        0        0      284 2024-05-09 19:22:12.000000 rendercat-1.0.1/RenderCat/mesh.py
+-rw-rw-rw-   0        0        0     4484 2024-05-13 18:43:00.000000 rendercat-1.0.1/RenderCat/model.py
+-rw-rw-rw-   0        0        0     2140 2024-05-13 18:35:22.000000 rendercat-1.0.1/RenderCat/scene.py
+-rw-rw-rw-   0        0        0      784 2024-05-09 20:10:30.000000 rendercat-1.0.1/RenderCat/scene_renderer.py
+-rw-rw-rw-   0        0        0     7344 2024-05-11 21:11:58.000000 rendercat-1.0.1/RenderCat/shader_program.py
+-rw-rw-rw-   0        0        0     2718 2024-05-09 19:43:02.000000 rendercat-1.0.1/RenderCat/texture.py
+-rw-rw-rw-   0        0        0     2087 2024-05-11 20:32:22.000000 rendercat-1.0.1/RenderCat/vao.py
+-rw-rw-rw-   0        0        0     4799 2024-05-11 20:32:22.000000 rendercat-1.0.1/RenderCat/vbo.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:48:16.890826 rendercat-1.0.1/rendercat.egg-info/
+-rw-rw-rw-   0        0        0      661 2024-05-13 18:48:16.000000 rendercat-1.0.1/rendercat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-13 18:48:16.000000 rendercat-1.0.1/rendercat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:48:16.000000 rendercat-1.0.1/rendercat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-13 18:48:16.000000 rendercat-1.0.1/rendercat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 18:48:16.000000 rendercat-1.0.1/rendercat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:48:16.892121 rendercat-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      940 2024-05-13 18:47:45.000000 rendercat-1.0.1/setup.py
```

### Comparing `rendercat-1.0.0.dev0/LICENSE` & `rendercat-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rendercat-1.0.0.dev0/PKG-INFO` & `rendercat-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: rendercat
-Version: 1.0.0.dev0
+Version: 1.0.1
 Summary: 3D engine made for pygame
 Home-page: https://github.com/TimofeyFilkin/RenderCat
 Author: TimofeyFilkin
 Author-email: timofejfilkin@gmail.com
 Keywords: python 3d opengl pygame
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <H1>Just a 3D engine <H3>made on python with OpenGl and pygame<H4>To start, just make a superclass of RenderCat.Engine.
+
+installation by
+
+```
+pip install rendercat
+```
```

### Comparing `rendercat-1.0.0.dev0/RenderCat/__init__.py` & `rendercat-1.0.1/RenderCat/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,21 @@
         self.scene_renderer = SceneRenderer(self)
         self.screen = pg.Surface(self.WIN_SIZE)
         self.overlay = self.mesh.vao.vaos['overlay']
         self.overlay.program['u_resolution'] = self.WIN_SIZE
 
     def check_events(self):
         for event in pg.event.get():
-            if event.type == pg.QUIT or (event.type == pg.KEYDOWN and event.key == pg.K_ESCAPE):
+            if event.type == pg.QUIT:
                 self.mesh.destroy()
                 self.scene_renderer.destroy()
                 sys.exit()
-            elif event.type == pg.KEYDOWN and event.key == pg.K_F11:
-                pg.display.toggle_fullscreen()
 
     def render(self):
         self.screen.fill((100, 200, 15))
-        pg.draw.circle(self.screen, (0, 0, 0), (self.WIN_SIZE[0] // 2, self.WIN_SIZE[1] // 2), 10)
         self.ctx.clear(color=(0.08, 0.16, 0.18))
         self.tick()
         self.scene_renderer.render()
         texture = self.screen.convert()
         texture = pg.transform.flip(texture, flip_x=False, flip_y=True)
         texture = self.ctx.texture(size=self.WIN_SIZE, components=3,
                                    data=pg.image.tostring(texture, 'RGB'))
@@ -65,14 +62,15 @@
         while True:
             self.get_time()
             self.check_events()
             self.render()
             self.delta_time = self.clock.tick(60)
 
     def tick(self):
+        pg.draw.circle(self.screen, (0, 0, 0), (self.WIN_SIZE[0] // 2, self.WIN_SIZE[1] // 2), 10)
         dx, dy = pg.mouse.get_rel()
         pg.mouse.set_pos((self.WIN_SIZE[0] / 2, self.WIN_SIZE[1] / 2))
         self.camera.rotate(dx, dy)
         self.camera.move()
 
 
 print("RenderCat v.1")
```

### Comparing `rendercat-1.0.0.dev0/RenderCat/camera.py` & `rendercat-1.0.1/RenderCat/camera.py`

 * *Files identical despite different names*

### Comparing `rendercat-1.0.0.dev0/RenderCat/model.py` & `rendercat-1.0.1/RenderCat/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glm
 import math
 
 
 class BaseModel:
-    def __init__(self, app, vao_name, tex_id, pos=(0, 0, 0), rot=(0, 0, 0), scale=(1, 1, 1)):
+    def __init__(self, app, vao_name, tex_id, pos=glm.vec3(0, 0, 0), rot=glm.vec3(0, 0, 0), scale=glm.vec3(1, 1, 1)):
         self.vao_name = vao_name
         self.app = app
         self.pos = pos
         self.rot = rot
         self.scale = scale
         self.m_model = self.get_model_matrix()
         self.tex_id = tex_id
@@ -17,15 +17,15 @@
 
     def update(self): ...
 
     def get_model_matrix(self):
         rot = list(self.rot)
         for i in range(0, 2):
             rot[i] = rot[i] / 180 * math.pi
-        m_model = glm.mat4()
+        m_model = glm.mat4(1.0)
         m_model = glm.translate(m_model, self.pos)
         m_model = glm.rotate(m_model, rot[0], glm.vec3(1, 0, 0))
         m_model = glm.rotate(m_model, rot[1], glm.vec3(0, 1, 0))
         m_model = glm.rotate(m_model, rot[2], glm.vec3(0, 0, 1))
         m_model = glm.scale(m_model, self.scale)
         return m_model
 
@@ -38,15 +38,26 @@
 class ExtendedBaseModel(BaseModel):
     def __init__(self, app, vao_name, tex_id, pos, rot, scale, attachment=''):
         self.script = attachment
         super().__init__(app, vao_name, tex_id, pos, rot, scale)
         self.on_init()
 
     def update(self):
+        pos, rot, scale = self.pos, self.rot, self.scale
+        print()
         exec(self.script)
+        pos, rot, scale = self.pos, self.rot, self.scale
+        m_model = glm.mat4(1.0)
+        m_model = glm.translate(m_model, pos)
+        m_model = glm.rotate(m_model, rot[0], glm.vec3(1, 0, 0))
+        m_model = glm.rotate(m_model, rot[1], glm.vec3(0, 1, 0))
+        m_model = glm.rotate(m_model, rot[2], glm.vec3(0, 0, 1))
+        m_model = glm.scale(m_model, scale)
+        self.pos, self.rot, self.scale = pos, rot, scale
+        self.m_model = m_model
         self.texture.use(location=0)
         self.program['camPos'].write(self.camera.position)
         self.program['m_view'].write(self.camera.m_view)
         self.program['m_model'].write(self.m_model)
         self.program['shadowMap'] = 1
         self.depth_texture.use(location=1)
```

### Comparing `rendercat-1.0.0.dev0/RenderCat/scene.py` & `rendercat-1.0.1/RenderCat/scene.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,30 +17,30 @@
         add = self.add_object
         objbuffer = []
         try:
             with open(file=f"Scenes/{map_to_load}.rcs", mode='r') as mapfile:
                 for line in mapfile:
                     value = line.split("|")
                     rawvalue = value[1].split(',')
-                    pos = (float(rawvalue[0]), float(rawvalue[1]), float(rawvalue[2]))
+                    pos = glm.vec3(float(rawvalue[0]), float(rawvalue[1]), float(rawvalue[2]))
                     rawvalue = value[2].split(',')
-                    rot = (float(rawvalue[0]), float(rawvalue[1]), float(rawvalue[2]))
+                    rot = glm.vec3(glm.radians(float(rawvalue[0])), glm.radians(float(rawvalue[1])), glm.radians(float(rawvalue[2])))
                     rawvalue = value[3].split(',')
-                    scale = (float(rawvalue[0]), float(rawvalue[1]), float(rawvalue[2]))
+                    scale = glm.vec3(float(rawvalue[0]), float(rawvalue[1]), float(rawvalue[2]))
                     objbuffer.append(Obj(vao_name=value[0], pos=pos, rot=rot, scale=scale,
                                          tex_id=value[4].rstrip(), attached_script=value[5].rstrip()))
                 mapfile.close()
             mapfile.close()
         except PermissionError:
             raise Exception("Cannot open map_to_load file: no permission.")
         except FileNotFoundError:
             raise Exception("Map not found!")
         for i in objbuffer:
             if i.script != 'None':
-                with open(file=f"Scenes/{map_to_load}/{i.script}") as scr:
+                with open(file=f"Scenes/{map_to_load}/{i.script}.py") as scr:
                     src = scr.read()
             else:
                 src = ''
             add(ExtendedBaseModel(app, pos=i.pos, rot=i.rot, scale=i.scale, tex_id=i.tex_id, vao_name=i.vao,
                                   attachment=src))
 
     def update(self):
```

### Comparing `rendercat-1.0.0.dev0/RenderCat/scene_renderer.py` & `rendercat-1.0.1/RenderCat/scene_renderer.py`

 * *Files identical despite different names*

### Comparing `rendercat-1.0.0.dev0/RenderCat/shader_program.py` & `rendercat-1.0.1/RenderCat/shader_program.py`

 * *Files identical despite different names*

### Comparing `rendercat-1.0.0.dev0/RenderCat/texture.py` & `rendercat-1.0.1/RenderCat/texture.py`

 * *Files identical despite different names*

### Comparing `rendercat-1.0.0.dev0/RenderCat/vao.py` & `rendercat-1.0.1/RenderCat/vao.py`

 * *Files identical despite different names*

### Comparing `rendercat-1.0.0.dev0/RenderCat/vbo.py` & `rendercat-1.0.1/RenderCat/vbo.py`

 * *Files identical despite different names*

### Comparing `rendercat-1.0.0.dev0/rendercat.egg-info/PKG-INFO` & `rendercat-1.0.1/rendercat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: rendercat
-Version: 1.0.0.dev0
+Version: 1.0.1
 Summary: 3D engine made for pygame
 Home-page: https://github.com/TimofeyFilkin/RenderCat
 Author: TimofeyFilkin
 Author-email: timofejfilkin@gmail.com
 Keywords: python 3d opengl pygame
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <H1>Just a 3D engine <H3>made on python with OpenGl and pygame<H4>To start, just make a superclass of RenderCat.Engine.
+
+installation by
+
+```
+pip install rendercat
+```
```

### Comparing `rendercat-1.0.0.dev0/setup.py` & `rendercat-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         for i in f:
             res.append(i)
         return res
 
 
 setup(
     name='rendercat',
-    version='1.0.0-DEV',
+    version='1.0.1',
     author='TimofeyFilkin',
     author_email='timofejfilkin@gmail.com',
     description='3D engine made for pygame',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/TimofeyFilkin/RenderCat',
     packages=find_packages(),
```

