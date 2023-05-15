# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.889.tar", last modified: Thu May 11 03:28:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.891.tar", last modified: Mon May 15 04:55:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.889.tar` & `tencentcloud-sdk-python-vpc-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   328827 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41072 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   839372 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 04:55:53.000000 tencentcloud-sdk-python-vpc-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   329012 2023-05-15 04:55:53.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41072 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   840728 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:55:53.000000 tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 04:55:53.000000 tencentcloud-sdk-python-vpc-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:55:54.000000 tencentcloud-sdk-python-vpc-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.891/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/README.rst` & `tencentcloud-sdk-python-vpc-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2515,15 +2515,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteVpnConnection(self, request):
-        """本接口(DeleteVpnConnection)用于删除VPN通道。
+        """本接口（DeleteVpnConnection）用于删除VPN通道。
 
         :param request: Request instance for DeleteVpnConnection.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnConnectionRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnConnectionResponse`
 
         """
         try:
@@ -4376,15 +4376,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeVpnConnections(self, request):
-        """本接口（DescribeVpnConnections）查询VPN通道列表。
+        """本接口（DescribeVpnConnections）用于查询VPN通道列表。
 
         :param request: Request instance for DescribeVpnConnections.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnConnectionsRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnConnectionsResponse`
 
         """
         try:
@@ -6913,15 +6913,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ResetVpnConnection(self, request):
-        """本接口(ResetVpnConnection)用于重置VPN通道。
+        """本接口（ResetVpnConnection）用于重置VPN通道。
 
         :param request: Request instance for ResetVpnConnection.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ResetVpnConnectionRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.ResetVpnConnectionResponse`
 
         """
         try:
@@ -6936,15 +6936,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ResetVpnGatewayInternetMaxBandwidth(self, request):
-        """本接口（ResetVpnGatewayInternetMaxBandwidth）调整VPN网关带宽上限。目前支持升级配置，如果是包年包月VPN网关需要在有效期内。
+        """本接口（ResetVpnGatewayInternetMaxBandwidth）用于调整VPN网关带宽上限。VPN网关带宽目前仅支持部分带宽范围内升降配，如【5,100】Mbps和【200,1000】Mbps，在各自带宽范围内可提升配额，跨范围提升配额和降配暂不支持，如果是包年包月VPN网关需要在有效期内。
 
         :param request: Request instance for ResetVpnGatewayInternetMaxBandwidth.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ResetVpnGatewayInternetMaxBandwidthRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.ResetVpnGatewayInternetMaxBandwidthResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -20721,15 +20721,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param VpnGatewayId: VPN网关实例ID。
         :type VpnGatewayId: str
-        :param InternetMaxBandwidthOut: 公网带宽设置。可选带宽规格：5, 10, 20, 50, 100；单位：Mbps。
+        :param InternetMaxBandwidthOut: 新规格公网带宽设置。可选带宽规格：5, 10, 20, 50, 100, 200, 500, 1000；单位：Mbps。VPN网关带宽目前仅支持部分带宽范围内升降配，如【5,100】Mbps和【200,1000】Mbps，在各自带宽范围内可提升配额，跨范围提升配额和降配暂不支持。
         :type InternetMaxBandwidthOut: int
         """
         self.VpnGatewayId = None
         self.InternetMaxBandwidthOut = None
 
 
     def _deserialize(self, params):
@@ -21425,28 +21425,40 @@
         :type SecurityGroupPolicyLimit: int
         :param ReferedSecurityGroupLimit: 安全组下嵌套安全组规则数
         :type ReferedSecurityGroupLimit: int
         :param SecurityGroupInstanceLimit: 单安全组关联实例数
         :type SecurityGroupInstanceLimit: int
         :param InstanceSecurityGroupLimit: 实例关联安全组数
         :type InstanceSecurityGroupLimit: int
+        :param SecurityGroupExtendedPolicyLimit: 安全组展开后的规则数限制
+        :type SecurityGroupExtendedPolicyLimit: int
+        :param SecurityGroupReferedCvmAndEniLimit: 被引用的安全组关联CVM、ENI的实例配额
+        :type SecurityGroupReferedCvmAndEniLimit: int
+        :param SecurityGroupReferedSvcLimit: 被引用的安全组关联数据库、LB等服务实例配额
+        :type SecurityGroupReferedSvcLimit: int
         """
         self.SecurityGroupLimit = None
         self.SecurityGroupPolicyLimit = None
         self.ReferedSecurityGroupLimit = None
         self.SecurityGroupInstanceLimit = None
         self.InstanceSecurityGroupLimit = None
+        self.SecurityGroupExtendedPolicyLimit = None
+        self.SecurityGroupReferedCvmAndEniLimit = None
+        self.SecurityGroupReferedSvcLimit = None
 
 
     def _deserialize(self, params):
         self.SecurityGroupLimit = params.get("SecurityGroupLimit")
         self.SecurityGroupPolicyLimit = params.get("SecurityGroupPolicyLimit")
         self.ReferedSecurityGroupLimit = params.get("ReferedSecurityGroupLimit")
         self.SecurityGroupInstanceLimit = params.get("SecurityGroupInstanceLimit")
         self.InstanceSecurityGroupLimit = params.get("InstanceSecurityGroupLimit")
+        self.SecurityGroupExtendedPolicyLimit = params.get("SecurityGroupExtendedPolicyLimit")
+        self.SecurityGroupReferedCvmAndEniLimit = params.get("SecurityGroupReferedCvmAndEniLimit")
+        self.SecurityGroupReferedSvcLimit = params.get("SecurityGroupReferedSvcLimit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -21464,15 +21476,15 @@
         :param Protocol: 协议, 取值: TCP,UDP,ICMP,ICMPv6,ALL。
         :type Protocol: str
         :param Port: 端口(all, 离散port,  range)。
 说明：如果Protocol设置为ALL，则Port也需要设置为all。
         :type Port: str
         :param ServiceTemplate: 协议端口ID或者协议端口组ID。ServiceTemplate和Protocol+Port互斥。
         :type ServiceTemplate: :class:`tencentcloud.vpc.v20170312.models.ServiceTemplateSpecification`
-        :param CidrBlock: 网段或IP(互斥)。
+        :param CidrBlock: 网段或IP(互斥)，特殊说明：0.0.0.0/n 都会映射为0.0.0.0/0。
         :type CidrBlock: str
         :param Ipv6CidrBlock: 网段或IPv6(互斥)。
         :type Ipv6CidrBlock: str
         :param SecurityGroupId: 安全组实例ID，例如：sg-ohuuioma。
         :type SecurityGroupId: str
         :param AddressTemplate: IP地址ID或者IP地址组ID。
         :type AddressTemplate: :class:`tencentcloud.vpc.v20170312.models.AddressTemplateSpecification`
@@ -21525,18 +21537,21 @@
     """安全组规则集合
 
     """
 
     def __init__(self):
         r"""
         :param Version: 安全组规则当前版本。用户每次更新安全规则版本会自动加1，防止更新的路由规则已过期，不填不考虑冲突。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Version: str
         :param Egress: 出站规则。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Egress: list of SecurityGroupPolicy
         :param Ingress: 入站规则。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Ingress: list of SecurityGroupPolicy
         """
         self.Version = None
         self.Egress = None
         self.Ingress = None
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.891/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.889'
+__version__ = '3.0.891'
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.891/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.889/setup.py` & `tencentcloud-sdk-python-vpc-3.0.891/setup.py`

 * *Files identical despite different names*

