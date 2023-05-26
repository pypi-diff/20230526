# Comparing `tmp/molecule-qemu-0.2.0.tar.gz` & `tmp/molecule-qemu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.2.0.tar", last modified: Fri May 26 05:25:18 2023, max compression
+gzip compressed data, was "molecule-qemu-0.3.0.tar", last modified: Fri May 26 06:03:26 2023, max compression
```

## Comparing `molecule-qemu-0.2.0.tar` & `molecule-qemu-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.136531 molecule-qemu-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-26 05:25:18.136531 molecule-qemu-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.136531 molecule-qemu-0.2.0/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.136531 molecule-qemu-0.2.0/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:25:18.132531 molecule-qemu-0.2.0/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-26 05:25:18.000000 molecule-qemu-0.2.0/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-26 05:25:18.000000 molecule-qemu-0.2.0/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:25:18.000000 molecule-qemu-0.2.0/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 05:25:18.000000 molecule-qemu-0.2.0/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 05:25:18.000000 molecule-qemu-0.2.0/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 05:25:18.000000 molecule-qemu-0.2.0/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 05:25:04.000000 molecule-qemu-0.2.0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 05:25:18.136531 molecule-qemu-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/setup.cfg
```

### Comparing `molecule-qemu-0.2.0/.github/workflows/python-publish.yml` & `molecule-qemu-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/.github/workflows/release.yml` & `molecule-qemu-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/.gitignore` & `molecule-qemu-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/LICENSE` & `molecule-qemu-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/Makefile` & `molecule-qemu-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/PKG-INFO` & `molecule-qemu-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.2.0
+Version: 0.3.0
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,45 +14,57 @@
 
 ## Usage
 
 ```bash
 pip install molecule-qemu
 ```
 
-## Dependencies
+Install QEMU and CDRTools on macOS:
 
 ```bash
 brew install qemu cdrtools
 ```
 
+Supported platforms:
+* MacOS 13.x (aaarch64)
+
+Support guest OS:
+* Ubuntu 20.04 LTS (aarch64)
+* Ubuntu 20.04 LTS (x86_64)
+* Debian 11 (x86_64)
+
+Support of other platforms and guest OS is possible, but not tested.
+
+# Examples
+
 ## Example scenario
 ```bash
 molecule init scenario scenario_name -d molecule-qemu
 ```
 
 ## Example `molecule.yml`
 ```yaml
 ---
 dependency:
   name: galaxy
 driver:
   name: molecule-qemu
 platforms:
   - name: ubuntu-1
-    image: ~/Downloads/focal-server-cloudimg-arm64.img
+    image: file:///Users/andrey/Downloads/focal-server-cloudimg-arm64.img
     image_arch: aarch64
     ssh_port: 10022
     ssh_user: ubuntu
   - name: ubuntu-2
-    image: ~/Downloads/focal-server-cloudimg-amd64.img
+    image: file:///Users/andrey/Downloads/focal-server-cloudimg-amd64.img
     image_arch: x86_64  # default
     ssh_port: 10023
     ssh_user: ubuntu
   - name: debian-1
-    image: ~/Downloads/debian-11-generic-amd64.qcow2
+    image: file:///Users/andrey/Downloads/debian-11-generic-amd64.qcow2
     image_arch: x86_64  # default
     ssh_port: 10024
     ssh_user: debian
 
 provisioner:
   name: ansible
 verifier:
```

### Comparing `molecule-qemu-0.2.0/molecule_qemu/driver.py` & `molecule-qemu-0.3.0/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.3.0/molecule_qemu/playbooks/create.yml`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     molecule_ephemeral_directory: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}"
     molecule_scenario_name: "{{ lookup('env', 'MOLECULE_SCENARIO_NAME') }}"
     molecule_project_name: "{{ lookup('env', 'MOLECULE_PROJECT_DIRECTORY') | basename }}"
     qemu_cap_hvf: false
     qemu_vm_image_arch: "x86_64"
     qemu_vm_image_format: "qcow2"
     qemu_vm_memory: "1024"
-    qemu_vm_cpus: "1"
+    qemu_vm_cpus: "2"
 
   tasks:
     ### configuration #########################################################
     - name: Register VMs data
       ansible.builtin.set_fact:
         instance: {
           "instance": "molecule-{{ molecule_project_name }}-{{ molecule_scenario_name }}-{{ item.name }}",
@@ -94,14 +94,43 @@
     - name: Fetch ARM VMs bios
       ansible.builtin.get_url:
         url: "https://releases.linaro.org/components/kernel/uefi-linaro/latest/release/qemu64/QEMU_EFI.fd"
         dest: "{{ molecule_ephemeral_directory }}/run/QEMU_EFI.fd"
         mode: "0644"
       when: "'aarch64' in molecule_instances | map(attribute='image_arch') | list | unique"
 
+    ### images ###############################################################
+    - name: Create images directory
+      ansible.builtin.file:
+        path: "{{ molecule_ephemeral_directory }}/run/images/"
+        state: directory
+        mode: "0755"
+
+    - name: Fetch images
+      ansible.builtin.get_url:
+        url: "{{ item }}"
+        dest: "{{ molecule_ephemeral_directory }}/run/images/{{ item | basename }}"
+        mode: "0644"
+      loop: "{{ molecule_instances | map(attribute='image') | list | unique }}"
+      loop_control:
+        label: "{{ item | basename }}"
+      register: images
+
+    - name: Get images
+      ansible.builtin.set_fact:
+        images: "{{ images.results | map(attribute='item') | list | zip(images.results | map(attribute='dest') | list) }}"
+        images_cache: {}
+
+    - name: Set images cache
+      ansible.builtin.set_fact:
+        images_cache: "{{ images_cache | combine({item[0]: item[1]}) }}"
+      loop: "{{ images }}"
+      loop_control:
+        label: "{{ item[0] | basename }}"
+
     ### cloud-init ############################################################
     - name: Create cloud-init folders
       ansible.builtin.file:
         path: "{{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}/"
         state: directory
         mode: "0755"
       loop: "{{ molecule_instances }}"
@@ -141,15 +170,15 @@
         label: "{{ item.name }}"
 
     ### qemu ##################################################################
     - name: Create VMs disks
       ansible.builtin.command: >
         qemu-img create
         -f qcow2
-        -o backing_file={{ item.image }},backing_fmt={{ item.image_format }}
+        -o backing_file={{ images_cache[item.image] }},backing_fmt={{ item.image_format }}
         {{ item.path_disk }}
       args:
         creates: "{{ item.path_disk }}"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
```

### Comparing `molecule-qemu-0.2.0/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.3.0/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.3.0/molecule_qemu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.2.0
+Version: 0.3.0
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,45 +14,57 @@
 
 ## Usage
 
 ```bash
 pip install molecule-qemu
 ```
 
-## Dependencies
+Install QEMU and CDRTools on macOS:
 
 ```bash
 brew install qemu cdrtools
 ```
 
+Supported platforms:
+* MacOS 13.x (aaarch64)
+
+Support guest OS:
+* Ubuntu 20.04 LTS (aarch64)
+* Ubuntu 20.04 LTS (x86_64)
+* Debian 11 (x86_64)
+
+Support of other platforms and guest OS is possible, but not tested.
+
+# Examples
+
 ## Example scenario
 ```bash
 molecule init scenario scenario_name -d molecule-qemu
 ```
 
 ## Example `molecule.yml`
 ```yaml
 ---
 dependency:
   name: galaxy
 driver:
   name: molecule-qemu
 platforms:
   - name: ubuntu-1
-    image: ~/Downloads/focal-server-cloudimg-arm64.img
+    image: file:///Users/andrey/Downloads/focal-server-cloudimg-arm64.img
     image_arch: aarch64
     ssh_port: 10022
     ssh_user: ubuntu
   - name: ubuntu-2
-    image: ~/Downloads/focal-server-cloudimg-amd64.img
+    image: file:///Users/andrey/Downloads/focal-server-cloudimg-amd64.img
     image_arch: x86_64  # default
     ssh_port: 10023
     ssh_user: ubuntu
   - name: debian-1
-    image: ~/Downloads/debian-11-generic-amd64.qcow2
+    image: file:///Users/andrey/Downloads/debian-11-generic-amd64.qcow2
     image_arch: x86_64  # default
     ssh_port: 10024
     ssh_user: debian
 
 provisioner:
   name: ansible
 verifier:
```

### Comparing `molecule-qemu-0.2.0/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.3.0/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.2.0/pyproject.toml` & `molecule-qemu-0.3.0/pyproject.toml`

 * *Files identical despite different names*

