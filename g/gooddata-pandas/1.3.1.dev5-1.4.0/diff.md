# Comparing `tmp/gooddata-pandas-1.3.1.dev5.tar.gz` & `tmp/gooddata-pandas-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-pandas-1.3.1.dev5.tar", last modified: Fri Jun 23 15:18:30 2023, max compression
+gzip compressed data, was "gooddata-pandas-1.4.0.tar", last modified: Mon Jul 31 09:28:07 2023, max compression
```

## Comparing `gooddata-pandas-1.3.1.dev5.tar` & `gooddata-pandas-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    78103 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/gooddata_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/data_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    16321 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/good_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/result_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-23 15:18:22.000000 gooddata-pandas-1.3.1.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:07.937632 gooddata-pandas-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    78103 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-31 09:28:07.937632 gooddata-pandas-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:07.937632 gooddata-pandas-1.4.0/gooddata_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/data_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/good_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22864 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/result_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/gooddata_pandas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:07.937632 gooddata-pandas-1.4.0/gooddata_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-31 09:28:07.000000 gooddata-pandas-1.4.0/gooddata_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-31 09:28:07.000000 gooddata-pandas-1.4.0/gooddata_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:28:07.000000 gooddata-pandas-1.4.0/gooddata_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 09:28:07.000000 gooddata-pandas-1.4.0/gooddata_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 09:28:07.000000 gooddata-pandas-1.4.0/gooddata_pandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:28:07.937632 gooddata-pandas-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-31 09:27:56.000000 gooddata-pandas-1.4.0/setup.py
```

### Comparing `gooddata-pandas-1.3.1.dev5/LICENSE.txt` & `gooddata-pandas-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev5/PKG-INFO` & `gooddata-pandas-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.3.1.dev5
+Version: 1.4.0
 Summary: GoodData.CN to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev5
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.4.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoodData Pandas
 
 This package contains a thin layer that utilizes gooddata-sdk and allows you to conveniently create pandas series and
 data frames from the computations done against semantic model in your [GoodData.CN](https://www.gooddata.com/developers/cloud-native/) workspace.
```

### Comparing `gooddata-pandas-1.3.1.dev5/README.md` & `gooddata-pandas-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev5/gooddata_pandas/data_access.py` & `gooddata-pandas-1.4.0/gooddata_pandas/dataframe.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,317 +1,314 @@
 # (C) 2021 GoodData Corporation
 from __future__ import annotations
 
-from typing import Any, Optional, Union
+from typing import Optional, Tuple, Union
 
+import pandas
+
+from gooddata_api_client import models
+from gooddata_pandas.data_access import compute_and_extract
+from gooddata_pandas.result_convertor import (
+    _DEFAULT_PAGE_SIZE,
+    DataFrameMetadata,
+    LabelOverrides,
+    convert_execution_response_to_dataframe,
+)
 from gooddata_pandas.utils import (
     ColumnsDef,
+    DefaultInsightColumnNaming,
     IndexDef,
     LabelItemDef,
-    _str_to_obj_id,
-    _to_attribute,
     _to_item,
-    _typed_attribute_value,
+    make_pandas_index,
 )
 from gooddata_sdk import (
     Attribute,
-    AttributeFilter,
-    CatalogWorkspaceContent,
+    BareExecutionResponse,
     ExecutionDefinition,
-    ExecutionResponse,
     Filter,
     GoodDataSdk,
-    Metric,
-    MetricValueFilter,
-    ObjId,
+    ResultCacheMetadata,
+    ResultSizeDimensions,
 )
 
 
-class ExecutionDefinitionBuilder:
-    _DEFAULT_INDEX_NAME: str = "0"
-
-    def __init__(self, columns: ColumnsDef, index_by: Optional[IndexDef] = None) -> None:
-        self._attributes: list[Attribute] = []
-        self._metrics: list[Metric] = []
-        self._col_to_attr_idx: dict[str, int] = dict()
-        self._index_to_attr_idx: dict[str, int] = dict()
-        self._col_to_metric_idx: dict[str, int] = dict()
-
-        self._process_columns(columns)
-        self._process_index(index_by)
-
-    @property
-    def col_to_attr_idx(self) -> dict[str, int]:
-        return self._col_to_attr_idx
-
-    @property
-    def index_to_attr_idx(self) -> dict[str, int]:
-        return self._index_to_attr_idx
-
-    @property
-    def col_to_metric_idx(self) -> dict[str, int]:
-        return self._col_to_metric_idx
-
-    def _process_columns(self, columns: ColumnsDef) -> None:
-        for column_name, column_def in columns.items():
-            self._add_column(column_name, column_def)
-
-    def _add_column(self, column_name: str, column_def: Union[str, Attribute, Metric, ObjId]) -> None:
-        item = _to_item(column_def)
-        if isinstance(item, Attribute):
-            # prevent double-add for attributes that are using same labels. this has no real effect on the result
-            # apart from extra load/size of the result that would contain the duplicates.
-            #
-            # this may typically happen when same labels are used for indexing & data
-            attr_index = self._find_attribute_index(item)
-
-            if attr_index is not None:
-                self._col_to_attr_idx[column_name] = attr_index
-            else:
-                self._col_to_attr_idx[column_name] = len(self._attributes)
-                self._attributes.append(item)
-        elif isinstance(item, Metric):
-            self._col_to_metric_idx[column_name] = len(self._metrics)
-            self._metrics.append(item)
-
-    def _process_index(self, index_by: Optional[IndexDef] = None) -> None:
-        if index_by is None:
-            return
-
-        if not isinstance(index_by, dict):
-            _index_by = {self._DEFAULT_INDEX_NAME: index_by}
-        else:
-            _index_by = index_by
-
-        for index_name, index_def in _index_by.items():
-            if isinstance(index_def, str) and (index_def in self._col_to_attr_idx):
-                # known attribute defined in columns referenced by the column key
-                attr_index = self._col_to_attr_idx[index_def]
-                self._index_to_attr_idx[index_name] = attr_index
-            elif isinstance(index_def, str) and (index_def in self._col_to_metric_idx):
-                # known metric defined in columns referenced by the column key - index_by cannot be a metric
-                raise ValueError(f"Invalid index_col item {index_def}, type={type(self._col_to_metric_idx[index_def])}")
-            else:
-                self._process_index_item_without_col_ref(index_name, index_def)
-
-    def _find_attribute_index(self, item: Attribute) -> Union[int | None]:
-        existing_attr_idx = next(
-            (idx for idx, attr in enumerate(self._attributes) if item.has_same_label(attr)),
-            None,
-        )
-        return existing_attr_idx
-
-    def _process_index_item_without_col_ref(self, index_name: str, index_def: LabelItemDef) -> None:
-        norm_index_def = index_def
-        if isinstance(index_def, str) and (not index_def.startswith("label/")):
-            # it is not a obj id in string form - consider it label_id and extend it to obj id string form
-            norm_index_def = f"label/{index_def}"
-        attr_item = _to_attribute(norm_index_def)
-        attr_index = self._find_attribute_index(attr_item)
-
-        if attr_index is not None:
-            self._index_to_attr_idx[index_name] = attr_index
-        else:
-            self._index_to_attr_idx[index_name] = len(self._attributes)
-            self._attributes.append(attr_item)
-
-    def _update_filter_ids(self, filter_by: Optional[Union[Filter, list[Filter]]] = None) -> Optional[list[Filter]]:
-        filters = [filter_by] if isinstance(filter_by, Filter) else filter_by
-        if filters:
-            for _filter in filters:
-                if isinstance(_filter, AttributeFilter) and isinstance(_filter.label, str):
-                    if _filter.label in self._col_to_attr_idx:
-                        _filter.label = self._attributes[self._col_to_attr_idx[_filter.label]].label
-                    elif _filter.label in self._index_to_attr_idx:
-                        _filter.label = self._attributes[self._index_to_attr_idx[_filter.label]].label
-                    elif _filter.label in self._col_to_metric_idx:
-                        raise ValueError(f"AttributeFilter instance referencing metric [{_filter.label}]")
-                    else:
-                        _filter.label = _str_to_obj_id(_filter.label) or _filter.label
-                elif isinstance(_filter, MetricValueFilter) and isinstance(_filter.metric, str):
-                    if _filter.metric in self._col_to_metric_idx:
-                        # Metric is referenced by local_id which was already generated during creation of columns
-                        # When Metric filter contains ObjId reference, it does not need to be modified
-                        _filter.metric = self._metrics[self._col_to_metric_idx[_filter.metric]].local_id
-
-        return filters
-
-    def build_execution_definition(
-        self, filter_by: Optional[Union[Filter, list[Filter]]] = None
-    ) -> ExecutionDefinition:
-        dimensions = [
-            ["measureGroup"] if len(self._metrics) else None,
-            [a.local_id for a in self._attributes] if len(self._attributes) else None,
-        ]
-
-        filters = self._update_filter_ids(filter_by)
-
-        return ExecutionDefinition(
-            attributes=self._attributes,
-            metrics=self._metrics,
-            filters=filters,
-            dimensions=dimensions,
-        )
-
-
-def _compute(
-    sdk: GoodDataSdk,
-    workspace_id: str,
-    columns: ColumnsDef,
-    index_by: Optional[IndexDef] = None,
-    filter_by: Optional[Union[Filter, list[Filter]]] = None,
-) -> tuple[ExecutionResponse, dict[str, int], dict[str, int], dict[str, int]]:
+class DataFrameFactory:
     """
-    Creates execution-by-convention to retrieve data for frame with the provided columns that is optionally
-    indexed by index_by label and optionally also filtered.
-
-    The convention is as follows:
+    Factory to create pandas.DataFrame instances.
 
-    -  If the columns contain labels and facts/metric, then two dimensional result will be created. first dim
-       will contain measureGroup, second dimension will be all the attributes
+    Methods:
+        - indexed(self, index_by: IndexDef, columns:ColumnsDef, filter_by: Optional[Union[Filter, list[Filter]]] = None)
+            -> pandas.DataFrame:
+        - not_indexed(self, columns: ColumnsDef, filter_by: Optional[Union[Filter, list[Filter]]] = None)
+            -> pandas.DataFrame:
+        - for_items(self, items: ColumnsDef, filter_by: Optional[Union[Filter, list[Filter]]] = None,
+            auto_index: bool = True) -> pandas.DataFrame:
+        - for_insight(self, insight_id: str, auto_index: bool = True)
+            -> pandas.DataFrame:
+        - result_cache_metadata_for_exec_result_id(self, result_id: str)
+            -> ResultCacheMetadata:
+        - for_exec_def(self, exec_def: ExecutionDefinition, label_overrides: Optional[LabelOverrides] = None,
+            result_size_dimensions_limits: ResultSizeDimensions = (), result_size_bytes_limit: Optional[int] = None,
+            page_size: int = _DEFAULT_PAGE_SIZE,) -> Tuple[pandas.DataFrame, DataFrameMetadata]:
+        - for_exec_result_id(self, result_id: str, label_overrides: Optional[LabelOverrides] = None,
+            result_cache_metadata: Optional[ResultCacheMetadata] = None,
+            result_size_dimensions_limits: ResultSizeDimensions = (),
+            result_size_bytes_limit: Optional[int] = None,
+            use_local_ids_in_headers: bool = False, page_size: int = _DEFAULT_PAGE_SIZE,)
+            -> Tuple[pandas.DataFrame, DataFrameMetadata]:
+    """
 
-    -  If indexing is desired, then the index label will be placed in the attribute dimension and will be the
-       first in that dimension
+    def __init__(self, sdk: GoodDataSdk, workspace_id: str) -> None:
+        """
+        Args:
+            sdk (GoodDataSdk): GoodData SDK instance.
+            workspace_id (str): Workspace identifier.
+        """
+        self._sdk = sdk
+        self._workspace_id = workspace_id
+
+    def indexed(
+        self, index_by: IndexDef, columns: ColumnsDef, filter_by: Optional[Union[Filter, list[Filter]]] = None
+    ) -> pandas.DataFrame:
+        """
+        Creates a data frame indexed by values of the label. The data frame columns will be created from either
+        metrics or other label values.
+
+        Note that depending on composition of the labels, the DataFrame's index may or may not be unique.
+
+        Args:
+            index_by (IndexDef): One or more labels to index by.
+            columns (ColumnsDef): Dictionary mapping column name to its definition.
+            filter_by (Optional[Union[Filter, list[Filter]]]):
+                Optional filters to apply during computation on the server.
+
+        Returns:
+            pandas.DataFrame: A DataFrame instance.
+        """
+        data, index = compute_and_extract(
+            self._sdk,
+            self._workspace_id,
+            columns=columns,
+            index_by=index_by,
+            filter_by=filter_by,
+        )
 
-    -  Otherwise the execution will be single-dim and will contain either measureGroup or all attributes
+        _idx = make_pandas_index(index)
 
-    Only columns contain always full identification of objects in a form { 'index', 'full identification' }.
-    index_by and filters may contain references to columns using the index!
+        return pandas.DataFrame(data=data, index=_idx)
 
-    The compute will return execution response and two mappings:
-    -  pandas name to index where headers appear in the attribute dimension
-    -  pandas col name to index where headers appear in metric dimension
-    -  pandas index name to index where headers appear in the attribute dimension
-    """
+    def not_indexed(
+        self, columns: ColumnsDef, filter_by: Optional[Union[Filter, list[Filter]]] = None
+    ) -> pandas.DataFrame:
+        """
+        Creates a data frame with columns created from metrics and or labels.
+
+        Args:
+            columns (ColumnsDef): Dictionary mapping column name to its definition.
+            filter_by (Optional[Union[Filter, list[Filter]]]): Optionally specify filters to apply during
+                computation on the server.
+
+        Returns:
+            pandas.DataFrame: A DataFrame instance.
+        """
+
+        data, _ = compute_and_extract(self._sdk, self._workspace_id, columns=columns, filter_by=filter_by)
+
+        return pandas.DataFrame(data=data)
+
+    def for_items(
+        self, items: ColumnsDef, filter_by: Optional[Union[Filter, list[Filter]]] = None, auto_index: bool = True
+    ) -> pandas.DataFrame:
+        """
+        Creates a data frame for named items. This is a convenience method that will create DataFrame with or
+        without index based on the context of the items that you pass.
+
+        Args:
+            items (ColumnsDef): Dictionary mapping item name to its definition.
+            filter_by (Optional[Union[Filter, list[Filter]]]): Optionally specify filters to apply during computation
+                on the server.
+            auto_index (bool): Default True. Enables creation of DataFrame with index depending on the contents
+                of the items.
+
+        Returns:
+            pandas.DataFrame: A DataFrame instance.
+        """
+        resolved_attr_cols: dict[str, LabelItemDef] = dict()
+        resolved_measure_cols: ColumnsDef = dict()
+        has_attributes = False
+        has_measures = False
+
+        for col_name, col_def in items.items():
+            item = _to_item(col_def, local_id=col_name)
+
+            if isinstance(item, Attribute):
+                has_attributes = True
+                resolved_attr_cols[col_name] = item
+            else:
+                has_measures = True
+                resolved_measure_cols[col_name] = item
 
-    builder = ExecutionDefinitionBuilder(columns, index_by)
-    exec_def = builder.build_execution_definition(filter_by)
+        if not auto_index or not has_measures or not has_attributes:
+            columns: ColumnsDef = {**resolved_attr_cols, **resolved_measure_cols}
 
-    return (
-        sdk.compute.for_exec_def(workspace_id, exec_def),
-        builder.col_to_attr_idx,
-        builder.col_to_metric_idx,
-        builder.index_to_attr_idx,
-    )
-
-
-_RESULT_PAGE_LEN = 1000
-
-
-#
-# Note: both of the extract functions assume the number of measures requested for the data frame is less than
-# page limit enforced by the server. The function for getting data frame for measures only does not paging at all
-# and the one that gets data from possibly two-dimensional result always pages only through the dimension that
-# contains attributes.
-#
-
-
-def _extract_for_metrics_only(response: ExecutionResponse, cols: list, col_to_metric_idx: dict) -> dict:
-    exec_def = response.exec_def
-    result = response.read_result(len(exec_def.metrics))
-    data = dict()
-
-    for col in cols:
-        data[col] = [result.data[col_to_metric_idx[col]]]
-
-    return data
-
-
-def _typed_result(catalog: CatalogWorkspaceContent, attribute: Attribute, result_values: list[Any]) -> list[Any]:
-    """Convert result_values to proper data types."""
-    catalog_attribute = catalog.find_label_attribute(attribute.label)
-    if catalog_attribute is None:
-        raise ValueError(f"Unable to find attribute {attribute.label} in catalog")
-    return [_typed_attribute_value(catalog_attribute, value) for value in result_values]
-
-
-def _extract_from_attributes_and_maybe_metrics(
-    response: ExecutionResponse,
-    catalog: CatalogWorkspaceContent,
-    cols: list[str],
-    col_to_attr_idx: dict[str, int],
-    col_to_metric_idx: dict[str, int],
-    index_to_attr_idx: Optional[dict[str, int]] = None,
-) -> tuple[dict, dict]:
-
-    exec_def = response.exec_def
-    offset = [0 for _ in exec_def.dimensions]
-    limit = [len(exec_def.metrics), _RESULT_PAGE_LEN] if exec_def.has_metrics() else [_RESULT_PAGE_LEN]
-    attribute_dim = 1 if exec_def.has_metrics() else 0
-    result = response.read_result(limit=limit, offset=offset)
-    safe_index_to_attr_idx = index_to_attr_idx if index_to_attr_idx is not None else dict()
-
-    # mappings from column name to Attribute
-    index_to_attribute = {index_name: exec_def.attributes[i] for index_name, i in safe_index_to_attr_idx.items()}
-    col_to_attribute = {col: exec_def.attributes[i] for col, i, in col_to_attr_idx.items()}
-
-    # datastructures to return
-    index: dict[str, list[Any]] = {idx_name: [] for idx_name in safe_index_to_attr_idx}
-    data: dict[str, list[Any]] = {col: [] for col in cols}
-
-    while True:
-        for idx_name in index:
-            rs = result.get_all_header_values(attribute_dim, safe_index_to_attr_idx[idx_name])
-            attribute = index_to_attribute[idx_name]
-            index[idx_name] += _typed_result(catalog, attribute, rs)
-        for col in cols:
-            if col in col_to_attr_idx:
-                rs = result.get_all_header_values(attribute_dim, col_to_attr_idx[col])
-                attribute = col_to_attribute[col]
-                data[col] += _typed_result(catalog, attribute, rs)
-            elif col_to_metric_idx[col] < len(result.data):
-                data[col] += result.data[col_to_metric_idx[col]]
-        if result.is_complete(attribute_dim):
-            break
-
-        offset[attribute_dim] = result.next_page_start(attribute_dim)
-        result = response.read_result(limit=limit, offset=offset)
-
-    return data, index
-
-
-def compute_and_extract(
-    sdk: GoodDataSdk,
-    workspace_id: str,
-    columns: ColumnsDef,
-    index_by: Optional[IndexDef] = None,
-    filter_by: Optional[Union[Filter, list[Filter]]] = None,
-) -> tuple[dict, dict]:
-    """
-    Convenience function to drive computation & data extraction on behalf of the series and data frame factories.
+            return self.not_indexed(columns=columns, filter_by=filter_by)
 
-    Given data columns and index columns, this function will create AFM execution and then read the results and
-    populate data and index dicts.
+        return self.indexed(
+            index_by=resolved_attr_cols,
+            columns=resolved_measure_cols,
+            filter_by=filter_by,
+        )
 
-    For each column in `columns`, the returned data will contain key under which there is array of data for that column
-    For each index in index_by, the returned data will contain key under which there is array with data to construct the
-    index. When there are multiple indexes, feed the indexes to MultiIndex.from_arrays().
+    def for_insight(self, insight_id: str, auto_index: bool = True) -> pandas.DataFrame:
+        """
+        Creates a data frame with columns based on the content of the insight with the provided identifier.
+
+        Args:
+            insight_id (str): Insight identifier.
+            auto_index (bool): Default True. Enables creation of DataFrame with index depending on the contents
+                of the insight.
+
+        Returns:
+            pandas.DataFrame: A DataFrame instance.
+        """
+        naming = DefaultInsightColumnNaming()
+        insight = self._sdk.insights.get_insight(workspace_id=self._workspace_id, insight_id=insight_id)
+        filter_by = [f.as_computable() for f in insight.filters]
+        columns: ColumnsDef = {
+            **{naming.col_name_for_attribute(a): a.as_computable() for a in insight.attributes},
+            **{naming.col_name_for_metric(m): m.as_computable() for m in insight.metrics},
+        }
+
+        return self.for_items(columns, filter_by=filter_by, auto_index=auto_index)
+
+    def result_cache_metadata_for_exec_result_id(self, result_id: str) -> ResultCacheMetadata:
+        """
+        Retrieves result cache metadata for given :result_id:
+
+        Args:
+            result_id (str): ID of execution result to retrieve the metadata for.
+
+        Returns:
+            ResultCacheMetadata: Corresponding result cache metadata.
+        """
+        return self._sdk.compute.retrieve_result_cache_metadata(workspace_id=self._workspace_id, result_id=result_id)
+
+    def for_exec_def(
+        self,
+        exec_def: ExecutionDefinition,
+        label_overrides: Optional[LabelOverrides] = None,
+        result_size_dimensions_limits: ResultSizeDimensions = (),
+        result_size_bytes_limit: Optional[int] = None,
+        page_size: int = _DEFAULT_PAGE_SIZE,
+    ) -> Tuple[pandas.DataFrame, DataFrameMetadata]:
+        """
+        Creates a data frame using an execution definition.
+
+        Each dimension may be sliced by multiple labels. The factory will create MultiIndex for the dataframe's
+        row index and the columns.
+
+        Example of label_overrides structure:
+
+        .. code-block:: python
+
+            {
+                "labels": {
+                    "local_attribute_id": {
+                        "title": "My new attribute label"
+                    ,...
+                },
+                "metrics": {
+                    "local_metric_id": {
+                        "title": "My new metric label"
+                    },...
+                }
+            }
+
+        Args:
+            exec_def (ExecutionDefinition): Execution definition.
+            label_overrides (Optional[LabelOverrides]): Label overrides for metrics and attributes.
+            result_size_dimensions_limits (ResultSizeDimensions): A tuple containing maximum size of result dimensions.
+            result_size_bytes_limit (Optional[int]): Maximum size of result in bytes.
+            page_size (int): Number of records per page.
+
+        Returns:
+            Tuple[pandas.DataFrame, DataFrameMetadata]: Tuple holding DataFrame and DataFrame metadata.
+        """
+        if label_overrides is None:
+            label_overrides = {}
+
+        execution = self._sdk.compute.for_exec_def(workspace_id=self._workspace_id, exec_def=exec_def)
+        result_cache_metadata = self.result_cache_metadata_for_exec_result_id(execution.result_id)
+
+        return convert_execution_response_to_dataframe(
+            execution_response=execution.bare_exec_response,
+            result_cache_metadata=result_cache_metadata,
+            label_overrides=label_overrides,
+            result_size_dimensions_limits=result_size_dimensions_limits,
+            result_size_bytes_limit=result_size_bytes_limit,
+            page_size=page_size,
+        )
 
-    Note that as convenience it is possible to pass just single index. in that case the index dict will contain exactly
-    one key of '0' (just get first value from dict when consuming the result).
-    """
-    result = _compute(
-        sdk=sdk,
-        workspace_id=workspace_id,
-        index_by=index_by,
-        columns=columns,
-        filter_by=filter_by,
-    )
-
-    response, col_to_attr_idx, col_to_metric_idx, index_to_attr_idx = result
-
-    exec_def = response.exec_def
-    cols = list(columns.keys())
-
-    catalog = sdk.catalog_workspace_content.get_full_catalog(workspace_id)
-
-    if not exec_def.has_attributes():
-        return _extract_for_metrics_only(response, cols, col_to_metric_idx), dict()
-    else:
-        return _extract_from_attributes_and_maybe_metrics(
-            response,
-            catalog,
-            cols,
-            col_to_attr_idx,
-            col_to_metric_idx,
-            index_to_attr_idx,
+    def for_exec_result_id(
+        self,
+        result_id: str,
+        label_overrides: Optional[LabelOverrides] = None,
+        result_cache_metadata: Optional[ResultCacheMetadata] = None,
+        result_size_dimensions_limits: ResultSizeDimensions = (),
+        result_size_bytes_limit: Optional[int] = None,
+        use_local_ids_in_headers: bool = False,
+        page_size: int = _DEFAULT_PAGE_SIZE,
+    ) -> Tuple[pandas.DataFrame, DataFrameMetadata]:
+        """
+            Retrieves a DataFrame and DataFrame metadata for a given execution result identifier.
+
+            Example of label_overrides structure:
+
+            .. code-block:: python
+
+                {
+                    "labels": {
+                        "local_attribute_id": {
+                            "title": "My new attribute label"
+                        ,...
+                    },
+                    "metrics": {
+                        "local_metric_id": {
+                            "title": "My new metric label"
+                        },...
+                    }
+                }
+
+        Args:
+            result_id (str): Execution result identifier.
+            label_overrides (Optional[LabelOverrides]): Label overrides for metrics and attributes.
+            result_cache_metadata (Optional[ResultCacheMetadata]): Cache metadata for the execution result.
+            result_size_dimensions_limits (ResultSizeDimensions): A tuple containing maximum size of result dimensions.
+            result_size_bytes_limit (Optional[int]): Maximum size of result in bytes.
+            use_local_ids_in_headers (bool): Use local identifier in headers.
+            page_size (int): Number of records per page.
+
+        Returns:
+            Tuple[pandas.DataFrame, DataFrameMetadata]: Tuple holding DataFrame and DataFrame metadata.
+        """
+        if label_overrides is None:
+            label_overrides = {}
+
+        if result_cache_metadata is None:
+            result_cache_metadata = self.result_cache_metadata_for_exec_result_id(result_id=result_id)
+
+        return convert_execution_response_to_dataframe(
+            execution_response=BareExecutionResponse(
+                api_client=self._sdk.client,
+                workspace_id=self._workspace_id,
+                execution_response=models.AfmExecutionResponse(
+                    result_cache_metadata.execution_response, _check_type=False
+                ),
+            ),
+            result_cache_metadata=result_cache_metadata,
+            label_overrides=label_overrides,
+            result_size_dimensions_limits=result_size_dimensions_limits,
+            result_size_bytes_limit=result_size_bytes_limit,
+            use_local_ids_in_headers=use_local_ids_in_headers,
+            page_size=page_size,
         )
```

### Comparing `gooddata-pandas-1.3.1.dev5/gooddata_pandas/good_pandas.py` & `gooddata-pandas-1.4.0/gooddata_pandas/good_pandas.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,45 +22,81 @@
     def __init__(
         self,
         host: str,
         token: str,
         headers_host: Optional[str] = None,
         **custom_headers_: Optional[str],
     ) -> None:
+        """
+        Initializes GoodPandas instance.
+
+        Args:
+            host (str): Host for GoodDataSdk.
+            token (str): Token for GoodDataSdk.
+            headers_host (Optional[str]): Host header, if needed.
+            **custom_headers_ (Optional[str]): Additional headers for GoodDataSdk.
+
+        """
         if headers_host is not None:
             custom_headers_["Host"] = headers_host
         self._sdk = GoodDataSdk.create(host, token, USER_AGENT, **custom_headers_)
         self._series_per_ws: dict[str, SeriesFactory] = dict()
         self._frames_per_ws: dict[str, DataFrameFactory] = dict()
 
     @classmethod
     def create_from_profile(cls, profile: str = "default", profiles_path: Path = PROFILES_FILE_PATH) -> GoodPandas:
+        """
+        Creates GoodPandas instance from a given profile.
+
+        Args:
+            profile (str): Name of the profile to use. Defaults to "default".
+            profiles_path (Path): Path to the profiles file. Defaults to PROFILES_FILE_PATH.
+
+        Returns:
+            GoodPandas: A new GoodPandas instance with the settings from the profile.
+
+        """
         content, custom_headers = good_pandas_profile_content(profile, profiles_path)
         return cls(**content, **custom_headers)
 
     @property
     def sdk(self) -> GoodDataSdk:
+        """
+        Retrieves GoodDataSdk instance.
+
+        Returns:
+            GoodDataSdk: The internal GoodDataSdk instance.
+
+        """
         return self._sdk
 
     def series(self, workspace_id: str) -> SeriesFactory:
         """
-        Creates factory to use for construction of pandas.Series.
+        Creates factory for constructing pandas.Series bound to a workspace.
+
+        Args:
+            workspace_id (str): ID of the workspace the factory will be bound to.
+
+        Returns:
+            SeriesFactory: Same instance for a given workspace.
 
-        :param workspace_id: workspace to which the factory will be bound
-        :return: always one same instance for given workspace
         """
         if workspace_id not in self._series_per_ws:
             self._series_per_ws[workspace_id] = SeriesFactory(sdk=self._sdk, workspace_id=workspace_id)
 
         return self._series_per_ws[workspace_id]
 
     def data_frames(self, workspace_id: str) -> DataFrameFactory:
         """
-        Creates factory to use for construction of pandas.DataFrame.
+        Creates factory for constructing pandas.DataFrame bound to a workspace.
+
+        Args:
+            workspace_id (str): ID of the workspace the factory will be bound to.
+
+        Returns:
+            DataFrameFactory: Same instance for a given workspace.
 
-        :param workspace_id: workspace to which the factory will be bound
-        :return: always one same instance for given workspace
         """
         if workspace_id not in self._frames_per_ws:
             self._frames_per_ws[workspace_id] = DataFrameFactory(sdk=self._sdk, workspace_id=workspace_id)
 
         return self._frames_per_ws[workspace_id]
```

### Comparing `gooddata-pandas-1.3.1.dev5/gooddata_pandas/result_convertor.py` & `gooddata-pandas-1.4.0/gooddata_pandas/result_convertor.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,70 +10,108 @@
 _DataHeaders = List[List[Any]]
 _DataArray = List[Union[int, None]]
 LabelOverrides = Dict[str, Dict[str, Dict[str, str]]]
 
 
 @frozen
 class _DataWithHeaders:
-    data: List[_DataArray]
-    """extracted data; either array of values for one-dimensional result or array of arrays of values"""
+    """Extracted data; either array of values for one-dimensional result or array of arrays of values.
 
-    data_headers: Tuple[_DataHeaders, Optional[_DataHeaders]]
-    """per-dimension headers for the data"""
+    Attributes:
+        data (List[_DataArray]):
+            Extracted data; either array of values for one-dimensional result or array of arrays of values.
+        data_headers (Tuple[_DataHeaders, Optional[_DataHeaders]]):
+            Per-dimension headers for the data.
+        grand_totals (Tuple[Optional[List[_DataArray]], Optional[List[_DataArray]]]):
+            Per-dimension grand total data.
+        grand_total_headers (Tuple[Optional[_DataHeaders], Optional[_DataHeaders]]):
+            Per-dimension grand total headers.
+    """
 
+    data: List[_DataArray]
+    data_headers: Tuple[_DataHeaders, Optional[_DataHeaders]]
     grand_totals: Tuple[Optional[List[_DataArray]], Optional[List[_DataArray]]]
-    """per-dimension grand total data"""
-
     grand_total_headers: Tuple[Optional[_DataHeaders], Optional[_DataHeaders]]
-    """per-dimension grand total headers"""
 
 
 @define
 class _AccumulatedData:
     """
     Utility class to offload code from the function that extracts all data and headers for a
     particular paged result. The method drives the paging and calls out to this class to accumulate
     the essential data and headers from the page.
+
+    Attributes:
+        data (List[_DataArray]): Holds the accumulated data arrays from the pages.
+        data_headers (List[Optional[_DataHeaders]]): Holds the headers for data arrays.
+        grand_totals (List[Optional[List[_DataArray]]]): Holds the grand total data arrays.
+        grand_totals_headers (List[Optional[_DataHeaders]]): Holds the headers for grand total data arrays.
     """
 
     data: List[_DataArray] = field(init=False, factory=list)
     data_headers: List[Optional[_DataHeaders]] = field(init=False, factory=lambda: [None, None])
     grand_totals: List[Optional[List[_DataArray]]] = field(init=False, factory=lambda: [None, None])
     grand_totals_headers: List[Optional[_DataHeaders]] = field(init=False, factory=lambda: [None, None])
 
     def accumulate_data(self, from_result: ExecutionResult) -> None:
         """
-        if one-dimensional result, the data is single array, so this adds the elements of that array into 'data'
-        if two-dimensional, the data is array of arrays, so this adds as many arrays as there are table rows
+        Accumulate data from the ExecutionResult.
+
+        If the result is one-dimensional, the data is a single array, so this adds the elements of that array
+        into 'data'. If it's two-dimensional, the data is an array of arrays, so this adds as many arrays as
+        there are table rows.
+
+        Args:
+            from_result (ExecutionResult): The result whose data will be extended into the current instance's data.
         """
         self.data.extend(from_result.data)
 
     def extend_existing_row_data(self, from_result: ExecutionResult) -> None:
+        """
+        Extend the existing row data with the data from the ExecutionResult.
+
+        Args:
+            from_result (ExecutionResult): The result whose data will be extended into the current instance's data.
+        """
         offset = from_result.paging_offset[0]
 
         for i in range(len(from_result.data)):
             self.data[offset + i].extend(from_result.data[i])
 
     def accumulate_headers(self, from_result: ExecutionResult, from_dim: int) -> None:
         """
-        Accumulates headers for particular dimension of a result into the provided `data_headers` array at the index
-        matching the dimension index. This will mutate the `data_headers`
+        Accumulate headers for a particular dimension of a result into the provided `data_headers` array at the index
+        matching the dimension index.
+
+        This will mutate the `data_headers`.
+
+        Args:
+            from_result (ExecutionResult): The result whose headers will be accumulated.
+            from_dim (int): The dimension index.
         """
+
         if self.data_headers[from_dim] is None:
             self.data_headers[from_dim] = from_result.get_all_headers(dim=from_dim)
         else:
             for idx, headers in enumerate(from_result.get_all_headers(dim=from_dim)):
                 cast(_DataHeaders, self.data_headers[from_dim])[idx].extend(headers)
 
     def accumulate_grand_totals(
         self, from_result: ExecutionResult, paging_dim: int, response: BareExecutionResponse
     ) -> None:
         """
-        accumulates grand totals from the results; processes all grand totals on all dimensions; the method
-        needs to know in which direction is the paging happening so that it can append new grand total data.
+        Accumulate grand totals from the results.
+
+        Processes all grand totals on all dimensions and needs to know in which direction the paging is happening
+        in order to append new grand total data.
+
+        Args:
+            from_result (ExecutionResult): The result whose grand totals will be accumulated.
+            paging_dim (int): The paging dimension.
+            response (BareExecutionResponse): The BareExecutionResponse instance.
         """
         grand_totals = from_result.grand_totals
         if not len(grand_totals):
             return
 
         # get dimension indexes mapping from response like {"dim1": 0, "dim0": 1}
         dim_idx_dict = {dim["localIdentifier"]: idx for idx, dim in enumerate(response.dimensions)}
@@ -112,44 +150,65 @@
                     for total_idx, total_data in enumerate(grand_total["data"]):
                         grand_totals_item[total_idx].extend(total_data)
                 else:
                     # have row totals and paging down, keep adding extra rows
                     grand_totals_item.extend(grand_total["data"])
 
     def result(self) -> _DataWithHeaders:
+        """
+        Returns the data with headers.
+
+        Returns:
+            _DataWithHeaders: The data, data headers, grand totals and grand total headers.
+        """
         return _DataWithHeaders(
             data=self.data,
             data_headers=(cast(_DataHeaders, self.data_headers[0]), self.data_headers[1]),
             grand_totals=(self.grand_totals[0], self.grand_totals[1]),
             grand_total_headers=(self.grand_totals_headers[0], self.grand_totals_headers[1]),
         )
 
 
 @define
 class DataFrameMetadata:
-    # row line location where total header is located per index header column
-    # example:
-    # Category  | Country | Budget
-    # Car       | Arizona |    100
-    #           | Texas   |     50
-    #           | SUM     |    150
-    # Train     | Arizona |    200    =>    [[7],[3,6]]
-    #           | Texas   |    100
-    #           | AVG     |    150
-    # SUM       |         |    450
-    row_totals_indexes: List[List[int]]
+    """
+    DataFrameMetadata class stores metadata about a DataFrame.
+
+    Attributes:
+    - row_totals_indexes: A nested list of integers. Each inner list represents
+                          the row indices containing totals per index header column.
+                          Example:
+                          Category  | Country | Budget
+                          Car       | Arizona |    100
+                                    | Texas   |     50
+                                    | SUM     |    150
+                          Train     | Arizona |    200    =>    [[7],[3,6]]
+                                    | Texas   |    100
+                                    | AVG     |    150
+                          SUM       |         |    450
+
+    - execution_response: An instance of BareExecutionResponse representing the
+                          execution response.
+    """
 
+    row_totals_indexes: List[List[int]]
     execution_response: BareExecutionResponse
 
     @classmethod
     def from_data(
         cls,
         headers: Tuple[_DataHeaders, Optional[_DataHeaders]],
         execution_response: BareExecutionResponse,
     ) -> "DataFrameMetadata":
+        """This method constructs a DataFrameMetadata object from data headers and an execution response.
+
+        Args: headers (Tuple[_DataHeaders, Optional[_DataHeaders]]):
+            A tuple containing data headers. execution_response (BareExecutionResponse): An ExecutionResponse object.
+
+        Returns: DataFrameMetadata: An initialized DataFrameMetadata object."""
         row_totals_indexes = [
             [idx for idx, hdr in enumerate(dim) if hdr is not None and "totalHeader" in hdr] for dim in headers[0]
         ]
         return cls(
             row_totals_indexes=row_totals_indexes,
             execution_response=execution_response,
         )
@@ -162,16 +221,23 @@
     result_size_bytes_limit: Optional[int] = None,
     page_size: int = _DEFAULT_PAGE_SIZE,
 ) -> _DataWithHeaders:
     """
     Extracts all data and headers for an execution result. This does page around the execution result to extract
     everything from the paged API.
 
-    :param execution_response: execution response to work with;
-    :return:
+    Args:
+        execution_response (BareExecutionResponse): Execution response to work with.
+        result_cache_metadata (ResultCacheMetadata): Metadata for the result cache.
+        result_size_dimensions_limits (ResultSizeDimensions): Limits for result size dimensions.
+        result_size_bytes_limit (Optional[int], optional): Limit for result size in bytes. Defaults to None.
+        page_size (int, optional): Page size to use when reading data. Defaults to _DEFAULT_PAGE_SIZE.
+
+    Returns:
+        _DataWithHeaders: All the data and headers from the execution result.
     """
     num_dims = len(execution_response.dimensions)
     offset = [0] * num_dims
     limit = [page_size] * num_dims
     acc = _AccumulatedData()
 
     result_size_limits_checked = False
@@ -230,22 +296,26 @@
 def _create_header_mapper(
     response: BareExecutionResponse,
     dim: int,
     label_overrides: Optional[LabelOverrides] = None,
     use_local_ids_in_headers: bool = False,
 ) -> Callable[[Any, Optional[int]], Optional[str]]:
     """
-    Prepares header mapper function which is doing header structures translations into appropriate label used
-    in a dataframe
-    :param response: Response structure to gather dimension header details
-    :param dim: dimension id
-    :param label_overrides: label overrides
-    :param use_local_ids_in_headers: Use local identifiers of header attributes and metrics. Optional.
+    Prepares a header mapper function which translates header structures into appropriate labels used
+    in a dataframe.
+
+    Args:
+        response (BareExecutionResponse): Response structure to gather dimension header details.
+        dim (int): Dimension id.
+        label_overrides (Optional[LabelOverrides]): Label overrides. Defaults to None.
+        use_local_ids_in_headers (bool): Use local identifiers of header attributes and metrics. Optional.
+            Defaults to False.
 
-    :return: Mapper function
+    Returns:
+        Callable[[Any, Optional[int]], Optional[str]]: Mapper function.
     """
     if label_overrides is None:
         label_overrides = {}
 
     dim_descriptor = response.dimensions[dim]
     attribute_labels = label_overrides.get("labels", {})
     measure_labels = label_overrides.get("metrics", {})
@@ -295,14 +365,29 @@
 def _headers_to_index(
     dim_idx: int,
     headers: Tuple[_DataHeaders, Optional[_DataHeaders]],
     response: BareExecutionResponse,
     label_overrides: LabelOverrides,
     use_local_ids_in_headers: bool = False,
 ) -> Optional[pandas.Index]:
+    """Converts headers to a pandas MultiIndex.
+
+    This function converts the headers present in the response to a pandas MultiIndex (can be used in pandas dataframes)
+
+    Args:
+        dim_idx (int): Index of the current dimension.
+        headers (Tuple[_DataHeaders, Optional[_DataHeaders]]):
+            Tuple of data headers and optional secondary data headers.
+        response (BareExecutionResponse): The execution response object with all data.
+        label_overrides (LabelOverrides): A dictionary containing label overrides for the headers.
+        use_local_ids_in_headers (bool, optional): If True, uses local Ids in headers, otherwise not. Defaults to False.
+
+    Returns:
+        Optional[pandas.Index]: A pandas MultiIndex object created from the headers, or None if the headers are empty.
+    """
     if len(response.dimensions) <= dim_idx or not len(response.dimensions[dim_idx]["headers"]):
         return None
 
     mapper = _create_header_mapper(
         response=response,
         dim=dim_idx,
         label_overrides=label_overrides,
@@ -316,16 +401,22 @@
         ],
         names=[mapper(dim_header, None) for dim_header in (response.dimensions[dim_idx]["headers"])],
     )
 
 
 def _merge_grand_totals_into_data(extract: _DataWithHeaders) -> Union[_DataArray, List[_DataArray]]:
     """
-    Merges grand totals into the extracted data. this function will mutate the extracted data, extending
-    the rows and columns with grand totals. Going with mutation here so as not to copy arrays around
+    Merges grand totals into the extracted data. This function will mutate the extracted data,
+    extending the rows and columns with grand totals. Going with mutation here so as not to copy arrays around.
+
+    Args:
+        extract (_DataWithHeaders): Extracted data with headers and grand totals.
+
+    Returns:
+        Union[_DataArray, List[_DataArray]]: Mutated data with rows and columns extended with grand totals.
     """
     data: List[_DataArray] = extract.data
 
     if extract.grand_totals[0] is not None:
         # column totals are computed into extra rows, one row per column total
         # add those rows at the end of the data rows
         data.extend(extract.grand_totals[0])
@@ -336,16 +427,22 @@
         for row_idx, cols_to_append in enumerate(extract.grand_totals[1]):
             data[row_idx].extend(cols_to_append)
 
     return data
 
 
 def _merge_grand_total_headers_into_headers(extract: _DataWithHeaders) -> Tuple[_DataHeaders, Optional[_DataHeaders]]:
-    """
-    Merges grand total headers into data headers. This function will mutate the extracted data.
+    """Merges grand total headers into data headers. This function will mutate the extracted data.
+
+    Args:
+        extract (_DataWithHeaders): The data along with its headers that need to be merged.
+
+    Returns:
+        Tuple[_DataHeaders, Optional[_DataHeaders]]:
+            A tuple containing the modified data headers and the grand total headers if present.
     """
     headers: Tuple[_DataHeaders, Optional[_DataHeaders]] = extract.data_headers
 
     for dim_idx, grand_total_headers in enumerate(extract.grand_total_headers):
         if grand_total_headers is None:
             continue
         header = cast(List[List[Any]], headers[dim_idx])
@@ -365,20 +462,26 @@
     result_size_bytes_limit: Optional[int] = None,
     use_local_ids_in_headers: bool = False,
     page_size: int = _DEFAULT_PAGE_SIZE,
 ) -> Tuple[pandas.DataFrame, DataFrameMetadata]:
     """
     Converts execution result to a pandas dataframe, maintaining the dimensionality of the result.
 
-    Because the result itself does not contain all the necessary metadata to do the full conversion, this method
-    expects that the execution _response_.
+    Args:
+        execution_response (BareExecutionResponse): Execution response through which the result can be read
+            and converted to a dataframe.
+        result_cache_metadata (ResultCacheMetadata): Metadata about the result cache.
+        label_overrides (LabelOverrides): Label overrides for the dataframe.
+        result_size_dimensions_limits (ResultSizeDimensions): Dimension limits for the dataframe.
+        result_size_bytes_limit (Optional[int], default=None): Size limit in bytes for the dataframe.
+        use_local_ids_in_headers (bool, default=False): Use local ids in headers if True, else use default settings.
+        page_size (int, default=_DEFAULT_PAGE_SIZE): Size of the page.
 
-    :param label_overrides: label overrides
-    :param execution_response: execution response through which the result can be read and converted to a dataframe
-    :return: a new dataframe
+    Returns:
+        Tuple[pandas.DataFrame, DataFrameMetadata]: A tuple containing the created dataframe and its metadata.
     """
     extract = _read_complete_execution_result(
         execution_response=execution_response,
         result_cache_metadata=result_cache_metadata,
         result_size_dimensions_limits=result_size_dimensions_limits,
         result_size_bytes_limit=result_size_bytes_limit,
         page_size=page_size,
```

### Comparing `gooddata-pandas-1.3.1.dev5/gooddata_pandas/series.py` & `gooddata-pandas-1.4.0/gooddata_pandas/series.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,57 +7,68 @@
 
 from gooddata_pandas.data_access import compute_and_extract
 from gooddata_pandas.utils import IndexDef, LabelItemDef, make_pandas_index
 from gooddata_sdk import Attribute, Filter, GoodDataSdk, ObjId, SimpleMetric
 
 
 class SeriesFactory:
+    """This class serves as a factory to create Series objects by providing the necessary parameters.
+
+    Attributes:
+      sdk (GoodDataSdk): An instance of the GoodData software development kit.
+      workspace_id (str): The unique identifier of the workspace.
+
+    """
+
     def __init__(self, sdk: GoodDataSdk, workspace_id: str) -> None:
         self._sdk = sdk
         self._workspace_id = workspace_id
 
     def indexed(
         self,
         index_by: IndexDef,
         data_by: Union[SimpleMetric, str, ObjId, Attribute],
         filter_by: Optional[Union[Filter, list[Filter]]] = None,
     ) -> pandas.Series:
-        """
-        Creates pandas Series from data points calculated from a single `data_by` that will be computed on granularity
-        of the index labels. The elements of the index labels will be used to construct simple or hierarchical index.
+        """Creates pandas Series from data points calculated from a single `data_by`.
 
-        :param index_by: label to index by; specify either:
+        Creates pandas Series from data points calculated from a single `data_by`, that will be computed on granularity
+        of the index labels. The elements of the index labels will be used to construct simple or hierarchical index.
 
-         - string with id: ``some_label_id``,
-         - object identifier: ``ObjId(id='some_label_id', type='label')``,
-         - string representation of object identifier: ``label/some_label_id``
-         - or an Attribute object used in the compute model: ``Attribute(local_id=..., label='some_label_id')``
-         - dict containing mapping of index name to label to use for indexing - specified in one of the ways list above
-
-        :param data_by: label, fact or metric to that will provide data (metric values or label elements); specify
-         either:
-
-         - object identifier: ``ObjId(id='some_id', type='<type>')`` - where type is either ``label``, ``fact``
-           or ``metric``
-         - string representation of object identifier: ``<type>/some_id`` - where type is either ``label``, ``fact`` or
-           ``metric``
-         - Attribute object used in the compute model: ``Attribute(local_id=..., label='some_label_id')``
-         - SimpleMetric object used in the compute model: ``SimpleMetric(local_id=..., item=..., aggregation=...)``
-
-        :param filter_by: optionally specify filter to apply during computation on the server, reference to filtering
-         column can be one of:
-
-         - string reference to index key
-         - object identifier in string form
-         - object identifier: ``ObjId(id='some_label_id', type='<type>')``
-         - Attribute or Metric depending on type of filter
+        Args:
+            index_by (IndexDef): label to index by; specify either:
 
-        :return: pandas series instance
+            - string with id: ``some_label_id``,
+            - object identifier: ``ObjId(id='some_label_id', type='label')``,
+            - string representation of object identifier: ``label/some_label_id``
+            - or an Attribute object used in the compute model: ``Attribute(local_id=..., label='some_label_id')``
+            - dict containing mapping of index name to label to use for indexing (in one of the ways listed above)
+
+            data_by (Union[SimpleMetric, str, ObjId, Attribute]): label, fact or metric to that will provide data
+              (metric values or label elements); specify either:
+
+            - object identifier: ``ObjId(id='some_id', type='<type>')`` - where type is either ``label``, ``fact``
+              or ``metric``
+            - string representation of object identifier: ``<type>/some_id`` - where type is either ``label``, ``fact``
+              or ``metric``
+            - Attribute object used in the compute model: ``Attribute(local_id=..., label='some_label_id')``
+            - SimpleMetric object used in the compute model: ``SimpleMetric(local_id=..., item=..., aggregation=...)``
+
+            filter_by (Optional[Union[Filter, list[Filter]]]): optionally specify filter to apply during computation on
+            the server, reference to filtering column can be one of:
+
+            - string reference to index key
+            - object identifier in string form
+            - object identifier: ``ObjId(id='some_label_id', type='<type>')``
+            - Attribute or Metric depending on type of filter
 
+        Returns:
+            pandas.Series: pandas series instance
         """
+
         data, index = compute_and_extract(
             self._sdk,
             self._workspace_id,
             index_by=index_by,
             columns={"_series": data_by},
             filter_by=filter_by,
         )
@@ -69,46 +80,41 @@
     def not_indexed(
         self,
         data_by: Union[SimpleMetric, str, ObjId, Attribute],
         granularity: Optional[Union[list[LabelItemDef], IndexDef]] = None,
         filter_by: Optional[Union[Filter, list[Filter]]] = None,
     ) -> pandas.Series:
         """
-        Creates pandas Series from data points calculated from a single `data_by` that will be computed on granularity
-        of the specified labels. No index will be constructed.
-
-        Note that data_by may also be a label in which case the Series will contain label elements.
-
-        :param data_by: label, fact or metric to get data from; specify either:
+        Creates a pandas.Series from data points calculated from a single `data_by` without constructing an index.
 
-         - object identifier: ``ObjId(id='some_id', type='<type>')`` - where type is either ``label``, ``fact``
-           or ``metric``
-         - string representation of object identifier: ``<type>/some_id`` - where type is either ``label``, ``fact`` or
-           ``metric``
-         - Attribute object used in the compute model: ``Attribute(local_id=..., label='some_label_id')``
-         - SimpleMetric object used in the compute model: ``SimpleMetric(local_id=..., item=..., aggregation=...)``
-
-        :param granularity: optionally specify label to slice the metric by; specify either:
-
-         - string with id: ``some_label_id``,
-         - object identifier: ``ObjId(id='some_label_id', type='label')``,
-         - string representation of object identifier: ``label/some_label_id``
-         - or an Attribute object used in the compute model: ``Attribute(local_id=..., label='some_label_id')``
-         - list containing multiple labels to slice the metric by - specified in one of the ways list above
-         - dict containing mapping of index name to label to use for indexing - specified in one of the ways list above;
-           this option is available so that you can easily switch from indexed factory method to this one if needed
-
-        :param filter_by: optionally specify filter to apply during computation on the server, reference to filtering
-         column can be one of:
-
-         - object identifier in string form
-         - object identifier: ``ObjId(id='some_label_id', type='<type>')``
-         - Attribute or Metric depending on type of filter
+        Args:
+            data_by (Union[SimpleMetric, str, ObjId, Attribute]): The label, fact, or metric to obtain data from.
+                Specify either:
+                    - ObjId: ObjId(id='some_id', type='<type>')
+                    - string representation of an identifier: '<type>/some_id'
+                    - Attribute: Attribute(local_id=..., label='some_label_id')
+                    - SimpleMetric: SimpleMetric(local_id=..., item=..., aggregation=...)
+            granularity (Optional[Union[list[LabelItemDef], IndexDef]], optional): The label to slice the metric by.
+                Specify either:
+                    - string with id: 'some_label_id'
+                    - ObjId: ObjId(id='some_label_id', type='label')
+                    - string representation of an identifier: 'label/some_label_id'
+                    - Attribute: Attribute(local_id=..., label='some_label_id')
+                    - list containing multiple labels to slice the metric by
+                    - dict containing mapping of index name to label
+                Defaults to None.
+            filter_by (Optional[Union[Filter, list[Filter]]], optional): The filter(s) to apply. Reference to filtering
+                column can be one of:
+                    - object identifier in string form
+                    - ObjId: ObjId(id='some_label_id', type='<type>')
+                    - Attribute or Metric depending on the type of filter
+                Defaults to None.
 
-        :return: pandas series instance
+        Returns:
+            pandas.Series: The resulting pandas Series instance.
         """
 
         if isinstance(granularity, list):
             _index: Optional[IndexDef] = {str(idx): label for idx, label in enumerate(granularity)}
         else:
             _index = granularity
```

### Comparing `gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/PKG-INFO` & `gooddata-pandas-1.4.0/gooddata_pandas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.3.1.dev5
+Version: 1.4.0
 Summary: GoodData.CN to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev5
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.4.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoodData Pandas
 
 This package contains a thin layer that utilizes gooddata-sdk and allows you to conveniently create pandas series and
 data frames from the computations done against semantic model in your [GoodData.CN](https://www.gooddata.com/developers/cloud-native/) workspace.
```

### Comparing `gooddata-pandas-1.3.1.dev5/setup.py` & `gooddata-pandas-1.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,45 +3,44 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.3.1.dev5",
+    "gooddata-sdk~=1.4.0",
     "pandas>=1.0.0,<2.0.0",
-    'importlib-metadata >= 1.0 ; python_version >= "3.7"',
 ]
 
 setup(
     name="gooddata-pandas",
     description="GoodData.CN to pandas",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.3.1.dev5",
+    version="1.4.0",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     project_urls={
-        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev5",
+        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.4.0",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Database",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development",
         "Typing :: Typed",
     ],
     keywords=[
         "gooddata",
```

