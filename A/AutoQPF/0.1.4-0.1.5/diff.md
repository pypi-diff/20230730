# Comparing `tmp/AutoQPF-0.1.4.tar.gz` & `tmp/AutoQPF-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoQPF-0.1.4.tar", last modified: Sun Jul 23 04:43:10 2023, max compression
+gzip compressed data, was "AutoQPF-0.1.5.tar", last modified: Sun Jul 30 16:40:47 2023, max compression
```

## Comparing `AutoQPF-0.1.4.tar` & `AutoQPF-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 04:43:10.051165 AutoQPF-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-07-23 04:43:10.047156 AutoQPF-0.1.4/AutoQPF.egg-info/
--rw-rw-rw-   0        0        0     2289 2023-07-23 04:43:09.000000 AutoQPF-0.1.4/AutoQPF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-23 04:43:09.000000 AutoQPF-0.1.4/AutoQPF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 04:43:09.000000 AutoQPF-0.1.4/AutoQPF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-23 04:43:09.000000 AutoQPF-0.1.4/AutoQPF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-23 04:43:09.000000 AutoQPF-0.1.4/AutoQPF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-07-22 05:44:21.000000 AutoQPF-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2289 2023-07-23 04:43:10.051165 AutoQPF-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2023-07-22 21:26:58.000000 AutoQPF-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 04:43:10.050162 AutoQPF-0.1.4/auto_qpf/
--rw-rw-rw-   0        0        0      259 2023-07-23 02:27:06.000000 AutoQPF-0.1.4/auto_qpf/__init__.py
--rw-rw-rw-   0        0        0      561 2023-07-23 04:41:05.000000 AutoQPF-0.1.4/auto_qpf/long_path.py
--rw-rw-rw-   0        0        0     6572 2023-07-23 04:42:31.000000 AutoQPF-0.1.4/auto_qpf/qpf.py
--rw-rw-rw-   0        0        0      257 2023-07-22 04:57:33.000000 AutoQPF-0.1.4/auto_qpf/qpf_exceptions.py
--rw-rw-rw-   0        0        0       42 2023-07-23 04:43:10.051165 AutoQPF-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-07-23 04:42:43.000000 AutoQPF-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:40:47.028483 AutoQPF-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-07-30 16:40:47.023481 AutoQPF-0.1.5/AutoQPF.egg-info/
+-rw-rw-rw-   0        0        0     4021 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 16:40:46.000000 AutoQPF-0.1.5/AutoQPF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-07-22 05:44:21.000000 AutoQPF-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4021 2023-07-30 16:40:47.027483 AutoQPF-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3349 2023-07-30 16:38:58.000000 AutoQPF-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 16:40:47.027483 AutoQPF-0.1.5/auto_qpf/
+-rw-rw-rw-   0        0        0      314 2023-07-30 16:27:31.000000 AutoQPF-0.1.5/auto_qpf/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 21:54:15.000000 AutoQPF-0.1.5/auto_qpf/enums.py
+-rw-rw-rw-   0        0        0     8968 2023-07-30 16:21:49.000000 AutoQPF-0.1.5/auto_qpf/generate_chapters.py
+-rw-rw-rw-   0        0        0      561 2023-07-23 04:41:05.000000 AutoQPF-0.1.5/auto_qpf/long_path.py
+-rw-rw-rw-   0        0        0     7258 2023-07-30 16:39:06.000000 AutoQPF-0.1.5/auto_qpf/qpf.py
+-rw-rw-rw-   0        0        0      257 2023-07-22 04:57:33.000000 AutoQPF-0.1.5/auto_qpf/qpf_exceptions.py
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:40:47.028483 AutoQPF-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-07-30 16:39:04.000000 AutoQPF-0.1.5/setup.py
```

### Comparing `AutoQPF-0.1.4/LICENSE` & `AutoQPF-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.4/auto_qpf/long_path.py` & `AutoQPF-0.1.5/auto_qpf/long_path.py`

 * *Files identical despite different names*

### Comparing `AutoQPF-0.1.4/auto_qpf/qpf.py` & `AutoQPF-0.1.5/auto_qpf/qpf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from auto_qpf.long_path import check_for_long_path
 from auto_qpf.qpf_exceptions import (
     ImproperChapterError,
     NoChapterDataError,
     ChapterIndexError,
 )
+from auto_qpf.generate_chapters import ChapterGenerator
 
 
 class QpfGenerator:
     """
     Generates QPF file, accepted formats are media or OGM text.
 
     Public method: generate_qpf
@@ -21,25 +22,28 @@
     def generate_qpf(
         self,
         file_input: Union[Path, str],
         file_output: Union[Path, str] = None,
         write_to_disk: bool = True,
         fps: Union[int, float] = 23.976,
         auto_detect_fps: bool = True,
+        generate_chapters: bool = True,
     ):
         """Creates chapter QPF and returns the path to the output file.
 
         Args:
             file_input (Union[Path, str]): File input.
             file_output (Union[Path, str], optional): File output. Defaults to None (will auto create name).
             write_to_disk (bool, optional): If this is set, writes to disk, if not it'll return an object with the qpf.
             fps (Union[int, float], optional): Source FPS. Defaults to 23.976. If auto_detect_fps is true and
             input is a not a .txt file, this will be over-ridden automatically.
             auto_detect_fps (bool, optional): Auto detects non text based sources if a video track is present.
             Defaults to True.
+            generate_chapters (bool, optional): When enabled this will run a helper class to extract and/or generate new
+            new chapters as needed to create a qpf code for.
         """
         # check if we're on a windows platform, if so check for long path support
         if platform.system() == "Windows":
             long_path = check_for_long_path()
             if not long_path:
                 print(
                     "WARNING: Long path is not enabled for this OS. This can cause issues for paths greater > 260 characters."
@@ -53,15 +57,26 @@
             file_output = self._auto_output(file_input)
 
         # check if input is a text file vs a media file
         if file_input.suffix == ".txt":
             auto_detect_fps = False
             time_codes = self._get_time_codes_text(file_input)
         else:
-            time_codes, detect_fps = self._get_time_codes_media_file(file_input)
+            media_info = MediaInfo.parse(file_input, parse_speed=0.1)
+            detect_fps = self._get_fps(media_info)
+
+            if generate_chapters:
+                file_input = ChapterGenerator().generate_ogm_chapters(
+                    media_info_obj=media_info,
+                    extract_tagged=False,
+                    output_path=file_output.with_suffix(".txt"),
+                )
+                time_codes = self._get_time_codes_text(file_input)
+            else:
+                time_codes = self._get_time_codes_media_file(media_info)
 
         # if we're auto detecting fps attempt to update fps
         if auto_detect_fps:
             if detect_fps:
                 fps = detect_fps
 
         # if no time codes are detected
@@ -82,17 +97,16 @@
     def _process_time_codes(self, time_codes: list, fps: Union[float, str]):
         converted_time_codes = []
         for code in time_codes:
             convert_time = self._calculate_frame_position(code, fps)
             converted_time_codes.append(convert_time)
         return converted_time_codes
 
-    def _get_time_codes_media_file(self, file_input: Path):
+    def _get_time_codes_media_file(self, media_info: MediaInfo.parse):
         time_code_list = []
-        media_info = MediaInfo.parse(file_input, parse_speed=0.1)
         menu_stream_count = media_info.general_tracks[0].count_of_menu_streams
         if menu_stream_count and int(menu_stream_count) > 0:
             chapter_data = media_info.menu_tracks[0].to_data()
             if chapter_data:
                 chapter_data = list(chapter_data.keys())
                 try:
                     get_index = chapter_data.index("chapters_pos_end") + 1
@@ -104,15 +118,15 @@
                         "Cannot find the position of chapters_pos_end"
                     )
             else:
                 raise NoChapterDataError("Input file has no chapter data")
         else:
             raise NoChapterDataError("Input file has no chapter data")
 
-        return time_code_list, self._get_fps(media_info)
+        return time_code_list
 
     @staticmethod
     def _auto_output(file_input: Path):
         return file_input.parent / Path(file_input.name).with_suffix(".qpf")
 
     @staticmethod
     def _get_time_codes_text(file_input: Path):
```

### Comparing `AutoQPF-0.1.4/setup.py` & `AutoQPF-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as fd:
     ext_long_desc = fd.read()
 
 setup(
     name="AutoQPF",
-    version="0.1.4",
+    version="0.1.5",
     description="Generates QPF frame time codes to be used with x264/x265",
     long_description=ext_long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/jlw4049/AutoQPF",
     author="Jessie Wilson",
     author_email="jessielw4049@gmail.com",
     license="MIT",
```

