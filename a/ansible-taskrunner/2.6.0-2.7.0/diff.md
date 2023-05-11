# Comparing `tmp/ansible_taskrunner-2.6.0.tar.gz` & `tmp/ansible_taskrunner-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_taskrunner-2.6.0.tar", last modified: Thu Mar 16 19:51:12 2023, max compression
+gzip compressed data, was "ansible_taskrunner-2.7.0.tar", last modified: Fri Mar 24 15:58:06 2023, max compression
```

## Comparing `ansible_taskrunner-2.6.0.tar` & `ansible_taskrunner-2.7.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.693807 ansible_taskrunner-2.6.0/
--rw-r--r--   0 etejeda    (501) staff       (20)      313 2022-09-14 03:08:59.000000 ansible_taskrunner-2.6.0/.editorconfig
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.659474 ansible_taskrunner-2.6.0/.github/
--rw-r--r--   0 etejeda    (501) staff       (20)      344 2022-09-14 03:08:56.000000 ansible_taskrunner-2.6.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1558 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      314 2022-09-14 03:05:03.000000 ansible_taskrunner-2.6.0/.travis.yml
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2022-09-14 03:04:51.000000 ansible_taskrunner-2.6.0/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     3790 2022-09-14 03:04:49.000000 ansible_taskrunner-2.6.0/CONTRIBUTING.rst
--rw-r--r--   0 etejeda    (501) staff       (20)    26248 2023-03-16 19:50:50.000000 ansible_taskrunner-2.6.0/HISTORY.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2022-09-14 03:04:47.000000 ansible_taskrunner-2.6.0/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      365 2022-09-14 03:18:38.000000 ansible_taskrunner-2.6.0/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)    11310 2023-03-07 16:33:18.000000 ansible_taskrunner-2.6.0/Makefile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-03-16 19:51:12.694182 ansible_taskrunner-2.6.0/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)    58542 2023-03-15 18:52:08.000000 ansible_taskrunner-2.6.0/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     5182 2023-03-08 21:35:43.000000 ansible_taskrunner-2.6.0/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-03-16 19:50:12.000000 ansible_taskrunner-2.6.0/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.661741 ansible_taskrunner-2.6.0/ansible_taskrunner/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2479 2023-03-07 16:10:01.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/cli.py
--rw-r--r--   0 etejeda    (501) staff       (20)      958 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      803 2023-03-08 21:32:42.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/defaults.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.665832 ansible_taskrunner-2.6.0/ansible_taskrunner/files/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.666483 ansible_taskrunner-2.6.0/ansible_taskrunner/files/cfg/
--rw-r--r--   0 etejeda    (501) staff       (20)      159 2023-01-10 10:27:20.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/files/cfg/default.ini
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.667097 ansible_taskrunner-2.6.0/ansible_taskrunner/files/macros/
--rw-r--r--   0 etejeda    (501) staff       (20)     1116 2023-01-10 10:27:25.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/files/macros/default.mac
--rw-r--r--   0 etejeda    (501) staff       (20)      956 2023-01-10 10:27:29.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/files/start-tutorial.bat
--rw-r--r--   0 etejeda    (501) staff       (20)     1772 2023-01-10 10:27:30.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/files/tasks-console.bat
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.667581 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.667836 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/bastion_mode/
--rw-r--r--   0 etejeda    (501) staff       (20)     1354 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/bastion_mode/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.670072 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/
--rw-r--r--   0 etejeda    (501) staff       (20)     6181 2023-03-07 16:23:01.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2868 2023-03-07 15:21:06.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_create_group.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2917 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_create_init.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5240 2023-03-09 08:40:19.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_create_sub.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5660 2023-03-10 21:27:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_init_sub.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4667 2023-03-15 18:34:45.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/invocation.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.671076 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/click_extras/
--rw-r--r--   0 etejeda    (501) staff       (20)     9512 2023-03-13 16:50:02.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/click_extras/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2059 2023-03-15 18:47:17.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/click_extras/help.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2512 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/click_extras/options_advanced.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.671465 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/errorhandler/
--rw-r--r--   0 etejeda    (501) staff       (20)      738 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/errorhandler/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.671791 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/formatting/
--rw-r--r--   0 etejeda    (501) staff       (20)      787 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/formatting/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.672136 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/help/
--rw-r--r--   0 etejeda    (501) staff       (20)     2738 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/help/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.673130 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/language/
--rw-r--r--   0 etejeda    (501) staff       (20)      876 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/language/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)       19 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/language/en.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.673756 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/logger/
--rw-r--r--   0 etejeda    (501) staff       (20)      462 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/logger/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.674503 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/proc_mgmt/
--rw-r--r--   0 etejeda    (501) staff       (20)     3334 2023-03-08 20:54:23.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/proc_mgmt/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.676124 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)    15894 2023-03-13 18:12:26.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/ansible.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2481 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/bash.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2561 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/vagrant.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.678466 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5474 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/client.py
--rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-01-09 04:21:28.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/scp.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2949 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/sync.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1485 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.678913 ansible_taskrunner-2.6.0/ansible_taskrunner/plugins/
--rw-r--r--   0 etejeda    (501) staff       (20)     1951 2023-01-10 10:29:26.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/plugins/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5089 2023-01-09 21:15:54.000000 ansible_taskrunner-2.6.0/ansible_taskrunner/setup.cx_freeze.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.664638 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-03-16 19:51:12.000000 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     2948 2023-03-16 19:51:12.000000 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-03-16 19:51:12.000000 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       53 2023-03-16 19:51:12.000000 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-03-16 19:51:12.000000 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      249 2023-03-16 19:51:12.000000 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       25 2023-03-16 19:51:12.000000 ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.684573 ansible_taskrunner-2.6.0/docs/
--rw-r--r--   0 etejeda    (501) staff       (20)      636 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/docs/Makefile
--rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/authors.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     5127 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/conf.py
--rw-r--r--   0 etejeda    (501) staff       (20)       34 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/contributing.rst
--rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/history.rst
--rw-r--r--   0 etejeda    (501) staff       (20)      335 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/index.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1261 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/installation.rst
--rw-r--r--   0 etejeda    (501) staff       (20)      816 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/make.bat
--rw-r--r--   0 etejeda    (501) staff       (20)       28 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/readme.rst
--rw-r--r--   0 etejeda    (501) staff       (20)       98 2022-09-14 03:04:03.000000 ansible_taskrunner-2.6.0/docs/usage.rst
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.650110 ansible_taskrunner-2.6.0/examples/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.685737 ansible_taskrunner-2.6.0/examples/ansible/
--rw-r--r--   0 etejeda    (501) staff       (20)     5071 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/ansible/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1967 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/ansible/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/ansible/config.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.687013 ansible_taskrunner-2.6.0/examples/bash/
--rw-r--r--   0 etejeda    (501) staff       (20)     2933 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/bash/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/bash/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       44 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/bash/config.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.687630 ansible_taskrunner-2.6.0/examples/choice/
--rw-r--r--   0 etejeda    (501) staff       (20)     2300 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/choice/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.689325 ansible_taskrunner-2.6.0/examples/custom-cli-provider/
--rw-r--r--   0 etejeda    (501) staff       (20)     3046 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/custom-cli-provider/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/custom-cli-provider/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/custom-cli-provider/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      177 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/custom-cli-provider/dynamic-import.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.648882 ansible_taskrunner-2.6.0/examples/custom-cli-provider/plugins/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.649061 ansible_taskrunner-2.6.0/examples/custom-cli-provider/plugins/providers/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.689798 ansible_taskrunner-2.6.0/examples/custom-cli-provider/plugins/providers/example/
--rw-r--r--   0 etejeda    (501) staff       (20)     2187 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/custom-cli-provider/plugins/providers/example/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.690399 ansible_taskrunner-2.6.0/examples/mutually-exclusive/
--rw-r--r--   0 etejeda    (501) staff       (20)     2354 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/mutually-exclusive/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.690922 ansible_taskrunner-2.6.0/examples/prompt/
--rw-r--r--   0 etejeda    (501) staff       (20)     2275 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/prompt/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.692517 ansible_taskrunner-2.6.0/examples/vagrant/
--rw-r--r--   0 etejeda    (501) staff       (20)     4168 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/vagrant/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1506 2023-03-07 02:31:15.000000 ansible_taskrunner-2.6.0/examples/vagrant/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     3092 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/vagrant/Vagrantfile
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2022-09-14 03:03:59.000000 ansible_taskrunner-2.6.0/examples/vagrant/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-03-07 16:28:11.000000 ansible_taskrunner-2.6.0/requirements_dev.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1596 2023-03-16 19:51:12.695096 ansible_taskrunner-2.6.0/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       39 2022-09-14 03:03:38.000000 ansible_taskrunner-2.6.0/setup.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-16 19:51:12.693308 ansible_taskrunner-2.6.0/tests/
--rw-r--r--   0 etejeda    (501) staff       (20)       76 2022-09-14 03:04:16.000000 ansible_taskrunner-2.6.0/tests/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2433 2023-03-13 18:35:06.000000 ansible_taskrunner-2.6.0/tests/test_ansible_taskrunner.py
--rw-r--r--   0 etejeda    (501) staff       (20)      343 2022-09-14 03:17:41.000000 ansible_taskrunner-2.6.0/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.963514 ansible_taskrunner-2.7.0/
+-rw-r--r--   0 etejeda    (501) staff       (20)      313 2022-09-14 03:08:59.000000 ansible_taskrunner-2.7.0/.editorconfig
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.917511 ansible_taskrunner-2.7.0/.github/
+-rw-r--r--   0 etejeda    (501) staff       (20)      344 2022-09-14 03:08:56.000000 ansible_taskrunner-2.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1558 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      314 2022-09-14 03:05:03.000000 ansible_taskrunner-2.7.0/.travis.yml
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2022-09-14 03:04:51.000000 ansible_taskrunner-2.7.0/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     3790 2022-09-14 03:04:49.000000 ansible_taskrunner-2.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)    26436 2023-03-24 15:57:41.000000 ansible_taskrunner-2.7.0/HISTORY.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2022-09-14 03:04:47.000000 ansible_taskrunner-2.7.0/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      365 2022-09-14 03:18:38.000000 ansible_taskrunner-2.7.0/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)    11310 2023-03-07 16:33:18.000000 ansible_taskrunner-2.7.0/Makefile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-03-24 15:58:06.963876 ansible_taskrunner-2.7.0/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)    58542 2023-03-15 18:52:08.000000 ansible_taskrunner-2.7.0/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     5182 2023-03-08 21:35:43.000000 ansible_taskrunner-2.7.0/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-03-24 15:56:32.000000 ansible_taskrunner-2.7.0/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.920653 ansible_taskrunner-2.7.0/ansible_taskrunner/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2479 2023-03-07 16:10:01.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/cli.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      958 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      803 2023-03-08 21:32:42.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/defaults.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.924894 ansible_taskrunner-2.7.0/ansible_taskrunner/files/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.925563 ansible_taskrunner-2.7.0/ansible_taskrunner/files/cfg/
+-rw-r--r--   0 etejeda    (501) staff       (20)      159 2023-01-10 10:27:20.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/files/cfg/default.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.926162 ansible_taskrunner-2.7.0/ansible_taskrunner/files/macros/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1116 2023-01-10 10:27:25.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/files/macros/default.mac
+-rw-r--r--   0 etejeda    (501) staff       (20)      956 2023-01-10 10:27:29.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/files/start-tutorial.bat
+-rw-r--r--   0 etejeda    (501) staff       (20)     1772 2023-01-10 10:27:30.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/files/tasks-console.bat
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.926681 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.926982 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/bastion_mode/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1354 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/bastion_mode/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.931664 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/
+-rw-r--r--   0 etejeda    (501) staff       (20)     6181 2023-03-07 16:23:01.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2868 2023-03-07 15:21:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_create_group.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2917 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_create_init.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5240 2023-03-09 08:40:19.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_create_sub.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5660 2023-03-24 15:45:23.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_init_sub.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4667 2023-03-15 18:34:45.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/invocation.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.933391 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/click_extras/
+-rw-r--r--   0 etejeda    (501) staff       (20)     9512 2023-03-13 16:50:02.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/click_extras/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2228 2023-03-24 15:54:02.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/click_extras/help.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2512 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/click_extras/options_advanced.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.934199 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/errorhandler/
+-rw-r--r--   0 etejeda    (501) staff       (20)      738 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/errorhandler/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.934894 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/formatting/
+-rw-r--r--   0 etejeda    (501) staff       (20)      787 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/formatting/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.935598 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/help/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2738 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/help/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.936962 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/language/
+-rw-r--r--   0 etejeda    (501) staff       (20)      876 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/language/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       19 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/language/en.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.937615 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/logger/
+-rw-r--r--   0 etejeda    (501) staff       (20)      462 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/logger/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.938254 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/proc_mgmt/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3334 2023-03-08 20:54:23.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/proc_mgmt/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.940520 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    15894 2023-03-13 18:12:26.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/ansible.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2481 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/bash.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2561 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/vagrant.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.942818 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5474 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/client.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-01-09 04:21:28.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/scp.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2949 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/sync.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1485 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.943392 ansible_taskrunner-2.7.0/ansible_taskrunner/plugins/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1951 2023-01-10 10:29:26.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/plugins/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5089 2023-01-09 21:15:54.000000 ansible_taskrunner-2.7.0/ansible_taskrunner/setup.cx_freeze.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.923832 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-03-24 15:58:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     2948 2023-03-24 15:58:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-03-24 15:58:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       53 2023-03-24 15:58:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-03-24 15:58:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      249 2023-03-24 15:58:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       25 2023-03-24 15:58:06.000000 ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.949218 ansible_taskrunner-2.7.0/docs/
+-rw-r--r--   0 etejeda    (501) staff       (20)      636 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/docs/Makefile
+-rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/authors.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     5127 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/conf.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       34 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/contributing.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/history.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)      335 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/index.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1261 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/installation.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)      816 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/make.bat
+-rw-r--r--   0 etejeda    (501) staff       (20)       28 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/readme.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)       98 2022-09-14 03:04:03.000000 ansible_taskrunner-2.7.0/docs/usage.rst
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.908799 ansible_taskrunner-2.7.0/examples/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.950946 ansible_taskrunner-2.7.0/examples/ansible/
+-rw-r--r--   0 etejeda    (501) staff       (20)     5071 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/ansible/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1967 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/ansible/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/ansible/config.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.952687 ansible_taskrunner-2.7.0/examples/bash/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2933 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/bash/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/bash/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       44 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/bash/config.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.953524 ansible_taskrunner-2.7.0/examples/choice/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2300 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/choice/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.957129 ansible_taskrunner-2.7.0/examples/custom-cli-provider/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3046 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/custom-cli-provider/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/custom-cli-provider/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/custom-cli-provider/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      177 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/custom-cli-provider/dynamic-import.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.908037 ansible_taskrunner-2.7.0/examples/custom-cli-provider/plugins/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.908183 ansible_taskrunner-2.7.0/examples/custom-cli-provider/plugins/providers/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.958084 ansible_taskrunner-2.7.0/examples/custom-cli-provider/plugins/providers/example/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2187 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/custom-cli-provider/plugins/providers/example/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.958805 ansible_taskrunner-2.7.0/examples/mutually-exclusive/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2354 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/mutually-exclusive/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.959685 ansible_taskrunner-2.7.0/examples/prompt/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2275 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/prompt/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.962025 ansible_taskrunner-2.7.0/examples/vagrant/
+-rw-r--r--   0 etejeda    (501) staff       (20)     4168 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/vagrant/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1506 2023-03-07 02:31:15.000000 ansible_taskrunner-2.7.0/examples/vagrant/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     3092 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/vagrant/Vagrantfile
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2022-09-14 03:03:59.000000 ansible_taskrunner-2.7.0/examples/vagrant/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-03-07 16:28:11.000000 ansible_taskrunner-2.7.0/requirements_dev.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1596 2023-03-24 15:58:06.964973 ansible_taskrunner-2.7.0/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       39 2022-09-14 03:03:38.000000 ansible_taskrunner-2.7.0/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-03-24 15:58:06.962836 ansible_taskrunner-2.7.0/tests/
+-rw-r--r--   0 etejeda    (501) staff       (20)       76 2022-09-14 03:04:16.000000 ansible_taskrunner-2.7.0/tests/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2433 2023-03-13 18:35:06.000000 ansible_taskrunner-2.7.0/tests/test_ansible_taskrunner.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      343 2022-09-14 03:17:41.000000 ansible_taskrunner-2.7.0/tox.ini
```

### Comparing `ansible_taskrunner-2.6.0/.gitignore` & `ansible_taskrunner-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/CONTRIBUTING.rst` & `ansible_taskrunner-2.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/HISTORY.md` & `ansible_taskrunner-2.7.0/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =======
 History
 =======
 
+## Release 2023-03-24 v2.7.0
+
+* Improved formatting for ExtendedHelp epilog parser [77a74da](git@github.com:berttejeda/ansible-taskrunner/commit/77a74dab41940a1ee8008d0c9af55991d6a12efe)
+
 ## Release 2023-03-16 v2.6.0
 
 * Adjusted ExtendedHelp epilog parser [cd0b0c9](git@github.com:berttejeda/ansible-taskrunner/commit/cd0b0c986b9cc8ca71157ca3d330cbe240c8e611)
 * Renamed the '---raw' option to '---' [ca473eb](git@github.com:berttejeda/ansible-taskrunner/commit/ca473eb9bc41af0af02e7b1df9d108eb7d28ed57)
 
 ## Release 2023-03-10 v2.5.4
```

### Comparing `ansible_taskrunner-2.6.0/LICENSE` & `ansible_taskrunner-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/Makefile.yaml` & `ansible_taskrunner-2.7.0/Makefile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/PKG-INFO` & `ansible_taskrunner-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible_taskrunner
-Version: 2.6.0
+Version: 2.7.0
 Summary: Ansible Task Runner
 Home-page: https://github.com/berttejeda/ansible-taskrunner.git
 Author: Engelbert Tejeda
 Author-email: etejeda@tecknicos.com
 Keywords: ansible,playbook,wrapper,bash,python,click,task-runner,subprocess,yaml,cli,options
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ansible_taskrunner-2.6.0/README.md` & `ansible_taskrunner-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/Taskfile.yaml` & `ansible_taskrunner-2.7.0/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/cli.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/config.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/config.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/defaults.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/defaults.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/files/macros/default.mac` & `ansible_taskrunner-2.7.0/ansible_taskrunner/files/macros/default.mac`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/files/start-tutorial.bat` & `ansible_taskrunner-2.7.0/ansible_taskrunner/files/start-tutorial.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/files/tasks-console.bat` & `ansible_taskrunner-2.7.0/ansible_taskrunner/files/tasks-console.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/bastion_mode/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/bastion_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_create_group.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_create_group.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_create_init.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_create_init.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_create_sub.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_create_sub.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/click_commands_init_sub.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/click_commands_init_sub.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/cli/invocation.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/cli/invocation.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/click_extras/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/click_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/click_extras/help.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/click_extras/help.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import click
 from ansible_taskrunner.logger import Logger
 import re
 
 logger_obj = Logger()
 logger = logger_obj.init_logger(__name__)
-example_pattern: Pattern[str] = re.compile('- .*[\d]+:')
+example_pattern: Pattern[str] = re.compile('Available shell functions|- .*: \|\W')
 
 class ExtendedEpilog(click.Group):
     def format_epilog(self, ctx, formatter):
         """Format click epilog to honor newline characters"""
         if self.epilog:
             formatter.write_paragraph()
             for line in self.epilog.split('\n'):
@@ -43,15 +43,17 @@
             if rv is not None:
                 opts.append(rv)
         if opts:
             with formatter.section('Options'):
                 formatter.write_dl(opts)
         if self.epilog:
             formatter.write_paragraph()
-            for line in self.epilog.split('\n'):
+            parsed_epilog = re.sub(':\n', ': |-\n', self.epilog.split('Examples:')[-1])
+            for line in parsed_epilog.split('\n'):
                 if line:
+                    tabbed_line = f'\t{line}'
                     if example_pattern.search(line):
                         self.colorize(formatter, 'magenta', line)
                     else:
-                        self.colorize(formatter, 'yellow', line)
+                        self.colorize(formatter, 'yellow', tabbed_line)
                 else:
                     formatter.write_text(line)
```

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/click_extras/options_advanced.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/click_extras/options_advanced.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/errorhandler/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/errorhandler/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/formatting/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/help/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/help/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/language/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/language/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/proc_mgmt/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/proc_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/ansible.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/ansible.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/bash.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/bash.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/providers/vagrant.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/providers/vagrant.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/client.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/client.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/scp.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/scp.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/libs/sshutil/sync.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/libs/sshutil/sync.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/logger.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/logger.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/plugins/__init__.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner/setup.cx_freeze.py` & `ansible_taskrunner-2.7.0/ansible_taskrunner/setup.cx_freeze.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/PKG-INFO` & `ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-taskrunner
-Version: 2.6.0
+Version: 2.7.0
 Summary: Ansible Task Runner
 Home-page: https://github.com/berttejeda/ansible-taskrunner.git
 Author: Engelbert Tejeda
 Author-email: etejeda@tecknicos.com
 Keywords: ansible,playbook,wrapper,bash,python,click,task-runner,subprocess,yaml,cli,options
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ansible_taskrunner-2.6.0/ansible_taskrunner.egg-info/SOURCES.txt` & `ansible_taskrunner-2.7.0/ansible_taskrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/docs/Makefile` & `ansible_taskrunner-2.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/docs/conf.py` & `ansible_taskrunner-2.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/docs/installation.rst` & `ansible_taskrunner-2.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/docs/make.bat` & `ansible_taskrunner-2.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/ansible/README.md` & `ansible_taskrunner-2.7.0/examples/ansible/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/ansible/Taskfile.yaml` & `ansible_taskrunner-2.7.0/examples/ansible/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/bash/README.md` & `ansible_taskrunner-2.7.0/examples/bash/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/bash/Taskfile.yaml` & `ansible_taskrunner-2.7.0/examples/bash/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/choice/Taskfile.yaml` & `ansible_taskrunner-2.7.0/examples/choice/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/custom-cli-provider/README.md` & `ansible_taskrunner-2.7.0/examples/custom-cli-provider/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/custom-cli-provider/Taskfile.yaml` & `ansible_taskrunner-2.7.0/examples/custom-cli-provider/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/custom-cli-provider/plugins/providers/example/__init__.py` & `ansible_taskrunner-2.7.0/examples/custom-cli-provider/plugins/providers/example/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/mutually-exclusive/Taskfile.yaml` & `ansible_taskrunner-2.7.0/examples/mutually-exclusive/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/prompt/Taskfile.yaml` & `ansible_taskrunner-2.7.0/examples/prompt/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/vagrant/README.md` & `ansible_taskrunner-2.7.0/examples/vagrant/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/vagrant/Taskfile.yaml` & `ansible_taskrunner-2.7.0/examples/vagrant/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/examples/vagrant/Vagrantfile` & `ansible_taskrunner-2.7.0/examples/vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/setup.cfg` & `ansible_taskrunner-2.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.6.0/tests/test_ansible_taskrunner.py` & `ansible_taskrunner-2.7.0/tests/test_ansible_taskrunner.py`

 * *Files identical despite different names*

