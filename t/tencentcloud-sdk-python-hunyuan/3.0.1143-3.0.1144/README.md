# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1143.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1143.tar", last modified: Wed May  8 21:06:08 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1144.tar", last modified: Mon May 13 04:53:37 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1144.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)     2032 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39983 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7419 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/hunyuan_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/setup.py
--rw-r--r--   0 root         (0) root         (0)      749 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-08 21:06:08.000000 tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      539 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)    48610 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-13 04:53:37.000000 tencentcloud-sdk-python-hunyuan-3.0.1144/setup.py
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1143
+Version: 3.0.1144
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class ChatCompletionsRequest(AbstractModel):
     """ChatCompletions请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Model: 模型名称，可选值包括 hunyuan-lite、hunyuan-standard、hunyuan-pro。
+        :param _Model: 模型名称，可选值包括 hunyuan-lite、hunyuan-standard、hunyuan-standard-256K、hunyuan-pro。
 各模型介绍请阅读 [产品概述](https://cloud.tencent.com/document/product/1729/104753) 中的说明。
 
 注意：
 不同的模型计费不同，请根据 [购买指南](https://cloud.tencent.com/document/product/1729/97731) 按需调用。
         :type Model: str
         :param _Messages: 聊天上下文信息。
 说明：
@@ -1188,14 +1188,290 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class QueryHunyuanImageJobRequest(AbstractModel):
+    """QueryHunyuanImageJob请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _JobId: 任务 ID。
+        :type JobId: str
+        """
+        self._JobId = None
+
+    @property
+    def JobId(self):
+        return self._JobId
+
+    @JobId.setter
+    def JobId(self, JobId):
+        self._JobId = JobId
+
+
+    def _deserialize(self, params):
+        self._JobId = params.get("JobId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class QueryHunyuanImageJobResponse(AbstractModel):
+    """QueryHunyuanImageJob返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _JobStatusCode: 当前任务状态码：
+1：等待中、2：运行中、4：处理失败、5：处理完成。
+        :type JobStatusCode: str
+        :param _JobStatusMsg: 当前任务状态：排队中、处理中、处理失败或者处理完成。
+
+        :type JobStatusMsg: str
+        :param _JobErrorCode: 任务处理失败错误码。
+
+        :type JobErrorCode: str
+        :param _JobErrorMsg: 任务处理失败错误信息。
+
+        :type JobErrorMsg: str
+        :param _ResultImage: 生成图 URL 列表，有效期1小时，请及时保存。
+
+        :type ResultImage: list of str
+        :param _ResultDetails: 结果 detail 数组，Success 代表成功。
+
+        :type ResultDetails: list of str
+        :param _RevisedPrompt: 对应 SubmitTextToImageProJob 接口中 Revise 参数。开启扩写时，返回扩写后的 prompt 文本。 如果关闭扩写，将直接返回原始输入的 prompt。
+        :type RevisedPrompt: list of str
+        :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._JobStatusCode = None
+        self._JobStatusMsg = None
+        self._JobErrorCode = None
+        self._JobErrorMsg = None
+        self._ResultImage = None
+        self._ResultDetails = None
+        self._RevisedPrompt = None
+        self._RequestId = None
+
+    @property
+    def JobStatusCode(self):
+        return self._JobStatusCode
+
+    @JobStatusCode.setter
+    def JobStatusCode(self, JobStatusCode):
+        self._JobStatusCode = JobStatusCode
+
+    @property
+    def JobStatusMsg(self):
+        return self._JobStatusMsg
+
+    @JobStatusMsg.setter
+    def JobStatusMsg(self, JobStatusMsg):
+        self._JobStatusMsg = JobStatusMsg
+
+    @property
+    def JobErrorCode(self):
+        return self._JobErrorCode
+
+    @JobErrorCode.setter
+    def JobErrorCode(self, JobErrorCode):
+        self._JobErrorCode = JobErrorCode
+
+    @property
+    def JobErrorMsg(self):
+        return self._JobErrorMsg
+
+    @JobErrorMsg.setter
+    def JobErrorMsg(self, JobErrorMsg):
+        self._JobErrorMsg = JobErrorMsg
+
+    @property
+    def ResultImage(self):
+        return self._ResultImage
+
+    @ResultImage.setter
+    def ResultImage(self, ResultImage):
+        self._ResultImage = ResultImage
+
+    @property
+    def ResultDetails(self):
+        return self._ResultDetails
+
+    @ResultDetails.setter
+    def ResultDetails(self, ResultDetails):
+        self._ResultDetails = ResultDetails
+
+    @property
+    def RevisedPrompt(self):
+        return self._RevisedPrompt
+
+    @RevisedPrompt.setter
+    def RevisedPrompt(self, RevisedPrompt):
+        self._RevisedPrompt = RevisedPrompt
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._JobStatusCode = params.get("JobStatusCode")
+        self._JobStatusMsg = params.get("JobStatusMsg")
+        self._JobErrorCode = params.get("JobErrorCode")
+        self._JobErrorMsg = params.get("JobErrorMsg")
+        self._ResultImage = params.get("ResultImage")
+        self._ResultDetails = params.get("ResultDetails")
+        self._RevisedPrompt = params.get("RevisedPrompt")
+        self._RequestId = params.get("RequestId")
+
+
+class SubmitHunyuanImageJobRequest(AbstractModel):
+    """SubmitHunyuanImageJob请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Prompt: 文本描述。 算法将根据输入的文本智能生成与之相关的图像。 不能为空，推荐使用中文。最多可传100个 utf-8 字符。
+        :type Prompt: str
+        :param _Style: 绘画风格。
+请在 [混元生图风格列表](https://cloud.tencent.com/document/product/1729/105846) 中选择期望的风格，传入风格编号。
+不传默认不指定风格。
+        :type Style: str
+        :param _Resolution: 生成图分辨率。
+支持生成以下分辨率的图片：768:768（1:1）、768:1024（3:4）、1024:768（4:3）、1024:1024（1:1）、720:1280（9:16）、1280:720（16:9）、768:1280（3:5）、1280:768（5:3），不传默认使用1024:1024。
+        :type Resolution: str
+        :param _LogoAdd: 为生成结果图添加显式水印标识的开关，默认为1。  
+1：添加。  
+0：不添加。  
+其他数值：默认按1处理。  
+建议您使用显著标识来提示结果图使用了 AI 绘画技术，是 AI 生成的图片。
+        :type LogoAdd: int
+        :param _Revise: prompt 扩写开关。1为开启，0为关闭，不传默认开启。
+开启扩写后，将自动扩写原始输入的 prompt 并使用扩写后的 prompt 生成图片，返回生成图片结果时将一并返回扩写后的 prompt 文本。
+如果关闭扩写，将直接使用原始输入的 prompt 生成图片。
+建议开启，在多数场景下可提升生成图片效果、丰富生成图片细节。
+        :type Revise: int
+        """
+        self._Prompt = None
+        self._Style = None
+        self._Resolution = None
+        self._LogoAdd = None
+        self._Revise = None
+
+    @property
+    def Prompt(self):
+        return self._Prompt
+
+    @Prompt.setter
+    def Prompt(self, Prompt):
+        self._Prompt = Prompt
+
+    @property
+    def Style(self):
+        return self._Style
+
+    @Style.setter
+    def Style(self, Style):
+        self._Style = Style
+
+    @property
+    def Resolution(self):
+        return self._Resolution
+
+    @Resolution.setter
+    def Resolution(self, Resolution):
+        self._Resolution = Resolution
+
+    @property
+    def LogoAdd(self):
+        return self._LogoAdd
+
+    @LogoAdd.setter
+    def LogoAdd(self, LogoAdd):
+        self._LogoAdd = LogoAdd
+
+    @property
+    def Revise(self):
+        return self._Revise
+
+    @Revise.setter
+    def Revise(self, Revise):
+        self._Revise = Revise
+
+
+    def _deserialize(self, params):
+        self._Prompt = params.get("Prompt")
+        self._Style = params.get("Style")
+        self._Resolution = params.get("Resolution")
+        self._LogoAdd = params.get("LogoAdd")
+        self._Revise = params.get("Revise")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SubmitHunyuanImageJobResponse(AbstractModel):
+    """SubmitHunyuanImageJob返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _JobId: 任务 ID。
+        :type JobId: str
+        :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._JobId = None
+        self._RequestId = None
+
+    @property
+    def JobId(self):
+        return self._JobId
+
+    @JobId.setter
+    def JobId(self, JobId):
+        self._JobId = JobId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._JobId = params.get("JobId")
+        self._RequestId = params.get("RequestId")
+
+
 class Usage(AbstractModel):
     """Token 数量
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -135,8 +135,60 @@
             model = models.GetTokenCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def QueryHunyuanImageJob(self, request):
+        """混元生图接口基于混元大模型，将根据输入的文本描述，智能生成与之相关的结果图。分为提交任务和查询任务2个接口。
+        提交任务：输入文本等，提交一个混元生图异步任务，获得任务 ID。
+        查询任务：根据任务 ID 查询任务的处理状态、处理结果，任务处理完成后可获得生成图像结果。
+        并发任务数（并发）说明：并发任务数指能同时处理的任务数量。混元生图默认提供1个并发任务数，代表最多能同时处理1个已提交的任务，上一个任务处理完毕后才能开始处理下一个任务。
+
+        :param request: Request instance for QueryHunyuanImageJob.
+        :type request: :class:`tencentcloud.hunyuan.v20230901.models.QueryHunyuanImageJobRequest`
+        :rtype: :class:`tencentcloud.hunyuan.v20230901.models.QueryHunyuanImageJobResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("QueryHunyuanImageJob", params, headers=headers)
+            response = json.loads(body)
+            model = models.QueryHunyuanImageJobResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def SubmitHunyuanImageJob(self, request):
+        """混元生图接口基于混元大模型，将根据输入的文本描述，智能生成与之相关的结果图。分为提交任务和查询任务2个接口。
+        提交任务：输入文本等，提交一个混元生图异步任务，获得任务 ID。
+        查询任务：根据任务 ID 查询任务的处理状态、处理结果，任务处理完成后可获得生成图像结果。
+        并发任务数（并发）说明：并发任务数指能同时处理的任务数量。混元生图默认提供1个并发任务数，代表最多能同时处理1个已提交的任务，上一个任务处理完毕后才能开始处理下一个任务。
+
+        :param request: Request instance for SubmitHunyuanImageJob.
+        :type request: :class:`tencentcloud.hunyuan.v20230901.models.SubmitHunyuanImageJobRequest`
+        :rtype: :class:`tencentcloud.hunyuan.v20230901.models.SubmitHunyuanImageJobResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SubmitHunyuanImageJob", params, headers=headers)
+            response = json.loads(body)
+            model = models.SubmitHunyuanImageJobResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1144/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1143"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1144"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1144/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1144/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1143
+Version: 3.0.1144
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1143/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1144/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

