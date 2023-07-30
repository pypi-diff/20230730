# Comparing `tmp/AutoQPF-0.1.5.tar.gz` & `tmp/AutoQPF-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoQPF-0.1.5.tar", last modified: Sun Jul 30 16:40:47 2023, max compression
+gzip compressed data, was "AutoQPF-0.1.6.tar", last modified: Sun Jul 30 19:55:04 2023, max compression
```

## Comparing `AutoQPF-0.1.5.tar` & `AutoQPF-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 16:40:47.028483 AutoQPF-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-07-30 16:40:47.023481 AutoQPF-0.1.5/AutoQPF.egg-info/
--rw-rw-rw-   0        0        0     4021 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-07-22 05:44:21.000000 AutoQPF-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4021 2023-07-30 16:40:47.027483 AutoQPF-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3349 2023-07-30 16:38:58.000000 AutoQPF-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 16:40:47.027483 AutoQPF-0.1.5/auto_qpf/
--rw-rw-rw-   0        0        0      314 2023-07-30 16:27:31.000000 AutoQPF-0.1.5/auto_qpf/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-28 21:54:15.000000 AutoQPF-0.1.5/auto_qpf/enums.py
--rw-rw-rw-   0        0        0     8968 2023-07-30 16:21:49.000000 AutoQPF-0.1.5/auto_qpf/generate_chapters.py
--rw-rw-rw-   0        0        0      561 2023-07-23 04:41:05.000000 AutoQPF-0.1.5/auto_qpf/long_path.py
--rw-rw-rw-   0        0        0     7258 2023-07-30 16:39:06.000000 AutoQPF-0.1.5/auto_qpf/qpf.py
--rw-rw-rw-   0        0        0      257 2023-07-22 04:57:33.000000 AutoQPF-0.1.5/auto_qpf/qpf_exceptions.py
--rw-rw-rw-   0        0        0       42 2023-07-30 16:40:47.028483 AutoQPF-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-07-30 16:39:04.000000 AutoQPF-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:55:04.564514 AutoQPF-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-07-30 19:55:04.556515 AutoQPF-0.1.6/AutoQPF.egg-info/
+-rw-rw-rw-   0        0        0     4021 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-07-22 05:44:21.000000 AutoQPF-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4021 2023-07-30 19:55:04.564514 AutoQPF-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3349 2023-07-30 16:38:58.000000 AutoQPF-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 19:55:04.563514 AutoQPF-0.1.6/auto_qpf/
+-rw-rw-rw-   0        0        0      314 2023-07-30 16:27:31.000000 AutoQPF-0.1.6/auto_qpf/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 21:54:15.000000 AutoQPF-0.1.6/auto_qpf/enums.py
+-rw-rw-rw-   0        0        0     8968 2023-07-30 16:21:49.000000 AutoQPF-0.1.6/auto_qpf/generate_chapters.py
+-rw-rw-rw-   0        0        0      561 2023-07-23 04:41:05.000000 AutoQPF-0.1.6/auto_qpf/long_path.py
+-rw-rw-rw-   0        0        0     7348 2023-07-30 19:54:18.000000 AutoQPF-0.1.6/auto_qpf/qpf.py
+-rw-rw-rw-   0        0        0      257 2023-07-22 04:57:33.000000 AutoQPF-0.1.6/auto_qpf/qpf_exceptions.py
+-rw-rw-rw-   0        0        0       42 2023-07-30 19:55:04.564514 AutoQPF-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-07-30 19:54:30.000000 AutoQPF-0.1.6/setup.py
```

### Comparing `AutoQPF-0.1.5/AutoQPF.egg-info/PKG-INFO` & `AutoQPF-0.1.6/AutoQPF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoQPF
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generates QPF frame time codes to be used with x264/x265
 Home-page: https://github.com/jlw4049/AutoQPF
 Author: Jessie Wilson
 Author-email: jessielw4049@gmail.com
 License: MIT
 Keywords: AutoQPF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AutoQPF-0.1.5/LICENSE` & `AutoQPF-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.5/PKG-INFO` & `AutoQPF-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoQPF
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generates QPF frame time codes to be used with x264/x265
 Home-page: https://github.com/jlw4049/AutoQPF
 Author: Jessie Wilson
 Author-email: jessielw4049@gmail.com
 License: MIT
 Keywords: AutoQPF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AutoQPF-0.1.5/README.md` & `AutoQPF-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.5/auto_qpf/generate_chapters.py` & `AutoQPF-0.1.6/auto_qpf/generate_chapters.py`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.5/auto_qpf/long_path.py` & `AutoQPF-0.1.6/auto_qpf/long_path.py`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.5/auto_qpf/qpf.py` & `AutoQPF-0.1.6/auto_qpf/qpf.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,17 @@
             media_info = MediaInfo.parse(file_input, parse_speed=0.1)
             detect_fps = self._get_fps(media_info)
 
             if generate_chapters:
                 file_input = ChapterGenerator().generate_ogm_chapters(
                     media_info_obj=media_info,
                     extract_tagged=False,
-                    output_path=file_output.with_suffix(".txt"),
+                    output_path=file_output.with_name(
+                        file_output.stem + "_chapters"
+                    ).with_suffix(".qpf"),
                 )
                 time_codes = self._get_time_codes_text(file_input)
             else:
                 time_codes = self._get_time_codes_media_file(media_info)
 
         # if we're auto detecting fps attempt to update fps
         if auto_detect_fps:
```

### Comparing `AutoQPF-0.1.5/setup.py` & `AutoQPF-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as fd:
     ext_long_desc = fd.read()
 
 setup(
     name="AutoQPF",
-    version="0.1.5",
+    version="0.1.6",
     description="Generates QPF frame time codes to be used with x264/x265",
     long_description=ext_long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/jlw4049/AutoQPF",
     author="Jessie Wilson",
     author_email="jessielw4049@gmail.com",
     license="MIT",
```

