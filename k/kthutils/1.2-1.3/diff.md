# Comparing `tmp/kthutils-1.2.tar.gz` & `tmp/kthutils-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthutils-1.2.tar", max compression
+gzip compressed data, was "kthutils-1.3.tar", max compression
```

## Comparing `kthutils-1.2.tar` & `kthutils-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.2/LICENSE
--rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.2/README.md
--rw-r--r--   0        0        0      721 2023-05-22 13:22:56.490253 kthutils-1.2/pyproject.toml
--rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.2/src/kthutils/.gitignore
--rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.2/src/kthutils/Makefile
--rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.2/src/kthutils/__init__.py
--rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.2/src/kthutils/cli.nw
--rw-r--r--   0        0        0      281 2023-04-27 18:36:23.514363 kthutils-1.2/src/kthutils/cli.py
--rw-r--r--   0        0        0      770 2023-04-27 18:36:23.514363 kthutils-1.2/src/kthutils/credentials.py
--rw-r--r--   0        0        0    16807 2023-05-22 13:22:37.453672 kthutils-1.2/src/kthutils/ug.nw
--rw-r--r--   0        0        0     8414 2023-05-22 13:23:19.007254 kthutils-1.2/src/kthutils/ug.py
--rw-r--r--   0        0        0      745 2023-05-22 13:23:19.227229 kthutils-1.2/tests/test_ug.py
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.3/LICENSE
+-rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.3/README.md
+-rw-r--r--   0        0        0      721 2023-05-26 15:55:06.744988 kthutils-1.3/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.3/src/kthutils/.gitignore
+-rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.3/src/kthutils/Makefile
+-rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.3/src/kthutils/__init__.py
+-rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.3/src/kthutils/cli.nw
+-rw-r--r--   0        0        0      281 2023-05-26 15:56:15.589305 kthutils-1.3/src/kthutils/cli.py
+-rw-r--r--   0        0        0      770 2023-05-26 15:56:15.589305 kthutils-1.3/src/kthutils/credentials.py
+-rw-r--r--   0        0        0    17844 2023-05-26 15:54:52.740964 kthutils-1.3/src/kthutils/ug.nw
+-rw-r--r--   0        0        0     9315 2023-05-26 15:56:15.593305 kthutils-1.3/src/kthutils/ug.py
+-rw-r--r--   0        0        0      745 2023-05-26 15:56:06.429250 kthutils-1.3/tests/test_ug.py
+-rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.3/PKG-INFO
```

### Comparing `kthutils-1.2/LICENSE` & `kthutils-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kthutils-1.2/README.md` & `kthutils-1.3/README.md`

 * *Files identical despite different names*

### Comparing `kthutils-1.2/pyproject.toml` & `kthutils-1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kthutils"
-version = "1.2"
+version = "1.3"
 description = "Various tools for automation at KTH"
 authors = ["Daniel Bosk <dbosk@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/kthutils"
 include = ["*/**/*.py"]
```

### Comparing `kthutils-1.2/src/kthutils/cli.nw` & `kthutils-1.3/src/kthutils/cli.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.2/src/kthutils/credentials.py` & `kthutils-1.3/src/kthutils/credentials.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.2/src/kthutils/ug.nw` & `kthutils-1.3/src/kthutils/ug.nw`

 * *Files 18% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 
 \section{Listing editable groups}
 
 The first thing we want to do is to be able to list all groups.
 <<list doc>>=
 Lists all groups that are editable by the logged in user.
-Returns list of JSON objects.
+Returns list of JSON objects (from `list_editable_groups()`).
 @
 
 This will be reused a lot in the other methods, so we want to cache it.
 It makes sense to cache it as well, since the data can't change.
 (Well, we can't change it, and it doesn't change that often.)
 <<UG constructor>>=
 self.cache = {}
@@ -299,15 +299,15 @@
   <<create UGsession instance ug or exit>>
   user_data = ug.find_user_by_username(username)[0]
   del user_data["memberOf"]
   print(user_data)
 @
 
 
-\section{Members of a group}
+\section{Members of groups}
 
 We can do two things with the members of a group:
 \begin{enumerate}
 \item list them,
 \item change them (set, add or remove).
 \end{enumerate}
 We have separate methods for these in [[UGsession]].
@@ -330,41 +330,60 @@
 cli.add_typer(members)
 
 <<common variables for members>>
 @
 
 All of these commands will take similar arguments.
 We see two types: the group name and a list of users.
+For the group name we would like to have a regular expression that matches the 
+users name so that we can match several courses at the same time.
 <<common variables for members>>=
-group_name_arg = typer.Argument(..., help="Group's name",
+group_regex_arg = typer.Argument(..., help="Regex for the group's name",
                                 autocompletion=complete_group)
 user_list_arg = typer.Argument(..., help="List of usernames")
 @
 
+This means that we can get the list of matching group names by using the 
+[[find_group_by_name]].
+<<generate a list [[groups]] from [[group_regex]]>>=
+groups = ug.find_group_by_name(group_regex)
+@
+
 Now, all of the [[UGsession]] methods take the KTH ID as argument.
 But for the CLI, we want to use the more human readable name.
-We add a method for translating the [[group_name]] argument to [[group_kthid]].
+We add a method for translating the [[group_regex]] argument to [[group_kthid]].
 We simply go through all groups to find the matching name and its KTH ID.
 <<UG methods>>=
 def group_name_to_kthid(self, name):
   """
   Takes `name` (e.g. edu.courses.DD.DD1317.20222.1.courseresponsible) and
   returns KTH ID (e.g. u25w6fyq).
 
   Raises KeyError if no group named `name` is found.
   """
   for group in self.list_editable_groups():
     if group["name"] == name:
       return group["kthid"]
   
   raise KeyError(f"{name} could not be found.")
-<<translate group name to kthid>>=
+<<translate [[group_name]] to [[group_kthid]]>>=
 group_kthid = ug.group_name_to_kthid(group_name)
 @
 
+Now, since most of these methods require KTH ID, we would like to turn a list 
+of groups into a list of the corresponding KTH IDs.
+<<generate a list of [[group_kthids]] from [[group_regex]]>>=
+<<generate a list [[groups]] from [[group_regex]]>>
+group_kthids = []
+for group in groups:
+  group_name = group["name"]
+  <<translate [[group_name]] to [[group_kthid]]>>
+  group_kthids.append(group_kthid)
+@
+
 In the same way, all member methods takes KTH IDs for users as arguments.
 We want to translate usernames to KTH IDs.
 <<UG methods>>=
 def usernames_to_kthids(self, usernames):
   """
   Takes a list of usernames,
   returns a list of KTH IDs for the users.
@@ -411,21 +430,22 @@
 The human readable name is better to use here than the KTH ID used by 
 [[.list_group_members]].
 We need to add a translation.
 We use the function [[complete_group]] from above for the tab completion for 
 the name.
 <<add commands to cli>>=
 @members.command(name="ls")
-def cli_list_members(group_name: str = group_name_arg):
+def cli_list_members(group_regex: str = group_regex_arg):
   """
   <<members doc>>
   """
   <<create UGsession instance ug or exit>>
-  <<translate group name to kthid>>
-  <<clean and print members>>
+  <<generate a list of [[group_kthids]] from [[group_regex]]>>
+  for group_kthid in group_kthids:
+    <<clean and print members>>
 @
 
 When printing the members, we don't want to print each member's JSON 
 object.
 We want something more useful for the terminal.
 We print tab-separated fields of data, so that we can use grep(1), cut(1) and 
 join(1).
@@ -478,23 +498,24 @@
 
   return response.json()
 @
 
 Now let's add its CLI command function.
 <<add commands to cli>>=
 @members.command(name="set")
-def cli_set_members(group_name: str = group_name_arg,
+def cli_set_members(group_regex: str = group_regex_arg,
                     users: typing.List[str] = user_list_arg):
   """
   Sets the members of a group. Any existing members not in the list will be 
   removed.
   """
   <<create UGsession instance ug or exit>>
-  ug.set_group_members(ug.usernames_to_kthids(users),
-                       ug.group_name_to_kthid(group_name))
+  <<generate a list of [[group_kthids]] from [[group_regex]]>>
+  for group_kthid in group_kthids:
+    ug.set_group_members(ug.usernames_to_kthids(users), group_kthid)
 @
 
 \subsubsection{Adding users}
 
 It will probably be more useful to provide a method for adding a user or set of 
 users.
 <<UG methods>>=
@@ -510,23 +531,24 @@
             set(current_members + new_members),
             group_kthid)
 @
 
 Now let's add its CLI command function.
 <<add commands to cli>>=
 @members.command(name="add")
-def cli_add_members(group_name: str = group_name_arg,
+def cli_add_members(group_regex: str = group_regex_arg,
                     users: typing.List[str] = user_list_arg):
   """
   Adds the members of a group. Any existing members will remain. Any members 
   already a member, will remain a member.
   """
   <<create UGsession instance ug or exit>>
-  ug.add_group_members(ug.usernames_to_kthids(users),
-                       ug.group_name_to_kthid(group_name))
+  <<generate a list of [[group_kthids]] from [[group_regex]]>>
+  for group_kthid in group_kthids:
+    ug.add_group_members(ug.usernames_to_kthids(users), group_kthid)
 @
 
 \subsubsection{Removing users}
 
 In a similar fashion, we want to remove users too.
 <<UG methods>>=
 def remove_group_members(self, members, group_kthid):
@@ -541,22 +563,23 @@
             set(current_members) - set(members),
             group_kthid)
 @
 
 Now let's add its CLI command function.
 <<add commands to cli>>=
 @members.command(name="rm")
-def cli_remove_members(group_name: str = group_name_arg,
+def cli_remove_members(group_regex: str = group_regex_arg,
                        users: typing.List[str] = user_list_arg):
   """
   Remove the members of a group. Any existing members not named will remain.
   """
   <<create UGsession instance ug or exit>>
-  ug.remove_group_members(ug.usernames_to_kthids(users),
-                          ug.group_name_to_kthid(group_name))
+  <<generate a list of [[group_kthids]] from [[group_regex]]>>
+  for group_kthid in group_kthids:
+    ug.remove_group_members(ug.usernames_to_kthids(users), group_kthid)
 @
 
 \subsection{Tests}
 
 We can test this by adding and removing a user from a group.
 <<test functions>>=
 def test_add_group_members():
```

### Comparing `kthutils-1.2/src/kthutils/ug.py` & `kthutils-1.3/src/kthutils/ug.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     self.cache = {}
 
   @ct.cachedmethod(operator.attrgetter("cache"),
     key=ft.partial(ct.keys.hashkey, "list_editable_groups"))
   def list_editable_groups(self):
     """
     Lists all groups that are editable by the logged in user.
-    Returns list of JSON objects.
+    Returns list of JSON objects (from `list_editable_groups()`).
     """
     response = self.__session.get(
         f"{self.BASE_URL}/api/ug/groups?editableBySelf=true")
     return response.json()
   def find_group_by_name(self, name_regex):
     """
     Searches for a group from `list_editable_groups()` whose name matches the regex 
@@ -154,15 +154,15 @@
 
 cli = typer.Typer(name="ug", help="Interacts with the KTH UG Editor")
 
 @cli.command(name="ls")
 def cli_list_groups():
   """
   Lists all groups that are editable by the logged in user.
-  Returns list of JSON objects.
+  Returns list of JSON objects (from `list_editable_groups()`).
   """
   ug = UGsession(*kthutils.credentials.get_credentials())
   for group in ug.list_editable_groups():
     name, desc = get_name_desc(group)
     print(f"{name}\t{desc}")
 def complete_group(incomplete: str) -> [str]:
   """
@@ -196,60 +196,84 @@
   user_data = ug.find_user_by_username(username)[0]
   del user_data["memberOf"]
   print(user_data)
 members = typer.Typer(name="members",
                       help="Operations on the members of a group")
 cli.add_typer(members)
 
-group_name_arg = typer.Argument(..., help="Group's name",
+group_regex_arg = typer.Argument(..., help="Regex for the group's name",
                                 autocompletion=complete_group)
 user_list_arg = typer.Argument(..., help="List of usernames")
 @members.command(name="ls")
-def cli_list_members(group_name: str = group_name_arg):
+def cli_list_members(group_regex: str = group_regex_arg):
   """
   Returns a list of the members of a group.
   The list contains JSON objects.
   """
   ug = UGsession(*kthutils.credentials.get_credentials())
-  group_kthid = ug.group_name_to_kthid(group_name)
-  for member in ug.list_group_members(group_kthid):
-    try:
-      title = member['title']['en'][0]
-    except IndexError:
-      title = None
-    print(f"{member['username']}"
-          f"\t{member['kthid']}"
-          f"\t{member['givenName']}"
-          f"\t{member['surname']}"
-          f"\t{title}")
+  groups = ug.find_group_by_name(group_regex)
+  group_kthids = []
+  for group in groups:
+    group_name = group["name"]
+    group_kthid = ug.group_name_to_kthid(group_name)
+    group_kthids.append(group_kthid)
+  for group_kthid in group_kthids:
+    for member in ug.list_group_members(group_kthid):
+      try:
+        title = member['title']['en'][0]
+      except IndexError:
+        title = None
+      print(f"{member['username']}"
+            f"\t{member['kthid']}"
+            f"\t{member['givenName']}"
+            f"\t{member['surname']}"
+            f"\t{title}")
 @members.command(name="set")
-def cli_set_members(group_name: str = group_name_arg,
+def cli_set_members(group_regex: str = group_regex_arg,
                     users: typing.List[str] = user_list_arg):
   """
   Sets the members of a group. Any existing members not in the list will be 
   removed.
   """
   ug = UGsession(*kthutils.credentials.get_credentials())
-  ug.set_group_members(ug.usernames_to_kthids(users),
-                       ug.group_name_to_kthid(group_name))
+  groups = ug.find_group_by_name(group_regex)
+  group_kthids = []
+  for group in groups:
+    group_name = group["name"]
+    group_kthid = ug.group_name_to_kthid(group_name)
+    group_kthids.append(group_kthid)
+  for group_kthid in group_kthids:
+    ug.set_group_members(ug.usernames_to_kthids(users), group_kthid)
 @members.command(name="add")
-def cli_add_members(group_name: str = group_name_arg,
+def cli_add_members(group_regex: str = group_regex_arg,
                     users: typing.List[str] = user_list_arg):
   """
   Adds the members of a group. Any existing members will remain. Any members 
   already a member, will remain a member.
   """
   ug = UGsession(*kthutils.credentials.get_credentials())
-  ug.add_group_members(ug.usernames_to_kthids(users),
-                       ug.group_name_to_kthid(group_name))
+  groups = ug.find_group_by_name(group_regex)
+  group_kthids = []
+  for group in groups:
+    group_name = group["name"]
+    group_kthid = ug.group_name_to_kthid(group_name)
+    group_kthids.append(group_kthid)
+  for group_kthid in group_kthids:
+    ug.add_group_members(ug.usernames_to_kthids(users), group_kthid)
 @members.command(name="rm")
-def cli_remove_members(group_name: str = group_name_arg,
+def cli_remove_members(group_regex: str = group_regex_arg,
                        users: typing.List[str] = user_list_arg):
   """
   Remove the members of a group. Any existing members not named will remain.
   """
   ug = UGsession(*kthutils.credentials.get_credentials())
-  ug.remove_group_members(ug.usernames_to_kthids(users),
-                          ug.group_name_to_kthid(group_name))
+  groups = ug.find_group_by_name(group_regex)
+  group_kthids = []
+  for group in groups:
+    group_name = group["name"]
+    group_kthid = ug.group_name_to_kthid(group_name)
+    group_kthids.append(group_kthid)
+  for group_kthid in group_kthids:
+    ug.remove_group_members(ug.usernames_to_kthids(users), group_kthid)
 
 if __name__ == "__main__":
   cli()
```

### Comparing `kthutils-1.2/tests/test_ug.py` & `kthutils-1.3/tests/test_ug.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.2/PKG-INFO` & `kthutils-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthutils
-Version: 1.2
+Version: 1.3
 Summary: Various tools for automation at KTH
 Home-page: https://github.com/dbosk/kthutils
 License: MIT
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

