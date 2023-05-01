# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.884.tar", last modified: Fri Apr 28 02:36:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.885.tar", last modified: Mon May  1 00:47:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.884.tar` & `tencentcloud-sdk-python-redis-3.0.885.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86664 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   291508 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:36:25.000000 tencentcloud-sdk-python-redis-3.0.884/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86757 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   292174 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:47:29.000000 tencentcloud-sdk-python-redis-3.0.885/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.884/README.rst` & `tencentcloud-sdk-python-redis-3.0.885/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -943,15 +943,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceShards(self, request):
-        """获取集群版实例分片信息
+        """本接口（DescribeInstanceShards）用于获取集群架构实例的分片信息。
 
         :param request: Request instance for DescribeInstanceShards.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceShardsRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceShardsResponse`
 
         """
         try:
@@ -989,15 +989,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstances(self, request):
-        """查询Redis实例列表
+        """本接口（DescribeInstances）用于查询Redis实例列表。
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstancesRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstancesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.884/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.885/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2920,17 +2920,19 @@
 class DescribeInstanceShardsRequest(AbstractModel):
     """DescribeInstanceShards请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param FilterSlave: 是否过滤掉从节信息
+        :param FilterSlave: 是否过滤掉从节信息。
+- true；过滤从节点。
+- false：不过滤。
         :type FilterSlave: bool
         """
         self.InstanceId = None
         self.FilterSlave = None
 
 
     def _deserialize(self, params):
@@ -2948,17 +2950,17 @@
 class DescribeInstanceShardsResponse(AbstractModel):
     """DescribeInstanceShards返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceShards: 实例分片列表信息
+        :param InstanceShards: 实例分片列表信息，包括：节点信息、节点ID、Key数量、使用容量、容量倾斜率等信息。
         :type InstanceShards: list of InstanceClusterShard
-        :param TotalCount: 实例分片节点总数
+        :param TotalCount: 实例分片节点数量。
         :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceShards = None
         self.TotalCount = None
         self.RequestId = None
@@ -3034,19 +3036,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param Limit: 每页输出实例的数量，参数默认值20，最大值为1000。
         :type Limit: int
-        :param Offset: 分页偏移量，取Limit整数倍。
+        :param Offset: 分页偏移量，取Limit整数倍。计算公式：offset=limit*(页码-1)。
         :type Offset: int
-        :param InstanceId: 实例 ID，如：crs-6ubhgouj。
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
+
+
         :type InstanceId: str
-        :param OrderBy: 实例排序依据，枚举值如下所示：<ul><li>projectId：项目ID。</li><li>createtime：实例创建时间。</li><li>instancename：实例名称。</li><li>type：实例类型。</li><li>curDeadline：实例到期时间。</li></ul>
+        :param OrderBy: 实例列表排序依据，枚举值如下所示：<ul><li>projectId：依据项目ID排序。</li><li>createtime：依据实例创建时间排序。</li><li>instancename：依据实例名称排序。</li><li>type：依据实例类型排序。</li><li>curDeadline：依据实例到期时间排序。</li></ul>
         :type OrderBy: str
         :param OrderType: 实例排序方式，默认为倒序排序。<ul><li>1：倒序。</li><li>0：顺序。</li></ul>
         :type OrderType: int
         :param VpcIds: 私有网络 ID 数组。如果不配置该参数或设置数组为空则默认选择基础网络。例如47525。该参数暂时保留，可忽略。请根据 UniqVpcIds 参数格式设置私有网络ID数组。
         :type VpcIds: list of str
         :param SubnetIds: 私有网络所属子网 ID 数组，例如：56854。该参数暂时保留，可忽略。请根据 UniqSubnetIds 参数格式设置私有网络子网 ID 数组。
         :type SubnetIds: list of str
@@ -3064,15 +3068,15 @@
         :type RegionIds: list of int
         :param Status: 实例状态。<ul><li>0：待初始化。</li><li>1：流程中。</li><li>2：运行中。</li><li>-2：已隔离。</li><li>-3：待删除。</li></ul>
         :type Status: list of int
         :param TypeVersion: 实例架构版本。<ul><li>1：单机版。</li><li>2：主从版。</li><li>3：集群版。</li></ul>
         :type TypeVersion: int
         :param EngineName: 存储引擎信息。可设置为Redis-2.8、Redis-4.0、Redis-5.0、Redis-6.0 或者 CKV。
         :type EngineName: str
-        :param AutoRenew: 续费模式。<ul><li>0：默认状态（手动续费）。</li><li>1：自动续费。</li><li>2：明确不自动续费。</ul>
+        :param AutoRenew: 续费模式。<ul><li>0：手动续费。</li><li>1：自动续费。</li><li>2：到期不再续费。</ul>
         :type AutoRenew: list of int
         :param BillingMode: 计费模式。<ul><li>postpaid：按量计费。</li><li>prepaid：包年包月。</li></ul>
         :type BillingMode: str
         :param Type: 实例类型。<ul><li>1：Redis 老集群版。</li><li>2：Redis 2.8 主从版。</li><li>3：CKV 主从版。</li><li>4：CKV 集群版。</li><li>5：Redis 2.8 单机版。</li><li>6：Redis 4.0主从版。</li><li>7：Redis 4.0 集群版。</li><li>8：Redis 5.0 主从版。</li><li>9：Redis 5.0 集群版。</li></ul>
         :type Type: int
         :param SearchKeys: 设置搜索关键字数组，可根据实例ID、实例名称、完整IP地址查询实例。
         :type SearchKeys: list of str
@@ -3080,15 +3084,15 @@
         :type TypeList: list of int
         :param MonitorVersion: 内部参数，用户可忽略。
         :type MonitorVersion: str
         :param InstanceTags: 根据标签的 Key 和 Value 筛选资源。该参数不配置或者数组设置为空值，则不根据标签进行过滤。
         :type InstanceTags: list of InstanceTagInfo
         :param TagKeys: 根据标签的 Key 筛选资源，该参数不配置或者数组设置为空值，则不根据标签Key进行过滤。
         :type TagKeys: list of str
-        :param ProductVersions: 实例的产品版本。如果该参数不配置或者数组设置为空值，则默认不依据此参数过滤实例。<ul><li>local：本地盘版。</li><li>cloud：云盘版。</li><li>cdc：独享集群版。</li></ul>
+        :param ProductVersions: 实例的产品版本。如果该参数不配置或者数组设置为空值，则默认不依据此参数过滤实例。<ul><li>local：本地盘版。</li><li>cdc：独享集群版。</li></ul>
         :type ProductVersions: list of str
         :param InstanceIds: 批量查询指定的实例 ID，返回结果已 Limit 限制为主。
         :type InstanceIds: list of str
         :param AzMode: 可用区模式。<ul><li>singleaz：单可用区。</li><li>multiaz：多可用区。</li></ul>
         :type AzMode: str
         """
         self.Limit = None
@@ -3749,25 +3753,26 @@
 class DescribeSlowLogRequest(AbstractModel):
     """DescribeSlowLog请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例Id。
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
+
         :type InstanceId: str
-        :param BeginTime: 开始时间。
+        :param BeginTime: 预查询慢日志的起始时间。
         :type BeginTime: str
-        :param EndTime: 结束时间。
+        :param EndTime: 预查询慢日志的结束时间。
         :type EndTime: str
-        :param MinQueryTime: 慢查询平均执行时间阈值（单位：毫秒）。
+        :param MinQueryTime: 慢查询平均执行时间阈值，单位：毫秒。
         :type MinQueryTime: int
         :param Limit: 每个页面展示的慢查询条数，默认值为20。
         :type Limit: int
-        :param Offset: 慢查询条数的偏移量，取Limit整数倍。
+        :param Offset: 慢查询条数的偏移量，取Limit整数倍。计算公式：offset=limit*(页码-1)。
         :type Offset: int
         :param Role: 节点所属角色。<ul><li>master：主节点。</li><li>slave：从节点。</li></ul>
         :type Role: str
         """
         self.InstanceId = None
         self.BeginTime = None
         self.EndTime = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.885/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.885/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.884/setup.py` & `tencentcloud-sdk-python-redis-3.0.885/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.884/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.885/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

