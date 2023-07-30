# Comparing `tmp/fl_studio_api_stubs-28.2.0.tar.gz` & `tmp/fl_studio_api_stubs-28.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl_studio_api_stubs-28.2.0.tar", max compression
+gzip compressed data, was "fl_studio_api_stubs-28.2.1.tar", max compression
```

## Comparing `fl_studio_api_stubs-28.2.0.tar` & `fl_studio_api_stubs-28.2.1.tar`

### file list

```diff
@@ -1,98 +1,100 @@
--rw-r--r--   0        0        0     7642 2023-05-02 13:48:38.511676 fl_studio_api_stubs-28.2.0/LICENSE.md
--rwxr-xr-x   0        0        0     2817 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/README.md
--rw-r--r--   0        0        0     2482 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/pyproject.toml
--rw-r--r--   0        0        0     2921 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/arrangement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/arrangement/py.typed
--rw-r--r--   0        0        0     2391 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__init__.py
--rw-r--r--   0        0        0     1401 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__notes.py
--rw-r--r--   0        0        0    18932 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__properties.py
--rw-r--r--   0        0        0     5115 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__sequencer.py
--rw-r--r--   0        0        0     3167 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__ui.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/py.typed
--rw-r--r--   0        0        0     6348 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__device.py
--rw-r--r--   0        0        0     2984 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__dispatch.py
--rw-r--r--   0        0        0     5049 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__fl.py
--rw-r--r--   0        0        0     1510 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__init__.py
--rw-r--r--   0        0        0     1804 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__util.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/py.typed
--rw-r--r--   0        0        0      597 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__init__.py
--rw-r--r--   0        0        0     7538 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__sample.py
--rw-r--r--   0        0        0     3336 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__script_dialog.py
--rw-r--r--   0        0        0     1172 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__utils.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/py.typed
--rw-r--r--   0        0        0       42 2023-05-02 13:48:38.891699 fl_studio_api_stubs-28.2.0/src/fl_classes/.git
--rw-r--r--   0        0        0     1366 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/.gitignore
--rw-r--r--   0        0        0     7642 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/LICENSE.md
--rw-r--r--   0        0        0      283 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/README.md
--rw-r--r--   0        0        0    20163 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/py.typed
--rw-r--r--   0        0        0      611 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/__init__.py
--rw-r--r--   0        0        0     8350 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/channels.py
--rw-r--r--   0        0        0      444 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/__init__.py
--rw-r--r--   0        0        0      561 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/config_typings.py
--rw-r--r--   0        0        0      170 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/default.json
--rw-r--r--   0        0        0     1383 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/load_data.py
--rw-r--r--   0        0        0     1453 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/schema.json
--rw-r--r--   0        0        0      698 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/target_version.py
--rw-r--r--   0        0        0     5535 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/consts.py
--rw-r--r--   0        0        0     2930 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/decorators.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/device.py
--rw-r--r--   0        0        0     6524 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/emulation.py
--rw-r--r--   0        0        0     2683 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/exceptions.py
--rw-r--r--   0        0        0       40 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/helpers/__init__.py
--rw-r--r--   0        0        0     1114 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/helpers/file_from_here.py
--rw-r--r--   0        0        0     1331 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/channels.py
--rw-r--r--   0        0        0      604 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/device.py
--rw-r--r--   0        0        0     2406 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/general.py
--rw-r--r--   0        0        0     1633 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/mixer.py
--rw-r--r--   0        0        0     2688 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/pattern.py
--rw-r--r--   0        0        0      532 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/plugin.py
--rw-r--r--   0        0        0      618 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/transport.py
--rw-r--r--   0        0        0     1178 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/ui.py
--rw-r--r--   0        0        0     1407 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/patterns.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/py.typed
--rw-r--r--   0        0        0     1928 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/state.py
--rw-r--r--   0        0        0      337 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/util.py
--rw-r--r--   0        0        0     3947 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__fl_state.py
--rw-r--r--   0        0        0     1058 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__init__.py
--rw-r--r--   0        0        0     6860 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__undo.py
--rw-r--r--   0        0        0     2730 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__undo_proposed.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/py.typed
--rw-r--r--   0        0        0     3503 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/launchMapPages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/launchMapPages/py.typed
--rw-r--r--   0        0        0      462 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/midi/__encode.py
--rw-r--r--   0        0        0    17402 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/midi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/midi/py.typed
--rw-r--r--   0        0        0     3996 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/mixer/__events.py
--rw-r--r--   0        0        0     2796 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__init__.py
--rw-r--r--   0        0        0     3235 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__properties.py
--rw-r--r--   0        0        0     2041 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__selection.py
--rw-r--r--   0        0        0    12844 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__tracks.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/py.typed
--rw-r--r--   0        0        0     1433 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__groups.py
--rw-r--r--   0        0        0      318 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__helpers.py
--rw-r--r--   0        0        0     1409 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__init__.py
--rw-r--r--   0        0        0     1095 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__performance.py
--rw-r--r--   0        0        0     8216 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__properties.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/py.typed
--rw-r--r--   0        0        0    15286 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/playlist/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/playlist/py.typed
--rw-r--r--   0        0        0    14450 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/plugins/py.typed
--rw-r--r--   0        0        0      919 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/__init__.py
--rw-r--r--   0        0        0     3171 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/__position.py
--rw-r--r--   0        0        0     9142 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/__state.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/py.typed
--rw-r--r--   0        0        0     3178 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__browser.py
--rw-r--r--   0        0        0     1353 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__editors.py
--rw-r--r--   0        0        0     7516 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__fl_state.py
--rw-r--r--   0        0        0     3127 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__init__.py
--rw-r--r--   0        0        0     4836 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__keyboard.py
--rw-r--r--   0        0        0     3520 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__navigation.py
--rw-r--r--   0        0        0     2403 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__overlays.py
--rw-r--r--   0        0        0     5896 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__windows.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/py.typed
--rw-r--r--   0        0        0    11427 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/utils/py.typed
--rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 fl_studio_api_stubs-28.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7642 2023-07-30 16:38:23.864902 fl_studio_api_stubs-28.2.1/LICENSE.md
+-rwxr-xr-x   0        0        0     2817 2023-07-30 16:38:23.864902 fl_studio_api_stubs-28.2.1/README.md
+-rw-r--r--   0        0        0     2524 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2942 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/arrangement/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/arrangement/py.typed
+-rw-r--r--   0        0        0     2391 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/channels/__init__.py
+-rw-r--r--   0        0        0     1401 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/channels/__notes.py
+-rw-r--r--   0        0        0    19087 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/channels/__properties.py
+-rw-r--r--   0        0        0     5183 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/channels/__sequencer.py
+-rw-r--r--   0        0        0     3191 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/channels/__ui.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/channels/py.typed
+-rw-r--r--   0        0        0     6379 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/device/__device.py
+-rw-r--r--   0        0        0     2984 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/device/__dispatch.py
+-rw-r--r--   0        0        0     5049 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/device/__fl.py
+-rw-r--r--   0        0        0     1510 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/device/__init__.py
+-rw-r--r--   0        0        0     1804 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/device/__util.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/device/py.typed
+-rw-r--r--   0        0        0      685 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/enveditor/__init__.py
+-rw-r--r--   0        0        0     7538 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/enveditor/__sample.py
+-rw-r--r--   0        0        0     3336 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/enveditor/__script_dialog.py
+-rw-r--r--   0        0        0     1172 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/enveditor/__utils.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/enveditor/py.typed
+-rw-r--r--   0        0        0       42 2023-07-30 16:38:24.384907 fl_studio_api_stubs-28.2.1/src/fl_classes/.git
+-rw-r--r--   0        0        0     1366 2023-07-30 16:38:24.392907 fl_studio_api_stubs-28.2.1/src/fl_classes/.gitignore
+-rw-r--r--   0        0        0     7642 2023-07-30 16:38:24.392907 fl_studio_api_stubs-28.2.1/src/fl_classes/LICENSE.md
+-rw-r--r--   0        0        0      283 2023-07-30 16:38:24.392907 fl_studio_api_stubs-28.2.1/src/fl_classes/README.md
+-rw-r--r--   0        0        0    20163 2023-07-30 16:38:24.392907 fl_studio_api_stubs-28.2.1/src/fl_classes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:24.392907 fl_studio_api_stubs-28.2.1/src/fl_classes/py.typed
+-rw-r--r--   0        0        0      611 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/__init__.py
+-rw-r--r--   0        0        0     8350 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/channels.py
+-rw-r--r--   0        0        0      444 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/configuration/__init__.py
+-rw-r--r--   0        0        0      561 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/configuration/config_typings.py
+-rw-r--r--   0        0        0      170 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/configuration/default.json
+-rw-r--r--   0        0        0     1383 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/configuration/load_data.py
+-rw-r--r--   0        0        0     1453 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/configuration/schema.json
+-rw-r--r--   0        0        0      698 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/configuration/target_version.py
+-rw-r--r--   0        0        0     5535 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/consts.py
+-rw-r--r--   0        0        0     2930 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/decorators.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/device.py
+-rw-r--r--   0        0        0     6524 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/emulation.py
+-rw-r--r--   0        0        0     2683 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/exceptions.py
+-rw-r--r--   0        0        0       40 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/helpers/__init__.py
+-rw-r--r--   0        0        0     1114 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/helpers/file_from_here.py
+-rw-r--r--   0        0        0     1331 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/__init__.py
+-rw-r--r--   0        0        0     1746 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/channels.py
+-rw-r--r--   0        0        0      604 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/device.py
+-rw-r--r--   0        0        0     2406 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/general.py
+-rw-r--r--   0        0        0     1633 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/mixer.py
+-rw-r--r--   0        0        0     2688 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/pattern.py
+-rw-r--r--   0        0        0      532 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/plugin.py
+-rw-r--r--   0        0        0      618 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/transport.py
+-rw-r--r--   0        0        0     1178 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/models/ui.py
+-rw-r--r--   0        0        0     1407 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/patterns.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/py.typed
+-rw-r--r--   0        0        0     1928 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/state.py
+-rw-r--r--   0        0        0      337 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/fl_model/util.py
+-rw-r--r--   0        0        0     4123 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/general/__fl_state.py
+-rw-r--r--   0        0        0     1058 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/general/__init__.py
+-rw-r--r--   0        0        0     6860 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/general/__undo.py
+-rw-r--r--   0        0        0     2730 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/general/__undo_proposed.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/general/py.typed
+-rw-r--r--   0        0        0     3501 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/launchMapPages/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/launchMapPages/py.typed
+-rw-r--r--   0        0        0      462 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/midi/__encode.py
+-rw-r--r--   0        0        0    17402 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/midi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/midi/py.typed
+-rw-r--r--   0        0        0     4022 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/mixer/__events.py
+-rw-r--r--   0        0        0     2796 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/mixer/__init__.py
+-rw-r--r--   0        0        0     3235 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/mixer/__properties.py
+-rw-r--r--   0        0        0     2041 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/mixer/__selection.py
+-rw-r--r--   0        0        0    12837 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/mixer/__tracks.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/mixer/py.typed
+-rw-r--r--   0        0        0     1433 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/patterns/__groups.py
+-rw-r--r--   0        0        0      318 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/patterns/__helpers.py
+-rw-r--r--   0        0        0     1409 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/patterns/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/patterns/__performance.py
+-rw-r--r--   0        0        0     8216 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/patterns/__properties.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/patterns/py.typed
+-rw-r--r--   0        0        0    15239 2023-07-30 16:38:23.868902 fl_studio_api_stubs-28.2.1/src/playlist/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/playlist/py.typed
+-rw-r--r--   0        0        0    14682 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/plugins/py.typed
+-rw-r--r--   0        0        0     3974 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/screen/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/screen/py.typed
+-rw-r--r--   0        0        0      919 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/transport/__init__.py
+-rw-r--r--   0        0        0     3208 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/transport/__position.py
+-rw-r--r--   0        0        0     9141 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/transport/__state.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/transport/py.typed
+-rw-r--r--   0        0        0     3178 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__browser.py
+-rw-r--r--   0        0        0     1353 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__editors.py
+-rw-r--r--   0        0        0     7516 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__fl_state.py
+-rw-r--r--   0        0        0     3127 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__init__.py
+-rw-r--r--   0        0        0     4836 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__keyboard.py
+-rw-r--r--   0        0        0     3520 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__navigation.py
+-rw-r--r--   0        0        0     2403 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__overlays.py
+-rw-r--r--   0        0        0     5913 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/__windows.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/ui/py.typed
+-rw-r--r--   0        0        0    11403 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:38:23.872902 fl_studio_api_stubs-28.2.1/src/utils/py.typed
+-rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 fl_studio_api_stubs-28.2.1/PKG-INFO
```

### Comparing `fl_studio_api_stubs-28.2.0/LICENSE.md` & `fl_studio_api_stubs-28.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/README.md` & `fl_studio_api_stubs-28.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/pyproject.toml` & `fl_studio_api_stubs-28.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fl-studio-api-stubs"
-version = "28.2.0"
+version = "28.2.1"
 
 description = "Module and function definitions and documentation for the FL Studio Python API"
 readme = "README.md"
 
 authors = ["Miguel Guthridge <hdsq@outlook.com.au>"]
 license = "LGPL-3.0-only"
 
@@ -46,14 +46,15 @@
     { include = "general", from = "src" },
     { include = "launchMapPages", from = "src" },
     { include = "midi", from = "src" },
     { include = "mixer", from = "src" },
     { include = "patterns", from = "src" },
     { include = "playlist", from = "src" },
     { include = "plugins", from = "src" },
+    { include = "screen", from = "src" },
     { include = "transport", from = "src" },
     { include = "ui", from = "src" },
     { include = "utils", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Online Documentation" = "https://miguelguthridge.github.io/FL-Studio-API-Stubs/"
```

### Comparing `fl_studio_api_stubs-28.2.0/src/arrangement/__init__.py` & `fl_studio_api_stubs-28.2.1/src/arrangement/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
     Included since API version 1
     """
     return 0
 
 
 def currentTime(snap: int) -> int:
     """Returns the current time in the current arrangement, in terms of ticks.
-    Note that by default, most projects have a PPQ of 96. Use `general.getRecPPQ()`
-    to get the PPQ of the project.
+    Note that by default, most projects have a PPQ of 96. Use
+    [`general.getRecPPQ()`][general.getRecPPQ] to get the PPQ of the project.
 
     ## Args:
     * `snap` (`int`): whether to get time snapped to grid
 
     ## Returns:
     * `int`: current time
```

### Comparing `fl_studio_api_stubs-28.2.0/src/channels/__init__.py` & `fl_studio_api_stubs-28.2.1/src/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/channels/__notes.py` & `fl_studio_api_stubs-28.2.1/src/channels/__notes.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/channels/__properties.py` & `fl_studio_api_stubs-28.2.1/src/channels/__properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,19 @@
     getGroupedChannelReference(index).name = name
 
 
 def getChannelColor(index: int) -> int:
     """Returns the color of the channel at `index` (respecting groups)
 
     Note that colors can be split into or built from components using the
-    functions provided in the module `utils`
+    functions provided in the module [`utils`][utils]
 
-    * `ColorToRGB()`
+    * [`ColorToRGB()`][utils.ColorToRBG]
 
-    * `RGBToColor()`
+    * [`RGBToColor()`][utils.RGBToColor]
 
     ## Args:
      * `index` (`int`): index of channel
 
     ## Returns:
      * `int`: channel color (0x--BBGGRR)
 
@@ -124,19 +124,19 @@
     return getGroupedChannelReference(index).color
 
 
 def setChannelColor(index: int, color: int) -> None:
     """Sets the color of the channel at `index` (respecting groups)
 
     Note that colors can be split into or built from components using the
-    functions provided in the module `utils`
+    functions provided in the module [`utils`][utils]
 
-    * `ColorToRGB()`
+    * [`ColorToRGB()`][utils.ColorToRBG]
 
-    * `RGBToColor()`
+    * [`RGBToColor()`][utils.RGBToColor]
 
     ## Args:
      * `index` (`int`): index of channel
      * `color` (`int`): new color for channel (0x--BBGGRR)
 
     Included since API version 1
     """
@@ -276,15 +276,15 @@
     index_global = getChannelIndex(index)
     return getState().channels.channel_list[index_global].pan
 
 
 def setChannelPan(index: int, pan: float, pickupMode: int = midi.PIM_None) -> None:
     """Sets the normalized pan of the channel at `index`, where `-1.0` is
     100% left, and `1.0` is 100% right. Note that the default
-    pan for channels is `0.0` (centre). Use the pickup mode flag to set pickup
+    pan for channels is `0.0` (centered). Use the pickup mode flag to set pickup
     options.
 
     ## Args:
      * `index` (`int`): index of channel
 
      * `pan` (`float`): channel pan
 
@@ -451,15 +451,15 @@
     offset: int = 0,
     indexGlobal: bool = False
 ) -> int:
     """Returns the index of the first selected channel, otherwise the nth
     selected channel where n is `offset` + 1. If n is greater than the number
     of selected channels, the global index of the last selected channel will be
     returned. If `indexGlobal` is set to `1`, this will replicate the behavior
-    of `channelNumber()` by returning global indexes.
+    of [`channelNumber()`][channels.channelNumber] by returning global indexes.
 
     ## NOTE:
     * This function replaces the functionality of `channelNumber()`
       entirely, with the added functionality of providing indexes respecting
       groups (when `indexGlobal` is not set).
 
     ## Args:
@@ -602,15 +602,15 @@
 def incEventValue(eventId: int, step: int, res: float = 1 / 24) -> int:
     """Get event value increased by step. Use (optional) res parameter to
     specify increment resolution.
 
     This can be used to map encoder-style controls to events, by allowing them
     to adjust a parameter using a delta value
 
-    Use result as new value in `general.processRECEvent`.
+    Use result as new value in [`general.processRECEvent()`][general.processRECEvent].
 
     ## Example usage:
     ```py
     '''
     Increases the volume of the first channel
     '''
     delta = 1
```

### Comparing `fl_studio_api_stubs-28.2.0/src/channels/__sequencer.py` & `fl_studio_api_stubs-28.2.1/src/channels/__sequencer.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 
     * `padsStride` (`int`, optional): ?????. Defaults to 16.
 
     ## Returns:
     * `int`: value for step parameter
 
     ## See also:
-    * `getCurrentStepParam()`
-    * `setStepParameterByIndex()`
+    * [`getCurrentStepParam()`][channels.getCurrentStepParam]
+    * [`setStepParameterByIndex()`][channels.setStepParameterByIndex]
 
     ## Step parameter types:
     * `0`: Note pitch (MIDI note number, default 60 for middle C)
     * `1`: Velocity (0 - 127, default 100)
     * `2`: Release velocity (0 - 127, default 64)
     * `3`: Fine pitch (in cents: 0 - 240, with default 120 for no tuning)
     * `4`: Panning (0 - 127, with default 64 for centred)
```

### Comparing `fl_studio_api_stubs-28.2.0/src/channels/__ui.py` & `fl_studio_api_stubs-28.2.1/src/channels/__ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     checkGroupIndex(index)
 
 
 def showCSForm(index: int, state: int = 1) -> None:
     """Show the channel settings window (or plugin window for plugins) for
     channel at `index`.
 
-    This appears to perform the same action as `focusEditor()`.
+    This appears to perform the same action as [`focusEditor()`][channels.focusEditor].
 
     ## Args:
      * `index` (int): channel index
 
      * `state` (`int`, optional): whether to hide (`0`), show
         (`1`) or toggle (`-1`) the plugin window. Defaults to `1`.
```

### Comparing `fl_studio_api_stubs-28.2.0/src/device/__device.py` & `fl_studio_api_stubs-28.2.1/src/device/__device.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,20 @@
     Included since API version 1
     """
     return getState().device.assigned
 
 
 def getPortNumber() -> int:
     """Returns the port number for the input device that the script is attached
-    to. If the device requires two-way communication, the output port (where
-    functions like `midiOutMsg()` send their data to) should be set to the
-    value of the input port, which is returned by this function.
+    to.
+
+    If the device requires two-way communication, the output port (where
+    functions like [`midiOutMsg()`][device.midiOutMsg] send their data to)
+    should be set to the value of the input port, which is returned by this
+    function.
 
     ## Returns:
     * `int`: port number of the input device
 
     Included since API version 1
     """
     return getState().device.port
@@ -55,15 +58,15 @@
 ) -> None:
     """Sends a MIDI message to the linked output device.
 
     This can be done either through a single combined message, or in its
     distinct components.
 
     ## WARNING:
-    * Sending an invalid message will cause FL Studio to crash (API v20)
+    * Sending an invalid message will cause FL Studio to crash (FL Studio <= 20.9.2)
 
     ## Args:
     * `message` (`int`):
           * the MIDI message to send (if sending a complete message):
               * Lowest byte: `status`
 
               * Middle byte: `data 1`
@@ -169,15 +172,15 @@
     Included since API version 1
     """
 
 
 def stopRepeatMidiEvent() -> None:
     """Stop sending a currently repeating MIDI event.
 
-    Refer to `repeatMidiEvent()`.
+    Refer to [`repeatMidiEvent()`][device.repeatMidiEvent].
 
     Included since API version 1
     """
 
 
 @since(18)
 def setMasterSync(value: bool) -> None:
@@ -219,16 +222,14 @@
 
 @since(25)
 def getDeviceId() -> bytes:
     """
     Returns the unique device identifier of the connected device, as determined
     by FL Studio when connecting the device.
 
-    NOTE: This may change depending
-
     Note that this does not include the Sysex header, or ending byte.
 
     For example, if the device responded to a universal device enquiry with
 
     ```py
     bytes([
         0xF0, 0x7E, 0x01, 0x06, 0x02,
```

### Comparing `fl_studio_api_stubs-28.2.0/src/device/__dispatch.py` & `fl_studio_api_stubs-28.2.1/src/device/__dispatch.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/device/__fl.py` & `fl_studio_api_stubs-28.2.1/src/device/__fl.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/device/__init__.py` & `fl_studio_api_stubs-28.2.1/src/device/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/device/__util.py` & `fl_studio_api_stubs-28.2.1/src/device/__util.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/enveditor/__sample.py` & `fl_studio_api_stubs-28.2.1/src/enveditor/__sample.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/enveditor/__script_dialog.py` & `fl_studio_api_stubs-28.2.1/src/enveditor/__script_dialog.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/enveditor/__utils.py` & `fl_studio_api_stubs-28.2.1/src/enveditor/__utils.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_classes/.gitignore` & `fl_studio_api_stubs-28.2.1/src/fl_classes/.gitignore`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_classes/LICENSE.md` & `fl_studio_api_stubs-28.2.1/src/fl_classes/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_classes/__init__.py` & `fl_studio_api_stubs-28.2.1/src/fl_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/__init__.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/channels.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/channels.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/config_typings.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/configuration/config_typings.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/load_data.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/configuration/load_data.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/schema.json` & `fl_studio_api_stubs-28.2.1/src/fl_model/configuration/schema.json`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/target_version.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/configuration/target_version.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/consts.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/consts.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/decorators.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/decorators.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/emulation.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/emulation.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/exceptions.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/exceptions.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/helpers/file_from_here.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/helpers/file_from_here.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/__init__.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/channels.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/channels.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/device.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/device.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/general.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/general.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/mixer.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/mixer.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/pattern.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/pattern.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/plugin.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/plugin.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/transport.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/transport.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/models/ui.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/models/ui.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/patterns.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/patterns.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/fl_model/state.py` & `fl_studio_api_stubs-28.2.1/src/fl_model/state.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/general/__fl_state.py` & `fl_studio_api_stubs-28.2.1/src/general/__fl_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,18 @@
     Included since API version 1
     """
     return 0
 
 
 def getVersion() -> int:
     """Returns MIDI Scripting API version number. Note that this is the API
-    version, rather than the FL Studio version
+    version, rather than the FL Studio version.
+
+    To get the version of FL Studio, use [`ui.getVersion()`][ui.getVersion]
+    instead.
 
     ## Returns:
      * `int`: version number
 
     Included since API version 1
     """
     return getState().general.api_version
@@ -97,20 +100,20 @@
     "REC events" represent every automatable control in FL studio.
     Each "REC" is identified with a unique integer, "event ID".
     FL Studio reserves a range of event IDs for each channel, mixer track, plugin,
     and so on.
 
     REC events have some other properties available:
 
-    * Descriptive name: `device.getLinkedParamName()`
+    * Descriptive name: [`device.getLinkedParamName()`][device.getLinkedParamName]
 
-    * Current value: `device.getLinkedValue()`
+    * Current value: [`device.getLinkedValue()`][device.getLinkedValue]
 
     * Current value as an appropriately formatted string:
-      `device.getLinkedValueString()`
+      [`device.getLinkedValueString()`][device.getLinkedValueString]
 
     ## HELP WANTED:
     * More information from Image-Line? More details on what `flags` can do?
 
     ## Args:
      * `eventId` (`int`): Refer to the [official documentation](https://www.image-line.com/fl-studio-learning/fl-studio-online-manual/html/midi_scripting.htm#RecEventParams)
```

### Comparing `fl_studio_api_stubs-28.2.0/src/general/__init__.py` & `fl_studio_api_stubs-28.2.1/src/general/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/general/__undo.py` & `fl_studio_api_stubs-28.2.1/src/general/__undo.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/general/__undo_proposed.py` & `fl_studio_api_stubs-28.2.1/src/general/__undo_proposed.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/launchMapPages/__init__.py` & `fl_studio_api_stubs-28.2.1/src/launchMapPages/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,23 +58,23 @@
      * `index` (`int`): index of page to update
 
     Included since API version 1
     """
 
 
 def getMapItemColor(index: int, itemIndex: int) -> int:
-    """Returns item colour of `itemIndex` in map `index`
+    """Returns item color of `itemIndex` in map `index`
 
     ## Args:
      * `index` (`int`): map index
 
      * `itemIndex` (`int`): item index
 
     ## Returns:
-     * `int`: colour
+     * `int`: color
 
     Included since API version 1
     """
     return 0
 
 
 def getMapCount(index: int) -> int:
```

### Comparing `fl_studio_api_stubs-28.2.0/src/midi/__init__.py` & `fl_studio_api_stubs-28.2.1/src/midi/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/mixer/__events.py` & `fl_studio_api_stubs-28.2.1/src/mixer/__events.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 
 def getTrackPluginId(index: int, plugIndex: int) -> int:
     """Returns the plugin ID of the plugin on track `index` in slot `plugIndex`
 
     A plugin ID is used internally by FL Studio to represent effects present
     on the mixer. A plugin ID can be used with REC events in order to automate
-    plugins, and is also the return value of `ui.getFocusedFormID()` if the
-    focused window is an effect plugin.
+    plugins, and is also the return value of
+    [`ui.getFocusedFormID()`][ui.getFocusedFormID] if the focused window is an
+    effect plugin.
 
     Plugin IDs are represented as `((track << 6) + index) << 16`, although
     the official documentation lists them as `(track << 6 + index) << 16`,
     which uses the order of operations incorrectly.
 
     ## Args:
      * index (`int`): track index
@@ -96,15 +97,15 @@
     """Returns event name for event at `index`
 
     ## HELP WANTED:
     * What does this do?
 
     ## NOTE:
     * The official documentation states that this function returns `None`,
-      but it actually returns a `str`. These stubs document the actual behaviour.
+      but it actually returns a `str`. These stubs document the actual behavior.
 
     ## Args:
      * `index` (`int`): ???
 
      * `shortname` (`int`, optional): ???. Defaults to 0.
 
     ## Returns:
```

### Comparing `fl_studio_api_stubs-28.2.0/src/mixer/__init__.py` & `fl_studio_api_stubs-28.2.1/src/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/mixer/__properties.py` & `fl_studio_api_stubs-28.2.1/src/mixer/__properties.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/mixer/__selection.py` & `fl_studio_api_stubs-28.2.1/src/mixer/__selection.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/mixer/__tracks.py` & `fl_studio_api_stubs-28.2.1/src/mixer/__tracks.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,34 +33,34 @@
      * name (`str`): new name
 
     Included since API version 1
     """
 
 
 def getTrackColor(index: int) -> int:
-    """Returns the colour of the track at `index`.
+    """Returns the color of the track at `index`.
 
     ## Args:
      * `index` (`int`): track index
 
     ## Returns:
-     * `int`: colour of track (0x--BBGGRR)
+     * `int`: color of track (0x--BBGGRR)
 
     Included since API version 1
     """
     return 0
 
 
 def setTrackColor(index: int, color: int) -> None:
-    """Sets the colour of the track at `index`.
+    """Sets the color of the track at `index`.
 
     ## Args:
      * `index` (`int`): track index
 
-     * `color` (`int`): colour of track (0x--BBGGRR)
+     * `color` (`int`): color of track (0x--BBGGRR)
 
     Included since API version 1
     """
 
 
 def isTrackArmed(index: int) -> bool:
     """Returns whether the track at `index` is armed for recording
@@ -230,15 +230,15 @@
     flag to set pickup options.
 
     ## Args:
      * `index` (`int`): track index
 
      * `volume` (`float`): volume of track
 
-     * `pickupMode` (`int`, optional): define the pickup behaviour. Refer to
+     * `pickupMode` (`int`, optional): define the pickup behavior. Refer to
        the [manual](https://www.image-line.com/fl-studio-learning/fl-studio-online-manual/html/midi_scripting.htm#pickupModes)
 
 
     Included since API version 1
     """
 
 
@@ -268,15 +268,15 @@
     `0.0`. Use the pickup mode flag to set pickup options.
 
     ## Args:
      * `index` (`int`): track index
 
      * `pan` (`float`): pan of track
 
-     * `pickupMode` (`int`, optional): define the pickup behaviour. Refer to
+     * `pickupMode` (`int`, optional): define the pickup behavior. Refer to
        the [manual](https://www.image-line.com/fl-studio-learning/fl-studio-online-manual/html/midi_scripting.htm#pickupModes)
 
 
     Included since API version 1
     """
 
 
@@ -309,15 +309,15 @@
     options.
 
     ## Args:
      * `index` (`int`): track index
 
      * `sep` (`float`): stereo separation of track
 
-     * `pickupMode` (`int`, optional): define the pickup behaviour. Refer to
+     * `pickupMode` (`int`, optional): define the pickup behavior. Refer to
        the [manual](https://www.image-line.com/fl-studio-learning/fl-studio-online-manual/html/midi_scripting.htm#pickupModes)
 
     Included since API version 12
     """
 
 
 def setRouteTo(index: int, destIndex: int, value: int) -> None:
```

### Comparing `fl_studio_api_stubs-28.2.0/src/patterns/__groups.py` & `fl_studio_api_stubs-28.2.1/src/patterns/__groups.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/patterns/__init__.py` & `fl_studio_api_stubs-28.2.1/src/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/patterns/__performance.py` & `fl_studio_api_stubs-28.2.1/src/patterns/__performance.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/patterns/__properties.py` & `fl_studio_api_stubs-28.2.1/src/patterns/__properties.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/playlist/__init__.py` & `fl_studio_api_stubs-28.2.1/src/playlist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,55 +64,55 @@
      * `TypeError`: Index out of range
 
     Included since API version 1
     """
 
 
 def getTrackColor(index: int) -> int:
-    """Returns the colour of the track at `index`
+    """Returns the color of the track at `index`
 
-    Note that colours can be split into or built from components using the
+    Note that colors can be split into or built from components using the
     functions provided in the module `utils`
 
     * `ColorToRGB()`
 
     * `RGBToColor()`
 
     Note that playlist track indexes start at 1
 
     ## Args:
      * `index` (`int`): track index
 
     ## Returns:
-     * `int`: track colour (0x--BBGGRR)
+     * `int`: track color (0x--BBGGRR)
 
     ## Raises:
      * `TypeError`: Index out of range
 
     Included since API version 1
     """
     return 0
 
 
 def setTrackColor(index: int, color: int) -> None:
-    """Sets the colour of the track at `index`
+    """Sets the color of the track at `index`
 
-    Note that colours can be split into or built from components using the
+    Note that colors can be split into or built from components using the
     functions provided in the module `utils`
 
     * `ColorToRGB()`
 
     * `RGBToColor()`
 
     Note that playlist track indexes start at 1
 
     ## Args:
      * `index` (`int`): track index
 
-     * `color` (`int`): track colour (0x--BBGGRR)
+     * `color` (`int`): track color (0x--BBGGRR)
 
     ## Raises:
      * `TypeError`: Index out of range
 
     Included since API version 1
     """
 
@@ -523,33 +523,33 @@
 
     Included since API version 1
     """
     return 0
 
 
 def getLiveBlockColor(index: int, blockNum: int) -> int:
-    """Returns the colour of block on track `index` at position `blockNum`
+    """Returns the color of block on track `index` at position `blockNum`
 
     ## HELP WANTED:
     * What does this do?
 
-    Note that colours can be split into or built from components using the
+    Note that colors can be split into or built from components using the
     functions provided in the module `utils`
 
     * `ColorToRGB()`
 
     * `RGBToColor()`
 
     ## Args:
      * `index` (`int`): track index
 
      * `blockNum` (`int`): block number
 
     ## Returns:
-     * `int`: block colour (`0x--BBGGRR`)
+     * `int`: block color (`0x--BBGGRR`)
 
     Included since API version 1
     """
     return 0
 
 
 def triggerLiveClip(index: int, subNum: int, flags: int, velocity: int = -1) -> None:
@@ -694,12 +694,9 @@
     """
     Returns whether FL Studio's performance mode is enabled
 
     ## Returns:
     * `bool`: whether performance mode is enabled
 
     Included since API Version 21
-
-    ## API Changes:
-    * v_: change
     """
     return False
```

### Comparing `fl_studio_api_stubs-28.2.0/src/plugins/__init__.py` & `fl_studio_api_stubs-28.2.1/src/plugins/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 
 @since(8)
 def setParamValue(
     value: float,
     paramIndex: int,
     index: int,
     slotIndex: int = -1,
+    pickupMode: int = 0,
     useGlobalIndex: bool = False,
 ) -> None:
     """Sets the value of the parameter at `paramIndex` for the plugin at
     `index`/`slotIndex`.
 
     ## Warnings:
     * This appears to have poor performance before FL Studio 21, being 40x
@@ -227,14 +228,20 @@
 
     * `paramIndex` (`int`): index of parameter
 
     * `index` (`int`): index of plugin on channel rack or mixer
 
     * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
 
+    * `pickupMode` (`int`, optional): pickup mode to use:
+
+          * `0`: do not use pickup
+          * `1`: always use pickup
+          * `2`: use pickup if FL Studio is configured to do so
+
     * `useGlobalIndex` (`bool`, optional): whether to use global channel
       indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     Included since API version 8
     """
 
 
@@ -324,36 +331,36 @@
     * Fixing the markdown formatting here: I can't get it to behave in VS Code.
 
     ## Args:
     * `index` (`int`): index of plugin on channel rack or mixer
 
     * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
 
-    * `flag` (`int`, optional): name type to return. Names marked with a *
+    * `flag` (`int`, optional): name type to return. Names marked with a `!`
       require the `paramIndex` parameter in order to work correctly.
-          * `FPN_Param` (`0`, default) * : Name of plugin parameter.
+          * `FPN_Param` (`0`, default) `*` : Name of plugin parameter.
               * Eg: `"Expression"`
 
-          * `FPN_ParamValue` (`1`) * : Text value of plugin parameter.
+          * `FPN_ParamValue` (`1`) `*` : Text value of plugin parameter.
               * Eg: `"62%"`
 
-          * `FPN_Semitone` (`2`) * : Name of note as defined by plugin.
+          * `FPN_Semitone` (`2`) `*` : Name of note as defined by plugin.
               * `paramIndex` should be the note number (eg `60` for middle C)
 
               * If note names aren't defined by the plugin, an empty string is given.
 
               * Eg: `"Kick"`
 
           * `FPN_Patch` (`3`): Name of the patch defined by plugin?
 
-          * `FPN_VoiceLevel` (`4`) * : Name of per-voice parameter defined by plugin
+          * `FPN_VoiceLevel` (`4`) `*` : Name of per-voice parameter defined by plugin
 
-          * `FPN_VoiceLevelHint` (`5`) * : Hint for per-voice parameter defined by plugin
+          * `FPN_VoiceLevelHint` (`5`) `*` : Hint for per-voice parameter defined by plugin
 
-          * `FPN_Preset` (`6`) * : For plugins that support internal presets, the name of the preset at `paramIndex`.
+          * `FPN_Preset` (`6`) `*` : For plugins that support internal presets, the name of the preset at `paramIndex`.
               * Eg: `"Dystopian lead"`
 
           * `FPN_OutCtrl` (`7`): For plugins that output controllers, the name of the output controller?
 
           * `FPN_VoiceColor` (`8`): Name of per-voice color
               * `paramIndex` as MIDI channel?
 
@@ -383,15 +390,15 @@
     useGlobalIndex: bool = False,
 ) -> int:
     """
     Returns info about drum pads
 
     Currently only supported by FPC
 
-    ## Notes:
+    ## Note:
     * The official documentation lists this as returning a string, but it
       actually returns an int.
 
     ## Args:
     * `chanIndex` (`int`): channel of plugin to check
 
     * `slotIndex` (`int`, optional): slot of mixer track plugin. Defaults to `-1`.
```

### Comparing `fl_studio_api_stubs-28.2.0/src/transport/__init__.py` & `fl_studio_api_stubs-28.2.1/src/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/transport/__position.py` & `fl_studio_api_stubs-28.2.1/src/transport/__position.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,17 +96,17 @@
 
     ## WARNING:
     * It is not recommended to use this function if a dedicated
       function is available for it. Its usage can make code difficult to read and
       comprehend. Almost all functionality provided by this function can be done
       more easily and cleanly by using the dedicated functions.
 
-    * Some commands will echo keypresses (such as `FPT_F1`), meaning they
-      can affect windows outside FL Studio. Make sure you test your code
-      thoroughly if you decide to use this function.
+    * Some commands will echo key-presses (such as `FPT_F1`), meaning they
+      can affect windows outside FL Studio in versions before FL Studio 21.0.0.
+      Make sure you test your code thoroughly if you decide to use this function.
 
     ## Args:
     * `command` (`int`): command to execute, refer to
       [official documentation](https://www.image-line.com/fl-studio-learning/fl-studio-online-manual/html/midi_scripting.htm#globalTransportCommands)
 
     * `value` (`int`): ???
```

### Comparing `fl_studio_api_stubs-28.2.0/src/transport/__state.py` & `fl_studio_api_stubs-28.2.1/src/transport/__state.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
           * `SONGLENGTH_STEPS` (`4`): bars-steps-ticks format, steps component
 
           * `SONGLENGTH_TICKS` (`5`): bars-steps-ticks format, ticks component
 
     ## NOTE:
     * The official documentation states that this function has no return,
-      but in practice, it returns an `int`. The actual behaviour is used by this
+      but in practice, it returns an `int`. The actual behavior is used by this
       documentation.
 
     ## Returns:
      * `int`: song length
 
     Included since API version 3
     """
```

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__browser.py` & `fl_studio_api_stubs-28.2.1/src/ui/__browser.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__editors.py` & `fl_studio_api_stubs-28.2.1/src/ui/__editors.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__fl_state.py` & `fl_studio_api_stubs-28.2.1/src/ui/__fl_state.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__init__.py` & `fl_studio_api_stubs-28.2.1/src/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__keyboard.py` & `fl_studio_api_stubs-28.2.1/src/ui/__keyboard.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__navigation.py` & `fl_studio_api_stubs-28.2.1/src/ui/__navigation.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__overlays.py` & `fl_studio_api_stubs-28.2.1/src/ui/__overlays.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.2.0/src/ui/__windows.py` & `fl_studio_api_stubs-28.2.1/src/ui/__windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 def getFocused(index: int) -> bool:
     """Returns whether an FL Studio window is focused (meaning it is the
     currently selected Window in FL Studio).
 
     ## NOTE:
     * this doesn't necessarily mean that it is the currently selected window
       in the host operating system, so functions that rely on keypress emulation
-      (such as `ui.copy()`) may not work as intended, even if this returns `True`.
+      (such as [`ui.copy()`][ui.copy]) may not work as intended, even if this
+      returns `True`.
 
     ## Args:
      * `index` (`int`): window index:
           * `widMixer` (`0`): Mixer
 
           * `widChannelRack` (`1`): Channel Rack
```

### Comparing `fl_studio_api_stubs-28.2.0/src/utils/__init__.py` & `fl_studio_api_stubs-28.2.1/src/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 package in the hope that it will be useful for script developers. It is not the
 creation of the repository authors, and no credit is claimed for the code
 content. However, the documentation for the provided code is created by the
 authors of this repository.
 
 ## WARNING:
 Many of the provided functions in the FL Studio installation have bugs
-that may result in unexpected behaviour. These bugs have been left as-is in this
+that may result in unexpected behavior. These bugs have been left as-is in this
 file for your inspection and warnings have been added to the docstrings. Use
 any functions here with caution.
 """
 
 # import warnings
 #
 # warnings.warn("The utils module contains exceptionally buggy code. Usage is "
@@ -298,15 +298,15 @@
     R.Left = R.Left + dx
     R.Top = R.Top + dy
     R.Right = R.Right + dx
     R.Bottom = R.Bottom + dy
 
 
 def RGBToHSV(R: float, G: float, B: float) -> 'tuple[float, float, float]':
-    """Convert an RGB colour to a HSV colour
+    """Convert an RGB color to a HSV color
 
     WARNING: Make sure to convert
 
     ## Args:
      * R (float): red (0.0 - 1.0)
 
      * G (float): green (0.0 - 1.0)
@@ -343,18 +343,18 @@
         if H < 0.0:  # type: ignore
             H = H + 360.0  # type: ignore
 
     return H, S, V  # type: ignore
 
 
 def RGBToHSVColor(Color: int) -> 'tuple[float, float, float]':
-    """Convert an RGB colour to a HSV colour
+    """Convert an RGB color to a HSV color
 
     ## Args:
-     * Color (int): colour as integer (`0x--BBGGRR`)
+     * Color (int): color as integer (`0x--BBGGRR`)
 
     ## Returns:
      * H: hue
 
      * S: saturation
 
      * V: value (brightness)
@@ -363,15 +363,15 @@
     g = ((Color & 0x00FF00) >> 8) / 255
     b = ((Color & 0x0000FF) >> 0) / 255
     H, S, V = RGBToHSV(r, g, b)
     return H, S, V
 
 
 def HSVtoRGB(H: float, S: float, V: float) -> 'tuple[float, float, float]':
-    """Convert an HSV colour to an RGB colour
+    """Convert an HSV color to an RGB color
 
     WARNING: This function returns data in an unexpected format! Be sure to
     convert as required before usage.
 
     ## Args:
      * H (float): hue (degrees: 0.0-360)
 
@@ -445,80 +445,80 @@
      * str: note name
     """
     NoteNum += 1200
     return NoteNameT[NoteNum % 12] + str((NoteNum // 12) - 100)
 
 
 def ColorToRGB(Color: int) -> 'tuple[int, int, int]':
-    """Convert an integer colour to an RGB tuple that uses range 0-255.
+    """Convert an integer color to an RGB tuple that uses range 0-255.
 
     ## Args:
-     * Color (int): colour as integer
+     * Color (int): color as integer
 
     ## Returns:
      * int: red
 
      * int: green
 
      * int: blue
     """
     return (Color >> 16) & 0xFF, (Color >> 8) & 0xFF, Color & 0xFF
 
 
 def RGBToColor(R: int, G: int, B: int) -> int:
-    """convert an RGB set to an integer colour. values must be 0-255
+    """convert an RGB set to an integer color. values must be 0-255
 
     ## Args:
      * R (int): red
 
      * G (int): green
 
      * B (int): blue
 
     ## Returns:
-     * int: colour
+     * int: color
     """
     return (R << 16) | (G << 8) | B
 
 
 def FadeColor(StartColor: int, EndColor: int, Value: float) -> int:
-    """Fade between two colour values
+    """Fade between two colorlues
 
     ## Args:
-     * StartColor (int): colour integer
+     * StartColor (int): colornteger
 
-     * EndColor (int): colour integer
+     * EndColor (int): color integer
 
      * Value (float): fade position (0-255)
 
     ## Returns:
-     * int: faded colour
+     * int: faded color
 
     WARNING:
      * Blue value is incorrect, using green start value
     """
     rStart, gStart, bStart = ColorToRGB(StartColor)
     rEnd, gEnd, bEnd = ColorToRGB(EndColor)
     ratio = Value / 255
     rEnd = round(rStart * (1 - ratio) + (rEnd * ratio))
     gEnd = round(gStart * (1 - ratio) + (gEnd * ratio))
     bEnd = round(gStart * (1 - ratio) + (bEnd * ratio))
     return RGBToColor(rEnd, gEnd, bEnd)
 
 
 def LightenColor(Color: int, Value: float) -> int:
-    """Lighten a colour by a certain amount
+    """Lighten a color by a certain amount
 
     ## Args:
-     * Color (int): colour integer
+     * Color (int): color integer
 
      * Value (float): amount to lighten by (0-255)
 
     ## Returns:
-     * int: lightened colour
+     * int: lightened color
     """
     r, g, b = ColorToRGB(Color)
     ratio = Value / 255
     return RGBToColor(round(r + (1.0 - r) * ratio), round(g + (1.0 - g) * ratio), round(b + (1.0 - b) * ratio))
 
 
 def VolTodB(Value: float) -> float:
```

### Comparing `fl_studio_api_stubs-28.2.0/PKG-INFO` & `fl_studio_api_stubs-28.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl-studio-api-stubs
-Version: 28.2.0
+Version: 28.2.1
 Summary: Module and function definitions and documentation for the FL Studio Python API
 Home-page: https://github.com/MiguelGuthridge/FL-Studio-Api-Stubs
 License: LGPL-3.0-only
 Keywords: fl-studio,midi,api,documentation,stubs,fl,studio,daw,controller
 Author: Miguel Guthridge
 Author-email: hdsq@outlook.com.au
 Requires-Python: >=3.9.1,<4.0.0
@@ -13,15 +13,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Stubs Only
 Classifier: Typing :: Typed
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/FL-Studio-Api-Stubs/issues
 Project-URL: Documentation, https://miguelguthridge.github.io/FL-Studio-API-Stubs/
```

