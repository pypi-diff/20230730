# Comparing `tmp/smartdoor-2.0.0.dev5.tar.gz` & `tmp/smartdoor-2.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdoor-2.0.0.dev5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "smartdoor-2.0.0.dev6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `smartdoor-2.0.0.dev5.tar` & `smartdoor-2.0.0.dev6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev5/.gitignore
--rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev5/LICENSE.md
--rw-r--r--   0        0        0     3481 2023-07-25 09:48:35.392457 smartdoor-2.0.0.dev5/README.md
--rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     9391 2023-07-25 10:28:45.411313 smartdoor-2.0.0.dev5/smartdoor/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev5/smartdoor/core/__init__.py
--rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev5/smartdoor/core/authenticate.py
--rw-r--r--   0        0        0     5180 2023-07-25 10:14:25.177153 smartdoor-2.0.0.dev5/smartdoor/core/smartlock.py
--rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev5/smartdoor/default_config.toml
--rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev5/smartdoor/logging.conf
--rw-r--r--   0        0        0      222 2023-07-25 10:31:54.119674 smartdoor-2.0.0.dev5/smartdoor/pigpio.service
--rw-r--r--   0        0        0     8856 2023-07-25 10:29:16.968711 smartdoor-2.0.0.dev5/smartdoor/smartdoor.py
--rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev5/smartdoor/smartdoor.service
--rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev6/.gitignore
+-rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev6/LICENSE.md
+-rw-r--r--   0        0        0     3481 2023-07-25 09:48:35.392457 smartdoor-2.0.0.dev6/README.md
+-rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0    10219 2023-07-25 10:38:11.176377 smartdoor-2.0.0.dev6/smartdoor/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev6/smartdoor/core/__init__.py
+-rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev6/smartdoor/core/authenticate.py
+-rw-r--r--   0        0        0     5180 2023-07-25 10:14:25.177153 smartdoor-2.0.0.dev6/smartdoor/core/smartlock.py
+-rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev6/smartdoor/default_config.toml
+-rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev6/smartdoor/logging.conf
+-rw-r--r--   0        0        0      222 2023-07-25 10:31:54.119674 smartdoor-2.0.0.dev6/smartdoor/pigpio.service
+-rw-r--r--   0        0        0     8856 2023-07-25 10:29:16.968711 smartdoor-2.0.0.dev6/smartdoor/smartdoor.py
+-rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev6/smartdoor/smartdoor.service
+-rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev6/PKG-INFO
```

### Comparing `smartdoor-2.0.0.dev5/.gitignore` & `smartdoor-2.0.0.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/.pre-commit-config.yaml` & `smartdoor-2.0.0.dev6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/LICENSE.md` & `smartdoor-2.0.0.dev6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/README.md` & `smartdoor-2.0.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/pyproject.toml` & `smartdoor-2.0.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/smartdoor/__init__.py` & `smartdoor-2.0.0.dev6/smartdoor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
 
 from .smartdoor import SmartDoor
 
-__version__ = "2.0.0.dev5"
+__version__ = "2.0.0.dev6"
 __all__ = ["SmartDoor"]
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(__version__, "-V", "--version")
 def cli():
     """Smartdoor system CLI."""
@@ -192,51 +192,71 @@
             subprocess.run(["sudo", "systemctl", "enable", "smartdoor.service"], check=True)
             click.echo("registered service to systemd")
         except subprocess.CalledProcessError as e:
             click.echo(e)
             click.echo("failed to register service to systemd")
 
     elif unregister:
+        # Unregister smartdoor service from systemd
+        try:
+            subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"], check=True)
+            subprocess.run(["sudo", "systemctl", "disable", "smartdoor.service"], check=True)
+            subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
+            click.echo("unregistered service from systemd")
+        except subprocess.CalledProcessError as e:
+            click.echo(e)
+            click.echo("failed to unregister service from systemd")
+
         # Unregister pigpio daemon from systemd
         if find_spec("pigpio") is not None:
             try:
                 subprocess.run(["sudo", "systemctl", "stop", "pigpio.service"], check=True)
                 subprocess.run(["sudo", "systemctl", "disable", "pigpio.service"], check=True)
                 subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
                 click.echo("unregistered pigpio daemon from systemd")
             except subprocess.CalledProcessError as e:
                 click.echo(e)
                 click.echo("failed to unregister pigpio daemon from systemd")
 
-        # Unregister smartdoor service from systemd
-        try:
-            subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"], check=True)
-            subprocess.run(["sudo", "systemctl", "disable", "smartdoor.service"], check=True)
-            subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
-            click.echo("unregistered service from systemd")
-        except subprocess.CalledProcessError as e:
-            click.echo(e)
-            click.echo("failed to unregister service from systemd")
-
     elif start:
+        # Start pigpio daemon
+        if find_spec("pigpio") is not None:
+            try:
+                subprocess.run(["sudo", "systemctl", "start", "pigpio.service"], check=True)
+                click.echo("started pigpio daemon")
+            except subprocess.CalledProcessError as e:
+                click.echo(e)
+                click.echo("failed to start pigpio daemon")
+
+        # Start smartdoor service
         try:
             subprocess.run(["sudo", "systemctl", "start", "smartdoor.service"], check=True)
             click.echo("started service")
         except subprocess.CalledProcessError as e:
             click.echo(e)
             click.echo("failed to start service")
 
     elif stop:
+        # Stop smartdoor service
         try:
             subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"], check=True)
             click.echo("stopped service")
         except subprocess.CalledProcessError as e:
             click.echo(e)
             click.echo("failed to stop service")
 
+        # Stop pigpio daemon
+        if find_spec("pigpio") is not None:
+            try:
+                subprocess.run(["sudo", "systemctl", "stop", "pigpio.service"], check=True)
+                click.echo("stopped pigpio daemon")
+            except subprocess.CalledProcessError as e:
+                click.echo(e)
+                click.echo("failed to stop pigpio daemon")
+
     elif restart:
         try:
             subprocess.run(["sudo", "systemctl", "restart", "smartdoor.service"], check=True)
             click.echo("restarted service")
         except subprocess.CalledProcessError as e:
             click.echo(e)
             click.echo("failed to restart service")
```

### Comparing `smartdoor-2.0.0.dev5/smartdoor/core/authenticate.py` & `smartdoor-2.0.0.dev6/smartdoor/core/authenticate.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/smartdoor/core/smartlock.py` & `smartdoor-2.0.0.dev6/smartdoor/core/smartlock.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/smartdoor/default_config.toml` & `smartdoor-2.0.0.dev6/smartdoor/default_config.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/smartdoor/logging.conf` & `smartdoor-2.0.0.dev6/smartdoor/logging.conf`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/smartdoor/smartdoor.py` & `smartdoor-2.0.0.dev6/smartdoor/smartdoor.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev5/PKG-INFO` & `smartdoor-2.0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdoor
-Version: 2.0.0.dev5
+Version: 2.0.0.dev6
 Summary: Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc.
 Author-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Maintainer-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

