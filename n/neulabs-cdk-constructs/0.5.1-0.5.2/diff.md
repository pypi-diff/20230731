# Comparing `tmp/neulabs-cdk-constructs-0.5.1.tar.gz` & `tmp/neulabs-cdk-constructs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.5.1.tar", last modified: Mon Jul 31 13:22:47 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.5.2.tar", last modified: Mon Jul 31 15:09:36 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.5.1.tar` & `neulabs-cdk-constructs-0.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.957720 neulabs-cdk-constructs-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-31 13:22:47.957720 neulabs-cdk-constructs-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:22:47.957720 neulabs-cdk-constructs-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.953720 neulabs-cdk-constructs-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.953720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.953720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   116717 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.953720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   306174 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.957720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    42813 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.957720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.957720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.957720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-31 13:22:34.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:22:47.953720 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-31 13:22:47.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-31 13:22:47.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:22:47.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-31 13:22:47.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 13:22:47.000000 neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.804113 neulabs-cdk-constructs-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.804113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117850 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   306174 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    49582 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.804113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.5.1/LICENSE` & `neulabs-cdk-constructs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.1/PKG-INFO` & `neulabs-cdk-constructs-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.5.1
+Version: 0.5.2
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.5.1/README.md` & `neulabs-cdk-constructs-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.1/setup.py` & `neulabs-cdk-constructs-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.5.1",
+    "version": "0.5.2",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.5.1.jsii.tgz"
+            "neulabs-cdk-constructs@0.5.2.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.5.1",
+    "0.5.2",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.5.1.jsii.tgz",
+    "neulabs-cdk-constructs@0.5.2.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,69 @@
 import aws_cdk.aws_secretsmanager as _aws_cdk_aws_secretsmanager_ceddda9d
 import constructs as _constructs_77d1e7e8
 from ..stack import (
     BaseStack as _BaseStack_8603347c, BaseStackProps as _BaseStackProps_bfec638c
 )
 
 
+@jsii.data_type(
+    jsii_type="neulabs-cdk-constructs.newrelic.CfnMetricStreamProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "exclude_filters": "excludeFilters",
+        "include_filters": "includeFilters",
+    },
+)
+class CfnMetricStreamProps:
+    def __init__(
+        self,
+        *,
+        exclude_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+        include_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    ) -> None:
+        '''
+        :param exclude_filters: 
+        :param include_filters: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ac6d20bbd3f7853ec725446e0e0bdc01a91d551e3b6b6403d48344fb0cac184f)
+            check_type(argname="argument exclude_filters", value=exclude_filters, expected_type=type_hints["exclude_filters"])
+            check_type(argname="argument include_filters", value=include_filters, expected_type=type_hints["include_filters"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if exclude_filters is not None:
+            self._values["exclude_filters"] = exclude_filters
+        if include_filters is not None:
+            self._values["include_filters"] = include_filters
+
+    @builtins.property
+    def exclude_filters(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.List[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty]]]]:
+        result = self._values.get("exclude_filters")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.List[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty]]]], result)
+
+    @builtins.property
+    def include_filters(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.List[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty]]]]:
+        result = self._values.get("include_filters")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.List[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty]]]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "CfnMetricStreamProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.enum(jsii_type="neulabs-cdk-constructs.newrelic.EndpointType")
 class EndpointType(enum.Enum):
     METRICS = "METRICS"
     LOGS = "LOGS"
 
 
 @jsii.enum(jsii_type="neulabs-cdk-constructs.newrelic.EndpointUrlLogs")
@@ -53,14 +108,15 @@
         id: builtins.str,
         *,
         new_relic_account_id: builtins.str,
         new_relic_api_url_logs: EndpointUrlLogs,
         new_relic_api_url_metrics: EndpointUrlMetrics,
         new_relic_bucket_name: builtins.str,
         new_relic_license_key: builtins.str,
+        cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
         stage: builtins.str,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
@@ -73,14 +129,15 @@
         :param scope: -
         :param id: -
         :param new_relic_account_id: 
         :param new_relic_api_url_logs: 
         :param new_relic_api_url_metrics: 
         :param new_relic_bucket_name: 
         :param new_relic_license_key: 
+        :param cloudwatch_metric_stream_props: 
         :param stage: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
@@ -95,14 +152,15 @@
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = NewRelicStackProps(
             new_relic_account_id=new_relic_account_id,
             new_relic_api_url_logs=new_relic_api_url_logs,
             new_relic_api_url_metrics=new_relic_api_url_metrics,
             new_relic_bucket_name=new_relic_bucket_name,
             new_relic_license_key=new_relic_license_key,
+            cloudwatch_metric_stream_props=cloudwatch_metric_stream_props,
             stage=stage,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
@@ -118,22 +176,31 @@
     def create_cloudwatch_logs_stream_role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.invoke(self, "createCloudwatchLogsStreamRole", []))
 
     @jsii.member(jsii_name="createCloudwatchMetricStream")
     def create_cloudwatch_metric_stream(
         self,
         firehose_arn: builtins.str,
+        *,
+        exclude_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+        include_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
     ) -> _aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream:
         '''
         :param firehose_arn: -
+        :param exclude_filters: 
+        :param include_filters: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5773e82050fc71ec7adaea596012c6633e76c642a3debe22d934aa0706495f65)
             check_type(argname="argument firehose_arn", value=firehose_arn, expected_type=type_hints["firehose_arn"])
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream, jsii.invoke(self, "createCloudwatchMetricStream", [firehose_arn]))
+        props = CfnMetricStreamProps(
+            exclude_filters=exclude_filters, include_filters=include_filters
+        )
+
+        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream, jsii.invoke(self, "createCloudwatchMetricStream", [firehose_arn, props]))
 
     @jsii.member(jsii_name="createFirehoseBucket")
     def create_firehose_bucket(
         self,
         new_relic_bucket_name: builtins.str,
     ) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
         '''
@@ -333,14 +400,15 @@
         "termination_protection": "terminationProtection",
         "stage": "stage",
         "new_relic_account_id": "newRelicAccountId",
         "new_relic_api_url_logs": "newRelicApiUrlLogs",
         "new_relic_api_url_metrics": "newRelicApiUrlMetrics",
         "new_relic_bucket_name": "newRelicBucketName",
         "new_relic_license_key": "newRelicLicenseKey",
+        "cloudwatch_metric_stream_props": "cloudwatchMetricStreamProps",
     },
 )
 class NewRelicStackProps(_BaseStackProps_bfec638c):
     def __init__(
         self,
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
@@ -355,14 +423,15 @@
         termination_protection: typing.Optional[builtins.bool] = None,
         stage: builtins.str,
         new_relic_account_id: builtins.str,
         new_relic_api_url_logs: EndpointUrlLogs,
         new_relic_api_url_metrics: EndpointUrlMetrics,
         new_relic_bucket_name: builtins.str,
         new_relic_license_key: builtins.str,
+        cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
@@ -373,17 +442,20 @@
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param stage: 
         :param new_relic_account_id: 
         :param new_relic_api_url_logs: 
         :param new_relic_api_url_metrics: 
         :param new_relic_bucket_name: 
         :param new_relic_license_key: 
+        :param cloudwatch_metric_stream_props: 
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
+        if isinstance(cloudwatch_metric_stream_props, dict):
+            cloudwatch_metric_stream_props = CfnMetricStreamProps(**cloudwatch_metric_stream_props)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1b73444472d0b16a38d845ab8c4feabeadd9937eadb9c68ca1f7a002e868c7df)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
@@ -394,14 +466,15 @@
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
             check_type(argname="argument new_relic_account_id", value=new_relic_account_id, expected_type=type_hints["new_relic_account_id"])
             check_type(argname="argument new_relic_api_url_logs", value=new_relic_api_url_logs, expected_type=type_hints["new_relic_api_url_logs"])
             check_type(argname="argument new_relic_api_url_metrics", value=new_relic_api_url_metrics, expected_type=type_hints["new_relic_api_url_metrics"])
             check_type(argname="argument new_relic_bucket_name", value=new_relic_bucket_name, expected_type=type_hints["new_relic_bucket_name"])
             check_type(argname="argument new_relic_license_key", value=new_relic_license_key, expected_type=type_hints["new_relic_license_key"])
+            check_type(argname="argument cloudwatch_metric_stream_props", value=cloudwatch_metric_stream_props, expected_type=type_hints["cloudwatch_metric_stream_props"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "stage": stage,
             "new_relic_account_id": new_relic_account_id,
             "new_relic_api_url_logs": new_relic_api_url_logs,
             "new_relic_api_url_metrics": new_relic_api_url_metrics,
             "new_relic_bucket_name": new_relic_bucket_name,
             "new_relic_license_key": new_relic_license_key,
@@ -422,14 +495,16 @@
             self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
+        if cloudwatch_metric_stream_props is not None:
+            self._values["cloudwatch_metric_stream_props"] = cloudwatch_metric_stream_props
 
     @builtins.property
     def analytics_reporting(self) -> typing.Optional[builtins.bool]:
         '''Include runtime versioning information in this Stack.
 
         :default:
 
@@ -634,45 +709,60 @@
 
     @builtins.property
     def new_relic_license_key(self) -> builtins.str:
         result = self._values.get("new_relic_license_key")
         assert result is not None, "Required property 'new_relic_license_key' is missing"
         return typing.cast(builtins.str, result)
 
+    @builtins.property
+    def cloudwatch_metric_stream_props(self) -> typing.Optional[CfnMetricStreamProps]:
+        result = self._values.get("cloudwatch_metric_stream_props")
+        return typing.cast(typing.Optional[CfnMetricStreamProps], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "NewRelicStackProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
+    "CfnMetricStreamProps",
     "EndpointType",
     "EndpointUrlLogs",
     "EndpointUrlMetrics",
     "NewRelicStack",
     "NewRelicStackProps",
 ]
 
 publication.publish()
 
+def _typecheckingstub__ac6d20bbd3f7853ec725446e0e0bdc01a91d551e3b6b6403d48344fb0cac184f(
+    *,
+    exclude_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    include_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__3d16994fa6098e1a11bee3003bb87e23e040f04cdc0edc42f729eccb764b26ca(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     new_relic_account_id: builtins.str,
     new_relic_api_url_logs: EndpointUrlLogs,
     new_relic_api_url_metrics: EndpointUrlMetrics,
     new_relic_bucket_name: builtins.str,
     new_relic_license_key: builtins.str,
+    cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
     stage: builtins.str,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
@@ -682,14 +772,17 @@
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__5773e82050fc71ec7adaea596012c6633e76c642a3debe22d934aa0706495f65(
     firehose_arn: builtins.str,
+    *,
+    exclude_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    include_filters: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.CfnMetricStream.MetricStreamFilterProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__293b2457a5464a82a7b9803bc92a5b11e65e07b096a59d01d32e5d5aeb5758de(
     new_relic_bucket_name: builtins.str,
 ) -> None:
@@ -781,10 +874,11 @@
     termination_protection: typing.Optional[builtins.bool] = None,
     stage: builtins.str,
     new_relic_account_id: builtins.str,
     new_relic_api_url_logs: EndpointUrlLogs,
     new_relic_api_url_metrics: EndpointUrlMetrics,
     new_relic_bucket_name: builtins.str,
     new_relic_license_key: builtins.str,
+    cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.5.1
+Version: 0.5.2
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.5.1/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.1.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.2.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

