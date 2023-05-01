# Comparing `tmp/tencentcloud-sdk-python-thpc-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-thpc-3.0.885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.884.tar", last modified: Fri Apr 28 02:41:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.885.tar", last modified: Mon May  1 00:56:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-thpc-3.0.884.tar` & `tencentcloud-sdk-python-thpc-3.0.885.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)     4733 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97393 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)    16733 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/thpc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43727 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/models.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)     4248 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97585 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)    15793 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud_sdk_python_thpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      781 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:41:21.000000 tencentcloud-sdk-python-thpc-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97393 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)    16733 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/thpc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/models.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101533 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)    16736 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud_sdk_python_thpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      781 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:56:01.000000 tencentcloud-sdk-python-thpc-3.0.885/setup.cfg
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/README.rst` & `tencentcloud-sdk-python-thpc-3.0.885/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -621,14 +621,16 @@
         :type LoginNode: :class:`tencentcloud.thpc.v20230321.models.LoginNode`
         :param LoginNodeCount: 指定登录节点的数量。默认取值：0。取值范围：0～10。
         :type LoginNodeCount: int
         :param Tags: 创建集群时同时绑定的标签对说明。
         :type Tags: list of Tag
         :param AutoScalingType: 弹性伸缩类型。默认值：THPC_AS<br><li>THPC_AS：集群自动扩缩容由THPC产品内部实现。<br><li>AS：集群自动扩缩容由[弹性伸缩](https://cloud.tencent.com/document/product/377/3154)产品实现。
         :type AutoScalingType: str
+        :param InitNodeScripts: 节点初始化脚本信息列表。
+        :type InitNodeScripts: list of NodeScript
         """
         self.Placement = None
         self.ManagerNode = None
         self.ManagerNodeCount = None
         self.ComputeNode = None
         self.ComputeNodeCount = None
         self.SchedulerType = None
@@ -641,14 +643,15 @@
         self.AccountType = None
         self.ClusterName = None
         self.StorageOption = None
         self.LoginNode = None
         self.LoginNodeCount = None
         self.Tags = None
         self.AutoScalingType = None
+        self.InitNodeScripts = None
 
 
     def _deserialize(self, params):
         if params.get("Placement") is not None:
             self.Placement = Placement()
             self.Placement._deserialize(params.get("Placement"))
         if params.get("ManagerNode") is not None:
@@ -682,14 +685,20 @@
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.AutoScalingType = params.get("AutoScalingType")
+        if params.get("InitNodeScripts") is not None:
+            self.InitNodeScripts = []
+            for item in params.get("InitNodeScripts"):
+                obj = NodeScript()
+                obj._deserialize(item)
+                self.InitNodeScripts.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1833,14 +1842,64 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ModifyInitNodeScriptsRequest(AbstractModel):
+    """ModifyInitNodeScripts请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID。
+        :type ClusterId: str
+        :param InitNodeScripts: 节点初始化脚本信息列表。
+        :type InitNodeScripts: list of NodeScript
+        """
+        self.ClusterId = None
+        self.InitNodeScripts = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        if params.get("InitNodeScripts") is not None:
+            self.InitNodeScripts = []
+            for item in params.get("InitNodeScripts"):
+                obj = NodeScript()
+                obj._deserialize(item)
+                self.InitNodeScripts.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyInitNodeScriptsResponse(AbstractModel):
+    """ModifyInitNodeScripts返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class NodeActivity(AbstractModel):
     """节点活动信息。
 
     """
 
     def __init__(self):
         r"""
@@ -1927,14 +1986,45 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class NodeScript(AbstractModel):
+    """描述节点执行脚本信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ScriptPath: 节点执行脚本获取地址。
+目前仅支持cos地址。地址最大长度：255。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScriptPath: str
+        :param Timeout: 脚本执行超时时间（包含拉取脚本的时间）。单位秒，默认值：30。取值范围：10～1200。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Timeout: int
+        """
+        self.ScriptPath = None
+        self.Timeout = None
+
+
+    def _deserialize(self, params):
+        self.ScriptPath = params.get("ScriptPath")
+        self.Timeout = params.get("Timeout")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Placement(AbstractModel):
     """描述了实例的抽象位置
 
     """
 
     def __init__(self):
         r"""
@@ -1979,25 +2069,28 @@
         :type SystemDisk: :class:`tencentcloud.thpc.v20230321.models.SystemDisk`
         :param DataDisks: 节点数据盘配置信息。若不指定该参数，则默认不购买数据盘。支持购买的时候指定21块数据盘，其中最多包含1块LOCAL_BASIC数据盘或者LOCAL_SSD数据盘，最多包含20块CLOUD_BASIC数据盘、CLOUD_PREMIUM数据盘或者CLOUD_SSD数据盘。
         :type DataDisks: list of DataDisk
         :param InternetAccessible: 公网带宽相关信息设置。若不指定该参数，则默认公网带宽为0Mbps。
         :type InternetAccessible: :class:`tencentcloud.thpc.v20230321.models.InternetAccessible`
         :param ExpansionNodeConfigs: 扩容节点配置信息。
         :type ExpansionNodeConfigs: list of ExpansionNodeConfig
+        :param DesiredIdleNodeCapacity: 队列中期望的空闲节点数量（包含弹性节点和静态节点）。默认值：0。队列中，处于空闲状态的节点小于此值，集群会扩容弹性节点；处于空闲状态的节点大于此值，集群会缩容弹性节点。
+        :type DesiredIdleNodeCapacity: int
         """
         self.QueueName = None
         self.MinSize = None
         self.MaxSize = None
         self.EnableAutoExpansion = None
         self.EnableAutoShrink = None
         self.ImageId = None
         self.SystemDisk = None
         self.DataDisks = None
         self.InternetAccessible = None
         self.ExpansionNodeConfigs = None
+        self.DesiredIdleNodeCapacity = None
 
 
     def _deserialize(self, params):
         self.QueueName = params.get("QueueName")
         self.MinSize = params.get("MinSize")
         self.MaxSize = params.get("MaxSize")
         self.EnableAutoExpansion = params.get("EnableAutoExpansion")
@@ -2017,14 +2110,15 @@
             self.InternetAccessible._deserialize(params.get("InternetAccessible"))
         if params.get("ExpansionNodeConfigs") is not None:
             self.ExpansionNodeConfigs = []
             for item in params.get("ExpansionNodeConfigs"):
                 obj = ExpansionNodeConfig()
                 obj._deserialize(item)
                 self.ExpansionNodeConfigs.append(obj)
+        self.DesiredIdleNodeCapacity = params.get("DesiredIdleNodeCapacity")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2045,35 +2139,40 @@
         :type MaxSize: int
         :param EnableAutoExpansion: 是否开启自动扩容。
         :type EnableAutoExpansion: bool
         :param EnableAutoShrink: 是否开启自动缩容。
         :type EnableAutoShrink: bool
         :param ExpansionNodeConfigs: 扩容节点配置信息。
         :type ExpansionNodeConfigs: list of ExpansionNodeConfigOverview
+        :param DesiredIdleNodeCapacity: 队列中期望的空闲节点数量（包含弹性节点和静态节点）。默认值：0。队列中，处于空闲状态的节点小于此值，集群会扩容弹性节点；处于空闲状态的节点大于此值，集群会缩容弹性节点。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DesiredIdleNodeCapacity: int
         """
         self.QueueName = None
         self.MinSize = None
         self.MaxSize = None
         self.EnableAutoExpansion = None
         self.EnableAutoShrink = None
         self.ExpansionNodeConfigs = None
+        self.DesiredIdleNodeCapacity = None
 
 
     def _deserialize(self, params):
         self.QueueName = params.get("QueueName")
         self.MinSize = params.get("MinSize")
         self.MaxSize = params.get("MaxSize")
         self.EnableAutoExpansion = params.get("EnableAutoExpansion")
         self.EnableAutoShrink = params.get("EnableAutoShrink")
         if params.get("ExpansionNodeConfigs") is not None:
             self.ExpansionNodeConfigs = []
             for item in params.get("ExpansionNodeConfigs"):
                 obj = ExpansionNodeConfigOverview()
                 obj._deserialize(item)
                 self.ExpansionNodeConfigs.append(obj)
+        self.DesiredIdleNodeCapacity = params.get("DesiredIdleNodeCapacity")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyInitNodeScripts(self, request):
+        """本接口 (ModifyInitNodeScripts) 用于修改节点初始化脚本。
+
+        :param request: Request instance for ModifyInitNodeScripts.
+        :type request: :class:`tencentcloud.thpc.v20230321.models.ModifyInitNodeScriptsRequest`
+        :rtype: :class:`tencentcloud.thpc.v20230321.models.ModifyInitNodeScriptsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyInitNodeScripts", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyInitNodeScriptsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def SetAutoScalingConfiguration(self, request):
         """本接口(SetAutoScalingConfiguration)用于为集群设置集群弹性伸缩配置信息。
 
         :param request: Request instance for SetAutoScalingConfiguration.
         :type request: :class:`tencentcloud.thpc.v20230321.models.SetAutoScalingConfigurationRequest`
         :rtype: :class:`tencentcloud.thpc.v20230321.models.SetAutoScalingConfigurationResponse`
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.885/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.885/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.884/setup.py` & `tencentcloud-sdk-python-thpc-3.0.885/setup.py`

 * *Files identical despite different names*

