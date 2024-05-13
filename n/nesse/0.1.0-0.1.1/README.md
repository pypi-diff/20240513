# Comparing `tmp/nesse-0.1.0.tar.gz` & `tmp/nesse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nesse-0.1.0.tar", last modified: Thu Dec 14 19:13:12 2023, max compression
+gzip compressed data, was "nesse-0.1.1.tar", last modified: Mon May 13 19:11:01 2024, max compression
```

## Comparing `nesse-0.1.0.tar` & `nesse-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-12-14 19:13:12.771632 nesse-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-03-24 17:59:44.000000 nesse-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       30 2023-03-24 17:59:44.000000 nesse-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1654 2023-12-14 19:13:12.769623 nesse-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-12-14 18:42:27.000000 nesse-0.1.0/README.md
--rw-rw-rw-   0        0        0      955 2023-12-14 19:12:44.000000 nesse-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-14 19:13:12.771632 nesse-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-12-14 19:13:12.722507 nesse-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-12-14 19:13:12.745548 nesse-0.1.0/src/nesse/
--rw-rw-rw-   0        0        0      147 2023-03-24 17:59:45.000000 nesse-0.1.0/src/nesse/__init__.py
--rw-rw-rw-   0        0        0     2855 2023-12-14 18:42:27.000000 nesse-0.1.0/src/nesse/charge_propagation.py
--rw-rw-rw-   0        0        0      880 2023-03-24 17:59:45.000000 nesse-0.1.0/src/nesse/constants.py
--rw-rw-rw-   0        0        0     7551 2023-12-14 18:42:27.000000 nesse-0.1.0/src/nesse/event.py
--rw-rw-rw-   0        0        0     7716 2023-12-14 18:42:27.000000 nesse-0.1.0/src/nesse/field.py
--rw-rw-rw-   0        0        0     1160 2023-03-24 18:56:31.000000 nesse-0.1.0/src/nesse/interp.pyx
--rw-rw-rw-   0        0        0     2803 2023-03-24 17:59:45.000000 nesse-0.1.0/src/nesse/interp_3d.py
--rw-rw-rw-   0        0        0     2066 2023-12-14 18:42:27.000000 nesse-0.1.0/src/nesse/mobility.py
--rw-rw-rw-   0        0        0     5121 2023-12-14 18:42:27.000000 nesse-0.1.0/src/nesse/plotting.py
--rw-rw-rw-   0        0        0     1856 2023-03-24 17:59:45.000000 nesse-0.1.0/src/nesse/quasiparticles.py
--rw-rw-rw-   0        0        0      241 2023-03-24 17:59:45.000000 nesse-0.1.0/src/nesse/silicon.py
--rw-rw-rw-   0        0        0    10037 2023-12-14 18:42:27.000000 nesse-0.1.0/src/nesse/simulation.py
-drwxrwxrwx   0        0        0        0 2023-12-14 19:13:12.768623 nesse-0.1.0/src/nesse.egg-info/
--rw-rw-rw-   0        0        0     1654 2023-12-14 19:13:12.000000 nesse-0.1.0/src/nesse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-12-14 19:13:12.000000 nesse-0.1.0/src/nesse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-14 19:13:12.000000 nesse-0.1.0/src/nesse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-12-14 19:13:12.000000 nesse-0.1.0/src/nesse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-12-14 19:13:12.000000 nesse-0.1.0/src/nesse.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-14 19:13:12.766108 nesse-0.1.0/tests/
--rw-rw-rw-   0        0        0     1140 2023-03-24 17:59:45.000000 nesse-0.1.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:11:01.438507 nesse-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-03-24 17:59:44.000000 nesse-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-03-24 17:59:44.000000 nesse-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1654 2024-05-13 19:11:01.436505 nesse-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-12-14 19:14:41.000000 nesse-0.1.1/README.md
+-rw-rw-rw-   0        0        0      955 2024-05-13 18:27:48.000000 nesse-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:11:01.439015 nesse-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 19:11:01.257104 nesse-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:11:01.396913 nesse-0.1.1/src/nesse/
+-rw-rw-rw-   0        0        0      147 2023-03-24 17:59:45.000000 nesse-0.1.1/src/nesse/__init__.py
+-rw-rw-rw-   0        0        0     2984 2024-05-13 15:50:31.000000 nesse-0.1.1/src/nesse/charge_propagation.py
+-rw-rw-rw-   0        0        0      880 2023-03-24 17:59:45.000000 nesse-0.1.1/src/nesse/constants.py
+-rw-rw-rw-   0        0        0     5978 2024-03-13 14:45:33.000000 nesse-0.1.1/src/nesse/event.py
+-rw-rw-rw-   0        0        0     7716 2023-12-14 18:42:27.000000 nesse-0.1.1/src/nesse/field.py
+-rw-rw-rw-   0        0        0     1160 2023-03-24 18:56:31.000000 nesse-0.1.1/src/nesse/interp.pyx
+-rw-rw-rw-   0        0        0     2803 2023-03-24 17:59:45.000000 nesse-0.1.1/src/nesse/interp_3d.py
+-rw-rw-rw-   0        0        0     3524 2024-05-13 15:49:09.000000 nesse-0.1.1/src/nesse/mobility.py
+-rw-rw-rw-   0        0        0     5293 2024-03-13 16:02:02.000000 nesse-0.1.1/src/nesse/plotting.py
+-rw-rw-rw-   0        0        0     1856 2023-03-24 17:59:45.000000 nesse-0.1.1/src/nesse/quasiparticles.py
+-rw-rw-rw-   0        0        0      241 2023-03-24 17:59:45.000000 nesse-0.1.1/src/nesse/silicon.py
+-rw-rw-rw-   0        0        0    11102 2024-05-13 17:54:54.000000 nesse-0.1.1/src/nesse/simulation.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:11:01.434507 nesse-0.1.1/src/nesse.egg-info/
+-rw-rw-rw-   0        0        0     1654 2024-05-13 19:11:01.000000 nesse-0.1.1/src/nesse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-13 19:11:01.000000 nesse-0.1.1/src/nesse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:11:01.000000 nesse-0.1.1/src/nesse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-13 19:11:01.000000 nesse-0.1.1/src/nesse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 19:11:01.000000 nesse-0.1.1/src/nesse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 19:11:01.432506 nesse-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1140 2023-03-24 17:59:45.000000 nesse-0.1.1/tests/test.py
```

### Comparing `nesse-0.1.0/LICENSE` & `nesse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nesse-0.1.0/PKG-INFO` & `nesse-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nesse
-Version: 0.1.0
+Version: 0.1.1
 Summary: A solid state detector simulation developed for the Nab experiment.
 Author-email: RJ Taylor <rjtaylo2@ncsu.edu>, Leendert Hayen <hayen@lpccaen.in2p3.fr>
 Project-URL: Homepage, https://github.com/rjtayl/nesse
 Project-URL: Bug Tracker, https://github.com/rjtayl/nesse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: h5py
 Requires-Dist: uproot==4.3.7
 Requires-Dist: pandas
 
 # nesse
-Nab Event Shape SImulation Effort (NESSE) is a python based solid state detector simulation developed for the Nab experiment. 
+Nab Event Shape Simulation Effort (NESSE) is a python based solid state detector simulation developed for the Nab experiment. 
 
 
 ### Dependencies
 Please insure the following dependencies are installed if installing nesse manually.
 
 - Cython==0.29.32
 - uproot==4.3.7
```

### Comparing `nesse-0.1.0/README.md` & `nesse-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # nesse
-Nab Event Shape SImulation Effort (NESSE) is a python based solid state detector simulation developed for the Nab experiment. 
+Nab Event Shape Simulation Effort (NESSE) is a python based solid state detector simulation developed for the Nab experiment. 
 
 
 ### Dependencies
 Please insure the following dependencies are installed if installing nesse manually.
 
 - Cython==0.29.32
 - uproot==4.3.7
```

### Comparing `nesse-0.1.0/pyproject.toml` & `nesse-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nesse"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "RJ Taylor", email = "rjtaylo2@ncsu.edu"},
     {name = "Leendert Hayen", email = "hayen@lpccaen.in2p3.fr"}  
 ]
 description = "A solid state detector simulation developed for the Nab experiment."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `nesse-0.1.0/src/nesse/charge_propagation.py` & `nesse-0.1.1/src/nesse/charge_propagation.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,33 +18,36 @@
             Ecoul[i] = F/Q
     return Ecoul
 
 def insideBoundaryCheck(pos, bounds):
     return ((pos[0] >= bounds[0][0]) & (pos[0] <= bounds[0][1]) & (pos[1] >= bounds[1][0]) & (pos[1] <= bounds[1][1])
             & (pos[2] >= bounds[2][0]) & (pos[2] <= bounds[2][1]))
 
-def updateQuasiParticles(objects, ds, maxdt, Ex_i, Ey_i, Ez_i, E_i, bounds, temp, diffusion=True, coulomb=False, tauTrap = lambda x, y, z : 1e9, NI = lambda x, y, z : 1e16):
+def updateQuasiParticles(objects, ds, maxdt, Ex_i, Ey_i, Ez_i, E_i, bounds, temp, diffusion=True, coulomb=False,
+                         tauTrap = lambda x, y, z : 1e9, NI = lambda x, y, z : 1e16,
+                         mobility_e = canali_mobility_e, mobility_h = canali_mobility_h):
     #Vector to save the effective electric field for each particle at the time step
     Eeff = np.zeros((len(objects), 3))
 
     # If coulomb is enabled, an effective electric field because of all other charges is added (plasma effects)
     if coulomb:
         Eeff += getEffectiveCoulombField(objects)
 
     for i in range(len(objects)):
         pos = objects[i].pos[-1]
         dt = maxdt
 
         Eeff[i] += np.array([Ex_i(pos), Ey_i(pos), Ez_i(pos)])
 
         if objects[i].q < 0:
-            mu = generalized_mobility_el(temp, NI(*pos), np.linalg.norm(Eeff[i]))
+            mu = mobility_e(temp, NI(*pos), np.linalg.norm(Eeff[i]))
             dv = -mu*Eeff[i]
+            # print(mu, dv, Eeff[i])
         else:
-            mu = generalized_mobility_h(temp, NI(*pos), np.linalg.norm(Eeff[i]))
+            mu = mobility_h(temp, NI(*pos), np.linalg.norm(Eeff[i]))
             dv = mu*Eeff[i]
 
         if not coulomb:
             dt = min(abs(ds/np.linalg.norm(dv)), maxdt)
 
         if diffusion:
             dv += ((diffusion_electron(temp) if objects[i].q < 0 else diffusion_hole(temp))/dt)**0.5*np.random.normal(size=3)
```

### Comparing `nesse-0.1.0/src/nesse/constants.py` & `nesse-0.1.1/src/nesse/constants.py`

 * *Files identical despite different names*

### Comparing `nesse-0.1.0/src/nesse/field.py` & `nesse-0.1.1/src/nesse/field.py`

 * *Files identical despite different names*

### Comparing `nesse-0.1.0/src/nesse/interp.pyx` & `nesse-0.1.1/src/nesse/interp.pyx`

 * *Files identical despite different names*

### Comparing `nesse-0.1.0/src/nesse/interp_3d.py` & `nesse-0.1.1/src/nesse/interp_3d.py`

 * *Files identical despite different names*

### Comparing `nesse-0.1.0/src/nesse/mobility.py` & `nesse-0.1.1/src/nesse/mobility.py`

 * *Files 24% similar despite different names*

```diff
@@ -60,20 +60,83 @@
 def mu_I_c(T):
     return mu_min*mu_max/(mu_max-mu_min)*(300/T)**0.5
 
 @jit(nopython=True, fastmath=True)
 def mu_I(T, NI):
     return mu_I_N(T)*(Nref1/NI)**alpha1 + mu_I_c(T)
 
+@jit(nopython=True)
 def generalized_mobility_el(T, NI, E):
     mu = 1/(1/mu0_el(T)+1/mu_I(T, NI))
     vsat = vs_el(T)
     return mu/(1+(mu*E/vsat)**(1/beta_el))**beta_el
 
 @jit(nopython=True)
 def generalized_mobility_h(T, NI, E):
     mu = 1/(1/mu0_h(T)+1/mu_I(T, NI))
     vsat = vs_h(T)
     return mu/(1+(mu*E/vsat)**(1/beta_h))**beta_h
 
 def generalized_diffusion_el(T, NI, E):
     return mobility(T, NI, E)*T*kB
+
+#mobility determined from fits to canali data
+#electrons
+mu_0_e = 1635*1e-4
+v_s_e = 1.04e7*1e-2
+c_e = 0.9438
+
+theta_mu_e = 2.462
+theta_v_s_e = 0.638
+theta_c_e = -0.7185
+
+#holes
+mu_0_h = 508*1e-4
+v_s_h = 9.98e6*1e-2
+c_h = 1.077
+
+theta_mu_h = 2.26
+theta_v_s_h = 0.09
+theta_c_h = -0.24
+
+def canali_mobility_e(T, NI, E):
+    mu = mu_0_e * (300/T)**theta_mu_e
+    v_s = v_s_e * (300/T)**theta_v_s_e
+    c = c_e * (300/T)**theta_c_e
+    return mu/(1+(mu*E/v_s)**c)**(1/c)
+
+def canali_mobility_h(T, NI, E):
+    mu = mu_0_h * (300/T)**theta_mu_h
+    v_s = v_s_h * (300/T)**theta_v_s_h
+    c = c_h * (300/T)**theta_c_h
+    return mu/(1+(mu*E/v_s)**c)**(1/c)
+
+#RJ fit to electrons
+@jit(nopython=True)
+def mu0_el_RJ(T):
+    return 0.1521 * (T/300)**-2.01 # m^2/V/s
+
+#RJ max fit  to electrons
+@jit(nopython=True)
+def mu0_el_RJ_max(T):
+    return 0.1721 * (T/300)**-2.01 # m^2/V/s
+
+@jit(nopython=True)
+def generalized_mobility_el_RJ(T, NI, E):
+    mu = 1/(1/mu0_el_RJ(T)+1/mu_I(T, NI))
+    vsat = vs_el(T)
+    return mu/(1+(mu*E/vsat)**(beta_el))**1/beta_el
+
+# @jit(nopython=True)
+# def mu0_h(T):
+#     return 0.0450 * (T/300)**-2.247 # m^2/V/s
+
+
+# @jit(nopython=True)
+# def vs_h(T):
+#     return mu0_h(T)/1.95e6
+
+# @jit(nopython=True)
+# def generalized_mobility_h(T, NI, E):
+#     mu = 1/(1/mu0_h(T)+1/mu_I(T, NI))
+#     vsat = vs_h(T)
+#     return mu/(1+(mu*E/vsat)**(beta_h))**1/beta_h
```

### Comparing `nesse-0.1.0/src/nesse/plotting.py` & `nesse-0.1.1/src/nesse/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 plt.rcParams['figure.figsize'] = [8, 5]
 plt.rcParams.update({'font.size': 18})
 
 def plot_current(event, show_plot=True, alpha=1, contact=0):
     plt.plot(event.dt[contact],event.dI[contact], alpha=alpha)
     if show_plot: plt.show()
     return None
+
+def plot_charge(event, show_plot=True, alpha=1, contact=0):
+    plt.plot(event.dt[contact],event.dQ[contact], alpha=alpha)
+    if show_plot: plt.show()
+    return None
     
 def plot_signal(event, show_plot=True, alpha=1, contact=0):
-    plt.plot(event.signal_times[contact],event.signal_I[contact], alpha=alpha)
+    plt.plot(event.signal_times[contact],event.signal[contact], alpha=alpha)
     if show_plot: plt.show()
     return None
 
 
 def plot_event_drift(event, bounds, prefix="",suffix="", show_plot=True, pairs=None, save=False):
     fig = plt.figure()
     ax = plt.axes(projection ='3d')
```

### Comparing `nesse-0.1.0/src/nesse/quasiparticles.py` & `nesse-0.1.1/src/nesse/quasiparticles.py`

 * *Files identical despite different names*

### Comparing `nesse-0.1.0/src/nesse/simulation.py` & `nesse-0.1.1/src/nesse/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,43 +4,45 @@
 from .quasiparticles import *
 from scipy.interpolate import RegularGridInterpolator 
 from .charge_propagation import *
 from tqdm.auto import tqdm
 import csv
 from .silicon import *
 import copy
+from .mobility import *
 
 #from line_profiler import LineProfiler
 
 #from joblib import Parallel, delayed
 #import multiprocessing
 
 #num_cores = multiprocessing.cpu_count()
 
 class Simulation:
     '''
     Object contains all nessie objects needed to simulate a signal. 
     Currently assumes only one contact.
     
     '''
-    def __init__(self, _name, _temp, _electricField=None, _weightingPotential=None, _electricPotential=None, _weightingField=None,  
-                    _cceField=None, _chargeCaptureField=None, _electronicResponse=None, contacts=1,
-                      _impurityConcentration= lambda x, y, z : 1e16):        
+    def __init__(self, _name, _temp, _electricField=None, _weightingPotential=None, _electricPotential=None,
+                 _weightingField=None, _cceField=None, _chargeCaptureField=None, _electronicResponse=None, contacts=1,
+                 _impurityConcentration= lambda x, y, z : 1e16, _mobility = [generalized_mobility_el, generalized_mobility_h]):        
         self.name = _name
         self.electricField = _electricField
         self.electricPotential = _electricPotential
         self.weightingPotential = _weightingPotential
         self.weightingField = _weightingField
         self.cceField = _cceField
         self.chargeCaptureField = _chargeCaptureField
         self.electronicResponse = _electronicResponse
         self.temp = _temp
         self.bounds = None
         self.contacts = contacts
         self.impurityConcentration = _impurityConcentration
+        self.mobility = _mobility
 
         if contacts is not None and type(_weightingPotential) is not list:
             centers = find_centers(contacts)
             wps = []
             for i in range(contacts):
                 wp_temp = copy.deepcopy(_weightingPotential)
                 wp_temp.shift(centers[i]+(0,))
@@ -55,14 +57,18 @@
                 % (self.name, self.electricField,self.weightingPotential, self.cceField, self.chargeCaptureField,          
                    self.electronicResponse))
     
     def setTemp(self,T):
         self.temp = T
         return None
     
+    def setMobility(self,mobility_e, mobility_h):
+        self.mobility = [mobility_e, mobility_h]
+        return None
+    
     def setIDP(self, IDP): #IDP(x,y,z)->NI[m^-3]
         if type(IDP) is Potential:
             self.impurityConcentration = IDP.interpolate()
 
         else:
             self.impurityConcentration = IDP
         return None
@@ -140,15 +146,16 @@
         
         if bounds is None:
             simBounds = self.bounds if self.bounds is not None else [[axis[0],axis[-1]] for axis in self.electricField.grid]
         else: 
             simBounds = bounds
 
         #Find electron and hole drift paths for each event
-        for i in tqdm(range(len(events))):
+        for i in (t:=tqdm(range(len(events)))):
+            t.set_description(f"Drift Calculation", refresh=True)
             event = events[i]
             #rint will give an integer number of e-h pairs, then adjust for variance using sigma = sqrt(FN)
             # assumes in linear regeme of fano factor
             pairs_0 = event.dE/ephBestFit(self.temp)
             pairs = np.rint(np.random.normal(pairs_0,np.sqrt(Fano_Si*pairs_0))) 
 
             # electron charge cloud assembly
@@ -167,21 +174,24 @@
                 # TODO: Provide a radius to smooth initial charge cloud (currently 0)
                 cc_e = cc_e + initializeChargeCloud(-factor*qe_SI, factor*me_SI, pairNr, event.times[j], 0, event.pos[j])
                 cc_h = cc_h + initializeChargeCloud(factor*qe_SI, factor*me_SI, pairNr, event.times[j], 0, event.pos[j])
 
             cc = cc_e + cc_h
 
             alive = np.ones(len(cc)) == 1
-            print("Total quasiparticles: %d" % len(cc))
+            # print("Total quasiparticles: %d" % len(cc))
+            # t.set_description(f"Event {i}, Total quasiparticles: {len(cc)}", refresh=True)
+            t.set_postfix_str(f"Event {i}, Total quasiparticles: {len(cc)}", refresh=True)
 
             # Loop over alive particles until all have been stopped/collected
             pbar = tqdm(disable=silence)
             while np.any(alive):
-                cc_new = updateQuasiParticles(list(compress(cc, alive)), ds, dt, Ex_i, Ey_i, Ez_i, Emag_i, simBounds, self.temp,
-                                               diffusion=diffusion, coulomb=coulomb, NI=self.impurityConcentration)
+                cc_new = updateQuasiParticles(list(compress(cc, alive)), ds, dt, Ex_i, Ey_i, Ez_i, Emag_i, simBounds,
+                                              self.temp, diffusion=diffusion, coulomb=coulomb,NI=self.impurityConcentration,
+                                              mobility_e = self.mobility[0], mobility_h = self.mobility[1])
                 
                 counter = 0
                 for j in range(len(alive)):
                     if alive[j]:
                         cc[j] = cc_new[counter]
                         counter+=1
 
@@ -198,20 +208,29 @@
         for contact in contacts:
             weightingFieldx_interp, weightingFieldy_interp, weightingFieldz_interp, weightingFieldMag_interp = self.weightingField[contact].interpolate(interp3d)
             wf_interp = [weightingFieldx_interp, weightingFieldy_interp, weightingFieldz_interp, weightingFieldMag_interp]
         
             for event in events:
                 event.calculateInducedCurrent(dt, wf_interp, contact)
 
+    def calculateInducedCharge(self, events, contacts = None):
+        if contacts is None: contacts=np.arange(self.contacts)
+        for contact in contacts:
+            for event in events:
+                event.calculateIntegratedCharge(contact)
+
     def calculateElectronicResponse(self, events, contacts = None):
         if contacts is None: contacts=np.arange(self.contacts)
         for event in events:
             for contact in contacts:
                 event.convolveElectronicResponse(self.electronicResponse, contact)
 
+    def getSignals(self, events, dt, contacts = None, interp3d=True):
+        self.calculateInducedCurrent(events, dt, contacts, interp3d)
+        self.calculateElectronicResponse(events, contacts)
 
 def find_centers(N,R=5.15e-3,s=0.1e-3):    
     ''' This functions finds where to place the centers of hexagonal configuration depending on the hexagon radius 
         and seperation between hexagons. Default values are correct for Nab detectors. This is here primarily to copy
         over weighting potentials for multiple contact sims. '''
     
     centers = [(0,0)]
```

### Comparing `nesse-0.1.0/src/nesse.egg-info/PKG-INFO` & `nesse-0.1.1/src/nesse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nesse
-Version: 0.1.0
+Version: 0.1.1
 Summary: A solid state detector simulation developed for the Nab experiment.
 Author-email: RJ Taylor <rjtaylo2@ncsu.edu>, Leendert Hayen <hayen@lpccaen.in2p3.fr>
 Project-URL: Homepage, https://github.com/rjtayl/nesse
 Project-URL: Bug Tracker, https://github.com/rjtayl/nesse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: h5py
 Requires-Dist: uproot==4.3.7
 Requires-Dist: pandas
 
 # nesse
-Nab Event Shape SImulation Effort (NESSE) is a python based solid state detector simulation developed for the Nab experiment. 
+Nab Event Shape Simulation Effort (NESSE) is a python based solid state detector simulation developed for the Nab experiment. 
 
 
 ### Dependencies
 Please insure the following dependencies are installed if installing nesse manually.
 
 - Cython==0.29.32
 - uproot==4.3.7
```

### Comparing `nesse-0.1.0/tests/test.py` & `nesse-0.1.1/tests/test.py`

 * *Files identical despite different names*

