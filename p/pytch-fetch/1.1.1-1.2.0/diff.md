# Comparing `tmp/pytch-fetch-1.1.1.tar.gz` & `tmp/pytch-fetch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytch-fetch-1.1.1.tar", last modified: Tue Jul 25 16:37:38 2023, max compression
+gzip compressed data, was "pytch-fetch-1.2.0.tar", last modified: Sun Jul 30 05:23:38 2023, max compression
```

## Comparing `pytch-fetch-1.1.1.tar` & `pytch-fetch-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.639725 pytch-fetch-1.1.1/
--rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.1.1/LICENSE
--rw-r--r--   0 krit      (1000) krit      (1001)     4258 2023-07-25 16:37:38.638725 pytch-fetch-1.1.1/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)     1779 2023-07-25 16:13:59.000000 pytch-fetch-1.1.1/README.md
--rw-r--r--   0 krit      (1000) krit      (1001)     1329 2023-07-25 16:37:25.000000 pytch-fetch-1.1.1/pyproject.toml
--rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-25 16:37:38.639725 pytch-fetch-1.1.1/setup.cfg
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.637725 pytch-fetch-1.1.1/src/
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.638725 pytch-fetch-1.1.1/src/pytch/
--rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.1.1/src/pytch/__init__.py
--rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-25 16:36:56.000000 pytch-fetch-1.1.1/src/pytch/__main__.py
--rw-r--r--   0 krit      (1000) krit      (1001)    21003 2023-07-25 16:13:59.000000 pytch-fetch-1.1.1/src/pytch/art.py
--rw-r--r--   0 krit      (1000) krit      (1001)     6373 2023-07-25 16:13:59.000000 pytch-fetch-1.1.1/src/pytch/funcs.py
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.638725 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/
--rw-r--r--   0 krit      (1000) krit      (1001)     4258 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/entry_points.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/top_level.txt
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/
+-rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.2.0/LICENSE
+-rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)     1825 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/README.md
+-rw-r--r--   0 krit      (1000) krit      (1001)     1374 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/pyproject.toml
+-rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/setup.cfg
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.022762 pytch-fetch-1.2.0/src/
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.023762 pytch-fetch-1.2.0/src/pytch/
+-rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.2.0/src/pytch/__init__.py
+-rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/src/pytch/__main__.py
+-rw-r--r--   0 krit      (1000) krit      (1001)    21693 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/src/pytch/art.py
+-rw-r--r--   0 krit      (1000) krit      (1001)     6733 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/src/pytch/funcs.py
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/
+-rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/entry_points.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/top_level.txt
```

### Comparing `pytch-fetch-1.1.1/LICENSE` & `pytch-fetch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.1.1/PKG-INFO` & `pytch-fetch-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.1.1
+Version: 1.2.0
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -25,19 +25,20 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kritdass/pytch
 Project-URL: Repository, https://github.com/kritdass/pytch
 Keywords: linux,fetch,terminal
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -55,21 +56,22 @@
 
 <br/>
 
 ![](https://lh3.googleusercontent.com/pw/AIL4fc_Z8qwS2and18m9T_TictE9eg82GOBcLVCsdvM5rJSt1ytndTxPbYtbkLVOrwiVev-Kq19oc5ge2c-dVKi65ec8FOF5__IceoUDGE-tGR0HxpO-Wa-j8peliYgIpedMdh-3SdkB1dNd_kG6uN3YghYH=w577-h811-s-no)
 
 ## Description
 
-Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions and macOS (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
+Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. Pytch currently supports macOS, FreeBSD, and many popular Linux distributions (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your system, please open up an issue and I will add support for your system. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pytch-fetch
 ```
 You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
 
 ## Acknowlegements
 
 - [@ssleert](https://github.com/ssleert) for creating [nitch](https://github.com/ssleert/nitch), which inspired this project
 - [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos
 - [@willrson](https://github.com/willrson) and [@kapoorkrish](https://github.com/kapoorkrish) for helping add macOS support
+- [@z-ffqq](https://github.com/z-ffqq) for adding FreeBSD support
```

### Comparing `pytch-fetch-1.1.1/README.md` & `pytch-fetch-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 <br/>
 
 ![](https://lh3.googleusercontent.com/pw/AIL4fc_Z8qwS2and18m9T_TictE9eg82GOBcLVCsdvM5rJSt1ytndTxPbYtbkLVOrwiVev-Kq19oc5ge2c-dVKi65ec8FOF5__IceoUDGE-tGR0HxpO-Wa-j8peliYgIpedMdh-3SdkB1dNd_kG6uN3YghYH=w577-h811-s-no)
 
 ## Description
 
-Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions and macOS (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
+Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. Pytch currently supports macOS, FreeBSD, and many popular Linux distributions (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your system, please open up an issue and I will add support for your system. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pytch-fetch
 ```
 You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
 
 ## Acknowlegements
 
 - [@ssleert](https://github.com/ssleert) for creating [nitch](https://github.com/ssleert/nitch), which inspired this project
 - [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos
 - [@willrson](https://github.com/willrson) and [@kapoorkrish](https://github.com/kapoorkrish) for helping add macOS support
+- [@z-ffqq](https://github.com/z-ffqq) for adding FreeBSD support
```

### Comparing `pytch-fetch-1.1.1/pyproject.toml` & `pytch-fetch-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytch-fetch"
-version = "1.1.1"
+version = "1.2.0"
 description="Pytch Yields Technical Characteristics Hastily"
 readme = "README.md"
 authors = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 maintainers = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
-  "Development Status :: 1 - Planning",
+  "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
+  "Operating System :: POSIX :: BSD :: FreeBSD",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
```

### Comparing `pytch-fetch-1.1.1/src/pytch/__main__.py` & `pytch-fetch-1.2.0/src/pytch/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "-l",
         "--logo",
         metavar="DISTRO",
         dest="logo",
         help="use an alternate distribution's logo",
     )
 
-    parser.add_argument("-v", "--version", action="version", version="1.1.1")
+    parser.add_argument("-v", "--version", action="version", version="1.2.0")
 
     args = parser.parse_args()
 
     attrs = [
         {"name": "user", "value": getlogin(), "icon": "", "color": "red"},
         {
             "name": "os",
```

### Comparing `pytch-fetch-1.1.1/src/pytch/art.py` & `pytch-fetch-1.2.0/src/pytch/art.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,8 +544,28 @@
  ${c5}'XMMMMMMMMMMMMMMMMMMMMMMMMMMk
   'XMMMMMMMMMMMMMMMMMMMMMMMMK.
     ${c6}kMMMMMMMMMMMMMMMMMMMMMMd
      ;KMMMMMMMWXXWMMMMMMMk.
        "cooc*"    "*coo'"
         """,
     },
+    "freebsd": {
+        "colors": ["red", "white"],
+        "ascii": r"""
+${c2}```                        ${c1}`
+${c2}  ` `.....---...${c1}....--.```   -/
+${c2}  +o   .--`         ${c1}/y:`      +.
+${c2}   yo`:.            ${c1}:o      `+-
+${c2}    y/               ${c1}-/`   -o/
+${c2}   .-                  ${c1}::/sy+:.
+${c2}   /                     ${c1}`--  /
+${c2}  `:                          ${c1}:`
+${c2}  `:                          ${c1}:`
+${c2}   /                          ${c1}/
+${c2}   .-                        ${c1}-.
+${c2}    --                      ${c1}-.
+${c2}     `:`                  ${c1}`:`
+       .--             `--.
+          .---.....----.
+        """,
+    },
 }
```

### Comparing `pytch-fetch-1.1.1/src/pytch/funcs.py` & `pytch-fetch-1.2.0/src/pytch/funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from os.path import isfile
 from platform import release
 from sys import platform
 from subprocess import check_output, DEVNULL, CalledProcessError
 from re import search, findall, sub, split
 from pytch.art import art_dict
 
-
 def get_output(cmd):
     return check_output([cmd], shell=True, text=True, stderr=DEVNULL)
 
 
 def color(text, color):
     colors = {
         "black": 90,
@@ -96,15 +95,15 @@
 def get_kernel():
     return release().split("-")[0].strip()
 
 
 def get_uptime():
     seconds = 0
 
-    if get_name() == "Darwin":
+    if get_name() in ["Darwin", "FreeBSD"]:
         boot = get_output("sysctl -n kern.boottime")
         boot = search(r"sec = (\d+)", boot).group(1)
         now = get_output("date +%s")
         seconds = int(now) - int(boot)
     else:
         with open("/proc/uptime", "r") as file:
             seconds = int(float(file.readline().split()[0]))
@@ -134,23 +133,27 @@
         ).group(1)
         mem = {}
         for line in vm_stat[1:]:
             mem[line.split(":")[0]] = int(float(line.split(":")[1].strip()))
         mem_available = (
             mem["Pages wired down"] + mem["Pages active"] + mem["Pages inactive"]
         ) * int(page_size)
+    elif get_name() == "FreeBSD":
+        mem_total = int(get_output("sysctl -n hw.physmem")) / 1024
+        page_size = int(get_output("sysctl -n hw.pagesize"))
+        mem_available = int(get_output("sysctl -n vm.stats.vm.v_free_count")) * page_size / 1024
     else:
         with open("/proc/meminfo", "r") as mem_file:
             for pair in mem_file.read().splitlines():
                 if pair.split(":")[0] == "MemTotal":
                     mem_total = pair.split(":")[1].replace("kB", "").strip()
                 elif pair.split(":")[0] == "MemAvailable":
                     mem_available = pair.split(":")[1].replace("kB", "").strip()
-    return f"{int((int(mem_total) - int(mem_available)) * 100 / int(mem_total))}%"
 
+    return f"{int((int(mem_total) - int(mem_available)) * 100 / int(mem_total))}%"
 
 def get_packages():
     def get_lines(cmd):
         packages = get_output(cmd)
         num_pkgs = len(packages.splitlines())
         return str(num_pkgs)
 
@@ -182,14 +185,16 @@
         packages.append(f"{get_lines('xbps-query -l')} (xbps)")
     elif name in ["Gentoo", "ChromeOS"]:
         packages.append(f"{get_lines('ls -d /var/db/pkg/*/*| cut -f5- -d/')} (portage)")
     elif name == "NixOS":
         packages.append(
             f"{get_lines('nix-store -qR /run/current-system/sw ~/.nix-profile')} (nix)"
         )
+    elif name == "FreeBSD":
+        packages.append(f"{get_lines('pkg info -q')} (pkg)")
 
     if name != "NixOS":
         if name == "Darwin":
             try:
                 packages.append(
                     f"{get_lines('nix-store -qR /run/current-system/sw ~/.nix-profile')} (nix)"
                 )
```

### Comparing `pytch-fetch-1.1.1/src/pytch_fetch.egg-info/PKG-INFO` & `pytch-fetch-1.2.0/src/pytch_fetch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.1.1
+Version: 1.2.0
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -25,19 +25,20 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kritdass/pytch
 Project-URL: Repository, https://github.com/kritdass/pytch
 Keywords: linux,fetch,terminal
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -55,21 +56,22 @@
 
 <br/>
 
 ![](https://lh3.googleusercontent.com/pw/AIL4fc_Z8qwS2and18m9T_TictE9eg82GOBcLVCsdvM5rJSt1ytndTxPbYtbkLVOrwiVev-Kq19oc5ge2c-dVKi65ec8FOF5__IceoUDGE-tGR0HxpO-Wa-j8peliYgIpedMdh-3SdkB1dNd_kG6uN3YghYH=w577-h811-s-no)
 
 ## Description
 
-Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions and macOS (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
+Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. Pytch currently supports macOS, FreeBSD, and many popular Linux distributions (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your system, please open up an issue and I will add support for your system. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pytch-fetch
 ```
 You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
 
 ## Acknowlegements
 
 - [@ssleert](https://github.com/ssleert) for creating [nitch](https://github.com/ssleert/nitch), which inspired this project
 - [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos
 - [@willrson](https://github.com/willrson) and [@kapoorkrish](https://github.com/kapoorkrish) for helping add macOS support
+- [@z-ffqq](https://github.com/z-ffqq) for adding FreeBSD support
```

