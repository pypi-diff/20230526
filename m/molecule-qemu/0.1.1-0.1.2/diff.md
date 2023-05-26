# Comparing `tmp/molecule-qemu-0.1.1.tar.gz` & `tmp/molecule-qemu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.1.1.tar", last modified: Thu May 25 06:56:32 2023, max compression
+gzip compressed data, was "molecule-qemu-0.1.2.tar", last modified: Thu May 25 06:57:33 2023, max compression
```

## Comparing `molecule-qemu-0.1.1.tar` & `molecule-qemu-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.385444 molecule-qemu-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.385444 molecule-qemu-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.385444 molecule-qemu-0.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.385444 molecule-qemu-0.1.1/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.385444 molecule-qemu-0.1.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-25 06:56:32.000000 molecule-qemu-0.1.1/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-25 06:56:32.000000 molecule-qemu-0.1.1/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:56:32.000000 molecule-qemu-0.1.1/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 06:56:32.000000 molecule-qemu-0.1.1/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 06:56:32.000000 molecule-qemu-0.1.1/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 06:56:32.000000 molecule-qemu-0.1.1/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 06:56:20.000000 molecule-qemu-0.1.1/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 06:56:32.389443 molecule-qemu-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.619681 molecule-qemu-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.611680 molecule-qemu-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.615680 molecule-qemu-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.615680 molecule-qemu-0.1.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 06:57:33.619681 molecule-qemu-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.615680 molecule-qemu-0.1.2/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.615680 molecule-qemu-0.1.2/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.611680 molecule-qemu-0.1.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.615680 molecule-qemu-0.1.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.615680 molecule-qemu-0.1.2/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.619681 molecule-qemu-0.1.2/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:33.615680 molecule-qemu-0.1.2/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 06:57:33.000000 molecule-qemu-0.1.2/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-25 06:57:33.000000 molecule-qemu-0.1.2/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:57:33.000000 molecule-qemu-0.1.2/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 06:57:33.000000 molecule-qemu-0.1.2/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 06:57:33.000000 molecule-qemu-0.1.2/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 06:57:33.000000 molecule-qemu-0.1.2/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 06:57:21.000000 molecule-qemu-0.1.2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 06:57:33.619681 molecule-qemu-0.1.2/setup.cfg
```

### Comparing `molecule-qemu-0.1.1/.github/workflows/python-publish.yml` & `molecule-qemu-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.1.1/.github/workflows/release.yml` & `molecule-qemu-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.1.1/.gitignore` & `molecule-qemu-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.1.1/LICENSE` & `molecule-qemu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.1.1/Makefile` & `molecule-qemu-0.1.2/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 		'pycodestyle==2.10.0'
 
 .PHONY: virtualenv
 virtualenv: $(ANSIBLE_VIRTUALENV) ## Create local environment
 
 .PHONY: lint
 lint: virtualenv ## Lint
-	$(ANSIBLE_VIRTUALENV)/bin/ansible-lint -v
+	$(ANSIBLE_VIRTUALENV)/bin/ansible-lint -v molecule_qemu
 	$(ANSIBLE_VIRTUALENV)/bin/pycodestyle molecule_qemu
 
 .PHONY: clean
 clean: ## Remove cache
 	rm -rf $(ANSIBLE_VIRTUALENV) build dist *.egg-info
```

### Comparing `molecule-qemu-0.1.1/molecule_qemu/driver.py` & `molecule-qemu-0.1.2/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.1.1/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.1.2/molecule_qemu/playbooks/create.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,23 @@
     molecule_ephemeral_directory: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}"
     molecule_scenario_name: "{{ lookup('env', 'MOLECULE_SCENARIO_NAME') }}"
     molecule_project_name: "{{ lookup('env', 'MOLECULE_PROJECT_DIRECTORY') | basename }}"
     qemu_vm_arch: "x86_64"
     qemu_vm_memory: "1024"
 
   tasks:
+    - name: Create run directory exists
+      ansible.builtin.file:
+        path: "{{ molecule_ephemeral_directory }}/run/"
+        state: directory
+        mode: "0755"
+
     - name: Generate OpenSSH key pair
       community.crypto.openssh_keypair:
-        path: "{{ molecule_ephemeral_directory }}/id_ed25519"
+        path: "{{ molecule_ephemeral_directory }}/run/id_ed25519"
         type: ed25519
       register: vm_ssh_keypair
 
     - name: Register VMs data
       ansible.builtin.set_fact:
         instance: {
           "instance": "molecule-{{ molecule_project_name }}-{{ molecule_scenario_name }}-{{ item.name }}",
@@ -38,28 +44,22 @@
         label: "{{ item.name }}"
       register: molecule_instances
 
     - name: Prepare VMs data
       ansible.builtin.set_fact:
         molecule_instances: "{{ molecule_instances.results | map(attribute='ansible_facts.instance') | list }}"
 
-    - debug: var=molecule_instances
-
-    - name: Ensure run directory exists
-      ansible.builtin.file:
-        path: "{{ molecule_ephemeral_directory }}/run/"
-        state: directory
-        mode: "0755"
-
     - name: Create VMs disks based on provided image
       ansible.builtin.command: >
         qemu-img create
         -f qcow2
         -o backing_file={{ item.vm_image }},backing_fmt={{ item.vm_image_format }}
         {{ item.vm_run_diskfile }}
+      args:
+        creates: "{{ item.vm_run_diskfile }}"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Create cloud-init folders
       ansible.builtin.file:
         path: "{{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}/"
@@ -91,14 +91,16 @@
       ansible.builtin.command: >
         mkisofs
         -output {{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}.iso
         -volid cidata
         -joliet
         -rock
         {{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}/
+      args:
+        creates: "{{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}.iso"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Launch VMs  # noqa: no-changed-when
       ansible.builtin.command: >
         qemu-system-{{ item.vm_arch }}
@@ -121,14 +123,28 @@
         port: "{{ item.vm_ssh_port }}"
         delay: 5
         timeout: 180
         search_regex: "OpenSSH"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
+      async: 300
+      poll: 0
+      register: qemu_launch
+
+    - name: Wait for launch jobs to finish
+      ansible.builtin.async_status:
+        jid: "{{ item.ansible_job_id }}"
+      loop: "{{ qemu_launch.results }}"
+      loop_control:
+        label: "{{ item.item.name }}"
+      register: qemu_launch_status
+      until: qemu_launch_status.finished
+      retries: 30
+      delay: 10
 
     - name: Prepare VMs config dict
       ansible.builtin.set_fact:
         instance_conf_dict: {
           "instance": "{{ item.instance }}",
           "name": "{{ item.name }}",
           "address": "{{ item.vm_ssh_host }}",
```

### Comparing `molecule-qemu-0.1.1/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.1.2/molecule_qemu/playbooks/destroy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,17 @@
         pid: "{{ lookup('file', item.pidfile) }}"
       loop: "{{ instance_conf }}"
       loop_control:
         label: "{{ item.name }}"
       register: qemu_processes
 
     - name: Destroy running VMs
-      ansible.builtin.shell: "kill {{ item.ansible_facts.pid }}"
+      ansible.builtin.command: >
+        kill {{ item.ansible_facts.pid }}
+      changed_when: false
       loop: "{{ qemu_processes.results }}"
       loop_control:
         label: "{{ item.item.name }}"
 
     - name: Delete PID files
       ansible.builtin.file:
         path: "{{ item.pidfile }}"
```

### Comparing `molecule-qemu-0.1.1/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.1.2/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.1.1/pyproject.toml` & `molecule-qemu-0.1.2/pyproject.toml`

 * *Files identical despite different names*

