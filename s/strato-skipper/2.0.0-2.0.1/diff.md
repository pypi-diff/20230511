# Comparing `tmp/strato-skipper-2.0.0.tar.gz` & `tmp/strato-skipper-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strato-skipper-2.0.0.tar", last modified: Tue Mar 14 19:18:49 2023, max compression
+gzip compressed data, was "strato-skipper-2.0.1.tar", last modified: Thu May 11 14:06:52 2023, max compression
```

## Comparing `strato-skipper-2.0.0.tar` & `strato-skipper-2.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:49.963000 strato-skipper-2.0.0/
--rw-r--r--   0 runner    (1001) runner    (1001)      101 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:49.955000 strato-skipper-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:49.959000 strato-skipper-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) runner    (1001)     1816 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) runner    (1001)      701 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) runner    (1001)    11123 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) runner    (1001)     1133 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) runner    (1001)    15143 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/ChangeLog
--rw-r--r--   0 runner    (1001) runner    (1001)      232 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/Dockerfile.skipper-build
--rw-r--r--   0 runner    (1001) runner    (1001)    11351 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)      437 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/Makefile
--rw-r--r--   0 runner    (1001) runner    (1001)     9837 2023-03-14 19:18:49.963000 strato-skipper-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     9528 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)       36 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      120 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      498 2023-03-14 19:18:49.963000 strato-skipper-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)      132 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:49.959000 strato-skipper-2.0.0/skipper/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20536 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/cli.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1421 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/config.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:49.959000 strato-skipper-2.0.0/skipper/data/
--rw-r--r--   0 runner    (1001) runner    (1001)     6615 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/data/skipper-complete.sh
--rwxr-xr-x   0 runner    (1001) runner    (1001)      934 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/data/skipper-entrypoint.sh
--rw-r--r--   0 runner    (1001) runner    (1001)      666 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/git.py
--rw-r--r--   0 runner    (1001) runner    (1001)      585 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/main.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7854 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/runner.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6301 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper/utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)       37 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/skipper.yaml
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:49.963000 strato-skipper-2.0.0/strato_skipper.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     9837 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      849 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       46 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) runner    (1001)       47 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) runner    (1001)      131 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2023-03-14 19:18:49.000000 strato-skipper-2.0.0/strato_skipper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:49.963000 strato-skipper-2.0.0/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    93107 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1792 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/tests/test_git.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28641 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/tests/test_runner.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14645 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/tests/test_runner_podman.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2037 2023-03-14 19:18:10.000000 strato-skipper-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:52.866257 strato-skipper-2.0.1/
+-rw-r--r--   0 runner    (1001) runner    (1001)      101 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:52.862256 strato-skipper-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:52.862256 strato-skipper-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1816 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) runner    (1001)      701 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) runner    (1001)    11123 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) runner    (1001)     1165 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) runner    (1001)    15324 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/ChangeLog
+-rw-r--r--   0 runner    (1001) runner    (1001)      232 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/Dockerfile.skipper-build
+-rw-r--r--   0 runner    (1001) runner    (1001)    11351 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)      437 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/Makefile
+-rw-r--r--   0 runner    (1001) runner    (1001)     9837 2023-05-11 14:06:52.866257 strato-skipper-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     9528 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)       36 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      120 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      498 2023-05-11 14:06:52.866257 strato-skipper-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      132 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:52.866257 strato-skipper-2.0.1/skipper/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20622 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/cli.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1421 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/config.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:52.866257 strato-skipper-2.0.1/skipper/data/
+-rw-r--r--   0 runner    (1001) runner    (1001)     6644 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/data/skipper-complete.sh
+-rwxr-xr-x   0 runner    (1001) runner    (1001)      934 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/data/skipper-entrypoint.sh
+-rw-r--r--   0 runner    (1001) runner    (1001)      666 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/git.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      585 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/main.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7949 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/runner.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6784 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)       37 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/skipper.yaml
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:52.866257 strato-skipper-2.0.1/strato_skipper.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     9837 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      849 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       46 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) runner    (1001)       47 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) runner    (1001)      131 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2023-05-11 14:06:52.000000 strato-skipper-2.0.1/strato_skipper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:52.866257 strato-skipper-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    93476 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1792 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/tests/test_git.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28641 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14855 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/tests/test_runner_podman.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2037 2023-05-11 14:06:04.000000 strato-skipper-2.0.1/tests/test_utils.py
```

### Comparing `strato-skipper-2.0.0/.github/workflows/build.yml` & `strato-skipper-2.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/.github/workflows/publish-to-pypi.yml` & `strato-skipper-2.0.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/.pylintrc` & `strato-skipper-2.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/AUTHORS` & `strato-skipper-2.0.1/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 Raz <rregev@redhat.com>
 Rom Freiman <rom@stratoscale.com>
 Roman Girshberg <romang@stratoscale.com>
 Ronnie Lazar <ronnie.lazar@redhat.com>
 Ronnie Lazar <ronnie@stratoscale.com>
 Shay Arbov <sarbov@shayarbov.strato>
 Shoham Peller <shohamp@gmail.com>
+Ygal Blum <ygal.blum@gmail.com>
 Ygal Blum <ygal.blum@stratoscale.com>
 Yuval Goldberg <yuvigoldi@gmail.com>
 doug-stratoscale <doug.shelley@stratoscale.com>
 michaelf-stratoscale <michael.filanov@stratoscale.com>
 raz <rregev@redhat.com>
 shay-stratoscale <shay.arbov@stratoscale.com>
```

### Comparing `strato-skipper-2.0.0/ChangeLog` & `strato-skipper-2.0.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+2.0.1
+-----
+
+* Add support for Containerfile in addition to Dockerfile
+* When running under podman use keep-groups to maintain the groups of the user
+* Fix tool recognition method
+
 2.0.0
 -----
 
 * Support wheels distribution
 * Dummy commit to allow the git action to start
 * README: escape dollars to avoid math rendering
 * fix unit-tests after changing the code
```

### Comparing `strato-skipper-2.0.0/LICENSE` & `strato-skipper-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/PKG-INFO` & `strato-skipper-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strato-skipper
-Version: 2.0.0
+Version: 2.0.1
 Summary: Easily dockerize your Git repository
 Home-page: http://github.com/Stratoscale/skipper
 Author: Adir Gabai
 Author-email: adir@stratoscale.com
 License: Apache-2
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `strato-skipper-2.0.0/README.md` & `strato-skipper-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/skipper/cli.py` & `strato-skipper-2.0.1/skipper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             valid_images_to_build[image] = valid_images[image]
 
     tag = git.get_hash()
     for image, dockerfile in six.iteritems(valid_images_to_build):
         utils.logger.info('Building image: %s', image)
 
         if not os.path.exists(dockerfile):
-            utils.logger.warning('Dockerfile %s does not exist! Skipping...', dockerfile)
+            utils.logger.warning('File %s does not exist! Skipping...', dockerfile)
             continue
 
         fqdn_image = image + ':' + tag
         if container_context is not None:
             build_context = container_context
         elif ctx.obj['container_context']:
             build_context = ctx.obj['container_context']
@@ -411,14 +411,17 @@
             raise click.exceptions.ClickException(f"Couldn't find build image {image} with tag {tag}")
 
     else:
         tagged_image_name = image
         utils.logger.info("No build container tag was provided")
 
     docker_file = utils.image_to_dockerfile(image)
+    if docker_file is None:
+        sys.exit(f'Could not find any dockerfile for {image}')
+
     utils.logger.info("Building image using docker file: %s", docker_file)
     if container_context is not None:
         build_context = container_context
     else:
         build_context = '.'
 
     command = ['build', '--network=host', '-t', tagged_image_name, '-f', docker_file, build_context]
```

### Comparing `strato-skipper-2.0.0/skipper/config.py` & `strato-skipper-2.0.1/skipper/config.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/skipper/data/skipper-complete.sh` & `strato-skipper-2.0.1/skipper/data/skipper-complete.sh`

 * *Files 3% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     for curr_word in "$@"; do
         [[ $curr_word == "$word" ]] && return
     done
 }
 
 
 _get_images_from_dockerfiles() {
-    local dockerfiles=$( ls Dockerfile.* )	
-    for dockerfile in $dockerfiles; do 
-        echo ${dockerfile##*.}; 
+    local dockerfiles=$( find * -type f -regex "\(Docker\|Container\)file\..*" )
+    for dockerfile in $dockerfiles; do
+        echo ${dockerfile##*.};
     done
 }
 
 _get_makefile() {
     local words=( "$@" )
     local makefile
 
@@ -152,15 +152,15 @@
     elif __contains_word "run" ${COMP_WORDS[*]}; then
         COMPREPLY=( $(compgen -W "${OPTS[RUN]}" -- $cur) )
 
     elif __contains_word "make" ${COMP_WORDS[*]}; then
         if [[ $cur == -* ]]; then
             COMPREPLY=( $(compgen -W "${OPTS[RUN]}" -- $cur) )
         else
-            if [[ $prev == -f ]]; then 
+            if [[ $prev == -f ]]; then
                 COMPREPLY=( $(compgen -f -X '!*[mM]akefile' -- $cur) )
             else
                 makefile=$(_get_makefile ${COMP_WORDS[*]})
 
                 # recognise that possible completions are only going to be displayed
                 # so only the base name is shown
                 local mode=--
@@ -168,20 +168,20 @@
                     mode=-d # display-only mode
                 fi
 
                 COMPREPLY=( $( LC_ALL=C make -npq __BASH_MAKE_COMPLETION__=1 -f "$makefile" "." .DEFAULT 2>/dev/null | \
                                command sed -nf <(_make_target_extract_script $mode "$cur") ) )
             fi
         fi
-    
+
     else
         if [[ $cur == -* ]]; then
             COMPREPLY=( $(compgen -W "${OPTS[GLOBAL]}" -- $cur) )
         else
-            COMPREPLY=( $(compgen -W "$COMMANDS" -- $cur) ) 
+            COMPREPLY=( $(compgen -W "$COMMANDS" -- $cur) )
         fi
     fi
 
     return 0
 }
 
 complete -F _skipper_completion skipper;
```

### Comparing `strato-skipper-2.0.0/skipper/data/skipper-entrypoint.sh` & `strato-skipper-2.0.1/skipper/data/skipper-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/skipper/git.py` & `strato-skipper-2.0.1/skipper/git.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/skipper/main.py` & `strato-skipper-2.0.1/skipper/main.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/skipper/runner.py` & `strato-skipper-2.0.1/skipper/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
     if utils.get_runtime_command() == "docker":
         try:
             docker_gid = grp.getgrnam('docker').gr_gid
             cmd += ['-e', f'SKIPPER_DOCKER_GID={docker_gid}']
         except KeyError:
             pass
 
+    if utils.get_runtime_command() == "podman":
+        cmd += ['--group-add', 'keep-groups']
+
     if use_cache:
         cmd += ['-e', 'SKIPPER_USE_CACHE_IMAGE=True']
 
     cmd = handle_volumes_bind_mount(cmd, homedir, volumes, workspace)
 
     cmd = handle_workdir(cmd, cwd, workdir)
```

### Comparing `strato-skipper-2.0.0/skipper/utils.py` & `strato-skipper-2.0.1/skipper/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -138,24 +138,34 @@
         fqdn_image = registry + '/' + fqdn_image
     if tag is not None:
         fqdn_image = fqdn_image + ':' + tag
     return fqdn_image
 
 
 def image_to_dockerfile(image):
-    return 'Dockerfile.' + image
+    prefixes = ['Docker', 'Container']
+    docker_files = [file for file in [prefix + "file." + image for prefix in prefixes] if os.path.exists(file)]
+    if len(docker_files) > 1:
+        logger.warning('Found more than one dockerfile for %s. Using %s', image, docker_files[0])
+    return docker_files[0] if len(docker_files) else None
 
 
 def dockerfile_to_image(dockerfile):
-    return dockerfile.replace('Dockerfile.', '')
+    return dockerfile.split('.', 1)[-1]
 
 
 def is_tool(name):
     """Check whether `name` is on PATH and marked as executable."""
-    return which(name) is not None
+    full_path = which(name)
+    if full_path is None:
+        return False
+    if not os.path.islink(full_path):
+        return True
+    actual_path = os.readlink(full_path)
+    return os.path.basename(actual_path) == name
 
 
 def get_runtime_command():
     global CONTAINER_RUNTIME_COMMAND  # pylint: disable=global-statement
     if not CONTAINER_RUNTIME_COMMAND:
         if is_tool(DOCKER):
             CONTAINER_RUNTIME_COMMAND = DOCKER
```

### Comparing `strato-skipper-2.0.0/strato_skipper.egg-info/PKG-INFO` & `strato-skipper-2.0.1/strato_skipper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strato-skipper
-Version: 2.0.0
+Version: 2.0.1
 Summary: Easily dockerize your Git repository
 Home-page: http://github.com/Stratoscale/skipper
 Author: Adir Gabai
 Author-email: adir@stratoscale.com
 License: Apache-2
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `strato-skipper-2.0.0/strato_skipper.egg-info/SOURCES.txt` & `strato-skipper-2.0.1/strato_skipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/tests/test_cli.py` & `strato-skipper-2.0.1/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1389,14 +1389,15 @@
         expected_fqdn_image = 'build-container-image:build-container-tag'
         skipper_runner_run_mock.assert_called_once_with(command, fqdn_image=expected_fqdn_image, environment=[],
                                                         interactive=True, name=None, net=None, publish=(), volumes=None,
                                                         workdir=None, workspace=None, use_cache=False,
                                                         env_file=())
 
     @mock.patch('subprocess.check_output', mock.MagicMock(autospec=True, return_value=''))
+    @mock.patch('skipper.utils.image_to_dockerfile', mock.MagicMock(autospec=True, side_effect=lambda x: 'Dockerfile.'+x))
     @mock.patch('skipper.runner.run', autospec=True, return_value=0)
     def test_run_without_build_container_tag(self, skipper_runner_run_mock):
         global_params = self.global_params[:-2]
         command = ['ls', '-l']
         run_params = command
         self._invoke_cli(
             global_params=global_params,
@@ -1410,14 +1411,15 @@
             mock.call(command, fqdn_image='build-container-image', environment=[],
                       interactive=False, name=None, net=None, publish=(), volumes=None, workdir=None, workspace=None,
                       use_cache=False, env_file=()),
         ]
         skipper_runner_run_mock.assert_has_calls(expected_commands)
 
     @mock.patch('subprocess.check_output', mock.MagicMock(autospec=True, return_value=''))
+    @mock.patch('skipper.utils.image_to_dockerfile', mock.MagicMock(autospec=True, side_effect=lambda x: 'Dockerfile.'+x))
     @mock.patch('skipper.runner.run', autospec=True, return_value=0)
     def test_run_without_build_container_tag_cached(self, skipper_runner_run_mock):
         global_params = self.global_params[:-2]
         command = ['ls', '-l']
         run_params = ['--cache'] + command
         self._invoke_cli(
             global_params=global_params,
@@ -1792,14 +1794,15 @@
                                                         environment=[],
                                                         interactive=False, name=None, net=None, publish=(),
                                                         volumes=None,
                                                         workdir=None, workspace=None, use_cache=False,
                                                         env_file=())
 
     @mock.patch('subprocess.check_output', mock.MagicMock(autospec=True, return_value=''))
+    @mock.patch('skipper.utils.image_to_dockerfile', mock.MagicMock(autospec=True, side_effect=lambda x: 'Dockerfile.'+x))
     @mock.patch('skipper.runner.run', autospec=True, return_value=0)
     def test_make_without_build_container_tag(self, skipper_runner_run_mock):
         global_params = self.global_params[:-2]
         makefile = 'Makefile'
         target = 'all'
         make_params = ['-f', makefile, target]
         self._invoke_cli(
```

### Comparing `strato-skipper-2.0.0/tests/test_git.py` & `strato-skipper-2.0.1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/tests/test_runner.py` & `strato-skipper-2.0.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.0.0/tests/test_runner_podman.py` & `strato-skipper-2.0.1/tests/test_runner_podman.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             '--ulimit', 'nofile=65536:65536',
             '--privileged',
             '--net', get_default_net(),
             '-e', 'SKIPPER_USERNAME=testuser',
             '-e', 'SKIPPER_UID=%(user_uid)s' % dict(user_uid=USER_ID),
             '-e', 'HOME=%(homedir)s' % dict(homedir=HOME_DIR),
             '-e', 'CONTAINER_RUNTIME_COMMAND=%(runtime_command)s' % dict(runtime_command=utils.get_runtime_command()),
+            '--group-add', 'keep-groups',
             '-v', get_volume_mapping('%(homedir)s/.netrc:%(homedir)s/.netrc:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.gitconfig:%(homedir)s/.gitconfig:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.docker/config.json:%(homedir)s/.docker/config.json:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('/etc/docker:/etc/docker:ro'),
             '-v', get_volume_mapping('%(workdir)s:%(workdir)s:rw' % dict(workdir=WORKDIR)),
             '-v', get_volume_mapping('entrypoint.sh:/opt/skipper/skipper-entrypoint.sh:rw'),
             '-v', get_volume_mapping('/var/run/docker.sock:/var/run/docker.sock:rw'),
@@ -119,14 +120,15 @@
             '--ulimit', 'nofile=65536:65536',
             '--privileged',
             '--net', get_default_net(),
             '-e', 'SKIPPER_USERNAME=testuser',
             '-e', 'SKIPPER_UID=%(user_uid)s' % dict(user_uid=USER_ID),
             '-e', 'HOME=%(homedir)s' % dict(homedir=HOME_DIR),
             '-e', 'CONTAINER_RUNTIME_COMMAND=%(runtime_command)s' % dict(runtime_command=utils.get_runtime_command()),
+            '--group-add', 'keep-groups',
             '-v', get_volume_mapping('%(homedir)s/.netrc:%(homedir)s/.netrc:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.gitconfig:%(homedir)s/.gitconfig:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.docker/config.json:%(homedir)s/.docker/config.json:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('/etc/docker:/etc/docker:ro'),
             '-v', get_volume_mapping('%(workdir)s:%(workdir)s:rw' % dict(workdir=WORKDIR)),
             '-v', get_volume_mapping('entrypoint.sh:/opt/skipper/skipper-entrypoint.sh:rw'),
             '-v', get_volume_mapping('/var/run/docker.sock:/var/run/docker.sock:rw'),
@@ -160,14 +162,15 @@
             '--ulimit', 'nofile=65536:65536',
             '--privileged',
             '--net', get_default_net(),
             '-e', 'SKIPPER_USERNAME=testuser',
             '-e', 'SKIPPER_UID=%(user_uid)s' % dict(user_uid=USER_ID),
             '-e', 'HOME=%(homedir)s' % dict(homedir=HOME_DIR),
             '-e', 'CONTAINER_RUNTIME_COMMAND=%(runtime_command)s' % dict(runtime_command=utils.get_runtime_command()),
+            '--group-add', 'keep-groups',
             '-v', get_volume_mapping('%(homedir)s/.netrc:%(homedir)s/.netrc:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.gitconfig:%(homedir)s/.gitconfig:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.docker/config.json:%(homedir)s/.docker/config.json:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('/etc/docker:/etc/docker:ro'),
             '-v', get_volume_mapping('%(workdir)s:%(workdir)s:rw' % dict(workdir=WORKDIR)),
             '-v', get_volume_mapping('entrypoint.sh:/opt/skipper/skipper-entrypoint.sh:rw'),
             '-v', get_volume_mapping('/var/run/docker.sock:/var/run/docker.sock:rw'),
@@ -205,14 +208,15 @@
             '--ulimit', 'nofile=65536:65536',
             '--privileged',
             '--net', get_default_net(),
             '-e', 'SKIPPER_USERNAME=testuser',
             '-e', 'SKIPPER_UID=%(user_uid)s' % dict(user_uid=USER_ID),
             '-e', 'HOME=%(homedir)s' % dict(homedir=HOME_DIR),
             '-e', 'CONTAINER_RUNTIME_COMMAND=%(runtime_command)s' % dict(runtime_command=utils.get_runtime_command()),
+            '--group-add', 'keep-groups',
             '-v', get_volume_mapping('%(homedir)s/.netrc:%(homedir)s/.netrc:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.gitconfig:%(homedir)s/.gitconfig:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.docker/config.json:%(homedir)s/.docker/config.json:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('/etc/docker:/etc/docker:ro'),
             '-v', get_volume_mapping('%(workdir)s:%(workdir)s:rw' % dict(workdir=WORKDIR)),
             '-v', get_volume_mapping('entrypoint.sh:/opt/skipper/skipper-entrypoint.sh:rw'),
             '-v', get_volume_mapping('/var/run/docker.sock:/var/run/docker.sock:rw'),
@@ -248,14 +252,15 @@
             '--net', get_default_net(),
             '-e', 'KEY1=VAL1',
             '-e', 'KEY2=VAL2',
             '-e', 'SKIPPER_USERNAME=testuser',
             '-e', 'SKIPPER_UID=%(user_uid)s' % dict(user_uid=USER_ID),
             '-e', 'HOME=%(homedir)s' % dict(homedir=HOME_DIR),
             '-e', 'CONTAINER_RUNTIME_COMMAND=%(runtime_command)s' % dict(runtime_command=utils.get_runtime_command()),
+            '--group-add', 'keep-groups',
             '-v', get_volume_mapping('%(homedir)s/.netrc:%(homedir)s/.netrc:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.gitconfig:%(homedir)s/.gitconfig:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('%(homedir)s/.docker/config.json:%(homedir)s/.docker/config.json:ro' % dict(homedir=HOME_DIR)),
             '-v', get_volume_mapping('/etc/docker:/etc/docker:ro'),
             '-v', get_volume_mapping('%(workdir)s:%(workdir)s:rw' % dict(workdir=WORKDIR)),
             '-v', get_volume_mapping('entrypoint.sh:/opt/skipper/skipper-entrypoint.sh:rw'),
             '-v', get_volume_mapping('/var/run/docker.sock:/var/run/docker.sock:rw'),
```

### Comparing `strato-skipper-2.0.0/tests/test_utils.py` & `strato-skipper-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

