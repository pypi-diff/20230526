# Comparing `tmp/cloudpy_org-1.2.7.tar.gz` & `tmp/cloudpy_org-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.2.7.tar", last modified: Tue Apr 18 15:12:49 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.2.8.tar", last modified: Fri May 26 21:14:00 2023, max compression
```

## Comparing `cloudpy_org-1.2.7.tar` & `cloudpy_org-1.2.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 15:12:49.224343 cloudpy_org-1.2.7/
--rw-rw-rw-   0        0        0      899 2023-04-18 15:12:49.223682 cloudpy_org-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 15:12:49.128670 cloudpy_org-1.2.7/cloudpy_org/
--rw-rw-rw-   0        0        0       46 2023-01-27 10:30:03.000000 cloudpy_org-1.2.7/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    48754 2023-04-18 15:08:13.000000 cloudpy_org-1.2.7/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:12:49.203998 cloudpy_org-1.2.7/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      899 2023-04-18 15:12:47.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-18 15:12:48.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 15:12:47.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-18 15:12:48.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 15:12:48.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 15:12:49.224343 cloudpy_org-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1288 2023-04-18 15:08:40.000000 cloudpy_org-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:14:00.488625 cloudpy_org-1.2.8/
+-rw-rw-rw-   0        0        0      936 2023-05-26 21:14:00.487982 cloudpy_org-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 21:14:00.389107 cloudpy_org-1.2.8/cloudpy_org/
+-rw-rw-rw-   0        0        0      112 2023-05-26 21:13:33.000000 cloudpy_org-1.2.8/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    20179 2023-05-26 20:42:11.000000 cloudpy_org-1.2.8/cloudpy_org/cloud_framework_api.py
+-rw-rw-rw-   0        0        0    52405 2023-05-26 20:39:56.000000 cloudpy_org-1.2.8/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:14:00.466337 cloudpy_org-1.2.8/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      936 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 21:14:00.488625 cloudpy_org-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-05-26 04:08:34.000000 cloudpy_org-1.2.8/setup.py
```

### Comparing `cloudpy_org-1.2.7/PKG-INFO` & `cloudpy_org-1.2.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.2.7
-Summary: Cloud data pipeline organization and automation library.
+Version: 1.2.8
+Summary: Cloud data pipeline organization and automation library. Cloud framework manager API for AWS.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudpy_org-1.2.7/cloudpy_org/tools.py` & `cloudpy_org-1.2.8/cloudpy_org/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 Copyright © 2023 Cloudpy.org
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Find documentation at https://cloudpy.org
+Find documentation at https://www.cloudpy.org
 """
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
 from pandasql import sqldf
 import datetime as dt
-from datetime import datetime
+from datetime import datetime,date
 import requests
 import boto3
 import awswrangler as wr
 from tqdm import tqdm
 from tqdm import trange
 
 from typing import Union
@@ -243,30 +243,34 @@
         'self.theseparams=p\n'\
         'self.this_source_code=source_code'
         self.this_description = self.this_description.replace("  "," ").replace("#","\n").strip()
         exec(dynamic_code)
         return self.this_source_code, self.theseparams, self.this_returns, self.this_description
     #██████████████████████████████████████████████████████████████████████████          
 class processing_tools:
-    
-    def __init__(self,encryptedSession:str='',bucket_name:str=''):
-
-        self.sta_bucket,self.environment = '','local'
+    def __init__(self,data:dict={},bucket_name:str='',region_name:str="us-east-2"):
+        self.aux = {}
+        self.__tdata = data
+        self.environment = 'local'
+        self.__set_aws_session(region_name=region_name)
+        if self.__session != None:
+            self.environment = 's3'
         self.__root_path = os.getcwd()
         self.local_directory = self.__root_path + '/'
         self.s3_bucket = bucket_name.replace('/','') + '/'
+        self.main_bucket = ''
         if bucket_name != '':
-            self.sta_bucket =  's3://' + bucket_name + '/'
+            self.main_bucket =  's3://' + bucket_name + '/'
             self.environment = bucket_name
         self.documentation_path = self.local_directory + 'documentation/'
         self.documentation_JSON_path = self.documentation_path + "json/"  
-        self.settings = self.sta_bucket + 'settings/'
+        self.settings = self.main_bucket + 'settings/'
         self.secrets = self.settings + 'secrets/'
         self.metadata = self.settings + 'metadata/'
-        self.datalake = self.s3_bucket + 'datalake-demo01/'
+        self.datalake = self.s3_bucket + 'datalake-demo-01/'
         self.hive = self.s3_bucket + 'default_hive/'
         self.dl_crypto = self.datalake + 'crypto/'
         self.dl_crypto_intraday = self.dl_crypto + 'intraday/'
         try:
             self.fs = s3fs.S3FileSystem()
         except:
             self.fs = None
@@ -342,19 +346,15 @@
             try:
                 if extension == "csv":
                     df_input.to_csv(folder_path + file_name,sep=sep,na_rep=na_rep,float_format=float_format,index=index,encoding=encoding)
                     rslt = "Data successfully stored locally as: " + folder_path + file_name
             except Exception as e:
                 rslt = str(e)
         return rslt
-                
-                
-
-                    
-                    
+            
     #__________________________________________________________________________
     def retrieve_object_name(self,objectInput:object)->str:
         '''
         ***
         Retrieves in a str, the name of the object provided.
         ***
         '''
@@ -386,23 +386,36 @@
         ***
         Decrypts a given emctrypted str input and with a given encryption key also in str datatype.
         Return the decrypted data as str.
         ***
         '''
         return Fernet(keyStr.encode('utf-8')).decrypt(inputStr.encode('utf-8')).decode()
     #__________________________________________________________________________
-    def set_aws_session(self)->None:
+    def __set_aws_session(self,region_name:str="us-east-2")->None:
         '''
         Sets a session with given AWS credentials.
         '''
-        self.session = boto3.Session(
-            aws_access_key_id=ACCESS_KEY,
-            aws_secret_access_key=SECRET_KEY,
-            aws_session_token=SESSION_TOKEN,
-        )
+        self.__session = None
+        self.__s3_client = None
+        if type(self.__tdata) == dict and self.__tdata != {}:
+            spd = self.decrypt_before_expiration(self.__tdata).split("*_xxx_*")
+            try:
+                self.__session = boto3.Session(aws_access_key_id=spd[0]
+                                         ,aws_secret_access_key=spd[1])
+                self.__s3_client = boto3.client('s3'
+                                                ,aws_access_key_id=spd[0]
+                                                ,aws_secret_access_key=spd[1]
+                                                ,region_name=region_name)
+                print("aws access achieved.")
+                spd = []
+            except Exception as e:
+                print('Error:',str(e))
+                self.__session = None
+                self.__s3_client = None
+            
     #__________________________________________________________________________
     def domain_commands(self,domain_name:str=None)->None:
         '''
         ***
         Prints the terminal commands required to connect to a given domain ubunto instance given the information 
         defined in commands and connection_details json files in metadata folder.
         ***
@@ -428,30 +441,32 @@
     def create_bucket(self,bucket_name:str,region:str="us-east-2")->None:
         '''
         ***
         Creates an s3 bucket with given bucket_name in a given region. If the region is not provided, it's default value "us-east-2" will be choosen.
         ***
         '''
         try:
-            s3_client = boto3.client('s3', region_name=region)
+            if self.__s3_client != None:
+                s3_client = self.__s3_client
+            else:
+                s3_client = boto3.client('s3', region_name=region)
             region_location = {'LocationConstraint': region}
             s3_client.create_bucket(Bucket=bucket_name,CreateBucketConfiguration=region_location)
             print("The bucket:",bucket_name, " was succesfully created!")
         except ClientError as e:
             print(e)
     #__________________________________________________________________________
-    def store_dict_as_json(self,dictionary_input:dict,writing_path:str,local:bool=True)->None:
+    def store_dict_as_json(self,dictionary_input:dict,writing_path:str)->None:
         '''
         ***
         Locally stores any dict a formatted json file in a giving path.
         ***
         '''
-        if local == True:
-            with open(writing_path,'w') as out_file:
-                json.dump(dictionary_input,out_file,sort_keys=False,indent=4)
+        with open(writing_path,'w') as out_file:
+            json.dump(dictionary_input,out_file,sort_keys=False,indent=4)
     #__________________________________________________________________________
     def date_time_id(self)->Union[int,int]:
         '''
         ***
         Returns the current date_id (yyymmdd) and the time_id which is the second of the day (which value is between 0 and 86400). Both outputs are ints.
         ***
         '''
@@ -498,28 +513,31 @@
         if path == None:
             path = self.local_directory
         files = [f for f in os.listdir(path)]
         if extension != None:
             files = [f for f in files if f.endswith('.' + extension)]
         return set(files)
     #__________________________________________________________________________ 
-    def store_str_as_file_in_s3_folder(self,strInput:str,fileName:str,s3FullFolderPath:str)->None:
+    def store_str_as_file_in_s3_folder(self,strInput:str,fileName:str,s3FullFolderPath:str,region_name:str="us-east-2")->None:
         '''
         ***
         Stores a given strInput with a given fileName in a given s3FullFolderPath.
         ***
         '''
         s3FullFolderPath = s3FullFolderPath.replace("s3://","")
         if type(strInput) != str:
             strInput = str(strInput)
         s = s3FullFolderPath
         bucketName=s[0:s.index('/')]
         rp = s.replace(bucketName,'')
         relativePath = rp[1:len(rp)]
-        client = boto3.client('s3')
+        if self.__s3_client != None:
+            client = self.__s3_client
+        else:
+            client = boto3.client('s3', region_name=region_name)
         fileKey = relativePath + fileName
         try:
             client.put_object(Body=strInput,Bucket=bucketName,Key=fileKey)
             print('file successfully stored in:\ns3://' + s3FullFolderPath + fileName)
         except Exception as e:
             print(str(e))
     #__________________________________________________________________________
@@ -593,15 +611,18 @@
         rslt_dict,fileContent,ext={},"",""
         if referenceName != "":
             s=s3FullFolderPath.replace('s3://','')
             filesFound=0
             bucketName=s[0:s.index('/')]
             rp=s.replace(bucketName,'')
             relativePath=rp[1:len(rp)]
-            resource=boto3.resource('s3')
+            if self.__session != None:
+                resource = self.__session.resource('s3')
+            else:
+                resource=boto3.resource('s3')
             my_bucket=resource.Bucket(bucketName)
             objectSumariesList=list(my_bucket.objects.filter(Prefix=relativePath))
             fileKeys=[]
             for obs in objectSumariesList:
                 fileKeys.append(obs.key)
             for fileKey in fileKeys:
                 a=fileKey[::-1]
@@ -629,15 +650,18 @@
         '''
         these_files =set()
         s=s3FullFolderPath.replace('s3://','')
         filesFound=0
         bucketName=s[0:s.index('/')]
         rp=s.replace(bucketName,'')
         relativePath=rp[1:len(rp)]
-        resource=boto3.resource('s3')
+        if self.__session != None:
+            resource = self.__session.resource('s3')
+        else:
+            resource=boto3.resource('s3')
         my_bucket=resource.Bucket(bucketName)
         objectSumariesList=list(my_bucket.objects.filter(Prefix=relativePath))
         fileKeys=[]
         for obs in objectSumariesList:
             fileKeys.append(obs.key)
         for fileKey in fileKeys:
             a=fileKey[::-1]
@@ -1029,7 +1053,55 @@
         x = ''
         if len(folder_path) > 1 and folder_path[::-1][0] not in ['/','\\']:
             x = '/'
             if '\\' in folder_path:
                 x = '\\'
         file_path = folder_path + x + file_name
         return file_path
+    #__________________________________________________________________________
+    def split_date_id(self,date_id:int):
+        date_idstr = str(date_id)
+        return int(date_idstr[0:4]),int(date_idstr[4:6]),int(date_idstr[6:8])
+    #__________________________________________________________________________
+    def minutes_diff(self,date_ida,time_ida,date_idb,time_idb)->int:
+        ya,ma,da = self.split_date_id(date_ida)
+        yb,mb,db = self.split_date_id(date_idb)
+        xa = date(ya, ma, da)
+        xb = date(yb, mb, db)
+        delta_b_a = xb - xa
+        days_b_a = delta_b_a.days
+        minutes_b_a = days_b_a*24*60 + ((time_idb - time_ida)/60) + 1
+        minutes_b_a = int(minutes_b_a)
+        return minutes_b_a
+    #__________________________________________________________________________
+    def save_s3_plain_content_locally(self
+                                      ,referenceName:str
+                                      ,s3FullFolderPath:str
+                                      ,destinyFileName:str = None
+                                      ,destinyFolderPath:str = None
+                                      ,exceptionCase:bool = False
+                                     )->None:
+        referenceName = referenceName.split(".")[0]
+        if destinyFolderPath == None:
+            destinyFolderPath = self.local_directory
+        content = self.get_s3_file_content(referenceName,s3FullFolderPath,exceptionCase=exceptionCase)
+        ext = "txt"
+        if type(content) == dict:
+            ext = ".json"
+        if destinyFileName == None:
+            destinyFileName = referenceName + ext
+        if ext == ".json":
+            self.store_dict_as_json(dictionary_input=content,writing_path=destinyFolderPath+destinyFileName)
+        else:
+            with open(destinyFolderPath+destinyFileName,'w') as f:
+                f.write(content)
+    #__________________________________________________________________________
+    def basic_dicstr_to_dict(self,dictstr:str)->dict:
+        date_id,time_id = self.date_time_id()
+        keyname = str(date_id) + "_" + str(time_id)
+        self.aux[keyname] = {}
+        dc = "self.aux['@keyname'] = " + dictstr
+        dc = dc.replace("@keyname",keyname)
+        exec(dc)
+        rslt = self.aux[keyname] 
+        self.aux.pop(keyname, None)
+        return rslt
```

### Comparing `cloudpy_org-1.2.7/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.2.8/cloudpy_org.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.2.7
-Summary: Cloud data pipeline organization and automation library.
+Version: 1.2.8
+Summary: Cloud data pipeline organization and automation library. Cloud framework manager API for AWS.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudpy_org-1.2.7/setup.py` & `cloudpy_org-1.2.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.2.7",
-    description="Cloud data pipeline organization and automation library.",
+    version="1.2.8",
+    description="Cloud data pipeline organization and automation library. Cloud framework manager API for AWS.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
     classifiers=[
```

