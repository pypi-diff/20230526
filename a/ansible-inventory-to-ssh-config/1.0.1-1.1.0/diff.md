# Comparing `tmp/ansible-inventory-to-ssh-config-1.0.1.tar.gz` & `tmp/ansible-inventory-to-ssh-config-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-inventory-to-ssh-config-1.0.1.tar", last modified: Fri Nov 11 10:32:07 2022, max compression
+gzip compressed data, was "ansible-inventory-to-ssh-config-1.1.0.tar", last modified: Fri May 26 06:28:21 2023, max compression
```

## Comparing `ansible-inventory-to-ssh-config-1.0.1.tar` & `ansible-inventory-to-ssh-config-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2022-11-11 10:32:07.391952 ansible-inventory-to-ssh-config-1.0.1/
--rw-r--r--   0 walter    (1000) walter    (1000)     1062 2020-11-25 03:50:02.000000 ansible-inventory-to-ssh-config-1.0.1/LICENSE
--rw-r--r--   0 walter    (1000) walter    (1000)      289 2022-11-11 10:32:07.391952 ansible-inventory-to-ssh-config-1.0.1/PKG-INFO
--rw-r--r--   0 walter    (1000) walter    (1000)     2029 2022-11-11 10:31:12.000000 ansible-inventory-to-ssh-config-1.0.1/README.md
-drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2022-11-11 10:32:07.381952 ansible-inventory-to-ssh-config-1.0.1/ansible_inventory_to_ssh_config.egg-info/
--rw-r--r--   0 walter    (1000) walter    (1000)      289 2022-11-11 10:32:07.000000 ansible-inventory-to-ssh-config-1.0.1/ansible_inventory_to_ssh_config.egg-info/PKG-INFO
--rw-r--r--   0 walter    (1000) walter    (1000)      386 2022-11-11 10:32:07.000000 ansible-inventory-to-ssh-config-1.0.1/ansible_inventory_to_ssh_config.egg-info/SOURCES.txt
--rw-r--r--   0 walter    (1000) walter    (1000)        1 2022-11-11 10:32:07.000000 ansible-inventory-to-ssh-config-1.0.1/ansible_inventory_to_ssh_config.egg-info/dependency_links.txt
--rw-r--r--   0 walter    (1000) walter    (1000)       88 2022-11-11 10:32:07.000000 ansible-inventory-to-ssh-config-1.0.1/ansible_inventory_to_ssh_config.egg-info/entry_points.txt
--rw-r--r--   0 walter    (1000) walter    (1000)       31 2022-11-11 10:32:07.000000 ansible-inventory-to-ssh-config-1.0.1/ansible_inventory_to_ssh_config.egg-info/requires.txt
--rw-r--r--   0 walter    (1000) walter    (1000)        4 2022-11-11 10:32:07.000000 ansible-inventory-to-ssh-config-1.0.1/ansible_inventory_to_ssh_config.egg-info/top_level.txt
--rw-r--r--   0 walter    (1000) walter    (1000)       38 2022-11-11 10:32:07.391952 ansible-inventory-to-ssh-config-1.0.1/setup.cfg
--rw-r--r--   0 walter    (1000) walter    (1000)      613 2022-11-11 10:32:03.000000 ansible-inventory-to-ssh-config-1.0.1/setup.py
-drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2022-11-11 10:32:07.391952 ansible-inventory-to-ssh-config-1.0.1/src/
--rw-r--r--   0 walter    (1000) walter    (1000)        0 2021-01-06 08:54:25.000000 ansible-inventory-to-ssh-config-1.0.1/src/__init__.py
--rw-r--r--   0 walter    (1000) walter    (1000)     3284 2022-11-11 08:27:06.000000 ansible-inventory-to-ssh-config-1.0.1/src/main.py
+drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/
+-rw-r--r--   0 walter    (1000) walter    (1000)     1062 2020-11-25 03:50:02.000000 ansible-inventory-to-ssh-config-1.1.0/LICENSE
+-rw-r--r--   0 walter    (1000) walter    (1000)      289 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/PKG-INFO
+-rw-r--r--   0 walter    (1000) walter    (1000)     2185 2023-05-26 06:21:45.000000 ansible-inventory-to-ssh-config-1.1.0/README.md
+drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/
+-rw-r--r--   0 walter    (1000) walter    (1000)      289 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/PKG-INFO
+-rw-r--r--   0 walter    (1000) walter    (1000)      386 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/SOURCES.txt
+-rw-r--r--   0 walter    (1000) walter    (1000)        1 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/dependency_links.txt
+-rw-r--r--   0 walter    (1000) walter    (1000)       88 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/entry_points.txt
+-rw-r--r--   0 walter    (1000) walter    (1000)       31 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/requires.txt
+-rw-r--r--   0 walter    (1000) walter    (1000)        4 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/top_level.txt
+-rw-r--r--   0 walter    (1000) walter    (1000)       38 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/setup.cfg
+-rw-r--r--   0 walter    (1000) walter    (1000)      613 2023-05-26 06:18:52.000000 ansible-inventory-to-ssh-config-1.1.0/setup.py
+drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/src/
+-rw-r--r--   0 walter    (1000) walter    (1000)        0 2021-01-06 08:54:25.000000 ansible-inventory-to-ssh-config-1.1.0/src/__init__.py
+-rw-r--r--   0 walter    (1000) walter    (1000)     3652 2023-05-26 06:15:07.000000 ansible-inventory-to-ssh-config-1.1.0/src/main.py
```

### Comparing `ansible-inventory-to-ssh-config-1.0.1/LICENSE` & `ansible-inventory-to-ssh-config-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-inventory-to-ssh-config-1.0.1/README.md` & `ansible-inventory-to-ssh-config-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -67,16 +67,16 @@
 $ cat hosts
 
 [group_1]
 node1 ansible_ssh_host=192.168.0.5
 node2 ansible_ssh_host=192.168.0.6
 
 [group_2]
-node3 ansible_host=192.168.0.7
-node4 ansible_host=192.168.0.8
+node3 ansible_host=192.168.0.7 ansible_ssh_private_key_file=~/.ssh/id_rsa_for_ansible
+node4 ansible_host=192.168.0.8 ansible_port=10422 ansible_user=foo
 
 # Commnad
 $ aitsc hosts -o newconfig
 Inventory: hosts
 Target: newconfig
 
 # Output (SSH Config Format)
@@ -88,12 +88,15 @@
 
 Host node2
   HostName 192.168.0.6
 
 
 Host node3
   HostName 192.168.0.7
+  IdentityFile ~/.ssh/id_rsa_for_ansible
 
 
 Host node4
   HostName 192.168.0.8
+  Port 10422
+  User foo
 ```
```

### Comparing `ansible-inventory-to-ssh-config-1.0.1/setup.py` & `ansible-inventory-to-ssh-config-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="ansible-inventory-to-ssh-config",
-    version='1.0.1',
+    version='1.1.0',
     description="Generate ssh config file from Ansible inventory",
     author="Yioda",
     author_email='jyc180g@gmail.com',
     url="https://github.com/yioda/ansible-inventory-to-ssh-config",
     packages=find_packages(),
     entry_points={
         'console_scripts': [
```

### Comparing `ansible-inventory-to-ssh-config-1.0.1/src/main.py` & `ansible-inventory-to-ssh-config-1.1.0/src/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,49 +11,62 @@
 
 
 def get_args():
     parser = ArgumentParser(formatter_class=RawTextHelpFormatter)
     parser.add_argument('-v', '--version', action='version',
                         version=get_distribution('ansible-inventory-to-ssh-config').version)
     parser.add_argument("inventory_file", help="ansible inventory file")
-    parser.add_argument("-o", "--output", help="ssh config output path (default: ~/.ssh/config.ansible)", default="~/.ssh/config.ansible")
-    parser.add_argument("-d", "--dry-run", help="show new configurations without updating file", action="store_true")
-    parser.add_argument("-b", "--with-backup", help="update with backup", action="store_true", default=False)
-    parser.add_argument("-O", "--override", help="override whole config, this would remove those hosts undefined in playbook", action="store_true", default=False)
+    parser.add_argument("-o", "--output",
+                        help="ssh config output path (default: ~/.ssh/config.ansible)",
+                        default="~/.ssh/config.ansible")
+    parser.add_argument("-d", "--dry-run",
+                        help="show new configurations without updating file",
+                        action="store_true")
+    parser.add_argument("-b", "--with-backup",
+                        help="update with backup",
+                        action="store_true",
+                        default=False)
+    parser.add_argument("-O", "--override",
+                        help="override whole config, would remove undefiend hosts in playbook",
+                        action="store_true", default=False)
 
     return parser.parse_args()
 
 
 def update_ssh_config(ssh_config_file, inventories, variables, group='all'):
     for host in inventories.get_hosts(group):
         # Get ssh connection info from playbook inventory
         host_vars = variables.get_vars(host=host)
         hostname = host_vars.get("ansible_ssh_host", host_vars.get("ansible_host", '127.0.0.1'))
         port = host_vars.get("ansible_ssh_port", host_vars.get("ansible_port", 22))
         user = host_vars.get("ansible_ssh_user", host_vars.get("ansible_user", None))
+        identityfile = host_vars.get("ansible_ssh_private_key_file")
 
         # Update to ssh config
         ssh_vars = ssh_config_file.host(host.get_name())
         ssh_vars.update({'Hostname': hostname})
         if port != 22:
             ssh_vars.update({'Port': port})
         if user:
             ssh_vars.update({'User': user})
+        if identityfile:
+            ssh_vars.update({'IdentityFile': identityfile})
 
         try:
             ssh_config_file.set(host.get_name(), **ssh_vars)
         except ValueError:
             ssh_config_file.add(host.get_name(), **ssh_vars)
 
 
 def backup(target_file):
     copyfile(target_file, f'{target_file}.{datetime.now().strftime("%Y%m%d_%H%M%S")}')
 
 
-def ansible_inventory_to_ssh_config(inventory_file, output, dry_run=False, with_backup=False, override=False):
+def ansible_inventory_to_ssh_config(
+        inventory_file, output, dry_run=False, with_backup=False, override=False):
     print(f'Inventory: {inventory_file}')
     print(f'Target: {output}')
 
     loader = DataLoader()
     inventories = InventoryManager(loader=loader, sources=[inventory_file])
     variables = VariableManager(loader=loader, inventory=inventories)
```

