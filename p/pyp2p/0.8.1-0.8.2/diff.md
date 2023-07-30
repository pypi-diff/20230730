# Comparing `tmp/pyp2p-0.8.1.tar.gz` & `tmp/pyp2p-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyp2p-0.8.1.tar", last modified: Fri Mar  4 16:12:24 2016, max compression
+gzip compressed data, was "dist/pyp2p-0.8.2.tar", last modified: Tue Mar 15 17:57:15 2016, max compression
```

## Comparing `pyp2p-0.8.1.tar` & `pyp2p-0.8.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-04 16:12:24.000000 pyp2p-0.8.1/
--rw-r--r--   0 root         (0) root         (0)     9049 2016-03-04 16:12:24.000000 pyp2p-0.8.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-04 16:12:24.000000 pyp2p-0.8.1/pyp2p.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9049 2016-03-04 16:12:23.000000 pyp2p-0.8.1/pyp2p.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2016-03-04 16:12:23.000000 pyp2p-0.8.1/pyp2p.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2016-03-04 16:12:23.000000 pyp2p-0.8.1/pyp2p.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2016-03-04 16:12:23.000000 pyp2p-0.8.1/pyp2p.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      424 2016-03-04 16:12:23.000000 pyp2p-0.8.1/pyp2p.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-04 16:12:24.000000 pyp2p-0.8.1/pyp2p/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     9652 2016-01-21 22:17:26.000000 pyp2p-0.8.1/pyp2p/upnp.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    21188 2016-01-21 22:17:26.000000 pyp2p-0.8.1/pyp2p/nat_pmp.py
--rwxrwxr-x   0 matthew   (1000) matthew   (1000)     7708 2016-02-02 16:00:02.000000 pyp2p-0.8.1/pyp2p/ipgetter.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     4292 2016-01-21 22:17:26.000000 pyp2p-0.8.1/pyp2p/sys_clock.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2016-01-20 18:22:38.000000 pyp2p-0.8.1/pyp2p/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    51542 2016-02-29 18:33:25.000000 pyp2p-0.8.1/pyp2p/net.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     4180 2016-01-21 22:17:26.000000 pyp2p-0.8.1/pyp2p/ip_routes.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     2174 2016-01-21 22:17:26.000000 pyp2p-0.8.1/pyp2p/hybrid_reply.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    21723 2016-02-29 17:32:03.000000 pyp2p-0.8.1/pyp2p/sock.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    23140 2016-01-21 22:17:26.000000 pyp2p-0.8.1/pyp2p/rendezvous_server.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    12482 2016-02-29 17:37:17.000000 pyp2p-0.8.1/pyp2p/lib.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    29185 2016-02-29 17:37:17.000000 pyp2p-0.8.1/pyp2p/rendezvous_client.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    17548 2016-01-23 19:26:19.000000 pyp2p-0.8.1/pyp2p/unl.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    16045 2016-03-04 16:11:18.000000 pyp2p-0.8.1/pyp2p/dht_msg.py
--rwxrwxr-x   0 matthew   (1000) matthew   (1000)     1431 2016-03-04 16:11:18.000000 pyp2p-0.8.1/setup.py
--rw-rw-r--   0 root         (0) root         (0)       88 2016-03-04 16:12:24.000000 pyp2p-0.8.1/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     7072 2016-01-21 22:17:26.000000 pyp2p-0.8.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-15 17:57:15.000000 pyp2p-0.8.2/
+-rw-r--r--   0 root         (0) root         (0)     9049 2016-03-15 17:57:15.000000 pyp2p-0.8.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9049 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      424 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     9652 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/upnp.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    21188 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/nat_pmp.py
+-rwxrwxr-x   0 matthew   (1000) matthew   (1000)     7708 2016-02-02 16:00:02.000000 pyp2p-0.8.2/pyp2p/ipgetter.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     4292 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/sys_clock.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2016-01-20 18:22:38.000000 pyp2p-0.8.2/pyp2p/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    51542 2016-02-29 18:33:25.000000 pyp2p-0.8.2/pyp2p/net.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     4180 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/ip_routes.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     2174 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/hybrid_reply.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    21723 2016-02-29 17:32:03.000000 pyp2p-0.8.2/pyp2p/sock.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    23140 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/rendezvous_server.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    12482 2016-02-29 17:37:17.000000 pyp2p-0.8.2/pyp2p/lib.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    29185 2016-02-29 17:37:17.000000 pyp2p-0.8.2/pyp2p/rendezvous_client.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    17548 2016-01-23 19:26:19.000000 pyp2p-0.8.2/pyp2p/unl.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    16297 2016-03-15 17:52:37.000000 pyp2p-0.8.2/pyp2p/dht_msg.py
+-rwxrwxr-x   0 matthew   (1000) matthew   (1000)     1431 2016-03-15 17:56:41.000000 pyp2p-0.8.2/setup.py
+-rw-rw-r--   0 root         (0) root         (0)       88 2016-03-15 17:57:15.000000 pyp2p-0.8.2/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     7072 2016-01-21 22:17:26.000000 pyp2p-0.8.2/README.rst
```

### Comparing `pyp2p-0.8.1/PKG-INFO` & `pyp2p-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyp2p
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python P2P networking library
 Home-page: http://github.com/Storj/pyp2p
 Author: Storj
 Author-email: matthew@storj.io
 License: MIT
 Description: ################
         Welcome to PyP2P
```

### Comparing `pyp2p-0.8.1/pyp2p.egg-info/PKG-INFO` & `pyp2p-0.8.2/pyp2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyp2p
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python P2P networking library
 Home-page: http://github.com/Storj/pyp2p
 Author: Storj
 Author-email: matthew@storj.io
 License: MIT
 Description: ################
         Welcome to PyP2P
```

### Comparing `pyp2p-0.8.1/pyp2p/upnp.py` & `pyp2p-0.8.2/pyp2p/upnp.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/nat_pmp.py` & `pyp2p-0.8.2/pyp2p/nat_pmp.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/ipgetter.py` & `pyp2p-0.8.2/pyp2p/ipgetter.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/sys_clock.py` & `pyp2p-0.8.2/pyp2p/sys_clock.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/net.py` & `pyp2p-0.8.2/pyp2p/net.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/ip_routes.py` & `pyp2p-0.8.2/pyp2p/ip_routes.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/hybrid_reply.py` & `pyp2p-0.8.2/pyp2p/hybrid_reply.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/sock.py` & `pyp2p-0.8.2/pyp2p/sock.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/rendezvous_server.py` & `pyp2p-0.8.2/pyp2p/rendezvous_server.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/lib.py` & `pyp2p-0.8.2/pyp2p/lib.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/rendezvous_client.py` & `pyp2p-0.8.2/pyp2p/rendezvous_client.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/unl.py` & `pyp2p-0.8.2/pyp2p/unl.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.1/pyp2p/dht_msg.py` & `pyp2p-0.8.2/pyp2p/dht_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import requests
 import binascii
 import umsgpack
 from ast import literal_eval
 from future.moves.urllib.parse import urlencode
 #from multiprocessing import Process as Thread, Event
 from threading import Thread, Event
-from storjkademlia.node import Node as KadNode
 from pyp2p.lib import is_ip_valid, is_valid_port
 from twisted.internet import defer
 
 import json
 import string
 import binascii
 
@@ -19,15 +18,16 @@
     from Queue import Queue  # py2
 except ImportError:
     from queue import Queue  # py3
 
 import time
 import logging
 
-dht_msg_endpoint = "http://162.243.213.95/dht_msg.php"
+#https://www.google.com/maps/place/AbsoluteCare+Medical+Center+%26+Pharmacy/@33.8118968,-84.3943467,17z/data=!4m2!3m1!1s0x88f505a894eff833:0xadc876bfec8fc2eedht_msg_endpoint = "http://162.243.213.95/dht_msg.php"
+dht_msg_endpoint = "http://localhost/dht_msg.php"
 logging.basicConfig()
 log = logging.getLogger(__name__)
 
 LONG_POLLING = True
 RESERVATION_TIMEOUT = (10 * 60) - 5
 MUTEX_TIMEOUT = RESERVATION_TIMEOUT
 
@@ -103,14 +103,15 @@
                         time.sleep(check_interval)
 
                         if not this_obj.running:
                             return
 
                     return
                 except Exception as e:
+                    print(e)
                     time.sleep(1)
 
         t = Thread(target=thread_loop, args=(self,))
         t.setDaemon(True)
         self.threads.append(t)
         t.start()
 
@@ -197,14 +198,15 @@
                     continue
 
                 neighbour["port"] = int(neighbour["port"])
                 if not is_valid_port(neighbour["port"]):
                     continue
 
                 neighbour["can_test"] = int(neighbour["can_test"])
+                from storjkademlia.node import Node as KadNode
                 knode = KadNode(
                     id=binascii.unhexlify(neighbour["id"].encode("ascii")),
                     ip=neighbour["ip"],
                     port=neighbour["port"],
                     can_test=neighbour["can_test"]
                 )
```

### Comparing `pyp2p-0.8.1/setup.py` & `pyp2p-0.8.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='0.8.1',
+    version='0.8.2',
     name='pyp2p',
     description='Python P2P networking library',
     keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP,'
               ' NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description=long_description,
     url='http://github.com/Storj/pyp2p',
     author='Storj',
```

### Comparing `pyp2p-0.8.1/README.rst` & `pyp2p-0.8.2/README.rst`

 * *Files identical despite different names*

