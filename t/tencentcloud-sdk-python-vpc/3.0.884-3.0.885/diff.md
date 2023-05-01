# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.884.tar", last modified: Fri Apr 28 02:47:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.885.tar", last modified: Mon May  1 00:59:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.884.tar` & `tencentcloud-sdk-python-vpc-3.0.885.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   328818 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    40497 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   838070 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:47:29.000000 tencentcloud-sdk-python-vpc-3.0.884/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:47:30.000000 tencentcloud-sdk-python-vpc-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   328818 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    40497 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   839190 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/README.rst` & `tencentcloud-sdk-python-vpc-3.0.885/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,29 +1071,33 @@
         r"""
         :param NetworkInterfaceId: 弹性网卡实例ID，例如：eni-m6dyj72l。
         :type NetworkInterfaceId: str
         :param PrivateIpAddresses: 指定的内网IP信息，单次最多指定10个。与SecondaryPrivateIpAddressCount至少提供一个。
         :type PrivateIpAddresses: list of PrivateIpAddressSpecification
         :param SecondaryPrivateIpAddressCount: 新申请的内网IP地址个数，与PrivateIpAddresses至少提供一个。内网IP地址个数总和不能超过配额数，详见<a href="/document/product/576/18527">弹性网卡使用限制</a>。
         :type SecondaryPrivateIpAddressCount: int
+        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :type QosLevel: str
         """
         self.NetworkInterfaceId = None
         self.PrivateIpAddresses = None
         self.SecondaryPrivateIpAddressCount = None
+        self.QosLevel = None
 
 
     def _deserialize(self, params):
         self.NetworkInterfaceId = params.get("NetworkInterfaceId")
         if params.get("PrivateIpAddresses") is not None:
             self.PrivateIpAddresses = []
             for item in params.get("PrivateIpAddresses"):
                 obj = PrivateIpAddressSpecification()
                 obj._deserialize(item)
                 self.PrivateIpAddresses.append(obj)
         self.SecondaryPrivateIpAddressCount = params.get("SecondaryPrivateIpAddressCount")
+        self.QosLevel = params.get("QosLevel")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2938,14 +2942,16 @@
         :type SubnetId: str
         :param InstanceId: 云服务器实例ID。
         :type InstanceId: str
         :param PrivateIpAddresses: 指定的内网IP信息，单次最多指定10个。
         :type PrivateIpAddresses: list of PrivateIpAddressSpecification
         :param SecondaryPrivateIpAddressCount: 新申请的内网IP地址个数，内网IP地址个数总和不能超过配额数。
         :type SecondaryPrivateIpAddressCount: int
+        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :type QosLevel: str
         :param SecurityGroupIds: 指定绑定的安全组，例如：['sg-1dd51d']。
         :type SecurityGroupIds: list of str
         :param NetworkInterfaceDescription: 弹性网卡描述，可任意命名，但不得超过60个字符。
         :type NetworkInterfaceDescription: str
         :param Tags: 指定绑定的标签列表，例如：[{"Key": "city", "Value": "shanghai"}]。
         :type Tags: list of Tag
         :param AttachType: 绑定类型：0 标准型 1 扩展型。
@@ -2953,14 +2959,15 @@
         """
         self.VpcId = None
         self.NetworkInterfaceName = None
         self.SubnetId = None
         self.InstanceId = None
         self.PrivateIpAddresses = None
         self.SecondaryPrivateIpAddressCount = None
+        self.QosLevel = None
         self.SecurityGroupIds = None
         self.NetworkInterfaceDescription = None
         self.Tags = None
         self.AttachType = None
 
 
     def _deserialize(self, params):
@@ -2971,14 +2978,15 @@
         if params.get("PrivateIpAddresses") is not None:
             self.PrivateIpAddresses = []
             for item in params.get("PrivateIpAddresses"):
                 obj = PrivateIpAddressSpecification()
                 obj._deserialize(item)
                 self.PrivateIpAddresses.append(obj)
         self.SecondaryPrivateIpAddressCount = params.get("SecondaryPrivateIpAddressCount")
+        self.QosLevel = params.get("QosLevel")
         self.SecurityGroupIds = params.get("SecurityGroupIds")
         self.NetworkInterfaceDescription = params.get("NetworkInterfaceDescription")
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
@@ -4256,40 +4264,44 @@
         :type NetworkInterfaceName: str
         :param SubnetId: 弹性网卡所在的子网实例ID，例如：subnet-0ap8nwca。
         :type SubnetId: str
         :param NetworkInterfaceDescription: 弹性网卡描述，可任意命名，但不得超过60个字符。
         :type NetworkInterfaceDescription: str
         :param SecondaryPrivateIpAddressCount: 新申请的内网IP地址个数，内网IP地址个数总和不能超过配额数。
         :type SecondaryPrivateIpAddressCount: int
+        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :type QosLevel: str
         :param SecurityGroupIds: 指定绑定的安全组，例如：['sg-1dd51d']。
         :type SecurityGroupIds: list of str
         :param PrivateIpAddresses: 指定的内网IP信息，单次最多指定10个。
         :type PrivateIpAddresses: list of PrivateIpAddressSpecification
         :param Tags: 指定绑定的标签列表，例如：[{"Key": "city", "Value": "shanghai"}]
         :type Tags: list of Tag
         :param TrunkingFlag: 网卡trunking模式设置，Enable-开启，Disable--关闭，默认关闭。
         :type TrunkingFlag: str
         """
         self.VpcId = None
         self.NetworkInterfaceName = None
         self.SubnetId = None
         self.NetworkInterfaceDescription = None
         self.SecondaryPrivateIpAddressCount = None
+        self.QosLevel = None
         self.SecurityGroupIds = None
         self.PrivateIpAddresses = None
         self.Tags = None
         self.TrunkingFlag = None
 
 
     def _deserialize(self, params):
         self.VpcId = params.get("VpcId")
         self.NetworkInterfaceName = params.get("NetworkInterfaceName")
         self.SubnetId = params.get("SubnetId")
         self.NetworkInterfaceDescription = params.get("NetworkInterfaceDescription")
         self.SecondaryPrivateIpAddressCount = params.get("SecondaryPrivateIpAddressCount")
+        self.QosLevel = params.get("QosLevel")
         self.SecurityGroupIds = params.get("SecurityGroupIds")
         if params.get("PrivateIpAddresses") is not None:
             self.PrivateIpAddresses = []
             for item in params.get("PrivateIpAddresses"):
                 obj = PrivateIpAddressSpecification()
                 obj._deserialize(item)
                 self.PrivateIpAddresses.append(obj)
@@ -19712,32 +19724,36 @@
         :type IsWanIpBlocked: bool
         :param State: IP状态：
 PENDING：生产中
 MIGRATING：迁移中
 DELETING：删除中
 AVAILABLE：可用的
         :type State: str
+        :param QosLevel: IP服务质量等级，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :type QosLevel: str
         """
         self.PrivateIpAddress = None
         self.Primary = None
         self.PublicIpAddress = None
         self.AddressId = None
         self.Description = None
         self.IsWanIpBlocked = None
         self.State = None
+        self.QosLevel = None
 
 
     def _deserialize(self, params):
         self.PrivateIpAddress = params.get("PrivateIpAddress")
         self.Primary = params.get("Primary")
         self.PublicIpAddress = params.get("PublicIpAddress")
         self.AddressId = params.get("AddressId")
         self.Description = params.get("Description")
         self.IsWanIpBlocked = params.get("IsWanIpBlocked")
         self.State = params.get("State")
+        self.QosLevel = params.get("QosLevel")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.885/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.884/setup.py` & `tencentcloud-sdk-python-vpc-3.0.885/setup.py`

 * *Files identical despite different names*

