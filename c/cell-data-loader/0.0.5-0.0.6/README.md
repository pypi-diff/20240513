# Comparing `tmp/cell_data_loader-0.0.5.tar.gz` & `tmp/cell_data_loader-0.0.6.tar.gz`

## Comparing `cell_data_loader-0.0.5.tar` & `cell_data_loader-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    38037 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/__init__.py
--rwxr-xr-x   0        0        0     1659 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/example_numpy.py
--rwxr-xr-x   0        0        0     2449 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/example_torch.py
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/github_push.sh
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/pypi_push.sh
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/requirements.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/setup.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/__init__.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/base_dataset.py
--rwxr-xr-x   0        0        0    17236 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/cell_data_loader.py
--rwxr-xr-x   0        0        0    29083 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/tests/__init__.py
--rwxr-xr-x   0        0        0     5774 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/tests/unit_tests.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    38037 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/__init__.py
+-rwxr-xr-x   0        0        0     1682 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/example_numpy.py
+-rwxr-xr-x   0        0        0     2453 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/example_torch.py
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/github_push.sh
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/pypi_push.sh
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/setup.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/src/cell_data_loader/__init__.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/src/cell_data_loader/base_dataset.py
+-rwxr-xr-x   0        0        0    18565 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/src/cell_data_loader/cell_data_loader.py
+-rwxr-xr-x   0        0        0    29083 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/src/cell_data_loader/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/tests/__init__.py
+-rwxr-xr-x   0        0        0     5791 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/tests/unit_tests.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 cell_data_loader-0.0.6/PKG-INFO
```

### Comparing `cell_data_loader-0.0.5/.gitattributes` & `cell_data_loader-0.0.6/.gitattributes`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.5/example_numpy.py` & `cell_data_loader-0.0.6/example_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 #!/usr/bin/python3
-
 from src.cell_data_loader import CellDataloader
 
 try:
 	import tensorflow as tf
 except:
 	try:
 		from keras import tensorflow as tf
 	except:
 		raise Exception("Need valid tensorflow")
 
-import numpy
+import numpy as np
 import os
 
 def example_numpy(verbose=True):
 
 	"""
 	Replace these folders with whatever folders of cells you may have. Note that
 	the test/train folders in this script are the same -- you would need to 
 	have a separate train/test set in your own implementation
 	"""
-	wd = os.path.dirname(os.path.realpath(__file__))
+	wd = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
 	imfolder1 = os.path.join(wd,'data',
 		'3368914_4_non_tumor')
 	imfolder2 = os.path.join(wd,'data',
 		'4173633_5')
 
-	model = resnet50()
+	#model = resnet50()
 	model = tf.keras.applications.resnet50.ResNet50(
 		include_top=True,
 		weights='imagenet',
 		input_tensor=None,
 		input_shape=None,
 		pooling=None,
 		classes=1000
@@ -38,21 +37,21 @@
 
 	# Train
 
 	dataloader_train = CellDataloader(imfolder1,imfolder2,
 		dtype="numpy",verbose=False)
 
 	z = None
-	for epoch in range(100):
+	for epoch in range(1):
 		for image,y in dataloader_train:
 			if z is None:
 				z_dim = list(y.shape)
 				z_dim[1] = 1000 - z_dim[1]
 				z = np.zeros(z_dim)
-			y = np.concatenate(y,z,axis=1)
+			y = np.concatenate((y,z),axis=1)
 			model.fit(image,y)
 
 	# Test
 
 	model.eval()
 	dataloader_test = CellDataloader(imfolder1,imfolder2,dtype="torch",
 		verbose=False)
```

### Comparing `cell_data_loader-0.0.5/example_torch.py` & `cell_data_loader-0.0.6/example_torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3
 
-from cell_data_loader import CellDataloader
+from src.cell_data_loader import CellDataloader
 from torchvision.models import resnet50 #, ResNet50_Weights
 import torch
 import os
 import glob
 
 def example_torch(gpu_ids = None,verbose=True):
 
@@ -44,15 +44,15 @@
 	model.train()
 	loss_fn = torch.nn.MSELoss(reduction='sum')
 	optimizer = torch.optim.Adam(model.parameters(), lr=1e-5)
 	dataloader_train = CellDataloader(imfolder1_train,imfolder2_train,
 		dtype="torch",
 		verbose=False, gpu_ids=gpu_ids)
 	if verbose: print("Beginning training")
-	n_epochs = 0
+	n_epochs = 1
 	for epoch in range(n_epochs):
 		l = 0
 		c = 0
 		for image,y in dataloader_train:
 			y_pred = model(image)
 			y_pred = y_pred[:,:y.size()[1]]
 			loss = loss_fn(y_pred, y)
```

### Comparing `cell_data_loader-0.0.5/src/cell_data_loader/base_dataset.py` & `cell_data_loader-0.0.6/src/cell_data_loader/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.5/src/cell_data_loader/cell_data_loader.py` & `cell_data_loader-0.0.6/src/cell_data_loader/cell_data_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from PIL import Image,ImageEnhance
 from scipy import ndimage
 from scipy.signal import resample
 from scipy.ndimage.interpolation import map_coordinates
 from scipy.ndimage.filters import gaussian_filter
 from .base_dataset import BaseDataset
 import torch,torchvision
+torchvision.disable_beta_transforms_warning()
 from .util import *
 import warnings
 
 
 #import openslide
 #import czifile
 try:
@@ -200,15 +201,16 @@
 		dtype = "torch",
 		gpu_ids = None,
 		label_balance = True,
 		cell_box_regex = None,
 		cell_box_filelist = None,
 		n_channels = None,
 		channels_first = True,
-		match_labels=False):
+		match_labels=False,
+		normalize=True):
 		
 		self.verbose = verbose
 		self.label_balance = label_balance
 		self.segment_image = segment_image.lower()
 		self.dim = dim
 		self.batch_size = batch_size
 		self.dtype = dtype
@@ -217,27 +219,28 @@
 		self.gpu_ids = gpu_ids
 		self.cell_box_regex = cell_box_regex
 		self.cell_box_filelist = cell_box_filelist
 		self.dtype = dtype
 		self.n_channels = n_channels
 		self.channels_first = channels_first
 		self.augment_image = augment_image
+		self.normalize = normalize
 		if self.augment_image and self.dtype == "torch":
-			from torchvision import transforms
+			import torchvision.transforms.v2 as transforms
 			
 			self.augment = transforms.Compose([
-				#transforms.ElasticTransform(),
 				transforms.RandomHorizontalFlip(0.5),
 				transforms.RandomVerticalFlip(0.5),
 				transforms.GaussianBlur(5),
 				transforms.ColorJitter(brightness=(0.5,1.5),
 					contrast=(1), saturation=(0.5,1.5), hue=(-0.1,0.1)),
-				transforms.RandomResizedCrop((self.dim))])#,
+				transforms.RandomResizedCrop(self.dim, antialias=True)])#,
 				#transforms.Normalize((0.5,0.5,0.5),(0.5,0.5,0.5))])
-		
+			self.augment2 = transforms.Compose([
+				transforms.ElasticTransform()])
 		"""
 		If true, outputs given labels equally. This may repeat images if the
 		counts of each don't line up.
 		"""
 		self.match_labels = match_labels
 		"""
 		Determines if image folders or file lists exist, then reads them in
@@ -375,14 +378,19 @@
 				self.label_batch = torch.zeros((self.batch_size,self.n_labels),
 					device = self.gpu_ids)
 		sample = self.image_objects[0]
 		if n_channels is None:
 			self.n_channels = sample.get_n_channels()
 		else:
 			self.n_channels = n_channels
+		if self.normalize and self.dtype == "torch":
+			from torchvision.transforms.v2 import Normalize
+			self.normalizer = Normalize(
+				tuple([0.5 for _ in range(self.n_channels)]),
+				tuple([0.5 for _ in range(self.n_channels)]))
 		for image_object in self.image_objects:
 			image_object.n_channels = self.n_channels
 		if self.verbose:
 			print("%d Channels Detected" % self.n_channels)
 		if self.dtype == "torch":
 			self.batch = torch.zeros(self.batch_size,self.dim[0],self.dim[1],
 				self.n_channels,device=self.gpu_ids)
@@ -467,16 +475,22 @@
 		if self.return_labels(): label = self.image_objects[self.index].label
 		self.im_index += 1
 		while self.im_index >= len(self.image_objects[self.index]) or \
 				(len(self.image_objects[self.index]) == 0):
 			self.im_index = 0
 			self.index += 1
 			if self.index >= len(self.image_objects): break
-		if self.augment_image and self.dtype == "torch":
-			im = self.augment(im)
+		#if self.augment_image and self.dtype == "torch":
+			#imdim = im.size()
+			#print("imdim: %s" % str(imdim))
+			#im = torch.permute(im,[len(imdim)-1]+list(range(0,len(imdim)-1)))
+			#print("imdim: %s" % str(im.size()))
+			#im = self.augment(im)
+			#im = torch.permute(im,list(range(1,len(imdim))) + [0])
+			#print("imdim: %s"%str(im.size()))
 		if self.return_labels():
 			return im,label
 		else:
 			return im
 	def __next__(self):
 		"""
 		Returns the next batch of images
@@ -504,14 +518,30 @@
 				if len(im.size()) == 2 and self.n_channels == 1:
 					im = torch.unsqueeze(im,2)
 				self.batch[i,...] = torch.unsqueeze(im,0)
 				if self.channels_first:
 					b = torch.moveaxis(self.batch,-1,1)
 				else:
 					b = self.batch
+				if (self.augment_image and self.n_channels <= 3) or self.normalize:
+					if not self.channels_first:
+						b = torch.permute(b,[0,-1] + list(range(1,len(b.size())-1)))
+					#print("b.size(): %s" % str(b.size()))
+					if self.n_channels <= 3 and self.augment:
+						b = self.augment(b)
+						if self.dim[0] > 32 and self.dim[1] > 32:
+							b = self.augment2(b)
+					#print("b.size(): %s" % str(b.size()))
+					#print([0]+list(range(2,len(b.size()))) + [1])
+					if self.normalize:
+						b = self.normalizer(b)
+					if not self.channels_first:
+						b = torch.permute(b,[0]+list(range(2,len(b.size()))) + [1])
+					#print("b.size(): %s" % str(b.size()))
+					#print("sss")
 			elif self.dtype == "numpy":
 				if len(im.shape) == 2 and self.n_channels == 1:
 					im = np.expand_dims(im,axis=2)
 				self.batch[i,...] = np.expand_dims(im,axis=0)
 				if self.channels_first:
 					b = np.moveaxis(self.batch,-1,1)
 				else:
```

### Comparing `cell_data_loader-0.0.5/src/cell_data_loader/util.py` & `cell_data_loader-0.0.6/src/cell_data_loader/util.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.5/tests/unit_tests.py` & `cell_data_loader-0.0.6/tests/unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #from src.cell_data_loader import *
 import os,sys,time
 import numpy as np
 import torch
 
 wd         = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
-im_root    = os.path.join(wd,'data')
+im_root    = os.path.join(os.path.dirname(wd),'data')
 #imfile_svs = os.path.join(im_root,'10447627_1.svs')
 imfolder1  = os.path.join(im_root,'4173633_5')
 imfolder2  = os.path.join(im_root,'3368914_4_non_tumor')
 imfolder3  = os.path.join(im_root,'H6-13_Mars1+dapi')
 sys.path.insert(0,os.path.join(wd))
 from src.cell_data_loader import *
```

### Comparing `cell_data_loader-0.0.5/README.md` & `cell_data_loader-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.5/pyproject.toml` & `cell_data_loader-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "cell_data_loader"
 
-version = "0.0.5"
+version = "0.0.6"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

### Comparing `cell_data_loader-0.0.5/PKG-INFO` & `cell_data_loader-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cell_data_loader
-Version: 0.0.5
+Version: 0.0.6
 Summary: Converts general images of cells into formats and labels for deep learning pipelines
 Project-URL: Homepage, https://github.com/mleming/CellDataLoader
 Author-email: Matt Leming <mleming@mgh.harvard.edu>
 Maintainer-email: Matt Leming <mleming@mgh.harvard.edu>
 License: MIT License
 Keywords: biomedical,cell,cell image,cellpose,csz,dataloader
 Requires-Python: >=3.8
```

