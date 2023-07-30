# Comparing `tmp/pyvidplayer2-0.9.0.tar.gz` & `tmp/pyvidplayer2-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvidplayer2-0.9.0.tar", last modified: Fri Jul 28 00:56:42 2023, max compression
+gzip compressed data, was "pyvidplayer2-0.9.1.tar", last modified: Sun Jul 30 14:52:15 2023, max compression
```

## Comparing `pyvidplayer2-0.9.0.tar` & `pyvidplayer2-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 00:56:42.949755 pyvidplayer2-0.9.0/
--rw-rw-rw-   0        0        0     1085 2023-07-19 21:30:21.000000 pyvidplayer2-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     2477 2023-07-28 00:56:42.949755 pyvidplayer2-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2144 2023-07-27 22:48:06.000000 pyvidplayer2-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 00:56:42.935516 pyvidplayer2-0.9.0/pyvidplayer2/
--rw-rw-rw-   0        0        0      636 2023-07-21 18:47:18.000000 pyvidplayer2-0.9.0/pyvidplayer2/__init__.py
--rw-rw-rw-   0        0        0     4625 2023-07-28 00:06:49.000000 pyvidplayer2-0.9.0/pyvidplayer2/parallel_video.py
--rw-rw-rw-   0        0        0     1341 2023-07-27 00:33:32.000000 pyvidplayer2-0.9.0/pyvidplayer2/post_processing.py
--rw-rw-rw-   0        0        0     2232 2023-07-26 19:34:24.000000 pyvidplayer2-0.9.0/pyvidplayer2/subtitles.py
--rw-rw-rw-   0        0        0     8460 2023-07-27 22:38:11.000000 pyvidplayer2-0.9.0/pyvidplayer2/video.py
--rw-rw-rw-   0        0        0     1752 2023-07-27 22:30:16.000000 pyvidplayer2-0.9.0/pyvidplayer2/video_collection.py
--rw-rw-rw-   0        0        0     9404 2023-07-28 00:41:46.000000 pyvidplayer2-0.9.0/pyvidplayer2/video_player.py
--rw-rw-rw-   0        0        0     1531 2023-07-26 18:35:59.000000 pyvidplayer2-0.9.0/pyvidplayer2/video_pyglet.py
--rw-rw-rw-   0        0        0     1511 2023-07-26 18:36:00.000000 pyvidplayer2-0.9.0/pyvidplayer2/video_tkinter.py
-drwxrwxrwx   0        0        0        0 2023-07-28 00:56:42.948755 pyvidplayer2-0.9.0/pyvidplayer2.egg-info/
--rw-rw-rw-   0        0        0     2477 2023-07-28 00:56:42.000000 pyvidplayer2-0.9.0/pyvidplayer2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-07-28 00:56:42.000000 pyvidplayer2-0.9.0/pyvidplayer2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 00:56:42.000000 pyvidplayer2-0.9.0/pyvidplayer2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-07-28 00:56:42.000000 pyvidplayer2-0.9.0/pyvidplayer2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 00:56:42.000000 pyvidplayer2-0.9.0/pyvidplayer2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 00:56:42.949755 pyvidplayer2-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-28 00:56:35.000000 pyvidplayer2-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:52:15.285997 pyvidplayer2-0.9.1/
+-rw-rw-rw-   0        0        0     1085 2023-07-19 21:30:21.000000 pyvidplayer2-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     2493 2023-07-30 14:52:15.285997 pyvidplayer2-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2160 2023-07-30 14:05:34.000000 pyvidplayer2-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 14:52:15.269986 pyvidplayer2-0.9.1/pyvidplayer2/
+-rw-rw-rw-   0        0        0      694 2023-07-30 13:39:04.000000 pyvidplayer2-0.9.1/pyvidplayer2/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-07-30 13:40:30.000000 pyvidplayer2-0.9.1/pyvidplayer2/audio_handler.py
+-rw-rw-rw-   0        0        0     1339 2023-07-30 13:44:08.000000 pyvidplayer2-0.9.1/pyvidplayer2/post_processing.py
+-rw-rw-rw-   0        0        0     2232 2023-07-29 04:31:47.000000 pyvidplayer2-0.9.1/pyvidplayer2/subtitles.py
+-rw-rw-rw-   0        0        0     7473 2023-07-30 14:34:13.000000 pyvidplayer2-0.9.1/pyvidplayer2/video.py
+-rw-rw-rw-   0        0        0     9560 2023-07-30 14:48:47.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_player.py
+-rw-rw-rw-   0        0        0     1336 2023-07-30 14:33:49.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_pygame.py
+-rw-rw-rw-   0        0        0     1531 2023-07-26 18:35:59.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_pyglet.py
+-rw-rw-rw-   0        0        0     1662 2023-07-30 14:49:19.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_pyqt.py
+-rw-rw-rw-   0        0        0     1500 2023-07-30 02:15:43.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_tkinter.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:52:15.284996 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/
+-rw-rw-rw-   0        0        0     2493 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:52:15.285997 pyvidplayer2-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-07-30 14:06:44.000000 pyvidplayer2-0.9.1/setup.py
```

### Comparing `pyvidplayer2-0.9.0/LICENSE` & `pyvidplayer2-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.0/PKG-INFO` & `pyvidplayer2-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.0
+Version: 0.9.1
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
@@ -23,27 +23,27 @@
 - Reliable playback
 - Fast load times
 - No audio/video sync issues
 - Low cpu usage
 - Subtitle support
 - Play multiple videos in parallel
 - Built in GUI
-- Support for Pygame, Pyglet, and Tkinter
+- Support for Pygame, Pyglet, Tkinter, and PyQT6
 - Can play all ffmpeg supported video formats
 - Post process effects
 
 # Installation
 ```
 pip install pyvidplayer2
 ```
 Note: FFMPEG must be installed and accessible via PATH.
 
 # Quickstart
 
-Refer to the examples folder for more basic guides, and docs.md contains more detailed information.
+Refer to the examples folder for more basic guides, and documentation.md contains more detailed information.
 
 ```
 import pygame
 from pyvidplayer2 import Video
 
 
 # create video object
```

### Comparing `pyvidplayer2-0.9.0/README.md` & `pyvidplayer2-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 - Reliable playback
 - Fast load times
 - No audio/video sync issues
 - Low cpu usage
 - Subtitle support
 - Play multiple videos in parallel
 - Built in GUI
-- Support for Pygame, Pyglet, and Tkinter
+- Support for Pygame, Pyglet, Tkinter, and PyQT6
 - Can play all ffmpeg supported video formats
 - Post process effects
 
 # Installation
 ```
 pip install pyvidplayer2
 ```
 Note: FFMPEG must be installed and accessible via PATH.
 
 # Quickstart
 
-Refer to the examples folder for more basic guides, and docs.md contains more detailed information.
+Refer to the examples folder for more basic guides, and documentation.md contains more detailed information.
 
 ```
 import pygame
 from pyvidplayer2 import Video
 
 
 # create video object
```

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2/__init__.py` & `pyvidplayer2-0.9.1/pyvidplayer2/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-import pygame 
-pygame.init()
-
 ffmpeg_path = "ffmpeg"
 
 def get_ffmpeg_path() -> str:
     return ffmpeg_path
 
 def set_ffmpeg_path(path: str) -> None:
+    global ffmpeg_path
     ffmpeg_path = path
 
-from .video import Video
+
 from .post_processing import PostProcessing 
-from .parallel_video import ParallelVideo 
-from .video_player import VideoPlayer 
-from .video_collection import VideoCollection
 from .video_tkinter import VideoTkinter
 
 try:
-    import srt 
+    import PyQt6
+except ImportError:
+    pass 
+else:
+    from .video_pyqt import VideoPyQT
+
+try:
+    import pygame
 except ImportError:
     pass 
 else:
+    pygame.init()
+
+    from .video_pygame import VideoPygame as Video
     from .subtitles import Subtitles
+    from .video_player import VideoPlayer
 
 try:
     import pyglet
 except ImportError:
     pass 
 else:
     from .video_pyglet import VideoPyglet
```

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2/post_processing.py` & `pyvidplayer2-0.9.1/pyvidplayer2/post_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         noise = numpy.zeros(data.shape, dtype=numpy.uint8)
         cv2.randn(noise, (0,) * 3, (20,) * 3)
         return data + noise
     
     def letterbox(data: numpy.ndarray) -> numpy.ndarray:
         background = numpy.zeros((*data.shape[:2], 3), dtype=numpy.uint8)
 
-        x1, y1 = 0, int(data.shape[0] * 0.15) #topleft crop
-        x2, y2 = data.shape[1], int(data.shape[0] * 0.85) #bottomright crop
+        x1, y1 = 0, int(data.shape[0] * 0.1) #topleft crop
+        x2, y2 = data.shape[1], int(data.shape[0] * 0.9) #bottomright crop
         data = data[y1:y2, x1:x2] # crops image
         background[y1:y1 + data.shape[0], x1:x1 + data.shape[1]] = data # draws image onto background
         return background
     
     def cel_shading(data: numpy.ndarray) -> numpy.ndarray:
         return cv2.subtract(data, cv2.blur(cv2.merge((cv2.Canny(data, 150, 200),) * 3), (2, 2)))
```

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2/subtitles.py` & `pyvidplayer2-0.9.1/pyvidplayer2/subtitles.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2/video.py` & `pyvidplayer2-0.9.1/pyvidplayer2/video.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import pygame 
 import cv2 
 import subprocess 
 import os
-import numpy
-from io import BytesIO
 from typing import Tuple 
 from threading import Thread
 from .post_processing import PostProcessing
+from .audio_handler import AudioHandler
 from . import get_ffmpeg_path
 
 
 class Video:
     def __init__(self, path: str, chunk_size=300, max_threads=1, max_chunks=1, subs=None, post_process=PostProcessing.none, interp=cv2.INTER_LINEAR) -> None:
         
         self.path = path
@@ -46,24 +44,17 @@
         self.buffering = False
         self.paused = False
 
         self.subs = subs
         self.post_func = post_process
         self.interp = interp
 
-        self.play()
-
-    def __str__(self) -> str:
-        return f"<Video(path={self.path})>"
+        self._audio = AudioHandler()
 
-    def _create_frame(self, data: numpy.ndarray) -> pygame.Surface:
-        return pygame.image.frombuffer(data.tobytes(), self.current_size, "BGR")
-    
-    def _render_frame(self, surf: pygame.Surface, pos: Tuple[int, int]) -> None:
-        surf.blit(self.frame_surf, pos)
+        self.play()
 
     def _chunks_len(self) -> int:
         i = 0
         for c in self._chunks:
             if c is not None:
                 i += 1
         return i
@@ -109,15 +100,15 @@
 
     def _update(self) -> bool:
         self._update_threads()
 
         n = False
         self.buffering = False
 
-        if pygame.mixer.music.get_busy() or self.paused:
+        if self._audio.get_busy() or self.paused:
 
             while self.get_pos() > self._vid.get(cv2.CAP_PROP_POS_FRAMES) * self.frame_delay:
 
                 has_frame, data = self._vid.read()
                 
                 if has_frame:
                     if self.original_size != self.current_size:
@@ -133,29 +124,22 @@
                     n = True
                 else:
                     break
 
         elif self.active:
             if self._chunks and self._chunks[0] is not None:
                 self._chunks_played += 1
-                pygame.mixer.music.load(BytesIO(self._chunks.pop(0)))
-                pygame.mixer.music.play()
+                self._audio.load(self._chunks.pop(0))
+                self._audio.play()
             elif self._stop_loading and self._chunks_played == self._chunks_claimed:
                 self.stop()
             else:
                 self.buffering = True
     
         return n
-
-    def draw(self, surf: pygame.Surface, pos: Tuple[int, int], force_draw=True) -> bool:
-        if self._update() or force_draw:
-            if self.frame_surf is not None:
-                self._render_frame(surf, pos)
-                return True
-        return False
     
     def play(self) -> None:
         self.active = True
 
     def stop(self) -> None:
         self.restart()
         self.active = False
@@ -167,77 +151,75 @@
 
     def change_resolution(self, height: int) -> None:
         self.current_size = (int(height * self.aspect_ratio), height)
 
     def close(self) -> None:
         self.stop()
         self._vid.release()
-        pygame.mixer.music.unload()
+        self._audio.unload()
         for t in self._threads:
             t.join()
 
     def restart(self) -> None:
         self.seek(0, relative=False)
         self.play()
 
     def set_volume(self, vol: float) -> None:
-        pygame.mixer.music.set_volume(vol)
+        self._audio.set_volume(vol)
 
     def get_volume(self) -> float:
-        return pygame.mixer.music.get_volume()
+        return self._audio.get_volume()
 
     def get_paused(self) -> bool:
         # here because the original pyvidplayer had get_paused
         return self.paused
     
     def toggle_pause(self) -> None:
         self.resume() if self.paused else self.pause()
 
     def pause(self) -> None:
         if self.active:
             self.paused = True
-            pygame.mixer.music.pause()
+            self._audio.pause()
 
     def resume(self) -> None:
         if self.active:
             self.paused = False
-
-            # unpausing when mixer hasn't loaded anything yet causes weird mixer behaviour
-
-            if pygame.mixer.music.get_pos() != -1:
-                pygame.mixer.music.unpause()
+            self._audio.unpause()
 
     def get_pos(self) -> float:
-        return min(self.duration, self._starting_time + max(0, self._chunks_played - 1) * self.chunk_size + max(0, pygame.mixer.music.get_pos()) / 1000)
+        return min(self.duration, self._starting_time + max(0, self._chunks_played - 1) * self.chunk_size + self._audio.get_pos())
 
     def seek(self, time: float, relative=True) -> None:
         # seeking accurate to 1 tenth of a second
 
         self._starting_time = self.get_pos() + time if relative else time
         self._starting_time = round(min(max(0, self._starting_time), self.duration), 1)
 
         for t in self._threads:
             t.join()
         self._chunks = []
         self._threads = []
         self._chunks_claimed = 0
         self._chunks_played = 0
-        pygame.mixer.music.stop()
+        self._audio.stop()
 
         self._vid.set(cv2.CAP_PROP_POS_FRAMES, self._starting_time * self.frame_rate)
         if self.subs is not None:
             self.subs._seek(self._starting_time)
 
-    def preview(self) -> None:
-        pygame.init()
-        win = pygame.display.set_mode(self.current_size)
-        pygame.display.set_caption(f"pygame - {self.name}")
-        self.play()
-        while self.active:
-            for event in pygame.event.get():
-                if event.type == pygame.QUIT:
-                    self.active = False
-            pygame.time.wait(16)
-            self.draw(win, (0, 0), force_draw=False)
-            pygame.display.update()
-        pygame.display.quit()
-        self.close()
+    def draw(self, surf, pos: Tuple[int, int], force_draw=True) -> bool:
+        if self._update() or force_draw:
+            if self.frame_surf is not None:
+                self._render_frame(surf, pos)
+                return True
+        return False
+
+    def _create_frame(self):
+        pass
+    
+    def _render_frame(self):
+        pass
+    
+    def preview(self):
+        pass 
+
```

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2/video_player.py` & `pyvidplayer2-0.9.1/pyvidplayer2/video_player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pygame
 import cv2 
 import math
 from typing import Tuple, List
-from .post_processing import PostProcessing
 from .video import Video
 
 
 class VideoPlayer:
     def __init__(self, video: Video, rect: Tuple[int, int, int, int], interactable=True, loop=False, preview_thumbnails=0) -> None:
 
         self.video = video
@@ -46,21 +45,29 @@
     def __str__(self) -> str:
         return f"<VideoPlayer(path={self.path})>"
     
     def _get_interval_frames(self):
         size = (int(70 * self.video.aspect_ratio), 70)
         for i in range(self.preview_thumbnails):
             self.video._vid.set(cv2.CAP_PROP_POS_FRAMES, int(i * self.video.frame_rate * self._interval))
-
+            
             self._interval_frames.append(pygame.image.frombuffer(cv2.resize(self.video._vid.read()[1], dsize=size, interpolation=cv2.INTER_AREA).tobytes(), size, "BGR"))
         
-        # add last frame
-        self.video._vid.set(cv2.CAP_PROP_POS_FRAMES, self.video.frame_count - 1)
-        self._interval_frames.append(pygame.image.frombuffer(cv2.resize(self.video._vid.read()[1], dsize=size, interpolation=cv2.INTER_AREA).tobytes(), size, "BGR"))
-        
+        # add last readable frame
+
+        i = 1
+        while True:
+            self.video._vid.set(cv2.CAP_PROP_POS_FRAMES, self.video.frame_count - i)
+            try:
+                self._interval_frames.append(pygame.image.frombuffer(cv2.resize(self.video._vid.read()[1], dsize=size, interpolation=cv2.INTER_AREA).tobytes(), size, "BGR"))
+            except:
+                i += 1
+            else:
+                break 
+
         self.video._vid.set(cv2.CAP_PROP_POS_FRAMES, 0)
     
     def _get_closest_frame(self, time):
         i = math.floor(time // self._interval)
         if (i + 1) * self._interval - time >= self._interval // 2:
             return self._interval_frames[i]
         else:
@@ -124,15 +131,15 @@
     def move(self, pos: Tuple[int, int], relative=False) -> None:
         if relative:
             self.frame_rect.move_ip(*pos)
         else:
             self.frame_rect.topleft = pos
         self._transform(self.frame_rect)
 
-    def update(self, events: List[pygame.event.Event] = None, show_ui=None) -> None:
+    def update(self, events: List[pygame.event.Event] = None, show_ui=None) -> bool:
         dt = self._clock.tick()
 
         if self.video._update() and self.video.current_size > self.frame_rect.size:
             self.video.frame_surf = self.video.frame_surf.subsurface(self.frame_rect.x - self.vid_rect.x, self.frame_rect.y - self.vid_rect.y, *self.frame_rect.size)
 
         if self.interactable:
 
@@ -170,14 +177,16 @@
                 self.video = Video(self.queue_.pop(0))
                 self._transform(self.frame_rect)
             elif self.loop:
                 self.video.restart()
 
         self._buffer_angle += dt / 10
 
+        return self._show_ui
+
     def draw(self, win: pygame.Surface) -> None:
         pygame.draw.rect(win, "black", self.frame_rect)
         if self.video.frame_surf is not None:
             win.blit(self.video.frame_surf, self.frame_rect.topleft if self.video.current_size > self.frame_rect.size else self.vid_rect.topleft)
 
         if self._show_ui:
             pygame.draw.line(win, (50, 50, 50), (self._progress_back.x, self._progress_back.centery), (self._progress_back.right, self._progress_back.centery), 5)
```

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2/video_pyglet.py` & `pyvidplayer2-0.9.1/pyvidplayer2/video_pyglet.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2/video_tkinter.py` & `pyvidplayer2-0.9.1/pyvidplayer2/video_tkinter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pygame
 import cv2
 import numpy
 import tkinter
 from .video import Video
 from typing import Tuple
 from .post_processing import PostProcessing
 
@@ -14,16 +13,16 @@
     def __str__(self) -> str:
         return f"<VideoTkinter(path={self.path})>"
 
     def _create_frame(self, data: numpy.ndarray) -> tkinter.PhotoImage:
         h, w = data.shape[:2]
         return tkinter.PhotoImage(width=w, height=h, data=f"P6 {w} {h} 255 ".encode() + cv2.cvtColor(data, cv2.COLOR_BGR2RGB).tobytes(), format='PPM')
 
-    def _render_frame(self, surf: pygame.Surface, pos: Tuple[int, int]) -> None:
-        surf.create_image(*pos, image=self.frame_surf)
+    def _render_frame(self, canvas: tkinter.Canvas, pos: Tuple[int, int]) -> None:
+        canvas.create_image(*pos, image=self.frame_surf)
 
     def preview(self) -> None:
         def update():
             self.draw(canvas, (self.current_size[0] / 2, self.current_size[1] / 2), force_draw=False)
             if self.active:
                 root.after(15, update) # for around 60 fps
             else:
```

### Comparing `pyvidplayer2-0.9.0/pyvidplayer2.egg-info/PKG-INFO` & `pyvidplayer2-0.9.1/pyvidplayer2.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.0
+Version: 0.9.1
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
@@ -23,27 +23,27 @@
 - Reliable playback
 - Fast load times
 - No audio/video sync issues
 - Low cpu usage
 - Subtitle support
 - Play multiple videos in parallel
 - Built in GUI
-- Support for Pygame, Pyglet, and Tkinter
+- Support for Pygame, Pyglet, Tkinter, and PyQT6
 - Can play all ffmpeg supported video formats
 - Post process effects
 
 # Installation
 ```
 pip install pyvidplayer2
 ```
 Note: FFMPEG must be installed and accessible via PATH.
 
 # Quickstart
 
-Refer to the examples folder for more basic guides, and docs.md contains more detailed information.
+Refer to the examples folder for more basic guides, and documentation.md contains more detailed information.
 
 ```
 import pygame
 from pyvidplayer2 import Video
 
 
 # create video object
```

### Comparing `pyvidplayer2-0.9.0/setup.py` & `pyvidplayer2-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 
 with open("README.md", 'r') as f:
     long_desc = f.read()
 
 
 setup(
     name="pyvidplayer2",
-    version="0.9.0",
+    version="0.9.1",
     description="Video playback in Python",
     long_description=long_desc,
     long_description_content_type = "text/markdown",
     author="Anray Liu",
     author_email="anrayliu@gmail.com",
     license="MIT",
     packages=["pyvidplayer2"],
     install_requires=["numpy>=1.24.3",
                     "opencv_python>=4.7.0.72",
                     "pygame>=2.4.0",
-                    "srt>=3.5.3"],
+                    "srt>=3.5.3",
+                    "PyAudio>=0.2.13"],
     url="https://github.com/ree1261/pyvidplayer2",
     platforms=["windows"],
     keywords=["pygame", "video", "playback"],
 )
```

