# Comparing `tmp/fovus-1.0.3-py3-none-any.whl.zip` & `tmp/fovus-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 43971 bytes, number of entries: 46
+Zip file size: 44119 bytes, number of entries: 46
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 23-Apr-05 06:40 fovus/root_config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/adapter/__init__.py
 -rw-r--r--  2.0 unx     3331 b- defN 23-Apr-05 06:40 fovus/adapter/aws_cognito_adapter.py
 -rw-r--r--  2.0 unx    10856 b- defN 23-Apr-12 04:12 fovus/adapter/fovus_api_adapter.py
--rw-r--r--  2.0 unx     8348 b- defN 23-Apr-05 06:40 fovus/adapter/fovus_s3_adapter.py
+-rw-r--r--  2.0 unx     8700 b- defN 23-May-25 22:01 fovus/adapter/fovus_s3_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/cli/__init__.py
 -rw-r--r--  2.0 unx    13184 b- defN 23-Apr-05 06:40 fovus/cli/cli_action_runner.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Apr-05 06:56 fovus/cli/documenter.py
 -rw-r--r--  2.0 unx      475 b- defN 23-Apr-05 06:40 fovus/cli/fovus_cli.py
 -rw-r--r--  2.0 unx    25901 b- defN 23-May-15 05:07 fovus/cli/fovus_cli_argument_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/config/__init__.py
--rw-r--r--  2.0 unx      138 b- defN 23-May-15 06:09 fovus/config/config.py
+-rw-r--r--  2.0 unx      138 b- defN 23-May-25 22:01 fovus/config/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/constants/__init__.py
 -rw-r--r--  2.0 unx       59 b- defN 23-Apr-05 06:40 fovus/constants/cli_action_runner_constants.py
 -rw-r--r--  2.0 unx     8641 b- defN 23-May-15 05:17 fovus/constants/cli_constants.py
 -rw-r--r--  2.0 unx     1446 b- defN 23-Apr-05 06:40 fovus/constants/fovus_api_constants.py
 -rw-r--r--  2.0 unx      194 b- defN 23-Apr-05 06:40 fovus/constants/util_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/exception/__init__.py
 -rw-r--r--  2.0 unx      291 b- defN 23-Apr-05 06:40 fovus/exception/status_code_exception.py
@@ -28,21 +28,21 @@
 -rw-r--r--  2.0 unx       42 b- defN 23-Apr-05 06:40 fovus/fovus_provided_configs/FOVUS_user_config_template.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/fovus_provided_configs/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/schema/__init__.py
 -rw-r--r--  2.0 unx    10183 b- defN 23-May-15 05:07 fovus/schema/create_job_schema.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/util/__init__.py
 -rw-r--r--  2.0 unx     3389 b- defN 23-Apr-05 06:40 fovus/util/aws_util.py
 -rw-r--r--  2.0 unx      334 b- defN 23-Apr-05 06:40 fovus/util/cli_action_runner_util.py
--rw-r--r--  2.0 unx     4208 b- defN 23-Apr-05 06:40 fovus/util/file_util.py
+-rw-r--r--  2.0 unx     4616 b- defN 23-May-25 22:01 fovus/util/file_util.py
 -rw-r--r--  2.0 unx     2871 b- defN 23-Apr-05 06:40 fovus/util/fovus_api_util.py
 -rw-r--r--  2.0 unx     1740 b- defN 23-Apr-05 06:40 fovus/util/fovus_cli_argument_parser_util.py
 -rw-r--r--  2.0 unx     1519 b- defN 23-Apr-05 06:40 fovus/util/fovus_s3_adapter_util.py
 -rw-r--r--  2.0 unx      533 b- defN 23-Apr-05 06:40 fovus/util/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/validator/__init__.py
 -rw-r--r--  2.0 unx     3935 b- defN 23-May-12 19:25 fovus/validator/fovus_api_validator.py
--rw-r--r--  2.0 unx    14101 b- defN 23-May-15 06:15 fovus-1.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8883 b- defN 23-May-15 06:15 fovus-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 06:15 fovus-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-May-15 06:15 fovus-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-15 06:15 fovus-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4089 b- defN 23-May-15 06:15 fovus-1.0.3.dist-info/RECORD
-46 files, 133603 bytes uncompressed, 37315 bytes compressed:  72.1%
+-rw-r--r--  2.0 unx    14101 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8883 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4089 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/RECORD
+46 files, 134363 bytes uncompressed, 37463 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -114,26 +114,26 @@
 
 Filename: fovus/validator/__init__.py
 Comment: 
 
 Filename: fovus/validator/fovus_api_validator.py
 Comment: 
 
-Filename: fovus-1.0.3.dist-info/LICENSE.txt
+Filename: fovus-1.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fovus-1.0.3.dist-info/METADATA
+Filename: fovus-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: fovus-1.0.3.dist-info/WHEEL
+Filename: fovus-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: fovus-1.0.3.dist-info/entry_points.txt
+Filename: fovus-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: fovus-1.0.3.dist-info/top_level.txt
+Filename: fovus-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: fovus-1.0.3.dist-info/RECORD
+Filename: fovus-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fovus/adapter/fovus_s3_adapter.py

```diff
@@ -37,14 +37,15 @@
         self.local_root_directory_path = root_directory_path
         self.job_id = FovusApiUtil.get_job_id(self.cli_dict)
 
         # Assigned if upload function is called.
         self.local_filepath_list = None
         self.task_count = None
         self.total_file_size_bytes = None
+        self.progress_bar = None
 
     def get_job_id(self):
         return self.job_id
 
     def upload_files(self):
         self._instantiate_upload_instance_variables()
         self._validate_root_directory()
@@ -73,18 +74,20 @@
         os.makedirs(fovus_job_info_directory_path)
         job_data_filepath = os.path.join(fovus_job_info_directory_path, JOB_DATA_FILENAME)
         with open(job_data_filepath, "w", encoding=UTF8) as job_data_file:
             json.dump(job_data, job_data_file)
 
     def download_files(self):
         s3_list_objects_v2_response = self._get_s3_list_objects_v2_response()
-        objects_to_download, total_size_bytes, tasks = AwsUtil.get_s3_object_list_info(
+        objects_to_download, self.total_file_size_bytes, self.task_count = AwsUtil.get_s3_object_list_info(
             s3_list_objects_v2_response, self.cli_dict[INCLUDE_OUTPUT], self.cli_dict[EXCLUDE_OUTPUT]
         )
-        FovusS3AdapterUtil.print_pre_operation_information(DOWNLOAD, len(objects_to_download), total_size_bytes, tasks)
+        FovusS3AdapterUtil.print_pre_operation_information(
+            DOWNLOAD, len(objects_to_download), self.total_file_size_bytes, self.task_count
+        )
         FileUtil.create_missing_directories(
             self.local_root_directory_path,
             AwsUtil.get_all_directories(
                 objects_to_download,
                 s3_list_objects_v2_response["Prefix"],
                 self.cli_dict[INCLUDE_OUTPUT],
                 self.cli_dict[EXCLUDE_OUTPUT],
@@ -92,35 +95,39 @@
         )
         self._operate_on_s3_in_parallel(objects_to_download, self._download_file, self._prepare_next_download_attempt)
         FovusS3AdapterUtil.print_post_operation_success(DOWNLOAD, is_success=True)
 
     def _operate_on_s3_in_parallel(self, remaining_items, file_operation, prepare_next_attempt_action):
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = []
-            progress_bar = tqdm(total=len(remaining_items), unit="files", desc="Progress")
+            self.progress_bar = tqdm(
+                total=self.total_file_size_bytes,
+                unit="B",
+                desc="Progress",
+                unit_scale=True,
+                unit_divisor=1024,
+            )
             while True:
                 s3_info = prepare_next_attempt_action(futures)
                 remaining_items = self._try_operate_on_file_list(
-                    file_operation, s3_info, futures, executor, remaining_items, progress_bar
+                    file_operation, s3_info, futures, executor, remaining_items
                 )
                 if not remaining_items:
-                    progress_bar.close()
+                    self.progress_bar.close()
                     return
 
     def _try_operate_on_file_list(  # pylint: disable=too-many-arguments
-        self, file_operation, s3_info, futures, executor, remaining_objects, progress_bar
+        self, file_operation, s3_info, futures, executor, remaining_objects
     ):
         failed_objects = []
         for obj in remaining_objects:
             futures.append(executor.submit(file_operation, s3_info, obj))
         for future in concurrent.futures.as_completed(futures):
             result = future.result()
-            if result[SUCCESS]:
-                progress_bar.update()
-            else:
+            if not result[SUCCESS]:
                 failed_objects.append(result[LOCAL_FILEPATH])
         return failed_objects
 
     def _instantiate_upload_instance_variables(self):
         self.local_filepath_list, self.task_count, self.total_file_size_bytes = FileUtil.get_files_in_directory(
             self.local_root_directory_path, self.cli_dict[INCLUDE_INPUT], self.cli_dict[EXCLUDE_INPUT]
         )
@@ -135,15 +142,15 @@
         local_relative_filepath = os.path.relpath(local_filepath, self.local_root_directory_path)
         s3_path = os.path.join(s3_prefix, self.job_id, local_relative_filepath)
         if Util.is_windows():
             s3_path = FileUtil.windows_to_unix_path(s3_path)
 
         result = {SUCCESS: True, LOCAL_FILEPATH: local_filepath}
         try:
-            s3_client.upload_file(local_filepath, s3_bucket, s3_path)
+            s3_client.upload_file(local_filepath, s3_bucket, s3_path, Callback=self.progress_bar.update)
         except boto3.exceptions.S3UploadFailedError as error:
             if AwsUtil.is_expired_token_error(error):
                 result[SUCCESS] = False
             else:
                 raise SystemException(HTTPStatus.INTERNAL_SERVER_ERROR, error)  # pylint: disable=raise-missing-from
         return result
 
@@ -168,21 +175,25 @@
             if FileUtil.include_exclude_allows_path(
                 os.path.relpath(local_filepath, self.local_root_directory_path),
                 self.cli_dict[INCLUDE_OUTPUT],
                 self.cli_dict[EXCLUDE_OUTPUT],
             ) and FovusS3AdapterUtil.should_download_file(local_filepath, s3_object):
                 os.makedirs(os.path.dirname(local_filepath), exist_ok=True)
                 try:
-                    s3_client.download_file(s3_bucket, s3_object["Key"], local_filepath)
+                    s3_client.download_file(
+                        s3_bucket, s3_object["Key"], local_filepath, Callback=self.progress_bar.update
+                    )
                 except botocore.exceptions.ClientError as error:
                     if AwsUtil.is_expired_token_error(error):
                         result[SUCCESS] = False
                     else:
                         raise SystemException(  # pylint: disable=raise-missing-from
                             HTTPStatus.INTERNAL_SERVER_ERROR, error
                         )
+            else:
+                self.progress_bar.update(s3_object["Size"])
         return result
 
     def _get_local_filepath(self, s3_object, s3_prefix):
         return os.path.join(
             self.local_root_directory_path, AwsUtil.get_s3_object_key_without_prefix(s3_object, s3_prefix)
         )
```

## fovus/util/file_util.py

```diff
@@ -8,38 +8,48 @@
 
 FOVUS_JOB_INFO_FOLDER = ".fovus"
 
 
 class FileUtil:
     @staticmethod
     def get_files_in_directory(root_directory_path, include_input_list, exclude_input_list):
+        task_directories = FileUtil._get_directories_in_directory(
+            root_directory_path, include_input_list, exclude_input_list
+        )
+        dirs_with_spaces = [dir for dir in task_directories if " " in dir]
+        if dirs_with_spaces:
+            raise UserException(
+                HTTPStatus.BAD_REQUEST,
+                FileUtil.__name__,
+                "Spaces are not allowed in task folder names. The following task folder names are invalid: "
+                + str(dirs_with_spaces),
+            )
+
         local_filepath_list = []
-        tasks = set()
         total_file_size_bytes = 0
-        for directory_path, _dirs, files in os.walk(root_directory_path):
+        for directory_path, _, files in os.walk(root_directory_path):
             for file in files:
                 local_filepath = os.path.join(directory_path, file)
                 if FileUtil.should_ignore_path(file) or not FileUtil.include_exclude_allows_path(
                     os.path.relpath(local_filepath, root_directory_path), include_input_list, exclude_input_list
                 ):
                     continue
                 local_filepath_list.append(local_filepath)
-                tasks.add(os.path.relpath(local_filepath, root_directory_path).split(os.path.sep)[0])
                 total_file_size_bytes += os.path.getsize(local_filepath)
-        return local_filepath_list, len(tasks), total_file_size_bytes
+        return local_filepath_list, len(task_directories), total_file_size_bytes
 
     @staticmethod
-    def _get_num_directories_in_directory(root_directory_path, include_input_list, exclude_input_list):
-        num_directories = 0
+    def _get_directories_in_directory(root_directory_path, include_input_list, exclude_input_list):
+        directories = []
         for entry in os.scandir(root_directory_path):
             if entry.is_dir() and FileUtil.include_exclude_allows_path(
                 entry.name, include_input_list, exclude_input_list
             ):
-                num_directories += 1
-        return num_directories
+                directories.append(entry.name)
+        return directories
 
     @staticmethod
     def should_ignore_path(file_name):
         if FileUtil._path_contains_directory(file_name, FOVUS_JOB_INFO_FOLDER):
             return True
         if Util.is_unix():
             return FileUtil._is_swap_or_hidden_file_unix(file_name)
```

## Comparing `fovus-1.0.3.dist-info/LICENSE.txt` & `fovus-1.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fovus-1.0.3.dist-info/METADATA` & `fovus-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fovus
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Fovus Python CLI
 Author: Fovus Corporation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3 (>=1.26.60)
 Requires-Dist: jsonschema (>=3.2.0)
```

## Comparing `fovus-1.0.3.dist-info/RECORD` & `fovus-1.0.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 fovus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/root_config.py,sha256=onsSNaAhzMvRK8o82IkASh4EVkyMxVMPBlUXcUq1Lcg,65
 fovus/adapter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/adapter/aws_cognito_adapter.py,sha256=RsqnPW2spH2DKn6mDf4cgbd3KwICANS4uL7vt0zo6k8,3331
 fovus/adapter/fovus_api_adapter.py,sha256=GhvZWNSFcS3rqxgI6pavacnI_GbBO_kf1ZEaxmpVlRw,10856
-fovus/adapter/fovus_s3_adapter.py,sha256=K-1QS4xJfGndXRg0uI_DPjwEyy1Q-ASMYWFs0__yJX4,8348
+fovus/adapter/fovus_s3_adapter.py,sha256=0O5IUT1WUk_i2GAoy_J3lZB0Onh4M2z6U-hX_lr1Lxs,8700
 fovus/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/cli/cli_action_runner.py,sha256=TYG2iJgfft0GgezuyyLtC_VxL0TmrV-HajeLuFSjVMo,13184
 fovus/cli/documenter.py,sha256=uzpu25Wd8YXirM7oQPLG3hqgAZa2_H_YPz0i522qxyo,161
 fovus/cli/fovus_cli.py,sha256=6YyqZ6-gzmH2eXVlwwbg-jl4P_lRJn77qx1_cG_432U,475
 fovus/cli/fovus_cli_argument_parser.py,sha256=Uhm80S-6cml5lnALUl8J2IrnLM8-L0aBaodcsJRNALI,25901
 fovus/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/config/config.py,sha256=LhikS-z0_0IL8uGJVDSf-HfPfq0a6_C3oOixw320sYM,138
@@ -27,20 +27,20 @@
 fovus/fovus_provided_configs/FOVUS_user_config_template.json,sha256=HMCwX1ffMaUFonqxfv94c1ZlianfRTXal3BsYMxuRAE,42
 fovus/fovus_provided_configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/schema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/schema/create_job_schema.json,sha256=rxVBkIytO6qvcLd_qmHtxkKJMvDb5SFFS33BUwOzSfQ,10183
 fovus/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/util/aws_util.py,sha256=KX6DJIkwZ8ruToI8O0fK0TYEVxfyZI-p3NkRSSbGuVg,3389
 fovus/util/cli_action_runner_util.py,sha256=cPVVedOavu7nO_bbRS8wlipc2PCB-Q94BAMV3aopOYo,334
-fovus/util/file_util.py,sha256=RK-2wtW4bFRNXZ79NgbfWceofxJV59sudr8-0-ewpmM,4208
+fovus/util/file_util.py,sha256=DGC-DYXh4YUv1EJmpa2U_SVRqiW4na2DMRdEAIi9sic,4616
 fovus/util/fovus_api_util.py,sha256=7Auhoqjh0drGODn9U4zWG6e2eXlvCvRiuqQDpQCZz2A,2871
 fovus/util/fovus_cli_argument_parser_util.py,sha256=kuVUIibYr_9crVH34aX-MotOwj_KBBt8R_bbbrEmiIw,1740
 fovus/util/fovus_s3_adapter_util.py,sha256=WQwqgaeVttAUTJ2MyO9KFXpaIsVFwzcUM3K6xZ5oeFU,1519
 fovus/util/util.py,sha256=i_mzAJDsIvvWEEOTVGYckYZInZe6EddwyJiiVQca7R4,533
 fovus/validator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/validator/fovus_api_validator.py,sha256=2X108-S2IIJyxdX2PvN1mAhe1de-be09GRGeyDWfw5g,3935
-fovus-1.0.3.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
-fovus-1.0.3.dist-info/METADATA,sha256=VSUYoIcPHpuWAHVBH4mydNn7Ob3mpOD8_4zoxE3SHAQ,8883
-fovus-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fovus-1.0.3.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
-fovus-1.0.3.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
-fovus-1.0.3.dist-info/RECORD,,
+fovus-1.0.4.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
+fovus-1.0.4.dist-info/METADATA,sha256=FQcwbhgxsM32wCdsbv6MIXACjloN8DpCDSjOk9gX-to,8883
+fovus-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fovus-1.0.4.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
+fovus-1.0.4.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
+fovus-1.0.4.dist-info/RECORD,,
```

