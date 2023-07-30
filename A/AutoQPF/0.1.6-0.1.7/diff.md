# Comparing `tmp/AutoQPF-0.1.6.tar.gz` & `tmp/AutoQPF-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoQPF-0.1.6.tar", last modified: Sun Jul 30 19:55:04 2023, max compression
+gzip compressed data, was "AutoQPF-0.1.7.tar", last modified: Sun Jul 30 20:17:56 2023, max compression
```

## Comparing `AutoQPF-0.1.6.tar` & `AutoQPF-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 19:55:04.564514 AutoQPF-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-07-30 19:55:04.556515 AutoQPF-0.1.6/AutoQPF.egg-info/
--rw-rw-rw-   0        0        0     4021 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 19:55:04.000000 AutoQPF-0.1.6/AutoQPF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-07-22 05:44:21.000000 AutoQPF-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     4021 2023-07-30 19:55:04.564514 AutoQPF-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3349 2023-07-30 16:38:58.000000 AutoQPF-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 19:55:04.563514 AutoQPF-0.1.6/auto_qpf/
--rw-rw-rw-   0        0        0      314 2023-07-30 16:27:31.000000 AutoQPF-0.1.6/auto_qpf/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-28 21:54:15.000000 AutoQPF-0.1.6/auto_qpf/enums.py
--rw-rw-rw-   0        0        0     8968 2023-07-30 16:21:49.000000 AutoQPF-0.1.6/auto_qpf/generate_chapters.py
--rw-rw-rw-   0        0        0      561 2023-07-23 04:41:05.000000 AutoQPF-0.1.6/auto_qpf/long_path.py
--rw-rw-rw-   0        0        0     7348 2023-07-30 19:54:18.000000 AutoQPF-0.1.6/auto_qpf/qpf.py
--rw-rw-rw-   0        0        0      257 2023-07-22 04:57:33.000000 AutoQPF-0.1.6/auto_qpf/qpf_exceptions.py
--rw-rw-rw-   0        0        0       42 2023-07-30 19:55:04.564514 AutoQPF-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-07-30 19:54:30.000000 AutoQPF-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:17:56.664936 AutoQPF-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-07-30 20:17:56.659936 AutoQPF-0.1.7/AutoQPF.egg-info/
+-rw-rw-rw-   0        0        0     4021 2023-07-30 20:17:56.000000 AutoQPF-0.1.7/AutoQPF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-30 20:17:56.000000 AutoQPF-0.1.7/AutoQPF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 20:17:56.000000 AutoQPF-0.1.7/AutoQPF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 20:17:56.000000 AutoQPF-0.1.7/AutoQPF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 20:17:56.000000 AutoQPF-0.1.7/AutoQPF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-07-22 05:44:21.000000 AutoQPF-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4021 2023-07-30 20:17:56.664936 AutoQPF-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3349 2023-07-30 16:38:58.000000 AutoQPF-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 20:17:56.663936 AutoQPF-0.1.7/auto_qpf/
+-rw-rw-rw-   0        0        0      314 2023-07-30 16:27:31.000000 AutoQPF-0.1.7/auto_qpf/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 21:54:15.000000 AutoQPF-0.1.7/auto_qpf/enums.py
+-rw-rw-rw-   0        0        0     8968 2023-07-30 16:21:49.000000 AutoQPF-0.1.7/auto_qpf/generate_chapters.py
+-rw-rw-rw-   0        0        0      561 2023-07-23 04:41:05.000000 AutoQPF-0.1.7/auto_qpf/long_path.py
+-rw-rw-rw-   0        0        0     7466 2023-07-30 20:16:55.000000 AutoQPF-0.1.7/auto_qpf/qpf.py
+-rw-rw-rw-   0        0        0      257 2023-07-22 04:57:33.000000 AutoQPF-0.1.7/auto_qpf/qpf_exceptions.py
+-rw-rw-rw-   0        0        0       42 2023-07-30 20:17:56.664936 AutoQPF-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-07-30 20:17:11.000000 AutoQPF-0.1.7/setup.py
```

### Comparing `AutoQPF-0.1.6/AutoQPF.egg-info/PKG-INFO` & `AutoQPF-0.1.7/AutoQPF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoQPF
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generates QPF frame time codes to be used with x264/x265
 Home-page: https://github.com/jlw4049/AutoQPF
 Author: Jessie Wilson
 Author-email: jessielw4049@gmail.com
 License: MIT
 Keywords: AutoQPF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AutoQPF-0.1.6/LICENSE` & `AutoQPF-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.6/PKG-INFO` & `AutoQPF-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoQPF
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generates QPF frame time codes to be used with x264/x265
 Home-page: https://github.com/jlw4049/AutoQPF
 Author: Jessie Wilson
 Author-email: jessielw4049@gmail.com
 License: MIT
 Keywords: AutoQPF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AutoQPF-0.1.6/README.md` & `AutoQPF-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.6/auto_qpf/generate_chapters.py` & `AutoQPF-0.1.7/auto_qpf/generate_chapters.py`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.6/auto_qpf/long_path.py` & `AutoQPF-0.1.7/auto_qpf/long_path.py`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.6/auto_qpf/qpf.py` & `AutoQPF-0.1.7/auto_qpf/qpf.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,22 +59,23 @@
         # check if input is a text file vs a media file
         if file_input.suffix == ".txt":
             auto_detect_fps = False
             time_codes = self._get_time_codes_text(file_input)
         else:
             media_info = MediaInfo.parse(file_input, parse_speed=0.1)
             detect_fps = self._get_fps(media_info)
-
+            
             if generate_chapters:
+                # generate new output with _chapters before the extension for txt files
+                txt_output = file_output.with_suffix("").with_name(file_output.stem + "_chapters.txt")
+                
                 file_input = ChapterGenerator().generate_ogm_chapters(
                     media_info_obj=media_info,
                     extract_tagged=False,
-                    output_path=file_output.with_name(
-                        file_output.stem + "_chapters"
-                    ).with_suffix(".qpf"),
+                    output_path=txt_output,
                 )
                 time_codes = self._get_time_codes_text(file_input)
             else:
                 time_codes = self._get_time_codes_media_file(media_info)
 
         # if we're auto detecting fps attempt to update fps
         if auto_detect_fps:
@@ -124,15 +125,15 @@
         else:
             raise NoChapterDataError("Input file has no chapter data")
 
         return time_code_list
 
     @staticmethod
     def _auto_output(file_input: Path):
-        return file_input.parent / Path(file_input.name).with_suffix(".qpf")
+        return Path(file_input.parent / Path(file_input.name).with_suffix(".qpf"))
 
     @staticmethod
     def _get_time_codes_text(file_input: Path):
         time_code_list = []
         with open(file_input, "rt", encoding="utf-8") as txt_file:
             time_codes = txt_file.readlines()
             for num, chap in enumerate(time_codes):
```

### Comparing `AutoQPF-0.1.6/setup.py` & `AutoQPF-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as fd:
     ext_long_desc = fd.read()
 
 setup(
     name="AutoQPF",
-    version="0.1.6",
+    version="0.1.7",
     description="Generates QPF frame time codes to be used with x264/x265",
     long_description=ext_long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/jlw4049/AutoQPF",
     author="Jessie Wilson",
     author_email="jessielw4049@gmail.com",
     license="MIT",
```

