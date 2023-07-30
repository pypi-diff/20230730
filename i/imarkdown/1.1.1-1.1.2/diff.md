# Comparing `tmp/imarkdown-1.1.1.tar.gz` & `tmp/imarkdown-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imarkdown-1.1.1.tar", last modified: Thu Jul 13 16:52:49 2023, max compression
+gzip compressed data, was "imarkdown-1.1.2.tar", last modified: Sun Jul 30 15:17:20 2023, max compression
```

## Comparing `imarkdown-1.1.1.tar` & `imarkdown-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.721447 imarkdown-1.1.1/
--rw-rw-rw-   0        0        0    17228 2023-07-13 16:52:49.720446 imarkdown-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    16366 2023-07-13 10:10:10.000000 imarkdown-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.691455 imarkdown-1.1.1/imarkdown/
--rw-rw-rw-   0        0        0      464 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.706447 imarkdown-1.1.1/imarkdown/adapter/
--rw-rw-rw-   0        0        0      476 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/aliyun_adapter.py
--rw-rw-rw-   0        0        0      835 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/base.py
--rw-rw-rw-   0        0        0      755 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/local_adapter.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.707446 imarkdown-1.1.1/imarkdown/client/
--rw-rw-rw-   0        0        0        0 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/client/__init__.py
--rw-rw-rw-   0        0        0     1371 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/config.py
--rw-rw-rw-   0        0        0      267 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/constant.py
--rw-rw-rw-   0        0        0    12736 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/converter.py
--rw-rw-rw-   0        0        0     9764 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/schema.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.712448 imarkdown-1.1.1/imarkdown/utils/
--rw-rw-rw-   0        0        0     2784 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/utils/__init__.py
--rw-rw-rw-   0        0        0      282 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/utils/cache.py
--rw-rw-rw-   0        0        0     1403 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/utils/singleton.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.699448 imarkdown-1.1.1/imarkdown.egg-info/
--rw-rw-rw-   0        0        0    17228 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2022-12-18 07:47:47.000000 imarkdown-1.1.1/license
--rw-rw-rw-   0        0        0       42 2023-07-13 16:52:49.721447 imarkdown-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1940 2023-07-13 16:52:05.000000 imarkdown-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.718448 imarkdown-1.1.1/tests/
--rw-rw-rw-   0        0        0     2379 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_adapter.py
--rw-rw-rw-   0        0        0     2273 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_image_converter.py
--rw-rw-rw-   0        0        0     2235 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_md_file.py
--rw-rw-rw-   0        0        0     2957 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.819378 imarkdown-1.1.2/
+-rw-rw-rw-   0        0        0    17228 2023-07-30 15:17:20.818376 imarkdown-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16366 2023-07-13 10:10:10.000000 imarkdown-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.790769 imarkdown-1.1.2/imarkdown/
+-rw-rw-rw-   0        0        0      464 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.803769 imarkdown-1.1.2/imarkdown/adapter/
+-rw-rw-rw-   0        0        0      476 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/__init__.py
+-rw-rw-rw-   0        0        0     2939 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/aliyun_adapter.py
+-rw-rw-rw-   0        0        0      835 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/base.py
+-rw-rw-rw-   0        0        0      755 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/local_adapter.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.805773 imarkdown-1.1.2/imarkdown/client/
+-rw-rw-rw-   0        0        0        0 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/client/__init__.py
+-rw-rw-rw-   0        0        0     1371 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/config.py
+-rw-rw-rw-   0        0        0      267 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/constant.py
+-rw-rw-rw-   0        0        0    13230 2023-07-30 15:11:33.000000 imarkdown-1.1.2/imarkdown/converter.py
+-rw-rw-rw-   0        0        0    10130 2023-07-30 14:13:57.000000 imarkdown-1.1.2/imarkdown/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.809770 imarkdown-1.1.2/imarkdown/utils/
+-rw-rw-rw-   0        0        0     2784 2023-07-30 13:02:07.000000 imarkdown-1.1.2/imarkdown/utils/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/utils/cache.py
+-rw-rw-rw-   0        0        0     1403 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/utils/singleton.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.797773 imarkdown-1.1.2/imarkdown.egg-info/
+-rw-rw-rw-   0        0        0    17228 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2022-12-18 07:47:47.000000 imarkdown-1.1.2/license
+-rw-rw-rw-   0        0        0       42 2023-07-30 15:17:20.819378 imarkdown-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1940 2023-07-30 15:13:01.000000 imarkdown-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.816479 imarkdown-1.1.2/tests/
+-rw-rw-rw-   0        0        0     2379 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_adapter.py
+-rw-rw-rw-   0        0        0     2273 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_image_converter.py
+-rw-rw-rw-   0        0        0     2235 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_md_file.py
+-rw-rw-rw-   0        0        0     2957 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_utils.py
```

### Comparing `imarkdown-1.1.1/PKG-INFO` & `imarkdown-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imarkdown
-Version: 1.1.1
+Version: 1.1.2
 Summary: A practical Markdown image url converter
 Home-page: https://github.com/Undertone0809/imarkdown
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: Markdown,markdown,imarkdown,markdown converter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imarkdown-1.1.1/README.md` & `imarkdown-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/imarkdown/adapter/aliyun_adapter.py` & `imarkdown-1.1.2/imarkdown/adapter/aliyun_adapter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/imarkdown/adapter/base.py` & `imarkdown-1.1.2/imarkdown/adapter/base.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/imarkdown/adapter/local_adapter.py` & `imarkdown-1.1.2/imarkdown/adapter/local_adapter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/imarkdown/config.py` & `imarkdown-1.1.2/imarkdown/config.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/imarkdown/converter.py` & `imarkdown-1.1.2/imarkdown/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Return converted image absolute path
     """
     try:
         response = requests.get(image_url)
         now_time = time.strftime("%Y%m%d_%H%M%S", time.localtime(time.time()))
         image_local_storage_directory = polish_path(image_local_storage_directory)
         if not os.path.exists(image_local_storage_directory):
-            os.mkdir(image_local_storage_directory)
+            os.makedirs(image_local_storage_directory, exist_ok=True)
 
         images_path = f"{image_local_storage_directory}{now_time}{random.randint(1000, 10000)}.png"
         with open(images_path, "wb") as f:
             f.write(response.content)
         logger.info(f"[imarkdown] <{images_path}> has stored in local successfully")
         return images_path
     except Exception as e:
@@ -144,15 +144,17 @@
         """
         md_file_path = supplementary_file_path(md_file_path)
         md_name = md_file_path.split("/")[-1][:-3]
 
         if enable_rename:
             if new_name != "":
                 if name_prefix or name_prefix:
-                    raise ValueError("You can not set `name_prefix` and `name_prefix` if you set `new_name`.")
+                    raise ValueError(
+                        "You can not set `name_prefix` and `name_prefix` if you set `new_name`."
+                    )
                 self.converted_md_file_name = new_name
             else:
                 self.converted_md_file_name = f"{name_prefix}{md_name}{name_suffix}.md"
             logger.debug(
                 f"[imarkdown] BaseMdImageConverter set converted_md_file_name {self.converted_md_file_name}"
             )
             return
@@ -216,26 +218,34 @@
 
         Args:
             md_str: markdown original data
 
         Returns:
             Markdown data for the image url has been changed.
         """
-        images = list(
-            map(
-                lambda item: item[1],
-                re.findall(
-                    r"(?:!\[(.*?)\]\((.*?)\))|<img.*?src=[\'\"](.*?)[\'\"].*?>", md_str
-                ),
-            )
+        _images = re.findall(
+            r"(?:!\[(.*?)\]\((.*?)\))|<img.*?src=[\'\"](.*?)[\'\"].*?>", md_str
         )
 
+        images = []
+        for image in _images:
+            if image[1] == "":
+                continue
+            # If current image link is local path URL and you need to web URL to a local path,
+            # the local path url will not be converted.
+            if not self.is_local_images and not image[1].startswith("http"):
+                continue
+            images.append(image[1])
+
         for image in images:
             converted_image_url = self._get_converted_image_url(image)
             md_str = md_str.replace(image, converted_image_url)
+        logger.info(
+            f"[imarkdown] All images conversion for this md file have been completed, ready to save to file."
+        )
         return md_str
 
     def _get_converted_image_url(self, original_image_url: str) -> str:
         """Get converted image url by adapter.
 
         Args:
             original_image_url: links to images that needs to be converted
```

### Comparing `imarkdown-1.1.1/imarkdown/schema.py` & `imarkdown-1.1.2/imarkdown/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,25 +61,25 @@
         assert os.path.exists(
             values["absolute_path_name"]
         ), f'<{values["absolute_path_name"]}> does not exists.'
         assert (
             values["name"][-3:] == ".md"
         ), f'<{values["name"][-3:]}> is not markdown file.'
 
+        values["name"] = values["absolute_path_name"].split("/")[-1]
         values["absolute_path"] = "/".join(values["absolute_path_name"].split("/")[:-1])
         if "image_type" in values and values["image_type"] == "local":
             assert (
                 "image_directory" in values and values["image_directory"]
             ), "If image_type is local, then image_directory is necessary."
             values["image_directory"] = supplementary_file_path(
                 values["image_directory"]
             )
             values["is_default_image_directory"] = False
         else:
-            # set default image_directory if image_type == remote
             if "image_directory" not in values or not values["image_directory"]:
                 values["image_directory"] = f"{values['absolute_path']}/images"
                 values["is_default_image_directory"] = True
 
         if "output_directory" not in values:
             values["output_directory"] = values["absolute_path"]
         os.makedirs(values["output_directory"], exist_ok=True)
@@ -94,15 +94,15 @@
                 "You can not set enable_save_images = False if you original markdown file image is local url."
             )
         return enable_save_images
 
     @property
     def to_convert_params(self) -> Dict[str, Any]:
         params = {
-            "md_file_path": self.name,
+            "md_file_path": self.absolute_path_name,
             "enable_rename": self.enable_rename,
             "output_md_directory": self.output_directory,
             "image_local_storage_directory": self.image_directory,
             "is_local_images": True if self.image_type == "local" else False,
             "enable_save_images": self.enable_save_images,
         }
         logger.debug(f"[imarkdown] MdFile convert params {params}")
@@ -195,14 +195,15 @@
     additional_kwargs: Optional[Dict[str, Any]] = None
 
     def update_config(
         self,
         output_directory: Optional[str] = None,
         enable_save_images: bool = True,
     ):
+        """Update every md_file basic parameters."""
         if not self._md_files:
             ValueError("Please run generate_md_files firstly.")
         for md_file in self._md_files:
             params = {
                 "output_directory": output_directory,
                 "enable_save_images": enable_save_images,
             }
@@ -211,14 +212,23 @@
 
             md_file.update_config(**params)
 
     def init_md_files(
         self,
         md_mediums: List[Union[MdFile, MdFolder]],
     ) -> List[MdFile]:
+        """MdFolder may contain several MdFile.This method can convert all
+        MdFolders and MdFiles to MdFiles list.
+
+        Args:
+            md_mediums(List[Union[MdFile, MdFolder]]): a list of MdFile and MdFolder
+
+        Returns:
+            A list of all MdFile.
+        """
         def find_sub_files(md_folder: MdFolder):
             for sub_node in md_folder.sub_nodes:
                 if isinstance(sub_node, MdFile):
                     self._md_files.append(sub_node)
                 elif isinstance(sub_node, MdFolder):
                     find_sub_files(sub_node)
```

### Comparing `imarkdown-1.1.1/imarkdown/utils/__init__.py` & `imarkdown-1.1.2/imarkdown/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/imarkdown/utils/singleton.py` & `imarkdown-1.1.2/imarkdown/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/imarkdown.egg-info/PKG-INFO` & `imarkdown-1.1.2/imarkdown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imarkdown
-Version: 1.1.1
+Version: 1.1.2
 Summary: A practical Markdown image url converter
 Home-page: https://github.com/Undertone0809/imarkdown
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: Markdown,markdown,imarkdown,markdown converter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imarkdown-1.1.1/imarkdown.egg-info/SOURCES.txt` & `imarkdown-1.1.2/imarkdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/license` & `imarkdown-1.1.2/license`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/setup.py` & `imarkdown-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import setuptools
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="imarkdown",
-    version="1.1.1",
+    version="1.1.2",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A practical Markdown image url converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/imarkdown",
     packages=setuptools.find_packages(),
```

### Comparing `imarkdown-1.1.1/tests/test_adapter.py` & `imarkdown-1.1.2/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/tests/test_image_converter.py` & `imarkdown-1.1.2/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/tests/test_md_file.py` & `imarkdown-1.1.2/tests/test_md_file.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.1/tests/test_utils.py` & `imarkdown-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

