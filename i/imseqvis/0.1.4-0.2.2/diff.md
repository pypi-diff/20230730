# Comparing `tmp/imseqvis-0.1.4.tar.gz` & `tmp/imseqvis-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imseqvis-0.1.4.tar", last modified: Sat Jul 29 15:06:58 2023, max compression
+gzip compressed data, was "imseqvis-0.2.2.tar", last modified: Sun Jul 30 11:33:54 2023, max compression
```

## Comparing `imseqvis-0.1.4.tar` & `imseqvis-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:06:58.894827 imseqvis-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:06:58.890827 imseqvis-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:06:58.894827 imseqvis-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-29 15:06:49.000000 imseqvis-0.1.4/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-29 15:06:49.000000 imseqvis-0.1.4/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-29 15:06:49.000000 imseqvis-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 15:06:49.000000 imseqvis-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-29 15:06:58.894827 imseqvis-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-29 15:06:49.000000 imseqvis-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:06:58.894827 imseqvis-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-29 15:06:49.000000 imseqvis-0.1.4/examples/demo_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-29 15:06:49.000000 imseqvis-0.1.4/examples/demo_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)    75232 2023-07-29 15:06:49.000000 imseqvis-0.1.4/examples/screenshot.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:06:58.894827 imseqvis-0.1.4/imseqvis/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-29 15:06:49.000000 imseqvis-0.1.4/imseqvis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-07-29 15:06:49.000000 imseqvis-0.1.4/imseqvis/control_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-07-29 15:06:49.000000 imseqvis-0.1.4/imseqvis/image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-29 15:06:49.000000 imseqvis-0.1.4/imseqvis/sequence_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:06:58.894827 imseqvis-0.1.4/imseqvis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-29 15:06:58.000000 imseqvis-0.1.4/imseqvis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-29 15:06:58.000000 imseqvis-0.1.4/imseqvis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:06:58.000000 imseqvis-0.1.4/imseqvis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-29 15:06:58.000000 imseqvis-0.1.4/imseqvis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 15:06:58.000000 imseqvis-0.1.4/imseqvis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-29 15:06:49.000000 imseqvis-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 15:06:58.894827 imseqvis-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.065924 imseqvis-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-30 11:33:44.000000 imseqvis-0.2.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-30 11:33:44.000000 imseqvis-0.2.2/.github/workflows/publish-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-30 11:33:44.000000 imseqvis-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 11:33:44.000000 imseqvis-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-30 11:33:54.065924 imseqvis-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-30 11:33:44.000000 imseqvis-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-30 11:33:44.000000 imseqvis-0.2.2/examples/demo_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-30 11:33:44.000000 imseqvis-0.2.2/examples/demo_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75232 2023-07-30 11:33:44.000000 imseqvis-0.2.2/examples/screenshot.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/imseqvis/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/sequence_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/imseqvis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 11:33:44.000000 imseqvis-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:33:54.065924 imseqvis-0.2.2/setup.cfg
```

### Comparing `imseqvis-0.1.4/.github/workflows/publish-pypi.yml` & `imseqvis-0.2.2/.github/workflows/publish-pypi.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name: Publish Release to PyPI
-on: release
+on:
+  release:
+    types: [published]
 
 jobs:
   package-upload:
     name: Build and publish to PyPI
     runs-on: ubuntu-latest
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
```

### Comparing `imseqvis-0.1.4/.github/workflows/publish-test-pypi.yml` & `imseqvis-0.2.2/.github/workflows/publish-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `imseqvis-0.1.4/.gitignore` & `imseqvis-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `imseqvis-0.1.4/LICENSE` & `imseqvis-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imseqvis-0.1.4/PKG-INFO` & `imseqvis-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imseqvis
-Version: 0.1.4
+Version: 0.2.2
 Summary: A Qt-based image sequence visualizer widget
 Author-email: snototter <snototter@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 snototter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,42 +75,54 @@
 
 Optionally, you can install `imseqvis` with a specific backend. Currently,
 `pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
 ```bash
 # PyQt5
 python -m pip install "imseqvis[pyqt5]"
 
-# OR
-
-# PyQt6
+# OR PyQt6
 python -m pip install "imseqvis[pyqt6]"
 
-# OR
-
-# PySide2
+# OR PySide2
 python -m pip install "imseqvis[pyside2]"
 
-# OR
-
-# PySide6
+# OR PySide6
 python -m pip install "imseqvis[pyside6]"
 ```
 
 ### Usage as Standalone Application
-To quickly visualize all images within a folder (and nothing else), you can use the provided to start a standalone GUI application:
+To quickly visualize all images within a folder or sequence (and nothing else),
+you can use the provided wrappers to start a standalone GUI application:
+```python
+import imseqvis
+# Show all images in the given folder.
+imseqvis.show_folder('path/to/images')
+
+# Show all images in a random access container. For an exemplary data source
+# refer to `imseqvis.sequence_viewer.ImageSequence`.
+sequence = [...]
+imseqvis.show_sequence(sequence)
+```
+
+Alternatively, you could simply use the provided `show` functionality:
 ```python
 import imseqvis
 imseqvis.show('path/to/images')
+
+sequence = [...]
+imseqvis.show(sequence)
 ```
 
 ### Usage as Widget
-To integrate the viewer into your own application, use the `ImageSequenceViewer` widget.
+To integrate the viewer into your own application, use the `ImageSequenceViewer`
+widget:
 ```python
 # Prepare the image data source. This must allow random access to the images.
-# See the provided data sources within the examples/ folder for best practices.
+# For an exemplary data source refer to
+# `imseqvis.sequence_viewer.ImageSequence`.
 sequence = [...]
 
 # Create & use the widget.
 viewer = SequenceViewer(image_sequence=sequence)
 layout.addWidget(viewer)
 ...
 
@@ -122,12 +134,13 @@
 ```
 
 To show a different sequence within the same viewer, simply call:
 ```python
 viewer.setSequence(new_sequence)
 ```
 
-More detailed usage examples are provided within `examples/`:
+More detailed usage examples are provided within `examples/`. These also
+demonstrate how to use the available signals to be notified of the user's
+interactions with the viewer:
 * `examples/demo_standalone.py` demonstrates the basic usage with a dummy
   sequence.
 * `examples/demo_folder.py` will playback all images within a local folder.
-
```

### Comparing `imseqvis-0.1.4/README.md` & `imseqvis-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,42 +34,54 @@
 
 Optionally, you can install `imseqvis` with a specific backend. Currently,
 `pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
 ```bash
 # PyQt5
 python -m pip install "imseqvis[pyqt5]"
 
-# OR
-
-# PyQt6
+# OR PyQt6
 python -m pip install "imseqvis[pyqt6]"
 
-# OR
-
-# PySide2
+# OR PySide2
 python -m pip install "imseqvis[pyside2]"
 
-# OR
-
-# PySide6
+# OR PySide6
 python -m pip install "imseqvis[pyside6]"
 ```
 
 ### Usage as Standalone Application
-To quickly visualize all images within a folder (and nothing else), you can use the provided to start a standalone GUI application:
+To quickly visualize all images within a folder or sequence (and nothing else),
+you can use the provided wrappers to start a standalone GUI application:
+```python
+import imseqvis
+# Show all images in the given folder.
+imseqvis.show_folder('path/to/images')
+
+# Show all images in a random access container. For an exemplary data source
+# refer to `imseqvis.sequence_viewer.ImageSequence`.
+sequence = [...]
+imseqvis.show_sequence(sequence)
+```
+
+Alternatively, you could simply use the provided `show` functionality:
 ```python
 import imseqvis
 imseqvis.show('path/to/images')
+
+sequence = [...]
+imseqvis.show(sequence)
 ```
 
 ### Usage as Widget
-To integrate the viewer into your own application, use the `ImageSequenceViewer` widget.
+To integrate the viewer into your own application, use the `ImageSequenceViewer`
+widget:
 ```python
 # Prepare the image data source. This must allow random access to the images.
-# See the provided data sources within the examples/ folder for best practices.
+# For an exemplary data source refer to
+# `imseqvis.sequence_viewer.ImageSequence`.
 sequence = [...]
 
 # Create & use the widget.
 viewer = SequenceViewer(image_sequence=sequence)
 layout.addWidget(viewer)
 ...
 
@@ -81,12 +93,13 @@
 ```
 
 To show a different sequence within the same viewer, simply call:
 ```python
 viewer.setSequence(new_sequence)
 ```
 
-More detailed usage examples are provided within `examples/`:
+More detailed usage examples are provided within `examples/`. These also
+demonstrate how to use the available signals to be notified of the user's
+interactions with the viewer:
 * `examples/demo_standalone.py` demonstrates the basic usage with a dummy
   sequence.
 * `examples/demo_folder.py` will playback all images within a local folder.
-
```

### Comparing `imseqvis-0.1.4/examples/demo_folder.py` & `imseqvis-0.2.2/examples/demo_folder.py`

 * *Files identical despite different names*

### Comparing `imseqvis-0.1.4/examples/demo_standalone.py` & `imseqvis-0.2.2/examples/demo_standalone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This demo shows how to instantiate the SequenceViewer, create an
+application and use some of its signals.
+"""
 from imseqvis.sequence_viewer import SequenceViewer
 import numpy as np
 import sys
 
 from qtpy.QtWidgets import QApplication
```

### Comparing `imseqvis-0.1.4/examples/screenshot.jpg` & `imseqvis-0.2.2/examples/screenshot.jpg`

 * *Files identical despite different names*

### Comparing `imseqvis-0.1.4/imseqvis/control_widget.py` & `imseqvis-0.2.2/imseqvis/control_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from qtpy.QtWidgets import (
     QWidget, QHBoxLayout, QSlider, QLineEdit, QLabel, QToolButton)
-from qtpy.QtCore import Qt, Signal, QTimer
+from qtpy.QtCore import Qt, Signal, Slot, QTimer
 from qtpy.QtGui import QIcon, QFontMetrics
 
 
 class SequenceControlWidget(QWidget):
     """
     Playback/seeking controls for a sequence/video player.
 
@@ -63,101 +63,103 @@
         self.playback_timer = QTimer()
         self.playback_timer.timeout.connect(self.onPlaybackTimeout)
         self.playback_wait_for_viewer_ready = playback_wait_for_viewer_ready
         self.is_viewer_ready = True
 
         self.initUI(include_sequence_navigation_buttons, include_zoom_buttons)
 
+    @Slot(int)
     def setMaxValue(self, max_value):
         self.max_value = max_value
         self.slider.setRange(1, self.max_value)
         self.label_current_value.setFixedWidth(
             QFontMetrics(self.font()).width(str(self.max_value)) + 10)
         self.updateSlider(1)
 
+    @Slot()
     def onViewerReady(self):
         self.is_viewer_ready = True
 
     def initUI(
             self,
             include_sequence_navigation_buttons: bool,
             include_zoom_buttons: bool):
         # List of theme icon names:
         # https://standards.freedesktop.org/icon-naming-spec/icon-naming-spec-latest.html
 
-        # Automatic playback button (toggles between play/pause)
+        # Automatic playback button (toggles between play/pause).
         self.button_playback = QToolButton()
         self.button_playback.setIcon(QIcon.fromTheme('media-playback-start'))
         self.button_playback.setToolTip('Toggle play/pause')
         self.button_playback.clicked.connect(self.togglePlayback)
 
-        # Reset button
+        # Reset button to skip to the first frame.
         button_reload = QToolButton()
         button_reload.setIcon(QIcon.fromTheme('view-refresh'))
         button_reload.setToolTip('Reset sequence')
         button_reload.clicked.connect(self.resetSlider)
 
-        # Navigation buttons (step forward/backward)
+        # Navigation buttons (step forward/backward).
         self.button_previous_frame = QToolButton()
         self.button_previous_frame.setIcon(QIcon.fromTheme('go-previous'))
         self.button_previous_frame.setToolTip('Previous frame')
         self.button_previous_frame.clicked.connect(
             lambda: self.skip(self.button_previous_frame, -1))
 
         self.button_next_frame = QToolButton()
         self.button_next_frame.setIcon(QIcon.fromTheme('go-next'))
         self.button_next_frame.setToolTip('Next frame')
         self.button_next_frame.clicked.connect(
             lambda: self.skip(self.button_next_frame, +1))
 
-        # Navigation buttons (skip to previous/next sequence)
+        # Navigation buttons (skip to previous/next sequence).
         button_previous_sequence = QToolButton()
         button_previous_sequence.setIcon(QIcon.fromTheme('go-up'))
         button_previous_sequence.setToolTip('Previous sequence')
         button_previous_sequence.clicked.connect(self.previousSequenceRequest)
 
         button_next_sequence = QToolButton()
         button_next_sequence.setIcon(QIcon.fromTheme('go-down'))
         button_next_sequence.setToolTip('Next sequence')
         button_next_sequence.clicked.connect(self.nextSequenceRequest)
 
-        # The slider
+        # The slider.
         self.slider = QSlider(Qt.Horizontal)
         self.slider.setRange(1, self.max_value)
         self.slider.setMinimumWidth(100)
         self.slider.valueChanged.connect(
             lambda value: self.sliderValueChanged(value))
 
-        # Text box to manually set the slider value
+        # Text box to manually set the slider value.
         self.manual_input = QLineEdit()
         self.manual_input.setFixedWidth(100)
         self.manual_input.setPlaceholderText('Jump to:')
         self.manual_input.setToolTip('Enter frame to jump to')
         self.manual_input.returnPressed.connect(self.updateSliderFromTextBox)
 
-        # Label to display the current value
+        # Label to display the current value.
         max_label_width = QFontMetrics(self.font()).width(str(self.max_value))
         self.label_current_value = QLabel('')
-        # Add minor padding to the label
+        # Add minor padding to the label.
         self.label_current_value.setFixedWidth(max_label_width + 10)
         self.label_current_value.setAlignment(
             Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter)
 
-        # Buttons to zoom the image viewer
+        # Buttons to zoom the image viewer.
         button_zoom_fit = QToolButton()
         button_zoom_fit.setIcon(QIcon.fromTheme('zoom-fit-best'))
         button_zoom_fit.setToolTip('Fit to window')
         button_zoom_fit.clicked.connect(self.zoomFitToWindowRequest)
 
         button_zoom_original = QToolButton()
         button_zoom_original.setIcon(QIcon.fromTheme('zoom-original'))
         button_zoom_original.setToolTip('Show at original size')
         button_zoom_original.clicked.connect(self.zoomOriginalSizeRequest)
 
-        # Align all controls horizontally
+        # Align all controls horizontally.
         layout = QHBoxLayout()
         if include_sequence_navigation_buttons:
             layout.addWidget(button_previous_sequence)
             layout.addWidget(button_next_sequence)
         layout.addWidget(self.button_previous_frame)
         layout.addWidget(self.button_next_frame)
         layout.addWidget(self.button_playback)
@@ -169,42 +171,40 @@
         layout.addWidget(self.manual_input)
 
         if include_zoom_buttons:
             layout.addWidget(button_zoom_fit)
             layout.addWidget(button_zoom_original)
 
         self.setLayout(layout)
-        # Emit signal & update labels
+        # Emit signal & update labels.
         self.sliderValueChanged(1)
 
     def keyPressEvent(self, event):
         """Custom event filter for keyboard inputs."""
         # Do not use:
         # * Space - leads to different behavior depending on which sub-widget
         #   has the focus. For example, if a button was previously clicked,
         #   space will re-trigger the button.
         # * Return/Enter - will (re-)start the timer every time the user
         #   manually selects a frame via the text box.
         # * Left/Right/PageUp/PageDown - these are handled by the slider and
         #   overriding them here would be confusing for the user (e.g.
         #   inconsistent step sizes).
-        if event.key() == Qt.Key_Escape:
+        if event.key() in [Qt.Key_Escape, Qt.Key_R]:
             self.resetSlider()
         elif event.key() in [Qt.Key_P, Qt.Key_X]:
             self.togglePlayback()
         elif event.key() == Qt.Key_B:
             self.skip(self.button_previous_frame, -1)
         elif event.key() == Qt.Key_V:
             self.skip(self.button_previous_frame, -10)
         elif event.key() == Qt.Key_N:
             self.skip(self.button_next_frame, +1)
         elif event.key() == Qt.Key_M:
             self.skip(self.button_next_frame, +10)
-        elif event.key() == Qt.Key_R:
-            self.resetSlider()
 
     def sliderValueChanged(self, value):
         self.is_viewer_ready = False
         self.button_previous_frame.setEnabled(value > 1)
         self.button_next_frame.setEnabled(value < self.max_value)
         self.label_current_value.setText(str(value))
         self.indexChanged.emit(value)
@@ -213,53 +213,59 @@
         self.stopPlayback()
         self.updateSlider(1)
 
     def skip(self, button, step):
         if not button.isEnabled():
             return
         self.updateSlider(self.slider.value() + step)
-        # A manual fwd/bwd request always stops the playback
+        # A manual fwd/bwd request always stops the playback.
         self.stopPlayback()
 
     def stopPlayback(self):
         self.playback_timer.stop()
         self.button_playback.setIcon(QIcon.fromTheme('media-playback-start'))
 
     def startPlayback(self):
         if self.slider.value() >= self.max_value:
-            # Restart playback from the beginning
+            # Restart playback from the beginning.
             self.updateSlider(1)
         self.playback_timer.start(self.playback_timeout)
         self.button_playback.setIcon(QIcon.fromTheme('media-playback-pause'))
 
     def togglePlayback(self):
         if self.playback_timer.isActive():
             self.stopPlayback()
         else:
             self.startPlayback()
 
     def onPlaybackTimeout(self):
         if self.playback_wait_for_viewer_ready and not self.is_viewer_ready:
-            # Skip this timeout if the viewer has not shown the last image yet
+            # Skip this timeout if the viewer has not shown the last image yet.
             return
         value = self.slider.value() + 1
         if value <= self.max_value:
             self.updateSlider(value)
         else:
             self.stopPlayback()
 
     def updateSlider(self, value):
-        # Update the slider and label with the new value
+        # Update the slider and label with the new value.
         if 1 <= value <= self.max_value:
             self.slider.setValue(value)
             self.label_current_value.setText(str(value))
 
     def updateSliderFromTextBox(self):
-        # Get the value from the text box
+        # Get the value from the text box.
         try:
             value = int(self.manual_input.text())
             self.stopPlayback()
             self.updateSlider(value)
         except ValueError:
             pass
-        # Always reset the input text box
+        # Always reset the input text box.
         self.manual_input.setText('')
+    
+    @Slot()
+    def focusOnManualInput(self):
+        """Focus the manual input text box and select all text."""
+        self.manual_input.setFocus()
+        self.manual_input.selectAll()
```

### Comparing `imseqvis-0.1.4/imseqvis/image_viewer.py` & `imseqvis-0.2.2/imseqvis/image_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 
 def getLocalPathFromMimeData(mime_data: QMimeData) -> Path:
     """
     Returns the path of a file or folder dropped onto the canvas.
     """
     if mime_data.hasUrls():
-        # Return the first locally existing file
+        # Return the first locally existing file.
         for url in mime_data.urls():
             fpath = Path(url.toLocalFile())
             if fpath.exists():
                 return fpath
     if mime_data.hasText():
         txt = mime_data.text()
         if txt.startswith('file://'):
@@ -99,15 +99,15 @@
     pathDropped = Signal(Path)
 
     def __init__(self, parent=None) -> None:
         super().__init__(parent)
         self._scale = 1.0
         self._pixmap = QPixmap()
         self._painter = QPainter()
-        # Indicates whether the user is currently dragging the image
+        # Indicates whether the user is currently dragging the image.
         self._is_dragging = False
         # Previous dragging position, relative to the parent widget, i.e. the
         # position within the ImageViewer's scroll area.
         self._prev_drag_pos = None
         self.setMouseTracking(True)
         self.setAcceptDrops(True)
 
@@ -129,29 +129,29 @@
         """Returns the currently displayed pixmap."""
         return self._pixmap
 
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
         """Event handle for mouse move events."""
         pos = self.transformPos(event.pos())
         if Qt.RightButton & event.buttons():
-            # Skip mouse move signals while panning the image
+            # Skip mouse move signals while panning the image.
             self._is_dragging = True
             self.drag(event.pos())
         else:
             self.mouseMoved.emit(pos)
 
     def drag(self, new_pos: QPointF) -> None:
         """
         Handles dragging/panning the image.
 
         Emits the scroll request to properly adjusts the scroll bar
         positions according to the given mouse position.
         """
         new_pos = self.mapToParent(new_pos)
-        # Previous position will always be set when the mouse is pressed
+        # Previous position will always be set when the mouse is pressed.
         delta_pos = new_pos - self._prev_drag_pos
         dx = int(delta_pos.x())
         dy = int(delta_pos.y())
         if self.parent() is not None:
             pr = self.parent().rect()
             new_pos.setX(max(pr.left(), min(pr.right(), new_pos.x())))
             new_pos.setY(max(pr.top(), min(pr.bottom(), new_pos.y())))
@@ -162,15 +162,15 @@
         # mouse pointer...
         dx and self.scrollRequest.emit(dx * 6, Qt.Horizontal)
         dy and self.scrollRequest.emit(dy * 6, Qt.Vertical)
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
         """Event handler for mouse press events."""
         if event.button() == Qt.RightButton:
-            # Viewer can be panned via the right button
+            # Viewer can be panned via the right button.
             self._prev_drag_pos = self.mapToParent(event.pos())
             QApplication.setOverrideCursor(Qt.ClosedHandCursor)
 
     def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         """Event handler for mouse release events."""
         if not self._is_dragging:
             pos = self.transformPos(event.pos())
@@ -275,33 +275,33 @@
     A zoom- and scrollable widget to display image data.
 
     This class has been adapted (stripped down functionality & simplified) from
     the iminspect project:
     https://github.com/snototter/iminspect
     """
 
-    # Mouse moved to this pixel position
+    # Mouse moved to this pixel position.
     mouseMoved = Signal(QPointF)
 
     # Left mouse button clicked at this pixel position.
     mouseClickedLeft = Signal(QPointF)
 
     # Middle mouse button (wheel) clicked at this pixel position.
     mouseClickedMiddle = Signal(QPointF)
 
     # Right mouse button clicked at this pixel position.
     mouseClickedRight = Signal(QPointF)
 
-    # Scaling factor of displayed image changed
+    # Scaling factor of displayed image changed.
     imageScaleChanged = Signal(float)
 
-    # The view changed due to the user scrolling or zooming
+    # The view changed due to the user scrolling or zooming.
     viewChanged = Signal()
 
-    # A file or folder has been dropped onto the canvas
+    # A file or folder has been dropped onto the canvas.
     pathDropped = Signal(Path)
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self._img_np = None
         self._img_scale = 1.0
         self._min_img_scale = None
@@ -390,26 +390,26 @@
           reset_scale: If True, the zoom setting of the viewer will be reset.
         """
         pixmap = pixmapFromNumpy(img)
         self._img_np = img.copy()
         self._canvas.showPixmap(pixmap)
 
         # Ensure that image has a minimum size of about 32x32 px (unless it is
-        # actually smaller)
+        # actually smaller).
         self._min_img_scale = min(1.0, 32.0/img.shape[0], 32.0/img.shape[1])
 
         if reset_scale:
             self._img_scale = 1.0
         self.paintCanvas()
 
     def scaleToFitWindow(self) -> None:
         """Scale the image such that it fills the canvas area."""
         if self._img_np is None:
             return
-        eps = 2.0  # Prevent scrollbars
+        eps = 2.0  # Minor spacing needed to prevent showing scrollbars.
         w1 = self.width() - eps
         h1 = self.height() - eps
         a1 = w1 / h1
         w2 = float(self._canvas.pixmap().width())
         h2 = float(self._canvas.pixmap().height())
         a2 = w2 / h2
         self._img_scale = w1 / w2 if a2 >= a1 else h1 / h2
```

### Comparing `imseqvis-0.1.4/imseqvis.egg-info/PKG-INFO` & `imseqvis-0.2.2/imseqvis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imseqvis
-Version: 0.1.4
+Version: 0.2.2
 Summary: A Qt-based image sequence visualizer widget
 Author-email: snototter <snototter@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 snototter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,42 +75,54 @@
 
 Optionally, you can install `imseqvis` with a specific backend. Currently,
 `pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
 ```bash
 # PyQt5
 python -m pip install "imseqvis[pyqt5]"
 
-# OR
-
-# PyQt6
+# OR PyQt6
 python -m pip install "imseqvis[pyqt6]"
 
-# OR
-
-# PySide2
+# OR PySide2
 python -m pip install "imseqvis[pyside2]"
 
-# OR
-
-# PySide6
+# OR PySide6
 python -m pip install "imseqvis[pyside6]"
 ```
 
 ### Usage as Standalone Application
-To quickly visualize all images within a folder (and nothing else), you can use the provided to start a standalone GUI application:
+To quickly visualize all images within a folder or sequence (and nothing else),
+you can use the provided wrappers to start a standalone GUI application:
+```python
+import imseqvis
+# Show all images in the given folder.
+imseqvis.show_folder('path/to/images')
+
+# Show all images in a random access container. For an exemplary data source
+# refer to `imseqvis.sequence_viewer.ImageSequence`.
+sequence = [...]
+imseqvis.show_sequence(sequence)
+```
+
+Alternatively, you could simply use the provided `show` functionality:
 ```python
 import imseqvis
 imseqvis.show('path/to/images')
+
+sequence = [...]
+imseqvis.show(sequence)
 ```
 
 ### Usage as Widget
-To integrate the viewer into your own application, use the `ImageSequenceViewer` widget.
+To integrate the viewer into your own application, use the `ImageSequenceViewer`
+widget:
 ```python
 # Prepare the image data source. This must allow random access to the images.
-# See the provided data sources within the examples/ folder for best practices.
+# For an exemplary data source refer to
+# `imseqvis.sequence_viewer.ImageSequence`.
 sequence = [...]
 
 # Create & use the widget.
 viewer = SequenceViewer(image_sequence=sequence)
 layout.addWidget(viewer)
 ...
 
@@ -122,12 +134,13 @@
 ```
 
 To show a different sequence within the same viewer, simply call:
 ```python
 viewer.setSequence(new_sequence)
 ```
 
-More detailed usage examples are provided within `examples/`:
+More detailed usage examples are provided within `examples/`. These also
+demonstrate how to use the available signals to be notified of the user's
+interactions with the viewer:
 * `examples/demo_standalone.py` demonstrates the basic usage with a dummy
   sequence.
 * `examples/demo_folder.py` will playback all images within a local folder.
-
```

### Comparing `imseqvis-0.1.4/pyproject.toml` & `imseqvis-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "imseqvis"
 
 description = "A Qt-based image sequence visualizer widget"
 readme = "README.md"
 
-version = "0.1.4"
+version = "0.2.2"
 license = {file = "LICENSE"}
 
 authors = [
     { name = "snototter", email = "snototter@users.noreply.github.com" }
 ]
 
 requires-python = ">=3.7"
```

