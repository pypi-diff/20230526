# Comparing `tmp/Contentstack-1.7.0.tar.gz` & `tmp/Contentstack-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Contentstack-1.7.0.tar", last modified: Thu Apr 14 06:54:31 2022, max compression
+gzip compressed data, was "Contentstack-1.8.0.tar", last modified: Fri May 26 06:25:21 2023, max compression
```

## Comparing `Contentstack-1.7.0.tar` & `Contentstack-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2022-04-14 06:54:31.987415 Contentstack-1.7.0/
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2022-04-14 06:54:31.978809 Contentstack-1.7.0/Contentstack.egg-info/
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     8997 2022-04-14 06:54:31.000000 Contentstack-1.7.0/Contentstack.egg-info/PKG-INFO
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      555 2022-04-14 06:54:31.000000 Contentstack-1.7.0/Contentstack.egg-info/SOURCES.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)        1 2022-04-14 06:54:31.000000 Contentstack-1.7.0/Contentstack.egg-info/dependency_links.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)        1 2022-04-14 06:54:30.000000 Contentstack-1.7.0/Contentstack.egg-info/not-zip-safe
--rw-r--r--   0 shaileshmishra   (501) staff       (20)       38 2022-04-14 06:54:31.000000 Contentstack-1.7.0/Contentstack.egg-info/requires.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)       13 2022-04-14 06:54:31.000000 Contentstack-1.7.0/Contentstack.egg-info/top_level.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     1099 2022-04-08 07:39:16.000000 Contentstack-1.7.0/LICENSE
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     8997 2022-04-14 06:54:31.986996 Contentstack-1.7.0/PKG-INFO
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     6830 2022-04-08 11:14:27.000000 Contentstack-1.7.0/README.rst
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2022-04-14 06:54:31.986200 Contentstack-1.7.0/contentstack/
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      848 2022-04-08 17:56:04.000000 Contentstack-1.7.0/contentstack/__init__.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     5593 2022-04-12 06:54:36.000000 Contentstack-1.7.0/contentstack/asset.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     6129 2022-04-12 06:57:40.000000 Contentstack-1.7.0/contentstack/assetquery.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     6461 2022-04-12 11:50:30.000000 Contentstack-1.7.0/contentstack/basequery.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     4929 2022-04-12 10:05:16.000000 Contentstack-1.7.0/contentstack/contenttype.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     8035 2022-04-12 11:50:25.000000 Contentstack-1.7.0/contentstack/entry.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     7429 2022-04-12 08:37:06.000000 Contentstack-1.7.0/contentstack/entryqueryable.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     3456 2022-04-12 08:36:55.000000 Contentstack-1.7.0/contentstack/https_connection.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     2270 2022-04-12 09:09:56.000000 Contentstack-1.7.0/contentstack/image_transform.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)    13032 2022-04-12 11:50:06.000000 Contentstack-1.7.0/contentstack/query.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)    14139 2022-04-12 11:39:43.000000 Contentstack-1.7.0/contentstack/stack.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     1865 2022-04-12 08:20:35.000000 Contentstack-1.7.0/contentstack/utility.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)       38 2022-04-14 06:54:31.987556 Contentstack-1.7.0/setup.cfg
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     1689 2022-04-12 11:06:07.000000 Contentstack-1.7.0/setup.py
+drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-26 06:25:21.943516 Contentstack-1.8.0/
+drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-26 06:25:21.925602 Contentstack-1.8.0/Contentstack.egg-info/
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     7648 2023-05-26 06:25:21.000000 Contentstack-1.8.0/Contentstack.egg-info/PKG-INFO
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)      720 2023-05-26 06:25:21.000000 Contentstack-1.8.0/Contentstack.egg-info/SOURCES.txt
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)        1 2023-05-26 06:25:21.000000 Contentstack-1.8.0/Contentstack.egg-info/dependency_links.txt
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)        1 2023-05-26 05:47:40.000000 Contentstack-1.8.0/Contentstack.egg-info/not-zip-safe
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)       38 2023-05-26 06:25:21.000000 Contentstack-1.8.0/Contentstack.egg-info/requires.txt
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)       13 2023-05-26 06:25:21.000000 Contentstack-1.8.0/Contentstack.egg-info/top_level.txt
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     1099 2023-05-23 12:27:47.000000 Contentstack-1.8.0/LICENSE
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     7648 2023-05-26 06:25:21.941600 Contentstack-1.8.0/PKG-INFO
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     6830 2023-05-23 12:27:47.000000 Contentstack-1.8.0/README.rst
+drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-26 06:25:21.935755 Contentstack-1.8.0/contentstack/
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)      697 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/__init__.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     5469 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/asset.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     6552 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/assetquery.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     6363 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/basequery.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     4888 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/contenttype.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     1028 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/controller.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)      798 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/deep_merge_lp.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     8815 2023-05-25 11:16:23.000000 Contentstack-1.8.0/contentstack/entry.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     7886 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/entryqueryable.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     1729 2023-05-25 11:16:23.000000 Contentstack-1.8.0/contentstack/https_connection.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     2165 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/image_transform.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)    14717 2023-05-25 11:16:23.000000 Contentstack-1.8.0/contentstack/query.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)    15054 2023-05-23 12:27:47.000000 Contentstack-1.8.0/contentstack/stack.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     1690 2023-05-25 11:16:23.000000 Contentstack-1.8.0/contentstack/utility.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)       38 2023-05-26 06:25:21.943869 Contentstack-1.8.0/setup.cfg
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     1811 2023-05-26 06:25:14.000000 Contentstack-1.8.0/setup.py
+drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-26 06:25:21.939849 Contentstack-1.8.0/tests/
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     9136 2023-05-23 12:27:47.000000 Contentstack-1.8.0/tests/test_assets.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     6166 2023-05-23 12:27:47.000000 Contentstack-1.8.0/tests/test_entry.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     6806 2023-05-25 11:16:23.000000 Contentstack-1.8.0/tests/test_live_preview.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     6078 2023-05-02 11:02:22.000000 Contentstack-1.8.0/tests/test_query.py
+-rw-r--r--   0 shaileshmishra   (501) staff       (20)     7181 2023-05-23 12:27:47.000000 Contentstack-1.8.0/tests/test_stack.py
```

### Comparing `Contentstack-1.7.0/Contentstack.egg-info/PKG-INFO` & `Contentstack-1.8.0/Contentstack.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,166 @@
 Metadata-Version: 2.1
 Name: Contentstack
-Version: 1.7.0
+Version: 1.8.0
 Summary: Contentstack is a headless CMS with an API-first approach.
 Home-page: https://github.com/contentstack/contentstack-python
 Author: Contentstack
 Author-email: shailesh.mishra@contentstack.com
 License: MIT
 Keywords: contentstack-python
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#
+================
+**Contentstack**
+================
 
-[![Contentstack](https://www.contentstack.com/docs/static/images/contentstack.png)](https://www.contentstack.com/)
+Python SDK for Contentstack
+===========================
 
-<!-- ![Python package](https://github.com/contentstack/contentstack-python/workflows/Python%20package/badge.svg?branch=master) -->
+  Contentstack is a headless CMS with an API-first approach. It is a CMS that developers can use to build powerful cross-platform applications in their favorite languages. Build your application frontend, and Contentstack will take care of the rest. `Read More <https://www.contentstack.com/>`_.
 
-![build](https://img.shields.io/badge/build-passing-green?style=plastic)
-![Coverage](https://raw.githubusercontent.com/contentstack/contentstack-python/b4edf799276f586dce3e57fa5502036cd5fd8da3/coverage.svg) ![pip](https://img.shields.io/badge/pip-v1.6.0-blue?style=plastic) ![python](https://img.shields.io/badge/python-3.5|3.6|3.7|3.8-blue?style=plastic) [![GitHub license](https://img.shields.io/github/license/contentstack/contentstack-python?style=plastic)](https://github.com/contentstack/contentstack-python/blob/master/LICENSE) [![GitHub stars](https://img.shields.io/github/stars/contentstack/contentstack-python?style=plastic)](https://github.com/contentstack/contentstack-python/stargazers)
+  Contentstack provides Python SDK to build an application on top of Python. Given below is the detailed guide and helpful resources to get started with our Python SDK.
 
-## Python SDK for Contentstack
+Prerequisite
+============
 
-Contentstack is a headless CMS with an API-first approach. It is a CMS that developers can use to build powerful cross-platform applications in their favorite languages. Build your application frontend, and Contentstack will take care of the rest. [Read More](https://www.contentstack.com/).
+  You will need python 3 installed on your machine. You can install it from `here <https://www.python.org/ftp/python/3.7.4/python-3.7.4-macosx10.9.pkg>`_
 
-Contentstack provides Python SDK to build application on top of Python. Given below is the detailed guide and helpful resources to get started with our Python SDK.
+Setup and Installation
+======================
 
-### Prerequisite
+  To use the Contentstack Python SDK to your existing project, perform the steps given below:
 
-You will need python 3 installed on your machine. You can install it from [here](https://www.python.org/ftp/python/3.7.4/python-3.7.4-macosx10.9.pkg).
+.. code-block:: python
+    install contentstack pip
 
-### Setup and Installation
+This is the preferred method to install contentstack, as it will always install the most recent stable release. If you don't have `pip <https://pip.pypa.io/>`_
+installed, this `Python installation guide <http://docs.python-guide.org/en/latest/starting/installation/>`_ can guide you through the process
 
-To use the Contentstack Python SDK to your existing project, perform the steps given below:
 
-### Install contentstack pip
+Key Concepts for using Contentstack
+-----------------------------------
 
-```pyhton
-pip install contentstack
-```
+**Stack**
 
-Install latest [contentstack](https://pypi.org/project/Contentstack) package from the [PyPI](https://pypi.org)
+  A stack is like a container that holds the content of your app. Learn more about `Stacks <https://www.contentstack.com/docs/developers/set-up-stack>`_.
 
-This is the preferred method to install contentstack, as it will always install the most recent stable release. If you don't have [pip](https://pip.pypa.io/) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process
+**Content-Type**
 
-### Key Concepts for using Contentstack
+  Content-type lets you define the structure or blueprint of a page or a section of your digital property. It is a form-like page that gives Content Managers an interface to input and upload content. `read_more <https://www.contentstack.com/docs/developers/create-content-types>`_.
 
-#### Stack
+**Entry**
 
-A stack is like a container that holds the content of your app. Learn more about [Stacks](https://www.contentstack.com/docs/developers/set-up-stack).
+    An entry is the actual piece of content created using one of the defined content types. Learn more about `Entries <https://www.contentstack.com/docs/content-managers/work-with-entries>`_.
 
-#### Content Type
+**Asset**
 
-Content type lets you define the structure or blueprint of a page or a section of your digital property. It is a form-like page that gives Content Managers an interface to input and upload content. [Read more](https://www.contentstack.com/docs/developers/create-content-types).
+    Assets refer to all the media files (images, videos, PDFs, audio files, and so on) uploaded to Contentstack. These files can be used in multiple entries. Read more about `Assets <https://www.contentstack.com/docs/content-managers/work-with-assets>`_.
 
-#### Entry
+**Environment**
 
-An entry is the actual piece of content created using one of the defined content types. Learn more about [Entries](https://www.contentstack.com/docs/content-managers/work-with-entries).
+    A publishing environment corresponds to one or more deployment servers or a content delivery destination where the entries need to be published. Learn how to work with `Environments <https://www.contentstack.com/docs/developers/set-up-environments)>`_.
 
-#### Asset
 
-Assets refer to all the media files (images, videos, PDFs, audio files, and so on) uploaded to Contentstack. These files can be used in multiple entries. Read more about [Assets](https://www.contentstack.com/docs/content-managers/work-with-assets).
 
-#### Environment
+Contentstack Python SDK: 5-minute Quickstart
+--------------------------------------------
 
-A publishing environment corresponds to one or more deployment servers or a content delivery destination where the entries need to be published. Learn how to work with [Environments](https://www.contentstack.com/docs/developers/set-up-environments).
+**Initializing your SDK**
 
-### Contentstack Python SDK: 5-minute Quickstart
+    To initialize the SDK, specify the application  API key, access token, and environment name of the stack as shown in the snippet given below:
 
-#### Initializing your SDK
+.. code-block:: python
 
-To initialize the SDK, specify application API key, access token, and environment name of the stack as shown in the snippet given below, You can provide optional parameters for config:
+   stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment')
-```
 
 To get the API credentials mentioned above, log in to your Contentstack account and then in your top panel navigation, go to Settings &gt; Stack to view the API Key and Access Token.
 
-#### Querying content from your stack
+
+
+**Querying content from your stack**
 
 To retrieve a single entry from a content type use the code snippet given below:
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment')
-content_type = stack.content_type("content_type_uid")
-entry = content_type.entry("entry_uid")
-result = entry.fetch()
-```
+.. code-block:: python
+
+   content_type = stack.content_type("content_type_uid")
+   entry = content_type.entry("entry_uid")
+   result = entry.fetch()
 
-##### Get Multiple Entries
+
+**Get Multiple Entries**
 
 To retrieve multiple entries of a particular content type, use the code snippet given below:
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment')
-query = stack.content_type("content_type_uid").query()
-result = query.find()
-```
 
-### Advanced Queries
+**stack is an instance of Stack class**
 
-You can query for content types, entries, assets and more using our Python API Reference.
+.. code-block:: python
 
-[Python API Reference Doc](https://www.contentstack.com/docs/platforms/python/api-reference/)
+   query = stack.content_type("content_type_uid").query()
+   result = query.find()
 
-### Working with Images
+**Advanced Queries**
 
-We have introduced Image Delivery APIs that let you retrieve images and then manipulate and optimize them for your digital properties. It lets you perform a host of other actions such as crop, trim, resize, rotate, overlay, and so on.
+     You can query for content types, entries, assets, and more using our Java API Reference. `Python API Reference Doc <https://www.contentstack.com/docs/platforms/python/api-reference/>`_
 
-For example, if you want to crop an image (with width as 300 and height as 400), you simply need to append query parameters at the end of the image URL, such as, `https://images.contentstack.io/v3/assets/download?crop=300,400`. There are several more parameters that you can use for your images.
 
-[Read Image Delivery API documentation](https://www.contentstack.com/docs/platforms/python/api-reference/).
+**Working with Images**
 
-You can use the Image Delivery API functions in this SDK as well. Here are a few examples of its usage in the SDK.
+    We have introduced Image Delivery APIs that let you retrieve images and then manipulate and optimize them for your digital properties. It lets you perform a host of other actions such as crop, trim, resize, rotate, overlay, and so on.
 
-```python
-image = stack.image_transform(url, {'quality': 100}).get_url()
-image = stack.image_transform(url, {'width': 100, 'height': 100}).get_url()
-image = stack.image_transform(url, {'auto': 'webp'}).get_url()
-```
+*For example:*
 
-### Using the Sync API with Python SDK
+    If you want to crop an image (with a width of 300 and height of 400), you simply need to append query parameters at the end of the image URL, such as
 
-The Sync API takes care of syncing your Contentstack data with your application and ensures that the data is always up-to-date by providing delta updates. Contentstack’s Python SDK supports Sync API, which you can use to build powerful applications.
+.. code-block:: python
+
+   https://images.contentstack.io/v3/assets/download?crop=300,400
+
+
+There are several more parameters that you can use for your images. `Read Image Delivery API documentation <https://www.contentstack.com/docs/platforms/python/api-reference/>`_
+
+You can use the Image Delivery API functions in this SDK as well. Here are a few examples of its usage in the SDK.
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment') #initialize sync
-response = stack.sync_init() #sycn using sync token
-response = stack.sync_token('sync_token') #sycn using pagination token
-response = stack.pagination('pagination_token') #sync using multiple parameters
-response = stack.sync_init(publish_type='entry_published', content_type_uid='content_type_uid')
-```
+.. code-block:: python
 
-Read through to understand how to use the Sync API with Contentstack Python SDK.
+   url = stack.image_transform(image_url, {'quality': 100})
+   url = stack.image_transform(imageUrl, {'width': 100, 'height': 100})
+   url = stack.image_transform(imageUrl, {'auto': 'webp'})
 
-[Using the Sync API with Python SDK](https://www.contentstack.com/docs/developers/python/using-the-sync-api-with-python-sdk)
+**Using the Sync API with Python SDK**
 
-### Helpful Links
+    The Sync API takes care of syncing your Contentstack data with your application and ensures that the data is always up-to-date by providing delta updates. Contentstack’s Python SDK supports Sync API, which you can use to build powerful applications.
 
-- [Contentstack Website](https://www.contentstack.com)
-- [Official Documentation](https://contentstack.com/docs)
-- [Content Delivery API Docs](https://www.contentstack.com/docs/developers/apis/content-delivery-api/)
+Read through to understand how to use the Sync API with Contentstack Python SDK. `Using the Sync API with Python SDK <https://www.contentstack.com/docs/developers/python/using-the-sync-api-with-python-sdk>`_
 
-### The MIT License (MIT)
 
-Copyright © 2012-2021 [Contentstack](https://www.contentstack.com/). All Rights Reserved
+**Helpful Links**
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+  `Contentstack Website <https://www.contentstack.com>`_
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+  `Official Documentation <https://www.contentstack.com/docs/developers/apis/content-delivery-api/>`_
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+  `Content Delivery API Docs <https://www.contentstack.com/docs/developers/apis/content-delivery-api>`_.
 
-- [Content Delivery API Docs](https://contentstack.com/docs/apis/content-delivery-api/)
 
+The MIT License (MIT)
+^^^^^^^^^^^^^^^^^^^^^
 
+    Copyright © 2012-2023 Contentstack. All Rights Reserved Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+    
+    The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+    
+    *THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE*
```

### Comparing `Contentstack-1.7.0/Contentstack.egg-info/SOURCES.txt` & `Contentstack-1.8.0/Contentstack.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 Contentstack.egg-info/requires.txt
 Contentstack.egg-info/top_level.txt
 contentstack/__init__.py
 contentstack/asset.py
 contentstack/assetquery.py
 contentstack/basequery.py
 contentstack/contenttype.py
+contentstack/controller.py
+contentstack/deep_merge_lp.py
 contentstack/entry.py
 contentstack/entryqueryable.py
 contentstack/https_connection.py
 contentstack/image_transform.py
 contentstack/query.py
 contentstack/stack.py
-contentstack/utility.py
+contentstack/utility.py
+tests/test_assets.py
+tests/test_entry.py
+tests/test_live_preview.py
+tests/test_query.py
+tests/test_stack.py
```

### Comparing `Contentstack-1.7.0/LICENSE` & `Contentstack-1.8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2012 - 2021 Contentstack. All rights reserved.
+Copyright (c) 2012 - 2023 Contentstack. All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `Contentstack-1.7.0/PKG-INFO` & `Contentstack-1.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,166 @@
 Metadata-Version: 2.1
 Name: Contentstack
-Version: 1.7.0
+Version: 1.8.0
 Summary: Contentstack is a headless CMS with an API-first approach.
 Home-page: https://github.com/contentstack/contentstack-python
 Author: Contentstack
 Author-email: shailesh.mishra@contentstack.com
 License: MIT
 Keywords: contentstack-python
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#
+================
+**Contentstack**
+================
 
-[![Contentstack](https://www.contentstack.com/docs/static/images/contentstack.png)](https://www.contentstack.com/)
+Python SDK for Contentstack
+===========================
 
-<!-- ![Python package](https://github.com/contentstack/contentstack-python/workflows/Python%20package/badge.svg?branch=master) -->
+  Contentstack is a headless CMS with an API-first approach. It is a CMS that developers can use to build powerful cross-platform applications in their favorite languages. Build your application frontend, and Contentstack will take care of the rest. `Read More <https://www.contentstack.com/>`_.
 
-![build](https://img.shields.io/badge/build-passing-green?style=plastic)
-![Coverage](https://raw.githubusercontent.com/contentstack/contentstack-python/b4edf799276f586dce3e57fa5502036cd5fd8da3/coverage.svg) ![pip](https://img.shields.io/badge/pip-v1.6.0-blue?style=plastic) ![python](https://img.shields.io/badge/python-3.5|3.6|3.7|3.8-blue?style=plastic) [![GitHub license](https://img.shields.io/github/license/contentstack/contentstack-python?style=plastic)](https://github.com/contentstack/contentstack-python/blob/master/LICENSE) [![GitHub stars](https://img.shields.io/github/stars/contentstack/contentstack-python?style=plastic)](https://github.com/contentstack/contentstack-python/stargazers)
+  Contentstack provides Python SDK to build an application on top of Python. Given below is the detailed guide and helpful resources to get started with our Python SDK.
 
-## Python SDK for Contentstack
+Prerequisite
+============
 
-Contentstack is a headless CMS with an API-first approach. It is a CMS that developers can use to build powerful cross-platform applications in their favorite languages. Build your application frontend, and Contentstack will take care of the rest. [Read More](https://www.contentstack.com/).
+  You will need python 3 installed on your machine. You can install it from `here <https://www.python.org/ftp/python/3.7.4/python-3.7.4-macosx10.9.pkg>`_
 
-Contentstack provides Python SDK to build application on top of Python. Given below is the detailed guide and helpful resources to get started with our Python SDK.
+Setup and Installation
+======================
 
-### Prerequisite
+  To use the Contentstack Python SDK to your existing project, perform the steps given below:
 
-You will need python 3 installed on your machine. You can install it from [here](https://www.python.org/ftp/python/3.7.4/python-3.7.4-macosx10.9.pkg).
+.. code-block:: python
+    install contentstack pip
 
-### Setup and Installation
+This is the preferred method to install contentstack, as it will always install the most recent stable release. If you don't have `pip <https://pip.pypa.io/>`_
+installed, this `Python installation guide <http://docs.python-guide.org/en/latest/starting/installation/>`_ can guide you through the process
 
-To use the Contentstack Python SDK to your existing project, perform the steps given below:
 
-### Install contentstack pip
+Key Concepts for using Contentstack
+-----------------------------------
 
-```pyhton
-pip install contentstack
-```
+**Stack**
 
-Install latest [contentstack](https://pypi.org/project/Contentstack) package from the [PyPI](https://pypi.org)
+  A stack is like a container that holds the content of your app. Learn more about `Stacks <https://www.contentstack.com/docs/developers/set-up-stack>`_.
 
-This is the preferred method to install contentstack, as it will always install the most recent stable release. If you don't have [pip](https://pip.pypa.io/) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process
+**Content-Type**
 
-### Key Concepts for using Contentstack
+  Content-type lets you define the structure or blueprint of a page or a section of your digital property. It is a form-like page that gives Content Managers an interface to input and upload content. `read_more <https://www.contentstack.com/docs/developers/create-content-types>`_.
 
-#### Stack
+**Entry**
 
-A stack is like a container that holds the content of your app. Learn more about [Stacks](https://www.contentstack.com/docs/developers/set-up-stack).
+    An entry is the actual piece of content created using one of the defined content types. Learn more about `Entries <https://www.contentstack.com/docs/content-managers/work-with-entries>`_.
 
-#### Content Type
+**Asset**
 
-Content type lets you define the structure or blueprint of a page or a section of your digital property. It is a form-like page that gives Content Managers an interface to input and upload content. [Read more](https://www.contentstack.com/docs/developers/create-content-types).
+    Assets refer to all the media files (images, videos, PDFs, audio files, and so on) uploaded to Contentstack. These files can be used in multiple entries. Read more about `Assets <https://www.contentstack.com/docs/content-managers/work-with-assets>`_.
 
-#### Entry
+**Environment**
 
-An entry is the actual piece of content created using one of the defined content types. Learn more about [Entries](https://www.contentstack.com/docs/content-managers/work-with-entries).
+    A publishing environment corresponds to one or more deployment servers or a content delivery destination where the entries need to be published. Learn how to work with `Environments <https://www.contentstack.com/docs/developers/set-up-environments)>`_.
 
-#### Asset
 
-Assets refer to all the media files (images, videos, PDFs, audio files, and so on) uploaded to Contentstack. These files can be used in multiple entries. Read more about [Assets](https://www.contentstack.com/docs/content-managers/work-with-assets).
 
-#### Environment
+Contentstack Python SDK: 5-minute Quickstart
+--------------------------------------------
 
-A publishing environment corresponds to one or more deployment servers or a content delivery destination where the entries need to be published. Learn how to work with [Environments](https://www.contentstack.com/docs/developers/set-up-environments).
+**Initializing your SDK**
 
-### Contentstack Python SDK: 5-minute Quickstart
+    To initialize the SDK, specify the application  API key, access token, and environment name of the stack as shown in the snippet given below:
 
-#### Initializing your SDK
+.. code-block:: python
 
-To initialize the SDK, specify application API key, access token, and environment name of the stack as shown in the snippet given below, You can provide optional parameters for config:
+   stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment')
-```
 
 To get the API credentials mentioned above, log in to your Contentstack account and then in your top panel navigation, go to Settings &gt; Stack to view the API Key and Access Token.
 
-#### Querying content from your stack
+
+
+**Querying content from your stack**
 
 To retrieve a single entry from a content type use the code snippet given below:
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment')
-content_type = stack.content_type("content_type_uid")
-entry = content_type.entry("entry_uid")
-result = entry.fetch()
-```
+.. code-block:: python
+
+   content_type = stack.content_type("content_type_uid")
+   entry = content_type.entry("entry_uid")
+   result = entry.fetch()
 
-##### Get Multiple Entries
+
+**Get Multiple Entries**
 
 To retrieve multiple entries of a particular content type, use the code snippet given below:
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment')
-query = stack.content_type("content_type_uid").query()
-result = query.find()
-```
 
-### Advanced Queries
+**stack is an instance of Stack class**
 
-You can query for content types, entries, assets and more using our Python API Reference.
+.. code-block:: python
 
-[Python API Reference Doc](https://www.contentstack.com/docs/platforms/python/api-reference/)
+   query = stack.content_type("content_type_uid").query()
+   result = query.find()
 
-### Working with Images
+**Advanced Queries**
 
-We have introduced Image Delivery APIs that let you retrieve images and then manipulate and optimize them for your digital properties. It lets you perform a host of other actions such as crop, trim, resize, rotate, overlay, and so on.
+     You can query for content types, entries, assets, and more using our Java API Reference. `Python API Reference Doc <https://www.contentstack.com/docs/platforms/python/api-reference/>`_
 
-For example, if you want to crop an image (with width as 300 and height as 400), you simply need to append query parameters at the end of the image URL, such as, `https://images.contentstack.io/v3/assets/download?crop=300,400`. There are several more parameters that you can use for your images.
 
-[Read Image Delivery API documentation](https://www.contentstack.com/docs/platforms/python/api-reference/).
+**Working with Images**
 
-You can use the Image Delivery API functions in this SDK as well. Here are a few examples of its usage in the SDK.
+    We have introduced Image Delivery APIs that let you retrieve images and then manipulate and optimize them for your digital properties. It lets you perform a host of other actions such as crop, trim, resize, rotate, overlay, and so on.
 
-```python
-image = stack.image_transform(url, {'quality': 100}).get_url()
-image = stack.image_transform(url, {'width': 100, 'height': 100}).get_url()
-image = stack.image_transform(url, {'auto': 'webp'}).get_url()
-```
+*For example:*
 
-### Using the Sync API with Python SDK
+    If you want to crop an image (with a width of 300 and height of 400), you simply need to append query parameters at the end of the image URL, such as
 
-The Sync API takes care of syncing your Contentstack data with your application and ensures that the data is always up-to-date by providing delta updates. Contentstack’s Python SDK supports Sync API, which you can use to build powerful applications.
+.. code-block:: python
+
+   https://images.contentstack.io/v3/assets/download?crop=300,400
+
+
+There are several more parameters that you can use for your images. `Read Image Delivery API documentation <https://www.contentstack.com/docs/platforms/python/api-reference/>`_
+
+You can use the Image Delivery API functions in this SDK as well. Here are a few examples of its usage in the SDK.
 
-```python
-stack = contentstack.Stack('api_key','delivery_token','environment') #initialize sync
-response = stack.sync_init() #sycn using sync token
-response = stack.sync_token('sync_token') #sycn using pagination token
-response = stack.pagination('pagination_token') #sync using multiple parameters
-response = stack.sync_init(publish_type='entry_published', content_type_uid='content_type_uid')
-```
+.. code-block:: python
 
-Read through to understand how to use the Sync API with Contentstack Python SDK.
+   url = stack.image_transform(image_url, {'quality': 100})
+   url = stack.image_transform(imageUrl, {'width': 100, 'height': 100})
+   url = stack.image_transform(imageUrl, {'auto': 'webp'})
 
-[Using the Sync API with Python SDK](https://www.contentstack.com/docs/developers/python/using-the-sync-api-with-python-sdk)
+**Using the Sync API with Python SDK**
 
-### Helpful Links
+    The Sync API takes care of syncing your Contentstack data with your application and ensures that the data is always up-to-date by providing delta updates. Contentstack’s Python SDK supports Sync API, which you can use to build powerful applications.
 
-- [Contentstack Website](https://www.contentstack.com)
-- [Official Documentation](https://contentstack.com/docs)
-- [Content Delivery API Docs](https://www.contentstack.com/docs/developers/apis/content-delivery-api/)
+Read through to understand how to use the Sync API with Contentstack Python SDK. `Using the Sync API with Python SDK <https://www.contentstack.com/docs/developers/python/using-the-sync-api-with-python-sdk>`_
 
-### The MIT License (MIT)
 
-Copyright © 2012-2021 [Contentstack](https://www.contentstack.com/). All Rights Reserved
+**Helpful Links**
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+  `Contentstack Website <https://www.contentstack.com>`_
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+  `Official Documentation <https://www.contentstack.com/docs/developers/apis/content-delivery-api/>`_
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+  `Content Delivery API Docs <https://www.contentstack.com/docs/developers/apis/content-delivery-api>`_.
 
-- [Content Delivery API Docs](https://contentstack.com/docs/apis/content-delivery-api/)
 
+The MIT License (MIT)
+^^^^^^^^^^^^^^^^^^^^^
 
+    Copyright © 2012-2023 Contentstack. All Rights Reserved Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+    
+    The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+    
+    *THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE*
```

### Comparing `Contentstack-1.7.0/README.rst` & `Contentstack-1.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -133,12 +133,12 @@
 
   `Content Delivery API Docs <https://www.contentstack.com/docs/developers/apis/content-delivery-api>`_.
 
 
 The MIT License (MIT)
 ^^^^^^^^^^^^^^^^^^^^^
 
-    Copyright © 2012-2020 Contentstack. All Rights Reserved Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+    Copyright © 2012-2023 Contentstack. All Rights Reserved Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
     
     The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
     
     *THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE*
```

### Comparing `Contentstack-1.7.0/contentstack/asset.py` & `Contentstack-1.8.0/contentstack/asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 r"""Assets refer to all the media files (images, videos, PDFs, audio files,
 and so on) uploaded in your Contentstack repository for future use.
 
 These files can be attached and used in multiple entries.
 """
 
-# ************* Module asset **************
-# Your code has been rated at 10/10 by pylint
-
 import logging
 from urllib import parse
 
 log = logging.getLogger(__name__)
 
 
 class Asset:
@@ -18,16 +15,15 @@
 
     def __init__(self, http_instance, uid=None):
         self.http_instance = http_instance
         self.asset_params = {}
         self.__uid = uid
         if self.__uid is None or self.__uid.strip() == 0:
             raise KeyError('Please provide valid uid')
-        self.base_url = '{}/assets/{}'.format(
-            self.http_instance.endpoint, self.__uid)
+        self.base_url = f'{self.http_instance.endpoint}/assets/{self.__uid}'
         if 'environment' in self.http_instance.headers:
             self.asset_params['environment'] = self.http_instance.headers['environment']
 
     def environment(self, environment):
         r"""Provide the name of the environment if you wish to retrieve the assets published
         in a particular environment.
         :param environment {str} - name of the environment
@@ -129,9 +125,9 @@
         [Example]:
             >>> import contentstack
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> asset = stack.asset(uid='asset_uid')
             >>> result = asset.fetch()
         ------------------------------
         """
-        url = '{}?{}'.format(self.base_url, parse.urlencode(self.asset_params))
+        url = f'{self.base_url}?{parse.urlencode(self.asset_params)}'
         return self.http_instance.get(url)
```

### Comparing `Contentstack-1.7.0/contentstack/assetquery.py` & `Contentstack-1.8.0/contentstack/assetquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 r"""This call fetches the list of all the assets of a particular stack.
 It also returns the content of each asset in JSON format.
 You can also specify the environment of which you wish to get the assets.
 """
 
-# ************* Module assetquery **************
-# Your code has been rated at 10/10 by pylint
-
 import json
 import logging
 
 from contentstack.basequery import BaseQuery
 from contentstack.utility import Utils
 
 log = logging.getLogger(__name__)
@@ -125,14 +122,30 @@
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> result = stack.asset_query().include_fallback().find()
         ----------------------------
         """
         self.asset_query_params['include_fallback'] = 'true'
         return self
 
+    def include_metadata(self):
+        """Retrieve the metadata in the response.
+
+        :return: AssetQuery, so we can chain the call
+
+        ----------------------------
+        Example::
+
+            >>> import contentstack
+            >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
+            >>> result = stack.asset_query().include_metadata().find()
+        ----------------------------
+        """
+        self.asset_query_params['include_metadata'] = 'true'
+        return self
+
     def locale(self, locale: str):
         """Enter locale code. e.g., en-us
         This retrieves published entries of specific locale..
 
         :return: AssetQuery, so we can chain the call
 
         ----------------------------
```

### Comparing `Contentstack-1.7.0/contentstack/basequery.py` & `Contentstack-1.8.0/contentstack/basequery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import enum
 import logging
 
 log = logging.getLogger(__name__)
 
 
-# ************* Module basequery.py **************
-# Your code has been rated at 10.00/10
-
 class QueryOperation(enum.Enum):
     """
     QueryOperation is enum that Provides Options to perform operation to query the result.
 
     Available Options for QueryOperation are below.
     EQUALS, NOT_EQUALS, INCLUDES, EXCLUDES, IS_LESS_THAN, IS_LESS_THAN_OR_EQUAL
     IS_GREATER_THAN, IS_GREATER_THAN_OR_EQUAL, EXISTS, MATCHES
@@ -156,15 +153,15 @@
             [self] -- Class instance, So that method chaining can be performed
         """
         self.query_params.update(param)
         return self
 
     def query(self, key: str, value):
         """
-        Adds key value pairs to the to the query parameters
+        Adds key value pairs to the query parameters
         Arguments:
             key {str} -- key of the query param
             value {any} -- value of query param
         Raises:
             `KeyError`: when key or value found None
         Returns:
             self-- Class instance, So that method chaining can be performed
```

### Comparing `Contentstack-1.7.0/contentstack/contenttype.py` & `Contentstack-1.8.0/contentstack/contenttype.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,18 +87,17 @@
             >>> response = content_type.fetch(some_dict)
         ------------------------------
         """
         if self.__content_type_uid is None:
             raise KeyError(
                 'content_type_uid can not be None to fetch contenttype')
         self.local_param['environment'] = self.http_instance.headers['environment']
-        uri = '{}/content_types/{}'.format(
-            self.http_instance.endpoint, self.__content_type_uid)
+        uri = f'{self.http_instance.endpoint}/content_types/{self.__content_type_uid}'
         encoded_params = parse.urlencode(self.local_param)
-        url = '{}?{}'.format(uri, encoded_params)
+        url = f'{uri}?{encoded_params}'
         result = self.http_instance.get(url)
         return result
 
     def find(self, params=None):
         """
         This method is useful to fetch ContentType of the of the stack.
         :param params: dictionary of params
@@ -113,11 +112,11 @@
             >>> response = content_type.find(param=some_dict)
         ------------------------------
         """
         self.local_param['environment'] = self.http_instance.headers['environment']
         if params is not None:
             self.local_param.update(params)
         encoded_params = parse.urlencode(self.local_param)
-        url = '{}?{}'.format(
-            '{}/content_types'.format(self.http_instance.endpoint), encoded_params)
+        endpoint = self.http_instance.endpoint
+        url = f'{endpoint}/content_types?{encoded_params}'
         result = self.http_instance.get(url)
         return result
```

### Comparing `Contentstack-1.7.0/contentstack/entry.py` & `Contentstack-1.8.0/contentstack/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """
 The Get a single entry request fetches a particular entry of a content type.
 API Reference: https://www.contentstack.com/docs/developers/apis/content-delivery-api/#single-entry
 """
-
+#min-similarity-lines=10
 import logging
 from urllib import parse
 
 import empty
 
+from contentstack.deep_merge_lp import DeepMergeMixin
 from contentstack.entryqueryable import EntryQueryable
 
-# ************* Module Entry **************
-# Your code has been rated at 10/10 by pylint
-
-
 log = logging.getLogger(__name__)
 
 
 class Entry(EntryQueryable):
     """
     An entry is the actual piece of content that you want to publish.
     Entries can be created for one of the available content types.
@@ -35,17 +32,17 @@
         self.http_instance = http_instance
         self.content_type_id = content_type_uid
         self.entry_uid = entry_uid
         self.base_url = self.__get_base_url()
 
     def environment(self, environment):
         """
-        Enter the name of the environment of which the entries needs to be included
+        Enter the name of the environment of which the entries need to be included
         Example: production
-        :param environment: {str} name of the environment of which the entries needs to be included.
+        :param environment: {str} name of the environment of which the entries need to be included.
         :return: Entry, so you can chain this call.
         ------------------------------
         Example::
 
             >>> import contentstack
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> content_type = stack.content_type('content_type_uid')
@@ -83,15 +80,15 @@
         return self
 
     def param(self, key, value):
         """
         This method is useful to add additional Query parameters to the entry
         :param key: {str} -- key The key as string which needs to be added to an Entry
         :param value: {object} -- value The value as string which needs to be added to an Entry
-        :return: Entry, so you can chain this call.
+        :return: @Entry, so you can chain this call.
         -----------------------------
         Example::
 
             >>> import contentstack
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> content_type = stack.content_type('content_type_uid')
             >>> entry = content_type.entry(uid='entry_uid')
@@ -164,38 +161,53 @@
             self.http_instance.endpoint = endpoint
         if None in (self.http_instance, self.content_type_id, self.entry_uid):
             raise KeyError(
                 'Provide valid http_instance, content_type_uid or entry_uid')
         url = f'{self.http_instance.endpoint}/content_types/{self.content_type_id}/entries/{self.entry_uid}'
         return url
 
-    def __validate_live_preview(self):
-        live_preview = self.http_instance.live_preview
-        if 'enable' in live_preview and live_preview['enable'] \
-                and self.content_type_id == live_preview['content_type_uid']:
-            if 'live_preview' in live_preview:
-                self.entry_param['live_preview'] = live_preview['live_preview']
-            else:
-                self.entry_param['live_preview'] = 'init'
-
     def fetch(self):
         """
         Fetches the latest version of the entries from stack
         :return: Entry, so you can chain this call.
         -------------------------------
         [Example:]
 
             >>> import contentstack
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> content_type = stack.content_type('content_type_uid')
             >>> entry = content_type.entry('uid')
             >>> result = entry.fetch()
         -------------------------------
         """
-        self.__validate_live_preview()
         if 'environment' in self.http_instance.headers:
             self.entry_param['environment'] = self.http_instance.headers['environment']
         if len(self.entry_queryable_param) > 0:
             self.entry_param.update(self.entry_queryable_param)
-        encoded_string = parse.urlencode(self.entry_param, doseq=True)
-        url = f'{self.base_url}?{encoded_string}'
-        return self.http_instance.get(url)
+        encoded_str = parse.urlencode(self.entry_param, doseq=True)
+        url = f'{self.base_url}?{encoded_str}'
+        self._impl_live_preview()
+        response = self.http_instance.get(url)
+        if self.http_instance.live_preview is not None and not 'errors' in response:
+            self.http_instance.live_preview['entry_response'] = response['entry']
+            return self._merged_response()
+        return response
+
+    def _impl_live_preview(self):
+        lv = self.http_instance.live_preview
+        if lv is not None and lv['enable'] and 'content_type_uid' in lv and lv[
+            'content_type_uid'] == self.content_type_id:
+            url = lv['url']
+            self.http_instance.headers['authorization'] = lv['management_token']
+            lp_resp = self.http_instance.get(url)
+            if lp_resp is not None and not 'error_code' in lp_resp:
+                self.http_instance.live_preview['lp_response'] = lp_resp
+            return None
+        return None
+
+    def _merged_response(self):
+        if 'entry_response' in self.http_instance.live_preview and 'lp_response' in self.http_instance.live_preview:
+            entry_response = self.http_instance.live_preview['entry_response']['entry']
+            lp_response = self.http_instance.live_preview['lp_response']
+            merged_response = DeepMergeMixin(entry_response, lp_response)
+            return merged_response.entry_response
+        pass
```

### Comparing `Contentstack-1.7.0/contentstack/entryqueryable.py` & `Contentstack-1.8.0/contentstack/entryqueryable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
 EntryQueryable class contains common functions
 that is used as parents class for the query and entry classes
 """
 import logging
 
-# ************* Module EntryQueryable **************
-# Your code has been rated at 10/10 by pylint
-
 log = logging.getLogger(__name__)
 
 
 class EntryQueryable:
     """
     This class is base class for the Entry and Query class that shares common functions
     """
@@ -153,14 +150,28 @@
             >>> entry = stack.content_type('content_type_uid').entry('entry_uid')
             >>> entry = entry.include_reference_content_type_uid()
             >>> result = entry.fetch()
         """
         self.entry_queryable_param['include_reference_content_type_uid'] = 'true'
         return self
 
+    def include_metadata(self):
+        """
+        This method also includes the metadata in the response
+        [Example for Query]
+            >>> import contentstack
+            >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
+            >>> content_type = stack.content_type('content_type_uid')
+            >>> query = content_type.query()
+            >>> query = query.include_metadata()
+            >>> result = query.find()
+        """
+        self.entry_queryable_param['include_metadata'] = 'true'
+        return self
+
     def add_param(self, key: str, value: str):
         """
         This method adds key and value to an Entry.
         :param key: The key as string which needs to be added to an Entry
         :param value: The value as string which needs to be added to an Entry
         :return: self: object, so you can chain this call.
```

### Comparing `Contentstack-1.7.0/contentstack/image_transform.py` & `Contentstack-1.8.0/contentstack/image_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 It is an second parameter in which we want to place different manipulation key and
 value in array form ImageTransform method is define for image manipulation with
 different transform_params in second parameter in array form
 """
 
 import logging
 
-# ************* Module image_transform **************
-# Your code has been rated at 10.00/10  by pylint
-
 log = logging.getLogger(__name__)
 
 
 class ImageTransform:  # pylint: disable=too-few-public-methods
     """
     The Image Delivery API is used to retrieve, manipulate and/or convert image
     files
```

### Comparing `Contentstack-1.7.0/contentstack/query.py` & `Contentstack-1.8.0/contentstack/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Contentstack provides certain queries that you can use to fetch filtered results
 """
+#min-similarity-lines=10
 import enum
 import json
 import logging
+import warnings
 from urllib import parse
+
 import empty
 
 from contentstack.basequery import BaseQuery
+from contentstack.deep_merge_lp import DeepMergeMixin
 from contentstack.entryqueryable import EntryQueryable
 
-# ************* Module query.py **************
-# Your code has been rated at 10.00/10  by pylint
-
 log = logging.getLogger(__name__)
 
 
 class QueryType(enum.Enum):
     """
     Get entries that satisfy all the conditions provided by enum(AND, OR)
     enum ([AND, OR]): Get entries that satisfy all the conditions provided by enum
@@ -118,14 +119,15 @@
             self.query_params["tags"] = ",".join(tags)
         return self
 
     def search(self, value: str):
         """
         This method provides only the entries matching
         the specified value.
+        @Deprecated deprecated in 1.7.0, Use #regex instaead
         Arguments:
             value {str} -- value used to match or compare
         Raises:
             ValueError: If value is None
             ValueError: If type od value is not str
         Returns:
             [Query] -- Query object, so you can chain this call.
@@ -135,14 +137,15 @@
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> content_type = stack.content_type('content_type_uid')
             >>> query = content_type.query()
             >>> query = query.search("search_keyword")
             >>> result = query.find()
         -------------------------------------
         """
+        warnings.warn('deprecated in 1.7.0, Use regex function instead')
         if value is not None:
             self.query_params["typeahead"] = value
         return self
 
     def where_in(self, key: str, query_object):
         """Get entries having values based on referenced fields.
         This query retrieves all entries that satisfy the query
@@ -255,14 +258,33 @@
             >>> query = query.include_embedded_items()
             >>> result = query.find()
         ----------------------------
         """
         self.query_params['include_embedded_items[]'] = "BASE"
         return self
 
+    def include_metadata(self):
+        """include_metadata instance of Query
+                includes metadata in the response (Entries and Assets) along with entry/entries details.
+                :return: Query, so we can chain the call
+
+                ----------------------------
+                Example:
+
+                    >>> import contentstack
+                    >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
+                    >>> content_type = stack.content_type('content_type_uid')
+                    >>> query = content_type.query()
+                    >>> query = query.include_metadata()
+                    >>> result = query.find()
+                ----------------------------
+                """
+        self.query_params['include_metadata'] = 'true'
+        return self
+
     def find(self):
         """It fetches the query result.
         List of :class:`Entry <contentstack.entry.Entry>` objects.
         Raises:
             ValueError: If content_type_id is None
             ValueError: If content_type_id is empty or not str type
         Returns:
@@ -290,28 +312,42 @@
             >>> query = content_type.query()
             >>> result = query.find_one()
         -------------------------------------
         """
         self.query_params["limit"] = 1
         return self.__execute_network_call()
 
-    def __validate_live_preview(self):
-        live_preview = self.http_instance.live_preview
-        if 'enable' in live_preview and live_preview['enable'] \
-                and self.content_type_uid == live_preview['content_type_uid']:
-            if 'live_preview' in live_preview:
-                self.query_params['live_preview'] = live_preview['live_preview']
-            else:
-                self.query_params['live_preview'] = 'init'  # initialise
-
     def __execute_network_call(self):
         if len(self.entry_queryable_param) > 0:
             self.query_params.update(self.entry_queryable_param)
         if len(self.parameters) > 0:
             self.query_params["query"] = json.dumps(self.parameters)
         if 'environment' in self.http_instance.headers:
             self.query_params['environment'] = self.http_instance.headers['environment']
-        self.__validate_live_preview()
         encoded_string = parse.urlencode(self.query_params, doseq=True)
         url = f'{self.base_url}?{encoded_string}'
-        # url = '{}?{}'.format(self.base_url, encoded_string)
-        return self.http_instance.get(url)
+        self._impl_live_preview()
+        response = self.http_instance.get(url)
+        if self.http_instance.live_preview is not None and not 'errors' in response:
+            self.http_instance.live_preview['entry_response'] = response['entries']
+            return self._merged_response()
+        return response
+
+    def _impl_live_preview(self):
+        lv = self.http_instance.live_preview
+        if lv is not None and lv['enable'] and 'content_type_uid' in lv and lv[
+            'content_type_uid'] == self.content_type_uid:
+            url = lv['url']
+            self.http_instance.headers['authorization'] = lv['management_token']
+            lp_resp = self.http_instance.get(url)
+            if lp_resp is not None and not 'error_code' in lp_resp:
+                self.http_instance.live_preview['lp_response'] = lp_resp
+            return None
+        return None
+
+    def _merged_response(self):
+        if 'entry_response' in self.http_instance.live_preview and 'lp_response' in self.http_instance.live_preview:
+            entry_response = self.http_instance.live_preview['entry_response']['entries']
+            lp_response = self.http_instance.live_preview['lp_response']
+            merged_response = DeepMergeMixin(entry_response, lp_response)
+            return merged_response.entry_response
+        pass
```

### Comparing `Contentstack-1.7.0/contentstack/stack.py` & `Contentstack-1.8.0/contentstack/stack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-"""
-Class that wraps the credentials of the authenticated user. Think of
-this as a container that holds authentication related data.
-"""
-
 import enum
 import logging
 from urllib import parse
 from urllib3.util import Retry
 
 from contentstack.asset import Asset
 from contentstack.assetquery import AssetQuery
 from contentstack.contenttype import ContentType
 from contentstack.https_connection import HTTPSConnection
 from contentstack.image_transform import ImageTransform
 
-__author__ = "ishaileshmishra (ishaileshmishra@gmail.com)"
+__author__ = "ishaileshmishra (shailesh.mishra@contentstack.com)"
 __license__ = "MIT"
-__version__ = '1.7.0'
+__version__ = '1.8.0'
 
 log = logging.getLogger(__name__)
 DEFAULT_HOST = 'cdn.contentstack.io'
 
 
 class ContentstackRegion(enum.Enum):
     """
     Sets region for the contentstack
     """
     US = 'us'
     EU = 'eu'
     AZURE_NA = 'azure-na'
+    AZURE_EU = 'azure-eu'
 
 
 class Stack:
     """
     A stack can be defined as a pool of data or a container that holds all
     the content/assets related to a site. It is a collaboration space where multiple users can work
     together to create, edit, approve, and publish content.
@@ -46,49 +42,48 @@
                  timeout=30,
                  retry_strategy=Retry(
                      total=5, backoff_factor=0, status_forcelist=[408, 429]),
                  live_preview=None,
                  branch=None,
                  ):
         """
-        Class that wraps the credentials of the authenticated user. Think of
+        # Class that wraps the credentials of the authenticated user. Think of
         this as a container that holds authentication related data.
 
         param api_key: api_key of the stack
         :param delivery_token: delivery_token of the stack
         :param environment: environment of the stack
         :param host: (optional) host of the stack default is cdm.contentstack.io
         :param branch: branch of the stack
         :param version: (optional) apiVersion of the stack default is v3
         :param region: (optional) region support of the stack default is ContentstackRegion.US
         :param live_preview: (optional) accepts type dictionary that enables
         live_preview option for request,
         takes input as dictionary object. containing one/multiple key value pair like below.
 
         ```python
-        live_preview = {
+    live_preview = {
             'enable': True,
+            'host': 'api.contentstack.io',
             'authorization': 'your_management_token',
-            'host': 'api.contentstack.com',
             'include_edit_tags': True,
             'edit_tags_type': object | str,
-        }
+            }
         ```
         :param retry_strategy: (optional) custom retry_strategy can be set.
         Method to create retry_strategy: create object of Retry() and provide the
         required parameters like below
         **Example:**
 
         >>> _strategy = Retry(total=5, backoff_factor=1, status_forcelist=[408, 429])
+        >>> import contentstack
         >>> stack = contentstack.Stack("api_key", "delivery_token", "environment",
-        live_preview={enable=True, authorization='your auth token'}, retry_strategy= _strategy)
+                live_preview={enable=True, authorization='your auth token'}, retry_strategy= _strategy)
         ```
         """
-        if live_preview is None:
-            live_preview = {'enable': False}
         logging.basicConfig(level=logging.DEBUG)
         self.headers = {}
         self._query_params = {}
         self.sync_param = {}
         self.endpoint = None
         self.http_instance = None
         self.api_key = api_key
@@ -96,68 +91,58 @@
         self.environment = environment
         self.host = host
         self.version = version
         self.region = region
         self.timeout = timeout
         self.branch = branch
         self.retry_strategy = retry_strategy
-        self.live_preview_dict = live_preview
-
+        self.live_preview = live_preview
         self._validate_stack()
 
     def _validate_stack(self):
         if self.api_key is None or self.api_key == '':
             raise PermissionError(
-                'You are not permitted to the stack without valid APIKey')
+                'You are not permitted to the stack without valid APIKey'
+            )
         if self.delivery_token is None or self.delivery_token == "":
             raise PermissionError(
-                'You are not permitted to the stack without valid Delivery Token')
+                'You are not permitted to the stack without valid Delivery Token'
+            )
         if self.environment is None or self.environment == "":
             raise PermissionError(
-                'You are not permitted to the stack without valid Environment')
+                'You are not permitted to the stack without valid Environment'
+            )
 
         if self.region.value == 'eu' and self.host == DEFAULT_HOST:
             self.host = 'eu-cdn.contentstack.com'
         elif self.region.value == 'azure-na' and self.host == DEFAULT_HOST:
             self.host = 'azure-na-cdn.contentstack.com'
+        elif self.region.value == 'azure-eu' and self.host == DEFAULT_HOST:
+            self.host = 'azure-eu-cdn.contentstack.com'
         elif self.region.value != 'us':
             self.host = f'{self.region.value}-{DEFAULT_HOST}'
         self.endpoint = f'https://{self.host}/{self.version}'
 
         self.headers = {
             'api_key': self.api_key,
             'access_token': self.delivery_token,
             'environment': self.environment
         }
 
         if self.branch is not None:
             self.headers['branch'] = self.branch
 
-        if self.live_preview_dict is not None:
-            self._validate_live_preview()
         self.http_instance = HTTPSConnection(
             endpoint=self.endpoint,
-            headers=self.headers, timeout=self.timeout,
+            headers=self.headers,
+            timeout=self.timeout,
             retry_strategy=self.retry_strategy,
-            live_preview=self.live_preview_dict
+            live_preview=self.live_preview
         )
 
-    def _validate_live_preview(self):
-        if isinstance(self.live_preview_dict, dict):
-            if 'enable' in self.live_preview_dict and self.live_preview_dict['enable']:
-                if 'authorization' not in self.live_preview_dict:
-                    raise PermissionError("management token is required")
-                if 'host' not in self.live_preview_dict:
-                    raise PermissionError("host is required")
-                self.headers['authorization'] = self.live_preview_dict['authorization']
-                self.host = self.live_preview_dict['host']
-                self.endpoint = f'https://{self.host}/{self.version}'
-                self.headers.pop('access_token')
-                self.headers.pop('environment')
-
     @property
     def get_api_key(self):
         """
         :return: api_key of the stack
         """
         return self.api_key
 
@@ -190,30 +175,30 @@
         return self.headers
 
     @property
     def get_live_preview(self):
         """
         :return: live preview dictionary
         """
-        return self.live_preview_dict
+        return self.live_preview
 
     def content_type(self, content_type_uid=None):
         """
         Content type defines the structure or schema of a page or a section
         of your web or mobile property.
-        :param content_type_uid:
+        param content_type_uid:
         :return: ContentType
         """
         return ContentType(self.http_instance, content_type_uid)
 
     def asset(self, uid):
         """
         Assets refer to all the media files (images, videos, PDFs, audio files, and so on)
         uploaded in your Contentstack repository for future use.
-        :param uid: asset_uid of the Asset
+        param uid: asset_uid of the Asset
         :return: Asset
 
         -----------------------------
         Example: provide asset_uid to fetch single asset:
             >>> import contentstack
             >>> stack = Stack('api_key', 'delivery_token', 'environment')
             >>> asset_instance = stack.asset(uid='asset_uid')
@@ -238,15 +223,15 @@
         -----------------------------
         """
         return AssetQuery(self.http_instance)
 
     def sync_init(self, content_type_uid=None, start_from=None, locale=None, publish_type=None):
         """
         Set init to ‘true’ if you want to sync all the published entries and assets.
-        This is usually used when the app does not have any content and you want to
+        This is usually used when the app does not have any content, and you want to
         get all the content for the first time.\n
 
         :param content_type_uid: (optional) content type UID. e.g., products
                     This retrieves published entries of specified content type
         :param start_from: (optional) The start date. e.g., 2018-08-14T00:00:00.000Z
                     This retrieves published entries starting from a specific date
         :param locale: (optional) locale code. e.g., en-us, This retrieves published
@@ -281,15 +266,15 @@
     def pagination(self, pagination_token: str):
         """
         If the result of the initial sync (or subsequent sync)
         contains more than 100 records, the response would be
         paginated. It provides pagination token in the response.
         However, you do not have to use the pagination token
         manually to get the next batch.
-        :param pagination_token:
+        param pagination_token:
         :return: list of sync items
         ------------------------------
         Example:
             >>> import contentstack
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> result = stack.pagination('pagination_token')
         ------------------------------
@@ -299,57 +284,94 @@
         return self.__sync_request()
 
     def sync_token(self, sync_token):
         """You can use the sync token (that you receive after initial sync)
         to get the updated content next time. The sync token fetches
         only the content that was added
         after your last sync, and the details of the content that was deleted or updated.
-        :param sync_token: sync_token
+        param sync_token: sync_token
         :return: list of Sync Result
         ------------------------------
         [Example]:
             >>> import contentstack
             >>> stack = contentstack.Stack('api_key', 'delivery_token', 'environment')
             >>> result = stack.sync_token('sync_token')
         -------------------------------
         """
         if isinstance(sync_token, str):
             self.sync_param = {'sync_token': sync_token}
         return self.__sync_request()
 
     def __sync_request(self):
         r"""Sends a GET request.
-        :param url URL for :class:`Request` object.
+        param url is URL for :class:`Request` object.
         in the query string for the :class:`Request`.
         :param \*\*kwargs: Optional arguments that ``request`` takes.
         :return: :class:`Response <Response>` object
         :rtype: requests.Response
         """
         base_url = f'{self.http_instance.endpoint}/stacks/sync'
         self.sync_param['environment'] = self.http_instance.headers['environment']
-        encoded_query = parse.urlencode(self.sync_param)
-        url = f'{base_url}?{encoded_query}'
-        result = self.http_instance.get(url)
-        return result
+        query = parse.urlencode(self.sync_param)
+        url = f'{base_url}?{query}'
+        return self.http_instance.get(url)
 
     def image_transform(self, image_url, **kwargs):
         """
         This document is a detailed reference to Contentstack’s Image Delivery
         API and covers the parameters that you can add to the URL to retrieve,
         manipulate (or convert) image files and display it to your web or
         mobile properties.\n
 
         :param image_url: base url on which queries to apply
-        :param kwargs: append queries to the asset URL.
+        :param kwargs: to append queries to the asset URL.
         :return: instance of ImageTransform
         """
         if image_url is None or image_url == '':
             raise PermissionError(
                 'image_url required for the image_transformation')
         return ImageTransform(self.http_instance, image_url, **kwargs)
 
     def live_preview_query(self, **kwargs):
         """
         live_preview_query accepts key value pair objects to the query
-        i.e hash and content_type_uid
-        """
-        self.live_preview_dict.update(kwargs)
+        hash, content_type_uid and entry_uid
+        Example:
+            # def live_preview_query(**kwargs):
+            # kwargs is a dict of the keyword args passed to the function
+            for key, value in kwargs.iteritems():
+                print "%s = %s" % (key, value)
+            Uses:=>
+        live_preview_query = (
+                'enable': True,
+                'live_preview': '#*#*#*#*#',
+                'host': 'your_host',
+                'content_type_uid': 'product',
+                'entry_uid': 'your_entry_uid',
+                'authorization': 'management_token'
+                )
+        """
+
+        if self.live_preview is not None and self.live_preview['enable'] and 'live_preview_query' in kwargs:
+            self.live_preview.update(**kwargs['live_preview_query'])
+            query = kwargs['live_preview_query']
+            if query is not None:
+                self.live_preview['live_preview'] = query['live_preview']
+            else:
+                self.live_preview['live_preview'] = 'init'
+            if 'content_type_uid' in self.live_preview and self.live_preview['content_type_uid'] is not None:
+                self.live_preview['content_type_uid'] = query['content_type_uid']
+            if 'entry_uid' in self.live_preview and self.live_preview['entry_uid'] is not None:
+                self.live_preview['entry_uid'] = query['entry_uid']
+            self._cal_url()
+        return self
+
+    def _cal_url(self):
+        host = self.live_preview['host']
+        ct = self.live_preview['content_type_uid']
+        url = f'https://{host}/v3/content_types/{ct}/entries'
+        if 'entry_uid' in self.live_preview:
+            uid = self.live_preview['entry_uid']
+            lv = self.live_preview['live_preview']
+            url = f'{url}/{uid}?live_preview={lv}'
+        self.live_preview['url'] = url
+        pass
```

### Comparing `Contentstack-1.7.0/contentstack/utility.py` & `Contentstack-1.8.0/contentstack/utility.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 """
-Utils
-contentstack
-Last modified by Shailesh Mishra on 06/08/20.
+Last modified by ishaileshmishra on 06/08/20.
 Copyright 2019 Contentstack. All rights reserved.
 """
 
-# ************* Module utility checked using pylint **************
-# Your code has been rated at 10.00/10
-
 import json
 import logging
 from urllib import parse
 
 log = logging.getLogger(__name__)
 
 
@@ -26,17 +21,14 @@
         level=logging_type,
         format='[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
         datefmt='%H:%M:%S'
     )
 
 
 class Utils:
-    """
-    Utility for the contentstack
-    """
 
     @staticmethod
     def config_logging():
         """ Setting up logging """
         logging.basicConfig(
             filename='report_log.log',
             format='%(asctime)s - %(message)s',
```

### Comparing `Contentstack-1.7.0/setup.py` & `Contentstack-1.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 # https://packaging.python.org/tutorials/packaging-projects/#creating-setup-py
 # setup.py is the build script for setuptools.
 # It tells setuptools about your package (such
 # as the name and version) as well as which code files to include
-
 import os
 
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
+# import os
+#
+# try:
+#     from setuptools import setup
+# except ImportError:
+#     from distutils.core import setup
+
+# with open("README.md", "r", encoding="utf-8") as fh:
+#     long_description = fh.read()
+
+from setuptools import setup
+
+
+def read(fname):
+    return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
-with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
-    long_description = readme.read()
 
 requirements = [
     'requests>=2.20.0,<3.0',
     'python-dateutil'
 ]
 
 setup(
     title="contentstack-python",
     name="Contentstack",
     status="Active",
     type="process",
     created="09 Jun 2020",
     keywords="contentstack-python",
-    version="1.7.0",
+    version="1.8.0",
     author="Contentstack",
     author_email="shailesh.mishra@contentstack.com",
     description="Contentstack is a headless CMS with an API-first approach.",
-    long_description=long_description,
+    long_description=read("README.rst"),
     long_description_content_type="text/markdown",
     url="https://github.com/contentstack/contentstack-python",
     packages=['contentstack'],
     license='MIT',
     test_suite='tests',
     install_requires=requirements,
     include_package_data=True,
```

