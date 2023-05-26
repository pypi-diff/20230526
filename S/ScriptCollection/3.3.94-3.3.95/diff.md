# Comparing `tmp/ScriptCollection-3.3.94-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.3.95-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 57989 bytes, number of entries: 14
+Zip file size: 59179 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    18064 b- defN 23-Mar-05 15:39 ScriptCollection/Executables.py
--rw-rw-rw-  2.0 fat    34149 b- defN 23-May-25 10:33 ScriptCollection/GeneralUtilities.py
+-rw-rw-rw-  2.0 fat    34151 b- defN 23-May-26 16:46 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
--rw-rw-rw-  2.0 fat     6273 b- defN 22-Oct-16 19:55 ScriptCollection/ProgramRunnerEpew.py
+-rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    86233 b- defN 23-May-25 10:33 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   130752 b- defN 23-May-23 21:53 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    89376 b- defN 23-May-26 16:47 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   133454 b- defN 23-May-26 16:46 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7864 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1968 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/RECORD
-14 files, 299585 bytes uncompressed, 55797 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7795 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1968 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/RECORD
+14 files, 305365 bytes uncompressed, 56987 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.3.94.dist-info/METADATA
+Filename: ScriptCollection-3.3.95.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.3.94.dist-info/WHEEL
+Filename: ScriptCollection-3.3.95.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.3.94.dist-info/entry_points.txt
+Filename: ScriptCollection-3.3.95.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.94.dist-info/top_level.txt
+Filename: ScriptCollection-3.3.95.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.94.dist-info/RECORD
+Filename: ScriptCollection-3.3.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/GeneralUtilities.py

```diff
@@ -269,15 +269,15 @@
     def string_is_none_or_empty(argument: str) -> bool:
         if argument is None:
             return True
         type_of_argument = type(argument)
         if type_of_argument == str:
             return argument == ""
         else:
-            raise Exception(f"expected string-variable in argument of string_is_none_or_empty but the type was '{str(type_of_argument)}'")
+            raise ValueError(f"expected string-variable in argument of string_is_none_or_empty but the type was '{str(type_of_argument)}'")
 
     @staticmethod
     @check_arguments
     def string_is_none_or_whitespace(string: str) -> bool:
         if GeneralUtilities.string_is_none_or_empty(string):
             return True
         else:
@@ -647,15 +647,15 @@
     def string_to_boolean(value: str) -> bool:
         value = value.strip().lower()
         if value in ('yes', 'y', 'true', 't', '1'):
             return True
         elif value in ('no', 'n', 'false', 'f', '0'):
             return False
         else:
-            raise Exception(f"Can not convert '{value}' to a boolean value")
+            raise ValueError(f"Can not convert '{value}' to a boolean value")
 
     @staticmethod
     @check_arguments
     def file_is_empty(file: str) -> bool:
         return os.stat(file).st_size == 0
 
     @staticmethod
```

## ScriptCollection/ProgramRunnerEpew.py

```diff
@@ -106,17 +106,17 @@
         for line in filecontent.splitlines():
             try:
                 striped_line = GeneralUtilities.strip_new_line_character(line)
                 result = int(striped_line)
                 return result
             except:
                 pass
-        raise Exception(f"'{filecontent}' does not containe an int-line")
+        raise ValueError(f"'{filecontent}' does not containe an int-line")
 
     @GeneralUtilities.check_arguments
     def __load_text(self, file: str) -> str:
         if os.path.isfile(file):
             content = GeneralUtilities.read_text_from_file(file).replace('\r', '')
             os.remove(file)
             return content
         else:
-            raise Exception(f"File '{file}' does not exist")
+            raise ValueError(f"File '{file}' does not exist")
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -11,25 +11,26 @@
 from subprocess import Popen
 import re
 import shutil
 import traceback
 import uuid
 import io
 import ntplib
+import requests
 import qrcode
 import pycdlib
 import send2trash
 from PyPDF2 import PdfFileMerger
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.3.94"
+version = "3.3.95"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -127,15 +128,15 @@
         if filename.lower().endswith(".dll"):
             filename = filename[:-4]
             extension = "dll"
         elif filename.lower().endswith(".exe"):
             filename = filename[:-4]
             extension = "exe"
         else:
-            raise Exception("Only .dll-files and .exe-files can be signed")
+            raise ValueError("Only .dll-files and .exe-files can be signed")
         self.run_program("ildasm",
                          f'/all /typelist /text /out="{filename}.il" "{filename}.{extension}"',
                          directory,  verbosity, False, "Sign: ildasm")
         self.run_program("ilasm",
                          f'/{extension} /res:"{filename}.res" /optimize /key="{snkfile}" "{filename}.il"',
                          directory,  verbosity, False, "Sign: ilasm")
         os.remove(directory+os.path.sep+filename+".il")
@@ -159,15 +160,15 @@
         if filename.lower().endswith(".dll"):
             filename = filename[:-4]
             extension = "dll"
         elif filename.lower().endswith(".exe"):
             filename = filename[:-4]
             extension = "exe"
         else:
-            raise Exception("Only .dll-files and .exe-files can be signed")
+            raise ValueError("Only .dll-files and .exe-files can be signed")
         self.run_program("ildasm", f'/all /typelist /text /out={filename}.il {filename}.{extension}', directory, verbosity=verbosity)
         self.run_program("ilasm", f'/{extension} /res:{filename}.res /optimize /key={keyfile} {filename}.il', directory, verbosity=verbosity)
         os.remove(directory+os.path.sep+filename+".il")
         os.remove(directory+os.path.sep+filename+".res")
 
     @GeneralUtilities.check_arguments
     def commit_is_signed_by_key(self, repository_folder: str, revision_identifier: str, key: str) -> bool:
@@ -462,15 +463,15 @@
     @GeneralUtilities.check_arguments
     def file_is_git_ignored(self, file_in_repository: str, repositorybasefolder: str) -> None:
         exit_code = self.run_program_argsasarray("git", ['check-ignore', file_in_repository], repositorybasefolder, throw_exception_if_exitcode_is_not_zero=False, verbosity=0)[0]
         if (exit_code == 0):
             return True
         if (exit_code == 1):
             return False
-        raise Exception(f"Unable to calculate whether '{file_in_repository}' in repository '{repositorybasefolder}' is ignored due to git-exitcode {exit_code}.")
+        raise ValueError(f"Unable to calculate whether '{file_in_repository}' in repository '{repositorybasefolder}' is ignored due to git-exitcode {exit_code}.")
 
     @GeneralUtilities.check_arguments
     def discard_all_changes(self, repository: str) -> None:
         self.run_program_argsasarray("git", ["reset", "HEAD", "."], repository, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
         self.run_program_argsasarray("git", ["checkout", "."], repository, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
 
     @GeneralUtilities.check_arguments
@@ -596,15 +597,15 @@
                 self.set_permission(full_path_of_file_or_folder, permissions)
             else:
                 if strict:
                     if filetype == "f":
                         filetype_full = "File"
                     if filetype == "d":
                         filetype_full = "Directory"
-                    raise Exception(f"{filetype_full} '{full_path_of_file_or_folder}' does not exist")
+                    raise ValueError(f"{filetype_full} '{full_path_of_file_or_folder}' does not exist")
 
     @GeneralUtilities.check_arguments
     def __calculate_lengh_in_seconds(self, filename: str, folder: str) -> float:
         argument = ['-v', 'error', '-show_entries', 'format=duration', '-of', 'default=noprint_wrappers=1:nokey=1', filename]
         result = self.run_program_argsasarray("ffprobe", argument, folder, throw_exception_if_exitcode_is_not_zero=True)
         return float(result[1].replace('\n', ''))
 
@@ -802,15 +803,15 @@
                         else:
                             send2trash.send2trash(new_filename)
                             os.rename(file, new_filename)
                     elif (conflictResolveMode == "merge"):
                         self.__merge_files(file, new_filename)
                         send2trash.send2trash(file)
                     else:
-                        raise Exception('Unknown conflict resolve mode')
+                        raise ValueError('Unknown conflict resolve mode')
             else:
                 os.rename(file, new_filename)
 
     @GeneralUtilities.check_arguments
     def SCReplaceSubstringsInFilenames(self, folder: str, substringInFilename: str, newSubstringInFilename: str, conflictResolveMode: str) -> None:
         for file in GeneralUtilities.absolute_file_paths(folder):
             self.__process_file(file, substringInFilename, newSubstringInFilename, conflictResolveMode)
@@ -953,15 +954,15 @@
             files_directory_obf = files_directory + "_Obfuscated"
             self.SCObfuscateFilesFolder(inputfolder, printtableheadline, namemappingfile, extensions)
             os.rename(namemappingfile, os.path.join(files_directory_obf, namemappingfile))
             if createisofile:
                 self.__create_iso(files_directory_obf, outputfile)
                 shutil.rmtree(files_directory_obf)
         else:
-            raise Exception(f"Directory not found: '{inputfolder}'")
+            raise ValueError(f"Directory not found: '{inputfolder}'")
 
     @GeneralUtilities.check_arguments
     def SCFilenameObfuscator(self, inputfolder: str, printtableheadline, namemappingfile: str, extensions: str) -> None:
         obfuscate_all_files = extensions == "*"
         if (not obfuscate_all_files):
             obfuscate_file_extensions = extensions.split(",")
 
@@ -981,15 +982,15 @@
                 hash_value = GeneralUtilities.get_sha256_of_file(file)
                 extension = Path(file).suffix
                 new_file_name_without_path = str(uuid.uuid4())[0:8] + extension
                 new_file_name = os.path.join(os.path.dirname(file), new_file_name_without_path)
                 os.rename(file, new_file_name)
                 GeneralUtilities.append_line_to_file(namemappingfile, os.path.basename(file) + ";" + new_file_name_without_path + ";" + hash_value)
         else:
-            raise Exception(f"Directory not found: '{inputfolder}'")
+            raise ValueError(f"Directory not found: '{inputfolder}'")
 
     @GeneralUtilities.check_arguments
     def __extension_matchs(self, file: str, obfuscate_file_extensions) -> bool:
         for extension in obfuscate_file_extensions:
             if file.lower().endswith("."+extension.lower()):
                 return True
         return False
@@ -1023,15 +1024,15 @@
             for file in GeneralUtilities.absolute_file_paths(inputfolder):
                 if obfuscate_all_files or self.__extension_matchs(file, obfuscate_file_extensions):
                     self.SCChangeHashOfProgram(file)
                     os.remove(file)
                     os.rename(file + ".modified", file)
             self.SCFilenameObfuscator(inputfolder, printtableheadline, namemappingfile, extensions)
         else:
-            raise Exception(f"Directory not found: '{inputfolder}'")
+            raise ValueError(f"Directory not found: '{inputfolder}'")
 
     @GeneralUtilities.check_arguments
     def upload_file_to_file_host(self, file: str, host: str) -> int:
         if (host is None):
             return self.upload_file_to_random_filesharing_service(file)
         elif host == "anonfiles.com":
             return self.upload_file_to_anonfiles(file)
@@ -1546,7 +1547,65 @@
     @GeneralUtilities.check_arguments
     def sign_certificate(self, folder: str, ca_folder: str, ca_name: str, domain: str, days_until_expire: int = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         ca = os.path.join(ca_folder, ca_name)
         self.run_program("openssl", f'x509 -req -in {domain}.csr -CA {ca}.crt -CAkey {ca}.key -CAserial {ca}.srl ' +
                          f'-out {domain}.crt -days {days_until_expire} -sha256 -extensions v3_req -extfile {domain}.san.conf', folder)
+
+    @GeneralUtilities.check_arguments
+    def update_dependencies_of_python_in_requirementstxt_file(self, file: str, verbosity: int):
+        lines = GeneralUtilities.read_lines_from_file(file)
+        new_lines = []
+        for line in lines:
+            new_lines.append(self.__get_updated_line_for_python_requirements(line.strip()))
+        GeneralUtilities.write_lines_to_file(file, new_lines)
+
+    @GeneralUtilities.check_arguments
+    def __get_updated_line_for_python_requirements(self, line: str) -> str:
+        if "==" in line or "<" in line:
+            return line
+        elif ">" in line:
+            try:
+                # line is something like "cyclonedx-bom>=2.0.2" and the function must return with the updated version
+                # (something like "cyclonedx-bom>=3.11.0" for example)
+                package = line.split(">")[0]
+                operator = ">=" if ">=" in line else ">"
+                response = requests.get(f'https://pypi.org/pypi/{package}/json', timeout=5)
+                latest_version = response.json()['info']['version']
+                return package+operator+latest_version
+            except:
+                return line
+        else:
+            raise ValueError(f'Unexpected line in requirements-file: "{line}"')
+
+    @GeneralUtilities.check_arguments
+    def update_dependencies_of_python_in_setupcfg_file(self, setup_cfg_file: str, verbosity: int):
+        lines = GeneralUtilities.read_lines_from_file(setup_cfg_file)
+        new_lines = []
+        requirement_parsing_mode = False
+        for line in lines:
+            new_line = line
+            if (requirement_parsing_mode):
+                if ("<" in line or "=" in line or ">" in line):
+                    updated_line = f"    {self.__get_updated_line_for_python_requirements(line.strip())}"
+                    new_line = updated_line
+                else:
+                    requirement_parsing_mode = False
+            else:
+                if line.startswith("install_requires ="):
+                    requirement_parsing_mode = True
+            new_lines.append(new_line)
+        GeneralUtilities.write_lines_to_file(setup_cfg_file, new_lines)
+
+    @GeneralUtilities.check_arguments
+    def update_dependencies_of_dotnet_project(self, csproj_file: str, verbosity: int):
+        folder = os.path.dirname(csproj_file)
+        csproj_filename = os.path.basename(csproj_file)
+        GeneralUtilities.write_message_to_stderr(f"Check for updates in {csproj_filename}")
+        result = self.run_program("dotnet", f"list {csproj_filename} package --outdated", folder)
+        for line in result[1].replace("\r", "").split("\n"):
+            # Relevant output-lines are something like "    > NJsonSchema             10.7.0        10.7.0      10.9.0"
+            if ">" in line:
+                package_name = line.replace(">", "").strip().split(" ")[0]
+                GeneralUtilities.write_message_to_stderr(f"Update package {package_name}")
+                self.run_program("dotnet", f"add {csproj_filename} package {package_name}", folder)
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -153,14 +153,21 @@
     def codeunit_hast_testable_sourcecode(self, codeunit_file) -> bool:
         root: etree._ElementTree = etree.parse(codeunit_file)
         return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@codeunithastestablesourcecode', namespaces={
             'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'
         })[0]))
 
     @GeneralUtilities.check_arguments
+    def codeunit_hast_updatable_dependencies(self, codeunit_file) -> bool:
+        root: etree._ElementTree = etree.parse(codeunit_file)
+        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@codeunithasupdatabledependencies', namespaces={
+            'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'
+        })[0]))
+
+    @GeneralUtilities.check_arguments
     def check_testcoverage(self, testcoverage_file_in_cobertura_format: str, repository_folder: str, codeunitname: str):
         root: etree._ElementTree = etree.parse(testcoverage_file_in_cobertura_format)
         # TODO check if there is at least one package in testcoverage_file_in_cobertura_format
         coverage_in_percent = round(float(str(root.xpath('//coverage/@line-rate')[0]))*100, 2)
         codeunit_file = os.path.join(repository_folder, codeunitname, f"{codeunitname}.codeunit.xml")
         minimalrequiredtestcoverageinpercent = self.get_testcoverage_threshold_from_codeunit_file(codeunit_file)
         minimalrecommendedcoverage = 80
@@ -686,15 +693,15 @@
                 GeneralUtilities.write_message_to_stdout(f"Check for linting-issues in {os.path.relpath(file,os.path.join(repository_folder,codeunitname))}.")
                 linting_result = self.__sc.python_file_has_errors(file, repository_folder)
                 if (linting_result[0]):
                     errors_found = True
                     for error in linting_result[1]:
                         GeneralUtilities.write_message_to_stderr(error)
         if errors_found:
-            raise Exception("Linting-issues occurred.")
+            raise ValueError("Linting-issues occurred.")
         else:
             GeneralUtilities.write_message_to_stdout("No linting-issues found.")
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_generate_coverage_report(self, repository_folder: str, codeunitname: str, verbosity: int, generate_badges: bool, targetenvironmenttype: str,
                                                     commandline_arguments: list[str], add_testcoverage_history_entry: bool = None):
         """This script expects that the file '<repositorybasefolder>/<codeunitname>/Other/Artifacts/TestCoverage/TestCoverage.xml'
@@ -1232,35 +1239,46 @@
         codeunit_name: str = str(os.path.basename(Path(os.path.dirname(common_tasks_scripts_file)).parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         project_version = self.get_version_of_project(repository_folder)
         codeunit_folder = os.path.join(repository_folder, codeunit_name)
 
         # Check codeunit-conformity
         # TODO check if foldername=="<codeunitname>[.codeunit.xml]" == <codeunitname> in file
-        codeunitfile = os.path.join(codeunit_folder, f"{codeunit_name}.codeunit.xml")
-        if not os.path.isfile(codeunitfile):
-            raise Exception(f'Codeunitfile "{codeunitfile}" does not exist.')
+        codeunit_file = os.path.join(codeunit_folder, f"{codeunit_name}.codeunit.xml")
+        if not os.path.isfile(codeunit_file):
+            raise ValueError(f'Codeunitfile "{codeunit_file}" does not exist.')
         # TODO implement usage of self.reference_latest_version_of_xsd_when_generating_xml
         namespaces = {'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure',
                       'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
-        root: etree._ElementTree = etree.parse(codeunitfile)
+        root: etree._ElementTree = etree.parse(codeunit_file)
 
         # Check codeunit-spcecification-version
         codeunit_file_version = root.xpath('//cps:codeunit/@codeunitspecificationversion', namespaces=namespaces)[0]
-        supported_codeunitspecificationversion = "1.4.0"
+        supported_codeunitspecificationversion = "2.7.1"  # must always be the latest version of the ProjectTemplates-repository
         if codeunit_file_version != supported_codeunitspecificationversion:
             raise ValueError(f"ScriptCollection only supports processing codeunits with codeunit-specification-version={supported_codeunitspecificationversion}.")
         schemaLocation = root.xpath('//cps:codeunit/@xsi:schemaLocation', namespaces=namespaces)[0]
-        xmlschema.validate(codeunitfile, schemaLocation)
+        xmlschema.validate(codeunit_file, schemaLocation)
 
         # Check codeunit-name
         codeunit_name_in_codeunit_file = root.xpath('//cps:codeunit/cps:name/text()', namespaces=namespaces)[0]
         if codeunit_name != codeunit_name_in_codeunit_file:
             raise ValueError(f"The folder-name ('{codeunit_name}') is not equal to the codeunit-name ('{codeunit_name_in_codeunit_file}').")
 
+        # Check for mandatory files
+        files = ["Other/Build/Build.py", "Other/QualityCheck/Linting.py", "Other/Reference/GenerateReference.py"]
+        if self.codeunit_hast_testable_sourcecode(codeunit_file):
+            files.append("Other/QualityCheck/RunTestcases.py")
+        if self.codeunit_hast_updatable_dependencies(codeunit_file):
+            files.append("Other/UpdateDependencies.py")
+        for file in files:
+            combined_file = os.path.join(codeunit_folder, file)
+            if not os.path.isfile(combined_file):
+                raise ValueError(f'The mandatory file "{file}" does not exist in the codeunit-folder.')
+
         # Check developer
         if self.validate_developers_of_repository:
             expected_authors: list[tuple[str, str]] = []
             expected_authors_in_xml = root.xpath('//cps:codeunit/cps:developerteam/cps:developer', namespaces=namespaces)
             for expected_author in expected_authors_in_xml:
                 author_name = expected_author.xpath('./cps:developername/text()', namespaces=namespaces)[0]
                 author_emailaddress = expected_author.xpath('./cps:developeremailaddress/text()', namespaces=namespaces)[0]
@@ -1315,15 +1333,15 @@
     @GeneralUtilities.check_arguments
     def generate_diff_report(self, repository_folder: str, codeunit_name: str, current_version: str):
         codeunit_folder = os.path.join(repository_folder, codeunit_name)
         target_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts/DiffReport", codeunit_folder)
         GeneralUtilities.ensure_directory_does_not_exist(target_folder)
         GeneralUtilities.ensure_directory_exists(target_folder)
         target_file = os.path.join(target_folder, "DiffReport.html").replace("\\", "/")
-        src = "4b825dc642cb6eb9a060e54bf8d69288fbee4904"  # hash/id of empty tree
+        src = "4b825dc642cb6eb9a060e54bf8d69288fbee4904"  # hash/id of empty git-tree
         src_prefix = "Begin"
         if self.__sc.get_current_branch_has_tag(repository_folder):
             latest_tag = self.__sc.get_latest_tag(repository_folder)
             src = self.__sc.git_get_commitid_of_tag(repository_folder, latest_tag)
             src_prefix = latest_tag
         dst = "HEAD"
         dst_prefix = f"v{current_version}"
@@ -1571,14 +1589,33 @@
         for codeunit in codeunits:
             artifact_files.append(self.__sc.find_file_by_extension(f"{build_artifacts_folder}\\{productname}\\{projectversion}\\{codeunit}", "Productive.Artifacts.zip"))
         changelog_file = os.path.join(repository_folder, "Other", "Resources", "Changelog", f"v{projectversion}.md")
         self.__sc.run_program_argsasarray("gh", ["release", "create", f"v{projectversion}", "--repo",  github_repo,  "--notes-file", changelog_file,
                                                  "--title", f"Release v{projectversion}"]+artifact_files, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
+    def update_dependencies_of_typical_python_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
+        verbosity = self.get_verbosity_from_commandline_arguments(cmd_args, verbosity)
+        codeunit_folder = GeneralUtilities.resolve_relative_path("..", os.path.dirname(update_script_file))
+        self.__sc.update_dependencies_of_python_in_setupcfg_file(os.path.join(codeunit_folder, "setup.cfg"), verbosity)
+        development_requirements_file = os.path.join(codeunit_folder, "requirements.txt")
+        if (os.path.isfile(development_requirements_file)):
+            self.__sc.update_dependencies_of_python_in_requirementstxt_file(development_requirements_file, verbosity)
+
+    @GeneralUtilities.check_arguments
+    def update_dependencies_of_typical_dotnet_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
+        verbosity = self.get_verbosity_from_commandline_arguments(cmd_args, verbosity)
+        codeunit_folder = GeneralUtilities.resolve_relative_path("..", os.path.dirname(update_script_file))
+        codeunit_name = os.path.basename(codeunit_folder)
+        csproj_file = os.path.join(codeunit_folder, codeunit_name, f"{codeunit_name}.csproj")
+        self.__sc.update_dependencies_of_dotnet_project(csproj_file, verbosity)
+        test_csproj_file = os.path.join(codeunit_folder, f"{codeunit_name}Tests", f"{codeunit_name}Tests.csproj")
+        self.__sc.update_dependencies_of_dotnet_project(test_csproj_file, verbosity)
+
+    @GeneralUtilities.check_arguments
     def standardized_tasks_update_version_in_docker_examples(self, file, codeunit_version):
         folder_of_current_file = os.path.dirname(file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", folder_of_current_file)
         codeunit_name = os.path.basename(codeunit_folder)
         codeunit_name_lower = codeunit_name.lower()
         examples_folder = GeneralUtilities.resolve_relative_path("Other/Reference/ReferenceContent/Examples", codeunit_folder)
         for example_folder in GeneralUtilities.get_direct_folders_of_folder(examples_folder):
@@ -1613,18 +1650,15 @@
         sc_epew = ScriptCollectionCore()
         sc_epew.program_runner = ProgramRunnerEpew()
         GeneralUtilities.write_message_to_stdout("Start docker-container...")
         sc_epew.run_program("docker-compose", f"--project-name {project_name} up", folder, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
     def _internal_sort_codenits(self, codeunits=dict[str, set[str]]) -> list[str]:
-        result: list[str] = list[str]()
-        ts = TopologicalSorter(codeunits)
-        result = list(ts.static_order())
-        return result
+        return list(TopologicalSorter(codeunits).static_order())
 
     @GeneralUtilities.check_arguments
     def build_codeunit(self, codeunit_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None,
                        is_pre_merge: bool = False, export_target_directory: str = None) -> None:
         codeunit_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(codeunit_folder)
         codeunit_name = os.path.basename(codeunit_folder)
         repository_folder = os.path.dirname(codeunit_folder)
```

## Comparing `ScriptCollection-3.3.94.dist-info/METADATA` & `ScriptCollection-3.3.95.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.3.94
+Version: 3.3.95
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
@@ -18,32 +18,30 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: autopep8 (>=2.0.2)
-Requires-Dist: build (>=0.10.0)
 Requires-Dist: coverage (>=7.2.5)
 Requires-Dist: cyclonedx-bom (>=3.11.0)
 Requires-Dist: defusedxml (>=0.7.1)
 Requires-Dist: keyboard (>=0.13.5)
 Requires-Dist: lxml (>=4.9.2)
 Requires-Dist: ntplib (>=0.4.0)
 Requires-Dist: pycdlib (>=1.14.0)
 Requires-Dist: Pygments (>=2.15.1)
-Requires-Dist: pylint (>=2.15.10)
-Requires-Dist: pyOpenSSL (>=23.0.0)
+Requires-Dist: pylint (>=2.17.4)
+Requires-Dist: pyOpenSSL (>=23.1.1)
 Requires-Dist: PyPDF2 (>=3.0.1)
 Requires-Dist: pytest (>=7.3.1)
-Requires-Dist: qrcode (>=7.3.1)
-Requires-Dist: send2trash (>=1.8.0)
+Requires-Dist: qrcode (>=7.4.2)
+Requires-Dist: send2trash (>=1.8.2)
 Requires-Dist: twine (>=4.0.2)
-Requires-Dist: xmlschema (>=2.1.1)
+Requires-Dist: xmlschema (>=2.3.0)
 
 # ScriptCollection
 
 ## General
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/ScriptCollection.svg)](https://pypi.org/project/ScriptCollection/)
 ![PyPI](https://img.shields.io/pypi/v/ScriptCollection)
```

## Comparing `ScriptCollection-3.3.94.dist-info/entry_points.txt` & `ScriptCollection-3.3.95.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.3.94.dist-info/RECORD` & `ScriptCollection-3.3.95.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=kXTIX92KLeFuxnYOlsyFs5lkznsxkuoBMVrV3OU7FZU,18064
-ScriptCollection/GeneralUtilities.py,sha256=RDK5DGX0GEu9dO9JKSRMZCrA_5rKuf12mvT8CE6vRQA,34149
+ScriptCollection/GeneralUtilities.py,sha256=rRQPyyRNZ1U0UDEuAqKZl3lHj38_4KofM6ON6hXqyRA,34151
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
-ScriptCollection/ProgramRunnerEpew.py,sha256=ZiBZVMcsphmo49z2BwUwQYXo2uTKXPu33QW3IxCT46E,6273
+ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=JOu7QAP4B-iSYZcmS1_0NAcZBiSfvlXcF8NaJwjm26s,86233
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=_R5kBf88cySZE_5q6Cch9eRddwbJrRzsBFTISVXFhr0,130752
+ScriptCollection/ScriptCollectionCore.py,sha256=rR5ASCMiRfeAVO_L1RckujpqgQDSsdEHVDC2YcjdnPg,89376
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=gZUEpmsqWqMi3Jd_6ur0yHJnZwJbelH47CawbXsiMNs,133454
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.3.94.dist-info/METADATA,sha256=MCJ65Y1i58EIE6aP7QJWH7mEq6Z6jS6_j0Atjdw6798,7864
-ScriptCollection-3.3.94.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.3.94.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
-ScriptCollection-3.3.94.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.3.94.dist-info/RECORD,,
+ScriptCollection-3.3.95.dist-info/METADATA,sha256=XP4pCfbejx3K-6hZsSiFYZ_xULbaoywGYON1SQrRxTo,7795
+ScriptCollection-3.3.95.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.3.95.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
+ScriptCollection-3.3.95.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.3.95.dist-info/RECORD,,
```

