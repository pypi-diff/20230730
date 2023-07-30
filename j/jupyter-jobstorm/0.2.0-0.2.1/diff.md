# Comparing `tmp/jupyter_jobstorm-0.2.0-py3-none-any.whl.zip` & `tmp/jupyter_jobstorm-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7267 bytes, number of entries: 8
--rw-r--r--  2.0 unx      143 b- defN 23-Jul-16 02:44 jobstorm/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-16 02:44 jobstorm/_version.py
--rw-r--r--  2.0 unx    18845 b- defN 23-Jul-16 02:44 jobstorm/jobcode.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2653 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      658 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/RECORD
-8 files, 23498 bytes uncompressed, 6111 bytes compressed:  74.0%
+Zip file size: 7870 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      143 b- defN 23-Jul-30 04:51 jobstorm/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-30 04:51 jobstorm/_version.py
+-rw-r--r--  2.0 unx    22199 b- defN 23-Jul-30 04:51 jobstorm/jobcode.py
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jul-30 04:51 jupyter_jobstorm-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2653 b- defN 23-Jul-30 04:51 jupyter_jobstorm-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 04:51 jupyter_jobstorm-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-30 04:51 jupyter_jobstorm-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-Jul-30 04:51 jupyter_jobstorm-0.2.1.dist-info/RECORD
+8 files, 26852 bytes uncompressed, 6714 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: jobstorm/_version.py
 Comment: 
 
 Filename: jobstorm/jobcode.py
 Comment: 
 
-Filename: jupyter_jobstorm-0.2.0.dist-info/LICENSE
+Filename: jupyter_jobstorm-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: jupyter_jobstorm-0.2.0.dist-info/METADATA
+Filename: jupyter_jobstorm-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: jupyter_jobstorm-0.2.0.dist-info/WHEEL
+Filename: jupyter_jobstorm-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: jupyter_jobstorm-0.2.0.dist-info/top_level.txt
+Filename: jupyter_jobstorm-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jupyter_jobstorm-0.2.0.dist-info/RECORD
+Filename: jupyter_jobstorm-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jobstorm/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

## jobstorm/jobcode.py

```diff
@@ -1,35 +1,42 @@
 import os
 import pathlib
 from datetime import datetime
 import re
 import inspect
 import dill
 import jenkins
+from jenkins.__init__ import DELETE_BUILD
 from tabulate import tabulate
+from urllib.parse import urljoin
+import requests
 
 PROJECT = "jobstorm"
 SHRDIR = "/home/shared"
 IPYTMP = ["/ipykernel", "ipython-input"]
-SUFFIX = "tmp_"
+PREFIX = "tmp_"
 JOBCMD = "python3"
 PYTCMD = "python3"
 SAGCMD = "sage"
 PRMNAME = "server.param"
 MAXLINE = 100
-pattern = re.compile('"([^"]+)"')
+func_script_pattern = re.compile('"([^"]+)"')
+tmp_pattern = re.compile("(tmp_[^_]+)")
 
 
 class JobResult:
     def __init__(self, output_paramfilepath, job_filename, jobstorm):
         self.output_paramfilepath = output_paramfilepath
         self.job_filename = job_filename
         self.jobstorm = jobstorm
         self.job_number = None
         self.server = jobstorm.server
+        job_prefix = jobstorm.get_job_prefix(job_filename)
+        message_filename = job_prefix + ".message"
+        self.message_filepath = os.path.join(jobstorm.dirpath, message_filename)
 
     def get_job_number(self):
         if self.job_number is None:
             self.job_number = self.jobstorm.find_job(self.job_filename)
         return self.job_number
 
     def get_status(self):
@@ -44,14 +51,28 @@
 
     def get_result(self):
         status = self.get_status()
         if status not in ["SUCCESS", "UNSTABLE"]:
             raise RuntimeError("job failure or job not finished.")
         return self.jobstorm.loadparam(self.output_paramfilepath)
 
+    def set_message(self, message):
+        f = open(self.message_filepath, "w")
+        f.write(message)
+        f.close()
+
+    def get_message(self):
+        try:
+            f = open(self.message_filepath)
+            message = f.readline()
+            f.close()
+        except:
+            message = ""
+        return message
+
 
 class JobStormBase:
     """Job generator.
 
     Constructor options
     -------------------
     server_url : str
@@ -268,66 +289,147 @@
             raise RuntimeError("all jobs must be deleted.")
         self.server.delete_job(self.project)
 
     def find_job(self, job_filename):
         job_info = self.server.get_job_info(self.project)
         for build in job_info["builds"]:
             job_number = build["number"]
-            build_info = self.server.get_build_info(self.project, job_number)
             try:
+                build_info = self.server.get_build_info(self.project, job_number)
                 filename = build_info["actions"][0]["parameters"][0]["value"]
                 if job_filename == filename:
                     return job_number
             except:
                 pass
         raise RuntimeError("job number not found.")
 
-    def get_job_list(self):
-        job_info = self.server.get_job_info(self.project)
-        job_list = []
-        for build in job_info["builds"]:
-            job_number = build["number"]
-            build_info = self.server.get_build_info(self.project, job_number)
-            result = build_info["result"]
-            ts = int(build_info["timestamp"] / 1000)
-            dt = datetime.fromtimestamp(ts)
+    def get_job(self, job_number, info="detail"):
+        def get_filename(build_info):
             try:
                 filename = build_info["actions"][0]["parameters"][0]["value"]
+            except:
+                filename = None
+            return filename
+
+        def get_script_file(filename):
+            script_file = ""
+            if not filename:
+                return script_file
+            try:
                 filepath = os.path.join(self.dirpath, filename)
-                script = open(filepath).readline()
-                match = pattern.search(script)
+                f = open(filepath)
+                script = f.readline()
+                f.close()
+                match = func_script_pattern.search(script)
                 script_file = match.group(1)
             except:
-                script_file = ""
-            job_list.append(
+                pass
+            return script_file
+
+        def get_message(filename):
+            message = ""
+            if not filename:
+                return message
+            try:
+                job_prefix = self.get_job_prefix(filename)
+                message_filename = job_prefix + ".message"
+                message_filepath = os.path.join(self.dirpath, message_filename)
+                f = open(message_filepath)
+                message = f.readline()
+                f.close()
+            except:
+                pass
+            return message
+
+        try:
+            build_info = self.server.get_build_info(self.project, job_number)
+            result = build_info["result"]
+            ts = int(build_info["timestamp"] / 1000)
+            dt = datetime.fromtimestamp(ts)
+            filename = get_filename(build_info)
+            message = get_message(filename)
+        except:
+            return None
+
+        if info != "simple":
+            script_file = get_script_file(filename)
+        job_elem = [
+            job_number,
+            dt.strftime("%Y/%m/%d %H:%M:%S"),
+            result,
+            message,
+        ]
+        if info != "simple":
+            job_elem.extend(
                 [
-                    job_number,
-                    dt.strftime("%Y/%m/%d %H:%M:%S"),
-                    result,
                     filename,
                     script_file,
                 ]
             )
+        return job_elem
+
+    def get_job_list(self, info="detail"):
+        job_info = self.server.get_job_info(self.project)
+        job_list = []
+        for build in job_info["builds"]:
+            job_number = build["number"]
+            job = self.get_job(job_number, info=info)
+            if job is None:
+                continue
+            job_list.append(job)
         return job_list
 
-    def print_job_list(self):
-        headers = ["job num", "timestamp", "result", "job script", "function script"]
+    def get_job_prefix(self, job_filename):
+        match = tmp_pattern.search(job_filename)
+        return match.group(1)
+
+    def get_jobresult(self, job_number):
+        try:
+            build_info = self.server.get_build_info(self.project, job_number)
+            filename = build_info["actions"][0]["parameters"][0]["value"]
+            job_prefix = self.get_job_prefix(filename)
+            output_paramfilename = job_prefix + ".param.output"
+            output_paramfilepath = os.path.join(self.dirpath, output_paramfilename)
+            return JobResult(output_paramfilepath, filename, self)
+        except:
+            return None
+
+    def print_job_list(self, max_cols=None, info="simple"):
+        job_list = self.get_job_list(info=info)
+        headers = ["job num", "timestamp", "result", "message"]
+        if info != "simple":
+            headers.extend(
+                [
+                    "job script",
+                    "function script",
+                ]
+            )
         table = tabulate(
-            tabular_data=self.get_job_list(), headers=headers, tablefmt="simple"
+            tabular_data=job_list[0:max_cols], headers=headers, tablefmt="simple"
         )
         print(table)
 
     def delete_file(self, filename):
         filepath = os.path.join(self.dirpath, filename)
         try:
             os.remove(filepath)
             print(f"{filepath} is removed.")
         except:
             print(f"{filepath} is not found or some error occurs.")
 
+    def server_delete_build(self, job_number):
+        # workaround
+        param = self.server._get_job_folder(self.project)
+        url_path = DELETE_BUILD % (
+            {"folder_url": param[0], "short_name": param[1], "number": job_number}
+        )
+        url = str(urljoin(self.server.server, url_path))
+        req = requests.Request("POST", url)
+        self.server.jenkins_request(req, True, True).text
+
 
 class JobStormPython(JobStormBase):
     def __init__(
         self,
         server_url=None,
         username=None,
         password=None,
@@ -353,27 +455,27 @@
         src += "\n"
         src += "from jobstorm import *\n"
         src += f'jobstorm = JobStorm(shared_dir="{self.shared_dir}", project="{self.project}")\n'
         src += "\n"
         src += "\n"
         src += self.getfunc()
         tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
-        filename = f"{SUFFIX}{tss}.py"
+        filename = f"{PREFIX}{tss}.py"
         filepath = os.path.join(self.dirpath, filename)
         with open(filepath, "w") as f:
             f.write(src)
         self.srcfilepath = filepath
         return filepath
 
     def makefuncjob(self, runfunc, *args, **kwargs):
         if self.srcfilepath is None:
             # error
             return
         tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
-        paramfilename = f"{SUFFIX}{tss}.param"
+        paramfilename = f"{PREFIX}{tss}.param"
         paramfilepath = os.path.join(self.dirpath, paramfilename)
         self.saveparam(paramfilepath, [args, kwargs])
         output_paramfilepath = f"{paramfilepath}.output"
 
         srcfile = os.path.basename(self.srcfilepath)
 
         if inspect.isfunction(runfunc):
@@ -384,15 +486,15 @@
         src = f'exec(open("{srcfile}").read())\n'
         src += "def run_jobcode():\n"
         src += f'    params = jobstorm.loadparam("{paramfilepath}")\n'
         src += f"    output = {runfuncname}(*params[0], **params[1])\n"
         src += f'    jobstorm.saveparam("{output_paramfilepath}", output)\n'
         src += "\n"
         src += "run_jobcode()\n"
-        filename = f"{SUFFIX}{tss}_job.py"
+        filename = f"{PREFIX}{tss}_job.py"
         filepath = os.path.join(self.dirpath, filename)
         with open(filepath, "w") as f:
             f.write(src)
 
         self.server.build_job(
             self.project, {"job_filename": filename, "job_cmd": self.job_cmd}
         )
@@ -409,24 +511,25 @@
 
         job_list = self.get_job_list()
         job_dict = {job[0]: job[1:] for job in job_list}
         job = job_dict.get(job_number)
         if job is None:
             print(f"job ({job_number}) is not found.")
             return
-        job_script = job[2]
-        func_script = job[3]
+        job_script = job[3]
+        func_script = job[4]
         job_name = job_script[0:-7]
         self.delete_file(f"{job_name}_job.py")
         self.delete_file(f"{job_name}.param")
         self.delete_file(f"{job_name}.param.output")
+        self.delete_file(f"{job_name}.message")
         if not is_same_func_script_exists(job_number, func_script):
             self.delete_file(func_script)
         # self.server.delete_build(self.project, job_number)
-        print("delete build job not implemented because of jenkins request error.")
+        self.server_delete_build(job_number)
         return
 
 
 class JobStormSage(JobStormBase):
     def __init__(
         self,
         server_url=None,
@@ -462,27 +565,27 @@
         src += "\n"
         src += "def RealNumber(x):\n"
         src += "    return x\n"
         src += "\n"
         src += "\n"
         src += self.getfunc()
         tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
-        filename = f"{SUFFIX}{tss}.sage"
+        filename = f"{PREFIX}{tss}.sage"
         filepath = os.path.join(self.dirpath, filename)
         with open(filepath, "w") as f:
             f.write(src)
         self.srcfilepath = filepath
         return filepath
 
     def makefuncjob(self, runfunc, *args, **kwargs):
         if self.srcfilepath is None:
             # error
             return
         tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
-        paramfilename = f"{SUFFIX}{tss}.param"
+        paramfilename = f"{PREFIX}{tss}.param"
         paramfilepath = os.path.join(self.dirpath, paramfilename)
         self.saveparam(paramfilepath, [args, kwargs])
         output_paramfilepath = f"{paramfilepath}.output"
 
         srcfile = os.path.basename(self.srcfilepath)
 
         if inspect.isfunction(runfunc):
@@ -493,15 +596,15 @@
         src = f'load("{srcfile}")\n'
         src += "def run_jobcode():\n"
         src += f'    params = jobstorm.loadparam("{paramfilepath}")\n'
         src += f"    output = {runfuncname}(*params[0], **params[1])\n"
         src += f'    jobstorm.saveparam("{output_paramfilepath}", output)\n'
         src += "\n"
         src += "run_jobcode()\n"
-        filename = f"{SUFFIX}{tss}_job.sage"
+        filename = f"{PREFIX}{tss}_job.sage"
         filepath = os.path.join(self.dirpath, filename)
         with open(filepath, "w") as f:
             f.write(src)
 
         self.server.build_job(
             self.project, {"job_filename": filename, "job_cmd": self.job_cmd}
         )
@@ -518,24 +621,25 @@
 
         job_list = self.get_job_list()
         job_dict = {job[0]: job[1:] for job in job_list}
         job = job_dict.get(job_number)
         if job is None:
             print(f"job ({job_number}) is not found.")
             return
-        job_script = job[2]
-        func_script = job[3]
+        job_script = job[3]
+        func_script = job[4]
         job_name = job_script[0:-7]
         self.delete_file(f"{job_name}_job.sage")
         self.delete_file(f"{job_name}.param")
         self.delete_file(f"{job_name}.param.output")
+        self.delete_file(f"{job_name}.message")
         if not is_same_func_script_exists(job_number, func_script):
             self.delete_file(func_script)
         # self.server.delete_build(self.project, job_number)
-        print("delete build job not implemented because of jenkins request error.")
+        self.server_delete_build(job_number)
         return
 
 
 class JobStorm(JobStormPython):
     def __init__(
         self,
         server_url=None,
```

## Comparing `jupyter_jobstorm-0.2.0.dist-info/LICENSE` & `jupyter_jobstorm-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupyter_jobstorm-0.2.0.dist-info/METADATA` & `jupyter_jobstorm-0.2.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-jobstorm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to run a function written in Jupyter cell as a job
 Home-page: https://github.com/schrodingers-koala/jupyter-jobstorm
 Author: schrodingers-koala
 Author-email: schrodingers.koala@gmail.com
 License: MIT
 Keywords: jupyter-jobstorm,jobstorm
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `jupyter_jobstorm-0.2.0.dist-info/RECORD` & `jupyter_jobstorm-0.2.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 jobstorm/__init__.py,sha256=x1zs_siOLfwFS1WSr-P1v4ihUAnFrGBio3G69LKEYaw,143
-jobstorm/_version.py,sha256=Zn1KFblwuFHiDRdRAiRnDBRkbPttWh44jKa5zG2ov0E,22
-jobstorm/jobcode.py,sha256=cfPBLn76rScW3i51Zk8HJh42r2nX92wmn4JDIYqfta0,18845
-jupyter_jobstorm-0.2.0.dist-info/LICENSE,sha256=gpHNqN3H5sSbdl0dj7qRN9Mer4KCrANAhpLhRdsV_kQ,1076
-jupyter_jobstorm-0.2.0.dist-info/METADATA,sha256=MkPUmc475ZOt9aoeYdXArhZWycHqgFuYgnyPfBWbddA,2653
-jupyter_jobstorm-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-jupyter_jobstorm-0.2.0.dist-info/top_level.txt,sha256=L-ShKot9sheiEOCCa7koMlcy_YTjwoGJdbcPD-huAxg,9
-jupyter_jobstorm-0.2.0.dist-info/RECORD,,
+jobstorm/_version.py,sha256=HfjVOrpTnmZ-xVFCYSVmX50EXaBQeJteUHG-PD6iQs8,22
+jobstorm/jobcode.py,sha256=xYu_6UBLW4VLKpSWKhVcm4NtrjdoeTkabSOThrmzNcs,22199
+jupyter_jobstorm-0.2.1.dist-info/LICENSE,sha256=gpHNqN3H5sSbdl0dj7qRN9Mer4KCrANAhpLhRdsV_kQ,1076
+jupyter_jobstorm-0.2.1.dist-info/METADATA,sha256=8Vm3Q_AL0m2cBaxEH5NyGJ2T1YPBlOoKg8q7-DgE8nE,2653
+jupyter_jobstorm-0.2.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+jupyter_jobstorm-0.2.1.dist-info/top_level.txt,sha256=L-ShKot9sheiEOCCa7koMlcy_YTjwoGJdbcPD-huAxg,9
+jupyter_jobstorm-0.2.1.dist-info/RECORD,,
```

