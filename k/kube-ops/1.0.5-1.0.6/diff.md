# Comparing `tmp/kube_ops-1.0.5-py3-none-any.whl.zip` & `tmp/kube_ops-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19882 bytes, number of entries: 12
+Zip file size: 19960 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     1664 b- defN 23-Jul-27 04:35 kube/__init__.py
--rw-r--r--  2.0 unx    38740 b- defN 23-Jul-27 09:03 kube/api.py
+-rw-r--r--  2.0 unx    38722 b- defN 23-Jul-30 06:28 kube/api.py
 -rw-r--r--  2.0 unx     2611 b- defN 23-Jul-23 07:44 kube/common.py
--rw-r--r--  2.0 unx     5085 b- defN 23-Jul-27 07:18 kube/config.py
+-rw-r--r--  2.0 unx     5086 b- defN 23-Jul-28 06:22 kube/config.py
 -rw-r--r--  2.0 unx     1400 b- defN 23-Jul-27 02:32 kube/enums.py
--rw-r--r--  2.0 unx    19771 b- defN 23-Jul-27 05:07 kube/manifests.py
+-rw-r--r--  2.0 unx    19385 b- defN 23-Jul-28 06:40 kube/manifests.py
 -rw-r--r--  2.0 unx    11913 b- defN 23-Jul-27 04:49 kube/templates.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-27 12:02 kube_ops-1.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3425 b- defN 23-Jul-27 12:02 kube_ops-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 12:02 kube_ops-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-27 12:02 kube_ops-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 23-Jul-27 12:02 kube_ops-1.0.5.dist-info/RECORD
-12 files, 86669 bytes uncompressed, 18416 bytes compressed:  78.8%
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3374 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/RECORD
+12 files, 86215 bytes uncompressed, 18494 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kube/manifests.py
 Comment: 
 
 Filename: kube/templates.py
 Comment: 
 
-Filename: kube_ops-1.0.5.dist-info/LICENSE
+Filename: kube_ops-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: kube_ops-1.0.5.dist-info/METADATA
+Filename: kube_ops-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: kube_ops-1.0.5.dist-info/WHEEL
+Filename: kube_ops-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: kube_ops-1.0.5.dist-info/top_level.txt
+Filename: kube_ops-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: kube_ops-1.0.5.dist-info/RECORD
+Filename: kube_ops-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kube/api.py

```diff
@@ -944,15 +944,15 @@
                             check_err: bool = True, **kwargs) -> client.V1RoleBinding:
         """
         Create RoleBinding.
         """
 
         return self._create(
             self.rbac_authorization_v1_api.create_namespaced_role_binding,
-            rb, check_err=check_err, namespaced=False, **kwargs)
+            rb, check_err=check_err, **kwargs)
 
     def role_binding_delete(self, name: str, **kwargs) -> client.V1RoleBinding | None:
         """
         Delete RoleBinding by name.
         """
 
         return self._delete(
```

## kube/config.py

```diff
@@ -61,15 +61,15 @@
         """
 
         if not server.startswith('https'):
             raise ValueError('Invalid server URL. URL must be start with https://...')
 
         parsed_url = urlparse(server)
         if not parsed_url.port:
-            server = f'http://{parsed_url.netloc}:443'
+            server = f'https://{parsed_url.netloc}:443'
             parsed_url = urlparse(server)
 
         namespace = kwargs.get('namespace', 'default')
 
         ca_cert = None
         try:
             cm = KubeApi.from_token(server, token, namespace).configmap_get('kube-root-ca.crt', check_err=False)
```

## kube/manifests.py

```diff
@@ -534,103 +534,92 @@
         self._sa.secrets.append(ref)
 
     def add_secret_name(self, name: str):
         self._sa.secrets.append(
             client.V1ObjectReference(name=name))
 
 
-class Role(ObjectMetadata):
-    def __init__(self, name: str):
+class _Role(ObjectMetadata):
+    def __init__(self, name: str, kind: str):
         super().__init__(name)
 
-        self._role = client.V1Role(
+        obj = client.V1Role
+        if kind == 'ClusterRole':
+            obj = client.V1ClusterRole
+
+        self._role = obj(
             api_version='rbac.authorization.k8s.io/v1',
-            kind='Role',
+            kind=kind,
             rules=[]
         )
 
     @property
     def manifest(self) -> client.V1Role:
         role = deepcopy(self._role)
         role.metadata = self._metadata
         return role
 
     def add_rule(self, rule: client.V1PolicyRule):
         self._role.rules.append(rule)
 
 
-class RoleBinding(ObjectMetadata):
-    def __init__(self, name: str):
+class _RoleBinding(ObjectMetadata):
+    def __init__(self, name: str, kind: str):
         super().__init__(name)
 
-        self._rb = client.V1RoleBinding(
+        default_role_ref_kind = 'Role'
+        obj = client.V1RoleBinding
+        if kind == 'ClusterRoleBinding':
+            default_role_ref_kind = 'ClusterRole'
+            obj = client.V1ClusterRoleBinding
+
+        self._role_binding = obj(
             api_version='rbac.authorization.k8s.io/v1',
-            kind='RoleBinding',
+            kind=kind,
+            role_ref=client.V1RoleRef('rbac.authorization.k8s.io', default_role_ref_kind, ''),
             subjects=[]
         )
 
     @property
-    def manifest(self) -> client.V1RoleBinding:
-        rb = deepcopy(self._rb)
+    def manifest(self):
+        rb = deepcopy(self._role_binding)
         rb.metadata = self._metadata
         return rb
 
-    def add_role_ref(self, api_group: str, kind: str, name: str):
-        self._rb.role_ref = client.V1RoleRef(
-            api_group=api_group, kind=kind, name=name)
+    def set_role_ref(self, name: str, api_group: str = None, kind: str = None):
+        self._role_binding.role_ref.name = name
+        if api_group:
+            self._role_binding.role_ref.api_group = api_group
+        if kind:
+            self._role_binding.role_ref.kind = kind
 
     def add_subject(self, kind: str, name: str, namespace: str, api_group: str = None):
-        self._rb.subjects.append(client.V1Subject(
+        self._role_binding.subjects.append(client.V1Subject(
             api_group=api_group, kind=kind, name=name, namespace=namespace))
 
 
-class ClusterRole(ObjectMetadata):
+class Role(_Role):
     def __init__(self, name: str):
-        super().__init__(name)
+        super().__init__(name, 'Role')
 
-        self._role = client.V1ClusterRole(
-            api_version='rbac.authorization.k8s.io/v1',
-            kind='ClusterRole',
-            rules=[]
-        )
 
-    @property
-    def manifest(self) -> client.V1ClusterRole:
-        role = deepcopy(self._role)
-        role.metadata = self._metadata
-        return role
+class RoleBinding(_RoleBinding):
+    def __init__(self, name: str):
+        super().__init__(name, 'RoleBinding')
 
-    def add_rule(self, rule: client.V1PolicyRule):
-        self._role.rules.append(rule)
+
+class ClusterRole(_Role):
+    def __init__(self, name: str):
+        super().__init__(name, 'ClusterRole')
 
     def add_aggregation_rule(self, rule: client.V1LabelSelector):
         if not self._role.aggregation_rule:
             self._role.aggregation_rule = client.V1AggregationRule(
                 cluster_role_selectors=[]
             )
 
         self._role.aggregation_rule.cluster_role_selectors.append(rule)
 
 
-class ClusterRoleBinding(ObjectMetadata):
+class ClusterRoleBinding(_RoleBinding):
     def __init__(self, name: str):
-        super().__init__(name)
-
-        self._crb = client.V1ClusterRoleBinding(
-            api_version='rbac.authorization.k8s.io/v1',
-            kind='ClusterRoleBinding',
-            subjects=[]
-        )
-
-    @property
-    def manifest(self) -> client.V1ClusterRoleBinding:
-        crb = deepcopy(self._crb)
-        crb.metadata = self._metadata
-        return crb
-
-    def add_role_ref(self, api_group: str, kind: str, name: str):
-        self._crb.role_ref = client.V1RoleRef(
-            api_group=api_group, kind=kind, name=name)
-
-    def add_subject(self, kind: str, name: str, namespace: str, api_group: str = None):
-        self._crb.subjects.append(client.V1Subject(
-            api_group=api_group, kind=kind, name=name, namespace=namespace))
+        super().__init__(name, 'ClusterRoleBinding')
```

## Comparing `kube_ops-1.0.5.dist-info/LICENSE` & `kube_ops-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kube_ops-1.0.5.dist-info/METADATA` & `kube_ops-1.0.6.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-ops
-Version: 1.0.5
+Version: 1.0.6
 Summary: Kubernetes OOP
 Author-email: myback <54638513+myback@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 myback.space
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,14 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/myback/kube-ops
 Project-URL: Bug Tracker, https://github.com/myback/kube-ops/issues
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml (~=6.0.1)
 Requires-Dist: kubernetes (~=27.2.0)
```

