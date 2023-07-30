# Comparing `tmp/easy_deployer-0.1.8.tar.gz` & `tmp/easy_deployer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_deployer-0.1.8.tar", last modified: Mon Jul 24 22:08:21 2023, max compression
+gzip compressed data, was "easy_deployer-0.1.9.tar", last modified: Fri Jul 28 19:07:58 2023, max compression
```

## Comparing `easy_deployer-0.1.8.tar` & `easy_deployer-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 22:08:21.300916 easy_deployer-0.1.8/
--rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1393 2023-07-24 22:08:21.298985 easy_deployer-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-24 20:24:38.000000 easy_deployer-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 22:08:21.280035 easy_deployer-0.1.8/easy_deployer/
--rw-rw-rw-   0        0        0       90 2023-07-24 22:04:37.000000 easy_deployer-0.1.8/easy_deployer/__init__.py
--rw-rw-rw-   0        0        0    26589 2023-07-24 22:08:07.000000 easy_deployer-0.1.8/easy_deployer/github.py
--rw-rw-rw-   0        0        0    11212 2023-07-24 22:08:07.000000 easy_deployer-0.1.8/easy_deployer/heroku.py
--rw-rw-rw-   0        0        0     9305 2023-07-24 22:08:08.000000 easy_deployer-0.1.8/easy_deployer/main.py
--rw-rw-rw-   0        0        0    12360 2023-07-24 22:08:08.000000 easy_deployer-0.1.8/easy_deployer/shared_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-24 22:08:21.297989 easy_deployer-0.1.8/easy_deployer.egg-info/
--rw-rw-rw-   0        0        0     1393 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 22:08:21.300916 easy_deployer-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1538 2023-07-24 22:04:42.000000 easy_deployer-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:07:58.812567 easy_deployer-0.1.9/
+-rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1393 2023-07-28 19:07:58.810976 easy_deployer-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-07-24 20:24:38.000000 easy_deployer-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 19:07:58.778488 easy_deployer-0.1.9/easy_deployer/
+-rw-rw-rw-   0        0        0      259 2023-07-28 19:06:55.000000 easy_deployer-0.1.9/easy_deployer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:07:58.798009 easy_deployer-0.1.9/easy_deployer/hostings/
+-rw-rw-rw-   0        0        0       61 2023-07-28 18:23:17.000000 easy_deployer-0.1.9/easy_deployer/hostings/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-07-28 18:23:59.000000 easy_deployer-0.1.9/easy_deployer/hostings/heroku.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:07:58.805990 easy_deployer-0.1.9/easy_deployer/utilities/
+-rw-rw-rw-   0        0        0      512 2023-07-28 02:22:20.000000 easy_deployer-0.1.9/easy_deployer/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1806 2023-07-28 02:06:10.000000 easy_deployer-0.1.9/easy_deployer/utilities/interface.py
+-rw-rw-rw-   0        0        0     2078 2023-07-27 18:59:43.000000 easy_deployer-0.1.9/easy_deployer/utilities/process.py
+-rw-rw-rw-   0        0        0     4574 2023-07-28 18:12:43.000000 easy_deployer-0.1.9/easy_deployer/utilities/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:07:58.808981 easy_deployer-0.1.9/easy_deployer/version_control/
+-rw-rw-rw-   0        0        0       41 2023-07-26 16:15:08.000000 easy_deployer-0.1.9/easy_deployer/version_control/__init__.py
+-rw-rw-rw-   0        0        0    23994 2023-07-28 19:04:58.000000 easy_deployer-0.1.9/easy_deployer/version_control/github.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:07:58.796010 easy_deployer-0.1.9/easy_deployer.egg-info/
+-rw-rw-rw-   0        0        0     1393 2023-07-28 19:07:58.000000 easy_deployer-0.1.9/easy_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-07-28 19:07:58.000000 easy_deployer-0.1.9/easy_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 19:07:58.000000 easy_deployer-0.1.9/easy_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 19:07:58.000000 easy_deployer-0.1.9/easy_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-28 19:07:58.000000 easy_deployer-0.1.9/easy_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 19:07:58.812567 easy_deployer-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1393 2023-07-28 19:07:54.000000 easy_deployer-0.1.9/setup.py
```

### Comparing `easy_deployer-0.1.8/LICENSE.txt` & `easy_deployer-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.8/PKG-INFO` & `easy_deployer-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_deployer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to simplify and quickly deploy your project/app/folders to the supported platforms.
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `easy_deployer-0.1.8/README.md` & `easy_deployer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.8/easy_deployer/github.py` & `easy_deployer-0.1.9/easy_deployer/version_control/github.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,322 +1,228 @@
-# coding=<utf-8>
-from subprocess import Popen, PIPE, DEVNULL
-from argparse import ArgumentParser
-import os, sys, json, getpass, re, time, itertools, threading, signal, webbrowser, keyboard
-
-from .shared_functions import printWarning, listPromptInquirer, promptPyInquirer, runCmd, getOS, openBash, defaultCommit
-
-def main():
-    args = takeArgs() # Take the arguments
-    if not os.path.exists(args["path"]):
-        print("Invalid Path!")
-        sys.exit(5)
-    args["path"] = os.path.abspath(args["path"])
-    args["path"] = args["path"].strip()
-    checkSoftware("git", "git --help") # check if git is installed in the current machine
-    args["path"] = os.path.abspath(args["path"]) # just changing 
-    createResourceDir() #create resources
-    # os.chdir(args["path"]) # changing directory
-    if getOS() == "windows": # to clean the screen
+import click
+import os
+import sys
+import re
+import json
+import time
+
+from subprocess import PIPE, DEVNULL
+
+from easy_deployer.utilities import ERROR_CODES
+from easy_deployer.utilities.terminal import check_software, handle_git_init, default_git_commit, run_cmd\
+    ,open_bash
+from easy_deployer.utilities.process import Loading, get_os, open_browser
+from easy_deployer.utilities.interface import path_input, text_input, confirm_input, select_input,\
+    print_warning
+
+available_commands = ('create-update', 'update', 'delete')
+
+@click.command(
+        help="""You basically enter one of the following commands:\n
+        ¤ create-update (which is the default one)\n
+        ¤ update (to update an existing repository)\n
+        ¤ delete (to delete an existing repository)\n
+then you need to specify the path by using the -p or --path argument."""
+)
+@click.option("-cmd", "--command",
+              type=click.Choice(available_commands,case_sensitive=False),
+              help="commands, default command is 'create-update'")
+@click.option("-p", "--path", type=str, help="Path of the folder")
+@click.option("-new", multiple=True, type=click.Choice(('user', 'token'), case_sensitive=False), 
+              help="if you want to resave user or token")
+@click.option("-repo", "--repository", "name", type=str, help="Repository name")
+@click.option("-ac", "--add-collaborators", "add_collab", is_flag=True, help="If you want to add collaborators, repository must exist to do so else you'll get an error")
+@click.option("-visibility", is_flag=True, help="Change visibility")
+@click.option("-git-ig", "--git-ignore", is_flag=True, help="Add a file to the .gitignore file")
+@click.option("-rm-git-ig", "--rm-git-ignore", is_flag=True, help="Remove file from .gitignore")
+@click.pass_context
+def main(ctx, command, path, new, name, add_collab, visibility, git_ignore, rm_git_ignore):
+    if get_os() == "windows": # to clean the screen
         os.system("cls") # clears the console
-    if args["git_ignore"]:
-        handleGitIgnore(args["path"])
-    if args["rm_git_ignore"]:
-        handleRmGitIgnore(args["path"])
-    if args["cmd"] == "update": # check if -u or --update is present when the user runs the script
-        update(args)
+    path, command = handle_args(path, command, git_ignore=git_ignore, rm_git_ignore=rm_git_ignore)
+    check_software("git", "git --help") # check if git is installed in the current machine
+    create_resource_dir() #create resources
+    # Update command is invoked
+    if command == "update": # check if -u or --update is present when the user runs the script
+        update(path=path, name=name, add_collab=add_collab)
+    elif command == "delete":
+        delete(path=path, name=name, new=new)
         return
-    if args["cmd"] == "delete":
-        delete(args)
+    elif command == "create-update":
+        create_update(path=path, name=name, new=new, add_collab=add_collab, visibility=visibility)
         return
-    if args["cmd"] == "create-update":
-        create_update(args)
-        return
-
-def takeArgs():
-    parser = ArgumentParser(prog="github-deployer",
-    usage="""You basically enter one of the following commands:
-        ¤ create-update (which is the default one)
-        ¤ update (to update an existing repository)
-        ¤ delete (to delete an existing repository)
-then you need to specify the path by using the -p or --path argument.""", description="%(prog)s <commands> [options]")
-    parser.add_argument("-v","--version", action="version", version="version 1.0", help="%(prog)s current version")
-    parser.add_argument("cmd", nargs="?", default="create-update", choices=["create-update", "update", "delete"],help="commands, default command is 'create-update'")
-    parser.add_argument("-p","--path", help="path of the folder intended to deploy.", required=True)
-    parser.add_argument("-new", nargs="*", default=[], choices=["user","token"], help="if you want to resave user or token")
-    parser.add_argument("-repo", "--repository",dest="name", help="repository name")
-    parser.add_argument("-ac", "--add-collaborators", action="store_true",help="if you want to add collaborators, repository must exist to do so else you'll get an error")
-    parser.add_argument("-visibility", action="store_true")
-    # parser.add_argument("-atp","--add-to-path-var", action="store_true", help="if you want to add the program to path environnement variable so that you can run it wherever you are")
-    parser.add_argument("-git-ig", "--git-ignore", action="store_true")
-    parser.add_argument("-rm-git-ig", "--rm-git-ignore", action="store_true")
-    args = parser.parse_args()
-    return vars(args)
 
-def create_update(args):
+# Functions responsable for commands
+def create_update(path, name, new, add_collab, visibility):
     """This functions runs when the user chooses the 'create-update' command"""
-    infoAboutToken() # info telling the user that he needs a token to create a repository
-    defaultCommit(args) # git add, git commit etc...
-    username = handleUsername(args) # takes care of the username 
-    token = handleToken(args, username) # takes care of the access token
-    data = infoAboutRepo(username,token,args["name"],args["add_collaborators"], args["path"])
-    url = getGithubUrl(data)
-    createRepo = repositoryCreationNeeded(url, token, args["path"])
-    if createRepo:
-        loading = Loading(startText="Creating repository", stopText="repository has been created!", type="dynamic", timeout=.1)
+    info_about_token() # info telling the user that he needs a token to create a repository
+    default_git_commit(path) # git add, git commit etc...
+    username = handle_username(new) # takes care of the username 
+    token = handle_token(new, username) # takes care of the access token
+    data = info_about_repo(username, token, name, add_collab, path)
+    url = get_github_URL(data)
+    create_repo = repository_creation_needed(url, token, path)
+    if create_repo:
+        loading = Loading(start_text="Creating repository", stop_text="repository has been created!", type="dynamic", timeout=.1)
         isCollaborators = data["collaborators"]
         data = {k:v for k,v in data.items() if k != "username" and k != "collaborators"}
         # cmd down is a command for creating a repository 
         loading.start()
         cmd = 'curl -f -u '+username+':'+token+' https://api.github.com/user/repos -d "'+json.dumps(data).replace("\"","\\\"")+'"'
-        out = openBash(cmd, stderr=PIPE ,stdout=PIPE, loading=loading, error="""Error has been caught:
+        out = open_bash(cmd, stderr=PIPE ,stdout=PIPE, loading=loading, error="""Error has been caught:
             Authorization Required! check your username and password
-        """, printBashError=False)
+        """, print_bash_error=False)
         loading.stop()
-        saveTokenIfnotSaved(token)
+        save_token_if_not_saved(token)
         if isCollaborators:
-            handleCollaborators(username=username, token=token, repo_name=data["name"])
-    elif not createRepo:
+            handle_collaborators(username=username, token=token, repo_name=data["name"])
+    elif not create_repo:
         #if we don't need to create a repository (which means it's already available) then we simply print that below
         print("repository already exist...")
-        if(args["visibility"]):
-            if args["visibility"]:
+        if(visibility):
+            if visibility:
                 changeVisibility(username=username, token=token, repo_name=data["name"])
-        if(args["add_collaborators"]):
-            handleCollaborators(username=username, token=token, repo_name=data["name"])
-    masterToMain(args["path"])
-    addRemoteAndPush(url, args["path"])
+        if(add_collab):
+            handle_collaborators(username=username, token=token, repo_name=data["name"])
+    master_to_main(path)
+    add_remote_and_push(url, path, username=username, token=token, repo_name=data["name"])
 
-def update(args):
+def update(path, name, new, add_collab):
     """
     it gets called when "-u" or "--update" are available
     it updates or (pushs) the specified directory to the specified repository
     """
-    defaultCommit(args)
-    username = handleUsername(args)
-    token = handleToken(args, username)
-    repo_name = getRepoName(args["name"], args["path"])
-    url = getGithubUrl({"username":username,"name":repo_name})
-    if args["add_collaborators"]:
-        addCollaborators(args, username=username, token=token, name=repo_name)
+    default_git_commit(path)
+    args = {}
+    username = handle_username(new)
+    token = handle_token(new, username)
+    repo_name = get_repo_name(name, path)
+    url = get_github_URL({"username":username,"name":repo_name})
+    if add_collab:
+        add_collaborators(path, name, new, username=username, token=token, name=repo_name)
     if args["visibility"]:
         changeVisibility(username=username, token=token, name=repo_name)
-    createRepo = repositoryCreationNeeded(url,token, args["path"])
-    saveTokenIfnotSaved(token)
-    if createRepo:
-        repoNotFoundError()
-    elif not createRepo:
-        masterToMain(args["path"])
-        addRemoteAndPush(url, args["path"])
-
-def delete(args):
-    username = handleUsername(args)
-    token = handleToken(args, username)
-    repo_name = getRepoName(args["name"], args["path"])
-    url = getGithubUrl({ "username":username, "name":repo_name })
-    createRepo = repositoryCreationNeeded(url=url,token=token, path=args["path"])
-    if createRepo:
-        repoNotFoundError()
-    elif not createRepo:
-        loading = Loading(startText="Deleting Repository",stopText="Repository Deleted", type="dynamic", timeout=.1)
+    create_repo = repository_creation_needed(url,token, path)
+    save_token_if_not_saved(token)
+    if create_repo:
+        repo_not_found()
+    elif not create_repo:
+        master_to_main(path)
+        add_remote_and_push(url, path, username=username, token=token, repo_name=repo_name)
+
+def delete(path, name, new):
+    username = handle_username(new)
+    token = handle_token(new, username)
+    repo_name = get_repo_name(name, path)
+    url = get_github_URL({ "username":username, "name":repo_name })
+    create_repo = repository_creation_needed(url=url,token=token, path=path)
+    if create_repo:
+        repo_not_found()
+    elif not create_repo:
+        loading = Loading(start_text="Deleting Repository",stop_text="Repository Deleted", type="dynamic", timeout=.1)
         loading.start()
-        openBash(f"curl -X DELETE -H 'Authorization: token {token}' https://api.github.com/repos/{username}/{repo_name}", stdout=PIPE, stderr=PIPE ,loading=loading)
+        open_bash(f"curl -X DELETE -H 'Authorization: token {token}' https://api.github.com/repos/{username}/{repo_name}", stdout=PIPE, stderr=PIPE ,loading=loading)
         loading.stop()
 
-def addCollaborators(args,**credentials):
-    if not credentials:
-        username = handleUsername(args)
-        token = handleToken(args, username)
-        repo = getRepoName(args["name"], args["path"])
-    elif credentials:
-        username = credentials["username"]
-        token = credentials["token"]
-        repo = credentials["name"]
-    url = getGithubUrl({"username": username, "name":repo})
-    repositoryNeeded = repositoryCreationNeeded(url, token, args["path"])
-    if repositoryNeeded:
-        print("ERROR\nRepository doesn't exist, check your repository name!")
-        sys.exit(3)
-    handleCollaborators(username=username, token=token, name=repo)
-    
-
-def add2Path(args):
-    path = args["path"]
-    if not os.path.isfile:
-        print("Error, this is not a file!")
-        sys.exit(3)
-    if getOS() == "windows":
-        if path in runCmd("echo %PATH%", stdout=PIPE, stderr=PIPE):
-            print("It's Already in the path variable!")
-            sys.exit(3)
-        print("ok")
-        runCmd('setx PATH "%PATH%;'+path+'"')
-
-
-def cacheToken(username):
-    path_token = promptPyInquirer({
-        "type": "input",
-        "name": "path_token",
-        "message": f"Enter either path of the file that contains the access token, or enter the access toke directly: ",
-        "validate": lambda val: "Invalid path/token" if len(val)==0 and (not os.path.isfile(val)) and (re.search("[^\w]", val)) else True
-    })["path_token"]
-    if os.path.isfile(path_token):
-        with open(path_token, 'r') as f:
-            return f.read()
-    else:
-        return path_token
-    # key = input("Enter 'f' if you have access token in a file path, or 'c' if you have it on the clipboard: ").strip().lower()
-    # if key == 'f':
-    #     fpath = input(f"Enter file path that contains the access token: (current directory {os.getcwd()}) ")
-    #     if os.path.exists(fpath) and os.path.isfile(fpath):
-    #         with open(fpath, 'r') as f:
-    #             return f.read()
-    #     elif os.path.exists(fpath) and not os.path.isfile(fpath):
-    #         print("Error!", "This is not a file!")
-    #         sys.exit(7)
-    #     elif not os.path.exists(fpath):
-    #         print("Error!","Invalid path!")
-    #         sys.exit(7)
-    # elif key == 'c':
-    #     return getpass.getpass("Enter host access token for user '"+username+"': ")
-    # else:
-    #     invalidAnswerExit()
-    
-
-def promptCollaborators():
-    isCollaborators = input("do you want collaborators with you in this repository? (y/n): ").strip().lower()
-    if isCollaborators == "y":
-        return True
-    elif isCollaborators == "n":
-        return False
-    else:
-        invalidAnswerExit()
-        
-
-
-def getToken():
-    path = tokenPath()["path"] # directory path
-    file_= tokenPath()["file_"] # file path
-    if os.path.exists(path + file_):
-        try:
-            with open(path+file_, "r") as f:
-                token = f.read()
-            if token != "":
-                return token
-        except FileNotFoundError as err:
-            print("Error token file has been remove or modified in runtime")
-            sys.exit(9)
-    return None
+# Handlers
+def handle_args(path: str, command: str, git_ignore, rm_git_ignore):
+    if command is None:
+        command = select_input("Which command would you like to execute:", 
+                               choices=('create-update', 'update', 'delete'), 
+                               default="create-update")
+    if command != "delete" or git_ignore or rm_git_ignore:
+        if path is None:
+            path = path_input("Enter path of the folder: ",  only_directories=True, default=os.getcwd(),
+                            validate=lambda x: os.path.isdir(x), invalid_message="Invalid directory path!")
+        elif not os.path.isdir(path):
+            print("Invalid path")
+            sys.exit(ERROR_CODES["invalid_path"])
+        if git_ignore:
+            handle_git_ignore(path)
+        if rm_git_ignore:
+            handle_rm_git_ignore(path)
+        return os.path.abspath(path.strip()), command
+    return None, command
 
-def isTokenSaved(): # checks if the token is already saved or not
-    path = tokenPath()["path"]
-    file_= tokenPath()["file_"]
-    if os.path.exists(path + file_):
-        try:
-            with open(path+file_, "r") as f:
-                token = f.read()
-            if token != "":
-                return True
-            return False
-        except FileNotFoundError as err:
-            return False
-    else:
-        return False
+def handle_git_ignore(path):
+    files_dirs = os.listdir(path)
+    files = input("Enter name of the file(s) you want to ignore seperated by commas if there one than one file: ").split(",")
+    files = [x.strip() for x in files]
+    if ".gitignore" not in files_dirs:
+        with open(f"{path}{os.sep}.gitignore", "w") as f:
+            f.write("\n".join(files))
+            f.write("\n")
+    elif ".gitignore" in files_dirs:
+        with open(f"{path}{os.sep}.gitignore", "a") as f:
+            f.write("\n".join(files))
+            f.write("\n")
+    handle_git_init(path)
+    run_cmd(f"git -C {path} add .gitignore", stdout=PIPE, stderr=PIPE)
+    run_cmd(f"git -C {path} rm -rf --cached .", stdout=PIPE, stderr=PIPE)
 
-def saveTokenIfnotSaved(token):
-    if not isTokenSaved():
-        wantTosaveToken = input("Do you want to save your token (y/n): ").strip().lower()
-        if wantTosaveToken == "y":
-            saveToken(token)
-        elif wantTosaveToken != "n":
-            invalidAnswerExit()
+def handle_rm_git_ignore(path):
+    files_dirs = os.listdir(path)
+    if ".gitignore" not in files_dirs:
+        print("there is no '.gitignore' file...")
+        sys.exit(ERROR_CODES["missing_gitignore_file"])
+    files = [f.strip() for f in input("Enter name of the file(s) you want to keep track of seperated by commas if there one than one file: ").split(",")]
+    with open(f"{path}{os.sep}.gitignore") as f:
+        lines = f.readlines()
+    lines = [re.sub("\n$","",line) for line in lines]
+    files = [line for line in lines if line not in files]
+    with open(f"{path}{os.sep}.gitignore", "w") as f:
+        f.write("\n".join(files))
+    handle_git_init(path)
+    run_cmd(f"git -C {path} add .gitignore", stdout=PIPE, stderr=PIPE)
+    run_cmd(f"git -C {path} rm -rf --cached .")
 
-def handleUsername(args): #self explanatory
-    fpath = usernamePath()["path"]+usernamePath()["file_"]
+def handle_username(new): #self explanatory
+    fpath = username_path()["path"]+username_path()["file_"]
     reg = re.compile("^([a-z0-9](?:-?[a-z0-9]){1,39})",re.IGNORECASE)
     if os.path.exists(fpath):
         with open(fpath, "r") as f:
                 data = f.read()
     else:
         data = None
-    if "user" in args["new"] :
-        username = getUserName()
+    if "user" in new :
+        username = get_username()
         if username != reg.findall(username)[0]:
             print("Invalid username")
             sys.exit(8)
-        saveUsername(username)
+        save_username(username)
         return username
     elif data and data != "":
         print("Username saved as "+data)
         return data
     else:
-        username = getUserName()
+        username = get_username()
         if username != reg.findall(username)[0]:
             print("Invalid username")
             sys.exit(8)
-        saveUsername(username)
+        save_username(username)
         return username
 
-def handleToken(args, username):
-    if "token" in args["new"] :
-        token = cacheToken(username)
+def handle_token(new, username):
+    if "token" in new :
+        token = cache_token(username)
         checkTokenValidation(token)
-        saveToken(token)
-        print("token got saved, you can either run this script with '-new token' argument again or go to "+tokenPath()["path"]+tokenPath()["file_"],"and edit the file.")
+        save_token(token)
+        print("token got saved, you can either run this script with '-new token' argument again or go to "+token_path()["path"]+token_path()["file_"],"and edit the file.")
     elif not isTokenSaved():
-        token = cacheToken(username)
+        token = cache_token(username)
         checkTokenValidation(token)
-        saveTokenIfnotSaved(token)
+        save_token_if_not_saved(token)
     elif isTokenSaved():
         token = getToken()
-    if token == None:
+    if token is None:
         print("error: token is None")
-        sys.exit(3)
+        sys.exit(ERROR_CODES["token_is_none"])
     return token
 
-def handleGitInit(path):
-    files_dirs = os.listdir(path)
-    if ".git" not in files_dirs:
-        runCmd(f"git -C {path} init", stdout=PIPE, stderr=PIPE)
-
-def handleGitIgnore(path):
-    files_dirs = os.listdir(path)
-    files = input("Enter name of the file(s) you want to ignore seperated by commas if there one than one file: ").split(",")
-    files = [x.strip() for x in files]
-    if ".gitignore" not in files_dirs:
-        with open(f"{path}{os.sep}.gitignore", "w") as f:
-            f.write("\n".join(files))
-            f.write("\n")
-    elif ".gitignore" in files_dirs:
-        with open(f"{path}{os.sep}.gitignore", "a") as f:
-            f.write("\n".join(files))
-            f.write("\n")
-    handleGitInit(path)
-    runCmd(f"git -C {path} add .gitignore", stdout=PIPE, stderr=PIPE)
-    runCmd(f"git -C {path} rm -rf --cached .", stdout=PIPE, stderr=PIPE)
-
-def handleRmGitIgnore(path):
-    files_dirs = os.listdir(path)
-    if ".gitignore" not in files_dirs:
-        print("there is no '.gitignore' file...")
-        sys.exit(15)
-    files = [f.strip() for f in input("Enter name of the file(s) you want to keep track of seperated by commas if there one than one file: ").split(",")]
-    with open(f"{path}{os.sep}.gitignore") as f:
-        lines = f.readlines()
-    lines = [re.sub("\n$","",line) for line in lines]
-    files = [line for line in lines if line not in files]
-    with open(f"{path}{os.sep}.gitignore", "w") as f:
-        f.write("\n".join(files))
-    handleGitInit(path)
-    runCmd(f"git -C {path} add .gitignore", stdout=PIPE, stderr=PIPE)
-    runCmd(f"git -C {path} rm -rf --cached .")
-
-
-
-def handleCollaborators(**credentials):
+def handle_collaborators(**credentials):
     username = credentials["username"]
     token = credentials["token"]
     name = credentials["repo_name"]
     try:
         n = int(input("how many collaborators do you want to invite: ")) # number of collaborattors
     except ValueError:
         print("Error! invalid number!")
@@ -358,153 +264,227 @@
     """)
     for collaborator in collaborators:
         permission = input("permission for '"+collaborator+"' : ")
         permissions = ["pull", "push", "admin", "maintain", "triage"]
         if permission not in permissions:
             permission = "push"
         command = "curl -H 'Authorization: token "+token+"' 'https://api.github.com/repos/"+username+"/"+name+"/collaborators/"+collaborator+"' -X PUT -d '{\"permission\":\""+permission+"\"}'"
-        process = openBash(command, returncode=True,stderr=PIPE, stdout=PIPE, error="error!\nperhaps you misspelled collaborator name, your access token, repository name or your username...")
+        process = open_bash(command, returncode=True,stderr=PIPE, stdout=PIPE, error="error!\nperhaps you misspelled collaborator name, your access token, repository name or your username...")
         returncode = process["returncode"]
         out = process["out"]
         err = process["err"]
         out = json.loads(out)
         if "message" in out:
             print(out["message"])
         else:
             print("Added!")
 
-def changeVisibility(**credentials):
-    username = credentials["username"]
-    token = credentials["token"]
-    repo_name = credentials["repo_name"]
-    # visiblity = promptPyInquirer({
-    #     "name": "visibility",
-    #     "question": "change it to?",
-    #     "choices": ["private", "public"]
-    # })["visibility"]
-    if(getOS() == "windows"):
-        visiblity = promptPyInquirer({
-            "type": "list",
-            "name": "visibility",
-            "message": "change it to?",
-            "choices": ["private", "public"]
-        })["visibility"]
-    else:
-        visiblity = listPromptInquirer({
-            "name": "visibility",
-            "question": "change it to?",
-            "choices": ["private", "public"]
-        })
-    command = "curl -H 'Authorization: token "+token+"' 'https://api.github.com/repos/"+username+"/"+repo_name+"' -H 'Accept: application/vnd.github.nebula-preview+json' -X PATCH -d '{\"visibility\":\""+visiblity+"\"}'"
+
+#ADDERS
+def add_collaborators(path, name, new, username=None, token=None, repo=None):
+    username = username if username else handle_username(new)
+    token = token if token else handle_token(new, username)
+    repo = repo if repo else get_repo_name(name, path)
+    url = get_github_URL({"username": username, "name":repo})
+    repositoryNeeded = repository_creation_needed(url, token, path)
+    if repositoryNeeded:
+        print("ERROR\nRepository doesn't exist, check your repository name!")
+        sys.exit(3)
+    handle_collaborators(username=username, token=token, name=repo)
+
+def add_remote_and_push(url, path, repo_name, username, token, remote_name="origin",):
+    out = run_cmd("git -C "+ path +" remote", stdout=PIPE, stderr=PIPE)
+    if remote_name in out:
+        run_cmd(f"git -C {path} remote rm {remote_name}")
+    loading = Loading(start_text="pushing to github")
+    loading.start()
+    run_cmd(f"git -C {path} remote add {remote_name} {url}", stdout=PIPE, stderr=PIPE)
+    process = run_cmd(f"git -C {path} push -u {remote_name} main --dry-run", quit_on_error=False,
+                      returncode=True, stderr=PIPE)
+    run_cmd(f"git -C {path} push -u {remote_name} main")
+    if "err" in process: 
+        if "hint: (e.g., 'git pull ...') before pushing again." in process["err"]:
+            loading.abort()
+            click.echo("\n" + click.style(process["err"], fg="yellow"), color=True)
+            
+            OPTION_1 = """Clone the repository, then just copy its .git folder to here, and therefore you will lose your current commits but not the past one's (from the cloned repo)"""
+            options = select_input("There is couple options to fixed it", choices=[OPTION_1])
+            if options == OPTION_1:
+                temp_dir = "../temp" + str(int(time.time()))
+                open_bash(f"git clone https://{token}@github.com/{username}/{repo_name}.git {temp_dir}")
+                open_bash(f"""
+                          shopt -s extglob
+                          cp -r !(.git) "{temp_dir}"
+                          cp -r {temp_dir}/.git .
+                          """)
+                commit_again = confirm_input("A git commit is about to happen, are you ok with that")
+                if commit_again:
+                    default_git_commit(path)
+                return add_remote_and_push(url, path, repo_name, username, token)
+        else:
+            sys.exit(process["returncode"])
+    loading.stop()
+    open_browser(url)       
+
+#CHECKERS
+def check_repository_name(repo_name):
+    regex = re.compile("[^A-Za-z0-9_\-]{1,}")
+    max_char = 100
+    repo_name = repo_name[:max_char]
     
-    loading = Loading(type="dynamic", startText="Changing", stopText="Changed!")
+    if regex.search(repo_name):
+        new_name = regex.sub("-", repo_name)
+        print_warning("Your new repository will be created as:",new_name,sep="\n\t",flush=True)
+        confirm = confirm_input("Do you want to Try another one?: ", default=True)
+        if not confirm:
+            repo_name = check_repository_name(text_input("Try another repository name: "))
+        elif confirm:
+            repo_name = new_name
+    return repo_name
+
+def checkTokenValidation(token):
+    loading = Loading(start_text="Checking Token Access Validation", stop_text="")
     loading.start()
-    process = openBash(command, stderr=PIPE, stdout=PIPE, returncode=True)
-    if("Visibility is already " in process["out"]):
+    if re.search("[^\w]",token) or token == "":
         loading.abort()
-        print("Visibility is already private.")
-    elif "Not found" in process["err"]:
-        print("Not found.")
-        sys.exit(12)
-    elif process["returncode"] == 0: 
-        loading.stop()
+        print("Invalid token")
+        sys.exit(17)
+    open_bash(f"curl -f -H \"Authorization: token {token}\" https://api.github.com/users/codertocat -I", stdout=PIPE, stderr=PIPE, error="there is no such token available",loading=loading, print_bash_error=False,timeout=10)
+    loading.stop()
+    pass
+
 
-def createResourceDir():
-    path = tokenPath()["path"]
+# RESOURCES
+def create_resource_dir():
+    path = token_path()["path"]
     if not os.path.exists(path=path):
         os.makedirs(path)
-def tokenPath(): # get token path depending on the operating system
-    if getOS() == "windows":
+
+# PATHS
+def token_path(): # get token path depending on the operating system
+    if get_os() == "windows":
         return {"path":"C:\\.gd\\","file_":".gd-token"}
 
-def usernamePath(): #get username path depending on the operating system
-    if getOS() == "windows":
+def username_path(): #get username path depending on the operating system
+    if get_os() == "windows":
         return {"path":"C:\\.gd\\","file_":".gd-username"}
+    
+# GETTERS
+def get_username():
+    return text_input("username (on github): ")
 
+def getToken():
+    path = token_path()["path"] # directory path
+    file_= token_path()["file_"] # file path
+    if os.path.exists(path + file_):
+        try:
+            with open(path+file_, "r") as f:
+                token = f.read()
+            if token != "":
+                return token
+        except FileNotFoundError as err:
+            print("Error token file has been remove or modified in runtime")
+            sys.exit(ERROR_CODES["token_file_not_found"])
+    return None
 
-def saveToken(token):
-    path = tokenPath()["path"]
-    file_= tokenPath()["file_"]
-    with open( path + file_, "w" ) as ft:
-        ft.write(token)
-
-def saveUsername(username):
-    fpath = usernamePath()["path"]+usernamePath()["file_"]
-    with open(fpath, "w") as f:
-        f.write(username)
-
-def getUserName():
-    return input("username (on github): ")
-
-
-def getRepoName(repo, path):
+def get_repo_name(repo, path):
     if not repo:
-        out = runCmd(f"git -C {path} remote -v", stdout=PIPE, stderr=PIPE, quitOnError=False)
+        out = run_cmd(f"git -C {path} remote -v", stdout=PIPE, stderr=PIPE, quit_on_error=False)
         if out:
             regex = re.compile("https:\/\/github\.com\/.+/(.+)\.git")
             matchs = regex.findall(out)
             if matchs:
-                repo = promptPyInquirer({
-                "name": "repo",
-                "type": "input",
-                "message": "Enter the name of the repository: ",
-                "default": matchs[1]
-            })['repo']
+                repo = text_input(
+                    message="Enter the name of the repository:",
+                    default=matchs[1]
+                    )
             else:
-                repo = input("Enter the name of the repository: ")
+                repo = text_input("Enter the name of the repository: ")
         else:
-            repo = input("Enter the name of the repository: ")
-    
-    return checkRepositoryName(repo)
+            repo = text_input("Enter the name of the repository: ")
     
+    return check_repository_name(repo)
 
-def getGithubUrl(data):
+def get_github_URL(data):
     # data['name'] = data['name'].replace(" ","-")
     return f"https://github.com/{data['username']}/{data['name']}.git"
 
-
-def infoAboutToken():
+#INFO
+def info_about_token():
     print("If you don't have your token yet go get it from https://github.com/settings/tokens (you must be loggedIn)")
 
-def infoAboutRepo(username,token,repo,collaboratorsCmdExist, path):
-    repo_name = getRepoName(repo, path)
-    if not repositoryCreationNeeded( getGithubUrl({"name":repo_name, "username":username}), token, path):
+def info_about_repo(username,token,repo,collaboratorsCmdExist, path):
+    repo_name = get_repo_name(repo, path)
+    if not repository_creation_needed( get_github_URL({"name":repo_name, "username":username}), token, path):
         return {"name":repo_name, "username":username}
     
-    private = input("want it to be private? (y/n): ").lower()
-    if private == "y":
-        private = True
-    elif private == "n":
-        private = False
-    else:
-        invalidAnswerExit()
+    private = confirm_input("want it to be private? (y/n): ")
     if collaboratorsCmdExist:
         collaborators = True
     elif not collaboratorsCmdExist:
-        collaborators = promptCollaborators()
+        collaborators = prompt_collaborators()
     return {"name": repo_name,"private":private,"username":username, "collaborators":collaborators}
 
-def openBrowser(url):
-    print("[¤] press any key to open repository in your browser or q to quit the program.")
-    if keyboard.read_key() == "q":
-        sys.exit(0)
+
+# SAVERS
+def save_username(username):
+    fpath = username_path()["path"]+username_path()["file_"]
+    with open(fpath, "w") as f:
+        f.write(username)
+
+def save_token_if_not_saved(token):
+    if not isTokenSaved():
+        wantTosaveToken = confirm_input("Do you want to save your token (y/n): ")
+        if wantTosaveToken:
+            save_token(token)
+
+def save_token(token):
+    path = token_path()["path"]
+    file_= token_path()["file_"]
+    with open( path + file_, "w" ) as ft:
+        ft.write(token)
+
+def cache_token(username):
+    path_token = path_input(
+        message="Enter either path of the file that contains the access token, or enter the access toke directly:",
+        invalid_message="Invalid path",
+        validate=lambda x: os.path.isfile(x) if re.search("[/\/]") else len(x) > 0
+    )
+    if os.path.isfile(path_token):
+        with open(path_token, 'r') as f:
+            return f.read()
     else:
-        loading = Loading(startText="Opening",stopText="Opened!", timeout=0.18)
-        loading.start()
-        webbrowser.open(url)
-        loading.stop()
+        return path_token
+    
+#is Functions (return bool)
+
+def isTokenSaved() -> bool: # checks if the token is already saved or not
+    path = token_path()["path"]
+    file_= token_path()["file_"]
+    if os.path.exists(path + file_):
+        try:
+            with open(path+file_, "r") as f:
+                token = f.read()
+            if token != "":
+                return True
+            return False
+        except FileNotFoundError as err:
+            return False
+    else:
+        return False
 
-def repositoryCreationNeeded(url, token, path): #check if we should create a repository, if not then it returns True
+#REPO STUFF
+def repository_creation_needed(url, token, path): #check if we should create a repository, if not then it returns True
     protocolAndSlash = "https://"
     suburl = url[len(protocolAndSlash):]
     username = re.findall("^https://github.com/(\w*)",url)[0]
     url = protocolAndSlash+username+":"+token+"@"+suburl
-    processing = Loading(stopText="", type="dynamic", timeout=.13)
+    processing = Loading(stop_text="", type="dynamic", timeout=.13)
     processing.start()
-    process = openBash('git ls-remote '+url, stderr=PIPE, stdout=PIPE, returncode=True, timeout=10)
+    process = open_bash('git ls-remote '+url, stderr=PIPE, stdout=PIPE, returncode=True, timeout=10)
     processing.stop()
     returncode = process["returncode"]
     err = process["err"]
     if 'remote: Invalid username or password.\nfatal: Authentication failed' == err:
         print(err)
         sys.exit(3)
     if returncode != 0 and err == "":
@@ -513,128 +493,49 @@
         return False
     elif returncode != 0 and "Repository not found" in err:
         return True
     else:
         print("ERROR")
         sys.exit(returncode)
 
-def addRemoteAndPush(url, path, remote_name="origin"):
-    out = runCmd("git -C "+ path +" remote", stdout=PIPE, stderr=PIPE)
-    if remote_name in out:
-        runCmd(f"git -C {path} remote rm {remote_name}")
-    # loading = Loading(startText="pushing to github")
-    # loading.start()
-    runCmd(f"git -C {path} remote add {remote_name} {url}", stdout=PIPE, stderr=PIPE)
-    runCmd(f"git -C {path} push -u {remote_name} main")
-    # loading.stop()
-    openBrowser(url)
-
-def invalidAnswerExit():
-    print("invalid answer")
-    sys.exit(12)
-
-def repoNotFoundError():
-    print("ERROR\nRepository doesn't exist, check your repository name!")
-    sys.exit(3)
-
-
-def checkTokenValidation(token):
-    loading = Loading(startText="Checking Token Access Validation", stopText="")
-    loading.start()
-    if re.search("[^\w]",token) or token == "":
-        loading.abort()
-        print("Invalid token")
-        sys.exit(17)
-    openBash(f"curl -f -H \"Authorization: token {token}\" https://api.github.com/users/codertocat -I", stdout=PIPE, stderr=PIPE, error="there is no such token available",loading=loading, printBashError=False,timeout=10)
-    loading.stop()
-    pass
-
-def checkRepositoryName(repo_name):
-    regex = re.compile("[^A-Za-z0-9_\-]{1,}")
-    max_char = 100
-    repo_name = repo_name[:max_char]
-    
-    if regex.search(repo_name):
-        new_name = regex.sub("-", repo_name)
-        printWarning("Your new repository will be created as:",new_name,sep="\n\t",flush=True)
-        confirm = input("Do you want to Try another one? (y/n): ").strip().lower()
-        if confirm == "y":
-            confirm = False
-        elif confirm == "n":
-            confirm = True
-        else:
-            invalidAnswerExit()
-        if not confirm:
-            repo_name = checkRepositoryName(input("Try another repository name: "))
-        elif confirm:
-            repo_name = new_name
-    return repo_name
-
-def checkSoftware(name, cmd, url=None):
-    err = f"It seems that {name} is not in your machine, please make sure to download it first"
-    err += f"\n you can find it at {url}" if url else ""
-    runCmd(cmd, stdout=DEVNULL,
-        error= err
-    )
-
-def checkCommit(path):
-    out = runCmd(f"git -C {path} status", stdout=PIPE, stderr=PIPE)
-    if "nothing to commit, working tree clean" in out:
-        print(out)
-        return False
-    return True
-
-def masterToMain(path):
-    out = runCmd(f"git -C {path} branch", stdout=PIPE, stderr=PIPE)
+def master_to_main(path):
+    out = run_cmd(f"git -C {path} branch", stdout=PIPE, stderr=PIPE)
     if "main" in out:
         return
-    runCmd(f"git -C {path} branch -m master main", stdout=PIPE, stderr=PIPE)
-    runCmd(f"git -C {path} checkout main", stdout=DEVNULL, stderr=PIPE)
+    run_cmd(f"git -C {path} branch -m master main", stdout=PIPE, stderr=PIPE)
+    run_cmd(f"git -C {path} checkout main", stdout=DEVNULL, stderr=PIPE)
 
+def prompt_collaborators():
+    isCollaborators = confirm_input("do you want collaborators with you in this repository: ")
+    return isCollaborators
 
-class Loading:
-    def __init__(self,**info):
-        self.type = info["type"] if "type" in info else "dots"
-        self.startText = info["startText"] if "startText" in info else "Processing"
-        self.stopText = info["stopText"] if "stopText" in info else "Done!"
-        self.timeout = info["timeout"] if "timeout" in info else 0.5
-        if self.type == "dots":
-            self.list_ = [ "", "." , ".." , "..."]
-        elif self.type == "dynamic":
-            self.list_ = info["list_"] if "list_" in info else ["/", "|", "\\", "-"]
-        else:
-            raise "Invalid Type"
-    
-    def start(self):
-        self.done = False
-        thread = threading.Thread(target=self.__loop)
-        thread.daemon = True
-        thread.start()
+def changeVisibility(**credentials):
+    username = credentials["username"]
+    token = credentials["token"]
+    repo_name = credentials["repo_name"]
+    # visiblity = promptPyInquirer({
+    #     "name": "visibility",
+    #     "question": "change it to?",
+    #     "choices": ["private", "public"]
+    # })["visibility"]
     
-    def __loop(self):
-        if self.type == "dots":
-            for i in itertools.cycle(self.list_):
-                if self.done:
-                    break
-                print("\r"+self.startText + i+" "*(len(self.list_)-self.list_.index(i)-1),end="",flush=True)
-                time.sleep(self.timeout)
-            
-        elif self.type == "dynamic":
-            for i in itertools.cycle(self.list_):
-                if self.done:
-                    break
-                print("\r"+self.startText,i,end="",flush=True)
-                time.sleep(self.timeout)
-
-    def stop(self):
-        self.done = True
-        if self.type == "dots":
-            print("\r"+self.stopText+" "*(len(self.startText)+len(self.list_)-len(self.stopText)))
-        elif self.type == "dynamic":
-            print("\r"+self.stopText+" "*(len(self.startText)+2-len(self.stopText))+"\r")
+    visiblity = select_input(
+        "Change it to:",
+        choices=["private", "public"]
+    )
+    command = "curl -H 'Authorization: token "+token+"' 'https://api.github.com/repos/"+username+"/"+repo_name+"' -H 'Accept: application/vnd.github.nebula-preview+json' -X PATCH -d '{\"visibility\":\""+visiblity+"\"}'"
     
-    def abort(self):
-        self.done = True
-        print("\r")
+    loading = Loading(type="dynamic", start_text="Changing", stop_text="Changed!")
+    loading.start()
+    process = open_bash(command, stderr=PIPE, stdout=PIPE, returncode=True)
+    if("Visibility is already " in process["out"]):
+        loading.abort()
+        print("Visibility is already private.")
+    elif "Not found" in process["err"]:
+        print("Not found.")
+        sys.exit(12)
+    elif process["returncode"] == 0: 
+        loading.stop()
 
-if __name__ == "__main__":
-    main()
+def repo_not_found():
+    print("ERROR\nRepository doesn't exist, check your repository name!")
+    sys.exit(ERROR_CODES["repository_not_found"])
```

### Comparing `easy_deployer-0.1.8/easy_deployer.egg-info/PKG-INFO` & `easy_deployer-0.1.9/easy_deployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-deployer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to simplify and quickly deploy your project/app/folders to the supported platforms.
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `easy_deployer-0.1.8/setup.py` & `easy_deployer-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_desc = f.read()
 setup(
     name="easy_deployer",
-    version="0.1.8",
+    version="0.1.9",
     description="A package to simplify and quickly deploy your project/app/folders to the supported platforms.",
     long_description=long_desc,
     long_description_content_type='text/markdown',
     author="Mohamed-Amine Benali",
     author_email="benali.medamine2002@gmail.com",
     url="https://github.com/medamine980/easy-deployer",
     packages=find_packages(exclude=["easy_deployer.dist", "easy_deployer.ignore"]),
@@ -21,17 +21,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.11'
     ],
     entry_points = {
         'console_scripts': [
-            'easy-deployer = easy_deployer.main:main',
-            'easy-deployer-github = easy_deployer.github:main',
-            'easy-deployer-heroku = easy_deployer.heroku:main'
+            'easy-deployer = cli:cli',
         ]
     }
     # console_scripts={
     #     "easy-deployer-github": "easy_deployer.github:main",
     #     "easy-deployer-heroku": "easy_deployer.heroku:main",
     #     "easy-deployer": "easy_deployer.main:main"
     # }
```

