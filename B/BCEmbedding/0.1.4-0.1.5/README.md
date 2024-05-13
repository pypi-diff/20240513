# Comparing `tmp/BCEmbedding-0.1.4-py3-none-any.whl.zip` & `tmp/BCEmbedding-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 30136 bytes, number of entries: 23
+Zip file size: 30132 bytes, number of entries: 23
 -rw-------  2.0 unx      145 b- defN 24-Jan-02 10:43 BCEmbedding/__init__.py
 -rw-------  2.0 unx      146 b- defN 24-Jan-02 10:43 BCEmbedding/evaluation/__init__.py
 -rw-------  2.0 unx     8786 b- defN 24-Jan-11 04:18 BCEmbedding/evaluation/c_mteb/Reranking.py
 -rw-------  2.0 unx    10905 b- defN 24-Jan-02 10:43 BCEmbedding/evaluation/c_mteb/Retrieval.py
 -rw-------  2.0 unx      234 b- defN 24-Jan-02 10:43 BCEmbedding/evaluation/c_mteb/__init__.py
 -rw-------  2.0 unx     3503 b- defN 24-Jan-06 16:17 BCEmbedding/evaluation/c_mteb/yd_dres_model.py
 -rw-------  2.0 unx      250 b- defN 24-Jan-15 16:50 BCEmbedding/models/__init__.py
--rw-------  2.0 unx     4404 b- defN 24-Jan-19 04:10 BCEmbedding/models/embedding.py
--rw-------  2.0 unx     5722 b- defN 24-Jan-19 04:11 BCEmbedding/models/reranker.py
+-rw-------  2.0 unx     4414 b- defN 24-May-13 09:04 BCEmbedding/models/embedding.py
+-rw-------  2.0 unx     5732 b- defN 24-May-13 09:04 BCEmbedding/models/reranker.py
 -rw-------  2.0 unx     2588 b- defN 24-Apr-09 09:33 BCEmbedding/models/utils.py
 -rw-------  2.0 unx      124 b- defN 24-Jan-15 16:53 BCEmbedding/tools/__init__.py
 -rw-------  2.0 unx      158 b- defN 24-Jan-15 16:53 BCEmbedding/tools/langchain/__init__.py
 -rw-------  2.0 unx     3338 b- defN 24-Feb-24 15:19 BCEmbedding/tools/langchain/bce_rerank.py
 -rw-------  2.0 unx      158 b- defN 24-Jan-15 16:53 BCEmbedding/tools/llama_index/__init__.py
 -rw-------  2.0 unx     3151 b- defN 24-Mar-04 08:00 BCEmbedding/tools/llama_index/bce_rerank.py
 -rw-------  2.0 unx      192 b- defN 24-Jan-02 10:43 BCEmbedding/utils/__init__.py
 -rw-------  2.0 unx      401 b- defN 24-Jan-02 10:43 BCEmbedding/utils/logger.py
 -rw-------  2.0 unx     1671 b- defN 24-Jan-06 16:22 BCEmbedding/utils/query_instructions.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-09 09:39 BCEmbedding-0.1.4.dist-info/LICENSE
--rw-------  2.0 unx    32615 b- defN 24-Apr-09 09:39 BCEmbedding-0.1.4.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 24-Apr-09 09:39 BCEmbedding-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-09 09:39 BCEmbedding-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2060 b- defN 24-Apr-09 09:39 BCEmbedding-0.1.4.dist-info/RECORD
-23 files, 92012 bytes uncompressed, 26740 bytes compressed:  70.9%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-13 09:06 BCEmbedding-0.1.5.dist-info/LICENSE
+-rw-------  2.0 unx    32615 b- defN 24-May-13 09:06 BCEmbedding-0.1.5.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 24-May-13 09:06 BCEmbedding-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-13 09:06 BCEmbedding-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2060 b- defN 24-May-13 09:06 BCEmbedding-0.1.5.dist-info/RECORD
+23 files, 92032 bytes uncompressed, 26736 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: BCEmbedding/utils/logger.py
 Comment: 
 
 Filename: BCEmbedding/utils/query_instructions.py
 Comment: 
 
-Filename: BCEmbedding-0.1.4.dist-info/LICENSE
+Filename: BCEmbedding-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: BCEmbedding-0.1.4.dist-info/METADATA
+Filename: BCEmbedding-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: BCEmbedding-0.1.4.dist-info/WHEEL
+Filename: BCEmbedding-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: BCEmbedding-0.1.4.dist-info/top_level.txt
+Filename: BCEmbedding-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: BCEmbedding-0.1.4.dist-info/RECORD
+Filename: BCEmbedding-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## BCEmbedding/models/embedding.py

```diff
@@ -1,12 +1,12 @@
 '''
 @Description: 
 @Author: shenlei
 @Date: 2023-11-28 14:04:27
-@LastEditTime: 2024-01-19 12:10:58
+@LastEditTime: 2024-05-13 17:04:23
 @LastEditors: shenlei
 '''
 import logging
 import torch
 
 from tqdm import tqdm
 from numpy import ndarray
@@ -22,15 +22,15 @@
             self,
             model_name_or_path: str='maidalun1020/bce-embedding-base_v1',
             pooler: str='cls',
             use_fp16: bool=False,
             device: str=None,
             **kwargs
         ):
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
+        self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, **kwargs)
         self.model = AutoModel.from_pretrained(model_name_or_path, **kwargs)
         logger.info(f"Loading from `{model_name_or_path}`.")
 
         assert pooler in ['cls', 'mean'], f"`pooler` should be in ['cls', 'mean']. 'cls' is recommended!"
         self.pooler = pooler
         
         num_gpus = torch.cuda.device_count()
```

## BCEmbedding/models/reranker.py

```diff
@@ -1,12 +1,12 @@
 '''
 @Description: 
 @Author: shenlei
 @Date: 2023-11-28 14:04:27
-@LastEditTime: 2024-01-19 12:11:05
+@LastEditTime: 2024-05-13 17:04:41
 @LastEditors: shenlei
 '''
 import logging
 import torch
 
 import numpy as np
 
@@ -25,15 +25,15 @@
     def __init__(
             self,
             model_name_or_path: str='maidalun1020/bce-reranker-base_v1',
             use_fp16: bool=False,
             device: str=None,
             **kwargs
         ):
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
+        self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, **kwargs)
         self.model = AutoModelForSequenceClassification.from_pretrained(model_name_or_path, **kwargs)
         logger.info(f"Loading from `{model_name_or_path}`.")
         
         num_gpus = torch.cuda.device_count()
         if device is None:
             self.device = "cuda" if num_gpus > 0 else "cpu"
         else:
```

## Comparing `BCEmbedding-0.1.4.dist-info/LICENSE` & `BCEmbedding-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `BCEmbedding-0.1.4.dist-info/METADATA` & `BCEmbedding-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BCEmbedding
-Version: 0.1.4
+Version: 0.1.5
 Summary: A text embedding model and reranking model produced by Netease Youdao Inc., which can be use for dense embedding retrieval and reranking in RAG workflow.
 Home-page: https://gitlab.corp.youdao.com/ai/BCEmbedding
 Author: Netease Youdao, Inc.
 Author-email: shenlei02@corp.netease.com
 License: apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,15 +14,15 @@
 Requires-Dist: sentence-transformers
 
 <!--
  * @Description: 
  * @Author: shenlei
  * @Modified: linhui
  * @Date: 2023-12-19 10:31:41
- * @LastEditTime: 2024-04-09 17:34:35
+ * @LastEditTime: 2024-05-13 17:05:35
  * @LastEditors: shenlei
 -->
 
 <h1 align="center">BCEmbedding: Bilingual and Crosslingual Embedding for RAG</h1>
 
 <div align="center">
     <a href="./LICENSE">
@@ -137,15 +137,15 @@
 conda create --name bce python=3.10 -y
 conda activate bce
 ```
 
 Then install `BCEmbedding` for minimal installation (To avoid cuda version conflicting, you should install [`torch`](https://pytorch.org/get-started/previous-versions/) that is compatible to your system cuda version manually first):
 
 ```bash
-pip install BCEmbedding==0.1.4
+pip install BCEmbedding==0.1.5
 ```
 
 Or install from source (**recommended**):
 
 ```bash
 git clone git@github.com:netease-youdao/BCEmbedding.git
 cd BCEmbedding
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BCEmbedding Version: 0.1.4 Summary: A text
+Metadata-Version: 2.1 Name: BCEmbedding Version: 0.1.5 Summary: A text
 embedding model and reranking model produced by Netease Youdao Inc., which can
 be use for dense embedding retrieval and reranking in RAG workflow. Home-page:
 https://gitlab.corp.youdao.com/ai/BCEmbedding Author: Netease Youdao, Inc.
 Author-email: shenlei02@corp.netease.com License: apache-2.0 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch >=1.6.0
 Requires-Dist: transformers <4.37.0,>=4.35.0 Requires-Dist: datasets Requires-
 Dist: sentence-transformers
@@ -99,15 +99,15 @@
 | ch, en, ja, ko | 279M | [Huggingface](https://huggingface.co/maidalun1020/
 bce-reranker-base_v1), [å½åéé](https://hf-mirror.com/maidalun1020/bce-
 reranker-base_v1) | ## ð Manual ### Installation First, create a conda
 environment and activate it. ```bash conda create --name bce python=3.10 -
 y conda activate bce ``` Then install `BCEmbedding` for minimal installation
 (To avoid cuda version conflicting, you should install [`torch`](https://
 pytorch.org/get-started/previous-versions/) that is compatible to your system
-cuda version manually first): ```bash pip install BCEmbedding==0.1.4 ``` Or
+cuda version manually first): ```bash pip install BCEmbedding==0.1.5 ``` Or
 install from source (**recommended**): ```bash git clone git@github.com:
 netease-youdao/BCEmbedding.git cd BCEmbedding pip install -v -e . ``` ### Quick
 Start #### 1. Based on `BCEmbedding` Use `EmbeddingModel`, and `cls` [pooler]
 (./BCEmbedding/models/embedding.py#L24) is default. ```python from BCEmbedding
 import EmbeddingModel # list of sentences sentences = ['sentence_0',
 'sentence_1'] # init embedding model model = EmbeddingModel
 (model_name_or_path="maidalun1020/bce-embedding-base_v1") # extract embeddings
```

## Comparing `BCEmbedding-0.1.4.dist-info/RECORD` & `BCEmbedding-0.1.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 BCEmbedding/__init__.py,sha256=H35SvW466Df1SHiCaOBfTNFHPnoSSeEKI5dssG1z8hM,145
 BCEmbedding/evaluation/__init__.py,sha256=YefkjYpadq-v3iB41EYw1g7JhPEwx2vC_eWYPehWR3c,146
 BCEmbedding/evaluation/c_mteb/Reranking.py,sha256=pxUVonkWvdIqsX7hg9QN4SY4qSMGY_UWQEZ67n4iV_A,8786
 BCEmbedding/evaluation/c_mteb/Retrieval.py,sha256=S3HsoGJDp5ix9Om8BPp9bgpyZEvCrCwqZMjnkAy7W8U,10905
 BCEmbedding/evaluation/c_mteb/__init__.py,sha256=t4jvOIUMjWwETNvPbxqGPx5UA-719tEmIDoWcEBjwsM,234
 BCEmbedding/evaluation/c_mteb/yd_dres_model.py,sha256=-fo-p-Pz9DTOdDQu9PMVsBDy4hHvmnD3Qda8IoKFRzA,3503
 BCEmbedding/models/__init__.py,sha256=Sm9_on6NLokJ3fjkYHsLW-xLypIdz5ihNVwDvUZ2b9o,250
-BCEmbedding/models/embedding.py,sha256=hqWAuaQsOeNy944QjGlFEaO_69hB__54w8Ef2gqLmBY,4404
-BCEmbedding/models/reranker.py,sha256=8ZP11I1TlI4lxD3QHujh-_N3KGaowHN0oIncJemwXig,5722
+BCEmbedding/models/embedding.py,sha256=y7jmm-bPz4rCz72T-H16dBaL5jNI2FXHrdCtCv2FSQU,4414
+BCEmbedding/models/reranker.py,sha256=wZBJP_YO7PhEYawLzS47Y5eWslRO0nNknsmvftCg9Gk,5732
 BCEmbedding/models/utils.py,sha256=W55zmT9yPqCikitF0t9Qw6OvKCfWH45zgbIT9FDj50o,2588
 BCEmbedding/tools/__init__.py,sha256=N6oz0MICVTEAWdhBgOzq1GVHpgihhcdF3p-_lDDedlk,124
 BCEmbedding/tools/langchain/__init__.py,sha256=CtQePyCxAaLUm3TXiZQGUeSkIN7f7aPRs2eizDpqiB0,158
 BCEmbedding/tools/langchain/bce_rerank.py,sha256=vMZD-L3jb5bzStxfcrm6NkiUxRFvsb_OHyxozb3KjjI,3338
 BCEmbedding/tools/llama_index/__init__.py,sha256=eZ3as37D-xAnf4tquFVNjCHQT16bj2KV2RxLtU2rZos,158
 BCEmbedding/tools/llama_index/bce_rerank.py,sha256=5jqJ8b17q_kiYP1mf0NSWaQLfMWkRVs45TM5iM38SeU,3151
 BCEmbedding/utils/__init__.py,sha256=Xt5C2GkMMaRuV6qbnmnu2OElq0FR0S_2f5Xn9hA7NRs,192
 BCEmbedding/utils/logger.py,sha256=k8d60HuFcaqnUCOwlgJ33n7gyqmXjMgC47tYHj77HLM,401
 BCEmbedding/utils/query_instructions.py,sha256=tywpweF2y3Hf3Uf6meMGK2QqZG6smNeQbbx5mY-ZpQ8,1671
-BCEmbedding-0.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-BCEmbedding-0.1.4.dist-info/METADATA,sha256=qgje9Dq71bJRB2ZWaz-yvLm00xW8vf77YH0YqNnrALM,32615
-BCEmbedding-0.1.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-BCEmbedding-0.1.4.dist-info/top_level.txt,sha256=h6kdwVU7f8_ae0K_sK5wG7m4kdEIpO3DQ-Eb2q-piGA,12
-BCEmbedding-0.1.4.dist-info/RECORD,,
+BCEmbedding-0.1.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+BCEmbedding-0.1.5.dist-info/METADATA,sha256=VOoMGH3JqFeevUNfFSDGdityzJPOPOpne2R7pD4AOLc,32615
+BCEmbedding-0.1.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+BCEmbedding-0.1.5.dist-info/top_level.txt,sha256=h6kdwVU7f8_ae0K_sK5wG7m4kdEIpO3DQ-Eb2q-piGA,12
+BCEmbedding-0.1.5.dist-info/RECORD,,
```

