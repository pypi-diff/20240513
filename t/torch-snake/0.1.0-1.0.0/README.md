# Comparing `tmp/torch-snake-0.1.0.tar.gz` & `tmp/torch-snake-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\torch-snake-0.1.0.tar", last modified: Fri Feb 12 12:10:26 2021, max compression
+gzip compressed data, was "torch-snake-1.0.0.tar", last modified: Mon May 13 09:41:22 2024, max compression
```

## Comparing `torch-snake-0.1.0.tar` & `torch-snake-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-02-12 12:10:26.232162 torch-snake-0.1.0/
--rw-rw-rw-   0        0        0     3073 2021-02-12 12:10:26.231163 torch-snake-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2335 2021-02-12 12:09:39.000000 torch-snake-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2021-02-12 12:10:26.232162 torch-snake-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      786 2021-02-12 12:05:38.000000 torch-snake-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-12 12:10:26.213163 torch-snake-0.1.0/snake/
--rw-rw-rw-   0        0        0        0 2021-02-12 11:54:05.000000 torch-snake-0.1.0/snake/__init__.py
--rw-rw-rw-   0        0        0     2412 2021-02-12 11:54:05.000000 torch-snake-0.1.0/snake/activations.py
-drwxrwxrwx   0        0        0        0 2021-02-12 12:10:26.229163 torch-snake-0.1.0/torch_snake.egg-info/
--rw-rw-rw-   0        0        0     3073 2021-02-12 12:10:26.000000 torch-snake-0.1.0/torch_snake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2021-02-12 12:10:26.000000 torch-snake-0.1.0/torch_snake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-12 12:10:26.000000 torch-snake-0.1.0/torch_snake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2021-02-12 12:10:26.000000 torch-snake-0.1.0/torch_snake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-02-12 12:10:26.000000 torch-snake-0.1.0/torch_snake.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 09:41:22.679949 torch-snake-1.0.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2024-05-13 09:36:38.000000 torch-snake-1.0.0/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2683 2024-05-13 09:41:22.679949 torch-snake-1.0.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2197 2024-05-13 09:36:38.000000 torch-snake-1.0.0/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-13 09:41:22.679949 torch-snake-1.0.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      762 2024-05-13 09:40:36.000000 torch-snake-1.0.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 09:41:22.675949 torch-snake-1.0.0/snake/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-13 09:36:38.000000 torch-snake-1.0.0/snake/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4764 2024-05-13 09:36:38.000000 torch-snake-1.0.0/snake/activations.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 09:41:22.679949 torch-snake-1.0.0/torch_snake.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2683 2024-05-13 09:41:22.000000 torch-snake-1.0.0/torch_snake.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2024-05-13 09:41:22.000000 torch-snake-1.0.0/torch_snake.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-13 09:41:22.000000 torch-snake-1.0.0/torch_snake.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2024-05-13 09:41:22.000000 torch-snake-1.0.0/torch_snake.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2024-05-13 09:41:22.000000 torch-snake-1.0.0/torch_snake.egg-info/top_level.txt
```

### Comparing `torch-snake-0.1.0/PKG-INFO` & `torch-snake-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,29 @@
-Metadata-Version: 2.1
-Name: torch-snake
-Version: 0.1.0
-Summary: Sample PyTorch implementation of the snake activation function
-Home-page: https://github.com/EdwardDixon/snake
-Author: Edward Dixon
-Author-email: dixon.edward@gmail.com
-License: UNKNOWN
-Description: [![PyPI version](https://badge.fury.io/py/torch-snake.svg)](https://badge.fury.io/py/torch-snake)
-        
-        # Snake
-        Based on ["Neural Networks Fail to Learn Periodic Functions and How to Fix It"](https://arxiv.org/abs/2006.08195) by Liu Ziyin, Tilman Hartwig, Masahito Ueda
-        
-        This is a PyTorch implementation of the `snake` activation function from the paper - or at least I _think_ it is, no affiliation with the authors, use at your own risk, etc., etc.
-        
-        A few variations of the function are discussed in the paper, this package implements:
-        
-         <img src="https://render.githubusercontent.com/render/math?math=x%2B\frac{1}{a}sin^{2}(ax)">
-         
-        Snake is **periodic**, but _also_ monotonic. To see how **snake** behaves for a range of x given various choices of `a`, watch this video:
-        
-        [![snake activation function gets wriggly for higher a](http://img.youtube.com/vi/5g7-8mtywuk/0.jpg)](http://www.youtube.com/watch?v=5g7-8mtywuk "Snake Activation")
-        
-        ## Installation
-        Two methods:
-        - Using **pip**, `pip install torch-snake`
-        - To install from source, first clone this repository.  Then, from the main repo folder, run `python setup.py install`
-        
-        ## Usage
-        Fairly easy really `from snake.activations import Snake`.  The `Snake` constructor [(code here)](snake/activations.py) has an optional **learnable** parameter alpha which defaults to 1.  The authors of the paper find values between 5 and 50 work quite well for "known-periodic" data, while for better results with non-periodic data, you should choose a small value like 0.2.  The constructor also takes an `alpha_learnable` parameter which defaults to `True`, so that you can disable "learnability" if your experiments so require.  
-        
-        ## Sample code
-        There's a notebook, still quite rough - [example.ipynb](example.ipynb).  Early indications are that good choices of hyperparameters are quite important for best results (though snake's own parameter trains quite readily).
-        
-        
-        ## Acknowledgements
-        This code probably wouldn't have gotten written if it hadn't been for [Alexandra Deis](https://towardsdatascience.com/@astakhova.aleksandra) and [her excellent article](https://towardsdatascience.com/extending-pytorch-with-custom-activation-functions-2d8b065ef2fa).  It has also benefitted hugely from generous contributions by [Federico Berto](https://github.com/Juju-botu).
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[![PyPI version](https://badge.fury.io/py/torch-snake.svg)](https://badge.fury.io/py/torch-snake)
+
+# Snake
+Based on ["Neural Networks Fail to Learn Periodic Functions and How to Fix It"](https://arxiv.org/abs/2006.08195) by Liu Ziyin, Tilman Hartwig, Masahito Ueda
+
+This is a PyTorch implementation of the `snake` activation function from the paper - or at least I _think_ it is, no affiliation with the authors, use at your own risk, etc., etc.
+
+A few variations of the function are discussed in the paper, this package implements:
+
+ <img src="https://render.githubusercontent.com/render/math?math=x%2B\frac{1}{a}sin^{2}(ax)">
+ 
+Snake is **periodic**, but _also_ monotonic. To see how **snake** behaves for a range of x given various choices of `a`, watch this video:
+
+[![snake activation function gets wriggly for higher a](http://img.youtube.com/vi/5g7-8mtywuk/0.jpg)](http://www.youtube.com/watch?v=5g7-8mtywuk "Snake Activation")
+
+## Installation
+Two methods:
+- Using **pip**, `pip install torch-snake`
+- To install from source, first clone this repository.  Then, from the main repo folder, run `python setup.py install`
+
+## Usage
+Fairly easy really `from snake.activations import Snake`.  The `Snake` constructor [(code here)](snake/activations.py) has an optional **learnable** parameter alpha which defaults to 1.  The authors of the paper find values between 5 and 50 work quite well for "known-periodic" data, while for better results with non-periodic data, you should choose a small value like 0.2.  The constructor also takes an `alpha_learnable` parameter which defaults to `True`, so that you can disable "learnability" if your experiments so require.  
+
+## Sample code
+There's a notebook, still quite rough - [example.ipynb](example.ipynb).  Early indications are that good choices of hyperparameters are quite important for best results (though snake's own parameter trains quite readily).
+
+
+## Acknowledgements
+This code probably wouldn't have gotten written if it hadn't been for [Alexandra Deis](https://towardsdatascience.com/@astakhova.aleksandra) and [her excellent article](https://towardsdatascience.com/extending-pytorch-with-custom-activation-functions-2d8b065ef2fa) .
```

### Comparing `torch-snake-0.1.0/README.md` & `torch-snake-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,44 @@
-[![PyPI version](https://badge.fury.io/py/torch-snake.svg)](https://badge.fury.io/py/torch-snake)
-
-# Snake
-Based on ["Neural Networks Fail to Learn Periodic Functions and How to Fix It"](https://arxiv.org/abs/2006.08195) by Liu Ziyin, Tilman Hartwig, Masahito Ueda
-
-This is a PyTorch implementation of the `snake` activation function from the paper - or at least I _think_ it is, no affiliation with the authors, use at your own risk, etc., etc.
-
-A few variations of the function are discussed in the paper, this package implements:
-
- <img src="https://render.githubusercontent.com/render/math?math=x%2B\frac{1}{a}sin^{2}(ax)">
- 
-Snake is **periodic**, but _also_ monotonic. To see how **snake** behaves for a range of x given various choices of `a`, watch this video:
-
-[![snake activation function gets wriggly for higher a](http://img.youtube.com/vi/5g7-8mtywuk/0.jpg)](http://www.youtube.com/watch?v=5g7-8mtywuk "Snake Activation")
-
-## Installation
-Two methods:
-- Using **pip**, `pip install torch-snake`
-- To install from source, first clone this repository.  Then, from the main repo folder, run `python setup.py install`
-
-## Usage
-Fairly easy really `from snake.activations import Snake`.  The `Snake` constructor [(code here)](snake/activations.py) has an optional **learnable** parameter alpha which defaults to 1.  The authors of the paper find values between 5 and 50 work quite well for "known-periodic" data, while for better results with non-periodic data, you should choose a small value like 0.2.  The constructor also takes an `alpha_learnable` parameter which defaults to `True`, so that you can disable "learnability" if your experiments so require.  
-
-## Sample code
-There's a notebook, still quite rough - [example.ipynb](example.ipynb).  Early indications are that good choices of hyperparameters are quite important for best results (though snake's own parameter trains quite readily).
-
-
-## Acknowledgements
-This code probably wouldn't have gotten written if it hadn't been for [Alexandra Deis](https://towardsdatascience.com/@astakhova.aleksandra) and [her excellent article](https://towardsdatascience.com/extending-pytorch-with-custom-activation-functions-2d8b065ef2fa).  It has also benefitted hugely from generous contributions by [Federico Berto](https://github.com/Juju-botu).
+Metadata-Version: 2.1
+Name: torch-snake
+Version: 1.0.0
+Summary: Sample PyTorch implementation of the snake activation function
+Home-page: https://github.com/EdwardDixon/snake
+Author: Edward Dixon
+Author-email: dixon.edward@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+
+[![PyPI version](https://badge.fury.io/py/torch-snake.svg)](https://badge.fury.io/py/torch-snake)
+
+# Snake
+Based on ["Neural Networks Fail to Learn Periodic Functions and How to Fix It"](https://arxiv.org/abs/2006.08195) by Liu Ziyin, Tilman Hartwig, Masahito Ueda
+
+This is a PyTorch implementation of the `snake` activation function from the paper - or at least I _think_ it is, no affiliation with the authors, use at your own risk, etc., etc.
+
+A few variations of the function are discussed in the paper, this package implements:
+
+ <img src="https://render.githubusercontent.com/render/math?math=x%2B\frac{1}{a}sin^{2}(ax)">
+ 
+Snake is **periodic**, but _also_ monotonic. To see how **snake** behaves for a range of x given various choices of `a`, watch this video:
+
+[![snake activation function gets wriggly for higher a](http://img.youtube.com/vi/5g7-8mtywuk/0.jpg)](http://www.youtube.com/watch?v=5g7-8mtywuk "Snake Activation")
+
+## Installation
+Two methods:
+- Using **pip**, `pip install torch-snake`
+- To install from source, first clone this repository.  Then, from the main repo folder, run `python setup.py install`
+
+## Usage
+Fairly easy really `from snake.activations import Snake`.  The `Snake` constructor [(code here)](snake/activations.py) has an optional **learnable** parameter alpha which defaults to 1.  The authors of the paper find values between 5 and 50 work quite well for "known-periodic" data, while for better results with non-periodic data, you should choose a small value like 0.2.  The constructor also takes an `alpha_learnable` parameter which defaults to `True`, so that you can disable "learnability" if your experiments so require.  
+
+## Sample code
+There's a notebook, still quite rough - [example.ipynb](example.ipynb).  Early indications are that good choices of hyperparameters are quite important for best results (though snake's own parameter trains quite readily).
+
+
+## Acknowledgements
+This code probably wouldn't have gotten written if it hadn't been for [Alexandra Deis](https://towardsdatascience.com/@astakhova.aleksandra) and [her excellent article](https://towardsdatascience.com/extending-pytorch-with-custom-activation-functions-2d8b065ef2fa) .
```

### Comparing `torch-snake-0.1.0/setup.py` & `torch-snake-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="torch-snake", # Replace with your own username
-    version="0.1.0",
-    author="Edward Dixon",
-    author_email="dixon.edward@gmail.com",
-    description="Sample PyTorch implementation of the snake activation function",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/EdwardDixon/snake",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=[
-        'torch',
-      ],
-    python_requires='>=3.6',
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="torch-snake", # Replace with your own username
+    version="1.0.0",
+    author="Edward Dixon",
+    author_email="dixon.edward@gmail.com",
+    description="Sample PyTorch implementation of the snake activation function",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/EdwardDixon/snake",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=[
+        'torch',
+      ],
+    python_requires='>=3.6',
 )
```

### Comparing `torch-snake-0.1.0/torch_snake.egg-info/PKG-INFO` & `torch-snake-1.0.0/torch_snake.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1
-Name: torch-snake
-Version: 0.1.0
-Summary: Sample PyTorch implementation of the snake activation function
-Home-page: https://github.com/EdwardDixon/snake
-Author: Edward Dixon
-Author-email: dixon.edward@gmail.com
-License: UNKNOWN
-Description: [![PyPI version](https://badge.fury.io/py/torch-snake.svg)](https://badge.fury.io/py/torch-snake)
-        
-        # Snake
-        Based on ["Neural Networks Fail to Learn Periodic Functions and How to Fix It"](https://arxiv.org/abs/2006.08195) by Liu Ziyin, Tilman Hartwig, Masahito Ueda
-        
-        This is a PyTorch implementation of the `snake` activation function from the paper - or at least I _think_ it is, no affiliation with the authors, use at your own risk, etc., etc.
-        
-        A few variations of the function are discussed in the paper, this package implements:
-        
-         <img src="https://render.githubusercontent.com/render/math?math=x%2B\frac{1}{a}sin^{2}(ax)">
-         
-        Snake is **periodic**, but _also_ monotonic. To see how **snake** behaves for a range of x given various choices of `a`, watch this video:
-        
-        [![snake activation function gets wriggly for higher a](http://img.youtube.com/vi/5g7-8mtywuk/0.jpg)](http://www.youtube.com/watch?v=5g7-8mtywuk "Snake Activation")
-        
-        ## Installation
-        Two methods:
-        - Using **pip**, `pip install torch-snake`
-        - To install from source, first clone this repository.  Then, from the main repo folder, run `python setup.py install`
-        
-        ## Usage
-        Fairly easy really `from snake.activations import Snake`.  The `Snake` constructor [(code here)](snake/activations.py) has an optional **learnable** parameter alpha which defaults to 1.  The authors of the paper find values between 5 and 50 work quite well for "known-periodic" data, while for better results with non-periodic data, you should choose a small value like 0.2.  The constructor also takes an `alpha_learnable` parameter which defaults to `True`, so that you can disable "learnability" if your experiments so require.  
-        
-        ## Sample code
-        There's a notebook, still quite rough - [example.ipynb](example.ipynb).  Early indications are that good choices of hyperparameters are quite important for best results (though snake's own parameter trains quite readily).
-        
-        
-        ## Acknowledgements
-        This code probably wouldn't have gotten written if it hadn't been for [Alexandra Deis](https://towardsdatascience.com/@astakhova.aleksandra) and [her excellent article](https://towardsdatascience.com/extending-pytorch-with-custom-activation-functions-2d8b065ef2fa).  It has also benefitted hugely from generous contributions by [Federico Berto](https://github.com/Juju-botu).
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: torch-snake
+Version: 1.0.0
+Summary: Sample PyTorch implementation of the snake activation function
+Home-page: https://github.com/EdwardDixon/snake
+Author: Edward Dixon
+Author-email: dixon.edward@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+
+[![PyPI version](https://badge.fury.io/py/torch-snake.svg)](https://badge.fury.io/py/torch-snake)
+
+# Snake
+Based on ["Neural Networks Fail to Learn Periodic Functions and How to Fix It"](https://arxiv.org/abs/2006.08195) by Liu Ziyin, Tilman Hartwig, Masahito Ueda
+
+This is a PyTorch implementation of the `snake` activation function from the paper - or at least I _think_ it is, no affiliation with the authors, use at your own risk, etc., etc.
+
+A few variations of the function are discussed in the paper, this package implements:
+
+ <img src="https://render.githubusercontent.com/render/math?math=x%2B\frac{1}{a}sin^{2}(ax)">
+ 
+Snake is **periodic**, but _also_ monotonic. To see how **snake** behaves for a range of x given various choices of `a`, watch this video:
+
+[![snake activation function gets wriggly for higher a](http://img.youtube.com/vi/5g7-8mtywuk/0.jpg)](http://www.youtube.com/watch?v=5g7-8mtywuk "Snake Activation")
+
+## Installation
+Two methods:
+- Using **pip**, `pip install torch-snake`
+- To install from source, first clone this repository.  Then, from the main repo folder, run `python setup.py install`
+
+## Usage
+Fairly easy really `from snake.activations import Snake`.  The `Snake` constructor [(code here)](snake/activations.py) has an optional **learnable** parameter alpha which defaults to 1.  The authors of the paper find values between 5 and 50 work quite well for "known-periodic" data, while for better results with non-periodic data, you should choose a small value like 0.2.  The constructor also takes an `alpha_learnable` parameter which defaults to `True`, so that you can disable "learnability" if your experiments so require.  
+
+## Sample code
+There's a notebook, still quite rough - [example.ipynb](example.ipynb).  Early indications are that good choices of hyperparameters are quite important for best results (though snake's own parameter trains quite readily).
+
+
+## Acknowledgements
+This code probably wouldn't have gotten written if it hadn't been for [Alexandra Deis](https://towardsdatascience.com/@astakhova.aleksandra) and [her excellent article](https://towardsdatascience.com/extending-pytorch-with-custom-activation-functions-2d8b065ef2fa) .
```

