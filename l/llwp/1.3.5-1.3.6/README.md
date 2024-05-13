# Comparing `tmp/llwp-1.3.5.tar.gz` & `tmp/llwp-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llwp-1.3.5.tar", last modified: Mon Oct  9 09:38:32 2023, max compression
+gzip compressed data, was "llwp-1.3.6.tar", last modified: Mon May 13 11:07:06 2024, max compression
```

## Comparing `llwp-1.3.5.tar` & `llwp-1.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-10-09 09:38:32.045113 llwp-1.3.5/
--rw-rw-rw-   0        0        0      832 2023-09-21 18:22:13.000000 llwp-1.3.5/LICENSE
--rw-rw-rw-   0        0        0       21 2023-09-21 18:22:13.000000 llwp-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1143 2023-10-09 09:38:32.045113 llwp-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-09-21 18:22:13.000000 llwp-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-10-09 09:38:32.029478 llwp-1.3.5/llwp/
--rw-rw-rw-   0        0        0   252988 2023-10-09 09:32:52.000000 llwp-1.3.5/llwp/LLWP.py
--rw-rw-rw-   0        0        0     1193 2023-09-21 18:22:13.000000 llwp-1.3.5/llwp/LLWP.svg
--rw-rw-rw-   0        0        0       20 2023-09-21 18:22:13.000000 llwp-1.3.5/llwp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-09 09:38:32.045113 llwp-1.3.5/llwp.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-10-09 09:38:31.000000 llwp-1.3.5/llwp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-10-09 09:38:32.000000 llwp-1.3.5/llwp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-09 09:38:31.000000 llwp-1.3.5/llwp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-10-09 09:38:32.000000 llwp-1.3.5/llwp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-10-09 09:38:32.000000 llwp-1.3.5/llwp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-10-09 09:38:32.000000 llwp-1.3.5/llwp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      807 2023-10-09 09:38:14.000000 llwp-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-09 09:38:32.045113 llwp-1.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 11:07:06.327287 llwp-1.3.6/
+-rw-rw-rw-   0        0        0      832 2023-09-21 18:22:13.000000 llwp-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-09-21 18:22:13.000000 llwp-1.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1143 2024-05-13 11:07:06.327287 llwp-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-09-21 18:22:13.000000 llwp-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 11:07:06.311661 llwp-1.3.6/llwp/
+-rw-rw-rw-   0        0        0   255108 2024-05-10 09:28:36.000000 llwp-1.3.6/llwp/LLWP.py
+-rw-rw-rw-   0        0        0     1193 2023-09-21 18:22:13.000000 llwp-1.3.6/llwp/LLWP.svg
+-rw-rw-rw-   0        0        0       20 2023-09-21 18:22:13.000000 llwp-1.3.6/llwp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:07:06.327287 llwp-1.3.6/llwp.egg-info/
+-rw-rw-rw-   0        0        0     1143 2024-05-13 11:07:06.000000 llwp-1.3.6/llwp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-13 11:07:06.000000 llwp-1.3.6/llwp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 11:07:06.000000 llwp-1.3.6/llwp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-13 11:07:06.000000 llwp-1.3.6/llwp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-13 11:07:06.000000 llwp-1.3.6/llwp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 11:07:06.000000 llwp-1.3.6/llwp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      807 2024-05-13 11:05:44.000000 llwp-1.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 11:07:06.327287 llwp-1.3.6/setup.cfg
```

### Comparing `llwp-1.3.5/LICENSE` & `llwp-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llwp-1.3.5/PKG-INFO` & `llwp-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llwp
-Version: 1.3.5
+Version: 1.3.6
 Summary: LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots.
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://llwp.astro.uni-koeln.de/
 Keywords: LLWP,Loomis-Wood Plots,Spectroscopy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `llwp-1.3.5/llwp/LLWP.py` & `llwp-1.3.6/llwp/LLWP.py`

 * *Files 1% similar despite different names*

```diff
@@ -1184,18 +1184,22 @@
 	def get_qns(self, transition, return_all=False):
 		nop = self.axs["ax"].shape[0]
 		noq = main.config["series_qns"]
 
 		qnus, qnls = np.array(transition["qnus"][:noq]), np.array(transition["qnls"][:noq])
 		diffs = np.array(transition["qndiffs"][:noq]) if transition["increase_freely"] else np.array(transition["qnincrs"][:noq])
 
+		# @Luis: Think about alternating signs
+		# alternating_signs = np.array([1, -1, 1, 1, 1, 1][:noq])
+
 		qns = []
 
 		for i in range(nop):
 			ind = nop-i-1
+			# upper, lower = (qnus+ind*diffs) * alternating_signs ** ind, (qnls+ind*diffs) * alternating_signs ** ind
 			upper, lower = qnus+ind*diffs, qnls+ind*diffs
 			qns.append((upper, lower))
 
 		if return_all:
 			return(qns, qnus, qnls, diffs)
 		else:
 			return(qns)
@@ -1209,17 +1213,18 @@
 
 		# Prefiltering cat_df (Similar to seriesfitwindow -> only one big query)
 		noq = main.config["series_qns"]
 
 		conditions = []
 		conditions_incr = []
 		for i, qnu, qnl, diff in zip(range(noq), qnus, qnls, diffs):
+			diff = int(diff)
 			if diff:
-				conditions_incr.append(f"(qnu{i+1} - {qnu})*{diff}")
-				conditions_incr.append(f"(qnl{i+1} - {qnl})*{diff}")
+				conditions_incr.append(f"((qnu{i+1} - {qnu})/{diff})")
+				conditions_incr.append(f"((qnl{i+1} - {qnl})/{diff})")
 			else:
 				conditions.append(f"(qnu{i+1} == {qnu})")
 				conditions.append(f"(qnl{i+1} == {qnl})")
 
 		if len(conditions_incr):
 			conditions.append(" == ".join(conditions_incr))
 
@@ -1410,46 +1415,61 @@
 
 	def fit_peak(self, xmin, xmax, index=None):
 		data = main.get_visible_data("exp", xrange=(xmin, xmax))
 		exp_xs = data["x"].to_numpy()
 		exp_ys = data["y"].to_numpy()
 		fit_xs = np.linspace(xmin, xmax, main.config["fit_xpoints"])
 
+		amplitude_direction = main.config["fit_amplitudedirection"]
 		fitfunction = main.config["fit_function"]
 		if len(exp_xs) < 2 and fitfunction != "Pgopher":
 			main.notification("<span style='color:#eda711;'>WARNING</span>: You did select less than two points of your spectrum, this fit will not work.")
 			raise CustomError("Too few points selected")
 
 		if self.fitline != None:
 			self.fitline.remove()
 			self.fitline = None
 		if self.fitcurve != None:
 			self.fitcurve.remove()
 			self.fitcurve = None
 
+		# @Luis: 
 		try:
 			if fitfunction == "Pgopher":
 				ymin, ymax = np.min(exp_ys), np.max(exp_ys)
-				cutoff = ymax - (ymax-ymin)/2
+				
+				if amplitude_direction < 0:
+					cutoff = ymin + (ymax-ymin)/2
+					mask = (exp_ys <= cutoff)
+				else:
+					cutoff = ymax - (ymax-ymin)/2
+					mask = (exp_ys >= cutoff)
 
-				mask = (exp_ys >= cutoff)
 				fit_xs = exp_xs[mask]
 				fit_ys = exp_ys[mask]
 
+				# @Luis: Check for the correct sign of exp_ys here
+
+				# @Luis: Check if average here should use relative fit_ys
+				# to correct for offsets in intensity
 				xmiddle = np.sum(fit_xs*fit_ys)/np.sum(fit_ys)
 				xuncert = 0
 			elif fitfunction == "Polynom":
 				try:
 					popt = np.polyfit(exp_xs, exp_ys, main.config["fit_polynomrank"])
 				except Exception as E:
 					popt = np.polyfit(exp_xs, exp_ys, main.config["fit_polynomrank"])
 				polynom = np.poly1d(popt)
 				fit_ys = polynom(fit_xs)
 
-				xmiddle = fit_xs[np.argmax(fit_ys)]
+				if amplitude_direction < 0:
+					xmiddle = fit_xs[np.argmin(fit_ys)]
+				else:
+					xmiddle = fit_xs[np.argmax(fit_ys)]
+				
 				xuncert = 0 # @Luis: Find real error for this part
 
 			elif fitfunction == "Polynom Autorank":
 				rms_best = np.inf
 				rank_best = 0
 
 				for rank in range(min((len(exp_ys), main.config["fit_polynommaxrank"]))):
@@ -1468,49 +1488,62 @@
 					except Exception as E:
 						continue
 
 				popt = np.polyfit(exp_xs, exp_ys, rank_best)
 				polynom = np.poly1d(popt)
 				fit_ys = polynom(fit_xs)
 
-				xmiddle = fit_xs[np.argmax(fit_ys)]
+				if amplitude_direction < 0:
+					xmiddle = fit_xs[np.argmin(fit_ys)]
+				else:
+					xmiddle = fit_xs[np.argmax(fit_ys)]
 				xuncert = 0 # @Luis: Find real error for this part
 
 			else:
 				x0 = (xmin+xmax)/2
 				ymin, ymax = np.min(exp_ys), np.max(exp_ys)
 				ymean = np.mean(exp_ys)
-				y0 = ymax-ymin
+				yptp = ymax-ymin
 				w0 = (xmax-xmin)
+				y0 = 0
+
+				amp_min, amp_max = -3*yptp, 3*yptp
+				if amplitude_direction < 0:
+					amp_max = 0
+					y0 = -yptp
+				if amplitude_direction > 0:
+					amp_min = 0
+					y0 = yptp
 
 				if main.config["fit_offset"]:
 					function, p0, bounds = {
-						"Gauss":					(lambda *x: lineshape("Gauss", 0, *x[:-1])+x[-1],   (x0, y0, w0, ymean),      ((xmin, 0, 0, ymin),    (xmax, 3*y0, 10*w0, ymax))),
-						"Lorentz":					(lambda *x: lineshape("Lorentz", 0, *x[:-1])+x[-1], (x0, y0, w0, ymean),      ((xmin, 0, 0, ymin),    (xmax, 3*y0, 10*w0, ymax))),
-						"Voigt":					(lambda *x: lineshape("Voigt", 0, *x[:-1])+x[-1],   (x0, y0, w0, w0, ymean),  ((xmin, 0, 0, 0, ymin), (xmax, 3*y0, 5*w0, 5*w0, ymax))),
-						"Gauss 1st Derivative":		(lambda *x: lineshape("Gauss", 1, *x[:-1])+x[-1],   (x0, y0, w0, ymean),      ((xmin, 0, 0, ymin),    (xmax, 3*y0, 10*w0, ymax))),
-						"Lorentz 1st Derivative":	(lambda *x: lineshape("Lorentz", 1, *x[:-1])+x[-1], (x0, y0, w0, ymean),      ((xmin, 0, 0, ymin),    (xmax, 3*y0, 10*w0, ymax))),
-						"Voigt 1st Derivative":		(lambda *x: lineshape("Voigt", 1, *x[:-1])+x[-1],   (x0, y0, w0, w0, ymean),  ((xmin, 0, 0, 0, ymin), (xmax, 3*y0, 5*w0, 5*w0, ymax))),
-						"Gauss 2nd Derivative":		(lambda *x: lineshape("Gauss", 2, *x[:-1])+x[-1],   (x0, y0, w0, ymean),      ((xmin, 0, 0, ymin),    (xmax, 3*y0, 10*w0, ymax))),
-						"Lorentz 2nd Derivative":	(lambda *x: lineshape("Lorentz", 2, *x[:-1])+x[-1], (x0, y0, w0, ymean),      ((xmin, 0, 0, ymin),    (xmax, 3*y0, 10*w0, ymax))),
-						"Voigt 2nd Derivative":		(lambda *x: lineshape("Voigt", 2, *x[:-1])+x[-1],   (x0, y0, w0, w0, ymean),  ((xmin, 0, 0, 0, ymin), (xmax, 3*y0, 5*w0, 5*w0, ymax))),
+						"Gauss":					(lambda *x: lineshape("Gauss", 0, *x[:-1])+x[-1],   (x0, y0, w0, ymean),      ((xmin, amp_min, 0, ymin),    (xmax, amp_max, 10*w0, ymax))),
+						"Lorentz":					(lambda *x: lineshape("Lorentz", 0, *x[:-1])+x[-1], (x0, y0, w0, ymean),      ((xmin, amp_min, 0, ymin),    (xmax, amp_max, 10*w0, ymax))),
+						"Voigt":					(lambda *x: lineshape("Voigt", 0, *x[:-1])+x[-1],   (x0, y0, w0, w0, ymean),  ((xmin, amp_min, 0, 0, ymin), (xmax, amp_max, 5*w0, 5*w0, ymax))),
+						"Gauss 1st Derivative":		(lambda *x: lineshape("Gauss", 1, *x[:-1])+x[-1],   (x0, y0, w0, ymean),      ((xmin, amp_min, 0, ymin),    (xmax, amp_max, 10*w0, ymax))),
+						"Lorentz 1st Derivative":	(lambda *x: lineshape("Lorentz", 1, *x[:-1])+x[-1], (x0, y0, w0, ymean),      ((xmin, amp_min, 0, ymin),    (xmax, amp_max, 10*w0, ymax))),
+						"Voigt 1st Derivative":		(lambda *x: lineshape("Voigt", 1, *x[:-1])+x[-1],   (x0, y0, w0, w0, ymean),  ((xmin, amp_min, 0, 0, ymin), (xmax, amp_max, 5*w0, 5*w0, ymax))),
+						"Gauss 2nd Derivative":		(lambda *x: lineshape("Gauss", 2, *x[:-1])+x[-1],   (x0, y0, w0, ymean),      ((xmin, amp_min, 0, ymin),    (xmax, amp_max, 10*w0, ymax))),
+						"Lorentz 2nd Derivative":	(lambda *x: lineshape("Lorentz", 2, *x[:-1])+x[-1], (x0, y0, w0, ymean),      ((xmin, amp_min, 0, ymin),    (xmax, amp_max, 10*w0, ymax))),
+						"Voigt 2nd Derivative":		(lambda *x: lineshape("Voigt", 2, *x[:-1])+x[-1],   (x0, y0, w0, w0, ymean),  ((xmin, amp_min, 0, 0, ymin), (xmax, amp_max, 5*w0, 5*w0, ymax))),
 					}.get(fitfunction)
 				else:
 					function, p0, bounds = {
-						"Gauss":					(lambda *x: lineshape("Gauss", 0, *x),   (x0, y0, w0),      ((xmin, 0, 0),    (xmax, 3*y0, 10*w0))),
-						"Lorentz":					(lambda *x: lineshape("Lorentz", 0, *x), (x0, y0, w0),      ((xmin, 0, 0),    (xmax, 3*y0, 10*w0))),
-						"Voigt":					(lambda *x: lineshape("Voigt", 0, *x),   (x0, y0, w0, w0),  ((xmin, 0, 0, 0), (xmax, 3*y0, 5*w0, 5*w0))),
-						"Gauss 1st Derivative":		(lambda *x: lineshape("Gauss", 1, *x),   (x0, y0, w0),      ((xmin, 0, 0),    (xmax, 3*y0, 10*w0))),
-						"Lorentz 1st Derivative":	(lambda *x: lineshape("Lorentz", 1, *x), (x0, y0, w0),      ((xmin, 0, 0),    (xmax, 3*y0, 10*w0))),
-						"Voigt 1st Derivative":		(lambda *x: lineshape("Voigt", 1, *x),   (x0, y0, w0, w0),  ((xmin, 0, 0, 0), (xmax, 3*y0, 5*w0, 5*w0))),
-						"Gauss 2nd Derivative":		(lambda *x: lineshape("Gauss", 2, *x),   (x0, y0, w0),      ((xmin, 0, 0),    (xmax, 3*y0, 10*w0))),
-						"Lorentz 2nd Derivative":	(lambda *x: lineshape("Lorentz", 2, *x), (x0, y0, w0),      ((xmin, 0, 0),    (xmax, 3*y0, 10*w0))),
-						"Voigt 2nd Derivative":		(lambda *x: lineshape("Voigt", 2, *x),   (x0, y0, w0, w0),  ((xmin, 0, 0, 0), (xmax, 3*y0, 5*w0, 5*w0))),
+						"Gauss":					(lambda *x: lineshape("Gauss", 0, *x),   (x0, y0, w0),      ((xmin, amp_min, 0),    (xmax, amp_max, 10*w0))),
+						"Lorentz":					(lambda *x: lineshape("Lorentz", 0, *x), (x0, y0, w0),      ((xmin, amp_min, 0),    (xmax, amp_max, 10*w0))),
+						"Voigt":					(lambda *x: lineshape("Voigt", 0, *x),   (x0, y0, w0, w0),  ((xmin, amp_min, 0, 0), (xmax, amp_max, 5*w0, 5*w0))),
+						"Gauss 1st Derivative":		(lambda *x: lineshape("Gauss", 1, *x),   (x0, y0, w0),      ((xmin, amp_min, 0),    (xmax, amp_max, 10*w0))),
+						"Lorentz 1st Derivative":	(lambda *x: lineshape("Lorentz", 1, *x), (x0, y0, w0),      ((xmin, amp_min, 0),    (xmax, amp_max, 10*w0))),
+						"Voigt 1st Derivative":		(lambda *x: lineshape("Voigt", 1, *x),   (x0, y0, w0, w0),  ((xmin, amp_min, 0, 0), (xmax, amp_max, 5*w0, 5*w0))),
+						"Gauss 2nd Derivative":		(lambda *x: lineshape("Gauss", 2, *x),   (x0, y0, w0),      ((xmin, amp_min, 0),    (xmax, amp_max, 10*w0))),
+						"Lorentz 2nd Derivative":	(lambda *x: lineshape("Lorentz", 2, *x), (x0, y0, w0),      ((xmin, amp_min, 0),    (xmax, amp_max, 10*w0))),
+						"Voigt 2nd Derivative":		(lambda *x: lineshape("Voigt", 2, *x),   (x0, y0, w0, w0),  ((xmin, amp_min, 0, 0), (xmax, amp_max, 5*w0, 5*w0))),
 					}.get(fitfunction)
 
+
 				try:
 					popt, pcov = optimize.curve_fit(function, exp_xs, exp_ys, p0=p0, bounds=bounds)
 				except Exception as E:
 					popt, pcov = optimize.curve_fit(function, exp_xs, exp_ys, p0=p0, bounds=bounds)
 				perr = np.sqrt(np.diag(pcov))
 				fit_ys = function(fit_xs, *popt)
 
@@ -2643,14 +2676,15 @@
 				try:
 					main.signalclass.fitindicator.emit("<span style='color:#eda711;'>Working ...</span>")
 					peaks = self.parent.peaks.copy()
 					profile = main.config["blendedlineswindow_lineshape"]
 					derivative = main.config["blendedlineswindow_derivative"]
 					polynomrank = main.config["blendedlineswindow_polynom"]+1
 					fixedwidth = main.config["blendedlineswindow_fixedwidth"]
+					amplitude_direction = main.config["fit_amplitudedirection"]
 					now = 2 if profile == "Voigt" else 1
 					noa = 2 + now * (not fixedwidth)
 
 					fitfunction = lambda x, *args, fixedwidth=fixedwidth: self.parent.fitfunction(x, profile, derivative, polynomrank, *args, fixedwidth=fixedwidth)
 					fitfunction_withoutbaseline = lambda x, *args, fixedwidth=fixedwidth: self.parent.fitfunction(x, profile, derivative, 0, *args, fixedwidth=fixedwidth)
 
 					for part in self.plot_parts:
@@ -2684,33 +2718,37 @@
 					xs = []
 					ys = []
 					ws = []
 					exp_mean = 0
 					if len(exp_ys) and (polynomrank + len(peaks)):
 						if main.config["blendedlineswindow_autopositionpeaks"]:
 							exp_mean = exp_ys.mean()
-						p0 = []
-						bounds = [[],[]]
 
-						y0 = 4*(np.amax(exp_ys)-np.amin(exp_ys))
+						yptp = 4*(np.amax(exp_ys)-np.amin(exp_ys))
 						w0 = xrange[1] - xrange[0]
 						wmax = main.config["blendedlineswindow_maxfwhm"] or w0
+						amp_min, amp_max = -3*yptp, 3*yptp
+						if amplitude_direction < 0:
+							amp_max = 0
+						if amplitude_direction > 0:
+							amp_min = 0
+						
 						for peak in peaks:
 							x, y, x_rel = peak
 
 							if not xrange[0] < x < xrange[1]:
 								x = self.center + x_rel
 								if not xrange[0] < x < xrange[1]:
 									x = sum(xrange)/2
-								y = y0/2
-							elif not 0 < y < y0:
-								y = y0/2
+								y = yptp * np.sign(amplitude_direction)
+							elif not amp_min < y < amp_max:
+								y = yptp * np.sign(amplitude_direction)
 
 							xs.append((x, *xrange))
-							ys.append((y, 0, y0))
+							ys.append((y, amp_min, amp_max))
 							ws.append((wmax/4, 0, wmax))
 
 						p0 = []
 						bounds = [[], []]
 						for x, y, w in zip(xs, ys, ws):
 							tmp_p0 = [z[0] for z in (x, y, w, w)]
 							tmp_b0 = [z[1] for z in (x, y, w, w)]
@@ -2734,14 +2772,15 @@
 							bounds[0].extend([wl]*now)
 							bounds[1].extend([wu]*now)
 
 						p0.extend([0]*polynomrank)
 						bounds[0].extend([-np.inf]*polynomrank)
 						bounds[1].extend([+np.inf]*polynomrank)
 
+						# @Luis: Work on the bounds and p0s here
 						try:
 							popt, pcov = optimize.curve_fit(fitfunction, exp_xs, exp_ys, p0=p0, bounds=bounds)
 						except Exception as E:
 							popt, pcov = optimize.curve_fit(fitfunction, exp_xs, exp_ys, p0=p0, bounds=bounds)
 						perr = np.sqrt(np.diag(pcov))
 						res_xs = np.linspace(xrange[0], xrange[1], main.config["blendedlineswindow_xpoints"])
 						res_ys = fitfunction(res_xs, *popt)
@@ -3158,14 +3197,24 @@
 		super().__init__(id, parent)
 		self.setWindowTitle("Assign Blend")
 
 		self.init_gui()
 		self.update_gui(entries, dict_, index)
 
 	def update_gui(self, entries, dict_, index):
+		tmp_cat = main.get_visible_data("cat", (dict_["xpre"], dict_["xpre"]))
+		qn_labels = [f"qn{ul}{i+1}" for ul in "ul" for i in range(6)]
+		query = " and ".join([f"( {label} == {dict_[label]} )" for label in qn_labels if label in dict_])
+		tmp_cat = tmp_cat.query(query)
+		y_at_xpre = tmp_cat["y"].values[0]
+
+		if main.config["series_blendminrelratio"] > 0:
+			min_y_value = y_at_xpre * main.config["series_blendminrelratio"]
+			entries = entries.query("y >= @min_y_value")
+
 		self.noq = main.config["series_qns"]
 		self.entries = entries.reset_index(drop=True)
 		self.xmiddle = dict_["x"]
 		self.index = index
 		self.error = dict_["error"]
 
 		self.label.setText(f"Assigning Blend for position {self.xmiddle}.")
@@ -4879,17 +4928,18 @@
 			cat_df = main.get_visible_data("cat", scale=False)
 			
 			if main.config["calibratewindow_queryexp"].strip():
 				exp_df = exp_df.query(main.config["calibratewindow_queryexp"])
 			if main.config["calibratewindow_querycat"].strip():
 				cat_df = cat_df.query(main.config["calibratewindow_querycat"])
 			
+			lineshape_type = main.config["calibratewindow_lineshape"]
 			blendwidth = main.config["calibratewindow_blendwidth"] / 2
 			fitwidth = main.config["calibratewindow_fitwidth"] / 2
-			fitfunction = lambda *args: lineshape(main.config["calibratewindow_lineshape"], main.config["calibratewindow_derivative"], *args[:-1]) + args[-1]
+			fitfunction = lambda *args: lineshape(lineshape_type, main.config["calibratewindow_derivative"], *args[:-1]) + args[-1]
 			
 			xs = cat_df["x"].to_numpy()
 			
 			i_starts_exp, i_stops_exp = exp_df["x"].searchsorted(xs - fitwidth, side="left"), exp_df["x"].searchsorted(xs + fitwidth, side="right")
 			i_starts_cat, i_stops_cat = cat_df["x"].searchsorted(xs - blendwidth, side="left"), cat_df["x"].searchsorted(xs + blendwidth, side="right")
 			
 			calibration_points = []
@@ -4909,14 +4959,20 @@
 				ymax = ys.max()
 				p0 = [x0, ymax, fitwidth/10, fitwidth/10, 0]
 				bounds = [
 					[x0-0.2, 0, 0, 0, 0],
 					[x0+0.2, 2*ymax, fitwidth/2.5, fitwidth/2.5, ymax/2],
 				]
 				
+				if lineshape_type != "Voigt":
+					del p0[2]
+					del bounds[0][2]
+					del bounds[1][2]
+				
+				
 				popt, pcov = optimize.curve_fit(fitfunction, xs, ys, p0=p0, bounds=bounds)
 				calibration_points.append((popt[0], y0/popt[1]))
 				
 				# @Luis: Perform checks to see if fit was sensible
 					
 			if not len(calibration_points):
 				calibration_points = np.array([[], []])
@@ -4934,19 +4990,19 @@
 			exp_df["y_old"] = exp_df["y"]
 			exp_df["y"] *= factors
 			exp_df["y"] /= exp_df["y"].max()
 			exp_df["factors"] = factors
 			
 			main.notification(f"Used {len(calibration_points)} of {len(cat_df)} predictions for calibration.")
 			
+			self.calibration_points = calibration_points
+			self.cal_df = exp_df
 		except Exception as E:
 			raise
 		finally:
-			self.calibration_points = calibration_points
-			self.cal_df = exp_df
 			main.signalclass.calibrationend.emit()
 	
 	def after_calibration(self):
 		self.run_button.setEnabled(True)
 		self.update_plot()
 
 	def save(self):
@@ -5297,15 +5353,15 @@
 		elif temp:
 			line, ok = QInputDialog().getMultiLineText(self, "Specify Custom List",
 			"Write list here (delimiters are all whitespace characters, comma and semicolon):")
 			if not ok or not line:
 				return
 
 			xs = []
-			tmp_xs = re.split('; |, |\s', line)
+			tmp_xs = re.split(r'; |, |\s', line)
 			for x in tmp_xs:
 				if not x.strip():
 					continue
 				try:
 					xs.append(float(x))
 				except ValueError:
 					main.notification(f"<span style='color:#eda711;'>WARNING</span>: Could not convert the string '{x}' to a numerical value.")
@@ -5324,15 +5380,15 @@
 			for fname in fnames:
 				with open(fname, "r", encoding="utf-8") as file:
 					for line in file:
 						line = line.strip()
 						if line == "" or line.startswith("#"):
 							continue
 
-						tmp = re.split('; |, |\s', line)
+						tmp = re.split(r'; |, |\s', line)
 						for x in tmp:
 							try:
 								xs.append(float(x))
 							except ValueError:
 								main.notification(f"<span style='color:#eda711;'>WARNING</span>: Could not convert the string '{x}' to a numerical value.")
 
 			self.state["list"].update({
@@ -5367,16 +5423,16 @@
 		self.parent = parent
 		if initial_values:
 			self.state.update(initial_values)
 
 		layout = QGridLayout()
 
 		self.labels  = [QQ(QLabel, text=f"QN {x+1}") for x in range(6)]
-		self.qnus    = [QQ(QSpinBox, minWidth=40, maxWidth=60, range=(0, None), singlestep=1, change=lambda x: self.changed()) for x in range(6)]
-		self.qnls    = [QQ(QSpinBox, minWidth=40, maxWidth=60, range=(0, None), singlestep=1, change=lambda x: self.changed()) for x in range(6)]
+		self.qnus    = [QQ(QSpinBox, minWidth=40, maxWidth=60, range=(None, None), singlestep=1, change=lambda x: self.changed()) for x in range(6)]
+		self.qnls    = [QQ(QSpinBox, minWidth=40, maxWidth=60, range=(None, None), singlestep=1, change=lambda x: self.changed()) for x in range(6)]
 		self.qnincrs = [QQ(QCheckBox, text="Incr", minWidth=40, maxWidth=60, change=lambda x: self.changed()) for x in range(6)]
 		self.qndiffs = [QQ(QSpinBox, minWidth=40, maxWidth=60, range=(None, None), singlestep=1, change=lambda x: self.changed()) for x in range(6)]
 
 		self.incqns = QQ(QPushButton, text="Increase", change=lambda x: self.incdecqns(+1))
 		self.decqns = QQ(QPushButton, text="Decrease", change=lambda x: self.incdecqns(-1))
 
 		self.incnoq = QQ(QPushButton, text="QN+", change=lambda x: self.alternoq(+1))
@@ -6770,14 +6826,15 @@
 	"fit_polynomrank":						[5, int],
 	"fit_polynommaxrank":					[20, int],
 	"fit_uncertaintystep":					[0.01, float],
 	"fit_xpoints":							[1000, int],
 	"fit_offset":							[True, bool],
 	"fit_comment":							["", str],
 	"fit_clipboard":						[True, bool],
+	"fit_amplitudedirection":				[1, int],
 
 	"plot_dpi":								[100, float],
 	"plot_annotations_dict":				[{"x": 1, "y": 1, "horizontalalignment": "right", "verticalalignment": "top"}, dict],
 	"plot_font_dict":						[{"size":10}, dict],
 	"plot_matplotlibkwargs":				[{"hspace": 0, "wspace": 0}, dict],
 	"plot_coupled":							[True, bool],
 	"plot_ymargin":							[0.1, float],
@@ -6799,14 +6856,15 @@
 	"plot_expasstickspectrum":				[False, bool],
 	"plot_relativegoto":					[False, bool],
 
 	"series_qns":							[3, int],
 	"series_annotate_xs":					[False, bool],
 	"series_annotate_fmt":					[".4f", str],
 	"series_blendwidth":					[1, float],
+	"series_blendminrelratio":				[0, float],
 	"series_blenddialog":					[True, bool],
 	"series_currenttab":					[1, int],
 	"series_references":					[[], list],
 
 	"flag_automatic_draw":					[True, bool],
 	"flag_appendonsave":					[True, bool],
 	"flag_hidecatalog":						[False, bool],
```

### Comparing `llwp-1.3.5/llwp/LLWP.svg` & `llwp-1.3.6/llwp/LLWP.svg`

 * *Files identical despite different names*

### Comparing `llwp-1.3.5/llwp.egg-info/PKG-INFO` & `llwp-1.3.6/llwp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llwp
-Version: 1.3.5
+Version: 1.3.6
 Summary: LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots.
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://llwp.astro.uni-koeln.de/
 Keywords: LLWP,Loomis-Wood Plots,Spectroscopy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `llwp-1.3.5/pyproject.toml` & `llwp-1.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llwp"
-version = "1.3.5"
+version = "1.3.6"
 authors = [
   { name="Luis Bonah", email="bonah@ph1.uni-koeln.de" },
 ]
 description = "LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['numpy', 'pandas', 'matplotlib', 'wrapt', 'pyckett', 'scipy', 'PyQt6']
```

