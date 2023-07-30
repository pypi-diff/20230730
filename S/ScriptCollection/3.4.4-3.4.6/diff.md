# Comparing `tmp/ScriptCollection-3.4.4-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 62443 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat    19324 b- defN 23-Jul-17 20:11 ScriptCollection/Executables.py
+Zip file size: 62178 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat    19002 b- defN 23-Jul-30 11:22 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34378 b- defN 23-Jun-27 21:57 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    96159 b- defN 23-Jul-17 20:11 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   144595 b- defN 23-Jul-17 20:11 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    94554 b- defN 23-Jul-30 11:34 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   145487 b- defN 23-Jul-30 11:34 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/RECORD
-14 files, 324746 bytes uncompressed, 60261 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/RECORD
+14 files, 323711 bytes uncompressed, 59996 bytes compressed:  81.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.4.4.dist-info/METADATA
+Filename: ScriptCollection-3.4.6.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.4.4.dist-info/WHEEL
+Filename: ScriptCollection-3.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.4.4.dist-info/entry_points.txt
+Filename: ScriptCollection-3.4.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.4.dist-info/top_level.txt
+Filename: ScriptCollection-3.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.4.dist-info/RECORD
+Filename: ScriptCollection-3.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/Executables.py

```diff
@@ -68,25 +68,14 @@
 
     args = parser.parse_args()
     GeneralUtilities.write_message_to_stdout(ScriptCollectionCore().SCCalculateBitcoinBlockHash(args.version, args.previousblockhash,
                                                                                                 args.transactionsmerkleroot, args.timestamp, args.target, args.nonce))
     return 0
 
 
-def UpdateNugetpackagesInCsharpProject() -> int:
-
-    parser = argparse.ArgumentParser(description="""TODO""")
-    parser.add_argument('csprojfile')
-    args = parser.parse_args()
-    if ScriptCollectionCore().SCUpdateNugetpackagesInCsharpProject(args.csprojfile):
-        return 1
-    else:
-        return 0
-
-
 def Show2FAAsQRCode():
 
     parser = argparse.ArgumentParser(description="""Always when you use 2-factor-authentication you have the problem:
 Where to backup the secret-key so that it is easy to re-setup them when you have a new phone?
 Using this script is a solution. Always when you setup a 2fa you copy and store the secret in a csv-file.
 It should be obviously that this csv-file must be stored encrypted!
 Now if you want to move your 2fa-codes to a new phone you simply call "SCShow2FAAsQRCode 2FA.csv"
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -25,15 +25,15 @@
 import PyPDF2
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.4.4"
+version = "3.4.6"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -876,24 +876,14 @@
         lines.sort(key=lambda items: ''.join(items).lower())
         for line in lines:
             GeneralUtilities.write_message_to_stdout(separator_line)
             self.__print_qr_code_by_csv_line(line[0], line[1], line[2], line[3], line[4])
         GeneralUtilities.write_message_to_stdout(separator_line)
 
     @GeneralUtilities.check_arguments
-    def SCUpdateNugetpackagesInCsharpProject(self, csprojfile: str) -> int:
-        outdated_packages = self.get_nuget_packages_of_csproj_file(csprojfile, True)
-        GeneralUtilities.write_message_to_stdout("The following packages will be updated:")
-        for outdated_package in outdated_packages:
-            GeneralUtilities.write_message_to_stdout(outdated_package)
-            self.update_nuget_package(csprojfile, outdated_package)
-        GeneralUtilities.write_message_to_stdout(f"{len(outdated_packages)} package(s) were updated")
-        return len(outdated_packages) > 0
-
-    @GeneralUtilities.check_arguments
     def SCUploadFileToFileHost(self, file: str, host: str) -> int:
         try:
             GeneralUtilities.write_message_to_stdout(self.upload_file_to_file_host(file, host))
             return 0
         except Exception as exception:
             GeneralUtilities.write_exception_to_stderr_with_traceback(exception, traceback)
             return 1
@@ -1115,33 +1105,14 @@
         self.run_program("coverage", "xml", repository_folder)
         GeneralUtilities.ensure_directory_exists(os.path.join(repository_folder, "Other/TestCoverage"))
         coveragefile = os.path.join(repository_folder, "Other/TestCoverage/TestCoverage.xml")
         GeneralUtilities.ensure_file_does_not_exist(coveragefile)
         os.rename(os.path.join(repository_folder, "coverage.xml"), coveragefile)
 
     @GeneralUtilities.check_arguments
-    def get_nuget_packages_of_csproj_file(self, csproj_file: str, only_outdated_packages: bool) -> bool:
-        self.run_program("dotnet", f'restore --disable-parallel --force --force-evaluate "{csproj_file}"')
-        if only_outdated_packages:
-            only_outdated_packages_argument = " --outdated"
-        else:
-            only_outdated_packages_argument = ""
-        stdout = self.run_program("dotnet", f'list "{csproj_file}" package{only_outdated_packages_argument}')[1]
-        result = []
-        for line in stdout.splitlines():
-            trimmed_line = line.replace("\t", "").strip()
-            if trimmed_line.startswith(">"):
-                result.append(trimmed_line[2:].split(" ")[0])
-        return result
-
-    @GeneralUtilities.check_arguments
-    def update_nuget_package(self, csproj_file: str, name: str) -> None:
-        self.run_program("dotnet", f'add "{csproj_file}" package {name}')
-
-    @GeneralUtilities.check_arguments
     def get_file_permission(self, file: str) -> str:
         """This function returns an usual octet-triple, for example "0700"."""
         ls_output = self.__ls(file)
         return self.__get_file_permission_helper(ls_output)
 
     @GeneralUtilities.check_arguments
     def __get_file_permission_helper(self, ls_output: str) -> str:
@@ -1542,15 +1513,15 @@
         if password is None:
             password = GeneralUtilities.generate_password()
         self.run_program("openssl", f'req -new -newkey ec -pkeyopt ec_paramgen_curve:prime256v1 -days {days_until_expire} -nodes -x509 -subj ' +
                          f'/C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={name}/OU={subj_ou} -passout pass:{password} ' +
                          f'-keyout {name}.key -out {name}.crt', folder)
 
     @GeneralUtilities.check_arguments
-    def generate_certificate(self, folder: str,  domain: str,filename:str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,
+    def generate_certificate(self, folder: str,  domain: str, filename: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,
                              days_until_expire: int = None, password: str = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         if password is None:
             password = GeneralUtilities.generate_password()
         rsa_key_length = 4096
         self.run_program("openssl", f'genrsa -out {filename}.key {rsa_key_length}', folder)
@@ -1578,20 +1549,20 @@
 subjectAltName      = @subject_alt_name
 
 [ subject_alt_name ]
 DNS                 = {domain}
 """)
 
     @GeneralUtilities.check_arguments
-    def generate_certificate_sign_request(self, folder: str, domain: str,filename:str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str) -> None:
+    def generate_certificate_sign_request(self, folder: str, domain: str, filename: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str) -> None:
         self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} ' +
                          f'-key {filename}.key -out {filename}.csr -config {filename}.san.conf', folder)
 
     @GeneralUtilities.check_arguments
-    def sign_certificate(self, folder: str, ca_folder: str, ca_name: str, domain: str,filename:str, days_until_expire: int = None) -> None:
+    def sign_certificate(self, folder: str, ca_folder: str, ca_name: str, domain: str, filename: str, days_until_expire: int = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         ca = os.path.join(ca_folder, ca_name)
         password_file = os.path.join(folder, f"{filename}.password")
         password = GeneralUtilities.read_text_from_file(password_file)
         self.run_program("openssl", f'x509 -req -in {filename}.csr -CA {ca}.crt -CAkey {ca}.key -CAcreateserial -CAserial {ca}.srl ' +
                          f'-out {filename}.crt -days {days_until_expire} -sha256 -extensions v3_req -extfile {filename}.san.conf', folder)
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -268,15 +268,15 @@
         # gpg_identity-value when wheel-file should not be signed: None
         folder = os.path.dirname(wheel_file)
         filename = os.path.basename(wheel_file)
 
         if gpg_identity is None:
             gpg_identity_argument = ""
         else:
-            pass  # gpg_identity_argument = f" --sign --identity {gpg_identity}"
+            gpg_identity_argument = ""  # f" --sign --identity {gpg_identity}"
             # disabled due to https://blog.pypi.org/posts/2023-05-23-removing-pgp/
 
         if verbosity > 2:
             verbose_argument = " --verbose"
         else:
             verbose_argument = ""
 
@@ -759,26 +759,25 @@
             self.__sc.run_program("reportgenerator", "-reports:Other/Artifacts/TestCoverage/TestCoverage.xml " +
                                   f"-targetdir:{testcoverageubfolger} -reporttypes:Badges " +
                                   f"--verbosity:{verbose_argument_for_reportgenerator}", os.path.join(repository_folder, codeunitname),
                                   verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_run_testcases_for_dotnet_project(self, runtestcases_file: str, targetenvironmenttype: str, verbosity: int, generate_badges: bool,
-                                                            target_environmenttype_mapping:  dict[str, str], commandline_arguments: list[str]):
-        dotnet_build_configuration: str = target_environmenttype_mapping[targetenvironmenttype]
+                                                            commandline_arguments: list[str]):
         codeunit_name: str = os.path.basename(str(Path(os.path.dirname(runtestcases_file)).parent.parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         repository_folder: str = str(Path(os.path.dirname(runtestcases_file)).parent.parent.parent.absolute())
         coverage_file_folder = os.path.join(repository_folder, codeunit_name, "Other/Artifacts/TestCoverage")
         working_directory = os.path.join(repository_folder, codeunit_name)
         runsettings_argument = ""
         runsettings_file = self.dotnet_runsettings_file
         if os.path.isfile(os.path.join(working_directory, runsettings_file)):
             runsettings_argument = f"--settings {runsettings_file} "
-        arg = f"collect dotnet test {runsettings_argument}-c {dotnet_build_configuration} --output-format cobertura --output Other\\Artifacts\\TestCoverage\\Testcoverage"
+        arg = f"collect dotnet test {runsettings_argument} --no-build --output-format cobertura --output Other\\Artifacts\\TestCoverage\\Testcoverage"
         self.__sc.run_program("dotnet-coverage", arg, working_directory, verbosity=verbosity)
         os.rename(os.path.join(coverage_file_folder,  "Testcoverage.cobertura.xml"), os.path.join(coverage_file_folder,  "TestCoverage.xml"))
         self.run_testcases_common_post_task(repository_folder, codeunit_name, verbosity, generate_badges, targetenvironmenttype, commandline_arguments)
 
     def run_testcases_common_post_task(self, repository_folder: str, codeunit_name: str, verbosity: int, generate_badges: bool,
                                        targetenvironmenttype: str, commandline_arguments: list[str]):
         coverage_file_folder = os.path.join(repository_folder, codeunit_name, "Other/Artifacts/TestCoverage")
@@ -1638,34 +1637,36 @@
             artifact_files.append(self.__sc.find_file_by_extension(f"{build_artifacts_folder}\\{productname}\\{projectversion}\\{codeunit}", "Productive.Artifacts.zip"))
         changelog_file = os.path.join(repository_folder, "Other", "Resources", "Changelog", f"v{projectversion}.md")
         self.__sc.run_program_argsasarray("gh", ["release", "create", f"v{projectversion}", "--repo",  github_repo,  "--notes-file", changelog_file,
                                                  "--title", f"Release v{projectversion}"]+artifact_files, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
     def update_dependencies_of_typical_python_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
+        # TODO generalize and add option to ignore certain dependencies
         verbosity = self.get_verbosity_from_commandline_arguments(cmd_args, verbosity)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", os.path.dirname(update_script_file))
         self.__sc.update_dependencies_of_python_in_setupcfg_file(os.path.join(codeunit_folder, "setup.cfg"), verbosity)
         development_requirements_file = os.path.join(codeunit_folder, "requirements.txt")
         if (os.path.isfile(development_requirements_file)):
             self.__sc.update_dependencies_of_python_in_requirementstxt_file(development_requirements_file, verbosity)
 
     @GeneralUtilities.check_arguments
     def update_dependencies_of_typical_dotnet_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
+        # TODO generalize and add option to ignore certain dependencies
         verbosity = self.get_verbosity_from_commandline_arguments(cmd_args, verbosity)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", os.path.dirname(update_script_file))
         codeunit_name = os.path.basename(codeunit_folder)
         csproj_file = os.path.join(codeunit_folder, codeunit_name, f"{codeunit_name}.csproj")
         self.__sc.update_dependencies_of_dotnet_project(csproj_file, verbosity)
         test_csproj_file = os.path.join(codeunit_folder, f"{codeunit_name}Tests", f"{codeunit_name}Tests.csproj")
         self.__sc.update_dependencies_of_dotnet_project(test_csproj_file, verbosity)
 
     @GeneralUtilities.check_arguments
     def update_dependencies_of_typical_node_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
-        pass  # TODO
+        pass  # TODO generalize and add option to ignore certain dependencies
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_update_version_in_docker_examples(self, file, codeunit_version):
         folder_of_current_file = os.path.dirname(file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", folder_of_current_file)
         codeunit_name = os.path.basename(codeunit_folder)
         codeunit_name_lower = codeunit_name.lower()
@@ -1966,14 +1967,15 @@
         quality_folder = os.path.join(other_folder, "QualityCheck")
         reference_folder = os.path.join(other_folder, "Reference")
         additional_arguments_c: str = ""
         additional_arguments_b: str = ""
         additional_arguments_r: str = ""
         additional_arguments_l: str = ""
         additional_arguments_g: str = ""
+        additional_arguments_f: str = ""
         general_argument = f' --overwrite_verbosity={str(verbosity)} --overwrite_targetenvironmenttype={target_environmenttype}'
 
         c_additionalargumentsfile_argument = ""
 
         if is_pre_merge:
             general_argument = general_argument+" --overwrite_is_pre_merge=true"
             GeneralUtilities.write_message_to_stdout("This is a pre-merge-build")
@@ -1985,23 +1987,25 @@
                 GeneralUtilities.write_message_to_stdout("Assume dependent codeunits are already built")
 
         if additional_arguments_file is not None:
             config = configparser.ConfigParser()
             config.read(additional_arguments_file)
             section_name = f"{codeunit_name}_Configuration"
             if config.has_option(section_name, "ArgumentsForCommonTasks"):
-                additional_arguments_c = " "+config.get(section_name, "ArgumentsForCommonTasks")
+                additional_arguments_c = " " + config.get(section_name, "ArgumentsForCommonTasks")
             if config.has_option(section_name, "ArgumentsForBuild"):
-                additional_arguments_b = " "+config.get(section_name, "ArgumentsForBuild")
+                additional_arguments_b = " " + config.get(section_name, "ArgumentsForBuild")
             if config.has_option(section_name, "ArgumentsForRunTestcases"):
-                additional_arguments_r = " "+config.get(section_name, "ArgumentsForRunTestcases")
+                additional_arguments_r = " " + config.get(section_name, "ArgumentsForRunTestcases")
             if config.has_option(section_name, "ArgumentsForLinting"):
-                additional_arguments_l = " "+config.get(section_name, "ArgumentsForLinting")
+                additional_arguments_l = " " + config.get(section_name, "ArgumentsForLinting")
             if config.has_option(section_name, "ArgumentsForGenerateReference"):
-                additional_arguments_g = " "+config.get(section_name, "ArgumentsForGenerateReference")
+                additional_arguments_g = " " + config.get(section_name, "ArgumentsForGenerateReference")
+            if config.has_option(section_name, "ArgumentsForOnFinish"):
+                additional_arguments_f = " " + config.get(section_name, "ArgumentsForOnFinish")
             c_additionalargumentsfile_argument = f' --overwrite_additionalargumentsfile="{additional_arguments_file}"'
 
         GeneralUtilities.write_message_to_stdout('Run "CommonTasks.py"...')
         execution_result = self.__sc.run_program("python", f"CommonTasks.py{additional_arguments_c}{general_argument}{c_additionalargumentsfile_argument}",
                                                  other_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
         if execution_result[0] != 0:
             raise ValueError(f"CommonTasks.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
@@ -2033,14 +2037,21 @@
         GeneralUtilities.write_message_to_stdout('Run "GenerateReference.py"...')
         execution_result = self.__sc.run_program(
             "python", f"GenerateReference.py{additional_arguments_g}{general_argument}", reference_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
         if execution_result[0] != 0:
             raise ValueError(f"GenerateReference.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
         self.verify_artifact_exists(codeunit_folder, dict[str, bool]({"Reference": True}))
 
+        if os.path.isfile(os.path.join(other_folder, "OnBuildingFinished.py")):
+            GeneralUtilities.write_message_to_stdout('Run "OnBuildingFinished.py"...')
+            execution_result = self.__sc.run_program(
+                "python", f"OnBuildingFinished.py{additional_arguments_f}{general_argument}", other_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
+            if execution_result[0] != 0:
+                raise ValueError(f"OnBuildingFinished.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
+
         artifactsinformation_file = os.path.join(artifacts_folder, f"{codeunit_name}.artifactsinformation.xml")
         codeunit_version = self.get_version_of_codeunit(codeunit_file)
         GeneralUtilities.ensure_file_exists(artifactsinformation_file)
         artifacts_list = []
         for artifact_folder in GeneralUtilities.get_direct_folders_of_folder(artifacts_folder):
             artifact_name = os.path.basename(artifact_folder)
             artifacts_list.append(f"        <cps:artifact>{artifact_name}<cps:artifact>")
```

## Comparing `ScriptCollection-3.4.4.dist-info/METADATA` & `ScriptCollection-3.4.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.4.4
+Version: 3.4.6
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.4.4.dist-info/entry_points.txt` & `ScriptCollection-3.4.6.dist-info/entry_points.txt`

 * *Files identical despite different names*

