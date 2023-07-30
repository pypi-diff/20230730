# Comparing `tmp/fshare-1.0.2.tar.gz` & `tmp/fshare-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fshare-1.0.2.tar", last modified: Sun Jul 30 14:52:17 2023, max compression
+gzip compressed data, was "fshare-1.1.0.tar", last modified: Sun Jul 30 15:15:12 2023, max compression
```

## Comparing `fshare-1.0.2.tar` & `fshare-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 14:52:17.375135 fshare-1.0.2/
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     2997 2023-07-30 14:52:17.375135 fshare-1.0.2/PKG-INFO
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     2289 2023-07-29 16:56:38.000000 fshare-1.0.2/README.md
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1045 2023-07-30 14:50:51.000000 fshare-1.0.2/pyproject.toml
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       38 2023-07-30 14:52:17.375135 fshare-1.0.2/setup.cfg
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 14:52:17.372135 fshare-1.0.2/src/
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 14:52:17.374135 fshare-1.0.2/src/fshare/
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       30 2023-07-29 20:52:17.000000 fshare-1.0.2/src/fshare/__init__.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       60 2023-07-30 14:52:01.000000 fshare-1.0.2/src/fshare/__main__.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      734 2023-07-30 14:51:50.000000 fshare-1.0.2/src/fshare/cli.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1636 2023-07-28 22:50:43.000000 fshare-1.0.2/src/fshare/filemanager.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3205 2023-07-28 22:46:37.000000 fshare-1.0.2/src/fshare/index.html
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      715 2023-07-28 22:35:20.000000 fshare-1.0.2/src/fshare/index.js
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1707 2023-07-30 14:51:23.000000 fshare-1.0.2/src/fshare/main.py
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 14:52:17.375135 fshare-1.0.2/src/fshare.egg-info/
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     2997 2023-07-30 14:52:17.000000 fshare-1.0.2/src/fshare.egg-info/PKG-INFO
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      311 2023-07-30 14:52:17.000000 fshare-1.0.2/src/fshare.egg-info/SOURCES.txt
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        1 2023-07-30 14:52:17.000000 fshare-1.0.2/src/fshare.egg-info/dependency_links.txt
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        7 2023-07-30 14:52:17.000000 fshare-1.0.2/src/fshare.egg-info/top_level.txt
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:15:12.277873 fshare-1.1.0/
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3967 2023-07-30 15:15:12.277873 fshare-1.1.0/PKG-INFO
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3260 2023-07-30 15:14:46.000000 fshare-1.1.0/README.md
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1037 2023-07-30 14:53:30.000000 fshare-1.1.0/pyproject.toml
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       38 2023-07-30 15:15:12.277873 fshare-1.1.0/setup.cfg
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:15:12.273873 fshare-1.1.0/src/
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:15:12.275873 fshare-1.1.0/src/fshare/
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       30 2023-07-29 20:52:17.000000 fshare-1.1.0/src/fshare/__init__.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       60 2023-07-30 14:52:01.000000 fshare-1.1.0/src/fshare/__main__.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      740 2023-07-30 14:56:26.000000 fshare-1.1.0/src/fshare/cli.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1636 2023-07-28 22:50:43.000000 fshare-1.1.0/src/fshare/filemanager.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3205 2023-07-28 22:46:37.000000 fshare-1.1.0/src/fshare/index.html
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      715 2023-07-28 22:35:20.000000 fshare-1.1.0/src/fshare/index.js
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1707 2023-07-30 14:51:23.000000 fshare-1.1.0/src/fshare/main.py
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:15:12.276873 fshare-1.1.0/src/fshare.egg-info/
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3967 2023-07-30 15:15:12.000000 fshare-1.1.0/src/fshare.egg-info/PKG-INFO
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      311 2023-07-30 15:15:12.000000 fshare-1.1.0/src/fshare.egg-info/SOURCES.txt
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        1 2023-07-30 15:15:12.000000 fshare-1.1.0/src/fshare.egg-info/dependency_links.txt
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        7 2023-07-30 15:15:12.000000 fshare-1.1.0/src/fshare.egg-info/top_level.txt
```

### Comparing `fshare-1.0.2/PKG-INFO` & `fshare-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,101 @@
-Metadata-Version: 2.1
-Name: fshare
-Version: 1.0.2
-Summary: A python package that serves as an easy file sharing application over local network
-Author-email: Stevo Mitric <stevomitric2000@gmail.com>
-Maintainer-email: Stevo Mitric <stevomitric2000@gmail.com>
-Project-URL: Homepage, https://github.com/stevomitric/fshare
-Project-URL: Bug Tracker, https://github.com/stevomitric/fshare/issues
-Keywords: file,share
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Flask
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
 
-# File-Share
+# File Share - Local File Sharing Service
 
-File-Share is a Python 3 package that simplifies file sharing over a local network. It provides an easy-to-use interface for users to share files with other devices connected to the same network. Whether you want to transfer documents, images, videos, or any other files, File-Share has got you covered!
+fshare is a Python package that serves as a file sharing service over a local network. It utilizes Flask to create a local server on port 8000, allowing users to upload files and share them within the network.
 
 ## Installation
 
-To use File-Share, you need to have Flask installed. If you don't have Flask, you can install it using pip:
+To install fshare, use pip:
 
-    pip install flask
+```bash
+pip install fshare
+```
 
-Next, you can install File-Share using pip as well:
+All of the required dependencies (`flask >= 1.0.0`) will be installed automatically by pip.
 
-    pip install fshare
+## Running the Service
 
-## Usage
+To start the file-sharing service, run the following command:
 
-Using File-Share is straightforward. Once you have installed the package and its dependencies, you can start sharing files with just a few lines of code. Here's an example of how to use File-Share in your Python script:
+```bash
+python -m fshare
+```
 
+You're all set! Servers is up and running on http://localhost:8000
 
-    from fshare import FileShare
 
-    # Initialize the FileShare object
-    file_share = FileShare()
+Default save-location is the temp directory (`/tmp/fshare` on unix like systems or `%tmp%/fshare` on windows)
 
-    # Set the path to the directory containing files to be shared
-    file_share.set_directory("/path/to/shared/files")
+## Command-Line Options
 
-    # Start the file sharing server
-    file_share.start_server()
+fshare supports the following command-line options:
 
-    # Once the server is running, you can access it from other devices on the local network
-    # Open a web browser and navigate to: http://your_server_ip:5000
+```plaintext
+usage: python -m fshare [-h] [--bind BIND] [--port PORT] [--location LOCATION]
 
-    # To stop the server (when you're done sharing files), use:
-    # file_share.stop_server()
+Starts the python file-sharing service application
 
-## Security
+options:
+  -h, --help            show this help message and exit
+  --bind BIND, -b BIND  The local address to bind the server
+  --port PORT, -p PORT  File server port to run on
+  --location LOCATION, -l LOCATION
+                        The path to the folder where files will be stored
+                        (default: /tmp/fshare)
+```
 
-File-Share is intended for use within local networks and is not designed for production environments or public internet access. As such, it does not provide advanced security features. Please ensure that you only use File-Share on trusted networks to avoid potential security risks.
+### Options
+
+- `-h`, `--help`: Displays the help message and exits.
+- `--bind BIND`, `-b BIND`: Sets the local address to bind the server (optional).
+- `--port PORT`, `-p PORT`: Specifies the file server port to run on (optional).
+- `--location LOCATION`, `-l LOCATION`: Sets the path to the folder where files will be stored. By default, files are stored in `/tmp/fshare`.
+
+## Example Usage
+
+Here's an example of running fshare with custom options:
+
+```bash
+python -m fshare --port 8080 --location /path/to/custom/folder
+```
+
+This will start the file-sharing service on port 8080 and use `/path/to/custom/folder` as the file storage location.
+
+## Running programatically
+
+Fshare can be imported in your project alongside with a reference to the `FileManager` class and the `flask` app.
+
+```python
+from fshare.main import app, fileManager
+
+# change the save-location path
+# fileManager.changeLocation('/new/location/path')
+
+app.run(host='0.0.0.0', port=8000, debug=True)
+
+```
 
 ## Contributing
 
 We welcome contributions from the community! If you find any issues, have suggestions for improvements, or want to add new features, please feel free to open an issue or submit a pull request on our GitHub repository.
-License
 
-File-Share is released under the MIT License.
+## License
 
-## Disclaimer
+fshare is open-source software released under the MIT License. See the [LICENSE](LICENSE) file for more details.
 
-File-Share is provided "as is" without warranty of any kind, express or implied. Use it at your own risk. The authors of File-Share are not responsible for any damages or liabilities resulting from the use of this package.
+## Issues
+
+For any issues or feedback, please visit the [Bug Tracker](https://github.com/stevomitric/fshare/issues) on GitHub.
 
 ## Contact
 
-If you have any questions or need further assistance, you can reach out to me stevomitric2000@gmail.com.
+For questions or inquiries, you can reach out to Stevo Mitric at stevomitric2000@gmail.com.
+
+## Disclaimer
+
+File-Share is provided "as is" without warranty of any kind, express or implied. Use it at your own risk. The authors of File-Share are not responsible for any damages or liabilities resulting from the use of this package.
+
+## Acknowledgments
 
-Happy file sharing!
+- fshare is built with the help of Flask and other open-source libraries.
+- Special thanks to the Python community for their continuous support.
```

### Comparing `fshare-1.0.2/pyproject.toml` & `fshare-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fshare"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="Stevo Mitric", email="stevomitric2000@gmail.com" },
 ]
 maintainers = [
   { name="Stevo Mitric", email="stevomitric2000@gmail.com" },
 ]
 description = "A python package that serves as an easy file sharing application over local network"
@@ -34,8 +34,8 @@
 where = ["src"]
 fshare = ["*.html", "*.js"]
 
 [tool.poetry.dependencies]
 flask = "^0.1"
 
 [tool.poetry.scripts]
-my_package_cli = 'fshare.main:run'
+fshare = 'fshare.main:run'
```

### Comparing `fshare-1.0.2/src/fshare/cli.py` & `fshare-1.1.0/src/fshare/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 
 from fshare.main import app, fileManager
 
 def main():
     parser = argparse.ArgumentParser(description="Starts the python file-sharing service application")
     parser.add_argument("--bind", "-b", type=str, default="0.0.0.0", help="The local address to bind the server")
     parser.add_argument("--port", "-p", type=int, default=8000, help="File server port to run on")
-    parser.add_argument("--location", "-l", type=str, default="", help="The path to the folder where files will be stored (default: %tmp%)")
+    parser.add_argument("--location", "-l", type=str, default="", help="The path to the folder where files will be stored (default: /tmp/fshare)")
     args = vars(parser.parse_args())
 
     if ("location" in args and args["location"]):
         fileManager.changeLocation(args["location"])
     app.run(debug=False, host = args["bind"], port=args["port"] )
```

### Comparing `fshare-1.0.2/src/fshare/filemanager.py` & `fshare-1.1.0/src/fshare/filemanager.py`

 * *Files identical despite different names*

### Comparing `fshare-1.0.2/src/fshare/index.html` & `fshare-1.1.0/src/fshare/index.html`

 * *Files identical despite different names*

### Comparing `fshare-1.0.2/src/fshare/index.js` & `fshare-1.1.0/src/fshare/index.js`

 * *Files identical despite different names*

### Comparing `fshare-1.0.2/src/fshare/main.py` & `fshare-1.1.0/src/fshare/main.py`

 * *Files identical despite different names*

