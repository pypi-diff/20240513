# Comparing `tmp/cell_data_loader-0.0.4.tar.gz` & `tmp/cell_data_loader-0.0.5.tar.gz`

## Comparing `cell_data_loader-0.0.4.tar` & `cell_data_loader-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    38037 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/__init__.py
--rwxr-xr-x   0        0        0     1659 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/example_numpy.py
--rwxr-xr-x   0        0        0     2451 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/example_torch.py
--rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/github_push.sh
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/pypi_push.sh
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/requirements.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/setup.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/__init__.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/base_dataset.py
--rwxr-xr-x   0        0        0    16625 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/cell_data_loader.py
--rwxr-xr-x   0        0        0    29083 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/tests/__init__.py
--rwxr-xr-x   0        0        0     5774 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/tests/unit_tests.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    38037 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/__init__.py
+-rwxr-xr-x   0        0        0     1659 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/example_numpy.py
+-rwxr-xr-x   0        0        0     2449 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/example_torch.py
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/github_push.sh
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/pypi_push.sh
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/setup.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/__init__.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/base_dataset.py
+-rwxr-xr-x   0        0        0    17236 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/cell_data_loader.py
+-rwxr-xr-x   0        0        0    29083 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/src/cell_data_loader/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/tests/__init__.py
+-rwxr-xr-x   0        0        0     5774 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/tests/unit_tests.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 cell_data_loader-0.0.5/PKG-INFO
```

### Comparing `cell_data_loader-0.0.4/.gitattributes` & `cell_data_loader-0.0.5/.gitattributes`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.4/example_numpy.py` & `cell_data_loader-0.0.5/example_numpy.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.4/example_torch.py` & `cell_data_loader-0.0.5/example_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 	model.train()
 	loss_fn = torch.nn.MSELoss(reduction='sum')
 	optimizer = torch.optim.Adam(model.parameters(), lr=1e-5)
 	dataloader_train = CellDataloader(imfolder1_train,imfolder2_train,
 		dtype="torch",
 		verbose=False, gpu_ids=gpu_ids)
 	if verbose: print("Beginning training")
-	n_epochs = 500
+	n_epochs = 0
 	for epoch in range(n_epochs):
 		l = 0
 		c = 0
 		for image,y in dataloader_train:
 			y_pred = model(image)
 			y_pred = y_pred[:,:y.size()[1]]
 			loss = loss_fn(y_pred, y)
@@ -61,15 +61,15 @@
 			optimizer.zero_grad()
 			loss.backward()
 			optimizer.step()
 		torch.save(model,model_file)
 		if verbose:
 			print(
 				"Epoch {epoch:d}/{n_epochs:d}: loss: {loss:.5f}".format(
-					epoch=epoch,n_epochs=e_epochs,loss=l/c)
+					epoch=epoch,n_epochs=n_epochs,loss=l/c)
 			)
 	# Test
 	
 	model.eval()
 
 	dataloader_test = CellDataloader(imfolder1_test,imfolder2_test,
 		dtype="torch",verbose=False, gpu_ids = gpu_ids)
```

### Comparing `cell_data_loader-0.0.4/src/cell_data_loader/base_dataset.py` & `cell_data_loader-0.0.5/src/cell_data_loader/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.4/src/cell_data_loader/cell_data_loader.py` & `cell_data_loader-0.0.5/src/cell_data_loader/cell_data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,28 @@
 		self.im_index = 0
 		self.gpu_ids = gpu_ids
 		self.cell_box_regex = cell_box_regex
 		self.cell_box_filelist = cell_box_filelist
 		self.dtype = dtype
 		self.n_channels = n_channels
 		self.channels_first = channels_first
+		self.augment_image = augment_image
+		if self.augment_image and self.dtype == "torch":
+			from torchvision import transforms
+			
+			self.augment = transforms.Compose([
+				#transforms.ElasticTransform(),
+				transforms.RandomHorizontalFlip(0.5),
+				transforms.RandomVerticalFlip(0.5),
+				transforms.GaussianBlur(5),
+				transforms.ColorJitter(brightness=(0.5,1.5),
+					contrast=(1), saturation=(0.5,1.5), hue=(-0.1,0.1)),
+				transforms.RandomResizedCrop((self.dim))])#,
+				#transforms.Normalize((0.5,0.5,0.5),(0.5,0.5,0.5))])
+		
 		"""
 		If true, outputs given labels equally. This may repeat images if the
 		counts of each don't line up.
 		"""
 		self.match_labels = match_labels
 		"""
 		Determines if image folders or file lists exist, then reads them in
@@ -453,14 +467,16 @@
 		if self.return_labels(): label = self.image_objects[self.index].label
 		self.im_index += 1
 		while self.im_index >= len(self.image_objects[self.index]) or \
 				(len(self.image_objects[self.index]) == 0):
 			self.im_index = 0
 			self.index += 1
 			if self.index >= len(self.image_objects): break
+		if self.augment_image and self.dtype == "torch":
+			im = self.augment(im)
 		if self.return_labels():
 			return im,label
 		else:
 			return im
 	def __next__(self):
 		"""
 		Returns the next batch of images
```

### Comparing `cell_data_loader-0.0.4/src/cell_data_loader/util.py` & `cell_data_loader-0.0.5/src/cell_data_loader/util.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.4/tests/unit_tests.py` & `cell_data_loader-0.0.5/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.4/README.md` & `cell_data_loader-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.4/pyproject.toml` & `cell_data_loader-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "cell_data_loader"
 
-version = "0.0.4"
+version = "0.0.5"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

### Comparing `cell_data_loader-0.0.4/PKG-INFO` & `cell_data_loader-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cell_data_loader
-Version: 0.0.4
+Version: 0.0.5
 Summary: Converts general images of cells into formats and labels for deep learning pipelines
 Project-URL: Homepage, https://github.com/mleming/CellDataLoader
 Author-email: Matt Leming <mleming@mgh.harvard.edu>
 Maintainer-email: Matt Leming <mleming@mgh.harvard.edu>
 License: MIT License
 Keywords: biomedical,cell,cell image,cellpose,csz,dataloader
 Requires-Python: >=3.8
```

