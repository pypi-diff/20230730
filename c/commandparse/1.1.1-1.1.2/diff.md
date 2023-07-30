# Comparing `tmp/commandparse-1.1.1.tar.gz` & `tmp/commandparse-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/commandparse-1.1.1.tar", last modified: Tue Dec 22 20:38:16 2020, max compression
+gzip compressed data, was "commandparse-1.1.2.tar", last modified: Sun Jul 30 18:17:25 2023, max compression
```

## Comparing `commandparse-1.1.1.tar` & `commandparse-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-22 20:38:16.000000 commandparse-1.1.1/
--rw-r--r--   0 user      (1000) user      (1000)       16 2020-12-20 20:04:28.000000 commandparse-1.1.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     1575 2020-12-22 20:38:16.000000 commandparse-1.1.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      751 2020-12-20 20:04:28.000000 commandparse-1.1.1/README.md
--rw-r--r--   0 user      (1000) user      (1000)        6 2020-12-22 20:37:15.000000 commandparse-1.1.1/VERSION
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-22 20:38:16.000000 commandparse-1.1.1/commandparse/
--rw-r--r--   0 user      (1000) user      (1000)     9283 2020-12-22 20:36:14.000000 commandparse-1.1.1/commandparse/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-22 20:38:16.000000 commandparse-1.1.1/commandparse.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1575 2020-12-22 20:38:16.000000 commandparse-1.1.1/commandparse.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      238 2020-12-22 20:38:16.000000 commandparse-1.1.1/commandparse.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2020-12-22 20:38:16.000000 commandparse-1.1.1/commandparse.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2020-12-22 20:38:16.000000 commandparse-1.1.1/commandparse.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2020-12-22 20:38:16.000000 commandparse-1.1.1/commandparse.egg-info/zip-safe
--rw-r--r--   0 user      (1000) user      (1000)       38 2020-12-22 20:38:16.000000 commandparse-1.1.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1031 2020-12-20 20:33:30.000000 commandparse-1.1.1/setup.py
+drwx------   0 user      (1000) user      (1000)        0 2023-07-30 18:17:25.740663 commandparse-1.1.2/
+-rw-------   0 user      (1000) user      (1000)     1061 2023-07-30 18:09:31.000000 commandparse-1.1.2/LICENCE
+-rw-------   0 user      (1000) user      (1000)       16 2023-07-30 18:09:31.000000 commandparse-1.1.2/MANIFEST.in
+-rw-------   0 user      (1000) user      (1000)     1408 2023-07-30 18:17:25.740663 commandparse-1.1.2/PKG-INFO
+-rw-------   0 user      (1000) user      (1000)      751 2023-07-30 18:09:31.000000 commandparse-1.1.2/README.md
+-rw-------   0 user      (1000) user      (1000)        6 2023-07-30 18:15:55.000000 commandparse-1.1.2/VERSION
+drwx------   0 user      (1000) user      (1000)        0 2023-07-30 18:17:25.740663 commandparse-1.1.2/commandparse/
+-rw-------   0 user      (1000) user      (1000)     9341 2023-07-30 18:11:42.000000 commandparse-1.1.2/commandparse/__init__.py
+drwx------   0 user      (1000) user      (1000)        0 2023-07-30 18:17:25.740663 commandparse-1.1.2/commandparse.egg-info/
+-rw-------   0 user      (1000) user      (1000)     1408 2023-07-30 18:17:25.000000 commandparse-1.1.2/commandparse.egg-info/PKG-INFO
+-rw-------   0 user      (1000) user      (1000)      246 2023-07-30 18:17:25.000000 commandparse-1.1.2/commandparse.egg-info/SOURCES.txt
+-rw-------   0 user      (1000) user      (1000)        1 2023-07-30 18:17:25.000000 commandparse-1.1.2/commandparse.egg-info/dependency_links.txt
+-rw-------   0 user      (1000) user      (1000)       13 2023-07-30 18:17:25.000000 commandparse-1.1.2/commandparse.egg-info/top_level.txt
+-rw-------   0 user      (1000) user      (1000)        1 2023-07-30 18:16:48.000000 commandparse-1.1.2/commandparse.egg-info/zip-safe
+-rw-------   0 user      (1000) user      (1000)       38 2023-07-30 18:17:25.740663 commandparse-1.1.2/setup.cfg
+-rw-------   0 user      (1000) user      (1000)     1031 2023-07-30 18:16:28.000000 commandparse-1.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `commandparse-1.1.1/PKG-INFO` & `commandparse-1.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: commandparse
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI application commands parser
 Home-page: https://github.com/flgy/commandparse
 Author: flgy
 Author-email: florian.guilbert@synacktiv.com
 License: MIT
-Description: # commandparse
-        
-        Module to parse command based CLI application.
-        
-        Usage:
-        
-        * Subclass the Command class
-        * Add a method with a name such as `prefix_commandname` with kwargs as required argument
-        * Create an ArgumentParser instance
-        * Call the `Subclass.add_suparsers` with the ArgumentParser instance and other settings
-        * Use the `dispatch_command` function with the args returned by `parser.parse_args()`
-        
-        ```
-        parser = ArgumentParser(...)
-        [...]
-        Subclass.add_subparsers(parser, prefixes=["get_", "do_", ...], title="commands", description="available commands")
-        
-        cmd = Subclass(...)
-        cmd.dispatch_command(commands, args)
-        ```
-        
-        See example.py for a more complete example. For a real world application using this lib, see: https://github.com/franc-pentest/ldeep
-        
 Keywords: CLI,command,argparse,parser
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# commandparse
+
+Module to parse command based CLI application.
+
+Usage:
+
+* Subclass the Command class
+* Add a method with a name such as `prefix_commandname` with kwargs as required argument
+* Create an ArgumentParser instance
+* Call the `Subclass.add_suparsers` with the ArgumentParser instance and other settings
+* Use the `dispatch_command` function with the args returned by `parser.parse_args()`
+
+```
+parser = ArgumentParser(...)
+[...]
+Subclass.add_subparsers(parser, prefixes=["get_", "do_", ...], title="commands", description="available commands")
+
+cmd = Subclass(...)
+cmd.dispatch_command(commands, args)
+```
+
+See example.py for a more complete example. For a real world application using this lib, see: https://github.com/franc-pentest/ldeep
```

### Comparing `commandparse-1.1.1/README.md` & `commandparse-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `commandparse-1.1.1/commandparse/__init__.py` & `commandparse-1.1.2/commandparse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 							arguments[name]["help_line"] = line
 						else:
 							arguments[name]["help_line"] += " " + line
 
 		return {"help_line": help_line.strip(), "arguments": arguments}
 
 	@classmethod
-	def add_subparsers(cls, parser, name="", prefixes=[], delim="_", title="commands", description="available commands"):
+	def add_subparsers(cls, parser, name="", prefixes=[], delim="_", title="commands", description="available commands", required=True):
 		"""
 		Parse the calling classes and extract commands, for each command register a subparser.
 	
 		:cls: class to register subparsers
 		:parser: add the subparsers to the provided parser
 		:prefixes: str list of prefixes corresponding to command methods
 		:delim: str delimiter to separate prefix from commnad name
@@ -270,20 +270,20 @@
 		"""
 		Executes the corresponding command with provided args.
 		Returns None if no command is provided otherwise forwards the command return.
 		Raises CommandNotFoundError if the command is not registered, should not happen.
 
 		:args: result from ArgumentParser.parse_args()
 		"""
-		arguments = vars(args)
+		arguments = {k: v for k, v in vars(args).items() if v is not None}
 		for c in self.COMMANDS.keys():
 			cmd = arguments.get(c, False)
 			idx = c
 			if cmd:
 				break
 		else:
 			return None
 
 		if cmd not in self.COMMANDS[idx]:
 			raise CommandNotFoundError("{cmd} not registered".format(cmd=cmd))
 
-		return getattr(self, self.COMMANDS[idx][cmd])(vars(args))
+		return getattr(self, self.COMMANDS[idx][cmd])(arguments)
```

### Comparing `commandparse-1.1.1/commandparse.egg-info/PKG-INFO` & `commandparse-1.1.2/commandparse.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: commandparse
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI application commands parser
 Home-page: https://github.com/flgy/commandparse
 Author: flgy
 Author-email: florian.guilbert@synacktiv.com
 License: MIT
-Description: # commandparse
-        
-        Module to parse command based CLI application.
-        
-        Usage:
-        
-        * Subclass the Command class
-        * Add a method with a name such as `prefix_commandname` with kwargs as required argument
-        * Create an ArgumentParser instance
-        * Call the `Subclass.add_suparsers` with the ArgumentParser instance and other settings
-        * Use the `dispatch_command` function with the args returned by `parser.parse_args()`
-        
-        ```
-        parser = ArgumentParser(...)
-        [...]
-        Subclass.add_subparsers(parser, prefixes=["get_", "do_", ...], title="commands", description="available commands")
-        
-        cmd = Subclass(...)
-        cmd.dispatch_command(commands, args)
-        ```
-        
-        See example.py for a more complete example. For a real world application using this lib, see: https://github.com/franc-pentest/ldeep
-        
 Keywords: CLI,command,argparse,parser
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# commandparse
+
+Module to parse command based CLI application.
+
+Usage:
+
+* Subclass the Command class
+* Add a method with a name such as `prefix_commandname` with kwargs as required argument
+* Create an ArgumentParser instance
+* Call the `Subclass.add_suparsers` with the ArgumentParser instance and other settings
+* Use the `dispatch_command` function with the args returned by `parser.parse_args()`
+
+```
+parser = ArgumentParser(...)
+[...]
+Subclass.add_subparsers(parser, prefixes=["get_", "do_", ...], title="commands", description="available commands")
+
+cmd = Subclass(...)
+cmd.dispatch_command(commands, args)
+```
+
+See example.py for a more complete example. For a real world application using this lib, see: https://github.com/franc-pentest/ldeep
```

### Comparing `commandparse-1.1.1/setup.py` & `commandparse-1.1.2/setup.py`

 * *Files identical despite different names*

