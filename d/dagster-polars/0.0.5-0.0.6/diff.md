# Comparing `tmp/dagster_polars-0.0.5.tar.gz` & `tmp/dagster_polars-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.0.5.tar", max compression
+gzip compressed data, was "dagster_polars-0.0.6.tar", max compression
```

## Comparing `dagster_polars-0.0.5.tar` & `dagster_polars-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11344 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/LICENSE
--rw-r--r--   0        0        0     3882 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/README.md
--rw-r--r--   0        0        0      358 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/__init__.py
--rw-r--r--   0        0        0       76 2023-07-06 11:37:09.484852 dagster_polars-0.0.5/dagster_polars/_version.py
--rw-r--r--   0        0        0        0 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0     5195 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     7200 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/bigquery.py
--rw-r--r--   0        0        0     4593 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/delta.py
--rw-r--r--   0        0        0     2143 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0     3936 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/py.typed
--rw-r--r--   0        0        0     2878 2023-07-06 11:37:09.484852 dagster_polars-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 dagster_polars-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3911 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/README.md
+-rw-r--r--   0        0        0      415 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-30 21:04:40.356696 dagster_polars-0.0.6/dagster_polars/_version.py
+-rw-r--r--   0        0        0        0 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0     5195 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     7200 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/bigquery.py
+-rw-r--r--   0        0        0     5027 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/delta.py
+-rw-r--r--   0        0        0     2143 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0     3936 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/utils.py
+-rw-r--r--   0        0        0        0 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/py.typed
+-rw-r--r--   0        0        0     2878 2023-07-30 21:04:40.356696 dagster_polars-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5250 1970-01-01 00:00:00.000000 dagster_polars-0.0.6/PKG-INFO
```

### Comparing `dagster_polars-0.0.5/LICENSE` & `dagster_polars-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.5/README.md` & `dagster_polars-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
-     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`. **Warning** [doesn't work good](https://github.com/pola-rs/polars/issues/9635) on MacOS
+     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `mode`, `overwrite_schema` and `version` can be set via config parameters. `partition_by` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). The IOManager won't manage partitioning in this case, and all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
  - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
 
 ## Quickstart
 
 ### Installation
 
 ```shell
```

### Comparing `dagster_polars-0.0.5/dagster_polars/io_managers/base.py` & `dagster_polars-0.0.6/dagster_polars/io_managers/base.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.5/dagster_polars/io_managers/bigquery.py` & `dagster_polars-0.0.6/dagster_polars/io_managers/bigquery.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.5/dagster_polars/io_managers/delta.py` & `dagster_polars-0.0.6/dagster_polars/io_managers/delta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,38 @@
+from enum import Enum
 from pprint import pformat
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
 import polars as pl
 from dagster import InputContext, MetadataValue, OutputContext
 from deltalake import DeltaTable
 from upath import UPath
 
 from dagster_polars.io_managers.base import BasePolarsUPathIOManager
 
 
+class DeltaWriteMode(str, Enum):
+    error = "error"
+    append = "append"
+    overwrite = "overwrite"
+    ignore = "ignore"
+
+
 class PolarsDeltaIOManager(BasePolarsUPathIOManager):
     extension: str = ".delta"
+    mode: DeltaWriteMode = DeltaWriteMode.overwrite.value  # type: ignore
+    overwrite_schema: bool = False
+    version: Optional[int] = None
 
     assert BasePolarsUPathIOManager.__doc__ is not None
     __doc__ = (
         BasePolarsUPathIOManager.__doc__
         + """\nWorks with Delta files.
-    All read/write arguments can be passed via corresponding metadata values."""
+    All read/write arguments can be passed via corresponding metadata values.
+    Metadata values take precedence over config parameters."""  # TODO: should this be opposite?
     )
 
     def dump_df_to_path(self, context: OutputContext, df: pl.DataFrame, path: UPath):
         assert context.metadata is not None
 
         delta_write_options = context.metadata.get("delta_write_options")
 
@@ -34,28 +46,28 @@
         if delta_write_options is not None:
             context.log.debug(f"Writing with delta_write_options: {pformat(delta_write_options)}")
 
         storage_options = self.get_storage_options(path)
 
         df.write_delta(
             str(path),
-            mode=context.metadata.get("mode", "overwrite"),  # type: ignore
-            overwrite_schema=context.metadata.get("overwrite_schema", False),
+            mode=context.metadata.get("mode", self.mode),  # type: ignore
+            overwrite_schema=context.metadata.get("overwrite_schema", self.overwrite_schema),
             storage_options=storage_options,
             delta_write_options=delta_write_options,
         )
         table = DeltaTable(str(path), storage_options=storage_options)
         context.add_output_metadata({"version": table.version()})
 
     def scan_df_from_path(self, path: UPath, context: InputContext) -> pl.LazyFrame:
         assert context.metadata is not None
 
         return pl.scan_delta(
             str(path),
-            version=context.metadata.get("version"),
+            version=context.metadata.get("version") or self.version or None,
             delta_table_options=context.metadata.get("delta_table_options"),
             pyarrow_options=context.metadata.get("pyarrow_options"),
             storage_options=self.get_storage_options(path),
         )
 
     def get_path_for_partition(self, context: Union[InputContext, OutputContext], path: UPath, partition: str) -> UPath:
         if isinstance(context, InputContext):
```

### Comparing `dagster_polars-0.0.5/dagster_polars/io_managers/parquet.py` & `dagster_polars-0.0.6/dagster_polars/io_managers/parquet.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.5/dagster_polars/io_managers/utils.py` & `dagster_polars-0.0.6/dagster_polars/io_managers/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.5/pyproject.toml` & `dagster_polars-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.0.5"
+version = "0.0.6"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
```

### Comparing `dagster_polars-0.0.5/PKG-INFO` & `dagster_polars-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -39,15 +39,15 @@
  - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
-     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`. **Warning** [doesn't work good](https://github.com/pola-rs/polars/issues/9635) on MacOS
+     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `mode`, `overwrite_schema` and `version` can be set via config parameters. `partition_by` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). The IOManager won't manage partitioning in this case, and all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
  - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
 
 ## Quickstart
 
 ### Installation
 
 ```shell
```

