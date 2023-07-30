# Comparing `tmp/licensecheck-2023.2.tar.gz` & `tmp/licensecheck-2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensecheck-2023.2.tar", max compression
+gzip compressed data, was "licensecheck-2023.3.tar", max compression
```

## Comparing `licensecheck-2023.2.tar` & `licensecheck-2023.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1080 2023-01-01 17:53:39.457996 licensecheck-2023.2/LICENSE.md
-drwxr-xr-x   0        0        0        0 2023-07-28 01:28:25.993549 licensecheck-2023.2/licensecheck/
--rw-r--r--   0        0        0     3151 2023-07-28 01:28:25.666660 licensecheck-2023.2/licensecheck/__init__.py
--rw-r--r--   0        0        0      113 2023-07-28 01:28:25.666660 licensecheck-2023.2/licensecheck/__main__.py
--rw-r--r--   0        0        0     4677 2023-07-28 01:28:25.662660 licensecheck-2023.2/licensecheck/formatter.py
--rw-r--r--   0        0        0     4895 2023-07-28 01:28:25.663661 licensecheck-2023.2/licensecheck/get_deps.py
--rw-r--r--   0        0        0     4447 2023-07-28 01:28:25.664660 licensecheck-2023.2/licensecheck/license_matrix.py
--rw-r--r--   0        0        0     1789 2023-07-27 22:51:47.916428 licensecheck-2023.2/licensecheck/matrix.csv
--rw-r--r--   0        0        0     5323 2023-07-28 01:28:25.665659 licensecheck-2023.2/licensecheck/packageinfo.py
--rw-r--r--   0        0        0     2459 2023-01-01 17:53:39.466968 licensecheck-2023.2/licensecheck/pypi_licenses/osi_approved.txt
--rw-r--r--   0        0        0      652 2023-01-01 17:53:39.466968 licensecheck-2023.2/licensecheck/pypi_licenses/other.txt
--rw-r--r--   0        0        0     2258 2023-07-28 01:28:25.665659 licensecheck-2023.2/licensecheck/types.py
--rw-r--r--   0        0        0     2218 2023-07-28 01:33:33.406856 licensecheck-2023.2/pyproject.toml
--rw-r--r--   0        0        0    22924 2023-03-07 00:27:16.455942 licensecheck-2023.2/README.md
--rw-r--r--   0        0        0    24636 1970-01-01 00:00:00.000000 licensecheck-2023.2/setup.py
--rw-r--r--   0        0        0    24422 1970-01-01 00:00:00.000000 licensecheck-2023.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-01-01 17:53:39.457996 licensecheck-2023.3/LICENSE.md
+drwxr-xr-x   0        0        0        0 2023-07-30 00:59:28.643654 licensecheck-2023.3/licensecheck/
+-rw-r--r--   0        0        0     3279 2023-07-30 00:59:28.236642 licensecheck-2023.3/licensecheck/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-30 00:59:28.237165 licensecheck-2023.3/licensecheck/__main__.py
+-rw-r--r--   0        0        0     4687 2023-07-30 00:59:28.230555 licensecheck-2023.3/licensecheck/formatter.py
+-rw-r--r--   0        0        0     5450 2023-07-30 00:59:28.643654 licensecheck-2023.3/licensecheck/get_deps.py
+-rw-r--r--   0        0        0     4553 2023-07-30 00:59:28.232642 licensecheck-2023.3/licensecheck/license_matrix.py
+-rw-r--r--   0        0        0     1789 2023-07-29 22:14:24.310463 licensecheck-2023.3/licensecheck/matrix.csv
+-rw-r--r--   0        0        0     5421 2023-07-30 00:59:28.234649 licensecheck-2023.3/licensecheck/packageinfo.py
+-rw-r--r--   0        0        0     2459 2023-01-01 17:53:39.466968 licensecheck-2023.3/licensecheck/pypi_licenses/osi_approved.txt
+-rw-r--r--   0        0        0      652 2023-01-01 17:53:39.466968 licensecheck-2023.3/licensecheck/pypi_licenses/other.txt
+-rw-r--r--   0        0        0     2586 2023-07-30 00:59:28.235641 licensecheck-2023.3/licensecheck/types.py
+-rw-r--r--   0        0        0     2285 2023-07-30 00:59:56.960659 licensecheck-2023.3/pyproject.toml
+-rw-r--r--   0        0        0    23356 2023-07-28 01:51:02.641542 licensecheck-2023.3/README.md
+-rw-r--r--   0        0        0    25140 1970-01-01 00:00:00.000000 licensecheck-2023.3/setup.py
+-rw-r--r--   0        0        0    24945 1970-01-01 00:00:00.000000 licensecheck-2023.3/PKG-INFO
```

### Comparing `licensecheck-2023.2/LICENSE.md` & `licensecheck-2023.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.2/licensecheck/__init__.py` & `licensecheck-2023.3/licensecheck/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 from pathlib import Path
 from sys import exit as sysexit
 from sys import stdout
 
 from fhconfparser import FHConfParser, SimpleConf
 
-from licensecheck import formatter, get_deps
+from licensecheck import formatter, get_deps, types
 
 stdout.reconfigure(encoding="utf-8")
 
 
 def cli() -> None:
 	"""Cli entry point."""
 	exitCode = 0
@@ -63,40 +63,41 @@
 	)
 	args = vars(parser.parse_args())
 
 	# ConfigParser (Parses in the following order: `pyproject.toml`,
 	# `setup.cfg`, `licensecheck.toml`, `licensecheck.json`,
 	# `licensecheck.ini`, `~/licensecheck.toml`, `~/licensecheck.json`, `~/licensecheck.ini`)
 	configparser = FHConfParser()
+	namespace = ["tool"]
 	configparser.parseConfigList(
 		[("pyproject.toml", "toml"), ("setup.cfg", "ini")]
 		+ [
 			(f"{directory}/licensecheck.{ext}", ext)
 			for ext in ("toml", "json", "ini")
 			for directory in [".", str(Path.home())]
 		],
-		["tool"],
-		["tool"],
+		namespace,
+		namespace,
 	)
 	simpleConf = SimpleConf(configparser, "licensecheck", args)
 
 	# File
 	filename = (
 		stdout
 		if simpleConf.get("file") is None
 		else open(simpleConf.get("file"), "w", encoding="utf-8")
 	)
 
 	# Get list of licenses
 	myLice, depsWithLicenses = get_deps.getDepsWithLicenses(
 		simpleConf.get("using", "poetry"),
-		simpleConf.get("ignore_packages", []),
-		simpleConf.get("fail_packages", []),
-		simpleConf.get("ignore_licenses", []),
-		simpleConf.get("fail_licenses", []),
+		list(map(types.ucstr, simpleConf.get("ignore_packages", []))),
+		list(map(types.ucstr, simpleConf.get("fail_packages", []))),
+		list(map(types.ucstr, simpleConf.get("ignore_licenses", []))),
+		list(map(types.ucstr, simpleConf.get("fail_licenses", []))),
 	)
 
 	# Are any licenses incompatible?
 	incompatible = any(not lice.licenseCompat for lice in depsWithLicenses)
 
 	# Format the results
 	if simpleConf.get("format", "simple") in formatter.formatMap:
```

### Comparing `licensecheck-2023.2/licensecheck/formatter.py` & `licensecheck-2023.3/licensecheck/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {
 	name: str
 	version: str
 	namever: str
 	size: int
 	homePage: str
 	author: str
-	license: str
+	license: ucstr
 	licenseCompat: bool
 }
 ```
 
 To one of the following formats:
 
 - ansi
@@ -29,15 +29,15 @@
 from io import StringIO
 
 from rich.console import Console
 from rich.table import Table
 
 from licensecheck.types import License, PackageInfo, printLicense
 
-INFO = {"program": "licensecheck", "version": "2023.1.3", "license": "mit"}
+INFO = {"program": "licensecheck", "version": "2023.1.3", "license": "MIT LICENSE"}
 
 
 def stripAnsi(string: str) -> str:
 	"""Strip ansi codes from a given string
 
 	Args:
 		string (str): string to strip codes from
```

### Comparing `licensecheck-2023.2/licensecheck/get_deps.py` & `licensecheck-2023.3/licensecheck/get_deps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Get a list of packages with package compatibility.
 """
 from __future__ import annotations
 
 from importlib import metadata
 from pathlib import Path
+from typing import Any
 
 import pkg_resources
-import requests
+import requirements
 import tomli
 
 from licensecheck import license_matrix, packageinfo
-from licensecheck.types import JOINS, License, PackageInfo
+from licensecheck.types import JOINS, License, PackageInfo, session, ucstr
 
 USINGS = ["requirements", "poetry", "PEP631"]
 
 
-def getReqs(using: str) -> set[str]:
+def getReqs(using: str) -> set[ucstr]:
 	"""Get requirements for the end user project/ lib.
 
 	>>> getReqs("poetry")
 	>>> getReqs("poetry:dev")
 	>>> getReqs("requirements")
 	>>> getReqs("requirements:requirements.txt;requirements-dev.txt")
 	>>> getReqs("PEP631")
@@ -28,36 +29,49 @@
 	Args:
 		using (str): use requirements, poetry or PEP631.
 
 	Returns:
 		set[str]: set of requirement packages
 	"""
 
-	resolveReq = lambda req: pkg_resources.Requirement.parse(req).project_name.lower()
-
 	_ = using.split(":", 1)
 	using, extras = _[0], _[1] if len(_) > 1 else None
 	if using not in USINGS:
 		using = "poetry"
-	reqs = set()
 
-	pyprojectPath = Path("pyproject.toml")
 	pyproject = {}
+	requirementsPaths = []
+
+	pyprojectPath = Path("pyproject.toml")
 	if pyprojectPath.exists():
 		pyproject = tomli.loads(pyprojectPath.read_text(encoding="utf-8"))
 
+	# Requirements
+	if using == "requirements":
+		requirementsPaths = [Path(x) for x in (extras or "requirements.txt").split(";")]
+
+	return _doGetReqs(using, extras, pyproject, requirementsPaths)
+
+
+def _doGetReqs(
+	using: str, extras: str | None, pyproject: dict[str, Any], requirementsPaths: list[Path]
+) -> set[ucstr]:
+	resolveReq = lambda req: ucstr(pkg_resources.Requirement.parse(req).project_name)
+
+	reqs = set()
+
 	if using == "poetry":
 		try:
 			project = pyproject["tool"]["poetry"]
 			reqLists = [project["dependencies"]]
 		except KeyError as error:
 			raise RuntimeError(
 				"Could not find specification of requirements (pyproject.toml)."
 			) from error
-		if extras:
+		if extras is not None:
 			reqLists.extend(
 				project.get("group", {x: {"dependencies": {}}})[x]["dependencies"]
 				for x in extras.split(";")
 			)
 			reqLists.append(project.get("dev-dependencies", {}))
 		for reqList in reqLists:
 			for req in reqList:
@@ -76,85 +90,89 @@
 			reqLists.extend(project["optional-dependencies"][x] for x in extras.split(";"))
 		for reqList in reqLists:
 			for req in reqList:
 				reqs.add(resolveReq(req))
 
 	# Requirements
 	if using == "requirements":
-		for reqTxt in (extras or "requirements.txt").split(";"):
-
-			reqPath = Path(reqTxt)
+		for reqPath in requirementsPaths:
 			if not reqPath.exists():
 				raise RuntimeError(f"Could not find specification of requirements ({reqPath}).")
 
-			for req in reqPath.read_text("utf-8").strip().split("\n"):
-				reqs.add(resolveReq(req))
+			with open(reqPath, encoding="utf-8") as requirementsTxt:
+				for req in requirements.parse(requirementsTxt):
+					reqs.add(str(req.name).lower())
 
 	try:
-		reqs.remove("python")
+		reqs.remove("PYTHON")
 	except KeyError:
 		pass
 
 	# Get Dependencies (1 deep)
 	requirementsWithDeps = reqs.copy()
 	for requirement in reqs:
 		try:
-			pkgMetadata = metadata.metadata(resolveReq(requirement))
+			pkgMetadata = metadata.metadata(requirement)
 			for req in [resolveReq(req) for req in pkgMetadata.get_all("Requires-Dist") or []]:
 				requirementsWithDeps.add(req)
 		except metadata.PackageNotFoundError:
-			request = requests.get(f"https://pypi.org/pypi/{requirement}/json", timeout=60)
+			request = session.get(f"https://pypi.org/pypi/{requirement}/json", timeout=60)
 			response = request.json()
 			try:
 				for req in [resolveReq(req) for req in response["info"]["requires_dist"]]:
 					requirementsWithDeps.add(req)
-			except KeyError:
+			except (KeyError, TypeError):
 				pass
 
 	return requirementsWithDeps
 
 
 def getDepsWithLicenses(
 	using: str,
-	ignorePackages: list[str],
-	failPackages: list[str],
-	ignoreLicenses: list[str],
-	failLicenses: list[str],
+	ignorePackages: list[ucstr],
+	failPackages: list[ucstr],
+	ignoreLicenses: list[ucstr],
+	failLicenses: list[ucstr],
 ) -> tuple[License, set[PackageInfo]]:
 	"""Get a set of dependencies with licenses and determine license compatibility.
 
 	Args:
 		using (str): use requirements or poetry
-		ignorePackages (list[str]): a list of packages to ignore (compat=True)
-		failPackages (list[str]): a list of packages to fail (compat=False)
-		ignoreLicenses (list[str]): a list of licenses to ignore (skipped, compat may still be False)
-		failLicenses (list[str]): a list of licenses to fail (compat=False)
+		ignorePackages (list[ucstr]): a list of packages to ignore (compat=True)
+		failPackages (list[ucstr]): a list of packages to fail (compat=False)
+		ignoreLicenses (list[ucstr]): a list of licenses to ignore (skipped, compat may still be False)
+		failLicenses (list[ucstr]): a list of licenses to fail (compat=False)
 
 	Returns:
 		tuple[License, set[PackageInfo]]: tuple of
 			my package license
 			set of updated dependencies with licenseCompat set
 	"""
 	reqs = getReqs(using)
 
 	# Get my license
 	myLiceTxt = packageinfo.getMyPackageLicense()
 	myLice = license_matrix.licenseType(myLiceTxt)[0]
+	ignoreLicensesType = license_matrix.licenseType(
+		ucstr(JOINS.join(ignoreLicenses)), ignoreLicenses
+	)
+	failLicensesType = license_matrix.licenseType(ucstr(JOINS.join(failLicenses)), ignoreLicenses)
 
 	# Check it is compatible with packages and add a note
 	packages = packageinfo.getPackages(reqs)
 	for package in packages:
 		# Deal with --ignore-packages and --fail-packages
 		package.licenseCompat = False
-		if package.name.lower() in [x.lower() for x in ignorePackages]:
+		packageName = package.name
+		if packageName in ignorePackages:
 			package.licenseCompat = True
-		elif package.name.lower() in [x.lower() for x in failPackages]:
+		elif packageName in failPackages:
 			pass  # package.licenseCompat = False
 		# Old behaviour
 		else:
 			package.licenseCompat = license_matrix.depCompatWMyLice(  # type: ignore
 				myLice,
-				license_matrix.licenseType(package.license),
-				license_matrix.licenseType(JOINS.join(ignoreLicenses)),
-				license_matrix.licenseType(JOINS.join(failLicenses)),
+				license_matrix.licenseType(package.license, ignoreLicenses),
+				ignoreLicensesType,
+				failLicensesType,
 			)
 	return myLice, packages
```

### Comparing `licensecheck-2023.2/licensecheck/license_matrix.py` & `licensecheck-2023.3/licensecheck/license_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,27 @@
 from __future__ import annotations
 
 import csv
 from pathlib import Path
 
 from licensecheck.types import JOINS
 from licensecheck.types import License as L
+from licensecheck.types import ucstr
 
 THISDIR = Path(__file__).resolve().parent
 
 with Path(THISDIR / "matrix.csv").open(mode="r", newline="", encoding="utf-8") as csv_file:
 	LICENSE_MATRIX = list(csv.reader(csv_file))
 
 
-def licenseLookup(licenseStr: str, ignoreLicenses: list[str] | None = None) -> L:
+def licenseLookup(licenseStr: ucstr, ignoreLicenses: list[ucstr] | None = None) -> L:
 	"""Identify a license from an uppercase string representation of a license.
 
 	Args:
-		licenseStr (str): uppercase string representation of a license
+		licenseStr (ucstr): uppercase string representation of a license
 
 	Returns:
 		L: License represented by licenseStr
 	"""
 	termToLicense = {
 		"PUBLIC DOMAIN": L.PUBLIC,
 		"CC-PDDC": L.PUBLIC,
@@ -102,26 +103,26 @@
 		if liceStr in licenseStr:
 			return lice
 	if licenseStr not in (ignoreLicenses or ""):
 		print(f"WARN: '{licenseStr}' License not identified so falling back to NO_LICENSE")
 	return L.NO_LICENSE
 
 
-def licenseType(lice: str) -> list[L]:
+def licenseType(lice: ucstr, ignoreLicenses: list[ucstr] | None = None) -> list[L]:
 	"""Return a list of license types from a license string.
 
 	Args:
-		lice (str): license name
+		lice (ucstr): license name
 
 	Returns:
 		list[L]: the license
 	"""
 	if len(lice or "") < 1:
 		return [L.NO_LICENSE]
-	return [licenseLookup(x) for x in lice.upper().split(JOINS)]
+	return [licenseLookup(ucstr(x), ignoreLicenses) for x in lice.split(JOINS)]
 
 
 def depCompatWMyLice(
 	myLicense: L,
 	depLice: list[L],
 	ignoreLicenses: list[L] | None = None,
 	failLicenses: list[L] | None = None,
```

### Comparing `licensecheck-2023.2/licensecheck/matrix.csv` & `licensecheck-2023.3/licensecheck/matrix.csv`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 GPL_2,1,1,1,1,1,1,1,1,0,0,0,1,1,0,1,0,1,1,0,1,0,0,1,1,0,0
 GPL_3,1,1,1,1,1,1,1,1,1,0,0,1,1,1,1,1,0,0,1,1,1,0,1,1,0,0
 GPL_2_PLUS,1,1,1,1,1,1,1,1,0,0,0,1,1,0,1,0,1,1,0,1,0,0,1,1,0,0
 GPL_3_PLUS,1,1,1,1,1,1,1,1,1,0,0,1,1,1,1,1,0,0,1,1,1,0,1,1,0,0
 AGPL_3_PLUS,1,1,1,1,1,1,1,1,0,0,0,1,1,1,1,1,1,1,1,1,1,0,1,1,0,0
 MPL,1,1,1,1,1,1,1,1,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,0,0,0
 EU,1,1,1,1,1,1,1,1,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,0,0
-PROPRIETARY,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
-NO_LICENSE,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
+PROPRIETARY,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,0,0,0,0,0,0,0,0,0,0
+NO_LICENSE,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,0,0,0,0,0,0,0,0,0,0
```

### Comparing `licensecheck-2023.2/licensecheck/packageinfo.py` & `licensecheck-2023.3/licensecheck/packageinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from __future__ import annotations
 
 import configparser
 from importlib import metadata
 from pathlib import Path
 from typing import Any
 
-import requests
 import tomli
 
-from licensecheck.types import JOINS, UNKNOWN, PackageInfo
+from licensecheck.types import JOINS, UNKNOWN, PackageInfo, session, ucstr
 
 
-def getPackageInfoLocal(requirement: str) -> PackageInfo:
+def getPackageInfoLocal(requirement: ucstr) -> PackageInfo:
 	"""Get package info from local files including version, author
 	and	the license.
 
 	:param str requirement: name of the package
 	:raises ModuleNotFoundError: if the package does not exist
 	:return PackageInfo: package information
 	"""
@@ -39,47 +38,47 @@
 		# append to pkgInfo
 		return PackageInfo(
 			name=name,
 			version=version,
 			homePage=homePage,
 			author=author,
 			size=size,
-			license=lice,
+			license=ucstr(lice),
 		)
 
 	except metadata.PackageNotFoundError as error:
 		raise ModuleNotFoundError from error
 
 
-def getPackageInfoPypi(requirement: str) -> PackageInfo:
+def getPackageInfoPypi(requirement: ucstr) -> PackageInfo:
 	"""Get package info from local files including version, author
 	and	the license.
 
 	:param str requirement: name of the package
 	:raises ModuleNotFoundError: if the package does not exist
 	:return PackageInfo: package information
 	"""
-	request = requests.get(f"https://pypi.org/pypi/{requirement}/json", timeout=60)
+	request = session.get(f"https://pypi.org/pypi/{requirement}/json", timeout=60)
 	response = request.json()
 	try:
 		info = response["info"]
 		licenseClassifier = licenseFromClassifierlist(info["classifiers"])
 		return PackageInfo(
-			name=requirement,
+			name=info["name"],
 			version=info["version"],
 			homePage=info["home_page"],
 			author=info["author"],
 			size=int(response["urls"][-1]["size"]),
-			license=licenseClassifier if licenseClassifier != UNKNOWN else info["license"],
+			license=ucstr(licenseClassifier if licenseClassifier != UNKNOWN else info["license"]),
 		)
 	except KeyError as error:
 		raise ModuleNotFoundError from error
 
 
-def licenseFromClassifierlist(classifiers: list[str]) -> str:
+def licenseFromClassifierlist(classifiers: list[str]) -> ucstr:
 	"""Get license string from a list of project classifiers.
 
 	Args:
 		classifiers (list[str]): list of classifiers
 
 	Returns:
 		str: the license name
@@ -88,22 +87,22 @@
 		return UNKNOWN
 	licenses = []
 	for val in classifiers:
 		if val.startswith("License"):
 			lice = val.split(" :: ")[-1]
 			if lice != "OSI Approved":
 				licenses.append(lice)
-	return JOINS.join(licenses) if len(licenses) > 0 else UNKNOWN
+	return ucstr(JOINS.join(licenses) if len(licenses) > 0 else UNKNOWN)
 
 
-def getPackages(reqs: set[str]) -> set[PackageInfo]:
+def getPackages(reqs: set[ucstr]) -> set[PackageInfo]:
 	"""Get dependency info.
 
 	Args:
-		reqs (set[str]): set of dependency names to gather info on
+		reqs (set[ucstr]): set of dependency names to gather info on
 
 	Returns:
 		set[PackageInfo]: set of dependencies
 	"""
 	packageinfo = set()
 	for requirement in reqs:
 		try:
@@ -117,15 +116,15 @@
 	return packageinfo
 
 
 def getMyPackageMetadata() -> dict[str, Any]:
 	"""Get the package classifiers and license from "setup.cfg", "pyproject.toml"
 
 	Returns:
-		dict[str, Any]: {"classifiers": list[str], "license": str}
+		dict[str, Any]: {"classifiers": list[str], "license": ucstr}
 	"""
 	if Path("setup.cfg").exists():
 		config = configparser.ConfigParser()
 		config.read("setup.cfg")
 		if "metadata" in config.sections() and "license" in config["metadata"]:
 			return config["metadata"].__dict__
 	if Path("pyproject.toml").exists():
@@ -134,35 +133,35 @@
 		if "poetry" in tool:
 			return tool["poetry"]
 		if "flit" in tool:
 			return tool["flit"]["metadata"]
 		if pyproject.get("project") is not None:
 			return pyproject["project"]
 
-	return {"classifiers": [], "license": ""}
+	return {"classifiers": [], "license": ucstr("")}
 
 
-def getMyPackageLicense() -> str:
+def getMyPackageLicense() -> ucstr:
 	"""Get the package license from "setup.cfg", "pyproject.toml" or user input
 
 	Returns:
 		str: license name
 	"""
 	metaData = getMyPackageMetadata()
 	licenseClassifier = licenseFromClassifierlist(metaData.get("classifiers", []))
 	if licenseClassifier != UNKNOWN:
 		return licenseClassifier
 	if "license" in metaData:
 		if isinstance(metaData["license"], dict) and metaData["license"].get("text") is not None:
-			return str(metaData["license"].get("text"))
-		return str(metaData["license"])
-	return input("Enter the project license\n>")
+			return ucstr(metaData["license"].get("text"))
+		return ucstr(metaData["license"])
+	return ucstr(input("Enter the project license\n>"))
 
 
-def getModuleSize(path: Path, name: str) -> int:
+def getModuleSize(path: Path, name: ucstr) -> int:
 	"""Get the size of a given module as an int.
 
 	Args:
 		path (Path): path to package
 		name (str): name of package
 
 	Returns:
@@ -175,10 +174,12 @@
 			for f in path.glob("**/*")
 			if f.is_file() and "__pycache__" not in str(f)
 		)
 	except AttributeError:
 		pass
 	if size > 0:
 		return size
-	request = requests.get(f"https://pypi.org/pypi/{name}/json", timeout=60)
+	request = session.get(f"https://pypi.org/pypi/{name}/json", timeout=60)
+	if request.status_code != 200:
+		return 0
 	response = request.json()
 	return int(response["urls"][-1]["size"])
```

### Comparing `licensecheck-2023.2/licensecheck/pypi_licenses/osi_approved.txt` & `licensecheck-2023.3/licensecheck/pypi_licenses/osi_approved.txt`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.2/licensecheck/pypi_licenses/other.txt` & `licensecheck-2023.3/licensecheck/pypi_licenses/other.txt`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.2/licensecheck/types.py` & `licensecheck-2023.3/licensecheck/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 """PackageCompat type.
 """
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
+from pathlib import Path
 
-UNKNOWN = "UNKNOWN"
-JOINS = ";; "
+THISDIR = Path(__file__).resolve().parent
+
+import requests_cache
+
+session = requests_cache.CachedSession(f"{THISDIR}/licensecheck")
+
+
+class ucstr(str):
+	"""Uppercase string"""
+
+	def __new__(cls, v) -> ucstr:
+		return super().__new__(cls, v.upper())
+
+
+UNKNOWN = ucstr("UNKNOWN")
+JOINS = ucstr(";; ")
 
 
 @dataclass(unsafe_hash=True, order=True)
 class PackageInfo:
 	"""PackageInfo type."""
 
 	name: str
 	version: str = UNKNOWN
 	namever: str = field(init=False)
 	size: int = -1
 	homePage: str = UNKNOWN
 	author: str = UNKNOWN
-	license: str = UNKNOWN
+	license: ucstr = UNKNOWN
 	licenseCompat: bool = False
 	errorCode: int = 0
 
 	def __post_init__(self):
 		self.namever = f"{self.name}-{self.version}"
 
 
@@ -74,39 +89,39 @@
 	"""Output a license as plain text
 
 	:param L licenseEnum: License
 	:return str: license of plain text
 	"""
 
 	licenseMap = {
-		L.PUBLIC: "public domain/ cc-pddc/ cc0-1.0",
-		L.UNLICENSE: "unlicense/ wtfpl",
-		L.BOOST: "boost/ bsl-1.0",
-		L.MIT: "mit",
-		L.BSD: "bsd",
-		L.ISC: "isc",
-		L.NCSA: "ncsa",
-		L.PSFL: "python/ psf-2.0",
-		L.APACHE: "apache",
-		L.ECLIPSE: "eclipse",
-		L.ACADEMIC_FREE: "afl",
-		L.LGPL_2_PLUS: "lgplv2+/ lgpl-2.0-or-later",
-		L.LGPL_3_PLUS: "lgplv3+/ lgpl-3.0-or-later",
-		L.LGPL_2: "lgpl-2.0-only/ lgplv2",
-		L.LGPL_3: "lgpl-3.0-only/ lgplv3",
-		L.LGPL_X: "lgpl",
-		L.AGPL_3_PLUS: "agpl",
-		L.GPL_2_PLUS: "gpl-2.0-or-later/ gplv2+",
-		L.GPL_3_PLUS: "gpl-3.0-or-later/ gplv3+",
-		L.GPL_2: "gplv2/ gpl-2.0",
-		L.GPL_3: "gplv3/ gpl-3.0",
-		L.GPL_X: "gpl",
-		L.MPL: "mpl",
-		L.EU: "eupl",
-		L.PROPRIETARY: "proprietary",
-		L.NO_LICENSE: "no license/ unknown",
+		L.PUBLIC: "PUBLIC DOMAIN/ CC-PDDC/ CC0-1.0",
+		L.UNLICENSE: "UNLICENSE/ WTFPL",
+		L.BOOST: "BOOST/ BSL-1.0",
+		L.MIT: "MIT",
+		L.BSD: "BSD",
+		L.ISC: "ISC",
+		L.NCSA: "NCSA",
+		L.PSFL: "PYTHON/ PSF-2.0",
+		L.APACHE: "APACHE",
+		L.ECLIPSE: "ECLIPSE",
+		L.ACADEMIC_FREE: "AFL",
+		L.LGPL_2_PLUS: "LGPLV2+/ LGPL-2.0-OR-LATER",
+		L.LGPL_3_PLUS: "LGPLV3+/ LGPL-3.0-OR-LATER",
+		L.LGPL_2: "LGPL-2.0-ONLY/ LGPLV2",
+		L.LGPL_3: "LGPL-3.0-ONLY/ LGPLV3",
+		L.LGPL_X: "LGPL",
+		L.AGPL_3_PLUS: "AGPL",
+		L.GPL_2_PLUS: "GPL-2.0-OR-LATER/ GPLV2+",
+		L.GPL_3_PLUS: "GPL-3.0-OR-LATER/ GPLV3+",
+		L.GPL_2: "GPLV2/ GPL-2.0",
+		L.GPL_3: "GPLV3/ GPL-3.0",
+		L.GPL_X: "GPL",
+		L.MPL: "MPL",
+		L.EU: "EUPL",
+		L.PROPRIETARY: "PROPRIETARY",
+		L.NO_LICENSE: "NO LICENSE/ UNKNOWN",
 	}
 
 	if licenseEnum not in licenseMap:
-		return "no license/ unknown"
+		return "NO LICENSE/ UNKNOWN LICENSE"
 
-	return licenseMap[licenseEnum]
+	return f"{licenseMap[licenseEnum]} LICENSE"
```

### Comparing `licensecheck-2023.2/pyproject.toml` & `licensecheck-2023.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "licensecheck"
-version = "2023.2"
+version = "2023.3"
 license = "mit"
 description = "Output the licenses used by dependencies and check if these are compatible with the project license"
 authors = ["FredHappyface"]
 classifiers = [
 	"Environment :: Console",
 	"Environment :: MacOS X",
 	"Environment :: Win32 (MS Windows)",
@@ -24,18 +24,20 @@
 readme = "README.md"
 
 [tool.poetry.scripts]
 licensecheck = 'licensecheck:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8"
+requirements-parser = "<2,>=0.5.0"
 requests = "<3,>=2.31.0"
 fhconfparser = "<2024,>=2022"
 tomli = "<3,>=2.0.1"
 rich = "<14,>=13.4.2"
+requests-cache = "<2,>=1.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pylint = "^2.13.5"
 handsdown = "^1.1.0"
 coverage = "^6.3.2"
```

### Comparing `licensecheck-2023.2/README.md` & `licensecheck-2023.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 [![PyPI Version](https://img.shields.io/pypi/v/licensecheck.svg?style=for-the-badge)](https://pypi.org/project/licensecheck)
 
 <!-- omit in toc -->
 # LicenseCheck
 
 <img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
 
+NOTICE: I am not a lawyer (IANAL)
+
+**Any output provided by this software is for general informational purposes only and
+should not be construed as legal advice. I am not a lawyer and there is no guarantee that the
+information provided here is complete or correct. Any reliance on the information provided by this
+software is at your own risk.**
+
+See also: https://en.wikipedia.org/wiki/IANAL, [project license (MIT)](/LICENSE.md)
+
 Output the licences used by dependencies and check if these are compatible with
 the project license
 
 <!-- omit in toc -->
 ## Table of Contents
 
 - [Examples from the command-line](#examples-from-the-command-line)
```

### Comparing `licensecheck-2023.2/setup.py` & `licensecheck-2023.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 ['licensecheck']
 
 package_data = \
 {'': ['*'], 'licensecheck': ['pypi_licenses/*']}
 
 install_requires = \
 ['fhconfparser>=2022,<2024',
+ 'requests-cache>=1.1.0,<2',
  'requests>=2.31.0,<3',
+ 'requirements-parser>=0.5.0,<2',
  'rich>=13.4.2,<14',
  'tomli>=2.0.1,<3']
 
 entry_points = \
 {'console_scripts': ['licensecheck = licensecheck:cli']}
 
 setup_kwargs = {
     'name': 'licensecheck',
-    'version': '2023.2',
+    'version': '2023.3',
     'description': 'Output the licenses used by dependencies and check if these are compatible with the project license',
-    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/licensecheck.svg?style=for-the-badge)](https://pypistats.org/packages/licensecheck)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Flicensecheck)](https://pepy.tech/project/licensecheck)\n[![PyPI Version](https://img.shields.io/pypi/v/licensecheck.svg?style=for-the-badge)](https://pypi.org/project/licensecheck)\n\n<!-- omit in toc -->\n# LicenseCheck\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nOutput the licences used by dependencies and check if these are compatible with\nthe project license\n\n<!-- omit in toc -->\n## Table of Contents\n\n- [Examples from the command-line](#examples-from-the-command-line)\n\t- [Using requirements](#using-requirements)\n\t- [Failing on packages under MIT license](#failing-on-packages-under-mit-license)\n\t- [Custom requirements.txt in json format](#custom-requirementstxt-in-json-format)\n\t- [Poetry with dev requirements](#poetry-with-dev-requirements)\n\t- [PEP 631 (with or without optional dependencies)](#pep-631-with-or-without-optional-dependencies)\n- [Help](#help)\n- [Configuration Example](#configuration-example)\n\t- [Example 1: pyproject.toml](#example-1-pyprojecttoml)\n\t- [Example 2: licensecheck.json](#example-2-licensecheckjson)\n\t- [Example 3: licensecheck.ini](#example-3-licensecheckini)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Examples from the command-line\n\nSee below for the output if you run `licensecheck` in this directory\n\n```txt\n>> licensecheck\n\n                             list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                           ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ urllib3             │ MIT License                          │\n│ ✔          │ types-setuptools    │ Apache Software License              │\n│ ✔          │ tomli               │ MIT License                          │\n│ ✔          │ idna                │ BSD License                          │\n│ ✔          │ Pygments            │ BSD License                          │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0) │\n│ ✔          │ fhconfparser        │ MIT License                          │\n│ ✔          │ rich                │ MIT License                          │\n│ ✔          │ charset-normalizer  │ MIT License                          │\n│ ✔          │ requirements-parser │ Apache Software License              │\n│ ✔          │ commonmark          │ BSD License                          │\n│ ✔          │ requests            │ Apache Software License              │\n│ ✔          │ attrs               │ MIT License                          │\n└────────────┴─────────────────────┴──────────────────────────────────────┘\n```\n\n### Using requirements\n\n```txt\n>> licensecheck -u requirements\n\n                       list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)              ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ requirements-parser │ Apache Software License │\n│ ✔          │ requests            │ Apache Software License │\n│ ✔          │ rich                │ MIT License             │\n│ ✔          │ fhconfparser        │ MIT License             │\n│ ✔          │ tomli               │ MIT License             │\n└────────────┴─────────────────────┴─────────────────────────┘\n```\n\n### Failing on packages under MIT license\n\n```txt\n>> licensecheck --fail-licenses mit\n\n                             list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                           ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ idna                │ BSD License                          │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0) │\n│ ✔          │ Pygments            │ BSD License                          │\n│ ✔          │ commonmark          │ BSD License                          │\n│ ✔          │ requirements-parser │ Apache Software License              │\n│ ✖          │ fhconfparser        │ MIT License                          │\n│ ✖          │ tomli               │ MIT License                          │\n│ ✔          │ types-setuptools    │ Apache Software License              │\n│ ✖          │ attrs               │ MIT License                          │\n│ ✖          │ charset-normalizer  │ MIT License                          │\n│ ✖          │ rich                │ MIT License                          │\n│ ✖          │ urllib3             │ MIT License                          │\n│ ✔          │ requests            │ Apache Software License              │\n└────────────┴─────────────────────┴──────────────────────────────────────┘\n```\n\n### Custom requirements.txt in json format\n\nAdd optional path to requirements.txt as outlined in https://github.com/FHPythonUtils/LicenseCheck/issues/9#issuecomment-898878228. Eg. `licensecheck --using requirements:c:/path/to/reqs.txt;path/to/other/reqs.txt`\n\n```txt\n>> licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json\n{\n\t"info": {\n\t\t"program": "licensecheck",\n\t\t"version": "2022.2.0"\n\t},\n\t"packages": [\n\t\t{\n\t\t\t"name": "requests",\n\t\t\t"version": "2.28.1",\n\t\t\t"namever": "requests-2.28.1",\n\t\t\t"size": 180253,\n\t\t\t"homePage": "https://requests.readthedocs.io",\n\t\t\t"author": "Kenneth Reitz",\n\t\t\t"license": "Apache Software License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "rich",\n\t\t\t"version": "12.6.0",\n\t\t\t"namever": "rich-12.6.0",\n\t\t\t"size": 905975,\n\t\t\t"homePage": "https://github.com/willmcgugan/rich",\n\t\t\t"author": "Will McGugan",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "tomli",\n\t\t\t"version": "2.0.1",\n\t\t\t"namever": "tomli-2.0.1",\n\t\t\t"size": 26252,\n\t\t\t"homePage": "UNKNOWN",\n\t\t\t"author": "UNKNOWN",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "requirements-parser",\n\t\t\t"version": "0.5.0",\n\t\t\t"namever": "requirements-parser-0.5.0",\n\t\t\t"size": 11523,\n\t\t\t"homePage": "https://github.com/madpah/requirements-parser",\n\t\t\t"author": "Paul Horton",\n\t\t\t"license": "Apache Software License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "fhconfparser",\n\t\t\t"version": "2022",\n\t\t\t"namever": "fhconfparser-2022",\n\t\t\t"size": 14586,\n\t\t\t"homePage": "https://github.com/FHPythonUtils/FHConfParser",\n\t\t\t"author": "FredHappyface",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t}\n\t]\n}\n```\n\n### Poetry with dev requirements\n\nAdd `-u poetry:dev` to command-line to include dev packages (excluded by default)\n\n```txt\n>> licensecheck -u poetry:dev\n\n                                  list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                                    ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ astroid             │ GNU Lesser General Public License v2 (LGPLv2) │\n│ ✔          │ rich                │ MIT License                                   │\n│ ✔          │ types-setuptools    │ Apache Software License                       │\n│ ✔          │ fhconfparser        │ MIT License                                   │\n│ ✔          │ typed-ast           │ Apache License 2.0                            │\n│ ✔          │ py                  │ MIT License                                   │\n│ ✔          │ mccabe              │ MIT License                                   │\n│ ✔          │ tomlkit             │ MIT License                                   │\n│ ✔          │ coverage            │ Apache Software License                       │\n│ ✔          │ Pygments            │ BSD License                                   │\n│ ✔          │ requests            │ Apache Software License                       │\n│ ✔          │ requirements-parser │ Apache Software License                       │\n│ ✔          │ tomli               │ MIT License                                   │\n│ ✔          │ pluggy              │ MIT License                                   │\n│ ✔          │ isort               │ MIT License                                   │\n│ ✔          │ urllib3             │ MIT License                                   │\n│ ✖          │ pylint              │ GNU General Public License v2 (GPLv2)         │\n│ ✔          │ iniconfig           │ MIT License                                   │\n│ ✔          │ wrapt               │ BSD License                                   │\n│ ✔          │ pytest              │ MIT License                                   │\n│ ✔          │ pip                 │ MIT License                                   │\n│ ✔          │ charset-normalizer  │ MIT License                                   │\n│ ✔          │ packaging           │ Apache Software License, BSD License          │\n│ ✔          │ commonmark          │ BSD License                                   │\n│ ✔          │ lazy-object-proxy   │ BSD License                                   │\n│ ✔          │ platformdirs        │ MIT License                                   │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0)          │\n│ ✔          │ colorama            │ BSD License                                   │\n│ ✔          │ attrs               │ MIT License                                   │\n│ ✔          │ dill                │ BSD License                                   │\n│ ✔          │ idna                │ BSD License                                   │\n│ ✔          │ importlib-resources │ Apache Software License                       │\n│ ✔          │ handsdown           │ MIT License                                   │\n│ ✔          │ pyparsing           │ MIT License                                   │\n└────────────┴─────────────────────┴───────────────────────────────────────────────┘\n```\n\n### PEP 631 (with or without optional dependencies)\n\nPEP 631 mode enables support for reading dependency information from `pyproject.toml` in the format specified by PEP 631.\nThis format is used by build systems such as hatch.\n\nYou can enable this mode by using `-u PEP631`, and include the optional dependencies of extras by using `-u PEP631:tests;dev;docs`,\nbut it\'s recommended to use this instead:\n\n```toml\n[tool.licensecheck]\nusing = "PEP631"\n\n# OR\n\n[tool.licensecheck]\nusing = "PEP631:tests;dev;docs"\n```\n\nBy default no optional dependencies are included.\n\n## Help\n\n```txt\nusage: __main__.py [-h] [--format FORMAT] [--file FILE] [--using USING]\n                   [--ignore-packages IGNORE_PACKAGES [IGNORE_PACKAGES ...]]\n                   [--fail-packages FAIL_PACKAGES [FAIL_PACKAGES ...]]\n                   [--ignore-licenses IGNORE_LICENSES [IGNORE_LICENSES ...]]\n                   [--fail-licenses FAIL_LICENSES [FAIL_LICENSES ...]] [--zero]\n\nOutput the licenses used by dependencies and check if these are compatible with the project license.\n\noptions:\n  -h, --help            show this help message and exit\n  --format FORMAT, -f FORMAT\n                        Output format. one of: json, markdown, csv, ansi, simple. default=simple\n  --file FILE, -o FILE  Filename to write to (omit for stdout)\n  --using USING, -u USING\n                        Environment to use e.g. requirements.txt. one of: requirements, poetry, PEP631. default=poetry\n  --ignore-packages IGNORE_PACKAGES [IGNORE_PACKAGES ...]\n                        a list of packages to ignore (compat=True)\n  --fail-packages FAIL_PACKAGES [FAIL_PACKAGES ...]\n                        a list of packages to fail (compat=False)\n  --ignore-licenses IGNORE_LICENSES [IGNORE_LICENSES ...]\n                        a list of licenses to ignore (skipped, compat may still be False)\n  --fail-licenses FAIL_LICENSES [FAIL_LICENSES ...]\n                        a list of licenses to fail (compat=False)\n  --zero, -0            Return non zero exit code if an incompatible license is found\n```\n\nYou can also import this into your own project and use any of the functions\nin the DOCS\n\n## Configuration Example\n\nConfiguration files are parsed in the following order: `pyproject.toml`,\n`setup.cfg`, `licensecheck.toml`, `licensecheck.json`, `licensecheck.ini`,\n`~/licensecheck.toml`, `~/licensecheck.json`, `~/licensecheck.ini`\n\n- ⚠ All config files are parsed, however configuration defined in previous files takes precedent\n\nAdd optional path to requirements.txt as outlined in\nhttps://github.com/FHPythonUtils/LicenseCheck/issues/9#issuecomment-898878228\nfor example: `licensecheck --using requirements:c:/path/to/reqs.txt;path/to/other/reqs.txt`\n\n### Example 1: pyproject.toml\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```toml\n[tool.licensecheck]\nusing = "requirements:requirements.txt;requirements_optional.txt"\nformat = "json"\n```\n\n### Example 2: licensecheck.json\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```json\n{\n\t"tool": {\n\t\t"licensecheck": {\n\t\t\t"using": "requirements:requirements.txt;requirements_optional.txt",\n\t\t\t"format": "json"\n\t\t}\n\t}\n}\n```\n\n### Example 3: licensecheck.ini\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```ini\n[licensecheck]\nusing = "requirements:requirements.txt;requirements_optional.txt"\nformat = "json"\n```\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install licensecheck\n```\n\nHead to https://pypi.org/project/licensecheck/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/LicenseCheck\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
+    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/licensecheck.svg?style=for-the-badge)](https://pypistats.org/packages/licensecheck)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Flicensecheck)](https://pepy.tech/project/licensecheck)\n[![PyPI Version](https://img.shields.io/pypi/v/licensecheck.svg?style=for-the-badge)](https://pypi.org/project/licensecheck)\n\n<!-- omit in toc -->\n# LicenseCheck\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nNOTICE: I am not a lawyer (IANAL)\n\n**Any output provided by this software is for general informational purposes only and\nshould not be construed as legal advice. I am not a lawyer and there is no guarantee that the\ninformation provided here is complete or correct. Any reliance on the information provided by this\nsoftware is at your own risk.**\n\nSee also: https://en.wikipedia.org/wiki/IANAL, [project license (MIT)](/LICENSE.md)\n\nOutput the licences used by dependencies and check if these are compatible with\nthe project license\n\n<!-- omit in toc -->\n## Table of Contents\n\n- [Examples from the command-line](#examples-from-the-command-line)\n\t- [Using requirements](#using-requirements)\n\t- [Failing on packages under MIT license](#failing-on-packages-under-mit-license)\n\t- [Custom requirements.txt in json format](#custom-requirementstxt-in-json-format)\n\t- [Poetry with dev requirements](#poetry-with-dev-requirements)\n\t- [PEP 631 (with or without optional dependencies)](#pep-631-with-or-without-optional-dependencies)\n- [Help](#help)\n- [Configuration Example](#configuration-example)\n\t- [Example 1: pyproject.toml](#example-1-pyprojecttoml)\n\t- [Example 2: licensecheck.json](#example-2-licensecheckjson)\n\t- [Example 3: licensecheck.ini](#example-3-licensecheckini)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Examples from the command-line\n\nSee below for the output if you run `licensecheck` in this directory\n\n```txt\n>> licensecheck\n\n                             list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                           ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ urllib3             │ MIT License                          │\n│ ✔          │ types-setuptools    │ Apache Software License              │\n│ ✔          │ tomli               │ MIT License                          │\n│ ✔          │ idna                │ BSD License                          │\n│ ✔          │ Pygments            │ BSD License                          │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0) │\n│ ✔          │ fhconfparser        │ MIT License                          │\n│ ✔          │ rich                │ MIT License                          │\n│ ✔          │ charset-normalizer  │ MIT License                          │\n│ ✔          │ requirements-parser │ Apache Software License              │\n│ ✔          │ commonmark          │ BSD License                          │\n│ ✔          │ requests            │ Apache Software License              │\n│ ✔          │ attrs               │ MIT License                          │\n└────────────┴─────────────────────┴──────────────────────────────────────┘\n```\n\n### Using requirements\n\n```txt\n>> licensecheck -u requirements\n\n                       list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)              ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ requirements-parser │ Apache Software License │\n│ ✔          │ requests            │ Apache Software License │\n│ ✔          │ rich                │ MIT License             │\n│ ✔          │ fhconfparser        │ MIT License             │\n│ ✔          │ tomli               │ MIT License             │\n└────────────┴─────────────────────┴─────────────────────────┘\n```\n\n### Failing on packages under MIT license\n\n```txt\n>> licensecheck --fail-licenses mit\n\n                             list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                           ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ idna                │ BSD License                          │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0) │\n│ ✔          │ Pygments            │ BSD License                          │\n│ ✔          │ commonmark          │ BSD License                          │\n│ ✔          │ requirements-parser │ Apache Software License              │\n│ ✖          │ fhconfparser        │ MIT License                          │\n│ ✖          │ tomli               │ MIT License                          │\n│ ✔          │ types-setuptools    │ Apache Software License              │\n│ ✖          │ attrs               │ MIT License                          │\n│ ✖          │ charset-normalizer  │ MIT License                          │\n│ ✖          │ rich                │ MIT License                          │\n│ ✖          │ urllib3             │ MIT License                          │\n│ ✔          │ requests            │ Apache Software License              │\n└────────────┴─────────────────────┴──────────────────────────────────────┘\n```\n\n### Custom requirements.txt in json format\n\nAdd optional path to requirements.txt as outlined in https://github.com/FHPythonUtils/LicenseCheck/issues/9#issuecomment-898878228. Eg. `licensecheck --using requirements:c:/path/to/reqs.txt;path/to/other/reqs.txt`\n\n```txt\n>> licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json\n{\n\t"info": {\n\t\t"program": "licensecheck",\n\t\t"version": "2022.2.0"\n\t},\n\t"packages": [\n\t\t{\n\t\t\t"name": "requests",\n\t\t\t"version": "2.28.1",\n\t\t\t"namever": "requests-2.28.1",\n\t\t\t"size": 180253,\n\t\t\t"homePage": "https://requests.readthedocs.io",\n\t\t\t"author": "Kenneth Reitz",\n\t\t\t"license": "Apache Software License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "rich",\n\t\t\t"version": "12.6.0",\n\t\t\t"namever": "rich-12.6.0",\n\t\t\t"size": 905975,\n\t\t\t"homePage": "https://github.com/willmcgugan/rich",\n\t\t\t"author": "Will McGugan",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "tomli",\n\t\t\t"version": "2.0.1",\n\t\t\t"namever": "tomli-2.0.1",\n\t\t\t"size": 26252,\n\t\t\t"homePage": "UNKNOWN",\n\t\t\t"author": "UNKNOWN",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "requirements-parser",\n\t\t\t"version": "0.5.0",\n\t\t\t"namever": "requirements-parser-0.5.0",\n\t\t\t"size": 11523,\n\t\t\t"homePage": "https://github.com/madpah/requirements-parser",\n\t\t\t"author": "Paul Horton",\n\t\t\t"license": "Apache Software License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "fhconfparser",\n\t\t\t"version": "2022",\n\t\t\t"namever": "fhconfparser-2022",\n\t\t\t"size": 14586,\n\t\t\t"homePage": "https://github.com/FHPythonUtils/FHConfParser",\n\t\t\t"author": "FredHappyface",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t}\n\t]\n}\n```\n\n### Poetry with dev requirements\n\nAdd `-u poetry:dev` to command-line to include dev packages (excluded by default)\n\n```txt\n>> licensecheck -u poetry:dev\n\n                                  list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                                    ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ astroid             │ GNU Lesser General Public License v2 (LGPLv2) │\n│ ✔          │ rich                │ MIT License                                   │\n│ ✔          │ types-setuptools    │ Apache Software License                       │\n│ ✔          │ fhconfparser        │ MIT License                                   │\n│ ✔          │ typed-ast           │ Apache License 2.0                            │\n│ ✔          │ py                  │ MIT License                                   │\n│ ✔          │ mccabe              │ MIT License                                   │\n│ ✔          │ tomlkit             │ MIT License                                   │\n│ ✔          │ coverage            │ Apache Software License                       │\n│ ✔          │ Pygments            │ BSD License                                   │\n│ ✔          │ requests            │ Apache Software License                       │\n│ ✔          │ requirements-parser │ Apache Software License                       │\n│ ✔          │ tomli               │ MIT License                                   │\n│ ✔          │ pluggy              │ MIT License                                   │\n│ ✔          │ isort               │ MIT License                                   │\n│ ✔          │ urllib3             │ MIT License                                   │\n│ ✖          │ pylint              │ GNU General Public License v2 (GPLv2)         │\n│ ✔          │ iniconfig           │ MIT License                                   │\n│ ✔          │ wrapt               │ BSD License                                   │\n│ ✔          │ pytest              │ MIT License                                   │\n│ ✔          │ pip                 │ MIT License                                   │\n│ ✔          │ charset-normalizer  │ MIT License                                   │\n│ ✔          │ packaging           │ Apache Software License, BSD License          │\n│ ✔          │ commonmark          │ BSD License                                   │\n│ ✔          │ lazy-object-proxy   │ BSD License                                   │\n│ ✔          │ platformdirs        │ MIT License                                   │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0)          │\n│ ✔          │ colorama            │ BSD License                                   │\n│ ✔          │ attrs               │ MIT License                                   │\n│ ✔          │ dill                │ BSD License                                   │\n│ ✔          │ idna                │ BSD License                                   │\n│ ✔          │ importlib-resources │ Apache Software License                       │\n│ ✔          │ handsdown           │ MIT License                                   │\n│ ✔          │ pyparsing           │ MIT License                                   │\n└────────────┴─────────────────────┴───────────────────────────────────────────────┘\n```\n\n### PEP 631 (with or without optional dependencies)\n\nPEP 631 mode enables support for reading dependency information from `pyproject.toml` in the format specified by PEP 631.\nThis format is used by build systems such as hatch.\n\nYou can enable this mode by using `-u PEP631`, and include the optional dependencies of extras by using `-u PEP631:tests;dev;docs`,\nbut it\'s recommended to use this instead:\n\n```toml\n[tool.licensecheck]\nusing = "PEP631"\n\n# OR\n\n[tool.licensecheck]\nusing = "PEP631:tests;dev;docs"\n```\n\nBy default no optional dependencies are included.\n\n## Help\n\n```txt\nusage: __main__.py [-h] [--format FORMAT] [--file FILE] [--using USING]\n                   [--ignore-packages IGNORE_PACKAGES [IGNORE_PACKAGES ...]]\n                   [--fail-packages FAIL_PACKAGES [FAIL_PACKAGES ...]]\n                   [--ignore-licenses IGNORE_LICENSES [IGNORE_LICENSES ...]]\n                   [--fail-licenses FAIL_LICENSES [FAIL_LICENSES ...]] [--zero]\n\nOutput the licenses used by dependencies and check if these are compatible with the project license.\n\noptions:\n  -h, --help            show this help message and exit\n  --format FORMAT, -f FORMAT\n                        Output format. one of: json, markdown, csv, ansi, simple. default=simple\n  --file FILE, -o FILE  Filename to write to (omit for stdout)\n  --using USING, -u USING\n                        Environment to use e.g. requirements.txt. one of: requirements, poetry, PEP631. default=poetry\n  --ignore-packages IGNORE_PACKAGES [IGNORE_PACKAGES ...]\n                        a list of packages to ignore (compat=True)\n  --fail-packages FAIL_PACKAGES [FAIL_PACKAGES ...]\n                        a list of packages to fail (compat=False)\n  --ignore-licenses IGNORE_LICENSES [IGNORE_LICENSES ...]\n                        a list of licenses to ignore (skipped, compat may still be False)\n  --fail-licenses FAIL_LICENSES [FAIL_LICENSES ...]\n                        a list of licenses to fail (compat=False)\n  --zero, -0            Return non zero exit code if an incompatible license is found\n```\n\nYou can also import this into your own project and use any of the functions\nin the DOCS\n\n## Configuration Example\n\nConfiguration files are parsed in the following order: `pyproject.toml`,\n`setup.cfg`, `licensecheck.toml`, `licensecheck.json`, `licensecheck.ini`,\n`~/licensecheck.toml`, `~/licensecheck.json`, `~/licensecheck.ini`\n\n- ⚠ All config files are parsed, however configuration defined in previous files takes precedent\n\nAdd optional path to requirements.txt as outlined in\nhttps://github.com/FHPythonUtils/LicenseCheck/issues/9#issuecomment-898878228\nfor example: `licensecheck --using requirements:c:/path/to/reqs.txt;path/to/other/reqs.txt`\n\n### Example 1: pyproject.toml\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```toml\n[tool.licensecheck]\nusing = "requirements:requirements.txt;requirements_optional.txt"\nformat = "json"\n```\n\n### Example 2: licensecheck.json\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```json\n{\n\t"tool": {\n\t\t"licensecheck": {\n\t\t\t"using": "requirements:requirements.txt;requirements_optional.txt",\n\t\t\t"format": "json"\n\t\t}\n\t}\n}\n```\n\n### Example 3: licensecheck.ini\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```ini\n[licensecheck]\nusing = "requirements:requirements.txt;requirements_optional.txt"\nformat = "json"\n```\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install licensecheck\n```\n\nHead to https://pypi.org/project/licensecheck/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/LicenseCheck\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
     'author': 'FredHappyface',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FHPythonUtils/LicenseCheck',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `licensecheck-2023.2/PKG-INFO` & `licensecheck-2023.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensecheck
-Version: 2023.2
+Version: 2023.3
 Summary: Output the licenses used by dependencies and check if these are compatible with the project license
 Home-page: https://github.com/FHPythonUtils/LicenseCheck
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -22,14 +22,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: fhconfparser (>=2022,<2024)
 Requires-Dist: requests (>=2.31.0,<3)
+Requires-Dist: requests-cache (>=1.1.0,<2)
+Requires-Dist: requirements-parser (>=0.5.0,<2)
 Requires-Dist: rich (>=13.4.2,<14)
 Requires-Dist: tomli (>=2.0.1,<3)
 Project-URL: Documentation, https://github.com/FHPythonUtils/LicenseCheck/blob/master/README.md
 Project-URL: Repository, https://github.com/FHPythonUtils/LicenseCheck
 Description-Content-Type: text/markdown
 
 [![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)
@@ -43,14 +45,23 @@
 [![PyPI Version](https://img.shields.io/pypi/v/licensecheck.svg?style=for-the-badge)](https://pypi.org/project/licensecheck)
 
 <!-- omit in toc -->
 # LicenseCheck
 
 <img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
 
+NOTICE: I am not a lawyer (IANAL)
+
+**Any output provided by this software is for general informational purposes only and
+should not be construed as legal advice. I am not a lawyer and there is no guarantee that the
+information provided here is complete or correct. Any reliance on the information provided by this
+software is at your own risk.**
+
+See also: https://en.wikipedia.org/wiki/IANAL, [project license (MIT)](/LICENSE.md)
+
 Output the licences used by dependencies and check if these are compatible with
 the project license
 
 <!-- omit in toc -->
 ## Table of Contents
 
 - [Examples from the command-line](#examples-from-the-command-line)
```

