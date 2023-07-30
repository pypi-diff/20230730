# Comparing `tmp/jsonator-0.1.3.tar.gz` & `tmp/jsonator-0.1.4.tar.gz`

## Comparing `jsonator-0.1.3.tar` & `jsonator-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 jsonator-0.1.3/jsonator/__init__.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 jsonator-0.1.3/jsonator/jsonator.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jsonator-0.1.3/jsonator/output.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jsonator-0.1.3/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jsonator-0.1.3/LICENSE
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jsonator-0.1.3/README.rst
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 jsonator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 jsonator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/__main__.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/jsonator.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/output.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 jsonator-0.1.4/README.rst
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jsonator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 jsonator-0.1.4/PKG-INFO
```

### Comparing `jsonator-0.1.3/jsonator/jsonator.py` & `jsonator-0.1.4/jsonator/jsonator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,94 @@
-"""
-Format JSON using json tool
-"""
-import filecmp
-import os
-import random
-import string
-import sys
-from enum import Enum
-from pathlib import Path
-from tempfile import gettempdir
-
-from jsonator import output
-
-INTERPRETER = Path(sys.executable).stem
-FILES_ENCODING = "utf-8"
-
-
-class ReturnCode(Enum):
-    """Set of possible return codes"""
-
-    NOTHING_WOULD_CHANGE = 0
-    SOME_FILES_WOULD_BE_REFORMATTED = 1
-    FILE_NOT_FOUND = 122
-    INTERNAL_ERROR = 123
-
-
-def random_str() -> str:
-    """Generating a random alphanumeric string of 8 characters long"""
-    return "".join(random.choices(string.ascii_letters + string.digits, k=8))
-
-
-def make_temp_file() -> Path:
-    """Generate temp file path"""
-    temp_dir = Path(gettempdir()).absolute()
-    temp_file = temp_dir / random_str()
-
-    while temp_file.exists():
-        temp_file = temp_dir / random_str()
-
-    return temp_file
-
-
-def format_json_file(json_file: Path, check: bool, diff: bool, color: bool) -> ReturnCode:
-    """
-    This function formats the file in JSON format.
-    It uses the json.tool module, built into Python, to create a readable JSON format.
-    """
-    if check or diff:
-        print(f"Comparing {json_file} - ", end="")
-    else:
-        print(f"Formatting {json_file}")
-
-    tmp_file = make_temp_file()
-    os.system(f"{INTERPRETER} -m json.tool {json_file} {tmp_file}")
-
-    if check or diff:
-        is_identical = filecmp.cmp(json_file, tmp_file, shallow=False)
-
-        if is_identical:
-            print("Ok")
-            os.unlink(tmp_file)
-            return ReturnCode.NOTHING_WOULD_CHANGE
-
-        print("Need to format")
-        diff_contents = output.diff(
-            json_file.read_text(encoding=FILES_ENCODING),
-            tmp_file.read_text(encoding=FILES_ENCODING),
-            json_file.name,
-            tmp_file.name,
-        )
-
-        if color:
-            diff_contents = output.color_diff(diff_contents)
-
-        print(diff_contents)
-
-        os.unlink(tmp_file)
-        return ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED
-
-    if tmp_file.exists():
-        os.unlink(json_file)
-        os.rename(tmp_file, json_file)
-    else:
-        return ReturnCode.INTERNAL_ERROR
-
-    return ReturnCode.NOTHING_WOULD_CHANGE
+"""
+Format JSON using json tool
+"""
+import filecmp
+import os
+import random
+import string
+import sys
+from enum import Enum
+from pathlib import Path
+from tempfile import gettempdir
+
+from jsonator import output
+
+INTERPRETER = Path(sys.executable).stem
+FILES_ENCODING = "utf-8"
+
+
+class ReturnCode(Enum):
+    """Set of possible return codes"""
+
+    NOTHING_WOULD_CHANGE = 0
+    SOME_FILES_WOULD_BE_REFORMATTED = 1
+    FILE_NOT_FOUND = 122
+    INTERNAL_ERROR = 123
+
+
+def random_str() -> str:
+    """Generating a random alphanumeric string of 8 characters long"""
+    return "".join(random.choices(string.ascii_letters + string.digits, k=8))
+
+
+def make_temp_file() -> Path:
+    """Generate temp file path"""
+    temp_dir = Path(gettempdir()).absolute()
+    temp_file = temp_dir / random_str()
+
+    while temp_file.exists():
+        temp_file = temp_dir / random_str()
+
+    return temp_file
+
+
+def format_json_file(
+    json_file: Path, check: bool, diff: bool, color: bool, sort_keys: bool
+) -> ReturnCode:
+    """
+    This function formats the file in JSON format.
+    It uses the json.tool module, built into Python, to create a readable JSON format.
+    """
+    if check or diff:
+        print(f"Comparing {json_file} - ", end="")
+    else:
+        print(f"Formatting {json_file}")
+
+    tmp_file = make_temp_file()
+
+    cmd = [INTERPRETER, "-m", "json.tool", json_file, tmp_file]
+    if sort_keys:
+        cmd.append("--sort-keys")
+
+    os.system(" ".join([str(command) for command in cmd]))
+
+    if check or diff:
+        is_identical = filecmp.cmp(json_file, tmp_file, shallow=False)
+
+        if is_identical:
+            print("Ok")
+            os.unlink(tmp_file)
+            return ReturnCode.NOTHING_WOULD_CHANGE
+
+        print("Need to format")
+        diff_contents = output.diff(
+            json_file.read_text(encoding=FILES_ENCODING),
+            tmp_file.read_text(encoding=FILES_ENCODING),
+            json_file.name,
+            tmp_file.name,
+        )
+
+        if color:
+            diff_contents = output.color_diff(diff_contents)
+
+        print(diff_contents)
+
+        os.unlink(tmp_file)
+        return ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED
+
+    if tmp_file.exists():
+        os.unlink(json_file)
+        os.rename(tmp_file, json_file)
+    else:
+        return ReturnCode.INTERNAL_ERROR
+
+    return ReturnCode.NOTHING_WOULD_CHANGE
```

### Comparing `jsonator-0.1.3/LICENSE` & `jsonator-0.1.4/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Sergey Fomin
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Sergey Fomin
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `jsonator-0.1.3/README.rst` & `jsonator-0.1.4/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,65 @@
-JSONator
-========
-
-Description
------------
-
-This module provides a command-line interface for formatting JSON files.
-It takes a path to either a JSON file or a directory containing JSON files
-as input and can recursively scan subdirectories for JSON files. The module
-returns an exit code indicating whether any files were reformatted or if there
-were any errors.
-
-Usage
------
-
-The main() function is the entry point for the module and returns an exit code
-indicating the result of the JSON formatting operation. The following arguments
-can be passed to the main() function:
-
-* path: A required argument that specifies the path to the JSON file or directory containing JSON files to be formatted.
-
-* --recursive or -r: An optional flag that specifies whether to scan subdirectories for JSON files.
-
-* --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
-
-* --diff: Don't write the files back, just output a diff for each file on stdout.
-
-* --color: Show colored diff. Only applies when `--diff` is given.
-
-The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
-
-* `0`: Indicates that no files would be reformatted.
-
-* `1`: Indicates that some files would be reformatted.
-
-* `122`: Indicates that the specified file or directory was not found.
-
-* `123`: Indicates that there was an internal error.
-
-Example usage:
---------------
-::
-
-$ jsonator /path/to/json/file.json --check
+JSONator
+========
+
+Description
+-----------
+
+This module provides a command-line interface for formatting JSON files.
+It takes a path to either a JSON file or a directory containing JSON files
+as input and can recursively scan subdirectories for JSON files. The module
+returns an exit code indicating whether any files were reformatted or if there
+were any errors.
+
+Usage
+-----
+
+The main() function is the entry point for the module and returns an exit code
+indicating the result of the JSON formatting operation. The following arguments
+can be passed to the main() function:
+
+* path: A required argument that specifies the path to the JSON file or directory containing JSON files to be formatted.
+
+* --recursive or -r: An optional flag that specifies whether to scan subdirectories for JSON files.
+
+* --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
+
+* --diff: Don't write the files back, just output a diff for each file on stdout.
+
+* --color: Show colored diff. Only applies when `--diff` is given.
+
+The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
+
+* `0`: Indicates that no files would be reformatted.
+
+* `1`: Indicates that some files would be reformatted.
+
+* `122`: Indicates that the specified file or directory was not found.
+
+* `123`: Indicates that there was an internal error.
+
+Example usage:
+--------------
+::
+
+$ jsonator /path/to/json/file.json --check
+
+
+Dev:
+--------------
+Build package
+
+::
+
+$ python -m build
+
+Check package
+
+::
+
+$ twine check dist/*
+
+Publish package
+
+::
+
+$ twine upload dist/*
```

### Comparing `jsonator-0.1.3/PKG-INFO` & `jsonator-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonator
-Version: 0.1.3
+Version: 0.1.4
 Summary: JSON formatting and validating tool
 Project-URL: Homepage, https://github.com/sfominx/jsonator
 Author-email: Sergey Fomin <sergiusnn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
@@ -50,7 +50,28 @@
 * `123`: Indicates that there was an internal error.
 
 Example usage:
 --------------
 ::
 
 $ jsonator /path/to/json/file.json --check
+
+
+Dev:
+--------------
+Build package
+
+::
+
+$ python -m build
+
+Check package
+
+::
+
+$ twine check dist/*
+
+Publish package
+
+::
+
+$ twine upload dist/*
```

