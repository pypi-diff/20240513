# Comparing `tmp/labelme2datasets-0.0.2.tar.gz` & `tmp/labelme2datasets-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelme2datasets-0.0.2.tar", last modified: Sun Nov 21 13:00:24 2021, max compression
+gzip compressed data, was "labelme2datasets-0.0.3.tar", last modified: Mon May 13 03:52:52 2024, max compression
```

## Comparing `labelme2datasets-0.0.2.tar` & `labelme2datasets-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 13:00:24.551655 labelme2datasets-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10405 2021-11-21 13:00:24.551655 labelme2datasets-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9931 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 13:00:24.551655 labelme2datasets-0.0.2/labelme2datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/labelme2datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8705 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/labelme2datasets/labelme_bbox_json2voc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3578 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/labelme2datasets/labelme_json2dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/labelme2datasets/split_voc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/labelme2datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6223 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/labelme2datasets/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 13:00:24.551655 labelme2datasets-0.0.2/labelme2datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10405 2021-11-21 13:00:24.000000 labelme2datasets-0.0.2/labelme2datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-11-21 13:00:24.000000 labelme2datasets-0.0.2/labelme2datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-21 13:00:24.000000 labelme2datasets-0.0.2/labelme2datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-11-21 13:00:24.000000 labelme2datasets-0.0.2/labelme2datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-11-21 13:00:24.000000 labelme2datasets-0.0.2/labelme2datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-21 13:00:24.000000 labelme2datasets-0.0.2/labelme2datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-21 13:00:24.551655 labelme2datasets-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-11-21 13:00:14.000000 labelme2datasets-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:52:52.207692 labelme2datasets-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-13 03:52:52.207692 labelme2datasets-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:52:52.203692 labelme2datasets-0.0.3/labelme2datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/labelme2datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/labelme2datasets/labelme_bbox_json2voc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/labelme2datasets/labelme_json2dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/labelme2datasets/split_voc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/labelme2datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/labelme2datasets/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/labelme2datasets/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:52:52.207692 labelme2datasets-0.0.3/labelme2datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-13 03:52:52.000000 labelme2datasets-0.0.3/labelme2datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 03:52:52.000000 labelme2datasets-0.0.3/labelme2datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 03:52:52.000000 labelme2datasets-0.0.3/labelme2datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-13 03:52:52.000000 labelme2datasets-0.0.3/labelme2datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 03:52:52.000000 labelme2datasets-0.0.3/labelme2datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 03:52:52.000000 labelme2datasets-0.0.3/labelme2datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 03:52:52.207692 labelme2datasets-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-13 03:52:05.000000 labelme2datasets-0.0.3/setup.py
```

### Comparing `labelme2datasets-0.0.2/LICENSE` & `labelme2datasets-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `labelme2datasets-0.0.2/PKG-INFO` & `labelme2datasets-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: labelme2datasets
-Version: 0.0.2
+Version: 0.0.3
 Summary: python scripts to convert labelme-generated-jsons to voc/coco style datasets.
 Home-page: https://github.com/veraposeidon/labelme2Datasets
 Author: veraposeidon
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: imgviz~=1.7.5
+Requires-Dist: labelme~=5.4.1
+Requires-Dist: progressbar~=2.5
+Requires-Dist: scikit-learn~=1.4.2
+Requires-Dist: xmltodict~=0.13.0
+Requires-Dist: setuptools~=69.5.1
+Requires-Dist: pillow~=10.3.0
+Requires-Dist: lxml~=5.2.1
 
 <div id="top"></div>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -27,17 +34,19 @@
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
 *** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
-[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml/badge.svg?branch=opensourceJourney)](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml)
-[![codebeat badge](https://codebeat.co/badges/5f99fcd3-c3a5-4154-91ca-4bb58b32bd53)](https://codebeat.co/projects/github-com-veraposeidon-labelme2datasets-opensourcejourney)
-[![english][en-sheild]][en-url]
+[![PyPI](https://img.shields.io/pypi/v/labelme2datasets.svg)](https://pypi.python.org/pypi/labelme2datasets)
+[![PythonVersion](https://img.shields.io/pypi/pyversions/labelme2datasets.svg)](https://pypi.org/project/labelme2datasets)
+[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml/badge.svg)](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml)
+[![codebeat badge](https://codebeat.co/badges/ab6b3bb6-213b-4a4f-ac55-277dd2840f28)](https://codebeat.co/projects/github-com-veraposeidon-labelme2datasets-main)
+[![chinese][zh-sheild]][zh-url]
 <br />
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 
@@ -50,24 +59,24 @@
   <a href="https://github.com/veraposeidon/labelme2Datasets">
     <img src="images/logo.png" alt="Logo" width="80" height="80">
   </a>
 
 <h3 align="center">labelme2Datasets</h3>
 
   <p align="center">
-    python scripts to convert labelme-generated-jsons to voc/coco style datasets.
+    用于将 LabelMe 标注的数据转换为 VOC 格式和 COCO 格式的数据集。
     <br />
     <a href="https://github.com/veraposeidon/labelme2Datasets/issues">Report Bug</a>
     ·
     <a href="https://github.com/veraposeidon/labelme2Datasets/issues">Request Feature</a>
   </p>
 </div>
 
 
-[（中文 README）](https://github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.zh.md)
+[English README Available](https://github.com/veraposeidon/labelme2Datasets//blob/main/README.en.md)
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
@@ -91,23 +100,23 @@
   </ol>
 </details>
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-Scripts in this repository are used to convert [labelme](https://github.com/wkentaro/labelme)-annotated jsons into standard datasets in [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) format or [MS COCO](https://cocodataset.org/#home) format.
+仓库中的脚本用于将 [labelme](https://github.com/wkentaro/labelme) 标注的数据转换为 [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) 格式和 [MS COCO](https://cocodataset.org/#home) 格式的数据集，便于直接利用支持这两种格式的框架进行训练。
 
-Scripts are written in [Python](https://www.python.org/).
+脚本都使用 [Python](https://www.python.org/) 写的。
 
-Most of the scripts refer to the [examples](https://github.com/wkentaro/labelme/tree/main/examples) section of labelme. Then I add some features according my own dataset, like class name conversion, customise image name, etc.
+大部分的脚步都是参考的 labelme 项目中的 [examples](https://github.com/wkentaro/labelme/tree/main/examples) 内容。然后添加一些根据自己的数据集自定义的功能，比如标签转换、自定义图像名称等。
 
-**Attention**: these scripts are not complicated, and if you have the basis of python, please go through the convert workflows, and ensure that it fits your datasets. There are some places I annotated `MARK`, which means pay attention to it, and you could customize it to fit your needs.
+**注意**：这些脚本其实并不复杂，有 Python 基础的同学可以过一遍转换的流程，确保在你的数据集上是可以正常运行的。有一些地方我标注了 `MARK`，表示在这些地方需要留意，可以根据自己的需要进行修改。
 
-**Customize**: these scripts are only for the conversion of data I currently have. If you want to convert datasets in other areas, like instance segmentation, segmantic segmentation, video annotation, etc. please take a look at the [examples](https://github.com/wkentaro/labelme/tree/main/examples) section in labelme.
+**拓展**：这些脚本当时只是用来转换我自己的数据集。如果你需要转换其他领域的数据集，比如实例分割、语义分割或者视频标注等等。建议去 lebelme 的 [examples](https://github.com/wkentaro/labelme/tree/main/examples) 部分看看，作者提供了一些示例代码，可以参考。
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 ### Built With
 
@@ -120,113 +129,106 @@
 
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 ### Prerequisites
 
-1. gather the labelme-annotated jsons into a folder. In the next steps, we will refer to this folder as `labelme_jsons_dir`.
+1. 将 lebelme 标注得到的 JSON 文件放在一个文件夹内。举个例子，命名为 `labelme_jsons_dir`。
 
-2. prepare a text file to store class names in your dataset. named it `label_names.txt`. take a look at `test/label_names.txt` for an example.
+2. 准备好一份 text 文本，里面包含数据集的分类标签。举个例子，命名为  `label_names.txt`。可以参考下项目里的 `test/label_names.txt`。
 
-3. if need class name conversion, prepare a text file to store the conversion rules. named it `label_dict.txt`. take a look at `test/label_dict.txt` for an example.
+3. 如果有转换标签的需求（比如中文标签转为英文），准备一个文本，包含转换的规则，举个例子，命名为`label_dict.txt`。可以参考下项目里的 `test/label_dict.txt` 。
 ### Installation
-
-#### install in develop mode
-1. suggested to use virtualenv to install python packages.
+#### develop mode 安装
+1. 建议使用虚拟环境安装 Python Package。
   
     ```sh
-    conda create --name=labelme python=3.6
+    conda create --name=labelme python=3.9
     conda activate labelme
     pip install -r requirements.txt
     ```
-2. clone the repo.
+2. 克隆仓库。
     ```sh
     git clone git@github.com:veraposeidon/labelme2Datasets.git
     ```
-3. install the package
+3. 本地安装
    ```sh
     cd labelme2Datasets
-    # (prefer this way!) install in editable mode, so that you can modify the package 
+    # （推荐）可编辑模式安装，即可以修改代码
     pip install -e .
-    # install in non-editable mode, so that you can use the package, but cannot modify it
+    # 第二种安装方式，可以直接运行脚本，但是不能修改代码
     #python setup.py install
    ```
    
-#### simply use PyPI
-
-I also published a PyPI package named [labelme2datasets](https://pypi.org/project/labelme2datasets/).
+#### 直接使用 PyPI
 
-you can just use `pip3 install labelme2datasets` to install this package.
+同时发布了一个 PyPI package，[labelme2datasets](https://pypi.org/project/labelme2datasets/)。
 
-if the baseline in this project not work for your datasets, you can install in develop mode, and modify the code by your own.
+可以直接使用 `pip3 install labelme2datasets` 进行安装。
 
+如果项目中的流程不适用于你的数据集，建议通过上述 develop mode 安装和修改代码。
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-- convert a single json into dataset. (`labelme_json2dataset.py`)
-    ```shell
-    labelme_json2dataset --json_file=data/test.json \
+- 转换单个 JSON 文件。 (`labelme_json2dataset.py`)
+    ```sh
+    labelme_json2dataset --json_file=data/sample.json \
       --output_dir=output/test_single_output
     ```
 
-- convert a folder of jsons into voc-format dataset. (`labelme_bbox_json2voc.py`)
-  - without label conversion
-    ```shell
-    labelme_bbox_json2voc --json_dir=data/test_jsons \
+- 转换 JSON 文件夹`labelme_jsons_dir` 到  VOC 格式的数据集。 (`labelme_bbox_json2voc.py`)
+  - 不需要标签转换
+    ```sh
+    labelme_bbox_json2voc --json_dir=data/sample_jsons \
       --output_dir=output/test_voc_output --labels data/label_names.txt
     ```
-  - with label conversion
-    ```shell
-    labelme_bbox_json2voc --json_dir=data/test_jsons \
+  - 需要标签转换
+    ```sh
+    labelme_bbox_json2voc --json_dir=data/sample_jsons \
       --output_dir=output/test_voc_output \
       --labels data/label_names.txt \
       --label_dict data/label_dict.txt
     ```
-- splitting voc datasets into train set and test set. (`split_voc_datasets.py`)
-  ```shell
+- 分割 VOC 数据的训练集和测试集。 (`split_voc_datasets.py`)
+  ```sh
     split_voc_datasets --voc_dir output/test_voc_output --test_ratio 0.3 --random_seed 42
   ```
-  `train.txt` and `test.txt` should be generated in `voc_dir/ImageSets/Main/`.
+  `train.txt` 和 `test.txt` 会出现在 `voc_dir/ImageSets/Main/` 文件夹下。
 
-- turn voc format dataset into coco style dataset. (`voc2coco.py`)
+- 将 VOC 数据集转换为 COCO 数据集 (`voc2coco.py`)
   ```shell
     voc2coco --voc_dir output/test_voc_output --coco_dir output/test_coco_output
   ```
-
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-
-
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] add all scripts with pylint passed
-- [x] chinese and english readme
-- [x] modify project architecture
-- [x] publish as package
+- [x] 将所有的脚本都通过 Pylint
+- [x] 中英文 README
+- [x] 调整项目结构
+- [x] 发布 Pypi 包
 
 See the [open issues](https://github.com/veraposeidon/labelme2Datasets/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
+如果你有什么建议可以让这个项目变得更好，可以 Fork 项目并且提交 Pull Request。
+也可以简单地在 [issues](https://github.com/veraposeidon/labelme2Datasets/issues) 中开一个 issue。
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
@@ -262,22 +264,20 @@
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[en-sheild]:https://img.shields.io/badge/language-english-blue
-[en-url]:https://github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.md
+[zh-sheild]:https://img.shields.io/badge/language-chinese-red
+[zh-url]:https://github.com/veraposeidon/labelme2Datasets//blob/main/README.md
 [contributors-shield]: https://img.shields.io/github/contributors/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [contributors-url]: https://github.com/veraposeidon/labelme2Datasets/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [forks-url]: https://github.com/veraposeidon/labelme2Datasets/network/members
 [stars-shield]: https://img.shields.io/github/stars/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [stars-url]: https://github.com/veraposeidon/labelme2Datasets/stargazers
 [issues-shield]: https://img.shields.io/github/issues/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [issues-url]: https://github.com/veraposeidon/labelme2Datasets/issues
 [license-shield]: https://img.shields.io/github/license/veraposeidon/labelme2Datasets.svg?style=for-the-badge
-[license-url]: https://github.com/veraposeidon/labelme2Datasets/blob/opensourceJourney/LICENSE
+[license-url]: https://github.com/veraposeidon/labelme2Datasets/blob/main/LICENSE
 [product-screenshot]: images/screenshot.png
-
-
```

#### html2text {}

```diff
@@ -1,128 +1,133 @@
-Metadata-Version: 2.1 Name: labelme2datasets Version: 0.0.2 Summary: python
+Metadata-Version: 2.1 Name: labelme2datasets Version: 0.0.3 Summary: python
 scripts to convert labelme-generated-jsons to voc/coco style datasets. Home-
 page: https://github.com/veraposeidon/labelme2Datasets Author: veraposeidon
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Description-Content-Type: text/markdown License-File:
-LICENSE
-[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/
-pylint.yml/badge.svg?branch=opensourceJourney)](https://github.com/
-veraposeidon/labelme2Datasets/actions/workflows/pylint.yml) [![codebeat badge]
-(https://codebeat.co/badges/5f99fcd3-c3a5-4154-91ca-4bb58b32bd53)](https://
-codebeat.co/projects/github-com-veraposeidon-labelme2datasets-
-opensourcejourney) [![english][en-sheild]][en-url]
+Classifier: Programming Language :: Python :: 3.9 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+beautifulsoup4~=4.12.3 Requires-Dist: imgviz~=1.7.5 Requires-Dist:
+labelme~=5.4.1 Requires-Dist: progressbar~=2.5 Requires-Dist: scikit-
+learn~=1.4.2 Requires-Dist: xmltodict~=0.13.0 Requires-Dist: setuptools~=69.5.1
+Requires-Dist: pillow~=10.3.0 Requires-Dist: lxml~=5.2.1
+[![PyPI](https://img.shields.io/pypi/v/labelme2datasets.svg)](https://
+pypi.python.org/pypi/labelme2datasets) [![PythonVersion](https://
+img.shields.io/pypi/pyversions/labelme2datasets.svg)](https://pypi.org/project/
+labelme2datasets) [![Pylint](https://github.com/veraposeidon/labelme2Datasets/
+actions/workflows/pylint.yml/badge.svg)](https://github.com/veraposeidon/
+labelme2Datasets/actions/workflows/pylint.yml) [![codebeat badge](https://
+codebeat.co/badges/ab6b3bb6-213b-4a4f-ac55-277dd2840f28)](https://codebeat.co/
+projects/github-com-veraposeidon-labelme2datasets-main) [![chinese][zh-sheild]]
+[zh-url]
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
 shield]][issues-url] [![MIT License][license-shield]][license-url]
                                     _[_L_o_g_o_]
                           ******** llaabbeellmmee22DDaattaasseettss ********
-python scripts to convert labelme-generated-jsons to voc/coco style datasets.
+         ç¨äºå° LabelMe æ æ³¨çæ°æ®è½¬æ¢ä¸º VOC æ ¼å¼å COCO
+                            æ ¼å¼çæ°æ®éã
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
-[ï¼ä¸­æ READMEï¼](https://github.com/veraposeidon/labelme2Datasets//blob/
-opensourceJourney/README.zh.md) Table of Contents
+[English README Available](https://github.com/veraposeidon/labelme2Datasets//
+blob/main/README.en.md) Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _L_i_c_e_n_s_e
    7. _C_o_n_t_a_c_t
    8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
-## About The Project Scripts in this repository are used to convert [labelme]
-(https://github.com/wkentaro/labelme)-annotated jsons into standard datasets in
-[PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) format or [MS COCO]
-(https://cocodataset.org/#home) format. Scripts are written in [Python](https:/
-/www.python.org/). Most of the scripts refer to the [examples](https://
-github.com/wkentaro/labelme/tree/main/examples) section of labelme. Then I add
-some features according my own dataset, like class name conversion, customise
-image name, etc. **Attention**: these scripts are not complicated, and if you
-have the basis of python, please go through the convert workflows, and ensure
-that it fits your datasets. There are some places I annotated `MARK`, which
-means pay attention to it, and you could customize it to fit your needs.
-**Customize**: these scripts are only for the conversion of data I currently
-have. If you want to convert datasets in other areas, like instance
-segmentation, segmantic segmentation, video annotation, etc. please take a look
-at the [examples](https://github.com/wkentaro/labelme/tree/main/examples)
-section in labelme.
+## About The Project ä»åºä¸­çèæ¬ç¨äºå° [labelme](https://github.com/
+wkentaro/labelme) æ æ³¨çæ°æ®è½¬æ¢ä¸º [PASCAL VOC](http://
+host.robots.ox.ac.uk/pascal/VOC/) æ ¼å¼å [MS COCO](https://cocodataset.org/
+#home)
+æ ¼å¼çæ°æ®éï¼ä¾¿äºç´æ¥å©ç¨æ¯æè¿ä¸¤ç§æ ¼å¼çæ¡æ¶è¿è¡è®­ç»ã
+èæ¬é½ä½¿ç¨ [Python](https://www.python.org/) åçã
+å¤§é¨åçèæ­¥é½æ¯åèç labelme é¡¹ç®ä¸­ç [examples](https://
+github.com/wkentaro/labelme/tree/main/examples)
+åå®¹ãç¶åæ·»å ä¸äºæ ¹æ®èªå·±çæ°æ®éèªå®ä¹çåè½ï¼æ¯å¦æ ç­¾è½¬æ¢ãèªå®ä¹å¾ååç§°ç­ã
+**æ³¨æ**ï¼è¿äºèæ¬å¶å®å¹¶ä¸å¤æï¼æ Python
+åºç¡çåå­¦å¯ä»¥è¿ä¸éè½¬æ¢çæµç¨ï¼ç¡®ä¿å¨ä½ çæ°æ®éä¸æ¯å¯ä»¥æ­£å¸¸è¿è¡çãæä¸äºå°æ¹ææ æ³¨äº
+`MARK`ï¼è¡¨ç¤ºå¨è¿äºå°æ¹éè¦çæï¼å¯ä»¥æ ¹æ®èªå·±çéè¦è¿è¡ä¿®æ¹ã
+**æå±**ï¼è¿äºèæ¬å½æ¶åªæ¯ç¨æ¥è½¬æ¢æèªå·±çæ°æ®éãå¦æä½ éè¦è½¬æ¢å¶ä»é¢åçæ°æ®éï¼æ¯å¦å®ä¾åå²ãè¯­ä¹åå²æèè§é¢æ æ³¨ç­ç­ãå»ºè®®å»
+lebelme ç [examples](https://github.com/wkentaro/labelme/tree/main/examples)
+é¨åççï¼ä½èæä¾äºä¸äºç¤ºä¾ä»£ç ï¼å¯ä»¥åèã
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With * [Python](https://www.python.org/) * [labelme](https://
 github.com/wkentaro/labelme) * [imgviz](https://github.com/wkentaro/imgviz)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started ### Prerequisites 1. gather the labelme-annotated jsons into
-a folder. In the next steps, we will refer to this folder as
-`labelme_jsons_dir`. 2. prepare a text file to store class names in your
-dataset. named it `label_names.txt`. take a look at `test/label_names.txt` for
-an example. 3. if need class name conversion, prepare a text file to store the
-conversion rules. named it `label_dict.txt`. take a look at `test/
-label_dict.txt` for an example. ### Installation #### install in develop mode
-1. suggested to use virtualenv to install python packages. ```sh conda create -
--name=labelme python=3.6 conda activate labelme pip install -r requirements.txt
-``` 2. clone the repo. ```sh git clone git@github.com:veraposeidon/
-labelme2Datasets.git ``` 3. install the package ```sh cd labelme2Datasets #
-(prefer this way!) install in editable mode, so that you can modify the package
-pip install -e . # install in non-editable mode, so that you can use the
-package, but cannot modify it #python setup.py install ``` #### simply use PyPI
-I also published a PyPI package named [labelme2datasets](https://pypi.org/
-project/labelme2datasets/). you can just use `pip3 install labelme2datasets` to
-install this package. if the baseline in this project not work for your
-datasets, you can install in develop mode, and modify the code by your own.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage - convert a single json into dataset. (`labelme_json2dataset.py`)
-```shell labelme_json2dataset --json_file=data/test.json \ --output_dir=output/
-test_single_output ``` - convert a folder of jsons into voc-format dataset.
-(`labelme_bbox_json2voc.py`) - without label conversion ```shell
-labelme_bbox_json2voc --json_dir=data/test_jsons \ --output_dir=output/
-test_voc_output --labels data/label_names.txt ``` - with label conversion
-```shell labelme_bbox_json2voc --json_dir=data/test_jsons \ --
-output_dir=output/test_voc_output \ --labels data/label_names.txt \ --
-label_dict data/label_dict.txt ``` - splitting voc datasets into train set and
-test set. (`split_voc_datasets.py`) ```shell split_voc_datasets --voc_dir
-output/test_voc_output --test_ratio 0.3 --random_seed 42 ``` `train.txt` and
-`test.txt` should be generated in `voc_dir/ImageSets/Main/`. - turn voc format
-dataset into coco style dataset. (`voc2coco.py`) ```shell voc2coco --voc_dir
+## Getting Started ### Prerequisites 1. å° lebelme æ æ³¨å¾å°ç JSON
+æä»¶æ¾å¨ä¸ä¸ªæä»¶å¤¹åãä¸¾ä¸ªä¾å­ï¼å½åä¸º
+`labelme_jsons_dir`ã 2. åå¤å¥½ä¸ä»½ text
+ææ¬ï¼éé¢åå«æ°æ®éçåç±»æ ç­¾ãä¸¾ä¸ªä¾å­ï¼å½åä¸º
+`label_names.txt`ãå¯ä»¥åèä¸é¡¹ç®éç `test/label_names.txt`ã 3.
+å¦ææè½¬æ¢æ ç­¾çéæ±ï¼æ¯å¦ä¸­ææ ç­¾è½¬ä¸ºè±æï¼ï¼åå¤ä¸ä¸ªææ¬ï¼åå«è½¬æ¢çè§åï¼ä¸¾ä¸ªä¾å­ï¼å½åä¸º`label_dict.txt`ãå¯ä»¥åèä¸é¡¹ç®éç
+`test/label_dict.txt` ã ### Installation #### develop mode å®è£ 1.
+å»ºè®®ä½¿ç¨èæç¯å¢å®è£ Python Packageã ```sh conda create --
+name=labelme python=3.9 conda activate labelme pip install -r requirements.txt
+``` 2. åéä»åºã ```sh git clone git@github.com:veraposeidon/
+labelme2Datasets.git ``` 3. æ¬å°å®è£ ```sh cd labelme2Datasets #
+ï¼æ¨èï¼å¯ç¼è¾æ¨¡å¼å®è£ï¼å³å¯ä»¥ä¿®æ¹ä»£ç  pip install -e . #
+ç¬¬äºç§å®è£æ¹å¼ï¼å¯ä»¥ç´æ¥è¿è¡èæ¬ï¼ä½æ¯ä¸è½ä¿®æ¹ä»£ç 
+#python setup.py install ``` #### ç´æ¥ä½¿ç¨ PyPI åæ¶åå¸äºä¸ä¸ª PyPI
+packageï¼[labelme2datasets](https://pypi.org/project/labelme2datasets/)ã
+å¯ä»¥ç´æ¥ä½¿ç¨ `pip3 install labelme2datasets` è¿è¡å®è£ã
+å¦æé¡¹ç®ä¸­çæµç¨ä¸éç¨äºä½ çæ°æ®éï¼å»ºè®®éè¿ä¸è¿°
+develop mode å®è£åä¿®æ¹ä»£ç ã
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Usage - è½¬æ¢åä¸ª JSON æä»¶ã (`labelme_json2dataset.py`) ```sh
+labelme_json2dataset --json_file=data/sample.json \ --output_dir=output/
+test_single_output ``` - è½¬æ¢ JSON æä»¶å¤¹`labelme_jsons_dir` å° VOC
+æ ¼å¼çæ°æ®éã (`labelme_bbox_json2voc.py`) - ä¸éè¦æ ç­¾è½¬æ¢
+```sh labelme_bbox_json2voc --json_dir=data/sample_jsons \ --output_dir=output/
+test_voc_output --labels data/label_names.txt ``` - éè¦æ ç­¾è½¬æ¢ ```sh
+labelme_bbox_json2voc --json_dir=data/sample_jsons \ --output_dir=output/
+test_voc_output \ --labels data/label_names.txt \ --label_dict data/
+label_dict.txt ``` - åå² VOC æ°æ®çè®­ç»éåæµè¯éã
+(`split_voc_datasets.py`) ```sh split_voc_datasets --voc_dir output/
+test_voc_output --test_ratio 0.3 --random_seed 42 ``` `train.txt` å
+`test.txt` ä¼åºç°å¨ `voc_dir/ImageSets/Main/` æä»¶å¤¹ä¸ã - å° VOC
+æ°æ®éè½¬æ¢ä¸º COCO æ°æ®é (`voc2coco.py`) ```shell voc2coco --voc_dir
 output/test_voc_output --coco_dir output/test_coco_output ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] add all scripts with pylint passed - [x] chinese and english
-readme - [x] modify project architecture - [x] publish as package See the [open
-issues](https://github.com/veraposeidon/labelme2Datasets/issues) for a full
-list of proposed features (and known issues).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Contributing Contributions are what make the open source community such an
-amazing place to learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. If you have a suggestion that would make this better,
-please fork the repo and create a pull request. You can also simply open an
-issue with the tag "enhancement". Don't forget to give the project a star!
-Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
--b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
+## Roadmap - [x] å°ææçèæ¬é½éè¿ Pylint - [x] ä¸­è±æ README -
+[x] è°æ´é¡¹ç®ç»æ - [x] åå¸ Pypi å See the [open issues](https://
+github.com/veraposeidon/labelme2Datasets/issues) for a full list of proposed
+features (and known issues).
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Contributing
+å¦æä½ æä»ä¹å»ºè®®å¯ä»¥è®©è¿ä¸ªé¡¹ç®åå¾æ´å¥½ï¼å¯ä»¥ Fork
+é¡¹ç®å¹¶ä¸æäº¤ Pull Requestã ä¹å¯ä»¥ç®åå°å¨ [issues](https://
+github.com/veraposeidon/labelme2Datasets/issues) ä¸­å¼ä¸ä¸ª issueã 1. Fork
+the Project 2. Create your Feature Branch (`git checkout -b feature/
+AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
 information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact veraposeidon - veraposeidon@gmail.com Project Link: [https://
 github.com/veraposeidon/labelme2Datasets](https://github.com/veraposeidon/
 labelme2Datasets)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments * [labelme](https://github.com/wkentaro/labelme) *
 [labelme2coco](https://github.com/fcakyon/labelme2coco)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-[en-sheild]:https://img.shields.io/badge/language-english-blue [en-url]:https:/
-/github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.md
-[contributors-shield]: https://img.shields.io/github/contributors/veraposeidon/
+[zh-sheild]:https://img.shields.io/badge/language-chinese-red [zh-url]:https://
+github.com/veraposeidon/labelme2Datasets//blob/main/README.md [contributors-
+shield]: https://img.shields.io/github/contributors/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [contributors-url]: https://
 github.com/veraposeidon/labelme2Datasets/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [forks-url]: https://github.com/
 veraposeidon/labelme2Datasets/network/members [stars-shield]: https://
 img.shields.io/github/stars/veraposeidon/labelme2Datasets.svg?style=for-the-
 badge [stars-url]: https://github.com/veraposeidon/labelme2Datasets/stargazers
 [issues-shield]: https://img.shields.io/github/issues/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [issues-url]: https://github.com/
 veraposeidon/labelme2Datasets/issues [license-shield]: https://img.shields.io/
 github/license/veraposeidon/labelme2Datasets.svg?style=for-the-badge [license-
-url]: https://github.com/veraposeidon/labelme2Datasets/blob/opensourceJourney/
-LICENSE [product-screenshot]: images/screenshot.png
+url]: https://github.com/veraposeidon/labelme2Datasets/blob/main/LICENSE
+[product-screenshot]: images/screenshot.png
```

### Comparing `labelme2datasets-0.0.2/README.md` & `labelme2datasets-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
 *** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
-[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml/badge.svg?branch=opensourceJourney)](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml)
-[![codebeat badge](https://codebeat.co/badges/5f99fcd3-c3a5-4154-91ca-4bb58b32bd53)](https://codebeat.co/projects/github-com-veraposeidon-labelme2datasets-opensourcejourney)
-[![english][en-sheild]][en-url]
+[![PyPI](https://img.shields.io/pypi/v/labelme2datasets.svg)](https://pypi.python.org/pypi/labelme2datasets)
+[![PythonVersion](https://img.shields.io/pypi/pyversions/labelme2datasets.svg)](https://pypi.org/project/labelme2datasets)
+[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml/badge.svg)](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml)
+[![codebeat badge](https://codebeat.co/badges/ab6b3bb6-213b-4a4f-ac55-277dd2840f28)](https://codebeat.co/projects/github-com-veraposeidon-labelme2datasets-main)
+[![chinese][zh-sheild]][zh-url]
 <br />
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 
@@ -36,24 +38,24 @@
   <a href="https://github.com/veraposeidon/labelme2Datasets">
     <img src="images/logo.png" alt="Logo" width="80" height="80">
   </a>
 
 <h3 align="center">labelme2Datasets</h3>
 
   <p align="center">
-    python scripts to convert labelme-generated-jsons to voc/coco style datasets.
+    用于将 LabelMe 标注的数据转换为 VOC 格式和 COCO 格式的数据集。
     <br />
     <a href="https://github.com/veraposeidon/labelme2Datasets/issues">Report Bug</a>
     ·
     <a href="https://github.com/veraposeidon/labelme2Datasets/issues">Request Feature</a>
   </p>
 </div>
 
 
-[（中文 README）](https://github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.zh.md)
+[English README Available](https://github.com/veraposeidon/labelme2Datasets//blob/main/README.en.md)
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
@@ -77,23 +79,23 @@
   </ol>
 </details>
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-Scripts in this repository are used to convert [labelme](https://github.com/wkentaro/labelme)-annotated jsons into standard datasets in [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) format or [MS COCO](https://cocodataset.org/#home) format.
+仓库中的脚本用于将 [labelme](https://github.com/wkentaro/labelme) 标注的数据转换为 [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) 格式和 [MS COCO](https://cocodataset.org/#home) 格式的数据集，便于直接利用支持这两种格式的框架进行训练。
 
-Scripts are written in [Python](https://www.python.org/).
+脚本都使用 [Python](https://www.python.org/) 写的。
 
-Most of the scripts refer to the [examples](https://github.com/wkentaro/labelme/tree/main/examples) section of labelme. Then I add some features according my own dataset, like class name conversion, customise image name, etc.
+大部分的脚步都是参考的 labelme 项目中的 [examples](https://github.com/wkentaro/labelme/tree/main/examples) 内容。然后添加一些根据自己的数据集自定义的功能，比如标签转换、自定义图像名称等。
 
-**Attention**: these scripts are not complicated, and if you have the basis of python, please go through the convert workflows, and ensure that it fits your datasets. There are some places I annotated `MARK`, which means pay attention to it, and you could customize it to fit your needs.
+**注意**：这些脚本其实并不复杂，有 Python 基础的同学可以过一遍转换的流程，确保在你的数据集上是可以正常运行的。有一些地方我标注了 `MARK`，表示在这些地方需要留意，可以根据自己的需要进行修改。
 
-**Customize**: these scripts are only for the conversion of data I currently have. If you want to convert datasets in other areas, like instance segmentation, segmantic segmentation, video annotation, etc. please take a look at the [examples](https://github.com/wkentaro/labelme/tree/main/examples) section in labelme.
+**拓展**：这些脚本当时只是用来转换我自己的数据集。如果你需要转换其他领域的数据集，比如实例分割、语义分割或者视频标注等等。建议去 lebelme 的 [examples](https://github.com/wkentaro/labelme/tree/main/examples) 部分看看，作者提供了一些示例代码，可以参考。
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 ### Built With
 
@@ -106,113 +108,106 @@
 
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 ### Prerequisites
 
-1. gather the labelme-annotated jsons into a folder. In the next steps, we will refer to this folder as `labelme_jsons_dir`.
+1. 将 lebelme 标注得到的 JSON 文件放在一个文件夹内。举个例子，命名为 `labelme_jsons_dir`。
 
-2. prepare a text file to store class names in your dataset. named it `label_names.txt`. take a look at `test/label_names.txt` for an example.
+2. 准备好一份 text 文本，里面包含数据集的分类标签。举个例子，命名为  `label_names.txt`。可以参考下项目里的 `test/label_names.txt`。
 
-3. if need class name conversion, prepare a text file to store the conversion rules. named it `label_dict.txt`. take a look at `test/label_dict.txt` for an example.
+3. 如果有转换标签的需求（比如中文标签转为英文），准备一个文本，包含转换的规则，举个例子，命名为`label_dict.txt`。可以参考下项目里的 `test/label_dict.txt` 。
 ### Installation
-
-#### install in develop mode
-1. suggested to use virtualenv to install python packages.
+#### develop mode 安装
+1. 建议使用虚拟环境安装 Python Package。
   
     ```sh
-    conda create --name=labelme python=3.6
+    conda create --name=labelme python=3.9
     conda activate labelme
     pip install -r requirements.txt
     ```
-2. clone the repo.
+2. 克隆仓库。
     ```sh
     git clone git@github.com:veraposeidon/labelme2Datasets.git
     ```
-3. install the package
+3. 本地安装
    ```sh
     cd labelme2Datasets
-    # (prefer this way!) install in editable mode, so that you can modify the package 
+    # （推荐）可编辑模式安装，即可以修改代码
     pip install -e .
-    # install in non-editable mode, so that you can use the package, but cannot modify it
+    # 第二种安装方式，可以直接运行脚本，但是不能修改代码
     #python setup.py install
    ```
    
-#### simply use PyPI
-
-I also published a PyPI package named [labelme2datasets](https://pypi.org/project/labelme2datasets/).
+#### 直接使用 PyPI
 
-you can just use `pip3 install labelme2datasets` to install this package.
+同时发布了一个 PyPI package，[labelme2datasets](https://pypi.org/project/labelme2datasets/)。
 
-if the baseline in this project not work for your datasets, you can install in develop mode, and modify the code by your own.
+可以直接使用 `pip3 install labelme2datasets` 进行安装。
 
+如果项目中的流程不适用于你的数据集，建议通过上述 develop mode 安装和修改代码。
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-- convert a single json into dataset. (`labelme_json2dataset.py`)
-    ```shell
-    labelme_json2dataset --json_file=data/test.json \
+- 转换单个 JSON 文件。 (`labelme_json2dataset.py`)
+    ```sh
+    labelme_json2dataset --json_file=data/sample.json \
       --output_dir=output/test_single_output
     ```
 
-- convert a folder of jsons into voc-format dataset. (`labelme_bbox_json2voc.py`)
-  - without label conversion
-    ```shell
-    labelme_bbox_json2voc --json_dir=data/test_jsons \
+- 转换 JSON 文件夹`labelme_jsons_dir` 到  VOC 格式的数据集。 (`labelme_bbox_json2voc.py`)
+  - 不需要标签转换
+    ```sh
+    labelme_bbox_json2voc --json_dir=data/sample_jsons \
       --output_dir=output/test_voc_output --labels data/label_names.txt
     ```
-  - with label conversion
-    ```shell
-    labelme_bbox_json2voc --json_dir=data/test_jsons \
+  - 需要标签转换
+    ```sh
+    labelme_bbox_json2voc --json_dir=data/sample_jsons \
       --output_dir=output/test_voc_output \
       --labels data/label_names.txt \
       --label_dict data/label_dict.txt
     ```
-- splitting voc datasets into train set and test set. (`split_voc_datasets.py`)
-  ```shell
+- 分割 VOC 数据的训练集和测试集。 (`split_voc_datasets.py`)
+  ```sh
     split_voc_datasets --voc_dir output/test_voc_output --test_ratio 0.3 --random_seed 42
   ```
-  `train.txt` and `test.txt` should be generated in `voc_dir/ImageSets/Main/`.
+  `train.txt` 和 `test.txt` 会出现在 `voc_dir/ImageSets/Main/` 文件夹下。
 
-- turn voc format dataset into coco style dataset. (`voc2coco.py`)
+- 将 VOC 数据集转换为 COCO 数据集 (`voc2coco.py`)
   ```shell
     voc2coco --voc_dir output/test_voc_output --coco_dir output/test_coco_output
   ```
-
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-
-
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] add all scripts with pylint passed
-- [x] chinese and english readme
-- [x] modify project architecture
-- [x] publish as package
+- [x] 将所有的脚本都通过 Pylint
+- [x] 中英文 README
+- [x] 调整项目结构
+- [x] 发布 Pypi 包
 
 See the [open issues](https://github.com/veraposeidon/labelme2Datasets/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
+如果你有什么建议可以让这个项目变得更好，可以 Fork 项目并且提交 Pull Request。
+也可以简单地在 [issues](https://github.com/veraposeidon/labelme2Datasets/issues) 中开一个 issue。
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
@@ -248,20 +243,20 @@
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[en-sheild]:https://img.shields.io/badge/language-english-blue
-[en-url]:https://github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.md
+[zh-sheild]:https://img.shields.io/badge/language-chinese-red
+[zh-url]:https://github.com/veraposeidon/labelme2Datasets//blob/main/README.md
 [contributors-shield]: https://img.shields.io/github/contributors/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [contributors-url]: https://github.com/veraposeidon/labelme2Datasets/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [forks-url]: https://github.com/veraposeidon/labelme2Datasets/network/members
 [stars-shield]: https://img.shields.io/github/stars/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [stars-url]: https://github.com/veraposeidon/labelme2Datasets/stargazers
 [issues-shield]: https://img.shields.io/github/issues/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [issues-url]: https://github.com/veraposeidon/labelme2Datasets/issues
 [license-shield]: https://img.shields.io/github/license/veraposeidon/labelme2Datasets.svg?style=for-the-badge
-[license-url]: https://github.com/veraposeidon/labelme2Datasets/blob/opensourceJourney/LICENSE
+[license-url]: https://github.com/veraposeidon/labelme2Datasets/blob/main/LICENSE
 [product-screenshot]: images/screenshot.png
```

#### html2text {}

```diff
@@ -1,121 +1,123 @@
-[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/
-pylint.yml/badge.svg?branch=opensourceJourney)](https://github.com/
-veraposeidon/labelme2Datasets/actions/workflows/pylint.yml) [![codebeat badge]
-(https://codebeat.co/badges/5f99fcd3-c3a5-4154-91ca-4bb58b32bd53)](https://
-codebeat.co/projects/github-com-veraposeidon-labelme2datasets-
-opensourcejourney) [![english][en-sheild]][en-url]
+[![PyPI](https://img.shields.io/pypi/v/labelme2datasets.svg)](https://
+pypi.python.org/pypi/labelme2datasets) [![PythonVersion](https://
+img.shields.io/pypi/pyversions/labelme2datasets.svg)](https://pypi.org/project/
+labelme2datasets) [![Pylint](https://github.com/veraposeidon/labelme2Datasets/
+actions/workflows/pylint.yml/badge.svg)](https://github.com/veraposeidon/
+labelme2Datasets/actions/workflows/pylint.yml) [![codebeat badge](https://
+codebeat.co/badges/ab6b3bb6-213b-4a4f-ac55-277dd2840f28)](https://codebeat.co/
+projects/github-com-veraposeidon-labelme2datasets-main) [![chinese][zh-sheild]]
+[zh-url]
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
 shield]][issues-url] [![MIT License][license-shield]][license-url]
                                     _[_L_o_g_o_]
                           ******** llaabbeellmmee22DDaattaasseettss ********
-python scripts to convert labelme-generated-jsons to voc/coco style datasets.
+         ç¨äºå° LabelMe æ æ³¨çæ°æ®è½¬æ¢ä¸º VOC æ ¼å¼å COCO
+                            æ ¼å¼çæ°æ®éã
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
-[ï¼ä¸­æ READMEï¼](https://github.com/veraposeidon/labelme2Datasets//blob/
-opensourceJourney/README.zh.md) Table of Contents
+[English README Available](https://github.com/veraposeidon/labelme2Datasets//
+blob/main/README.en.md) Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _L_i_c_e_n_s_e
    7. _C_o_n_t_a_c_t
    8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
-## About The Project Scripts in this repository are used to convert [labelme]
-(https://github.com/wkentaro/labelme)-annotated jsons into standard datasets in
-[PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) format or [MS COCO]
-(https://cocodataset.org/#home) format. Scripts are written in [Python](https:/
-/www.python.org/). Most of the scripts refer to the [examples](https://
-github.com/wkentaro/labelme/tree/main/examples) section of labelme. Then I add
-some features according my own dataset, like class name conversion, customise
-image name, etc. **Attention**: these scripts are not complicated, and if you
-have the basis of python, please go through the convert workflows, and ensure
-that it fits your datasets. There are some places I annotated `MARK`, which
-means pay attention to it, and you could customize it to fit your needs.
-**Customize**: these scripts are only for the conversion of data I currently
-have. If you want to convert datasets in other areas, like instance
-segmentation, segmantic segmentation, video annotation, etc. please take a look
-at the [examples](https://github.com/wkentaro/labelme/tree/main/examples)
-section in labelme.
+## About The Project ä»åºä¸­çèæ¬ç¨äºå° [labelme](https://github.com/
+wkentaro/labelme) æ æ³¨çæ°æ®è½¬æ¢ä¸º [PASCAL VOC](http://
+host.robots.ox.ac.uk/pascal/VOC/) æ ¼å¼å [MS COCO](https://cocodataset.org/
+#home)
+æ ¼å¼çæ°æ®éï¼ä¾¿äºç´æ¥å©ç¨æ¯æè¿ä¸¤ç§æ ¼å¼çæ¡æ¶è¿è¡è®­ç»ã
+èæ¬é½ä½¿ç¨ [Python](https://www.python.org/) åçã
+å¤§é¨åçèæ­¥é½æ¯åèç labelme é¡¹ç®ä¸­ç [examples](https://
+github.com/wkentaro/labelme/tree/main/examples)
+åå®¹ãç¶åæ·»å ä¸äºæ ¹æ®èªå·±çæ°æ®éèªå®ä¹çåè½ï¼æ¯å¦æ ç­¾è½¬æ¢ãèªå®ä¹å¾ååç§°ç­ã
+**æ³¨æ**ï¼è¿äºèæ¬å¶å®å¹¶ä¸å¤æï¼æ Python
+åºç¡çåå­¦å¯ä»¥è¿ä¸éè½¬æ¢çæµç¨ï¼ç¡®ä¿å¨ä½ çæ°æ®éä¸æ¯å¯ä»¥æ­£å¸¸è¿è¡çãæä¸äºå°æ¹ææ æ³¨äº
+`MARK`ï¼è¡¨ç¤ºå¨è¿äºå°æ¹éè¦çæï¼å¯ä»¥æ ¹æ®èªå·±çéè¦è¿è¡ä¿®æ¹ã
+**æå±**ï¼è¿äºèæ¬å½æ¶åªæ¯ç¨æ¥è½¬æ¢æèªå·±çæ°æ®éãå¦æä½ éè¦è½¬æ¢å¶ä»é¢åçæ°æ®éï¼æ¯å¦å®ä¾åå²ãè¯­ä¹åå²æèè§é¢æ æ³¨ç­ç­ãå»ºè®®å»
+lebelme ç [examples](https://github.com/wkentaro/labelme/tree/main/examples)
+é¨åççï¼ä½èæä¾äºä¸äºç¤ºä¾ä»£ç ï¼å¯ä»¥åèã
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With * [Python](https://www.python.org/) * [labelme](https://
 github.com/wkentaro/labelme) * [imgviz](https://github.com/wkentaro/imgviz)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started ### Prerequisites 1. gather the labelme-annotated jsons into
-a folder. In the next steps, we will refer to this folder as
-`labelme_jsons_dir`. 2. prepare a text file to store class names in your
-dataset. named it `label_names.txt`. take a look at `test/label_names.txt` for
-an example. 3. if need class name conversion, prepare a text file to store the
-conversion rules. named it `label_dict.txt`. take a look at `test/
-label_dict.txt` for an example. ### Installation #### install in develop mode
-1. suggested to use virtualenv to install python packages. ```sh conda create -
--name=labelme python=3.6 conda activate labelme pip install -r requirements.txt
-``` 2. clone the repo. ```sh git clone git@github.com:veraposeidon/
-labelme2Datasets.git ``` 3. install the package ```sh cd labelme2Datasets #
-(prefer this way!) install in editable mode, so that you can modify the package
-pip install -e . # install in non-editable mode, so that you can use the
-package, but cannot modify it #python setup.py install ``` #### simply use PyPI
-I also published a PyPI package named [labelme2datasets](https://pypi.org/
-project/labelme2datasets/). you can just use `pip3 install labelme2datasets` to
-install this package. if the baseline in this project not work for your
-datasets, you can install in develop mode, and modify the code by your own.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage - convert a single json into dataset. (`labelme_json2dataset.py`)
-```shell labelme_json2dataset --json_file=data/test.json \ --output_dir=output/
-test_single_output ``` - convert a folder of jsons into voc-format dataset.
-(`labelme_bbox_json2voc.py`) - without label conversion ```shell
-labelme_bbox_json2voc --json_dir=data/test_jsons \ --output_dir=output/
-test_voc_output --labels data/label_names.txt ``` - with label conversion
-```shell labelme_bbox_json2voc --json_dir=data/test_jsons \ --
-output_dir=output/test_voc_output \ --labels data/label_names.txt \ --
-label_dict data/label_dict.txt ``` - splitting voc datasets into train set and
-test set. (`split_voc_datasets.py`) ```shell split_voc_datasets --voc_dir
-output/test_voc_output --test_ratio 0.3 --random_seed 42 ``` `train.txt` and
-`test.txt` should be generated in `voc_dir/ImageSets/Main/`. - turn voc format
-dataset into coco style dataset. (`voc2coco.py`) ```shell voc2coco --voc_dir
+## Getting Started ### Prerequisites 1. å° lebelme æ æ³¨å¾å°ç JSON
+æä»¶æ¾å¨ä¸ä¸ªæä»¶å¤¹åãä¸¾ä¸ªä¾å­ï¼å½åä¸º
+`labelme_jsons_dir`ã 2. åå¤å¥½ä¸ä»½ text
+ææ¬ï¼éé¢åå«æ°æ®éçåç±»æ ç­¾ãä¸¾ä¸ªä¾å­ï¼å½åä¸º
+`label_names.txt`ãå¯ä»¥åèä¸é¡¹ç®éç `test/label_names.txt`ã 3.
+å¦ææè½¬æ¢æ ç­¾çéæ±ï¼æ¯å¦ä¸­ææ ç­¾è½¬ä¸ºè±æï¼ï¼åå¤ä¸ä¸ªææ¬ï¼åå«è½¬æ¢çè§åï¼ä¸¾ä¸ªä¾å­ï¼å½åä¸º`label_dict.txt`ãå¯ä»¥åèä¸é¡¹ç®éç
+`test/label_dict.txt` ã ### Installation #### develop mode å®è£ 1.
+å»ºè®®ä½¿ç¨èæç¯å¢å®è£ Python Packageã ```sh conda create --
+name=labelme python=3.9 conda activate labelme pip install -r requirements.txt
+``` 2. åéä»åºã ```sh git clone git@github.com:veraposeidon/
+labelme2Datasets.git ``` 3. æ¬å°å®è£ ```sh cd labelme2Datasets #
+ï¼æ¨èï¼å¯ç¼è¾æ¨¡å¼å®è£ï¼å³å¯ä»¥ä¿®æ¹ä»£ç  pip install -e . #
+ç¬¬äºç§å®è£æ¹å¼ï¼å¯ä»¥ç´æ¥è¿è¡èæ¬ï¼ä½æ¯ä¸è½ä¿®æ¹ä»£ç 
+#python setup.py install ``` #### ç´æ¥ä½¿ç¨ PyPI åæ¶åå¸äºä¸ä¸ª PyPI
+packageï¼[labelme2datasets](https://pypi.org/project/labelme2datasets/)ã
+å¯ä»¥ç´æ¥ä½¿ç¨ `pip3 install labelme2datasets` è¿è¡å®è£ã
+å¦æé¡¹ç®ä¸­çæµç¨ä¸éç¨äºä½ çæ°æ®éï¼å»ºè®®éè¿ä¸è¿°
+develop mode å®è£åä¿®æ¹ä»£ç ã
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Usage - è½¬æ¢åä¸ª JSON æä»¶ã (`labelme_json2dataset.py`) ```sh
+labelme_json2dataset --json_file=data/sample.json \ --output_dir=output/
+test_single_output ``` - è½¬æ¢ JSON æä»¶å¤¹`labelme_jsons_dir` å° VOC
+æ ¼å¼çæ°æ®éã (`labelme_bbox_json2voc.py`) - ä¸éè¦æ ç­¾è½¬æ¢
+```sh labelme_bbox_json2voc --json_dir=data/sample_jsons \ --output_dir=output/
+test_voc_output --labels data/label_names.txt ``` - éè¦æ ç­¾è½¬æ¢ ```sh
+labelme_bbox_json2voc --json_dir=data/sample_jsons \ --output_dir=output/
+test_voc_output \ --labels data/label_names.txt \ --label_dict data/
+label_dict.txt ``` - åå² VOC æ°æ®çè®­ç»éåæµè¯éã
+(`split_voc_datasets.py`) ```sh split_voc_datasets --voc_dir output/
+test_voc_output --test_ratio 0.3 --random_seed 42 ``` `train.txt` å
+`test.txt` ä¼åºç°å¨ `voc_dir/ImageSets/Main/` æä»¶å¤¹ä¸ã - å° VOC
+æ°æ®éè½¬æ¢ä¸º COCO æ°æ®é (`voc2coco.py`) ```shell voc2coco --voc_dir
 output/test_voc_output --coco_dir output/test_coco_output ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] add all scripts with pylint passed - [x] chinese and english
-readme - [x] modify project architecture - [x] publish as package See the [open
-issues](https://github.com/veraposeidon/labelme2Datasets/issues) for a full
-list of proposed features (and known issues).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Contributing Contributions are what make the open source community such an
-amazing place to learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. If you have a suggestion that would make this better,
-please fork the repo and create a pull request. You can also simply open an
-issue with the tag "enhancement". Don't forget to give the project a star!
-Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
--b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
+## Roadmap - [x] å°ææçèæ¬é½éè¿ Pylint - [x] ä¸­è±æ README -
+[x] è°æ´é¡¹ç®ç»æ - [x] åå¸ Pypi å See the [open issues](https://
+github.com/veraposeidon/labelme2Datasets/issues) for a full list of proposed
+features (and known issues).
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Contributing
+å¦æä½ æä»ä¹å»ºè®®å¯ä»¥è®©è¿ä¸ªé¡¹ç®åå¾æ´å¥½ï¼å¯ä»¥ Fork
+é¡¹ç®å¹¶ä¸æäº¤ Pull Requestã ä¹å¯ä»¥ç®åå°å¨ [issues](https://
+github.com/veraposeidon/labelme2Datasets/issues) ä¸­å¼ä¸ä¸ª issueã 1. Fork
+the Project 2. Create your Feature Branch (`git checkout -b feature/
+AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
 information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact veraposeidon - veraposeidon@gmail.com Project Link: [https://
 github.com/veraposeidon/labelme2Datasets](https://github.com/veraposeidon/
 labelme2Datasets)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments * [labelme](https://github.com/wkentaro/labelme) *
 [labelme2coco](https://github.com/fcakyon/labelme2coco)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-[en-sheild]:https://img.shields.io/badge/language-english-blue [en-url]:https:/
-/github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.md
-[contributors-shield]: https://img.shields.io/github/contributors/veraposeidon/
+[zh-sheild]:https://img.shields.io/badge/language-chinese-red [zh-url]:https://
+github.com/veraposeidon/labelme2Datasets//blob/main/README.md [contributors-
+shield]: https://img.shields.io/github/contributors/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [contributors-url]: https://
 github.com/veraposeidon/labelme2Datasets/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [forks-url]: https://github.com/
 veraposeidon/labelme2Datasets/network/members [stars-shield]: https://
 img.shields.io/github/stars/veraposeidon/labelme2Datasets.svg?style=for-the-
 badge [stars-url]: https://github.com/veraposeidon/labelme2Datasets/stargazers
 [issues-shield]: https://img.shields.io/github/issues/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [issues-url]: https://github.com/
 veraposeidon/labelme2Datasets/issues [license-shield]: https://img.shields.io/
 github/license/veraposeidon/labelme2Datasets.svg?style=for-the-badge [license-
-url]: https://github.com/veraposeidon/labelme2Datasets/blob/opensourceJourney/
-LICENSE [product-screenshot]: images/screenshot.png
+url]: https://github.com/veraposeidon/labelme2Datasets/blob/main/LICENSE
+[product-screenshot]: images/screenshot.png
```

### Comparing `labelme2datasets-0.0.2/labelme2datasets/labelme_bbox_json2voc.py` & `labelme2datasets-0.0.3/labelme2datasets/labelme_bbox_json2voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+# coding=utf-8
 """
 desc: gather json files annotated by labelme into a dictionary,
     and use this script to generate a voc style dataset.
 
 reference: https://github.com/wkentaro/labelme/blob/main/examples/bbox_detection/labelme2voc.py
 """
 
-# coding=utf-8
 
 from __future__ import print_function
 
 import argparse
 import glob
 import os
 import os.path as osp
@@ -194,15 +194,15 @@
     # viz image file
     out_viz_file = osp.join(output_dir, "AnnotationsVisualization", base + ".jpg")
 
     label_file = labelme.LabelFile(filename=filename)
 
     # save source image
     img = labelme.utils.img_data_to_arr(label_file.imageData)
-    imgviz.io.imsave(out_img_file, img)
+    imgviz.io.imsave(str(out_img_file), img)
 
     # get xml
     (xml, bboxes, labels) = get_xml_with_labelfile(label_file, base, label_dict, class_names)
 
     # save visualized image
     save_visualization_image(img, labels, bboxes, class_names, output_file=out_viz_file)
 
@@ -211,20 +211,24 @@
         out_f.write(lxml.etree.tostring(xml, pretty_print=True))
 
 
 def save_visualization_image(img, labels, bboxes, class_names, output_file):
     """save visualized image"""
     # caption for visualize drawing
     captions = [class_names[label] for label in labels]
+    # font can display chinese
+    # MARK: change font path if you need
+    font_path = "SimSun.ttf"
     viz = imgviz.instances2rgb(
         image=img,
         labels=labels,
         bboxes=bboxes,
         captions=captions,
-        font_size=15,
+        font_size=20,
+        font_path=font_path,
     )
     imgviz.io.imsave(output_file, viz)
 
 
 def main():
     """main"""
     parser = argparse.ArgumentParser(
```

### Comparing `labelme2datasets-0.0.2/labelme2datasets/labelme_json2dataset.py` & `labelme2datasets-0.0.3/labelme2datasets/labelme_json2dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
+# coding=utf-8
 """
 brief: covert single json file to single image dataset.
 
 usage：python labelme_json2dataset.py json_file -o output_directory
 
 reference: https://github.com/wkentaro/labelme/blob/main/labelme/cli/json_to_dataset.py
 """
 
-# coding=utf-8
-
 import argparse
 import base64
 import json
 import os
 import os.path as osp
 
 import PIL.Image
@@ -46,18 +45,17 @@
     :param image: image
     :return: label names and lbl
     """
     label_name_to_value = {'_background_': 0}
     for shape in sorted(data['shapes'], key=lambda x: x['label']):
         label_name = shape['label']
         if label_name in label_name_to_value:
-            pass
-        else:
-            label_value = len(label_name_to_value)
-            label_name_to_value[label_name] = label_value
+            continue
+        label_value = len(label_name_to_value)
+        label_name_to_value[label_name] = label_value
     lbl, _ = utils.shapes_to_label(image.shape, data['shapes'], label_name_to_value)
 
     label_names = [None] * (max(label_name_to_value.values()) + 1)
     for name, value in label_name_to_value.items():
         label_names[value] = name
 
     return label_names, lbl
@@ -81,36 +79,41 @@
         for lbl_name in label_names:
             label_f.write(lbl_name + '\n')
 
     print(f"Saved to: {output_dir}")
 
 
 def main():
-    """ main """
+    """ Main function. """
     logger.warning(
-        'This script is aimed to demonstrate how to convert the'
-        'JSON file to a single image dataset, and not to handle'
-        'multiple JSON files to generate a real-use dataset.'
+        'This script demonstrates how to convert a JSON file '
+        'into a single image dataset. However, it is not intended '
+        'to handle multiple JSON files for generating a real-world dataset.'
     )
     logger.warning(
-        "It won't handle multiple JSON files to generate a "
-        "real-use dataset."
+        "This script does not support processing multiple JSON files "
+        "to create a real-world dataset."
     )
     parser = argparse.ArgumentParser()
     parser.add_argument('--json_file')
     parser.add_argument('--output_dir', default=None)
     args = parser.parse_args()
 
     json_file = args.json_file
 
+    if json_file is None or not os.path.exists(json_file):
+        logger.error("JSON file is not provided or does not exist. -h for help.")
+        return
+
     if args.output_dir is None:
         out_dir = osp.basename(json_file).replace('.', '_')
-        out_dir = osp.join(osp.dirname(json_file), out_dir)
+        out_dir = osp.join(osp.dirname(json_file), str(out_dir))
     else:
         out_dir = args.output_dir
+
     if not osp.exists(out_dir):
         os.mkdir(out_dir)
 
     (data, img) = get_data_and_image(json_file)
 
     (label_names, lbl) = get_label_names(data, img)
```

### Comparing `labelme2datasets-0.0.2/labelme2datasets/split_voc_datasets.py` & `labelme2datasets-0.0.3/labelme2datasets/split_voc_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""splitting voc format datasets into training set and test set"""
 # coding=utf-8
+"""splitting voc format datasets into training set and test set"""
+
 
 import argparse
 import sys
 import os
 import os.path as osp
 import glob
 from pathlib import Path
```

### Comparing `labelme2datasets-0.0.2/labelme2datasets/utils.py` & `labelme2datasets-0.0.3/labelme2datasets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+# coding=utf-8
 """
 some common functions.
 """
 
-# coding=utf-8
 
 import os.path as osp
 
+
 def get_label_conversion_dict(dict_file):
     """
     自定义标签转换，例如将中文标签转换为英文标签
     custom label conversion, for example, convert chinese label to english label, vice versa.
     """
     if dict_file is None:
         return {}
```

### Comparing `labelme2datasets-0.0.2/labelme2datasets/voc2coco.py` & `labelme2datasets-0.0.3/labelme2datasets/voc2coco.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+# coding=utf-8
 """turn voc format datasets into coco format datasets"""
-# coding = utf-8
 
 import argparse
 import sys
 import os
 import os.path as osp
 from pathlib import Path
 import json
```

### Comparing `labelme2datasets-0.0.2/labelme2datasets.egg-info/PKG-INFO` & `labelme2datasets-0.0.3/labelme2datasets.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: labelme2datasets
-Version: 0.0.2
+Version: 0.0.3
 Summary: python scripts to convert labelme-generated-jsons to voc/coco style datasets.
 Home-page: https://github.com/veraposeidon/labelme2Datasets
 Author: veraposeidon
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: imgviz~=1.7.5
+Requires-Dist: labelme~=5.4.1
+Requires-Dist: progressbar~=2.5
+Requires-Dist: scikit-learn~=1.4.2
+Requires-Dist: xmltodict~=0.13.0
+Requires-Dist: setuptools~=69.5.1
+Requires-Dist: pillow~=10.3.0
+Requires-Dist: lxml~=5.2.1
 
 <div id="top"></div>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -27,17 +34,19 @@
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
 *** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
-[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml/badge.svg?branch=opensourceJourney)](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml)
-[![codebeat badge](https://codebeat.co/badges/5f99fcd3-c3a5-4154-91ca-4bb58b32bd53)](https://codebeat.co/projects/github-com-veraposeidon-labelme2datasets-opensourcejourney)
-[![english][en-sheild]][en-url]
+[![PyPI](https://img.shields.io/pypi/v/labelme2datasets.svg)](https://pypi.python.org/pypi/labelme2datasets)
+[![PythonVersion](https://img.shields.io/pypi/pyversions/labelme2datasets.svg)](https://pypi.org/project/labelme2datasets)
+[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml/badge.svg)](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/pylint.yml)
+[![codebeat badge](https://codebeat.co/badges/ab6b3bb6-213b-4a4f-ac55-277dd2840f28)](https://codebeat.co/projects/github-com-veraposeidon-labelme2datasets-main)
+[![chinese][zh-sheild]][zh-url]
 <br />
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 
@@ -50,24 +59,24 @@
   <a href="https://github.com/veraposeidon/labelme2Datasets">
     <img src="images/logo.png" alt="Logo" width="80" height="80">
   </a>
 
 <h3 align="center">labelme2Datasets</h3>
 
   <p align="center">
-    python scripts to convert labelme-generated-jsons to voc/coco style datasets.
+    用于将 LabelMe 标注的数据转换为 VOC 格式和 COCO 格式的数据集。
     <br />
     <a href="https://github.com/veraposeidon/labelme2Datasets/issues">Report Bug</a>
     ·
     <a href="https://github.com/veraposeidon/labelme2Datasets/issues">Request Feature</a>
   </p>
 </div>
 
 
-[（中文 README）](https://github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.zh.md)
+[English README Available](https://github.com/veraposeidon/labelme2Datasets//blob/main/README.en.md)
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
@@ -91,23 +100,23 @@
   </ol>
 </details>
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-Scripts in this repository are used to convert [labelme](https://github.com/wkentaro/labelme)-annotated jsons into standard datasets in [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) format or [MS COCO](https://cocodataset.org/#home) format.
+仓库中的脚本用于将 [labelme](https://github.com/wkentaro/labelme) 标注的数据转换为 [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) 格式和 [MS COCO](https://cocodataset.org/#home) 格式的数据集，便于直接利用支持这两种格式的框架进行训练。
 
-Scripts are written in [Python](https://www.python.org/).
+脚本都使用 [Python](https://www.python.org/) 写的。
 
-Most of the scripts refer to the [examples](https://github.com/wkentaro/labelme/tree/main/examples) section of labelme. Then I add some features according my own dataset, like class name conversion, customise image name, etc.
+大部分的脚步都是参考的 labelme 项目中的 [examples](https://github.com/wkentaro/labelme/tree/main/examples) 内容。然后添加一些根据自己的数据集自定义的功能，比如标签转换、自定义图像名称等。
 
-**Attention**: these scripts are not complicated, and if you have the basis of python, please go through the convert workflows, and ensure that it fits your datasets. There are some places I annotated `MARK`, which means pay attention to it, and you could customize it to fit your needs.
+**注意**：这些脚本其实并不复杂，有 Python 基础的同学可以过一遍转换的流程，确保在你的数据集上是可以正常运行的。有一些地方我标注了 `MARK`，表示在这些地方需要留意，可以根据自己的需要进行修改。
 
-**Customize**: these scripts are only for the conversion of data I currently have. If you want to convert datasets in other areas, like instance segmentation, segmantic segmentation, video annotation, etc. please take a look at the [examples](https://github.com/wkentaro/labelme/tree/main/examples) section in labelme.
+**拓展**：这些脚本当时只是用来转换我自己的数据集。如果你需要转换其他领域的数据集，比如实例分割、语义分割或者视频标注等等。建议去 lebelme 的 [examples](https://github.com/wkentaro/labelme/tree/main/examples) 部分看看，作者提供了一些示例代码，可以参考。
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 ### Built With
 
@@ -120,113 +129,106 @@
 
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 ### Prerequisites
 
-1. gather the labelme-annotated jsons into a folder. In the next steps, we will refer to this folder as `labelme_jsons_dir`.
+1. 将 lebelme 标注得到的 JSON 文件放在一个文件夹内。举个例子，命名为 `labelme_jsons_dir`。
 
-2. prepare a text file to store class names in your dataset. named it `label_names.txt`. take a look at `test/label_names.txt` for an example.
+2. 准备好一份 text 文本，里面包含数据集的分类标签。举个例子，命名为  `label_names.txt`。可以参考下项目里的 `test/label_names.txt`。
 
-3. if need class name conversion, prepare a text file to store the conversion rules. named it `label_dict.txt`. take a look at `test/label_dict.txt` for an example.
+3. 如果有转换标签的需求（比如中文标签转为英文），准备一个文本，包含转换的规则，举个例子，命名为`label_dict.txt`。可以参考下项目里的 `test/label_dict.txt` 。
 ### Installation
-
-#### install in develop mode
-1. suggested to use virtualenv to install python packages.
+#### develop mode 安装
+1. 建议使用虚拟环境安装 Python Package。
   
     ```sh
-    conda create --name=labelme python=3.6
+    conda create --name=labelme python=3.9
     conda activate labelme
     pip install -r requirements.txt
     ```
-2. clone the repo.
+2. 克隆仓库。
     ```sh
     git clone git@github.com:veraposeidon/labelme2Datasets.git
     ```
-3. install the package
+3. 本地安装
    ```sh
     cd labelme2Datasets
-    # (prefer this way!) install in editable mode, so that you can modify the package 
+    # （推荐）可编辑模式安装，即可以修改代码
     pip install -e .
-    # install in non-editable mode, so that you can use the package, but cannot modify it
+    # 第二种安装方式，可以直接运行脚本，但是不能修改代码
     #python setup.py install
    ```
    
-#### simply use PyPI
-
-I also published a PyPI package named [labelme2datasets](https://pypi.org/project/labelme2datasets/).
+#### 直接使用 PyPI
 
-you can just use `pip3 install labelme2datasets` to install this package.
+同时发布了一个 PyPI package，[labelme2datasets](https://pypi.org/project/labelme2datasets/)。
 
-if the baseline in this project not work for your datasets, you can install in develop mode, and modify the code by your own.
+可以直接使用 `pip3 install labelme2datasets` 进行安装。
 
+如果项目中的流程不适用于你的数据集，建议通过上述 develop mode 安装和修改代码。
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-- convert a single json into dataset. (`labelme_json2dataset.py`)
-    ```shell
-    labelme_json2dataset --json_file=data/test.json \
+- 转换单个 JSON 文件。 (`labelme_json2dataset.py`)
+    ```sh
+    labelme_json2dataset --json_file=data/sample.json \
       --output_dir=output/test_single_output
     ```
 
-- convert a folder of jsons into voc-format dataset. (`labelme_bbox_json2voc.py`)
-  - without label conversion
-    ```shell
-    labelme_bbox_json2voc --json_dir=data/test_jsons \
+- 转换 JSON 文件夹`labelme_jsons_dir` 到  VOC 格式的数据集。 (`labelme_bbox_json2voc.py`)
+  - 不需要标签转换
+    ```sh
+    labelme_bbox_json2voc --json_dir=data/sample_jsons \
       --output_dir=output/test_voc_output --labels data/label_names.txt
     ```
-  - with label conversion
-    ```shell
-    labelme_bbox_json2voc --json_dir=data/test_jsons \
+  - 需要标签转换
+    ```sh
+    labelme_bbox_json2voc --json_dir=data/sample_jsons \
       --output_dir=output/test_voc_output \
       --labels data/label_names.txt \
       --label_dict data/label_dict.txt
     ```
-- splitting voc datasets into train set and test set. (`split_voc_datasets.py`)
-  ```shell
+- 分割 VOC 数据的训练集和测试集。 (`split_voc_datasets.py`)
+  ```sh
     split_voc_datasets --voc_dir output/test_voc_output --test_ratio 0.3 --random_seed 42
   ```
-  `train.txt` and `test.txt` should be generated in `voc_dir/ImageSets/Main/`.
+  `train.txt` 和 `test.txt` 会出现在 `voc_dir/ImageSets/Main/` 文件夹下。
 
-- turn voc format dataset into coco style dataset. (`voc2coco.py`)
+- 将 VOC 数据集转换为 COCO 数据集 (`voc2coco.py`)
   ```shell
     voc2coco --voc_dir output/test_voc_output --coco_dir output/test_coco_output
   ```
-
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-
-
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] add all scripts with pylint passed
-- [x] chinese and english readme
-- [x] modify project architecture
-- [x] publish as package
+- [x] 将所有的脚本都通过 Pylint
+- [x] 中英文 README
+- [x] 调整项目结构
+- [x] 发布 Pypi 包
 
 See the [open issues](https://github.com/veraposeidon/labelme2Datasets/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
+如果你有什么建议可以让这个项目变得更好，可以 Fork 项目并且提交 Pull Request。
+也可以简单地在 [issues](https://github.com/veraposeidon/labelme2Datasets/issues) 中开一个 issue。
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
@@ -262,22 +264,20 @@
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[en-sheild]:https://img.shields.io/badge/language-english-blue
-[en-url]:https://github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.md
+[zh-sheild]:https://img.shields.io/badge/language-chinese-red
+[zh-url]:https://github.com/veraposeidon/labelme2Datasets//blob/main/README.md
 [contributors-shield]: https://img.shields.io/github/contributors/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [contributors-url]: https://github.com/veraposeidon/labelme2Datasets/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [forks-url]: https://github.com/veraposeidon/labelme2Datasets/network/members
 [stars-shield]: https://img.shields.io/github/stars/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [stars-url]: https://github.com/veraposeidon/labelme2Datasets/stargazers
 [issues-shield]: https://img.shields.io/github/issues/veraposeidon/labelme2Datasets.svg?style=for-the-badge
 [issues-url]: https://github.com/veraposeidon/labelme2Datasets/issues
 [license-shield]: https://img.shields.io/github/license/veraposeidon/labelme2Datasets.svg?style=for-the-badge
-[license-url]: https://github.com/veraposeidon/labelme2Datasets/blob/opensourceJourney/LICENSE
+[license-url]: https://github.com/veraposeidon/labelme2Datasets/blob/main/LICENSE
 [product-screenshot]: images/screenshot.png
-
-
```

#### html2text {}

```diff
@@ -1,128 +1,133 @@
-Metadata-Version: 2.1 Name: labelme2datasets Version: 0.0.2 Summary: python
+Metadata-Version: 2.1 Name: labelme2datasets Version: 0.0.3 Summary: python
 scripts to convert labelme-generated-jsons to voc/coco style datasets. Home-
 page: https://github.com/veraposeidon/labelme2Datasets Author: veraposeidon
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Description-Content-Type: text/markdown License-File:
-LICENSE
-[![Pylint](https://github.com/veraposeidon/labelme2Datasets/actions/workflows/
-pylint.yml/badge.svg?branch=opensourceJourney)](https://github.com/
-veraposeidon/labelme2Datasets/actions/workflows/pylint.yml) [![codebeat badge]
-(https://codebeat.co/badges/5f99fcd3-c3a5-4154-91ca-4bb58b32bd53)](https://
-codebeat.co/projects/github-com-veraposeidon-labelme2datasets-
-opensourcejourney) [![english][en-sheild]][en-url]
+Classifier: Programming Language :: Python :: 3.9 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+beautifulsoup4~=4.12.3 Requires-Dist: imgviz~=1.7.5 Requires-Dist:
+labelme~=5.4.1 Requires-Dist: progressbar~=2.5 Requires-Dist: scikit-
+learn~=1.4.2 Requires-Dist: xmltodict~=0.13.0 Requires-Dist: setuptools~=69.5.1
+Requires-Dist: pillow~=10.3.0 Requires-Dist: lxml~=5.2.1
+[![PyPI](https://img.shields.io/pypi/v/labelme2datasets.svg)](https://
+pypi.python.org/pypi/labelme2datasets) [![PythonVersion](https://
+img.shields.io/pypi/pyversions/labelme2datasets.svg)](https://pypi.org/project/
+labelme2datasets) [![Pylint](https://github.com/veraposeidon/labelme2Datasets/
+actions/workflows/pylint.yml/badge.svg)](https://github.com/veraposeidon/
+labelme2Datasets/actions/workflows/pylint.yml) [![codebeat badge](https://
+codebeat.co/badges/ab6b3bb6-213b-4a4f-ac55-277dd2840f28)](https://codebeat.co/
+projects/github-com-veraposeidon-labelme2datasets-main) [![chinese][zh-sheild]]
+[zh-url]
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
 shield]][issues-url] [![MIT License][license-shield]][license-url]
                                     _[_L_o_g_o_]
                           ******** llaabbeellmmee22DDaattaasseettss ********
-python scripts to convert labelme-generated-jsons to voc/coco style datasets.
+         ç¨äºå° LabelMe æ æ³¨çæ°æ®è½¬æ¢ä¸º VOC æ ¼å¼å COCO
+                            æ ¼å¼çæ°æ®éã
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
-[ï¼ä¸­æ READMEï¼](https://github.com/veraposeidon/labelme2Datasets//blob/
-opensourceJourney/README.zh.md) Table of Contents
+[English README Available](https://github.com/veraposeidon/labelme2Datasets//
+blob/main/README.en.md) Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _L_i_c_e_n_s_e
    7. _C_o_n_t_a_c_t
    8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
-## About The Project Scripts in this repository are used to convert [labelme]
-(https://github.com/wkentaro/labelme)-annotated jsons into standard datasets in
-[PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/) format or [MS COCO]
-(https://cocodataset.org/#home) format. Scripts are written in [Python](https:/
-/www.python.org/). Most of the scripts refer to the [examples](https://
-github.com/wkentaro/labelme/tree/main/examples) section of labelme. Then I add
-some features according my own dataset, like class name conversion, customise
-image name, etc. **Attention**: these scripts are not complicated, and if you
-have the basis of python, please go through the convert workflows, and ensure
-that it fits your datasets. There are some places I annotated `MARK`, which
-means pay attention to it, and you could customize it to fit your needs.
-**Customize**: these scripts are only for the conversion of data I currently
-have. If you want to convert datasets in other areas, like instance
-segmentation, segmantic segmentation, video annotation, etc. please take a look
-at the [examples](https://github.com/wkentaro/labelme/tree/main/examples)
-section in labelme.
+## About The Project ä»åºä¸­çèæ¬ç¨äºå° [labelme](https://github.com/
+wkentaro/labelme) æ æ³¨çæ°æ®è½¬æ¢ä¸º [PASCAL VOC](http://
+host.robots.ox.ac.uk/pascal/VOC/) æ ¼å¼å [MS COCO](https://cocodataset.org/
+#home)
+æ ¼å¼çæ°æ®éï¼ä¾¿äºç´æ¥å©ç¨æ¯æè¿ä¸¤ç§æ ¼å¼çæ¡æ¶è¿è¡è®­ç»ã
+èæ¬é½ä½¿ç¨ [Python](https://www.python.org/) åçã
+å¤§é¨åçèæ­¥é½æ¯åèç labelme é¡¹ç®ä¸­ç [examples](https://
+github.com/wkentaro/labelme/tree/main/examples)
+åå®¹ãç¶åæ·»å ä¸äºæ ¹æ®èªå·±çæ°æ®éèªå®ä¹çåè½ï¼æ¯å¦æ ç­¾è½¬æ¢ãèªå®ä¹å¾ååç§°ç­ã
+**æ³¨æ**ï¼è¿äºèæ¬å¶å®å¹¶ä¸å¤æï¼æ Python
+åºç¡çåå­¦å¯ä»¥è¿ä¸éè½¬æ¢çæµç¨ï¼ç¡®ä¿å¨ä½ çæ°æ®éä¸æ¯å¯ä»¥æ­£å¸¸è¿è¡çãæä¸äºå°æ¹ææ æ³¨äº
+`MARK`ï¼è¡¨ç¤ºå¨è¿äºå°æ¹éè¦çæï¼å¯ä»¥æ ¹æ®èªå·±çéè¦è¿è¡ä¿®æ¹ã
+**æå±**ï¼è¿äºèæ¬å½æ¶åªæ¯ç¨æ¥è½¬æ¢æèªå·±çæ°æ®éãå¦æä½ éè¦è½¬æ¢å¶ä»é¢åçæ°æ®éï¼æ¯å¦å®ä¾åå²ãè¯­ä¹åå²æèè§é¢æ æ³¨ç­ç­ãå»ºè®®å»
+lebelme ç [examples](https://github.com/wkentaro/labelme/tree/main/examples)
+é¨åççï¼ä½èæä¾äºä¸äºç¤ºä¾ä»£ç ï¼å¯ä»¥åèã
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With * [Python](https://www.python.org/) * [labelme](https://
 github.com/wkentaro/labelme) * [imgviz](https://github.com/wkentaro/imgviz)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started ### Prerequisites 1. gather the labelme-annotated jsons into
-a folder. In the next steps, we will refer to this folder as
-`labelme_jsons_dir`. 2. prepare a text file to store class names in your
-dataset. named it `label_names.txt`. take a look at `test/label_names.txt` for
-an example. 3. if need class name conversion, prepare a text file to store the
-conversion rules. named it `label_dict.txt`. take a look at `test/
-label_dict.txt` for an example. ### Installation #### install in develop mode
-1. suggested to use virtualenv to install python packages. ```sh conda create -
--name=labelme python=3.6 conda activate labelme pip install -r requirements.txt
-``` 2. clone the repo. ```sh git clone git@github.com:veraposeidon/
-labelme2Datasets.git ``` 3. install the package ```sh cd labelme2Datasets #
-(prefer this way!) install in editable mode, so that you can modify the package
-pip install -e . # install in non-editable mode, so that you can use the
-package, but cannot modify it #python setup.py install ``` #### simply use PyPI
-I also published a PyPI package named [labelme2datasets](https://pypi.org/
-project/labelme2datasets/). you can just use `pip3 install labelme2datasets` to
-install this package. if the baseline in this project not work for your
-datasets, you can install in develop mode, and modify the code by your own.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage - convert a single json into dataset. (`labelme_json2dataset.py`)
-```shell labelme_json2dataset --json_file=data/test.json \ --output_dir=output/
-test_single_output ``` - convert a folder of jsons into voc-format dataset.
-(`labelme_bbox_json2voc.py`) - without label conversion ```shell
-labelme_bbox_json2voc --json_dir=data/test_jsons \ --output_dir=output/
-test_voc_output --labels data/label_names.txt ``` - with label conversion
-```shell labelme_bbox_json2voc --json_dir=data/test_jsons \ --
-output_dir=output/test_voc_output \ --labels data/label_names.txt \ --
-label_dict data/label_dict.txt ``` - splitting voc datasets into train set and
-test set. (`split_voc_datasets.py`) ```shell split_voc_datasets --voc_dir
-output/test_voc_output --test_ratio 0.3 --random_seed 42 ``` `train.txt` and
-`test.txt` should be generated in `voc_dir/ImageSets/Main/`. - turn voc format
-dataset into coco style dataset. (`voc2coco.py`) ```shell voc2coco --voc_dir
+## Getting Started ### Prerequisites 1. å° lebelme æ æ³¨å¾å°ç JSON
+æä»¶æ¾å¨ä¸ä¸ªæä»¶å¤¹åãä¸¾ä¸ªä¾å­ï¼å½åä¸º
+`labelme_jsons_dir`ã 2. åå¤å¥½ä¸ä»½ text
+ææ¬ï¼éé¢åå«æ°æ®éçåç±»æ ç­¾ãä¸¾ä¸ªä¾å­ï¼å½åä¸º
+`label_names.txt`ãå¯ä»¥åèä¸é¡¹ç®éç `test/label_names.txt`ã 3.
+å¦ææè½¬æ¢æ ç­¾çéæ±ï¼æ¯å¦ä¸­ææ ç­¾è½¬ä¸ºè±æï¼ï¼åå¤ä¸ä¸ªææ¬ï¼åå«è½¬æ¢çè§åï¼ä¸¾ä¸ªä¾å­ï¼å½åä¸º`label_dict.txt`ãå¯ä»¥åèä¸é¡¹ç®éç
+`test/label_dict.txt` ã ### Installation #### develop mode å®è£ 1.
+å»ºè®®ä½¿ç¨èæç¯å¢å®è£ Python Packageã ```sh conda create --
+name=labelme python=3.9 conda activate labelme pip install -r requirements.txt
+``` 2. åéä»åºã ```sh git clone git@github.com:veraposeidon/
+labelme2Datasets.git ``` 3. æ¬å°å®è£ ```sh cd labelme2Datasets #
+ï¼æ¨èï¼å¯ç¼è¾æ¨¡å¼å®è£ï¼å³å¯ä»¥ä¿®æ¹ä»£ç  pip install -e . #
+ç¬¬äºç§å®è£æ¹å¼ï¼å¯ä»¥ç´æ¥è¿è¡èæ¬ï¼ä½æ¯ä¸è½ä¿®æ¹ä»£ç 
+#python setup.py install ``` #### ç´æ¥ä½¿ç¨ PyPI åæ¶åå¸äºä¸ä¸ª PyPI
+packageï¼[labelme2datasets](https://pypi.org/project/labelme2datasets/)ã
+å¯ä»¥ç´æ¥ä½¿ç¨ `pip3 install labelme2datasets` è¿è¡å®è£ã
+å¦æé¡¹ç®ä¸­çæµç¨ä¸éç¨äºä½ çæ°æ®éï¼å»ºè®®éè¿ä¸è¿°
+develop mode å®è£åä¿®æ¹ä»£ç ã
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Usage - è½¬æ¢åä¸ª JSON æä»¶ã (`labelme_json2dataset.py`) ```sh
+labelme_json2dataset --json_file=data/sample.json \ --output_dir=output/
+test_single_output ``` - è½¬æ¢ JSON æä»¶å¤¹`labelme_jsons_dir` å° VOC
+æ ¼å¼çæ°æ®éã (`labelme_bbox_json2voc.py`) - ä¸éè¦æ ç­¾è½¬æ¢
+```sh labelme_bbox_json2voc --json_dir=data/sample_jsons \ --output_dir=output/
+test_voc_output --labels data/label_names.txt ``` - éè¦æ ç­¾è½¬æ¢ ```sh
+labelme_bbox_json2voc --json_dir=data/sample_jsons \ --output_dir=output/
+test_voc_output \ --labels data/label_names.txt \ --label_dict data/
+label_dict.txt ``` - åå² VOC æ°æ®çè®­ç»éåæµè¯éã
+(`split_voc_datasets.py`) ```sh split_voc_datasets --voc_dir output/
+test_voc_output --test_ratio 0.3 --random_seed 42 ``` `train.txt` å
+`test.txt` ä¼åºç°å¨ `voc_dir/ImageSets/Main/` æä»¶å¤¹ä¸ã - å° VOC
+æ°æ®éè½¬æ¢ä¸º COCO æ°æ®é (`voc2coco.py`) ```shell voc2coco --voc_dir
 output/test_voc_output --coco_dir output/test_coco_output ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] add all scripts with pylint passed - [x] chinese and english
-readme - [x] modify project architecture - [x] publish as package See the [open
-issues](https://github.com/veraposeidon/labelme2Datasets/issues) for a full
-list of proposed features (and known issues).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Contributing Contributions are what make the open source community such an
-amazing place to learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. If you have a suggestion that would make this better,
-please fork the repo and create a pull request. You can also simply open an
-issue with the tag "enhancement". Don't forget to give the project a star!
-Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
--b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
+## Roadmap - [x] å°ææçèæ¬é½éè¿ Pylint - [x] ä¸­è±æ README -
+[x] è°æ´é¡¹ç®ç»æ - [x] åå¸ Pypi å See the [open issues](https://
+github.com/veraposeidon/labelme2Datasets/issues) for a full list of proposed
+features (and known issues).
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Contributing
+å¦æä½ æä»ä¹å»ºè®®å¯ä»¥è®©è¿ä¸ªé¡¹ç®åå¾æ´å¥½ï¼å¯ä»¥ Fork
+é¡¹ç®å¹¶ä¸æäº¤ Pull Requestã ä¹å¯ä»¥ç®åå°å¨ [issues](https://
+github.com/veraposeidon/labelme2Datasets/issues) ä¸­å¼ä¸ä¸ª issueã 1. Fork
+the Project 2. Create your Feature Branch (`git checkout -b feature/
+AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
 information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact veraposeidon - veraposeidon@gmail.com Project Link: [https://
 github.com/veraposeidon/labelme2Datasets](https://github.com/veraposeidon/
 labelme2Datasets)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments * [labelme](https://github.com/wkentaro/labelme) *
 [labelme2coco](https://github.com/fcakyon/labelme2coco)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-[en-sheild]:https://img.shields.io/badge/language-english-blue [en-url]:https:/
-/github.com/veraposeidon/labelme2Datasets//blob/opensourceJourney/README.md
-[contributors-shield]: https://img.shields.io/github/contributors/veraposeidon/
+[zh-sheild]:https://img.shields.io/badge/language-chinese-red [zh-url]:https://
+github.com/veraposeidon/labelme2Datasets//blob/main/README.md [contributors-
+shield]: https://img.shields.io/github/contributors/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [contributors-url]: https://
 github.com/veraposeidon/labelme2Datasets/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [forks-url]: https://github.com/
 veraposeidon/labelme2Datasets/network/members [stars-shield]: https://
 img.shields.io/github/stars/veraposeidon/labelme2Datasets.svg?style=for-the-
 badge [stars-url]: https://github.com/veraposeidon/labelme2Datasets/stargazers
 [issues-shield]: https://img.shields.io/github/issues/veraposeidon/
 labelme2Datasets.svg?style=for-the-badge [issues-url]: https://github.com/
 veraposeidon/labelme2Datasets/issues [license-shield]: https://img.shields.io/
 github/license/veraposeidon/labelme2Datasets.svg?style=for-the-badge [license-
-url]: https://github.com/veraposeidon/labelme2Datasets/blob/opensourceJourney/
-LICENSE [product-screenshot]: images/screenshot.png
+url]: https://github.com/veraposeidon/labelme2Datasets/blob/main/LICENSE
+[product-screenshot]: images/screenshot.png
```

### Comparing `labelme2datasets-0.0.2/setup.py` & `labelme2datasets-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 """setup.py for install this package"""
 from setuptools import setup, find_packages
+from labelme2datasets.version import __version__
+
+
+def get_long_description():
+    with open('README.md', encoding='utf-8') as readme_f:
+        return readme_f.read()
+
+
+def get_install_requires():
+    with open('requirements.txt', encoding='utf-8') as req_f:
+        return req_f.read().splitlines()
+
+
+def get_version():
+    return __version__
 
-with open('README.md', encoding='utf-8') as readme_f:
-    long_description = readme_f.read()
 
 setup(
     name='labelme2datasets',
-    version='0.0.2',
+    version=get_version(),
     description='python scripts to convert labelme-generated-jsons to voc/coco style datasets.',
-    long_description=long_description,
+    long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/veraposeidon/labelme2Datasets",
     author='veraposeidon',
     packages=find_packages(include=['labelme2datasets', 'labelme2datasets.*']),
     install_requires=[
-        'imgviz~=1.4.1',
-        'pillow~=8.4.0',
-        'labelme~=4.5.13',
-        'lxml~=4.6.4',
+        'beautifulsoup4~=4.12.3',
+        'imgviz~=1.7.5',
+        'labelme~=5.4.1',
         'progressbar~=2.5',
-        'xmltodict~=0.12.0',
-        'sklearn~=0.0',
-        'scikit-learn~=0.24.2',
+        'scikit-learn~=1.4.2',
+        'xmltodict~=0.13.0',
+        'setuptools~=69.5.1',
+        'pillow~=10.3.0',
+        'lxml~=5.2.1'
     ],
     entry_points={
         'console_scripts': [
             'labelme_json2dataset = labelme2datasets.labelme_json2dataset:main',
             'labelme_bbox_json2voc = labelme2datasets.labelme_bbox_json2voc:main',
             'split_voc_datasets = labelme2datasets.split_voc_datasets:main',
             'voc2coco = labelme2datasets.voc2coco:main',
         ]
     },
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

