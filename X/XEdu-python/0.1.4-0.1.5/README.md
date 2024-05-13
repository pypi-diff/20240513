# Comparing `tmp/XEdu-python-0.1.4.tar.gz` & `tmp/XEdu-python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/XEdu-python-0.1.4.tar", last modified: Fri Apr 19 08:28:00 2024, max compression
+gzip compressed data, was "XEdu-python-0.1.5.tar", last modified: Mon May 13 08:34:04 2024, max compression
```

## Comparing `XEdu-python-0.1.4.tar` & `XEdu-python-0.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/
--rw-rw-r--   0 user      (1001) user      (1001)      192 2023-12-19 09:45:45.000000 XEdu-python-0.1.4/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      252 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/PKG-INFO
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/
--rw-rw-r--   0 user      (1001) user      (1001)     1160 2023-12-19 09:25:26.000000 XEdu-python-0.1.4/XEdu/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/examples/
--rw-rw-r--   0 user      (1001) user      (1001)      138 2022-08-22 02:06:19.000000 XEdu-python-0.1.4/XEdu/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    15534 2024-04-19 08:07:10.000000 XEdu-python-0.1.4/XEdu/examples/demo.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-10-07 08:07:43.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    32512 2024-03-15 09:06:21.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    37314 2023-06-26 06:07:55.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)    15668 2023-06-26 05:44:24.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)    24028 2023-10-20 05:39:29.000000 XEdu-python-0.1.4/XEdu/hub/BaseDeploy.py
--rw-rw-r--   0 user      (1001) user      (1001)      124 2023-12-13 09:25:51.000000 XEdu-python-0.1.4/XEdu/hub/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)    35020 2023-12-18 08:16:14.000000 XEdu-python-0.1.4/XEdu/hub/datatset_class.py
--rw-r--r--   0 user      (1001) user      (1001)     1667 2024-01-31 10:22:57.000000 XEdu-python-0.1.4/XEdu/hub/errorcode.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/font/
--rw-rw-r--   0 user      (1001) user      (1001)  3241748 2023-10-25 09:32:52.000000 XEdu-python-0.1.4/XEdu/hub/font/FZYTK.TTF
--rw-rw-r--   0 user      (1001) user      (1001)   135758 2023-10-19 07:26:34.000000 XEdu-python-0.1.4/XEdu/hub/none.jpg
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/
--rw-r--r--   0 user      (1001) user      (1001)       53 2023-12-18 07:23:59.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)  1356917 2023-12-12 09:36:39.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 user      (1001) user      (1001)    13159 2023-12-13 09:25:30.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/clip_tokenizer.py
--rw-r--r--   0 user      (1001) user      (1001)    24841 2023-12-18 08:05:47.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_squadprocess.py
--rw-r--r--   0 user      (1001) user      (1001)    12359 2023-11-07 13:19:31.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_tokenizer.py
--rw-r--r--   0 user      (1001) user      (1001)   231508 2018-10-18 22:21:12.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_vocab.txt
--rw-rw-r--   0 user      (1001) user      (1001)    78428 2024-04-19 08:26:59.000000 XEdu-python-0.1.4/XEdu/hub/workflow.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/utils/
--rw-r--r--   0 user      (1001) user      (1001)       20 2023-12-13 09:36:29.000000 XEdu-python-0.1.4/XEdu/utils/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     3723 2023-12-14 06:42:53.000000 XEdu-python-0.1.4/XEdu/utils/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)     2230 2024-04-19 07:31:43.000000 XEdu-python-0.1.4/XEdu/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      252 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      964 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       45 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)      107 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        5 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-12-19 09:50:02.000000 XEdu-python-0.1.4/XEdu_python.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      106 2024-04-19 07:30:10.000000 XEdu-python-0.1.4/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3575 2024-04-19 07:31:31.000000 XEdu-python-0.1.4/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.845916 XEdu-python-0.1.5/
+-rw-rw-r--   0 user      (1001) user      (1001)      192 2023-12-19 09:45:45.000000 XEdu-python-0.1.5/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      252 2024-05-13 08:34:04.845916 XEdu-python-0.1.5/PKG-INFO
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.837917 XEdu-python-0.1.5/XEdu/
+-rw-rw-r--   0 user      (1001) user      (1001)     1160 2023-12-19 09:25:26.000000 XEdu-python-0.1.5/XEdu/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.837917 XEdu-python-0.1.5/XEdu/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)      138 2022-08-22 02:06:19.000000 XEdu-python-0.1.5/XEdu/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    22716 2024-05-13 08:29:40.000000 XEdu-python-0.1.5/XEdu/examples/demo.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.837917 XEdu-python-0.1.5/XEdu/hub/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.837917 XEdu-python-0.1.5/XEdu/hub/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-10-07 08:07:43.000000 XEdu-python-0.1.5/XEdu/hub/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    32512 2024-03-15 09:06:21.000000 XEdu-python-0.1.5/XEdu/hub/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 XEdu-python-0.1.5/XEdu/hub/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    37314 2023-06-26 06:07:55.000000 XEdu-python-0.1.5/XEdu/hub/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 XEdu-python-0.1.5/XEdu/hub/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    15668 2023-06-26 05:44:24.000000 XEdu-python-0.1.5/XEdu/hub/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 XEdu-python-0.1.5/XEdu/hub/BaseDT/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)    24028 2023-10-20 05:39:29.000000 XEdu-python-0.1.5/XEdu/hub/BaseDeploy.py
+-rw-rw-r--   0 user      (1001) user      (1001)      124 2023-12-13 09:25:51.000000 XEdu-python-0.1.5/XEdu/hub/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)    35020 2023-12-18 08:16:14.000000 XEdu-python-0.1.5/XEdu/hub/datatset_class.py
+-rw-r--r--   0 user      (1001) user      (1001)     1667 2024-01-31 10:22:57.000000 XEdu-python-0.1.5/XEdu/hub/errorcode.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.837917 XEdu-python-0.1.5/XEdu/hub/font/
+-rw-rw-r--   0 user      (1001) user      (1001)  3241748 2023-10-25 09:32:52.000000 XEdu-python-0.1.5/XEdu/hub/font/FZYTK.TTF
+-rw-rw-r--   0 user      (1001) user      (1001)   135758 2023-10-19 07:26:34.000000 XEdu-python-0.1.5/XEdu/hub/none.jpg
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.841916 XEdu-python-0.1.5/XEdu/hub/tokenizer/
+-rw-r--r--   0 user      (1001) user      (1001)       53 2023-12-18 07:23:59.000000 XEdu-python-0.1.5/XEdu/hub/tokenizer/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)  1356917 2023-12-12 09:36:39.000000 XEdu-python-0.1.5/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 user      (1001) user      (1001)    13159 2023-12-13 09:25:30.000000 XEdu-python-0.1.5/XEdu/hub/tokenizer/clip_tokenizer.py
+-rw-r--r--   0 user      (1001) user      (1001)    24841 2023-12-18 08:05:47.000000 XEdu-python-0.1.5/XEdu/hub/tokenizer/qa_squadprocess.py
+-rw-r--r--   0 user      (1001) user      (1001)    12359 2023-11-07 13:19:31.000000 XEdu-python-0.1.5/XEdu/hub/tokenizer/qa_tokenizer.py
+-rw-r--r--   0 user      (1001) user      (1001)   231508 2018-10-18 22:21:12.000000 XEdu-python-0.1.5/XEdu/hub/tokenizer/qa_vocab.txt
+-rw-rw-r--   0 user      (1001) user      (1001)    78428 2024-04-19 08:26:59.000000 XEdu-python-0.1.5/XEdu/hub/workflow.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.845916 XEdu-python-0.1.5/XEdu/utils/
+-rw-r--r--   0 user      (1001) user      (1001)       20 2023-12-13 09:36:29.000000 XEdu-python-0.1.5/XEdu/utils/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     9515 2024-05-13 08:32:49.000000 XEdu-python-0.1.5/XEdu/utils/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2230 2024-05-13 08:33:35.000000 XEdu-python-0.1.5/XEdu/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 08:34:04.845916 XEdu-python-0.1.5/XEdu_python.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      252 2024-05-13 08:34:04.000000 XEdu-python-0.1.5/XEdu_python.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      964 2024-05-13 08:34:04.000000 XEdu-python-0.1.5/XEdu_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2024-05-13 08:34:04.000000 XEdu-python-0.1.5/XEdu_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       45 2024-05-13 08:34:04.000000 XEdu-python-0.1.5/XEdu_python.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)      107 2024-05-13 08:34:04.000000 XEdu-python-0.1.5/XEdu_python.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        5 2024-05-13 08:34:04.000000 XEdu-python-0.1.5/XEdu_python.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-12-19 09:50:02.000000 XEdu-python-0.1.5/XEdu_python.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      106 2024-04-19 07:30:10.000000 XEdu-python-0.1.5/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2024-05-13 08:34:04.845916 XEdu-python-0.1.5/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3575 2024-05-13 08:33:44.000000 XEdu-python-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `XEdu-python-0.1.4/XEdu/__init__.py` & `XEdu-python-0.1.5/XEdu/__init__.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/examples/demo.py` & `XEdu-python-0.1.5/XEdu/examples/demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -273,47 +273,46 @@
 
     drp.show(image)
     # drp.save(image,"demo_ou.jpg")
 
 def embedding_demo():
     # 导入依赖库
     from XEdu.hub import Workflow as wf
-    from XEdu.utils import get_similarity
+    from XEdu.utils import get_similarity,visualize_similarity,visualize_probability
     # 实例化图像嵌入模型
     img_emb = wf(task='embedding_image')
     # 实例化文本嵌入模型
     text_emb = wf(task='embedding_text')
-    images = ["cat.jpg"]
+    images = ["cat.jpg","cat1.jpg","cat2.jpg","cat3.jpg","ele.jpg","dog.jpg"]
+    # images = images*4
     texts_zh = ["猫", "狗"]
-    texts_en = ["cat", "dog"]
+    texts_en = ["cat", "dog","room","elephant"]
 
     image_embeddings = img_emb.inference(data=images)
     text_zh_embeddings = text_emb.inference(data=texts_zh)
     text_en_embeddings = text_emb.inference(data=texts_en)
 
-    # logits = get_similarity(image_embeddings,text_zh_embeddings,method='cosine',use_softmax=False)
-    logits = get_similarity(text_en_embeddings,text_zh_embeddings) # ,method='cosine',use_softmax=False)
-    print("cosine", logits)
+    # # 图像 - 文本相似度
+    logits = get_similarity(image_embeddings,text_en_embeddings,method='euclidean',use_softmax=False)
+    visualize_similarity(logits, images, texts_en)
+    visualize_probability(logits, images, texts_en,topk=6)
+
+    # 文本 - 文本相似度
+    logits = get_similarity(text_en_embeddings,text_en_embeddings ,method='cosine',use_softmax=False)
+    visualize_similarity(logits, texts_en, texts_en)
+
+    # 文本 - 图像相似度
+    logits = get_similarity(text_en_embeddings,image_embeddings,method='cosine',use_softmax=False)
+    visualize_similarity(logits, texts_en, images)
+
+    # 图像 - 图像相似度
+    logits = get_similarity(image_embeddings,image_embeddings,method='cosine',use_softmax=False)
+    visualize_similarity(logits, images, images)
 
-    # 导入依赖库
-    from XEdu.hub import Workflow as wf
-    from XEdu.utils import get_similarity
-    # 实例化图像嵌入模型
-    img_emb = wf(task='embedding_image')
-    # 实例化文本嵌入模型
-    text_emb = wf(task='embedding_text')
-    # 示例输入
-    images = ["cat.jpg"]
-    texts = ["猫", "狗"]
-    # 对图像进行编码
-    image_embeddings = img_emb.inference(data=images)
-    # 对文本进行编码
-    text_embeddings = text_emb.inference(data=texts)
-    # 计算相似度
-    similarity = get_similarity(image_embeddings,text_embeddings,method='cosine')
+    print("cosine", logits)
 
 
 def openvino_demo():
     import openvino as ov 
     from openvino.runtime import Core
     ie = Core()
     devices = ie.available_devices
@@ -398,14 +397,220 @@
     from XEdu.hub import Workflow as wf
     color = wf(task='gen_color',download_path='new_download')# ,checkpoint='/home/user/下载/colorization-master/colorizer_siggraph17.onnx')
     img = cv2.imread('/home/user/下载/colorization-master/imgs/ansel_adams3.jpg')
     result = color.inference(data='/home/user/下载/colorization-master/imgs/ansel_adams3.jpg',img_type='pil')
     color.save(result,"color_ou.jpg")
 
 
+def kimi_stream_demo():
+    import os
+    from openai import OpenAI
+    
+    client = OpenAI(
+        api_key="sk-c1nBfFK5mcwtilUBr6uvAVulwUhIBWNOqrbVZstvmwBXUcI9",
+        base_url="https://api.moonshot.cn/v1",
+    )
+    
+    response = client.chat.completions.create(
+        model="moonshot-v1-8k",
+        messages=[
+            {
+                "role": "system",
+                "content": "你是 Kimi，由 Moonshot AI 提供的人工智能助手，你更擅长中文和英文的对话。你会为用户提供安全，有帮助，准确的回答。同时，你会拒绝一切涉及恐怖主义，种族歧视，黄色暴力等问题的回答。Moonshot AI 为专有名词，不可翻译成其他语言。",
+            },
+            {"role": "user", "content": "你好，我叫李雷，1+1等于多少？"},
+        ],
+        temperature=0.3,
+        stream=True,
+    )
+    
+    collected_messages = []
+    for idx, chunk in enumerate(response):
+        # print("Chunk received, value: ", chunk)
+        chunk_message = chunk.choices[0].delta
+        if not chunk_message.content:
+            continue
+        collected_messages.append(chunk_message)  # save the message
+        print(f"#{idx}: {''.join([m.content for m in collected_messages])}")
+    print(f"Full conversation received: {''.join([m.content for m in collected_messages])}")
+
+def  llm_stream():
+    import json
+    import requests
+
+    url = "https://api.moonshot.cn/v1"  # 替换为目标URL
+    data = {
+        "stream": True,
+        "model": "moonshot-v1-8k",
+        "messages": [
+            {
+                "role": "user",
+                "content": "你是谁"
+            },
+        ]
+    }
+    headers = {
+        "Authorization": "Bearer sk-c1nBfFK5mcwtilUBr6uvAVulwUhIBWNOqrbVZstvmwBXUcI9",
+    }
+
+    # 使用 with 语句确保请求完成后释放资源
+    with requests.post(url, json=data, headers=headers, timeout=60000, stream=True) as response:
+        # print(response.headers)
+        for chunk in response.iter_lines(chunk_size=None):
+            mChunk = chunk.decode('utf-8')
+            if "[DONE]" in mChunk:
+                break
+            print(mChunk)
+            lines = mChunk.splitlines()
+            for line in lines:
+                respStr = line.strip().replace("data: ", "")
+                respContent = ""
+                try:
+                    respJson = json.loads(respStr)
+                    respContent = respJson["choices"][0]["delta"]["content"]
+                except  Exception as e:
+                    respContent = ""
+                print(respContent)
+
+# 存储各种服务的API Key和URL
+class ServiceProvider:
+    BASE_URL = {
+        "openrouter":"https://openrouter.ai/api/v1/chat/completions",
+        "moonshot":"https://api.moonshot.cn/v1/chat/completions",
+        "google": "https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key=AIzaSyBY-2VWbVvWybt8qjnruUY4tip4X_OwCp8"
+
+    }
+    API_KEY = {
+        "openrouter": "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",
+        "moonshot": "sk-c1nBfFK5mcwtilUBr6uvAVulwUhIBWNOqrbVZstvmwBXUcI9",
+        "google": "AIzaSyBY-2VWbVvWybt8qjnruUY4tip4X_OwCp8"
+    }
+    MODEL = {
+        "openrouter": "mistralai/mistral-7b-instruct:free",
+        "moonshot": "moonshot-v1-8k",
+        "google": "gemini-pro"
+    }
+    def __init__(self, service_name):
+        self.api_key = ServiceProvider.API_KEY[service_name]
+        self.url = ServiceProvider.BASE_URL[service_name]
+        self.model = ServiceProvider.MODEL[service_name]
+import requests
+import json
+class Client:
+    """docstring for Client
+    
+    """
+
+    def __init__(self, provider=None,base_url=None,api_key=None,model=None):
+        self.provider = provider
+        self.base_url = base_url
+        self.api_key = api_key
+        self.model = model
+
+        if provider:
+            self.api_key = ServiceProvider.API_KEY[provider]
+            self.url = ServiceProvider.BASE_URL[provider]
+            self.model = ServiceProvider.MODEL[provider]
+    
+    def inference(self, message, stream=False):
+        if isinstance(message,str):
+            messages = [{"role": "user", "content": message}]
+        else:
+            messages = message
+        if stream:
+            data = json.dumps({
+                        "model": self.model, # Optional
+                        "messages": messages,
+                        "stream": stream,
+                    })
+        else:
+            data = json.dumps({
+                        "model": self.model, # Optional
+                        "messages": messages,
+                    })
+        response = requests.post(
+            url=self.url,
+            headers={
+                'Accept': 'text/event-stream',
+                "Authorization": f"Bearer {self.api_key}",
+                "Content-Type": "application/json",
+            },
+            data=data
+            # stream=stream,
+        )
+        if stream:
+            content = ''
+            for output in response.iter_lines(chunk_size=None):
+                # print("+++++++++++",output)
+                if output==b'data: [DONE]':
+                    break
+                # 判断content是否为空
+                elif output[:6] == b'data: ':
+                    # print("------------",output[6:])
+                    data = output[6:]
+                    output = json.loads(data)
+                    content = output["choices"][0]["delta"]["content"]# .encode('latin1').decode('utf-8')
+        else:
+            try:
+                content = response.json()["choices"][0]["message"]
+            except Exception as e:
+                content = response.json()
+
+        print(content)
+        return content
+
+def llm_demo(stream=False):
+    import requests
+    import json
+    # openrouter = ServiceProvider("google")
+    openrouter = ServiceProvider("openrouter")
+    # openrouter = ServiceProvider("moonshot")
+
+    data = json.dumps({
+            "model": openrouter.model, # Optional
+            "messages": [
+            {"role": "user", "content": "你好,用中文介绍一下你自己"}
+            ],
+            "stream": stream,
+        })
+    gemini_data = json.dumps({
+      "contents": [{
+        "parts":[{"text": "Give me python code to sort a list."}]
+        }]
+        })
+    response = requests.post(
+        url=openrouter.url,
+        headers={
+            'Accept': 'text/event-stream',
+            "Authorization": f"Bearer {openrouter.api_key}",
+            "Content-Type": "application/json",
+        },
+        data=data
+        # stream=stream,
+    )
+    # print(response.text)
+    content = ''
+    for output in response.iter_lines(chunk_size=None):
+        # print("+++++++++++",output)
+        if output==b'data: [DONE]':
+            break
+        # 判断content是否为空
+        elif output[:6] == b'data: ':
+            # print("------------",output[6:])
+            data = output[6:]
+            # try:
+            output = json.loads(data)
+            # except Exception as e:
+            #     print(data)
+            
+            content = output["choices"][0]["delta"]["content"]# .encode('latin1').decode('utf-8')
+            # print(content)
+            print(content)
+
+
 if __name__ == "__main__":
     # pose_infer_demo()
     # det_infer_demo()
     # video_infer_demo()
     # hand_video_demo()
     # coco_det_demo()
     # hand_det_demo()
@@ -415,16 +620,16 @@
     # custom_demo()
     # basenn_demo()
     # cls_demo()
     # baseml_demo()
     # style_demo()
     # qa_demo()
     # drive_demo()
-    # embedding_demo()
-    color_demo()
-    # from openxlab.model import download
-    # download(model_repo='xedu/hub-model', model_name='gen_color.onnx')
-    # url = "https://download.openxlab.org.cn/repos/file/xedu/hub-model/main?filepath=gen_color.onnx&sign=2838feb49073bb8f756d57a9f78a68ab&nonce=1713425582020"
-    # path = "git-lfs/gen_color.onnx"
-    # downloader = Downloader(url, path)
-    # downloader.start()
+    embedding_demo()
+    # color_demo()
+    # kimi_stream_demo()
+    # llm_demo(stream=True)
+    # client = Client(provider="openrouter")
+    # client.inference("你好,用中文介绍一下你自己")
+    # llm_stream()
+
```

### Comparing `XEdu-python-0.1.4/XEdu/hub/BaseDT/data.py` & `XEdu-python-0.1.5/XEdu/hub/BaseDT/data.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/BaseDT/data_image.py` & `XEdu-python-0.1.5/XEdu/hub/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/BaseDT/dataset.py` & `XEdu-python-0.1.5/XEdu/hub/BaseDT/dataset.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/BaseDT/io.py` & `XEdu-python-0.1.5/XEdu/hub/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/BaseDT/plot.py` & `XEdu-python-0.1.5/XEdu/hub/BaseDT/plot.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/BaseDT/utils.py` & `XEdu-python-0.1.5/XEdu/hub/BaseDT/utils.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/BaseDeploy.py` & `XEdu-python-0.1.5/XEdu/hub/BaseDeploy.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/datatset_class.py` & `XEdu-python-0.1.5/XEdu/hub/datatset_class.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/errorcode.py` & `XEdu-python-0.1.5/XEdu/hub/errorcode.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/font/FZYTK.TTF` & `XEdu-python-0.1.5/XEdu/hub/font/FZYTK.TTF`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/none.jpg` & `XEdu-python-0.1.5/XEdu/hub/none.jpg`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz` & `XEdu-python-0.1.5/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/tokenizer/clip_tokenizer.py` & `XEdu-python-0.1.5/XEdu/hub/tokenizer/clip_tokenizer.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_squadprocess.py` & `XEdu-python-0.1.5/XEdu/hub/tokenizer/qa_squadprocess.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_tokenizer.py` & `XEdu-python-0.1.5/XEdu/hub/tokenizer/qa_tokenizer.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_vocab.txt` & `XEdu-python-0.1.5/XEdu/hub/tokenizer/qa_vocab.txt`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/hub/workflow.py` & `XEdu-python-0.1.5/XEdu/hub/workflow.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/XEdu/version.py` & `XEdu-python-0.1.5/XEdu/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.4'
+__version__='0.1.5'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `XEdu-python-0.1.4/XEdu_python.egg-info/SOURCES.txt` & `XEdu-python-0.1.5/XEdu_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.4/setup.py` & `XEdu-python-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='XEdu-python',
-    version='0.1.4',
+    version='0.1.5',
     description='XEdu',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

