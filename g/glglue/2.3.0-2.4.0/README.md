# Comparing `tmp/glglue-2.3.0.tar.gz` & `tmp/glglue-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glglue-2.3.0.tar", last modified: Fri May 10 11:00:43 2024, max compression
+gzip compressed data, was "glglue-2.4.0.tar", last modified: Mon May 13 04:07:41 2024, max compression
```

## Comparing `glglue-2.3.0.tar` & `glglue-2.4.0.tar`

### file list

```diff
@@ -1,127 +1,129 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.897657 glglue-2.3.0/
--rw-rw-rw-   0        0        0      321 2024-05-07 04:24:13.000000 glglue-2.3.0/.clang-format
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.829623 glglue-2.3.0/.github/
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.840880 glglue-2.3.0/.github/workflows/
--rw-rw-rw-   0        0        0     1321 2024-05-07 09:21:29.000000 glglue-2.3.0/.github/workflows/docusaurus.yml
--rw-rw-rw-   0        0        0       86 2024-05-08 10:16:01.000000 glglue-2.3.0/.gitignore
--rw-rw-rw-   0        0        0       75 2024-05-07 04:24:13.000000 glglue-2.3.0/.remarkrc
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.841879 glglue-2.3.0/.vscode/
--rw-rw-rw-   0        0        0     2760 2024-05-08 10:28:17.000000 glglue-2.3.0/.vscode/launch.json
--rw-rw-rw-   0        0        0      602 2024-05-07 04:24:13.000000 glglue-2.3.0/.vscode/settings.json
--rw-rw-rw-   0        0        0      555 2024-05-07 04:24:13.000000 glglue-2.3.0/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1065 2024-05-07 04:24:13.000000 glglue-2.3.0/LICENSE
--rw-rw-rw-   0        0        0     1884 2024-05-10 11:00:43.896872 glglue-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-05-07 09:19:11.000000 glglue-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.849395 glglue-2.3.0/docs/
--rw-rw-rw-   0        0        0      233 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/.gitignore
--rw-rw-rw-   0        0        0      768 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/README.md
--rw-rw-rw-   0        0        0       89 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/babel.config.js
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.851394 glglue-2.3.0/docs/blog/
--rw-rw-rw-   0        0        0      389 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2019-05-28-first-blog-post.md
--rw-rw-rw-   0        0        0     3116 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2019-05-29-long-blog-post.md
--rw-rw-rw-   0        0        0      439 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2021-08-01-mdx-blog-post.mdx
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.852395 glglue-2.3.0/docs/blog/2021-08-26-welcome/
--rw-rw-rw-   0        0        0    96122 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-rw-rw-   0        0        0      783 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2021-08-26-welcome/index.md
--rw-rw-rw-   0        0        0      447 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/authors.yml
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.853394 glglue-2.3.0/docs/docs/
--rw-rw-rw-   0        0        0      875 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/docs/index.md
--rw-rw-rw-   0        0        0     3760 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/docusaurus.config.ts
--rw-rw-rw-   0        0        0   570118 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/package-lock.json
--rw-rw-rw-   0        0        0     1150 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/package.json
--rw-rw-rw-   0        0        0      645 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/sidebars.ts
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.833417 glglue-2.3.0/docs/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.832312 glglue-2.3.0/docs/src/components/
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.854480 glglue-2.3.0/docs/src/components/HomepageFeatures/
--rw-rw-rw-   0        0        0     1889 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/components/HomepageFeatures/index.tsx
--rw-rw-rw-   0        0        0      138 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/components/HomepageFeatures/styles.module.css
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.854480 glglue-2.3.0/docs/src/css/
--rw-rw-rw-   0        0        0     1042 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/css/custom.css
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.856480 glglue-2.3.0/docs/src/pages/
--rw-rw-rw-   0        0        0      365 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/pages/index.module.css
--rw-rw-rw-   0        0        0     1343 2024-05-07 09:25:04.000000 glglue-2.3.0/docs/src/pages/index.tsx
--rw-rw-rw-   0        0        0      118 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/pages/markdown-page.md
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.856480 glglue-2.3.0/docs/static/
--rw-rw-rw-   0        0        0        0 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/.nojekyll
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.859500 glglue-2.3.0/docs/static/img/
--rw-rw-rw-   0        0        0    55746 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/docusaurus-social-card.jpg
--rw-rw-rw-   0        0        0     5142 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/docusaurus.png
--rw-rw-rw-   0        0        0     3626 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/favicon.ico
--rw-rw-rw-   0        0        0     6438 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/logo.svg
--rw-rw-rw-   0        0        0    31486 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/undraw_docusaurus_mountain.svg
--rw-rw-rw-   0        0        0    36002 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/undraw_docusaurus_react.svg
--rw-rw-rw-   0        0        0    11887 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/undraw_docusaurus_tree.svg
--rw-rw-rw-   0        0        0      176 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/tsconfig.json
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.834376 glglue-2.3.0/examples/
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.864011 glglue-2.3.0/examples/basic/
--rw-rw-rw-   0        0        0      533 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/freeglut_sample.py
--rw-rw-rw-   0        0        0      394 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/glfw_sample.py
--rw-rw-rw-   0        0        0      632 2024-05-07 04:24:13.000000 glglue-2.3.0/examples/basic/gtk3_sample.py
--rw-rw-rw-   0        0        0      776 2024-05-07 04:24:13.000000 glglue-2.3.0/examples/basic/gtk4_sample.py
--rw-rw-rw-   0        0        0      391 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/pysdl2_sample.py
--rw-rw-rw-   0        0        0      591 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/pyside6_sample.py
--rw-rw-rw-   0        0        0      657 2024-05-07 04:24:13.000000 glglue-2.3.0/examples/basic/wgl_sample.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.865010 glglue-2.3.0/examples/gui/
--rw-rw-rw-   0        0        0     2630 2024-05-08 11:56:08.000000 glglue-2.3.0/examples/gui/pyside6_gui.py
--rw-rw-rw-   0        0        0      816 2024-05-07 09:19:11.000000 glglue-2.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 11:00:43.897657 glglue-2.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.835375 glglue-2.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.874369 glglue-2.3.0/src/glglue/
--rw-rw-rw-   0        0        0       67 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/__init__.py
--rw-rw-rw-   0        0        0      427 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.884585 glglue-2.3.0/src/glglue/assets/
--rw-rw-rw-   0        0        0   471984 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/assets/Utah_teapot_(solid).stl
--rw-rw-rw-   0        0        0      103 2024-05-10 10:42:28.000000 glglue-2.3.0/src/glglue/assets/line.frag
--rw-rw-rw-   0        0        0      261 2024-05-10 10:43:01.000000 glglue-2.3.0/src/glglue/assets/line.vert
--rw-rw-rw-   0        0        0      103 2024-05-10 10:39:30.000000 glglue-2.3.0/src/glglue/assets/mesh.frag
--rw-rw-rw-   0        0        0      462 2024-05-10 10:40:21.000000 glglue-2.3.0/src/glglue/assets/mesh.vert
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.886583 glglue-2.3.0/src/glglue/camera/
--rw-rw-rw-   0        0        0      279 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/camera/__init__.py
--rw-rw-rw-   0        0        0     7991 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/camera/camera.py
--rw-rw-rw-   0        0        0      891 2024-05-08 09:14:56.000000 glglue-2.3.0/src/glglue/camera/mouse_camera.py
--rw-rw-rw-   0        0        0     4730 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/camera/mouse_event.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.890790 glglue-2.3.0/src/glglue/drawable/
--rw-rw-rw-   0        0        0       55 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/drawable/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-05-08 13:11:26.000000 glglue-2.3.0/src/glglue/drawable/axes.py
--rw-rw-rw-   0        0        0     1398 2024-05-08 12:54:14.000000 glglue-2.3.0/src/glglue/drawable/cube.py
--rw-rw-rw-   0        0        0     1374 2024-05-10 10:51:55.000000 glglue-2.3.0/src/glglue/drawable/drawable.py
--rw-rw-rw-   0        0        0      892 2024-05-08 13:10:38.000000 glglue-2.3.0/src/glglue/drawable/grid.py
--rw-rw-rw-   0        0        0     1045 2024-05-08 12:56:37.000000 glglue-2.3.0/src/glglue/drawable/line_builder.py
--rw-rw-rw-   0        0        0     1699 2024-05-08 12:52:09.000000 glglue-2.3.0/src/glglue/drawable/mesh_builder.py
--rw-rw-rw-   0        0        0     2815 2024-05-08 13:02:37.000000 glglue-2.3.0/src/glglue/drawable/teapot.py
--rw-rw-rw-   0        0        0      509 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/frame_input.py
--rw-rw-rw-   0        0        0     5210 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glfw.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.893301 glglue-2.3.0/src/glglue/glo/
--rw-rw-rw-   0        0        0      470 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glo/__init__.py
--rw-rw-rw-   0        0        0     2461 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glo/fbo.py
--rw-rw-rw-   0        0        0     6221 2024-05-10 10:41:35.000000 glglue-2.3.0/src/glglue/glo/shader.py
--rw-rw-rw-   0        0        0     1980 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glo/texture.py
--rw-rw-rw-   0        0        0     1689 2024-05-10 08:05:17.000000 glglue-2.3.0/src/glglue/glo/vao.py
--rw-rw-rw-   0        0        0     3140 2024-05-10 10:30:35.000000 glglue-2.3.0/src/glglue/glo/vbo.py
--rw-rw-rw-   0        0        0     3755 2024-05-08 09:43:52.000000 glglue-2.3.0/src/glglue/glo/vertex_layout.py
--rw-rw-rw-   0        0        0     3144 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glut.py
--rw-rw-rw-   0        0        0     2659 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/gtk3.py
--rw-rw-rw-   0        0        0     3156 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/gtk4.py
--rw-rw-rw-   0        0        0     3625 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/pysdl2.py
--rw-rw-rw-   0        0        0     4672 2024-05-08 11:20:04.000000 glglue-2.3.0/src/glglue/pyside6.py
--rw-rw-rw-   0        0        0     2443 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/qgl4.py
--rw-rw-rw-   0        0        0     2452 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/qgl5.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.894301 glglue-2.3.0/src/glglue/scene/
--rw-rw-rw-   0        0        0     2781 2024-05-08 13:09:20.000000 glglue-2.3.0/src/glglue/scene/sample.py
--rw-rw-rw-   0        0        0      962 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/sdl.py
--rw-rw-rw-   0        0        0     2885 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/togl.py
--rw-rw-rw-   0        0        0     1475 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/util.py
--rw-rw-rw-   0        0        0    21812 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/wgl.py
--rw-rw-rw-   0        0        0   122098 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/win32con.py
--rw-rw-rw-   0        0        0      529 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/windowconfig.py
--rw-rw-rw-   0        0        0     3190 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/wxglcanvas.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.896369 glglue-2.3.0/src/glglue.egg-info/
--rw-rw-rw-   0        0        0     1884 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2653 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.895301 glglue-2.3.0/tests/
--rw-rw-rw-   0        0        0     1410 2024-05-07 04:24:13.000000 glglue-2.3.0/tests/test_numpy.py
--rw-rw-rw-   0        0        0      287 2024-05-07 09:19:11.000000 glglue-2.3.0/tests/test_py.py
--rw-rw-rw-   0        0        0      221 2024-05-07 09:19:11.000000 glglue-2.3.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.309191 glglue-2.4.0/
+-rw-rw-rw-   0        0        0      321 2024-05-07 04:24:13.000000 glglue-2.4.0/.clang-format
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.010920 glglue-2.4.0/.github/
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.120323 glglue-2.4.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1321 2024-05-07 09:21:29.000000 glglue-2.4.0/.github/workflows/docusaurus.yml
+-rw-rw-rw-   0        0        0       86 2024-05-08 10:16:01.000000 glglue-2.4.0/.gitignore
+-rw-rw-rw-   0        0        0       75 2024-05-07 04:24:13.000000 glglue-2.4.0/.remarkrc
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.182803 glglue-2.4.0/.vscode/
+-rw-rw-rw-   0        0        0     3074 2024-05-13 04:07:01.000000 glglue-2.4.0/.vscode/launch.json
+-rw-rw-rw-   0        0        0      602 2024-05-07 04:24:13.000000 glglue-2.4.0/.vscode/settings.json
+-rw-rw-rw-   0        0        0      555 2024-05-07 04:24:13.000000 glglue-2.4.0/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1065 2024-05-07 04:24:13.000000 glglue-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1884 2024-05-13 04:07:41.309191 glglue-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-05-07 09:19:11.000000 glglue-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.323957 glglue-2.4.0/docs/
+-rw-rw-rw-   0        0        0      233 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/.gitignore
+-rw-rw-rw-   0        0        0      768 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/README.md
+-rw-rw-rw-   0        0        0       89 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/babel.config.js
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.417819 glglue-2.4.0/docs/blog/
+-rw-rw-rw-   0        0        0      389 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2019-05-28-first-blog-post.md
+-rw-rw-rw-   0        0        0     3116 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2019-05-29-long-blog-post.md
+-rw-rw-rw-   0        0        0      439 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2021-08-01-mdx-blog-post.mdx
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.417819 glglue-2.4.0/docs/blog/2021-08-26-welcome/
+-rw-rw-rw-   0        0        0    96122 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-rw-rw-   0        0        0      783 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2021-08-26-welcome/index.md
+-rw-rw-rw-   0        0        0      447 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/authors.yml
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.433348 glglue-2.4.0/docs/docs/
+-rw-rw-rw-   0        0        0      875 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/docs/index.md
+-rw-rw-rw-   0        0        0     3760 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/docusaurus.config.ts
+-rw-rw-rw-   0        0        0   570118 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/package-lock.json
+-rw-rw-rw-   0        0        0     1150 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/package.json
+-rw-rw-rw-   0        0        0      645 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/sidebars.ts
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.026454 glglue-2.4.0/docs/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.010920 glglue-2.4.0/docs/src/components/
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.449008 glglue-2.4.0/docs/src/components/HomepageFeatures/
+-rw-rw-rw-   0        0        0     1889 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/components/HomepageFeatures/index.tsx
+-rw-rw-rw-   0        0        0      138 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/components/HomepageFeatures/styles.module.css
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.464702 glglue-2.4.0/docs/src/css/
+-rw-rw-rw-   0        0        0     1042 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/css/custom.css
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.495942 glglue-2.4.0/docs/src/pages/
+-rw-rw-rw-   0        0        0      365 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/pages/index.module.css
+-rw-rw-rw-   0        0        0     1343 2024-05-07 09:25:04.000000 glglue-2.4.0/docs/src/pages/index.tsx
+-rw-rw-rw-   0        0        0      118 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/pages/markdown-page.md
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.495942 glglue-2.4.0/docs/static/
+-rw-rw-rw-   0        0        0        0 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/.nojekyll
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.558453 glglue-2.4.0/docs/static/img/
+-rw-rw-rw-   0        0        0    55746 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/docusaurus-social-card.jpg
+-rw-rw-rw-   0        0        0     5142 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/docusaurus.png
+-rw-rw-rw-   0        0        0     3626 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/favicon.ico
+-rw-rw-rw-   0        0        0     6438 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/logo.svg
+-rw-rw-rw-   0        0        0    31486 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-rw-rw-   0        0        0    36002 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/undraw_docusaurus_react.svg
+-rw-rw-rw-   0        0        0    11887 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/undraw_docusaurus_tree.svg
+-rw-rw-rw-   0        0        0      176 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/tsconfig.json
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.026454 glglue-2.4.0/examples/
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.620945 glglue-2.4.0/examples/basic/
+-rw-rw-rw-   0        0        0      533 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/freeglut_sample.py
+-rw-rw-rw-   0        0        0      394 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/glfw_sample.py
+-rw-rw-rw-   0        0        0      632 2024-05-07 04:24:13.000000 glglue-2.4.0/examples/basic/gtk3_sample.py
+-rw-rw-rw-   0        0        0      776 2024-05-07 04:24:13.000000 glglue-2.4.0/examples/basic/gtk4_sample.py
+-rw-rw-rw-   0        0        0      391 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/pysdl2_sample.py
+-rw-rw-rw-   0        0        0      591 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/pyside6_sample.py
+-rw-rw-rw-   0        0        0      657 2024-05-07 04:24:13.000000 glglue-2.4.0/examples/basic/wgl_sample.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.636579 glglue-2.4.0/examples/gui/
+-rw-rw-rw-   0        0        0     2630 2024-05-08 11:56:08.000000 glglue-2.4.0/examples/gui/pyside6_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.652196 glglue-2.4.0/examples/scene/
+-rw-rw-rw-   0        0        0     3832 2024-05-13 04:07:01.000000 glglue-2.4.0/examples/scene/pyside6_texture.py
+-rw-rw-rw-   0        0        0      816 2024-05-07 09:19:11.000000 glglue-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 04:07:41.309191 glglue-2.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.026454 glglue-2.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.933448 glglue-2.4.0/src/glglue/
+-rw-rw-rw-   0        0        0       67 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.011580 glglue-2.4.0/src/glglue/assets/
+-rw-rw-rw-   0        0        0   471984 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/assets/Utah_teapot_(solid).stl
+-rw-rw-rw-   0        0        0      103 2024-05-10 10:42:28.000000 glglue-2.4.0/src/glglue/assets/line.frag
+-rw-rw-rw-   0        0        0      261 2024-05-10 10:43:01.000000 glglue-2.4.0/src/glglue/assets/line.vert
+-rw-rw-rw-   0        0        0      103 2024-05-10 10:39:30.000000 glglue-2.4.0/src/glglue/assets/mesh.frag
+-rw-rw-rw-   0        0        0      462 2024-05-10 10:40:21.000000 glglue-2.4.0/src/glglue/assets/mesh.vert
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.042821 glglue-2.4.0/src/glglue/camera/
+-rw-rw-rw-   0        0        0      279 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/camera/__init__.py
+-rw-rw-rw-   0        0        0     7991 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/camera/camera.py
+-rw-rw-rw-   0        0        0      891 2024-05-08 09:14:56.000000 glglue-2.4.0/src/glglue/camera/mouse_camera.py
+-rw-rw-rw-   0        0        0     4730 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/camera/mouse_event.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.168456 glglue-2.4.0/src/glglue/drawable/
+-rw-rw-rw-   0        0        0       55 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/drawable/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-05-08 13:11:26.000000 glglue-2.4.0/src/glglue/drawable/axes.py
+-rw-rw-rw-   0        0        0     1816 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/drawable/cube.py
+-rw-rw-rw-   0        0        0     1374 2024-05-10 10:51:55.000000 glglue-2.4.0/src/glglue/drawable/drawable.py
+-rw-rw-rw-   0        0        0      892 2024-05-08 13:10:38.000000 glglue-2.4.0/src/glglue/drawable/grid.py
+-rw-rw-rw-   0        0        0     1045 2024-05-08 12:56:37.000000 glglue-2.4.0/src/glglue/drawable/line_builder.py
+-rw-rw-rw-   0        0        0     1335 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/drawable/mesh_builder.py
+-rw-rw-rw-   0        0        0     2949 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/drawable/teapot.py
+-rw-rw-rw-   0        0        0      509 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/frame_input.py
+-rw-rw-rw-   0        0        0     5210 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glfw.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.246630 glglue-2.4.0/src/glglue/glo/
+-rw-rw-rw-   0        0        0      470 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glo/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glo/fbo.py
+-rw-rw-rw-   0        0        0     6071 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/shader.py
+-rw-rw-rw-   0        0        0     2263 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/texture.py
+-rw-rw-rw-   0        0        0     1707 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/vao.py
+-rw-rw-rw-   0        0        0     3228 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/vbo.py
+-rw-rw-rw-   0        0        0     3755 2024-05-08 09:43:52.000000 glglue-2.4.0/src/glglue/glo/vertex_layout.py
+-rw-rw-rw-   0        0        0     3144 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glut.py
+-rw-rw-rw-   0        0        0     2659 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/gtk3.py
+-rw-rw-rw-   0        0        0     3156 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/gtk4.py
+-rw-rw-rw-   0        0        0     3625 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/pysdl2.py
+-rw-rw-rw-   0        0        0     4672 2024-05-08 11:20:04.000000 glglue-2.4.0/src/glglue/pyside6.py
+-rw-rw-rw-   0        0        0     2443 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/qgl4.py
+-rw-rw-rw-   0        0        0     2452 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/qgl5.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.262326 glglue-2.4.0/src/glglue/scene/
+-rw-rw-rw-   0        0        0     2999 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/scene/sample.py
+-rw-rw-rw-   0        0        0      962 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/sdl.py
+-rw-rw-rw-   0        0        0     2885 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/togl.py
+-rw-rw-rw-   0        0        0     1475 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/util.py
+-rw-rw-rw-   0        0        0    21812 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/wgl.py
+-rw-rw-rw-   0        0        0   122098 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/win32con.py
+-rw-rw-rw-   0        0        0      529 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/windowconfig.py
+-rw-rw-rw-   0        0        0     3190 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/wxglcanvas.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.309191 glglue-2.4.0/src/glglue.egg-info/
+-rw-rw-rw-   0        0        0     1884 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2687 2024-05-13 04:07:40.000000 glglue-2.4.0/src/glglue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.309191 glglue-2.4.0/tests/
+-rw-rw-rw-   0        0        0     1410 2024-05-07 04:24:13.000000 glglue-2.4.0/tests/test_numpy.py
+-rw-rw-rw-   0        0        0      287 2024-05-07 09:19:11.000000 glglue-2.4.0/tests/test_py.py
+-rw-rw-rw-   0        0        0      221 2024-05-07 09:19:11.000000 glglue-2.4.0/tests/test_utils.py
```

### Comparing `glglue-2.3.0/.github/workflows/docusaurus.yml` & `glglue-2.4.0/.github/workflows/docusaurus.yml`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/.vscode/launch.json` & `glglue-2.4.0/.vscode/launch.json`

 * *Files 6% similar despite different names*

```diff
@@ -72,9 +72,18 @@
             "type": "debugpy",
             "request": "launch",
             "stopOnEntry": false,
             "program": "${workspaceFolder}/examples/gui/pyside6_gui.py",
             "cwd": "${workspaceRoot}",
             "justMyCode": false
         },
+        {
+            "name": "scene/pyside6_texture",
+            "type": "debugpy",
+            "request": "launch",
+            "stopOnEntry": false,
+            "program": "${workspaceFolder}/examples/scene/pyside6_texture.py",
+            "cwd": "${workspaceRoot}",
+            "justMyCode": false
+        },
     ]
 }
```

### Comparing `glglue-2.3.0/.vscode/settings.json` & `glglue-2.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/.vscode/tasks.json` & `glglue-2.4.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/LICENSE` & `glglue-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/PKG-INFO` & `glglue-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glglue
-Version: 2.3.0
+Version: 2.4.0
 Summary: The glue code which mediates between OpenGL and some GUI
 Author-email: ousttrue <ousttrue@gmail.com>
 Project-URL: HomePage, https://ousttrue.github.io/glglue/
 Project-URL: Repository, https://github.com/ousttrue/glglue/
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
```

### Comparing `glglue-2.3.0/README.md` & `glglue-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/README.md` & `glglue-2.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/blog/2019-05-29-long-blog-post.md` & `glglue-2.4.0/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `glglue-2.4.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/blog/2021-08-26-welcome/index.md` & `glglue-2.4.0/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/docs/index.md` & `glglue-2.4.0/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/docusaurus.config.ts` & `glglue-2.4.0/docs/docusaurus.config.ts`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/package-lock.json` & `glglue-2.4.0/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/package.json` & `glglue-2.4.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/sidebars.ts` & `glglue-2.4.0/docs/sidebars.ts`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/src/components/HomepageFeatures/index.tsx` & `glglue-2.4.0/docs/src/components/HomepageFeatures/index.tsx`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/src/css/custom.css` & `glglue-2.4.0/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/src/pages/index.tsx` & `glglue-2.4.0/docs/src/pages/index.tsx`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/static/img/docusaurus-social-card.jpg` & `glglue-2.4.0/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/static/img/docusaurus.png` & `glglue-2.4.0/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/static/img/favicon.ico` & `glglue-2.4.0/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/static/img/logo.svg` & `glglue-2.4.0/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/static/img/undraw_docusaurus_mountain.svg` & `glglue-2.4.0/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/static/img/undraw_docusaurus_react.svg` & `glglue-2.4.0/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/docs/static/img/undraw_docusaurus_tree.svg` & `glglue-2.4.0/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/examples/basic/freeglut_sample.py` & `glglue-2.4.0/examples/basic/freeglut_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/examples/basic/gtk3_sample.py` & `glglue-2.4.0/examples/basic/gtk3_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/examples/basic/gtk4_sample.py` & `glglue-2.4.0/examples/basic/gtk4_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/examples/basic/pyside6_sample.py` & `glglue-2.4.0/examples/basic/pyside6_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/examples/basic/wgl_sample.py` & `glglue-2.4.0/examples/basic/wgl_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/examples/gui/pyside6_gui.py` & `glglue-2.4.0/examples/gui/pyside6_gui.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/pyproject.toml` & `glglue-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/assets/Utah_teapot_(solid).stl` & `glglue-2.4.0/src/glglue/assets/Utah_teapot_(solid).stl`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/camera/camera.py` & `glglue-2.4.0/src/glglue/camera/camera.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/camera/mouse_camera.py` & `glglue-2.4.0/src/glglue/camera/mouse_camera.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/camera/mouse_event.py` & `glglue-2.4.0/src/glglue/camera/mouse_event.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/drawable/axes.py` & `glglue-2.4.0/src/glglue/drawable/axes.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/drawable/cube.py` & `glglue-2.4.0/src/glglue/drawable/grid.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,31 @@
-from typing import NamedTuple
-import glm
-from glglue import glo
-from .mesh_builder import MeshBuilder
-from .drawable import Drawable
-
-"""
-OpenGL default is ccw
-
-+->
-|
-v
-  4 5
-  +-+
- / /
-+-+
-7 6
-  0 1
-  +-+
- / /
-+-+
-3 2
-"""
-S = 0.6
-VERTICES = [
-    glm.vec3(-S, -S, -S),
-    glm.vec3(S, -S, -S),
-    glm.vec3(S, -S, S),
-    glm.vec3(-S, -S, S),
-    glm.vec3(-S, S, -S),
-    glm.vec3(S, S, -S),
-    glm.vec3(S, S, S),
-    glm.vec3(-S, S, S),
-]
-
-
-class Face(NamedTuple):
-    indices: tuple[int, int, int, int]
-    color: tuple[float, float, float]
-
-
-# CCW
-QUADS = [
-    Face((7, 3, 2, 6), (0.5, 0.5, 1)),  # front
-    Face((5, 1, 0, 4), (0.5, 0.5, 1)),  # back
-    Face((6, 2, 1, 5), (1, 0.5, 0.5)),  # right
-    Face((4, 0, 3, 7), (1, 0.5, 0.5)),  # left
-    Face((4, 7, 6, 5), (0.5, 1, 0.5)),  # top
-    Face((0, 1, 2, 3), (0.5, 1, 0.5)),  # bottom
-]
-
-
-def create(shader: glo.Shader, props: list[glo.UniformUpdater]) -> Drawable:
-    builder = MeshBuilder()
-    for (i0, i1, i2, i3), rgb in QUADS:
-        builder.push_quad(
-            VERTICES[i0], VERTICES[i1], VERTICES[i2], VERTICES[i3], glm.vec3(*rgb)
-        )
-    vertices = builder.create_vertices()
-
-    vbo = glo.Vbo()
-    vbo.set_vertices(memoryview(vertices))
-
-    vao = glo.Vao(vbo, glo.VertexLayout.create_list(shader.program))
-
-    drawable = Drawable(vao)
-    drawable.push_submesh(shader, len(vertices), props)
-    return drawable
+from .. import glo
+from .line_builder import LineBuilder
+from .drawable import Drawable
+import glm
+from OpenGL import GL  # type: ignore
+
+
+def create(shader: glo.Shader, props: list[glo.UniformUpdater], n: int = 5) -> Drawable:
+    builder = LineBuilder()
+
+    for x in range(-n, n + 1):
+        builder.push_line(
+            glm.vec3(x, 0, -n), glm.vec3(x, 0, n), glm.vec3(0.5, 0.5, 0.5)
+        )
+    for z in range(-n, n + 1):
+        builder.push_line(
+            glm.vec3(-n, 0, z), glm.vec3(n, 0, z), glm.vec3(0.5, 0.5, 0.5)
+        )
+
+    vertices = builder.create_vertices()
+
+    vbo = glo.Vbo()
+    vbo.set_vertices(memoryview(vertices))
+
+    vao = glo.Vao(
+        vbo, glo.VertexLayout.create_list(shader.program), topology=GL.GL_LINES
+    )
+
+    drawable = Drawable(vao)
+    drawable.push_submesh(shader, len(vertices), props)
+    return drawable
```

### Comparing `glglue-2.3.0/src/glglue/drawable/drawable.py` & `glglue-2.4.0/src/glglue/drawable/drawable.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/drawable/line_builder.py` & `glglue-2.4.0/src/glglue/drawable/line_builder.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/drawable/mesh_builder.py` & `glglue-2.4.0/src/glglue/drawable/mesh_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,54 @@
-from typing import List
+from typing import TypeVar, Generic, Type
 import ctypes
 import glm
 
 
-class Float3(ctypes.Structure):
+class Float2(ctypes.Structure):
     _fields_ = [
         ("x", ctypes.c_float),
         ("y", ctypes.c_float),
-        ("z", ctypes.c_float),
     ]
 
     def __iter__(self):
         yield self.x
         yield self.y
         yield self.z
 
 
-class Vertex(ctypes.Structure):
+class Float3(ctypes.Structure):
     _fields_ = [
-        ("position", Float3),
-        ("normal", Float3),
-        ("color", Float3),
+        ("x", ctypes.c_float),
+        ("y", ctypes.c_float),
+        ("z", ctypes.c_float),
     ]
 
+    def __iter__(self):
+        yield self.x
+        yield self.y
+        yield self.z
+
+
+def calc_normal(p0: glm.vec3, p1: glm.vec3, p2: glm.vec3) -> glm.vec3:
+    return glm.cross(glm.normalize(p0 - p1), glm.normalize(p2 - p1))  # type: ignore
+
+
+T = TypeVar("T", bound=ctypes.Structure)
+
+
+class MeshBuilder(Generic[T]):
+    # https://stackoverflow.com/questions/67717984/how-to-add-python-type-hints-to-runtime-type
+    def __init__(self, t: Type[T]) -> None:
+        self.T = t
+        self.vertices: list[T] = []
+
+    def push_triangle(self, p0: T, p1: T, p2: T):
+        self.vertices.append(p0)
+        self.vertices.append(p1)
+        self.vertices.append(p2)
+
+    def push_quad(self, p0: T, p1: T, p2: T, p3: T):
+        self.push_triangle(p0, p1, p2)
+        self.push_triangle(p2, p3, p0)
 
-class MeshBuilder:
-    def __init__(self) -> None:
-        self.vertices: List[Vertex] = []
-
-    def push_triangle(
-        self, p0: glm.vec3, p1: glm.vec3, p2: glm.vec3, n: glm.vec3, color: glm.vec3
-    ):
-        self.vertices.append(
-            Vertex(
-                Float3(p0.x, p0.y, p0.z),
-                Float3(n.x, n.y, n.z),
-                Float3(color.x, color.y, color.z),
-            )
-        )
-        self.vertices.append(
-            Vertex(
-                Float3(p1.x, p1.y, p1.z),
-                Float3(n.x, n.y, n.z),
-                Float3(color.x, color.y, color.z),
-            )
-        )
-        self.vertices.append(
-            Vertex(
-                Float3(p2.x, p2.y, p2.z),
-                Float3(n.x, n.y, n.z),
-                Float3(color.x, color.y, color.z),
-            )
-        )
-
-    def push_quad(
-        self, p0: glm.vec3, p1: glm.vec3, p2: glm.vec3, p3: glm.vec3, color: glm.vec3
-    ):
-        n = glm.cross(glm.normalize(p0 - p1), glm.normalize(p2 - p1))  # type: ignore
-        self.push_triangle(p0, p1, p2, n, color)
-        self.push_triangle(p2, p3, p0, n, color)
-
-    def create_vertices(self) -> ctypes.Array[Vertex]:
-        vertices = (Vertex * len(self.vertices))(*self.vertices)
-        return vertices
+    def create_vertices(self) -> ctypes.Array[T]:
+        return (self.T * len(self.vertices))(*self.vertices)
```

### Comparing `glglue-2.3.0/src/glglue/drawable/teapot.py` & `glglue-2.4.0/src/glglue/drawable/teapot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ctypes
 import struct
 import pkgutil
 from glglue import glo
-from .mesh_builder import Float3, Vertex
+from .mesh_builder import Float3
 from .drawable import Drawable
 
 
 WHITE = Float3(1, 1, 1)
 
 
 class StlTriangle(ctypes.Structure):
@@ -40,14 +40,22 @@
         return struct.unpack("I", data)[0]
 
     def read_float32(self) -> float:
         data = self.read(4)
         return struct.unpack("f", data)[0]
 
 
+class Vertex(ctypes.Structure):
+    _fields_ = [
+        ("position", Float3),
+        ("normal", Float3),
+        ("color", Float3),
+    ]
+
+
 def load_teapot() -> ctypes.Array[Vertex]:
     # https://en.wikipedia.org/wiki/Utah_teapot#/media/File:Utah_teapot_(solid).stl
     data = pkgutil.get_data("glglue", "assets/Utah_teapot_(solid).stl")
     assert data
 
     # https://en.wikipedia.org/wiki/STL_%28file_format%29
     r = BinaryReader(data)
```

### Comparing `glglue-2.3.0/src/glglue/glfw.py` & `glglue-2.4.0/src/glglue/glfw.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/glo/fbo.py` & `glglue-2.4.0/src/glglue/glo/fbo.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/glo/shader.py` & `glglue-2.4.0/src/glglue/glo/shader.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,44 +94,38 @@
             return True, ""
 
         # error message
         info = GL.glGetProgramInfoLog(self.program)
         return False, info.decode("ascii")
 
     @staticmethod
-    def load(
-        vs_src: Union[str, bytes], fs_src: Union[str, bytes]
-    ) -> Union["Shader", str]:
+    def load(vs_src: Union[str, bytes], fs_src: Union[str, bytes]) -> "Shader":
         vs = ShaderCompile(GL.GL_VERTEX_SHADER)  # type: ignore
         success, info = vs.compile(vs_src)
         if not success:
-            return "vs: " + info
+            raise RuntimeError("vs: " + info)
         fs = ShaderCompile(GL.GL_FRAGMENT_SHADER)  # type: ignore
         success, info = fs.compile(fs_src)
         if not success:
-            return "fs: " + info
+            raise RuntimeError("fs: " + info)
         shader = Shader()
         success, info = shader.link(vs.shader, fs.shader)
         if not success:
-            return "link: " + info
+            raise RuntimeError("link: " + info)
         return shader
 
     @staticmethod
-    def load_from_pkg(pkg: str, name: str) -> Optional["Shader"]:
+    def load_from_pkg(pkg: str, name: str) -> "Shader":
         import pkgutil
 
         vs = pkgutil.get_data(pkg, f"{name}.vert")
         assert vs
         fs = pkgutil.get_data(pkg, f"{name}.frag")
         assert fs
-        match Shader.load(vs, fs):
-            case Shader() as shader:
-                return shader
-            case str() as info:
-                LOGGER.error(f"{pkg}#{name}: {info}")
+        return Shader.load(vs, fs)
 
     def create_props(
         self, camera: Camera, node: Node | None = None
     ) -> List[UniformUpdater]:
 
         props: List[Callable[[], None]] = []
```

### Comparing `glglue-2.3.0/src/glglue/glo/texture.py` & `glglue-2.4.0/src/glglue/glo/texture.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,70 @@
 from typing import Optional
 from OpenGL import GL
 import logging
+
 logger = logging.getLogger(__name__)
 
 
 class Texture:
-    def __init__(self, width: int, height: int, data: Optional[bytes] = None, *, pixel_type=GL.GL_RGBA) -> None:
+    def __init__(
+        self,
+        width: int,
+        height: int,
+        data: Optional[bytes] = None,
+        *,
+        pixel_type=GL.GL_RGBA,
+    ) -> None:
         self.width = width
         self.height = height
         # GL.GL_RGBA(32bit) or GL.GL_RED(8bit graysclale)
         self.pixel_type = pixel_type
         self.handle = GL.glGenTextures(1)
-        logger.debug(f'Texture: {self.handle}')
+        logger.debug(f"Texture: {self.handle}")
 
         self.bind()
 
         GL.glPixelStorei(GL.GL_UNPACK_ALIGNMENT, 1)
         # GL.glPixelStorei(GL.GL_UNPACK_ROW_LENGTH, width)
         GL.glPixelStorei(GL.GL_UNPACK_SKIP_PIXELS, 0)
         GL.glPixelStorei(GL.GL_UNPACK_SKIP_ROWS, 0)
 
-        GL.glTexImage2D(GL.GL_TEXTURE_2D, 0, self.pixel_type,
-                        width, height, 0, self.pixel_type, GL.GL_UNSIGNED_BYTE, data)
-        GL.glTexParameteri(
-            GL.GL_TEXTURE_2D, GL.GL_TEXTURE_MIN_FILTER, GL.GL_LINEAR)
-        GL.glTexParameteri(
-            GL.GL_TEXTURE_2D, GL.GL_TEXTURE_MAG_FILTER, GL.GL_LINEAR)
+        GL.glTexImage2D(
+            GL.GL_TEXTURE_2D,
+            0,
+            self.pixel_type,
+            width,
+            height,
+            0,
+            self.pixel_type,
+            GL.GL_UNSIGNED_BYTE,
+            data,
+        )
+        GL.glTexParameteri(GL.GL_TEXTURE_2D, GL.GL_TEXTURE_MIN_FILTER, GL.GL_LINEAR)
+        GL.glTexParameteri(GL.GL_TEXTURE_2D, GL.GL_TEXTURE_MAG_FILTER, GL.GL_LINEAR)
+        GL.glTexParameterf(GL.GL_TEXTURE_2D, GL.GL_TEXTURE_WRAP_S, GL.GL_REPEAT)
+        GL.glTexParameterf(GL.GL_TEXTURE_2D, GL.GL_TEXTURE_WRAP_T, GL.GL_REPEAT)
+
         self.unbind()
 
     def __del__(self):
-        logger.debug(f'{self.handle}')
+        logger.debug(f"{self.handle}")
         GL.glDeleteTextures([self.handle])
 
     def update(self, x, y, w, h, data):
         self.bind()
 
         GL.glPixelStorei(GL.GL_UNPACK_ALIGNMENT, 1)
         GL.glPixelStorei(GL.GL_UNPACK_ROW_LENGTH, self.width)
         GL.glPixelStorei(GL.GL_UNPACK_SKIP_PIXELS, x)
         GL.glPixelStorei(GL.GL_UNPACK_SKIP_ROWS, y)
 
-        GL.glTexSubImage2D(GL.GL_TEXTURE_2D, 0, x, y, w, h,
-                           self.pixel_type, GL.GL_UNSIGNED_BYTE, data)
+        GL.glTexSubImage2D(
+            GL.GL_TEXTURE_2D, 0, x, y, w, h, self.pixel_type, GL.GL_UNSIGNED_BYTE, data
+        )
 
         GL.glPixelStorei(GL.GL_UNPACK_ALIGNMENT, 4)
         GL.glPixelStorei(GL.GL_UNPACK_ROW_LENGTH, 0)
         GL.glPixelStorei(GL.GL_UNPACK_SKIP_PIXELS, 0)
         GL.glPixelStorei(GL.GL_UNPACK_SKIP_ROWS, 0)
 
         self.unbind()
```

### Comparing `glglue-2.3.0/src/glglue/glo/vao.py` & `glglue-2.4.0/src/glglue/glo/vao.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,11 +46,11 @@
 
     def draw(self, count: int, offset: int = 0, *, topology: int | None = None) -> None:
         if topology == None:
             topology = self.topology
 
         self.bind()
         if self.ibo:
-            GL.glDrawElements(topology, count, self.ibo.format, ctypes.c_void_p(offset))  # type: ignore
+            GL.glDrawElements(topology, count, self.ibo.format, ctypes.c_void_p(offset * self.ibo.stride))  # type: ignore
         else:
             GL.glDrawArrays(topology, offset, count)  # type: ignore
         self.unbind()
```

### Comparing `glglue-2.3.0/src/glglue/glo/vbo.py` & `glglue-2.4.0/src/glglue/glo/vbo.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self.unbind()
 
 
 class Ibo:
     def __init__(self):
         self.vbo: int = GL.glGenBuffers(1)
         self.format = 0
+        self.stride = 0
 
     def __del__(self) -> None:
         LOGGER.debug(f"delete vbo: {self.vbo}")
         GL.glDeleteBuffers(1, [self.vbo])
 
     def bind(self) -> None:
         GL.glBindBuffer(GL.GL_ELEMENT_ARRAY_BUFFER, self.vbo)  # type: ignore
@@ -59,16 +60,18 @@
         indices: bytes,
         stride: int,
         *,
         is_dynamic: bool = False,
     ):
         match stride:
             case 2:
+                self.stride = 2
                 self.format = GL.GL_UNSIGNED_SHORT  # type: ignore
             case 4:
+                self.stride = 4
                 self.format = GL.GL_UNSIGNED_INT  # type: ignore
             case _:
                 raise NotImplementedError()
         self.bind()
         GL.glBufferData(  # type: ignore
             GL.GL_ELEMENT_ARRAY_BUFFER,  # type: ignore
             len(indices),  # bytesize
```

### Comparing `glglue-2.3.0/src/glglue/glo/vertex_layout.py` & `glglue-2.4.0/src/glglue/glo/vertex_layout.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/glut.py` & `glglue-2.4.0/src/glglue/glut.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/gtk3.py` & `glglue-2.4.0/src/glglue/gtk3.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/gtk4.py` & `glglue-2.4.0/src/glglue/gtk4.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/pysdl2.py` & `glglue-2.4.0/src/glglue/pysdl2.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/pyside6.py` & `glglue-2.4.0/src/glglue/pyside6.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/qgl4.py` & `glglue-2.4.0/src/glglue/qgl4.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/qgl5.py` & `glglue-2.4.0/src/glglue/qgl5.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/scene/sample.py` & `glglue-2.4.0/src/glglue/scene/sample.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,53 +24,59 @@
     def __init__(self) -> None:
         self.initialized = False
         self.mouse_camera = MouseCamera()
         self.drawables: list[Drawable] = []
         self.cube_node = Node("cube")
         self.teapot_node = Node("teapot")
 
-    def lazy_initialize(self):
-        if self.initialized:
-            return
-        self.initialized = True
-
-        # shader
-        mesh_shader = glo.Shader.load_from_pkg("glglue", "assets/mesh")
-        assert mesh_shader
-        self.drawables.append(
-            cube.create(
-                mesh_shader,
-                mesh_shader.create_props(self.mouse_camera.camera, self.cube_node),
+    def render(self, frame: glglue.frame_input.FrameInput):
+        self.begin_render(frame)
+        self.draw()
+        self.end_render()
+
+    def draw(self):
+        if not self.initialized:
+            self.initialized = True
+
+            # shader
+            mesh_shader = glo.Shader.load_from_pkg("glglue", "assets/mesh")
+            self.drawables.append(
+                cube.create(
+                    mesh_shader,
+                    mesh_shader.create_props(self.mouse_camera.camera, self.cube_node),
+                )
             )
-        )
-        self.drawables.append(
-            teapot.create(
-                mesh_shader,
-                mesh_shader.create_props(self.mouse_camera.camera, self.teapot_node),
+            self.drawables.append(
+                teapot.create(
+                    mesh_shader,
+                    mesh_shader.create_props(
+                        self.mouse_camera.camera, self.teapot_node
+                    ),
+                )
             )
-        )
 
-        line_shader = glo.Shader.load_from_pkg("glglue", "assets/line")
-        assert line_shader
-        self.drawables.append(
-            axes.create(
-                line_shader,
-                line_shader.create_props(self.mouse_camera.camera),
+            line_shader = glo.Shader.load_from_pkg("glglue", "assets/line")
+            self.drawables.append(
+                axes.create(
+                    line_shader,
+                    line_shader.create_props(self.mouse_camera.camera),
+                )
             )
-        )
-        self.drawables.append(
-            grid.create(
-                line_shader,
-                line_shader.create_props(self.mouse_camera.camera),
+            self.drawables.append(
+                grid.create(
+                    line_shader,
+                    line_shader.create_props(self.mouse_camera.camera),
+                )
             )
-        )
 
-    def render(self, frame: glglue.frame_input.FrameInput):
-        self.lazy_initialize()
+        # render
+        for drawable in self.drawables:
+            drawable.draw()
 
+    def begin_render(self, frame: glglue.frame_input.FrameInput):
         # update camera
         self.mouse_camera.process(frame)
 
         # https://learnopengl.com/Advanced-OpenGL/Depth-testing
         GL.glEnable(GL.GL_DEPTH_TEST)  # type: ignore
         GL.glDepthFunc(GL.GL_LESS)  # type: ignore
 
@@ -87,13 +93,10 @@
             g = 0
         if frame.height == 0:
             return
         b = 0
         GL.glClearColor(r, g, b, 1.0)  # type: ignore
         GL.glClear(GL.GL_COLOR_BUFFER_BIT | GL.GL_DEPTH_BUFFER_BIT)  # type: ignore
 
-        # render
-        for drawable in self.drawables:
-            drawable.draw()
-
+    def end_render(self):
         # flush
         GL.glFlush()
```

### Comparing `glglue-2.3.0/src/glglue/sdl.py` & `glglue-2.4.0/src/glglue/sdl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/togl.py` & `glglue-2.4.0/src/glglue/togl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/util.py` & `glglue-2.4.0/src/glglue/util.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/wgl.py` & `glglue-2.4.0/src/glglue/wgl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/win32con.py` & `glglue-2.4.0/src/glglue/win32con.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/windowconfig.py` & `glglue-2.4.0/src/glglue/windowconfig.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue/wxglcanvas.py` & `glglue-2.4.0/src/glglue/wxglcanvas.py`

 * *Files identical despite different names*

### Comparing `glglue-2.3.0/src/glglue.egg-info/PKG-INFO` & `glglue-2.4.0/src/glglue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glglue
-Version: 2.3.0
+Version: 2.4.0
 Summary: The glue code which mediates between OpenGL and some GUI
 Author-email: ousttrue <ousttrue@gmail.com>
 Project-URL: HomePage, https://ousttrue.github.io/glglue/
 Project-URL: Repository, https://github.com/ousttrue/glglue/
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
```

### Comparing `glglue-2.3.0/src/glglue.egg-info/SOURCES.txt` & `glglue-2.4.0/src/glglue.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 examples/basic/glfw_sample.py
 examples/basic/gtk3_sample.py
 examples/basic/gtk4_sample.py
 examples/basic/pysdl2_sample.py
 examples/basic/pyside6_sample.py
 examples/basic/wgl_sample.py
 examples/gui/pyside6_gui.py
+examples/scene/pyside6_texture.py
 src/glglue/__init__.py
 src/glglue/_version.py
 src/glglue/frame_input.py
 src/glglue/glfw.py
 src/glglue/glut.py
 src/glglue/gtk3.py
 src/glglue/gtk4.py
```

### Comparing `glglue-2.3.0/tests/test_numpy.py` & `glglue-2.4.0/tests/test_numpy.py`

 * *Files identical despite different names*

