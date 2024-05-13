# Comparing `tmp/specpolflow-0.4.0.tar.gz` & `tmp/specpolflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specpolflow-0.4.0.tar", last modified: Sun May 12 00:33:33 2024, max compression
+gzip compressed data, was "specpolflow-0.4.1.tar", last modified: Mon May 13 17:02:25 2024, max compression
```

## Comparing `specpolflow-0.4.0.tar` & `specpolflow-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/
--rw-rw-r--   0 colin     (1000) colin     (1000)    18092 2022-06-10 18:49:06.000000 specpolflow-0.4.0/LICENSE
--rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-05-12 00:33:33.866972 specpolflow-0.4.0/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)     2491 2024-04-13 03:59:50.000000 specpolflow-0.4.0/README.md
--rw-rw-r--   0 colin     (1000) colin     (1000)     1607 2024-05-11 17:51:30.000000 specpolflow-0.4.0/pyproject.toml
--rw-rw-r--   0 colin     (1000) colin     (1000)       38 2024-05-12 00:33:33.866972 specpolflow-0.4.0/setup.cfg
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow/
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow/CommandLine/
--rw-rw-r--   0 colin     (1000) colin     (1000)        0 2024-03-13 20:56:33.000000 specpolflow-0.4.0/specpolFlow/CommandLine/__init__.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     4650 2024-03-15 22:20:13.000000 specpolflow-0.4.0/specpolFlow/CommandLine/bz.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     2343 2024-05-11 04:23:30.000000 specpolflow-0.4.0/specpolFlow/CommandLine/cleanMaskUI.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     3170 2024-05-11 18:22:22.000000 specpolflow-0.4.0/specpolFlow/CommandLine/makeMask.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     1820 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/CommandLine/plotLSD.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     2093 2024-03-15 22:20:52.000000 specpolflow-0.4.0/specpolFlow/CommandLine/rvFit.py
--rw-rw-r--   0 colin     (1000) colin     (1000)      179 2024-05-11 17:51:42.000000 specpolflow-0.4.0/specpolFlow/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     6048 2024-05-11 05:01:55.000000 specpolflow-0.4.0/specpolFlow/cleanMaskUI.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    58136 2024-05-11 04:58:30.000000 specpolflow-0.4.0/specpolFlow/cleanMaskUISubroutines.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow/converters/
--rw-rw-r--   0 colin     (1000) colin     (1000)       23 2023-10-24 00:52:17.000000 specpolflow-0.4.0/specpolFlow/converters/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     7530 2023-05-25 16:03:53.000000 specpolflow-0.4.0/specpolFlow/converters/convert-spirou-fits-s0.2.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     6293 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/converters/espadons.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    26719 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/lineList.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    24221 2024-05-11 18:18:52.000000 specpolflow-0.4.0/specpolFlow/mask.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    22255 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/obsSpec.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    46978 2024-05-11 23:55:29.000000 specpolflow-0.4.0/specpolFlow/profileLSD.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow.egg-info/
--rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)      756 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/SOURCES.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        1 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/dependency_links.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)      361 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/entry_points.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       54 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/requires.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       12 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/top_level.txt
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-13 17:02:25.249213 specpolflow-0.4.1/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    18092 2022-06-10 18:49:06.000000 specpolflow-0.4.1/LICENSE
+-rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-05-13 17:02:25.249213 specpolflow-0.4.1/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2491 2024-04-13 03:59:50.000000 specpolflow-0.4.1/README.md
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1607 2024-05-13 17:01:13.000000 specpolflow-0.4.1/pyproject.toml
+-rw-rw-r--   0 colin     (1000) colin     (1000)       38 2024-05-13 17:02:25.249213 specpolflow-0.4.1/setup.cfg
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-13 17:02:25.249213 specpolflow-0.4.1/specpolFlow/
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-13 17:02:25.249213 specpolflow-0.4.1/specpolFlow/CommandLine/
+-rw-rw-r--   0 colin     (1000) colin     (1000)        0 2024-03-13 20:56:33.000000 specpolflow-0.4.1/specpolFlow/CommandLine/__init__.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     4650 2024-03-15 22:20:13.000000 specpolflow-0.4.1/specpolFlow/CommandLine/bz.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     2343 2024-05-11 04:23:30.000000 specpolflow-0.4.1/specpolFlow/CommandLine/cleanMaskUI.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     3170 2024-05-11 18:22:22.000000 specpolflow-0.4.1/specpolFlow/CommandLine/makeMask.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     1820 2024-05-10 20:30:57.000000 specpolflow-0.4.1/specpolFlow/CommandLine/plotLSD.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     2093 2024-03-15 22:20:52.000000 specpolflow-0.4.1/specpolFlow/CommandLine/rvFit.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)      179 2024-05-13 17:01:26.000000 specpolflow-0.4.1/specpolFlow/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6055 2024-05-13 16:57:39.000000 specpolflow-0.4.1/specpolFlow/cleanMaskUI.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    58392 2024-05-13 16:58:24.000000 specpolflow-0.4.1/specpolFlow/cleanMaskUISubroutines.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-13 17:02:25.249213 specpolflow-0.4.1/specpolFlow/converters/
+-rw-rw-r--   0 colin     (1000) colin     (1000)       23 2023-10-24 00:52:17.000000 specpolflow-0.4.1/specpolFlow/converters/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     7530 2023-05-25 16:03:53.000000 specpolflow-0.4.1/specpolFlow/converters/convert-spirou-fits-s0.2.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6293 2024-05-10 20:30:57.000000 specpolflow-0.4.1/specpolFlow/converters/espadons.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    26719 2024-05-10 20:30:57.000000 specpolflow-0.4.1/specpolFlow/lineList.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    24221 2024-05-11 18:18:52.000000 specpolflow-0.4.1/specpolFlow/mask.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    22255 2024-05-10 20:30:57.000000 specpolflow-0.4.1/specpolFlow/obsSpec.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    46978 2024-05-11 23:55:29.000000 specpolflow-0.4.1/specpolFlow/profileLSD.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-13 17:02:25.249213 specpolflow-0.4.1/specpolFlow.egg-info/
+-rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-05-13 17:02:25.000000 specpolflow-0.4.1/specpolFlow.egg-info/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)      756 2024-05-13 17:02:25.000000 specpolflow-0.4.1/specpolFlow.egg-info/SOURCES.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        1 2024-05-13 17:02:25.000000 specpolflow-0.4.1/specpolFlow.egg-info/dependency_links.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)      361 2024-05-13 17:02:25.000000 specpolflow-0.4.1/specpolFlow.egg-info/entry_points.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       54 2024-05-13 17:02:25.000000 specpolflow-0.4.1/specpolFlow.egg-info/requires.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       12 2024-05-13 17:02:25.000000 specpolflow-0.4.1/specpolFlow.egg-info/top_level.txt
```

### Comparing `specpolflow-0.4.0/LICENSE` & `specpolflow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/PKG-INFO` & `specpolflow-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specpolFlow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for the analysis of stellar spectropolarimetric data
 Author-email: SpecpolFlow Team <specpolflow@gmail.com>
 Project-URL: Homepage, https://github.com/folsomcp/specpolFlow
 Project-URL: Documentation, https://folsomcp.github.io/specpolFlow/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `specpolflow-0.4.0/README.md` & `specpolflow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/pyproject.toml` & `specpolflow-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 #where = ["src"]  # ["."] by default
 include = ["specpolFlow*"]  # ["*"] by default
 
 [project]
 name = "specpolFlow"
-version = "0.4.0"
+version = "0.4.1"
 authors = [ {name="SpecpolFlow Team", email="specpolflow@gmail.com"},
 ]
 description = "Tools for the analysis of stellar spectropolarimetric data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `specpolflow-0.4.0/specpolFlow/CommandLine/bz.py` & `specpolflow-0.4.1/specpolFlow/CommandLine/bz.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/CommandLine/cleanMaskUI.py` & `specpolflow-0.4.1/specpolFlow/CommandLine/cleanMaskUI.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/CommandLine/makeMask.py` & `specpolflow-0.4.1/specpolFlow/CommandLine/makeMask.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/CommandLine/plotLSD.py` & `specpolflow-0.4.1/specpolFlow/CommandLine/plotLSD.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/CommandLine/rvFit.py` & `specpolflow-0.4.1/specpolFlow/CommandLine/rvFit.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/cleanMaskUI.py` & `specpolflow-0.4.1/specpolFlow/cleanMaskUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
         ax1.set_xlabel('Wavelength')
         ax1.set_ylabel('Flux')
 
         #initialize an array of flags for fitting LSD line depths
         fitDepthFlags = np.zeros_like(mask.wl, dtype=int)
         
         #Run the main interactive program
-        cleanSub.makeWin(fig, ax1, mask, obs, lsdp, pltMaskU, 
-                         pltMaskN, pltMaskF, pltModelI, excludeRanges, 
+        cleanSub.makeWin(fig, ax1, mask, obs, lsdp, lsdProf, pltMaskU,
+                         pltMaskN, pltMaskF, pltModelI, excludeRanges,
                          outExcludeName, fitDepthFlags)
 
     #make an ExcludeMaskRegions object to return
     wlStarts = np.array([ran[0] for ran in excludeRanges])
     wlEnds = np.array([ran[1] for ran in excludeRanges])
     labels = np.array(['cleanMaskUI']*len(excludeRanges),dtype=object)
     regions = maskTools.ExcludeMaskRegions(wlStarts, wlEnds, labels)
```

### Comparing `specpolflow-0.4.0/specpolFlow/cleanMaskUISubroutines.py` & `specpolflow-0.4.1/specpolFlow/cleanMaskUISubroutines.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     except ImportError: #if that fails, just don't use this extra toolbar
         _mplToolbar=0
 
 from . import profileLSD
 from . import mask as maskTools
 from . import obsSpec
 
-def makeWin(fig, ax, mask, obs, lsdp, pltMaskU, pltMaskN,
+def makeWin(fig, ax, mask, obs, lsdp, lsdProf, pltMaskU, pltMaskN,
             pltMaskF, pltModelI, excludeRanges, outExcludeName, fitDepthFlags):
     #Build GUI with tkinter
     root = tk.Tk(className='Clean Masks')
     #the className seems to set an icon title (at least in Ubuntu)
     root.title("Clean Masks")
 
     ##For an icon image (used by window managers)
@@ -143,16 +143,16 @@
                              command=unselectFitDepth.runSpanSelect)
     ToolTip(butUnselRange, 'Unselect lines to fit for depth in the mask')
     butUnselRange.grid(row=0, column=1, sticky=tk.W, padx=2, pady=2)
     #Link the select and unselect buttons so they can turn each other off
     selectFitDepth.linkButton(butSelRange, unselectFitDepth)
     unselectFitDepth.linkButton(butUnselRange, selectFitDepth)
     #Apply the depth fitting
-    fitDepthsM = fitDepths(mask, obs, lsdp, fitDepthFlags, root, canvas,
-                           pltMaskU, pltMaskN, pltMaskF)
+    fitDepthsM = fitDepths(mask, obs, lsdp, lsdProf, fitDepthFlags, root,
+                           canvas, pltMaskU, pltMaskN, pltMaskF)
     butFitDepths = ttk.Button(master=tools, text='fit\ndepths',
                                command=fitDepthsM.runFit)
     ToolTip(butFitDepths, 'Fit the selected line depths, using the current LSD profile and observation')
     butFitDepths.grid(row=0, column=3, sticky=tk.W, padx=2, pady=2)
     #Undo the depth fitting
     undoDepthsM = undoDepths(mask, fitDepthFlags, canvas,
                              pltMaskU, pltMaskN, pltMaskF)
@@ -192,15 +192,15 @@
     modifyLSDparM = modifyLSDpar(root, lsdp)
     butModLSD = ttk.Button(master=tools, text='LSD param.',
                               command=modifyLSDparM.openWindow)
     ToolTip(butModLSD, 'Modify the parameters related to the LSD calculation')
     butModLSD.grid(row=3, column=8, sticky=tk.E, padx=2)
     
     #Update the LSD calculation and the plotted spectrum
-    updateLSDM = updateLSD(canvas, root, mask, lsdp, pltModelI)
+    updateLSDM = updateLSD(canvas, root, mask, lsdp, lsdProf, pltModelI)
     butUpdateLSD = ttk.Button(master=tools, text='update LSD',
                               command=updateLSDM.rerunLSD)
     ToolTip(butUpdateLSD, 'Save the mask, run LSD, and update the model spectrum')
     butUpdateLSD.grid(row=3, column=9, sticky=(tk.N, tk.S, tk.E, tk.W), padx=2)
     
     #Run the main loop!
     root.mainloop()
@@ -744,19 +744,20 @@
         #Save the set of exclude ranges to a file
         regions.save(self.fname)
         return
 
 
 class fitDepths:
     #mini manager to run the fitting of line depths
-    def __init__(self, mask, obs, lsdp, fitDepthFlags, root, canvas,
-                 pltMaskU, pltMaskN, pltMaskF):
+    def __init__(self, mask, obs, lsdp, lsdProf, fitDepthFlags, root,
+                 canvas, pltMaskU, pltMaskN, pltMaskF):
         self.mask = mask
         self.obs = obs
         self.lsdp = lsdp
+        self.lsdProf = lsdProf
         self.fitDepthFlags = fitDepthFlags
         self.root = root
         self.canvas = canvas
         self.pltMaskU = pltMaskU
         self.pltMaskN = pltMaskN
         self.pltMaskF = pltMaskF
         
@@ -772,15 +773,15 @@
         self.root.update()
 
         #Get the lines that are flagged to be fit (and used)
         indUse1 = np.nonzero((self.fitDepthFlags == 1) & (self.mask.iuse == 1))
         useMask1 = self.mask[indUse1]
         if len(useMask1) > 0:
             #Get the reference LSD profile
-            prof = profileLSD.read_lsd(self.lsdp.outName) 
+            prof = self.lsdProf
             #Remove degenerate (or nearly) lines
             pixVel = prof.vel[1]-prof.vel[0]
             removePoorLines(useMask1, pixVel, fracPix = 3.0, sumDepths=False)
             self.mask.iuse[indUse1] = useMask1.iuse
             #and save the good lines in the mask for fitting
             indUse2 = np.nonzero(useMask1.iuse == 1)
             useMask2 = useMask1[indUse2]
@@ -1137,19 +1138,20 @@
             self.lsdp.plotLSD = False
         else:
             self.lsdp.plotLSD = True
         return
 
 
 class updateLSD:
-    def __init__(self, canvas, root, mask, lsdp, pltModelI):
+    def __init__(self, canvas, root, mask, lsdp, lsdProf, pltModelI):
         self.canvas = canvas
         self.root = root
         self.mask = mask
         self.lsdp = lsdp
+        self.lsdProf = lsdProf
         self.pltModelI = pltModelI
     def rerunLSD(self):
         #Recalculate the LSD profile and update the plot
         #First set a 'wait' cursor
         oldCursor = self.root.cget('cursor')
         self.root.config(cursor='watch')
         self.root.update()
@@ -1160,14 +1162,17 @@
             outLSDName=lsdp.outName, velStart=lsdp.velStart, velEnd=lsdp.velEnd,
             velPixel=lsdp.velPixel, normDepth=lsdp.normDepth,
             normLande=lsdp.normLande, normWave=lsdp.normWave,
             removeContPol=lsdp.removeContPol, trimMask=lsdp.trimMask,
             sigmaClipIter=lsdp.sigmaClipIter, sigmaClip=lsdp.sigmaClip,
             outModelName=lsdp.outModelName,
             plotLSD=lsdp.plotLSD, outPlotLSDName=lsdp.outPlotLSDName)
+        #update the current LSD object, rather than replacing it
+        #(since fitDepths needs to retain a reference to the same object)
+        self.lsdProf[:] = lsdProf[:]
         #Return the cursor to normal
         self.root.config(cursor=oldCursor)
         
         #re-draw points used in the fit
         for dline in self.pltModelI:
             dline.set_data(modelSpec.wl, modelSpec.specI)
         self.canvas.draw()
```

### Comparing `specpolflow-0.4.0/specpolFlow/converters/convert-spirou-fits-s0.2.py` & `specpolflow-0.4.1/specpolFlow/converters/convert-spirou-fits-s0.2.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/converters/espadons.py` & `specpolflow-0.4.1/specpolFlow/converters/espadons.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/lineList.py` & `specpolflow-0.4.1/specpolFlow/lineList.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/mask.py` & `specpolflow-0.4.1/specpolFlow/mask.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/obsSpec.py` & `specpolflow-0.4.1/specpolFlow/obsSpec.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow/profileLSD.py` & `specpolflow-0.4.1/specpolFlow/profileLSD.py`

 * *Files identical despite different names*

### Comparing `specpolflow-0.4.0/specpolFlow.egg-info/PKG-INFO` & `specpolflow-0.4.1/specpolFlow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specpolFlow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for the analysis of stellar spectropolarimetric data
 Author-email: SpecpolFlow Team <specpolflow@gmail.com>
 Project-URL: Homepage, https://github.com/folsomcp/specpolFlow
 Project-URL: Documentation, https://folsomcp.github.io/specpolFlow/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `specpolflow-0.4.0/specpolFlow.egg-info/SOURCES.txt` & `specpolflow-0.4.1/specpolFlow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

