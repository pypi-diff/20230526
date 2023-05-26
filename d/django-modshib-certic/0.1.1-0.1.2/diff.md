# Comparing `tmp/django-modshib-CERTIC-0.1.1.tar.gz` & `tmp/django-modshib-CERTIC-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-modshib-CERTIC-0.1.1.tar", max compression
+gzip compressed data, was "django-modshib-CERTIC-0.1.2.tar", max compression
```

## Comparing `django-modshib-CERTIC-0.1.1.tar` & `django-modshib-CERTIC-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.653227 django-modshib-CERTIC-0.1.1/modshib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-19 06:10:59.654166 django-modshib-CERTIC-0.1.1/modshib/admin.py
--rw-r--r--   0        0        0      146 2023-05-24 09:58:37.360521 django-modshib-CERTIC-0.1.1/modshib/apps.py
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.656283 django-modshib-CERTIC-0.1.1/modshib/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-05-19 06:10:59.655746 django-modshib-CERTIC-0.1.1/modshib/models.py
--rw-r--r--   0        0        0      747 2023-05-22 09:55:06.204141 django-modshib-CERTIC-0.1.1/modshib/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1315 2023-05-24 08:51:31.235141 django-modshib-CERTIC-0.1.1/modshib/templates/registration/login.html
--rw-r--r--   0        0        0      838 2023-05-19 07:02:49.960081 django-modshib-CERTIC-0.1.1/modshib/templates/registration/reg_base.html
--rw-r--r--   0        0        0      794 2023-05-24 08:22:05.742051 django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_fail.html
--rw-r--r--   0        0        0      813 2023-05-24 09:54:48.646844 django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_no_account.html
--rw-r--r--   0        0        0       60 2023-05-19 06:10:59.655994 django-modshib-CERTIC-0.1.1/modshib/tests.py
--rw-r--r--   0        0        0      117 2023-05-22 09:06:53.828987 django-modshib-CERTIC-0.1.1/modshib/urls.py
--rw-r--r--   0        0        0     2706 2023-05-25 20:13:39.942458 django-modshib-CERTIC-0.1.1/modshib/views.py
--rw-r--r--   0        0        0      551 2023-05-25 20:11:35.911724 django-modshib-CERTIC-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      722 2023-05-25 20:56:12.103703 django-modshib-CERTIC-0.1.1/setup.py
--rw-r--r--   0        0        0      700 2023-05-25 20:56:12.103973 django-modshib-CERTIC-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-19 06:10:59.653227 django-modshib-CERTIC-0.1.2/modshib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-19 06:10:59.654166 django-modshib-CERTIC-0.1.2/modshib/admin.py
+-rw-r--r--   0        0        0      146 2023-05-24 09:58:37.360521 django-modshib-CERTIC-0.1.2/modshib/apps.py
+-rw-r--r--   0        0        0      310 2023-05-26 07:17:40.682916 django-modshib-CERTIC-0.1.2/modshib/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:10:59.656283 django-modshib-CERTIC-0.1.2/modshib/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-19 06:10:59.655746 django-modshib-CERTIC-0.1.2/modshib/models.py
+-rw-r--r--   0        0        0      897 2023-05-26 08:00:55.045522 django-modshib-CERTIC-0.1.2/modshib/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1315 2023-05-24 08:51:31.235141 django-modshib-CERTIC-0.1.2/modshib/templates/registration/login.html
+-rw-r--r--   0        0        0      838 2023-05-19 07:02:49.960081 django-modshib-CERTIC-0.1.2/modshib/templates/registration/reg_base.html
+-rw-r--r--   0        0        0      794 2023-05-24 08:22:05.742051 django-modshib-CERTIC-0.1.2/modshib/templates/registration/sso_fail.html
+-rw-r--r--   0        0        0      813 2023-05-24 09:54:48.646844 django-modshib-CERTIC-0.1.2/modshib/templates/registration/sso_no_account.html
+-rw-r--r--   0        0        0       60 2023-05-19 06:10:59.655994 django-modshib-CERTIC-0.1.2/modshib/tests.py
+-rw-r--r--   0        0        0      117 2023-05-22 09:06:53.828987 django-modshib-CERTIC-0.1.2/modshib/urls.py
+-rw-r--r--   0        0        0     2761 2023-05-26 06:27:37.660477 django-modshib-CERTIC-0.1.2/modshib/views.py
+-rw-r--r--   0        0        0      551 2023-05-26 08:01:29.464166 django-modshib-CERTIC-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      722 2023-05-26 08:09:47.354958 django-modshib-CERTIC-0.1.2/setup.py
+-rw-r--r--   0        0        0      700 2023-05-26 08:09:47.355192 django-modshib-CERTIC-0.1.2/PKG-INFO
```

### Comparing `django-modshib-CERTIC-0.1.1/modshib/templates/registration/logged_out.html` & `django-modshib-CERTIC-0.1.2/modshib/templates/registration/logged_out.html`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,11 @@
                 <div class="card-text">
                     {% translate "Vous êtes déconnecté." %}
                 </div>
                 <a href="/">{% translate "Retour à l'accueil" %}</a>
             </div>
         </div>
     </div>
+    {% if MODSHIB_SP_LOGOUT_URL %}
+        <iframe src="{{ MODSHIB_SP_LOGOUT_URL }}" style="display:none" title="SP Logout"></iframe>
+    {% endif %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% extends "registration/reg_base.html" %} {% load i18n %} {% block head_title
 %}{% translate "DÃ©connexion" %}{% endblock head_title %} {% block content %}
 ** {{ site_name }} **
 * {% translate "DÃ©connexion" %} *
 {% translate "Vous Ãªtes dÃ©connectÃ©." %}
 {%_translate_"Retour_Ã _l'accueil"_%}
-{% endblock content %}
+{% if MODSHIB_SP_LOGOUT_URL %}  {% endif %} {% endblock content %}
```

### Comparing `django-modshib-CERTIC-0.1.1/modshib/templates/registration/login.html` & `django-modshib-CERTIC-0.1.2/modshib/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.1/modshib/templates/registration/reg_base.html` & `django-modshib-CERTIC-0.1.2/modshib/templates/registration/reg_base.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_fail.html` & `django-modshib-CERTIC-0.1.2/modshib/templates/registration/sso_fail.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_no_account.html` & `django-modshib-CERTIC-0.1.2/modshib/templates/registration/sso_no_account.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.1/modshib/views.py` & `django-modshib-CERTIC-0.1.2/modshib/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,9 +68,10 @@
         user.is_active = True
         user.save()
     if not user.is_active:
         logger.info(f"user {eppn} inactive, rejecting auth")
         return render(request, "registration/sso_no_account.html")
     if user and user.is_active:
         logger.info(f"active user {eppn} found, login")
+        request.session["auth_is_from_modshib"] = True
         login(request, user)
         return HttpResponseRedirect(settings.LOGIN_REDIRECT_URL)
```

### Comparing `django-modshib-CERTIC-0.1.1/pyproject.toml` & `django-modshib-CERTIC-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-modshib-CERTIC"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>"]
 license = "Cecill-B"
 packages = [
     { include = "modshib"},
 ]
 homepage = "https://www.certic.unicaen.fr"
```

### Comparing `django-modshib-CERTIC-0.1.1/setup.py` & `django-modshib-CERTIC-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'modshib': ['templates/registration/*']}
 
 install_requires = \
 ['Django>=4.0', 'django-auth-cli-certic>=0.1.3']
 
 setup_kwargs = {
     'name': 'django-modshib-certic',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': None,
     'author': 'Mickaël Desfrênes',
     'author_email': 'mickael.desfrenes@unicaen.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.certic.unicaen.fr',
```

### Comparing `django-modshib-CERTIC-0.1.1/PKG-INFO` & `django-modshib-CERTIC-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modshib-certic
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://www.certic.unicaen.fr
 License: CECILL-B
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 Requires-Python: >=3.7
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
```

