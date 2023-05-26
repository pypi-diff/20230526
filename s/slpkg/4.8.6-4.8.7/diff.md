# Comparing `tmp/slpkg-4.8.6.tar.gz` & `tmp/slpkg-4.8.7.tar.gz`

## Comparing `slpkg-4.8.6.tar` & `slpkg-4.8.7.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:52:49.000000 slpkg-4.8.6/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-23 19:48:28.000000 slpkg-4.8.6/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      464 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4262 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-23 19:48:28.000000 slpkg-4.8.6/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-05-23 19:48:28.000000 slpkg-4.8.6/.pyproject.toml
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-23 19:48:28.000000 slpkg-4.8.6/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8822 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/slpkg.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/rules.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-23 19:48:28.000000 slpkg-4.8.6/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-23 19:48:28.000000 slpkg-4.8.6/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    46721 2023-05-23 19:48:28.000000 slpkg-4.8.6/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-05-23 19:48:28.000000 slpkg-4.8.6/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-23 19:48:28.000000 slpkg-4.8.6/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-23 19:48:28.000000 slpkg-4.8.6/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-23 19:48:28.000000 slpkg-4.8.6/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7441 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    65376 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11472 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/sbo_generate.py
--rw-r--r--   0 dslackw   (1000) users      (100)    34125 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3174 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/models/models.py
--rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/rules.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     6574 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5928 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/asciibox.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/logging_deps.py
--rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/new_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/multi_process.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/cleanings.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2195 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6100 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6782 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3427 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    33217 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3245 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-05-23 19:48:28.000000 slpkg-4.8.6/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/entry_points.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1301 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8603 2023-05-23 19:48:28.000000 slpkg-4.8.6/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-23 19:48:28.000000 slpkg-4.8.6/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:24:47.000000 slpkg-4.8.7/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-26 09:20:22.000000 slpkg-4.8.7/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      464 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4262 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-26 09:20:22.000000 slpkg-4.8.7/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-05-26 09:20:22.000000 slpkg-4.8.7/.pyproject.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-26 09:20:22.000000 slpkg-4.8.7/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8802 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/slpkg.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/rules.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-26 09:20:22.000000 slpkg-4.8.7/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-26 09:20:22.000000 slpkg-4.8.7/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    46862 2023-05-26 09:20:22.000000 slpkg-4.8.7/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-05-26 09:20:22.000000 slpkg-4.8.7/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-26 09:20:22.000000 slpkg-4.8.7/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-26 09:20:22.000000 slpkg-4.8.7/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-26 09:20:22.000000 slpkg-4.8.7/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7565 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    65376 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11615 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    36482 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3163 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/models/models.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/rules.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6604 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5935 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/asciibox.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/multi_process.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1906 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6100 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3481 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    33380 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3428 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-05-26 09:20:22.000000 slpkg-4.8.7/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1301 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8595 2023-05-26 09:20:22.000000 slpkg-4.8.7/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-26 09:20:22.000000 slpkg-4.8.7/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.6/filelists/multilib/README.ERIC` & `slpkg-4.8.7/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/filelists/multilib/README` & `slpkg-4.8.7/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/filelists/multilib/compat32.pkgs` & `slpkg-4.8.7/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/repositories.txt` & `slpkg-4.8.7/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slackbuild/slack-desc` & `slpkg-4.8.7/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.7/slackbuild/slpkg.SlackBuild`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/.pyproject.toml` & `slpkg-4.8.7/.pyproject.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/configs/repositories.toml` & `slpkg-4.8.7/configs/repositories.toml`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 SLACK_PATCHES_REPO = false
 SLACK_PATCHES_REPO_NAME = "slack_patches"
 SLACK_PATCHES_REPO_LOCAL = [""]
 SLACK_PATCHES_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "patches/"]
 SLACK_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
-SLACK_PATCHES_REPO_TAG = "_slack15.0"
+SLACK_PATCHES_REPO_TAG = ""
 
 # AlienBob Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["http://slackware.uk/people/alien/sbrepos/", "current/", "x86_64/"]
 ALIEN_REPO = false
 ALIEN_REPO_NAME = "alien"
 ALIEN_REPO_LOCAL = [""]
@@ -205,15 +205,15 @@
 SALIXOS_PATCHES_REPO = false
 SALIXOS_PATCHES_REPO_NAME = "salixos_patches"
 SALIXOS_PATCHES_REPO_LOCAL = [""]
 SALIXOS_PATCHES_REPO_MIRROR = ["https://download.salixos.org/x86_64/slackware-15.0/", "patches/"]
 SALIXOS_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SALIXOS_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SALIXOS_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
-SALIXOS_PATCHES_REPO_TAG = "_slack15.0"
+SALIXOS_PATCHES_REPO_TAG = ""
 
 # Repository for Slackel OS x86_64 -current.
 SLACKEL_REPO = false
 SLACKEL_REPO_NAME = "slackel"
 SLACKEL_REPO_LOCAL = [""]
 SLACKEL_REPO_MIRROR = ["http://www.slackel.gr/repo/x86_64/current/"]
 SLACKEL_REPO_PACKAGES = "PACKAGES.TXT"
```

### Comparing `slpkg-4.8.6/configs/slpkg.toml` & `slpkg-4.8.7/configs/slpkg.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/test_configs.py` & `slpkg-4.8.7/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/test_checks.py` & `slpkg-4.8.7/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/test_utilities.py` & `slpkg-4.8.7/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/test_sbo_queries.py` & `slpkg-4.8.7/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/test_colors.py` & `slpkg-4.8.7/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/check_updates_test.py` & `slpkg-4.8.7/tests/check_updates_test.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/test_upgrade.py` & `slpkg-4.8.7/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/tests/test_bin_queries.py` & `slpkg-4.8.7/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/LICENSE` & `slpkg-4.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/install.sh` & `slpkg-4.8.7/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/ChangeLog.txt` & `slpkg-4.8.7/ChangeLog.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+4.8.7 - 23/05/2023
+Fixed:
+- Package tag for slack_patches and salixos_patches
+- Parallel download for slackbuilds repositories (sbo, ponce)
+
 4.8.6 - 21/05/2023
 Updated:
 - Load the database when used #172
 Fixed:
 - ValueError with search command
 - Updates some packages to the same version #169
 - For --skip-installed option
```

### Comparing `slpkg-4.8.6/man/slpkg.1` & `slpkg-4.8.7/man/slpkg.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/man/slpkg-fr.1` & `slpkg-4.8.7/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/completion/slpkg` & `slpkg-4.8.7/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/dialog_configs.py` & `slpkg-4.8.7/slpkg/dialog_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/binaries/required.py` & `slpkg-4.8.7/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/binaries/queries.py` & `slpkg-4.8.7/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/binaries/install.py` & `slpkg-4.8.7/slpkg/binaries/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from slpkg.configs import Configs
 from slpkg.checksum import Md5sum
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
+from slpkg.views.asciibox import AsciiBox
 from slpkg.views.views import ViewMessage
 from slpkg.logging_deps import LoggingDeps
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
 from slpkg.binaries.required import Required
 
 
@@ -32,14 +33,16 @@
         self.repos = Repositories()
         self.dialogbox = DialogBox()
         self.multi_proc = MultiProcess(flags)
         self.logs_deps = LoggingDeps(repository, data)
         self.upgrade = Upgrade(repository, data)
         self.view_message = ViewMessage(flags, repository, data)
         self.check_md5 = Md5sum(flags)
+        self.download = Downloader(flags)
+        self.ascii = AsciiBox()
 
         self.dependencies: list = []
         self.install_order: list = []
         self.binary_packages: list = []
         self.slackware_command: str = self.installpkg
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
 
@@ -74,19 +77,21 @@
         self.install_packages()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
         if not self.option_for_resolve_off:
+            print('\rResolving dependencies... ', end='')
             for package in self.packages:
                 dependencies: tuple = Required(self.data, package).resolve()
 
                 for dependency in dependencies:
                     self.dependencies.append(dependency)
+            print(f'{self.yellow}{self.ascii.done}{self.endc}')
 
     def remove_duplicate_from_dependencies_list(self) -> None:
         if self.dependencies:
             self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
         self.install_order.extend(self.dependencies)
@@ -96,38 +101,36 @@
             if dependency in self.packages:
                 self.packages.remove(dependency)
 
     def add_main_packages_to_install_order(self) -> None:
         self.install_order.extend(self.packages)
 
     def crating_the_package_urls_list(self) -> None:
-        package_urls: list = []
+        packages: dict = {}
 
         for pkg in self.install_order:
             if self.continue_to_install(pkg):
                 package: str = self.data[pkg]['package']
                 mirror: str = self.data[pkg]['mirror']
                 location: str = self.data[pkg]['location']
 
-                package_urls.append(f'{mirror}{location}/{package}')
+                packages[f'{mirror}{location}/{package}'] = self.tmp_slpkg
 
                 self.binary_packages.append(package)
                 self.utils.remove_file_if_exists(self.tmp_slpkg, package)
             else:
                 installed_package: str = self.utils.is_package_installed(pkg)
                 self.view_message.view_skipping_packages(installed_package)
 
-        self.download_the_binary_packages(package_urls)
+        self.download_the_binary_packages(packages)
 
-    def download_the_binary_packages(self, package_urls: list) -> None:
-        if package_urls:
-            print(f'Started to download total ({self.cyan}{len(package_urls)}{self.endc}) packages:\n')
-        if package_urls:
-            down = Downloader(self.tmp_slpkg, package_urls, self.flags)
-            down.download()
+    def download_the_binary_packages(self, packages: dict) -> None:
+        if packages:
+            print(f'Started to download total ({self.cyan}{len(packages)}{self.endc}) packages:\n')
+            self.download.download(packages)
             print()
 
     def continue_to_install(self, name: str) -> bool:
         """ Skip installed package when the option --skip-installed is applied
             and continue to install if the package is upgradable or the --reinstall option
             applied.
          """
@@ -161,15 +164,15 @@
             self.progress_message: str = f'{self.cyan}Upgrading{self.endc}'
 
     def set_slackware_command(self) -> None:
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.slackware_command: str = self.reinstall
 
     def choose_package_dependencies(self) -> None:
-        if self.dependencies:
+        if self.dependencies and self.dialog:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = ' Choose dependencies you want to install '
 
             for package in self.dependencies:
@@ -183,11 +186,10 @@
 
                 if self.option_for_reinstall:
                     status: bool = True
 
                 choices.extend([(package, repo_ver, status, help_text)])
 
             text: str = f'There are {len(choices)} dependencies:'
-            code, self.dependencies = self.dialogbox.checklist(
-                text, self.dependencies, title, height, width, list_height, choices)
+            code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
 
             os.system('clear')
```

### Comparing `slpkg-4.8.6/slpkg/install_data.py` & `slpkg-4.8.7/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/repositories.py` & `slpkg-4.8.7/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/repo_info.py` & `slpkg-4.8.7/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/sbos/queries.py` & `slpkg-4.8.7/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/sbos/slackbuild.py` & `slpkg-4.8.7/slpkg/sbos/slackbuild.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from slpkg.checksum import Md5sum
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
 from slpkg.error_messages import Errors
+from slpkg.views.asciibox import AsciiBox
 from slpkg.views.views import ViewMessage
 from slpkg.logging_deps import LoggingDeps
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
 from slpkg.sbos.dependencies import Requires
 from slpkg.logging_config import LoggingConfig
 
@@ -40,15 +41,17 @@
         self.repos = Repositories()
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.multi_proc = MultiProcess(flags)
         self.logs_deps = LoggingDeps(repository, data)
         self.upgrade = Upgrade(repository, data)
         self.view_message = ViewMessage(flags, repository, data)
-        self.check_md5 = Md5sum(self.flags)
+        self.check_md5 = Md5sum(flags)
+        self.download = Downloader(flags)
+        self.ascii = AsciiBox()
 
         self.sources: dict = {}
         self.install_order: list = []
         self.dependencies: list = []
         self.slackware_command: str = str()
         self.slackware_command: str = self.installpkg
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
@@ -94,19 +97,21 @@
         self.build_and_install_the_slackbuilds()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
         if not self.option_for_resolve_off:
+            print('\rResolving dependencies... ', end='')
             for slackbuild in self.slackbuilds:
                 dependencies: tuple = Requires(self.data, slackbuild).resolve()
 
                 for dependency in dependencies:
                     self.dependencies.append(dependency)
+            print(f'{self.yellow}{self.ascii.done}{self.endc}')
 
     def remove_duplicate_from_dependencies_list(self) -> None:
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
         self.install_order.extend(self.dependencies)
 
@@ -154,25 +159,24 @@
                 # Copy slackbuilds to the build folder.
                 path_repo_package: Path = Path(self.repos.repositories[self.repository]['path'], location, sbo)
                 shutil.copytree(path_repo_package, build_path)
 
                 os.chmod(slackbuild, 0o775)
 
                 if self.os_arch == 'x86_64' and self.data[sbo]['download64']:
-                    self.sources[sbo] = self.data[sbo]['download64'].split()
+                    sources: list = self.data[sbo]['download64'].split()
                 else:
-                    self.sources[sbo] = self.data[sbo]['download'].split()
+                    sources: list = self.data[sbo]['download'].split()
+                for source in sources:
+                    self.sources[source] = Path(self.build_path, sbo)
 
     def download_the_sources(self) -> None:
         if self.sources:
             print(f'Started to download total ({self.cyan}{len(self.sources)}{self.endc}) sources:\n')
-        if self.sources:
-            for package, sbo_sources in self.sources.items():
-                down_urls = Downloader(Path(self.build_path, package), sbo_sources, self.flags)
-                down_urls.download()
+            self.download.download(self.sources)
             print()
 
             self.checksum_downloaded_sources()
 
     def checksum_downloaded_sources(self) -> None:
         for sbo in self.install_order:
             path: Path = Path(self.build_path, sbo)
@@ -250,15 +254,15 @@
             self.slackware_command: str = self.reinstall
 
     def set_makeflags(self) -> None:
         if self.option_for_jobs:
             os.environ['MAKEFLAGS'] = f'-j {cpu_count()}'
 
     def choose_package_dependencies(self) -> None:
-        if self.dependencies:
+        if self.dependencies and self.dialog:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = ' Choose dependencies you want to install '
 
             for package in self.dependencies:
@@ -275,11 +279,10 @@
                     status: bool = True
 
                 choices.extend(
                     [(package, repo_ver, status, help_text)]
                 )
             text: str = f'There are {len(choices)} dependencies:'
 
-            code, self.dependencies = self.dialogbox.checklist(
-                text, self.dependencies, title, height, width, list_height, choices)
+            code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
 
             os.system('clear')
```

### Comparing `slpkg-4.8.6/slpkg/sbos/dependencies.py` & `slpkg-4.8.7/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/sbos/sbo_generate.py` & `slpkg-4.8.7/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/update_repository.py` & `slpkg-4.8.7/slpkg/update_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         self.view = ViewMessage(flags)
         self.repos = Repositories()
         self.progress = ProgressBar()
         self.utils = Utilities()
         self.data = InstallData()
         self.generate = SBoGenerate()
         self.check_updates = CheckUpdates(flags, repository)
+        self.download = Downloader(flags)
 
         self.repos_for_update: dict = {}
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_repository: bool = self.utils.is_option(
             ('-o', '--repository='), flags)
@@ -90,472 +91,525 @@
 
     def view_downloading_message(self, repo: str) -> None:
         print(f"Downloading the '{self.green}{repo}{self.endc}' repository "
               f"in the '{self.repos.repositories[repo]['path']}' folder, please wait...\n")
 
     def slack_repository(self):
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.slack_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
 
             if self.repos.slack_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {self.repos.slack_repo_mirror[0]} '
                     f'{self.repos.slack_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}')
-                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}')
-                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}')
+                changelog: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}'
+                packages: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}'
+                checksums: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}'
+
+                urls[changelog] = self.repos.slack_repo_path
+                urls[packages] = self.repos.slack_repo_path
+                urls[checksums] = self.repos.slack_repo_path
 
-                down = Downloader(self.repos.slack_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slack_repo_name)
         self.delete_last_updated(self.repos.slack_repo_name)
         self.data.install_slack_data()
 
     def slack_extra_repository(self):
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.slack_extra_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_checksums)
 
-            urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}')
+            changelog: str = f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}'
+            urls[changelog] = self.repos.slack_extra_repo_path
 
             if self.repos.slack_extra_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_extra_repo_mirror)} '
                     f'{self.repos.slack_extra_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}')
-                urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_checksums}')
+                packages: str = f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}'
+                checksums: str = f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_checksums}'
 
-            down = Downloader(self.repos.slack_extra_repo_path, urls, self.flags)
-            down.download()
+                urls[packages] = self.repos.slack_extra_repo_path
+                urls[checksums] = self.repos.slack_extra_repo_path
+
+            self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.slack_extra_repo_name)
         self.delete_last_updated(self.repos.slack_extra_repo_name)
         self.data.install_slack_extra_data()
 
     def slack_patches_repository(self):
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.slack_patches_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_checksums)
 
-            urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}')
+            changelog: str = f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}'
+            urls[changelog] = self.repos.slack_patches_repo_path
 
             if self.repos.slack_patches_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_patches_repo_mirror)} '
                     f'{self.repos.slack_patches_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_packages}')
-                urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_checksums}')
+                packages: str = (f'{"".join(self.repos.slack_patches_repo_mirror)}'
+                                 f'{self.repos.slack_patches_repo_packages}')
+                checksums: str = (f'{"".join(self.repos.slack_patches_repo_mirror)}'
+                                  f'{self.repos.slack_patches_repo_checksums}')
+
+                urls[packages] = self.repos.slack_patches_repo_path
+                urls[checksums] = self.repos.slack_patches_repo_path
 
-            down = Downloader(self.repos.slack_patches_repo_path, urls, self.flags)
-            down.download()
+            self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.slack_patches_repo_name)
         self.delete_last_updated(self.repos.slack_patches_repo_name)
         self.data.install_slack_patches_data()
 
     def alien_repository(self):
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.alien_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
 
-            urls.append(f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}')
+            changelog: str = f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}'
+            urls[changelog] = self.repos.alien_repo_path
 
             if self.repos.alien_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.alien_repo_mirror)} '
                     f'{self.repos.alien_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}')
-                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}')
+                packages: str = f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}'
+                checksums: str = f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}'
+
+                urls[packages] = self.repos.alien_repo_path
+                urls[checksums] = self.repos.alien_repo_path
 
-            down = Downloader(self.repos.alien_repo_path, urls, self.flags)
-            down.download()
+            self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.alien_repo_name)
         self.delete_last_updated(self.repos.alien_repo_name)
         self.data.install_alien_data()
 
     def multilib_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.multilib_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
 
-            urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}')
+            changelog: str = f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}'
+            urls[changelog] = self.repos.multilib_repo_path
 
             if self.repos.multilib_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.multilib_repo_mirror)} '
                     f'{self.repos.multilib_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}')
-                urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_checksums}')
+                packages: str = f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}'
+                checksums: str = f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_checksums}'
 
-            down = Downloader(self.repos.multilib_repo_path, urls, self.flags)
-            down.download()
+                urls[packages] = self.repos.multilib_repo_path
+                urls[checksums] = self.repos.multilib_repo_path
+
+            self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.multilib_repo_name)
         self.delete_last_updated(self.repos.multilib_repo_name)
         self.data.install_multilib_data()
 
     def restricted_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.restricted_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
 
-            urls.append(f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}')
+            changelog: str = f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}'
+            urls[changelog] = self.repos.restricted_repo_path
 
             if self.repos.restricted_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.restricted_repo_mirror)} '
                     f'{self.repos.restricted_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}')
-                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}')
+                packages: str = f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}'
+                checksums: str = f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}'
+
+                urls[packages] = self.repos.restricted_repo_path
+                urls[checksums] = self.repos.restricted_repo_path
 
-            down = Downloader(self.repos.restricted_repo_path, urls, self.flags)
-            down.download()
+            self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.restricted_repo_name)
         self.delete_last_updated(self.repos.restricted_repo_name)
         self.data.install_restricted_data()
 
     def gnome_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.gnome_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
             self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
 
             if self.repos.gnome_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {self.repos.gnome_repo_mirror[0]} '
                     f'{self.repos.gnome_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}')
-                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}')
-                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}')
+                changelog: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}'
+                packages: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}'
+                checksums: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}'
+
+                urls[changelog] = self.repos.gnome_repo_path
+                urls[packages] = self.repos.gnome_repo_path
+                urls[checksums] = self.repos.gnome_repo_path
 
-                down = Downloader(self.repos.gnome_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.gnome_repo_name)
         self.delete_last_updated(self.repos.gnome_repo_name)
         self.data.install_gnome_data()
 
     def msb_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.msb_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_packages)
             self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_checksums)
 
-            urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}')
+            changelog: str = f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}'
+            urls[changelog] = self.repos.msb_repo_path
 
             if self.repos.msb_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.msb_repo_mirror)} '
                     f'{self.repos.msb_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}')
-                urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_checksums}')
+                packages: str = f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}'
+                checksums: str = f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_checksums}'
 
-            down = Downloader(self.repos.msb_repo_path, urls, self.flags)
-            down.download()
+                urls[packages] = self.repos.msb_repo_path
+                urls[checksums] = self.repos.msb_repo_path
+
+            self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.msb_repo_name)
         self.delete_last_updated(self.repos.msb_repo_name)
         self.data.install_msb_data()
 
     def csb_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.csb_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_packages)
             self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_checksums)
 
             if self.repos.csb_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.csb_repo_mirror)} '
                     f'{self.repos.csb_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_changelog}')
-                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}')
-                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_checksums}')
+                changelog: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_changelog}'
+                packages: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}'
+                checksums: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_checksums}'
+
+                urls[changelog] = self.repos.csb_repo_path
+                urls[packages] = self.repos.csb_repo_path
+                urls[checksums] = self.repos.csb_repo_path
 
-                down = Downloader(self.repos.csb_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.csb_repo_name)
         self.delete_last_updated(self.repos.csb_repo_name)
         self.data.install_csb_data()
 
     def conraid_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.conraid_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
             self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
 
             if self.repos.conraid_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {self.repos.conraid_repo_mirror[0]} '
                     f'{self.repos.conraid_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}')
-                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}')
-                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}')
+                changelog: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}'
+                packages: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}'
+                checksums: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}'
+
+                urls[changelog] = self.repos.conraid_repo_path
+                urls[packages] = self.repos.conraid_repo_path
+                urls[checksums] = self.repos.conraid_repo_path
 
-                down = Downloader(self.repos.conraid_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.conraid_repo_name)
         self.delete_last_updated(self.repos.conraid_repo_name)
         self.data.install_conraid_data()
 
     def slackonly_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.slackonly_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
 
             if self.repos.slackonly_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {self.repos.slackonly_repo_mirror[0]} '
                     f'{self.repos.slackonly_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}')
-                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}')
-                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}')
+                changelog: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}'
+                packages: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}'
+                checksums: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}'
+
+                urls[changelog] = self.repos.slackonly_repo_path
+                urls[packages] = self.repos.slackonly_repo_path
+                urls[checksums] = self.repos.slackonly_repo_path
 
-                down = Downloader(self.repos.slackonly_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slackonly_repo_name)
         self.delete_last_updated(self.repos.slackonly_repo_name)
         self.data.install_slackonly_data()
 
     def salixos_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.salixos_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
 
             if self.repos.salixos_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {self.repos.salixos_repo_mirror[0]} '
                     f'{self.repos.salixos_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}')
-                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}')
-                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}')
+                changelog: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}'
+                packages: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}'
+                checksums: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}'
+
+                urls[changelog] = self.repos.salixos_repo_path
+                urls[packages] = self.repos.salixos_repo_path
+                urls[checksums] = self.repos.salixos_repo_path
 
-                down = Downloader(self.repos.salixos_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.salixos_repo_name)
         self.delete_last_updated(self.repos.salixos_repo_name)
         self.data.install_salixos_data()
 
     def salixos_extra_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.salixos_extra_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_checksums)
 
-            urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}')
+            changelog: str = f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}'
+            urls[changelog] = self.repos.salixos_extra_repo_path
 
             if self.repos.salixos_extra_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_extra_repo_mirror)} '
                     f'{self.repos.salixos_extra_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_packages}')
-                urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_checksums}')
+                packages: str = f'{"".join(self.repos.salixos_extra_repo_mirror)}' \
+                                f'{self.repos.salixos_extra_repo_packages}'
+                checksums: str = (f'{"".join(self.repos.salixos_extra_repo_mirror)}'
+                                  f'{self.repos.salixos_extra_repo_checksums}')
+
+                urls[packages] = self.repos.salixos_extra_repo_path
+                urls[checksums] = self.repos.salixos_extra_repo_path
 
-            down = Downloader(self.repos.salixos_extra_repo_path, urls, self.flags)
-            down.download()
+            self.download.download(urls)
+            print()
 
         self.delete_bin_database_data(self.repos.salixos_extra_repo_name)
         self.delete_last_updated(self.repos.salixos_extra_repo_name)
         self.data.install_salixos_extra_data()
 
     def salixos_patches_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.slack_patches_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
                                              self.repos.salixos_patches_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
                                              self.repos.salixos_patches_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
                                              self.repos.salixos_patches_repo_checksums)
 
-            urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}')
+            changelog: str = f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}'
+            urls[changelog] = self.repos.salixos_patches_repo_path
 
             if self.repos.salixos_patches_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_patches_repo_mirror)} '
                     f'{self.repos.salixos_patches_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
-                            f'{self.repos.salixos_patches_repo_packages}')
-                urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
-                            f'{self.repos.salixos_patches_repo_checksums}')
+                packages: str = (f'{"".join(self.repos.salixos_patches_repo_mirror)}'
+                                 f'{self.repos.salixos_patches_repo_packages}')
+                checksums: str = (f'{"".join(self.repos.salixos_patches_repo_mirror)}'
+                                  f'{self.repos.salixos_patches_repo_checksums}')
 
-            down = Downloader(self.repos.salixos_patches_repo_path, urls, self.flags)
-            down.download()
+                urls[packages] = self.repos.salixos_patches_repo_path
+                urls[checksums] = self.repos.salixos_patches_repo_path
+
+            self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.salixos_patches_repo_name)
         self.delete_last_updated(self.repos.salixos_patches_repo_name)
         self.data.install_salixos_patches_data()
 
     def slackel_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.slackel_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
 
             if self.repos.slackel_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {self.repos.slackel_repo_mirror[0]} '
                     f'{self.repos.slackel_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}')
-                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}')
-                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}')
+                changelog: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}'
+                packages: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}'
+                checksums: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}'
+
+                urls[changelog] = self.repos.slackel_repo_path
+                urls[packages] = self.repos.slackel_repo_path
+                urls[checksums] = self.repos.slackel_repo_path
 
-                down = Downloader(self.repos.slackel_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slackel_repo_name)
         self.delete_last_updated(self.repos.slackel_repo_name)
         self.data.install_slackel_data()
 
     def slint_repository(self) -> None:
         if not self.option_for_install_data:
-            urls: list = []
+            urls: dict = {}
             self.utils.create_directory(self.repos.slint_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
 
             if self.repos.slint_repo_local[0].startswith('file'):
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {self.repos.slint_repo_mirror[0]} '
                     f'{self.repos.slint_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
-                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}')
-                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}')
-                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}')
+                changelog: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}'
+                packages: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}'
+                checksums: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}'
+
+                urls[changelog] = self.repos.slint_repo_path
+                urls[packages] = self.repos.slint_repo_path
+                urls[checksums] = self.repos.slint_repo_path
 
-                down = Downloader(self.repos.slint_repo_path, urls, self.flags)
-                down.download()
+                self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slint_repo_name)
         self.delete_last_updated(self.repos.slint_repo_name)
         self.data.install_slint_data()
 
     def ponce_repository(self) -> None:
@@ -593,15 +647,15 @@
         if not Path(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds).is_file():
             self.generate.slackbuild_file(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
 
         self.delete_last_updated(self.repos.sbo_repo_name)
         self.delete_sbo_database_data()
         self.data.install_sbo_data()
 
-    def check_for_updates(self, queue) -> None:
+    def check_for_updates(self, queue) -> dict:
         compare: dict = self.check_updates.check_the_repositories()
         self.print_the_messages(compare)
 
         return queue.put(compare)
 
     def print_the_messages(self, compare: dict) -> None:
         print()
@@ -630,15 +684,14 @@
 
         # Terminate process 2 if process 1 finished
         if not process_1.is_alive():
             process_2.terminate()
 
         # Restore the terminal cursor
         print('\x1b[?25h', self.endc, end='')
-
         self.repos_for_update: dict = queue.get()
         self.update_the_repositories()
 
     def delete_sbo_database_data(self) -> None:
         """ Delete all the data from a table of the database. """
         self.session.query(SBoTable).delete()
         self.session.commit()
```

### Comparing `slpkg-4.8.6/slpkg/progress_bar.py` & `slpkg-4.8.7/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/downloader.py` & `slpkg-4.8.7/slpkg/downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import shutil
-from typing import Union
 from pathlib import Path
 from multiprocessing import Process
 from urllib.parse import unquote, urlparse
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 
 
 class Downloader(Configs):
 
-    def __init__(self, path: Union[str, Path], urls: list, flags: list):
+    def __init__(self, flags: list):
         super(Configs, self).__init__()
-        self.path: Path = path
-        self.urls: list = urls
         self.flags: list = flags
 
         self.errors = Errors()
         self.utils = Utilities()
 
         self.filename = None
         self.downloader_command: str = str()
@@ -30,59 +27,59 @@
             'wget2': self.wget_downloader,
             'curl': self.curl_downloader,
             'lftp': self.lftp_downloader
         }
         self.option_for_parallel: bool = self.utils.is_option(
             ('-P', '--parallel'), flags)
 
-    def download(self) -> None:
+    def download(self, sources: dict) -> None:
         """ Starting the processing for downloading. """
         processes: list = []
 
         if self.parallel_downloads or self.option_for_parallel:
-            for url in self.urls:
-                proc = Process(target=self.tools, args=(url,))
+            for url, path in sources.items():
+                proc = Process(target=self.tools, args=(url, path))
                 processes.append(proc)
                 proc.start()
 
             for process in processes:
                 process.join()
         else:
-            for url in self.urls:
-                self.tools(url)
+            for url, path in sources.items():
+                self.tools(url, path)
 
-    def tools(self, url: str) -> None:
-        path: str = urlparse(url).path
-        self.filename: str = unquote(Path(path).name)
+    def tools(self, url: str, path: Path) -> None:
+        url_parse: str = urlparse(url).path
+        self.filename: str = unquote(Path(url_parse).name)
 
         if url.startswith('file'):
             self.copy_local_binary_file(url)
         else:
             try:
-                self.downloader_tools[self.downloader](url)
+                self.downloader_tools[self.downloader](url, path)
             except KeyError:
                 self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported", exit_status=1)
 
             self.utils.process(self.downloader_command)
-            self.check_if_downloaded(url)
+            self.check_if_downloaded(url, path)
 
     def copy_local_binary_file(self, url: str) -> None:
         try:
             shutil.copy2(Path(url.replace('file:', '')), self.tmp_slpkg)
             print(f"{self.byellow}Copying{self.endc}: {Path(url.replace('file:', ''))} -> {self.tmp_slpkg}")
         except FileNotFoundError as error:
             self.errors.raise_error_message(f'{error}', 1)
 
-    def wget_downloader(self, url: str) -> None:
-        self.downloader_command: str = f'{self.downloader} {self.wget_options} --directory-prefix={self.path} "{url}"'
+    def wget_downloader(self, url: str, path: Path) -> None:
+        self.downloader_command: str = f'{self.downloader} {self.wget_options} --directory-prefix={path} "{url}"'
 
-    def curl_downloader(self, url: str) -> None:
+    def curl_downloader(self, url: str, path: Path) -> None:
         self.downloader_command: str = (f'{self.downloader} {self.curl_options} "{url}" '
-                                        f'--output {self.path}/{self.filename}')
+                                        f'--output {path}/{self.filename}')
 
-    def lftp_downloader(self, url: str) -> None:
-        self.downloader_command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {self.path}'
+    def lftp_downloader(self, url: str, path: Path) -> None:
+        self.downloader_command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {path}'
 
-    def check_if_downloaded(self, url: str) -> None:
-        path_file: Path = Path(self.path, self.filename)
+    def check_if_downloaded(self, url: str, path: Path) -> None:
+        path_file: Path = Path(path, self.filename)
         if not path_file.exists():
             self.errors.raise_error_message(f"Download the '{url}'", exit_status=20)
```

### Comparing `slpkg-4.8.6/slpkg/models/models.py` & `slpkg-4.8.7/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/rules.py` & `slpkg-4.8.7/slpkg/rules.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/views/view_package.py` & `slpkg-4.8.7/slpkg/views/view_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self.repo_tar_suffix: str = str()
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def slackbuild(self, data: dict, slackbuilds: list) -> None:
         """ View slackbuild packages information. """
+        print()
         repo: dict = {
             self.repos.sbo_repo_name: self.repos.sbo_repo_tar_suffix,
             self.repos.ponce_repo_name: str()
         }
         self.repo_tar_suffix: str = repo[self.repository]
         self.repository_packages: tuple = tuple(data.keys())
 
@@ -106,18 +107,19 @@
               f"Md5sum_x86_64: {self.yellow}{item['md5sum64']}{self.endc}\n"
               f"Files: {self.green}{item['files']}{self.endc}\n"
               f"Description: {self.green}{item['description']}{self.endc}\n"
               f"Category: {self.red}{item['location']}{self.endc}\n"
               f"SBo url: {self.blue}{self.mirror}{item['location']}/{name}{self.endc}\n"
               f"Maintainer: {self.yellow}{self.maintainer}{self.endc}\n"
               f"Email: {self.yellow}{self.email}{self.endc}\n"
-              f"\nREADME: {self.cyan}{''.join(self.readme)}{self.endc}")
+              f"README: {self.cyan}{''.join(self.readme)}{self.endc}")
 
     def package(self, data: dict, packages: list) -> None:
         """ View binary packages information. """
+        print()
         self.repository_packages: tuple = tuple(data.keys())
         for package in packages:
             for name, item in data.items():
                 if package == name or package == '*':
 
                     self.assign_dependencies(item)
                     self.assign_dependencies_with_version(item, data)
```

### Comparing `slpkg-4.8.6/slpkg/views/version.py` & `slpkg-4.8.7/slpkg/views/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 6)
+        self.version_info: tuple = (4, 8, 7)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.6/slpkg/views/cli_menu.py` & `slpkg-4.8.7/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/views/asciibox.py` & `slpkg-4.8.7/slpkg/views/asciibox.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,18 +86,19 @@
               f"{self.bd_color}{self.vertical_line}")
         self.draw_middle_line()
         print(f"{self.bd_color}{self.vertical_line}{self.endc} {'Package:':<{self.package_alignment}}"
               f"{'Version:':<{self.version_alignment}}{'Size:':<{self.size_alignment}}{'Repo:':>{self.repo_alignment}} "
               f"{self.bd_color}{self.vertical_line}{self.endc}")
 
     def draw_package_line(self, package: str, version: str, size: str, color: str, repo: str) -> None:
-        if len(version) >= 20 and self.columns <= 80:
+        if len(version) >= (self.version_alignment - 5):
             version: str = f'{version[:self.version_alignment - 5]}...'
-        if len(package) >= 15 and self.columns <= 80:
-            package: str = f'{package[:self.package_alignment - 5]}...'
+        if len(package) >= (self.package_alignment - 4):
+            package: str = f'{package[:self.package_alignment - 4]}...'
+
         print(f"{self.bd_color}{self.vertical_line} {self.bold}{color}{package:<{self.package_alignment}}{self.endc}"
               f"{self.bd_color}{version:<{self.version_alignment}}{self.endc}{size:<{self.size_alignment}}{self.blue}"
               f"{repo:>{self.repo_alignment}}{self.bd_color} {self.vertical_line}{self.endc}")
 
     def draw_middle_line(self) -> None:
         print(f"{self.bd_color}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
               f"{self.vertical_and_left}")
```

### Comparing `slpkg-4.8.6/slpkg/views/help_commands.py` & `slpkg-4.8.7/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/views/views.py` & `slpkg-4.8.7/slpkg/views/views.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/checks.py` & `slpkg-4.8.7/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/logging_deps.py` & `slpkg-4.8.7/slpkg/logging_deps.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/new_configs.py` & `slpkg-4.8.7/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/multi_process.py` & `slpkg-4.8.7/slpkg/multi_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/cleanings.py` & `slpkg-4.8.7/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/checksum.py` & `slpkg-4.8.7/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/configs.py` & `slpkg-4.8.7/slpkg/configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/utilities.py` & `slpkg-4.8.7/slpkg/utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/dependees.py` & `slpkg-4.8.7/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/toml_error_message.py` & `slpkg-4.8.7/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/check_updates.py` & `slpkg-4.8.7/slpkg/check_updates.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/remove_packages.py` & `slpkg-4.8.7/slpkg/remove_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,23 +144,22 @@
     def delete_package_from_logs(self, package) -> None:
         if not self.option_for_resolve_off:
             self.session.query(LogsDependencies).filter(
                 LogsDependencies.name == package).delete()
             self.session.commit()
 
     def choose_dependencies_for_remove(self) -> None:
-        if self.dependencies:
+        if self.dependencies and self.dialog:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = " Choose dependencies you want to remove "
 
             for package in self.dependencies:
                 installed_package: str = self.utils.is_package_installed(package)
                 installed_version: str = self.utils.split_package(installed_package)['version']
                 choices.extend([(package, installed_version, True, f'Package: {installed_package}')])
 
             text: str = f'There are {len(choices)} dependencies:'
-            code, self.dependencies = self.dialogbox.checklist(text, self.dependencies, title, height,
-                                                               width, list_height, choices)
+            code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
             os.system('clear')
```

### Comparing `slpkg-4.8.6/slpkg/blacklist.py` & `slpkg-4.8.7/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/download_only.py` & `slpkg-4.8.7/slpkg/download_only.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,19 @@
         super(Configs, self).__init__()
         self.directory: Path = directory
         self.flags: list = flags
         self.data: dict = data
         self.repository: str = repository
 
         self.view = ViewMessage(flags, repository, data)
+        self.download = Downloader(flags)
         self.repos = Repositories()
         self.utils = Utilities()
         self.session = Session
-        self.urls: list = []
+        self.urls: dict = {}
         self.download_path: Path = Path()
 
         self.sbo_repo: dict = {
             self.repos.sbo_repo_name: self.repos.sbo_repo_path,
             self.repos.ponce_repo_name: self.repos.ponce_repo_path
         }
 
@@ -65,27 +66,27 @@
         if self.option_for_directory:
             self.download_path: Path = self.directory
 
     def save_binary_sources(self, name: str) -> None:
         package: str = self.data[name]['package']
         mirror: str = self.data[name]['mirror']
         location: str = self.data[name]['location']
-        self.urls.append(f'{mirror}{location}/{package}')
+        self.urls[f'{mirror}{location}/{package}'] = self.tmp_slpkg
 
     def save_slackbuild_sources(self, name: str) -> None:
         if self.os_arch == 'x86_64' and self.data[name]['download64']:
             sources: list = self.data[name]['download64'].split()
         else:
             sources: list = self.data[name]['download'].split()
-        self.urls.extend(sources)
+        for source in sources:
+            self.urls[source] = Path(self.build_path, name)
 
     def copy_slackbuild_scripts(self, name: str) -> None:
         repo_path_package: Path = Path(self.sbo_repo[self.repository], self.data[name]['location'], name)
         if not Path(self.download_path, name).is_dir():
             shutil.copytree(repo_path_package, Path(self.download_path, name))
         print(f"{self.byellow}Copying{self.endc}: {repo_path_package} -> {Path(self.download_path, name)}")
 
     def download_the_sources(self) -> None:
         if self.urls:
             print(f'\nStarted to download total ({self.cyan}{len(self.urls)}{self.endc}) sources:\n')
-            down = Downloader(self.download_path, self.urls, self.flags)
-            down.download()
+            self.download.download(self.urls)
```

### Comparing `slpkg-4.8.6/slpkg/tracking.py` & `slpkg-4.8.7/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/logging_config.py` & `slpkg-4.8.7/slpkg/logging_config.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/main.py` & `slpkg-4.8.7/slpkg/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from slpkg.dependees import Dependees
 from slpkg.utilities import Utilities
 from slpkg.cleanings import Cleanings
 from slpkg.search import SearchPackage
 from slpkg.views.cli_menu import Usage
 from slpkg.dialog_box import DialogBox
 from slpkg.views.version import Version
+from slpkg.views.asciibox import AsciiBox
 from slpkg.sbos.queries import SBoQueries
 from slpkg.views.help_commands import Help
 from slpkg.repositories import Repositories
 from slpkg.binaries.install import Packages
 from slpkg.dialog_configs import FormConfigs
 from slpkg.check_updates import CheckUpdates
 from slpkg.download_only import DownloadOnly
@@ -41,14 +42,15 @@
         self.args: list = args
         self.flags: list = []
         self.directory: Path = self.tmp_slpkg
 
         self.utils = Utilities()
         self.usage = Usage()
         self.repos = Repositories()
+        self.ascii = AsciiBox()
 
         self.repository: str = self.repos.default_repository
 
         self.data: dict = {}
         self.flag_yes: str = '--yes'
         self.flag_short_yes: str = '-y'
         self.flag_jobs: str = '--jobs'
@@ -311,18 +313,20 @@
         logger = logging.getLogger(LoggingConfig.date_time)
         logger.info(f'{self.__class__.__name__}: '
                     f'{self.__class__.__init__.__name__}: '
                     f'{args=}, {self.flags=}, {self.repository=}')
 
     def load_database(self):
         if self.repository != '*' and not self.data:
+            print('\rDatabase loading... ', end='')
             if self.is_binary:
                 self.data: dict = BinQueries(self.repository).repository_data()
             else:
                 self.data: dict = SBoQueries(self.repository).repository_data()
+            print(f'{self.yellow}{self.ascii.done}{self.endc}')
 
     def check_for_repositories(self) -> None:
         """ Checks combination for binaries use repositories only and if repository exists. """
         except_options: tuple = (
             '-s', 'search',
         )
         if self.repository == '*' and not self.utils.is_option(except_options, self.args):
@@ -637,18 +641,14 @@
     def search(self) -> None:
         command: str = Menu.search.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
-            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
-                self.load_database()
-                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
-
             if self.utils.is_option(self.flag_searches, self.flags):
                 self.load_database()
                 packages: list = self.choose.packages(self.data, packages, command)
 
             pkgs = SearchPackage(self.flags, packages, self.repository)
             pkgs.search()
             raise SystemExit()
@@ -754,87 +754,89 @@
     def clean_data(self) -> None:
         if len(self.args) == 1:
             self.clean.db_tables()
             raise SystemExit()
         self.usage.help_short(1)
 
 
-class ChoosePackages:
+class ChoosePackages(Configs):
     """ Choose packages with dialog utility and -S, --search flag. """
 
     def __init__(self, repository: str):
         self.repository: str = repository
 
         self.utils = Utilities()
         self.dialogbox = DialogBox()
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
     def packages(self, data: dict, packages: list, method: str) -> list:
-        height: int = 10
-        width: int = 70
-        list_height: int = 0
-        choices: list = []
-        title: str = f' Choose packages you want to {method} '
-
-        repo_packages: list = list(data.keys())
-
-        if method in ['remove', 'find']:
-            installed: list = list(self.utils.installed_packages.values())
-
-            for package in installed:
-                package_name: str = self.utils.split_package(package)['name']
-                package_version: str = self.utils.split_package(package)['version']
+        if self.dialog:
+            height: int = 10
+            width: int = 70
+            list_height: int = 0
+            choices: list = []
+            title: str = f' Choose packages you want to {method} '
+
+            repo_packages: list = list(data.keys())
+
+            if method in ['remove', 'find']:
+                installed: list = list(self.utils.installed_packages.values())
+
+                for package in installed:
+                    package_name: str = self.utils.split_package(package)['name']
+                    package_version: str = self.utils.split_package(package)['version']
+
+                    for pkg in packages:
+                        if pkg in package or pkg == '*':
+                            choices.extend([(package_name, package_version, False, f'Package: {package}')])
 
+            elif method == 'upgrade':
                 for pkg in packages:
-                    if pkg in package or pkg == '*':
-                        choices.extend([(package_name, package_version, False, f'Package: {package}')])
+                    for package in repo_packages:
 
-        elif method == 'upgrade':
-            for pkg in packages:
-                for package in repo_packages:
-
-                    if pkg == package:
-                        inst_pkg: str = self.utils.is_package_installed(package)
-                        inst_package_version: str = self.utils.split_package(inst_pkg)['version']
-                        inst_package_build: str = self.utils.split_package(inst_pkg)['build']
-                        repo_ver: str = data[package]['version']
-
-                        if self.is_binary:
-                            bin_pkg: str = data[package]['package']
-                            repo_build_tag: str = self.utils.split_package(bin_pkg[:-4])['build']
-                        else:
-                            repo_location: str = data[package]['location']
-                            repo_build_tag: str = self.utils.read_slackbuild_build_tag(
-                                package, repo_location, self.repository
+                        if pkg == package:
+                            inst_pkg: str = self.utils.is_package_installed(package)
+                            inst_package_version: str = self.utils.split_package(inst_pkg)['version']
+                            inst_package_build: str = self.utils.split_package(inst_pkg)['build']
+                            repo_ver: str = data[package]['version']
+
+                            if self.is_binary:
+                                bin_pkg: str = data[package]['package']
+                                repo_build_tag: str = self.utils.split_package(bin_pkg[:-4])['build']
+                            else:
+                                repo_location: str = data[package]['location']
+                                repo_build_tag: str = self.utils.read_slackbuild_build_tag(
+                                    package, repo_location, self.repository
+                                )
+
+                            choices.extend(
+                                [(package, f'{inst_package_version} -> {repo_ver}', True,
+                                  f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
+                                  f'Available: {repo_ver} Build: {repo_build_tag}')]
                             )
+            else:
+                for pkg in packages:
+                    for package in repo_packages:
 
-                        choices.extend([(package, f'{inst_package_version} -> {repo_ver}', True,
-                                         f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
-                                        f'Available: {repo_ver} Build: {repo_build_tag}')])
-        else:
-            for pkg in packages:
-                for package in repo_packages:
+                        if pkg in package or pkg == '*':
+                            version: str = data[package]['version']
+                            choices.extend([(package, version, False, f'Package: {package}-{version} '
+                                           f'> {self.repository}')])
+
+            if not choices:
+                return packages
+
+            text: str = f'There are {len(choices)} packages:'
+            code, packages = self.dialogbox.checklist(text, title, height, width, list_height, choices)
+            if code == 'cancel' or not packages:
+                os.system('clear')
+                raise SystemExit()
 
-                    if pkg in package or pkg == '*':
-                        version: str = data[package]['version']
-                        choices.extend([(package, version, False, f'Package: {package}-{version} '
-                                       f'> {self.repository}')])
-
-        if not choices:
-            return packages
-
-        text: str = f'There are {len(choices)} packages:'
-        code, packages = self.dialogbox.checklist(text, packages, title, height,
-                                                  width, list_height, choices)
-        if code == 'cancel' or not packages:
             os.system('clear')
-            raise SystemExit()
-
-        os.system('clear')
 
         return packages
 
 
 def main() -> None:
     args: list = sys.argv
     args.pop(0)
```

### Comparing `slpkg-4.8.6/slpkg/find_installed.py` & `slpkg-4.8.7/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg/upgrade.py` & `slpkg-4.8.7/slpkg/upgrade.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import logging
 from typing import Generator
 from packaging.version import parse, InvalidVersion
 
+from slpkg.rules import Rules
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
-from slpkg.rules import Rules
 
 
 class Upgrade(Configs):
     """ Upgrade the installed packages. """
 
     def __init__(self, repository: str, data: dict):
         super(Configs, self).__init__()
```

### Comparing `slpkg-4.8.6/slpkg/search.py` & `slpkg-4.8.7/slpkg/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
+from slpkg.views.asciibox import AsciiBox
 from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
 from slpkg.binaries.queries import BinQueries
 
 
 class SearchPackage(Configs):
     """ Search packages from the repositories. """
@@ -14,33 +15,37 @@
     def __init__(self, flags: list, packages: list, repository: str):
         super(Configs, self).__init__()
         self.packages: list = packages
         self.repository: str = repository
 
         self.utils = Utilities()
         self.repos = Repositories()
+        self.ascii = AsciiBox()
 
         self.matching: int = 0
         self.repo_data: dict = {}
         self.data_dict: dict = {}
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_no_case: bool = self.utils.is_option(
             ('-m', '--no-case'), flags)
 
     def search(self) -> None:
-        print(f'The list below shows the repo '
-              f'packages that contains \'{", ".join([p for p in self.packages])}\':\n')
+        print('\rDatabase loading... ', end='')
 
         if self.repository == '*':
             self.search_to_all_repositories()
         else:
             self.search_to_the_repository()
 
+        print(f'{self.yellow}{self.ascii.done}{self.endc}')
+        print(f'The list below shows the repo '
+              f'packages that contains \'{", ".join([p for p in self.packages])}\':\n')
+
         self.summary_of_searching()
 
     def search_to_all_repositories(self) -> None:
         for repo, item in self.repos.repositories.items():
             if item['enable']:  # Check if the repository is enabled
                 if self.utils.is_binary_repo(repo):
                     self.repo_data: dict = BinQueries(repo).repository_data()
```

### Comparing `slpkg-4.8.6/setup.cfg` & `slpkg-4.8.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.8.6
+version = 4.8.7
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = dslackw@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls =
```

### Comparing `slpkg-4.8.6/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.7/slpkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.6/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.7/slpkg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.6
+Version: 4.8.7
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: dslackw@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
```

### Comparing `slpkg-4.8.6/README.md` & `slpkg-4.8.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
 ```
 $ slpkg repo-info
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_repo_info.png" width="900">
 
 ```
-$ slpkg install audacity --repository=alien
+$ slpkg install lilv --repository=alien
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png" width="900">
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_done.png" width="900">
 
 ```
-$ slpkg remove audacity
+$ slpkg remove lilv
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove.png" width="900">
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove_done.png" width="900">
 
 ```
 $ slpkg dependees --pkg-version --full-reverse greenlet
 ```
@@ -56,16 +56,16 @@
 $ slpkg tracking --pkg-version Flask awscli pychess
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.6.tar.gz
-$ cd slpkg-4.8.6
+$ tar xvf slpkg-4.8.7.tar.gz
+$ cd slpkg-4.8.7
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -82,15 +82,15 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-slpkg - version 4.8.6
+slpkg - version 4.8.7
 
 USAGE:
   slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
 
 DESCRIPTION:
   Package manager utility for Slackware.
```

### Comparing `slpkg-4.8.6/tools/gen_sbo_txt.sh` & `slpkg-4.8.7/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

