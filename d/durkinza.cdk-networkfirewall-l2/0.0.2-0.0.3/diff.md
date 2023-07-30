# Comparing `tmp/durkinza.cdk-networkfirewall-l2-0.0.2.tar.gz` & `tmp/durkinza.cdk-networkfirewall-l2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durkinza.cdk-networkfirewall-l2-0.0.2.tar", last modified: Wed Jul 26 04:02:26 2023, max compression
+gzip compressed data, was "durkinza.cdk-networkfirewall-l2-0.0.3.tar", last modified: Sun Jul 30 18:32:30 2023, max compression
```

## Comparing `durkinza.cdk-networkfirewall-l2-0.0.2.tar` & `durkinza.cdk-networkfirewall-l2-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:02:26.941846 durkinza.cdk-networkfirewall-l2-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-26 04:02:26.941846 durkinza.cdk-networkfirewall-l2-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 04:02:26.941846 durkinza.cdk-networkfirewall-l2-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:02:26.937846 durkinza.cdk-networkfirewall-l2-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:02:26.937846 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:02:26.937846 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/cdk_networkfirewall_l2/
--rw-r--r--   0 runner    (1001) docker     (123)   206923 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/cdk_networkfirewall_l2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:02:26.937846 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/cdk_networkfirewall_l2/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100753 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:02:14.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/cdk_networkfirewall_l2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:02:26.937846 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-26 04:02:26.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-26 04:02:26.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:02:26.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 04:02:26.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 04:02:26.000000 durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.787728 durkinza.cdk-networkfirewall-l2-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.787728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/
+-rw-r--r--   0 runner    (1001) docker     (123)   217751 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102135 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.2/LICENSE` & `durkinza.cdk-networkfirewall-l2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.2/PKG-INFO` & `durkinza.cdk-networkfirewall-l2-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durkinza.cdk-networkfirewall-l2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Experimental L2 constructs for the aws-networkfirewall
 Home-page: https://github.com/durkinza/cdk-networkfirewall-l2#readme
 Author: durkinza<8985088+durkinza@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/durkinza/cdk-networkfirewall-l2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.2/README.md` & `durkinza.cdk-networkfirewall-l2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.2/setup.py` & `durkinza.cdk-networkfirewall-l2-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "durkinza.cdk-networkfirewall-l2",
-    "version": "0.0.2",
+    "version": "0.0.3",
     "description": "Experimental L2 constructs for the aws-networkfirewall",
     "license": "Apache-2.0",
     "url": "https://github.com/durkinza/cdk-networkfirewall-l2#readme",
     "long_description_content_type": "text/markdown",
     "author": "durkinza<8985088+durkinza@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "durkinza.cdk_networkfirewall_l2",
         "durkinza.cdk_networkfirewall_l2._jsii"
     ],
     "package_data": {
         "durkinza.cdk_networkfirewall_l2._jsii": [
-            "cdk-networkfirewall-l2@0.0.2.jsii.tgz"
+            "cdk-networkfirewall-l2@0.0.3.jsii.tgz"
         ],
         "durkinza.cdk_networkfirewall_l2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza/cdk_networkfirewall_l2/__init__.py` & `durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2391,14 +2391,60 @@
             rule_order=rule_order,
             rules=rules,
             variables=variables,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
+    @jsii.member(jsii_name="fromFile")
+    @builtins.classmethod
+    def from_file(
+        cls,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        path: builtins.str,
+        capacity: typing.Optional[jsii.Number] = None,
+        description: typing.Optional[builtins.str] = None,
+        encoding: typing.Optional[builtins.str] = None,
+        rule_group_name: typing.Optional[builtins.str] = None,
+        rule_order: typing.Optional[StatefulRuleOptions] = None,
+        variables: typing.Optional[typing.Union[_aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> "StatefulSuricataRuleGroup":
+        '''(experimental) Reference Suricata rules from a file,.
+
+        :param scope: -
+        :param id: -
+        :param path: (experimental) The suricata rules file location.
+        :param capacity: (experimental) The maximum operating resources that this rule group can use. Estimate a stateful rule group's capacity as the number of rules that you expect to have in it during its lifetime. You can't change this setting after you create the rule group Default: - 200
+        :param description: (experimental) Description of the rule group. Default: - undefined
+        :param encoding: (experimental) The encoding to use for the file. Default: - uft-8
+        :param rule_group_name: (experimental) The descriptive name of the stateful rule group. Default: - CloudFormation-generated name
+        :param rule_order: (experimental) Rule Order. Default: - DEFAULT_RULE_ACTION_ORDER
+        :param variables: (experimental) Settings that are available for use in the rules. Default: - undefined
+
+        :stability: experimental
+        :resource: AWS::NetworkFirewall::RuleGroup
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e2afaa1480e87fa8bd625ff6985dfad168d9ba6d1e13e0c84d0cc9efb78668da)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = StatefulSuricataRuleGroupFromFileProps(
+            path=path,
+            capacity=capacity,
+            description=description,
+            encoding=encoding,
+            rule_group_name=rule_group_name,
+            rule_order=rule_order,
+            variables=variables,
+        )
+
+        return typing.cast("StatefulSuricataRuleGroup", jsii.sinvoke(cls, "fromFile", [scope, id, props]))
+
     @jsii.member(jsii_name="fromRuleGroupArn")
     @builtins.classmethod
     def from_rule_group_arn(
         cls,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         rule_group_arn: builtins.str,
@@ -2434,14 +2480,172 @@
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "ruleGroupId"))
 
 
 @jsii.data_type(
+    jsii_type="@durkinza/cdk-networkfirewall-l2.StatefulSuricataRuleGroupFromFileProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "path": "path",
+        "capacity": "capacity",
+        "description": "description",
+        "encoding": "encoding",
+        "rule_group_name": "ruleGroupName",
+        "rule_order": "ruleOrder",
+        "variables": "variables",
+    },
+)
+class StatefulSuricataRuleGroupFromFileProps:
+    def __init__(
+        self,
+        *,
+        path: builtins.str,
+        capacity: typing.Optional[jsii.Number] = None,
+        description: typing.Optional[builtins.str] = None,
+        encoding: typing.Optional[builtins.str] = None,
+        rule_group_name: typing.Optional[builtins.str] = None,
+        rule_order: typing.Optional[StatefulRuleOptions] = None,
+        variables: typing.Optional[typing.Union[_aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''(experimental) Properties for defining a Stateful Suricata Rule Group from a file.
+
+        :param path: (experimental) The suricata rules file location.
+        :param capacity: (experimental) The maximum operating resources that this rule group can use. Estimate a stateful rule group's capacity as the number of rules that you expect to have in it during its lifetime. You can't change this setting after you create the rule group Default: - 200
+        :param description: (experimental) Description of the rule group. Default: - undefined
+        :param encoding: (experimental) The encoding to use for the file. Default: - uft-8
+        :param rule_group_name: (experimental) The descriptive name of the stateful rule group. Default: - CloudFormation-generated name
+        :param rule_order: (experimental) Rule Order. Default: - DEFAULT_RULE_ACTION_ORDER
+        :param variables: (experimental) Settings that are available for use in the rules. Default: - undefined
+
+        :stability: experimental
+        :resource: AWS::NetworkFIrewall::RuleGroup
+        '''
+        if isinstance(variables, dict):
+            variables = _aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty(**variables)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__5485a09476759c5e75fb7cce8b3bd4b9889793dfe6d19aea78857a4938935089)
+            check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+            check_type(argname="argument capacity", value=capacity, expected_type=type_hints["capacity"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument encoding", value=encoding, expected_type=type_hints["encoding"])
+            check_type(argname="argument rule_group_name", value=rule_group_name, expected_type=type_hints["rule_group_name"])
+            check_type(argname="argument rule_order", value=rule_order, expected_type=type_hints["rule_order"])
+            check_type(argname="argument variables", value=variables, expected_type=type_hints["variables"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "path": path,
+        }
+        if capacity is not None:
+            self._values["capacity"] = capacity
+        if description is not None:
+            self._values["description"] = description
+        if encoding is not None:
+            self._values["encoding"] = encoding
+        if rule_group_name is not None:
+            self._values["rule_group_name"] = rule_group_name
+        if rule_order is not None:
+            self._values["rule_order"] = rule_order
+        if variables is not None:
+            self._values["variables"] = variables
+
+    @builtins.property
+    def path(self) -> builtins.str:
+        '''(experimental) The suricata rules file location.
+
+        :stability: experimental
+        '''
+        result = self._values.get("path")
+        assert result is not None, "Required property 'path' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def capacity(self) -> typing.Optional[jsii.Number]:
+        '''(experimental) The maximum operating resources that this rule group can use.
+
+        Estimate a stateful rule group's capacity as the number of rules that you expect to have in it during its lifetime.
+        You can't change this setting after you create the rule group
+
+        :default: - 200
+
+        :stability: experimental
+        '''
+        result = self._values.get("capacity")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def description(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Description of the rule group.
+
+        :default: - undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("description")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def encoding(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The encoding to use for the file.
+
+        :default: - uft-8
+
+        :stability: experimental
+        '''
+        result = self._values.get("encoding")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def rule_group_name(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The descriptive name of the stateful rule group.
+
+        :default: - CloudFormation-generated name
+
+        :stability: experimental
+        '''
+        result = self._values.get("rule_group_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def rule_order(self) -> typing.Optional[StatefulRuleOptions]:
+        '''(experimental) Rule Order.
+
+        :default: - DEFAULT_RULE_ACTION_ORDER
+
+        :stability: experimental
+        '''
+        result = self._values.get("rule_order")
+        return typing.cast(typing.Optional[StatefulRuleOptions], result)
+
+    @builtins.property
+    def variables(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty]:
+        '''(experimental) Settings that are available for use in the rules.
+
+        :default: - undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("variables")
+        return typing.cast(typing.Optional[_aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "StatefulSuricataRuleGroupFromFileProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="@durkinza/cdk-networkfirewall-l2.StatefulSuricataRuleGroupProps",
     jsii_struct_bases=[],
     name_mapping={
         "capacity": "capacity",
         "description": "description",
         "rule_group_name": "ruleGroupName",
         "rule_order": "ruleOrder",
@@ -4315,14 +4519,15 @@
     "StatefulRuleBase",
     "StatefulRuleBaseProps",
     "StatefulRuleGroupList",
     "StatefulRuleOptions",
     "StatefulStandardAction",
     "StatefulStrictAction",
     "StatefulSuricataRuleGroup",
+    "StatefulSuricataRuleGroupFromFileProps",
     "StatefulSuricataRuleGroupProps",
     "StatelessRule",
     "StatelessRuleGroup",
     "StatelessRuleGroupList",
     "StatelessRuleGroupProps",
     "StatelessRuleList",
     "StatelessRuleProps",
@@ -4508,22 +4713,50 @@
     rule_order: typing.Optional[StatefulRuleOptions] = None,
     rules: typing.Optional[builtins.str] = None,
     variables: typing.Optional[typing.Union[_aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__e2afaa1480e87fa8bd625ff6985dfad168d9ba6d1e13e0c84d0cc9efb78668da(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    path: builtins.str,
+    capacity: typing.Optional[jsii.Number] = None,
+    description: typing.Optional[builtins.str] = None,
+    encoding: typing.Optional[builtins.str] = None,
+    rule_group_name: typing.Optional[builtins.str] = None,
+    rule_order: typing.Optional[StatefulRuleOptions] = None,
+    variables: typing.Optional[typing.Union[_aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__23d4ceba10ad19d785444a5cefc47ebfc90a8d5bbf5d7818f8be4cb15ce8d56e(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     rule_group_arn: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__5485a09476759c5e75fb7cce8b3bd4b9889793dfe6d19aea78857a4938935089(
+    *,
+    path: builtins.str,
+    capacity: typing.Optional[jsii.Number] = None,
+    description: typing.Optional[builtins.str] = None,
+    encoding: typing.Optional[builtins.str] = None,
+    rule_group_name: typing.Optional[builtins.str] = None,
+    rule_order: typing.Optional[StatefulRuleOptions] = None,
+    variables: typing.Optional[typing.Union[_aws_cdk_aws_networkfirewall_ceddda9d.CfnRuleGroup.RuleVariablesProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__23856d3a152b06d39d4ba08d112a04dc652a95ac2d69d1f1ad6f54049b658a18(
     *,
     capacity: typing.Optional[jsii.Number] = None,
     description: typing.Optional[builtins.str] = None,
     rule_group_name: typing.Optional[builtins.str] = None,
     rule_order: typing.Optional[StatefulRuleOptions] = None,
     rules: typing.Optional[builtins.str] = None,
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO` & `durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durkinza.cdk-networkfirewall-l2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Experimental L2 constructs for the aws-networkfirewall
 Home-page: https://github.com/durkinza/cdk-networkfirewall-l2#readme
 Author: durkinza<8985088+durkinza@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/durkinza/cdk-networkfirewall-l2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.2/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt` & `durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
 src/durkinza/cdk_networkfirewall_l2/__init__.py
 src/durkinza/cdk_networkfirewall_l2/py.typed
 src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
-src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.2.jsii.tgz
+src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.3.jsii.tgz
```

