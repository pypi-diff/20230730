# Comparing `tmp/github4api-1.1.8.tar.gz` & `tmp/github4api-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github4api-1.1.8.tar", last modified: Wed Jul 26 18:51:36 2023, max compression
+gzip compressed data, was "github4api-1.1.9.tar", last modified: Fri Jul 28 22:05:35 2023, max compression
```

## Comparing `github4api-1.1.8.tar` & `github4api-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.617595 github4api-1.1.8/
--rw-rw-rw-   0        0        0     7799 2023-07-07 16:56:50.000000 github4api-1.1.8/LICENSE
--rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     9880 2023-07-26 18:51:36.616594 github4api-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8803 2023-07-26 18:39:16.000000 github4api-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.581594 github4api-1.1.8/github4api/
--rw-rw-rw-   0        0        0      372 2023-06-13 23:43:00.000000 github4api-1.1.8/github4api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.599594 github4api-1.1.8/github4api/exceptions/
--rw-rw-rw-   0        0        0      285 2023-06-13 23:42:53.000000 github4api-1.1.8/github4api/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.600594 github4api-1.1.8/github4api/handlers/
--rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.8/github4api/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.601596 github4api-1.1.8/github4api/handlers/request_handler/
--rw-rw-rw-   0        0        0     1091 2023-06-13 22:34:53.000000 github4api-1.1.8/github4api/handlers/request_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.602595 github4api-1.1.8/github4api/handlers/user_handler/
--rw-rw-rw-   0        0        0      976 2023-06-13 22:36:24.000000 github4api-1.1.8/github4api/handlers/user_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.614596 github4api-1.1.8/github4api/scraper/
--rw-rw-rw-   0        0        0    13087 2023-07-26 18:41:12.000000 github4api-1.1.8/github4api/scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.597595 github4api-1.1.8/github4api.egg-info/
--rw-rw-rw-   0        0        0     9880 2023-07-26 18:51:36.000000 github4api-1.1.8/github4api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-07-26 18:51:36.000000 github4api-1.1.8/github4api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 18:51:36.000000 github4api-1.1.8/github4api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-26 18:51:36.000000 github4api-1.1.8/github4api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 18:51:36.000000 github4api-1.1.8/github4api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      424 2023-07-26 18:39:19.000000 github4api-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 18:51:36.617595 github4api-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-07-26 18:39:12.000000 github4api-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:51:36.615594 github4api-1.1.8/tests/
--rw-rw-rw-   0        0        0      603 2023-06-09 19:43:12.000000 github4api-1.1.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.935378 github4api-1.1.9/
+-rw-rw-rw-   0        0        0     7799 2023-07-07 16:56:50.000000 github4api-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    12803 2023-07-28 22:05:35.934380 github4api-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11642 2023-07-28 22:02:49.000000 github4api-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.855879 github4api-1.1.9/github4api/
+-rw-rw-rw-   0        0        0      388 2023-07-28 15:02:54.000000 github4api-1.1.9/github4api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.917380 github4api-1.1.9/github4api/exceptions/
+-rw-rw-rw-   0        0        0      285 2023-06-13 23:42:53.000000 github4api-1.1.9/github4api/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.919383 github4api-1.1.9/github4api/handlers/
+-rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.9/github4api/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.920379 github4api-1.1.9/github4api/handlers/request_handler/
+-rw-rw-rw-   0        0        0     1091 2023-07-28 15:02:22.000000 github4api-1.1.9/github4api/handlers/request_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.921379 github4api-1.1.9/github4api/handlers/user_handler/
+-rw-rw-rw-   0        0        0     1735 2023-07-28 20:57:53.000000 github4api-1.1.9/github4api/handlers/user_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.931381 github4api-1.1.9/github4api/scraper/
+-rw-rw-rw-   0        0        0    23274 2023-07-28 21:55:42.000000 github4api-1.1.9/github4api/scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.916410 github4api-1.1.9/github4api.egg-info/
+-rw-rw-rw-   0        0        0    12803 2023-07-28 22:05:35.000000 github4api-1.1.9/github4api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-07-28 22:05:35.000000 github4api-1.1.9/github4api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 22:05:35.000000 github4api-1.1.9/github4api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-28 22:05:35.000000 github4api-1.1.9/github4api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 22:05:35.000000 github4api-1.1.9/github4api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      424 2023-07-27 23:31:02.000000 github4api-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 22:05:35.935378 github4api-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-07-27 23:30:55.000000 github4api-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:05:35.933381 github4api-1.1.9/tests/
+-rw-rw-rw-   0        0        0      603 2023-06-09 19:43:12.000000 github4api-1.1.9/tests/__init__.py
```

### Comparing `github4api-1.1.8/LICENSE` & `github4api-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `github4api-1.1.8/README.md` & `github4api-1.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.8</b></p>
+<p align='center'><b>Version 1.1.9</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
@@ -282,14 +282,98 @@
     
 
 
 
 if (__name__ == "__main__"):
     main()
 
+
+```
+
+<br><br><br>
+
+# New Changes on Version 1.1.9
+
+## Now you can Access
+
+- ### List of User's Followings
+- ### List of User's Followers
+- ### Check Last Commit date of Repository with selected Branch
+- ### Check all Commit Dates of a Repository
+- ### Count the Repository Branches
+- ### Check if a Repository is froked from another Repository
+- ### Check if Repository has a LICENSE
+- ### Check the Repository's License Type
+- ### List Repository's Branches
+<br><br>
+
+## +2 Beta Methods
+
+- ### Get all Stars that the User has given to the Repositories
+- ### List all of the Watchers of a Repository
+
+
+```python
+
+
+from github4api.scraper import Scrape
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
+
+
+
+
+def main():
+    user: UserHandler = UserHandler(username='shervinbdndev').serialize()
+    
+    request: RequestHandler = RequestHandler(url=user).sendGetRequest(content=True)
+    
+    scraper: Scrape = Scrape(data=request)
+    
+    scraper.startApi(log=False)
+    
+    print(scraper.listFollowings(username='shervinbdndev')) # List of User's Followings
+    print(scraper.listFollowers(username='shervinbdndev')) # List of User's Followings
+
+    # This Method is in Beta version of itself
+    # It doesn't show all User's Stars that given to Repositories
+    # It only Lists The Repositories on the first page
+    print(scraper.starsGivenRepositoriesNames(username='shervinbdndev'))
+
+    # Last Commit date of Repository with selected Branch
+    print(scraper.repositoryLastCommitDateOnBranch(username='shervinbdndev', repo_name='github4api', branch_name='master'))
+
+    # Commits dates of Repository with selected Branch
+    print(scraper.repositoryCommitsDatesOnBranch(username='shervinbdndev', repo_name='github4api', branch_name='master'))
+
+    # Count of selected Repository Branches
+    print(scraper.repositoryBranchesCount(username='shervinbdndev', repo_name='github4api'))
+
+    # Check if current Repository is Forked from another Repository
+    print(scraper.currentRepositoryIsForkedFromAnotherRepository(username='shervinbdndev', repo_name='github4api'))
+
+    # Check if Repository has a LICENSE
+    print(scraper.repositoryHasLicense(username='shervinbdndev', repo_name='github4api'))
+
+    # Get License Type of a Repository
+    print(scraper.repositoryLicenseType(username='shervinbdndev', repo_name='github4api'))
+
+    # List of Repository Watchers
+    # This Method is in Beta version of itself
+    print(scraper.listRepositoryWatchers(username='shervinbdndev', repo_name='github4api'))
+
+    # List of Repository Branches
+    print(scraper.listRepositoryBranches(username='shervinbdndev', repo_name='github4api'))
+    
+
+
+
+if (__name__ == "__main__"):
+    main()
+
 
 ```
 
 <br>
 
 <h1 align='left'>Enjoy :)</h1>
```

### Comparing `github4api-1.1.8/github4api/handlers/request_handler/__init__.py` & `github4api-1.1.9/github4api/handlers/request_handler/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 if (__debug__):
     try:
         import requests
         from typing import Self, Literal, Union
     
-    except* ModuleNotFoundError as mnfe:
-        raise mnfe.__doc__
+    except* ModuleNotFoundError.__doc__ as mnfe:
+        raise mnfe
     
-    except* ImportError as ie:
-        raise ie.__doc__
+    except* ImportError.__doc__ as ie:
+        raise ie
```

### Comparing `github4api-1.1.8/setup.py` & `github4api-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with codecs.open(os.path.normpath(path=os.path.join(os.path.abspath(path=os.path.dirname(p=__file__)) , r"README.md")) , encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 setup(
     name="github4api",
-    version='1.1.8',
+    version='1.1.9',
     author="Shervin Badanara (shervinbdndev)",
     maintainer="Shervin Badanara",
     author_email="shervin2234@gmail.com",
     description='A python Package API for getting Github Users Information.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages() ,
```

### Comparing `github4api-1.1.8/tests/__init__.py` & `github4api-1.1.9/tests/__init__.py`

 * *Files identical despite different names*

