# Comparing `tmp/datapipe_core-0.13.0a6.tar.gz` & `tmp/datapipe_core-0.13.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.13.0a6.tar", max compression
+gzip compressed data, was "datapipe_core-0.13.0a7.tar", max compression
```

## Comparing `datapipe_core-0.13.0a6.tar` & `datapipe_core-0.13.0a7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a6/LICENSE
--rw-r--r--   0        0        0      779 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/README.md
--rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0a6/datapipe/__init__.py
--rw-r--r--   0        0        0    18265 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/cli.py
--rw-r--r--   0        0        0     9584 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/compute.py
--rw-r--r--   0        0        0    37210 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/core_steps.py
--rw-r--r--   0        0        0     6780 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/datatable.py
--rw-r--r--   0        0        0     4649 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/event_logger.py
--rw-r--r--   0        0        0     1562 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/executor/__init__.py
--rw-r--r--   0        0        0     1972 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/executor/ray.py
--rw-r--r--   0        0        0     4168 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/lints.py
--rw-r--r--   0        0        0    21906 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/metastore.py
--rw-r--r--   0        0        0      969 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/run_config.py
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a6/datapipe/store/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/store/database.py
--rw-r--r--   0        0        0    18238 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3595 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1337 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/pandas.py
--rw-r--r--   0        0        0     8674 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/qdrant.py
--rw-r--r--   0        0        0     3209 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/redis.py
--rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0a6/datapipe/store/table_store.py
--rw-r--r--   0        0        0     9945 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/types.py
--rw-r--r--   0        0        0     2145 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a7/LICENSE
+-rw-r--r--   0        0        0      779 2023-07-30 16:02:08.285417 datapipe_core-0.13.0a7/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0a7/datapipe/__init__.py
+-rw-r--r--   0        0        0    18038 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/cli.py
+-rw-r--r--   0        0        0     9520 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/compute.py
+-rw-r--r--   0        0        0    37412 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/core_steps.py
+-rw-r--r--   0        0        0     6780 2023-07-30 16:03:27.685421 datapipe_core-0.13.0a7/datapipe/datatable.py
+-rw-r--r--   0        0        0     4649 2023-07-30 16:03:31.215421 datapipe_core-0.13.0a7/datapipe/event_logger.py
+-rw-r--r--   0        0        0     1628 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/executor/__init__.py
+-rw-r--r--   0        0        0     2183 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/executor/ray.py
+-rw-r--r--   0        0        0     4236 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/lints.py
+-rw-r--r--   0        0        0    22222 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/metastore.py
+-rw-r--r--   0        0        0      969 2023-07-30 16:08:00.215417 datapipe_core-0.13.0a7/datapipe/run_config.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a7/datapipe/store/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/database.py
+-rw-r--r--   0        0        0    18238 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1337 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/pandas.py
+-rw-r--r--   0        0        0     8674 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/qdrant.py
+-rw-r--r--   0        0        0     3209 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0a7/datapipe/store/table_store.py
+-rw-r--r--   0        0        0     9945 2023-07-30 16:08:03.355417 datapipe_core-0.13.0a7/datapipe/types.py
+-rw-r--r--   0        0        0     2145 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0a7/PKG-INFO
```

### Comparing `datapipe_core-0.13.0a6/LICENSE` & `datapipe_core-0.13.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/README.md` & `datapipe_core-0.13.0a7/README.md`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/cli.py` & `datapipe_core-0.13.0a7/datapipe/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, ConsoleSpanExporter
 from rich import print as rprint
 from sqlalchemy import insert, literal
 from sqlalchemy.sql import and_, func, select
+from tqdm_loggable.auto import tqdm
 
 from datapipe.compute import ComputeStep, DatapipeApp, run_steps, run_steps_changelist
 from datapipe.core_steps import BaseBatchTransformStep
 from datapipe.executor import Executor, SingleThreadExecutor
 from datapipe.types import ChangeList, IndexDF, Labels
 
 tracer = trace.get_tracer("datapipe_app")
@@ -92,41 +93,51 @@
 @click.option("--trace-jaeger", is_flag=True, help="Enable tracing to Jaeger")
 @click.option(
     "--trace-jaeger-host", type=click.STRING, default="localhost", help="Jaeger host"
 )
 @click.option("--trace-jaeger-port", type=click.INT, default=14268, help="Jaeger port")
 @click.option("--trace-gcp", is_flag=True, help="Enable tracing to Google Cloud Trace")
 @click.option("--pipeline", type=click.STRING, default="app")
+@click.option("--executor", type=click.STRING, default="SingleThreadExecutor")
 @click.pass_context
 def cli(
     ctx: click.Context,
     debug: bool,
     debug_sql: bool,
     trace_stdout: bool,
     trace_jaeger: bool,
     trace_jaeger_host: str,
     trace_jaeger_port: int,
     trace_gcp: bool,
     pipeline: str,
+    executor: str,
 ) -> None:
-    import logging
+    ctx.ensure_object(dict)
 
-    if debug:
-        datapipe_logger = logging.getLogger("datapipe")
-        datapipe_logger.setLevel(logging.DEBUG)
+    def setup_logging():
+        import logging
 
-        datapipe_core_steps_logger = logging.getLogger("datapipe.core_steps")
-        datapipe_core_steps_logger.setLevel(logging.DEBUG)
+        if debug:
+            datapipe_logger = logging.getLogger("datapipe")
+            datapipe_logger.setLevel(logging.DEBUG)
 
-        logging.basicConfig(level=logging.DEBUG)
-    else:
-        logging.basicConfig(level=logging.INFO)
+            datapipe_core_steps_logger = logging.getLogger("datapipe.core_steps")
+            datapipe_core_steps_logger.setLevel(logging.DEBUG)
+
+            logging.basicConfig(level=logging.DEBUG, stream=sys.stderr)
+        else:
+            for logger_name in [None, "datapipe", "tqdm_loggable"]:
+                logger = logging.getLogger(logger_name)
+                logger.setLevel(logging.INFO)
+            logging.basicConfig(level=logging.INFO, stream=sys.stderr)
+
+        if debug_sql:
+            logging.getLogger("sqlalchemy.engine").setLevel(logging.INFO)
 
-    if debug_sql:
-        logging.getLogger("sqlalchemy.engine").setLevel(logging.INFO)
+    setup_logging()
 
     trace.set_tracer_provider(
         TracerProvider(resource=Resource.create({SERVICE_NAME: "datapipe"}))
     )
 
     SQLAlchemyInstrumentor().instrument()
 
@@ -159,15 +170,27 @@
         from opentelemetry.exporter.cloud_trace import CloudTraceSpanExporter
 
         cloud_trace_exporter = CloudTraceSpanExporter(
             resource_regex=r".*",
         )
         trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(cloud_trace_exporter))  # type: ignore
 
-    ctx.ensure_object(dict)
+    if executor == "SingleThreadExecutor":
+        ctx.obj["executor"] = SingleThreadExecutor
+    elif executor == "RayExecutor":
+        import ray
+
+        from datapipe.executor.ray import RayExecutor
+
+        ray_ctx = ray.init()
+
+        ctx.obj["executor"] = RayExecutor()
+    else:
+        raise ValueError(f"Unknown executor: {executor}")
+
     with tracer.start_as_current_span("init"):
         ctx.obj["pipeline"] = load_pipeline(pipeline)
 
 
 @cli.group()
 def table():
     pass
@@ -271,45 +294,27 @@
                 print()
             print()
 
 
 @cli.group()
 @click.option("--labels", type=click.STRING, default="")
 @click.option("--name", type=click.STRING, default="")
-@click.option("--executor", type=click.STRING, default="SingleThreadExecutor")
 @click.pass_context
 def step(
     ctx: click.Context,
     labels: str,
     name: str,
-    executor: str,
 ) -> None:
     app: DatapipeApp = ctx.obj["pipeline"]
 
-    labels_dict = parse_labels(labels)
-    steps = filter_steps_by_labels_and_name(app, labels=labels_dict, name_prefix=name)
+    labels_list = parse_labels(labels)
+    steps = filter_steps_by_labels_and_name(app, labels=labels_list, name_prefix=name)
 
     ctx.obj["steps"] = steps
 
-    if executor == "SingleThreadExecutor":
-        ctx.obj["executor"] = SingleThreadExecutor()
-    elif executor == "RayExecutor":
-        import ray
-
-        from datapipe.executor.ray import RayExecutor
-
-        ray_ctx = ray.init()
-
-        if hasattr(ctx, "dashboard_url"):
-            rprint(f"Dashboard URL: {ctx.dashboard_url}")
-
-        ctx.obj["executor"] = RayExecutor()
-    else:
-        raise ValueError(f"Unknown executor: {executor}")
-
 
 def to_human_repr(step: ComputeStep, extra_args: Optional[Dict] = None) -> str:
     res = []
 
     res.append(f"[green][bold]{step.name}[/bold][/green] ({step.__class__.__name__})")
 
     if step.labels:
@@ -405,70 +410,69 @@
 
 @step.command()  # type: ignore
 @click.option("--loop", is_flag=True, default=False, help="Run continuosly in a loop")
 @click.option(
     "--loop-delay", type=click.INT, default=1, help="Delay between loops in seconds"
 )
 @click.option("--chunk-size", type=click.INT, default=None, help="Chunk size")
+@click.option("--start-step", type=click.STRING)
 @click.pass_context
 def run_changelist(
-    ctx: click.Context, loop: bool, loop_delay: int, chunk_size: Optional[int] = None
+    ctx: click.Context,
+    start_step: str,
+    loop: bool,
+    loop_delay: int,
+    chunk_size: Optional[int] = None,
 ) -> None:
     app: DatapipeApp = ctx.obj["pipeline"]
+
+    start_step_objs = filter_steps_by_labels_and_name(
+        app, labels=[], name_prefix=start_step
+    )
+    assert len(start_step_objs) == 1
+
+    start_step_obj = start_step_objs[0]
+    assert isinstance(start_step_obj, BaseBatchTransformStep)
+
     steps_to_run: List[ComputeStep] = ctx.obj["steps"]
+
+    if start_step_obj not in steps_to_run:
+        steps_to_run = [start_step_obj] + steps_to_run
+
     steps_to_run_names = [f"'{i.name}'" for i in steps_to_run]
 
     print(f"Running following steps: {', '.join(steps_to_run_names)}")
 
-    idx_gen, cnt = None, None
+    executor: Executor = ctx.obj["executor"]()
+
+    idx_count, idx_gen = start_step_obj.get_full_process_ids(
+        app.ds,
+        chunk_size=chunk_size,
+    )
+    cnt = 0
+
     while True:
-        if len(steps_to_run) > 0:
-            step = steps_to_run[0]
-            assert isinstance(step, BaseBatchTransformStep)
+        for idx in tqdm(idx_gen, total=idx_count):
+            changes = start_step_obj.run_idx(
+                ds=app.ds,
+                idx=idx,
+                executor=executor,
+            )
+
+            run_steps_changelist(app.ds, steps_to_run, changes, executor=executor)
 
-            if idx_gen is None:
-                idx_count, idx_gen = step.get_full_process_ids(
-                    app.ds, chunk_size=chunk_size
-                )
-                cnt = 0
-            try:
-                idx = next(idx_gen)  # type: ignore
-                cl = ChangeList()
-                take_all_idxs = False
-                if all(
-                    [
-                        key not in input_dt.primary_keys
-                        for key in step.transform_keys
-                        for input_dt in steps_to_run[0].input_dts
-                    ]
-                ):
-                    take_all_idxs = True
-
-                for input_dt in step.input_dts:
-                    if not take_all_idxs and any(
-                        [key in input_dt.primary_keys for key in step.transform_keys]
-                    ):
-                        cl.append(
-                            input_dt.name, cast(IndexDF, input_dt.get_data(idx=idx))
-                        )
-
-                run_steps_changelist(app.ds, steps_to_run, cl)
-            except StopIteration:
-                idx_gen = None
-                cnt = 0
-        if idx_gen is not None and cnt is not None:
             rprint(f"Chunk {cnt}/{idx_count} ended")
             cnt += 1
+
+        if not loop:
+            break
         else:
-            if not loop:
-                break
-            else:
-                rprint(f"All chunks ended, sleeping {loop_delay}s...")
-                time.sleep(loop_delay)
-                print("\n\n")
+            rprint(f"All chunks ended, sleeping {loop_delay}s...")
+            time.sleep(loop_delay)
+            print("\n\n")
 
 
 @step.command()
 @click.pass_context
 def fill_metadata(ctx: click.Context) -> None:
     app: DatapipeApp = ctx.obj["pipeline"]
     steps_to_run: List[ComputeStep] = ctx.obj["steps"]
@@ -491,23 +495,14 @@
     print(f"Resetting following steps: {', '.join(steps_to_run_names)}")
 
     for step in steps_to_run:
         if isinstance(step, BaseBatchTransformStep):
             step.reset_metadata(app.ds)
 
 
-for entry_point in metadata.entry_points().get("datapipe.cli", []):
-    register_commands = entry_point.load()
-    register_commands(cli)
-
-
-def main():
-    cli(auto_envvar_prefix="DATAPIPE")
-
-
 @table.command()
 @click.pass_context
 @click.option("--name", type=click.STRING, default="")
 @click.option("--labels", type=click.STRING, default="")
 def migrate_transform_tables(ctx: click.Context, labels: str, name: str) -> None:
     app: DatapipeApp = ctx.obj["pipeline"]
     labels_dict = parse_labels(labels)
@@ -559,7 +554,20 @@
                 literal(True),
                 literal(None),
                 literal(0),
             ),
         )
         app.ds.meta_dbconn.con.execute(insert_stmt)
         rprint("  [green] ok[/green]")
+
+
+for entry_point in metadata.entry_points().get("datapipe.cli", []):
+    register_commands = entry_point.load()
+    register_commands(cli)
+
+
+def main():
+    cli(auto_envvar_prefix="DATAPIPE")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `datapipe_core-0.13.0a6/datapipe/compute.py` & `datapipe_core-0.13.0a7/datapipe/compute.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,14 +256,15 @@
 
 
 def run_steps_changelist(
     ds: DataStore,
     steps: List[ComputeStep],
     changelist: ChangeList,
     run_config: Optional[RunConfig] = None,
+    executor: Optional[Executor] = None,
 ) -> None:
     # FIXME extract Batch* steps to separate module
     from datapipe.core_steps import BaseBatchTransformStep
 
     current_changes = changelist
     next_changes = ChangeList()
     iteration = 0
@@ -277,20 +278,19 @@
                         f"{[i.name for i in step.input_dts]} -> {[i.name for i in step.output_dts]}"
                     ):
                         logger.info(
                             f"Running {step.get_name()} "
                             f"{[i.name for i in step.input_dts]} -> {[i.name for i in step.output_dts]}"
                         )
 
-                        try:
-                            if isinstance(step, BaseBatchTransformStep):
-                                step_changes = step.run_changelist(
-                                    ds, current_changes, run_config
-                                )
-                                next_changes.extend(step_changes)
-                        except NotImplementedError:
-                            # Some steps do not implement `.run_changelist`, that's ok
-                            pass
+                        if isinstance(step, BaseBatchTransformStep):
+                            step_changes = step.run_changelist(
+                                ds,
+                                current_changes,
+                                run_config,
+                                executor=executor,
+                            )
+                            next_changes.extend(step_changes)
 
             current_changes = next_changes
             next_changes = ChangeList()
             iteration += 1
```

### Comparing `datapipe_core-0.13.0a6/datapipe/core_steps.py` & `datapipe_core-0.13.0a7/datapipe/core_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,19 +571,21 @@
                         changes.append(table_changes_df)
                     else:
                         changes.append(data_to_index(idx, self.transform_keys))
 
             idx_df = pd.concat(changes).drop_duplicates(subset=self.transform_keys)
             idx = IndexDF(idx_df[self.transform_keys])
 
+            chunk_count = math.ceil(len(idx) / self.chunk_size)
+
             def gen():
-                for i in range(math.ceil(len(idx) / self.chunk_size)):
+                for i in range(chunk_count):
                     yield idx[i * self.chunk_size : (i + 1) * self.chunk_size]
 
-            return len(idx), gen()
+            return chunk_count, gen()
 
     def store_batch_result(
         self,
         ds: DataStore,
         idx: IndexDF,
         output_dfs: Optional[TransformResult],
         process_ts: float,
@@ -741,14 +743,15 @@
 
         logger.info(f"Batches to process {idx_count}")
 
         if idx_count is not None and idx_count == 0:
             return
 
         executor.run_process_batch(
+            name=self.name,
             ds=ds,
             idx_count=idx_count,
             idx_gen=idx_gen,
             process_fn=self.process_batch,
             run_config=run_config,
             executor_config=self.executor_config,
         )
@@ -761,44 +764,49 @@
         change_list: ChangeList,
         run_config: Optional[RunConfig] = None,
         executor: Optional[Executor] = None,
     ) -> ChangeList:
         if executor is None:
             executor = SingleThreadExecutor()
 
-        logger.info(f"Running: {self.name}")
         run_config = RunConfig.add_labels(run_config, {"step_name": self.name})
 
         (idx_count, idx_gen) = self.get_change_list_process_ids(
             ds, change_list, run_config
         )
 
         logger.info(f"Batches to process {idx_count}")
 
         if idx_count is not None and idx_count == 0:
             return ChangeList()
 
-        res_changelist = ChangeList()
+        logger.info(f"Running: {self.name}")
 
-        for idx in tqdm(idx_gen, total=idx_count):
-            changes = self.process_batch(
-                ds=ds,
-                idx=idx,
-                run_config=run_config,
-            )
-            res_changelist.extend(changes)
+        changes = executor.run_process_batch(
+            name=self.name,
+            ds=ds,
+            idx_count=idx_count,
+            idx_gen=idx_gen,
+            process_fn=self.process_batch,
+            run_config=run_config,
+            executor_config=self.executor_config,
+        )
 
-        return res_changelist
+        return changes
 
     def run_idx(
         self,
         ds: DataStore,
         idx: IndexDF,
         run_config: Optional[RunConfig] = None,
+        executor: Optional[Executor] = None,
     ) -> ChangeList:
+        if executor is None:
+            executor = SingleThreadExecutor()
+
         logger.info(f"Running: {self.name}")
         run_config = RunConfig.add_labels(run_config, {"step_name": self.name})
 
         return self.process_batch(
             ds=ds,
             idx=idx,
             run_config=run_config,
```

### Comparing `datapipe_core-0.13.0a6/datapipe/datatable.py` & `datapipe_core-0.13.0a7/datapipe/datatable.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/event_logger.py` & `datapipe_core-0.13.0a7/datapipe/event_logger.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/executor/__init__.py` & `datapipe_core-0.13.0a7/datapipe/executor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,32 +21,36 @@
 
 @dataclass
 class ExecutorConfig:
     memory: Optional[int] = None
     cpu: Optional[float] = None
     gpu: Optional[int] = None
 
+    parallelism: int = 100
+
 
 class Executor(ABC):
     @abstractmethod
     def run_process_batch(
         self,
+        name: str,
         ds: DataStore,
         idx_count: int,
         idx_gen: Iterable[IndexDF],
         process_fn: ProcessFn,
         run_config: Optional[RunConfig] = None,
         executor_config: Optional[ExecutorConfig] = None,
     ) -> ChangeList:
         ...
 
 
 class SingleThreadExecutor(Executor):
     def run_process_batch(
         self,
+        name: str,
         ds: DataStore,
         idx_count: int,
         idx_gen: Iterable[IndexDF],
         process_fn: ProcessFn,
         run_config: Optional[RunConfig] = None,
         executor_config: Optional[ExecutorConfig] = None,
     ) -> ChangeList:
```

### Comparing `datapipe_core-0.13.0a6/datapipe/executor/ray.py` & `datapipe_core-0.13.0a7/datapipe/executor/ray.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,66 @@
+from functools import wraps
 from typing import Any, Dict, Iterable, Optional
 
 import ray
 from tqdm_loggable.auto import tqdm
 
 from datapipe.datatable import DataStore
 from datapipe.executor import Executor, ExecutorConfig, ProcessFn
 from datapipe.run_config import RunConfig
 from datapipe.types import ChangeList, IndexDF
 
 
 class RayExecutor(Executor):
     def run_process_batch(
         self,
+        name: str,
         ds: DataStore,
         idx_count: int,
         idx_gen: Iterable[IndexDF],
         process_fn: ProcessFn,
         run_config: Optional[RunConfig] = None,
         executor_config: Optional[ExecutorConfig] = None,
     ) -> ChangeList:
         res_changelist = ChangeList()
 
-        remote_kwargs: Dict[str, Any] = {}
+        remote_kwargs: Dict[str, Any] = {
+            "name": name,
+        }
 
         if executor_config is not None:
             if executor_config.memory is not None:
                 remote_kwargs["memory"] = executor_config.memory
             if executor_config.cpu is not None:
                 remote_kwargs["num_cpus"] = executor_config.cpu
 
-        if remote_kwargs:
-
-            @ray.remote(**remote_kwargs)
-            def process_fn_remote(ds, idx, run_config):
-                return process_fn(ds, idx, run_config)
-
+            parallelism = executor_config.parallelism
         else:
+            parallelism = 10
 
-            @ray.remote
-            def process_fn_remote(ds, idx, run_config):
-                return process_fn(ds, idx, run_config)
-
-        # Submit tasks to remote functions using Ray
-        futures = []
-        for idx in idx_gen:
-            future = process_fn_remote.remote(ds, idx, run_config)
-            futures.append(future)
+        @ray.remote(**remote_kwargs)
+        def process_fn_remote(ds, idx, run_config):
+            return process_fn(ds, idx, run_config)
 
         # Generator to collect results, so tqdm can show progress
-        def _results(futures):
+        def _results(idx_gen):
+            # Submit tasks to remote functions using Ray
+            futures = []
+            for idx in idx_gen:
+                if len(futures) > parallelism:
+                    ready, futures = ray.wait(futures, timeout=None)
+                    for result in ray.get(ready):
+                        yield result
+
+                future = process_fn_remote.remote(ds, idx, run_config)
+                futures.append(future)
+
             ready, futures = ray.wait(futures, timeout=None)
             while len(ready) > 0:
                 for result in ray.get(ready):
                     yield result
                 ready, futures = ray.wait(futures, timeout=None)
 
-        for result in tqdm(_results(futures), total=len(futures)):
+        for result in tqdm(_results(idx_gen), total=idx_count):
             res_changelist.extend(result)
 
         return res_changelist
```

### Comparing `datapipe_core-0.13.0a6/datapipe/lints.py` & `datapipe_core-0.13.0a7/datapipe/lints.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
     def check(self, dt: DataTable) -> Tuple[LintStatus, Optional[str]]:
         query = self.check_query(dt)
 
         if query is None:
             return (LintStatus.SKIP, None)
 
-        (cnt,) = dt.meta_table.dbconn.con.execute(query).fetchone()
+        res = dt.meta_table.dbconn.con.execute(query).fetchone()
+
+        assert res is not None and len(res) == 1
+        (cnt,) = res
 
         if cnt == 0:
             return (LintStatus.OK, None)
         else:
             return (LintStatus.FAIL, f"{cnt} rows")
 
     def check_query(self, dt: DataTable):
```

### Comparing `datapipe_core-0.13.0a6/datapipe/metastore.py` & `datapipe_core-0.13.0a7/datapipe/metastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import logging
 import math
 import time
 from dataclasses import dataclass
-from typing import Iterator, List, Optional, Tuple, cast
+from typing import Any, Iterator, List, Optional, Tuple, cast
 
 import pandas as pd
 from cityhash import CityHash32
 from sqlalchemy import Boolean, Column, Float, Integer, String, Table, func, update
 from sqlalchemy.sql.expression import and_, delete, or_, select, text, tuple_
 
 from datapipe.run_config import RunConfig
@@ -149,15 +149,15 @@
                 res.append(pd.read_sql_query(chunk_sql, con=con))
 
             if len(res) > 0:
                 return cast(MetadataDF, pd.concat(res))
             else:
                 return cast(
                     MetadataDF,
-                    pd.DataFrame(columns=[column.name for column in self.sql_schema]),
+                    pd.DataFrame(columns=[column.name for column in self.sql_schema]),  # type: ignore
                 )
 
     def get_metadata_size(
         self, idx: Optional[IndexDF] = None, include_deleted: bool = False
     ) -> int:
         """
         Получить количество строк метаданных.
@@ -167,14 +167,16 @@
         """
 
         sql = select([func.count()]).select_from(self.sql_table)
         sql = self._build_metadata_query(sql, idx, include_deleted)
 
         with self.dbconn.con.begin() as con:
             res = con.execute(sql).fetchone()
+
+            assert res is not None and len(res) == 1
             return res[0]
 
     def _make_new_metadata_df(self, now: float, df: DataDF) -> MetadataDF:
         meta_keys = self.primary_keys + list(self.meta_keys.values())
         res_df = df[meta_keys]
 
         res_df = res_df.assign(
@@ -210,15 +212,15 @@
         sql = select(self.sql_schema)
 
         if idx is not None:
             if len(idx.index) == 0:
                 # Empty index -> empty result
                 return cast(
                     IndexDF,
-                    pd.DataFrame(columns=[column.name for column in self.sql_schema]),
+                    pd.DataFrame(columns=[column.name for column in self.sql_schema]),  # type: ignore
                 )
             idx_cols = list(set(idx.columns.tolist()) & set(self.primary_keys))
         else:
             idx_cols = []
 
         if len(idx_cols) > 0:
             row_queries = []
@@ -244,19 +246,22 @@
                 con=con,
             )
 
         return data_to_index(res_df, self.primary_keys)
 
     def get_table_debug_info(self) -> TableDebugInfo:
         with self.dbconn.con.begin() as con:
+            res = con.execute(
+                select([func.count()]).select_from(self.sql_table)
+            ).fetchone()
+
+            assert res is not None and len(res) == 1
             return TableDebugInfo(
                 name=self.name,
-                size=con.execute(
-                    select([func.count()]).select_from(self.sql_table)
-                ).fetchone()[0],
+                size=res[0],
             )
 
     # TODO Может быть переделать работу с метадатой на контекстный менеджер?
     # FIXME поправить возвращаемые структуры данных, _meta_df должны содержать только _meta колонки
     def get_changes_for_store_chunk(
         self, data_df: DataDF, now: Optional[float] = None
     ) -> Tuple[DataDF, DataDF, MetadataDF, MetadataDF]:
@@ -334,15 +339,15 @@
                     name=self.sql_table.name,
                     con=con,
                     schema=self.dbconn.schema,
                     if_exists="append",
                     index=False,
                     chunksize=1000,
                     method="multi",
-                    dtype=sql_schema_to_sqltype(self.sql_schema),
+                    dtype=sql_schema_to_sqltype(self.sql_schema),  # type: ignore
                 )
 
     def _delete_rows(self, df: MetadataDF) -> None:
         if len(df) == 0:
             return
 
         idx = df[self.primary_keys]
@@ -354,15 +359,17 @@
                 key = self.primary_keys[0]
                 chunk_sql = sql.where(
                     self.sql_table.c[key].in_(chunk_idx[key].to_list())
                 )
 
             else:
                 # Когда ключей много - сравниваем через tuple
-                keys = tuple_(*[self.sql_table.c[key] for key in self.primary_keys])
+                keys: Any = tuple_(
+                    *[self.sql_table.c[key] for key in self.primary_keys]
+                )
 
                 chunk_sql = sql.where(
                     keys.in_(
                         [
                             tuple([r[key] for key in self.primary_keys])  # type: ignore
                             for r in chunk_idx.to_dict(orient="records")
                         ]
@@ -378,15 +385,15 @@
 
         table = (
             f"{self.dbconn.schema}.{self.sql_table.name}"
             if self.dbconn.schema
             else self.sql_table.name
         )
         values_table = f"{self.sql_table.name}_values"
-        columns = [column.name for column in self.sql_schema]
+        columns = [column.name for column in self.sql_schema]  # type: ignore
         update_columns = set(columns) - set(self.primary_keys)
 
         update_expression = ", ".join(
             [f"{column}={values_table}.{column}" for column in update_columns]
         )
 
         where_expressiom = " AND ".join(
@@ -396,15 +403,15 @@
         for chunk_df in self._chunk_idx_df(df):
             params_df = chunk_df.reset_index()[columns]
             values_params = []
             params = {}
 
             for index, row in params_df.iterrows():
                 row_values = [
-                    f"CAST(:{column.name}_{index} AS {column.type})"
+                    f"CAST(:{column.name}_{index} AS {column.type})"  # type: ignore
                     for column in self.sql_schema
                 ]
                 row_params = {f"{key}_{index}": row[key] for key in row.keys()}
 
                 values_params.append(f'({", ".join(row_values)})')
                 params.update(row_params)
 
@@ -495,15 +502,15 @@
         create_table: bool = False,
     ) -> None:
         self.dbconn = dbconn
         self.name = name
         self.primary_schema = primary_schema
         self.primary_keys = [i.name for i in primary_schema]
 
-        self.sql_schema = [i.copy() for i in primary_schema + TRANSFORM_META_SCHEMA]
+        self.sql_schema = [i.copy() for i in primary_schema + TRANSFORM_META_SCHEMA]  # type: ignore
 
         self.sql_table = Table(
             name,
             dbconn.sqla_metadata,
             *self.sql_schema,
         )
 
@@ -615,14 +622,16 @@
     def get_metadata_size(self) -> int:
         """
         Получить количество строк метаданных трансформации.
         """
 
         sql = select([func.count()]).select_from(self.sql_table)
         res = self.dbconn.con.execute(sql).fetchone()
+
+        assert res is not None and len(res) == 1
         return res[0]
 
     def mark_all_rows_unprocessed(
         self,
         run_config: Optional[RunConfig] = None,
     ) -> None:
         update_sql = (
```

### Comparing `datapipe_core-0.13.0a6/datapipe/run_config.py` & `datapipe_core-0.13.0a7/datapipe/run_config.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/store/database.py` & `datapipe_core-0.13.0a7/datapipe/store/database.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/store/filedir.py` & `datapipe_core-0.13.0a7/datapipe/store/filedir.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/store/milvus.py` & `datapipe_core-0.13.0a7/datapipe/store/milvus.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/store/pandas.py` & `datapipe_core-0.13.0a7/datapipe/store/pandas.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/store/qdrant.py` & `datapipe_core-0.13.0a7/datapipe/store/qdrant.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/store/redis.py` & `datapipe_core-0.13.0a7/datapipe/store/redis.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/store/table_store.py` & `datapipe_core-0.13.0a7/datapipe/store/table_store.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/datapipe/types.py` & `datapipe_core-0.13.0a7/datapipe/types.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a6/pyproject.toml` & `datapipe_core-0.13.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.13.0-alpha.6"
+version = "0.13.0-alpha.7"
 description = "`datapipe` is a realtime incremental ETL library for Python application"
 readme = "README.md"
 repository = "https://github.com/epoch8/datapipe"
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
```

### Comparing `datapipe_core-0.13.0a6/PKG-INFO` & `datapipe_core-0.13.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.13.0a6
+Version: 0.13.0a7
 Summary: `datapipe` is a realtime incremental ETL library for Python application
 Home-page: https://github.com/epoch8/datapipe
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

