# Comparing `tmp/pyp2p-0.8.2.tar.gz` & `tmp/pyp2p-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyp2p-0.8.2.tar", last modified: Tue Mar 15 17:57:15 2016, max compression
+gzip compressed data, was "pyp2p-0.8.3.tar", last modified: Sun Jul 30 06:04:45 2023, max compression
```

## Comparing `pyp2p-0.8.2.tar` & `pyp2p-0.8.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-15 17:57:15.000000 pyp2p-0.8.2/
--rw-r--r--   0 root         (0) root         (0)     9049 2016-03-15 17:57:15.000000 pyp2p-0.8.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9049 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      424 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-15 17:57:15.000000 pyp2p-0.8.2/pyp2p/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     9652 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/upnp.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    21188 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/nat_pmp.py
--rwxrwxr-x   0 matthew   (1000) matthew   (1000)     7708 2016-02-02 16:00:02.000000 pyp2p-0.8.2/pyp2p/ipgetter.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     4292 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/sys_clock.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2016-01-20 18:22:38.000000 pyp2p-0.8.2/pyp2p/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    51542 2016-02-29 18:33:25.000000 pyp2p-0.8.2/pyp2p/net.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     4180 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/ip_routes.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     2174 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/hybrid_reply.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    21723 2016-02-29 17:32:03.000000 pyp2p-0.8.2/pyp2p/sock.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    23140 2016-01-21 22:17:26.000000 pyp2p-0.8.2/pyp2p/rendezvous_server.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    12482 2016-02-29 17:37:17.000000 pyp2p-0.8.2/pyp2p/lib.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    29185 2016-02-29 17:37:17.000000 pyp2p-0.8.2/pyp2p/rendezvous_client.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    17548 2016-01-23 19:26:19.000000 pyp2p-0.8.2/pyp2p/unl.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    16297 2016-03-15 17:52:37.000000 pyp2p-0.8.2/pyp2p/dht_msg.py
--rwxrwxr-x   0 matthew   (1000) matthew   (1000)     1431 2016-03-15 17:56:41.000000 pyp2p-0.8.2/setup.py
--rw-rw-r--   0 root         (0) root         (0)       88 2016-03-15 17:57:15.000000 pyp2p-0.8.2/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     7072 2016-01-21 22:17:26.000000 pyp2p-0.8.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-30 06:04:45.543133 pyp2p-0.8.3/
+-rw-rw-rw-   0        0        0     1105 2023-07-30 05:52:05.000000 pyp2p-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0     8111 2023-07-30 06:04:45.543133 pyp2p-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7224 2023-07-30 06:01:19.000000 pyp2p-0.8.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-30 06:04:45.533069 pyp2p-0.8.3/pyp2p/
+-rw-rw-rw-   0        0        0        2 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/__init__.py
+-rw-rw-rw-   0        0        0    16156 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/dht_msg.py
+-rw-rw-rw-   0        0        0     2174 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/hybrid_reply.py
+-rw-rw-rw-   0        0        0     4289 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/ip_routes.py
+-rw-rw-rw-   0        0        0     7708 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/ipgetter.py
+-rw-rw-rw-   0        0        0    13131 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/lib.py
+-rw-rw-rw-   0        0        0    21188 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/nat_pmp.py
+-rw-rw-rw-   0        0        0    51489 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/net.py
+-rw-rw-rw-   0        0        0    29189 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/rendezvous_client.py
+-rw-rw-rw-   0        0        0    23140 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/rendezvous_server.py
+-rw-rw-rw-   0        0        0    22392 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/sock.py
+-rw-rw-rw-   0        0        0     4454 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/sys_clock.py
+-rw-rw-rw-   0        0        0    17548 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/unl.py
+-rw-rw-rw-   0        0        0     9905 2023-07-30 05:52:05.000000 pyp2p-0.8.3/pyp2p/upnp.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:04:45.542136 pyp2p-0.8.3/pyp2p.egg-info/
+-rw-rw-rw-   0        0        0     8111 2023-07-30 06:04:45.000000 pyp2p-0.8.3/pyp2p.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-07-30 06:04:45.000000 pyp2p-0.8.3/pyp2p.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 06:04:45.000000 pyp2p-0.8.3/pyp2p.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-07-30 06:04:45.000000 pyp2p-0.8.3/pyp2p.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-30 06:04:45.000000 pyp2p-0.8.3/pyp2p.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-30 06:04:45.544129 pyp2p-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-07-30 06:04:26.000000 pyp2p-0.8.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyp2p-0.8.2/PKG-INFO` & `pyp2p-0.8.3/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,176 +1,156 @@
-Metadata-Version: 1.1
-Name: pyp2p
-Version: 0.8.2
-Summary: Python P2P networking library
-Home-page: http://github.com/Storj/pyp2p
-Author: Storj
-Author-email: matthew@storj.io
-License: MIT
-Description: ################
-        Welcome to PyP2P
-        ################
-        
-        |BuildLink|_ |CoverageLink|_ |BuildLink2|_ |CoverageLink2|_ |LicenseLink|_
-        
-        .. |BuildLink| image:: https://img.shields.io/travis/Storj/pyp2p/master.svg?label=Build-Master
-        .. _BuildLink: https://travis-ci.org/Storj/pyp2p
-        
-        .. |CoverageLink| image:: https://img.shields.io/coveralls/Storj/pyp2p/master.svg?label=Coverage-Master
-        .. _CoverageLink: https://coveralls.io/r/Storj/pyp2p
-        
-        .. |BuildLink2| image:: https://img.shields.io/travis/Storj/pyp2p/develop.svg?label=Build-Develop
-        .. _BuildLink2: https://travis-ci.org/Storj/pyp2p
-        
-        .. |CoverageLink2| image:: https://img.shields.io/coveralls/Storj/pyp2p/develop.svg?label=Coverage-Develop
-        .. _CoverageLink2: https://coveralls.io/r/Storj/pyp2p
-        
-        .. |LicenseLink| image:: https://img.shields.io/badge/license-MIT-blue.svg
-        .. _LicenseLink: https://raw.githubusercontent.com/Storj/pyp2p
-        
-        PyP2P is a simplified networking library for building peer-to-peer networks in Python. The library is designed to solve the pain of finding nodes and bypassing NATs so you can focus on writing your application code.
-        
-        * Automated port forwarding with UPnP and NATPMP
-        * Support for TCP hole punching / simultaneous open
-        * Reverse connect (tell a node to connect to you)
-        * Fail-safe proxying (planned feature)
-        * Python 2 (tested on 2.7 - experimental) & 3 (tested on 3.3)
-        * Linux and Windows - yep
-        
-        ============
-        Code example
-        ============
-        PyP2P is designed to work with simple non-blocking TCP sockets. To use them, your application must create an infinite loop which is used to periodically look for new replies. As you look for replies, the software also handles accepting new connections and removing old ones automatically.
-        
-        The library also handles constructing replies, which are returned in full as a simple list. The underlying message format is a simple line-based protocol: the messages you want to send are terminated with a new line and are returned in full when they've arrived which makes debugging and developing p2p protocols very simple (text-based protocols are easy to debug.)
-        
-        ==========
-        Alice node
-        ==========
-        This will create a new listening server on port 44444, bound to listen for connections from the LAN. The interface is specified mostly to ensure that connections are only made from that interface. By default, connections will be made from the default interface (usually wlan0 or eth0) which isn't useful for simulating and testing a P2P network on the same computer.
-        
-        .. code:: python
-        
-            from pyp2p.net import *
-            import time
-        
-            #Setup Alice's p2p node.
-            alice = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", node_type="passive", debug=1)
-            alice.start()
-            alice.bootstrap()
-            alice.advertise()
-        
-            #Event loop.
-            while 1:
-                for con in alice:
-                    for reply in con:
-                        print(reply)
-        
-                time.sleep(1)
-        
-        ========
-        Bob node
-        ========
-        This code will make a connection to the Alice node and repeatedly send her the word test. Note how they're both on different interfaces, with completely different IPs. This is necessary for connecting to nodes on the same computer as the library doesn't allow the Net class to connect to itself itself when running in P2P mode (type="p2p" for the Net class.) If you want to be able to make duplicate connections to nodes on the same interface then specify the type as "direct" which will make testing code easier. Note that type is "p2p" by default.
-        
-        .. code:: python
-        
-            from pyp2p.net import *
-        
-            #Setup Bob's p2p node.
-            bob = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", node_type="passive", debug=1)
-            bob.start()
-            bob.bootstrap()
-            bob.advertise()
-        
-            #Event loop.
-            while 1:
-                for con in bob:
-                    con.send_line("test")
-        
-                time.sleep(1)
-        
-        ==============
-        Direct connect
-        ==============
-        The code shown so far is good for standard broadcast / flooding style P2P networks where the only requirement is to get a message out to the whole network (e.g. Bitcoin and Bitmessage) - but if you want to do anything more complicated you're going to need to be able to communicate with nodes directly.
-        
-        Theoretically you can specify the recipient of a message and broadcast it to the network to reach them but this approach won't scale well for most people. What is needed is a way to direct connect to a node with a high level of reliability. To support this function we use something called a UNL: short for Universal Node Locator.
-        
-        UNLs describe how to connect to a node behind a NAT, firewall, or on the same LAN by looking at the nodes network information in relation to other nodes and using a variety of subversive techniques including UPnP, NATPMP, and TCP hole punching. To further increase the reliability of this code: the software can also be used with a patched instance of the Kademlia DHT to accept direct messages from other nodes on the DHT that instruct it where to connect back to. This is extremely useful for connecting to nodes behind a NAT as it completely bypasses the need for port forwarding assuming that the source is accessible.
-        
-        .. code:: python
-        
-            from pyp2p.net import *
-            from pyp2p.unl import UNL
-            from pyp2p.dht_msg import DHT
-            import time
-        
-        
-            #Start Alice's direct server.
-            alice_dht = DHT()
-            alice_direct = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", net_type="direct", dht_node=alice_dht, debug=1)
-            alice_direct.start()
-        
-            #Start Bob's direct server.
-            bob_dht = DHT()
-            bob_direct = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", net_type="direct", node_type="active", dht_node=bob_dht, debug=1)
-            bob_direct.start()
-        
-            #Callbacks.
-            def success(con):
-                print("Alice successfully connected to Bob.")
-                con.send_line("Sup Bob.")
-        
-            def failure(con):
-            print("Alice failed to connec to Bob\a")
-        
-            events = {
-                "success": success,
-                "failure": failure
-            }
-        
-            #Have Alice connect to Bob.
-            alice_direct.unl.connect(bob_direct.unl.construct(), events)
-        
-            #Event loop.
-            while 1:
-            #Bob get reply.
-            for con in bob_direct:
-                for reply in con:
-                    print(reply)
-        
-            #Alice accept con.
-            for con in alice_direct:
-                x = 1
-        
-            time.sleep(0.5)
-        
-        
-        In the previous code the Net class was used to spawn a server to accept connections from nodes on the p2p network and managing connections for the purpose of broadcasting. To manage direct connections the same class is used, the difference is the class disables bootstrapping and advertising the connection details to the bootstrapping server as this service is reserved specifically for receiving direct connections.
-        
-        ============
-        Dependencies
-        ============
-        * netifaces
-        * ntplib
-        * twisted
-        * ipaddress
-        * requests
-        * nose
-        * setuptools
-        * pyroute2
-        
-        Installation: python3.3 setup.py install
-        
-        Status: Experimental, may have bugs
-        
-Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,NATPMP,P2P,Peer-to-peer networking library,python
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
+**This library is depricated. See https://github.com/robertsdotpm/p2pd for the new version**
+#############################################################################################
+
+Welcome to PyP2P |BuildLink|_ |CoverageLink|_ |BuildLink2|_ |CoverageLink2|_ |LicenseLink|_
+
+.. |BuildLink| image:: https://img.shields.io/travis/Storj/pyp2p/master.svg?label=Build-Master
+.. _BuildLink: https://travis-ci.org/Storj/pyp2p
+
+.. |CoverageLink| image:: https://img.shields.io/coveralls/Storj/pyp2p/master.svg?label=Coverage-Master
+.. _CoverageLink: https://coveralls.io/r/Storj/pyp2p
+
+.. |BuildLink2| image:: https://img.shields.io/travis/Storj/pyp2p/develop.svg?label=Build-Develop
+.. _BuildLink2: https://travis-ci.org/Storj/pyp2p
+
+.. |CoverageLink2| image:: https://img.shields.io/coveralls/Storj/pyp2p/develop.svg?label=Coverage-Develop
+.. _CoverageLink2: https://coveralls.io/r/Storj/pyp2p
+
+.. |LicenseLink| image:: https://img.shields.io/badge/license-MIT-blue.svg
+.. _LicenseLink: https://raw.githubusercontent.com/Storj/pyp2p
+
+PyP2P is a simplified networking library for building peer-to-peer networks in Python. The library is designed to solve the pain of finding nodes and bypassing NATs so you can focus on writing your application code.
+
+* Automated port forwarding with UPnP and NATPMP
+* Support for TCP hole punching / simultaneous open
+* Reverse connect (tell a node to connect to you)
+* Fail-safe proxying (planned feature)
+* Python 2 (tested on 2.7 - experimental) & 3 (tested on 3.3)
+* Linux and Windows - yep
+
+============
+Code example
+============
+PyP2P is designed to work with simple non-blocking TCP sockets. To use them, your application must create an infinite loop which is used to periodically look for new replies. As you look for replies, the software also handles accepting new connections and removing old ones automatically.
+
+The library also handles constructing replies, which are returned in full as a simple list. The underlying message format is a simple line-based protocol: the messages you want to send are terminated with a new line and are returned in full when they've arrived which makes debugging and developing p2p protocols very simple (text-based protocols are easy to debug.)
+
+==========
+Alice node
+==========
+This will create a new listening server on port 44444, bound to listen for connections from the LAN. The interface is specified mostly to ensure that connections are only made from that interface. By default, connections will be made from the default interface (usually wlan0 or eth0) which isn't useful for simulating and testing a P2P network on the same computer.
+
+.. code:: python
+
+    from pyp2p.net import *
+    import time
+
+    #Setup Alice's p2p node.
+    alice = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", node_type="passive", debug=1)
+    alice.start()
+    alice.bootstrap()
+    alice.advertise()
+
+    #Event loop.
+    while 1:
+        for con in alice:
+            for reply in con:
+                print(reply)
+
+        time.sleep(1)
+
+========
+Bob node
+========
+This code will make a connection to the Alice node and repeatedly send her the word test. Note how they're both on different interfaces, with completely different IPs. This is necessary for connecting to nodes on the same computer as the library doesn't allow the Net class to connect to itself itself when running in P2P mode (type="p2p" for the Net class.) If you want to be able to make duplicate connections to nodes on the same interface then specify the type as "direct" which will make testing code easier. Note that type is "p2p" by default.
+
+.. code:: python
+
+    from pyp2p.net import *
+
+    #Setup Bob's p2p node.
+    bob = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", node_type="passive", debug=1)
+    bob.start()
+    bob.bootstrap()
+    bob.advertise()
+
+    #Event loop.
+    while 1:
+        for con in bob:
+            con.send_line("test")
+
+        time.sleep(1)
+
+==============
+Direct connect
+==============
+The code shown so far is good for standard broadcast / flooding style P2P networks where the only requirement is to get a message out to the whole network (e.g. Bitcoin and Bitmessage) - but if you want to do anything more complicated you're going to need to be able to communicate with nodes directly.
+
+Theoretically you can specify the recipient of a message and broadcast it to the network to reach them but this approach won't scale well for most people. What is needed is a way to direct connect to a node with a high level of reliability. To support this function we use something called a UNL: short for Universal Node Locator.
+
+UNLs describe how to connect to a node behind a NAT, firewall, or on the same LAN by looking at the nodes network information in relation to other nodes and using a variety of subversive techniques including UPnP, NATPMP, and TCP hole punching. To further increase the reliability of this code: the software can also be used with a patched instance of the Kademlia DHT to accept direct messages from other nodes on the DHT that instruct it where to connect back to. This is extremely useful for connecting to nodes behind a NAT as it completely bypasses the need for port forwarding assuming that the source is accessible.
+
+.. code:: python
+
+    from pyp2p.net import *
+    from pyp2p.unl import UNL
+    from pyp2p.dht_msg import DHT
+    import time
+
+
+    #Start Alice's direct server.
+    alice_dht = DHT()
+    alice_direct = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", net_type="direct", dht_node=alice_dht, debug=1)
+    alice_direct.start()
+
+    #Start Bob's direct server.
+    bob_dht = DHT()
+    bob_direct = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", net_type="direct", node_type="active", dht_node=bob_dht, debug=1)
+    bob_direct.start()
+
+    #Callbacks.
+    def success(con):
+        print("Alice successfully connected to Bob.")
+        con.send_line("Sup Bob.")
+
+    def failure(con):
+    print("Alice failed to connec to Bob\a")
+
+    events = {
+        "success": success,
+        "failure": failure
+    }
+
+    #Have Alice connect to Bob.
+    alice_direct.unl.connect(bob_direct.unl.construct(), events)
+
+    #Event loop.
+    while 1:
+    #Bob get reply.
+    for con in bob_direct:
+        for reply in con:
+            print(reply)
+
+    #Alice accept con.
+    for con in alice_direct:
+        x = 1
+
+    time.sleep(0.5)
+
+
+In the previous code the Net class was used to spawn a server to accept connections from nodes on the p2p network and managing connections for the purpose of broadcasting. To manage direct connections the same class is used, the difference is the class disables bootstrapping and advertising the connection details to the bootstrapping server as this service is reserved specifically for receiving direct connections.
+
+============
+Dependencies
+============
+* netifaces
+* ntplib
+* twisted
+* ipaddress
+* requests
+* nose
+* setuptools
+* pyroute2
+
+Installation: python3.3 setup.py install
+
+Status: Experimental, may have bugs
```

### Comparing `pyp2p-0.8.2/pyp2p.egg-info/PKG-INFO` & `pyp2p-0.8.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,176 +1,175 @@
-Metadata-Version: 1.1
-Name: pyp2p
-Version: 0.8.2
-Summary: Python P2P networking library
-Home-page: http://github.com/Storj/pyp2p
-Author: Storj
-Author-email: matthew@storj.io
-License: MIT
-Description: ################
-        Welcome to PyP2P
-        ################
-        
-        |BuildLink|_ |CoverageLink|_ |BuildLink2|_ |CoverageLink2|_ |LicenseLink|_
-        
-        .. |BuildLink| image:: https://img.shields.io/travis/Storj/pyp2p/master.svg?label=Build-Master
-        .. _BuildLink: https://travis-ci.org/Storj/pyp2p
-        
-        .. |CoverageLink| image:: https://img.shields.io/coveralls/Storj/pyp2p/master.svg?label=Coverage-Master
-        .. _CoverageLink: https://coveralls.io/r/Storj/pyp2p
-        
-        .. |BuildLink2| image:: https://img.shields.io/travis/Storj/pyp2p/develop.svg?label=Build-Develop
-        .. _BuildLink2: https://travis-ci.org/Storj/pyp2p
-        
-        .. |CoverageLink2| image:: https://img.shields.io/coveralls/Storj/pyp2p/develop.svg?label=Coverage-Develop
-        .. _CoverageLink2: https://coveralls.io/r/Storj/pyp2p
-        
-        .. |LicenseLink| image:: https://img.shields.io/badge/license-MIT-blue.svg
-        .. _LicenseLink: https://raw.githubusercontent.com/Storj/pyp2p
-        
-        PyP2P is a simplified networking library for building peer-to-peer networks in Python. The library is designed to solve the pain of finding nodes and bypassing NATs so you can focus on writing your application code.
-        
-        * Automated port forwarding with UPnP and NATPMP
-        * Support for TCP hole punching / simultaneous open
-        * Reverse connect (tell a node to connect to you)
-        * Fail-safe proxying (planned feature)
-        * Python 2 (tested on 2.7 - experimental) & 3 (tested on 3.3)
-        * Linux and Windows - yep
-        
-        ============
-        Code example
-        ============
-        PyP2P is designed to work with simple non-blocking TCP sockets. To use them, your application must create an infinite loop which is used to periodically look for new replies. As you look for replies, the software also handles accepting new connections and removing old ones automatically.
-        
-        The library also handles constructing replies, which are returned in full as a simple list. The underlying message format is a simple line-based protocol: the messages you want to send are terminated with a new line and are returned in full when they've arrived which makes debugging and developing p2p protocols very simple (text-based protocols are easy to debug.)
-        
-        ==========
-        Alice node
-        ==========
-        This will create a new listening server on port 44444, bound to listen for connections from the LAN. The interface is specified mostly to ensure that connections are only made from that interface. By default, connections will be made from the default interface (usually wlan0 or eth0) which isn't useful for simulating and testing a P2P network on the same computer.
-        
-        .. code:: python
-        
-            from pyp2p.net import *
-            import time
-        
-            #Setup Alice's p2p node.
-            alice = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", node_type="passive", debug=1)
-            alice.start()
-            alice.bootstrap()
-            alice.advertise()
-        
-            #Event loop.
-            while 1:
-                for con in alice:
-                    for reply in con:
-                        print(reply)
-        
-                time.sleep(1)
-        
-        ========
-        Bob node
-        ========
-        This code will make a connection to the Alice node and repeatedly send her the word test. Note how they're both on different interfaces, with completely different IPs. This is necessary for connecting to nodes on the same computer as the library doesn't allow the Net class to connect to itself itself when running in P2P mode (type="p2p" for the Net class.) If you want to be able to make duplicate connections to nodes on the same interface then specify the type as "direct" which will make testing code easier. Note that type is "p2p" by default.
-        
-        .. code:: python
-        
-            from pyp2p.net import *
-        
-            #Setup Bob's p2p node.
-            bob = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", node_type="passive", debug=1)
-            bob.start()
-            bob.bootstrap()
-            bob.advertise()
-        
-            #Event loop.
-            while 1:
-                for con in bob:
-                    con.send_line("test")
-        
-                time.sleep(1)
-        
-        ==============
-        Direct connect
-        ==============
-        The code shown so far is good for standard broadcast / flooding style P2P networks where the only requirement is to get a message out to the whole network (e.g. Bitcoin and Bitmessage) - but if you want to do anything more complicated you're going to need to be able to communicate with nodes directly.
-        
-        Theoretically you can specify the recipient of a message and broadcast it to the network to reach them but this approach won't scale well for most people. What is needed is a way to direct connect to a node with a high level of reliability. To support this function we use something called a UNL: short for Universal Node Locator.
-        
-        UNLs describe how to connect to a node behind a NAT, firewall, or on the same LAN by looking at the nodes network information in relation to other nodes and using a variety of subversive techniques including UPnP, NATPMP, and TCP hole punching. To further increase the reliability of this code: the software can also be used with a patched instance of the Kademlia DHT to accept direct messages from other nodes on the DHT that instruct it where to connect back to. This is extremely useful for connecting to nodes behind a NAT as it completely bypasses the need for port forwarding assuming that the source is accessible.
-        
-        .. code:: python
-        
-            from pyp2p.net import *
-            from pyp2p.unl import UNL
-            from pyp2p.dht_msg import DHT
-            import time
-        
-        
-            #Start Alice's direct server.
-            alice_dht = DHT()
-            alice_direct = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", net_type="direct", dht_node=alice_dht, debug=1)
-            alice_direct.start()
-        
-            #Start Bob's direct server.
-            bob_dht = DHT()
-            bob_direct = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", net_type="direct", node_type="active", dht_node=bob_dht, debug=1)
-            bob_direct.start()
-        
-            #Callbacks.
-            def success(con):
-                print("Alice successfully connected to Bob.")
-                con.send_line("Sup Bob.")
-        
-            def failure(con):
-            print("Alice failed to connec to Bob\a")
-        
-            events = {
-                "success": success,
-                "failure": failure
-            }
-        
-            #Have Alice connect to Bob.
-            alice_direct.unl.connect(bob_direct.unl.construct(), events)
-        
-            #Event loop.
-            while 1:
-            #Bob get reply.
-            for con in bob_direct:
-                for reply in con:
-                    print(reply)
-        
-            #Alice accept con.
-            for con in alice_direct:
-                x = 1
-        
-            time.sleep(0.5)
-        
-        
-        In the previous code the Net class was used to spawn a server to accept connections from nodes on the p2p network and managing connections for the purpose of broadcasting. To manage direct connections the same class is used, the difference is the class disables bootstrapping and advertising the connection details to the bootstrapping server as this service is reserved specifically for receiving direct connections.
-        
-        ============
-        Dependencies
-        ============
-        * netifaces
-        * ntplib
-        * twisted
-        * ipaddress
-        * requests
-        * nose
-        * setuptools
-        * pyroute2
-        
-        Installation: python3.3 setup.py install
-        
-        Status: Experimental, may have bugs
-        
-Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,NATPMP,P2P,Peer-to-peer networking library,python
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
+Metadata-Version: 2.1
+Name: pyp2p
+Version: 0.8.3
+Summary: Python P2P networking library
+Home-page: http://github.com/Storj/pyp2p
+Author: Storj
+Author-email: matthew@storj.io
+License: MIT
+Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,NATPMP,P2P,Peer-to-peer networking library,python
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+License-File: LICENSE
+
+**This library is depricated. See https://github.com/robertsdotpm/p2pd for the new version**
+#############################################################################################
+
+Welcome to PyP2P |BuildLink|_ |CoverageLink|_ |BuildLink2|_ |CoverageLink2|_ |LicenseLink|_
+
+.. |BuildLink| image:: https://img.shields.io/travis/Storj/pyp2p/master.svg?label=Build-Master
+.. _BuildLink: https://travis-ci.org/Storj/pyp2p
+
+.. |CoverageLink| image:: https://img.shields.io/coveralls/Storj/pyp2p/master.svg?label=Coverage-Master
+.. _CoverageLink: https://coveralls.io/r/Storj/pyp2p
+
+.. |BuildLink2| image:: https://img.shields.io/travis/Storj/pyp2p/develop.svg?label=Build-Develop
+.. _BuildLink2: https://travis-ci.org/Storj/pyp2p
+
+.. |CoverageLink2| image:: https://img.shields.io/coveralls/Storj/pyp2p/develop.svg?label=Coverage-Develop
+.. _CoverageLink2: https://coveralls.io/r/Storj/pyp2p
+
+.. |LicenseLink| image:: https://img.shields.io/badge/license-MIT-blue.svg
+.. _LicenseLink: https://raw.githubusercontent.com/Storj/pyp2p
+
+PyP2P is a simplified networking library for building peer-to-peer networks in Python. The library is designed to solve the pain of finding nodes and bypassing NATs so you can focus on writing your application code.
+
+* Automated port forwarding with UPnP and NATPMP
+* Support for TCP hole punching / simultaneous open
+* Reverse connect (tell a node to connect to you)
+* Fail-safe proxying (planned feature)
+* Python 2 (tested on 2.7 - experimental) & 3 (tested on 3.3)
+* Linux and Windows - yep
+
+============
+Code example
+============
+PyP2P is designed to work with simple non-blocking TCP sockets. To use them, your application must create an infinite loop which is used to periodically look for new replies. As you look for replies, the software also handles accepting new connections and removing old ones automatically.
+
+The library also handles constructing replies, which are returned in full as a simple list. The underlying message format is a simple line-based protocol: the messages you want to send are terminated with a new line and are returned in full when they've arrived which makes debugging and developing p2p protocols very simple (text-based protocols are easy to debug.)
+
+==========
+Alice node
+==========
+This will create a new listening server on port 44444, bound to listen for connections from the LAN. The interface is specified mostly to ensure that connections are only made from that interface. By default, connections will be made from the default interface (usually wlan0 or eth0) which isn't useful for simulating and testing a P2P network on the same computer.
+
+.. code:: python
+
+    from pyp2p.net import *
+    import time
+
+    #Setup Alice's p2p node.
+    alice = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", node_type="passive", debug=1)
+    alice.start()
+    alice.bootstrap()
+    alice.advertise()
+
+    #Event loop.
+    while 1:
+        for con in alice:
+            for reply in con:
+                print(reply)
+
+        time.sleep(1)
+
+========
+Bob node
+========
+This code will make a connection to the Alice node and repeatedly send her the word test. Note how they're both on different interfaces, with completely different IPs. This is necessary for connecting to nodes on the same computer as the library doesn't allow the Net class to connect to itself itself when running in P2P mode (type="p2p" for the Net class.) If you want to be able to make duplicate connections to nodes on the same interface then specify the type as "direct" which will make testing code easier. Note that type is "p2p" by default.
+
+.. code:: python
+
+    from pyp2p.net import *
+
+    #Setup Bob's p2p node.
+    bob = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", node_type="passive", debug=1)
+    bob.start()
+    bob.bootstrap()
+    bob.advertise()
+
+    #Event loop.
+    while 1:
+        for con in bob:
+            con.send_line("test")
+
+        time.sleep(1)
+
+==============
+Direct connect
+==============
+The code shown so far is good for standard broadcast / flooding style P2P networks where the only requirement is to get a message out to the whole network (e.g. Bitcoin and Bitmessage) - but if you want to do anything more complicated you're going to need to be able to communicate with nodes directly.
+
+Theoretically you can specify the recipient of a message and broadcast it to the network to reach them but this approach won't scale well for most people. What is needed is a way to direct connect to a node with a high level of reliability. To support this function we use something called a UNL: short for Universal Node Locator.
+
+UNLs describe how to connect to a node behind a NAT, firewall, or on the same LAN by looking at the nodes network information in relation to other nodes and using a variety of subversive techniques including UPnP, NATPMP, and TCP hole punching. To further increase the reliability of this code: the software can also be used with a patched instance of the Kademlia DHT to accept direct messages from other nodes on the DHT that instruct it where to connect back to. This is extremely useful for connecting to nodes behind a NAT as it completely bypasses the need for port forwarding assuming that the source is accessible.
+
+.. code:: python
+
+    from pyp2p.net import *
+    from pyp2p.unl import UNL
+    from pyp2p.dht_msg import DHT
+    import time
+
+
+    #Start Alice's direct server.
+    alice_dht = DHT()
+    alice_direct = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", net_type="direct", dht_node=alice_dht, debug=1)
+    alice_direct.start()
+
+    #Start Bob's direct server.
+    bob_dht = DHT()
+    bob_direct = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", net_type="direct", node_type="active", dht_node=bob_dht, debug=1)
+    bob_direct.start()
+
+    #Callbacks.
+    def success(con):
+        print("Alice successfully connected to Bob.")
+        con.send_line("Sup Bob.")
+
+    def failure(con):
+    print("Alice failed to connec to Bob\a")
+
+    events = {
+        "success": success,
+        "failure": failure
+    }
+
+    #Have Alice connect to Bob.
+    alice_direct.unl.connect(bob_direct.unl.construct(), events)
+
+    #Event loop.
+    while 1:
+    #Bob get reply.
+    for con in bob_direct:
+        for reply in con:
+            print(reply)
+
+    #Alice accept con.
+    for con in alice_direct:
+        x = 1
+
+    time.sleep(0.5)
+
+
+In the previous code the Net class was used to spawn a server to accept connections from nodes on the p2p network and managing connections for the purpose of broadcasting. To manage direct connections the same class is used, the difference is the class disables bootstrapping and advertising the connection details to the bootstrapping server as this service is reserved specifically for receiving direct connections.
+
+============
+Dependencies
+============
+* netifaces
+* ntplib
+* twisted
+* ipaddress
+* requests
+* nose
+* setuptools
+* pyroute2
+
+Installation: python3.3 setup.py install
+
+Status: Experimental, may have bugs
```

### Comparing `pyp2p-0.8.2/pyp2p/upnp.py` & `pyp2p-0.8.3/pyp2p/upnp.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-import select
-
-from .lib import *
-from .sock import *
-
-from future.moves.urllib.request import urlopen, Request
-
-import platform
-import subprocess
-from threading import Thread
-
-"""
-This is a modified version of "UPnP-Exploiter." It's been
-changed to work with Python 3.3, the code has been
-restructured to make it modular, commented, and easier to use.
-I've also removed the original exploit code and only the port
-forwarding code remains.
-
-Original code available here: https://github.com/dc414/Upnp-Exploiter
-Credits to "Anarchy Angel", "Ngharo", and www.dc414.org
-for the code.
-"""
-
-
-class UPnP:
-    def __init__(self, interface=u"default"):
-        """
-        Port used to listen to UPnP replies on.
-        This port is actually arbitrary because
-        all the sockets used are datagram sockets
-        bound to all address which lets
-        the socket hear broadcasts.
-        """
-        self.listen_port = 49170
-
-        # Port that UPnP configured hosts listen on.
-        self.upnp_port = 1900
-
-        # Address used for IPv4 multicasts.
-        self.multicast = b"239.255.255.250"
-
-        # Number of seconds to wait for replies.
-        self.reply_wait = 3
-
-        # Socket timeout.
-        self.timeout = 2
-
-        # Networking interface.
-        self.interface = interface
-
-        # Address of a UPnP gateway.
-        self.gateway = []
-
-    # Uses broadcasting to find default UPnP compatible gateway.
-    def find_gateway(self):
-        replies = []
-
-        # Create socket for UDP broadcasts.
-        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        s.bind(('', self.upnp_port))  # All addresses.
-        s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-        s.setblocking(0)
-
-        # Broadcast search message to multicast address.
-        search_msg = b"M-SEARCH * HTTP/1.1\r\n"
-        search_msg += b"HOST: %s" + self.multicast + b":"
-        if sys.version_info >= (3, 0, 0):
-            search_msg += str(self.upnp_port).encode("ascii")
-        else:
-            search_msg += str(self.upnp_port)
-        search_msg += b"\r\nST: ssdp:all\r\n"
-        search_msg += b"""MAN: "ssdp:discover"\r\n"""
-        search_msg += b"MX: 1\r\n"
-        search_msg += b"\r\n"
-        s.sendto(search_msg, (self.multicast, self.upnp_port))
-
-        # Receive replies for n seconds..
-        old_time = time.time()
-        while (int(time.time()) - int(old_time)) < self.reply_wait:
-            res = select.select([s], [], [], self.timeout)
-            if len(res[0]):
-                (string, addr) = res[0][0].recvfrom(1024)
-                replies.append([addr[0], string])
-
-        # Cleanup socket.
-        if s is not None:
-            s.close()
-            s = None
-
-        # Error: no UPnP replies - try guess gateway.
-        if not replies:
-            default_gateway = get_default_gateway(self.interface)
-            if default_gateway is None or default_gateway == {}:
-                return None
-            else:
-                # Optimise scanning.
-                likely_candidates = [80, 1780, 1900, 1981, 2468, 5555, 5678,
-                                     49000, 55345, 65535]
-
-                def check_gateway(self, ip, port):
-                    try:
-                        # Fast connect() / SYN open scanning.
-                        s = Sock(ip, port, blocking=1, timeout=5,
-                                 interface=self.interface)
-                        s.close()
-
-                        # Build http request.
-                        gateway_addr = "http://" + str(ip) + ":" +\
-                                       str(port) + "/"
-                        buf = urlopen(gateway_addr, timeout=self.timeout).\
-                            read().decode("utf-8")
-
-                        # Check response is XML and device is a router.
-                        if 'InternetGatewayDevice' in buf:
-                            return self.gateway.append(gateway_addr)
-                    except:
-                        return
-
-                # Brute force port by scanning.
-                for port in likely_candidates:
-                    t = Thread(target=check_gateway,
-                               args=(self, default_gateway, port))
-                    t.start()
-
-                time.sleep(5)
-                if len(self.gateway):
-                    return self.gateway[0]
-                else:
-                    return None
-
-        # Find gateway address in replies.
-        gateway_addr = None
-        pdata = list(dict((x[0], x) for x in replies).values())
-        # return None
-        rh = []
-        for L in pdata:
-            rh.append(L[0])
-        hosts = []
-        pd = []
-        for host in rh:
-            try:
-                spot = rh.index(host)
-                hdata = pdata[spot][1]
-                url = 'http://' + host + ':'
-                port = re.findall("http:\/\/[0-9\.]+:(\d.+)",
-                                  hdata.decode("utf-8"))
-                url += port[0]
-                p = urlopen(url, timeout=self.timeout)
-                rd = re.findall('schemas-upnp-org:device:([^:]+)',
-                                p.read().decode("utf-8"))
-                if rd[0] == 'InternetGatewayDevice':
-                    gateway_addr = url
-                    break
-            except:
-                continue
-
-        return gateway_addr
-
-    def forward_port(self, proto, src_port, dest_ip, dest_port=None):
-        """
-        Creates a new mapping for the default gateway to forward ports.
-        Source port is from the perspective of the original client.
-        For example, if a client tries to connect to us on port 80,
-        the source port is port 80. The destination port isn't
-        necessarily 80, however. We might wish to run our web server
-        on a different port so we can have the router forward requests
-        for port 80 to another port (what I call the destination port.)
-
-        If the destination port isn't specified, it defaults to the
-        source port. Proto is either TCP or UDP. Function returns None
-        on success, otherwise it raises an exception.
-        """
-
-        proto = proto.upper()
-        valid_protos = ["TCP", "UDP"]
-        if proto not in valid_protos:
-            raise Exception("Invalid protocol for forwarding.")
-
-        valid_ports = range(1, 65535)
-        if src_port not in valid_ports:
-            raise Exception("Invalid port for forwarding.")
-
-        # Source port is forwarded to same destination port number.
-        if dest_port is None:
-            dest_port = src_port
-
-        # Use UPnP binary for forwarding on Windows.
-        if platform.system() == "Windows":
-            cmd = "upnpc-static.exe -a %s %s %s %s" % (get_lan_ip(),
-                                                       str(src_port),
-                                                       str(dest_port),
-                                                       proto)
-            out, err = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
-                                        stderr=subprocess.PIPE).communicate()
-            if "is not recognized" in err:
-                raise Exception("Missing upnpc-static.exe")
-            
-            return
-
-        # Find gateway address.
-        gateway_addr = self.find_gateway()
-        if gateway_addr is None:
-            raise Exception("Unable to find UPnP compatible gateway.")
-
-        # Get control URL.
-        rhost = re.findall('([^/]+)', gateway_addr)
-        res = urlopen(gateway_addr, timeout=self.timeout).read().decode("utf-8")
-        res = res.replace('\r', '')
-        res = res.replace('\n', '')
-        res = res.replace('\t', '')
-        pres = res.split('<serviceId>urn:upnp-org:serviceId:WANIPConn1'
-                         '</serviceId>')
-        p2res = pres[1].split('</controlURL>')
-        p3res = p2res[0].split('<controlURL>')
-        ctrl = p3res[1]
-        rip = res.split('<presentationURL>')
-        rip1 = rip[1].split('</presentationURL>')
-        router_ip = rip1[0]
-
-        port_map_desc = "PyP2P"
-        msg = \
-            '<?xml version="1.0"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/"><s:Body><u:AddPortMapping xmlns:u="urn:schemas-upnp-org:service:WANIPConnection:1"><NewRemoteHost></NewRemoteHost><NewExternalPort>' \
-            + str(src_port) \
-            + '</NewExternalPort><NewProtocol>' + str(proto) + '</NewProtocol><NewInternalPort>' \
-            + str(dest_port) + '</NewInternalPort><NewInternalClient>' + str(dest_ip) \
-            + '</NewInternalClient><NewEnabled>1</NewEnabled><NewPortMappingDescription>' + str(port_map_desc) + '</NewPortMappingDescription><NewLeaseDuration>0</NewLeaseDuration></u:AddPortMapping></s:Body></s:Envelope>'
-
-        # Attempt to add new port map.
-        x = 'http://' + rhost[1] + '/' + ctrl
-        if sys.version_info >= (3, 0, 0):
-            msg = bytes(msg, "utf-8")
-
-        req = Request('http://' + rhost[1] + '/' + ctrl, msg)
-        req.add_header('SOAPAction',
-                       '"urn:schemas-upnp-org:service:WANIPConnection:1#AddPortMapping"'
-                       )
-        req.add_header('Content-type', 'application/xml')
-        res = urlopen(req, timeout=self.timeout)
-
-
-if __name__ == "__main__":
-    """
-    if sys.version_info < (3,0,0):
-
-
-    port = 51020
-    addr = "192.168.0.60"
-    forwarding_servers = [{"addr": "158.69.201.105", "port": 80, "url": "/pyp2p/net.php"}]
-
-
-    print(UPnP().forward_port("TCP", port, addr))
-    print(is_port_forwarded(get_lan_ip(), str(port), "TCP", forwarding_servers))
-    """
+import select
+
+from .lib import *
+from .sock import *
+
+from future.moves.urllib.request import urlopen, Request
+
+import platform
+import subprocess
+from threading import Thread
+
+"""
+This is a modified version of "UPnP-Exploiter." It's been
+changed to work with Python 3.3, the code has been
+restructured to make it modular, commented, and easier to use.
+I've also removed the original exploit code and only the port
+forwarding code remains.
+
+Original code available here: https://github.com/dc414/Upnp-Exploiter
+Credits to "Anarchy Angel", "Ngharo", and www.dc414.org
+for the code.
+"""
+
+
+class UPnP:
+    def __init__(self, interface=u"default"):
+        """
+        Port used to listen to UPnP replies on.
+        This port is actually arbitrary because
+        all the sockets used are datagram sockets
+        bound to all address which lets
+        the socket hear broadcasts.
+        """
+        self.listen_port = 49170
+
+        # Port that UPnP configured hosts listen on.
+        self.upnp_port = 1900
+
+        # Address used for IPv4 multicasts.
+        self.multicast = b"239.255.255.250"
+
+        # Number of seconds to wait for replies.
+        self.reply_wait = 3
+
+        # Socket timeout.
+        self.timeout = 2
+
+        # Networking interface.
+        self.interface = interface
+
+        # Address of a UPnP gateway.
+        self.gateway = []
+
+    # Uses broadcasting to find default UPnP compatible gateway.
+    def find_gateway(self):
+        replies = []
+
+        # Create socket for UDP broadcasts.
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        s.bind(('', self.upnp_port))  # All addresses.
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+        s.setblocking(0)
+
+        # Broadcast search message to multicast address.
+        search_msg = b"M-SEARCH * HTTP/1.1\r\n"
+        search_msg += b"HOST: %s" + self.multicast + b":"
+        if sys.version_info >= (3, 0, 0):
+            search_msg += str(self.upnp_port).encode("ascii")
+        else:
+            search_msg += str(self.upnp_port)
+        search_msg += b"\r\nST: ssdp:all\r\n"
+        search_msg += b"""MAN: "ssdp:discover"\r\n"""
+        search_msg += b"MX: 1\r\n"
+        search_msg += b"\r\n"
+        s.sendto(search_msg, (self.multicast, self.upnp_port))
+
+        # Receive replies for n seconds..
+        old_time = time.time()
+        while (int(time.time()) - int(old_time)) < self.reply_wait:
+            res = select.select([s], [], [], self.timeout)
+            if len(res[0]):
+                (string, addr) = res[0][0].recvfrom(1024)
+                replies.append([addr[0], string])
+
+        # Cleanup socket.
+        if s is not None:
+            s.close()
+            s = None
+
+        # Error: no UPnP replies - try guess gateway.
+        if not replies:
+            default_gateway = get_default_gateway(self.interface)
+            if default_gateway is None or default_gateway == {}:
+                return None
+            else:
+                # Optimise scanning.
+                likely_candidates = [80, 1780, 1900, 1981, 2468, 5555, 5678,
+                                     49000, 55345, 65535]
+
+                def check_gateway(self, ip, port):
+                    try:
+                        # Fast connect() / SYN open scanning.
+                        s = Sock(ip, port, blocking=1, timeout=5,
+                                 interface=self.interface)
+                        s.close()
+
+                        # Build http request.
+                        gateway_addr = "http://" + str(ip) + ":" +\
+                                       str(port) + "/"
+                        buf = urlopen(gateway_addr, timeout=self.timeout).\
+                            read().decode("utf-8")
+
+                        # Check response is XML and device is a router.
+                        if 'InternetGatewayDevice' in buf:
+                            return self.gateway.append(gateway_addr)
+                    except:
+                        return
+
+                # Brute force port by scanning.
+                for port in likely_candidates:
+                    t = Thread(target=check_gateway,
+                               args=(self, default_gateway, port))
+                    t.start()
+
+                time.sleep(5)
+                if len(self.gateway):
+                    return self.gateway[0]
+                else:
+                    return None
+
+        # Find gateway address in replies.
+        gateway_addr = None
+        pdata = list(dict((x[0], x) for x in replies).values())
+        # return None
+        rh = []
+        for L in pdata:
+            rh.append(L[0])
+        hosts = []
+        pd = []
+        for host in rh:
+            try:
+                spot = rh.index(host)
+                hdata = pdata[spot][1]
+                url = 'http://' + host + ':'
+                port = re.findall("http:\/\/[0-9\.]+:(\d.+)",
+                                  hdata.decode("utf-8"))
+                url += port[0]
+                p = urlopen(url, timeout=self.timeout)
+                rd = re.findall('schemas-upnp-org:device:([^:]+)',
+                                p.read().decode("utf-8"))
+                if rd[0] == 'InternetGatewayDevice':
+                    gateway_addr = url
+                    break
+            except:
+                continue
+
+        return gateway_addr
+
+    def forward_port(self, proto, src_port, dest_ip, dest_port=None):
+        """
+        Creates a new mapping for the default gateway to forward ports.
+        Source port is from the perspective of the original client.
+        For example, if a client tries to connect to us on port 80,
+        the source port is port 80. The destination port isn't
+        necessarily 80, however. We might wish to run our web server
+        on a different port so we can have the router forward requests
+        for port 80 to another port (what I call the destination port.)
+
+        If the destination port isn't specified, it defaults to the
+        source port. Proto is either TCP or UDP. Function returns None
+        on success, otherwise it raises an exception.
+        """
+
+        proto = proto.upper()
+        valid_protos = ["TCP", "UDP"]
+        if proto not in valid_protos:
+            raise Exception("Invalid protocol for forwarding.")
+
+        valid_ports = range(1, 65535)
+        if src_port not in valid_ports:
+            raise Exception("Invalid port for forwarding.")
+
+        # Source port is forwarded to same destination port number.
+        if dest_port is None:
+            dest_port = src_port
+
+        # Use UPnP binary for forwarding on Windows.
+        if platform.system() == "Windows":
+            cmd = "upnpc-static.exe -a %s %s %s %s" % (get_lan_ip(),
+                                                       str(src_port),
+                                                       str(dest_port),
+                                                       proto)
+            out, err = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
+                                        stderr=subprocess.PIPE).communicate()
+            if "is not recognized" in err:
+                raise Exception("Missing upnpc-static.exe")
+            
+            return
+
+        # Find gateway address.
+        gateway_addr = self.find_gateway()
+        if gateway_addr is None:
+            raise Exception("Unable to find UPnP compatible gateway.")
+
+        # Get control URL.
+        rhost = re.findall('([^/]+)', gateway_addr)
+        res = urlopen(gateway_addr, timeout=self.timeout).read().decode("utf-8")
+        res = res.replace('\r', '')
+        res = res.replace('\n', '')
+        res = res.replace('\t', '')
+        pres = res.split('<serviceId>urn:upnp-org:serviceId:WANIPConn1'
+                         '</serviceId>')
+        p2res = pres[1].split('</controlURL>')
+        p3res = p2res[0].split('<controlURL>')
+        ctrl = p3res[1]
+        rip = res.split('<presentationURL>')
+        rip1 = rip[1].split('</presentationURL>')
+        router_ip = rip1[0]
+
+        port_map_desc = "PyP2P"
+        msg = \
+            '<?xml version="1.0"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/"><s:Body><u:AddPortMapping xmlns:u="urn:schemas-upnp-org:service:WANIPConnection:1"><NewRemoteHost></NewRemoteHost><NewExternalPort>' \
+            + str(src_port) \
+            + '</NewExternalPort><NewProtocol>' + str(proto) + '</NewProtocol><NewInternalPort>' \
+            + str(dest_port) + '</NewInternalPort><NewInternalClient>' + str(dest_ip) \
+            + '</NewInternalClient><NewEnabled>1</NewEnabled><NewPortMappingDescription>' + str(port_map_desc) + '</NewPortMappingDescription><NewLeaseDuration>0</NewLeaseDuration></u:AddPortMapping></s:Body></s:Envelope>'
+
+        # Attempt to add new port map.
+        x = 'http://' + rhost[1] + '/' + ctrl
+        if sys.version_info >= (3, 0, 0):
+            msg = bytes(msg, "utf-8")
+
+        req = Request('http://' + rhost[1] + '/' + ctrl, msg)
+        req.add_header('SOAPAction',
+                       '"urn:schemas-upnp-org:service:WANIPConnection:1#AddPortMapping"'
+                       )
+        req.add_header('Content-type', 'application/xml')
+        res = urlopen(req, timeout=self.timeout)
+
+
+if __name__ == "__main__":
+    """
+    if sys.version_info < (3,0,0):
+
+
+    port = 51020
+    addr = "192.168.0.60"
+    forwarding_servers = [{"addr": "158.69.201.105", "port": 80, "url": "/pyp2p/net.php"}]
+
+
+    print(UPnP().forward_port("TCP", port, addr))
+    print(is_port_forwarded(get_lan_ip(), str(port), "TCP", forwarding_servers))
+    """
```

### Comparing `pyp2p-0.8.2/pyp2p/nat_pmp.py` & `pyp2p-0.8.3/pyp2p/nat_pmp.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.2/pyp2p/ipgetter.py` & `pyp2p-0.8.3/pyp2p/ipgetter.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.2/pyp2p/sys_clock.py` & `pyp2p-0.8.3/pyp2p/sys_clock.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-"""
-Given an NTP accurate time, this module computes an
-approximation of how far off the system clock is
-from the NTP time (clock skew.) The algorithm was
-taken from gtk-gnutella.
-
-https://github.com/gtk-gnutella/gtk-gnutella/
-blob/devel/src/core/clock.c 
-"""
-
-
-from decimal import Decimal
-
-from .lib import *
-
-
-class SysClock:
-    def __init__(self, clock_skew=Decimal("0")):
-        self.enough_data = 40
-        self.min_data = 20
-        self.max_sdev = 60
-        self.clean_steps = 3
-        self.data_points = []
-        self.clock_skew = clock_skew
-        if not self.clock_skew:
-            self.collect_data_points()
-            self.clock_skew = self.calculate_clock_skew()
-
-    def time(self):
-        return Decimal(time.time()) - self.clock_skew
-
-    def collect_data_points(self):
-        while len(self.data_points) < self.enough_data + 10:
-            clock_skew = Decimal(time.time()) - Decimal(get_ntp())
-            self.data_points.append(clock_skew)
-
-    def statx_n(self, data_points):
-        return len(data_points)
-
-    def statx_avg(self, data_points):
-        total = Decimal("0")
-        n = self.statx_n(data_points)
-        for i in range(0, n):
-            total += data_points[i]
-
-        return total / Decimal(n)
-
-    def statx_sdev(self, data_points):
-        def _ss(data):
-            """Return sum of square deviations of sequence data."""
-            c = self.statx_avg(data)
-            ss = sum((x-c)**2 for x in data)
-            return ss
-
-        def pstdev(data):
-            """Calculates the population standard deviation."""
-            n = len(data)
-            if n < 2:
-                raise ValueError('variance requires at least two data points')
-            ss = _ss(data)
-            pvar = ss/n  # the population variance
-            return pvar**Decimal("0.5")
-
-        return pstdev(data_points)
-
-    def calculate_clock_skew(self):
-        """
-        Computer average and standard deviation
-        using all the data points.
-        """
-        n = self.statx_n(self.data_points)
-
-        """
-        Required to be able to compute the standard
-        deviation.
-        """
-        if n < 1:
-            return Decimal("0")
-
-        avg = self.statx_avg(self.data_points)
-        sdev = self.statx_sdev(self.data_points)
-
-        """
-        Incrementally remove aberration points.
-        """
-        for k in range(0, self.clean_steps):
-            """
-            Remove aberration points: keep only
-            the sigma range around the average.
-            """
-            min_val = avg - sdev
-            max_val = avg + sdev
-
-            cleaned_data_points = []
-            for i in range(0, n):
-                v = self.data_points[i]
-                if v < min_val or v > max_val:
-                    continue
-                cleaned_data_points.append(v)
-
-            self.data_points = cleaned_data_points[:]
-
-            """
-            Recompute the new average using the
-            "sound" points we kept.
-            """
-            n = self.statx_n(self.data_points)
-
-            """
-            Not enough data to compute standard
-            deviation.
-            """
-            if n < 2:
-                break
-
-            avg = self.statx_avg(self.data_points)
-            sdev = self.statx_sdev(self.data_points)
-
-            if sdev <= self.max_sdev or n < self.min_data:
-                break
-
-        """
-        If standard deviation is too large still, we
-        cannot update our clock. Collect more points.
-
-        If we don't have a minimum amount of data,
-        don't attempt the update yet, continue collecting.
-        """
-        if sdev > self.max_sdev or n < self.min_data:
-            return Decimal("0")
-
-        return avg
-        
-if __name__ == "__main__":
-    sys_clock = SysClock()
-    print(sys_clock.clock_skew)
-
-    while 0:
-        sys_clock = SysClock()
-        ntp = Decimal(get_ntp())
-        adjusted = sys_clock.time()
-        dif = ntp - adjusted
-        if dif < 0:
-            dif = -dif
-
-        print(dif)
-        if dif < 0.05:
-            break
-
-    # print(get_ntp())
-    # print(get_ntp())
-
-    """
-    print(sys_clock.time())
-    print()
-    print(get_ntp())
-    print(sys_clock.time())
-    print()
-    print(get_ntp())
-    print(sys_clock.time())
-    """
-
+"""
+Given an NTP accurate time, this module computes an
+approximation of how far off the system clock is
+from the NTP time (clock skew.) The algorithm was
+taken from gtk-gnutella.
+
+https://github.com/gtk-gnutella/gtk-gnutella/
+blob/devel/src/core/clock.c 
+"""
+
+
+from decimal import Decimal
+
+from .lib import *
+
+
+class SysClock:
+    def __init__(self, clock_skew=Decimal("0")):
+        self.enough_data = 40
+        self.min_data = 20
+        self.max_sdev = 60
+        self.clean_steps = 3
+        self.data_points = []
+        self.clock_skew = clock_skew
+        if not self.clock_skew:
+            self.collect_data_points()
+            self.clock_skew = self.calculate_clock_skew()
+
+    def time(self):
+        return Decimal(time.time()) - self.clock_skew
+
+    def collect_data_points(self):
+        while len(self.data_points) < self.enough_data + 10:
+            clock_skew = Decimal(time.time()) - Decimal(get_ntp())
+            self.data_points.append(clock_skew)
+
+    def statx_n(self, data_points):
+        return len(data_points)
+
+    def statx_avg(self, data_points):
+        total = Decimal("0")
+        n = self.statx_n(data_points)
+        for i in range(0, n):
+            total += data_points[i]
+
+        return total / Decimal(n)
+
+    def statx_sdev(self, data_points):
+        def _ss(data):
+            """Return sum of square deviations of sequence data."""
+            c = self.statx_avg(data)
+            ss = sum((x-c)**2 for x in data)
+            return ss
+
+        def pstdev(data):
+            """Calculates the population standard deviation."""
+            n = len(data)
+            if n < 2:
+                raise ValueError('variance requires at least two data points')
+            ss = _ss(data)
+            pvar = ss/n  # the population variance
+            return pvar**Decimal("0.5")
+
+        return pstdev(data_points)
+
+    def calculate_clock_skew(self):
+        """
+        Computer average and standard deviation
+        using all the data points.
+        """
+        n = self.statx_n(self.data_points)
+
+        """
+        Required to be able to compute the standard
+        deviation.
+        """
+        if n < 1:
+            return Decimal("0")
+
+        avg = self.statx_avg(self.data_points)
+        sdev = self.statx_sdev(self.data_points)
+
+        """
+        Incrementally remove aberration points.
+        """
+        for k in range(0, self.clean_steps):
+            """
+            Remove aberration points: keep only
+            the sigma range around the average.
+            """
+            min_val = avg - sdev
+            max_val = avg + sdev
+
+            cleaned_data_points = []
+            for i in range(0, n):
+                v = self.data_points[i]
+                if v < min_val or v > max_val:
+                    continue
+                cleaned_data_points.append(v)
+
+            self.data_points = cleaned_data_points[:]
+
+            """
+            Recompute the new average using the
+            "sound" points we kept.
+            """
+            n = self.statx_n(self.data_points)
+
+            """
+            Not enough data to compute standard
+            deviation.
+            """
+            if n < 2:
+                break
+
+            avg = self.statx_avg(self.data_points)
+            sdev = self.statx_sdev(self.data_points)
+
+            if sdev <= self.max_sdev or n < self.min_data:
+                break
+
+        """
+        If standard deviation is too large still, we
+        cannot update our clock. Collect more points.
+
+        If we don't have a minimum amount of data,
+        don't attempt the update yet, continue collecting.
+        """
+        if sdev > self.max_sdev or n < self.min_data:
+            return Decimal("0")
+
+        return avg
+        
+if __name__ == "__main__":
+    sys_clock = SysClock()
+    print(sys_clock.clock_skew)
+
+    while 0:
+        sys_clock = SysClock()
+        ntp = Decimal(get_ntp())
+        adjusted = sys_clock.time()
+        dif = ntp - adjusted
+        if dif < 0:
+            dif = -dif
+
+        print(dif)
+        if dif < 0.05:
+            break
+
+    # print(get_ntp())
+    # print(get_ntp())
+
+    """
+    print(sys_clock.time())
+    print()
+    print(get_ntp())
+    print(sys_clock.time())
+    print()
+    print(get_ntp())
+    print(sys_clock.time())
+    """
+
```

### Comparing `pyp2p-0.8.2/pyp2p/net.py` & `pyp2p-0.8.3/pyp2p/net.py`

 * *Files 0% similar despite different names*

```diff
@@ -715,18 +715,15 @@
         """
 
         self.debug_print("Starting networking.")
         self.debug_print("Make sure to iterate over replies if you need"
                          " connection alive management!")
 
         # Register a cnt + c handler
-        try:
-            signal.signal(signal.SIGINT, self.stop)
-        except:
-            pass
+        signal.signal(signal.SIGINT, self.stop)
 
         # Save WAN IP.
         self.debug_print("WAN IP = " + str(self.wan_ip))
 
         # Check rendezvous server is up.
         try:
             rendezvous_con = self.rendezvous.server_connect()
```

### Comparing `pyp2p-0.8.2/pyp2p/ip_routes.py` & `pyp2p-0.8.3/pyp2p/ip_routes.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import platform
-
-if platform.system() == "Windows":
-    import ctypes
-    from ctypes import windll
-    from ctypes import wintypes
-
-    kernel32 = windll.kernel32
-    iphlpapi = windll.iphlpapi
-    Ws2_32 = windll.Ws2_32
-    ERROR_INSUFFICIENT_BUFFER = 122
-    ERROR_NO_DATA = 232
-
-    class Win32MIBIPFORWARDROW(ctypes.Structure):
-        _fields_ = [
-            ('dwForwardDest', wintypes.DWORD),
-            ('dwForwardMask', wintypes.DWORD),
-            ('dwForwardPolicy', wintypes.DWORD),
-            ('dwForwardNextHop', wintypes.DWORD),
-            ('dwForwardIfIndex', wintypes.DWORD),
-            ('dwForwardType', wintypes.DWORD),
-            ('dwForwardProto', wintypes.DWORD),
-            ('dwForwardAge', wintypes.DWORD),
-            ('dwForwardNextHopAS', wintypes.DWORD),
-            ('dwForwardMetric1', wintypes.DWORD),
-            ('dwForwardMetric2', wintypes.DWORD),
-            ('dwForwardMetric3', wintypes.DWORD),
-            ('dwForwardMetric4', wintypes.DWORD),
-            ('dwForwardMetric5', wintypes.DWORD)
-        ]
-
-    class Win32MIBIPFORWARDTABLE(ctypes.Structure):
-        _fields_ = [
-            ('dwNumEntries', wintypes.DWORD),
-            ('table', Win32MIBIPFORWARDROW * 1)
-        ]
-
-    kernel32.GetProcessHeap.argtypes = []
-    kernel32.GetProcessHeap.restype = wintypes.HANDLE
-
-    # Note: wintypes.ULONG must be replaced with a 64 bit variable on x64
-    kernel32.HeapAlloc.argtypes = [wintypes.HANDLE, wintypes.DWORD,
-                                   wintypes.ULONG]
-    kernel32.HeapAlloc.restype = wintypes.LPVOID
-
-    kernel32.HeapFree.argtypes = [wintypes.HANDLE, wintypes.DWORD,
-                                  wintypes.LPVOID]
-    kernel32.HeapFree.restype = wintypes.BOOL
-
-    iphlpapi.GetIpForwardTable.argtypes = [
-        ctypes.POINTER(Win32MIBIPFORWARDTABLE),
-        ctypes.POINTER(wintypes.ULONG),
-        wintypes.BOOL]
-    iphlpapi.GetIpForwardTable.restype = wintypes.DWORD
-
-    Ws2_32.inet_ntoa.restype = ctypes.c_char_p
-
-    def get_ipv4_routing_table():
-        routing_table = []
-
-        heap = kernel32.GetProcessHeap()
-
-        size = wintypes.ULONG(ctypes.sizeof(Win32MIBIPFORWARDTABLE))
-        p = kernel32.HeapAlloc(heap, 0, size)
-        if not p:
-            raise Exception('Unable to allocate memory for the IP forward '
-                            'table')
-        p_forward_table = ctypes.cast(
-            p, ctypes.POINTER(Win32MIBIPFORWARDTABLE))
-
-        try:
-            err = iphlpapi.GetIpForwardTable(p_forward_table,
-                                             ctypes.byref(size), 0)
-            if err == ERROR_INSUFFICIENT_BUFFER:
-                kernel32.HeapFree(heap, 0, p_forward_table)
-                p = kernel32.HeapAlloc(heap, 0, size)
-                if not p:
-                    raise Exception('Unable to allocate memory for the IP '
-                                    'forward table')
-                p_forward_table = ctypes.cast(
-                    p, ctypes.POINTER(Win32MIBIPFORWARDTABLE))
-
-            err = iphlpapi.GetIpForwardTable(p_forward_table,
-                                             ctypes.byref(size), 0)
-            if err != ERROR_NO_DATA:
-                if err:
-                    raise Exception('Unable to get IP forward table. '
-                                    'Error: %s' % err)
-
-                forward_table = p_forward_table.contents
-                table = ctypes.cast(
-                    ctypes.addressof(forward_table.table),
-                    ctypes.POINTER(Win32MIBIPFORWARDROW *
-                                   forward_table.dwNumEntries)).contents
-
-                i = 0
-                while i < forward_table.dwNumEntries:
-                    row = table[i]
-                    routing_table.append((
-                        Ws2_32.inet_ntoa(row.dwForwardDest),
-                        Ws2_32.inet_ntoa(row.dwForwardMask),
-                        Ws2_32.inet_ntoa(row.dwForwardNextHop),
-                        row.dwForwardIfIndex,
-                        row.dwForwardMetric1))
-                    i += 1
-
-            return routing_table
-        finally:
-            kernel32.HeapFree(heap, 0, p_forward_table)
+import platform
+
+if platform.system() == "Windows":
+    import ctypes
+    from ctypes import windll
+    from ctypes import wintypes
+
+    kernel32 = windll.kernel32
+    iphlpapi = windll.iphlpapi
+    Ws2_32 = windll.Ws2_32
+    ERROR_INSUFFICIENT_BUFFER = 122
+    ERROR_NO_DATA = 232
+
+    class Win32MIBIPFORWARDROW(ctypes.Structure):
+        _fields_ = [
+            ('dwForwardDest', wintypes.DWORD),
+            ('dwForwardMask', wintypes.DWORD),
+            ('dwForwardPolicy', wintypes.DWORD),
+            ('dwForwardNextHop', wintypes.DWORD),
+            ('dwForwardIfIndex', wintypes.DWORD),
+            ('dwForwardType', wintypes.DWORD),
+            ('dwForwardProto', wintypes.DWORD),
+            ('dwForwardAge', wintypes.DWORD),
+            ('dwForwardNextHopAS', wintypes.DWORD),
+            ('dwForwardMetric1', wintypes.DWORD),
+            ('dwForwardMetric2', wintypes.DWORD),
+            ('dwForwardMetric3', wintypes.DWORD),
+            ('dwForwardMetric4', wintypes.DWORD),
+            ('dwForwardMetric5', wintypes.DWORD)
+        ]
+
+    class Win32MIBIPFORWARDTABLE(ctypes.Structure):
+        _fields_ = [
+            ('dwNumEntries', wintypes.DWORD),
+            ('table', Win32MIBIPFORWARDROW * 1)
+        ]
+
+    kernel32.GetProcessHeap.argtypes = []
+    kernel32.GetProcessHeap.restype = wintypes.HANDLE
+
+    # Note: wintypes.ULONG must be replaced with a 64 bit variable on x64
+    kernel32.HeapAlloc.argtypes = [wintypes.HANDLE, wintypes.DWORD,
+                                   wintypes.ULONG]
+    kernel32.HeapAlloc.restype = wintypes.LPVOID
+
+    kernel32.HeapFree.argtypes = [wintypes.HANDLE, wintypes.DWORD,
+                                  wintypes.LPVOID]
+    kernel32.HeapFree.restype = wintypes.BOOL
+
+    iphlpapi.GetIpForwardTable.argtypes = [
+        ctypes.POINTER(Win32MIBIPFORWARDTABLE),
+        ctypes.POINTER(wintypes.ULONG),
+        wintypes.BOOL]
+    iphlpapi.GetIpForwardTable.restype = wintypes.DWORD
+
+    Ws2_32.inet_ntoa.restype = ctypes.c_char_p
+
+    def get_ipv4_routing_table():
+        routing_table = []
+
+        heap = kernel32.GetProcessHeap()
+
+        size = wintypes.ULONG(ctypes.sizeof(Win32MIBIPFORWARDTABLE))
+        p = kernel32.HeapAlloc(heap, 0, size)
+        if not p:
+            raise Exception('Unable to allocate memory for the IP forward '
+                            'table')
+        p_forward_table = ctypes.cast(
+            p, ctypes.POINTER(Win32MIBIPFORWARDTABLE))
+
+        try:
+            err = iphlpapi.GetIpForwardTable(p_forward_table,
+                                             ctypes.byref(size), 0)
+            if err == ERROR_INSUFFICIENT_BUFFER:
+                kernel32.HeapFree(heap, 0, p_forward_table)
+                p = kernel32.HeapAlloc(heap, 0, size)
+                if not p:
+                    raise Exception('Unable to allocate memory for the IP '
+                                    'forward table')
+                p_forward_table = ctypes.cast(
+                    p, ctypes.POINTER(Win32MIBIPFORWARDTABLE))
+
+            err = iphlpapi.GetIpForwardTable(p_forward_table,
+                                             ctypes.byref(size), 0)
+            if err != ERROR_NO_DATA:
+                if err:
+                    raise Exception('Unable to get IP forward table. '
+                                    'Error: %s' % err)
+
+                forward_table = p_forward_table.contents
+                table = ctypes.cast(
+                    ctypes.addressof(forward_table.table),
+                    ctypes.POINTER(Win32MIBIPFORWARDROW *
+                                   forward_table.dwNumEntries)).contents
+
+                i = 0
+                while i < forward_table.dwNumEntries:
+                    row = table[i]
+                    routing_table.append((
+                        Ws2_32.inet_ntoa(row.dwForwardDest),
+                        Ws2_32.inet_ntoa(row.dwForwardMask),
+                        Ws2_32.inet_ntoa(row.dwForwardNextHop),
+                        row.dwForwardIfIndex,
+                        row.dwForwardMetric1))
+                    i += 1
+
+            return routing_table
+        finally:
+            kernel32.HeapFree(heap, 0, p_forward_table)
```

### Comparing `pyp2p-0.8.2/pyp2p/hybrid_reply.py` & `pyp2p-0.8.3/pyp2p/hybrid_reply.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.2/pyp2p/rendezvous_server.py` & `pyp2p-0.8.3/pyp2p/rendezvous_server.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.2/pyp2p/lib.py` & `pyp2p-0.8.3/pyp2p/lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,491 +1,494 @@
-import netifaces
-import os
-import struct
-import sys
-import time
-import psutil
-import gc
-import ipaddress
-import ntplib
-import re
-from future.moves.urllib.request import urlopen
-
-import traceback
-from .ipgetter import *
-from .ip_routes import *
-
-if platform.system() == "Linux":
-    try:
-        from pyroute2 import IPDB
-        ip = IPDB()
-    except IOError:
-        ip = None
-else:
-    ip = None
-
-
-def get_unused_port():
-    """Checks if port is already in use."""
-    port = random.randint(1024, 65535)
-    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    try:
-        s.bind(('', port))  # Try to open port
-    except socket.error as e:
-        if e.errno in (98, 10048):  # 98, 10048 means address already bound
-            return get_unused_port()
-        raise e
-    s.close()
-    return port
-
-
-def log_exception(file_path, msg):
-    msg = "\r\n" + msg
-    with open(file_path, "a") as error_log:
-        error_log.write(msg)
-
-
-def parse_exception(e, output=0):
-    tb = traceback.format_exc()
-    exc_type, exc_obj, exc_tb = sys.exc_info()
-    fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-    error = "%s %s %s %s %s" % (str(tb), str(exc_type), str(fname),
-                                str(exc_tb.tb_lineno), str(e))
-
-    if output:
-        print(error)
-
-    return str(error)
-
-
-def ip2int(addr):
-    return struct.unpack("!I", socket.inet_aton(addr))[0]
-
-
-def int2ip(addr):
-    return socket.inet_ntoa(struct.pack("!I", addr))
-
-# Patches for urllib2 and requests to bind on specific interface.
-# http://rossbates.com/2009/10/26/urllib2-with-multiple-network-interfaces/
-true_socket = socket.socket
-
-
-def build_bound_socket(source_ip):
-    def bound_socket(*a, **k):
-        if source_ip == "127.0.0.1":
-            raise Exception("This function requires a LAN IP"
-                            " (127.0.0.1 passed.)")
-
-        sock = true_socket(*a, **k)
-        sock.bind((source_ip, 0))
-        return sock
-
-    return bound_socket
-
-
-def busy_wait(dt):
-    # Use most accurate timer.
-    if platform.system() == "Windows":
-        timer = time.clock
-    else:
-        timer = time.time
-
-    current_time = timer()
-    while timer() < current_time + dt:
-        pass
-
-
-def get_ntp_worker(server):
-    try:
-        client = ntplib.NTPClient()
-        response = client.request(server, version=3)
-        ntp = response.tx_time
-        return ntp
-    except Exception as e:
-        return None
-
-ntp_servers = [
-    "pool.ntp.org",
-    "2.pool.ntp.org",
-    "0.pool.ntp.org",
-    "1.pool.ntp.org",
-    "3.pool.ntp.org"
-]
-
-bad_ntp_servers = None
-
-
-def remove_bad_ntp_servers():
-    global ntp_servers
-    global bad_ntp_servers
-
-    bad_ntp_servers = []
-    for server in ntp_servers:
-        ntp = get_ntp_worker(server)
-        if ntp is None:
-            bad_ntp_servers.append(server)
-
-    for server in bad_ntp_servers:
-        ntp_servers.remove(server)
-
-
-def get_ntp(local_time=0):
-    global ntp_servers
-    global bad_ntp_servers
-
-    if local_time:
-        return time.time()
-
-    if bad_ntp_servers is None:
-        remove_bad_ntp_servers()
-
-    random.shuffle(ntp_servers, random.random)
-    for server in ntp_servers:
-        ntp = get_ntp_worker(server)
-        if ntp is not None:
-            return ntp
-
-    return None
-
-
-def get_default_gateway(interface="default"):
-    if sys.version_info < (3, 0, 0):
-        if type(interface) == str:
-            interface = unicode(interface)
-    else:
-        if type(interface) == bytes:
-            interface = interface.decode("utf-8")
-
-    if platform.system() == "Windows":
-        if interface == "default":
-            default_routes = [r for r in get_ipv4_routing_table()
-                              if r[0] == '0.0.0.0']
-            if default_routes:
-                return default_routes[0][2]
-
-    try:
-        gws = netifaces.gateways()
-        if sys.version_info < (3, 0, 0):
-            return gws[interface][netifaces.AF_INET][0].decode("utf-8")
-        else:
-            return gws[interface][netifaces.AF_INET][0]
-    except:
-        # This can also mean the machine is directly accessible.
-        return None
-
-
-def get_lan_ip(interface="default"):
-    if sys.version_info < (3, 0, 0):
-        if type(interface) == str:
-            interface = unicode(interface)
-    else:
-        if type(interface) == bytes:
-            interface = interface.decode("utf-8")
-
-    # Get ID of interface that handles WAN stuff.
-    default_gateway = get_default_gateway(interface)
-    gateways = netifaces.gateways()
-    wan_id = None
-    if netifaces.AF_INET in gateways:
-        gw_list = gateways[netifaces.AF_INET]
-        for gw_info in gw_list:
-            if gw_info[0] == default_gateway:
-                wan_id = gw_info[1]
-                break
-
-    # Find LAN IP of interface for WAN stuff.
-    interfaces = netifaces.interfaces()
-    if wan_id in interfaces:
-        families = netifaces.ifaddresses(wan_id)
-        if netifaces.AF_INET in families:
-            if_info_list = families[netifaces.AF_INET]
-            for if_info in if_info_list:
-                if "addr" in if_info:
-                    return if_info["addr"]
-
-    """
-    Execution may reach here if the host is using
-    virtual interfaces on Linux and there are no gateways
-    which suggests the host is a VPS or server. In this
-    case
-    """
-    if platform.system() == "Linux":
-        if ip is not None:
-            return ip.routes["8.8.8.8"]["prefsrc"]
-
-    return None
-
-
-def sequential_bind(n, interface="default"):
-    # Get bind address.
-    addr = ''
-    if interface != "default":
-        addr = get_lan_ip(interface)
-
-    # Start the process.
-    bound = 0
-    mappings = []
-    prospects = []
-    while not bound:
-        # Grab a random place to start.
-        bound = 1
-        start = random.randrange(1024, 65535 - n)
-
-        # Use connect to see if its already bound.
-        for i in range(0, n):
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            local = start + i
-            try:
-                sock.connect((addr, local))
-                sock.close()
-                bound = 0
-                break
-            except socket.error:
-                pass
-
-            prospect = {
-                "local": local,
-            }
-            prospects.append(prospect)
-
-        for prospect in prospects:
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            try:
-                sock.bind((addr, prospect["local"]))
-            except Exception as e:
-                bound = 0
-                for mapping in mappings:
-                    mapping["sock"].close()
-                mappings = []
-                break
-
-            mapping = {
-                "source": prospect["local"],
-                "sock": sock
-            }
-            mappings.append(mapping)
-
-    return mappings
-
-
-def is_port_forwarded(source_ip, port, proto, forwarding_servers):
-    global true_socket
-    if source_ip is not None:
-        socket.socket = build_bound_socket(source_ip)
-
-    ret = 0
-    for forwarding_server in forwarding_servers:
-        url = "http://" + forwarding_server["addr"] + ":"
-        url += str(forwarding_server["port"])
-        url += forwarding_server["url"]
-        url += "?action=is_port_forwarded&port=" + str(port)
-        url += "&proto=" + str(proto.upper())
-
-        try:
-            r = urlopen(url, timeout=2)
-            response = r.read().decode("utf-8")
-            if "yes" in response:
-                ret = 1
-                break
-        except:
-            continue
-
-    socket.socket = true_socket
-    return ret
-
-
-def is_ip_private(ip_addr):
-    if sys.version_info < (3, 0, 0):
-        if type(ip_addr) == str:
-            ip_addr = unicode(ip_addr)
-    else:
-        if type(ip_addr) == bytes:
-            ip_addr = ip_addr.decode("utf-8")
-
-    if ipaddress.ip_address(ip_addr).is_private and ip_addr != "127.0.0.1":
-        return 1
-    else:
-        return 0
-
-
-def is_ip_public(ip_addr):
-    if sys.version_info < (3, 0, 0):
-        if type(ip_addr) == str:
-            ip_addr = unicode(ip_addr)
-    else:
-        if type(ip_addr) == bytes:
-            ip_addr = ip_addr.decode("utf-8")
-
-    if is_ip_private(ip_addr):
-        return 0
-    elif ip_addr == "127.0.0.1":
-        return 0
-    else:
-        return 1
-
-
-def is_ip_valid(ip_addr):
-    if sys.version_info < (3, 0, 0):
-        if type(ip_addr) == str:
-            ip_addr = unicode(ip_addr)
-    else:
-        if type(ip_addr) == bytes:
-            ip_addr = ip_addr.decode("utf-8")
-
-    try:
-        ipaddress.ip_address(ip_addr)
-        return 1
-    except:
-        return 0
-
-
-def is_valid_port(port):
-    try:
-        port = int(port)
-    except:
-        return 0
-    if port < 1 or port > 65535:
-        return 0
-    else:
-        return 1
-
-
-def memoize(function):
-    memo = {}
-
-    def wrapper(*args):
-        if args in memo:
-            return memo[args]
-        else:
-            rv = function(*args)
-            memo[args] = rv
-            return rv
-    return wrapper
-
-
-def extract_ip(s):
-    ip = re.findall("[0-9]+[.][0-9]+[.][0-9]+[.][0-9]+", s)
-    if len(ip):
-        return ip[0]
-
-    return ""
-
-
-@memoize
-def get_wan_ip(n=0):
-    """
-    That IP module sucks. Occasionally it returns an IP address behind
-    cloudflare which probably happens when cloudflare tries to proxy your web
-    request because it thinks you're trying to DoS. It's better if we just run
-    our own infrastructure.
-    """
-
-    if n == 2:
-        try:
-            ip = myip()
-            ip = extract_ip(ip)
-            if is_ip_valid(ip):
-                return ip
-        except Exception as e:
-            print(str(e))
-            return None
-
-    # Fail-safe: use centralized server for IP lookup.
-    from pyp2p.net import forwarding_servers
-    for forwarding_server in forwarding_servers:
-        url = "http://" + forwarding_server["addr"] + ":"
-        url += str(forwarding_server["port"])
-        url += forwarding_server["url"]
-        url += "?action=get_wan_ip"
-        try:
-            r = urlopen(url, timeout=5)
-            response = r.read().decode("utf-8")
-            response = extract_ip(response)
-            if is_ip_valid(response):
-                return response
-        except Exception as e:
-            print(str(e))
-            continue
-
-    time.sleep(1)
-    return get_wan_ip(n + 1)
-
-
-def request_priority_execution():
-    gc.disable()
-    sys.setcheckinterval(999999999)
-    if sys.version_info > (3, 0, 0):
-        sys.setswitchinterval(1000)
-    p = psutil.Process(os.getpid())
-    try:
-        if platform.system() == "Windows":
-            p.nice(psutil.HIGH_PRIORITY_CLASS)
-        else:
-            p.nice(10)
-    except psutil.AccessDenied:
-        pass
-
-    return p
-
-
-def release_priority_execution(p):
-    sys.setcheckinterval(100)
-    if sys.version_info > (3, 0, 0):
-        sys.setswitchinterval(0.005)
-    try:
-        if platform.system() == "Windows":
-            p.nice(psutil.NORMAL_PRIORITY_CLASS)
-        else:
-            p.nice(5)
-    except psutil.AccessDenied:
-        pass
-    gc.enable()
-
-
-def encode_str(s, encoding="unicode"):
-    # Encode unsafe binary to unicode
-    # Encode unsafe unicode to binary
-    if sys.version_info >= (3, 0, 0):
-        # str in Python 3+ is unicode.
-        if type(s) == str:
-            if encoding == "ascii":
-                # Encodes unicode directly as bytes.
-                codes = []
-                for ch in s:
-                    codes.append(ord(ch))
-
-                if len(codes):
-                    return bytes(codes)
-                else:
-                    return b""
-        else:
-            # bytes
-            if encoding == "unicode":
-                # Converts bytes to unicode.
-                return s.decode("utf-8")
-    else:
-        # unicode in python 2 is unicode.
-        if type(s) == unicode:
-            # Encodes unicode directly as bytes.
-            if encoding == "ascii":
-                byte_str = b""
-                for ch in s:
-                    byte_str += chr(ord(ch))
-
-                return byte_str
-        else:
-            # bytes.
-            if encoding == "unicode":
-                # Converts bytes to unicode.
-                return s.decode("utf-8")
-
-    if type(s) == type(u""):
-        s = s.encode("utf-8")
-
-    return s
-
-if __name__ == "__main__":
-    # print(get_wan_ip())
-    # pass
-    print("In lib")
-
+import netifaces
+import os
+import struct
+import sys
+import time
+import psutil
+import gc
+import ipaddress
+import ntplib
+import re
+from future.moves.urllib.request import urlopen
+
+import traceback
+from .ipgetter import *
+from .ip_routes import *
+
+if platform.system() == "Linux":
+    try:
+        from pyroute2 import IPDB
+        ip = IPDB()
+    except IOError:
+        ip = None
+else:
+    ip = None
+
+
+def get_unused_port(port=None):
+    """Checks if port is already in use."""
+    if port is None or port < 1024 or port > 65535:
+        port = random.randint(1024, 65535)
+    assert(1024 <= port <= 65535)
+    while True:
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        try:
+            s.bind(('', port))  # Try to open port
+        except socket.error as e:
+            if e.errno in (98, 10048):  # 98, 10048 means address already bound
+                return get_unused_port(None)
+            raise e
+        s.close()
+        return port
+
+
+def log_exception(file_path, msg):
+    msg = "\r\n" + msg
+    with open(file_path, "a") as error_log:
+        error_log.write(msg)
+
+
+def parse_exception(e, output=0):
+    tb = traceback.format_exc()
+    exc_type, exc_obj, exc_tb = sys.exc_info()
+    fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+    error = "%s %s %s %s %s" % (str(tb), str(exc_type), str(fname),
+                                str(exc_tb.tb_lineno), str(e))
+
+    if output:
+        print(error)
+
+    return str(error)
+
+
+def ip2int(addr):
+    return struct.unpack("!I", socket.inet_aton(addr))[0]
+
+
+def int2ip(addr):
+    return socket.inet_ntoa(struct.pack("!I", addr))
+
+# Patches for urllib2 and requests to bind on specific interface.
+# http://rossbates.com/2009/10/26/urllib2-with-multiple-network-interfaces/
+true_socket = socket.socket
+
+
+def build_bound_socket(source_ip):
+    def bound_socket(*a, **k):
+        if source_ip == "127.0.0.1":
+            raise Exception("This function requires a LAN IP"
+                            " (127.0.0.1 passed.)")
+
+        sock = true_socket(*a, **k)
+        sock.bind((source_ip, 0))
+        return sock
+
+    return bound_socket
+
+
+def busy_wait(dt):
+    # Use most accurate timer.
+    if platform.system() == "Windows":
+        timer = time.clock
+    else:
+        timer = time.time
+
+    current_time = timer()
+    while timer() < current_time + dt:
+        pass
+
+
+def get_ntp_worker(server):
+    try:
+        client = ntplib.NTPClient()
+        response = client.request(server, version=3)
+        ntp = response.tx_time
+        return ntp
+    except Exception as e:
+        return None
+
+ntp_servers = [
+    "pool.ntp.org",
+    "2.pool.ntp.org",
+    "0.pool.ntp.org",
+    "1.pool.ntp.org",
+    "3.pool.ntp.org"
+]
+
+bad_ntp_servers = None
+
+
+def remove_bad_ntp_servers():
+    global ntp_servers
+    global bad_ntp_servers
+
+    bad_ntp_servers = []
+    for server in ntp_servers:
+        ntp = get_ntp_worker(server)
+        if ntp is None:
+            bad_ntp_servers.append(server)
+
+    for server in bad_ntp_servers:
+        ntp_servers.remove(server)
+
+
+def get_ntp(local_time=0):
+    global ntp_servers
+    global bad_ntp_servers
+
+    if local_time:
+        return time.time()
+
+    if bad_ntp_servers is None:
+        remove_bad_ntp_servers()
+
+    random.shuffle(ntp_servers, random.random)
+    for server in ntp_servers:
+        ntp = get_ntp_worker(server)
+        if ntp is not None:
+            return ntp
+
+    return None
+
+
+def get_default_gateway(interface="default"):
+    if sys.version_info < (3, 0, 0):
+        if type(interface) == str:
+            interface = unicode(interface)
+    else:
+        if type(interface) == bytes:
+            interface = interface.decode("utf-8")
+
+    if platform.system() == "Windows":
+        if interface == "default":
+            default_routes = [r for r in get_ipv4_routing_table()
+                              if r[0] == '0.0.0.0']
+            if default_routes:
+                return default_routes[0][2]
+
+    try:
+        gws = netifaces.gateways()
+        if sys.version_info < (3, 0, 0):
+            return gws[interface][netifaces.AF_INET][0].decode("utf-8")
+        else:
+            return gws[interface][netifaces.AF_INET][0]
+    except:
+        # This can also mean the machine is directly accessible.
+        return None
+
+
+def get_lan_ip(interface="default"):
+    if sys.version_info < (3, 0, 0):
+        if type(interface) == str:
+            interface = unicode(interface)
+    else:
+        if type(interface) == bytes:
+            interface = interface.decode("utf-8")
+
+    # Get ID of interface that handles WAN stuff.
+    default_gateway = get_default_gateway(interface)
+    gateways = netifaces.gateways()
+    wan_id = None
+    if netifaces.AF_INET in gateways:
+        gw_list = gateways[netifaces.AF_INET]
+        for gw_info in gw_list:
+            if gw_info[0] == default_gateway:
+                wan_id = gw_info[1]
+                break
+
+    # Find LAN IP of interface for WAN stuff.
+    interfaces = netifaces.interfaces()
+    if wan_id in interfaces:
+        families = netifaces.ifaddresses(wan_id)
+        if netifaces.AF_INET in families:
+            if_info_list = families[netifaces.AF_INET]
+            for if_info in if_info_list:
+                if "addr" in if_info:
+                    return if_info["addr"]
+
+    """
+    Execution may reach here if the host is using
+    virtual interfaces on Linux and there are no gateways
+    which suggests the host is a VPS or server. In this
+    case
+    """
+    if platform.system() == "Linux":
+        if ip is not None:
+            return ip.routes["8.8.8.8"]["prefsrc"]
+
+    return None
+
+
+def sequential_bind(n, interface="default"):
+    # Get bind address.
+    addr = ''
+    if interface != "default":
+        addr = get_lan_ip(interface)
+
+    # Start the process.
+    bound = 0
+    mappings = []
+    prospects = []
+    while not bound:
+        # Grab a random place to start.
+        bound = 1
+        start = random.randrange(1024, 65535 - n)
+
+        # Use connect to see if its already bound.
+        for i in range(0, n):
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            local = start + i
+            try:
+                sock.connect((addr, local))
+                sock.close()
+                bound = 0
+                break
+            except socket.error:
+                pass
+
+            prospect = {
+                "local": local,
+            }
+            prospects.append(prospect)
+
+        for prospect in prospects:
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            try:
+                sock.bind((addr, prospect["local"]))
+            except Exception as e:
+                bound = 0
+                for mapping in mappings:
+                    mapping["sock"].close()
+                mappings = []
+                break
+
+            mapping = {
+                "source": prospect["local"],
+                "sock": sock
+            }
+            mappings.append(mapping)
+
+    return mappings
+
+
+def is_port_forwarded(source_ip, port, proto, forwarding_servers):
+    global true_socket
+    if source_ip is not None:
+        socket.socket = build_bound_socket(source_ip)
+
+    ret = 0
+    for forwarding_server in forwarding_servers:
+        url = "http://" + forwarding_server["addr"] + ":"
+        url += str(forwarding_server["port"])
+        url += forwarding_server["url"]
+        url += "?action=is_port_forwarded&port=" + str(port)
+        url += "&proto=" + str(proto.upper())
+
+        try:
+            r = urlopen(url, timeout=2)
+            response = r.read().decode("utf-8")
+            if "yes" in response:
+                ret = 1
+                break
+        except:
+            continue
+
+    socket.socket = true_socket
+    return ret
+
+
+def is_ip_private(ip_addr):
+    if sys.version_info < (3, 0, 0):
+        if type(ip_addr) == str:
+            ip_addr = unicode(ip_addr)
+    else:
+        if type(ip_addr) == bytes:
+            ip_addr = ip_addr.decode("utf-8")
+
+    if ipaddress.ip_address(ip_addr).is_private and ip_addr != "127.0.0.1":
+        return 1
+    else:
+        return 0
+
+
+def is_ip_public(ip_addr):
+    if sys.version_info < (3, 0, 0):
+        if type(ip_addr) == str:
+            ip_addr = unicode(ip_addr)
+    else:
+        if type(ip_addr) == bytes:
+            ip_addr = ip_addr.decode("utf-8")
+
+    if is_ip_private(ip_addr):
+        return 0
+    elif ip_addr == "127.0.0.1":
+        return 0
+    else:
+        return 1
+
+
+def is_ip_valid(ip_addr):
+    if sys.version_info < (3, 0, 0):
+        if type(ip_addr) == str:
+            ip_addr = unicode(ip_addr)
+    else:
+        if type(ip_addr) == bytes:
+            ip_addr = ip_addr.decode("utf-8")
+
+    try:
+        ipaddress.ip_address(ip_addr)
+        return 1
+    except:
+        return 0
+
+
+def is_valid_port(port):
+    try:
+        port = int(port)
+    except:
+        return 0
+    if port < 1 or port > 65535:
+        return 0
+    else:
+        return 1
+
+
+def memoize(function):
+    memo = {}
+
+    def wrapper(*args):
+        if args in memo:
+            return memo[args]
+        else:
+            rv = function(*args)
+            memo[args] = rv
+            return rv
+    return wrapper
+
+
+def extract_ip(s):
+    ip = re.findall("[0-9]+[.][0-9]+[.][0-9]+[.][0-9]+", s)
+    if len(ip):
+        return ip[0]
+
+    return ""
+
+
+@memoize
+def get_wan_ip(n=0):
+    """
+    That IP module sucks. Occasionally it returns an IP address behind
+    cloudflare which probably happens when cloudflare tries to proxy your web
+    request because it thinks you're trying to DoS. It's better if we just run
+    our own infrastructure.
+    """
+
+    if n == 2:
+        try:
+            ip = myip()
+            ip = extract_ip(ip)
+            if is_ip_valid(ip):
+                return ip
+        except Exception as e:
+            print(str(e))
+            return None
+
+    # Fail-safe: use centralized server for IP lookup.
+    from pyp2p.net import forwarding_servers
+    for forwarding_server in forwarding_servers:
+        url = "http://" + forwarding_server["addr"] + ":"
+        url += str(forwarding_server["port"])
+        url += forwarding_server["url"]
+        url += "?action=get_wan_ip"
+        try:
+            r = urlopen(url, timeout=5)
+            response = r.read().decode("utf-8")
+            response = extract_ip(response)
+            if is_ip_valid(response):
+                return response
+        except Exception as e:
+            print(str(e))
+            continue
+
+    time.sleep(1)
+    return get_wan_ip(n + 1)
+
+
+def request_priority_execution():
+    gc.disable()
+    sys.setcheckinterval(999999999)
+    if sys.version_info > (3, 0, 0):
+        sys.setswitchinterval(1000)
+    p = psutil.Process(os.getpid())
+    try:
+        if platform.system() == "Windows":
+            p.nice(psutil.HIGH_PRIORITY_CLASS)
+        else:
+            p.nice(10)
+    except psutil.AccessDenied:
+        pass
+
+    return p
+
+
+def release_priority_execution(p):
+    sys.setcheckinterval(100)
+    if sys.version_info > (3, 0, 0):
+        sys.setswitchinterval(0.005)
+    try:
+        if platform.system() == "Windows":
+            p.nice(psutil.NORMAL_PRIORITY_CLASS)
+        else:
+            p.nice(5)
+    except psutil.AccessDenied:
+        pass
+    gc.enable()
+
+
+def encode_str(s, encoding="unicode"):
+    # Encode unsafe binary to unicode
+    # Encode unsafe unicode to binary
+    if sys.version_info >= (3, 0, 0):
+        # str in Python 3+ is unicode.
+        if type(s) == str:
+            if encoding == "ascii":
+                # Encodes unicode directly as bytes.
+                codes = []
+                for ch in s:
+                    codes.append(ord(ch))
+
+                if len(codes):
+                    return bytes(codes)
+                else:
+                    return b""
+        else:
+            # bytes
+            if encoding == "unicode":
+                # Converts bytes to unicode.
+                return s.decode("utf-8")
+    else:
+        # unicode in python 2 is unicode.
+        if type(s) == unicode:
+            # Encodes unicode directly as bytes.
+            if encoding == "ascii":
+                byte_str = b""
+                for ch in s:
+                    byte_str += chr(ord(ch))
+
+                return byte_str
+        else:
+            # bytes.
+            if encoding == "unicode":
+                # Converts bytes to unicode.
+                return s.decode("utf-8")
+
+    if type(s) == type(u""):
+        s = s.encode("utf-8")
+
+    return s
+
+if __name__ == "__main__":
+    # print(get_wan_ip())
+    # pass
+    print("In lib")
+
```

### Comparing `pyp2p-0.8.2/pyp2p/rendezvous_client.py` & `pyp2p-0.8.3/pyp2p/rendezvous_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -689,15 +689,15 @@
             # source port specified
             servers = servers or self.rendezvous_servers
             con = None
             while con is None:
                 try:
                     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                     sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-                    port = port or get_unused_port()
+                    port = port or get_unused_port(None)
                     sock.bind(('', port))
                     source_port = sock.getsockname()[1]
                     index = random.randrange(0, len(servers))
                     log.debug("Trying index: " + str(index))
                     con = self.server_connect(sock, index, servers)
                 except:
                     time.sleep(1)
```

### Comparing `pyp2p-0.8.2/pyp2p/unl.py` & `pyp2p-0.8.3/pyp2p/unl.py`

 * *Files identical despite different names*

### Comparing `pyp2p-0.8.2/setup.py` & `pyp2p-0.8.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='0.8.2',
+    version='0.8.3',
     name='pyp2p',
     description='Python P2P networking library',
-    keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP,'
-              ' NATPMP, P2P, Peer-to-peer networking library, python'),
+    keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP, NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description=long_description,
     url='http://github.com/Storj/pyp2p',
     author='Storj',
     author_email='matthew@storj.io',
     test_suite="tests",
     license='MIT',
     packages=find_packages(exclude=('tests', 'docs')),
```

### Comparing `pyp2p-0.8.2/README.rst` & `pyp2p-0.8.3/pyp2p.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,157 +1,175 @@
-################
-Welcome to PyP2P
-################
-
-|BuildLink|_ |CoverageLink|_ |BuildLink2|_ |CoverageLink2|_ |LicenseLink|_
-
-.. |BuildLink| image:: https://img.shields.io/travis/Storj/pyp2p/master.svg?label=Build-Master
-.. _BuildLink: https://travis-ci.org/Storj/pyp2p
-
-.. |CoverageLink| image:: https://img.shields.io/coveralls/Storj/pyp2p/master.svg?label=Coverage-Master
-.. _CoverageLink: https://coveralls.io/r/Storj/pyp2p
-
-.. |BuildLink2| image:: https://img.shields.io/travis/Storj/pyp2p/develop.svg?label=Build-Develop
-.. _BuildLink2: https://travis-ci.org/Storj/pyp2p
-
-.. |CoverageLink2| image:: https://img.shields.io/coveralls/Storj/pyp2p/develop.svg?label=Coverage-Develop
-.. _CoverageLink2: https://coveralls.io/r/Storj/pyp2p
-
-.. |LicenseLink| image:: https://img.shields.io/badge/license-MIT-blue.svg
-.. _LicenseLink: https://raw.githubusercontent.com/Storj/pyp2p
-
-PyP2P is a simplified networking library for building peer-to-peer networks in Python. The library is designed to solve the pain of finding nodes and bypassing NATs so you can focus on writing your application code.
-
-* Automated port forwarding with UPnP and NATPMP
-* Support for TCP hole punching / simultaneous open
-* Reverse connect (tell a node to connect to you)
-* Fail-safe proxying (planned feature)
-* Python 2 (tested on 2.7 - experimental) & 3 (tested on 3.3)
-* Linux and Windows - yep
-
-============
-Code example
-============
-PyP2P is designed to work with simple non-blocking TCP sockets. To use them, your application must create an infinite loop which is used to periodically look for new replies. As you look for replies, the software also handles accepting new connections and removing old ones automatically.
-
-The library also handles constructing replies, which are returned in full as a simple list. The underlying message format is a simple line-based protocol: the messages you want to send are terminated with a new line and are returned in full when they've arrived which makes debugging and developing p2p protocols very simple (text-based protocols are easy to debug.)
-
-==========
-Alice node
-==========
-This will create a new listening server on port 44444, bound to listen for connections from the LAN. The interface is specified mostly to ensure that connections are only made from that interface. By default, connections will be made from the default interface (usually wlan0 or eth0) which isn't useful for simulating and testing a P2P network on the same computer.
-
-.. code:: python
-
-    from pyp2p.net import *
-    import time
-
-    #Setup Alice's p2p node.
-    alice = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", node_type="passive", debug=1)
-    alice.start()
-    alice.bootstrap()
-    alice.advertise()
-
-    #Event loop.
-    while 1:
-        for con in alice:
-            for reply in con:
-                print(reply)
-
-        time.sleep(1)
-
-========
-Bob node
-========
-This code will make a connection to the Alice node and repeatedly send her the word test. Note how they're both on different interfaces, with completely different IPs. This is necessary for connecting to nodes on the same computer as the library doesn't allow the Net class to connect to itself itself when running in P2P mode (type="p2p" for the Net class.) If you want to be able to make duplicate connections to nodes on the same interface then specify the type as "direct" which will make testing code easier. Note that type is "p2p" by default.
-
-.. code:: python
-
-    from pyp2p.net import *
-
-    #Setup Bob's p2p node.
-    bob = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", node_type="passive", debug=1)
-    bob.start()
-    bob.bootstrap()
-    bob.advertise()
-
-    #Event loop.
-    while 1:
-        for con in bob:
-            con.send_line("test")
-
-        time.sleep(1)
-
-==============
-Direct connect
-==============
-The code shown so far is good for standard broadcast / flooding style P2P networks where the only requirement is to get a message out to the whole network (e.g. Bitcoin and Bitmessage) - but if you want to do anything more complicated you're going to need to be able to communicate with nodes directly.
-
-Theoretically you can specify the recipient of a message and broadcast it to the network to reach them but this approach won't scale well for most people. What is needed is a way to direct connect to a node with a high level of reliability. To support this function we use something called a UNL: short for Universal Node Locator.
-
-UNLs describe how to connect to a node behind a NAT, firewall, or on the same LAN by looking at the nodes network information in relation to other nodes and using a variety of subversive techniques including UPnP, NATPMP, and TCP hole punching. To further increase the reliability of this code: the software can also be used with a patched instance of the Kademlia DHT to accept direct messages from other nodes on the DHT that instruct it where to connect back to. This is extremely useful for connecting to nodes behind a NAT as it completely bypasses the need for port forwarding assuming that the source is accessible.
-
-.. code:: python
-
-    from pyp2p.net import *
-    from pyp2p.unl import UNL
-    from pyp2p.dht_msg import DHT
-    import time
-
-
-    #Start Alice's direct server.
-    alice_dht = DHT()
-    alice_direct = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", net_type="direct", dht_node=alice_dht, debug=1)
-    alice_direct.start()
-
-    #Start Bob's direct server.
-    bob_dht = DHT()
-    bob_direct = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", net_type="direct", node_type="active", dht_node=bob_dht, debug=1)
-    bob_direct.start()
-
-    #Callbacks.
-    def success(con):
-        print("Alice successfully connected to Bob.")
-        con.send_line("Sup Bob.")
-
-    def failure(con):
-    print("Alice failed to connec to Bob\a")
-
-    events = {
-        "success": success,
-        "failure": failure
-    }
-
-    #Have Alice connect to Bob.
-    alice_direct.unl.connect(bob_direct.unl.construct(), events)
-
-    #Event loop.
-    while 1:
-    #Bob get reply.
-    for con in bob_direct:
-        for reply in con:
-            print(reply)
-
-    #Alice accept con.
-    for con in alice_direct:
-        x = 1
-
-    time.sleep(0.5)
-
-
-In the previous code the Net class was used to spawn a server to accept connections from nodes on the p2p network and managing connections for the purpose of broadcasting. To manage direct connections the same class is used, the difference is the class disables bootstrapping and advertising the connection details to the bootstrapping server as this service is reserved specifically for receiving direct connections.
-
-============
-Dependencies
-============
-* netifaces
-* ntplib
-* twisted
-* ipaddress
-* requests
-* nose
-* setuptools
-* pyroute2
-
-Installation: python3.3 setup.py install
-
-Status: Experimental, may have bugs
+Metadata-Version: 2.1
+Name: pyp2p
+Version: 0.8.3
+Summary: Python P2P networking library
+Home-page: http://github.com/Storj/pyp2p
+Author: Storj
+Author-email: matthew@storj.io
+License: MIT
+Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,NATPMP,P2P,Peer-to-peer networking library,python
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+License-File: LICENSE
+
+**This library is depricated. See https://github.com/robertsdotpm/p2pd for the new version**
+#############################################################################################
+
+Welcome to PyP2P |BuildLink|_ |CoverageLink|_ |BuildLink2|_ |CoverageLink2|_ |LicenseLink|_
+
+.. |BuildLink| image:: https://img.shields.io/travis/Storj/pyp2p/master.svg?label=Build-Master
+.. _BuildLink: https://travis-ci.org/Storj/pyp2p
+
+.. |CoverageLink| image:: https://img.shields.io/coveralls/Storj/pyp2p/master.svg?label=Coverage-Master
+.. _CoverageLink: https://coveralls.io/r/Storj/pyp2p
+
+.. |BuildLink2| image:: https://img.shields.io/travis/Storj/pyp2p/develop.svg?label=Build-Develop
+.. _BuildLink2: https://travis-ci.org/Storj/pyp2p
+
+.. |CoverageLink2| image:: https://img.shields.io/coveralls/Storj/pyp2p/develop.svg?label=Coverage-Develop
+.. _CoverageLink2: https://coveralls.io/r/Storj/pyp2p
+
+.. |LicenseLink| image:: https://img.shields.io/badge/license-MIT-blue.svg
+.. _LicenseLink: https://raw.githubusercontent.com/Storj/pyp2p
+
+PyP2P is a simplified networking library for building peer-to-peer networks in Python. The library is designed to solve the pain of finding nodes and bypassing NATs so you can focus on writing your application code.
+
+* Automated port forwarding with UPnP and NATPMP
+* Support for TCP hole punching / simultaneous open
+* Reverse connect (tell a node to connect to you)
+* Fail-safe proxying (planned feature)
+* Python 2 (tested on 2.7 - experimental) & 3 (tested on 3.3)
+* Linux and Windows - yep
+
+============
+Code example
+============
+PyP2P is designed to work with simple non-blocking TCP sockets. To use them, your application must create an infinite loop which is used to periodically look for new replies. As you look for replies, the software also handles accepting new connections and removing old ones automatically.
+
+The library also handles constructing replies, which are returned in full as a simple list. The underlying message format is a simple line-based protocol: the messages you want to send are terminated with a new line and are returned in full when they've arrived which makes debugging and developing p2p protocols very simple (text-based protocols are easy to debug.)
+
+==========
+Alice node
+==========
+This will create a new listening server on port 44444, bound to listen for connections from the LAN. The interface is specified mostly to ensure that connections are only made from that interface. By default, connections will be made from the default interface (usually wlan0 or eth0) which isn't useful for simulating and testing a P2P network on the same computer.
+
+.. code:: python
+
+    from pyp2p.net import *
+    import time
+
+    #Setup Alice's p2p node.
+    alice = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", node_type="passive", debug=1)
+    alice.start()
+    alice.bootstrap()
+    alice.advertise()
+
+    #Event loop.
+    while 1:
+        for con in alice:
+            for reply in con:
+                print(reply)
+
+        time.sleep(1)
+
+========
+Bob node
+========
+This code will make a connection to the Alice node and repeatedly send her the word test. Note how they're both on different interfaces, with completely different IPs. This is necessary for connecting to nodes on the same computer as the library doesn't allow the Net class to connect to itself itself when running in P2P mode (type="p2p" for the Net class.) If you want to be able to make duplicate connections to nodes on the same interface then specify the type as "direct" which will make testing code easier. Note that type is "p2p" by default.
+
+.. code:: python
+
+    from pyp2p.net import *
+
+    #Setup Bob's p2p node.
+    bob = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", node_type="passive", debug=1)
+    bob.start()
+    bob.bootstrap()
+    bob.advertise()
+
+    #Event loop.
+    while 1:
+        for con in bob:
+            con.send_line("test")
+
+        time.sleep(1)
+
+==============
+Direct connect
+==============
+The code shown so far is good for standard broadcast / flooding style P2P networks where the only requirement is to get a message out to the whole network (e.g. Bitcoin and Bitmessage) - but if you want to do anything more complicated you're going to need to be able to communicate with nodes directly.
+
+Theoretically you can specify the recipient of a message and broadcast it to the network to reach them but this approach won't scale well for most people. What is needed is a way to direct connect to a node with a high level of reliability. To support this function we use something called a UNL: short for Universal Node Locator.
+
+UNLs describe how to connect to a node behind a NAT, firewall, or on the same LAN by looking at the nodes network information in relation to other nodes and using a variety of subversive techniques including UPnP, NATPMP, and TCP hole punching. To further increase the reliability of this code: the software can also be used with a patched instance of the Kademlia DHT to accept direct messages from other nodes on the DHT that instruct it where to connect back to. This is extremely useful for connecting to nodes behind a NAT as it completely bypasses the need for port forwarding assuming that the source is accessible.
+
+.. code:: python
+
+    from pyp2p.net import *
+    from pyp2p.unl import UNL
+    from pyp2p.dht_msg import DHT
+    import time
+
+
+    #Start Alice's direct server.
+    alice_dht = DHT()
+    alice_direct = Net(passive_bind="192.168.0.45", passive_port=44444, interface="eth0:2", net_type="direct", dht_node=alice_dht, debug=1)
+    alice_direct.start()
+
+    #Start Bob's direct server.
+    bob_dht = DHT()
+    bob_direct = Net(passive_bind="192.168.0.44", passive_port=44445, interface="eth0:1", net_type="direct", node_type="active", dht_node=bob_dht, debug=1)
+    bob_direct.start()
+
+    #Callbacks.
+    def success(con):
+        print("Alice successfully connected to Bob.")
+        con.send_line("Sup Bob.")
+
+    def failure(con):
+    print("Alice failed to connec to Bob\a")
+
+    events = {
+        "success": success,
+        "failure": failure
+    }
+
+    #Have Alice connect to Bob.
+    alice_direct.unl.connect(bob_direct.unl.construct(), events)
+
+    #Event loop.
+    while 1:
+    #Bob get reply.
+    for con in bob_direct:
+        for reply in con:
+            print(reply)
+
+    #Alice accept con.
+    for con in alice_direct:
+        x = 1
+
+    time.sleep(0.5)
+
+
+In the previous code the Net class was used to spawn a server to accept connections from nodes on the p2p network and managing connections for the purpose of broadcasting. To manage direct connections the same class is used, the difference is the class disables bootstrapping and advertising the connection details to the bootstrapping server as this service is reserved specifically for receiving direct connections.
+
+============
+Dependencies
+============
+* netifaces
+* ntplib
+* twisted
+* ipaddress
+* requests
+* nose
+* setuptools
+* pyroute2
+
+Installation: python3.3 setup.py install
+
+Status: Experimental, may have bugs
```

