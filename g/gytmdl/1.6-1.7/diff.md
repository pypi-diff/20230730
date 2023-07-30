# Comparing `tmp/gytmdl-1.6.tar.gz` & `tmp/gytmdl-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytmdl-1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gytmdl-1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gytmdl-1.6.tar` & `gytmdl-1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1176 2023-07-26 13:38:41.672486 gytmdl-1.6/.github/workflows/main.yml
--rw-r--r--   0        0        0       80 2023-07-26 13:38:41.672486 gytmdl-1.6/.gitignore
--rw-r--r--   0        0        0     3767 2023-07-26 13:38:41.672486 gytmdl-1.6/README.md
--rw-r--r--   0        0        0       20 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/__init__.py
--rw-r--r--   0        0        0       28 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/__main__.py
--rw-r--r--   0        0        0     7906 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/cli.py
--rw-r--r--   0        0        0     8809 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/dl.py
--rw-r--r--   0        0        0      460 2023-07-26 13:38:41.672486 gytmdl-1.6/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-26 13:38:41.672486 gytmdl-1.6/requirements.txt
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 gytmdl-1.6/PKG-INFO
+-rw-r--r--   0        0        0     1176 2023-07-30 19:59:25.260901 gytmdl-1.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0       80 2023-07-30 19:59:25.264901 gytmdl-1.7/.gitignore
+-rw-r--r--   0        0        0     3775 2023-07-30 19:59:25.264901 gytmdl-1.7/README.md
+-rw-r--r--   0        0        0       20 2023-07-30 19:59:25.264901 gytmdl-1.7/gytmdl/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-30 19:59:25.264901 gytmdl-1.7/gytmdl/__main__.py
+-rw-r--r--   0        0        0     7906 2023-07-30 19:59:25.264901 gytmdl-1.7/gytmdl/cli.py
+-rw-r--r--   0        0        0     8894 2023-07-30 19:59:25.264901 gytmdl-1.7/gytmdl/dl.py
+-rw-r--r--   0        0        0      460 2023-07-30 19:59:25.264901 gytmdl-1.7/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-30 19:59:25.264901 gytmdl-1.7/requirements.txt
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 gytmdl-1.7/PKG-INFO
```

### Comparing `gytmdl-1.6/.github/workflows/main.yml` & `gytmdl-1.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gytmdl-1.6/README.md` & `gytmdl-1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 | `--ffmpeg-location` | `ffmpeg_location` | Location of the FFmpeg binary. | `ffmpeg` |
 | `--config-location` | - | Location of the config file. | `<home>/.gytmdl/config.json` |
 | `-i`, `--itag` | `itag` | Itag (audio quality). Can be `141` (256kbps AAC), `251` (128kbps Opus) or `140` (128kbps AAC). | `140` |
 | `--cover-size` | `cover_size` | Size of the cover. Can be any number between `0` and `16383`. `0` gets the highest resolution available. | `1200` |
 | `--cover-format` | `cover_format` | Format of the cover. Can be `jpg` or `png`. | `jpg` |
 | `--cover-quality` | `cover_quality` | JPEG quality of the cover. Can be any number between `0` and `100`. | `94` |
 | `--final-path-structure` | `final_path_structure` | Structure of the final path as a format string. Possible variables are `album`, `album_artist`, `artist`, `media_type`, `rating`, `title`, `track`, `track_total` and `year`. | `{album_artist}/{album}/{track:02d} {title}` |
-| `-e`, `--exclude-tags` | `exclude_tags` | List of tags to exclude from file tagging separated by commas. Possible variables are `album`, `album_artist`, `artist`, `comment`, `cover`, `lyrics`, `media_type`, `rating`, `title`, `track`, `track_total` and `year`. | `null` |
+| `-e`, `--exclude-tags` | `exclude_tags` | List of tags to exclude from file tagging separated by commas. Possible variables are `album`, `album_artist`, `artist`, `comment`, `cover`, `lyrics`, `media_type`, `rating`, `release_date`, `title`, `track` and `track_total`. | `null` |
 | `--truncate` | `truncate` | Maximum length of the file/folder names. | `40` |
 | `-l`, `--log-level` | `log_level` | Log level. Can be `DEBUG`, `INFO`, `WARNING`, `ERROR` or `CRITICAL`. | `INFO` |
 | `-s`, `--save-cover` | `save_cover` | Save cover as a separate file. | `false` |
 | `-o`, `--overwrite` | `overwrite` | Overwrite existing files. | `false` |
 | `-p`. `--print-exceptions` | `print_exceptions` | Print exceptions. | `false` |
 | `-u`, `--url-txt` | - | Read URLs as location of text files containing URLs. | `false` |
 | `-n`, `--no-config-file` | - | Don't use the config file. | `false` |
```

### Comparing `gytmdl-1.6/gytmdl/cli.py` & `gytmdl-1.7/gytmdl/cli.py`

 * *Files identical despite different names*

### Comparing `gytmdl-1.6/gytmdl/dl.py` & `gytmdl-1.7/gytmdl/dl.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import functools
 import re
 import shutil
 import subprocess
 from pathlib import Path
 
 import requests
@@ -13,16 +14,16 @@
     "album": "\xa9alb",
     "album_artist": "aART",
     "artist": "\xa9ART",
     "comment": "\xa9cmt",
     "lyrics": "\xa9lyr",
     "media_type": "stik",
     "rating": "rtng",
+    "release_date": "\xa9day",
     "title": "\xa9nam",
-    "year": "\xa9day",
 }
 
 
 class Dl:
     def __init__(
         self,
         final_path: Path,
@@ -32,15 +33,14 @@
         itag: str,
         cover_size: int,
         cover_format: str,
         cover_quality: int,
         final_path_structure: str,
         exclude_tags: str,
         truncate: int,
-        overwrite: bool,
         **kwargs,
     ):
         self.ytmusic = YTMusic()
         self.final_path = final_path
         self.temp_path = temp_path
         self.cookies_location = cookies_location
         self.ffmpeg_location = ffmpeg_location
@@ -51,15 +51,14 @@
         self.final_path_structure = final_path_structure
         self.exclude_tags = (
             [i.lower() for i in exclude_tags.split(",")]
             if exclude_tags is not None
             else []
         )
         self.truncate = None if truncate < 4 else truncate
-        self.overwrite = overwrite
 
     @functools.lru_cache()
     def get_ydl_extract_info(self, url):
         ydl_opts = {
             "quiet": True,
             "no_warnings": True,
             "extract_flat": True,
@@ -82,17 +81,18 @@
         if "watch" in ydl_extract_info["webpage_url_basename"]:
             download_queue.append(ydl_extract_info)
         return download_queue
 
     def get_artist(self, artist_list):
         if len(artist_list) == 1:
             return artist_list[0]["name"]
-        artist = ", ".join([i["name"] for i in artist_list][:-1])
-        artist += f' & {artist_list[-1]["name"]}'
-        return artist
+        return (
+            ", ".join([i["name"] for i in artist_list][:-1])
+            + f' & {artist_list[-1]["name"]}'
+        )
 
     def get_ytmusic_watch_playlist(self, video_id):
         ytmusic_watch_playlist = self.ytmusic.get_watch_playlist(video_id)
         if not ytmusic_watch_playlist["tracks"][0]["length"] and ytmusic_watch_playlist[
             "tracks"
         ][0].get("album"):
             raise Exception("Track is not available")
@@ -117,18 +117,16 @@
             ytmusic_watch_playlist["tracks"][0]["album"]["id"]
         )
         tags = {
             "album": ytmusic_album["title"],
             "album_artist": self.get_artist(ytmusic_album["artists"]),
             "artist": self.get_artist(ytmusic_watch_playlist["tracks"][0]["artists"]),
             "comment": f"https://music.youtube.com/watch?v={video_id}",
-            "cover": self.get_cover(
-                f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}'
-                + f'=w{self.cover_size}-l{self.cover_quality}-{"rj" if self.cover_format == "jpg" else "rp"}'
-            ),
+            "cover_url": f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}'
+            + f'=w{self.cover_size}-l{self.cover_quality}-{"rj" if self.cover_format == "jpg" else "rp"}',
             "media_type": 1,
             "title": ytmusic_watch_playlist["tracks"][0]["title"],
             "track_total": ytmusic_album["trackCount"],
         }
         for i, video in enumerate(
             self.get_ydl_extract_info(
                 f'https://www.youtube.com/playlist?list={ytmusic_album["audioPlaylistId"]}'
@@ -142,14 +140,18 @@
                 tags["track"] = i + 1
                 break
         if ytmusic_watch_playlist["lyrics"]:
             lyrics = self.ytmusic.get_lyrics(ytmusic_watch_playlist["lyrics"])["lyrics"]
             if lyrics is not None:
                 tags["lyrics"] = lyrics
         if ytmusic_album.get("year"):
+            tags["release_date"] = (
+                datetime.datetime.strptime(ytmusic_album["year"], "%Y").isoformat()
+                + "Z"
+            )
             tags["year"] = ytmusic_album["year"]
         return tags
 
     def get_sanizated_string(self, dirty_string, is_folder):
         dirty_string = re.sub(r'[\\/:*?"<>|;]', "_", dirty_string)
         if is_folder:
             dirty_string = dirty_string[: self.truncate]
@@ -164,29 +166,29 @@
         return self.temp_path / f"{video_id}.m4a"
 
     def get_fixed_location(self, video_id):
         return self.temp_path / f"{video_id}_fixed.m4a"
 
     def get_final_location(self, tags):
         final_location = self.final_path_structure.split("/")
-        final_location[-1] = (
+        final_location = [
+            self.get_sanizated_string(i.format(**tags), True)
+            for i in final_location[:-1]
+        ] + [
             self.get_sanizated_string(final_location[-1].format(**tags), False) + ".m4a"
-        )
-        for i, path in enumerate(final_location[:-1]):
-            final_location[i] = self.get_sanizated_string(path.format(**tags), True)
+        ]
         return self.final_path.joinpath(*final_location)
 
     def get_cover_location(self, final_location):
         return final_location.parent / f"Cover.{self.cover_format}"
 
     def download(self, video_id, temp_location):
         ydl_opts = {
             "quiet": True,
             "no_warnings": True,
-            "overwrites": self.overwrite,
             "fixup": "never",
             "format": self.itag,
             "outtmpl": str(temp_location),
         }
         if self.cookies_location is not None:
             ydl_opts["cookiefile"] = str(self.cookies_location)
         with YoutubeDL(ydl_opts) as ydl:
@@ -216,40 +218,39 @@
                 "copy",
                 fixed_location,
             ],
             check=True,
         )
 
     def apply_tags(self, fixed_location, tags):
+        _tags = {
+            v: [tags[k]]
+            for k, v in MP4_TAGS_MAP.items()
+            if k not in self.exclude_tags and tags.get(k) is not None
+        }
+        if not {"track", "track_total"} & set(self.exclude_tags):
+            _tags["trkn"] = [[0, 0]]
+        if "cover" not in self.exclude_tags:
+            _tags["covr"] = [
+                MP4Cover(
+                    self.get_cover(tags["cover_url"]), imageformat=MP4Cover.FORMAT_JPEG
+                )
+            ]
+        if "track" not in self.exclude_tags:
+            _tags["trkn"][0][0] = tags["track"]
+        if "track_total" not in self.exclude_tags:
+            _tags["trkn"][0][1] = tags["track_total"]
         mp4 = MP4(fixed_location)
         mp4.clear()
-        mp4["trkn"] = [[0, 0]]
-        for k, v in tags.items():
-            if k in self.exclude_tags:
-                continue
-            if k == "cover":
-                mp4["covr"] = [
-                    MP4Cover(
-                        v,
-                        imageformat=MP4Cover.FORMAT_JPEG
-                        if self.cover_format == "jpg"
-                        else MP4Cover.FORMAT_PNG,
-                    )
-                ]
-            elif k == "track":
-                mp4["trkn"][0][0] = v
-            elif k == "track_total":
-                mp4["trkn"][0][1] = v
-            else:
-                mp4[MP4_TAGS_MAP[k]] = [v]
+        mp4.update(_tags)
         mp4.save()
 
     def move_to_final_location(self, fixed_location, final_location):
         final_location.parent.mkdir(parents=True, exist_ok=True)
         shutil.move(fixed_location, final_location)
 
     def save_cover(self, tags, cover_location):
         with open(cover_location, "wb") as f:
-            f.write(tags["cover"])
+            f.write(self.get_cover(tags["cover_url"]))
 
     def cleanup(self):
         shutil.rmtree(self.temp_path)
```

### Comparing `gytmdl-1.6/PKG-INFO` & `gytmdl-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gytmdl
-Version: 1.6
+Version: 1.7
 Summary: Download YouTube Music songs/albums/playlists with tags from YouTube Music
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: yt-dlp
 Requires-Dist: ytmusicapi
@@ -44,15 +44,15 @@
 | `--ffmpeg-location` | `ffmpeg_location` | Location of the FFmpeg binary. | `ffmpeg` |
 | `--config-location` | - | Location of the config file. | `<home>/.gytmdl/config.json` |
 | `-i`, `--itag` | `itag` | Itag (audio quality). Can be `141` (256kbps AAC), `251` (128kbps Opus) or `140` (128kbps AAC). | `140` |
 | `--cover-size` | `cover_size` | Size of the cover. Can be any number between `0` and `16383`. `0` gets the highest resolution available. | `1200` |
 | `--cover-format` | `cover_format` | Format of the cover. Can be `jpg` or `png`. | `jpg` |
 | `--cover-quality` | `cover_quality` | JPEG quality of the cover. Can be any number between `0` and `100`. | `94` |
 | `--final-path-structure` | `final_path_structure` | Structure of the final path as a format string. Possible variables are `album`, `album_artist`, `artist`, `media_type`, `rating`, `title`, `track`, `track_total` and `year`. | `{album_artist}/{album}/{track:02d} {title}` |
-| `-e`, `--exclude-tags` | `exclude_tags` | List of tags to exclude from file tagging separated by commas. Possible variables are `album`, `album_artist`, `artist`, `comment`, `cover`, `lyrics`, `media_type`, `rating`, `title`, `track`, `track_total` and `year`. | `null` |
+| `-e`, `--exclude-tags` | `exclude_tags` | List of tags to exclude from file tagging separated by commas. Possible variables are `album`, `album_artist`, `artist`, `comment`, `cover`, `lyrics`, `media_type`, `rating`, `release_date`, `title`, `track` and `track_total`. | `null` |
 | `--truncate` | `truncate` | Maximum length of the file/folder names. | `40` |
 | `-l`, `--log-level` | `log_level` | Log level. Can be `DEBUG`, `INFO`, `WARNING`, `ERROR` or `CRITICAL`. | `INFO` |
 | `-s`, `--save-cover` | `save_cover` | Save cover as a separate file. | `false` |
 | `-o`, `--overwrite` | `overwrite` | Overwrite existing files. | `false` |
 | `-p`. `--print-exceptions` | `print_exceptions` | Print exceptions. | `false` |
 | `-u`, `--url-txt` | - | Read URLs as location of text files containing URLs. | `false` |
 | `-n`, `--no-config-file` | - | Don't use the config file. | `false` |
```

