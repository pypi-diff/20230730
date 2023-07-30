# Comparing `tmp/dimits-0.0.21a0.tar.gz` & `tmp/dimits-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimits-0.0.21a0.tar", max compression
+gzip compressed data, was "dimits-0.0.2a0.tar", max compression
```

## Comparing `dimits-0.0.21a0.tar` & `dimits-0.0.2a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      164 2023-07-30 07:02:38.458229 dimits-0.0.21a0/dimits/__init__.py
--rw-r--r--   0        0        0     8114 2023-07-29 15:52:47.945568 dimits-0.0.21a0/dimits/main.py
--rw-r--r--   0        0        0     6104 2023-07-29 15:49:49.628760 dimits-0.0.21a0/dimits/ttsmodel.py
--rw-r--r--   0        0        0     2056 2023-07-06 10:19:58.221599 dimits-0.0.21a0/dimits/utils.py
--rw-r--r--   0        0        0     1079 2023-06-28 10:26:13.254270 dimits-0.0.21a0/LICENSE
--rw-r--r--   0        0        0      750 2023-07-30 07:02:51.927471 dimits-0.0.21a0/pyproject.toml
--rw-r--r--   0        0        0     2843 2023-07-29 14:58:34.457187 dimits-0.0.21a0/README.md
--rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 dimits-0.0.21a0/PKG-INFO
+-rw-r--r--   0        0        0      163 2023-07-29 15:53:03.793881 dimits-0.0.2a0/dimits/__init__.py
+-rw-r--r--   0        0        0     8114 2023-07-29 15:52:47.945568 dimits-0.0.2a0/dimits/main.py
+-rw-r--r--   0        0        0     6104 2023-07-29 15:49:49.628760 dimits-0.0.2a0/dimits/ttsmodel.py
+-rw-r--r--   0        0        0     2056 2023-07-06 10:19:58.221599 dimits-0.0.2a0/dimits/utils.py
+-rw-r--r--   0        0        0     1079 2023-06-28 10:26:13.254270 dimits-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0      711 2023-07-29 15:56:45.375138 dimits-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2843 2023-07-29 14:58:34.457187 dimits-0.0.2a0/README.md
+-rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 dimits-0.0.2a0/PKG-INFO
```

### Comparing `dimits-0.0.21a0/dimits/main.py` & `dimits-0.0.2a0/dimits/main.py`

 * *Files identical despite different names*

### Comparing `dimits-0.0.21a0/dimits/ttsmodel.py` & `dimits-0.0.2a0/dimits/ttsmodel.py`

 * *Files identical despite different names*

### Comparing `dimits-0.0.21a0/dimits/utils.py` & `dimits-0.0.2a0/dimits/utils.py`

 * *Files identical despite different names*

### Comparing `dimits-0.0.21a0/LICENSE` & `dimits-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dimits-0.0.21a0/pyproject.toml` & `dimits-0.0.2a0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "dimits"
-version = "0.0.21-alpha"
+version = "0.0.2-alpha"
 description = "Dimits is a Python library that provides an easy-to-use interface to the Piper text-to-speech (TTS) system. It utilizes the powerful Piper TTS engine, which is optimized for Raspberry Pi 4, to generate high-quality synthesized speech."
 authors = ["Reqeique <ananiyajemberu21@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "Dimits"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = { version = "^2.13.0", source = "private" }
-espeak-phonemizer = { version = "*"}
 espeak-phonemizer-windows = { version = "*", platform = "win32" }
 tqdm = "4.64.0" 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dimits-0.0.21a0/README.md` & `dimits-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `dimits-0.0.21a0/PKG-INFO` & `dimits-0.0.2a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dimits
-Version: 0.0.21a0
+Version: 0.0.2a0
 Summary: Dimits is a Python library that provides an easy-to-use interface to the Piper text-to-speech (TTS) system. It utilizes the powerful Piper TTS engine, which is optimized for Raspberry Pi 4, to generate high-quality synthesized speech.
 License: MIT
 Author: Reqeique
 Author-email: ananiyajemberu21@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: espeak-phonemizer
 Requires-Dist: espeak-phonemizer-windows ; sys_platform == "win32"
 Requires-Dist: requests (>=2.13.0,<3.0.0)
 Requires-Dist: tqdm (==4.64.0)
 Description-Content-Type: text/markdown
 
 
 # **Dimits - Python Bindings for Piper TTS**
```

