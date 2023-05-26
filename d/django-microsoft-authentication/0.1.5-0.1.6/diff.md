# Comparing `tmp/django-microsoft-authentication-0.1.5.tar.gz` & `tmp/django-microsoft-authentication-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-microsoft-authentication-0.1.5.tar", last modified: Wed Apr 12 22:51:53 2023, max compression
+gzip compressed data, was "django-microsoft-authentication-0.1.6.tar", last modified: Fri May 26 09:49:04 2023, max compression
```

## Comparing `django-microsoft-authentication-0.1.5.tar` & `django-microsoft-authentication-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.752261 django-microsoft-authentication-0.1.5/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1072 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/LICENSE
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     4136 2023-04-12 22:51:53.752014 django-microsoft-authentication-0.1.5/PKG-INFO
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     3584 2023-02-16 21:39:07.000000 django-microsoft-authentication-0.1.5/README.md
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.750145 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     4136 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/PKG-INFO
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      723 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        1 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       21 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/requires.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       25 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/top_level.txt
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.751163 django-microsoft-authentication-0.1.5/microsoft_authentication/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/__init__.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/admin.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      122 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/apps.py
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.751610 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/__init__.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1002 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_decorators.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     2812 2023-02-16 21:38:43.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_utils.py
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.751855 django-microsoft-authentication-0.1.5/microsoft_authentication/migrations/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/migrations/__init__.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/models.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       60 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/tests.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      425 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/urls.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1243 2023-04-12 22:49:57.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/views.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       38 2023-04-12 22:51:53.752330 django-microsoft-authentication-0.1.5/setup.cfg
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1646 2023-04-12 22:50:48.000000 django-microsoft-authentication-0.1.5/setup.py
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-05-26 09:49:04.450044 django-microsoft-authentication-0.1.6/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1072 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/LICENSE
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     4213 2023-05-26 09:49:04.449915 django-microsoft-authentication-0.1.6/PKG-INFO
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     3661 2023-05-26 08:52:30.000000 django-microsoft-authentication-0.1.6/README.md
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-05-26 09:49:04.447824 django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     4213 2023-05-26 09:49:04.000000 django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      723 2023-05-26 09:49:04.000000 django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        1 2023-05-26 09:49:04.000000 django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       21 2023-05-26 09:49:04.000000 django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/requires.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       25 2023-05-26 09:49:04.000000 django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-05-26 09:49:04.449045 django-microsoft-authentication-0.1.6/microsoft_authentication/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/__init__.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/admin.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      122 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/apps.py
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-05-26 09:49:04.449538 django-microsoft-authentication-0.1.6/microsoft_authentication/auth/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/auth/__init__.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1002 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/auth/auth_decorators.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     3137 2023-05-26 09:44:48.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/auth/auth_utils.py
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-05-26 09:49:04.449751 django-microsoft-authentication-0.1.6/microsoft_authentication/migrations/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/migrations/__init__.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/models.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       60 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/tests.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      425 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/urls.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1243 2023-04-12 22:49:57.000000 django-microsoft-authentication-0.1.6/microsoft_authentication/views.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       38 2023-05-26 09:49:04.450093 django-microsoft-authentication-0.1.6/setup.cfg
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1646 2023-05-26 09:45:28.000000 django-microsoft-authentication-0.1.6/setup.py
```

### Comparing `django-microsoft-authentication-0.1.5/LICENSE` & `django-microsoft-authentication-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.5/PKG-INFO` & `django-microsoft-authentication-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microsoft-authentication
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django based app for Microsoft authentication of users.
 Home-page: https://github.com/shubhamdipt/django-microsoft-authentication
 Author: Shubham Dipt
 Author-email: shubham.dipt@gmail.com
 License: MIT
 Keywords: django,microsoft,authentication
 Platform: any
@@ -57,14 +57,15 @@
 LOGIN_REDIRECT_URL = "/admin"  # optional and can be changed to any other url
 
 
 # True: creates new Django User after valid microsoft authentication. 
 # False: it will only allow those users which are already created in Django User model and 
 # will validate the email using Microsoft.
 MICROSOFT_CREATE_NEW_DJANGO_USER = True  # Optional, default value is True
+MICROSOFT_NEW_DJANGO_USER_IS_STAFF = True  # Optional, default value is True
 ```
 
 
 * Add 'microsoft_authentication' to INSTALLED_APPS
 * Add the following to the project/urls.py
 
 ```python
```

### Comparing `django-microsoft-authentication-0.1.5/README.md` & `django-microsoft-authentication-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 LOGIN_REDIRECT_URL = "/admin"  # optional and can be changed to any other url
 
 
 # True: creates new Django User after valid microsoft authentication. 
 # False: it will only allow those users which are already created in Django User model and 
 # will validate the email using Microsoft.
 MICROSOFT_CREATE_NEW_DJANGO_USER = True  # Optional, default value is True
+MICROSOFT_NEW_DJANGO_USER_IS_STAFF = True  # Optional, default value is True
 ```
 
 
 * Add 'microsoft_authentication' to INSTALLED_APPS
 * Add the following to the project/urls.py
 
 ```python
```

### Comparing `django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/PKG-INFO` & `django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microsoft-authentication
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django based app for Microsoft authentication of users.
 Home-page: https://github.com/shubhamdipt/django-microsoft-authentication
 Author: Shubham Dipt
 Author-email: shubham.dipt@gmail.com
 License: MIT
 Keywords: django,microsoft,authentication
 Platform: any
@@ -57,14 +57,15 @@
 LOGIN_REDIRECT_URL = "/admin"  # optional and can be changed to any other url
 
 
 # True: creates new Django User after valid microsoft authentication. 
 # False: it will only allow those users which are already created in Django User model and 
 # will validate the email using Microsoft.
 MICROSOFT_CREATE_NEW_DJANGO_USER = True  # Optional, default value is True
+MICROSOFT_NEW_DJANGO_USER_IS_STAFF = True  # Optional, default value is True
 ```
 
 
 * Add 'microsoft_authentication' to INSTALLED_APPS
 * Add the following to the project/urls.py
 
 ```python
```

### Comparing `django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/SOURCES.txt` & `django-microsoft-authentication-0.1.6/django_microsoft_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_decorators.py` & `django-microsoft-authentication-0.1.6/microsoft_authentication/auth/auth_decorators.py`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_utils.py` & `django-microsoft-authentication-0.1.6/microsoft_authentication/auth/auth_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -84,20 +84,25 @@
 # Non-microsoft related functions
 
 
 def validate_email(email):
     return "@" in email and email.split("@")[1] in settings.MICROSOFT["valid_email_domains"]
 
 
-def get_django_user(email, create_new=True):
+def get_django_user(email, create_new=True, is_staff=True):
     if not validate_email(email=email):
         return
     try:
         user = User.objects.get(email=email)
     except User.DoesNotExist:
+        # By default creates new user
+        if hasattr(settings, "MICROSOFT_CREATE_NEW_DJANGO_USER"):
+            create_new = settings.MICROSOFT_CREATE_NEW_DJANGO_USER
+        if hasattr(settings, "MICROSOFT_NEW_DJANGO_USER_IS_STAFF"):
+            is_staff = settings.MICROSOFT_NEW_DJANGO_USER_IS_STAFF
         if not create_new:
             return
         random_password = "".join(random.choice(string.ascii_letters) for i in range(32))
         user = User(username=email, email=email, password=make_password(random_password))
-        user.is_staff = True
+        user.is_staff = is_staff
         user.save()
     return user
```

### Comparing `django-microsoft-authentication-0.1.5/microsoft_authentication/views.py` & `django-microsoft-authentication-0.1.6/microsoft_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.5/setup.py` & `django-microsoft-authentication-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools import setup
 
 # Usage: python setup.py sdist bdist_wheel
 
 links = []  # for repo urls (dependency_links)
 
 DESCRIPTION = "Django based app for Microsoft authentication of users."
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 
 setup(
     name="django-microsoft-authentication",
     version=VERSION,
     author="Shubham Dipt",
     author_email="shubham.dipt@gmail.com",
     description=DESCRIPTION,
```

