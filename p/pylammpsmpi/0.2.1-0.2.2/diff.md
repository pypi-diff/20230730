# Comparing `tmp/pylammpsmpi-0.2.1.tar.gz` & `tmp/pylammpsmpi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylammpsmpi-0.2.1.tar", last modified: Mon Jul 24 23:50:23 2023, max compression
+gzip compressed data, was "pylammpsmpi-0.2.2.tar", last modified: Sun Jul 30 19:09:54 2023, max compression
```

## Comparing `pylammpsmpi-0.2.1.tar` & `pylammpsmpi-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/pylammpsmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/pylammpsmpi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.129724 pylammpsmpi-0.2.1/pylammpsmpi/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/mpi/lmpmpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.129724 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/extended.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.129724 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 23:50:22.000000 pylammpsmpi-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_ase_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_pylammpsmpi_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/pylammpsmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/pylammpsmpi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/pylammpsmpi/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/mpi/lmpmpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/pylammpsmpi/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/wrapper/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/wrapper/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/pylammpsmpi/wrapper/extended.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/pylammpsmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-30 19:09:54.000000 pylammpsmpi-0.2.2/pylammpsmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-30 19:09:54.000000 pylammpsmpi-0.2.2/pylammpsmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:09:54.000000 pylammpsmpi-0.2.2/pylammpsmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 19:09:54.000000 pylammpsmpi-0.2.2/pylammpsmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 19:09:54.000000 pylammpsmpi-0.2.2/pylammpsmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-30 19:09:54.000000 pylammpsmpi-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:09:54.567116 pylammpsmpi-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/tests/test_ase_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/tests/test_pylammpsmpi_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-30 19:09:48.000000 pylammpsmpi-0.2.2/versioneer.py
```

### Comparing `pylammpsmpi-0.2.1/LICENSE` & `pylammpsmpi-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/PKG-INFO` & `pylammpsmpi-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.2.1/README.md` & `pylammpsmpi-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/pylammpsmpi/mpi/lmpmpi.py` & `pylammpsmpi-0.2.2/pylammpsmpi/mpi/lmpmpi.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from ctypes import c_double, c_int
 from mpi4py import MPI
 import numpy as np
 import sys
 from lammps import lammps
 from pympipool import (
-    connect_to_socket_interface,
-    send_result,
-    close_connection,
-    receive_instruction,
+    interface_connect,
+    interface_send,
+    interface_shutdown,
+    interface_receive,
 )
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -459,42 +459,45 @@
         for vl in data_gather:
             for v in vl:
                 data.append(v)
         return data
 
 
 def _run_lammps_mpi(argument_lst):
+    index_selected = argument_lst.index("--zmqport")
+    port_selected = argument_lst[index_selected + 1]
+    if "--host" in argument_lst:
+        index_selected = argument_lst.index("--host")
+        host = argument_lst[index_selected + 1]
+    else:
+        host = "localhost"
+    argument_red_lst = argument_lst[:index_selected]
     if MPI.COMM_WORLD.rank == 0:
-        port_selected = argument_lst[argument_lst.index("--zmqport") + 1]
-        if "--host" in argument_lst:
-            host = argument_lst[argument_lst.index("--host") + 1]
-        else:
-            host = "localhost"
-        context, socket = connect_to_socket_interface(host=host, port=port_selected)
+        context, socket = interface_connect(host=host, port=port_selected)
     else:
         context, socket = None, None
     # Lammps executable
     args = ["-screen", "none"]
-    if len(argument_lst) > 3:
-        args.extend(argument_lst[3:])
+    if len(argument_red_lst) > 1:
+        args.extend(argument_red_lst[1:])
     job = lammps(cmdargs=args)
     while True:
         if MPI.COMM_WORLD.rank == 0:
-            input_dict = receive_instruction(socket=socket)
+            input_dict = interface_receive(socket=socket)
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
         if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
             job.close()
             if MPI.COMM_WORLD.rank == 0:
-                send_result(socket=socket, result_dict={"result": True})
-                close_connection(socket=socket, context=context)
+                interface_send(socket=socket, result_dict={"result": True})
+                interface_shutdown(socket=socket, context=context)
             break
         output = select_cmd(input_dict["command"])(
             job=job, funct_args=input_dict["args"]
         )
         if MPI.COMM_WORLD.rank == 0 and output is not None:
-            send_result(socket=socket, result_dict={"result": output})
+            interface_send(socket=socket, result_dict={"result": output})
 
 
 if __name__ == "__main__":
     _run_lammps_mpi(argument_lst=sys.argv)
```

### Comparing `pylammpsmpi-0.2.1/pylammpsmpi/wrapper/ase.py` & `pylammpsmpi-0.2.2/pylammpsmpi/wrapper/ase.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/pylammpsmpi/wrapper/base.py` & `pylammpsmpi-0.2.2/pylammpsmpi/wrapper/base.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/pylammpsmpi/wrapper/concurrent.py` & `pylammpsmpi-0.2.2/pylammpsmpi/wrapper/concurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,80 +2,58 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import os
 import socket
 from concurrent.futures import Future
 from queue import Queue
-from pympipool import RaisingThread, SocketInterface, cancel_items_in_queue
+from pympipool import RaisingThread, cancel_items_in_queue, interface_bootup
 
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Feb 28, 2020"
 
 
-def _initialize_socket(
-    interface, cmdargs, cwd, cores, oversubscribe=False, enable_flux_backend=False
-):
-    port_selected = interface.bind_to_random_port()
-    executable = os.path.join(
-        os.path.dirname(os.path.abspath(__file__)), "../mpi", "lmpmpi.py"
-    )
-    if enable_flux_backend:
-        cmds = ["flux", "run"]
-    else:
-        cmds = ["mpiexec"]
-    if oversubscribe:
-        cmds += ["--oversubscribe"]
-    cmds += [
-        "-n",
-        str(cores),
-        "python",
-        executable,
-        "--zmqport",
-        str(port_selected),
-    ]
-    if enable_flux_backend:
-        cmds += [
-            "--host",
-            socket.gethostname(),
-        ]
-    if cmdargs is not None:
-        cmds.extend(cmdargs)
-    interface.bootup(command_lst=cmds, cwd=cwd)
-    return interface
-
-
 def execute_async(
     future_queue,
-    cmdargs,
-    cores,
+    cmdargs=None,
+    cores=1,
     oversubscribe=False,
     enable_flux_backend=False,
+    enable_slurm_backend=False,
     cwd=None,
     queue_adapter=None,
     queue_adapter_kwargs=None,
 ):
-    interface = _initialize_socket(
-        interface=SocketInterface(
-            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
-        ),
-        cmdargs=cmdargs,
+    executable = os.path.join(
+        os.path.dirname(os.path.abspath(__file__)), "../mpi", "lmpmpi.py"
+    )
+    if cmdargs is not None:
+        command_lst = ["python", executable] + cmdargs
+    else:
+        command_lst = ["python", executable]
+    interface = interface_bootup(
+        command_lst=command_lst,
         cwd=cwd,
         cores=cores,
-        enable_flux_backend=enable_flux_backend,
+        gpus_per_core=0,
         oversubscribe=oversubscribe,
+        enable_flux_backend=enable_flux_backend,
+        enable_slurm_backend=enable_slurm_backend,
+        queue_adapter=queue_adapter,
+        queue_type=None,
+        queue_adapter_kwargs=queue_adapter_kwargs,
     )
     while True:
         task_dict = future_queue.get()
         if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
             interface.shutdown(wait=task_dict["wait"])
             break
         elif "command" in task_dict.keys() and "future" in task_dict.keys():
@@ -86,39 +64,42 @@
 
 class LammpsConcurrent:
     def __init__(
         self,
         cores=8,
         oversubscribe=False,
         enable_flux_backend=False,
+        enable_slurm_backend=False,
         working_directory=".",
         cmdargs=None,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
         self.cores = cores
         self.working_directory = working_directory
         self._future_queue = Queue()
         self._process = None
         self._oversubscribe = oversubscribe
         self._enable_flux_backend = enable_flux_backend
+        self._enable_slurm_backend = enable_slurm_backend
         self._cmdargs = cmdargs
         self._queue_adapter = queue_adapter
         self._queue_adapter_kwargs = queue_adapter_kwargs
         self._start_process()
 
     def _start_process(self):
         self._process = RaisingThread(
             target=execute_async,
             kwargs={
                 "future_queue": self._future_queue,
                 "cmdargs": self._cmdargs,
                 "cores": self.cores,
                 "oversubscribe": self._oversubscribe,
                 "enable_flux_backend": self._enable_flux_backend,
+                "enable_slurm_backend": self._enable_slurm_backend,
                 "cwd": self.working_directory,
                 "queue_adapter": self._queue_adapter,
                 "queue_adapter_kwargs": self._queue_adapter_kwargs,
             },
         )
         self._process.start()
```

### Comparing `pylammpsmpi-0.2.1/pylammpsmpi/wrapper/extended.py` & `pylammpsmpi-0.2.2/pylammpsmpi/wrapper/extended.py`

 * *Files 3% similar despite different names*

```diff
@@ -241,31 +241,34 @@
     """
 
     def __init__(
         self,
         cores=1,
         oversubscribe=False,
         enable_flux_backend=False,
+        enable_slurm_backend=False,
         working_directory=".",
         client=None,
         mode="local",
         cmdargs=None,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
         self.cores = cores
         self.working_directory = working_directory
         self.oversubscribe = oversubscribe
         self.enable_flux_backend = enable_flux_backend
+        self.enable_slurm_backend = enable_slurm_backend
         self.client = client
         self.mode = mode
         self.lmp = LammpsConcurrent(
             cores=self.cores,
             oversubscribe=self.oversubscribe,
             enable_flux_backend=self.enable_flux_backend,
+            enable_slurm_backend=self.enable_slurm_backend,
             working_directory=self.working_directory,
             cmdargs=cmdargs,
             queue_adapter=queue_adapter,
             queue_adapter_kwargs=queue_adapter_kwargs,
         )
 
     def __getattr__(self, name):
```

### Comparing `pylammpsmpi-0.2.1/pylammpsmpi.egg-info/PKG-INFO` & `pylammpsmpi-0.2.2/pylammpsmpi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.2.1/pylammpsmpi.egg-info/SOURCES.txt` & `pylammpsmpi-0.2.2/pylammpsmpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/setup.py` & `pylammpsmpi-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
          'Programming Language :: Python :: 3.10',
          'Programming Language :: Python :: 3.11',
     ],
 
     keywords='lammps, mpi4py',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        "mpi4py>=3.1.4", "pympipool>=0.5.6", "numpy>=1.23.5"
+        "mpi4py>=3.1.4", "pympipool>=0.6.0", "numpy>=1.23.5"
     ],
     extras_require={
         "ase": ["ase>=3.22.1", "scipy>=1.10.1"],
     },
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `pylammpsmpi-0.2.1/tests/test_ase_constraints.py` & `pylammpsmpi-0.2.2/tests/test_ase_constraints.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/tests/test_base.py` & `pylammpsmpi-0.2.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/tests/test_concurrent.py` & `pylammpsmpi-0.2.2/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/tests/test_pylammpsmpi_local.py` & `pylammpsmpi-0.2.2/tests/test_pylammpsmpi_local.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.1/versioneer.py` & `pylammpsmpi-0.2.2/versioneer.py`

 * *Files identical despite different names*

