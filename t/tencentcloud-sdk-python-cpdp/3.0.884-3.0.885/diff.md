# Comparing `tmp/tencentcloud-sdk-python-cpdp-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-cpdp-3.0.885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.884.tar", last modified: Fri Apr 28 02:10:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.885.tar", last modified: Mon May  1 00:33:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cpdp-3.0.884.tar` & `tencentcloud-sdk-python-cpdp-3.0.885.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/
--rw-r--r--   0 root         (0) root         (0)   208899 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/cpdp_client.py
--rw-r--r--   0 root         (0) root         (0)    19183 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1213952 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/models.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud_sdk_python_cpdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/
+-rw-r--r--   0 root         (0) root         (0)   210732 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/cpdp_client.py
+-rw-r--r--   0 root         (0) root         (0)    19183 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1223290 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/models.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:33:36.000000 tencentcloud-sdk-python-cpdp-3.0.885/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/README.rst` & `tencentcloud-sdk-python-cpdp-3.0.885/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.884'
+__version__ = '3.0.885'
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/cpdp_client.py` & `tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/cpdp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ApplyFlexWechatPreAuth(self, request):
+        """微工卡开通预核身接口
+
+        :param request: Request instance for ApplyFlexWechatPreAuth.
+        :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyFlexWechatPreAuthRequest`
+        :rtype: :class:`tencentcloud.cpdp.v20190820.models.ApplyFlexWechatPreAuthResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ApplyFlexWechatPreAuth", params, headers=headers)
+            response = json.loads(body)
+            model = models.ApplyFlexWechatPreAuthResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ApplyOpenBankOrderDetailReceipt(self, request):
         """云企付-申请单笔交易回单
 
         :param request: Request instance for ApplyOpenBankOrderDetailReceipt.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyOpenBankOrderDetailReceiptRequest`
         :rtype: :class:`tencentcloud.cpdp.v20190820.models.ApplyOpenBankOrderDetailReceiptResponse`
 
@@ -3135,14 +3158,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def QueryFlexWechatAuthResult(self, request):
+        """查询微工卡核身结果
+
+        :param request: Request instance for QueryFlexWechatAuthResult.
+        :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexWechatAuthResultRequest`
+        :rtype: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexWechatAuthResultResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("QueryFlexWechatAuthResult", params, headers=headers)
+            response = json.loads(body)
+            model = models.QueryFlexWechatAuthResultResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def QueryFundsTransactionDetails(self, request):
         """聚鑫-查询会员资金交易信息列表
 
         :param request: Request instance for QueryFundsTransactionDetails.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFundsTransactionDetailsRequest`
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/errorcodes.py` & `tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/models.py` & `tencentcloud-sdk-python-cpdp-3.0.885/tencentcloud/cpdp/v20190820/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1638,14 +1638,111 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ApplyFlexWechatPreAuthRequest(AbstractModel):
+    """ApplyFlexWechatPreAuth请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AuthNo: 商家核身单号
+        :type AuthNo: str
+        :param OpenId: 微信用户标识
+        :type OpenId: str
+        :param ProjectName: 项目名称
+        :type ProjectName: str
+        :param EmployerName: 用工单位名称
+        :type EmployerName: str
+        :param UserName: 用户姓名
+        :type UserName: str
+        :param IdNo: 用户证件号
+        :type IdNo: str
+        :param EmploymentType: 用工类型
+LONG_TERM_EMPLOYMENT：长期用工，
+SHORT_TERM_EMPLOYMENT： 短期用工，
+COOPERATION_EMPLOYMENT：合作关系
+        :type EmploymentType: str
+        :param AuthType: 核身类型
+SIGN_IN：考勤、签到打卡类型
+INSURANCE：投保类型
+CONTRACT：签约类型
+        :type AuthType: str
+        :param Environment: 环境类型
+test 测试
+release 生产
+sandbox 沙箱
+        :type Environment: str
+        """
+        self.AuthNo = None
+        self.OpenId = None
+        self.ProjectName = None
+        self.EmployerName = None
+        self.UserName = None
+        self.IdNo = None
+        self.EmploymentType = None
+        self.AuthType = None
+        self.Environment = None
+
+
+    def _deserialize(self, params):
+        self.AuthNo = params.get("AuthNo")
+        self.OpenId = params.get("OpenId")
+        self.ProjectName = params.get("ProjectName")
+        self.EmployerName = params.get("EmployerName")
+        self.UserName = params.get("UserName")
+        self.IdNo = params.get("IdNo")
+        self.EmploymentType = params.get("EmploymentType")
+        self.AuthType = params.get("AuthType")
+        self.Environment = params.get("Environment")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ApplyFlexWechatPreAuthResponse(AbstractModel):
+    """ApplyFlexWechatPreAuth返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ErrCode: 错误码。SUCCESS为成功，其他为失败
+        :type ErrCode: str
+        :param ErrMessage: 错误信息
+        :type ErrMessage: str
+        :param Result: 返回结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: :class:`tencentcloud.cpdp.v20190820.models.WechatPreAuthResult`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ErrCode = None
+        self.ErrMessage = None
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.ErrCode = params.get("ErrCode")
+        self.ErrMessage = params.get("ErrMessage")
+        if params.get("Result") is not None:
+            self.Result = WechatPreAuthResult()
+            self.Result._deserialize(params.get("Result"))
+        self.RequestId = params.get("RequestId")
+
+
 class ApplyOpenBankOrderDetailReceiptRequest(AbstractModel):
     """ApplyOpenBankOrderDetailReceipt请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -20181,14 +20278,77 @@
         self.ErrMessage = params.get("ErrMessage")
         if params.get("Result") is not None:
             self.Result = SettlementOrders()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class QueryFlexWechatAuthResultRequest(AbstractModel):
+    """QueryFlexWechatAuthResult请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AuthNo: 商户核身单号
+        :type AuthNo: str
+        :param Environment: 环境类型
+test 测试
+release 生产
+sandbox 沙箱
+        :type Environment: str
+        """
+        self.AuthNo = None
+        self.Environment = None
+
+
+    def _deserialize(self, params):
+        self.AuthNo = params.get("AuthNo")
+        self.Environment = params.get("Environment")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class QueryFlexWechatAuthResultResponse(AbstractModel):
+    """QueryFlexWechatAuthResult返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ErrCode: 错误码。SUCCESS为成功，其他为失败
+        :type ErrCode: str
+        :param ErrMessage: 错误消息
+        :type ErrMessage: str
+        :param Result: 返回结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: :class:`tencentcloud.cpdp.v20190820.models.QueryWechatAuthResult`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ErrCode = None
+        self.ErrMessage = None
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.ErrCode = params.get("ErrCode")
+        self.ErrMessage = params.get("ErrMessage")
+        if params.get("Result") is not None:
+            self.Result = QueryWechatAuthResult()
+            self.Result._deserialize(params.get("Result"))
+        self.RequestId = params.get("RequestId")
+
+
 class QueryFundsTransactionDetailsRequest(AbstractModel):
     """QueryFundsTransactionDetails请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -26549,14 +26709,98 @@
         self.ErrMessage = params.get("ErrMessage")
         if params.get("Result") is not None:
             self.Result = QueryTransferResultData()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class QueryWechatAuthResult(AbstractModel):
+    """查询用户微工卡核身结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AuthNo: 商户核身单号
+        :type AuthNo: str
+        :param OpenId: 微信用户标识
+        :type OpenId: str
+        :param MchId: 商户号
+        :type MchId: str
+        :param SubMchId: 子商户号
+        :type SubMchId: str
+        :param AuthScene: 核身渠道
+FROM_MINI_APP：来自小程序方式核身
+FROM_HARDWARE：来自硬件设备方式核身
+        :type AuthScene: str
+        :param AuthSource: 核身渠道标识
+
+用于定位渠道具体来源，如果是扫码打卡渠道标识就是具体的小程序appid，若是硬件设备，则是设备的序列号等
+        :type AuthSource: str
+        :param ProjectName: 项目名称
+        :type ProjectName: str
+        :param EmployerName: 所属单位名称
+        :type EmployerName: str
+        :param AuthTime: 核身时间
+yyyy-MM-DDTHH:mm:ss+TIMEZONE
+
+示例值：2015-05-20T13:29:35+08:00
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AuthTime: str
+        :param AuthType: 核身类型
+
+SIGN_IN：考勤、签到打卡类型
+INSURANCE：投保类型
+CONTRACT：签约类型
+        :type AuthType: str
+        :param AuthState: 核身状态
+AUTHENTICATE_PROCESSING：核身中
+AUTHENTICATE_SUCCESS：核身成功
+AUTHENTICATE_FAILED：核身失败
+        :type AuthState: str
+        :param AuthFailReason: 核身失败原因描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AuthFailReason: str
+        """
+        self.AuthNo = None
+        self.OpenId = None
+        self.MchId = None
+        self.SubMchId = None
+        self.AuthScene = None
+        self.AuthSource = None
+        self.ProjectName = None
+        self.EmployerName = None
+        self.AuthTime = None
+        self.AuthType = None
+        self.AuthState = None
+        self.AuthFailReason = None
+
+
+    def _deserialize(self, params):
+        self.AuthNo = params.get("AuthNo")
+        self.OpenId = params.get("OpenId")
+        self.MchId = params.get("MchId")
+        self.SubMchId = params.get("SubMchId")
+        self.AuthScene = params.get("AuthScene")
+        self.AuthSource = params.get("AuthSource")
+        self.ProjectName = params.get("ProjectName")
+        self.EmployerName = params.get("EmployerName")
+        self.AuthTime = params.get("AuthTime")
+        self.AuthType = params.get("AuthType")
+        self.AuthState = params.get("AuthState")
+        self.AuthFailReason = params.get("AuthFailReason")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RechargeByThirdPayRequest(AbstractModel):
     """RechargeByThirdPay请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -32116,14 +32360,58 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class WechatPreAuthResult(AbstractModel):
+    """微工卡预核身结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AuthNo: 商户核身单号
+        :type AuthNo: str
+        :param OpenId: 微信用户标识
+        :type OpenId: str
+        :param MchId: 商户号
+        :type MchId: str
+        :param SubMchId: 子商户号
+        :type SubMchId: str
+        :param Token: 预核身token值
+        :type Token: str
+        :param Expire: token有效期时间，单位：秒
+        :type Expire: int
+        """
+        self.AuthNo = None
+        self.OpenId = None
+        self.MchId = None
+        self.SubMchId = None
+        self.Token = None
+        self.Expire = None
+
+
+    def _deserialize(self, params):
+        self.AuthNo = params.get("AuthNo")
+        self.OpenId = params.get("OpenId")
+        self.MchId = params.get("MchId")
+        self.SubMchId = params.get("SubMchId")
+        self.Token = params.get("Token")
+        self.Expire = params.get("Expire")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class WithdrawBill(AbstractModel):
     """聚鑫提现订单内容
 
     """
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.885/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.884/setup.py` & `tencentcloud-sdk-python-cpdp-3.0.885/setup.py`

 * *Files identical despite different names*

