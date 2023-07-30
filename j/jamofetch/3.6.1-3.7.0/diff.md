# Comparing `tmp/jamofetch-3.6.1.tar.gz` & `tmp/jamofetch-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamofetch-3.6.1.tar", max compression
+gzip compressed data, was "jamofetch-3.7.0.tar", max compression
```

## Comparing `jamofetch-3.6.1.tar` & `jamofetch-3.7.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4675 2023-07-27 23:09:54.226061 jamofetch-3.6.1/README.md
--rw-r--r--   0        0        0      522 2023-07-27 23:44:36.482154 jamofetch-3.6.1/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-27 23:09:54.227061 jamofetch-3.6.1/src/jamofetch/__init__.py
--rwxr-xr-x   0        0        0    10932 2023-07-27 23:09:54.227061 jamofetch-3.6.1/src/jamofetch/jamofetch.py
--rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4675 2023-07-27 23:09:54.226061 jamofetch-3.7.0/README.md
+-rw-r--r--   0        0        0      522 2023-07-30 20:05:03.823308 jamofetch-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-27 23:09:54.227061 jamofetch-3.7.0/src/jamofetch/__init__.py
+-rwxr-xr-x   0        0        0    10931 2023-07-30 20:05:03.823308 jamofetch-3.7.0/src/jamofetch/jamofetch.py
+-rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.7.0/PKG-INFO
```

### Comparing `jamofetch-3.6.1/README.md` & `jamofetch-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `jamofetch-3.6.1/pyproject.toml` & `jamofetch-3.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jamofetch"
-version = "3.6.1"
+version = "3.7.0"
 description = "A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori."
 authors = ["Duncan Scott"]
 license = "None"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `jamofetch-3.6.1/src/jamofetch/jamofetch.py` & `jamofetch-3.7.0/src/jamofetch/jamofetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,22 @@
 import time
 from argparse import ArgumentParser
 from stat import ST_CTIME
 
 JAMO_CMD_NERSC = 'module load jamo; jamo link library'
 JAMO_CMD_DORI = 'apptainer --silent run docker://doejgi/jamo-dori jamo link -s dori library'
 
-TWO_HOURS = 7200
-ONE_MINUTE = 60
+TWO_HOURS = 7200  # seconds
+ONE_MINUTE = 60   # seconds
+
+
+def _get_cmd(clean_lib_name) -> str:
+    if os.getenv('SLURM_PARTITION') == 'dori':
+        return f"{JAMO_CMD_DORI} {clean_lib_name}"
+    return f"{JAMO_CMD_NERSC} {clean_lib_name}"
 
 
 def _clean_library_name(library_name):
     clean_name = f"{library_name}".strip()
     if not re.match(r'^[A-Z]+$', clean_name):
         raise ValueError(f"invalid library name {library_name}")
     return clean_name
@@ -153,29 +159,24 @@
 
 class JamoFetcher():
     def __init__(self, link_dir='.', wait_interval_secs=10, wait_max_secs=-1):
         self._wait_interval_secs = _check_int_not_negative(wait_interval_secs, 'wait_interval_secs')
         self._wait_max_secs = _check_int_not_negative(wait_max_secs, 'wait_max_secs', allow_minus_1=True)
         self._link_dir = os.path.realpath(link_dir)
 
-    def get_cmd(self, clean_lib_name) -> str:
-        if os.getenv('SLURM_PARTITION') == 'dori':
-            return f"{JAMO_CMD_DORI} {clean_lib_name}"
-        return f"{JAMO_CMD_NERSC} {clean_lib_name}"
-
     def fetch_lib_seq(self, lib_name, out_file=sys.stderr) -> JamoLibSeq:
         """
         Execute JAMO command to link sequence for library
         and return a LibSeq object containing the path to the sequence.
         """
         pathlib.Path(self._link_dir).mkdir(parents=True, exist_ok=True, mode=0o775)
         os.chdir(self._link_dir)
         clean_lib_name = _clean_library_name(lib_name)
 
-        cmd = self.get_cmd(clean_lib_name)
+        cmd = _get_cmd(clean_lib_name)
         print(cmd, file=out_file)
         output = subprocess.check_output(cmd, shell=True)
         for line in output.splitlines():
             print(line.decode("utf-8"), file=out_file)
         seq_path = _find_fastq_path(clean_lib_name, self._link_dir)
         print(f"{clean_lib_name} {seq_path}", file=out_file)
         return JamoLibSeq(clean_lib_name, seq_path, self._wait_interval_secs, self._wait_max_secs)
```

### Comparing `jamofetch-3.6.1/PKG-INFO` & `jamofetch-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamofetch
-Version: 3.6.1
+Version: 3.7.0
 Summary: A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori.
 License: None
 Author: Duncan Scott
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

