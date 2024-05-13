# Comparing `tmp/kbp2video-0.1.4.tar.gz` & `tmp/kbp2video-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbp2video-0.1.4.tar", last modified: Fri May 10 16:45:28 2024, max compression
+gzip compressed data, was "kbp2video-0.1.5.tar", last modified: Mon May 13 01:03:01 2024, max compression
```

## Comparing `kbp2video-0.1.4.tar` & `kbp2video-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 16:45:28.519838 kbp2video-0.1.4/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.4/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-10 16:45:28.519838 kbp2video-0.1.4/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.4/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 16:45:28.516505 kbp2video-0.1.4/kbp2video/
--rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-10 16:45:07.000000 kbp2video-0.1.4/kbp2video/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.4/kbp2video/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.4/kbp2video/_ffmpegcolor.py
--rw-r--r--   0 matt      (1000) matt      (1000)    76272 2024-05-10 16:45:07.000000 kbp2video-0.1.4/kbp2video/_gui.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.4/kbp2video/advanced_editor.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.4/kbp2video/utils.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 16:45:28.519838 kbp2video-0.1.4/kbp2video.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-10 16:45:28.000000 kbp2video-0.1.4/kbp2video.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-10 16:45:28.000000 kbp2video-0.1.4/kbp2video.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-10 16:45:28.000000 kbp2video-0.1.4/kbp2video.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-10 16:45:28.000000 kbp2video-0.1.4/kbp2video.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       53 2024-05-10 16:45:28.000000 kbp2video-0.1.4/kbp2video.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-10 16:45:28.000000 kbp2video-0.1.4/kbp2video.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-03 18:36:57.000000 kbp2video-0.1.4/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-10 16:45:28.519838 kbp2video-0.1.4/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-13 01:03:01.101735 kbp2video-0.1.5/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.5/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-13 01:03:01.098402 kbp2video-0.1.5/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.5/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-13 01:03:01.098402 kbp2video-0.1.5/kbp2video/
+-rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-13 01:02:39.000000 kbp2video-0.1.5/kbp2video/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.5/kbp2video/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.5/kbp2video/_ffmpegcolor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    80080 2024-05-13 01:02:39.000000 kbp2video-0.1.5/kbp2video/_gui.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.5/kbp2video/advanced_editor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.5/kbp2video/utils.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-13 01:03:01.098402 kbp2video-0.1.5/kbp2video.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-13 01:03:01.000000 kbp2video-0.1.5/kbp2video.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-13 01:03:01.000000 kbp2video-0.1.5/kbp2video.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-13 01:03:01.000000 kbp2video-0.1.5/kbp2video.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-13 01:03:01.000000 kbp2video-0.1.5/kbp2video.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       65 2024-05-13 01:03:01.000000 kbp2video-0.1.5/kbp2video.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-13 01:03:01.000000 kbp2video-0.1.5/kbp2video.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      433 2024-05-13 01:02:39.000000 kbp2video-0.1.5/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-13 01:03:01.101735 kbp2video-0.1.5/setup.cfg
```

### Comparing `kbp2video-0.1.4/LICENSE` & `kbp2video-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.4/kbp2video/_ffmpegcolor.py` & `kbp2video-0.1.5/kbp2video/_ffmpegcolor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.4/kbp2video/_gui.py` & `kbp2video-0.1.5/kbp2video/_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,30 @@
 from ._ffmpegcolor import ffmpeg_color
 import enum
 import kbputils
 import io
 import shutil
 from . import __version__
 import traceback
+import lastversion
 
 class TrackTableColumn(enum.Enum):
     KBP_ASS = 0
     Audio = 1
     Background = 2
     Advanced = 3
 
 # TODO: Possibly pull PlayRes? from .ass to letterbox
 class KBPASSWrapper:
     def __init__(self, path):
         if path.endswith(".ass"):
             self.ass_path = path
+            # raise correct exception we would get later from opening
+            with open(path, "r") as _:
+                pass
         else:
             self.kbp_path = path
             self.kbp_obj = kbputils.KBPFile(path)
     def ass_data(self, **kwargs):
         if hasattr(self,"kbp_path"):
             # Re-read file in case it changed on disk
             self.kbp_obj = kbputils.KBPFile(self.kbp_path)
@@ -471,35 +475,73 @@
 
     def dragLeaveEvent(self, event):
         self.parentWidget().setCurrentIndex(0)
 
 class ConverterSignals(QObject):
     finished = Signal()
     progress = Signal(int, int)
+    data = Signal(dict)
 
 class Converter(QRunnable):
     def __init__(self, function, *args, **kwargs):
         super().__init__()
         self.signals = ConverterSignals()
         self.function = function
         self.args = args
         self.kwargs = kwargs
 
     @Slot()
     def run(self):
         self.function(self.signals, *self.args, **self.kwargs)
 
+class UpdateBox(QMessageBox):
+    def _lastversion_wrap(self, signals):
+        try:
+            result = {}
+            version = lastversion.has_update(repo="ItMightBeKaraoke/kbp2video", at="github", pre_ok=True, current_version=__version__)
+            if version:
+                result['version'] = version
+                result['urls'] = lastversion.latest(repo='ItMightBeKaraoke/kbp2video', pre_ok=True, output_format='assets')
+        except:
+            result = {'error': traceback.format_exc(limit=2)}
+        signals.data.emit(result)
+
+    def __init__(self, parent, threadpool):
+        super().__init__(QMessageBox.Information, "Check for updates", "Checking for updates...", QMessageBox.StandardButton(QMessageBox.Ok), parent=parent)
+        self.runner = Converter(self._lastversion_wrap)
+        self.runner.signals.data.connect(self._display_data)
+        threadpool.start(self.runner)
+    
+    def update_check(parent, threadpool):
+        box = UpdateBox(parent, threadpool)
+        box.exec()
+
+    def _display_data(self, data):
+        if 'error' in data:
+            self.setWindowTitle("Check for updates: failed!")
+            self.setText(f"Failed to check for update:\n{data['error']}")
+        elif data:
+            self.setWindowTitle("Check for updates: update available!")
+            dl_info = ''.join(f'<br>Download <a href="{url}">{url.split("/")[-1]}</a>' for url in data['urls'])
+            self.setText(f"New version of kbp2video available ({data['version']})<br>&nbsp;{dl_info}")
+        else:
+            self.setWindowTitle("Check for updates: kbp2video up to date!")
+            self.setText(f"kbp2video current version {__version__} is running")
+
+        
+
 class Ui_MainWindow(QMainWindow):
 
     RELEVANT_FILE_FILTER = "*." + " *.".join(
         "kbp flac wav ogg opus mp3 aac mp4 mkv avi webm mov mpg mpeg jpg jpeg png gif jfif jxl bmp tiff webp".split())
 
-    def __init__(self):
+    def __init__(self, app):
         super().__init__()
         self.threadpool = QThreadPool()
+        self.app = app
         self.setupUi()
 
     # Convenience method for adding a Qt object as a property in self and and
     # setting its Qt object name
     def bind(self, name, obj):
         setattr(self, name, obj)
         obj.setObjectName(name)
@@ -508,20 +550,34 @@
     def setupUi(self):
         if not self.objectName():
             self.setObjectName("KBP to Video")
         self.resize(1280, 720)
         self.bind("centralWidget", QWidget(self))
 
         self.setCentralWidget(self.centralWidget)
-        # TODO: Create menubar with contents
-        # self.menubar = QMenuBar()
-        # self.menubar.setObjectName("menubar")
-        # self.menubar.setGeometry(QRect(0, 0, 886, 25))
-        # self.menubar.addMenu("test")
-        # self.setMenuBar(self.menubar)
+
+        # TODO: Create menubar contents
+        self.menubar = QMenuBar()
+        self.menubar.setObjectName("menubar")
+        #self.menubar.setGeometry(QRect(0, 0, 886, 25))
+        self.filemenu = self.menubar.addMenu("File")
+        self.filemenu.addAction("&Add/Import Files", Qt.CTRL | Qt.Key_I, self.add_files_button)
+        self.filemenu.addAction("&Quit", QKeySequence.Quit, self.app.quit)
+        self.editmenu = self.menubar.addMenu("Edit")
+        # TODO: Ctrl-A already works, would this be helpful
+        #self.editmenu.addAction("&Select All", self.select_all)
+        self.editmenu.addAction("&Remove Selected", QKeySequence.Delete, self.remove_files_button)
+        self.editmenu.addAction("&Add empty row", self.add_row_button)
+        self.editmenu.addAction("&Open/Edit Selected Files", QKeySequence.Open, self.remove_files_button)
+        self.editmenu.addAction("&Intro/Outro Settings", Qt.CTRL | Qt.Key_Return, self.advanced_button)
+        self.helpmenu = self.menubar.addMenu("Help")
+        self.helpmenu.addAction("&About", lambda: QMessageBox.about(self, "About kbp2video", f"kbp2video version: {__version__}\n\nUsing:\nkbputils version: {kbputils.__version__}\nffmpeg version: {ffmpeg_version}"))
+        self.helpmenu.addAction("&Check for Updates...", lambda: UpdateBox.update_check(self, self.threadpool))
+        self.setMenuBar(self.menubar)
+
         self.setStatusBar(self.bind("statusbar", QStatusBar(self)))
         try:
             q = QProcess(program="ffmpeg", arguments=["-version"])
             q.start()
             q.waitForFinished(1000)
             q.setReadChannel(QProcess.StandardOutput)
             version_line = str(q.readLine()).split()
@@ -934,15 +990,16 @@
         for row in sorted(
                 set(x.row() for x in self.tableWidget.selectedIndexes()),
                 reverse=True):
             self.tableWidget.setItem(row, TrackTableColumn.Background.value, QTableWidgetItem(
                 f"color: {self.colorText.text()}"))
 
     def advanced_button(self):
-        AdvancedEditor.showAdvancedEditor(self.tableWidget)
+        if self.tableWidget.selectedIndexes():
+            AdvancedEditor.showAdvancedEditor(self.tableWidget)
 
     def edit_button(self):
         rows = set(x.row() for x in self.tableWidget.selectedIndexes())
         if len(rows) == 1 or QMessageBox.question(self, f"Open {len(rows)} files?", f"Are you sure you want to open {len(rows)} files at the same time?") == QMessageBox.Yes:
             for row in rows:
                 QDesktopServices.openUrl(QUrl.fromLocalFile(self.tableWidget.filename(row, TrackTableColumn.KBP_ASS.value)))
 
@@ -1098,19 +1155,17 @@
     
     def vidFile(self, kbp):
         filename = os.path.basename(kbp)
         return self.resolved_output_dir(kbp) + "/" + filename[:-4] + "." + self.containerBox.currentText()
 
     def audioffmpegBitrate(self):
         if self.acodecBox.currentText() == 'flac':
-            # return ''
             return {}
         # TODO: Good defaults based on format
         else:
-            #return self.abitrateBox.text() or '-b:a 256k' # This couldn't have been working before for manually entered
             return {"audio_bitrate": self.abitrateBox.text() or '256k'}
 
     def get_aspect_ratio(self):
         text = self.aspectRatioBox.currentText()
         if (res := re.search(r'\((.*)\)', text)):
             text = res.group(1)
         ratio, border = (x.strip() for x in text.partition(",")[0:3:2])
@@ -1187,14 +1242,15 @@
         if self.overrideOffset.checkState() == Qt.Checked:
             assOptions += ["-o", f"{self.offset.value()}"]
             kbputils_options['offset'] = self.offset.value()
         if self.transparencyBox.checkState() != Qt.Checked:
             assOptions += ["--no-t"]
             kbputils_options['transparency'] = False
         kbputils_options['overflow'] = kbputils.AssOverflow[self.overflowBox.currentText().replace(" ", "_").upper()]
+        conversion_errors = False
         for row in range(self.tableWidget.rowCount()):
             kbp_table_item = self.tableWidget.item(row, TrackTableColumn.KBP_ASS.value)
             kbp_obj = kbp_table_item.data(Qt.UserRole) or kbp_table_item.text()
             kbp = str(kbp_obj)
             audio = self.tableWidget.filename(row, TrackTableColumn.Audio.value)
             background = self.tableWidget.filename(row, TrackTableColumn.Background.value)
             advanced = self.tableWidget.item(row, TrackTableColumn.Advanced.value).data(Qt.UserRole) or {}
@@ -1216,51 +1272,49 @@
             # bad mime type (not image/video or nonexistant file), or no background specified
             if background_type == None:
                 background_type = 0
                 background = default_bg
 
             assfile = self.assFile(kbp)
 
+            # Handle manually-typed filename. TODO: convert earlier, when the text value is updated
+            if not isinstance(kbp_obj, KBPASSWrapper):
+                try:
+                    kbp_obj = KBPASSWrapper(kbp_obj)
+                except:
+                    conversion_errors = True
+                    QMetaObject.invokeMethod(
+                        self,
+                        'info', 
+                        Qt.AutoConnection,
+                        Q_ARG(str, "Failed to process file"),
+                        Q_ARG(str, f"Failed to process file\n{kbp}\n\nError Output:\n{traceback.format_exc()}"))
+                    continue
             if hasattr(kbp_obj, "kbp_path"):
                 print("Converting the new way")
                 print(kbputils_options)
                 try:
                     data = kbp_obj.ass_data(**kbputils_options)
                 except:
+                    conversion_errors = True
                     QMetaObject.invokeMethod(
                         self,
                         'info', 
                         Qt.AutoConnection,
                         Q_ARG(str, "Failed to process kbp"),
                         Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{traceback.format_exc()}"))
                     continue
-            elif kbp.endswith(".ass"): # kbp_obj is either a KBPASSWrapper with a .ass file, or a manually entered string with .ass
+            else: # kbp_obj is a KBPASSWrapper with a .ass file
                 if any(x in kbp for x in ":;,'=\""):
                     print("Already .ass file, but needs new filename for ffmpeg")
                     QFile(kbp).copy(assfile)
                 else:
                     print("Using existing .ass file")
                     assfile = kbp
                     
-            else:
-                print("Falling back to kbp2ass")
-                print("kbp2ass " + " ".join(assOptions) + " " + kbp)
-                q = QProcess(program="kbp2ass", arguments=assOptions+[kbp])
-                q.start()
-                q.waitForFinished(-1)
-                data = q.readAllStandardOutput()
-                if q.exitStatus() != QProcess.NormalExit or data.isEmpty():
-                    QMetaObject.invokeMethod(
-                        self,
-                        'info', 
-                        Qt.AutoConnection,
-                        Q_ARG(str, "Failed to process kbp"),
-                        Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{q.readAllStandardError().toStdString()}"))
-                    continue
-
             # QDir is inconsistent. Needs to be static to check existence, and
             # mkdir needs to be run from an instantiated instance in the parent
             # directory, not worth the hassle
             if not os.path.isdir(outdir := self.resolved_output_dir(kbp)):
                 os.mkdir(outdir)
 
             # File was converted and .ass file needs to be written
@@ -1286,37 +1340,56 @@
                     kbp_table_item.setText(os.path.basename(assfile))
                     kbp_table_item.setToolTip(assfile)
                     kbp_table_item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsEnabled | Qt.ItemNeverHasChildren)
 
             if assOnly:
                 continue
 
-            #ffmpeg_options = ["-y"]
             output_options = {}
             base_assfile = os.path.basename(assfile)
             if background_type == 0:
-                #ffmpeg_options += f"-f lavfi -i color=color={background}:r=60:s={resolution}".split()
                 background_video = ffmpeg.input(f"color=color={background}:r=60:s={resolution}", f="lavfi")
                 bg_size = QSize(*(int(x) for x in resolution.split('x')))
             elif background_type == 1:
                 bg_size = QImage(background).size()
-                #ffmpeg_options += f"-loop 1 -framerate 60 -i".split() + [background]
                 background_video = ffmpeg.input(background, loop=1, framerate=60)
             elif background_type == 2:
                 # Pull the dimensions of the first video stream found in the file
-                bginfo = ffmpeg.probe(background)
+                try:
+                    bginfo = ffmpeg.probe(background)
+                except:
+                    conversion_errors = True
+                    QMetaObject.invokeMethod(
+                        self,
+                        'info',
+                        Qt.AutoConnection,
+                        Q_ARG(str, "Unable to process background video"),
+                        Q_ARG(str, f"Unable to determine the resolution of file\n{background}\n{traceback.format_exc()}"))
+                    continue
                 bg_size = next(QSize(x['width'],x['height']) for x in bginfo['streams'] if x['codec_type'] == 'video')
-                #ffmpeg_options += ["-i", background]
                 background_video = ffmpeg.input(background).video
-            #ffmpeg_options += ["-i", audio]
 
+            song_length = None
             # TODO figure out time/frame for outro
-            song_length = ffmpeg.probe(audio)['format']['duration']
             for x in ("intro", "outro"):
                 if f"{x}_enable" in advanced and advanced[f"{x}_enable"]:
+                    if not song_length:
+                        try:
+                            song_length = ffmpeg.probe(audio)['format']['duration']
+                        except:
+                            conversion_errors = True
+                            QMetaObject.invokeMethod(
+                                self,
+                                'info',
+                                Qt.AutoConnection,
+                                Q_ARG(str, "Unable to process audio"),
+                                Q_ARG(str, f"Unable to process audio file\n{audio}\n{traceback.format_exc()}"))
+                            # See continue after this loop that skips iteration of outer loop
+                            song_length = -1
+                            break
                     # TODO: alpha, sound?
                     opts = {}
                     if self.filedrop.mimedb.mimeTypeForFile(advanced[f"{x}_file"]).name().startswith('image/'):
                         opts["loop"]=1
                         opts["framerate"]=60
                     # TODO skip scale if matching?
                     # TODO set x/y if mismatched aspect ratio?
@@ -1342,14 +1415,18 @@
                                 if y == "Out":
                                     fade_settings["st"] = float(song_length) - float(advanced[f"{x}_fadeOut"].split(":")[1])
                                 else:
                                     fade_settings["st"] = float(song_length) - float(advanced[f"{x}_length"].split(":")[1])
                             overlay = overlay.filter_("fade", t=y.lower(), d=advanced[f"{x}_fade{y}"].split(":")[1], **fade_settings)
                     background_video = background_video.overlay(overlay, eof_action=("pass" if x == "intro" else "repeat"))
 
+            # Broke from inner loop after error
+            if song_length == -1:
+                continue
+
             audio_stream = ffmpeg.input(audio).audio
             if background_type == 1 or background_type == 2:
                 if not bg_size:
                     QMetaObject.invokeMethod(
                         self,
                         'info',
                         Qt.AutoConnection,
@@ -1380,30 +1457,26 @@
                 ass_move = {"y": round((bg_size.height() - ass_size.height())/2)}
             else:
                 ass_size = bg_size
                 # ass_move = ""
                 ass_move = {}
 
             if ass_move:
-                # ffmpeg_options += ["-filter_complex", f"color=color=000000@0:r=60:s={ass_size.width()}x{ass_size.height()},format=rgba,ass={base_assfile}:alpha=1[out1];[0:v][out1]overlay=eof_action=pass{ass_move}[out]", "-map", "[out]:v", "-map", "1:a"]
                 filtered_video = background_video.overlay(
                     ffmpeg_color(color="000000@0", r=60, s=f"{ass_size.width()}x{ass_size.height()}")
                         .filter_("format", "rgba")
                         .filter_("ass", base_assfile, alpha=1),
                     eof_action="pass",
                     **ass_move
                 )
             else:
-                # ffmpeg_options += ["-vf", f"ass={base_assfile}"]
                 filtered_video = background_video.filter_("ass", base_assfile)
             if background_type == 0 or background_type == 1:
-                #ffmpeg_options += ["-shortest"]
                 output_options["shortest"] = None
             # TODO: should pix_fmt be configurable or change default based on codec?
-            #ffmpeg_options += f"-pix_fmt yuv420p -c:a {self.acodecBox.currentText()} {self.audioffmpegBitrate()} -c:v {self.vcodecBox.currentText()}".split()
             output_options.update(self.audioffmpegBitrate())
 
             if check2bool(self.lossless):
                 if self.vcodecBox.currentText() == "libvpx-vp9":
                     output_options["lossless"]=1
                 elif self.vcodecBox.currentText() == "libx265":
                     output_options["x265-params"]="lossless=1"
@@ -1412,25 +1485,38 @@
             else:
                 output_options["crf"]=self.quality.value()
 
             if self.vcodecBox.currentText() == "libvpx-vp9":
                 output_options["video_bitrate"] = 0 # Required for the format to use CRF only
                 output_options["row-mt"] = 1 # Speeds up encode for most multicore systems
 
-            output_options.update({"pix_fmt": "yuv420p", "c:a": self.acodecBox.currentText(), "c:v": self.vcodecBox.currentText()})
-            # ffmpeg_options += [self.vidFile(kbp)]
+            output_options.update({
+                "pix_fmt": "yuv420p",
+                "c:a": self.acodecBox.currentText(),
+                "c:v": self.vcodecBox.currentText(),
+                "hide_banner": None,
+            })
             # TODO: determine if it's best to leave this as a QProcess, or use ffmpeg.run() and have it POpen itself
             ffmpeg_options = ffmpeg.output(filtered_video, audio_stream, self.vidFile(kbp), **output_options).overwrite_output().get_args()
             print(f'cd "{os.path.dirname(assfile)}"')
             print("ffmpeg" + " " + " ".join(f'"{x}"' for x in ffmpeg_options))
             q = QProcess(program="ffmpeg", arguments=ffmpeg_options, workingDirectory=os.path.dirname(assfile))
             q.start()
             q.waitForFinished(-1)
+            if q.exitStatus() != QProcess.NormalExit or q.exitCode() != 0:
+                conversion_errors = True
+                QMetaObject.invokeMethod(
+                    self,
+                    'info',
+                    Qt.AutoConnection,
+                    Q_ARG(str, "Failed to convert file"),
+                    Q_ARG(str, f"Failed to process file\n{kbp}\n\nError Output:\n{q.readAllStandardError().toStdString()}"))
+
         
-        self.statusbar.showMessage("Conversion completed!")
+        self.statusbar.showMessage(f"Conversion completed{' (with errors)' if conversion_errors else ''}!")
         signals.finished.emit()
 
     def retranslateUi(self):
         self.setWindowTitle(QCoreApplication.translate(
             "MainWindow", "KBP to Video", None))
         self.addButton.setText(QCoreApplication.translate(
             "MainWindow", "&Add Files...", None))
@@ -1548,10 +1634,10 @@
             os.environ['PATH'] = os.pathsep.join([result, orig_path])
         if not shutil.which("ffmpeg"):
             QMessageBox.critical(None, "ffmpeg not found", "ffmpeg still not found, please download the full release or otherwise install ffmpeg.")
             sys.exit(1)
     if not shutil.which("ffprobe"):
         QMessageBox.critical(None, "ffprobe not found", "ffprobe still not found, please download the full release or otherwise install ffmpeg.")
         sys.exit(1)
-    window = Ui_MainWindow()
+    window = Ui_MainWindow(app)
     window.show()
     sys.exit(app.exec())
```

### Comparing `kbp2video-0.1.4/kbp2video/advanced_editor.py` & `kbp2video-0.1.5/kbp2video/advanced_editor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.4/kbp2video/utils.py` & `kbp2video-0.1.5/kbp2video/utils.py`

 * *Files identical despite different names*

