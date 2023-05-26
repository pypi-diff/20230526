# Comparing `tmp/tlcpack-sphinx-addon-0.2.1.tar.gz` & `tmp/tlcpack-sphinx-addon-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tlcpack-sphinx-addon-0.2.1.tar", last modified: Mon Jun 28 15:12:19 2021, max compression
+gzip compressed data, was "tlcpack-sphinx-addon-0.2.2.tar", last modified: Fri May 26 17:10:18 2023, max compression
```

## Comparing `tlcpack-sphinx-addon-0.2.1.tar` & `tlcpack-sphinx-addon-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)       23 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/README.md
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)     2436 2021-04-29 16:06:52.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/themeheader.html
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)     1307 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/footer.html
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)     4289 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/breadcrumbs.html
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)    10246 2021-06-28 15:11:15.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/layout.html
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/js/
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)     1043 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/js/tlcpack_theme.js
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      245 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/downangle.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      184 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/show.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      218 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/note.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      295 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/source.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)    27870 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/pattern.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      496 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/right.svg
--rwxr-xr-x   0 tqchen    (1000) tqchen    (1000)      341 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/menu-icon.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      148 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/hide.svg
--rwxr-xr-x   0 tqchen    (1000) tqchen    (1000)      344 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/dropdown-icon.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      281 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/dwonloaddoc.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      221 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/nextarrow.svg
--rwxr-xr-x   0 tqchen    (1000) tqchen    (1000)      633 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/close-icon.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      245 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/rightangle.svg
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      223 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/prevarrow.svg
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/css/
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)    23663 2021-06-28 15:11:15.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/css/tlcpack_theme.css
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)     4186 2020-11-03 17:11:09.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/css/gallery.css
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      363 2021-04-29 17:28:57.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/__init__.py
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      990 2021-06-28 15:11:32.000000 tlcpack-sphinx-addon-0.2.1/setup.py
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      572 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/PKG-INFO
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)       79 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/setup.cfg
-drwxr-xr-x   0 tqchen    (1000) tqchen    (1000)        0 2021-06-28 15:12:19.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)       21 2021-06-28 15:12:18.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/top_level.txt
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)        1 2020-11-03 16:37:33.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/not-zip-safe
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)     1253 2021-06-28 15:12:18.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/SOURCES.txt
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)      572 2021-06-28 15:12:18.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/PKG-INFO
--rw-r--r--   0 tqchen    (1000) tqchen    (1000)        1 2021-06-28 15:12:18.000000 tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/dependency_links.txt
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.704990 tlcpack-sphinx-addon-0.2.2/
+-rw-r--r--   0 tqchen     (501) staff       (20)    11357 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/LICENSE
+-rw-r--r--   0 tqchen     (501) staff       (20)      555 2023-05-26 17:10:18.705032 tlcpack-sphinx-addon-0.2.2/PKG-INFO
+-rw-r--r--   0 tqchen     (501) staff       (20)       23 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/README.md
+-rw-r--r--   0 tqchen     (501) staff       (20)       79 2023-05-26 17:10:18.705209 tlcpack-sphinx-addon-0.2.2/setup.cfg
+-rw-r--r--   0 tqchen     (501) staff       (20)      990 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/setup.py
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.702077 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/
+-rw-r--r--   0 tqchen     (501) staff       (20)      363 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/__init__.py
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.701517 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.702813 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/css/
+-rw-r--r--   0 tqchen     (501) staff       (20)     4186 2021-06-05 17:12:12.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/css/gallery.css
+-rw-r--r--   0 tqchen     (501) staff       (20)    24330 2023-05-26 17:05:10.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/css/tlcpack_theme.css
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.704357 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/
+-rwxr-xr-x   0 tqchen     (501) staff       (20)      633 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/close-icon.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      245 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/downangle.svg
+-rwxr-xr-x   0 tqchen     (501) staff       (20)      344 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/dropdown-icon.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      281 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/dwonloaddoc.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      148 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/hide.svg
+-rwxr-xr-x   0 tqchen     (501) staff       (20)      341 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/menu-icon.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      221 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/nextarrow.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      218 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/note.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)    27870 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/pattern.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      223 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/prevarrow.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      496 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/right.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      245 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/rightangle.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      184 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/show.svg
+-rw-r--r--   0 tqchen     (501) staff       (20)      295 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/source.svg
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.704460 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/js/
+-rw-r--r--   0 tqchen     (501) staff       (20)     1212 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/js/tlcpack_theme.js
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.704884 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/
+-rw-r--r--   0 tqchen     (501) staff       (20)     4420 2023-05-26 16:16:03.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/breadcrumbs.html
+-rw-r--r--   0 tqchen     (501) staff       (20)     1320 2023-05-26 16:15:51.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/footer.html
+-rw-r--r--   0 tqchen     (501) staff       (20)    11733 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/layout.html
+-rw-r--r--   0 tqchen     (501) staff       (20)     2436 2023-05-26 16:00:14.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/themeheader.html
+drwxr-xr-x   0 tqchen     (501) staff       (20)        0 2023-05-26 17:10:18.702594 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/
+-rw-r--r--   0 tqchen     (501) staff       (20)      555 2023-05-26 17:10:18.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/PKG-INFO
+-rw-r--r--   0 tqchen     (501) staff       (20)     1261 2023-05-26 17:10:18.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/SOURCES.txt
+-rw-r--r--   0 tqchen     (501) staff       (20)        1 2023-05-26 17:10:18.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/dependency_links.txt
+-rw-r--r--   0 tqchen     (501) staff       (20)        1 2023-05-26 17:10:18.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/not-zip-safe
+-rw-r--r--   0 tqchen     (501) staff       (20)       21 2023-05-26 17:10:18.000000 tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/themeheader.html` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/themeheader.html`

 * *Files identical despite different names*

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/footer.html` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/footer.html`

 * *Files 15% similar despite different names*

```diff
@@ -7,24 +7,24 @@
         <a href="{{ next.link|e }}" class="btn btn-neutral float-right" title="{{ next.title|striptags|e }}" accesskey="n" rel="next">{{ _('Next') }} <span class="fa fa-arrow-circle-right"></span></a>
       {% endif %}
       {% if prev %}
         <a href="{{ prev.link|e }}" class="btn btn-neutral float-left" title="{{ prev.title|striptags|e }}" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left"></span> {{ _('Previous') }}</a>
       {% endif %}
     </div>
 {% endif %}
-<div id="button" class="backtop"><img src="{{ theme_asset_url }}/img/right.svg" alt="backtop"/> </div>
+<div id="button" class="backtop"><img src="{{ pathto('_static/img/right.svg', 1) }}" alt="backtop"/> </div>
 <section class="footerSec">
     <div class="footerHeader">
-      <ul class="d-flex align-md-items-center justify-content-between flex-column flex-md-row">
-        <li class="copywrite d-flex align-items-center">
+      <div class="d-flex align-md-items-center justify-content-between flex-column flex-md-row">
+        <div class="copywrite d-flex align-items-center">
           <h5 id="copy-right-info">{{ footer_copyright }}</h5>
-        </li>
-      </ul>
+        </div>
+      </div>
 
     </div>
 
-    <ul>
-      <li class="footernote">{{ footer_note }}</li>
-    </ul>
+    <div>
+      <div class="footernote">{{ footer_note }}</div>
+    </div>
 
 </section>
 </footer>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% set theme_asset_url = theme_asset_url | default(pathto('_static/',1 )) %}
 {% if (theme_prev_next_buttons_location == 'bottom' or
 theme_prev_next_buttons_location == 'both') and (next or prev) %}
 {% if next %} {{__('Next')_}} {% endif %} {% if prev %} {{__('Previous')_}} {%
 endif %}
 {% endif %}
 [backtop]
-    * ** {{ footer_copyright }} **
-    * {{ footer_note }}
+** {{ footer_copyright }} **
+{{ footer_note }}
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/breadcrumbs.html` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/breadcrumbs.html`

 * *Files 5% similar despite different names*

```diff
@@ -40,23 +40,29 @@
     {% block breadcrumbs %}
       <li><a href="{{ pathto(master_doc) }}">Docs</a> <span class="br-arrow">></span></li>
         {% for doc in parents %}
           <li><a href="{{ doc.link|e }}">{{ doc.title }}</a> <span class="br-arrow">></span></li>
         {% endfor %}
       <li>{{ title }}</li>
     {% endblock %}
+    {% if suffix %}
+      {% set _edit_url = 'https://github.com/' + github_user + '/' + github_repo + '/' + theme_vcs_pageview_mode + '/' + github_version + pagename + suffix %}
+      {% if edit_link_hook_fn %}
+        {% set _edit_url = edit_link_hook_fn(_edit_url) %}
+      {% endif %}
+    {% endif %}
     {% block breadcrumbs_aside %}
       <li class="wy-breadcrumbs-aside">
         {% if hasdoc(pagename) %}
             {% if display_github %}
             {% if check_meta and 'github_url' in meta %}
               <!-- User defined GitHub URL -->
               <a href="{{ meta['github_url'] }}" class="fa fa-github"> {{ _('Edit on GitHub') }}</a>
             {% else %}
-              <a href="https://{{ github_host|default("github.com") }}/{{ github_user }}/{{ github_repo }}/{{ theme_vcs_pageview_mode|default("blob") }}/{{ github_version }}{{ conf_py_path }}{{ pagename }}{{ suffix }}" class="fa fa-github"> {{ _('Edit on GitHub') }}</a>
+              <a href="{{ _edit_url }}" class="fa fa-github"> {{ _('Edit on GitHub') }}</a>
             {% endif %}
           {% elif display_bitbucket %}
             {% if check_meta and 'bitbucket_url' in meta %}
               <!-- User defined Bitbucket URL -->
               <a href="{{ meta['bitbucket_url'] }}" class="fa fa-bitbucket"> {{ _('Edit on Bitbucket') }}</a>
             {% else %}
               <a href="https://bitbucket.org/{{ bitbucket_user }}/{{ bitbucket_repo }}/src/{{ bitbucket_version}}{{ conf_py_path }}{{ pagename }}{{ suffix }}?mode={{ theme_vcs_pageview_mode|default("view") }}" class="fa fa-bitbucket"> {{ _('Edit on Bitbucket') }}</a>
@@ -67,15 +73,15 @@
               <a href="{{ meta['gitlab_url'] }}" class="fa fa-gitlab"> {{ _('Edit on GitLab') }}</a>
             {% else %}
               <a href="https://{{ gitlab_host|default("gitlab.com") }}/{{ gitlab_user }}/{{ gitlab_repo }}/{{ theme_vcs_pageview_mode|default("blob") }}/{{ gitlab_version }}{{ conf_py_path }}{{ pagename }}{{ suffix }}" class="fa fa-gitlab"> {{ _('Edit on GitLab') }}</a>
             {% endif %}
           {% elif show_source and source_url_prefix %}
             <a href="{{ source_url_prefix }}{{ pagename }}{{ suffix }}">{{ _('View page source') }}</a>
           {% elif show_source and has_source and sourcename %}
-            <a href="{{ pathto('_sources/' + sourcename, true)|e }}" rel="nofollow"> <img src="{{ theme_asset_url }}/img/source.svg" alt="viewsource"/></a>
+            <a href="{{ pathto('_sources/' + sourcename, true)|e }}" rel="nofollow"> <img src="{{ pathto('_static/img/source.svg', 1) }}" alt="viewsource"/></a>
           {% endif %}
         {% endif %}
       </li>
     {% endblock %}
   </ul>
 
   {% if (theme_prev_next_buttons_location == 'top' or theme_prev_next_buttons_location == 'both') and (next or prev) %}
```

#### html2text {}

```diff
@@ -12,23 +12,24 @@
 theme_asset_url | default(pathto('_static/',1 )) %}
     * {% block breadcrumbs %}
     * Docs >
     * {% for doc in parents %}
     * {{_doc.title_}} >
     * {% endfor %}
     * {{ title }}
-    * {% endblock %} {% block breadcrumbs_aside %}
+    * {% endblock %} {% if suffix %} {% set _edit_url = 'https://github.com/' +
+      github_user + '/' + github_repo + '/' + theme_vcs_pageview_mode + '/' +
+      github_version + pagename + suffix %} {% if edit_link_hook_fn %} {% set
+      _edit_url = edit_link_hook_fn(_edit_url) %} {% endif %} {% endif %} {%
+      block breadcrumbs_aside %}
     * {% if hasdoc(pagename) %} {% if display_github %} {% if check_meta and
-      'github_url' in meta %}  {{__('Edit_on_GitHub')_}} {% else %} com") }}/{
-      { github_user }}/{{ github_repo }}/{{ theme_vcs_pageview_mode|default
-      ("blob") }}/{{ github_version }}{{ conf_py_path }}{{ pagename }}{{ suffix
-      }}" class="fa fa-github"> {{ _('Edit on GitHub') }}
- {% endif %} {% elif display_bitbucket %} {% if check_meta and 'bitbucket_url'
-in meta %}  {{__('Edit_on_Bitbucket')_}} {% else %}
-) }}" class="fa fa-bitbucket"> {{ _('Edit on Bitbucket') }}
+      'github_url' in meta %}  {{__('Edit_on_GitHub')_}} {% else %} {{__('Edit
+      on_GitHub')_}} {% endif %} {% elif display_bitbucket %} {% if check_meta
+      and 'bitbucket_url' in meta %}  {{__('Edit_on_Bitbucket')_}} {% else %} )
+      }}" class="fa fa-bitbucket"> {{ _('Edit on Bitbucket') }}
  {% endif %} {% elif display_gitlab %} {% if check_meta and 'gitlab_url' in
 meta %}  {{__('Edit_on_GitLab')_}} {% else %}
 com") }}/{{ gitlab_user }}/{{ gitlab_repo }}/{{ theme_vcs_pageview_mode|default
 ("blob") }}/{{ gitlab_version }}{{ conf_py_path }}{{ pagename }}{{ suffix }}"
 class="fa fa-gitlab"> {{ _('Edit on GitLab') }}
  {% endif %} {% elif show_source and source_url_prefix %} {{__('View_page
 source')_}} {% elif show_source and has_source and sourcename %} [viewsource]
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_templates/layout.html` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_templates/layout.html`

 * *Files 10% similar despite different names*

```diff
@@ -141,17 +141,31 @@
 
           {% if theme_display_version %}
             {%- set nav_version = version %}
             {% if READTHEDOCS and current_version %}
               {%- set nav_version = current_version %}
             {% endif %}
             {% if nav_version %}
-              {%- if version_selecter is defined %}
-                <div class="version">
-                  <a href="{{ version_selecter }}">{{ nav_version }} ▼ </a>
+              {%- if version_prefixes is defined %}
+              <input type="checkbox" class="version-toggle-box" hidden id="version-toggle">
+              <label for="version-toggle" class="version-toggle-label">
+                  <div tabindex="0" class="version version-selector version-selector-show">
+                    {{ nav_version }} <span class="chevron versions-hidden"><svg fill="none" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg"><path d="m8 4 8 8-8 8" stroke="#000" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/></svg></span><span class="chevron versions-shown"><svg fill="none" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg"><path d="m4 8 8 8 8-8" stroke="#000" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/></svg></span>
+                  </div>
+                </label>
+                <div class="version-details wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="main navigation">
+                  <p class="caption" role="heading"><span class="caption-text">Versions</span></p>
+                  <ol style="text-align: left">
+                    {% for version in version_prefixes %}
+                    {% set version_url = "/" if version == "main" else version %}
+                    {% set version_desc = nav_version + " (main)" if version == "main" else version.strip("/") %}
+                    
+                      <li><div class="version"><a style="font-size: 0.8em; padding: 4px" href="{{ version_url }}">{{ version_desc }}</a></div></li>
+                    {% endfor %}
+                  </ol>
                 </div>
               {%- else %}
                 <div class="version">
                   {{ nav_version }}
                 </div>
               {%- endif %}
             {% endif %}
@@ -192,15 +206,15 @@
       <nav class="wy-nav-top" aria-label="top navigation" data-toggle="wy-nav-top">
         {% block mobile_nav %}
             <div class="togglemenu">
 
             </div>
             <div class="nav-content">
               <!-- {{ project }} -->
-              Table of content
+              Table of Contents
             </div>
         {% endblock %}
       </nav>
 
 
       <div class="wy-nav-content">
       {%- block content %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -41,16 +41,22 @@
 % if theme_style_nav_header_background %} style="background: {
 {theme_style_nav_header_background}}" {% endif %}> {% block sidebartitle %} {%
 if logo and theme_logo_only %} {%_else_%}_)_}}">_{{_project_}}_{%_endif_%}_{%
 if_logo_%}_{#_Not_strictly_valid_HTML,_but_it's_the_only_way_to_display/scale
 it_properly,_without_weird_scripting_or_heaps_of_work_#}_[{{__('Logo')_}}]_{%
 endif_%} {% if theme_display_version %} {%- set nav_version = version %} {% if
 READTHEDOCS and current_version %} {%- set nav_version = current_version %} {%
-endif %} {% if nav_version %} {%- if version_selecter is defined %}
-{{_nav_version_}}_â¼
+endif %} {% if nav_version %} {%- if version_prefixes is defined %} ⁰
+{{ nav_version }}
+Versions
+   1. {% for version in version_prefixes %} {% set version_url = "/" if version
+      == "main" else version %} {% set version_desc = nav_version + " (main)"
+      if version == "main" else version.strip("/") %}
+   2. {{_version_desc_}}
+   3. {% endfor %}
 {%- else %}
 {{ nav_version }}
 {%- endif %} {% endif %} {% endif %} {% include "searchbox.html" %} {% endblock
 %}
 {% block navigation %}
 {% block menu %} {# The singlehtml builder doesn't handle this toctree call
 when the toctree is empty. Skip building this for now. #} {% if 'singlehtml'
@@ -59,15 +65,15 @@
 collapse=theme_collapse_navigation|tobool,
 includehidden=theme_includehidden|tobool, titles_only=theme_titles_only|tobool)
 %} {% endif %} {% if global_toc %} {{ global_toc }} {% else %}
 {{ toc }}
 {% endif %} {% endblock %}
 {% endblock %}
   {# MOBILE NAV, TRIGGLES SIDE NAV ON TOGGLE #}  {% block mobile_nav %}
- Table of content
+ Table of Contents
 {% endblock %}
 {%- block content %} {% if theme_style_external_links|tobool %}
 {% else %}
 {% endif %} {% include "breadcrumbs.html" %}
 {%- block document %}
 {% block body %}{% endblock %}
 {% if self.comments()|trim %}
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/js/tlcpack_theme.js` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/js/tlcpack_theme.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -35,8 +35,15 @@
         $(".header").addClass('navigation-hide');
         $(".wy-nav-top").addClass('navigation-hide');
     } else {
         btn.removeClass('show');
         $(".header").removeClass('navigation-hide');
         $(".wy-nav-top").removeClass('navigation-hide');
     }
-});
+});
+
+// Remove empty code blocks
+document.querySelectorAll("div.highlight > pre").forEach(p => {
+    if (p.innerText.trim() === "") {
+        p.parentNode.removeChild(p);
+    }
+})
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/pattern.svg` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/pattern.svg`

 * *Files identical despite different names*

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/img/close-icon.svg` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/img/close-icon.svg`

 * *Files identical despite different names*

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/css/tlcpack_theme.css` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/css/tlcpack_theme.css`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
   background: #ffffff;
 }
 body.scroll-hide {
   overflow: hidden;
 }
 
 p {
-  font-size: 14px;
   line-height: 25px;
   color: #3c3c3c;
   margin-bottom: 15px;
   font-family: "PT Sans", sans-serif;
   font-weight: 400;
 }
 p a {
@@ -113,15 +112,14 @@
 .dropdown-menu ul li:last-child {
   border-bottom: 0px;
   padding-bottom: 0px;
 }
 .dropdown-menu ul li a {
   color: #505d68;
   font-weight: 400;
-  font-size: 14px;
   line-height: 19px;
   font-family: "Ubuntu", sans-serif;
   display: block;
 }
 
 .highlight .c1 {
   color: #27AE60;
@@ -162,27 +160,28 @@
 @media (min-width: 1025px) {
   .rst-content .sphx-glr-thumbcontainer:hover {
     transform: scale(1.05);
     box-shadow: 0px 20px 32px rgba(3, 109, 162, 0.15);
     border: none;
   }
 }
-.rst-content .sphx-glr-thumbcontainer a.internal {
+.rst-content .sphx-glr-thumbcontainer div {
   bottom: 0;
   display: flex;
   align-items: flex-end;
   left: 0;
   padding: 0 25px 30px;
   position: absolute;
   text-decoration: none;
   right: 0;
   top: 0;
   font-size: 16px;
   color: #ffffff;
   font-style: normal;
+  pointer-events: none;
 }
 .rst-content .sphx-glr-thumbcontainer .figure {
   margin: 0;
   width: 235px;
 }
 .rst-content div.sphx-glr-download a {
   background-color:#0379B6;
@@ -232,15 +231,14 @@
 .rst-content .note .admonition-title {
   background: #0379b6 !important;
 }
 .rst-content .admonition-title, .rst-content .wy-alert-title {
   padding: 7px 20px 7px 38px;
   font-weight: 700;
   font-family: "PT Sans", sans-serif;
-  font-size: 14px;
   line-height: 25px;
   position: relative;
   margin: -20px -20px 20px;
 }
 .rst-content .admonition-title::before, .rst-content .wy-alert-title::before {
   content: "";
   height: 12px;
@@ -268,25 +266,23 @@
   font-weight: 400;
 }
 
 .rst-content .section ol, .rst-content ol.arabic, .wy-plain-list-decimal, article ol {
   margin-bottom: 15px;
 }
 .rst-content .section ol li, .rst-content ol.arabic li, .wy-plain-list-decimal li, article ol li {
-  font-size: 14px;
   line-height: 25px;
   color: #252d5a;
   font-family: "PT Sans", sans-serif;
   font-weight: 400;
   margin-left: 16px;
   list-style: decimal;
 }
 
 .rst-content .section ul, .rst-content .toctree-wrapper ul, .wy-plain-list-disc, article ul {
-  font-size: 14px;
   color: #252d5a;
   line-height: 25px;
   margin-bottom: 15px;
   list-style: none;
 }
 
 .rst-content ul.simple li {
@@ -348,15 +344,14 @@
 
 .docutils dt {
   display: inline-block;
   padding: 5px 15px;
   background: rgba(3, 121, 182, 0.1);
   border-left: 2px solid #0379b6;
   font-weight: 700;
-  font-size: 14px;
   font-family: "PT Sans", sans-serif;
   color: #0379b6;
 }
 
 footer .btn {
   min-width: 168px;
   font-size: 12px;
@@ -499,15 +494,14 @@
     padding: 0 10px;
   }
 }
 .header .headerInner .headerNav .nav .nav-item .nav-link {
   color: #ffffff;
   text-transform: uppercase;
   font-weight: 400;
-  font-size: 14px;
   line-height: 18px;
   letter-spacing: 1px;
   padding: 0 4px;
   position: relative;
 }
 @media only screen and (max-width : 991px) {
   .header .headerInner .headerNav .nav .nav-item .nav-link {
@@ -575,15 +569,14 @@
   margin: 0;
 }
 .header .headerInner .headerNav .responsivetlcdropdown ul li {
   list-style: none;
   margin-bottom: 10px;
 }
 .header .headerInner .headerNav .responsivetlcdropdown ul li a {
-  font-size: 14px;
   line-height: 21px;
   color: #505d68;
   display: block;
 }
 @media only screen and (max-width : 991px) {
   .header .headerInner .headerNav .responsivetlcdropdown {
     display: block;
@@ -596,15 +589,14 @@
 }
 .header .headerInner .tlcDropdown .dropdown {
   position: relative;
 }
 .header .headerInner .tlcDropdown .dropdown .btn-link {
   padding: 0 18px 0px 1px;
   background-color: transparent;
-  font-size: 14px;
   line-height: 15px;
   text-align: center;
   letter-spacing: 1.16667px;
   text-transform: uppercase;
   color: #ffffff;
   position: relative;
   border: 0;
@@ -643,15 +635,14 @@
   padding: 0;
   border: 0px;
   background-color: transparent;
 }
 
 .wy-breadcrumbs .br-arrow {
   font-family: "PT Sans", sans-serif;
-  font-size: 14px;
   margin-right: 2px;
   color: #0379b6;
 }
 
 .wy-nav-side {
   background: #F8F9FA;
 }
@@ -700,15 +691,14 @@
     margin-left: 0;
   }
 }
 .wy-nav-side .wy-side-nav-search input[type=text] {
   box-shadow: none;
   border: none;
   padding: 8px 12px;
-  font-size: 14px;
   line-height: 25px;
   border-radius: 0;
   font-family: "PT Sans", sans-serif;
   font-weight: 400;
   color: #252d5a;
 }
 .wy-nav-side .wy-side-nav-search a {
@@ -788,15 +778,14 @@
 .wy-nav-side .wy-menu-vertical li.toctree-l1.current a {
   border: none;
   background: transparent !important;
 }
 .wy-nav-side .wy-menu-vertical li.toctree-l2 a {
   padding: 0 0 0 18px;
   color: #252d5a;
-  font-size: 14px;
   font-family: "PT Sans", sans-serif;
   margin-bottom: 5px;
 }
 @media only screen and (max-width : 991px) {
   .wy-nav-side .wy-menu-vertical li.toctree-l2 a {
     padding: 5px 0 5px 18px;
   }
@@ -806,15 +795,14 @@
   color: #0379b6;
 }
 .wy-nav-side .wy-menu-vertical li.toctree-l2.current .toctree-l3.current > a {
   color: #0379b6;
 }
 .wy-nav-side .wy-menu-vertical li.toctree-l2.current .toctree-l3 a {
   padding: 0 0 0 38px;
-  font-size: 14px;
   font-family: "PT Sans", sans-serif;
   font-weight: 400;
   margin-bottom: 5px;
 }
 @media only screen and (max-width : 991px) {
   .wy-nav-side .wy-menu-vertical li.toctree-l2.current .toctree-l3 a {
     padding: 5px 0 5px 38px;
@@ -903,14 +891,15 @@
   }
   .wy-nav-top .nav-content {
     flex: 1 1 auto;
     color: #252d5a;
     font-family: "PT Sans Caption", sans-serif;
     font-size: 15px;
     font-weight: 700;
+    cursor: pointer;
   }
   .wy-nav-top .togglemenu {
     width: 30px;
     height: 30px;
     background: url(../img/rightangle.svg) no-repeat center;
     transition: 0.1s all;
   }
@@ -947,26 +936,24 @@
 .rst-footer-buttons {
   margin-bottom: 57px;
 }
 
 .footerSec {
   background: #001B29;
   font-family: "Ubuntu", sans-serif;
-  font-size: 14px;
   line-height: 21px;
   color: #ffffff;
   padding-bottom: 43px;
 }
 @media only screen and (max-width : 991px) {
   .footerSec {
     padding: 0 30px;
   }
 }
 .footerSec h5 {
-  font-size: 14px;
   margin-bottom: 0;
   font-weight: normal;
   font-family: "Ubuntu", sans-serif;
 }
 @media only screen and (max-width : 767px) {
   .footerSec h5 {
     margin-top: 10px;
@@ -1055,7 +1042,61 @@
     opacity: 1;
     visibility: visible;
   }
 }
 .rst-content .container{
   padding:0;
 }
+
+/* .version-selector-content {
+  display: none;
+}
+
+.version-selector-show .versions-shown {
+  display: none;
+}
+
+.version-selector-show:focus {
+  color: red;
+}
+
+.version-selector-hide, .version-selector-show {
+  cursor: pointer;
+}
+
+.version-selector-show:focus ~ .version-selector-content {
+  display: block;
+}
+.version-selector-show:focus .versions-hidden {
+  display: none;
+}
+.version-selector-show:focus .versions-shown {
+  display: block;
+} */
+
+.version-details {
+  display: none;
+  margin-bottom: 1.5em;
+}
+
+.versions-shown {
+  display: none;
+}
+
+.chevron svg {
+  line-height: 0.5em;
+  margin-top: -10px;
+  height: 1em;
+  transform: translateY(17%);
+}
+
+.version-toggle-box:checked ~ .version-details {
+  display: block;
+}
+
+.version-toggle-box:checked ~ .version-toggle-label .versions-hidden {
+  display: none;
+}
+
+.version-toggle-box:checked ~ .version-toggle-label .versions-shown {
+  display: inline-block;
+}
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon/_static/css/gallery.css` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon/_static/css/gallery.css`

 * *Files identical despite different names*

### Comparing `tlcpack-sphinx-addon-0.2.1/setup.py` & `tlcpack-sphinx-addon-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint: disable=invalid-name, exec-used
 """Setup TLCPack."""
 from setuptools import setup, find_packages
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 
 setup(
     name="tlcpack-sphinx-addon",
     version=__version__,
     license="Apache-2.0",
     description="TLCPack Sphinx addon",
```

### Comparing `tlcpack-sphinx-addon-0.2.1/PKG-INFO` & `tlcpack-sphinx-addon-0.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tlcpack-sphinx-addon
-Version: 0.2.1
+Version: 0.2.2
 Summary: TLCPack Sphinx addon
 Home-page: https://github.com/tlc-pack/tlcpack-sphinx-addon
 Author: tlcpack
 Author-email: tianqi.tchen@gmail.com
 License: Apache-2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/SOURCES.txt` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 tlcpack_sphinx_addon/__init__.py
 tlcpack_sphinx_addon.egg-info/PKG-INFO
 tlcpack_sphinx_addon.egg-info/SOURCES.txt
 tlcpack_sphinx_addon.egg-info/dependency_links.txt
```

### Comparing `tlcpack-sphinx-addon-0.2.1/tlcpack_sphinx_addon.egg-info/PKG-INFO` & `tlcpack-sphinx-addon-0.2.2/tlcpack_sphinx_addon.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tlcpack-sphinx-addon
-Version: 0.2.1
+Version: 0.2.2
 Summary: TLCPack Sphinx addon
 Home-page: https://github.com/tlc-pack/tlcpack-sphinx-addon
 Author: tlcpack
 Author-email: tianqi.tchen@gmail.com
 License: Apache-2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
```

