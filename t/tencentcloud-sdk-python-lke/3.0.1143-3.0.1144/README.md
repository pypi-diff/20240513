# Comparing `tmp/tencentcloud-sdk-python-lke-3.0.1143.tar.gz` & `tmp/tencentcloud-sdk-python-lke-3.0.1144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1143.tar", last modified: Wed May  8 21:17:04 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1144.tar", last modified: Mon May 13 04:58:40 2024, max compression
```

## Comparing `tencentcloud-sdk-python-lke-3.0.1143.tar` & `tencentcloud-sdk-python-lke-3.0.1144.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud_sdk_python_lke.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud_sdk_python_lke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud_sdk_python_lke.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   379527 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/models.py
--rw-r--r--   0 root         (0) root         (0)    66032 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/lke_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-08 21:17:04.000000 tencentcloud-sdk-python-lke-3.0.1143/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/
+-rw-r--r--   0 root         (0) root         (0)   384266 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/models.py
+-rw-r--r--   0 root         (0) root         (0)    66494 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/lke_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud_sdk_python_lke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud_sdk_python_lke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/tencentcloud_sdk_python_lke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-13 04:58:40.000000 tencentcloud-sdk-python-lke-3.0.1144/setup.py
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1144/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1143
+Version: 3.0.1144
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/tencentcloud_sdk_python_lke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1144/tencentcloud_sdk_python_lke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1143
+Version: 3.0.1144
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1143'
+__version__ = '3.0.1144'
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/errorcodes.py` & `tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/models.py` & `tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10526,14 +10526,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Content: 内容
         :type Content: str
+        :param _SessionId: 当前记录所对应的 Session ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionId: str
         :param _RecordId: 记录ID
         :type RecordId: str
         :param _RelatedRecordId: 关联记录ID
         :type RelatedRecordId: str
         :param _IsFromSelf: 是否来自自己
         :type IsFromSelf: bool
         :param _FromName: 发送者名称
@@ -10544,54 +10547,79 @@
         :type Timestamp: str
         :param _HasRead: 是否已读
         :type HasRead: bool
         :param _Score: 评价
         :type Score: int
         :param _CanRating: 是否评分
         :type CanRating: bool
+        :param _CanFeedback: 是否展示反馈按钮
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CanFeedback: bool
         :param _Type: 记录类型
         :type Type: int
         :param _References: 引用来源
         :type References: list of MsgRecordReference
         :param _Reasons: 评价原因
         :type Reasons: list of str
         :param _IsLlmGenerated: 是否大模型
         :type IsLlmGenerated: bool
         :param _ImageUrls: 图片链接，可公有读
         :type ImageUrls: list of str
         :param _TokenStat: 当次 token 统计信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type TokenStat: :class:`tencentcloud.lke.v20231130.models.TokenStat`
+        :param _ReplyMethod: 回复方式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ReplyMethod: int
+        :param _OptionCards: 选项卡, 用于多轮对话
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OptionCards: list of str
+        :param _TaskFlow: 任务信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskFlow: :class:`tencentcloud.lke.v20231130.models.TaskFlowInfo`
         """
         self._Content = None
+        self._SessionId = None
         self._RecordId = None
         self._RelatedRecordId = None
         self._IsFromSelf = None
         self._FromName = None
         self._FromAvatar = None
         self._Timestamp = None
         self._HasRead = None
         self._Score = None
         self._CanRating = None
+        self._CanFeedback = None
         self._Type = None
         self._References = None
         self._Reasons = None
         self._IsLlmGenerated = None
         self._ImageUrls = None
         self._TokenStat = None
+        self._ReplyMethod = None
+        self._OptionCards = None
+        self._TaskFlow = None
 
     @property
     def Content(self):
         return self._Content
 
     @Content.setter
     def Content(self, Content):
         self._Content = Content
 
     @property
+    def SessionId(self):
+        return self._SessionId
+
+    @SessionId.setter
+    def SessionId(self, SessionId):
+        self._SessionId = SessionId
+
+    @property
     def RecordId(self):
         return self._RecordId
 
     @RecordId.setter
     def RecordId(self, RecordId):
         self._RecordId = RecordId
 
@@ -10656,14 +10684,22 @@
         return self._CanRating
 
     @CanRating.setter
     def CanRating(self, CanRating):
         self._CanRating = CanRating
 
     @property
+    def CanFeedback(self):
+        return self._CanFeedback
+
+    @CanFeedback.setter
+    def CanFeedback(self, CanFeedback):
+        self._CanFeedback = CanFeedback
+
+    @property
     def Type(self):
         return self._Type
 
     @Type.setter
     def Type(self, Type):
         self._Type = Type
 
@@ -10703,39 +10739,70 @@
     def TokenStat(self):
         return self._TokenStat
 
     @TokenStat.setter
     def TokenStat(self, TokenStat):
         self._TokenStat = TokenStat
 
+    @property
+    def ReplyMethod(self):
+        return self._ReplyMethod
+
+    @ReplyMethod.setter
+    def ReplyMethod(self, ReplyMethod):
+        self._ReplyMethod = ReplyMethod
+
+    @property
+    def OptionCards(self):
+        return self._OptionCards
+
+    @OptionCards.setter
+    def OptionCards(self, OptionCards):
+        self._OptionCards = OptionCards
+
+    @property
+    def TaskFlow(self):
+        return self._TaskFlow
+
+    @TaskFlow.setter
+    def TaskFlow(self, TaskFlow):
+        self._TaskFlow = TaskFlow
+
 
     def _deserialize(self, params):
         self._Content = params.get("Content")
+        self._SessionId = params.get("SessionId")
         self._RecordId = params.get("RecordId")
         self._RelatedRecordId = params.get("RelatedRecordId")
         self._IsFromSelf = params.get("IsFromSelf")
         self._FromName = params.get("FromName")
         self._FromAvatar = params.get("FromAvatar")
         self._Timestamp = params.get("Timestamp")
         self._HasRead = params.get("HasRead")
         self._Score = params.get("Score")
         self._CanRating = params.get("CanRating")
+        self._CanFeedback = params.get("CanFeedback")
         self._Type = params.get("Type")
         if params.get("References") is not None:
             self._References = []
             for item in params.get("References"):
                 obj = MsgRecordReference()
                 obj._deserialize(item)
                 self._References.append(obj)
         self._Reasons = params.get("Reasons")
         self._IsLlmGenerated = params.get("IsLlmGenerated")
         self._ImageUrls = params.get("ImageUrls")
         if params.get("TokenStat") is not None:
             self._TokenStat = TokenStat()
             self._TokenStat._deserialize(params.get("TokenStat"))
+        self._ReplyMethod = params.get("ReplyMethod")
+        self._OptionCards = params.get("OptionCards")
+        if params.get("TaskFlow") is not None:
+            self._TaskFlow = TaskFlowInfo()
+            self._TaskFlow._deserialize(params.get("TaskFlow"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -13286,14 +13353,104 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TaskFlowInfo(AbstractModel):
+    """任务流程信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskFlowId: 任务流程ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskFlowId: str
+        :param _TaskFlowName: 任务流程名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskFlowName: str
+        :param _QueryRewrite: Query 重写结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QueryRewrite: str
+        :param _HitIntent: 命中意图
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HitIntent: str
+        :param _Type: 任务流程回复类型
+0: 任务流回复
+1: 任务流静默
+2: 任务流拉回话术
+3: 任务流自定义回复
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: int
+        """
+        self._TaskFlowId = None
+        self._TaskFlowName = None
+        self._QueryRewrite = None
+        self._HitIntent = None
+        self._Type = None
+
+    @property
+    def TaskFlowId(self):
+        return self._TaskFlowId
+
+    @TaskFlowId.setter
+    def TaskFlowId(self, TaskFlowId):
+        self._TaskFlowId = TaskFlowId
+
+    @property
+    def TaskFlowName(self):
+        return self._TaskFlowName
+
+    @TaskFlowName.setter
+    def TaskFlowName(self, TaskFlowName):
+        self._TaskFlowName = TaskFlowName
+
+    @property
+    def QueryRewrite(self):
+        return self._QueryRewrite
+
+    @QueryRewrite.setter
+    def QueryRewrite(self, QueryRewrite):
+        self._QueryRewrite = QueryRewrite
+
+    @property
+    def HitIntent(self):
+        return self._HitIntent
+
+    @HitIntent.setter
+    def HitIntent(self, HitIntent):
+        self._HitIntent = HitIntent
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+
+    def _deserialize(self, params):
+        self._TaskFlowId = params.get("TaskFlowId")
+        self._TaskFlowName = params.get("TaskFlowName")
+        self._QueryRewrite = params.get("QueryRewrite")
+        self._HitIntent = params.get("HitIntent")
+        self._Type = params.get("Type")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TaskParams(AbstractModel):
     """任务参数
 
     """
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/tencentcloud/lke/v20231130/lke_client.py` & `tencentcloud-sdk-python-lke-3.0.1144/tencentcloud/lke/v20231130/lke_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -782,16 +782,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEmbedding(self, request):
-        """获取特征向量
-        本接口有单账号调用上限控制，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
+        """本接口（GetEmbedding）调用文本表示模型，将文本转化为用数值表示的向量形式，可用于文本检索、信息推荐、知识挖掘等场景。
+        本接口（GetEmbedding）有单账号调用上限控制，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
 
         :param request: Request instance for GetEmbedding.
         :type request: :class:`tencentcloud.lke.v20231130.models.GetEmbeddingRequest`
         :rtype: :class:`tencentcloud.lke.v20231130.models.GetEmbeddingResponse`
 
         """
         try:
@@ -1519,16 +1519,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryRewrite(self, request):
-        """多轮改写
-        本接口有单账号调用上限控制，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
+        """多轮改写（QueryRewrite）主要用于多轮对话中，进行指代消解和省略补全。使用本接口，无需输入prompt描述，根据对话历史即可生成更精确的用户查询。在应用场景上，本接口可应用于智能问答、对话式搜索等多种场景。
+        本接口（QueryRewrite）有单账号调用上限控制，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
 
         :param request: Request instance for QueryRewrite.
         :type request: :class:`tencentcloud.lke.v20231130.models.QueryRewriteRequest`
         :rtype: :class:`tencentcloud.lke.v20231130.models.QueryRewriteResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/setup.py` & `tencentcloud-sdk-python-lke-3.0.1144/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-lke',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1143"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1144"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Lke SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1143/README.rst` & `tencentcloud-sdk-python-lke-3.0.1144/README.rst`

 * *Files identical despite different names*

