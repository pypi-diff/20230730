# Comparing `tmp/pylogbeat-2.0.0.tar.gz` & `tmp/pylogbeat-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylogbeat-2.0.0.tar", last modified: Sun Oct  4 16:44:20 2020, max compression
+gzip compressed data, was "pylogbeat-2.0.1.tar", last modified: Sun Jul 30 14:27:42 2023, max compression
```

## Comparing `pylogbeat-2.0.0.tar` & `pylogbeat-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2020-10-04 16:44:20.026221 pylogbeat-2.0.0/
--rw-r--r--   0 enrico    (1000) enrico    (1000)    11345 2018-11-16 13:01:43.000000 pylogbeat-2.0.0/LICENSE
--rw-r--r--   0 enrico    (1000) enrico    (1000)       34 2018-12-27 22:16:09.000000 pylogbeat-2.0.0/MANIFEST.in
--rw-r--r--   0 enrico    (1000) enrico    (1000)     9169 2020-10-04 16:44:20.026221 pylogbeat-2.0.0/PKG-INFO
--rw-r--r--   0 enrico    (1000) enrico    (1000)     6308 2020-10-04 16:43:56.000000 pylogbeat-2.0.0/README.md
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2020-10-04 16:44:20.026221 pylogbeat-2.0.0/pylogbeat.egg-info/
--rw-r--r--   0 enrico    (1000) enrico    (1000)     9169 2020-10-04 16:44:19.000000 pylogbeat-2.0.0/pylogbeat.egg-info/PKG-INFO
--rw-r--r--   0 enrico    (1000) enrico    (1000)      193 2020-10-04 16:44:19.000000 pylogbeat-2.0.0/pylogbeat.egg-info/SOURCES.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2020-10-04 16:44:19.000000 pylogbeat-2.0.0/pylogbeat.egg-info/dependency_links.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)       10 2020-10-04 16:44:19.000000 pylogbeat-2.0.0/pylogbeat.egg-info/top_level.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)     8812 2020-10-04 16:39:44.000000 pylogbeat-2.0.0/pylogbeat.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1225 2020-10-04 16:44:20.029555 pylogbeat-2.0.0/setup.cfg
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1765 2020-10-04 16:43:56.000000 pylogbeat-2.0.0/setup.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-07-30 14:27:42.217484 pylogbeat-2.0.1/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)    11345 2018-11-16 13:01:43.000000 pylogbeat-2.0.1/LICENSE
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       34 2018-12-27 22:16:09.000000 pylogbeat-2.0.1/MANIFEST.in
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     7424 2023-07-30 14:27:42.217484 pylogbeat-2.0.1/PKG-INFO
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     6436 2023-07-30 14:26:26.000000 pylogbeat-2.0.1/README.md
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-07-30 14:27:42.217484 pylogbeat-2.0.1/pylogbeat.egg-info/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     7424 2023-07-30 14:27:42.000000 pylogbeat-2.0.1/pylogbeat.egg-info/PKG-INFO
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      193 2023-07-30 14:27:42.000000 pylogbeat-2.0.1/pylogbeat.egg-info/SOURCES.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-07-30 14:27:42.000000 pylogbeat-2.0.1/pylogbeat.egg-info/dependency_links.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       10 2023-07-30 14:27:42.000000 pylogbeat-2.0.1/pylogbeat.egg-info/top_level.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     8671 2023-07-30 14:25:18.000000 pylogbeat-2.0.1/pylogbeat.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1194 2023-07-30 14:27:42.217484 pylogbeat-2.0.1/setup.cfg
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1765 2023-07-30 14:25:25.000000 pylogbeat-2.0.1/setup.py
```

### Comparing `pylogbeat-2.0.0/LICENSE` & `pylogbeat-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogbeat-2.0.0/README.md` & `pylogbeat-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 PyLogBeat
 =========
 
-[![Travis CI](https://travis-ci.org/eht16/pylogbeat.svg?branch=master)](https://travis-ci.org/eht16/pylogbeat)
+[![CI Tests](https://github.com/eht16/pylogbeat/actions/workflows/tests.yml/badge.svg)](https://github.com/eht16/pylogbeat/actions/workflows/tests.yml)
 [![PyPI](https://img.shields.io/pypi/v/pylogbeat.svg)](https://pypi.org/project/pylogbeat/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pylogbeat.svg)](https://pypi.org/project/pylogbeat/)
 [![License](https://img.shields.io/pypi/l/pylogbeat.svg)](https://pypi.org/project/pylogbeat/)
 
 PyLogBeat is a simple, incomplete implementation of the Beats protocol
 used by Elastic Beats and Logstash. For more information about Beats see
 https://www.elastic.co/products/beats and
@@ -178,14 +178,19 @@
 adopted to support version 2 of the protocol.
 Thanks to brxie for the initial code.
 
 
 ChangeLog
 ---------
 
+### 2.0.1 / 2023-07-30
+
+- Load certificate chain only if a certificate was specified
+
+
 ### 2.0.0 / 2020-10-04
 
 - Remove "six" dependency
 - Require Python >= 3.6
 
 
 ### 1.0.5 / 2020-10-04
```

### Comparing `pylogbeat-2.0.0/pylogbeat.py` & `pylogbeat-2.0.1/pylogbeat.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import logging
 import socket
 import ssl
 import sys
 import zlib
 
 
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 
 FRAME_TYPE_ACK = 0x41               # 'A'
 FRAME_TYPE_COMPRESSED_FRAME = 0x43  # 'C'
 FRAME_TYPE_JSON_FRAME = 0x4A        # 'J'
 FRAME_TYPE_WINDOW_SIZE = 0x57       # 'W'
 PAYLOAD_CHARSET = 'utf-8'           # encoding used for the payload / input message
 PROTOCOL_VERSION = 0x32             # version = 2
@@ -65,20 +65,16 @@
         self._last_ack = 0
         self._use_logging = use_logging
 
     def _log(self, level, format_, *args, **kwargs):
         if self._use_logging:
             LOGGER.log(level, format_, *args, **kwargs)
         elif level >= logging.WARNING:  # print warnings to stderr
-            message_format = '{} {} {}'.format(
-                datetime.now(),
-                logging.getLevelName(level),
-                format_,
-                *args,
-                **kwargs)
+            message = format_.format(*args, **kwargs)
+            message_format = f'{datetime.now()} {logging.getLevelName(level)} {message}'
             print(message_format, *args, file=sys.stderr, **kwargs)
 
     def __enter__(self):
         self.connect()
         return self
 
     def __exit__(self, type_, value, traceback):
@@ -103,29 +99,29 @@
         if self._ssl_verify:
             cert_reqs = ssl.CERT_REQUIRED
         elif self._ca_certs:
             cert_reqs = ssl.CERT_OPTIONAL
         else:
             cert_reqs = ssl.CERT_NONE
 
-        self._socket = ssl.wrap_socket(
-            self._socket,
-            keyfile=self._keyfile,
-            certfile=self._certfile,
-            ca_certs=self._ca_certs,
-            cert_reqs=cert_reqs)
+        ssl_context = ssl.create_default_context(cafile=self._ca_certs)
+        ssl_context.check_hostname = False
+        ssl_context.verify_mode = cert_reqs
+        if self._certfile and self._keyfile:
+            ssl_context.load_cert_chain(self._certfile, self._keyfile)
+        self._socket = ssl_context.wrap_socket(self._socket, server_side=False)
 
     def close(self):
         if self._socket is None:
             return  # nothing to do
 
         try:
             self._socket.close()
         except socket.error as exc:
-            self._log(logging.ERROR, 'Error closing socket: {}'.format(exc), exc_info=True)
+            self._log(logging.ERROR, f'Error closing socket: {exc}', exc_info=True)
         finally:
             self._socket = None
 
     def send(self, elements):
         self._validate_elements_sequence(elements)
 
         self.connect()  # lazy init
@@ -142,46 +138,43 @@
         while not self._expected_ack_received():
             self._read_ack()
 
     def _validate_elements_sequence(self, elements):
         # exclude strings to not detect them below as sequence
         valid_string_types = (str, bytes)
         if isinstance(elements, valid_string_types):
-            raise TypeError(
-                'Passed value has type "{}" but a sequence is expected'.format(type(elements)))
+            raise TypeError(f'Passed value has type "{type(elements)}" but a sequence is expected')
 
         sequence_types = (Sequence, Set)
         if not isinstance(elements, sequence_types):
-            raise TypeError(
-                'Passed value has type "{}" but a sequence is expected'.format(type(elements)))
+            raise TypeError(f'Passed value has type "{type(elements)}" but a sequence is expected')
 
         if not elements:
             return  # an empty sequence doesn't make much sense but is ok
 
         # check the elements to be a dict or string
         for element in elements:
             if isinstance(element, valid_string_types):
                 continue
             if isinstance(element, Mapping):
                 continue
 
             element_index = elements.index(element)
             raise TypeError(
-                'Element {} has type "{}" but a mapping, bytes or string object is expected'.format(
-                    element_index,
-                    type(element)))
+                f'Element {element_index} has type "{type(element)}" but a mapping, '
+                'bytes or string object is expected')
 
     def _reinit_last_ack(self):
         self._last_ack = 0
 
     def _factor_window_size(self, elements):
         return len(elements)
 
     def _factor_payload(self, elements):
-        payload_elements = list()
+        payload_elements = []
         for element in elements:
             self._increment_sequence()
             encoded_element = self._encode_json(element)
             payload_elements.append(encoded_element)
 
         return b''.join(payload_elements)
 
@@ -195,23 +188,23 @@
             element = json.dumps(element)
 
         if isinstance(element, str):
             element = element.encode(PAYLOAD_CHARSET)
 
         json_length = len(element)
         frame = [PROTOCOL_VERSION, FRAME_TYPE_JSON_FRAME, self._sequence, json_length, element]
-        pack_param = '>BBII{}s'.format(json_length)
+        pack_param = f'>BBII{json_length}s'
 
         payload = pack(pack_param, *frame)
         return payload
 
     def _compress_payload(self, payload):
         compressed_payload = zlib.compress(payload)
         compressed_payload_bytes = len(compressed_payload)
-        pack_format = '>BBI{}s'.format(compressed_payload_bytes)
+        pack_format = f'>BBI{compressed_payload_bytes}s'
         compress = pack(
             pack_format,
             PROTOCOL_VERSION,
             FRAME_TYPE_COMPRESSED_FRAME,
             compressed_payload_bytes,
             compressed_payload)
         return compress
@@ -219,56 +212,51 @@
     def _send_window_size(self):
         packed_window_size = pack(
             '>BBI',
             PROTOCOL_VERSION,
             FRAME_TYPE_WINDOW_SIZE,
             self._window_size)
         self._socket.send(packed_window_size)
-        self._log(logging.DEBUG, 'Sent window size: {}'.format(self._window_size))
+        self._log(logging.DEBUG, f'Sent window size: {self._window_size}')
 
     def _send_payload(self, compressed_payload):
         def chunker(chunk, size):
             for i in range(0, len(chunk), size):
                 start = i
                 end = start + size
                 yield chunk[start:end]
 
         written_bytes = 0
         # SSL and TLS channels must be segmented into records of no more than 16Kb
         for segment in chunker(compressed_payload, size=8192):
             written_bytes += self._socket.send(segment)
         self._log(
             logging.DEBUG,
-            'Sent payload bytes: {}, waiting for ACK: {}'.format(
-                written_bytes,
-                self._sequence))
+            f'Sent payload bytes: {written_bytes}, waiting for ACK: {self._sequence}')
 
     def _expected_ack_received(self):
         return self._last_ack == self._sequence
 
     def _read_ack(self):
         # first byte: read the version
         self._socket.recv(1)
         # second byte: frame type
         frame_type_packed = self._socket.recv(1)
         self._assert_frame_type_is_ack(frame_type_packed)
 
         received_ack = self._socket.recv(4)
         self._last_ack = unpack('>I', received_ack)[0]
-        self._log(logging.DEBUG, 'Received ACK: {}'.format(self._last_ack))
+        self._log(logging.DEBUG, f'Received ACK: {self._last_ack}')
 
     def _assert_frame_type_is_ack(self, frame_type_packed):
         if frame_type_packed:
             frame_type = unpack('B', frame_type_packed)[0]
             if frame_type == FRAME_TYPE_ACK:
                 return
         else:
             frame_type = 0
 
         self._log(
             logging.WARNING,
             'Waited for ACK from server but received an unexpected frame: '
-            '"0x{:02X}". Aborting.'.format(
-                frame_type))
-        raise ConnectionException(
-            'No ACK received or wrong frame type "0x{:02X}"'.format(
-                frame_type))
+            f'"0x{frame_type:02X}". Aborting.')
+        raise ConnectionException(f'No ACK received or wrong frame type "0x{frame_type:02X}"')
```

### Comparing `pylogbeat-2.0.0/setup.cfg` & `pylogbeat-2.0.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -16,56 +16,53 @@
 length_sort = false
 force_alphabetical_sort_within_sections = true
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 lines_after_imports = 2
 from_first = true
 include_trailing_comma = true
 
-[MASTER]
+[pylint.main]
 ignore = .git
 persistent = no
 load-plugins = 
 	pylint.extensions.bad_builtin,
 	pylint.extensions.check_elif,
 	pylint.extensions.comparetozero,
 	pylint.extensions.emptystring,
 	pylint.extensions.mccabe,
 	pylint.extensions.overlapping_exceptions,
 	pylint.extensions.redefined_variable_type
 
-[MESSAGES CONTROL]
+[pylint]
 disable = 
 	fixme,
 	duplicate-code,
 	empty-docstring,
 	logging-format-interpolation,
 	missing-docstring,
 	no-else-raise,
 	no-else-return,
-	no-self-use,
-	unnecessary-pass,
-	useless-object-inheritance
+	unnecessary-pass
 
-[REPORTS]
+[pylint.reports]
 output-format = parseable
-files-output = no
 reports = no
 
-[FORMAT]
+[pylint.format]
 max-line-length = 100
 
-[VARIABLES]
+[pylint.variables]
 dummy-variables-rgx = _|dummy
 
-[DESIGN]
+[pylint.design]
 min-public-methods = 0
 max-attributes = 15
 max-args = 7
 max-parents = 9
 
-[EXCEPTIONS]
+[pylint.exceptions]
 overgeneral-exceptions = 
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pylogbeat-2.0.0/setup.py` & `pylogbeat-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from shutil import rmtree
 import sys
 
 from setuptools import setup
 
 
 NAME = 'pylogbeat'
-VERSION = '2.0.0'
+VERSION = '2.0.1'
 
 here = path.abspath(path. dirname(__file__))
 with open(path.join(here, 'README.md'), 'rb') as f:
     LONG_DESCRIPTION = f.read().decode('utf-8')
 
 
 if 'bdist_wheel' in sys.argv:
```

