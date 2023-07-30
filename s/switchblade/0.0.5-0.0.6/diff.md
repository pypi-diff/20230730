# Comparing `tmp/switchblade-0.0.5.tar.gz` & `tmp/switchblade-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switchblade-0.0.5.tar", last modified: Sun Jul 30 01:02:03 2023, max compression
+gzip compressed data, was "switchblade-0.0.6.tar", last modified: Sun Jul 30 02:50:36 2023, max compression
```

## Comparing `switchblade-0.0.5.tar` & `switchblade-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.286813 switchblade-0.0.5/
--rw-r--r--   0 oriyonay   (501) staff       (20)     1066 2023-07-30 01:00:20.000000 switchblade-0.0.5/LICENSE
--rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-30 01:02:03.286475 switchblade-0.0.5/PKG-INFO
--rw-r--r--   0 oriyonay   (501) staff       (20)      177 2023-07-30 01:00:20.000000 switchblade-0.0.5/README.md
--rw-r--r--   0 oriyonay   (501) staff       (20)      590 2023-07-30 01:01:16.000000 switchblade-0.0.5/pyproject.toml
--rw-r--r--   0 oriyonay   (501) staff       (20)       38 2023-07-30 01:02:03.286940 switchblade-0.0.5/setup.cfg
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.278543 switchblade-0.0.5/src/
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.282289 switchblade-0.0.5/src/switchblade/
--rw-r--r--   0 oriyonay   (501) staff       (20)        4 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/__init__.py
--rw-r--r--   0 oriyonay   (501) staff       (20)      425 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/debugging.py
--rw-r--r--   0 oriyonay   (501) staff       (20)      540 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/logging.py
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.286087 switchblade-0.0.5/src/switchblade/modules/
--rw-r--r--   0 oriyonay   (501) staff       (20)     3747 2023-07-29 23:03:04.000000 switchblade-0.0.5/src/switchblade/modules/ResNetIA.py
--rw-r--r--   0 oriyonay   (501) staff       (20)       30 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/modules/__init__.py
--rw-r--r--   0 oriyonay   (501) staff       (20)     2550 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/utils.py
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.285339 switchblade-0.0.5/src/switchblade.egg-info/
--rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/PKG-INFO
--rw-r--r--   0 oriyonay   (501) staff       (20)      369 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/SOURCES.txt
--rw-r--r--   0 oriyonay   (501) staff       (20)        1 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/dependency_links.txt
--rw-r--r--   0 oriyonay   (501) staff       (20)       12 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/top_level.txt
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 02:50:36.372202 switchblade-0.0.6/
+-rw-r--r--   0 oriyonay   (501) staff       (20)     1066 2023-07-30 01:00:20.000000 switchblade-0.0.6/LICENSE
+-rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-30 02:50:36.371926 switchblade-0.0.6/PKG-INFO
+-rw-r--r--   0 oriyonay   (501) staff       (20)      177 2023-07-30 01:00:20.000000 switchblade-0.0.6/README.md
+-rw-r--r--   0 oriyonay   (501) staff       (20)      590 2023-07-30 02:48:37.000000 switchblade-0.0.6/pyproject.toml
+-rw-r--r--   0 oriyonay   (501) staff       (20)       38 2023-07-30 02:50:36.372303 switchblade-0.0.6/setup.cfg
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 02:50:36.364042 switchblade-0.0.6/src/
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 02:50:36.369375 switchblade-0.0.6/src/switchblade/
+-rw-r--r--   0 oriyonay   (501) staff       (20)        4 2023-07-30 01:00:20.000000 switchblade-0.0.6/src/switchblade/__init__.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)      425 2023-07-30 01:00:20.000000 switchblade-0.0.6/src/switchblade/debugging.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)      540 2023-07-30 01:00:20.000000 switchblade-0.0.6/src/switchblade/logging.py
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 02:50:36.371483 switchblade-0.0.6/src/switchblade/modules/
+-rw-r--r--   0 oriyonay   (501) staff       (20)     3747 2023-07-30 02:46:23.000000 switchblade-0.0.6/src/switchblade/modules/ResNetIA.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)       30 2023-07-30 01:00:20.000000 switchblade-0.0.6/src/switchblade/modules/__init__.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)     2550 2023-07-30 01:00:20.000000 switchblade-0.0.6/src/switchblade/utils.py
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 02:50:36.370770 switchblade-0.0.6/src/switchblade.egg-info/
+-rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-30 02:50:36.000000 switchblade-0.0.6/src/switchblade.egg-info/PKG-INFO
+-rw-r--r--   0 oriyonay   (501) staff       (20)      369 2023-07-30 02:50:36.000000 switchblade-0.0.6/src/switchblade.egg-info/SOURCES.txt
+-rw-r--r--   0 oriyonay   (501) staff       (20)        1 2023-07-30 02:50:36.000000 switchblade-0.0.6/src/switchblade.egg-info/dependency_links.txt
+-rw-r--r--   0 oriyonay   (501) staff       (20)       12 2023-07-30 02:50:36.000000 switchblade-0.0.6/src/switchblade.egg-info/top_level.txt
```

### Comparing `switchblade-0.0.5/LICENSE` & `switchblade-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `switchblade-0.0.5/PKG-INFO` & `switchblade-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchblade
-Version: 0.0.5
+Version: 0.0.6
 Summary: Deep learning utilities for PyTorch
 Author-email: Ori Yonay <oriyonay12@gmail.com>
 Project-URL: Homepage, https://github.com/oriyonay/switchblade
 Project-URL: Bug Tracker, https://github.com/oriyonay/switchblade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `switchblade-0.0.5/pyproject.toml` & `switchblade-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "switchblade"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Ori Yonay", email="oriyonay12@gmail.com" },
 ]
 description = "Deep learning utilities for PyTorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `switchblade-0.0.5/src/switchblade/logging.py` & `switchblade-0.0.6/src/switchblade/logging.py`

 * *Files identical despite different names*

### Comparing `switchblade-0.0.5/src/switchblade/modules/ResNetIA.py` & `switchblade-0.0.6/src/switchblade/modules/ResNetIA.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             )
 
     def forward(self, x):
         return nn.ReLU(inplace=True)(self.residual_function(x) + self.shortcut(x))
 
 
 class ResNet(nn.Module):
-    def __init__(self, block, num_block, num_classes=10, in_channels=1):
+    def __init__(self, block, num_block, num_classes=10, in_channels=3):
         super(ResNet, self).__init__()
 
         self.conv1 = nn.Sequential(
             nn.Conv2d(in_channels, 64, kernel_size=3, padding=1, bias=False),
             nn.BatchNorm2d(64),
             nn.ReLU(inplace=True)
         )
```

### Comparing `switchblade-0.0.5/src/switchblade/utils.py` & `switchblade-0.0.6/src/switchblade/utils.py`

 * *Files identical despite different names*

### Comparing `switchblade-0.0.5/src/switchblade.egg-info/PKG-INFO` & `switchblade-0.0.6/src/switchblade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchblade
-Version: 0.0.5
+Version: 0.0.6
 Summary: Deep learning utilities for PyTorch
 Author-email: Ori Yonay <oriyonay12@gmail.com>
 Project-URL: Homepage, https://github.com/oriyonay/switchblade
 Project-URL: Bug Tracker, https://github.com/oriyonay/switchblade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

