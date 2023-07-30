# Comparing `tmp/pyarmor-8.3.dev1.zip` & `tmp/pyarmor-8.3.dev2.zip`

## zipinfo {}

```diff
@@ -1,145 +1,148 @@
-Zip file size: 2330610 bytes, number of entries: 143
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor.egg-info/
--rw-r--r--  2.0 unx     3004 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/PKG-INFO
--rwxr-xr-x  2.0 unx      191 b- defN 23-Mar-04 11:58 pyarmor-8.3.dev1/MANIFEST.in
--rw-r--r--  2.0 unx     6553 b- defN 23-May-11 12:30 pyarmor-8.3.dev1/README.md
--rw-r--r--  2.0 unx     4352 b- defN 23-Jul-19 09:21 pyarmor-8.3.dev1/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/setup.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/plugins/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/polyfills/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/helper/
--rw-r--r--  2.0 unx      234 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev1/pyarmor/pyshield.lic
--rwxr-xr-x  2.0 unx     2038 b- defN 23-Jul-19 09:21 pyarmor-8.3.dev1/pyarmor/config.py
--rwxr-xr-x  2.0 unx    10197 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/benchmark.py
--rw-r--r--  2.0 unx     6994 b- defN 23-May-12 06:32 pyarmor-8.3.dev1/pyarmor/register.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev1/pyarmor/product.key
--rwxr-xr-x  2.0 unx    65827 b- defN 23-Mar-26 00:20 pyarmor-8.3.dev1/pyarmor/pyarmor.py
--rw-r--r--  2.0 unx     2664 b- defN 22-Jan-29 09:20 pyarmor-8.3.dev1/pyarmor/protect_code.pt
--rw-r--r--  2.0 unx    13587 b- defN 21-Nov-02 17:34 pyarmor-8.3.dev1/pyarmor/pytransform.py
--rw-r--r--  2.0 unx     3363 b- defN 22-Jun-27 00:08 pyarmor-8.3.dev1/pyarmor/sppmode.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev1/pyarmor/public.key
--rwxr-xr-x  2.0 unx      113 b- defN 20-Jan-02 11:09 pyarmor-8.3.dev1/pyarmor/__init__.py
--rw-r--r--  2.0 unx     2191 b- defN 22-Dec-04 19:13 pyarmor-8.3.dev1/pyarmor/reform.py
--rwxr-xr-x  2.0 unx    25832 b- defN 22-Nov-20 13:42 pyarmor-8.3.dev1/pyarmor/packer.py
--rw-r--r--  2.0 unx     5200 b- defN 23-Jan-06 00:02 pyarmor-8.3.dev1/pyarmor/cobuilder.py
--rwxr-xr-x  2.0 unx    67431 b- defN 22-Dec-23 17:42 pyarmor-8.3.dev1/pyarmor/utils.py
--rw-r--r--  2.0 unx       37 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/pyarmor-webui.py
--rwxr-xr-x  2.0 unx    28176 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/pyarmor-deprecated.py
--rw-r--r--  2.0 unx     4028 b- defN 21-Dec-16 08:28 pyarmor-8.3.dev1/pyarmor/build_meta.py
--rw-r--r--  2.0 unx      256 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev1/pyarmor/license.tri
--rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor-8.3.dev1/pyarmor/README.rst
--rw-r--r--  2.0 unx     1596 b- defN 22-Jan-30 11:51 pyarmor-8.3.dev1/pyarmor/protect_code2.pt
--rw-r--r--  2.0 unx     2234 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/pyimcore.py
--rw-r--r--  2.0 unx     2487 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev1/pyarmor/public_capsule.zip
--rwxr-xr-x  2.0 unx     8023 b- defN 22-Jun-28 09:01 pyarmor-8.3.dev1/pyarmor/project.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev1/pyarmor/pyshield.key
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/linux/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/darwin/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/windows/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/linux/x86/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/linux/x86_64/
--rwxr-xr-x  2.0 unx  1421600 b- defN 22-Sep-28 20:59 pyarmor-8.3.dev1/pyarmor/platforms/linux/x86/_pytransform.so
--rwxr-xr-x  2.0 unx  1198080 b- defN 22-Sep-28 20:59 pyarmor-8.3.dev1/pyarmor/platforms/linux/x86_64/_pytransform.so
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/darwin/x86_64/
--rwxr-xr-x  2.0 unx  1469620 b- defN 22-Sep-28 18:28 pyarmor-8.3.dev1/pyarmor/platforms/darwin/x86_64/_pytransform.dylib
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/windows/x86/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/platforms/windows/x86_64/
--rw-r--r--  2.0 unx  1373710 b- defN 22-Sep-28 21:00 pyarmor-8.3.dev1/pyarmor/platforms/windows/x86/_pytransform.dll
--rwxr-xr-x  2.0 unx  1165824 b- defN 22-Sep-28 20:59 pyarmor-8.3.dev1/pyarmor/platforms/windows/x86_64/_pytransform.dll
--rw-r--r--  2.0 unx     6360 b- defN 22-Jul-14 19:38 pyarmor-8.3.dev1/pyarmor/plugins/README.md
--rw-r--r--  2.0 unx    13688 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/plugins/check_ntp_time.py
--rw-r--r--  2.0 unx     7036 b- defN 23-Jun-21 23:40 pyarmor-8.3.dev1/pyarmor/cli/bootstrap.py
--rw-r--r--  2.0 unx     7184 b- defN 23-May-31 08:47 pyarmor-8.3.dev1/pyarmor/cli/merge.py
--rw-r--r--  2.0 unx    10726 b- defN 23-May-31 08:18 pyarmor-8.3.dev1/pyarmor/cli/config.py
--rw-r--r--  2.0 unx    18993 b- defN 23-Jul-23 15:37 pyarmor-8.3.dev1/pyarmor/cli/register.py
--rw-r--r--  2.0 unx     5835 b- defN 23-May-22 18:36 pyarmor-8.3.dev1/pyarmor/cli/generate.py
--rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor-8.3.dev1/pyarmor/cli/shell.py
--rw-r--r--  2.0 unx     7158 b- defN 23-May-07 11:39 pyarmor-8.3.dev1/pyarmor/cli/resource.py
--rw-r--r--  2.0 unx     1526 b- defN 23-Jul-19 09:21 pyarmor-8.3.dev1/pyarmor/cli/__init__.py
--rw-r--r--  2.0 unx     4594 b- defN 23-Jun-30 13:25 pyarmor-8.3.dev1/pyarmor/cli/docker.py
--rw-r--r--  2.0 unx    19470 b- defN 23-Jul-20 10:16 pyarmor-8.3.dev1/pyarmor/cli/context.py
--rw-r--r--  2.0 unx     3137 b- defN 23-Jun-25 16:00 pyarmor-8.3.dev1/pyarmor/cli/group.py
--rw-r--r--  2.0 unx     7718 b- defN 23-Jun-09 14:11 pyarmor-8.3.dev1/pyarmor/cli/plugin.py
--rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 15:02 pyarmor-8.3.dev1/pyarmor/cli/mixer.py
--rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor-8.3.dev1/pyarmor/cli/public_capsule.zip
--rw-r--r--  2.0 unx     9133 b- defN 23-Jul-20 10:08 pyarmor-8.3.dev1/pyarmor/cli/default.cfg
--rw-r--r--  2.0 unx    23065 b- defN 23-Jun-30 23:02 pyarmor-8.3.dev1/pyarmor/cli/__main__.py
--rw-r--r--  2.0 unx    16099 b- defN 23-Jun-21 23:40 pyarmor-8.3.dev1/pyarmor/cli/repack.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/helloworld/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/simple/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/pybench/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/testpkg/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/testmod/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/py2exe/
--rwxr-xr-x  2.0 unx     2048 b- defN 22-Mar-10 20:03 pyarmor-8.3.dev1/pyarmor/examples/obfuscate-pkg.bat
--rwxr-xr-x  2.0 unx     1645 b- defN 22-Mar-10 20:03 pyarmor-8.3.dev1/pyarmor/examples/obfuscate-app.bat
--rwxr-xr-x  2.0 unx     1103 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/obfuscate-app.sh
--rwxr-xr-x  2.0 unx     1685 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/obfuscate-pkg.sh
--rwxr-xr-x  2.0 unx     4102 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/build-with-project.bat
--rw-r--r--  2.0 unx     6876 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/README.md
--rwxr-xr-x  2.0 unx      773 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/pack-obfuscated-scripts.sh
--rwxr-xr-x  2.0 unx      928 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/pack-obfuscated-scripts.bat
--rwxr-xr-x  2.0 unx     3146 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/build-with-project.sh
--rwxr-xr-x  2.0 unx     4395 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/build-for-freeze.bat
--rw-r--r--  2.0 unx     7078 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/examples/README-ZH.md
--rwxr-xr-x  2.0 unx     4231 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/build-for-exe.bat
--rw-r--r--  2.0 unx     1747 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/helloworld/foo.py
--rwxr-xr-x  2.0 unx       49 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/hello.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/queens.py
--rwxr-xr-x  2.0 unx      641 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/setup.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/simple/queens.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/pybench/package/
--rwxr-xr-x  2.0 unx    13565 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Arithmetic.py
--rwxr-xr-x  2.0 unx     4134 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/With.py
--rwxr-xr-x  2.0 unx     6460 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Lists.py
--rwxr-xr-x  2.0 unx     8034 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Tuples.py
--rwxr-xr-x  2.0 unx     1388 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Instances.py
--rwxr-xr-x  2.0 unx     6672 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/systimes.py
--rwxr-xr-x  2.0 unx     1193 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/clockres.py
--rwxr-xr-x  2.0 unx    15254 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Lookups.py
--rwxr-xr-x  2.0 unx    16870 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/CommandLine.py
--rwxr-xr-x  2.0 unx    16198 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Numbers.py
--rwxr-xr-x  2.0 unx     2941 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Imports.py
--rwxr-xr-x  2.0 unx      961 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Setup.py
--rwxr-xr-x  2.0 unx    13400 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Exceptions.py
--rwxr-xr-x  2.0 unx     9261 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Dict.py
--rwxr-xr-x  2.0 unx    31828 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/pybench.py
--rwxr-xr-x  2.0 unx     1561 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/NewInstances.py
--rwxr-xr-x  2.0 unx     9252 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Calls.py
--rwxr-xr-x  2.0 unx    10946 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Strings.py
--rwxr-xr-x  2.0 unx    13207 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/Constructs.py
--rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/package/__init__.py
--rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/pybench/package/submodule.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor/examples/testpkg/mypkg/
--rw-r--r--  2.0 unx       66 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/testpkg/main.py
--rw-r--r--  2.0 unx      202 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/testpkg/mypkg/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/testpkg/mypkg/foo.py
--rwxr-xr-x  2.0 unx     1734 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/testmod/hello.py
--rwxr-xr-x  2.0 unx     3694 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/testmod/queens.py
--rwxr-xr-x  2.0 unx       44 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/py2exe/hello.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/py2exe/queens.py
--rwxr-xr-x  2.0 unx     1081 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/examples/py2exe/setup.py
--rw-r--r--  2.0 unx       28 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/polyfills/__init__.py
--rwxr-xr-x  2.0 unx    88440 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev1/pyarmor/polyfills/argparse.py
--rw-r--r--  2.0 unx     1505 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/helper/superuntime.py
--rw-r--r--  2.0 unx     9191 b- defN 22-Jan-06 22:40 pyarmor-8.3.dev1/pyarmor/helper/merge.py
--rw-r--r--  2.0 unx    11618 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/helper/buildext.py
--rw-r--r--  2.0 unx     2144 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/helper/get_platform_name.py
--rw-r--r--  2.0 unx      778 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/helper/get_license_info.py
--rw-r--r--  2.0 unx      728 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/helper/get_bind_key.py
--rw-r--r--  2.0 unx        1 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/helper/__init__.py
--rw-r--r--  2.0 unx     3821 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev1/pyarmor/helper/build_data_module.py
--rw-r--r--  2.0 unx    12719 b- defN 23-Mar-21 13:48 pyarmor-8.3.dev1/pyarmor/helper/repack.py
--rw-r--r--  2.0 unx     3004 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     3450 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      174 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-23 20:58 pyarmor-8.3.dev1/pyarmor.egg-info/dependency_links.txt
-143 files, 7442858 bytes uncompressed, 2306968 bytes compressed:  69.0%
+Zip file size: 2706172 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor.egg-info/
+-rw-r--r--  2.0 unx     3004 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/PKG-INFO
+-rwxr-xr-x  2.0 unx      191 b- defN 23-Mar-04 11:58 pyarmor-8.3.dev2/MANIFEST.in
+-rw-r--r--  2.0 unx     6553 b- defN 23-May-11 12:30 pyarmor-8.3.dev2/README.md
+-rw-r--r--  2.0 unx     4364 b- defN 23-Jul-29 08:15 pyarmor-8.3.dev2/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/setup.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/plugins/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/polyfills/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/helper/
+-rw-r--r--  2.0 unx      234 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev2/pyarmor/pyshield.lic
+-rwxr-xr-x  2.0 unx     2038 b- defN 23-Jul-29 08:15 pyarmor-8.3.dev2/pyarmor/config.py
+-rwxr-xr-x  2.0 unx    10197 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/benchmark.py
+-rw-r--r--  2.0 unx     6994 b- defN 23-May-12 06:32 pyarmor-8.3.dev2/pyarmor/register.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev2/pyarmor/product.key
+-rwxr-xr-x  2.0 unx    65827 b- defN 23-Mar-26 00:20 pyarmor-8.3.dev2/pyarmor/pyarmor.py
+-rw-r--r--  2.0 unx     2664 b- defN 22-Jan-29 09:20 pyarmor-8.3.dev2/pyarmor/protect_code.pt
+-rw-r--r--  2.0 unx    13587 b- defN 21-Nov-02 17:34 pyarmor-8.3.dev2/pyarmor/pytransform.py
+-rw-r--r--  2.0 unx     3363 b- defN 22-Jun-27 00:08 pyarmor-8.3.dev2/pyarmor/sppmode.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev2/pyarmor/public.key
+-rwxr-xr-x  2.0 unx      113 b- defN 20-Jan-02 11:09 pyarmor-8.3.dev2/pyarmor/__init__.py
+-rw-r--r--  2.0 unx     2191 b- defN 22-Dec-04 19:13 pyarmor-8.3.dev2/pyarmor/reform.py
+-rwxr-xr-x  2.0 unx    25832 b- defN 22-Nov-20 13:42 pyarmor-8.3.dev2/pyarmor/packer.py
+-rw-r--r--  2.0 unx     5200 b- defN 23-Jan-06 00:02 pyarmor-8.3.dev2/pyarmor/cobuilder.py
+-rwxr-xr-x  2.0 unx    67431 b- defN 22-Dec-23 17:42 pyarmor-8.3.dev2/pyarmor/utils.py
+-rw-r--r--  2.0 unx       37 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/pyarmor-webui.py
+-rwxr-xr-x  2.0 unx    28176 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/pyarmor-deprecated.py
+-rw-r--r--  2.0 unx     4028 b- defN 21-Dec-16 08:28 pyarmor-8.3.dev2/pyarmor/build_meta.py
+-rw-r--r--  2.0 unx      256 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev2/pyarmor/license.tri
+-rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor-8.3.dev2/pyarmor/README.rst
+-rw-r--r--  2.0 unx     1596 b- defN 22-Jan-30 11:51 pyarmor-8.3.dev2/pyarmor/protect_code2.pt
+-rw-r--r--  2.0 unx     2234 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/pyimcore.py
+-rw-r--r--  2.0 unx     2487 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev2/pyarmor/public_capsule.zip
+-rwxr-xr-x  2.0 unx     8023 b- defN 22-Jun-28 09:01 pyarmor-8.3.dev2/pyarmor/project.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.3.dev2/pyarmor/pyshield.key
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/linux/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/darwin/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/windows/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/linux/x86/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/linux/x86_64/
+-rwxr-xr-x  2.0 unx  1421600 b- defN 22-Sep-28 20:59 pyarmor-8.3.dev2/pyarmor/platforms/linux/x86/_pytransform.so
+-rwxr-xr-x  2.0 unx  1198080 b- defN 22-Sep-28 20:59 pyarmor-8.3.dev2/pyarmor/platforms/linux/x86_64/_pytransform.so
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/darwin/x86_64/
+-rwxr-xr-x  2.0 unx  1469620 b- defN 22-Sep-28 18:28 pyarmor-8.3.dev2/pyarmor/platforms/darwin/x86_64/_pytransform.dylib
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/windows/x86/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/platforms/windows/x86_64/
+-rw-r--r--  2.0 unx  1373710 b- defN 22-Sep-28 21:00 pyarmor-8.3.dev2/pyarmor/platforms/windows/x86/_pytransform.dll
+-rwxr-xr-x  2.0 unx  1165824 b- defN 22-Sep-28 20:59 pyarmor-8.3.dev2/pyarmor/platforms/windows/x86_64/_pytransform.dll
+-rw-r--r--  2.0 unx     6360 b- defN 22-Jul-14 19:38 pyarmor-8.3.dev2/pyarmor/plugins/README.md
+-rw-r--r--  2.0 unx    13688 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/plugins/check_ntp_time.py
+-rw-r--r--  2.0 unx     7036 b- defN 23-Jun-21 23:40 pyarmor-8.3.dev2/pyarmor/cli/bootstrap.py
+-rw-r--r--  2.0 unx     7184 b- defN 23-May-31 08:47 pyarmor-8.3.dev2/pyarmor/cli/merge.py
+-rw-r--r--  2.0 unx   132120 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/cli/core.data.2
+-rw-r--r--  2.0 unx    10726 b- defN 23-May-31 08:18 pyarmor-8.3.dev2/pyarmor/cli/config.py
+-rw-r--r--  2.0 unx    55974 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/cli/core.data.3
+-rw-r--r--  2.0 unx    18993 b- defN 23-Jul-23 15:37 pyarmor-8.3.dev2/pyarmor/cli/register.py
+-rw-r--r--  2.0 unx     5835 b- defN 23-May-22 18:36 pyarmor-8.3.dev2/pyarmor/cli/generate.py
+-rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor-8.3.dev2/pyarmor/cli/shell.py
+-rw-r--r--  2.0 unx     7158 b- defN 23-May-07 11:39 pyarmor-8.3.dev2/pyarmor/cli/resource.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Jul-30 16:59 pyarmor-8.3.dev2/pyarmor/cli/__init__.py
+-rw-r--r--  2.0 unx     4594 b- defN 23-Jun-30 13:25 pyarmor-8.3.dev2/pyarmor/cli/docker.py
+-rw-r--r--  2.0 unx    19926 b- defN 23-Jul-28 17:10 pyarmor-8.3.dev2/pyarmor/cli/context.py
+-rw-r--r--  2.0 unx   186837 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/cli/core.data.1
+-rw-r--r--  2.0 unx     3137 b- defN 23-Jun-25 16:00 pyarmor-8.3.dev2/pyarmor/cli/group.py
+-rw-r--r--  2.0 unx     7718 b- defN 23-Jun-09 14:11 pyarmor-8.3.dev2/pyarmor/cli/plugin.py
+-rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 15:02 pyarmor-8.3.dev2/pyarmor/cli/mixer.py
+-rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor-8.3.dev2/pyarmor/cli/public_capsule.zip
+-rw-r--r--  2.0 unx     9190 b- defN 23-Jul-29 08:15 pyarmor-8.3.dev2/pyarmor/cli/default.cfg
+-rw-r--r--  2.0 unx    23065 b- defN 23-Jun-30 23:02 pyarmor-8.3.dev2/pyarmor/cli/__main__.py
+-rw-r--r--  2.0 unx    16099 b- defN 23-Jun-21 23:40 pyarmor-8.3.dev2/pyarmor/cli/repack.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/helloworld/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/simple/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/pybench/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/testpkg/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/testmod/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/py2exe/
+-rwxr-xr-x  2.0 unx     2048 b- defN 22-Mar-10 20:03 pyarmor-8.3.dev2/pyarmor/examples/obfuscate-pkg.bat
+-rwxr-xr-x  2.0 unx     1645 b- defN 22-Mar-10 20:03 pyarmor-8.3.dev2/pyarmor/examples/obfuscate-app.bat
+-rwxr-xr-x  2.0 unx     1103 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/obfuscate-app.sh
+-rwxr-xr-x  2.0 unx     1685 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/obfuscate-pkg.sh
+-rwxr-xr-x  2.0 unx     4102 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/build-with-project.bat
+-rw-r--r--  2.0 unx     6876 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/README.md
+-rwxr-xr-x  2.0 unx      773 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/pack-obfuscated-scripts.sh
+-rwxr-xr-x  2.0 unx      928 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/pack-obfuscated-scripts.bat
+-rwxr-xr-x  2.0 unx     3146 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/build-with-project.sh
+-rwxr-xr-x  2.0 unx     4395 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/build-for-freeze.bat
+-rw-r--r--  2.0 unx     7078 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/examples/README-ZH.md
+-rwxr-xr-x  2.0 unx     4231 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/build-for-exe.bat
+-rw-r--r--  2.0 unx     1747 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/helloworld/foo.py
+-rwxr-xr-x  2.0 unx       49 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/hello.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/queens.py
+-rwxr-xr-x  2.0 unx      641 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/setup.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/simple/queens.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/pybench/package/
+-rwxr-xr-x  2.0 unx    13565 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Arithmetic.py
+-rwxr-xr-x  2.0 unx     4134 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/With.py
+-rwxr-xr-x  2.0 unx     6460 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Lists.py
+-rwxr-xr-x  2.0 unx     8034 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Tuples.py
+-rwxr-xr-x  2.0 unx     1388 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Instances.py
+-rwxr-xr-x  2.0 unx     6672 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/systimes.py
+-rwxr-xr-x  2.0 unx     1193 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/clockres.py
+-rwxr-xr-x  2.0 unx    15254 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Lookups.py
+-rwxr-xr-x  2.0 unx    16870 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/CommandLine.py
+-rwxr-xr-x  2.0 unx    16198 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Numbers.py
+-rwxr-xr-x  2.0 unx     2941 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Imports.py
+-rwxr-xr-x  2.0 unx      961 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Setup.py
+-rwxr-xr-x  2.0 unx    13400 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Exceptions.py
+-rwxr-xr-x  2.0 unx     9261 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Dict.py
+-rwxr-xr-x  2.0 unx    31828 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/pybench.py
+-rwxr-xr-x  2.0 unx     1561 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/NewInstances.py
+-rwxr-xr-x  2.0 unx     9252 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Calls.py
+-rwxr-xr-x  2.0 unx    10946 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Strings.py
+-rwxr-xr-x  2.0 unx    13207 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/Constructs.py
+-rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/package/__init__.py
+-rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/pybench/package/submodule.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor/examples/testpkg/mypkg/
+-rw-r--r--  2.0 unx       66 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/testpkg/main.py
+-rw-r--r--  2.0 unx      202 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/testpkg/mypkg/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/testpkg/mypkg/foo.py
+-rwxr-xr-x  2.0 unx     1734 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/testmod/hello.py
+-rwxr-xr-x  2.0 unx     3694 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/testmod/queens.py
+-rwxr-xr-x  2.0 unx       44 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/py2exe/hello.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/py2exe/queens.py
+-rwxr-xr-x  2.0 unx     1081 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/examples/py2exe/setup.py
+-rw-r--r--  2.0 unx       28 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/polyfills/__init__.py
+-rwxr-xr-x  2.0 unx    88440 b- defN 19-Dec-05 18:38 pyarmor-8.3.dev2/pyarmor/polyfills/argparse.py
+-rw-r--r--  2.0 unx     1505 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/helper/superuntime.py
+-rw-r--r--  2.0 unx     9191 b- defN 22-Jan-06 22:40 pyarmor-8.3.dev2/pyarmor/helper/merge.py
+-rw-r--r--  2.0 unx    11618 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/helper/buildext.py
+-rw-r--r--  2.0 unx     2144 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/helper/get_platform_name.py
+-rw-r--r--  2.0 unx      778 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/helper/get_license_info.py
+-rw-r--r--  2.0 unx      728 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/helper/get_bind_key.py
+-rw-r--r--  2.0 unx        1 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/helper/__init__.py
+-rw-r--r--  2.0 unx     3821 b- defN 21-Oct-13 13:01 pyarmor-8.3.dev2/pyarmor/helper/build_data_module.py
+-rw-r--r--  2.0 unx    12719 b- defN 23-Mar-21 13:48 pyarmor-8.3.dev2/pyarmor/helper/repack.py
+-rw-r--r--  2.0 unx     3004 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     3522 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 18:12 pyarmor-8.3.dev2/pyarmor.egg-info/dependency_links.txt
+146 files, 7818013 bytes uncompressed, 2682062 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,430 +1,439 @@
-Filename: pyarmor-8.3.dev1/
+Filename: pyarmor-8.3.dev2/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/
+Filename: pyarmor-8.3.dev2/pyarmor/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor.egg-info/
+Filename: pyarmor-8.3.dev2/pyarmor.egg-info/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/PKG-INFO
+Filename: pyarmor-8.3.dev2/PKG-INFO
 Comment: 
 
-Filename: pyarmor-8.3.dev1/MANIFEST.in
+Filename: pyarmor-8.3.dev2/MANIFEST.in
 Comment: 
 
-Filename: pyarmor-8.3.dev1/README.md
+Filename: pyarmor-8.3.dev2/README.md
 Comment: 
 
-Filename: pyarmor-8.3.dev1/setup.py
+Filename: pyarmor-8.3.dev2/setup.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/setup.cfg
+Filename: pyarmor-8.3.dev2/setup.cfg
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/plugins/
+Filename: pyarmor-8.3.dev2/pyarmor/plugins/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/
+Filename: pyarmor-8.3.dev2/pyarmor/cli/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/
+Filename: pyarmor-8.3.dev2/pyarmor/examples/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/polyfills/
+Filename: pyarmor-8.3.dev2/pyarmor/polyfills/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/
+Filename: pyarmor-8.3.dev2/pyarmor/helper/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/pyshield.lic
+Filename: pyarmor-8.3.dev2/pyarmor/pyshield.lic
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/config.py
+Filename: pyarmor-8.3.dev2/pyarmor/config.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/benchmark.py
+Filename: pyarmor-8.3.dev2/pyarmor/benchmark.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/register.py
+Filename: pyarmor-8.3.dev2/pyarmor/register.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/product.key
+Filename: pyarmor-8.3.dev2/pyarmor/product.key
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/pyarmor.py
+Filename: pyarmor-8.3.dev2/pyarmor/pyarmor.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/protect_code.pt
+Filename: pyarmor-8.3.dev2/pyarmor/protect_code.pt
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/pytransform.py
+Filename: pyarmor-8.3.dev2/pyarmor/pytransform.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/sppmode.py
+Filename: pyarmor-8.3.dev2/pyarmor/sppmode.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/public.key
+Filename: pyarmor-8.3.dev2/pyarmor/public.key
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/__init__.py
+Filename: pyarmor-8.3.dev2/pyarmor/__init__.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/reform.py
+Filename: pyarmor-8.3.dev2/pyarmor/reform.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/packer.py
+Filename: pyarmor-8.3.dev2/pyarmor/packer.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cobuilder.py
+Filename: pyarmor-8.3.dev2/pyarmor/cobuilder.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/utils.py
+Filename: pyarmor-8.3.dev2/pyarmor/utils.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/pyarmor-webui.py
+Filename: pyarmor-8.3.dev2/pyarmor/pyarmor-webui.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/pyarmor-deprecated.py
+Filename: pyarmor-8.3.dev2/pyarmor/pyarmor-deprecated.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/build_meta.py
+Filename: pyarmor-8.3.dev2/pyarmor/build_meta.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/license.tri
+Filename: pyarmor-8.3.dev2/pyarmor/license.tri
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/README.rst
+Filename: pyarmor-8.3.dev2/pyarmor/README.rst
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/protect_code2.pt
+Filename: pyarmor-8.3.dev2/pyarmor/protect_code2.pt
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/pyimcore.py
+Filename: pyarmor-8.3.dev2/pyarmor/pyimcore.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/public_capsule.zip
+Filename: pyarmor-8.3.dev2/pyarmor/public_capsule.zip
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/project.py
+Filename: pyarmor-8.3.dev2/pyarmor/project.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/pyshield.key
+Filename: pyarmor-8.3.dev2/pyarmor/pyshield.key
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/linux/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/linux/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/darwin/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/darwin/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/windows/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/windows/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/linux/x86/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/linux/x86/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/linux/x86_64/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/linux/x86_64/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/linux/x86/_pytransform.so
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/linux/x86/_pytransform.so
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/linux/x86_64/_pytransform.so
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/linux/x86_64/_pytransform.so
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/darwin/x86_64/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/darwin/x86_64/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/darwin/x86_64/_pytransform.dylib
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/darwin/x86_64/_pytransform.dylib
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/windows/x86/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/windows/x86/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/windows/x86_64/
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/windows/x86_64/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/windows/x86/_pytransform.dll
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/windows/x86/_pytransform.dll
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/platforms/windows/x86_64/_pytransform.dll
+Filename: pyarmor-8.3.dev2/pyarmor/platforms/windows/x86_64/_pytransform.dll
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/plugins/README.md
+Filename: pyarmor-8.3.dev2/pyarmor/plugins/README.md
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/plugins/check_ntp_time.py
+Filename: pyarmor-8.3.dev2/pyarmor/plugins/check_ntp_time.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/bootstrap.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/bootstrap.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/merge.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/merge.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/config.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/core.data.2
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/register.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/config.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/generate.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/core.data.3
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/shell.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/register.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/resource.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/generate.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/__init__.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/shell.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/docker.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/resource.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/context.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/__init__.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/group.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/docker.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/plugin.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/context.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/mixer.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/core.data.1
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/public_capsule.zip
+Filename: pyarmor-8.3.dev2/pyarmor/cli/group.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/default.cfg
+Filename: pyarmor-8.3.dev2/pyarmor/cli/plugin.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/__main__.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/mixer.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/cli/repack.py
+Filename: pyarmor-8.3.dev2/pyarmor/cli/public_capsule.zip
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/helloworld/
+Filename: pyarmor-8.3.dev2/pyarmor/cli/default.cfg
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/
+Filename: pyarmor-8.3.dev2/pyarmor/cli/__main__.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/simple/
+Filename: pyarmor-8.3.dev2/pyarmor/cli/repack.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/
+Filename: pyarmor-8.3.dev2/pyarmor/examples/helloworld/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testpkg/
+Filename: pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testmod/
+Filename: pyarmor-8.3.dev2/pyarmor/examples/simple/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/py2exe/
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/obfuscate-pkg.bat
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testpkg/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/obfuscate-app.bat
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testmod/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/obfuscate-app.sh
+Filename: pyarmor-8.3.dev2/pyarmor/examples/py2exe/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/obfuscate-pkg.sh
+Filename: pyarmor-8.3.dev2/pyarmor/examples/obfuscate-pkg.bat
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/build-with-project.bat
+Filename: pyarmor-8.3.dev2/pyarmor/examples/obfuscate-app.bat
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/README.md
+Filename: pyarmor-8.3.dev2/pyarmor/examples/obfuscate-app.sh
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pack-obfuscated-scripts.sh
+Filename: pyarmor-8.3.dev2/pyarmor/examples/obfuscate-pkg.sh
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pack-obfuscated-scripts.bat
+Filename: pyarmor-8.3.dev2/pyarmor/examples/build-with-project.bat
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/build-with-project.sh
+Filename: pyarmor-8.3.dev2/pyarmor/examples/README.md
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/build-for-freeze.bat
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pack-obfuscated-scripts.sh
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/README-ZH.md
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pack-obfuscated-scripts.bat
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/build-for-exe.bat
+Filename: pyarmor-8.3.dev2/pyarmor/examples/build-with-project.sh
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/helloworld/foo.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/build-for-freeze.bat
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/hello.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/README-ZH.md
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/queens.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/build-for-exe.bat
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/setup.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/helloworld/foo.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/simple/queens.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/hello.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/package/
+Filename: pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/queens.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Arithmetic.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/setup.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/With.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/simple/queens.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Lists.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/package/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Tuples.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Arithmetic.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Instances.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/With.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/systimes.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Lists.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/clockres.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Tuples.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Lookups.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Instances.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/CommandLine.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/systimes.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Numbers.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/clockres.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Imports.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Lookups.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Setup.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/CommandLine.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Exceptions.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Numbers.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Dict.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Imports.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/pybench.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Setup.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/NewInstances.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Exceptions.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Calls.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Dict.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Strings.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/pybench.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/Constructs.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/NewInstances.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/package/__init__.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Calls.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/pybench/package/submodule.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Strings.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testpkg/mypkg/
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/Constructs.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testpkg/main.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/package/__init__.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testpkg/mypkg/__init__.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/pybench/package/submodule.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testpkg/mypkg/foo.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testpkg/mypkg/
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testmod/hello.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testpkg/main.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/testmod/queens.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testpkg/mypkg/__init__.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/py2exe/hello.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testpkg/mypkg/foo.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/py2exe/queens.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testmod/hello.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/examples/py2exe/setup.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/testmod/queens.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/polyfills/__init__.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/py2exe/hello.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/polyfills/argparse.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/py2exe/queens.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/superuntime.py
+Filename: pyarmor-8.3.dev2/pyarmor/examples/py2exe/setup.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/merge.py
+Filename: pyarmor-8.3.dev2/pyarmor/polyfills/__init__.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/buildext.py
+Filename: pyarmor-8.3.dev2/pyarmor/polyfills/argparse.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/get_platform_name.py
+Filename: pyarmor-8.3.dev2/pyarmor/helper/superuntime.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/get_license_info.py
+Filename: pyarmor-8.3.dev2/pyarmor/helper/merge.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/get_bind_key.py
+Filename: pyarmor-8.3.dev2/pyarmor/helper/buildext.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/__init__.py
+Filename: pyarmor-8.3.dev2/pyarmor/helper/get_platform_name.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/build_data_module.py
+Filename: pyarmor-8.3.dev2/pyarmor/helper/get_license_info.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor/helper/repack.py
+Filename: pyarmor-8.3.dev2/pyarmor/helper/get_bind_key.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor.egg-info/PKG-INFO
+Filename: pyarmor-8.3.dev2/pyarmor/helper/__init__.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor.egg-info/SOURCES.txt
+Filename: pyarmor-8.3.dev2/pyarmor/helper/build_data_module.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor.egg-info/entry_points.txt
+Filename: pyarmor-8.3.dev2/pyarmor/helper/repack.py
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor.egg-info/requires.txt
+Filename: pyarmor-8.3.dev2/pyarmor.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor.egg-info/top_level.txt
+Filename: pyarmor-8.3.dev2/pyarmor.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor-8.3.dev1/pyarmor.egg-info/dependency_links.txt
+Filename: pyarmor-8.3.dev2/pyarmor.egg-info/entry_points.txt
+Comment: 
+
+Filename: pyarmor-8.3.dev2/pyarmor.egg-info/requires.txt
+Comment: 
+
+Filename: pyarmor-8.3.dev2/pyarmor.egg-info/top_level.txt
+Comment: 
+
+Filename: pyarmor-8.3.dev2/pyarmor.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor-8.3.dev1/PKG-INFO` & `pyarmor-8.3.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor
-Version: 8.3.dev1
+Version: 8.3.dev2
 Summary: A tool used to obfuscate python scripts, bind obfuscated scripts to fixed machine or expire obfuscated scripts.
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor-8.3.dev1/README.md` & `pyarmor-8.3.dev2/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/setup.py` & `pyarmor-8.3.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,19 +105,19 @@
     # Note that this is a string of words separated by whitespace, not a list.
     keywords='protect obfuscate encrypt obfuscation distribute',
 
     packages=['pyarmor', 'pyarmor.polyfills', 'pyarmor.helper', 'pyarmor.cli'],
     package_dir={'pyarmor': 'pyarmor'},
     package_data={
         'pyarmor': pyarmor_data_files + platform_data_files,
-        'pyarmor.cli': ['default.cfg', 'public_capsule.zip'],
+        'pyarmor.cli': ['default.cfg', 'public_capsule.zip', 'core.data.*'],
     },
 
     install_requires=[
-        'pyarmor.cli.core~=4.3.dev1'
+        'pyarmor.cli.core~=4.3.0'
     ],
 
     entry_points={
         'console_scripts': [
             'pyarmor=pyarmor.pyarmor:main_entry_8',
             'pyarmor-auth=pyarmor.cli.docker:main',
             'pyarmor-7=pyarmor.pyarmor:main_entry',
```

## Comparing `pyarmor-8.3.dev1/pyarmor/config.py` & `pyarmor-8.3.dev2/pyarmor/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sys import platform
 
-version = '8.3.dev1'
+version = '8.3.dev2'
 
 # The corresponding version of pytransform.so
 core_version = 'r52.6'
 
 version_info = '''
 PyArmor is a command line tool used to obfuscate python scripts, bind
 obfuscated scripts to fixed machine or expire obfuscated scripts.
```

## Comparing `pyarmor-8.3.dev1/pyarmor/benchmark.py` & `pyarmor-8.3.dev2/pyarmor/benchmark.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/register.py` & `pyarmor-8.3.dev2/pyarmor/register.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/pyarmor.py` & `pyarmor-8.3.dev2/pyarmor/pyarmor.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/protect_code.pt` & `pyarmor-8.3.dev2/pyarmor/protect_code.pt`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/pytransform.py` & `pyarmor-8.3.dev2/pyarmor/pytransform.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/sppmode.py` & `pyarmor-8.3.dev2/pyarmor/sppmode.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/reform.py` & `pyarmor-8.3.dev2/pyarmor/reform.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/packer.py` & `pyarmor-8.3.dev2/pyarmor/packer.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cobuilder.py` & `pyarmor-8.3.dev2/pyarmor/cobuilder.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/utils.py` & `pyarmor-8.3.dev2/pyarmor/utils.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/pyarmor-deprecated.py` & `pyarmor-8.3.dev2/pyarmor/pyarmor-deprecated.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/build_meta.py` & `pyarmor-8.3.dev2/pyarmor/build_meta.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/README.rst` & `pyarmor-8.3.dev2/pyarmor/README.rst`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/protect_code2.pt` & `pyarmor-8.3.dev2/pyarmor/protect_code2.pt`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/pyimcore.py` & `pyarmor-8.3.dev2/pyarmor/pyimcore.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/public_capsule.zip` & `pyarmor-8.3.dev2/pyarmor/public_capsule.zip`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/project.py` & `pyarmor-8.3.dev2/pyarmor/project.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/platforms/linux/x86/_pytransform.so` & `pyarmor-8.3.dev2/pyarmor/platforms/linux/x86/_pytransform.so`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/platforms/linux/x86_64/_pytransform.so` & `pyarmor-8.3.dev2/pyarmor/platforms/linux/x86_64/_pytransform.so`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/platforms/darwin/x86_64/_pytransform.dylib` & `pyarmor-8.3.dev2/pyarmor/platforms/darwin/x86_64/_pytransform.dylib`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/platforms/windows/x86/_pytransform.dll` & `pyarmor-8.3.dev2/pyarmor/platforms/windows/x86/_pytransform.dll`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/platforms/windows/x86_64/_pytransform.dll` & `pyarmor-8.3.dev2/pyarmor/platforms/windows/x86_64/_pytransform.dll`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/plugins/README.md` & `pyarmor-8.3.dev2/pyarmor/plugins/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/plugins/check_ntp_time.py` & `pyarmor-8.3.dev2/pyarmor/plugins/check_ntp_time.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/bootstrap.py` & `pyarmor-8.3.dev2/pyarmor/cli/bootstrap.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/merge.py` & `pyarmor-8.3.dev2/pyarmor/cli/merge.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/config.py` & `pyarmor-8.3.dev2/pyarmor/cli/config.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/register.py` & `pyarmor-8.3.dev2/pyarmor/cli/register.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/generate.py` & `pyarmor-8.3.dev2/pyarmor/cli/generate.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/shell.py` & `pyarmor-8.3.dev2/pyarmor/cli/shell.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/resource.py` & `pyarmor-8.3.dev2/pyarmor/cli/resource.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/docker.py` & `pyarmor-8.3.dev2/pyarmor/cli/docker.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/context.py` & `pyarmor-8.3.dev2/pyarmor/cli/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -637,7 +637,27 @@
                 with open(filename, encoding=encoding) as f:
                     return f.read()
 
     def runtime_plugin(self, source, target, platforms):
         for plugin in self.plugins:
             if hasattr(plugin, 'post_runtime'):
                 plugin.post_runtime(self, source, target, platforms)
+
+    #
+    # Core data, new in 8.3
+    #
+    def _core_data(self, name):
+        n = __file__.find('context.py')
+        with open(__file__[:n] + name, 'rb') as f:
+            return f.read()
+
+    @property
+    def core_data_1(self):
+        return self._core_data('core.data.1')
+
+    @property
+    def core_data_2(self):
+        return self._core_data('core.data.2')
+
+    @property
+    def core_data_3(self):
+        return self._core_data('core.data.3')
```

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/group.py` & `pyarmor-8.3.dev2/pyarmor/cli/group.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/plugin.py` & `pyarmor-8.3.dev2/pyarmor/cli/plugin.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/mixer.py` & `pyarmor-8.3.dev2/pyarmor/cli/mixer.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/public_capsule.zip` & `pyarmor-8.3.dev2/pyarmor/cli/public_capsule.zip`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/default.cfg` & `pyarmor-8.3.dev2/pyarmor/cli/default.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [pyarmor]
 
 ;; Pyarmor version
 major = 8
 minor = 3
-patch = dev1
+patch = dev2
 
 ;; Core version
-cli.core = 4.3.dev1
+cli.core = 4.3.0
 
 ;; Deprecated since Pyarmor 8.2.5
 ; cli.runtime = 3.2.5
 
 ;; Default timeout when send request to remote server for
 ;;     check Pyarmor license
 ;;     register Pyarmor license
@@ -323,15 +323,15 @@
 cc = clang.exe
 cflags = --target=i686-elf-linux -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -mno-sse -std=c99 -c
 
 [linux.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [linux.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -DENABLE_BCC_MEMSET -Tlinux.aarch64.ldscript
 
 [linux.x86.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -c
 
 [linux.armv7.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -shared -nostdlib -Tlinux.armv7.ldscript
 
@@ -341,23 +341,23 @@
 [darwin.aarch64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem
 
 [android.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [android.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -DENABLE_BCC_MEMSET -Tlinux.aarch64.ldscript
 
 [android.x86.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -c
 
 [android.armv7.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -shared -nostdlib -Tlinux.armv7.ldscript
 
 [alpine.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [alpine.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -DENABLE_BCC_MEMSET -Tlinux.aarch64.ldscript
 
 [freebsd.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
```

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/__main__.py` & `pyarmor-8.3.dev2/pyarmor/cli/__main__.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/cli/repack.py` & `pyarmor-8.3.dev2/pyarmor/cli/repack.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/obfuscate-pkg.bat` & `pyarmor-8.3.dev2/pyarmor/examples/obfuscate-pkg.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/obfuscate-app.bat` & `pyarmor-8.3.dev2/pyarmor/examples/obfuscate-app.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/obfuscate-app.sh` & `pyarmor-8.3.dev2/pyarmor/examples/obfuscate-app.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/obfuscate-pkg.sh` & `pyarmor-8.3.dev2/pyarmor/examples/obfuscate-pkg.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/build-with-project.bat` & `pyarmor-8.3.dev2/pyarmor/examples/build-with-project.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/README.md` & `pyarmor-8.3.dev2/pyarmor/examples/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pack-obfuscated-scripts.sh` & `pyarmor-8.3.dev2/pyarmor/examples/pack-obfuscated-scripts.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pack-obfuscated-scripts.bat` & `pyarmor-8.3.dev2/pyarmor/examples/pack-obfuscated-scripts.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/build-with-project.sh` & `pyarmor-8.3.dev2/pyarmor/examples/build-with-project.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/build-for-freeze.bat` & `pyarmor-8.3.dev2/pyarmor/examples/build-for-freeze.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/README-ZH.md` & `pyarmor-8.3.dev2/pyarmor/examples/README-ZH.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/build-for-exe.bat` & `pyarmor-8.3.dev2/pyarmor/examples/build-for-exe.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/helloworld/foo.py` & `pyarmor-8.3.dev2/pyarmor/examples/helloworld/foo.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/queens.py` & `pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/cx_Freeze/setup.py` & `pyarmor-8.3.dev2/pyarmor/examples/cx_Freeze/setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/simple/queens.py` & `pyarmor-8.3.dev2/pyarmor/examples/simple/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Arithmetic.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Arithmetic.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/With.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/With.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Lists.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Lists.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Tuples.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Tuples.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Instances.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Instances.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/systimes.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/systimes.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/clockres.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/clockres.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Lookups.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Lookups.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/CommandLine.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/CommandLine.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Numbers.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Numbers.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Imports.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Imports.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Setup.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Exceptions.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Exceptions.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Dict.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Dict.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/pybench.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/pybench.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/NewInstances.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/NewInstances.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Calls.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Calls.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Strings.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Strings.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/pybench/Constructs.py` & `pyarmor-8.3.dev2/pyarmor/examples/pybench/Constructs.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/testmod/hello.py` & `pyarmor-8.3.dev2/pyarmor/examples/testmod/hello.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/testmod/queens.py` & `pyarmor-8.3.dev2/pyarmor/examples/testmod/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/py2exe/queens.py` & `pyarmor-8.3.dev2/pyarmor/examples/py2exe/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/examples/py2exe/setup.py` & `pyarmor-8.3.dev2/pyarmor/examples/py2exe/setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/polyfills/argparse.py` & `pyarmor-8.3.dev2/pyarmor/polyfills/argparse.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/superuntime.py` & `pyarmor-8.3.dev2/pyarmor/helper/superuntime.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/merge.py` & `pyarmor-8.3.dev2/pyarmor/helper/merge.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/buildext.py` & `pyarmor-8.3.dev2/pyarmor/helper/buildext.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/get_platform_name.py` & `pyarmor-8.3.dev2/pyarmor/helper/get_platform_name.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/get_license_info.py` & `pyarmor-8.3.dev2/pyarmor/helper/get_license_info.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/get_bind_key.py` & `pyarmor-8.3.dev2/pyarmor/helper/get_bind_key.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/build_data_module.py` & `pyarmor-8.3.dev2/pyarmor/helper/build_data_module.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor/helper/repack.py` & `pyarmor-8.3.dev2/pyarmor/helper/repack.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.3.dev1/pyarmor.egg-info/PKG-INFO` & `pyarmor-8.3.dev2/pyarmor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor
-Version: 8.3.dev1
+Version: 8.3.dev2
 Summary: A tool used to obfuscate python scripts, bind obfuscated scripts to fixed machine or expire obfuscated scripts.
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor-8.3.dev1/pyarmor.egg-info/SOURCES.txt` & `pyarmor-8.3.dev2/pyarmor.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 pyarmor.egg-info/requires.txt
 pyarmor.egg-info/top_level.txt
 pyarmor/cli/__init__.py
 pyarmor/cli/__main__.py
 pyarmor/cli/bootstrap.py
 pyarmor/cli/config.py
 pyarmor/cli/context.py
+pyarmor/cli/core.data.1
+pyarmor/cli/core.data.2
+pyarmor/cli/core.data.3
 pyarmor/cli/default.cfg
 pyarmor/cli/docker.py
 pyarmor/cli/generate.py
 pyarmor/cli/group.py
 pyarmor/cli/merge.py
 pyarmor/cli/mixer.py
 pyarmor/cli/plugin.py
```

