# Comparing `tmp/docker-6.1.1.tar.gz` & `tmp/docker-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-6.1.1.tar", last modified: Sun May  7 23:54:11 2023, max compression
+gzip compressed data, was "docker-6.1.2.tar", last modified: Thu May 11 19:36:54 2023, max compression
```

## Comparing `docker-6.1.1.tar` & `docker-6.1.2.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.693834 docker-6.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-07 23:54:04.000000 docker-6.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 23:54:04.000000 docker-6.1.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-07 23:54:04.000000 docker-6.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-07 23:54:04.000000 docker-6.1.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-07 23:54:04.000000 docker-6.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 23:54:04.000000 docker-6.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-07 23:54:04.000000 docker-6.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-07 23:54:04.000000 docker-6.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-07 23:54:04.000000 docker-6.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-07 23:54:04.000000 docker-6.1.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-07 23:54:04.000000 docker-6.1.1/Dockerfile-docs
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-07 23:54:04.000000 docker-6.1.1/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-07 23:54:04.000000 docker-6.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-07 23:54:04.000000 docker-6.1.1/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 23:54:04.000000 docker-6.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-07 23:54:04.000000 docker-6.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-07 23:54:11.693834 docker-6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-07 23:54:04.000000 docker-6.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 23:54:04.000000 docker-6.1.1/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 23:54:11.000000 docker-6.1.1/docker/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/api/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    52534 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/exec_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-07 23:54:04.000000 docker-6.1.1/docker/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-07 23:54:04.000000 docker-6.1.1/docker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-07 23:54:04.000000 docker-6.1.1/docker/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/context/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-07 23:54:04.000000 docker-6.1.1/docker/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46077 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-07 23:54:04.000000 docker-6.1.1/docker/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/basehttpadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/npipeconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/npipesocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/sshconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/ssladapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/unixconn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docker/types/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    33158 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/swarm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/fnmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-07 23:54:04.000000 docker-6.1.1/docker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-07 23:54:04.000000 docker-6.1.1/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 23:54:04.000000 docker-6.1.1/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-07 23:54:04.000000 docker-6.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    75067 2023-05-07 23:54:04.000000 docker-6.1.1/docs/change-log.md
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-07 23:54:04.000000 docker-6.1.1/docs/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-07 23:54:04.000000 docker-6.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-07 23:54:04.000000 docker-6.1.1/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-07 23:54:04.000000 docker-6.1.1/docs/containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-07 23:54:04.000000 docker-6.1.1/docs/favicon_whale.png
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-07 23:54:04.000000 docker-6.1.1/docs/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-07 23:54:04.000000 docker-6.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-07 23:54:04.000000 docker-6.1.1/docs/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-07 23:54:04.000000 docker-6.1.1/docs/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-07 23:54:04.000000 docker-6.1.1/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-07 23:54:04.000000 docker-6.1.1/docs/secrets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-07 23:54:04.000000 docker-6.1.1/docs/services.rst
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 23:54:04.000000 docker-6.1.1/docs/swarm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-07 23:54:04.000000 docker-6.1.1/docs/tls.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/user_guides/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-07 23:54:04.000000 docker-6.1.1/docs/user_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-07 23:54:04.000000 docker-6.1.1/docs/user_guides/multiplex.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-07 23:54:04.000000 docker-6.1.1/docs/user_guides/swarm_services.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-07 23:54:04.000000 docker-6.1.1/docs/volumes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 23:54:04.000000 docker-6.1.1/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-07 23:54:04.000000 docker-6.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 23:54:04.000000 docker-6.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-07 23:54:04.000000 docker-6.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-05-07 23:54:04.000000 docker-6.1.1/scripts/release.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2186 2023-05-07 23:54:04.000000 docker-6.1.1/scripts/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 23:54:11.693834 docker-6.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-07 23:54:04.000000 docker-6.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 23:54:04.000000 docker-6.1.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-07 23:54:04.000000 docker-6.1.1/tests/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-07 23:54:04.000000 docker-6.1.1/tests/Dockerfile-dind-certs
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 23:54:04.000000 docker-6.1.1/tests/Dockerfile-ssh-dind
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/gpg-keys/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-07 23:54:04.000000 docker-6.1.1/tests/gpg-keys/ownertrust
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 23:54:04.000000 docker-6.1.1/tests/gpg-keys/secret
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-07 23:54:04.000000 docker-6.1.1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    56459 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_healthcheck_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18933 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_secret_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    62334 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/context_api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/integration/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/create_gpg_key.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/store_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_nodes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_volumes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/regression_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/integration/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/integration/testdata/dummy-plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/testdata/dummy-plugin/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/integration/testdata/dummy-plugin/rootfs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/integration/testdata/dummy-plugin/rootfs/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/ssh/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/ssh/config/client/
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/client/id_rsa
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/client/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/ssh/config/server/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/known_ed25519
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/known_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/sshd_config
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/unknown_ed25519
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/unknown_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/connect_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.693834 docker-6.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    59084 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28287 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/context_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/dockertypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/fake_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/fake_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/fake_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    24231 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_secrets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/sshadapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/ssladapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/swarm_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/unit/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.693834 docker-6.1.1/tests/unit/testdata/certs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/testdata/certs/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/testdata/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/testdata/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/types_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16046 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_json_stream_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23196 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-07 23:54:04.000000 docker-6.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.036477 docker-6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 19:36:47.000000 docker-6.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 19:36:47.000000 docker-6.1.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 19:36:47.000000 docker-6.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.016477 docker-6.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-11 19:36:47.000000 docker-6.1.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.016477 docker-6.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-11 19:36:47.000000 docker-6.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-11 19:36:47.000000 docker-6.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 19:36:47.000000 docker-6.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 19:36:47.000000 docker-6.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-11 19:36:47.000000 docker-6.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 19:36:47.000000 docker-6.1.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-11 19:36:47.000000 docker-6.1.2/Dockerfile-docs
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-11 19:36:47.000000 docker-6.1.2/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-11 19:36:47.000000 docker-6.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-11 19:36:47.000000 docker-6.1.2/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 19:36:47.000000 docker-6.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-11 19:36:47.000000 docker-6.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-11 19:36:54.036477 docker-6.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-11 19:36:47.000000 docker-6.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.016477 docker-6.1.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 19:36:47.000000 docker-6.1.2/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 19:36:53.000000 docker-6.1.2/docker/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.016477 docker-6.1.2/docker/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52534 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/exec_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-11 19:36:47.000000 docker-6.1.2/docker/api/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-11 19:36:47.000000 docker-6.1.2/docker/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-11 19:36:47.000000 docker-6.1.2/docker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-11 19:36:47.000000 docker-6.1.2/docker/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.016477 docker-6.1.2/docker/context/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 19:36:47.000000 docker-6.1.2/docker/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-11 19:36:47.000000 docker-6.1.2/docker/context/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-11 19:36:47.000000 docker-6.1.2/docker/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-11 19:36:47.000000 docker-6.1.2/docker/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.020477 docker-6.1.2/docker/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 19:36:47.000000 docker-6.1.2/docker/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-11 19:36:47.000000 docker-6.1.2/docker/credentials/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 19:36:47.000000 docker-6.1.2/docker/credentials/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-11 19:36:47.000000 docker-6.1.2/docker/credentials/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 19:36:47.000000 docker-6.1.2/docker/credentials/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-11 19:36:47.000000 docker-6.1.2/docker/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.020477 docker-6.1.2/docker/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46077 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-11 19:36:47.000000 docker-6.1.2/docker/models/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-11 19:36:47.000000 docker-6.1.2/docker/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.020477 docker-6.1.2/docker/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 19:36:47.000000 docker-6.1.2/docker/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 19:36:47.000000 docker-6.1.2/docker/transport/basehttpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-11 19:36:47.000000 docker-6.1.2/docker/transport/npipeconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-11 19:36:47.000000 docker-6.1.2/docker/transport/npipesocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-11 19:36:47.000000 docker-6.1.2/docker/transport/sshconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-11 19:36:47.000000 docker-6.1.2/docker/transport/ssladapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-11 19:36:47.000000 docker-6.1.2/docker/transport/unixconn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.020477 docker-6.1.2/docker/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33158 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-11 19:36:47.000000 docker-6.1.2/docker/types/swarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/fnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-05-11 19:36:47.000000 docker-6.1.2/docker/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 19:36:47.000000 docker-6.1.2/docker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.016477 docker-6.1.2/docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-11 19:36:53.000000 docker-6.1.2/docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-11 19:36:54.000000 docker-6.1.2/docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:36:53.000000 docker-6.1.2/docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:36:53.000000 docker-6.1.2/docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-11 19:36:53.000000 docker-6.1.2/docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 19:36:53.000000 docker-6.1.2/docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-11 19:36:47.000000 docker-6.1.2/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 19:36:47.000000 docker-6.1.2/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-11 19:36:47.000000 docker-6.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    76114 2023-05-11 19:36:47.000000 docker-6.1.2/docs/change-log.md
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-11 19:36:47.000000 docker-6.1.2/docs/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-11 19:36:47.000000 docker-6.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-11 19:36:47.000000 docker-6.1.2/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-11 19:36:47.000000 docker-6.1.2/docs/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-11 19:36:47.000000 docker-6.1.2/docs/favicon_whale.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-11 19:36:47.000000 docker-6.1.2/docs/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-11 19:36:47.000000 docker-6.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-11 19:36:47.000000 docker-6.1.2/docs/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-11 19:36:47.000000 docker-6.1.2/docs/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 19:36:47.000000 docker-6.1.2/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-11 19:36:47.000000 docker-6.1.2/docs/secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-11 19:36:47.000000 docker-6.1.2/docs/services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 19:36:47.000000 docker-6.1.2/docs/swarm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-11 19:36:47.000000 docker-6.1.2/docs/tls.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/docs/user_guides/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 19:36:47.000000 docker-6.1.2/docs/user_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-11 19:36:47.000000 docker-6.1.2/docs/user_guides/multiplex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-11 19:36:47.000000 docker-6.1.2/docs/user_guides/swarm_services.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-11 19:36:47.000000 docker-6.1.2/docs/volumes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 19:36:47.000000 docker-6.1.2/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 19:36:47.000000 docker-6.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 19:36:47.000000 docker-6.1.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 19:36:47.000000 docker-6.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-05-11 19:36:47.000000 docker-6.1.2/scripts/release.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2186 2023-05-11 19:36:47.000000 docker-6.1.2/scripts/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 19:36:54.036477 docker-6.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-11 19:36:47.000000 docker-6.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 19:36:47.000000 docker-6.1.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-11 19:36:47.000000 docker-6.1.2/tests/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-11 19:36:47.000000 docker-6.1.2/tests/Dockerfile-dind-certs
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 19:36:47.000000 docker-6.1.2/tests/Dockerfile-ssh-dind
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.024477 docker-6.1.2/tests/gpg-keys/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-11 19:36:47.000000 docker-6.1.2/tests/gpg-keys/ownertrust
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-11 19:36:47.000000 docker-6.1.2/tests/gpg-keys/secret
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-11 19:36:47.000000 docker-6.1.2/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.028477 docker-6.1.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56459 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_healthcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18933 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_secret_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62334 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/context_api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.028477 docker-6.1.2/tests/integration/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/credentials/create_gpg_key.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/credentials/store_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/credentials/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_nodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/models_volumes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/regression_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.012477 docker-6.1.2/tests/integration/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.028477 docker-6.1.2/tests/integration/testdata/dummy-plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/testdata/dummy-plugin/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.012477 docker-6.1.2/tests/integration/testdata/dummy-plugin/rootfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.028477 docker-6.1.2/tests/integration/testdata/dummy-plugin/rootfs/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.028477 docker-6.1.2/tests/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.012477 docker-6.1.2/tests/ssh/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.028477 docker-6.1.2/tests/ssh/config/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/config/client/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/config/client/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.032477 docker-6.1.2/tests/ssh/config/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/config/server/known_ed25519
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/config/server/known_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/config/server/sshd_config
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/config/server/unknown_ed25519
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/config/server/unknown_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-11 19:36:47.000000 docker-6.1.2/tests/ssh/connect_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.032477 docker-6.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59084 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28287 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/dockertypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/fake_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/fake_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/fake_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24231 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/models_secrets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/sshadapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/ssladapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/swarm_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.012477 docker-6.1.2/tests/unit/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:54.032477 docker-6.1.2/tests/unit/testdata/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/testdata/certs/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/testdata/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/testdata/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/types_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16046 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/utils_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/utils_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/utils_json_stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/utils_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23196 2023-05-11 19:36:47.000000 docker-6.1.2/tests/unit/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-11 19:36:47.000000 docker-6.1.2/tox.ini
```

### Comparing `docker-6.1.1/.github/workflows/ci.yml` & `docker-6.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/.github/workflows/release.yml` & `docker-6.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/CONTRIBUTING.md` & `docker-6.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/Jenkinsfile` & `docker-6.1.2/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/LICENSE` & `docker-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/MAINTAINERS` & `docker-6.1.2/MAINTAINERS`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/Makefile` & `docker-6.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/PKG-INFO` & `docker-6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 6.1.1
+Version: 6.1.2
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-6.1.1/README.md` & `docker-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/build.py` & `docker-6.1.2/docker/api/build.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/client.py` & `docker-6.1.2/docker/api/client.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/config.py` & `docker-6.1.2/docker/api/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/container.py` & `docker-6.1.2/docker/api/container.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/daemon.py` & `docker-6.1.2/docker/api/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/exec_api.py` & `docker-6.1.2/docker/api/exec_api.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/image.py` & `docker-6.1.2/docker/api/image.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/network.py` & `docker-6.1.2/docker/api/network.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/plugin.py` & `docker-6.1.2/docker/api/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/secret.py` & `docker-6.1.2/docker/api/secret.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/service.py` & `docker-6.1.2/docker/api/service.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/swarm.py` & `docker-6.1.2/docker/api/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/api/volume.py` & `docker-6.1.2/docker/api/volume.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/auth.py` & `docker-6.1.2/docker/auth.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/client.py` & `docker-6.1.2/docker/client.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/constants.py` & `docker-6.1.2/docker/constants.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/context/api.py` & `docker-6.1.2/docker/context/api.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/context/config.py` & `docker-6.1.2/docker/context/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/context/context.py` & `docker-6.1.2/docker/context/context.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/credentials/errors.py` & `docker-6.1.2/docker/credentials/errors.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/credentials/store.py` & `docker-6.1.2/docker/credentials/store.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/errors.py` & `docker-6.1.2/docker/errors.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/configs.py` & `docker-6.1.2/docker/models/configs.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/containers.py` & `docker-6.1.2/docker/models/containers.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/images.py` & `docker-6.1.2/docker/models/images.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/networks.py` & `docker-6.1.2/docker/models/networks.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/nodes.py` & `docker-6.1.2/docker/models/nodes.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/plugins.py` & `docker-6.1.2/docker/models/plugins.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/resource.py` & `docker-6.1.2/docker/models/resource.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/secrets.py` & `docker-6.1.2/docker/models/secrets.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/services.py` & `docker-6.1.2/docker/models/services.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/swarm.py` & `docker-6.1.2/docker/models/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/models/volumes.py` & `docker-6.1.2/docker/models/volumes.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/tls.py` & `docker-6.1.2/docker/tls.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/transport/npipeconn.py` & `docker-6.1.2/docker/transport/npipeconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/transport/npipesocket.py` & `docker-6.1.2/docker/transport/npipesocket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import functools
 import time
 import io
 
 import win32file
 import win32pipe
+import pywintypes
+import win32event
+import win32api
 
 cERROR_PIPE_BUSY = 0xe7
 cSECURITY_SQOS_PRESENT = 0x100000
 cSECURITY_ANONYMOUS = 0
 
 MAXIMUM_RETRY_COUNT = 10
 
@@ -50,15 +53,17 @@
         try:
             handle = win32file.CreateFile(
                 address,
                 win32file.GENERIC_READ | win32file.GENERIC_WRITE,
                 0,
                 None,
                 win32file.OPEN_EXISTING,
-                cSECURITY_ANONYMOUS | cSECURITY_SQOS_PRESENT,
+                (cSECURITY_ANONYMOUS
+                    | cSECURITY_SQOS_PRESENT
+                    | win32file.FILE_FLAG_OVERLAPPED),
                 0
             )
         except win32pipe.error as e:
             # See Remarks:
             # https://msdn.microsoft.com/en-us/library/aa365800.aspx
             if e.winerror == cERROR_PIPE_BUSY:
                 # Another program or thread has grabbed our pipe instance
@@ -127,30 +132,45 @@
 
     @check_closed
     def recv_into(self, buf, nbytes=0):
         readbuf = buf
         if not isinstance(buf, memoryview):
             readbuf = memoryview(buf)
 
-        err, data = win32file.ReadFile(
-            self._handle,
-            readbuf[:nbytes] if nbytes else readbuf
-        )
-        return len(data)
-
-    def _recv_into_py2(self, buf, nbytes):
-        err, data = win32file.ReadFile(self._handle, nbytes or len(buf))
-        n = len(data)
-        buf[:n] = data
-        return n
+        event = win32event.CreateEvent(None, True, True, None)
+        try:
+            overlapped = pywintypes.OVERLAPPED()
+            overlapped.hEvent = event
+            err, data = win32file.ReadFile(
+                self._handle,
+                readbuf[:nbytes] if nbytes else readbuf,
+                overlapped
+            )
+            wait_result = win32event.WaitForSingleObject(event, self._timeout)
+            if wait_result == win32event.WAIT_TIMEOUT:
+                win32file.CancelIo(self._handle)
+                raise TimeoutError
+            return win32file.GetOverlappedResult(self._handle, overlapped, 0)
+        finally:
+            win32api.CloseHandle(event)
 
     @check_closed
     def send(self, string, flags=0):
-        err, nbytes = win32file.WriteFile(self._handle, string)
-        return nbytes
+        event = win32event.CreateEvent(None, True, True, None)
+        try:
+            overlapped = pywintypes.OVERLAPPED()
+            overlapped.hEvent = event
+            win32file.WriteFile(self._handle, string, overlapped)
+            wait_result = win32event.WaitForSingleObject(event, self._timeout)
+            if wait_result == win32event.WAIT_TIMEOUT:
+                win32file.CancelIo(self._handle)
+                raise TimeoutError
+            return win32file.GetOverlappedResult(self._handle, overlapped, 0)
+        finally:
+            win32api.CloseHandle(event)
 
     @check_closed
     def sendall(self, string, flags=0):
         return self.send(string, flags)
 
     @check_closed
     def sendto(self, string, address):
@@ -161,23 +181,20 @@
         if flag:
             return self.settimeout(None)
         return self.settimeout(0)
 
     def settimeout(self, value):
         if value is None:
             # Blocking mode
-            self._timeout = win32pipe.NMPWAIT_WAIT_FOREVER
+            self._timeout = win32event.INFINITE
         elif not isinstance(value, (float, int)) or value < 0:
             raise ValueError('Timeout value out of range')
-        elif value == 0:
-            # Non-blocking mode
-            self._timeout = win32pipe.NMPWAIT_NO_WAIT
         else:
             # Timeout mode - Value converted to milliseconds
-            self._timeout = value * 1000
+            self._timeout = int(value * 1000)
 
     def gettimeout(self):
         return self._timeout
 
     def setsockopt(self, level, optname, value):
         raise NotImplementedError()
```

### Comparing `docker-6.1.1/docker/transport/sshconn.py` & `docker-6.1.2/docker/transport/sshconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/transport/ssladapter.py` & `docker-6.1.2/docker/transport/ssladapter.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/transport/unixconn.py` & `docker-6.1.2/docker/transport/unixconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/types/__init__.py` & `docker-6.1.2/docker/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/types/containers.py` & `docker-6.1.2/docker/types/containers.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/types/daemon.py` & `docker-6.1.2/docker/types/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/types/healthcheck.py` & `docker-6.1.2/docker/types/healthcheck.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/types/networks.py` & `docker-6.1.2/docker/types/networks.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/types/services.py` & `docker-6.1.2/docker/types/services.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/types/swarm.py` & `docker-6.1.2/docker/types/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/__init__.py` & `docker-6.1.2/docker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/build.py` & `docker-6.1.2/docker/utils/build.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/config.py` & `docker-6.1.2/docker/utils/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/decorators.py` & `docker-6.1.2/docker/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/fnmatch.py` & `docker-6.1.2/docker/utils/fnmatch.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/json_stream.py` & `docker-6.1.2/docker/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/ports.py` & `docker-6.1.2/docker/utils/ports.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/proxy.py` & `docker-6.1.2/docker/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/utils/socket.py` & `docker-6.1.2/docker/utils/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     if not isinstance(socket, NpipeSocket):
         if sys.platform == 'win32':
             # Limited to 1024
             select.select([socket], [], [])
         else:
             poll = select.poll()
-            poll.register(socket)
+            poll.register(socket, select.POLLIN | select.POLLPRI)
             poll.poll()
 
     try:
         if hasattr(socket, 'recv'):
             return socket.recv(n)
         if isinstance(socket, getattr(pysocket, 'SocketIO')):
             return socket.read(n)
```

### Comparing `docker-6.1.1/docker/utils/utils.py` & `docker-6.1.2/docker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker/version.py` & `docker-6.1.2/docker/version.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docker.egg-info/PKG-INFO` & `docker-6.1.2/docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 6.1.1
+Version: 6.1.2
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-6.1.1/docker.egg-info/SOURCES.txt` & `docker-6.1.2/docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/api.rst` & `docker-6.1.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/change-log.md` & `docker-6.1.2/docs/change-log.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,4692 +1,4758 @@
 00000000: 4368 616e 6765 6c6f 670a 3d3d 3d3d 3d3d  Changelog.======
-00000010: 3d3d 3d3d 0a0a 362e 302e 300a 2d2d 2d2d  ====..6.0.0.----
-00000020: 2d0a 0a23 2323 2055 7067 7261 6465 204e  -..### Upgrade N
-00000030: 6f74 6573 0a2d 204d 696e 696d 756d 2073  otes.- Minimum s
-00000040: 7570 706f 7274 6564 2050 7974 686f 6e20  upported Python 
-00000050: 7665 7273 696f 6e20 6973 2033 2e37 2b0a  version is 3.7+.
-00000060: 2d20 5768 656e 2069 6e73 7461 6c6c 696e  - When installin
-00000070: 6720 7769 7468 2070 6970 2c20 7468 6520  g with pip, the 
-00000080: 6064 6f63 6b65 725b 746c 735d 6020 6578  `docker[tls]` ex
-00000090: 7472 6120 6973 2064 6570 7265 6361 7465  tra is deprecate
-000000a0: 6420 616e 6420 6120 6e6f 2d6f 702c 0a20  d and a no-op,. 
-000000b0: 2075 7365 2060 646f 636b 6572 6020 666f   use `docker` fo
-000000c0: 7220 7361 6d65 2066 756e 6374 696f 6e61  r same functiona
-000000d0: 6c69 7479 2028 544c 5320 7375 7070 6f72  lity (TLS suppor
-000000e0: 7420 6973 2061 6c77 6179 7320 6176 6169  t is always avai
-000000f0: 6c61 626c 6520 6e6f 7729 0a2d 204e 6174  lable now).- Nat
-00000100: 6976 6520 5079 7468 6f6e 2053 5348 2063  ive Python SSH c
-00000110: 6c69 656e 7420 2875 7365 6420 6279 2064  lient (used by d
-00000120: 6566 6175 6c74 202f 2060 7573 655f 7373  efault / `use_ss
-00000130: 685f 636c 6965 6e74 3d46 616c 7365 6029  h_client=False`)
-00000140: 2077 696c 6c20 6e6f 770a 2020 7265 6a65   will now.  reje
-00000150: 6374 2075 6e6b 6e6f 776e 2068 6f73 7420  ct unknown host 
-00000160: 6b65 7973 2077 6974 6820 6070 6172 616d  keys with `param
-00000170: 696b 6f2e 7373 685f 6578 6365 7074 696f  iko.ssh_exceptio
-00000180: 6e2e 5353 4845 7863 6570 7469 6f6e 600a  n.SSHException`.
-00000190: 2d20 5368 6f72 7420 4944 7320 6172 6520  - Short IDs are 
-000001a0: 6e6f 7720 3132 2063 6861 7261 6374 6572  now 12 character
-000001b0: 7320 696e 7374 6561 6420 6f66 2031 3020  s instead of 10 
-000001c0: 6368 6172 6163 7465 7273 2028 7361 6d65  characters (same
-000001d0: 2061 7320 446f 636b 6572 2043 4c49 290a   as Docker CLI).
-000001e0: 0a23 2323 2046 6561 7475 7265 730a 2d20  .### Features.- 
-000001f0: 5079 7468 6f6e 2033 2e31 3020 7375 7070  Python 3.10 supp
-00000200: 6f72 740a 2d20 4175 746f 6d61 7469 6361  ort.- Automatica
-00000210: 6c6c 7920 6e65 676f 7469 6174 6520 6d6f  lly negotiate mo
-00000220: 7374 2073 6563 7572 6520 544c 5320 7665  st secure TLS ve
-00000230: 7273 696f 6e0a 2d20 4164 6420 6070 6c61  rsion.- Add `pla
-00000240: 7466 6f72 6d60 2028 652e 672e 2060 6c69  tform` (e.g. `li
-00000250: 6e75 782f 616d 6436 3460 2c20 6064 6172  nux/amd64`, `dar
-00000260: 7769 6e2f 6172 6d36 3460 2920 746f 2063  win/arm64`) to c
-00000270: 6f6e 7461 696e 6572 2063 7265 6174 6520  ontainer create 
-00000280: 2620 7275 6e0a 2d20 4164 6420 7375 7070  & run.- Add supp
-00000290: 6f72 7420 666f 7220 6047 6c6f 6261 6c4a  ort for `GlobalJ
-000002a0: 6f62 6020 616e 6420 6052 6570 6c69 6361  ob` and `Replica
-000002b0: 7465 644a 6f62 7360 2066 6f72 2053 7761  tedJobs` for Swa
-000002c0: 726d 0a2d 2041 6464 2060 7265 6d6f 7665  rm.- Add `remove
-000002d0: 2829 6020 6d65 7468 6f64 206f 6e20 6049  ()` method on `I
-000002e0: 6d61 6765 600a 2d20 4164 6420 6066 6f72  mage`.- Add `for
-000002f0: 6365 6020 7061 7261 6d20 746f 2060 6469  ce` param to `di
-00000300: 7361 626c 6528 2960 206f 6e20 6050 6c75  sable()` on `Plu
-00000310: 6769 6e60 0a0a 2323 2320 4275 6766 6978  gin`..### Bugfix
-00000320: 6573 0a2d 2046 6978 2069 6e73 7461 6c6c  es.- Fix install
-00000330: 2069 7373 7565 7320 6f6e 2057 696e 646f   issues on Windo
-00000340: 7773 2072 656c 6174 6564 2074 6f20 6070  ws related to `p
-00000350: 7977 696e 3332 600a 2d20 446f 206e 6f74  ywin32`.- Do not
-00000360: 2061 6363 6570 7420 756e 6b6e 6f77 6e20   accept unknown 
-00000370: 5353 4820 686f 7374 206b 6579 7320 696e  SSH host keys in
-00000380: 206e 6174 6976 6520 5079 7468 6f6e 2053   native Python S
-00000390: 5348 206d 6f64 650a 2d20 5573 6520 3132  SH mode.- Use 12
-000003a0: 2063 6861 7261 6374 6572 2073 686f 7274   character short
-000003b0: 2049 4473 2066 6f72 2063 6f6e 7369 7374   IDs for consist
-000003c0: 656e 6379 2077 6974 6820 446f 636b 6572  ency with Docker
-000003d0: 2043 4c49 0a2d 2049 676e 6f72 6520 7472   CLI.- Ignore tr
-000003e0: 6169 6c69 6e67 2077 6869 7465 7370 6163  ailing whitespac
-000003f0: 6520 696e 2060 2e64 6f63 6b65 7269 676e  e in `.dockerign
-00000400: 6f72 6560 2066 696c 6573 0a2d 2046 6978  ore` files.- Fix
-00000410: 2049 5076 3620 686f 7374 2070 6172 7369   IPv6 host parsi
-00000420: 6e67 2077 6865 6e20 6578 706c 6963 6974  ng when explicit
-00000430: 2070 6f72 7420 7370 6563 6966 6965 640a   port specified.
-00000440: 2d20 4669 7820 6050 726f 7879 436f 6d6d  - Fix `ProxyComm
-00000450: 616e 6460 206f 7074 696f 6e20 666f 7220  and` option for 
-00000460: 5353 4820 636f 6e6e 6563 7469 6f6e 730a  SSH connections.
-00000470: 2d20 446f 206e 6f74 2073 7061 776e 2065  - Do not spawn e
-00000480: 7874 7261 2073 7562 7368 656c 6c20 7768  xtra subshell wh
-00000490: 656e 206c 6175 6e63 6869 6e67 2065 7874  en launching ext
-000004a0: 6572 6e61 6c20 5353 4820 636c 6965 6e74  ernal SSH client
-000004b0: 0a2d 2049 6d70 726f 7665 2065 7863 6570  .- Improve excep
-000004c0: 7469 6f6e 2073 656d 616e 7469 6373 2074  tion semantics t
-000004d0: 6f20 7072 6573 6572 7665 2063 6f6e 7465  o preserve conte
-000004e0: 7874 0a2d 2044 6f63 756d 656e 7461 7469  xt.- Documentati
-000004f0: 6f6e 2069 6d70 726f 7665 6d65 6e74 7320  on improvements 
-00000500: 2866 6f72 6d61 7474 696e 672c 2065 7861  (formatting, exa
-00000510: 6d70 6c65 732c 2074 7970 6f73 2c20 6d69  mples, typos, mi
-00000520: 7373 696e 6720 7061 7261 6d73 290a 0a23  ssing params)..#
-00000530: 2323 204d 6973 6365 6c6c 616e 656f 7573  ## Miscellaneous
-00000540: 0a2d 2055 7067 7261 6465 2064 6570 656e  .- Upgrade depen
-00000550: 6465 6e63 6965 7320 696e 2060 7265 7175  dencies in `requ
-00000560: 6972 656d 656e 7473 2e74 7874 6020 746f  irements.txt` to
-00000570: 206c 6174 6573 7420 7665 7273 696f 6e73   latest versions
-00000580: 0a2d 2052 656d 6f76 6520 6578 7472 616e  .- Remove extran
-00000590: 656f 7573 2074 7261 6e73 6974 6976 6520  eous transitive 
-000005a0: 6465 7065 6e64 656e 6369 6573 0a2d 2045  dependencies.- E
-000005b0: 6c69 6d69 6e61 7465 2075 7361 6765 7320  liminate usages 
-000005c0: 6f66 2064 6570 7265 6361 7465 6420 6675  of deprecated fu
-000005d0: 6e63 7469 6f6e 732f 6d65 7468 6f64 730a  nctions/methods.
-000005e0: 2d20 5465 7374 2073 7569 7465 2072 656c  - Test suite rel
-000005f0: 6961 6269 6c69 7479 2069 6d70 726f 7665  iability improve
-00000600: 6d65 6e74 730a 2d20 4769 7448 7562 2041  ments.- GitHub A
-00000610: 6374 696f 6e73 2077 6f72 6b66 6c6f 7773  ctions workflows
-00000620: 2066 6f72 206c 696e 7469 6e67 2c20 756e   for linting, un
-00000630: 6974 2074 6573 7473 2c20 696e 7465 6772  it tests, integr
-00000640: 6174 696f 6e20 7465 7374 732c 2061 6e64  ation tests, and
-00000650: 0a20 2070 7562 6c69 7368 696e 6720 7265  .  publishing re
-00000660: 6c65 6173 6573 0a0a 352e 302e 330a 2d2d  leases..5.0.3.--
-00000670: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
-00000680: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
-00000690: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-000006a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000006b0: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
-000006c0: 2f6d 696c 6573 746f 6e65 2f37 363f 636c  /milestone/76?cl
-000006d0: 6f73 6564 3d31 290a 0a23 2323 2046 6561  osed=1)..### Fea
-000006e0: 7475 7265 730a 2d20 4164 6420 6063 6170  tures.- Add `cap
-000006f0: 5f61 6464 6020 616e 6420 6063 6170 5f64  _add` and `cap_d
-00000700: 726f 7060 2070 6172 616d 6574 6572 7320  rop` parameters 
-00000710: 746f 2073 6572 7669 6365 2063 7265 6174  to service creat
-00000720: 6520 616e 6420 436f 6e74 6169 6e65 7253  e and ContainerS
-00000730: 7065 630a 2d20 4164 6420 6074 656d 706c  pec.- Add `templ
-00000740: 6174 696e 6760 2070 6172 616d 6574 6572  ating` parameter
-00000750: 2074 6f20 636f 6e66 6967 2063 7265 6174   to config creat
-00000760: 650a 0a23 2323 2042 7567 6669 7865 730a  e..### Bugfixes.
-00000770: 2d20 4669 7820 6765 7474 696e 6720 6120  - Fix getting a 
-00000780: 7265 6164 2074 696d 656f 7574 2066 6f72  read timeout for
-00000790: 206c 6f67 732f 6174 7461 6368 2077 6974   logs/attach wit
-000007a0: 6820 6120 7474 7920 616e 6420 736c 6f77  h a tty and slow
-000007b0: 206f 7574 7075 740a 0a23 2323 204d 6973   output..### Mis
-000007c0: 6365 6c6c 616e 656f 7573 0a2d 2046 6978  cellaneous.- Fix
-000007d0: 2064 6f63 756d 656e 7461 7469 6f6e 2065   documentation e
-000007e0: 7861 6d70 6c65 730a 0a35 2e30 2e32 0a2d  xamples..5.0.2.-
-000007f0: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-00000800: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-00000810: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-00000820: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000830: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-00000840: 792f 6d69 6c65 7374 6f6e 652f 3735 3f63  y/milestone/75?c
-00000850: 6c6f 7365 643d 3129 0a0a 2323 2320 4275  losed=1)..### Bu
-00000860: 6766 6978 6573 0a2d 2046 6978 2060 6469  gfixes.- Fix `di
-00000870: 7361 626c 655f 6275 6666 6572 696e 6760  sable_buffering`
-00000880: 2072 6567 7265 7373 696f 6e0a 0a35 2e30   regression..5.0
-00000890: 2e31 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420  .1.-----..[List 
-000008a0: 6f66 2050 5273 202f 2069 7373 7565 7320  of PRs / issues 
-000008b0: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
-000008c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000008d0: 2e63 6f6d 2f64 6f63 6b65 722f 646f 636b  .com/docker/dock
-000008e0: 6572 2d70 792f 6d69 6c65 7374 6f6e 652f  er-py/milestone/
-000008f0: 3734 3f63 6c6f 7365 643d 3129 0a0a 2323  74?closed=1)..##
-00000900: 2320 4275 6766 6978 6573 0a2d 2042 7269  # Bugfixes.- Bri
-00000910: 6e67 2062 6163 6b20 7375 7070 6f72 7420  ng back support 
-00000920: 666f 7220 7373 6820 6964 656e 7469 7479  for ssh identity
-00000930: 2066 696c 650a 2d20 436c 6561 6e75 7020   file.- Cleanup 
-00000940: 7265 6d61 696e 696e 6720 7079 7468 6f6e  remaining python
-00000950: 2d32 2064 6570 656e 6465 6e63 6965 730a  -2 dependencies.
-00000960: 2d20 4669 7820 696d 6167 6520 7361 7665  - Fix image save
-00000970: 2065 7861 6d70 6c65 2069 6e20 646f 6373   example in docs
-00000980: 0a0a 2323 2320 4d69 7363 656c 6c61 6e65  ..### Miscellane
-00000990: 6f75 730a 2d20 4275 6d70 2075 726c 6c69  ous.- Bump urlli
-000009a0: 6233 2074 6f20 312e 3236 2e35 0a2d 2042  b3 to 1.26.5.- B
-000009b0: 756d 7020 7265 7175 6573 7473 2074 6f20  ump requests to 
-000009c0: 322e 3236 2e30 0a0a 352e 302e 300a 2d2d  2.26.0..5.0.0.--
-000009d0: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
-000009e0: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
-000009f0: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-00000a00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000a10: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
-00000a20: 2f6d 696c 6573 746f 6e65 2f37 303f 636c  /milestone/70?cl
-00000a30: 6f73 6564 3d31 290a 0a23 2323 2042 7265  osed=1)..### Bre
-00000a40: 616b 696e 6720 6368 616e 6765 730a 2d20  aking changes.- 
-00000a50: 5265 6d6f 7665 2073 7570 706f 7274 2066  Remove support f
-00000a60: 6f72 2050 7974 686f 6e20 322e 370a 2d20  or Python 2.7.- 
-00000a70: 4d61 6b65 2050 7974 686f 6e20 332e 3620  Make Python 3.6 
-00000a80: 7468 6520 6d69 6e69 6d75 6d20 7665 7273  the minimum vers
-00000a90: 696f 6e20 7375 7070 6f72 7465 640a 0a23  ion supported..#
-00000aa0: 2323 2046 6561 7475 7265 730a 2d20 4164  ## Features.- Ad
-00000ab0: 6420 606c 696d 6974 6020 7061 7261 6d65  d `limit` parame
-00000ac0: 7465 7220 746f 2069 6d61 6765 2073 6561  ter to image sea
-00000ad0: 7263 6820 656e 6470 6f69 6e74 0a0a 2323  rch endpoint..##
-00000ae0: 2320 4275 6766 6978 6573 0a2d 2046 6978  # Bugfixes.- Fix
-00000af0: 2060 4b65 7945 7272 6f72 6020 6578 6365   `KeyError` exce
-00000b00: 7074 696f 6e20 6f6e 2073 6563 7265 7420  ption on secret 
-00000b10: 6372 6561 7465 0a2d 2056 6572 6966 7920  create.- Verify 
-00000b20: 544c 5320 6b65 7973 206c 6f61 6465 6420  TLS keys loaded 
-00000b30: 6672 6f6d 2064 6f63 6b65 7220 636f 6e74  from docker cont
-00000b40: 6578 7473 0a2d 2055 7064 6174 6520 504f  exts.- Update PO
-00000b50: 5254 5f53 5045 4320 7265 6765 7820 746f  RT_SPEC regex to
-00000b60: 2061 6c6c 6f77 2073 7175 6172 6520 6272   allow square br
-00000b70: 6163 6b65 7473 2066 6f72 2049 5076 3620  ackets for IPv6 
-00000b80: 6164 6472 6573 7365 730a 2d20 4669 7820  addresses.- Fix 
-00000b90: 636f 6e74 6169 6e65 7273 2061 6e64 2069  containers and i
-00000ba0: 6d61 6765 7320 646f 6375 6d65 6e74 6174  mages documentat
-00000bb0: 696f 6e20 6578 616d 706c 6573 0a0a 342e  ion examples..4.
-00000bc0: 342e 340a 2d2d 2d2d 2d0a 0a5b 4c69 7374  4.4.-----..[List
-00000bd0: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
-00000be0: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-00000bf0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000c00: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
-00000c10: 6b65 722d 7079 2f6d 696c 6573 746f 6e65  ker-py/milestone
-00000c20: 2f37 333f 636c 6f73 6564 3d31 290a 0a23  /73?closed=1)..#
-00000c30: 2323 2042 7567 6669 7865 730a 2d20 5265  ## Bugfixes.- Re
-00000c40: 6d6f 7665 2060 4c44 5f4c 4942 5241 5259  move `LD_LIBRARY
-00000c50: 5f50 4154 4860 2061 6e64 2060 5353 4c5f  _PATH` and `SSL_
-00000c60: 4345 5254 5f46 494c 4560 2065 6e76 6972  CERT_FILE` envir
-00000c70: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-00000c80: 2077 6865 6e20 7368 656c 6c69 6e67 206f   when shelling o
-00000c90: 7574 2074 6f20 7468 6520 7373 6820 636c  ut to the ssh cl
-00000ca0: 6965 6e74 0a0a 342e 342e 330a 2d2d 2d2d  ient..4.4.3.----
-00000cb0: 2d0a 0a5b 4c69 7374 206f 6620 5052 7320  -..[List of PRs 
-00000cc0: 2f20 6973 7375 6573 2066 6f72 2074 6869  / issues for thi
-00000cd0: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
-00000ce0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-00000cf0: 636b 6572 2f64 6f63 6b65 722d 7079 2f6d  cker/docker-py/m
-00000d00: 696c 6573 746f 6e65 2f37 323f 636c 6f73  ilestone/72?clos
-00000d10: 6564 3d31 290a 0a23 2323 2046 6561 7475  ed=1)..### Featu
-00000d20: 7265 730a 2d20 4164 6420 7375 7070 6f72  res.- Add suppor
-00000d30: 7420 666f 7220 646f 636b 6572 2e74 7970  t for docker.typ
-00000d40: 6573 2e50 6c61 6365 6d65 6e74 2e4d 6178  es.Placement.Max
-00000d50: 5265 706c 6963 6173 0a0a 2323 2320 4275  Replicas..### Bu
-00000d60: 6766 6978 6573 0a2d 2046 6978 2053 5348  gfixes.- Fix SSH
-00000d70: 2070 6f72 7420 7061 7273 696e 6720 7768   port parsing wh
-00000d80: 656e 2073 6865 6c6c 696e 6720 6f75 7420  en shelling out 
-00000d90: 746f 2074 6865 2073 7368 2063 6c69 656e  to the ssh clien
-00000da0: 740a 0a34 2e34 2e32 0a2d 2d2d 2d2d 0a0a  t..4.4.2.-----..
-00000db0: 5b4c 6973 7420 6f66 2050 5273 202f 2069  [List of PRs / i
-00000dc0: 7373 7565 7320 666f 7220 7468 6973 2072  ssues for this r
-00000dd0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
-00000de0: 6769 7468 7562 2e63 6f6d 2f64 6f63 6b65  github.com/docke
-00000df0: 722f 646f 636b 6572 2d70 792f 6d69 6c65  r/docker-py/mile
-00000e00: 7374 6f6e 652f 3731 3f63 6c6f 7365 643d  stone/71?closed=
-00000e10: 3129 0a0a 2323 2320 4275 6766 6978 6573  1)..### Bugfixes
-00000e20: 0a2d 2046 6978 2053 5348 2063 6f6e 6e65  .- Fix SSH conne
-00000e30: 6374 696f 6e20 6275 6720 7768 6572 6520  ction bug where 
-00000e40: 7468 6520 686f 7374 6e61 6d65 2077 6173  the hostname was
-00000e50: 2069 6e63 6f72 7265 6374 6c79 2074 7269   incorrectly tri
-00000e60: 6d6d 6564 2061 6e64 2074 6865 2065 7272  mmed and the err
-00000e70: 6f72 2077 6173 2068 6964 6465 6e0a 2d20  or was hidden.- 
-00000e80: 4669 7820 646f 6373 2065 7861 6d70 6c65  Fix docs example
-00000e90: 0a0a 2323 2320 4d69 7363 656c 6c61 6e65  ..### Miscellane
-00000ea0: 6f75 730a 2d20 4164 6420 5079 7468 6f6e  ous.- Add Python
-00000eb0: 332e 3820 616e 6420 332e 3920 696e 2073  3.8 and 3.9 in s
-00000ec0: 6574 7570 2e70 7920 636c 6173 7369 6669  etup.py classifi
-00000ed0: 6572 206c 6973 740a 0a34 2e34 2e31 0a2d  er list..4.4.1.-
-00000ee0: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-00000ef0: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-00000f00: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-00000f10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000f20: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-00000f30: 792f 6d69 6c65 7374 6f6e 652f 3639 3f63  y/milestone/69?c
-00000f40: 6c6f 7365 643d 3129 0a0a 2323 2320 4275  losed=1)..### Bu
-00000f50: 6766 6978 6573 0a2d 2041 766f 6964 2073  gfixes.- Avoid s
-00000f60: 6574 7469 6e67 2075 6e73 7570 6f72 7465  etting unsuporte
-00000f70: 6420 7061 7261 6d65 7465 7220 666f 7220  d parameter for 
-00000f80: 7375 6270 726f 6365 7373 2e50 6f70 656e  subprocess.Popen
-00000f90: 206f 6e20 5769 6e64 6f77 730a 2d20 5265   on Windows.- Re
-00000fa0: 706c 6163 6520 7573 6520 6f66 2064 6570  place use of dep
-00000fb0: 7265 6361 7465 6420 2266 696c 7465 7222  recated "filter"
-00000fc0: 2061 7267 756d 656e 7420 6f6e 2022 2264   argument on ""d
-00000fd0: 6f63 6b65 722f 6170 692f 696d 6167 6522  ocker/api/image"
-00000fe0: 0a0a 342e 342e 300a 2d2d 2d2d 2d0a 0a5b  ..4.4.0.-----..[
-00000ff0: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
-00001000: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
-00001010: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00001020: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
-00001030: 2f64 6f63 6b65 722d 7079 2f6d 696c 6573  /docker-py/miles
-00001040: 746f 6e65 2f36 373f 636c 6f73 6564 3d31  tone/67?closed=1
-00001050: 290a 0a23 2323 2046 6561 7475 7265 730a  )..### Features.
-00001060: 2d20 4164 6420 616e 2061 6c74 6572 6e61  - Add an alterna
-00001070: 7469 7665 2053 5348 2063 6f6e 6e65 6374  tive SSH connect
-00001080: 696f 6e20 746f 2074 6865 2070 6172 616d  ion to the param
-00001090: 696b 6f20 6f6e 652c 2062 6173 6564 206f  iko one, based o
-000010a0: 6e20 7368 656c 6c69 6e67 206f 7574 2074  n shelling out t
-000010b0: 6f20 7468 6520 5353 6820 636c 6965 6e74  o the SSh client
-000010c0: 2e20 5369 6d69 6c61 7220 746f 2074 6865  . Similar to the
-000010d0: 2062 6568 6176 696f 7572 206f 6620 446f   behaviour of Do
-000010e0: 636b 6572 2063 6c69 0a2d 2044 6566 6175  cker cli.- Defau
-000010f0: 6c74 2069 6d61 6765 2074 6167 2074 6f20  lt image tag to 
-00001100: 606c 6174 6573 7460 206f 6e20 6070 756c  `latest` on `pul
-00001110: 6c60 0a0a 2323 2320 4275 6766 6978 6573  l`..### Bugfixes
-00001120: 0a2d 2046 6978 2070 6c75 6769 6e20 6d6f  .- Fix plugin mo
-00001130: 6465 6c20 7570 6772 6164 650a 2d20 4669  del upgrade.- Fi
-00001140: 7820 6578 616d 706c 6573 2055 524c 2069  x examples URL i
-00001150: 6e20 756c 696d 6974 730a 0a23 2323 204d  n ulimits..### M
-00001160: 6973 6365 6c6c 616e 656f 7573 0a2d 2049  iscellaneous.- I
-00001170: 6d70 726f 7665 2065 7863 6570 7469 6f6e  mprove exception
-00001180: 206d 6573 7361 6765 7320 666f 7220 7365   messages for se
-00001190: 7276 6572 2061 6e64 2063 6c69 656e 7420  rver and client 
-000011a0: 6572 726f 7273 0a2d 2042 756d 7020 6372  errors.- Bump cr
-000011b0: 7970 746f 6772 6170 6879 2066 726f 6d20  yptography from 
-000011c0: 322e 3320 746f 2033 2e32 0a0a 342e 332e  2.3 to 3.2..4.3.
-000011d0: 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f  1.-----..[List o
-000011e0: 6620 5052 7320 2f20 6973 7375 6573 2066  f PRs / issues f
-000011f0: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
-00001200: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001210: 636f 6d2f 646f 636b 6572 2f64 6f63 6b65  com/docker/docke
-00001220: 722d 7079 2f6d 696c 6573 746f 6e65 2f36  r-py/milestone/6
-00001230: 383f 636c 6f73 6564 3d31 290a 0a23 2323  8?closed=1)..###
-00001240: 204d 6973 6365 6c6c 616e 656f 7573 0a2d   Miscellaneous.-
-00001250: 2053 6574 2064 6566 6175 6c74 2041 5049   Set default API
-00001260: 2076 6572 7369 6f6e 2074 6f20 6061 7574   version to `aut
-00001270: 6f60 0a2d 2046 6978 2063 6f6e 7665 7273  o`.- Fix convers
-00001280: 696f 6e20 746f 2062 7974 6573 2066 6f72  ion to bytes for
-00001290: 2060 666c 6f61 7460 0a2d 2053 7570 706f   `float`.- Suppo
-000012a0: 7274 204f 7065 6e53 5348 2060 6964 656e  rt OpenSSH `iden
-000012b0: 7469 7479 6669 6c65 6020 6f70 7469 6f6e  tityfile` option
-000012c0: 0a0a 342e 332e 300a 2d2d 2d2d 2d0a 0a5b  ..4.3.0.-----..[
-000012d0: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
-000012e0: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
-000012f0: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00001300: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
-00001310: 2f64 6f63 6b65 722d 7079 2f6d 696c 6573  /docker-py/miles
-00001320: 746f 6e65 2f36 343f 636c 6f73 6564 3d31  tone/64?closed=1
-00001330: 290a 0a23 2323 2046 6561 7475 7265 730a  )..### Features.
-00001340: 2d20 4164 6420 6044 6576 6963 6552 6571  - Add `DeviceReq
-00001350: 7565 7374 6020 7479 7065 2074 6f20 6578  uest` type to ex
-00001360: 706f 7365 2068 6f73 7420 7265 736f 7572  pose host resour
-00001370: 6365 7320 7375 6368 2061 7320 4750 5573  ces such as GPUs
-00001380: 0a2d 2041 6464 2073 7570 706f 7274 2066  .- Add support f
-00001390: 6f72 2060 4472 6976 6572 4f70 7473 6020  or `DriverOpts` 
-000013a0: 696e 2045 6e64 706f 696e 7443 6f6e 6669  in EndpointConfi
-000013b0: 670a 2d20 4469 7361 626c 6520 636f 6d70  g.- Disable comp
-000013c0: 7265 7373 696f 6e20 6279 2064 6566 6175  ression by defau
-000013d0: 6c74 2077 6865 6e20 7573 696e 6720 636f  lt when using co
-000013e0: 6e74 6169 6e65 722e 6765 745f 6172 6368  ntainer.get_arch
-000013f0: 6976 6520 6d65 7468 6f64 0a0a 2323 2320  ive method..### 
-00001400: 4d69 7363 656c 6c61 6e65 6f75 730a 2d20  Miscellaneous.- 
-00001410: 5570 6461 7465 2064 6566 6175 6c74 2041  Update default A
-00001420: 5049 2076 6572 7369 6f6e 2074 6f20 7631  PI version to v1
-00001430: 2e33 390a 2d20 5570 6461 7465 2074 6573  .39.- Update tes
-00001440: 7420 656e 6769 6e65 2076 6572 7369 6f6e  t engine version
-00001450: 2074 6f20 3139 2e30 332e 3132 0a0a 342e   to 19.03.12..4.
-00001460: 322e 320a 2d2d 2d2d 2d0a 0a5b 4c69 7374  2.2.-----..[List
-00001470: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
-00001480: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-00001490: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-000014a0: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
-000014b0: 6b65 722d 7079 2f6d 696c 6573 746f 6e65  ker-py/milestone
-000014c0: 2f36 363f 636c 6f73 6564 3d31 290a 0a23  /66?closed=1)..#
-000014d0: 2323 2042 7567 6669 7865 730a 0a2d 2046  ## Bugfixes..- F
-000014e0: 6978 2063 6f6e 7465 7874 206c 6f61 6420  ix context load 
-000014f0: 666f 7220 6e6f 6e2d 646f 636b 6572 2065  for non-docker e
-00001500: 6e64 706f 696e 7473 0a0a 342e 322e 310a  ndpoints..4.2.1.
-00001510: 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f 6620  -----..[List of 
-00001520: 5052 7320 2f20 6973 7375 6573 2066 6f72  PRs / issues for
-00001530: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
-00001540: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001550: 6d2f 646f 636b 6572 2f64 6f63 6b65 722d  m/docker/docker-
-00001560: 7079 2f6d 696c 6573 746f 6e65 2f36 353f  py/milestone/65?
-00001570: 636c 6f73 6564 3d31 290a 0a23 2323 2046  closed=1)..### F
-00001580: 6561 7475 7265 730a 0a2d 2041 6464 206f  eatures..- Add o
-00001590: 7074 696f 6e20 6f6e 2077 6865 6e20 746f  ption on when to
-000015a0: 2075 7365 2060 746c 7360 206f 6e20 436f   use `tls` on Co
-000015b0: 6e74 6578 7420 636f 6e73 7472 7563 746f  ntext constructo
-000015c0: 720a 2d20 4d61 6b65 2063 6f6e 7465 7874  r.- Make context
-000015d0: 206f 7263 6865 7374 7261 746f 7220 6669   orchestrator fi
-000015e0: 656c 6420 6f70 7469 6f6e 616c 0a0a 342e  eld optional..4.
-000015f0: 322e 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374  2.0.-----..[List
-00001600: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
-00001610: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-00001620: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00001630: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
-00001640: 6b65 722d 7079 2f6d 696c 6573 746f 6e65  ker-py/milestone
-00001650: 2f36 333f 636c 6f73 6564 3d31 290a 0a23  /63?closed=1)..#
-00001660: 2323 2042 7567 6669 7865 730a 0a2d 2046  ## Bugfixes..- F
-00001670: 6978 2060 7769 6e33 3270 6970 652e 5761  ix `win32pipe.Wa
-00001680: 6974 4e61 6d65 6450 6970 6560 2074 6872  itNamedPipe` thr
-00001690: 6f77 2065 7863 6570 7469 6f6e 2069 6e20  ow exception in 
-000016a0: 5769 6e64 6f77 7320 636f 6e74 6169 6e65  Windows containe
-000016b0: 7273 0a2d 2055 7365 2060 486f 7374 6e61  rs.- Use `Hostna
-000016c0: 6d65 602c 2060 5573 6572 6e61 6d65 602c  me`, `Username`,
-000016d0: 2060 506f 7274 6020 616e 6420 6050 726f   `Port` and `Pro
-000016e0: 7879 436f 6d6d 616e 6460 2073 6574 7469  xyCommand` setti
-000016f0: 6e67 7320 6672 6f6d 2060 2e73 7368 2f63  ngs from `.ssh/c
-00001700: 6f6e 6669 6760 2077 6865 6e20 6f6e 2053  onfig` when on S
-00001710: 5348 0a2d 2053 6574 2068 6f73 7420 6b65  SH.- Set host ke
-00001720: 7920 706f 6c69 6379 2066 6f72 2073 7368  y policy for ssh
-00001730: 2074 7261 6e73 706f 7274 2074 6f20 6070   transport to `p
-00001740: 6172 616d 696b 6f2e 5761 726e 696e 6750  aramiko.WarningP
-00001750: 6f6c 6963 7928 2960 0a2d 2053 6574 206c  olicy()`.- Set l
-00001760: 6f67 6769 6e67 206c 6576 656c 206f 6620  ogging level of 
-00001770: 6070 6172 616d 696b 6f60 2074 6f20 7761  `paramiko` to wa
-00001780: 726e 0a0a 2323 2320 4665 6174 7572 6573  rn..### Features
-00001790: 0a0a 2d20 4164 6420 7375 7070 6f72 7420  ..- Add support 
-000017a0: 666f 7220 646f 636b 6572 2063 6f6e 7465  for docker conte
-000017b0: 7874 7320 7468 726f 7567 6820 6064 6f63  xts through `doc
-000017c0: 6b65 722e 436f 6e74 6578 7441 5049 600a  ker.ContextAPI`.
-000017d0: 0a34 2e31 2e30 0a2d 2d2d 2d2d 0a0a 5b4c  .4.1.0.-----..[L
-000017e0: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
-000017f0: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
-00001800: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-00001810: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
-00001820: 646f 636b 6572 2d70 792f 6d69 6c65 7374  docker-py/milest
-00001830: 6f6e 652f 3631 3f63 6c6f 7365 643d 3129  one/61?closed=1)
-00001840: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-00001850: 2d20 436f 7272 6563 7420 6049 4e44 4558  - Correct `INDEX
-00001860: 5f55 524c 6020 6c6f 6769 6320 696e 2062  _URL` logic in b
-00001870: 7569 6c64 2e70 7920 5f73 6574 5f61 7574  uild.py _set_aut
-00001880: 685f 6865 6164 6572 730a 2d20 4669 7820  h_headers.- Fix 
-00001890: 666f 7220 656d 7074 7920 6175 7468 206b  for empty auth k
-000018a0: 6579 7320 696e 2063 6f6e 6669 672e 6a73  eys in config.js
-000018b0: 6f6e 0a0a 2323 2320 4665 6174 7572 6573  on..### Features
-000018c0: 0a0a 2d20 4164 6420 604e 6574 776f 726b  ..- Add `Network
-000018d0: 4174 7461 6368 6d65 6e74 436f 6e66 6967  AttachmentConfig
-000018e0: 6020 666f 7220 7365 7276 6963 6520 6372  ` for service cr
-000018f0: 6561 7465 2f75 7064 6174 650a 0a23 2323  eate/update..###
-00001900: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
-00001910: 2d20 4275 6d70 2070 7974 6573 7420 746f  - Bump pytest to
-00001920: 2034 2e33 2e31 0a2d 2041 646a 7573 7420   4.3.1.- Adjust 
-00001930: 602d 2d70 6c61 7466 6f72 6d60 2074 6573  `--platform` tes
-00001940: 7473 2066 6f72 2063 6861 6e67 6573 2069  ts for changes i
-00001950: 6e20 646f 636b 6572 2065 6e67 696e 650a  n docker engine.
-00001960: 2d20 5570 6461 7465 2063 7265 6465 6e74  - Update credent
-00001970: 6961 6c73 2d68 656c 7065 7273 2074 6f20  ials-helpers to 
-00001980: 7630 2e36 2e33 0a0a 342e 302e 320a 2d2d  v0.6.3..4.0.2.--
-00001990: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
-000019a0: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
-000019b0: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-000019c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000019d0: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
-000019e0: 2f6d 696c 6573 746f 6e65 2f36 323f 636c  /milestone/62?cl
-000019f0: 6f73 6564 3d31 290a 0a23 2323 2042 7567  osed=1)..### Bug
-00001a00: 6669 7865 730a 0a2d 2055 6e69 6669 6564  fixes..- Unified
-00001a10: 2074 6865 2077 6179 2060 4865 616c 7468   the way `Health
-00001a20: 4368 6563 6b60 2069 7320 6372 6561 7465  Check` is create
-00001a30: 642f 636f 6e66 6967 7572 6564 0a0a 2323  d/configured..##
-00001a40: 2320 4d69 7363 656c 6c61 6e65 6f75 730a  # Miscellaneous.
-00001a50: 0a2d 2042 756d 7065 6420 7665 7273 696f  .- Bumped versio
-00001a60: 6e20 6f66 2077 6562 736f 636b 6574 2d63  n of websocket-c
-00001a70: 6c69 656e 740a 0a34 2e30 2e31 0a2d 2d2d  lient..4.0.1.---
-00001a80: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
-00001a90: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
-00001aa0: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-00001ab0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00001ac0: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
-00001ad0: 6d69 6c65 7374 6f6e 652f 3630 3f63 6c6f  milestone/60?clo
-00001ae0: 7365 643d 3129 0a0a 2323 2320 4275 6766  sed=1)..### Bugf
-00001af0: 6978 6573 0a0a 2d20 4669 7865 6420 616e  ixes..- Fixed an
-00001b00: 206f 6273 6f6c 6574 6520 696d 706f 7274   obsolete import
-00001b10: 2069 6e20 7468 6520 6063 7265 6465 6e74   in the `credent
-00001b20: 6961 6c73 6020 7375 6270 6163 6b61 6765  ials` subpackage
-00001b30: 2074 6861 7420 6361 7573 6564 2069 6d70   that caused imp
-00001b40: 6f72 7420 6572 726f 7273 2069 6e0a 2020  ort errors in.  
-00001b50: 5079 7468 6f6e 2033 2e37 0a0a 2323 2320  Python 3.7..### 
-00001b60: 4d69 7363 656c 6c61 6e65 6f75 730a 0a2d  Miscellaneous..-
-00001b70: 2044 6f63 7320 6275 696c 6469 6e67 2068   Docs building h
-00001b80: 6173 2062 6565 6e20 7265 7061 6972 6564  as been repaired
-00001b90: 0a0a 342e 302e 300a 2d2d 2d2d 2d0a 0a5b  ..4.0.0.-----..[
-00001ba0: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
-00001bb0: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
-00001bc0: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00001bd0: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
-00001be0: 2f64 6f63 6b65 722d 7079 2f6d 696c 6573  /docker-py/miles
-00001bf0: 746f 6e65 2f35 373f 636c 6f73 6564 3d31  tone/57?closed=1
-00001c00: 290a 0a23 2323 2042 7265 616b 696e 6720  )..### Breaking 
-00001c10: 6368 616e 6765 730a 0a2d 2053 7570 706f  changes..- Suppo
-00001c20: 7274 2066 6f72 2050 7974 686f 6e20 332e  rt for Python 3.
-00001c30: 3320 616e 6420 5079 7468 6f6e 2033 2e34  3 and Python 3.4
-00001c40: 2068 6173 2062 6565 6e20 6472 6f70 7065   has been droppe
-00001c50: 640a 2d20 6041 5049 436c 6965 6e74 2e75  d.- `APIClient.u
-00001c60: 7064 6174 655f 7365 7276 6963 6560 2c20  pdate_service`, 
-00001c70: 6041 5049 436c 6965 6e74 2e69 6e69 745f  `APIClient.init_
-00001c80: 7377 6172 6d60 2c20 616e 640a 2020 6044  swarm`, and.  `D
-00001c90: 6f63 6b65 7243 6c69 656e 742e 7377 6172  ockerClient.swar
-00001ca0: 6d2e 696e 6974 6020 6e6f 7720 7265 7475  m.init` now retu
-00001cb0: 726e 2061 2060 6469 6374 6020 6672 6f6d  rn a `dict` from
-00001cc0: 2074 6865 2041 5049 2773 2072 6573 706f   the API's respo
-00001cd0: 6e73 6520 626f 6479 0a2d 2049 6e20 6041  nse body.- In `A
-00001ce0: 5049 436c 6965 6e74 2e62 7569 6c64 6020  PIClient.build` 
-00001cf0: 616e 6420 6044 6f63 6b65 7243 6c69 656e  and `DockerClien
-00001d00: 742e 696d 6167 6573 2e62 7569 6c64 602c  t.images.build`,
-00001d10: 2074 6865 2060 7573 655f 636f 6e66 6967   the `use_config
-00001d20: 5f70 726f 7879 600a 2020 7061 7261 6d65  _proxy`.  parame
-00001d30: 7465 7220 6e6f 7720 6465 6661 756c 7473  ter now defaults
-00001d40: 2074 6f20 5472 7565 0a2d 2060 696e 6974   to True.- `init
-00001d50: 5f70 6174 6860 2069 7320 6e6f 206c 6f6e  _path` is no lon
-00001d60: 6765 7220 6120 7661 6c69 6420 7061 7261  ger a valid para
-00001d70: 6d65 7465 7220 666f 7220 6048 6f73 7443  meter for `HostC
-00001d80: 6f6e 6669 6760 0a0a 2323 2320 4665 6174  onfig`..### Feat
-00001d90: 7572 6573 0a0a 2d20 4974 2069 7320 6e6f  ures..- It is no
-00001da0: 7720 706f 7373 6962 6c65 2074 6f20 7072  w possible to pr
-00001db0: 6f76 6964 6520 6053 4354 5060 2070 6f72  ovide `SCTP` por
-00001dc0: 7473 2066 6f72 2070 6f72 7420 6d61 7070  ts for port mapp
-00001dd0: 696e 6773 0a2d 2060 436f 6e74 6169 6e65  ings.- `Containe
-00001de0: 7253 7065 6360 7320 6e6f 7720 7375 7070  rSpec`s now supp
-00001df0: 6f72 7420 7468 6520 6069 6e69 7460 2070  ort the `init` p
-00001e00: 6172 616d 6574 6572 0a2d 2060 446f 636b  arameter.- `Dock
-00001e10: 6572 436c 6965 6e74 2e73 7761 726d 2e69  erClient.swarm.i
-00001e20: 6e69 7460 2061 6e64 2060 4150 4943 6c69  nit` and `APICli
-00001e30: 656e 742e 696e 6974 5f73 7761 726d 6020  ent.init_swarm` 
-00001e40: 6e6f 7720 7375 7070 6f72 7420 7468 650a  now support the.
-00001e50: 2020 6064 6174 615f 7061 7468 5f61 6464    `data_path_add
-00001e60: 7260 2070 6172 616d 6574 6572 0a2d 2060  r` parameter.- `
-00001e70: 4150 4943 6c69 656e 742e 7570 6461 7465  APIClient.update
-00001e80: 5f73 7761 726d 6020 616e 6420 6044 6f63  _swarm` and `Doc
-00001e90: 6b65 7243 6c69 656e 742e 7377 6172 6d2e  kerClient.swarm.
-00001ea0: 7570 6461 7465 6020 6e6f 7720 7375 7070  update` now supp
-00001eb0: 6f72 7420 7468 650a 2020 6072 6f74 6174  ort the.  `rotat
-00001ec0: 655f 6d61 6e61 6765 725f 756e 6c6f 636b  e_manager_unlock
-00001ed0: 5f6b 6579 6020 7061 7261 6d65 7465 720a  _key` parameter.
-00001ee0: 2d20 6041 5049 436c 6965 6e74 2e75 7064  - `APIClient.upd
-00001ef0: 6174 655f 7365 7276 6963 6560 2072 6574  ate_service` ret
-00001f00: 7572 6e73 2074 6865 2041 5049 2773 2072  urns the API's r
-00001f10: 6573 706f 6e73 6520 626f 6479 2061 7320  esponse body as 
-00001f20: 6120 6064 6963 7460 0a2d 2060 4150 4943  a `dict`.- `APIC
-00001f30: 6c69 656e 742e 696e 6974 5f73 7761 726d  lient.init_swarm
-00001f40: 602c 2061 6e64 2060 446f 636b 6572 436c  `, and `DockerCl
-00001f50: 6965 6e74 2e73 7761 726d 2e69 6e69 7460  ient.swarm.init`
-00001f60: 206e 6f77 2072 6574 7572 6e20 7468 6520   now return the 
-00001f70: 4150 4927 730a 2020 7265 7370 6f6e 7365  API's.  response
-00001f80: 2062 6f64 7920 6173 2061 2060 6469 6374   body as a `dict
-00001f90: 600a 0a23 2323 2042 7567 6669 7865 730a  `..### Bugfixes.
-00001fa0: 0a2d 2046 6978 6564 2060 506c 6163 656d  .- Fixed `Placem
-00001fb0: 656e 7450 7265 6665 7265 6e63 6560 2069  entPreference` i
-00001fc0: 6e73 7461 6e63 6573 2074 6f20 7072 6f64  nstances to prod
-00001fd0: 7563 6520 6120 7661 6c69 6420 4150 4920  uce a valid API 
-00001fe0: 7479 7065 0a2d 2046 6978 6564 2061 2062  type.- Fixed a b
-00001ff0: 7567 2077 6865 7265 206e 6f74 2073 6574  ug where not set
-00002000: 7469 6e67 2061 2076 616c 7565 2066 6f72  ting a value for
-00002010: 2060 6275 696c 6461 7267 7360 2069 6e20   `buildargs` in 
-00002020: 6062 7569 6c64 6020 636f 756c 6420 6361  `build` could ca
-00002030: 7573 650a 2020 7468 6520 6c69 6272 6172  use.  the librar
-00002040: 7920 746f 2061 7474 656d 7074 2061 6363  y to attempt acc
-00002050: 6573 7369 6e67 2061 7474 7269 6275 7465  essing attribute
-00002060: 7320 6f66 2061 2060 4e6f 6e65 6020 7661  s of a `None` va
-00002070: 6c75 650a 2d20 4669 7865 6420 6120 6275  lue.- Fixed a bu
-00002080: 6720 7768 6572 6520 7365 7474 696e 6720  g where setting 
-00002090: 7468 6520 6076 6f6c 756d 655f 6472 6976  the `volume_driv
-000020a0: 6572 6020 7061 7261 6d65 7465 7220 696e  er` parameter in
-000020b0: 0a20 2060 446f 636b 6572 436c 6965 6e74  .  `DockerClient
-000020c0: 2e63 6f6e 7461 696e 6572 732e 6372 6561  .containers.crea
-000020d0: 7465 6020 776f 756c 6420 7265 7375 6c74  te` would result
-000020e0: 2069 6e20 616e 2065 7272 6f72 0a2d 2060   in an error.- `
-000020f0: 4150 4943 6c69 656e 742e 696e 7370 6563  APIClient.inspec
-00002100: 745f 6469 7374 7269 6275 7469 6f6e 6020  t_distribution` 
-00002110: 6e6f 7720 636f 7272 6563 746c 7920 7365  now correctly se
-00002120: 7473 2074 6865 2061 7574 6865 6e74 6963  ts the authentic
-00002130: 6174 696f 6e0a 2020 6865 6164 6572 7320  ation.  headers 
-00002140: 6f6e 2074 6865 2072 6571 7565 7374 2c20  on the request, 
-00002150: 616c 6c6f 7769 6e67 2069 7420 746f 2062  allowing it to b
-00002160: 6520 7573 6564 2077 6974 6820 7072 6976  e used with priv
-00002170: 6174 6520 7265 706f 7369 746f 7269 6573  ate repositories
-00002180: 0a20 2054 6869 7320 6368 616e 6765 2061  .  This change a
-00002190: 6c73 6f20 6170 706c 6965 7320 746f 2060  lso applies to `
-000021a0: 446f 636b 6572 436c 6965 6e74 2e67 6574  DockerClient.get
-000021b0: 5f72 6567 6973 7472 795f 6461 7461 600a  _registry_data`.
-000021c0: 0a33 2e37 2e32 0a2d 2d2d 2d2d 0a0a 5b4c  .3.7.2.-----..[L
-000021d0: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
-000021e0: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
-000021f0: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-00002200: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
-00002210: 646f 636b 6572 2d70 792f 6d69 6c65 7374  docker-py/milest
-00002220: 6f6e 652f 3539 3f63 6c6f 7365 643d 3129  one/59?closed=1)
-00002230: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-00002240: 2a20 4669 7820 6261 7365 5f75 726c 2074  * Fix base_url t
-00002250: 6f20 6b65 6570 2054 4350 2070 726f 746f  o keep TCP proto
-00002260: 636f 6c20 6f6e 2075 7469 6c73 2e70 7920  col on utils.py 
-00002270: 6279 206c 6574 7469 6e67 2074 6865 2072  by letting the r
-00002280: 6573 706f 6e73 6962 696c 6974 7920 6f66  esponsibility of
-00002290: 2063 6861 6e67 696e 6720 7468 650a 7072   changing the.pr
-000022a0: 6f74 6f63 6f6c 2074 6f20 6070 6172 7365  otocol to `parse
-000022b0: 5f68 6f73 7460 2061 6674 6572 7761 7264  _host` afterward
-000022c0: 732c 206c 6574 7469 6e67 2060 6261 7365  s, letting `base
-000022d0: 5f75 726c 6020 7769 7468 2074 6865 206f  _url` with the o
-000022e0: 7269 6769 6e61 6c20 7661 6c75 652e 0a2a  riginal value..*
-000022f0: 2058 4641 494c 2074 6573 745f 6174 7461   XFAIL test_atta
-00002300: 6368 5f73 7472 6561 6d5f 616e 645f 6361  ch_stream_and_ca
-00002310: 6e63 656c 206f 6e20 544c 530a 0a33 2e37  ncel on TLS..3.7
-00002320: 2e31 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420  .1.-----..[List 
-00002330: 6f66 2050 5273 202f 2069 7373 7565 7320  of PRs / issues 
-00002340: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
-00002350: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002360: 2e63 6f6d 2f64 6f63 6b65 722f 646f 636b  .com/docker/dock
-00002370: 6572 2d70 792f 6d69 6c65 7374 6f6e 652f  er-py/milestone/
-00002380: 3538 3f63 6c6f 7365 643d 3129 0a0a 2323  58?closed=1)..##
-00002390: 2320 4275 6766 6978 6573 0a0a 2a20 5365  # Bugfixes..* Se
-000023a0: 7420 6120 6469 6666 6572 656e 7420 6465  t a different de
-000023b0: 6661 756c 7420 6e75 6d62 6572 2028 7768  fault number (wh
-000023c0: 6963 6820 6973 206e 6f77 2039 2920 666f  ich is now 9) fo
-000023d0: 7220 5353 4820 706f 6f6c 730a 2a20 4164  r SSH pools.* Ad
-000023e0: 6473 2061 2042 6173 6548 5454 5041 6461  ds a BaseHTTPAda
-000023f0: 7074 6572 2077 6974 6820 6120 636c 6f73  pter with a clos
-00002400: 6520 6d65 7468 6f64 2074 6f20 656e 7375  e method to ensu
-00002410: 7265 2074 6861 7420 7468 650a 706f 6f6c  re that the.pool
-00002420: 7320 6973 2063 6c65 616e 206f 6e20 636c  s is clean on cl
-00002430: 6f73 6528 290a 2a20 4d61 6b65 7320 5353  ose().* Makes SS
-00002440: 4848 5454 5041 6461 7074 6572 2072 656f  HHTTPAdapter reo
-00002450: 7065 6e20 6120 636c 6f73 6564 2063 6f6e  pen a closed con
-00002460: 6e65 6374 696f 6e20 7768 656e 206e 6565  nection when nee
-00002470: 6465 640a 6c69 6b65 2074 6865 206f 7468  ded.like the oth
-00002480: 6572 730a 0a33 2e37 2e30 0a2d 2d2d 2d2d  ers..3.7.0.-----
-00002490: 0a0a 5b4c 6973 7420 6f66 2050 5273 202f  ..[List of PRs /
-000024a0: 2069 7373 7565 7320 666f 7220 7468 6973   issues for this
-000024b0: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
-000024c0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
-000024d0: 6b65 722f 646f 636b 6572 2d70 792f 6d69  ker/docker-py/mi
-000024e0: 6c65 7374 6f6e 652f 3536 3f63 6c6f 7365  lestone/56?close
-000024f0: 643d 3129 0a0a 2323 2320 4665 6174 7572  d=1)..### Featur
-00002500: 6573 0a0a 2a20 4164 6465 6420 7375 7070  es..* Added supp
-00002510: 6f72 7420 666f 7220 6d75 6c74 6970 6c65  ort for multiple
-00002520: 7865 6420 7374 7265 616d 7320 2866 6f72  xed streams (for
-00002530: 2060 6174 7461 6368 6020 616e 6420 6065   `attach` and `e
-00002540: 7865 635f 7374 6172 7460 292e 204c 6561  xec_start`). Lea
-00002550: 726e 0a20 206d 6f72 6520 6174 2068 7474  rn.  more at htt
-00002560: 7073 3a2f 2f64 6f63 6b65 722d 7079 2e72  ps://docker-py.r
-00002570: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00002580: 2f73 7461 626c 652f 7573 6572 5f67 7569  /stable/user_gui
-00002590: 6465 732f 6d75 6c74 6970 6c65 782e 6874  des/multiplex.ht
-000025a0: 6d6c 0a2a 2041 6464 6564 2074 6865 2060  ml.* Added the `
-000025b0: 7573 655f 636f 6e66 6967 5f70 726f 7879  use_config_proxy
-000025c0: 6020 7061 7261 6d65 7465 7220 746f 2074  ` parameter to t
-000025d0: 6865 2066 6f6c 6c6f 7769 6e67 206d 6574  he following met
-000025e0: 686f 6473 3a0a 2020 6041 5049 436c 6965  hods:.  `APIClie
-000025f0: 6e74 2e62 7569 6c64 602c 2060 4150 4943  nt.build`, `APIC
-00002600: 6c69 656e 742e 6372 6561 7465 5f63 6f6e  lient.create_con
-00002610: 7461 696e 6572 602c 2060 446f 636b 6572  tainer`, `Docker
-00002620: 436c 6965 6e74 2e69 6d61 6765 732e 6275  Client.images.bu
-00002630: 696c 6460 0a20 2061 6e64 2060 446f 636b  ild`.  and `Dock
-00002640: 6572 436c 6965 6e74 2e63 6f6e 7461 696e  erClient.contain
-00002650: 6572 732e 7275 6e60 2028 6046 616c 7365  ers.run` (`False
-00002660: 6020 6279 2064 6566 6175 6c74 292e 202a  ` by default). *
-00002670: 2a54 6869 7320 7061 7261 6d65 7465 722a  *This parameter*
-00002680: 2a0a 2020 2a2a 7769 6c6c 2062 6563 6f6d  *.  **will becom
-00002690: 6520 6054 7275 6560 2062 7920 6465 6661  e `True` by defa
-000026a0: 756c 7420 696e 2074 6865 2034 2e30 2e30  ult in the 4.0.0
-000026b0: 2072 656c 6561 7365 2e2a 2a0a 2a20 506c   release.**.* Pl
-000026c0: 6163 656d 656e 7420 7072 6566 6572 656e  acement preferen
-000026d0: 6365 7320 666f 7220 5377 6172 6d20 7365  ces for Swarm se
-000026e0: 7276 6963 6573 2061 7265 2062 6574 7465  rvices are bette
-000026f0: 7220 7661 6c69 6461 7465 6420 6f6e 2074  r validated on t
-00002700: 6865 2063 6c69 656e 740a 2020 616e 6420  he client.  and 
-00002710: 646f 6375 6d65 6e74 6174 696f 6e20 6861  documentation ha
-00002720: 7320 6265 656e 2075 7064 6174 6564 2061  s been updated a
-00002730: 6363 6f72 6469 6e67 6c79 0a0a 2323 2320  ccordingly..### 
-00002740: 4275 6766 6978 6573 0a0a 2a20 4669 7865  Bugfixes..* Fixe
-00002750: 6420 6120 6275 6720 7768 6572 6520 6372  d a bug where cr
-00002760: 6564 656e 7469 616c 2073 746f 7265 7320  edential stores 
-00002770: 7765 7265 6e27 7420 7175 6572 6965 6420  weren't queried 
-00002780: 666f 7220 7265 6c65 7661 6e74 2072 6567  for relevant reg
-00002790: 6973 7472 790a 2020 6372 6564 656e 7469  istry.  credenti
-000027a0: 616c 7320 7769 7468 2063 6572 7461 696e  als with certain
-000027b0: 2076 6172 6961 7469 6f6e 7320 6f66 2074   variations of t
-000027c0: 6865 2060 636f 6e66 6967 2e6a 736f 6e60  he `config.json`
-000027d0: 2066 696c 652e 0a2a 2060 446f 636b 6572   file..* `Docker
-000027e0: 436c 6965 6e74 2e73 7761 726d 2e69 6e69  Client.swarm.ini
-000027f0: 7460 206e 6f77 2072 6574 7572 6e73 2061  t` now returns a
-00002800: 2062 6f6f 6c65 616e 2076 616c 7565 2061   boolean value a
-00002810: 7320 6164 7665 7274 6973 6564 2e0a 0a33  s advertised...3
-00002820: 2e36 2e30 0a2d 2d2d 2d2d 0a0a 5b4c 6973  .6.0.-----..[Lis
-00002830: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
-00002840: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
-00002850: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-00002860: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
-00002870: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
-00002880: 653d 3535 3f63 6c6f 7365 643d 3129 0a0a  e=55?closed=1)..
-00002890: 2323 2320 4665 6174 7572 6573 0a0a 2a20  ### Features..* 
-000028a0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-000028b0: 7220 636f 6e6e 6563 7469 6e67 2074 6f20  r connecting to 
-000028c0: 7468 6520 446f 636b 6572 2045 6e67 696e  the Docker Engin
-000028d0: 6520 6f76 6572 2053 5348 2e20 4164 6469  e over SSH. Addi
-000028e0: 7469 6f6e 616c 0a20 2064 6570 656e 6465  tional.  depende
-000028f0: 6e63 6965 7320 666f 7220 7468 6973 2066  ncies for this f
-00002900: 6561 7475 7265 2063 616e 2062 6520 696e  eature can be in
-00002910: 7374 616c 6c65 6420 7769 7468 0a20 2060  stalled with.  `
-00002920: 7069 7020 696e 7374 616c 6c20 2264 6f63  pip install "doc
-00002930: 6b65 725b 7373 685d 2260 0a2a 2041 6464  ker[ssh]"`.* Add
-00002940: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
-00002950: 6865 2060 6e61 6d65 6460 2070 6172 616d  he `named` param
-00002960: 6574 6572 2069 6e20 6049 6d61 6765 2e73  eter in `Image.s
-00002970: 6176 6560 2c20 7768 6963 6820 6d61 7920  ave`, which may 
-00002980: 6265 0a20 2075 7365 6420 746f 2065 6e73  be.  used to ens
-00002990: 7572 6520 7468 6520 7265 7375 6c74 696e  ure the resultin
-000029a0: 6720 7461 7262 616c 6c20 7265 7461 696e  g tarball retain
-000029b0: 7320 7468 6520 696d 6167 6527 7320 6e61  s the image's na
-000029c0: 6d65 206f 6e20 7361 7665 2e0a 0a23 2323  me on save...###
-000029d0: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
-000029e0: 6564 2061 2062 7567 2077 6865 7265 2062  ed a bug where b
-000029f0: 7569 6c64 7320 6f6e 2057 696e 646f 7773  uilds on Windows
-00002a00: 2077 6974 6820 6120 636f 6e74 6578 7420   with a context 
-00002a10: 7061 7468 2075 7369 6e67 2074 6865 2060  path using the `
-00002a20: 5c5c 3f5c 600a 2020 7072 6566 6978 2077  \\?\`.  prefix w
-00002a30: 6f75 6c64 2066 6169 6c20 7769 7468 2073  ould fail with s
-00002a40: 6f6d 6520 7265 6c61 7469 7665 2044 6f63  ome relative Doc
-00002a50: 6b65 7266 696c 6520 7061 7468 732e 0a2a  kerfile paths..*
-00002a60: 2046 6978 6564 2061 6e20 6973 7375 6520   Fixed an issue 
-00002a70: 7768 6572 6520 7075 6c6c 7320 6d61 6465  where pulls made
-00002a80: 2077 6974 6820 7468 6520 6044 6f63 6b65   with the `Docke
-00002a90: 7243 6c69 656e 7460 2077 6f75 6c64 2066  rClient` would f
-00002aa0: 6169 6c20 7768 656e 0a20 2073 6574 7469  ail when.  setti
-00002ab0: 6e67 2074 6865 2060 7374 7265 616d 6020  ng the `stream` 
-00002ac0: 7061 7261 6d65 7465 7220 746f 2060 5472  parameter to `Tr
-00002ad0: 7565 602e 0a0a 2323 2320 4d69 7363 656c  ue`...### Miscel
-00002ae0: 6c61 6e65 6f75 730a 0a2a 2054 6865 206d  laneous..* The m
-00002af0: 696e 696d 756d 2072 6571 7569 7265 6d65  inimum requireme
-00002b00: 6e74 2066 6f72 2074 6865 2060 7265 7175  nt for the `requ
-00002b10: 6573 7473 6020 6465 7065 6e64 656e 6379  ests` dependency
-00002b20: 2068 6173 2062 6565 6e20 6275 6d70 6564   has been bumped
-00002b30: 0a20 2074 6f20 322e 3230 2e30 0a0a 332e  .  to 2.20.0..3.
-00002b40: 352e 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374  5.1.-----..[List
-00002b50: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
-00002b60: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-00002b70: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00002b80: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
-00002b90: 6b65 722d 7079 2f6d 696c 6573 746f 6e65  ker-py/milestone
-00002ba0: 2f35 343f 636c 6f73 6564 3d31 290a 0a23  /54?closed=1)..#
-00002bb0: 2323 204d 6973 6365 6c6c 616e 656f 7573  ## Miscellaneous
-00002bc0: 0a0a 2a20 4275 6d70 6564 2076 6572 7369  ..* Bumped versi
-00002bd0: 6f6e 206f 6620 6070 794f 7065 6e53 534c  on of `pyOpenSSL
-00002be0: 6020 696e 2060 7265 7175 6972 656d 656e  ` in `requiremen
-00002bf0: 7473 2e74 7874 6020 616e 6420 6073 6574  ts.txt` and `set
-00002c00: 7570 2e70 7960 2074 6f20 7072 6576 656e  up.py` to preven
-00002c10: 740a 2020 696e 7374 616c 6c61 7469 6f6e  t.  installation
-00002c20: 206f 6620 6120 7675 6c6e 6572 6162 6c65   of a vulnerable
-00002c30: 2076 6572 7369 6f6e 0a0a 2a20 446f 6373   version..* Docs
-00002c40: 2066 6978 6573 0a0a 332e 352e 300a 2d2d   fixes..3.5.0.--
-00002c50: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
-00002c60: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
-00002c70: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-00002c80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002c90: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
-00002ca0: 2f6d 696c 6573 746f 6e65 2f35 333f 636c  /milestone/53?cl
-00002cb0: 6f73 6564 3d31 290a 0a23 2323 2044 6570  osed=1)..### Dep
-00002cc0: 7265 6361 7469 6f6e 2077 6172 6e69 6e67  recation warning
-00002cd0: 0a0a 2a20 5375 7070 6f72 7420 666f 7220  ..* Support for 
-00002ce0: 5079 7468 6f6e 2033 2e33 2077 696c 6c20  Python 3.3 will 
-00002cf0: 6265 2064 726f 7070 6564 2069 6e20 7468  be dropped in th
-00002d00: 6520 342e 302e 3020 7265 6c65 6173 650a  e 4.0.0 release.
-00002d10: 0a23 2323 2046 6561 7475 7265 730a 0a2a  .### Features..*
-00002d20: 2055 7064 6174 6564 2064 6570 656e 6465   Updated depende
-00002d30: 6e63 6965 7320 746f 2065 6e73 7572 6520  ncies to ensure 
-00002d40: 7375 7070 6f72 7420 666f 7220 5079 7468  support for Pyth
-00002d50: 6f6e 2033 2e37 2065 6e76 6972 6f6e 6d65  on 3.7 environme
-00002d60: 6e74 730a 2a20 4164 6465 6420 7375 7070  nts.* Added supp
-00002d70: 6f72 7420 666f 7220 7468 6520 6075 7473  ort for the `uts
-00002d80: 5f6d 6f64 6560 2070 6172 616d 6574 6572  _mode` parameter
-00002d90: 2069 6e20 6048 6f73 7443 6f6e 6669 6760   in `HostConfig`
-00002da0: 0a2a 2054 6865 2060 5570 6461 7465 436f  .* The `UpdateCo
-00002db0: 6e66 6967 6020 636f 6e73 7472 7563 746f  nfig` constructo
-00002dc0: 7220 6e6f 7720 616c 6c6f 7773 2060 726f  r now allows `ro
-00002dd0: 6c6c 6261 636b 6020 6173 2061 2076 616c  llback` as a val
-00002de0: 6964 0a20 2076 616c 7565 2066 6f72 2060  id.  value for `
-00002df0: 6661 696c 7572 655f 6163 7469 6f6e 600a  failure_action`.
-00002e00: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-00002e10: 666f 7220 6072 6f6c 6c62 6163 6b5f 636f  for `rollback_co
-00002e20: 6e66 6967 6020 696e 2060 4150 4943 6c69  nfig` in `APICli
-00002e30: 656e 742e 6372 6561 7465 5f73 6572 7669  ent.create_servi
-00002e40: 6365 602c 0a20 2060 4150 4943 6c69 656e  ce`,.  `APIClien
-00002e50: 742e 7570 6461 7465 5f73 6572 7669 6365  t.update_service
-00002e60: 602c 2060 446f 636b 6572 436c 6965 6e74  `, `DockerClient
-00002e70: 2e73 6572 7669 6365 732e 6372 6561 7465  .services.create
-00002e80: 6020 616e 640a 2020 6053 6572 7669 6365  ` and.  `Service
-00002e90: 2e75 7064 6174 6560 2e0a 0a23 2323 2042  .update`...### B
-00002ea0: 7567 6669 7865 730a 0a2a 2043 7265 6465  ugfixes..* Crede
-00002eb0: 6e74 6961 6c20 6865 6c70 6572 7320 6172  ntial helpers ar
-00002ec0: 6520 6e6f 7720 7072 6f70 6572 6c79 206c  e now properly l
-00002ed0: 6576 6572 6167 6564 2062 7920 7468 6520  everaged by the 
-00002ee0: 6062 7569 6c64 6020 6d65 7468 6f64 0a2a  `build` method.*
-00002ef0: 2046 6978 6564 2061 2062 7567 2074 6861   Fixed a bug tha
-00002f00: 7420 6361 7573 6564 2070 6c61 6365 6d65  t caused placeme
-00002f10: 6e74 2070 7265 6665 7265 6e63 6573 2074  nt preferences t
-00002f20: 6f20 6265 2069 676e 6f72 6564 2077 6865  o be ignored whe
-00002f30: 6e20 7072 6f76 6964 6564 0a20 2074 6f20  n provided.  to 
-00002f40: 6044 6f63 6b65 7243 6c69 656e 742e 7365  `DockerClient.se
-00002f50: 7276 6963 6573 2e63 7265 6174 6560 0a2a  rvices.create`.*
-00002f60: 2046 6978 6564 2061 2062 7567 2074 6861   Fixed a bug tha
-00002f70: 7420 6361 7573 6564 2061 2060 7573 6572  t caused a `user
-00002f80: 6020 7661 6c75 6520 6f66 2060 3060 2074  ` value of `0` t
-00002f90: 6f20 6265 2069 676e 6f72 6564 2069 6e0a  o be ignored in.
-00002fa0: 2020 6041 5049 436c 6965 6e74 2e63 7265    `APIClient.cre
-00002fb0: 6174 655f 636f 6e74 6169 6e65 7260 2061  ate_container` a
-00002fc0: 6e64 2060 446f 636b 6572 436c 6965 6e74  nd `DockerClient
-00002fd0: 2e63 6f6e 7461 696e 6572 732e 6372 6561  .containers.crea
-00002fe0: 7465 600a 0a33 2e34 2e31 0a2d 2d2d 2d2d  te`..3.4.1.-----
-00002ff0: 0a0a 5b4c 6973 7420 6f66 2050 5273 202f  ..[List of PRs /
-00003000: 2069 7373 7565 7320 666f 7220 7468 6973   issues for this
-00003010: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
-00003020: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
-00003030: 6b65 722f 646f 636b 6572 2d70 792f 6d69  ker/docker-py/mi
-00003040: 6c65 7374 6f6e 652f 3532 3f63 6c6f 7365  lestone/52?close
-00003050: 643d 3129 0a0a 2323 2320 4275 6766 6978  d=1)..### Bugfix
-00003060: 6573 0a0a 2a20 4669 7865 6420 6120 6275  es..* Fixed a bu
-00003070: 6720 7468 6174 2063 6175 7365 6420 6175  g that caused au
-00003080: 7468 2076 616c 7565 7320 696e 2063 6f6e  th values in con
-00003090: 6669 6720 6669 6c65 7320 7772 6974 7465  fig files writte
-000030a0: 6e20 7573 696e 6720 6f6e 6520 6f66 2074  n using one of t
-000030b0: 6865 0a20 206c 6567 6163 7920 666f 726d  he.  legacy form
-000030c0: 6174 7320 746f 2062 6520 6967 6e6f 7265  ats to be ignore
-000030d0: 640a 2a20 4669 7865 6420 6973 7375 6573  d.* Fixed issues
-000030e0: 2077 6974 6820 6861 6e64 6c69 6e67 206f   with handling o
-000030f0: 6620 646f 7562 6c65 2d77 696c 6463 6172  f double-wildcar
-00003100: 6420 602a 2a60 2070 6174 7465 726e 7320  d `**` patterns 
-00003110: 696e 0a20 2060 2e64 6f63 6b65 7269 676e  in.  `.dockerign
-00003120: 6f72 6560 2066 696c 6573 0a0a 332e 342e  ore` files..3.4.
-00003130: 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f  0.-----..[List o
-00003140: 6620 5052 7320 2f20 6973 7375 6573 2066  f PRs / issues f
-00003150: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
-00003160: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003170: 636f 6d2f 646f 636b 6572 2f64 6f63 6b65  com/docker/docke
-00003180: 722d 7079 2f6d 696c 6573 746f 6e65 2f35  r-py/milestone/5
-00003190: 313f 636c 6f73 6564 3d31 290a 0a23 2323  1?closed=1)..###
-000031a0: 2046 6561 7475 7265 730a 0a2a 2054 6865   Features..* The
-000031b0: 2060 4150 4943 6c69 656e 7460 2061 6e64   `APIClient` and
-000031c0: 2060 446f 636b 6572 436c 6965 6e74 6020   `DockerClient` 
-000031d0: 636f 6e73 7472 7563 746f 7273 206e 6f77  constructors now
-000031e0: 2061 6363 6570 7420 6120 6063 7265 6473   accept a `creds
-000031f0: 746f 7265 5f65 6e76 600a 2020 7061 7261  tore_env`.  para
-00003200: 6d65 7465 722e 2057 6865 6e20 7365 742c  meter. When set,
-00003210: 2076 616c 7565 7320 696e 2074 6869 7320   values in this 
-00003220: 6469 6374 696f 6e61 7279 2061 7265 2061  dictionary are a
-00003230: 6464 6564 2074 6f20 7468 6520 656e 7669  dded to the envi
-00003240: 726f 6e6d 656e 740a 2020 7768 656e 2065  ronment.  when e
-00003250: 7865 6375 7469 6e67 2074 6865 2063 7265  xecuting the cre
-00003260: 6465 6e74 6961 6c20 7374 6f72 6520 7072  dential store pr
-00003270: 6f63 6573 732e 0a0a 2323 2320 4275 6766  ocess...### Bugf
-00003280: 6978 6573 0a0a 2a20 6044 6f63 6b65 7243  ixes..* `DockerC
-00003290: 6c69 656e 742e 6e65 7477 6f72 6b73 2e70  lient.networks.p
-000032a0: 7275 6e65 6020 6e6f 7720 7072 6f70 6572  rune` now proper
-000032b0: 6c79 2072 6574 7572 6e73 2074 6865 206f  ly returns the o
-000032c0: 7065 7261 7469 6f6e 2773 2072 6573 756c  peration's resul
-000032d0: 740a 2a20 4669 7865 6420 6120 6275 6720  t.* Fixed a bug 
-000032e0: 7468 6174 2063 6175 7365 6420 6375 7374  that caused cust
-000032f0: 6f6d 2044 6f63 6b65 7266 696c 6520 7061  om Dockerfile pa
-00003300: 7468 7320 696e 2061 2073 7562 666f 6c64  ths in a subfold
-00003310: 6572 206f 6620 7468 6520 6275 696c 640a  er of the build.
-00003320: 2020 636f 6e74 6578 7420 746f 2062 6520    context to be 
-00003330: 696e 7661 6c69 6461 7465 642c 2070 7265  invalidated, pre
-00003340: 7665 6e74 696e 6720 7468 6573 6520 6275  venting these bu
-00003350: 696c 6473 2066 726f 6d20 776f 726b 696e  ilds from workin
-00003360: 670a 2a20 5468 6520 6070 6c75 6769 6e5f  g.* The `plugin_
-00003370: 7072 6976 696c 6567 6573 6020 6d65 7468  privileges` meth
-00003380: 6f64 2063 616e 206e 6f77 2062 6520 6361  od can now be ca
-00003390: 6c6c 6564 2066 6f72 2070 6c75 6769 6e73  lled for plugins
-000033a0: 2072 6571 7569 7269 6e67 0a20 2061 7574   requiring.  aut
-000033b0: 6865 6e74 6963 6174 696f 6e20 746f 2061  hentication to a
-000033c0: 6363 6573 730a 2a20 4669 7865 6420 6120  ccess.* Fixed a 
-000033d0: 6275 6720 7468 6174 2063 6175 7365 6420  bug that caused 
-000033e0: 6174 7465 6d70 7473 2074 6f20 7265 6164  attempts to read
-000033f0: 2061 2064 6174 6120 7374 7265 616d 206f   a data stream o
-00003400: 7665 7220 616e 2075 6e73 6563 7572 6564  ver an unsecured
-00003410: 2054 4350 0a20 2073 6f63 6b65 7420 746f   TCP.  socket to
-00003420: 2063 7261 7368 206f 6e20 5769 6e64 6f77   crash on Window
-00003430: 7320 636c 6965 6e74 730a 2a20 4669 7865  s clients.* Fixe
-00003440: 6420 6120 6275 6720 7768 6572 6520 7573  d a bug where us
-00003450: 696e 6720 7468 6520 6072 6561 645f 6f6e  ing the `read_on
-00003460: 6c79 6020 7061 7261 6d65 7465 7220 7768  ly` parameter wh
-00003470: 656e 2063 7265 6174 696e 6720 6120 7365  en creating a se
-00003480: 7276 6963 6520 7573 696e 670a 2020 7468  rvice using.  th
-00003490: 6520 6044 6f63 6b65 7243 6c69 656e 7460  e `DockerClient`
-000034a0: 2077 6173 2062 6569 6e67 2069 676e 6f72   was being ignor
-000034b0: 6564 0a2a 2046 6978 6564 2061 6e20 6973  ed.* Fixed an is
-000034c0: 7375 6520 7768 6572 6520 6053 6572 7669  sue where `Servi
-000034d0: 6365 2e73 6361 6c65 6020 776f 756c 6420  ce.scale` would 
-000034e0: 6e6f 7420 7072 6f70 6572 6c79 2075 7064  not properly upd
-000034f0: 6174 6520 7468 6520 7365 7276 6963 6527  ate the service'
-00003500: 730a 2020 6d6f 6465 2c20 6361 7573 696e  s.  mode, causin
-00003510: 6720 7468 6520 6f70 6572 6174 696f 6e20  g the operation 
-00003520: 746f 2066 6169 6c20 7369 6c65 6e74 6c79  to fail silently
-00003530: 0a0a 332e 332e 300a 2d2d 2d2d 2d0a 0a5b  ..3.3.0.-----..[
-00003540: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
-00003550: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
-00003560: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00003570: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
-00003580: 2f64 6f63 6b65 722d 7079 2f6d 696c 6573  /docker-py/miles
-00003590: 746f 6e65 2f34 393f 636c 6f73 6564 3d31  tone/49?closed=1
-000035a0: 290a 0a23 2323 2046 6561 7475 7265 730a  )..### Features.
-000035b0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-000035c0: 2066 6f72 2060 7072 756e 655f 6275 696c   for `prune_buil
-000035d0: 6473 6020 696e 2060 4150 4943 6c69 656e  ds` in `APIClien
-000035e0: 7460 2061 6e64 2060 446f 636b 6572 436c  t` and `DockerCl
-000035f0: 6965 6e74 2e69 6d61 6765 7360 0a2a 2041  ient.images`.* A
-00003600: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
-00003610: 2060 6967 6e6f 7265 5f72 656d 6f76 6564   `ignore_removed
-00003620: 6020 7061 7261 6d65 7465 7220 696e 0a20  ` parameter in. 
-00003630: 2060 446f 636b 6572 436c 6965 6e74 2e63   `DockerClient.c
-00003640: 6f6e 7461 696e 6572 732e 6c69 7374 600a  ontainers.list`.
-00003650: 0a23 2323 2042 7567 6669 7865 730a 0a2a  .### Bugfixes..*
-00003660: 2046 6978 6564 2061 6e20 6973 7375 6520   Fixed an issue 
-00003670: 7468 6174 2063 6175 7365 6420 6275 696c  that caused buil
-00003680: 6473 2074 6f20 6661 696c 2077 6865 6e20  ds to fail when 
-00003690: 616e 2069 6e2d 636f 6e74 6578 7420 446f  an in-context Do
-000036a0: 636b 6572 6669 6c65 0a20 2077 6f75 6c64  ckerfile.  would
-000036b0: 2062 6520 7370 6563 6966 6965 6420 7573   be specified us
-000036c0: 696e 6720 6974 7320 6162 736f 6c75 7465  ing its absolute
-000036d0: 2070 6174 680a 2a20 496e 7374 616c 6c61   path.* Installa
-000036e0: 7469 6f6e 2077 6974 6820 7069 7020 3130  tion with pip 10
-000036f0: 2e30 2e30 2061 6e64 2061 626f 7665 206e  .0.0 and above n
-00003700: 6f20 6c6f 6e67 6572 2066 6169 6c73 0a2a  o longer fails.*
-00003710: 2043 6f6e 6e65 6374 696f 6e20 7469 6d65   Connection time
-00003720: 6f75 7420 666f 7220 6073 746f 7060 2061  out for `stop` a
-00003730: 6e64 2060 7265 7374 6172 7460 206e 6f77  nd `restart` now
-00003740: 2067 6574 7320 7072 6f70 6572 6c79 2061   gets properly a
-00003750: 646a 7573 7465 6420 746f 0a20 2061 6c6c  djusted to.  all
-00003760: 6f77 2066 6f72 2074 6865 206f 7065 7261  ow for the opera
-00003770: 7469 6f6e 2074 6f20 6669 6e69 7368 2069  tion to finish i
-00003780: 6e20 7468 6520 7370 6563 6966 6965 6420  n the specified 
-00003790: 7469 6d65 0a2a 2049 6d70 726f 7665 6420  time.* Improved 
-000037a0: 646f 636b 6572 2063 7265 6465 6e74 6961  docker credentia
-000037b0: 6c20 7374 6f72 6520 7375 7070 6f72 7420  l store support 
-000037c0: 6f6e 2057 696e 646f 7773 0a0a 332e 322e  on Windows..3.2.
-000037d0: 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f  1.-----..[List o
-000037e0: 6620 5052 7320 2f20 6973 7375 6573 2066  f PRs / issues f
-000037f0: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
-00003800: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003810: 636f 6d2f 646f 636b 6572 2f64 6f63 6b65  com/docker/docke
-00003820: 722d 7079 2f6d 696c 6573 746f 6e65 2f35  r-py/milestone/5
-00003830: 303f 636c 6f73 6564 3d31 290a 0a23 2323  0?closed=1)..###
-00003840: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
-00003850: 6564 2061 2062 7567 2077 6974 6820 6275  ed a bug with bu
-00003860: 696c 6473 206e 6f74 2070 726f 7065 726c  ilds not properl
-00003870: 7920 6964 656e 7469 6679 696e 6720 446f  y identifying Do
-00003880: 636b 6572 6669 6c65 2070 6174 6873 2072  ckerfile paths r
-00003890: 656c 6174 6976 650a 2020 746f 2074 6865  elative.  to the
-000038a0: 2062 7569 6c64 2063 6f6e 7465 7874 0a2a   build context.*
-000038b0: 2046 6978 6564 2061 6e20 6973 7375 6520   Fixed an issue 
-000038c0: 7768 6572 6520 6275 696c 6473 2077 6f75  where builds wou
-000038d0: 6c64 2072 6169 7365 2061 2060 5661 6c75  ld raise a `Valu
-000038e0: 6545 7272 6f72 6020 7768 656e 2061 7474  eError` when att
-000038f0: 656d 7074 696e 6720 746f 0a20 2062 7569  empting to.  bui
-00003900: 6c64 2077 6974 6820 6120 446f 636b 6572  ld with a Docker
-00003910: 6669 6c65 206f 6e20 6120 6469 6666 6572  file on a differ
-00003920: 656e 7420 5769 6e64 6f77 7320 6472 6976  ent Windows driv
-00003930: 652e 0a0a 332e 322e 300a 2d2d 2d2d 2d0a  e...3.2.0.-----.
-00003940: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
-00003950: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
-00003960: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
-00003970: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
-00003980: 6572 2f64 6f63 6b65 722d 7079 2f6d 696c  er/docker-py/mil
-00003990: 6573 746f 6e65 2f34 353f 636c 6f73 6564  estone/45?closed
-000039a0: 3d31 290a 0a23 2323 2046 6561 7475 7265  =1)..### Feature
-000039b0: 730a 0a2a 2047 656e 6572 6174 6f72 7320  s..* Generators 
-000039c0: 7265 7475 726e 6564 2062 7920 6061 7474  returned by `att
-000039d0: 6163 6828 2960 2c20 606c 6f67 7328 2960  ach()`, `logs()`
-000039e0: 2061 6e64 2060 6576 656e 7473 2829 6020   and `events()` 
-000039f0: 6e6f 7720 6861 7665 2061 0a20 2060 6361  now have a.  `ca
-00003a00: 6e63 656c 2829 6020 6d65 7468 6f64 2074  ncel()` method t
-00003a10: 6f20 6c65 7420 636f 6e73 756d 6572 7320  o let consumers 
-00003a20: 7374 6f70 2074 6865 2069 7465 7261 7469  stop the iterati
-00003a30: 6f6e 2063 6c69 656e 742d 7369 6465 2e0a  on client-side..
-00003a40: 2a20 6062 7569 6c64 2829 6020 6d65 7468  * `build()` meth
-00003a50: 6f64 7320 6361 6e20 6e6f 7720 6861 6e64  ods can now hand
-00003a60: 6c65 2044 6f63 6b65 7266 696c 6573 2073  le Dockerfiles s
-00003a70: 7570 706c 6965 6420 6f75 7473 6964 6520  upplied outside 
-00003a80: 6f66 2074 6865 0a20 2062 7569 6c64 2063  of the.  build c
-00003a90: 6f6e 7465 7874 2e0a 2a20 4164 6465 6420  ontext..* Added 
-00003aa0: 6073 7061 7273 6560 2061 7267 756d 656e  `sparse` argumen
-00003ab0: 7420 746f 2060 446f 636b 6572 436c 6965  t to `DockerClie
-00003ac0: 6e74 2e63 6f6e 7461 696e 6572 732e 6c69  nt.containers.li
-00003ad0: 7374 2829 600a 2a20 4164 6465 6420 6069  st()`.* Added `i
-00003ae0: 736f 6c61 7469 6f6e 6020 7061 7261 6d65  solation` parame
-00003af0: 7465 7220 746f 2060 6275 696c 6428 2960  ter to `build()`
-00003b00: 206d 6574 686f 6473 2e0a 2a20 4164 6465   methods..* Adde
-00003b10: 6420 6063 6c6f 7365 2829 6020 6d65 7468  d `close()` meth
-00003b20: 6f64 2074 6f20 6044 6f63 6b65 7243 6c69  od to `DockerCli
-00003b30: 656e 7460 0a2a 2041 6464 6564 2060 4150  ent`.* Added `AP
-00003b40: 4943 6c69 656e 742e 696e 7370 6563 745f  IClient.inspect_
-00003b50: 6469 7374 7269 6275 7469 6f6e 2829 6020  distribution()` 
-00003b60: 6d65 7468 6f64 2061 6e64 0a20 2060 446f  method and.  `Do
-00003b70: 636b 6572 436c 6965 6e74 2e69 6d61 6765  ckerClient.image
-00003b80: 732e 6765 745f 7265 6769 7374 7279 5f64  s.get_registry_d
-00003b90: 6174 6128 2960 0a20 202a 2054 6865 206c  ata()`.  * The l
-00003ba0: 6174 7465 7220 7265 7475 726e 7320 616e  atter returns an
-00003bb0: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
-00003bc0: 206e 6577 2060 5265 6769 7374 7279 4461   new `RegistryDa
-00003bd0: 7461 6020 636c 6173 730a 0a33 2e31 2e34  ta` class..3.1.4
-00003be0: 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66  .-----..[List of
-00003bf0: 2050 5273 202f 2069 7373 7565 7320 666f   PRs / issues fo
-00003c00: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
-00003c10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003c20: 6f6d 2f64 6f63 6b65 722f 646f 636b 6572  om/docker/docker
-00003c30: 2d70 792f 6d69 6c65 7374 6f6e 652f 3438  -py/milestone/48
-00003c40: 3f63 6c6f 7365 643d 3129 0a0a 2323 2320  ?closed=1)..### 
-00003c50: 4275 6766 6978 6573 0a0a 2a20 4669 7865  Bugfixes..* Fixe
-00003c60: 6420 6120 6275 6720 7768 6572 6520 6275  d a bug where bu
-00003c70: 696c 6420 636f 6e74 6578 7473 2063 6f6e  ild contexts con
-00003c80: 7461 696e 696e 6720 6469 7265 6374 6f72  taining director
-00003c90: 7920 7379 6d6c 696e 6b73 2077 6f75 6c64  y symlinks would
-00003ca0: 2070 726f 6475 6365 0a20 2069 6e76 616c   produce.  inval
-00003cb0: 6964 2074 6172 2061 7263 6869 7665 730a  id tar archives.
-00003cc0: 0a33 2e31 2e33 0a2d 2d2d 2d2d 0a0a 2323  .3.1.3.-----..##
-00003cd0: 2320 4275 6766 6978 6573 0a0a 2a20 5265  # Bugfixes..* Re
-00003ce0: 6765 6e65 7261 7465 6420 696e 7661 6c69  generated invali
-00003cf0: 6420 7768 6565 6c20 7061 636b 6167 650a  d wheel package.
-00003d00: 0a33 2e31 2e32 0a2d 2d2d 2d2d 0a0a 5b4c  .3.1.2.-----..[L
-00003d10: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
-00003d20: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
-00003d30: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-00003d40: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
-00003d50: 646f 636b 6572 2d70 792f 6d69 6c65 7374  docker-py/milest
-00003d60: 6f6e 652f 3437 3f63 6c6f 7365 643d 3129  one/47?closed=1)
-00003d70: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-00003d80: 2a20 4669 7865 6420 6120 6275 6720 7468  * Fixed a bug th
-00003d90: 6174 206c 6564 2074 6f20 6120 446f 636b  at led to a Dock
-00003da0: 6572 6669 6c65 206e 6f74 2062 6569 6e67  erfile not being
-00003db0: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
-00003dc0: 2062 7569 6c64 2063 6f6e 7465 7874 0a20   build context. 
-00003dd0: 2069 6e20 736f 6d65 2073 6974 7561 7469   in some situati
-00003de0: 6f6e 7320 7768 656e 2074 6865 2044 6f63  ons when the Doc
-00003df0: 6b65 7266 696c 6527 7320 7061 7468 2077  kerfile's path w
-00003e00: 6173 2070 7265 6669 7865 6420 7769 7468  as prefixed with
-00003e10: 2060 2e2f 600a 0a33 2e31 2e31 0a2d 2d2d   `./`..3.1.1.---
-00003e20: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
-00003e30: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
-00003e40: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-00003e50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00003e60: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
-00003e70: 6d69 6c65 7374 6f6e 652f 3436 3f63 6c6f  milestone/46?clo
-00003e80: 7365 643d 3129 0a0a 2323 2320 4275 6766  sed=1)..### Bugf
-00003e90: 6978 6573 0a0a 2a20 4669 7865 6420 6120  ixes..* Fixed a 
-00003ea0: 6275 6720 7468 6174 2063 6175 7365 6420  bug that caused 
-00003eb0: 636f 7374 6c79 2044 4e53 206c 6f6f 6b75  costly DNS looku
-00003ec0: 7073 206f 6e20 4d61 6320 4f53 5820 7768  ps on Mac OSX wh
-00003ed0: 656e 2063 6f6e 6e65 6374 696e 6720 746f  en connecting to
-00003ee0: 2074 6865 0a20 2065 6e67 696e 6520 7468   the.  engine th
-00003ef0: 726f 7567 6820 554e 4958 2073 6f63 6b65  rough UNIX socke
-00003f00: 740a 2a20 4669 7865 6420 6120 6275 6720  t.* Fixed a bug 
-00003f10: 7468 6174 2063 6175 7365 6420 602e 646f  that caused `.do
-00003f20: 636b 6572 6967 6e6f 7265 6020 636f 6d6d  ckerignore` comm
-00003f30: 656e 7473 2074 6f20 6265 2072 6561 6420  ents to be read 
-00003f40: 6173 2065 7863 6c75 7369 6f6e 0a20 2070  as exclusion.  p
-00003f50: 6174 7465 726e 730a 0a33 2e31 2e30 0a2d  atterns..3.1.0.-
-00003f60: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-00003f70: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-00003f80: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-00003f90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003fa0: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-00003fb0: 792f 6d69 6c65 7374 6f6e 652f 3434 3f63  y/milestone/44?c
-00003fc0: 6c6f 7365 643d 3129 0a0a 2323 2320 4665  losed=1)..### Fe
-00003fd0: 6174 7572 6573 0a0a 2a20 4164 6465 6420  atures..* Added 
-00003fe0: 7375 7070 6f72 7420 666f 7220 6064 6576  support for `dev
-00003ff0: 6963 655f 6367 726f 7570 5f72 756c 6573  ice_cgroup_rules
-00004000: 6020 696e 2068 6f73 7420 636f 6e66 6967  ` in host config
-00004010: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-00004020: 2066 6f72 2060 6765 6e65 7269 635f 7265   for `generic_re
-00004030: 736f 7572 6365 7360 2077 6865 6e20 6372  sources` when cr
-00004040: 6561 7469 6e67 2061 2060 5265 736f 7572  eating a `Resour
-00004050: 6365 7360 0a20 206f 626a 6563 742e 0a2a  ces`.  object..*
-00004060: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-00004070: 6f72 2061 2063 6f6e 6669 6775 7261 626c  or a configurabl
-00004080: 6520 6063 6875 6e6b 5f73 697a 6560 2070  e `chunk_size` p
-00004090: 6172 616d 6574 6572 2069 6e20 6065 7870  arameter in `exp
-000040a0: 6f72 7460 2c0a 2020 6067 6574 5f61 7263  ort`,.  `get_arc
-000040b0: 6869 7665 6020 616e 6420 6067 6574 5f69  hive` and `get_i
-000040c0: 6d61 6765 6020 2860 496d 6167 652e 7361  mage` (`Image.sa
-000040d0: 7665 6029 0a2a 2041 6464 6564 2061 2060  ve`).* Added a `
-000040e0: 666f 7263 655f 7570 6461 7465 6020 6d65  force_update` me
-000040f0: 7468 6f64 2074 6f20 7468 6520 6053 6572  thod to the `Ser
-00004100: 7669 6365 6020 636c 6173 732e 0a2a 2049  vice` class..* I
-00004110: 6e20 6053 6572 7669 6365 2e75 7064 6174  n `Service.updat
-00004120: 6560 2c20 7768 656e 2074 6865 2060 666f  e`, when the `fo
-00004130: 7263 655f 7570 6461 7465 6020 7061 7261  rce_update` para
-00004140: 6d65 7465 7220 6973 2073 6574 2074 6f20  meter is set to 
-00004150: 6054 7275 6560 2c0a 2020 7468 6520 6375  `True`,.  the cu
-00004160: 7272 656e 7420 6066 6f72 6365 5f75 7064  rrent `force_upd
-00004170: 6174 6560 2063 6f75 6e74 6572 2069 7320  ate` counter is 
-00004180: 696e 6372 656d 656e 7465 6420 6279 206f  incremented by o
-00004190: 6e65 2069 6e20 7468 6520 7570 6461 7465  ne in the update
-000041a0: 0a20 2072 6571 7565 7374 2e0a 0a23 2323  .  request...###
-000041b0: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
-000041c0: 6564 2061 2062 7567 2077 6865 7265 2061  ed a bug where a
-000041d0: 7574 6865 6e74 6963 6174 696f 6e20 7468  uthentication th
-000041e0: 726f 7567 6820 606c 6f67 696e 2829 6020  rough `login()` 
-000041f0: 7761 7320 6265 696e 6720 6967 6e6f 7265  was being ignore
-00004200: 6420 6966 2074 6865 0a20 2053 444b 2077  d if the.  SDK w
-00004210: 6173 2063 6f6e 6669 6775 7265 6420 746f  as configured to
-00004220: 2075 7365 2061 2063 7265 6465 6e74 6961   use a credentia
-00004230: 6c20 7374 6f72 652e 0a2a 2046 6978 6564  l store..* Fixed
-00004240: 2061 2062 7567 2077 6865 7265 2064 6f77   a bug where dow
-00004250: 6e6c 6f61 6420 6d65 7468 6f64 7320 776f  nload methods wo
-00004260: 756c 6420 7573 6520 616e 2061 6273 7572  uld use an absur
-00004270: 646c 7920 736d 616c 6c20 6368 756e 6b20  dly small chunk 
-00004280: 7369 7a65 2c0a 2020 6c65 6164 696e 6720  size,.  leading 
-00004290: 746f 2073 6c6f 7720 6461 7461 2072 6574  to slow data ret
-000042a0: 7269 6576 616c 0a2a 2046 6978 6564 2061  rieval.* Fixed a
-000042b0: 2062 7567 2077 6865 7265 2075 7369 6e67   bug where using
-000042c0: 2060 446f 636b 6572 436c 6965 6e74 2e69   `DockerClient.i
-000042d0: 6d61 6765 732e 7075 6c6c 6020 746f 2070  mages.pull` to p
-000042e0: 756c 6c20 616e 2069 6d61 6765 2062 7920  ull an image by 
-000042f0: 6469 6765 7374 0a20 2077 6f75 6c64 206c  digest.  would l
-00004300: 6561 6420 746f 2061 6e20 6578 6365 7074  ead to an except
-00004310: 696f 6e20 6265 696e 6720 7261 6973 6564  ion being raised
-00004320: 2e0a 2a20 602e 646f 636b 6572 6967 6e6f  ..* `.dockerigno
-00004330: 7265 6020 7275 6c65 7320 7368 6f75 6c64  re` rules should
-00004340: 206e 6f77 2062 6520 7265 7370 6563 7465   now be respecte
-00004350: 6420 6173 2064 6566 696e 6564 2062 7920  d as defined by 
-00004360: 7468 6520 7370 6563 2c0a 2020 696e 636c  the spec,.  incl
-00004370: 7564 696e 6720 7265 7370 6563 7420 666f  uding respect fo
-00004380: 7220 6c61 7374 2d6c 696e 6520 7072 6563  r last-line prec
-00004390: 6564 656e 6365 2061 6e64 2070 726f 7065  edence and prope
-000043a0: 7220 6861 6e64 6c69 6e67 206f 6620 6162  r handling of ab
-000043b0: 736f 6c75 7465 0a20 2070 6174 6873 0a2a  solute.  paths.*
-000043c0: 2054 6865 2060 7061 7373 6020 6372 6564   The `pass` cred
-000043d0: 656e 7469 616c 2073 746f 7265 2069 7320  ential store is 
-000043e0: 6e6f 7720 7072 6f70 6572 6c79 2073 7570  now properly sup
-000043f0: 706f 7274 6564 2e0a 0a33 2e30 2e31 0a2d  ported...3.0.1.-
-00004400: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-00004410: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-00004420: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-00004430: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004440: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-00004450: 792f 6d69 6c65 7374 6f6e 652f 3433 3f63  y/milestone/43?c
-00004460: 6c6f 7365 643d 3129 0a0a 2323 2320 4275  losed=1)..### Bu
-00004470: 6766 6978 6573 0a0a 2a20 4669 7865 6420  gfixes..* Fixed 
-00004480: 6120 6275 6720 7768 6572 6520 6041 5049  a bug where `API
-00004490: 436c 6965 6e74 2e6c 6f67 696e 6020 6469  Client.login` di
-000044a0: 646e 2774 2070 6f70 756c 6174 6520 7468  dn't populate th
-000044b0: 6520 605f 6175 7468 5f63 6f6e 6669 6773  e `_auth_configs
-000044c0: 600a 2020 6469 6374 696f 6e61 7279 2070  `.  dictionary p
-000044d0: 726f 7065 726c 792c 2063 6175 7369 6e67  roperly, causing
-000044e0: 2073 7562 7365 7175 656e 7420 6070 756c   subsequent `pul
-000044f0: 6c60 2061 6e64 2060 7075 7368 6020 6f70  l` and `push` op
-00004500: 6572 6174 696f 6e73 2074 6f20 6661 696c  erations to fail
-00004510: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-00004520: 6865 7265 2073 6f6d 6520 6275 696c 6420  here some build 
-00004530: 636f 6e74 6578 7420 6669 6c65 7320 7765  context files we
-00004540: 7265 2069 6e63 6f72 7265 6374 6c79 2072  re incorrectly r
-00004550: 6563 6f67 6e69 7a65 6420 6173 0a20 2062  ecognized as.  b
-00004560: 6569 6e67 2069 6e61 6363 6573 7369 626c  eing inaccessibl
-00004570: 652e 0a2a 2046 6978 6564 2061 2062 7567  e..* Fixed a bug
-00004580: 2077 6865 7265 2066 696c 6573 2077 6974   where files wit
-00004590: 6820 6120 6e65 6761 7469 7665 206d 7469  h a negative mti
-000045a0: 6d65 2076 616c 7565 2077 6f75 6c64 0a20  me value would. 
-000045b0: 2063 6175 7365 2065 7272 6f72 7320 7768   cause errors wh
-000045c0: 656e 2069 6e63 6c75 6465 6420 696e 2061  en included in a
-000045d0: 2062 7569 6c64 2063 6f6e 7465 7874 0a0a   build context..
-000045e0: 332e 302e 300a 2d2d 2d2d 2d0a 0a5b 4c69  3.0.0.-----..[Li
-000045f0: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
-00004600: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
-00004610: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
-00004620: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
-00004630: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
-00004640: 6e65 2f33 393f 636c 6f73 6564 3d31 290a  ne/39?closed=1).
-00004650: 0a23 2323 2042 7265 616b 696e 6720 6368  .### Breaking ch
-00004660: 616e 6765 730a 0a2a 2053 7570 706f 7274  anges..* Support
-00004670: 2066 6f72 2041 5049 2076 6572 7369 6f6e   for API version
-00004680: 203c 2031 2e32 3120 6861 7320 6265 656e   < 1.21 has been
-00004690: 2072 656d 6f76 6564 2e0a 2a20 5468 6520   removed..* The 
-000046a0: 666f 6c6c 6f77 696e 6720 6d65 7468 6f64  following method
-000046b0: 7320 6861 7665 2062 6565 6e20 7265 6d6f  s have been remo
-000046c0: 7665 643a 0a20 202a 2060 4150 4943 6c69  ved:.  * `APICli
-000046d0: 656e 742e 636f 7079 6020 6861 7320 6265  ent.copy` has be
-000046e0: 656e 2072 656d 6f76 6564 2e20 5573 6572  en removed. User
-000046f0: 7320 7368 6f75 6c64 2075 7365 2060 4150  s should use `AP
-00004700: 4943 6c69 656e 742e 6765 745f 6172 6368  IClient.get_arch
-00004710: 6976 6560 0a20 2020 2069 6e73 7465 6164  ive`.    instead
-00004720: 2e0a 2020 2a20 6041 5049 436c 6965 6e74  ..  * `APIClient
-00004730: 2e69 6e73 6572 7460 2068 6173 2062 6565  .insert` has bee
-00004740: 6e20 7265 6d6f 7665 642e 2055 7365 7273  n removed. Users
-00004750: 206d 6179 2075 7365 2060 4150 4943 6c69   may use `APICli
-00004760: 656e 742e 7075 745f 6172 6368 6976 6560  ent.put_archive`
-00004770: 0a20 2020 2063 6f6d 6269 6e65 6420 7769  .    combined wi
-00004780: 7468 2060 4150 4943 6c69 656e 742e 636f  th `APIClient.co
-00004790: 6d6d 6974 6020 746f 2072 6570 6c69 6361  mmit` to replica
-000047a0: 7465 2074 6865 206d 6574 686f 6427 7320  te the method's 
-000047b0: 6265 6861 7669 6f72 2e0a 2020 2a20 6075  behavior..  * `u
-000047c0: 7469 6c73 2e70 696e 675f 7265 6769 7374  tils.ping_regist
-000047d0: 7279 6020 616e 6420 6075 7469 6c73 2e70  ry` and `utils.p
-000047e0: 696e 6760 2068 6176 6520 6265 656e 2072  ing` have been r
-000047f0: 656d 6f76 6564 2e0a 2a20 5468 6520 666f  emoved..* The fo
-00004800: 6c6c 6f77 696e 6720 7061 7261 6d65 7465  llowing paramete
-00004810: 7273 2068 6176 6520 6265 656e 2072 656d  rs have been rem
-00004820: 6f76 6564 3a0a 2020 2a20 6073 7472 6561  oved:.  * `strea
-00004830: 6d60 2069 6e20 6041 5049 436c 6965 6e74  m` in `APIClient
-00004840: 2e62 7569 6c64 600a 2020 2a20 6063 7075  .build`.  * `cpu
-00004850: 5f73 6861 7265 7360 2c20 6063 7075 7365  _shares`, `cpuse
-00004860: 7460 2c20 6064 6e73 602c 2060 6d65 6d5f  t`, `dns`, `mem_
-00004870: 6c69 6d69 7460 2c20 606d 656d 7377 6170  limit`, `memswap
-00004880: 5f6c 696d 6974 602c 0a20 2020 2060 766f  _limit`,.    `vo
-00004890: 6c75 6d65 5f64 7269 7665 7260 2c20 6076  lume_driver`, `v
-000048a0: 6f6c 756d 6573 5f66 726f 6d60 2069 6e20  olumes_from` in 
-000048b0: 6041 5049 436c 6965 6e74 2e63 7265 6174  `APIClient.creat
-000048c0: 655f 636f 6e74 6169 6e65 7260 2e20 5468  e_container`. Th
-000048d0: 6573 6520 6172 650a 2020 2020 616c 6c20  ese are.    all 
-000048e0: 7265 706c 6163 6564 2062 7920 7468 6569  replaced by thei
-000048f0: 7220 6571 7569 7661 6c65 6e74 2069 6e20  r equivalent in 
-00004900: 6063 7265 6174 655f 686f 7374 5f63 6f6e  `create_host_con
-00004910: 6669 6760 0a20 202a 2060 696e 7365 6375  fig`.  * `insecu
-00004920: 7265 5f72 6567 6973 7472 7960 2069 6e20  re_registry` in 
-00004930: 6041 5049 436c 6965 6e74 2e6c 6f67 696e  `APIClient.login
-00004940: 602c 2060 4150 4943 6c69 656e 742e 7075  `, `APIClient.pu
-00004950: 6c6c 602c 0a20 2020 2060 4150 4943 6c69  ll`,.    `APICli
-00004960: 656e 742e 7075 7368 602c 2060 446f 636b  ent.push`, `Dock
-00004970: 6572 436c 6965 6e74 2e69 6d61 6765 732e  erClient.images.
-00004980: 7075 7368 6020 616e 6420 6044 6f63 6b65  push` and `Docke
-00004990: 7243 6c69 656e 742e 696d 6167 6573 2e70  rClient.images.p
-000049a0: 756c 6c60 0a20 202a 2060 7669 7a60 2069  ull`.  * `viz` i
-000049b0: 6e20 6041 5049 436c 6965 6e74 2e69 6d61  n `APIClient.ima
-000049c0: 6765 7360 0a2a 2054 6865 2066 6f6c 6c6f  ges`.* The follo
-000049d0: 7769 6e67 2070 6172 616d 6574 6572 7320  wing parameters 
-000049e0: 6861 7665 2062 6565 6e20 7265 6e61 6d65  have been rename
-000049f0: 643a 0a20 202a 2060 656e 6470 6f69 6e74  d:.  * `endpoint
-00004a00: 5f63 6f6e 6669 6760 2069 6e20 6041 5049  _config` in `API
-00004a10: 436c 6965 6e74 2e63 7265 6174 655f 7365  Client.create_se
-00004a20: 7276 6963 6560 2061 6e64 0a20 2020 2060  rvice` and.    `
-00004a30: 4150 4943 6c69 656e 742e 7570 6461 7465  APIClient.update
-00004a40: 5f73 6572 7669 6365 6020 6973 206e 6f77  _service` is now
-00004a50: 2060 656e 6470 6f69 6e74 5f73 7065 6360   `endpoint_spec`
-00004a60: 0a20 202a 2060 6e61 6d65 6020 696e 2060  .  * `name` in `
-00004a70: 446f 636b 6572 436c 6965 6e74 2e69 6d61  DockerClient.ima
-00004a80: 6765 732e 7075 6c6c 6020 6973 206e 6f77  ges.pull` is now
-00004a90: 2060 7265 706f 7369 746f 7279 600a 2a20   `repository`.* 
-00004aa0: 5468 6520 7265 7475 726e 2076 616c 7565  The return value
-00004ab0: 2066 6f72 2074 6865 2066 6f6c 6c6f 7769   for the followi
-00004ac0: 6e67 206d 6574 686f 6473 2068 6173 2063  ng methods has c
-00004ad0: 6861 6e67 6564 3a0a 2020 2a20 6041 5049  hanged:.  * `API
-00004ae0: 436c 6965 6e74 2e77 6169 7460 2061 6e64  Client.wait` and
-00004af0: 2060 436f 6e74 6169 6e65 722e 7761 6974   `Container.wait
-00004b00: 6020 6e6f 7720 7265 7475 726e 2061 2060  ` now return a `
-00004b10: 6064 6963 7460 6020 7265 7072 6573 656e  `dict`` represen
-00004b20: 7469 6e67 0a20 2020 2074 6865 2041 5049  ting.    the API
-00004b30: 2773 2072 6573 706f 6e73 6520 696e 7374  's response inst
-00004b40: 6561 6420 6f66 2072 6574 7572 6e69 6e67  ead of returning
-00004b50: 2074 6865 2073 7461 7475 7320 636f 6465   the status code
-00004b60: 2064 6972 6563 746c 792e 0a20 202a 2060   directly..  * `
-00004b70: 446f 636b 6572 436c 6965 6e74 2e69 6d61  DockerClient.ima
-00004b80: 6765 732e 6c6f 6164 6020 6e6f 7720 7265  ges.load` now re
-00004b90: 7475 726e 7320 6120 6c69 7374 206f 6620  turns a list of 
-00004ba0: 6049 6d61 6765 6020 6f62 6a65 6374 7320  `Image` objects 
-00004bb0: 7468 6174 2068 6176 650a 2020 2020 666f  that have.    fo
-00004bc0: 7220 7468 6520 696d 6167 6573 2074 6861  r the images tha
-00004bd0: 7420 7765 7265 206c 6f61 6465 642c 2069  t were loaded, i
-00004be0: 6e73 7465 6164 206f 6620 6120 6c6f 6720  nstead of a log 
-00004bf0: 7374 7265 616d 2e0a 2020 2a20 6043 6f6e  stream..  * `Con
-00004c00: 7461 696e 6572 2e65 7865 635f 7275 6e60  tainer.exec_run`
-00004c10: 206e 6f77 2072 6574 7572 6e73 2061 2074   now returns a t
-00004c20: 7570 6c65 206f 6620 2865 7869 745f 636f  uple of (exit_co
-00004c30: 6465 2c20 6f75 7470 7574 2920 696e 7374  de, output) inst
-00004c40: 6561 6420 6f66 0a20 2020 206a 7573 7420  ead of.    just 
-00004c50: 7468 6520 6f75 7470 7574 2e0a 2020 2a20  the output..  * 
-00004c60: 6044 6f63 6b65 7243 6c69 656e 742e 696d  `DockerClient.im
-00004c70: 6167 6573 2e62 7569 6c64 6020 6e6f 7720  ages.build` now 
-00004c80: 7265 7475 726e 7320 6120 7475 706c 6520  returns a tuple 
-00004c90: 6f66 2028 696d 6167 652c 2062 7569 6c64  of (image, build
-00004ca0: 5f6c 6f67 7329 0a20 2020 2069 6e73 7465  _logs).    inste
-00004cb0: 6164 206f 6620 6a75 7374 2074 6865 2069  ad of just the i
-00004cc0: 6d61 6765 206f 626a 6563 742e 0a20 202a  mage object..  *
-00004cd0: 2060 4150 4943 6c69 656e 742e 6578 706f   `APIClient.expo
-00004ce0: 7274 602c 2060 4150 4943 6c69 656e 742e  rt`, `APIClient.
-00004cf0: 6765 745f 6172 6368 6976 6560 2061 6e64  get_archive` and
-00004d00: 2060 4150 4943 6c69 656e 742e 6765 745f   `APIClient.get_
-00004d10: 696d 6167 6560 206e 6f77 0a20 2020 2072  image` now.    r
-00004d20: 6574 7572 6e20 6765 6e65 7261 746f 7273  eturn generators
-00004d30: 2073 7472 6561 6d69 6e67 2074 6865 2072   streaming the r
-00004d40: 6177 2062 696e 6172 7920 6461 7461 2066  aw binary data f
-00004d50: 726f 6d20 7468 6520 7365 7276 6572 2773  rom the server's
-00004d60: 2072 6573 706f 6e73 652e 0a20 202a 2057   response..  * W
-00004d70: 6865 6e20 6e6f 2074 6167 2069 7320 7072  hen no tag is pr
-00004d80: 6f76 6964 6564 2c20 6044 6f63 6b65 7243  ovided, `DockerC
-00004d90: 6c69 656e 742e 696d 6167 6573 2e70 756c  lient.images.pul
-00004da0: 6c60 206e 6f77 2072 6574 7572 6e73 2061  l` now returns a
-00004db0: 206c 6973 7420 6f66 0a20 2020 2060 496d   list of.    `Im
-00004dc0: 6167 6560 7320 6173 736f 6369 6174 6564  age`s associated
-00004dd0: 2074 6f20 7468 6520 7075 6c6c 6564 2072   to the pulled r
-00004de0: 6570 6f73 6974 6f72 7920 696e 7374 6561  epository instea
-00004df0: 6420 6f66 206a 7573 7420 7468 6520 606c  d of just the `l
-00004e00: 6174 6573 7460 0a20 2020 2069 6d61 6765  atest`.    image
-00004e10: 2e0a 0a23 2323 2046 6561 7475 7265 730a  ...### Features.
-00004e20: 0a2a 2054 6865 2044 6f63 6b65 7220 5079  .* The Docker Py
-00004e30: 7468 6f6e 2053 444b 2069 7320 6e6f 7720  thon SDK is now 
-00004e40: 6f66 6669 6369 616c 6c79 2073 7570 706f  officially suppo
-00004e50: 7274 6564 206f 6e20 5079 7468 6f6e 2033  rted on Python 3
-00004e60: 2e36 0a2a 2041 6464 6564 2060 7363 616c  .6.* Added `scal
-00004e70: 6560 206d 6574 686f 6420 746f 2074 6865  e` method to the
-00004e80: 2060 5365 7276 6963 6560 206d 6f64 656c   `Service` model
-00004e90: 203b 2074 6869 7320 6d65 7468 6f64 2069   ; this method i
-00004ea0: 7320 6120 7368 6f72 7468 616e 640a 2020  s a shorthand.  
-00004eb0: 7468 6174 2063 616c 6c73 2060 7570 6461  that calls `upda
-00004ec0: 7465 5f73 6572 7669 6365 6020 7769 7468  te_service` with
-00004ed0: 2074 6865 2072 6571 7569 7265 6420 6e75   the required nu
-00004ee0: 6d62 6572 206f 6620 7265 706c 6963 6173  mber of replicas
-00004ef0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-00004f00: 2066 6f72 2074 6865 2060 706c 6174 666f   for the `platfo
-00004f10: 726d 6020 7061 7261 6d65 7465 7220 696e  rm` parameter in
-00004f20: 2060 4150 4943 6c69 656e 742e 6275 696c   `APIClient.buil
-00004f30: 6460 2c0a 2020 6044 6f63 6b65 7243 6c69  d`,.  `DockerCli
-00004f40: 656e 742e 696d 6167 6573 2e62 7569 6c64  ent.images.build
-00004f50: 602c 2060 4150 4943 6c69 656e 742e 7075  `, `APIClient.pu
-00004f60: 6c6c 6020 616e 6420 6044 6f63 6b65 7243  ll` and `DockerC
-00004f70: 6c69 656e 742e 696d 6167 6573 2e70 756c  lient.images.pul
-00004f80: 6c60 0a2a 2041 6464 6564 2073 7570 706f  l`.* Added suppo
-00004f90: 7274 2066 6f72 2074 6865 2060 756e 7469  rt for the `unti
-00004fa0: 6c60 2070 6172 616d 6574 6572 2069 6e20  l` parameter in 
-00004fb0: 6041 5049 436c 6965 6e74 2e6c 6f67 7360  `APIClient.logs`
-00004fc0: 2061 6e64 0a20 2060 436f 6e74 6169 6e65   and.  `Containe
-00004fd0: 722e 6c6f 6773 600a 2a20 4164 6465 6420  r.logs`.* Added 
-00004fe0: 7375 7070 6f72 7420 666f 7220 7468 6520  support for the 
-00004ff0: 6077 6f72 6b64 6972 6020 6172 6775 6d65  `workdir` argume
-00005000: 6e74 2069 6e20 6041 5049 436c 6965 6e74  nt in `APIClient
-00005010: 2e65 7865 635f 6372 6561 7465 6020 616e  .exec_create` an
-00005020: 640a 2020 6043 6f6e 7461 696e 6572 2e65  d.  `Container.e
-00005030: 7865 635f 7275 6e60 0a2a 2041 6464 6564  xec_run`.* Added
-00005040: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
-00005050: 2060 636f 6e64 6974 696f 6e60 2061 7267   `condition` arg
-00005060: 756d 656e 7420 696e 2060 4150 4943 6c69  ument in `APICli
-00005070: 656e 742e 7761 6974 6020 616e 640a 2020  ent.wait` and.  
-00005080: 6043 6f6e 7461 696e 6572 2e77 6169 7460  `Container.wait`
-00005090: 0a2a 2055 7365 7273 2063 616e 206e 6f77  .* Users can now
-000050a0: 2073 7065 6369 6679 2061 2070 7562 6c69   specify a publi
-000050b0: 7368 206d 6f64 6520 666f 7220 706f 7274  sh mode for port
-000050c0: 7320 696e 2060 456e 6470 6f69 6e74 5370  s in `EndpointSp
-000050d0: 6563 6020 7573 696e 670a 2020 7468 6520  ec` using.  the 
-000050e0: 607b 7075 626c 6973 6865 645f 706f 7274  `{published_port
-000050f0: 3a20 2874 6172 6765 745f 706f 7274 2c20  : (target_port, 
-00005100: 7072 6f74 6f63 6f6c 2c20 7075 626c 6973  protocol, publis
-00005110: 685f 6d6f 6465 297d 6020 7379 6e74 6178  h_mode)}` syntax
-00005120: 2e0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
-00005130: 7420 666f 7220 7468 6520 6069 736f 6c61  t for the `isola
-00005140: 7469 6f6e 6020 7061 7261 6d65 7465 7220  tion` parameter 
-00005150: 696e 2060 436f 6e74 6169 6e65 7253 7065  in `ContainerSpe
-00005160: 6360 2c0a 2020 6044 6f63 6b65 7243 6c69  c`,.  `DockerCli
-00005170: 656e 742e 7365 7276 6963 6573 2e63 7265  ent.services.cre
-00005180: 6174 6560 2061 6e64 2060 5365 7276 6963  ate` and `Servic
-00005190: 652e 7570 6461 7465 600a 2a20 6041 5049  e.update`.* `API
-000051a0: 436c 6965 6e74 2e61 7474 6163 685f 736f  Client.attach_so
-000051b0: 636b 6574 602c 2060 4150 4943 6c69 656e  cket`, `APIClien
-000051c0: 742e 6578 6563 5f63 7265 6174 6560 206e  t.exec_create` n
-000051d0: 6f77 2061 6c6c 6f77 2073 7065 6369 6679  ow allow specify
-000051e0: 696e 6720 610a 2020 6064 6574 6163 685f  ing a.  `detach_
-000051f0: 6b65 7973 6020 636f 6d62 696e 6174 696f  keys` combinatio
-00005200: 6e2e 2049 6620 756e 7370 6563 6966 6965  n. If unspecifie
-00005210: 642c 2074 6865 2076 616c 7565 2066 726f  d, the value fro
-00005220: 6d20 7468 6520 6063 6f6e 6669 672e 6a73  m the `config.js
-00005230: 6f6e 600a 2020 6669 6c65 2077 696c 6c20  on`.  file will 
-00005240: 6265 2075 7365 640a 2a20 544c 5320 636f  be used.* TLS co
-00005250: 6e6e 6563 7469 6f6e 7320 6e6f 7720 6465  nnections now de
-00005260: 6661 756c 7420 746f 2075 7369 6e67 2074  fault to using t
-00005270: 6865 2054 4c53 7631 2e32 2070 726f 746f  he TLSv1.2 proto
-00005280: 636f 6c20 7768 656e 2061 7661 696c 6162  col when availab
-00005290: 6c65 0a0a 0a23 2323 2042 7567 6669 7865  le...### Bugfixe
-000052a0: 730a 0a2a 2046 6978 6564 2061 2062 7567  s..* Fixed a bug
-000052b0: 2077 6865 7265 2077 6869 7465 7370 6163   where whitespac
-000052c0: 652d 6f6e 6c79 206c 696e 6573 2069 6e20  e-only lines in 
-000052d0: 602e 646f 636b 6572 6967 6e6f 7265 6020  `.dockerignore` 
-000052e0: 776f 756c 6420 6272 6561 6b20 6275 696c  would break buil
-000052f0: 6473 0a20 206f 6e20 5769 6e64 6f77 730a  ds.  on Windows.
-00005300: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-00005310: 6572 6520 6272 6f6b 656e 2073 796d 6c69  ere broken symli
-00005320: 6e6b 7320 696e 7369 6465 2061 2062 7569  nks inside a bui
-00005330: 6c64 2063 6f6e 7465 7874 2077 6f75 6c64  ld context would
-00005340: 2063 6175 7365 2074 6865 0a20 2062 7569   cause the.  bui
-00005350: 6c64 2074 6f20 6661 696c 0a2a 2046 6978  ld to fail.* Fix
-00005360: 6564 2061 2062 7567 2077 6865 7265 2073  ed a bug where s
-00005370: 7065 6369 6679 696e 6720 766f 6c75 6d65  pecifying volume
-00005380: 7320 7769 7468 2057 696e 646f 7773 2064  s with Windows d
-00005390: 7269 7665 7320 776f 756c 6420 6361 7573  rives would caus
-000053a0: 650a 2020 696e 636f 7272 6563 7420 7061  e.  incorrect pa
-000053b0: 7273 696e 6720 696e 2060 446f 636b 6572  rsing in `Docker
-000053c0: 436c 6965 6e74 2e63 6f6e 7461 696e 6572  Client.container
-000053d0: 732e 7275 6e60 0a2a 2046 6978 6564 2061  s.run`.* Fixed a
-000053e0: 2062 7567 2077 6865 7265 2074 6865 2060   bug where the `
-000053f0: 6e65 7477 6f72 6b73 6020 6461 7461 2070  networks` data p
-00005400: 726f 7669 6465 6420 746f 2060 6372 6561  rovided to `crea
-00005410: 7465 5f73 6572 7669 6365 6020 616e 640a  te_service` and.
-00005420: 2020 6075 7064 6174 655f 7365 7276 6963    `update_servic
-00005430: 6560 2077 6f75 6c64 2062 6520 7365 6e74  e` would be sent
-00005440: 2069 6e63 6f72 7265 6374 6c79 2074 6f20   incorrectly to 
-00005450: 7468 6520 456e 6769 6e65 2077 6974 6820  the Engine with 
-00005460: 4150 4920 3c20 312e 3235 0a2a 2050 756c  API < 1.25.* Pul
-00005470: 6c69 6e67 2061 6c6c 2074 6167 7320 6672  ling all tags fr
-00005480: 6f6d 2061 2072 6570 6f73 6974 6f72 7920  om a repository 
-00005490: 7769 7468 206e 6f20 606c 6174 6573 7460  with no `latest`
-000054a0: 2074 6167 2075 7369 6e67 2074 6865 0a20   tag using the. 
-000054b0: 2060 446f 636b 6572 436c 6965 6e74 6020   `DockerClient` 
-000054c0: 7769 6c6c 206e 6f20 6c6f 6e67 6572 2072  will no longer r
-000054d0: 6169 7365 2061 2060 4e6f 7446 6f75 6e64  aise a `NotFound
-000054e0: 6020 6578 6365 7074 696f 6e0a 0a32 2e37  ` exception..2.7
-000054f0: 2e30 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420  .0.-----..[List 
-00005500: 6f66 2050 5273 202f 2069 7373 7565 7320  of PRs / issues 
-00005510: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
-00005520: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005530: 2e63 6f6d 2f64 6f63 6b65 722f 646f 636b  .com/docker/dock
-00005540: 6572 2d70 792f 6d69 6c65 7374 6f6e 652f  er-py/milestone/
-00005550: 3431 3f63 6c6f 7365 643d 3129 0a0a 2323  41?closed=1)..##
-00005560: 2320 4665 6174 7572 6573 0a0a 2a20 4164  # Features..* Ad
-00005570: 6465 6420 6075 6e6c 6f63 6b5f 7377 6172  ded `unlock_swar
-00005580: 6d60 2061 6e64 2060 6765 745f 756e 6c6f  m` and `get_unlo
-00005590: 636b 5f6b 6579 6020 6d65 7468 6f64 7320  ck_key` methods 
-000055a0: 746f 2074 6865 2060 4150 4943 6c69 656e  to the `APIClien
-000055b0: 7460 2e0a 2020 2020 2a20 4164 6465 6420  t`..    * Added 
-000055c0: 6075 6e6c 6f63 6b60 2061 6e64 2060 6765  `unlock` and `ge
-000055d0: 745f 756e 6c6f 636b 5f6b 6579 6020 746f  t_unlock_key` to
-000055e0: 2060 446f 636b 6572 436c 6965 6e74 2e73   `DockerClient.s
-000055f0: 7761 726d 602e 0a2a 2041 6464 6564 2061  warm`..* Added a
-00005600: 2060 6772 6565 6479 6020 7061 7261 6d65   `greedy` parame
-00005610: 7465 7220 746f 2060 446f 636b 6572 436c  ter to `DockerCl
-00005620: 6965 6e74 2e6e 6574 776f 726b 732e 6c69  ient.networks.li
-00005630: 7374 602c 2079 6965 6c64 696e 670a 2020  st`, yielding.  
-00005640: 6164 6469 7469 6f6e 616c 2064 6574 6169  additional detai
-00005650: 6c73 2061 626f 7574 2074 6865 206c 6973  ls about the lis
-00005660: 7465 6420 6e65 7477 6f72 6b73 2e0a 2a20  ted networks..* 
-00005670: 4164 6465 6420 6063 7075 5f72 745f 7275  Added `cpu_rt_ru
-00005680: 6e74 696d 6560 2061 6e64 2060 6370 755f  ntime` and `cpu_
-00005690: 7274 5f70 6572 696f 6460 2061 7320 7061  rt_period` as pa
-000056a0: 7261 6d65 7465 7273 2074 6f0a 2020 6041  rameters to.  `A
-000056b0: 5049 436c 6965 6e74 2e63 7265 6174 655f  PIClient.create_
-000056c0: 686f 7374 5f63 6f6e 6669 6760 2061 6e64  host_config` and
-000056d0: 2060 446f 636b 6572 436c 6965 6e74 2e63   `DockerClient.c
-000056e0: 6f6e 7461 696e 6572 732e 7275 6e60 2e0a  ontainers.run`..
-000056f0: 2a20 4164 6465 6420 7468 6520 606f 7264  * Added the `ord
-00005700: 6572 6020 6172 6775 6d65 6e74 2074 6f20  er` argument to 
-00005710: 6055 7064 6174 6543 6f6e 6669 6760 2e0a  `UpdateConfig`..
-00005720: 2a20 4164 6465 6420 6066 6574 6368 5f63  * Added `fetch_c
-00005730: 7572 7265 6e74 5f73 7065 6360 2074 6f20  urrent_spec` to 
-00005740: 6041 5049 436c 6965 6e74 2e75 7064 6174  `APIClient.updat
-00005750: 655f 7365 7276 6963 6560 2061 6e64 2060  e_service` and `
-00005760: 5365 7276 6963 652e 7570 6461 7465 600a  Service.update`.
-00005770: 2020 7468 6174 2077 696c 6c20 7265 7472    that will retr
-00005780: 6965 7665 2074 6865 2063 7572 7265 6e74  ieve the current
-00005790: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
-000057a0: 6620 7468 6520 7365 7276 6963 6520 616e  f the service an
-000057b0: 6420 6d65 7267 6520 6974 2077 6974 680a  d merge it with.
-000057c0: 2020 7468 6520 7072 6f76 6964 6564 2070    the provided p
-000057d0: 6172 616d 6574 6572 7320 746f 2064 6574  arameters to det
-000057e0: 6572 6d69 6e65 2074 6865 206e 6577 2063  ermine the new c
-000057f0: 6f6e 6669 6775 7261 7469 6f6e 2e0a 0a23  onfiguration...#
-00005800: 2323 2042 7567 6669 7865 730a 0a2a 2046  ## Bugfixes..* F
-00005810: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
-00005820: 2074 6865 2060 6275 696c 6460 206d 6574   the `build` met
-00005830: 686f 6420 7472 6965 6420 746f 2069 6e63  hod tried to inc
-00005840: 6c75 6465 2069 6e61 6363 6573 7369 626c  lude inaccessibl
-00005850: 6520 6669 6c65 730a 2020 696e 2074 6865  e files.  in the
-00005860: 2063 6f6e 7465 7874 2c20 6c65 6164 696e   context, leadin
-00005870: 6720 746f 206f 6273 6375 7265 2065 7272  g to obscure err
-00005880: 6f72 7320 6475 7269 6e67 2074 6865 2062  ors during the b
-00005890: 7569 6c64 2070 6861 7365 0a20 2028 696e  uild phase.  (in
-000058a0: 6163 6365 7373 6962 6c65 2066 696c 6573  accessible files
-000058b0: 2069 6e73 6964 6520 7468 6520 636f 6e74   inside the cont
-000058c0: 6578 7420 6e6f 7720 7261 6973 6520 616e  ext now raise an
-000058d0: 2060 494f 4572 726f 7260 2069 6e73 7465   `IOError` inste
-000058e0: 6164 292e 0a2a 2046 6978 6564 2061 2062  ad)..* Fixed a b
-000058f0: 7567 2077 6865 7265 2074 6865 2060 6275  ug where the `bu
-00005900: 696c 6460 206d 6574 686f 6420 776f 756c  ild` method woul
-00005910: 6420 7472 7920 746f 2072 6561 6420 6672  d try to read fr
-00005920: 6f6d 2046 4946 4f73 2070 7265 7365 6e74  om FIFOs present
-00005930: 0a20 2069 6e73 6964 6520 7468 6520 6275  .  inside the bu
-00005940: 696c 6420 636f 6e74 6578 742c 2063 6175  ild context, cau
-00005950: 7369 6e67 2069 7420 746f 2068 616e 672e  sing it to hang.
-00005960: 0a2a 2060 4150 4943 6c69 656e 742e 7374  .* `APIClient.st
-00005970: 6f70 6020 7769 6c6c 206e 6f20 6c6f 6e67  op` will no long
-00005980: 6572 206f 7665 7272 6964 6520 7468 6520  er override the 
-00005990: 6073 746f 705f 7469 6d65 6f75 7460 2076  `stop_timeout` v
-000059a0: 616c 7565 2070 7265 7365 6e74 0a20 2069  alue present.  i
-000059b0: 6e20 7468 6520 636f 6e74 6169 6e65 7227  n the container'
-000059c0: 7320 636f 6e66 6967 7572 6174 696f 6e2e  s configuration.
-000059d0: 0a2a 2046 6978 6564 2061 2062 7567 2070  .* Fixed a bug p
-000059e0: 7265 7665 6e74 696e 6720 7265 6d6f 7661  reventing remova
-000059f0: 6c20 6f66 206e 6574 776f 726b 7320 7769  l of networks wi
-00005a00: 7468 206e 616d 6573 2063 6f6e 7461 696e  th names contain
-00005a10: 696e 6720 6120 7370 6163 652e 0a2a 2046  ing a space..* F
-00005a20: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
-00005a30: 2060 446f 636b 6572 436c 6965 6e74 2e63   `DockerClient.c
-00005a40: 6f6e 7461 696e 6572 732e 7275 6e60 2077  ontainers.run` w
-00005a50: 6f75 6c64 2063 7261 7368 2069 6620 7468  ould crash if th
-00005a60: 650a 2020 6061 7574 6f5f 7265 6d6f 7665  e.  `auto_remove
-00005a70: 6020 7061 7261 6d65 7465 7220 7761 7320  ` parameter was 
-00005a80: 7365 7420 746f 2060 5472 7565 602e 0a2a  set to `True`..*
-00005a90: 2043 6861 6e67 6564 2074 6865 2064 6566   Changed the def
-00005aa0: 6175 6c74 2076 616c 7565 206f 6620 606c  ault value of `l
-00005ab0: 6973 7465 6e5f 6164 6472 6020 696e 2060  isten_addr` in `
-00005ac0: 6a6f 696e 5f73 7761 726d 6020 746f 206d  join_swarm` to m
-00005ad0: 6174 6368 2074 6865 0a20 206f 6e65 2069  atch the.  one i
-00005ae0: 6e20 6069 6e69 745f 7377 6172 6d60 2e0a  n `init_swarm`..
-00005af0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-00005b00: 6572 6520 6861 6e64 6c69 6e67 2048 5454  ere handling HTT
-00005b10: 5020 6572 726f 7273 2077 6974 6820 6e6f  P errors with no
-00005b20: 2062 6f64 7920 776f 756c 6420 6361 7573   body would caus
-00005b30: 6520 616e 2075 6e65 7870 6563 7465 640a  e an unexpected.
-00005b40: 2020 6578 6365 7074 696f 6e20 746f 2062    exception to b
-00005b50: 6520 7468 726f 776e 2077 6869 6c65 2067  e thrown while g
-00005b60: 656e 6572 6174 696e 6720 616e 2060 4150  enerating an `AP
-00005b70: 4945 7272 6f72 6020 6f62 6a65 6374 2e0a  IError` object..
-00005b80: 0a32 2e36 2e31 0a2d 2d2d 2d2d 0a0a 5b4c  .2.6.1.-----..[L
-00005b90: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
-00005ba0: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
-00005bb0: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-00005bc0: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
-00005bd0: 646f 636b 6572 2d70 792f 6d69 6c65 7374  docker-py/milest
-00005be0: 6f6e 652f 3430 3f63 6c6f 7365 643d 3129  one/40?closed=1)
-00005bf0: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-00005c00: 2a20 4669 7865 6420 6120 6275 6720 6f6e  * Fixed a bug on
-00005c10: 2050 7974 686f 6e20 3320 696e 7374 616c   Python 3 instal
-00005c20: 6c61 7469 6f6e 7320 7072 6576 656e 7469  lations preventi
-00005c30: 6e67 2074 6865 2075 7365 206f 6620 7468  ng the use of th
-00005c40: 6520 6061 7474 6163 6860 2061 6e64 0a20  e `attach` and. 
-00005c50: 2060 6578 6563 5f72 756e 6020 6d65 7468   `exec_run` meth
-00005c60: 6f64 732e 0a0a 0a32 2e36 2e30 0a2d 2d2d  ods....2.6.0.---
-00005c70: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
-00005c80: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
-00005c90: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-00005ca0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00005cb0: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
-00005cc0: 6d69 6c65 7374 6f6e 652f 3338 3f63 6c6f  milestone/38?clo
-00005cd0: 7365 643d 3129 0a0a 2323 2320 4665 6174  sed=1)..### Feat
-00005ce0: 7572 6573 0a0a 2a20 4164 6465 6420 7375  ures..* Added su
-00005cf0: 7070 6f72 7420 666f 7220 606d 6f75 6e74  pport for `mount
-00005d00: 7360 2069 6e20 6041 5049 436c 6965 6e74  s` in `APIClient
-00005d10: 2e63 7265 6174 655f 686f 7374 5f63 6f6e  .create_host_con
-00005d20: 6669 6760 2061 6e64 0a20 2060 446f 636b  fig` and.  `Dock
-00005d30: 6572 436c 6965 6e74 2e63 6f6e 7461 696e  erClient.contain
-00005d40: 6572 732e 7275 6e60 0a2a 2041 6464 6564  ers.run`.* Added
-00005d50: 2073 7570 706f 7274 2066 6f72 2060 636f   support for `co
-00005d60: 6e73 6973 7465 6e63 7960 2c20 6074 6d70  nsistency`, `tmp
-00005d70: 6673 5f73 697a 6560 2061 6e64 2060 746d  fs_size` and `tm
-00005d80: 7066 735f 6d6f 6465 6020 7768 656e 0a20  pfs_mode` when. 
-00005d90: 2063 7265 6174 696e 6720 6d6f 756e 7420   creating mount 
-00005da0: 6f62 6a65 6374 732e 0a2a 2060 4d6f 756e  objects..* `Moun
-00005db0: 7460 206f 626a 6563 7473 206e 6f77 2073  t` objects now s
-00005dc0: 7570 706f 7274 2074 6865 2060 746d 7066  upport the `tmpf
-00005dd0: 7360 2061 6e64 2060 6e70 6970 6560 2074  s` and `npipe` t
-00005de0: 7970 6573 2e0a 2a20 4164 6465 6420 7375  ypes..* Added su
-00005df0: 7070 6f72 7420 666f 7220 6065 7874 7261  pport for `extra
-00005e00: 5f68 6f73 7473 6020 696e 2074 6865 2060  _hosts` in the `
-00005e10: 6275 696c 6460 206d 6574 686f 6473 2e0a  build` methods..
-00005e20: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-00005e30: 666f 7220 7468 6520 636f 6e66 6967 7320  for the configs 
-00005e40: 4150 493a 0a20 2020 202a 2049 6e20 6041  API:.    * In `A
-00005e50: 5049 436c 6965 6e74 603a 2060 6372 6561  PIClient`: `crea
-00005e60: 7465 5f63 6f6e 6669 6760 2c20 6069 6e73  te_config`, `ins
-00005e70: 7065 6374 5f63 6f6e 6669 6760 2c20 6072  pect_config`, `r
-00005e80: 656d 6f76 655f 636f 6e66 6967 602c 0a20  emove_config`,. 
-00005e90: 2020 2020 2060 636f 6e66 6967 7360 0a20       `configs`. 
-00005ea0: 2020 202a 2049 6e20 6044 6f63 6b65 7243     * In `DockerC
-00005eb0: 6c69 656e 7460 3a20 6063 6f6e 6669 6773  lient`: `configs
-00005ec0: 2e63 7265 6174 6560 2c20 6063 6f6e 6669  .create`, `confi
-00005ed0: 6773 2e67 6574 602c 2060 636f 6e66 6967  gs.get`, `config
-00005ee0: 732e 6c69 7374 6020 616e 640a 2020 2020  s.list` and.    
-00005ef0: 2020 7468 6520 6043 6f6e 6669 6760 206d    the `Config` m
-00005f00: 6f64 656c 2e0a 2020 2020 2a20 4164 6465  odel..    * Adde
-00005f10: 6420 6063 6f6e 6669 6773 6020 7061 7261  d `configs` para
-00005f20: 6d65 7465 7220 746f 2060 436f 6e74 6169  meter to `Contai
-00005f30: 6e65 7253 7065 6360 2e20 4561 6368 2069  nerSpec`. Each i
-00005f40: 7465 6d20 696e 2074 6865 2060 636f 6e66  tem in the `conf
-00005f50: 6967 7360 0a20 2020 2020 206c 6973 7420  igs`.      list 
-00005f60: 6d75 7374 2062 6520 6120 6064 6f63 6b65  must be a `docke
-00005f70: 722e 7479 7065 732e 436f 6e66 6967 5265  r.types.ConfigRe
-00005f80: 6665 7265 6e63 6560 2069 6e73 7461 6e63  ference` instanc
-00005f90: 652e 0a2a 2041 6464 6564 2073 7570 706f  e..* Added suppo
-00005fa0: 7274 2066 6f72 2074 6865 2066 6f6c 6c6f  rt for the follo
-00005fb0: 7769 6e67 2070 6172 616d 6574 6572 7320  wing parameters 
-00005fc0: 7768 656e 2063 7265 6174 696e 6720 6120  when creating a 
-00005fd0: 6043 6f6e 7461 696e 6572 5370 6563 600a  `ContainerSpec`.
-00005fe0: 2020 6f62 6a65 6374 3a20 6067 726f 7570    object: `group
-00005ff0: 7360 2c20 606f 7065 6e5f 7374 6469 6e60  s`, `open_stdin`
-00006000: 2c20 6072 6561 645f 6f6e 6c79 602c 2060  , `read_only`, `
-00006010: 7374 6f70 5f73 6967 6e61 6c60 2c20 6068  stop_signal`, `h
-00006020: 656c 6174 6863 6865 636b 602c 0a20 2060  elathcheck`,.  `
-00006030: 686f 7374 7360 2c20 606e 735f 636f 6e66  hosts`, `ns_conf
-00006040: 6967 602c 2060 636f 6e66 6967 7360 2c20  ig`, `configs`, 
-00006050: 6070 7269 7669 6c65 6765 7360 2e0a 2a20  `privileges`..* 
-00006060: 4164 6465 6420 7468 6520 666f 6c6c 6f77  Added the follow
-00006070: 696e 6720 636f 6e66 6967 7572 6174 696f  ing configuratio
-00006080: 6e20 636c 6173 7365 7320 746f 2060 646f  n classes to `do
-00006090: 636b 6572 2e74 7970 6573 603a 0a20 2060  cker.types`:.  `
-000060a0: 436f 6e66 6967 5265 6665 7265 6e63 6560  ConfigReference`
-000060b0: 2c20 6044 4e53 436f 6e66 6967 602c 2060  , `DNSConfig`, `
-000060c0: 5072 6976 696c 6567 6573 602c 2060 5377  Privileges`, `Sw
-000060d0: 6172 6d45 7874 6572 6e61 6c43 4160 2e0a  armExternalCA`..
-000060e0: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-000060f0: 666f 7220 6064 7269 7665 7260 2069 6e20  for `driver` in 
-00006100: 6041 5049 436c 6965 6e74 2e63 7265 6174  `APIClient.creat
-00006110: 655f 7365 6372 6574 6020 616e 640a 2020  e_secret` and.  
-00006120: 6044 6f63 6b65 7243 6c69 656e 742e 7365  `DockerClient.se
-00006130: 6372 6574 732e 6372 6561 7465 602e 0a2a  crets.create`..*
-00006140: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-00006150: 6f72 2060 7363 6f70 6560 2069 6e20 6041  or `scope` in `A
-00006160: 5049 436c 6965 6e74 2e69 6e73 7065 6374  PIClient.inspect
-00006170: 5f6e 6574 776f 726b 6020 616e 640a 2020  _network` and.  
-00006180: 6041 5049 436c 6965 6e74 2e63 7265 6174  `APIClient.creat
-00006190: 655f 6e65 7477 6f72 6b60 2c20 616e 6420  e_network`, and 
-000061a0: 7468 6569 7220 6044 6f63 6b65 7243 6c69  their `DockerCli
-000061b0: 656e 7460 2065 7175 6976 616c 656e 742e  ent` equivalent.
-000061c0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-000061d0: 2066 6f72 2074 6865 2066 6f6c 6c6f 7769   for the followi
-000061e0: 6e67 2070 6172 616d 6574 6572 7320 746f  ng parameters to
-000061f0: 2060 6372 6561 7465 5f73 7761 726d 5f73   `create_swarm_s
-00006200: 7065 6360 3a0a 2020 6065 7874 6572 6e61  pec`:.  `externa
-00006210: 6c5f 6361 7360 2c20 606c 6162 656c 7360  l_cas`, `labels`
-00006220: 2c20 6073 6967 6e69 6e67 5f63 615f 6365  , `signing_ca_ce
-00006230: 7274 602c 2060 7369 676e 696e 675f 6361  rt`, `signing_ca
-00006240: 5f6b 6579 602c 0a20 2060 6361 5f66 6f72  _key`,.  `ca_for
-00006250: 6365 5f72 6f74 6174 6560 2c20 6061 7574  ce_rotate`, `aut
-00006260: 6f6c 6f63 6b5f 6d61 6e61 6765 7273 602c  olock_managers`,
-00006270: 2060 6c6f 675f 6472 6976 6572 602e 2054   `log_driver`. T
-00006280: 6865 7365 2061 6464 6974 696f 6e73 0a20  hese additions. 
-00006290: 2061 6c73 6f20 6170 706c 7920 746f 2060   also apply to `
-000062a0: 446f 636b 6572 436c 6965 6e74 2e73 7761  DockerClient.swa
-000062b0: 726d 2e69 6e69 7460 2e0a 2a20 4164 6465  rm.init`..* Adde
-000062c0: 6420 7375 7070 6f72 7420 666f 7220 6069  d support for `i
-000062d0: 6e73 6572 745f 6465 6661 756c 7473 6020  nsert_defaults` 
-000062e0: 696e 2060 4150 4943 6c69 656e 742e 696e  in `APIClient.in
-000062f0: 7370 6563 745f 7365 7276 6963 6560 2061  spect_service` a
-00006300: 6e64 0a20 2060 446f 636b 6572 436c 6965  nd.  `DockerClie
-00006310: 6e74 2e73 6572 7669 6365 732e 6765 7460  nt.services.get`
-00006320: 2e0a 0a23 2323 2042 7567 6669 7865 730a  ...### Bugfixes.
-00006330: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-00006340: 6865 7265 2072 6561 6469 6e67 2061 2030  here reading a 0
-00006350: 2d6c 656e 6774 6820 6672 616d 6520 696e  -length frame in
-00006360: 206c 6f67 2073 7472 6561 6d73 2077 6f75   log streams wou
-00006370: 6c64 2069 6e63 6f72 7265 6374 6c79 0a20  ld incorrectly. 
-00006380: 2069 6e74 6572 7275 7074 2073 7472 6561   interrupt strea
-00006390: 6d69 6e67 2e0a 2a20 4669 7865 6420 6120  ming..* Fixed a 
-000063a0: 6275 6720 7768 6572 6520 7468 6520 6069  bug where the `i
-000063b0: 6460 206d 656d 6265 7220 6f6e 2060 5377  d` member on `Sw
-000063c0: 6172 6d60 206f 626a 6563 7473 2077 6173  arm` objects was
-000063d0: 6e27 7420 6265 696e 6720 706f 7075 6c61  n't being popula
-000063e0: 7465 642e 0a2a 2046 6978 6564 2061 2062  ted..* Fixed a b
-000063f0: 7567 2074 6861 7420 776f 756c 6420 6361  ug that would ca
-00006400: 7573 6520 736f 6d65 2064 6174 6120 6174  use some data at
-00006410: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
-00006420: 6620 616e 2075 7067 7261 6465 640a 2020  f an upgraded.  
-00006430: 636f 6e6e 6563 7469 6f6e 2073 7472 6561  connection strea
-00006440: 6d20 2860 6174 7461 6368 602c 2060 6578  m (`attach`, `ex
-00006450: 6563 5f72 756e 6029 2074 6f20 6469 7361  ec_run`) to disa
-00006460: 7070 6561 722e 0a0a 322e 352e 310a 2d2d  ppear...2.5.1.--
-00006470: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
-00006480: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
-00006490: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-000064a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000064b0: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
-000064c0: 2f6d 696c 6573 746f 6e65 2f33 373f 636c  /milestone/37?cl
-000064d0: 6f73 6564 3d31 290a 0a23 2323 2042 7567  osed=1)..### Bug
-000064e0: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
-000064f0: 2062 7567 2077 6865 7265 2070 6174 7465   bug where patte
-00006500: 726e 7320 656e 6469 6e67 2077 6974 6820  rns ending with 
-00006510: 602a 2a60 2069 6e20 602e 646f 636b 6572  `**` in `.docker
-00006520: 6967 6e6f 7265 6020 776f 756c 640a 2020  ignore` would.  
-00006530: 7261 6973 6520 616e 2065 7863 6570 7469  raise an excepti
-00006540: 6f6e 0a2a 2046 6978 6564 2061 2062 7567  on.* Fixed a bug
-00006550: 2077 6865 7265 2075 7369 6e67 2060 6174   where using `at
-00006560: 7461 6368 6020 7769 7468 2074 6865 2060  tach` with the `
-00006570: 7374 7265 616d 6020 6172 6775 6d65 6e74  stream` argument
-00006580: 2073 6574 2074 6f20 6046 616c 7365 600a   set to `False`.
-00006590: 2020 776f 756c 6420 7261 6973 6520 616e    would raise an
-000065a0: 2065 7863 6570 7469 6f6e 0a0a 322e 352e   exception..2.5.
-000065b0: 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f  0.-----..[List o
-000065c0: 6620 5052 7320 2f20 6973 7375 6573 2066  f PRs / issues f
-000065d0: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
-000065e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000065f0: 636f 6d2f 646f 636b 6572 2f64 6f63 6b65  com/docker/docke
-00006600: 722d 7079 2f6d 696c 6573 746f 6e65 2f33  r-py/milestone/3
-00006610: 343f 636c 6f73 6564 3d31 290a 0a23 2323  4?closed=1)..###
-00006620: 2046 6561 7475 7265 730a 0a2a 2041 6464   Features..* Add
-00006630: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
-00006640: 6865 2060 7371 7561 7368 6020 7061 7261  he `squash` para
-00006650: 6d65 7465 7220 696e 2060 4150 4943 6c69  meter in `APICli
-00006660: 656e 742e 6275 696c 6460 2061 6e64 0a20  ent.build` and. 
-00006670: 2060 446f 636b 6572 436c 6965 6e74 2e69   `DockerClient.i
-00006680: 6d61 6765 732e 6275 696c 6460 2e0a 2a20  mages.build`..* 
-00006690: 5768 656e 2075 7369 6e67 2041 5049 2076  When using API v
-000066a0: 6572 7369 6f6e 2031 2e32 3320 6f72 2061  ersion 1.23 or a
-000066b0: 626f 7665 2c20 606c 6f61 645f 696d 6167  bove, `load_imag
-000066c0: 6560 2077 696c 6c20 6e6f 7720 7265 7475  e` will now retu
-000066d0: 726e 2061 0a20 2067 656e 6572 6174 6f72  rn a.  generator
-000066e0: 206f 6620 7072 6f67 7265 7373 2061 7320   of progress as 
-000066f0: 4a53 4f4e 2060 6469 6374 6073 2e0a 2a20  JSON `dict`s..* 
-00006700: 6072 656d 6f76 655f 696d 6167 6560 206e  `remove_image` n
-00006710: 6f77 2072 6574 7572 6e73 2074 6865 2063  ow returns the c
-00006720: 6f6e 7465 6e74 206f 6620 7468 6520 4150  ontent of the AP
-00006730: 4927 7320 7265 7370 6f6e 7365 2e0a 0a0a  I's response....
-00006740: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
-00006750: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-00006760: 6865 7265 2074 6865 2060 6175 746f 5f72  here the `auto_r
-00006770: 656d 6f76 6560 2070 6172 616d 6574 6572  emove` parameter
-00006780: 2069 6e0a 2020 6044 6f63 6b65 7243 6c69   in.  `DockerCli
-00006790: 656e 742e 636f 6e74 6169 6e65 7273 2e72  ent.containers.r
-000067a0: 756e 6020 7761 7320 6e6f 7420 7461 6b65  un` was not take
-000067b0: 6e20 696e 746f 2061 6363 6f75 6e74 2e0a  n into account..
-000067c0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-000067d0: 6572 6520 602e 646f 636b 6572 6967 6e6f  ere `.dockerigno
-000067e0: 7265 6020 7061 7474 6572 6e73 2073 7461  re` patterns sta
-000067f0: 7274 696e 6720 7769 7468 2061 2073 6c61  rting with a sla
-00006800: 7368 0a20 2077 6572 6520 6967 6e6f 7265  sh.  were ignore
-00006810: 642e 0a2a 2046 6978 6564 2061 6e20 6973  d..* Fixed an is
-00006820: 7375 6520 7769 7468 2074 6865 2068 616e  sue with the han
-00006830: 646c 696e 6720 6f66 2060 2a2a 6020 7061  dling of `**` pa
-00006840: 7474 6572 6e73 2069 6e20 602e 646f 636b  tterns in `.dock
-00006850: 6572 6967 6e6f 7265 600a 2a20 4669 7865  erignore`.* Fixe
-00006860: 6420 6120 6275 6720 7768 6572 6520 6275  d a bug where bu
-00006870: 696c 6469 6e67 2060 4652 4f4d 6020 6120  ilding `FROM` a 
-00006880: 7072 6976 6174 6520 446f 636b 6572 2048  private Docker H
-00006890: 7562 2069 6d61 6765 2077 6865 6e20 6e6f  ub image when no
-000068a0: 740a 2020 7573 696e 6720 6120 6372 6564  t.  using a cred
-000068b0: 2073 746f 7265 2077 6f75 6c64 2066 6169   store would fai
-000068c0: 6c2e 0a2a 2046 6978 6564 2061 2062 7567  l..* Fixed a bug
-000068d0: 2077 6865 7265 2063 616c 6c69 6e67 2060   where calling `
-000068e0: 6372 6561 7465 5f73 6572 7669 6365 6020  create_service` 
-000068f0: 6f72 2060 7570 6461 7465 5f73 6572 7669  or `update_servi
-00006900: 6365 6020 7769 7468 0a20 2060 7461 736b  ce` with.  `task
-00006910: 5f74 656d 706c 6174 6560 2061 7320 6120  _template` as a 
-00006920: 6064 6963 7460 2077 6f75 6c64 2072 6169  `dict` would rai
-00006930: 7365 2061 6e20 6578 6365 7074 696f 6e2e  se an exception.
-00006940: 0a2a 2046 6978 6564 2074 6865 2068 616e  .* Fixed the han
-00006950: 646c 696e 6720 6f66 2054 5459 2d65 6e61  dling of TTY-ena
-00006960: 626c 6564 2063 6f6e 7461 696e 6572 7320  bled containers 
-00006970: 696e 2060 6174 7461 6368 6020 616e 6420  in `attach` and 
-00006980: 6065 7865 635f 7275 6e60 2e0a 2a20 6044  `exec_run`..* `D
-00006990: 6f63 6b65 7243 6c69 656e 742e 636f 6e74  ockerClient.cont
-000069a0: 6169 6e65 7273 2e72 756e 6020 7769 6c6c  ainers.run` will
-000069b0: 206e 6f20 6c6f 6e67 6572 2061 7474 656d   no longer attem
-000069c0: 7074 2074 6f20 7374 7265 616d 206c 6f67  pt to stream log
-000069d0: 7320 6966 2074 6865 0a20 206c 6f67 2064  s if the.  log d
-000069e0: 7269 7665 7220 646f 6573 6e27 7420 7375  river doesn't su
-000069f0: 7070 6f72 7420 7468 6520 6f70 6572 6174  pport the operat
-00006a00: 696f 6e2e 0a0a 2323 2320 4d69 7363 656c  ion...### Miscel
-00006a10: 6c61 6e65 6f75 730a 0a2a 2041 6464 6564  laneous..* Added
-00006a20: 2065 7874 7261 2072 6571 7569 7265 6d65   extra requireme
-00006a30: 6e74 7320 666f 7220 6265 7474 6572 2054  nts for better T
-00006a40: 4c53 2073 7570 706f 7274 206f 6e20 736f  LS support on so
-00006a50: 6d65 2070 6c61 7466 6f72 6d73 2e0a 2020  me platforms..  
-00006a60: 5468 6573 6520 6361 6e20 6265 2069 6e73  These can be ins
-00006a70: 7461 6c6c 6564 206f 7220 7265 7175 6972  talled or requir
-00006a80: 6564 2074 6872 6f75 6768 2074 6865 2060  ed through the `
-00006a90: 646f 636b 6572 5b74 6c73 5d60 206e 6f74  docker[tls]` not
-00006aa0: 6174 696f 6e2e 0a0a 322e 342e 320a 2d2d  ation...2.4.2.--
-00006ab0: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
-00006ac0: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
-00006ad0: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-00006ae0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00006af0: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
-00006b00: 2f6d 696c 6573 746f 6e65 2f33 363f 636c  /milestone/36?cl
-00006b10: 6f73 6564 3d31 290a 0a23 2323 2042 7567  osed=1)..### Bug
-00006b20: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
-00006b30: 2062 7567 2077 6865 7265 2074 6865 2060   bug where the `
-00006b40: 7370 6c69 745f 706f 7274 6020 7574 696c  split_port` util
-00006b50: 6974 7920 776f 756c 6420 7261 6973 6520  ity would raise 
-00006b60: 616e 2065 7863 6570 7469 6f6e 2077 6865  an exception whe
-00006b70: 6e0a 2020 7061 7373 6564 2061 206e 6f6e  n.  passed a non
-00006b80: 2d73 7472 696e 6720 6172 6775 6d65 6e74  -string argument
-00006b90: 2e0a 0a32 2e34 2e30 0a2d 2d2d 2d2d 0a0a  ...2.4.0.-----..
-00006ba0: 5b4c 6973 7420 6f66 2050 5273 202f 2069  [List of PRs / i
-00006bb0: 7373 7565 7320 666f 7220 7468 6973 2072  ssues for this r
-00006bc0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
-00006bd0: 6769 7468 7562 2e63 6f6d 2f64 6f63 6b65  github.com/docke
-00006be0: 722f 646f 636b 6572 2d70 792f 6d69 6c65  r/docker-py/mile
-00006bf0: 7374 6f6e 652f 3333 3f63 6c6f 7365 643d  stone/33?closed=
-00006c00: 3129 0a0a 2323 2320 4665 6174 7572 6573  1)..### Features
-00006c10: 0a0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
-00006c20: 7420 666f 7220 7468 6520 6074 6172 6765  t for the `targe
-00006c30: 7460 2061 6e64 2060 6e65 7477 6f72 6b5f  t` and `network_
-00006c40: 6d6f 6465 6020 7061 7261 6d65 7465 7273  mode` parameters
-00006c50: 2069 6e0a 2020 6041 5049 436c 6965 6e74   in.  `APIClient
-00006c60: 2e62 7569 6c64 6020 616e 6420 6044 6f63  .build` and `Doc
-00006c70: 6b65 7243 6c69 656e 742e 696d 6167 6573  kerClient.images
-00006c80: 2e62 7569 6c64 602e 0a2a 2041 6464 6564  .build`..* Added
-00006c90: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
-00006ca0: 2060 7275 6e74 696d 6560 2070 6172 616d   `runtime` param
-00006cb0: 6574 6572 2069 6e20 6041 5049 436c 6965  eter in `APIClie
-00006cc0: 6e74 2e63 7265 6174 655f 636f 6e74 6169  nt.create_contai
-00006cd0: 6e65 7260 0a20 2061 6e64 2060 446f 636b  ner`.  and `Dock
-00006ce0: 6572 436c 6965 6e74 2e63 6f6e 7461 696e  erClient.contain
-00006cf0: 6572 732e 7275 6e60 2e0a 2a20 4164 6465  ers.run`..* Adde
-00006d00: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
-00006d10: 6520 6069 6e67 7265 7373 6020 7061 7261  e `ingress` para
-00006d20: 6d65 7465 7220 696e 2060 4150 4943 6c69  meter in `APICli
-00006d30: 656e 742e 6372 6561 7465 5f6e 6574 776f  ent.create_netwo
-00006d40: 726b 6020 616e 640a 2020 6044 6f63 6b65  rk` and.  `Docke
-00006d50: 7243 6c69 656e 742e 6e65 7477 6f72 6b73  rClient.networks
-00006d60: 2e63 7265 6174 6560 2e0a 2a20 4164 6465  .create`..* Adde
-00006d70: 6420 7375 7070 6f72 7420 666f 7220 6070  d support for `p
-00006d80: 6c61 6365 6d65 6e74 6020 636f 6e66 6967  lacement` config
-00006d90: 7572 6174 696f 6e20 696e 2060 646f 636b  uration in `dock
-00006da0: 6572 2e74 7970 6573 2e54 6173 6b54 656d  er.types.TaskTem
-00006db0: 706c 6174 6560 2e0a 2a20 4164 6465 6420  plate`..* Added 
-00006dc0: 7375 7070 6f72 7420 666f 7220 6074 7479  support for `tty
-00006dd0: 6020 636f 6e66 6967 7572 6174 696f 6e20  ` configuration 
-00006de0: 696e 2060 646f 636b 6572 2e74 7970 6573  in `docker.types
-00006df0: 2e43 6f6e 7461 696e 6572 5370 6563 602e  .ContainerSpec`.
-00006e00: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-00006e10: 2066 6f72 2060 7374 6172 745f 7065 7269   for `start_peri
-00006e20: 6f64 6020 636f 6e66 6967 7572 6174 696f  od` configuratio
-00006e30: 6e20 696e 2060 646f 636b 6572 2e74 7970  n in `docker.typ
-00006e40: 6573 2e48 6561 6c74 6863 6865 636b 602e  es.Healthcheck`.
-00006e50: 0a2a 2054 6865 2060 6372 6564 4865 6c70  .* The `credHelp
-00006e60: 6572 7360 2073 6563 7469 6f6e 2069 6e20  ers` section in 
-00006e70: 446f 636b 6572 2773 2063 6f6e 6669 6775  Docker's configu
-00006e80: 7261 7469 6f6e 2066 696c 6520 6973 206e  ration file is n
-00006e90: 6f77 2072 6563 6f67 6e69 7a65 642e 0a2a  ow recognized..*
-00006ea0: 2050 6f72 7420 7370 6563 6966 6963 6174   Port specificat
-00006eb0: 696f 6e73 2069 6e63 6c75 6469 6e67 2049  ions including I
-00006ec0: 5076 3620 656e 6470 6f69 6e74 7320 6172  Pv6 endpoints ar
-00006ed0: 6520 6e6f 7720 7375 7070 6f72 7465 642e  e now supported.
-00006ee0: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-00006ef0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-00006f00: 6572 6520 696e 7374 616e 7469 6174 696e  ere instantiatin
-00006f10: 6720 6120 6044 6f63 6b65 7243 6c69 656e  g a `DockerClien
-00006f20: 7460 2075 7369 6e67 2060 646f 636b 6572  t` using `docker
-00006f30: 2e66 726f 6d5f 656e 7660 0a20 2077 6f75  .from_env`.  wou
-00006f40: 6c64 6e27 7420 636f 7272 6563 746c 7920  ldn't correctly 
-00006f50: 7365 7420 7468 6520 6465 6661 756c 7420  set the default 
-00006f60: 7469 6d65 6f75 7420 7661 6c75 652e 0a2a  timeout value..*
-00006f70: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
-00006f80: 7265 2060 446f 636b 6572 436c 6965 6e74  re `DockerClient
-00006f90: 2e73 6563 7265 7473 6020 7761 7320 6e6f  .secrets` was no
-00006fa0: 7420 6163 6365 7373 6962 6c65 2061 7320  t accessible as 
-00006fb0: 6120 7072 6f70 6572 7479 2e0a 2a20 4669  a property..* Fi
-00006fc0: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
-00006fd0: 6044 6f63 6b65 7243 6c69 656e 742e 6275  `DockerClient.bu
-00006fe0: 696c 6460 2077 6f75 6c64 2073 6f6d 6574  ild` would somet
-00006ff0: 696d 6573 2072 6574 7572 6e20 7468 6520  imes return the 
-00007000: 7772 6f6e 670a 2020 696d 6167 652e 0a2a  wrong.  image..*
-00007010: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
-00007020: 7265 2076 616c 7565 7320 666f 7220 6048  re values for `H
-00007030: 6f73 7443 6f6e 6669 672e 6e61 6e6f 5f63  ostConfig.nano_c
-00007040: 7075 7360 2065 7863 6565 6469 6e67 2032  pus` exceeding 2
-00007050: 5e33 3220 776f 756c 640a 2020 7261 6973  ^32 would.  rais
-00007060: 6520 6120 7479 7065 2065 7272 6f72 2e0a  e a type error..
-00007070: 2a20 6049 6d61 6765 2e74 6167 6020 6e6f  * `Image.tag` no
-00007080: 7720 7072 6f70 6572 6c79 2072 6574 7572  w properly retur
-00007090: 6e73 2060 5472 7565 6020 7768 656e 2074  ns `True` when t
-000070a0: 6865 206f 7065 7261 7469 6f6e 2069 7320  he operation is 
-000070b0: 7375 6363 6573 7366 756c 2e0a 2a20 6041  successful..* `A
-000070c0: 5049 436c 6965 6e74 2e6c 6f67 7360 2061  PIClient.logs` a
-000070d0: 6e64 2060 436f 6e74 6169 6e65 722e 6c6f  nd `Container.lo
-000070e0: 6773 6020 6e6f 7720 7261 6973 6520 616e  gs` now raise an
-000070f0: 2065 7863 6570 7469 6f6e 2069 6620 7468   exception if th
-00007100: 6520 6073 696e 6365 600a 2020 6172 6775  e `since`.  argu
-00007110: 6d65 6e74 2075 7365 7320 616e 2075 6e73  ment uses an uns
-00007120: 7570 706f 7274 6564 2074 7970 6520 696e  upported type in
-00007130: 7374 6561 6420 6f66 2069 676e 6f72 696e  stead of ignorin
-00007140: 6720 7468 6520 7661 6c75 652e 0a2a 2046  g the value..* F
-00007150: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
-00007160: 2073 6f6d 6520 6d65 7468 6f64 7320 776f   some methods wo
-00007170: 756c 6420 7261 6973 6520 6120 604e 756c  uld raise a `Nul
-00007180: 6c52 6573 6f75 7263 6560 2065 7863 6570  lResource` excep
-00007190: 7469 6f6e 2077 6865 6e0a 2020 7468 6520  tion when.  the 
-000071a0: 7265 736f 7572 6365 2049 4420 7761 7320  resource ID was 
-000071b0: 7072 6f76 6964 6564 2075 7369 6e67 2061  provided using a
-000071c0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-000071d0: 742e 0a0a 2323 2320 4d69 7363 656c 6c61  t...### Miscella
-000071e0: 6e65 6f75 730a 0a2a 2060 4150 4943 6c69  neous..* `APICli
-000071f0: 656e 7460 2069 6e73 7461 6e63 6573 2063  ent` instances c
-00007200: 616e 206e 6f77 2062 6520 7069 636b 6c65  an now be pickle
-00007210: 642e 0a0a 322e 332e 300a 2d2d 2d2d 2d0a  d...2.3.0.-----.
-00007220: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
-00007230: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
-00007240: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
-00007250: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
-00007260: 6572 2f64 6f63 6b65 722d 7079 2f6d 696c  er/docker-py/mil
-00007270: 6573 746f 6e65 2f33 313f 636c 6f73 6564  estone/31?closed
-00007280: 3d31 290a 0a23 2323 2046 6561 7475 7265  =1)..### Feature
-00007290: 730a 0a2a 2041 6464 6564 2073 7570 706f  s..* Added suppo
-000072a0: 7274 2066 6f72 2074 6865 2066 6f6c 6c6f  rt for the follo
-000072b0: 7769 6e67 2060 486f 7374 436f 6e66 6967  wing `HostConfig
-000072c0: 6020 7061 7261 6d65 7465 7273 3a20 6076  ` parameters: `v
-000072d0: 6f6c 756d 655f 6472 6976 6572 602c 0a20  olume_driver`,. 
-000072e0: 2060 6370 755f 636f 756e 7460 2c20 6063   `cpu_count`, `c
-000072f0: 7075 5f70 6572 6365 6e74 602c 2060 6e61  pu_percent`, `na
-00007300: 6e6f 5f63 7075 7360 2c20 6063 7075 7365  no_cpus`, `cpuse
-00007310: 745f 6d65 6d73 602e 0a2a 2041 6464 6564  t_mems`..* Added
-00007320: 2073 7570 706f 7274 2066 6f72 2060 7665   support for `ve
-00007330: 7262 6f73 6560 2070 6172 616d 6574 6572  rbose` parameter
-00007340: 2069 6e20 6041 5049 436c 6965 6e74 2e69   in `APIClient.i
-00007350: 6e73 7065 6374 5f6e 6574 776f 726b 6020  nspect_network` 
-00007360: 616e 640a 2020 6044 6f63 6b65 7243 6c69  and.  `DockerCli
-00007370: 656e 742e 6e65 7477 6f72 6b73 2e67 6574  ent.networks.get
-00007380: 602e 0a2a 2041 6464 6564 2073 7570 706f  `..* Added suppo
-00007390: 7274 2066 6f72 2074 6865 2060 656e 7669  rt for the `envi
-000073a0: 726f 6e6d 656e 7460 2070 6172 616d 6574  ronment` paramet
-000073b0: 6572 2069 6e20 6041 5049 436c 6965 6e74  er in `APIClient
-000073c0: 2e65 7865 635f 6372 6561 7465 600a 2020  .exec_create`.  
-000073d0: 616e 6420 6043 6f6e 7461 696e 6572 2e65  and `Container.e
-000073e0: 7865 635f 7275 6e60 0a2a 2041 6464 6564  xec_run`.* Added
-000073f0: 2060 7265 6c6f 6164 5f63 6f6e 6669 6760   `reload_config`
-00007400: 206d 6574 686f 6420 746f 2060 4150 4943   method to `APIC
-00007410: 6c69 656e 7460 2c20 7468 6174 206c 6574  lient`, that let
-00007420: 7320 7468 6520 7573 6572 2072 656c 6f61  s the user reloa
-00007430: 640a 2020 7468 6520 6063 6f6e 6669 672e  d.  the `config.
-00007440: 6a73 6f6e 6020 6461 7461 2066 726f 6d20  json` data from 
-00007450: 6469 736b 2e0a 2a20 4164 6465 6420 606c  disk..* Added `l
-00007460: 6162 656c 7360 2070 726f 7065 7274 7920  abels` property 
-00007470: 746f 2074 6865 2060 496d 6167 6560 2061  to the `Image` a
-00007480: 6e64 2060 436f 6e74 6169 6e65 7260 2063  nd `Container` c
-00007490: 6c61 7373 6573 2e0a 2a20 4164 6465 6420  lasses..* Added 
-000074a0: 6069 6d61 6765 6020 7072 6f70 6572 7479  `image` property
-000074b0: 2074 6f20 7468 6520 6043 6f6e 7461 696e   to the `Contain
-000074c0: 6572 6020 636c 6173 732e 0a0a 2323 2320  er` class...### 
-000074d0: 4275 6766 6978 6573 0a0a 2a20 4669 7865  Bugfixes..* Fixe
-000074e0: 6420 6120 6275 6720 7768 6572 6520 7365  d a bug where se
-000074f0: 7474 696e 6720 6072 6570 6c69 6361 7360  tting `replicas`
-00007500: 2074 6f20 7a65 726f 2069 6e20 6053 6572   to zero in `Ser
-00007510: 7669 6365 4d6f 6465 6020 776f 756c 6420  viceMode` would 
-00007520: 6e6f 740a 2020 7265 6769 7374 6572 2061  not.  register a
-00007530: 7320 6120 7661 6c69 6420 656e 7472 792e  s a valid entry.
-00007540: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-00007550: 6865 7265 2060 446f 636b 6572 436c 6965  here `DockerClie
-00007560: 6e74 2e69 6d61 6765 732e 6275 696c 6460  nt.images.build`
-00007570: 2077 6f75 6c64 2072 6570 6f72 7420 6120   would report a 
-00007580: 6661 696c 7572 6520 6166 7465 720a 2020  failure after.  
-00007590: 6120 7375 6363 6573 7366 756c 2062 7569  a successful bui
-000075a0: 6c64 2069 6620 6120 6074 6167 6020 7761  ld if a `tag` wa
-000075b0: 7320 7365 742e 0a2a 2046 6978 6564 2061  s set..* Fixed a
-000075c0: 6e20 6973 7375 6520 7768 6572 6520 6044  n issue where `D
-000075d0: 6f63 6b65 7243 6c69 656e 742e 696d 6167  ockerClient.imag
-000075e0: 6573 2e70 756c 6c60 2077 6f75 6c64 2066  es.pull` would f
-000075f0: 6169 6c20 746f 2072 6574 7572 6e20 7468  ail to return th
-00007600: 650a 2020 636f 7272 6573 706f 6e64 696e  e.  correspondin
-00007610: 6720 696d 6167 6520 6f62 6a65 6374 2069  g image object i
-00007620: 6620 6120 6074 6167 6020 7761 7320 7365  f a `tag` was se
-00007630: 742e 0a2a 2046 6978 6564 2061 2062 7567  t..* Fixed a bug
-00007640: 2077 6865 7265 2061 206c 6973 7420 6f66   where a list of
-00007650: 2060 6d6f 756e 7473 6020 7072 6f76 6964   `mounts` provid
-00007660: 6564 2074 6f20 6041 5049 436c 6965 6e74  ed to `APIClient
-00007670: 2e63 7265 6174 655f 7365 7276 6963 6560  .create_service`
-00007680: 0a20 2077 6f75 6c64 2073 6f6d 6574 696d  .  would sometim
-00007690: 6573 2062 6520 7061 7273 6564 2069 6e63  es be parsed inc
-000076a0: 6f72 7265 6374 6c79 2e0a 2a20 4669 7865  orrectly..* Fixe
-000076b0: 6420 6120 6275 6720 7768 6572 6520 6361  d a bug where ca
-000076c0: 6c6c 696e 6720 604e 6574 776f 726b 2e63  lling `Network.c
-000076d0: 6f6e 7461 696e 6572 7360 2077 6f75 6c64  ontainers` would
-000076e0: 2063 7261 7368 2077 6865 6e20 6e6f 2063   crash when no c
-000076f0: 6f6e 7461 696e 6572 730a 2020 7765 7265  ontainers.  were
-00007700: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00007710: 2074 6865 206e 6574 776f 726b 2e0a 2a20   the network..* 
-00007720: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-00007730: 6865 7265 2060 4e65 7477 6f72 6b2e 636f  here `Network.co
-00007740: 6e6e 6563 7460 2061 6e64 2060 4e65 7477  nnect` and `Netw
-00007750: 6f72 6b2e 6469 7363 6f6e 6e65 6374 6020  ork.disconnect` 
-00007760: 776f 756c 6420 6e6f 740a 2020 6163 6365  would not.  acce
-00007770: 7074 2073 6f6d 6520 6f66 2074 6865 2064  pt some of the d
-00007780: 6f63 756d 656e 7465 6420 7061 7261 6d65  ocumented parame
-00007790: 7465 7273 2e0a 2a20 4669 7865 6420 6120  ters..* Fixed a 
-000077a0: 6275 6720 7768 6572 6520 7468 6520 6063  bug where the `c
-000077b0: 7075 7365 745f 6370 7573 6020 7061 7261  puset_cpus` para
-000077c0: 6d65 7465 7220 776f 756c 6420 6e6f 7420  meter would not 
-000077d0: 6265 2070 726f 7065 726c 7920 7365 7420  be properly set 
-000077e0: 696e 0a20 2060 4150 4943 6c69 656e 742e  in.  `APIClient.
-000077f0: 6372 6561 7465 5f68 6f73 745f 636f 6e66  create_host_conf
-00007800: 6967 602e 0a0a 2323 2320 4d69 7363 656c  ig`...### Miscel
-00007810: 6c61 6e65 6f75 730a 0a2a 2054 6865 2069  laneous..* The i
-00007820: 6e76 616c 6964 2060 6e65 7477 6f72 6b73  nvalid `networks
-00007830: 6020 6172 6775 6d65 6e74 2069 6e20 6044  ` argument in `D
-00007840: 6f63 6b65 7243 6c69 656e 742e 636f 6e74  ockerClient.cont
-00007850: 6169 6e65 7273 2e72 756e 6020 6861 7320  ainers.run` has 
-00007860: 6265 656e 0a20 2072 6570 6c61 6365 6420  been.  replaced 
-00007870: 7769 7468 2061 2028 776f 726b 696e 6729  with a (working)
-00007880: 2073 696e 6775 6c61 7220 606e 6574 776f   singular `netwo
-00007890: 726b 6020 6172 6775 6d65 6e74 2e0a 0a0a  rk` argument....
-000078a0: 322e 322e 310a 2d2d 2d2d 2d0a 0a5b 4c69  2.2.1.-----..[Li
-000078b0: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
-000078c0: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
-000078d0: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
-000078e0: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
-000078f0: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
-00007900: 6e65 2f33 323f 636c 6f73 6564 3d31 290a  ne/32?closed=1).
-00007910: 0a23 2323 2042 7567 6669 7865 730a 0a2a  .### Bugfixes..*
-00007920: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
-00007930: 7265 2074 6865 2060 7374 6174 7573 5f63  re the `status_c
-00007940: 6f64 6560 2061 7474 7269 6275 7465 206f  ode` attribute o
-00007950: 6620 6041 5049 4572 726f 7260 2065 7863  f `APIError` exc
-00007960: 6570 7469 6f6e 7320 776f 756c 640a 2020  eptions would.  
-00007970: 6e6f 7420 7265 666c 6563 7420 7468 6520  not reflect the 
-00007980: 6578 7065 6374 6564 2076 616c 7565 2e0a  expected value..
-00007990: 2a20 4669 7865 6420 616e 2069 7373 7565  * Fixed an issue
-000079a0: 2077 6865 7265 2074 6865 2060 6576 656e   where the `even
-000079b0: 7473 6020 6d65 7468 6f64 2077 6f75 6c64  ts` method would
-000079c0: 2074 696d 6520 6f75 7420 756e 6578 7065   time out unexpe
-000079d0: 6374 6564 6c79 2069 6620 6e6f 0a20 2064  ctedly if no.  d
-000079e0: 6174 6120 7761 7320 7365 6e74 2062 7920  ata was sent by 
-000079f0: 7468 6520 656e 6769 6e65 2066 6f72 2061  the engine for a
-00007a00: 2067 6976 656e 2061 6d6f 756e 7420 6f66   given amount of
-00007a10: 2074 696d 652e 0a0a 0a32 2e32 2e30 0a2d   time....2.2.0.-
-00007a20: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-00007a30: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-00007a40: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-00007a50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00007a60: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-00007a70: 792f 6d69 6c65 7374 6f6e 652f 3330 3f63  y/milestone/30?c
-00007a80: 6c6f 7365 643d 3129 0a0a 2323 2320 4665  losed=1)..### Fe
-00007a90: 6174 7572 6573 0a0a 2a20 4465 6661 756c  atures..* Defaul
-00007aa0: 7420 4150 4920 7665 7273 696f 6e20 6861  t API version ha
-00007ab0: 7320 6265 656e 2062 756d 7065 6420 746f  s been bumped to
-00007ac0: 2060 312e 3236 6020 2845 6e67 696e 6520   `1.26` (Engine 
-00007ad0: 312e 3133 2e31 2b29 0a2a 2055 7067 7261  1.13.1+).* Upgra
-00007ae0: 6465 2070 6c75 6769 6e3a 0a20 202a 2041  de plugin:.  * A
-00007af0: 6464 6564 2074 6865 2060 7570 6772 6164  dded the `upgrad
-00007b00: 655f 706c 7567 696e 6020 6d65 7468 6f64  e_plugin` method
-00007b10: 2074 6f20 7468 6520 6041 5049 436c 6965   to the `APIClie
-00007b20: 6e74 6020 636c 6173 730a 2020 2a20 4164  nt` class.  * Ad
-00007b30: 6465 6420 7468 6520 6075 7067 7261 6465  ded the `upgrade
-00007b40: 6020 6d65 7468 6f64 2074 6f20 7468 6520  ` method to the 
-00007b50: 6050 6c75 6769 6e60 2063 6c61 7373 0a2a  `Plugin` class.*
-00007b60: 2053 6572 7669 6365 206c 6f67 733a 0a20   Service logs:. 
-00007b70: 202a 2041 6464 6564 2074 6865 2060 7365   * Added the `se
-00007b80: 7276 6963 655f 6c6f 6773 6020 6d65 7468  rvice_logs` meth
-00007b90: 6f64 2074 6f20 7468 6520 6041 5049 436c  od to the `APICl
-00007ba0: 6965 6e74 6020 636c 6173 730a 2020 2a20  ient` class.  * 
-00007bb0: 4164 6465 6420 7468 6520 606c 6f67 7360  Added the `logs`
-00007bc0: 206d 6574 686f 6420 746f 2074 6865 2060   method to the `
-00007bd0: 5365 7276 6963 6560 2063 6c61 7373 0a2a  Service` class.*
-00007be0: 2041 6464 6564 2074 6865 2060 6466 6020   Added the `df` 
-00007bf0: 6d65 7468 6f64 2074 6f20 6041 5049 436c  method to `APICl
-00007c00: 6965 6e74 6020 616e 6420 6044 6f63 6b65  ient` and `Docke
-00007c10: 7243 6c69 656e 7460 0a2a 2041 6464 6564  rClient`.* Added
-00007c20: 2073 7570 706f 7274 2066 6f72 2060 696e   support for `in
-00007c30: 6974 6020 616e 6420 6069 6e69 745f 7061  it` and `init_pa
-00007c40: 7468 6020 7061 7261 6d65 7465 7273 2069  th` parameters i
-00007c50: 6e20 6048 6f73 7443 6f6e 6669 6760 0a20  n `HostConfig`. 
-00007c60: 2061 6e64 2060 446f 636b 6572 436c 6965   and `DockerClie
-00007c70: 6e74 2e63 6f6e 7461 696e 6572 732e 7275  nt.containers.ru
-00007c80: 6e60 0a2a 2041 6464 6564 2073 7570 706f  n`.* Added suppo
-00007c90: 7274 2066 6f72 2060 686f 7374 6e61 6d65  rt for `hostname
-00007ca0: 6020 7061 7261 6d65 7465 7220 696e 2060  ` parameter in `
-00007cb0: 436f 6e74 6169 6e65 7253 7065 6360 2061  ContainerSpec` a
-00007cc0: 6e64 0a20 2060 446f 636b 6572 436c 6965  nd.  `DockerClie
-00007cd0: 6e74 2e73 6572 7669 6365 2e63 7265 6174  nt.service.creat
-00007ce0: 6560 0a2a 2041 6464 6564 2073 7570 706f  e`.* Added suppo
-00007cf0: 7274 2066 6f72 2070 6f72 7420 7261 6e67  rt for port rang
-00007d00: 6520 746f 2073 696e 676c 6520 706f 7274  e to single port
-00007d10: 2069 6e20 706f 7274 206d 6170 7069 6e67   in port mapping
-00007d20: 730a 2020 2865 2e67 2e20 6038 3030 302d  s.  (e.g. `8000-
-00007d30: 3830 3130 3a38 3060 290a 0a23 2323 2042  8010:80`)..### B
-00007d40: 7567 6669 7865 730a 0a2a 2046 6978 6564  ugfixes..* Fixed
-00007d50: 2061 2062 7567 2077 6865 7265 2061 206d   a bug where a m
-00007d60: 6973 7369 6e67 2063 6f6e 7461 696e 6572  issing container
-00007d70: 2070 6f72 7420 696e 2061 2070 6f72 7420   port in a port 
-00007d80: 6d61 7070 696e 6720 776f 756c 6420 7261  mapping would ra
-00007d90: 6973 650a 2020 616e 2075 6e65 7870 6563  ise.  an unexpec
-00007da0: 7465 6420 6054 7970 6545 7272 6f72 600a  ted `TypeError`.
-00007db0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-00007dc0: 6572 6520 7468 6520 6065 7665 6e74 7360  ere the `events`
-00007dd0: 206d 6574 686f 6420 696e 2060 4150 4943   method in `APIC
-00007de0: 6c69 656e 7460 2061 6e64 2060 446f 636b  lient` and `Dock
-00007df0: 6572 436c 6965 6e74 600a 2020 776f 756c  erClient`.  woul
-00007e00: 6420 6e6f 7420 7265 7370 6563 7420 6375  d not respect cu
-00007e10: 7374 6f6d 2068 6561 6465 7273 2073 6574  stom headers set
-00007e20: 2069 6e20 6063 6f6e 6669 672e 6a73 6f6e   in `config.json
-00007e30: 600a 0a0a 322e 312e 300a 2d2d 2d2d 2d0a  `...2.1.0.-----.
-00007e40: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
-00007e50: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
-00007e60: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
-00007e70: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
-00007e80: 6572 2f64 6f63 6b65 722d 7079 2f6d 696c  er/docker-py/mil
-00007e90: 6573 746f 6e65 2f32 373f 636c 6f73 6564  estone/27?closed
-00007ea0: 3d31 290a 0a23 2323 2046 6561 7475 7265  =1)..### Feature
-00007eb0: 730a 0a2a 2041 6464 6564 2074 6865 2066  s..* Added the f
-00007ec0: 6f6c 6c6f 7769 6e67 2070 7275 6e69 6e67  ollowing pruning
-00007ed0: 206d 6574 686f 6473 3a0a 2020 2020 2a20   methods:.    * 
-00007ee0: 496e 2060 4150 4943 6c69 656e 7460 3a20  In `APIClient`: 
-00007ef0: 6070 7275 6e65 5f63 6f6e 7461 696e 6572  `prune_container
-00007f00: 7360 2c20 6070 7275 6e65 5f69 6d61 6765  s`, `prune_image
-00007f10: 7360 2c20 6070 7275 6e65 5f6e 6574 776f  s`, `prune_netwo
-00007f20: 726b 7360 2c0a 2020 2020 2020 6070 7275  rks`,.      `pru
-00007f30: 6e65 5f76 6f6c 756d 6573 600a 2020 2020  ne_volumes`.    
-00007f40: 2a20 496e 2060 446f 636b 6572 436c 6965  * In `DockerClie
-00007f50: 6e74 603a 2060 636f 6e74 6169 6e65 7273  nt`: `containers
-00007f60: 2e70 7275 6e65 602c 2060 696d 6167 6573  .prune`, `images
-00007f70: 2e70 7275 6e65 602c 2060 6e65 7477 6f72  .prune`, `networ
-00007f80: 6b73 2e70 7275 6e65 602c 0a20 2020 2020  ks.prune`,.     
-00007f90: 2060 766f 6c75 6d65 732e 7072 756e 6560   `volumes.prune`
-00007fa0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-00007fb0: 2066 6f72 2074 6865 2070 6c75 6769 6e73   for the plugins
-00007fc0: 2041 5049 3a0a 2020 2020 2a20 496e 2060   API:.    * In `
-00007fd0: 4150 4943 6c69 656e 7460 3a20 6063 6f6e  APIClient`: `con
-00007fe0: 6669 6775 7265 5f70 6c75 6769 6e60 2c20  figure_plugin`, 
-00007ff0: 6063 7265 6174 655f 706c 7567 696e 602c  `create_plugin`,
-00008000: 2060 6469 7361 626c 655f 706c 7567 696e   `disable_plugin
-00008010: 602c 0a20 2020 2020 2060 656e 6162 6c65  `,.      `enable
-00008020: 5f70 6c75 6769 6e60 2c20 6069 6e73 7065  _plugin`, `inspe
-00008030: 6374 5f70 6c75 6769 6e60 2c20 6070 756c  ct_plugin`, `pul
-00008040: 6c5f 706c 7567 696e 602c 2060 706c 7567  l_plugin`, `plug
-00008050: 696e 7360 2c0a 2020 2020 2020 6070 6c75  ins`,.      `plu
-00008060: 6769 6e5f 7072 6976 696c 6567 6573 602c  gin_privileges`,
-00008070: 2060 7075 7368 5f70 6c75 6769 6e60 2c20   `push_plugin`, 
-00008080: 6072 656d 6f76 655f 706c 7567 696e 600a  `remove_plugin`.
-00008090: 2020 2020 2a20 496e 2060 446f 636b 6572      * In `Docker
-000080a0: 436c 6965 6e74 603a 2060 706c 7567 696e  Client`: `plugin
-000080b0: 732e 6372 6561 7465 602c 2060 706c 7567  s.create`, `plug
-000080c0: 696e 732e 6765 7460 2c20 6070 6c75 6769  ins.get`, `plugi
-000080d0: 6e73 2e69 6e73 7461 6c6c 602c 0a20 2020  ns.install`,.   
-000080e0: 2020 2060 706c 7567 696e 732e 6c69 7374     `plugins.list
-000080f0: 602c 2061 6e64 2074 6865 2060 506c 7567  `, and the `Plug
-00008100: 696e 6020 6d6f 6465 6c2e 0a2a 2041 6464  in` model..* Add
-00008110: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
-00008120: 6865 2073 6563 7265 7473 2041 5049 3a0a  he secrets API:.
-00008130: 2020 2020 2a20 496e 2060 4150 4943 6c69      * In `APICli
-00008140: 656e 7460 3a20 6063 7265 6174 655f 7365  ent`: `create_se
-00008150: 6372 6574 602c 2060 696e 7370 6563 745f  cret`, `inspect_
-00008160: 7365 6372 6574 602c 2060 7265 6d6f 7665  secret`, `remove
-00008170: 5f73 6563 7265 7460 2c0a 2020 2020 2020  _secret`,.      
-00008180: 6073 6563 7265 7473 600a 2020 2020 2a20  `secrets`.    * 
-00008190: 496e 2060 446f 636b 6572 436c 6965 6e74  In `DockerClient
-000081a0: 603a 2060 7365 6372 6574 2e63 7265 6174  `: `secret.creat
-000081b0: 6560 2c20 6073 6563 7265 742e 6765 7460  e`, `secret.get`
-000081c0: 2c20 6073 6563 7265 742e 6c69 7374 6020  , `secret.list` 
-000081d0: 616e 640a 2020 2020 2020 7468 6520 6053  and.      the `S
-000081e0: 6563 7265 7460 206d 6f64 656c 2e0a 2020  ecret` model..  
-000081f0: 2020 2a20 4164 6465 6420 6073 6563 7265    * Added `secre
-00008200: 7473 6020 7061 7261 6d65 7465 7220 746f  ts` parameter to
-00008210: 2060 436f 6e74 6169 6e65 7253 7065 6360   `ContainerSpec`
-00008220: 2e20 4561 6368 2069 7465 6d20 696e 2074  . Each item in t
-00008230: 6865 2060 7365 6372 6574 7360 0a20 2020  he `secrets`.   
-00008240: 2020 206c 6973 7420 6d75 7374 2062 6520     list must be 
-00008250: 6120 6064 6f63 6b65 722e 7479 7065 732e  a `docker.types.
-00008260: 5365 6372 6574 5265 6665 7265 6e63 6560  SecretReference`
-00008270: 2069 6e73 7461 6e63 652e 0a2a 2041 6464   instance..* Add
-00008280: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
-00008290: 6361 6368 655f 6672 6f6d 6020 696e 2060  cache_from` in `
-000082a0: 4150 4943 6c69 656e 742e 6275 696c 6460  APIClient.build`
-000082b0: 2061 6e64 0a20 2060 446f 636b 6572 436c   and.  `DockerCl
-000082c0: 6965 6e74 2e69 6d61 6765 732e 6275 696c  ient.images.buil
-000082d0: 6460 2e0a 2a20 4164 6465 6420 7375 7070  d`..* Added supp
-000082e0: 6f72 7420 666f 7220 6061 7574 6f5f 7265  ort for `auto_re
-000082f0: 6d6f 7665 6020 616e 6420 6073 746f 7261  move` and `stora
-00008300: 6765 5f6f 7074 6020 696e 0a20 2060 4150  ge_opt` in.  `AP
-00008310: 4943 6c69 656e 742e 6372 6561 7465 5f68  IClient.create_h
-00008320: 6f73 745f 636f 6e66 6967 6020 616e 6420  ost_config` and 
-00008330: 6044 6f63 6b65 7243 6c69 656e 742e 636f  `DockerClient.co
-00008340: 6e74 6169 6e65 7273 2e72 756e 600a 2a20  ntainers.run`.* 
-00008350: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-00008360: 7220 6073 746f 705f 7469 6d65 6f75 7460  r `stop_timeout`
-00008370: 2069 6e20 6041 5049 436c 6965 6e74 2e63   in `APIClient.c
-00008380: 7265 6174 655f 636f 6e74 6169 6e65 7260  reate_container`
-00008390: 2061 6e64 0a20 2060 446f 636b 6572 436c   and.  `DockerCl
-000083a0: 6965 6e74 2e63 6f6e 7461 696e 6572 732e  ient.containers.
-000083b0: 7275 6e60 0a2a 2041 6464 6564 2073 7570  run`.* Added sup
-000083c0: 706f 7274 2066 6f72 2074 6865 2060 666f  port for the `fo
-000083d0: 7263 6560 2070 6172 616d 6574 6572 2069  rce` parameter i
-000083e0: 6e20 6041 5049 436c 6965 6e74 2e72 656d  n `APIClient.rem
-000083f0: 6f76 655f 766f 6c75 6d65 6020 616e 640a  ove_volume` and.
-00008400: 2020 6056 6f6c 756d 652e 7265 6d6f 7665    `Volume.remove
-00008410: 600a 2a20 4164 6465 6420 7375 7070 6f72  `.* Added suppor
-00008420: 7420 666f 7220 606d 6178 5f66 6169 6c75  t for `max_failu
-00008430: 7265 5f72 6174 696f 6020 616e 6420 606d  re_ratio` and `m
-00008440: 6f6e 6974 6f72 6020 696e 2060 5570 6461  onitor` in `Upda
-00008450: 7465 436f 6e66 6967 600a 2a20 4164 6465  teConfig`.* Adde
-00008460: 6420 7375 7070 6f72 7420 666f 7220 6066  d support for `f
-00008470: 6f72 6365 5f75 7064 6174 6560 2069 6e20  orce_update` in 
-00008480: 6054 6173 6b54 656d 706c 6174 6560 0a2a  `TaskTemplate`.*
-00008490: 204d 6164 6520 606e 616d 6560 2070 6172   Made `name` par
-000084a0: 616d 6574 6572 206f 7074 696f 6e61 6c20  ameter optional 
-000084b0: 696e 2060 4150 4943 6c69 656e 742e 6372  in `APIClient.cr
-000084c0: 6561 7465 5f76 6f6c 756d 6560 2061 6e64  eate_volume` and
-000084d0: 0a20 2060 446f 636b 6572 436c 6965 6e74  .  `DockerClient
-000084e0: 2e76 6f6c 756d 6573 2e63 7265 6174 6560  .volumes.create`
-000084f0: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-00008500: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-00008510: 6572 6520 6275 696c 6469 6e67 2066 726f  ere building fro
-00008520: 6d20 6120 6469 7265 6374 6f72 7920 636f  m a directory co
-00008530: 6e74 6169 6e69 6e67 2073 6f63 6b65 742d  ntaining socket-
-00008540: 7479 7065 2066 696c 6573 0a20 2077 6f75  type files.  wou
-00008550: 6c64 2072 6169 7365 2061 6e20 756e 6578  ld raise an unex
-00008560: 7065 6374 6564 2060 4174 7472 6962 7574  pected `Attribut
-00008570: 6545 7272 6f72 602e 0a2a 2046 6978 6564  eError`..* Fixed
-00008580: 2061 6e20 6973 7375 6520 7468 6174 2077   an issue that w
-00008590: 6173 2070 7265 7665 6e74 696e 6720 7468  as preventing th
-000085a0: 6520 6044 6f63 6b65 7243 6c69 656e 742e  e `DockerClient.
-000085b0: 7377 6172 6d2e 696e 6974 6020 6d65 7468  swarm.init` meth
-000085c0: 6f64 2074 6f0a 2020 7461 6b65 2069 6e74  od to.  take int
-000085d0: 6f20 6163 636f 756e 7420 6172 6775 6d65  o account argume
-000085e0: 6e74 7320 7061 7373 6564 2074 6f20 6974  nts passed to it
-000085f0: 2e0a 2a20 6049 6d61 6765 2e74 6167 6020  ..* `Image.tag` 
-00008600: 6e6f 7720 636f 7272 6563 746c 7920 7265  now correctly re
-00008610: 7475 726e 7320 6120 626f 6f6c 6561 6e20  turns a boolean 
-00008620: 7661 6c75 6520 7570 6f6e 2063 6f6d 706c  value upon compl
-00008630: 6574 696f 6e2e 0a2a 2046 6978 6564 2073  etion..* Fixed s
-00008640: 6576 6572 616c 2069 7373 7565 7320 7265  everal issues re
-00008650: 6c61 7465 6420 746f 2070 6173 7369 6e67  lated to passing
-00008660: 2060 766f 6c75 6d65 7360 2069 6e0a 2020   `volumes` in.  
-00008670: 6044 6f63 6b65 7243 6c69 656e 742e 636f  `DockerClient.co
-00008680: 6e74 6169 6e65 7273 2e72 756e 600a 2a20  ntainers.run`.* 
-00008690: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-000086a0: 6865 7265 2060 446f 636b 6572 436c 6965  here `DockerClie
-000086b0: 6e74 2e69 6d61 6765 2e62 7569 6c64 6020  nt.image.build` 
-000086c0: 776f 756c 646e 2774 2072 6574 7572 6e20  wouldn't return 
-000086d0: 616e 2060 496d 6167 6560 0a20 206f 626a  an `Image`.  obj
-000086e0: 6563 7420 6576 656e 2077 6865 6e20 7468  ect even when th
-000086f0: 6520 6275 696c 6420 7761 7320 7375 6363  e build was succ
-00008700: 6573 7366 756c 0a0a 0a32 2e30 2e32 0a2d  essful...2.0.2.-
-00008710: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-00008720: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-00008730: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-00008740: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00008750: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-00008760: 792f 6d69 6c65 7374 6f6e 652f 3239 3f63  y/milestone/29?c
-00008770: 6c6f 7365 643d 3129 0a0a 2323 2320 4275  losed=1)..### Bu
-00008780: 6766 6978 6573 0a0a 2a20 496e 7374 616c  gfixes..* Instal
-00008790: 6c61 7469 6f6e 206f 6620 7468 6520 7061  lation of the pa
-000087a0: 636b 6167 6520 6e6f 7720 6661 696c 7320  ckage now fails 
-000087b0: 6966 2074 6865 2060 646f 636b 6572 2d70  if the `docker-p
-000087c0: 7960 2070 6163 6b61 6765 2069 730a 2020  y` package is.  
-000087d0: 696e 7374 616c 6c65 6420 696e 206f 7264  installed in ord
-000087e0: 6572 2074 6f20 7072 6576 656e 7420 6f62  er to prevent ob
-000087f0: 7363 7572 6520 6e61 6d69 6e67 2063 6f6e  scure naming con
-00008800: 666c 6963 7473 2077 6865 6e20 626f 7468  flicts when both
-00008810: 0a20 2070 6163 6b61 6765 7320 636f 2d65  .  packages co-e
-00008820: 7869 7374 2e0a 2a20 4164 6465 6420 6d69  xist..* Added mi
-00008830: 7373 696e 6720 6066 696c 7465 7273 6020  ssing `filters` 
-00008840: 7061 7261 6d65 7465 7220 746f 2060 4150  parameter to `AP
-00008850: 4943 6c69 656e 742e 6e65 7477 6f72 6b73  IClient.networks
-00008860: 602e 0a2a 2052 6573 6f75 7263 6520 6f62  `..* Resource ob
-00008870: 6a65 6374 7320 6765 6e65 7261 7465 6420  jects generated 
-00008880: 6279 2074 6865 2060 446f 636b 6572 436c  by the `DockerCl
-00008890: 6965 6e74 6020 6172 6520 6e6f 7720 6861  ient` are now ha
-000088a0: 7368 6162 6c65 2e0a 2a20 4669 7865 6420  shable..* Fixed 
-000088b0: 6120 6275 6720 7768 6572 6520 7265 7472  a bug where retr
-000088c0: 6965 7669 6e67 2075 6e74 6167 6765 6420  ieving untagged 
-000088d0: 696d 6167 6573 2075 7369 6e67 2060 446f  images using `Do
-000088e0: 636b 6572 436c 6965 6e74 600a 2020 776f  ckerClient`.  wo
-000088f0: 756c 6420 7261 6973 6520 6120 6054 7970  uld raise a `Typ
-00008900: 6545 7272 6f72 6020 6578 6365 7074 696f  eError` exceptio
-00008910: 6e2e 0a2a 2060 6d6f 6465 6020 7061 7261  n..* `mode` para
-00008920: 6d65 7465 7220 696e 2060 6372 6561 7465  meter in `create
-00008930: 5f73 6572 7669 6365 6020 6973 206e 6f77  _service` is now
-00008940: 2070 726f 7065 726c 7920 636f 6e76 6572   properly conver
-00008950: 7465 6420 746f 0a20 2061 2076 616c 6964  ted to.  a valid
-00008960: 2064 6174 6120 7479 7065 2066 6f72 2074   data type for t
-00008970: 6865 2045 6e67 696e 6520 4150 492e 2055  he Engine API. U
-00008980: 7365 2060 5365 7276 6963 654d 6f64 6560  se `ServiceMode`
-00008990: 2066 6f72 2061 6476 616e 6365 640a 2020   for advanced.  
-000089a0: 636f 6e66 6967 7572 6174 696f 6e73 2e0a  configurations..
-000089b0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-000089c0: 6572 6520 7468 6520 6465 636f 6465 6420  ere the decoded 
-000089d0: 6041 5049 436c 6965 6e74 2e65 7665 6e74  `APIClient.event
-000089e0: 7360 2073 7472 6561 6d20 776f 756c 6420  s` stream would 
-000089f0: 736f 6d65 7469 6d65 7320 7261 6973 650a  sometimes raise.
-00008a00: 2020 616e 2065 7863 6570 7469 6f6e 2077    an exception w
-00008a10: 6865 6e20 6120 636f 6e74 6169 6e65 7220  hen a container 
-00008a20: 6973 2073 746f 7070 6564 206f 7220 7265  is stopped or re
-00008a30: 7374 6172 7465 642e 0a0a 322e 302e 310a  started...2.0.1.
-00008a40: 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f 6620  -----..[List of 
-00008a50: 5052 7320 2f20 6973 7375 6573 2066 6f72  PRs / issues for
-00008a60: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
-00008a70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00008a80: 6d2f 646f 636b 6572 2f64 6f63 6b65 722d  m/docker/docker-
-00008a90: 7079 2f6d 696c 6573 746f 6e65 2f32 383f  py/milestone/28?
-00008aa0: 636c 6f73 6564 3d31 290a 0a23 2323 2042  closed=1)..### B
-00008ab0: 7567 6669 7865 730a 0a2a 2046 6978 6564  ugfixes..* Fixed
-00008ac0: 2061 2062 7567 2077 6865 7265 2066 6f72   a bug where for
-00008ad0: 7761 7264 2073 6c61 7368 6573 2069 6e20  ward slashes in 
-00008ae0: 736f 6d65 202e 646f 636b 6572 6967 6e6f  some .dockerigno
-00008af0: 7265 2070 6174 7465 726e 7320 7765 7265  re patterns were
-00008b00: 6e27 740a 2020 6265 696e 6720 7061 7273  n't.  being pars
-00008b10: 6564 2063 6f72 7265 6374 6c79 206f 6e20  ed correctly on 
-00008b20: 5769 6e64 6f77 730a 2a20 4669 7865 6420  Windows.* Fixed 
-00008b30: 6120 6275 6720 7768 6572 6520 604d 6f75  a bug where `Mou
-00008b40: 6e74 2e70 6172 7365 5f6d 6f75 6e74 5f73  nt.parse_mount_s
-00008b50: 7472 696e 6760 2077 6f75 6c64 206e 6576  tring` would nev
-00008b60: 6572 2073 6574 2074 6865 2072 6561 645f  er set the read_
-00008b70: 6f6e 6c79 0a20 2070 6172 616d 6574 6572  only.  parameter
-00008b80: 206f 6e20 7468 6520 7265 7375 6c74 696e   on the resultin
-00008b90: 6720 604d 6f75 6e74 602e 0a2a 2046 6978  g `Mount`..* Fix
-00008ba0: 6564 2061 2062 7567 2077 6865 7265 2060  ed a bug where `
-00008bb0: 4d6f 756e 742e 7061 7273 655f 6d6f 756e  Mount.parse_moun
-00008bc0: 745f 7374 7269 6e67 6020 776f 756c 6420  t_string` would 
-00008bd0: 696e 636f 7272 6563 746c 7920 6d61 726b  incorrectly mark
-00008be0: 2068 6f73 740a 2020 6269 6e64 7320 6173   host.  binds as
-00008bf0: 2062 6569 6e67 206f 6620 6076 6f6c 756d   being of `volum
-00008c00: 6560 2074 7970 652e 0a0a 322e 302e 300a  e` type...2.0.0.
-00008c10: 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f 6620  -----..[List of 
-00008c20: 5052 7320 2f20 6973 7375 6573 2066 6f72  PRs / issues for
-00008c30: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
-00008c40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00008c50: 6d2f 646f 636b 6572 2f64 6f63 6b65 722d  m/docker/docker-
-00008c60: 7079 2f6d 696c 6573 746f 6e65 2f32 323f  py/milestone/22?
-00008c70: 636c 6f73 6564 3d31 290a 0a23 2323 2042  closed=1)..### B
-00008c80: 7265 616b 696e 6720 6368 616e 6765 730a  reaking changes.
-00008c90: 0a2a 2044 726f 7070 6564 2073 7570 706f  .* Dropped suppo
-00008ca0: 7274 2066 6f72 2050 7974 686f 6e20 322e  rt for Python 2.
-00008cb0: 360a 2a20 6064 6f63 6b65 722e 436c 6965  6.* `docker.Clie
-00008cc0: 6e74 6020 6861 7320 6265 656e 2072 656e  nt` has been ren
-00008cd0: 616d 6564 2074 6f20 6064 6f63 6b65 722e  amed to `docker.
-00008ce0: 4150 4943 6c69 656e 7460 0a2a 2060 646f  APIClient`.* `do
-00008cf0: 636b 6572 2e66 726f 6d5f 656e 7660 206e  cker.from_env` n
-00008d00: 6f77 2063 7265 6174 6573 2061 2060 446f  ow creates a `Do
-00008d10: 636b 6572 436c 6965 6e74 6020 696e 7374  ckerClient` inst
-00008d20: 616e 6365 2069 6e73 7465 6164 206f 6620  ance instead of 
-00008d30: 616e 0a20 2060 4150 4943 6c69 656e 7460  an.  `APIClient`
-00008d40: 2069 6e73 7461 6e63 652e 0a2a 2052 656d   instance..* Rem
-00008d50: 6f76 6564 2048 6f73 7443 6f6e 6669 6720  oved HostConfig 
-00008d60: 7061 7261 6d65 7465 7273 2066 726f 6d20  parameters from 
-00008d70: 6041 5049 436c 6965 6e74 2e73 7461 7274  `APIClient.start
-00008d80: 600a 2a20 5468 6520 6d69 6e69 6d75 6d20  `.* The minimum 
-00008d90: 7375 7070 6f72 7465 6420 4150 4920 7665  supported API ve
-00008da0: 7273 696f 6e20 6973 206e 6f77 2031 2e32  rsion is now 1.2
-00008db0: 3120 2845 6e67 696e 6520 7665 7273 696f  1 (Engine versio
-00008dc0: 6e20 312e 392e 302b 290a 2a20 5468 6520  n 1.9.0+).* The 
-00008dd0: 6e61 6d65 206f 6620 7468 6520 6070 6970  name of the `pip
-00008de0: 6020 7061 636b 6167 6520 6973 206e 6f77  ` package is now
-00008df0: 2060 646f 636b 6572 6020 2877 6173 3a20   `docker` (was: 
-00008e00: 6064 6f63 6b65 722d 7079 6029 2e20 4e65  `docker-py`). Ne
-00008e10: 770a 2020 7665 7273 696f 6e73 206f 6620  w.  versions of 
-00008e20: 7468 6973 206c 6962 7261 7279 2077 696c  this library wil
-00008e30: 6c20 6f6e 6c79 2062 6520 7075 626c 6973  l only be publis
-00008e40: 6865 6420 6173 2060 646f 636b 6572 6020  hed as `docker` 
-00008e50: 6672 6f6d 206e 6f77 206f 6e2e 0a2a 2060  from now on..* `
-00008e60: 646f 636b 6572 2e73 736c 6164 6170 7465  docker.ssladapte
-00008e70: 7260 2069 7320 6e6f 7720 6064 6f63 6b65  r` is now `docke
-00008e80: 722e 7472 616e 7370 6f72 742e 7373 6c61  r.transport.ssla
-00008e90: 6461 7074 6572 600a 2a20 5468 6520 7061  dapter`.* The pa
-00008ea0: 636b 6167 6520 7374 7275 6374 7572 6520  ckage structure 
-00008eb0: 6861 7320 6265 656e 2066 6c61 7474 656e  has been flatten
-00008ec0: 6564 2069 6e20 6365 7274 6169 6e20 6361  ed in certain ca
-00008ed0: 7365 732c 2077 6869 6368 206d 6179 2061  ses, which may a
-00008ee0: 6666 6563 740a 2020 696d 706f 7274 2066  ffect.  import f
-00008ef0: 6f72 2060 646f 636b 6572 2e61 7574 6860  or `docker.auth`
-00008f00: 2061 6e64 2060 646f 636b 6572 2e75 7469   and `docker.uti
-00008f10: 6c73 2e70 6f72 7473 600a 2a20 6064 6f63  ls.ports`.* `doc
-00008f20: 6b65 722e 7574 696c 732e 7479 7065 7360  ker.utils.types`
-00008f30: 2068 6173 2062 6565 6e20 6d6f 7665 6420   has been moved 
-00008f40: 746f 2060 646f 636b 6572 2e74 7970 6573  to `docker.types
-00008f50: 600a 2a20 6063 7265 6174 655f 686f 7374  `.* `create_host
-00008f60: 5f63 6f6e 6669 6760 2c20 6063 7265 6174  _config`, `creat
-00008f70: 655f 6970 616d 5f70 6f6f 6c60 2061 6e64  e_ipam_pool` and
-00008f80: 2060 6372 6561 7465 5f69 7061 6d5f 636f   `create_ipam_co
-00008f90: 6e66 6967 6020 6861 7665 2062 6565 6e0a  nfig` have been.
-00008fa0: 2020 7265 6d6f 7665 6420 6672 6f6d 2060    removed from `
-00008fb0: 646f 636b 6572 2e75 7469 6c73 602e 2054  docker.utils`. T
-00008fc0: 6865 7920 6861 7665 2062 6565 6e20 7265  hey have been re
-00008fd0: 706c 6163 6564 2062 7920 7468 6520 666f  placed by the fo
-00008fe0: 6c6c 6f77 696e 6720 636c 6173 7365 730a  llowing classes.
-00008ff0: 2020 696e 2060 646f 636b 6572 2e74 7970    in `docker.typ
-00009000: 6573 603a 2060 486f 7374 436f 6e66 6967  es`: `HostConfig
-00009010: 602c 2060 4950 414d 506f 6f6c 6020 616e  `, `IPAMPool` an
-00009020: 6420 6049 5041 4d43 4f6e 6669 6760 2e0a  d `IPAMCOnfig`..
-00009030: 0a23 2323 2046 6561 7475 7265 730a 0a2a  .### Features..*
-00009040: 2041 6464 6564 2061 2068 6967 682d 6c65   Added a high-le
-00009050: 7665 6c2c 2075 7365 722d 666f 6375 7365  vel, user-focuse
-00009060: 6420 4150 4920 6173 2060 646f 636b 6572  d API as `docker
-00009070: 2e44 6f63 6b65 7243 6c69 656e 7460 2e20  .DockerClient`. 
-00009080: 5365 6520 7468 650a 2020 5245 4144 4d45  See the.  README
-00009090: 2061 6e64 2064 6f63 756d 656e 7461 7469   and documentati
-000090a0: 6f6e 2066 6f72 206d 6f72 6520 696e 666f  on for more info
-000090b0: 726d 6174 696f 6e2e 0a2a 2049 6d70 6c65  rmation..* Imple
-000090c0: 6d65 6e74 6564 2060 7570 6461 7465 5f6e  mented `update_n
-000090d0: 6f64 6560 206d 6574 686f 6420 696e 2060  ode` method in `
-000090e0: 4150 4943 6c69 656e 7460 2e0a 2a20 496d  APIClient`..* Im
-000090f0: 706c 656d 656e 7465 6420 6072 656d 6f76  plemented `remov
-00009100: 655f 6e6f 6465 6020 6d65 7468 6f64 2069  e_node` method i
-00009110: 6e20 6041 5049 436c 6965 6e74 602e 0a2a  n `APIClient`..*
-00009120: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-00009130: 6f72 2060 7265 7374 6172 745f 706f 6c69  or `restart_poli
-00009140: 6379 6020 696e 2060 7570 6461 7465 5f63  cy` in `update_c
-00009150: 6f6e 7461 696e 6572 602e 0a2a 2041 6464  ontainer`..* Add
-00009160: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
-00009170: 6c61 6265 6c73 6020 616e 6420 6073 686d  labels` and `shm
-00009180: 7369 7a65 6020 696e 2060 6275 696c 6460  size` in `build`
-00009190: 2e0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
-000091a0: 7420 666f 7220 6061 7474 6163 6861 626c  t for `attachabl
-000091b0: 6560 2069 6e20 6063 7265 6174 655f 6e65  e` in `create_ne
-000091c0: 7477 6f72 6b60 0a2a 2041 6464 6564 2073  twork`.* Added s
-000091d0: 7570 706f 7274 2066 6f72 2060 6865 616c  upport for `heal
-000091e0: 7468 6368 6563 6b60 2069 6e20 6063 7265  thcheck` in `cre
-000091f0: 6174 655f 636f 6e74 6169 6e65 7260 2e0a  ate_container`..
-00009200: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-00009210: 666f 7220 6069 736f 6c61 7469 6f6e 6020  for `isolation` 
-00009220: 696e 2060 486f 7374 436f 6e66 6967 602e  in `HostConfig`.
-00009230: 0a2a 2045 7870 616e 6465 6420 7375 7070  .* Expanded supp
-00009240: 6f72 7420 666f 7220 6070 6964 5f6d 6f64  ort for `pid_mod
-00009250: 6560 2069 6e20 6048 6f73 7443 6f6e 6669  e` in `HostConfi
-00009260: 6760 2028 6e6f 7720 7375 7070 6f72 7473  g` (now supports
-00009270: 2061 7262 6974 7261 7279 0a20 2076 616c   arbitrary.  val
-00009280: 7565 7320 666f 7220 4150 4920 7665 7273  ues for API vers
-00009290: 696f 6e20 3e3d 2031 2e32 3429 2e0a 2a20  ion >= 1.24)..* 
-000092a0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-000092b0: 7220 606f 7074 696f 6e73 6020 696e 2060  r `options` in `
-000092c0: 4950 414d 436f 6e66 6967 600a 2a20 4164  IPAMConfig`.* Ad
-000092d0: 6465 6420 6120 6048 6561 6c74 6843 6865  ded a `HealthChe
-000092e0: 636b 6020 636c 6173 7320 746f 2060 646f  ck` class to `do
-000092f0: 636b 6572 2e74 7970 6573 6020 746f 2062  cker.types` to b
-00009300: 6520 7573 6564 2069 6e0a 2020 6063 7265  e used in.  `cre
-00009310: 6174 655f 636f 6e74 6169 6e65 7260 2e0a  ate_container`..
-00009320: 2a20 4164 6465 6420 616e 2060 456e 6470  * Added an `Endp
-00009330: 6f69 6e74 5370 6563 6020 636c 6173 7320  ointSpec` class 
-00009340: 746f 2060 646f 636b 6572 2e74 7970 6573  to `docker.types
-00009350: 6020 746f 2062 6520 7573 6564 2069 6e0a  ` to be used in.
-00009360: 2020 6063 7265 6174 655f 7365 7276 6963    `create_servic
-00009370: 6560 2061 6e64 2060 7570 6461 7465 5f73  e` and `update_s
-00009380: 6572 7669 6365 602e 0a0a 0a23 2323 2042  ervice`....### B
-00009390: 7567 6669 7865 730a 0a2a 2046 6978 6564  ugfixes..* Fixed
-000093a0: 2061 2062 7567 2077 6865 7265 2061 7574   a bug where aut
-000093b0: 6820 696e 666f 726d 6174 696f 6e20 776f  h information wo
-000093c0: 756c 6420 6e6f 7420 6265 2070 726f 7065  uld not be prope
-000093d0: 726c 7920 7061 7373 6564 2074 6f20 7468  rly passed to th
-000093e0: 6520 656e 6769 6e65 0a20 2064 7572 696e  e engine.  durin
-000093f0: 6720 6120 6062 7569 6c64 6020 6966 2074  g a `build` if t
-00009400: 6865 2063 6c69 656e 7420 7573 6564 2061  he client used a
-00009410: 2063 7265 6465 6e74 6961 6c73 2073 746f   credentials sto
-00009420: 7265 2e0a 2a20 4669 7865 6420 616e 2069  re..* Fixed an i
-00009430: 7373 7565 2077 6974 6820 736f 6d65 2065  ssue with some e
-00009440: 7863 6c75 7369 6f6e 2070 6174 7465 726e  xclusion pattern
-00009450: 7320 696e 2060 6275 696c 6460 2e0a 2a20  s in `build`..* 
-00009460: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-00009470: 6865 7265 2063 6f6e 7465 7874 2066 696c  here context fil
-00009480: 6573 2077 6572 6520 6275 6e64 6c65 6420  es were bundled 
-00009490: 7769 7468 2074 6865 2077 726f 6e67 2070  with the wrong p
-000094a0: 6572 6d69 7373 696f 6e73 0a20 2077 6865  ermissions.  whe
-000094b0: 6e20 6361 6c6c 696e 6720 6062 7569 6c64  n calling `build
-000094c0: 6020 6f6e 2057 696e 646f 7773 2e0a 2a20  ` on Windows..* 
-000094d0: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-000094e0: 6865 7265 2061 7574 6820 696e 666f 2077  here auth info w
-000094f0: 6f75 6c64 206e 6f74 2062 6520 7265 7472  ould not be retr
-00009500: 6965 7665 6420 6672 6f6d 2069 7473 2064  ieved from its d
-00009510: 6566 6175 6c74 206c 6f63 6174 696f 6e0a  efault location.
-00009520: 2020 6f6e 2057 696e 646f 7773 2e0a 2a20    on Windows..* 
-00009530: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-00009540: 6865 7265 206c 6973 7473 206f 6620 606e  here lists of `n
-00009550: 6574 776f 726b 7360 2069 6e20 6063 7265  etworks` in `cre
-00009560: 6174 655f 7365 7276 6963 6560 2061 6e64  ate_service` and
-00009570: 0a20 2060 7570 6461 7465 5f73 6572 7669  .  `update_servi
-00009580: 6365 6020 776f 756c 646e 2774 2062 6520  ce` wouldn't be 
-00009590: 7072 6f70 6572 6c79 2063 6f6e 7665 7274  properly convert
-000095a0: 6564 2066 6f72 2074 6865 2065 6e67 696e  ed for the engin
-000095b0: 652e 0a2a 2046 6978 6564 2061 6e20 6973  e..* Fixed an is
-000095c0: 7375 6520 7768 6572 6520 6065 6e64 706f  sue where `endpo
-000095d0: 696e 745f 636f 6e66 6967 6020 696e 2060  int_config` in `
-000095e0: 6372 6561 7465 5f73 6572 7669 6365 6020  create_service` 
-000095f0: 616e 640a 2020 6075 7064 6174 655f 7365  and.  `update_se
-00009600: 7276 6963 6560 2077 6f75 6c64 2062 6520  rvice` would be 
-00009610: 6967 6e6f 7265 642e 0a2a 2060 656e 6470  ignored..* `endp
-00009620: 6f69 6e74 5f63 6f6e 6669 6760 2069 6e20  oint_config` in 
-00009630: 6063 7265 6174 655f 7365 7276 6963 6560  `create_service`
-00009640: 2061 6e64 2060 7570 6461 7465 5f73 6572   and `update_ser
-00009650: 7669 6365 6020 6861 7320 6265 656e 0a20  vice` has been. 
-00009660: 2064 6570 7265 6361 7465 6420 696e 2066   deprecated in f
-00009670: 6176 6f72 206f 6620 6065 6e64 706f 696e  avor of `endpoin
-00009680: 745f 7370 6563 600a 2a20 4669 7865 6420  t_spec`.* Fixed 
-00009690: 6120 6275 6720 7768 6572 6520 6063 6f6e  a bug where `con
-000096a0: 7374 7261 696e 7473 6020 696e 2061 2060  straints` in a `
-000096b0: 5461 736b 5465 6d70 6c61 7465 6020 6f62  TaskTemplate` ob
-000096c0: 6a65 6374 2077 6f75 6c64 6e27 7420 6265  ject wouldn't be
-000096d0: 0a20 2070 726f 7065 726c 7920 636f 6e76  .  properly conv
-000096e0: 6572 7465 6420 666f 7220 7468 6520 656e  erted for the en
-000096f0: 6769 6e65 2e0a 2a20 4669 7865 6420 616e  gine..* Fixed an
-00009700: 2069 7373 7565 2077 6865 7265 2070 726f   issue where pro
-00009710: 7669 6469 6e67 2061 2064 6963 7469 6f6e  viding a diction
-00009720: 6172 7920 666f 7220 6065 6e76 6020 696e  ary for `env` in
-00009730: 2060 436f 6e74 6169 6e65 7253 7065 6360   `ContainerSpec`
-00009740: 0a20 2077 6f75 6c64 2070 726f 766f 6b65  .  would provoke
-00009750: 2061 6e20 6041 5049 4572 726f 7260 2077   an `APIError` w
-00009760: 6865 6e20 7365 6e74 2074 6f20 7468 6520  hen sent to the 
-00009770: 656e 6769 6e65 2e0a 2a20 4669 7865 6420  engine..* Fixed 
-00009780: 6120 6275 6720 7768 6572 6520 7072 6f76  a bug where prov
-00009790: 6964 696e 6720 616e 2060 656e 765f 6669  iding an `env_fi
-000097a0: 6c65 6020 636f 6e74 6169 6e69 6e67 2065  le` containing e
-000097b0: 6d70 7479 206c 696e 6573 2069 6e0a 2020  mpty lines in.  
-000097c0: 6063 7265 6174 655f 636f 6e74 6169 6e65  `create_containe
-000097d0: 7260 776f 756c 6420 7261 6973 6520 616e  r`would raise an
-000097e0: 2065 7863 6570 7469 6f6e 2e0a 2a20 4669   exception..* Fi
-000097f0: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
-00009800: 6064 6574 6163 6860 2077 6173 2062 6569  `detach` was bei
-00009810: 6e67 2069 676e 6f72 6564 2062 7920 6065  ng ignored by `e
-00009820: 7865 635f 7374 6172 7460 2e0a 0a23 2323  xec_start`...###
-00009830: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
-00009840: 2a20 446f 6375 6d65 6e74 6174 696f 6e20  * Documentation 
-00009850: 666f 7220 636c 6173 7365 7320 616e 6420  for classes and 
-00009860: 6d65 7468 6f64 7320 6973 206e 6f77 2069  methods is now i
-00009870: 6e63 6c75 6465 6420 616c 6f6e 6773 6964  ncluded alongsid
-00009880: 6520 7468 6520 636f 6465 2061 730a 2020  e the code as.  
-00009890: 646f 6373 7472 696e 6773 2e0a 0a31 2e31  docstrings...1.1
-000098a0: 302e 360a 2d2d 2d2d 2d2d 0a0a 5b4c 6973  0.6.------..[Lis
-000098b0: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
-000098c0: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
-000098d0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-000098e0: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
-000098f0: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
-00009900: 652f 3236 3f63 6c6f 7365 643d 3129 0a0a  e/26?closed=1)..
-00009910: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
-00009920: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-00009930: 6865 7265 2073 6574 7469 6e67 2061 2060  here setting a `
-00009940: 4e70 6970 6553 6f63 6b65 7460 2069 6e73  NpipeSocket` ins
-00009950: 7461 6e63 6520 746f 2062 6c6f 636b 696e  tance to blockin
-00009960: 6720 6d6f 6465 2077 6f75 6c64 0a20 2070  g mode would.  p
-00009970: 7574 2069 7420 696e 206e 6f6e 2d62 6c6f  ut it in non-blo
-00009980: 636b 696e 6720 6d6f 6465 2061 6e64 2076  cking mode and v
-00009990: 6963 652d 7665 7273 612e 0a0a 0a31 2e31  ice-versa....1.1
-000099a0: 302e 350a 2d2d 2d2d 2d2d 0a0a 5b4c 6973  0.5.------..[Lis
-000099b0: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
-000099c0: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
-000099d0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-000099e0: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
-000099f0: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
-00009a00: 652f 3235 3f63 6c6f 7365 643d 3129 0a0a  e/25?closed=1)..
-00009a10: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
-00009a20: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-00009a30: 6865 7265 2063 6f6e 6375 7272 656e 7420  here concurrent 
-00009a40: 6174 7465 6d70 7473 2074 6f20 6163 6365  attempts to acce
-00009a50: 7373 2074 6f20 6120 6e61 6d65 6420 7069  ss to a named pi
-00009a60: 7065 2062 7920 7468 650a 2020 636c 6965  pe by the.  clie
-00009a70: 6e74 2077 6f75 6c64 2073 6f6d 6574 696d  nt would sometim
-00009a80: 6573 2063 6175 7365 2072 6563 6f76 6572  es cause recover
-00009a90: 6162 6c65 2065 7863 6570 7469 6f6e 7320  able exceptions 
-00009aa0: 746f 2062 6520 7261 6973 6564 2e0a 0a0a  to be raised....
-00009ab0: 312e 3130 2e34 0a2d 2d2d 2d2d 2d0a 0a5b  1.10.4.------..[
-00009ac0: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
-00009ad0: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
-00009ae0: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00009af0: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
-00009b00: 2f64 6f63 6b65 722d 7079 2f6d 696c 6573  /docker-py/miles
-00009b10: 746f 6e65 2f32 343f 636c 6f73 6564 3d31  tone/24?closed=1
-00009b20: 290a 0a23 2323 2042 7567 6669 7865 730a  )..### Bugfixes.
-00009b30: 0a2a 2046 6978 6564 2061 6e20 6973 7375  .* Fixed an issu
-00009b40: 6520 7768 6572 6520 6052 6573 7461 7274  e where `Restart
-00009b50: 506f 6c69 6379 2e63 6f6e 6469 7469 6f6e  Policy.condition
-00009b60: 5f74 7970 6573 2e4f 4e5f 4641 494c 5552  _types.ON_FAILUR
-00009b70: 4560 2077 6f75 6c64 2079 6965 6c64 0a20  E` would yield. 
-00009b80: 2061 6e20 696e 7661 6c69 6420 7661 6c75   an invalid valu
-00009b90: 652e 0a2a 2046 6978 6564 2061 6e20 6973  e..* Fixed an is
-00009ba0: 7375 6520 7768 6572 6520 7468 6520 5353  sue where the SS
-00009bb0: 4c20 636f 6e6e 6563 7469 6f6e 2061 6461  L connection ada
-00009bc0: 7074 6572 2077 6f75 6c64 2072 6563 6569  pter would recei
-00009bd0: 7665 2061 6e20 696e 7661 6c69 640a 2020  ve an invalid.  
-00009be0: 6172 6775 6d65 6e74 2e0a 2a20 4669 7865  argument..* Fixe
-00009bf0: 6420 616e 2069 7373 7565 2074 6861 7420  d an issue that 
-00009c00: 6361 7573 6564 2074 6865 2043 6c69 656e  caused the Clien
-00009c10: 7420 746f 2066 6169 6c20 746f 2072 6561  t to fail to rea
-00009c20: 6368 2041 5049 2065 6e64 706f 696e 7473  ch API endpoints
-00009c30: 2077 6865 6e0a 2020 7468 6520 7072 6f76   when.  the prov
-00009c40: 6964 6564 2060 6261 7365 5f75 726c 6020  ided `base_url` 
-00009c50: 6861 6420 6120 7472 6169 6c69 6e67 2073  had a trailing s
-00009c60: 6c61 7368 2e0a 2a20 4669 7865 6420 6120  lash..* Fixed a 
-00009c70: 6275 6720 7768 6572 6520 736f 6d65 2060  bug where some `
-00009c80: 656e 7669 726f 6e6d 656e 7460 2076 616c  environment` val
-00009c90: 7565 7320 696e 2060 6372 6561 7465 5f63  ues in `create_c
-00009ca0: 6f6e 7461 696e 6572 600a 2020 636f 6e74  ontainer`.  cont
-00009cb0: 6169 6e69 6e67 2075 6e69 636f 6465 2063  aining unicode c
-00009cc0: 6861 7261 6374 6572 7320 776f 756c 6420  haracters would 
-00009cd0: 7261 6973 6520 616e 2065 6e63 6f64 696e  raise an encodin
-00009ce0: 6720 6572 726f 722e 0a2a 2046 6978 6564  g error..* Fixed
-00009cf0: 2061 206e 756d 6265 7220 6f66 2069 7373   a number of iss
-00009d00: 7565 7320 7469 6564 2077 6974 6820 6e61  ues tied with na
-00009d10: 6d65 6420 7069 7065 2074 7261 6e73 706f  med pipe transpo
-00009d20: 7274 206f 6e20 5769 6e64 6f77 732e 0a2a  rt on Windows..*
-00009d30: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
-00009d40: 7265 2069 6e63 6c75 7369 6f6e 2070 6174  re inclusion pat
-00009d50: 7465 726e 7320 696e 2060 2e64 6f63 6b65  terns in `.docke
-00009d60: 7269 676e 6f72 6560 2077 6f75 6c64 2063  rignore` would c
-00009d70: 6175 7365 2073 6f6d 650a 2020 6578 636c  ause some.  excl
-00009d80: 7564 6564 2066 696c 6573 2074 6f20 6170  uded files to ap
-00009d90: 7065 6172 2069 6e20 7468 6520 6275 696c  pear in the buil
-00009da0: 6420 636f 6e74 6578 7420 6f6e 2057 696e  d context on Win
-00009db0: 646f 7773 2e0a 0a23 2323 204d 6973 6365  dows...### Misce
-00009dc0: 6c6c 616e 656f 7573 0a0a 2a20 4164 6a75  llaneous..* Adju
-00009dd0: 7374 6564 2076 6572 7369 6f6e 2072 6571  sted version req
-00009de0: 7569 7265 6d65 6e74 7320 666f 7220 7468  uirements for th
-00009df0: 6520 6072 6571 7565 7374 7360 206c 6962  e `requests` lib
-00009e00: 7261 7279 2e0a 2a20 4974 2069 7320 6e6f  rary..* It is no
-00009e10: 7720 706f 7373 6962 6c65 2074 6f20 7275  w possible to ru
-00009e20: 6e20 7468 6520 646f 636b 6572 2d70 7920  n the docker-py 
-00009e30: 7465 7374 2073 7569 7465 206f 6e20 5769  test suite on Wi
-00009e40: 6e64 6f77 732e 0a0a 0a31 2e31 302e 330a  ndows....1.10.3.
-00009e50: 2d2d 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66  ------..[List of
-00009e60: 2050 5273 202f 2069 7373 7565 7320 666f   PRs / issues fo
-00009e70: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
-00009e80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00009e90: 6f6d 2f64 6f63 6b65 722f 646f 636b 6572  om/docker/docker
-00009ea0: 2d70 792f 6973 7375 6573 3f71 3d6d 696c  -py/issues?q=mil
-00009eb0: 6573 746f 6e65 2533 4131 2e31 302e 332b  estone%3A1.10.3+
-00009ec0: 6973 2533 4163 6c6f 7365 6429 0a0a 2323  is%3Aclosed)..##
-00009ed0: 2320 4275 6766 6978 6573 0a0a 2a20 4669  # Bugfixes..* Fi
-00009ee0: 7865 6420 616e 2069 7373 7565 2077 6865  xed an issue whe
-00009ef0: 7265 2069 6465 6e74 6974 7920 746f 6b65  re identity toke
-00009f00: 6e73 2069 6e20 636f 6e66 6967 7572 6174  ns in configurat
-00009f10: 696f 6e20 6669 6c65 7320 7765 7265 6e27  ion files weren'
-00009f20: 7420 6861 6e64 6c65 640a 2020 6279 2074  t handled.  by t
-00009f30: 6865 206c 6962 7261 7279 2e0a 0a23 2323  he library...###
-00009f40: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
-00009f50: 2a20 496e 6372 6561 7365 6420 7468 6520  * Increased the 
-00009f60: 6465 6661 756c 7420 6e75 6d62 6572 206f  default number o
-00009f70: 6620 636f 6e6e 6563 7469 6f6e 2070 6f6f  f connection poo
-00009f80: 6c73 2066 726f 6d20 3130 2074 6f20 3235  ls from 10 to 25
-00009f90: 2e20 5468 6973 206e 756d 6265 720a 2020  . This number.  
-00009fa0: 6361 6e20 6e6f 7720 6265 2063 6f6e 6669  can now be confi
-00009fb0: 6775 7265 6420 7573 696e 6720 7468 6520  gured using the 
-00009fc0: 606e 756d 5f70 6f6f 6c73 6020 7061 7261  `num_pools` para
-00009fd0: 6d65 7465 7220 696e 2074 6865 2060 436c  meter in the `Cl
-00009fe0: 6965 6e74 600a 2020 636f 6e73 7472 7563  ient`.  construc
-00009ff0: 746f 722e 0a0a 0a31 2e31 302e 320a 2d2d  tor....1.10.2.--
-0000a000: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-0000a010: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-0000a020: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-0000a030: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000a040: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-0000a050: 792f 6973 7375 6573 3f71 3d6d 696c 6573  y/issues?q=miles
-0000a060: 746f 6e65 2533 4131 2e31 302e 302b 6973  tone%3A1.10.0+is
-0000a070: 2533 4163 6c6f 7365 6429 0a0a 2323 2320  %3Aclosed)..### 
-0000a080: 4275 6766 6978 6573 0a0a 2a20 5570 6461  Bugfixes..* Upda
-0000a090: 7465 6420 7468 6520 646f 636b 6572 2d70  ted the docker-p
-0000a0a0: 7963 7265 6473 2064 6570 656e 6465 6e63  ycreds dependenc
-0000a0b0: 7920 6173 2069 7420 7761 7320 6361 7573  y as it was caus
-0000a0c0: 696e 6720 6973 7375 6573 2066 6f72 2073  ing issues for s
-0000a0d0: 6f6d 650a 2020 7573 6572 7320 7769 7468  ome.  users with
-0000a0e0: 2064 6570 656e 6465 6e63 7920 7265 736f   dependency reso
-0000a0f0: 6c75 7469 6f6e 2069 6e20 6170 706c 6963  lution in applic
-0000a100: 6174 696f 6e73 2075 7369 6e67 2064 6f63  ations using doc
-0000a110: 6b65 722d 7079 2e0a 0a0a 312e 3130 2e31  ker-py....1.10.1
-0000a120: 0a2d 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f  .------..[List o
-0000a130: 6620 5052 7320 2f20 6973 7375 6573 2066  f PRs / issues f
-0000a140: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
-0000a150: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000a160: 636f 6d2f 646f 636b 6572 2f64 6f63 6b65  com/docker/docke
-0000a170: 722d 7079 2f69 7373 7565 733f 713d 6d69  r-py/issues?q=mi
-0000a180: 6c65 7374 6f6e 6525 3341 312e 3130 2e30  lestone%3A1.10.0
-0000a190: 2b69 7325 3341 636c 6f73 6564 290a 0a23  +is%3Aclosed)..#
-0000a1a0: 2323 2042 7567 6669 7865 730a 0a2a 2054  ## Bugfixes..* T
-0000a1b0: 6865 2064 6f63 6b65 722e 7574 696c 732e  he docker.utils.
-0000a1c0: 7479 7065 7320 6d6f 6475 6c65 2077 6173  types module was
-0000a1d0: 2072 656d 6f76 6564 2069 6e20 6661 766f   removed in favo
-0000a1e0: 7220 6f66 2064 6f63 6b65 722e 7479 7065  r of docker.type
-0000a1f0: 732c 2062 7574 2073 6f6d 650a 2020 6170  s, but some.  ap
-0000a200: 706c 6963 6174 696f 6e73 2069 6d70 6f72  plications impor
-0000a210: 7465 6420 6974 2065 7870 6c69 6369 746c  ted it explicitl
-0000a220: 792e 2049 7420 6861 7320 6265 656e 2072  y. It has been r
-0000a230: 652d 6164 6465 6420 7769 7468 2061 6e20  e-added with an 
-0000a240: 696d 706f 7274 0a20 2077 6172 6e69 6e67  import.  warning
-0000a250: 2061 6476 6973 696e 6720 746f 2075 7365   advising to use
-0000a260: 2074 6865 206e 6577 206d 6f64 756c 6520   the new module 
-0000a270: 7061 7468 2e0a 0a31 2e31 302e 300a 2d2d  path...1.10.0.--
-0000a280: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
-0000a290: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
-0000a2a0: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-0000a2b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000a2c0: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
-0000a2d0: 792f 6973 7375 6573 3f71 3d6d 696c 6573  y/issues?q=miles
-0000a2e0: 746f 6e65 2533 4131 2e31 302e 302b 6973  tone%3A1.10.0+is
-0000a2f0: 2533 4163 6c6f 7365 6429 0a0a 2323 2320  %3Aclosed)..### 
-0000a300: 4665 6174 7572 6573 0a0a 2a20 4164 6465  Features..* Adde
-0000a310: 6420 7377 6172 6d20 6d6f 6465 2061 6e64  d swarm mode and
-0000a320: 2073 6572 7669 6365 206d 616e 6167 656d   service managem
-0000a330: 656e 7420 6d65 7468 6f64 732e 2053 6565  ent methods. See
-0000a340: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-0000a350: 6f6e 2066 6f72 0a20 2064 6574 6169 6c73  on for.  details
-0000a360: 2e0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
-0000a370: 7420 666f 7220 4950 7636 2044 6f63 6b65  t for IPv6 Docke
-0000a380: 7220 686f 7374 2061 6464 7265 7373 6573  r host addresses
-0000a390: 2069 6e20 7468 6520 6043 6c69 656e 7460   in the `Client`
-0000a3a0: 2063 6f6e 7374 7275 6374 6f72 2e0a 2a20   constructor..* 
-0000a3b0: 4164 6465 6420 2872 6561 642d 6f6e 6c79  Added (read-only
-0000a3c0: 2920 7375 7070 6f72 7420 666f 7220 7468  ) support for th
-0000a3d0: 6520 446f 636b 6572 2063 7265 6465 6e74  e Docker credent
-0000a3e0: 6961 6c73 2073 746f 7265 2e0a 2a20 4164  ials store..* Ad
-0000a3f0: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
-0000a400: 6375 7374 6f6d 2060 6175 7468 5f63 6f6e  custom `auth_con
-0000a410: 6669 6760 2069 6e20 6043 6c69 656e 742e  fig` in `Client.
-0000a420: 7075 7368 602e 0a2a 2041 6464 6564 2073  push`..* Added s
-0000a430: 7570 706f 7274 2066 6f72 2060 6c61 6265  upport for `labe
-0000a440: 6c73 6020 696e 2060 436c 6965 6e74 2e63  ls` in `Client.c
-0000a450: 7265 6174 655f 766f 6c75 6d65 602e 0a2a  reate_volume`..*
-0000a460: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-0000a470: 6f72 2060 6c61 6265 6c73 6020 616e 6420  or `labels` and 
-0000a480: 6065 6e61 626c 655f 6970 7636 6020 696e  `enable_ipv6` in
-0000a490: 2060 436c 6965 6e74 2e63 7265 6174 655f   `Client.create_
-0000a4a0: 6e65 7477 6f72 6b60 2e0a 2a20 4164 6465  network`..* Adde
-0000a4b0: 6420 7375 7070 6f72 7420 666f 7220 6066  d support for `f
-0000a4c0: 6f72 6365 6020 7061 7261 6d20 696e 0a20  orce` param in. 
-0000a4d0: 2060 436c 6965 6e74 2e64 6973 636f 6e6e   `Client.disconn
-0000a4e0: 6563 745f 636f 6e74 6169 6e65 725f 6672  ect_container_fr
-0000a4f0: 6f6d 5f6e 6574 776f 726b 602e 0a2a 2041  om_network`..* A
-0000a500: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
-0000a510: 2060 7069 6473 5f6c 696d 6974 602c 2060   `pids_limit`, `
-0000a520: 7379 7363 746c 7360 2c20 6075 7365 726e  sysctls`, `usern
-0000a530: 735f 6d6f 6465 602c 2060 6370 7573 6574  s_mode`, `cpuset
-0000a540: 5f63 7075 7360 2c0a 2020 6063 7075 5f73  _cpus`,.  `cpu_s
-0000a550: 6861 7265 7360 2c20 606d 656d 5f72 6573  hares`, `mem_res
-0000a560: 6572 7661 7469 6f6e 6020 616e 6420 606b  ervation` and `k
-0000a570: 6572 6e65 6c5f 6d65 6d6f 7279 6020 7061  ernel_memory` pa
-0000a580: 7261 6d65 7465 7273 2069 6e0a 2020 6043  rameters in.  `C
-0000a590: 6c69 656e 742e 6372 6561 7465 5f68 6f73  lient.create_hos
-0000a5a0: 745f 636f 6e66 6967 602e 0a2a 2041 6464  t_config`..* Add
-0000a5b0: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
-0000a5c0: 6c69 6e6b 5f6c 6f63 616c 5f69 7073 6020  link_local_ips` 
-0000a5d0: 696e 2060 6372 6561 7465 5f65 6e64 706f  in `create_endpo
-0000a5e0: 696e 745f 636f 6e66 6967 602e 0a2a 2041  int_config`..* A
-0000a5f0: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
-0000a600: 2061 2060 6368 616e 6765 7360 2070 6172   a `changes` par
-0000a610: 616d 6574 6572 2069 6e20 6043 6c69 656e  ameter in `Clien
-0000a620: 742e 696d 706f 7274 5f69 6d61 6765 602e  t.import_image`.
-0000a630: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-0000a640: 2066 6f72 2061 2060 7665 7273 696f 6e60   for a `version`
-0000a650: 2070 6172 616d 6574 6572 2069 6e20 6043   parameter in `C
-0000a660: 6c69 656e 742e 6672 6f6d 5f65 6e76 602e  lient.from_env`.
-0000a670: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-0000a680: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-0000a690: 6572 6520 6043 6c69 656e 742e 6275 696c  ere `Client.buil
-0000a6a0: 6460 2077 6f75 6c64 2063 7261 7368 2069  d` would crash i
-0000a6b0: 6620 7468 6520 6063 6f6e 6669 672e 6a73  f the `config.js
-0000a6c0: 6f6e 6020 6669 6c65 0a20 2063 6f6e 7461  on` file.  conta
-0000a6d0: 696e 6564 2061 2060 4874 7470 4865 6164  ined a `HttpHead
-0000a6e0: 6572 7360 2065 6e74 7279 2e0a 2a20 4669  ers` entry..* Fi
-0000a6f0: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
-0000a700: 7061 7373 696e 6720 6064 6563 6f64 653d  passing `decode=
-0000a710: 5472 7565 6020 696e 2073 6f6d 6520 7374  True` in some st
-0000a720: 7265 616d 696e 6720 6d65 7468 6f64 7320  reaming methods 
-0000a730: 776f 756c 640a 2020 6372 6173 6820 7768  would.  crash wh
-0000a740: 656e 2074 6865 2064 6165 6d6f 6e27 7320  en the daemon's 
-0000a750: 7265 7370 6f6e 7365 2068 6164 2061 6e20  response had an 
-0000a760: 756e 6578 7065 6374 6564 2066 6f72 6d61  unexpected forma
-0000a770: 742e 0a2a 2046 6978 6564 2061 2062 7567  t..* Fixed a bug
-0000a780: 2077 6865 7265 2060 656e 7669 726f 6e6d   where `environm
-0000a790: 656e 7460 2076 616c 7565 7320 7769 7468  ent` values with
-0000a7a0: 2075 6e69 636f 6465 2063 6861 7261 6374   unicode charact
-0000a7b0: 6572 7320 7765 7265 6e27 740a 2020 6861  ers weren't.  ha
-0000a7c0: 6e64 6c65 6420 7072 6f70 6572 6c79 2069  ndled properly i
-0000a7d0: 6e20 6063 7265 6174 655f 636f 6e74 6169  n `create_contai
-0000a7e0: 6e65 7260 2e0a 2a20 4669 7865 6420 6120  ner`..* Fixed a 
-0000a7f0: 6275 6720 7768 6572 6520 7573 696e 6720  bug where using 
-0000a800: 7468 6520 606e 7069 7065 6020 7072 6f74  the `npipe` prot
-0000a810: 6f63 6f6c 2077 6f75 6c64 2073 6f6d 6574  ocol would somet
-0000a820: 696d 6573 2062 7265 616b 2077 6974 680a  imes break with.
-0000a830: 2020 6056 616c 7565 4572 726f 723a 2062    `ValueError: b
-0000a840: 7566 6665 7220 7369 7a65 206d 7573 7420  uffer size must 
-0000a850: 6265 2073 7472 6963 746c 7920 706f 7369  be strictly posi
-0000a860: 7469 7665 602e 0a0a 2323 2320 4d69 7363  tive`...### Misc
-0000a870: 656c 6c61 6e65 6f75 730a 0a2a 2046 6978  ellaneous..* Fix
-0000a880: 6564 2061 6e20 6973 7375 6520 7768 6572  ed an issue wher
-0000a890: 6520 5552 4c2d 7175 6f74 696e 6720 696e  e URL-quoting in
-0000a8a0: 2064 6f63 6b65 722d 7079 2077 6173 2069   docker-py was i
-0000a8b0: 6e63 6f6e 7369 7374 656e 7420 7769 7468  nconsistent with
-0000a8c0: 2074 6865 0a20 2071 756f 7469 6e67 2064   the.  quoting d
-0000a8d0: 6f6e 6520 6279 2074 6865 2044 6f63 6b65  one by the Docke
-0000a8e0: 7220 434c 4920 636c 6965 6e74 2e0a 2a20  r CLI client..* 
-0000a8f0: 5468 6520 636c 6965 6e74 206e 6f77 2073  The client now s
-0000a900: 656e 6473 2054 4350 2075 7067 7261 6465  ends TCP upgrade
-0000a910: 2068 6561 6465 7273 2074 6f20 6869 6e74   headers to hint
-0000a920: 2070 6f74 656e 7469 616c 2070 726f 7869   potential proxi
-0000a930: 6573 2061 626f 7574 0a20 2063 6f6e 6e65  es about.  conne
-0000a940: 6374 696f 6e20 6869 6a61 636b 696e 672e  ction hijacking.
-0000a950: 0a2a 2054 6865 2063 6c69 656e 7420 6e6f  .* The client no
-0000a960: 7720 6465 6661 756c 7473 2074 6f20 7573  w defaults to us
-0000a970: 696e 6720 7468 6520 606e 7069 7065 6020  ing the `npipe` 
-0000a980: 7072 6f74 6f63 6f6c 206f 6e20 5769 6e64  protocol on Wind
-0000a990: 6f77 732e 0a0a 0a31 2e39 2e30 0a2d 2d2d  ows....1.9.0.---
-0000a9a0: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
-0000a9b0: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
-0000a9c0: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-0000a9d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-0000a9e0: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
-0000a9f0: 6973 7375 6573 3f71 3d6d 696c 6573 746f  issues?q=milesto
-0000aa00: 6e65 2533 4131 2e39 2e30 2b69 7325 3341  ne%3A1.9.0+is%3A
-0000aa10: 636c 6f73 6564 290a 0a23 2323 2046 6561  closed)..### Fea
-0000aa20: 7475 7265 730a 0a2a 2041 6464 6564 202a  tures..* Added *
-0000aa30: 2a65 7870 6572 696d 656e 7461 6c2a 2a20  *experimental** 
-0000aa40: 7375 7070 6f72 7420 666f 7220 5769 6e64  support for Wind
-0000aa50: 6f77 7320 6e61 6d65 6420 7069 7065 7320  ows named pipes 
-0000aa60: 2860 6e70 6970 653a 2f2f 6020 7072 6f74  (`npipe://` prot
-0000aa70: 6f63 6f6c 292e 0a2a 2041 6464 6564 2073  ocol)..* Added s
-0000aa80: 7570 706f 7274 2066 6f72 2042 6c6f 636b  upport for Block
-0000aa90: 2049 4f20 636f 6e73 7472 6169 6e74 7320   IO constraints 
-0000aaa0: 696e 2060 436c 6965 6e74 2e63 7265 6174  in `Client.creat
-0000aab0: 655f 686f 7374 5f63 6f6e 6669 6760 2e20  e_host_config`. 
-0000aac0: 5468 6973 0a20 2069 6e63 6c75 6465 7320  This.  includes 
-0000aad0: 7061 7261 6d65 7465 7273 2060 626c 6b69  parameters `blki
-0000aae0: 6f5f 7765 6967 6874 602c 2060 626c 6b69  o_weight`, `blki
-0000aaf0: 6f5f 7765 6967 6874 5f64 6576 6963 6560  o_weight_device`
-0000ab00: 2c20 6064 6576 6963 655f 7265 6164 5f62  , `device_read_b
-0000ab10: 7073 602c 0a20 2060 6465 7669 6365 5f77  ps`,.  `device_w
-0000ab20: 7269 7465 5f62 7073 602c 2060 6465 7669  rite_bps`, `devi
-0000ab30: 6365 5f72 6561 645f 696f 7073 6020 616e  ce_read_iops` an
-0000ab40: 6420 6064 6576 6963 655f 7772 6974 655f  d `device_write_
-0000ab50: 696f 7073 602e 0a2a 2041 6464 6564 2073  iops`..* Added s
-0000ab60: 7570 706f 7274 2066 6f72 2074 6865 2060  upport for the `
-0000ab70: 696e 7465 726e 616c 6020 7061 7261 6d20  internal` param 
-0000ab80: 696e 2060 436c 6965 6e74 2e63 7265 6174  in `Client.creat
-0000ab90: 655f 6e65 7477 6f72 6b60 2e0a 2a20 4164  e_network`..* Ad
-0000aba0: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
-0000abb0: 6069 7076 345f 6164 6472 6573 7360 2061  `ipv4_address` a
-0000abc0: 6e64 2060 6970 7636 5f61 6464 7265 7373  nd `ipv6_address
-0000abd0: 6020 696e 2075 7469 6c73 2066 756e 6374  ` in utils funct
-0000abe0: 696f 6e0a 2020 6063 7265 6174 655f 656e  ion.  `create_en
-0000abf0: 6470 6f69 6e74 5f63 6f6e 6669 6760 2e0a  dpoint_config`..
-0000ac00: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-0000ac10: 666f 7220 6375 7374 6f6d 2075 7365 7220  for custom user 
-0000ac20: 6167 656e 7420 7365 7474 696e 6720 696e  agent setting in
-0000ac30: 2074 6865 2060 436c 6965 6e74 6020 636f   the `Client` co
-0000ac40: 6e73 7472 7563 746f 722e 0a20 2042 7920  nstructor..  By 
-0000ac50: 6465 6661 756c 742c 2064 6f63 6b65 722d  default, docker-
-0000ac60: 7079 206e 6f77 2061 6c73 6f20 6465 636c  py now also decl
-0000ac70: 6172 6573 2069 7473 656c 6620 696e 2074  ares itself in t
-0000ac80: 6865 2060 5573 6572 2d41 6765 6e74 6020  he `User-Agent` 
-0000ac90: 6865 6164 6572 2e0a 0a23 2323 2042 7567  header...### Bug
-0000aca0: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
-0000acb0: 6e20 6973 7375 6520 7768 6572 6520 7468  n issue where th
-0000acc0: 6520 4854 5450 2074 696d 656f 7574 206f  e HTTP timeout o
-0000acd0: 6e20 7374 7265 616d 696e 6720 7265 7370  n streaming resp
-0000ace0: 6f6e 7365 7320 776f 756c 6420 736f 6d65  onses would some
-0000acf0: 7469 6d65 730a 2020 6265 2073 6574 2069  times.  be set i
-0000ad00: 6e63 6f72 7265 6374 6c79 2e0a 2a20 4669  ncorrectly..* Fi
-0000ad10: 7865 6420 616e 2069 7373 7565 2077 6865  xed an issue whe
-0000ad20: 7265 2065 7870 6c69 6369 7420 7265 6c61  re explicit rela
-0000ad30: 7469 7665 2070 6174 6873 2069 6e20 602e  tive paths in `.
-0000ad40: 646f 636b 6572 6967 6e6f 7265 6020 6669  dockerignore` fi
-0000ad50: 6c65 7320 7765 7265 0a20 206e 6f74 2062  les were.  not b
-0000ad60: 6569 6e67 2072 6563 6f67 6e69 7a65 642e  eing recognized.
-0000ad70: 0a0a 312e 382e 310a 2d2d 2d2d 2d0a 0a5b  ..1.8.1.-----..[
-0000ad80: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
-0000ad90: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
-0000ada0: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-0000adb0: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
-0000adc0: 2f64 6f63 6b65 722d 7079 2f69 7373 7565  /docker-py/issue
-0000add0: 733f 713d 6d69 6c65 7374 6f6e 6525 3341  s?q=milestone%3A
-0000ade0: 312e 382e 312b 6973 2533 4163 6c6f 7365  1.8.1+is%3Aclose
-0000adf0: 6429 0a0a 2323 2320 4275 6766 6978 6573  d)..### Bugfixes
-0000ae00: 0a0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
-0000ae10: 7768 6572 6520 6361 6c6c 696e 6720 606c  where calling `l
-0000ae20: 6f67 696e 2829 6020 6167 6169 6e73 7420  ogin()` against 
-0000ae30: 7468 6520 6465 6661 756c 7420 7265 6769  the default regi
-0000ae40: 7374 7279 2077 6f75 6c64 2066 6169 6c0a  stry would fail.
-0000ae50: 2020 7769 7468 2074 6865 2031 2e31 302e    with the 1.10.
-0000ae60: 7820 656e 6769 6e65 0a2a 2046 6978 6564  x engine.* Fixed
-0000ae70: 2061 2062 7567 2077 6865 7265 2076 616c   a bug where val
-0000ae80: 7565 7320 696e 2065 6e76 6972 6f6e 6d65  ues in environme
-0000ae90: 6e74 2066 696c 6573 2077 6f75 6c64 2062  nt files would b
-0000aea0: 6520 7061 7273 6564 2069 6e63 6f72 7265  e parsed incorre
-0000aeb0: 6374 6c79 2069 660a 2020 7468 6579 2063  ctly if.  they c
-0000aec0: 6f6e 7461 696e 6564 2061 6e20 6571 7561  ontained an equa
-0000aed0: 6c20 7369 676e 2e0a 2a20 5377 6974 6368  l sign..* Switch
-0000aee0: 6564 2074 6f20 6120 6265 7474 6572 2073  ed to a better s
-0000aef0: 7570 706f 7274 6564 2062 6163 6b70 6f72  upported backpor
-0000af00: 7420 6f66 2074 6865 2060 6d61 7463 685f  t of the `match_
-0000af10: 686f 7374 6e61 6d65 6020 6675 6e63 7469  hostname` functi
-0000af20: 6f6e 2c0a 2020 6669 7869 6e67 2064 6570  on,.  fixing dep
-0000af30: 656e 6465 6e63 7920 6973 7375 6573 2069  endency issues i
-0000af40: 6e20 736f 6d65 2065 6e76 6972 6f6e 6d65  n some environme
-0000af50: 6e74 732e 0a0a 0a31 2e38 2e30 0a2d 2d2d  nts....1.8.0.---
-0000af60: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
-0000af70: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
-0000af80: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-0000af90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-0000afa0: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
-0000afb0: 6973 7375 6573 3f71 3d6d 696c 6573 746f  issues?q=milesto
-0000afc0: 6e65 2533 4131 2e38 2e30 2b69 7325 3341  ne%3A1.8.0+is%3A
-0000afd0: 636c 6f73 6564 290a 0a23 2323 2046 6561  closed)..### Fea
-0000afe0: 7475 7265 730a 0a2a 2041 6464 6564 2060  tures..* Added `
-0000aff0: 436c 6965 6e74 2e75 7064 6174 655f 636f  Client.update_co
-0000b000: 6e74 6169 6e65 7260 206d 6574 686f 6420  ntainer` method 
-0000b010: 2855 7064 6174 6520 7265 736f 7572 6365  (Update resource
-0000b020: 2063 6f6e 6669 6773 206f 6620 610a 2020   configs of a.  
-0000b030: 636f 6e74 6169 6e65 7229 0a2a 2041 6464  container).* Add
-0000b040: 6564 2073 7570 706f 7274 2066 6f72 2067  ed support for g
-0000b050: 7a69 7070 6564 2063 6f6e 7465 7874 2069  zipped context i
-0000b060: 6e20 6043 6c69 656e 742e 6275 696c 6460  n `Client.build`
-0000b070: 0a2a 2041 6464 6564 2061 6269 6c69 7479  .* Added ability
-0000b080: 2074 6f20 7370 6563 6966 7920 4950 2061   to specify IP a
-0000b090: 6464 7265 7373 2077 6865 6e20 636f 6e6e  ddress when conn
-0000b0a0: 6563 7469 6e67 2061 2063 6f6e 7461 696e  ecting a contain
-0000b0b0: 6572 2074 6f20 610a 2020 6e65 7477 6f72  er to a.  networ
-0000b0c0: 6b0a 2a20 4164 6465 6420 6074 6d70 6673  k.* Added `tmpfs
-0000b0d0: 6020 7375 7070 6f72 7420 746f 2060 436c  ` support to `Cl
-0000b0e0: 6965 6e74 2e63 7265 6174 655f 686f 7374  ient.create_host
-0000b0f0: 5f63 6f6e 6669 6760 0a2a 2041 6464 6564  _config`.* Added
-0000b100: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
-0000b110: 2060 6368 616e 6765 7360 2070 6172 616d   `changes` param
-0000b120: 2069 6e20 6043 6c69 656e 742e 636f 6d6d   in `Client.comm
-0000b130: 6974 600a 2a20 4164 6465 6420 7375 7070  it`.* Added supp
-0000b140: 6f72 7420 666f 7220 7468 6520 6066 6f6c  ort for the `fol
-0000b150: 6c6f 7760 2070 6172 616d 2069 6e20 6043  low` param in `C
-0000b160: 6c69 656e 742e 6c6f 6773 600a 2a20 4164  lient.logs`.* Ad
-0000b170: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
-0000b180: 7468 6520 6063 6865 636b 5f64 7570 6c69  the `check_dupli
-0000b190: 6361 7465 6020 7061 7261 6d20 696e 2060  cate` param in `
-0000b1a0: 436c 6965 6e74 2e63 7265 6174 655f 6e65  Client.create_ne
-0000b1b0: 7477 6f72 6b60 0a2a 2041 6464 6564 2073  twork`.* Added s
-0000b1c0: 7570 706f 7274 2066 6f72 2074 6865 2060  upport for the `
-0000b1d0: 6465 636f 6465 6020 7061 7261 6d20 696e  decode` param in
-0000b1e0: 2060 436c 6965 6e74 2e70 7573 6860 2061   `Client.push` a
-0000b1f0: 6e64 2060 436c 6965 6e74 2e70 756c 6c60  nd `Client.pull`
-0000b200: 0a2a 2041 6464 6564 2060 646f 636b 6572  .* Added `docker
-0000b210: 2e66 726f 6d5f 656e 7660 2073 686f 7274  .from_env` short
-0000b220: 6375 7420 6675 6e63 7469 6f6e 2e20 496e  cut function. In
-0000b230: 7374 616e 7469 6174 6573 2061 2063 6c69  stantiates a cli
-0000b240: 656e 7420 7769 7468 0a20 2060 6b77 6172  ent with.  `kwar
-0000b250: 6773 5f66 726f 6d5f 656e 7660 0a2a 2060  gs_from_env`.* `
-0000b260: 6b77 6172 6773 5f66 726f 6d5f 656e 7660  kwargs_from_env`
-0000b270: 206e 6f77 2073 7570 706f 7274 7320 616e   now supports an
-0000b280: 206f 7074 696f 6e61 6c20 6065 6e76 6972   optional `envir
-0000b290: 6f6e 6d65 6e74 6020 7061 7261 6d65 7465  onment` paramete
-0000b2a0: 722e 0a20 2049 6620 7072 6573 656e 742c  r..  If present,
-0000b2b0: 2076 616c 7565 7320 7769 6c6c 2062 6520   values will be 
-0000b2c0: 6665 7463 6865 6420 6672 6f6d 2074 6869  fetched from thi
-0000b2d0: 7320 6469 6374 696f 6e61 7279 2069 6e73  s dictionary ins
-0000b2e0: 7465 6164 206f 660a 2020 606f 732e 656e  tead of.  `os.en
-0000b2f0: 7669 726f 6e60 0a0a 0a23 2323 2042 7567  viron`...### Bug
-0000b300: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
-0000b310: 2062 7567 2077 6865 7265 2054 4c53 2076   bug where TLS v
-0000b320: 6572 6966 6963 6174 696f 6e20 776f 756c  erification woul
-0000b330: 6420 6661 696c 2077 6865 6e20 7573 696e  d fail when usin
-0000b340: 6720 4950 2061 6464 7265 7373 6573 0a20  g IP addresses. 
-0000b350: 2069 6e20 7468 6520 6365 7274 6966 6963   in the certific
-0000b360: 6174 6527 7320 6073 7562 6a65 6374 416c  ate's `subjectAl
-0000b370: 744e 616d 6560 2066 6965 6c64 730a 2a20  tName` fields.* 
-0000b380: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
-0000b390: 6865 7265 2074 6865 2064 6566 6175 6c74  here the default
-0000b3a0: 2054 4c53 2076 6572 7369 6f6e 2069 6e20   TLS version in 
-0000b3b0: 544c 5343 6f6e 6669 6720 776f 756c 640a  TLSConfig would.
-0000b3c0: 2020 6272 6561 6b20 696e 2073 6f6d 6520    break in some 
-0000b3d0: 656e 7669 726f 6e6d 656e 7473 2e20 6064  environments. `d
-0000b3e0: 6f63 6b65 722d 7079 6020 6e6f 7720 7573  ocker-py` now us
-0000b3f0: 6573 2054 4c53 7631 2062 7920 6465 6661  es TLSv1 by defa
-0000b400: 756c 740a 2020 5468 6973 2073 6574 7469  ult.  This setti
-0000b410: 6e67 2063 616e 2062 6520 6f76 6572 7269  ng can be overri
-0000b420: 6464 656e 2075 7369 6e67 2074 6865 2060  dden using the `
-0000b430: 7373 6c5f 7665 7273 696f 6e60 2070 6172  ssl_version` par
-0000b440: 616d 2069 6e0a 2020 606b 7761 7267 735f  am in.  `kwargs_
-0000b450: 6672 6f6d 5f65 6e76 6020 6f72 2074 6865  from_env` or the
-0000b460: 2060 544c 5343 6f6e 6669 6760 2063 6f6e   `TLSConfig` con
-0000b470: 7374 7275 6374 6f72 0a2a 2046 6978 6564  structor.* Fixed
-0000b480: 2061 2062 7567 2077 6865 7265 2060 7463   a bug where `tc
-0000b490: 7060 2068 6f73 7473 2077 6f75 6c64 2066  p` hosts would f
-0000b4a0: 6169 6c20 746f 2063 6f6e 6e65 6374 2074  ail to connect t
-0000b4b0: 6f20 544c 532d 656e 6162 6c65 640a 2020  o TLS-enabled.  
-0000b4c0: 656e 6470 6f69 6e74 730a 2a20 4669 7865  endpoints.* Fixe
-0000b4d0: 6420 6120 6275 6720 7768 6572 6520 6c6f  d a bug where lo
-0000b4e0: 6164 696e 6720 6120 7661 6c69 6420 646f  ading a valid do
-0000b4f0: 636b 6572 2063 6f6e 6669 6775 7261 7469  cker configurati
-0000b500: 6f6e 2066 696c 6520 776f 756c 6420 6661  on file would fa
-0000b510: 696c 0a2a 2046 6978 6564 2061 2062 7567  il.* Fixed a bug
-0000b520: 2077 6865 7265 2073 6f6d 6520 656e 7669   where some envi
-0000b530: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-0000b540: 7320 7370 6563 6966 6965 6420 7468 726f  s specified thro
-0000b550: 7567 680a 2020 6063 7265 6174 655f 636f  ugh.  `create_co
-0000b560: 6e74 6169 6e65 7260 2077 6f75 6c64 2062  ntainer` would b
-0000b570: 6520 696d 7072 6f70 6572 6c79 2066 6f72  e improperly for
-0000b580: 6d61 7474 6564 0a2a 2046 6978 6564 2061  matted.* Fixed a
-0000b590: 2062 7567 2077 6865 7265 2075 7369 6e67   bug where using
-0000b5a0: 2074 6865 2075 6e69 7820 736f 636b 6574   the unix socket
-0000b5b0: 2063 6f6e 6e65 6374 696f 6e20 776f 756c   connection woul
-0000b5c0: 6420 7261 6973 650a 2020 616e 2065 7272  d raise.  an err
-0000b5d0: 6f72 2069 6e20 736f 6d65 2065 6467 652d  or in some edge-
-0000b5e0: 6361 7365 2073 6974 7561 7469 6f6e 730a  case situations.
-0000b5f0: 0a23 2323 204d 6973 6365 6c6c 616e 656f  .### Miscellaneo
-0000b600: 7573 0a0a 2a20 4465 6661 756c 7420 4150  us..* Default AP
-0000b610: 4920 7665 7273 696f 6e20 6973 206e 6f77  I version is now
-0000b620: 2031 2e32 3220 2869 6e74 726f 6475 6365   1.22 (introduce
-0000b630: 6420 696e 2044 6f63 6b65 7220 312e 3130  d in Docker 1.10
-0000b640: 2e30 290a 0a0a 312e 372e 320a 2d2d 2d2d  .0)...1.7.2.----
-0000b650: 2d0a 0a5b 4c69 7374 206f 6620 5052 7320  -..[List of PRs 
-0000b660: 2f20 6973 7375 6573 2066 6f72 2074 6869  / issues for thi
-0000b670: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
-0000b680: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-0000b690: 636b 6572 2f64 6f63 6b65 722d 7079 2f69  cker/docker-py/i
-0000b6a0: 7373 7565 733f 713d 6d69 6c65 7374 6f6e  ssues?q=mileston
-0000b6b0: 6525 3341 312e 372e 322b 6973 2533 4163  e%3A1.7.2+is%3Ac
-0000b6c0: 6c6f 7365 6429 0a0a 2323 2320 4275 6766  losed)..### Bugf
-0000b6d0: 6978 6573 0a0a 2a20 4669 7865 6420 6120  ixes..* Fixed a 
-0000b6e0: 6275 6720 7768 6572 6520 544c 5320 7665  bug where TLS ve
-0000b6f0: 7269 6669 6361 7469 6f6e 2077 6173 2069  rification was i
-0000b700: 6d70 726f 7065 726c 7920 6578 6563 7574  mproperly execut
-0000b710: 6564 2077 6865 6e20 7072 6f76 6964 696e  ed when providin
-0000b720: 670a 2020 6120 6375 7374 6f6d 2043 4120  g.  a custom CA 
-0000b730: 6365 7274 6966 6963 6174 652e 0a0a 312e  certificate...1.
-0000b740: 372e 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374  7.1.-----..[List
-0000b750: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
-0000b760: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-0000b770: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-0000b780: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
-0000b790: 6b65 722d 7079 2f69 7373 7565 733f 713d  ker-py/issues?q=
-0000b7a0: 6d69 6c65 7374 6f6e 6525 3341 312e 372e  milestone%3A1.7.
-0000b7b0: 312b 6973 2533 4163 6c6f 7365 6429 0a0a  1+is%3Aclosed)..
-0000b7c0: 2323 2320 4665 6174 7572 6573 0a0a 2a20  ### Features..* 
-0000b7d0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-0000b7e0: 7220 6073 686d 5f73 697a 6560 2069 6e20  r `shm_size` in 
-0000b7f0: 6043 6c69 656e 742e 6372 6561 7465 5f68  `Client.create_h
-0000b800: 6f73 745f 636f 6e66 6967 600a 0a23 2323  ost_config`..###
-0000b810: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
-0000b820: 6564 2061 2062 7567 2077 6865 7265 2044  ed a bug where D
-0000b830: 6f63 6b65 7266 696c 6520 776f 756c 6420  ockerfile would 
-0000b840: 736f 6d65 7469 6d65 7320 6265 2065 7863  sometimes be exc
-0000b850: 6c75 6465 6420 6672 6f6d 2074 6865 2062  luded from the b
-0000b860: 7569 6c64 0a20 2063 6f6e 7465 7874 2e0a  uild.  context..
-0000b870: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-0000b880: 6572 6520 6120 646f 636b 6572 2063 6f6e  ere a docker con
-0000b890: 6669 6720 6669 6c65 2063 6f6e 7461 696e  fig file contain
-0000b8a0: 696e 6720 756e 6b6e 6f77 6e20 6b65 7973  ing unknown keys
-0000b8b0: 2077 6f75 6c64 2072 6169 7365 0a20 2061   would raise.  a
-0000b8c0: 6e20 6578 6365 7074 696f 6e2e 0a2a 2046  n exception..* F
-0000b8d0: 6978 6564 2061 6e20 6973 7375 6520 7769  ixed an issue wi
-0000b8e0: 7468 2053 534c 2063 6f6e 6e65 6374 696f  th SSL connectio
-0000b8f0: 6e73 2062 6568 6176 696e 6720 696d 7072  ns behaving impr
-0000b900: 6f70 6572 6c79 2077 6865 6e20 7079 4f70  operly when pyOp
-0000b910: 656e 5353 4c0a 2020 7761 7320 696e 7374  enSSL.  was inst
-0000b920: 616c 6c65 6420 696e 2074 6865 2073 616d  alled in the sam
-0000b930: 6520 656e 7669 726f 6e6d 656e 742e 0a2a  e environment..*
-0000b940: 2053 6576 6572 616c 2054 4c53 2063 6f6e   Several TLS con
-0000b950: 6669 6775 7261 7469 6f6e 2069 6d70 726f  figuration impro
-0000b960: 7665 6d65 6e74 730a 0a0a 312e 372e 300a  vements...1.7.0.
-0000b970: 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f 6620  -----..[List of 
-0000b980: 5052 7320 2f20 6973 7375 6573 2066 6f72  PRs / issues for
-0000b990: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
-0000b9a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000b9b0: 6d2f 646f 636b 6572 2f64 6f63 6b65 722d  m/docker/docker-
-0000b9c0: 7079 2f69 7373 7565 733f 713d 6d69 6c65  py/issues?q=mile
-0000b9d0: 7374 6f6e 6525 3341 312e 372e 302b 6973  stone%3A1.7.0+is
-0000b9e0: 2533 4163 6c6f 7365 6429 0a0a 2323 2320  %3Aclosed)..### 
-0000b9f0: 4665 6174 7572 6573 0a0a 2a20 4164 6465  Features..* Adde
-0000ba00: 6420 7375 7070 6f72 7420 666f 7220 6375  d support for cu
-0000ba10: 736f 6d20 4950 414d 2063 6f6e 6669 6775  som IPAM configu
-0000ba20: 7261 7469 6f6e 2069 6e20 6043 6c69 656e  ration in `Clien
-0000ba30: 742e 6372 6561 7465 5f6e 6574 776f 726b  t.create_network
-0000ba40: 600a 2a20 4164 6465 6420 696e 7075 7420  `.* Added input 
-0000ba50: 7375 7070 6f72 7420 746f 2060 436c 6965  support to `Clie
-0000ba60: 6e74 2e65 7865 635f 6372 6561 7465 600a  nt.exec_create`.
-0000ba70: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-0000ba80: 666f 7220 6073 746f 705f 7369 676e 616c  for `stop_signal
-0000ba90: 6020 696e 2060 436c 6965 6e74 2e63 7265  ` in `Client.cre
-0000baa0: 6174 655f 686f 7374 5f63 6f6e 6669 6760  ate_host_config`
-0000bab0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-0000bac0: 2066 6f72 2063 7573 746f 6d20 4854 5450   for custom HTTP
-0000bad0: 2068 6561 6465 7273 2069 6e20 446f 636b   headers in Dock
-0000bae0: 6572 2063 6f6e 6669 6720 6669 6c65 2e0a  er config file..
-0000baf0: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-0000bb00: 666f 7220 756e 7370 6563 6966 6965 6420  for unspecified 
-0000bb10: 7472 616e 7366 6572 2070 726f 746f 636f  transfer protoco
-0000bb20: 6c20 696e 2060 6261 7365 5f75 726c 6020  l in `base_url` 
-0000bb30: 7768 656e 2054 4c53 2069 730a 2020 656e  when TLS is.  en
-0000bb40: 6162 6c65 642e 0a0a 0a23 2323 2042 7567  abled....### Bug
-0000bb50: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
-0000bb60: 2062 7567 2077 6865 7265 2074 6865 2060   bug where the `
-0000bb70: 6669 6c74 6572 7360 2070 6172 616d 6574  filters` paramet
-0000bb80: 6572 2069 6e20 6043 6c69 656e 742e 766f  er in `Client.vo
-0000bb90: 6c75 6d65 7360 2077 6f75 6c64 206e 6f74  lumes` would not
-0000bba0: 2062 650a 2020 6170 706c 6965 6420 7072   be.  applied pr
-0000bbb0: 6f70 6572 6c79 2e0a 2a20 4669 7865 6420  operly..* Fixed 
-0000bbc0: 6120 6275 6720 7768 6572 6520 6d65 6d6f  a bug where memo
-0000bbd0: 7279 206c 696d 6974 7320 776f 756c 6420  ry limits would 
-0000bbe0: 7061 7273 6520 746f 2069 6e63 6f72 7265  parse to incorre
-0000bbf0: 6374 2076 616c 7565 732e 0a2a 2046 6978  ct values..* Fix
-0000bc00: 6564 2061 2062 7567 2077 6865 7265 2074  ed a bug where t
-0000bc10: 6865 2060 6465 7669 6365 7360 2070 6172  he `devices` par
-0000bc20: 616d 6574 6572 2069 6e20 6043 6c69 656e  ameter in `Clien
-0000bc30: 742e 6372 6561 7465 5f68 6f73 745f 636f  t.create_host_co
-0000bc40: 6e66 6967 600a 2020 776f 756c 6420 736f  nfig`.  would so
-0000bc50: 6d65 7469 6d65 7320 6265 206d 6973 696e  metimes be misin
-0000bc60: 7465 7270 7265 7465 642e 0a2a 2046 6978  terpreted..* Fix
-0000bc70: 6564 2061 2062 7567 2077 6865 7265 2069  ed a bug where i
-0000bc80: 6e73 7461 6e74 6961 7469 6e67 2061 2060  nstantiating a `
-0000bc90: 436c 6965 6e74 6020 6f62 6a65 6374 2077  Client` object w
-0000bca0: 6f75 6c64 2073 6f6d 6574 696d 6573 2063  ould sometimes c
-0000bcb0: 7261 7368 2069 660a 2020 6062 6173 655f  rash if.  `base_
-0000bcc0: 7572 6c60 2077 6173 2075 6e73 7065 6369  url` was unspeci
-0000bcd0: 6669 6564 2e0a 2a20 4669 7865 6420 6120  fied..* Fixed a 
-0000bce0: 6275 6720 7768 6572 6520 616e 2065 7272  bug where an err
-0000bcf0: 6f72 206d 6573 7361 6765 2072 656c 6174  or message relat
-0000bd00: 6564 2074 6f20 544c 5320 636f 6e66 6967  ed to TLS config
-0000bd10: 7572 6174 696f 6e20 776f 756c 6420 6c69  uration would li
-0000bd20: 6e6b 0a20 2074 6f20 6120 6e6f 6e2d 6578  nk.  to a non-ex
-0000bd30: 6973 7465 6e74 2028 6f75 7464 6174 6564  istent (outdated
-0000bd40: 2920 646f 6373 2070 6167 652e 0a0a 0a23  ) docs page....#
-0000bd50: 2323 204d 6973 6365 6c6c 616e 656f 7573  ## Miscellaneous
-0000bd60: 0a0a 2a20 5072 6f63 6573 7369 6e67 206f  ..* Processing o
-0000bd70: 6620 602e 646f 636b 6572 6967 6e6f 7265  f `.dockerignore
-0000bd80: 6020 6861 7320 6265 656e 206d 6164 6520  ` has been made 
-0000bd90: 7369 676e 6966 6963 616e 746c 7920 6661  significantly fa
-0000bda0: 7374 6572 2e0a 2a20 4472 6f70 7065 6420  ster..* Dropped 
-0000bdb0: 6578 706c 6963 6974 2073 7570 706f 7274  explicit support
-0000bdc0: 2066 6f72 2050 7974 686f 6e20 332e 320a   for Python 3.2.
-0000bdd0: 0a31 2e36 2e30 0a2d 2d2d 2d2d 0a0a 5b4c  .1.6.0.-----..[L
-0000bde0: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
-0000bdf0: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
-0000be00: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-0000be10: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
-0000be20: 646f 636b 6572 2d70 792f 6973 7375 6573  docker-py/issues
-0000be30: 3f71 3d6d 696c 6573 746f 6e65 2533 4131  ?q=milestone%3A1
-0000be40: 2e36 2e30 2b69 7325 3341 636c 6f73 6564  .6.0+is%3Aclosed
-0000be50: 290a 0a23 2323 2046 6561 7475 7265 730a  )..### Features.
-0000be60: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-0000be70: 2066 6f72 2074 6865 2060 7369 6e63 6560   for the `since`
-0000be80: 2070 6172 616d 2069 6e20 6043 6c69 656e   param in `Clien
-0000be90: 742e 6c6f 6773 6020 2869 6e74 726f 6475  t.logs` (introdu
-0000bea0: 6365 6420 696e 2041 5049 0a20 2076 6572  ced in API.  ver
-0000beb0: 7369 6f6e 2031 2e31 3929 0a2a 2041 6464  sion 1.19).* Add
-0000bec0: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
-0000bed0: 6865 2060 444f 434b 4552 5f43 4f4e 4649  he `DOCKER_CONFI
-0000bee0: 4760 2065 6e76 6972 6f6e 6d65 6e74 2076  G` environment v
-0000bef0: 6172 6961 626c 6520 7768 656e 206c 6f6f  ariable when loo
-0000bf00: 6b69 6e67 2075 700a 2020 6175 7468 2063  king up.  auth c
-0000bf10: 6f6e 6669 670a 2a20 4164 6465 6420 7375  onfig.* Added su
-0000bf20: 7070 6f72 7420 666f 7220 7468 6520 6073  pport for the `s
-0000bf30: 7472 6561 6d60 2070 6172 616d 2069 6e20  tream` param in 
-0000bf40: 6043 6c69 656e 742e 7374 6174 7360 2028  `Client.stats` (
-0000bf50: 7768 656e 2073 6574 2074 6f20 6046 616c  when set to `Fal
-0000bf60: 7365 602c 0a20 2061 6c6c 6f77 7320 7573  se`,.  allows us
-0000bf70: 6572 2074 6f20 7265 7472 6965 7665 2061  er to retrieve a
-0000bf80: 2073 696e 676c 6520 736e 6170 7368 6f74   single snapshot
-0000bf90: 2069 6e73 7465 6164 206f 6620 6120 636f   instead of a co
-0000bfa0: 6e73 7461 6e74 2064 6174 6120 7374 7265  nstant data stre
-0000bfb0: 616d 290a 2a20 4164 6465 6420 7375 7070  am).* Added supp
-0000bfc0: 6f72 7420 666f 7220 7468 6520 606d 656d  ort for the `mem
-0000bfd0: 5f73 7761 7070 696e 6573 7360 2c20 606f  _swappiness`, `o
-0000bfe0: 6f6d 5f6b 696c 6c5f 6469 7361 626c 6560  om_kill_disable`
-0000bff0: 2070 6172 616d 730a 2020 696e 2060 436c   params.  in `Cl
-0000c000: 6965 6e74 2e63 7265 6174 655f 686f 7374  ient.create_host
-0000c010: 5f63 6f6e 6669 6760 0a2a 2041 6464 6564  _config`.* Added
-0000c020: 2073 7570 706f 7274 2066 6f72 2062 7569   support for bui
-0000c030: 6c64 2061 7267 756d 656e 7473 2069 6e20  ld arguments in 
-0000c040: 6043 6c69 656e 742e 6275 696c 6460 2074  `Client.build` t
-0000c050: 6872 6f75 6768 2074 6865 2060 6275 696c  hrough the `buil
-0000c060: 6461 7267 7360 0a20 2070 6172 616d 2e0a  dargs`.  param..
-0000c070: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-0000c080: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-0000c090: 6572 6520 7374 7265 616d 696e 6720 6461  ere streaming da
-0000c0a0: 7461 206f 7665 7220 4854 5450 5320 776f  ta over HTTPS wo
-0000c0b0: 756c 6420 736f 6d65 7469 6d65 7320 6265  uld sometimes be
-0000c0c0: 6861 7665 0a20 2069 6e63 6f72 7265 6374  have.  incorrect
-0000c0d0: 6c79 2077 6974 6820 5079 7468 6f6e 2033  ly with Python 3
-0000c0e0: 2e78 0a2a 2046 6978 6564 2061 2062 7567  .x.* Fixed a bug
-0000c0f0: 2077 6865 7265 2063 6f6d 6d61 6e64 7320   where commands 
-0000c100: 636f 6e74 6169 6e69 6e67 2075 6e69 636f  containing unico
-0000c110: 6465 2063 6861 7261 6374 6572 7320 776f  de characters wo
-0000c120: 756c 6420 6265 2069 6e63 6f72 7265 6374  uld be incorrect
-0000c130: 6c79 0a20 2068 616e 646c 6564 2062 7920  ly.  handled by 
-0000c140: 6043 6c69 656e 742e 6372 6561 7465 5f63  `Client.create_c
-0000c150: 6f6e 7461 696e 6572 602e 0a2a 2046 6978  ontainer`..* Fix
-0000c160: 6564 2061 2062 7567 2077 6865 7265 2061  ed a bug where a
-0000c170: 7574 6820 636f 6e66 6967 2063 7265 6465  uth config crede
-0000c180: 6e74 6961 6c73 2063 6f6e 7461 696e 696e  ntials containin
-0000c190: 6720 756e 6963 6f64 6520 6368 6172 6163  g unicode charac
-0000c1a0: 7465 7273 2077 6f75 6c64 0a20 2063 6175  ters would.  cau
-0000c1b0: 7365 2066 6169 6c75 7265 7320 7768 656e  se failures when
-0000c1c0: 2070 7573 6869 6e67 202f 2070 756c 6c69   pushing / pulli
-0000c1d0: 6e67 2069 6d61 6765 732e 0a2a 2053 6574  ng images..* Set
-0000c1e0: 7469 6e67 2060 7461 696c 3d30 6020 696e  ting `tail=0` in
-0000c1f0: 2060 436c 6965 6e74 2e6c 6f67 7360 206e   `Client.logs` n
-0000c200: 6f20 6c6f 6e67 6572 2073 686f 7773 2070  o longer shows p
-0000c210: 6173 7420 6c6f 6773 2e0a 2a20 4669 7865  ast logs..* Fixe
-0000c220: 6420 6120 6275 6720 7768 6572 6520 6043  d a bug where `C
-0000c230: 6c69 656e 742e 7075 6c6c 6020 616e 6420  lient.pull` and 
-0000c240: 6043 6c69 656e 742e 7075 7368 6020 636f  `Client.push` co
-0000c250: 756c 646e 2774 2068 616e 646c 6520 696d  uldn't handle im
-0000c260: 6167 6520 6e61 6d65 730a 2020 636f 6e74  age names.  cont
-0000c270: 6169 6e69 6e67 2061 2064 6f74 2e0a 0a0a  aining a dot....
-0000c280: 2323 2320 4d69 7363 656c 6c61 6e65 6f75  ### Miscellaneou
-0000c290: 730a 0a2a 2044 6566 6175 6c74 2041 5049  s..* Default API
-0000c2a0: 2076 6572 7369 6f6e 2069 7320 6e6f 7720   version is now 
-0000c2b0: 312e 3231 2028 696e 7472 6f64 7563 6564  1.21 (introduced
-0000c2c0: 2069 6e20 446f 636b 6572 2031 2e39 2e30   in Docker 1.9.0
-0000c2d0: 290a 2a20 5365 7665 7261 6c20 7465 7374  ).* Several test
-0000c2e0: 2069 6d70 726f 7665 6d65 6e74 7320 616e   improvements an
-0000c2f0: 6420 636c 6561 6e75 7020 7468 6174 2073  d cleanup that s
-0000c300: 686f 756c 6420 6d61 6b65 2074 6865 2073  hould make the s
-0000c310: 7569 7465 2065 6173 6965 7220 746f 0a20  uite easier to. 
-0000c320: 2065 7870 616e 6420 616e 6420 6d61 696e   expand and main
-0000c330: 7461 696e 206d 6f76 696e 6720 666f 7277  tain moving forw
-0000c340: 6172 642e 0a0a 0a31 2e35 2e30 0a2d 2d2d  ard....1.5.0.---
-0000c350: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
-0000c360: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
-0000c370: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-0000c380: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-0000c390: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
-0000c3a0: 6973 7375 6573 3f71 3d6d 696c 6573 746f  issues?q=milesto
-0000c3b0: 6e65 2533 4131 2e35 2e30 2b69 7325 3341  ne%3A1.5.0+is%3A
-0000c3c0: 636c 6f73 6564 290a 0a23 2323 2046 6561  closed)..### Fea
-0000c3d0: 7475 7265 730a 0a2a 2041 6464 6564 2073  tures..* Added s
-0000c3e0: 7570 706f 7274 2066 6f72 2074 6865 206e  upport for the n
-0000c3f0: 6574 776f 726b 696e 6720 4150 4920 696e  etworking API in
-0000c400: 7472 6f64 7563 6564 2069 6e20 446f 636b  troduced in Dock
-0000c410: 6572 2031 2e39 2e30 0a20 2028 6043 6c69  er 1.9.0.  (`Cli
-0000c420: 656e 742e 6e65 7477 6f72 6b73 602c 2060  ent.networks`, `
-0000c430: 436c 6965 6e74 2e63 7265 6174 655f 6e65  Client.create_ne
-0000c440: 7477 6f72 6b60 2c20 6043 6c69 656e 742e  twork`, `Client.
-0000c450: 7265 6d6f 7665 5f6e 6574 776f 726b 602c  remove_network`,
-0000c460: 0a20 2060 436c 6965 6e74 2e69 6e73 7065  .  `Client.inspe
-0000c470: 6374 5f6e 6574 776f 726b 602c 2060 436c  ct_network`, `Cl
-0000c480: 6965 6e74 2e63 6f6e 6e65 6374 5f63 6f6e  ient.connect_con
-0000c490: 7461 696e 6572 5f74 6f5f 6e65 7477 6f72  tainer_to_networ
-0000c4a0: 6b60 2c0a 2020 6043 6c69 656e 742e 6469  k`,.  `Client.di
-0000c4b0: 7363 6f6e 6e65 6374 5f63 6f6e 7461 696e  sconnect_contain
-0000c4c0: 6572 5f66 726f 6d5f 6e65 7477 6f72 6b60  er_from_network`
-0000c4d0: 292e 0a2a 2041 6464 6564 2073 7570 706f  )..* Added suppo
-0000c4e0: 7274 2066 6f72 2074 6865 2076 6f6c 756d  rt for the volum
-0000c4f0: 6573 2041 5049 2069 6e74 726f 6475 6365  es API introduce
-0000c500: 6420 696e 2044 6f63 6b65 7220 312e 392e  d in Docker 1.9.
-0000c510: 300a 2020 2860 436c 6965 6e74 2e76 6f6c  0.  (`Client.vol
-0000c520: 756d 6573 602c 2060 436c 6965 6e74 2e63  umes`, `Client.c
-0000c530: 7265 6174 655f 766f 6c75 6d65 602c 2060  reate_volume`, `
-0000c540: 436c 6965 6e74 2e69 6e73 7065 6374 5f76  Client.inspect_v
-0000c550: 6f6c 756d 6560 2c0a 2020 6043 6c69 656e  olume`,.  `Clien
-0000c560: 742e 7265 6d6f 7665 5f76 6f6c 756d 6560  t.remove_volume`
-0000c570: 292e 0a2a 2041 6464 6564 2073 7570 706f  )..* Added suppo
-0000c580: 7274 2066 6f72 2074 6865 2060 6772 6f75  rt for the `grou
-0000c590: 705f 6164 6460 2070 6172 616d 6574 6572  p_add` parameter
-0000c5a0: 2069 6e20 6063 7265 6174 655f 686f 7374   in `create_host
-0000c5b0: 5f63 6f6e 6669 6760 2e0a 2a20 4164 6465  _config`..* Adde
-0000c5c0: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
-0000c5d0: 6520 4350 5520 4346 5320 2860 6370 755f  e CPU CFS (`cpu_
-0000c5e0: 7175 6f74 6160 2061 6e64 2060 6370 755f  quota` and `cpu_
-0000c5f0: 7065 7269 6f64 6029 2070 6172 616d 6574  period`) paramet
-0000c600: 6572 730a 2020 696e 2060 6372 6561 7465  ers.  in `create
-0000c610: 5f68 6f73 745f 636f 6e66 6967 602e 0a2a  _host_config`..*
-0000c620: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-0000c630: 6f72 2074 6865 2061 7263 6869 7665 2041  or the archive A
-0000c640: 5049 2065 6e64 706f 696e 7420 2860 436c  PI endpoint (`Cl
-0000c650: 6965 6e74 2e67 6574 5f61 7263 6869 7665  ient.get_archive
-0000c660: 602c 0a20 2060 436c 6965 6e74 2e70 7574  `,.  `Client.put
-0000c670: 5f61 7263 6869 7665 6029 2e0a 2a20 4164  _archive`)..* Ad
-0000c680: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
-0000c690: 6070 735f 6172 6773 6020 7061 7261 6d65  `ps_args` parame
-0000c6a0: 7465 7220 696e 2060 436c 6965 6e74 2e74  ter in `Client.t
-0000c6b0: 6f70 602e 0a0a 0a23 2323 2042 7567 6669  op`....### Bugfi
-0000c6c0: 7865 730a 0a2a 2046 6978 6564 2061 2062  xes..* Fixed a b
-0000c6d0: 7567 2077 6865 7265 2073 7065 6369 6679  ug where specify
-0000c6e0: 696e 6720 766f 6c75 6d65 2062 696e 6473  ing volume binds
-0000c6f0: 2077 6974 6820 756e 6963 6f64 6520 6368   with unicode ch
-0000c700: 6172 6163 7465 7273 2077 6f75 6c64 0a20  aracters would. 
-0000c710: 2066 6169 6c2e 0a2a 2046 6978 6564 2061   fail..* Fixed a
-0000c720: 2062 7567 2077 6865 7265 2070 726f 7669   bug where provi
-0000c730: 6469 6e67 2061 6e20 6578 706c 6963 6974  ding an explicit
-0000c740: 2070 726f 746f 636f 6c20 696e 2060 436c   protocol in `Cl
-0000c750: 6965 6e74 2e70 6f72 7460 2077 6f75 6c64  ient.port` would
-0000c760: 2066 6169 6c0a 2020 746f 2079 6965 6c64   fail.  to yield
-0000c770: 2074 6865 2065 7870 6563 7465 6420 7265   the expected re
-0000c780: 7375 6c74 2e0a 2a20 4669 7865 6420 6120  sult..* Fixed a 
-0000c790: 6275 6720 7768 6572 6520 7468 6520 7072  bug where the pr
-0000c7a0: 696f 7269 7479 2070 726f 746f 636f 6c20  iority protocol 
-0000c7b0: 7265 7475 726e 6564 2062 7920 6043 6c69  returned by `Cli
-0000c7c0: 656e 742e 706f 7274 6020 776f 756c 6420  ent.port` would 
-0000c7d0: 6265 2055 4450 0a20 2069 6e73 7465 6164  be UDP.  instead
-0000c7e0: 206f 6620 7468 6520 6578 7065 6374 6564   of the expected
-0000c7f0: 2054 4350 2e0a 0a23 2323 204d 6973 6365   TCP...### Misce
-0000c800: 6c6c 616e 656f 7573 0a0a 2a20 4272 6f6b  llaneous..* Brok
-0000c810: 6520 7570 2043 6c69 656e 7420 636f 6465  e up Client code
-0000c820: 2069 6e74 6f20 7365 7665 7261 6c20 6669   into several fi
-0000c830: 6c65 7320 746f 2066 6163 696c 6974 6174  les to facilitat
-0000c840: 6520 6d61 696e 7465 6e61 6e63 6520 616e  e maintenance an
-0000c850: 640a 2020 636f 6e74 7269 6275 7469 6f6e  d.  contribution
-0000c860: 2e0a 2a20 4164 6465 6420 636f 6e74 7269  ..* Added contri
-0000c870: 6275 7469 6e67 2067 7569 6465 6c69 6e65  buting guideline
-0000c880: 7320 746f 2074 6865 2072 6570 6f73 6974  s to the reposit
-0000c890: 6f72 792e 0a0a 312e 342e 300a 2d2d 2d2d  ory...1.4.0.----
-0000c8a0: 2d0a 0a5b 4c69 7374 206f 6620 5052 7320  -..[List of PRs 
-0000c8b0: 2f20 6973 7375 6573 2066 6f72 2074 6869  / issues for thi
-0000c8c0: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
-0000c8d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-0000c8e0: 636b 6572 2f64 6f63 6b65 722d 7079 2f69  cker/docker-py/i
-0000c8f0: 7373 7565 733f 713d 6d69 6c65 7374 6f6e  ssues?q=mileston
-0000c900: 6525 3341 312e 342e 302b 6973 2533 4163  e%3A1.4.0+is%3Ac
-0000c910: 6c6f 7365 6429 0a0a 2323 2320 4465 7072  losed)..### Depr
-0000c920: 6563 6174 696f 6e20 7761 726e 696e 670a  ecation warning.
-0000c930: 0a2a 2060 646f 636b 6572 2e75 7469 6c73  .* `docker.utils
-0000c940: 2e63 7265 6174 655f 686f 7374 5f63 6f6e  .create_host_con
-0000c950: 6669 6760 2069 7320 6465 7072 6563 6174  fig` is deprecat
-0000c960: 6564 2069 6e20 6661 766f 7220 6f66 0a20  ed in favor of. 
-0000c970: 2060 436c 6965 6e74 2e63 7265 6174 655f   `Client.create_
-0000c980: 686f 7374 5f63 6f6e 6669 6760 2e0a 0a23  host_config`...#
-0000c990: 2323 2046 6561 7475 7265 730a 0a2a 2041  ## Features..* A
-0000c9a0: 6464 6564 2060 7574 696c 732e 7061 7273  dded `utils.pars
-0000c9b0: 655f 656e 765f 6669 6c65 6020 746f 2073  e_env_file` to s
-0000c9c0: 7570 706f 7274 2065 6e76 2d66 696c 6573  upport env-files
-0000c9d0: 2e0a 2020 5365 6520 5b64 6f63 735d 2868  ..  See [docs](h
-0000c9e0: 7474 7073 3a2f 2f64 6f63 6b65 722d 7079  ttps://docker-py
-0000c9f0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-0000ca00: 656e 2f6c 6174 6573 742f 6170 692f 2363  en/latest/api/#c
-0000ca10: 7265 6174 655f 636f 6e74 6169 6e65 7229  reate_container)
-0000ca20: 0a20 2066 6f72 2075 7361 6765 2e0a 2a20  .  for usage..* 
-0000ca30: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-0000ca40: 7220 6172 6269 7472 6172 7920 6c6f 6720  r arbitrary log 
-0000ca50: 6472 6976 6572 730a 2a20 4164 6465 6420  drivers.* Added 
-0000ca60: 7375 7070 6f72 7420 666f 7220 5552 4c20  support for URL 
-0000ca70: 7061 7468 7320 696e 2074 6865 2064 6f63  paths in the doc
-0000ca80: 6b65 7220 686f 7374 2055 524c 2028 6062  ker host URL (`b
-0000ca90: 6173 655f 7572 6c60 290a 2a20 4472 6173  ase_url`).* Dras
-0000caa0: 7469 6361 6c6c 7920 696d 7072 6f76 6564  tically improved
-0000cab0: 2073 7570 706f 7274 2066 6f72 202e 646f   support for .do
-0000cac0: 636b 6572 6967 6e6f 7265 2073 796e 7461  ckerignore synta
-0000cad0: 780a 0a23 2323 2042 7567 6669 7865 730a  x..### Bugfixes.
-0000cae0: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-0000caf0: 6865 7265 2065 7865 635f 696e 7370 6563  here exec_inspec
-0000cb00: 7420 776f 756c 6420 616c 6c6f 7720 696e  t would allow in
-0000cb10: 766f 6361 7469 6f6e 2077 6865 6e20 7468  vocation when th
-0000cb20: 6520 4150 4920 7665 7273 696f 6e0a 2020  e API version.  
-0000cb30: 7761 7320 746f 6f20 6c6f 772e 0a2a 2046  was too low..* F
-0000cb40: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
-0000cb50: 2060 646f 636b 6572 2e75 7469 6c73 2e70   `docker.utils.p
-0000cb60: 6f72 7473 2e73 706c 6974 5f70 6f72 7460  orts.split_port`
-0000cb70: 2077 6f75 6c64 2062 7265 616b 2069 6620   would break if 
-0000cb80: 616e 206f 7065 6e0a 2020 7261 6e67 6520  an open.  range 
-0000cb90: 7761 7320 7072 6f76 6964 6564 2e0a 2a20  was provided..* 
-0000cba0: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
-0000cbb0: 6520 696e 7661 6c69 6420 696d 6167 6520  e invalid image 
-0000cbc0: 4944 7320 2f20 636f 6e74 6169 6e65 7220  IDs / container 
-0000cbd0: 4944 7320 636f 756c 6420 6265 2070 726f  IDs could be pro
-0000cbe0: 7669 6465 6420 746f 0a20 2062 7970 6173  vided to.  bypas
-0000cbf0: 7320 6f72 2072 6572 6f75 7465 2072 6571  s or reroute req
-0000cc00: 7565 7374 2055 524c 730a 2a20 4465 6661  uest URLs.* Defa
-0000cc10: 756c 7420 6062 6173 655f 7572 6c60 206e  ult `base_url` n
-0000cc20: 6f77 2061 6461 7074 7320 6465 7065 6e64  ow adapts depend
-0000cc30: 696e 6720 6f6e 2074 6865 204f 5320 2862  ing on the OS (b
-0000cc40: 6574 7465 7220 5769 6e64 6f77 7320 7375  etter Windows su
-0000cc50: 7070 6f72 7429 0a2a 2046 6978 6564 2061  pport).* Fixed a
-0000cc60: 2062 7567 2077 6865 7265 2075 7369 6e67   bug where using
-0000cc70: 2061 6e20 696e 7465 6765 7220 6173 2074   an integer as t
-0000cc80: 6865 2075 7365 7220 7061 7261 6d20 696e  he user param in
-0000cc90: 0a20 2060 436c 6965 6e74 2e63 7265 6174  .  `Client.creat
-0000cca0: 655f 636f 6e74 6169 6e65 7260 2077 6f75  e_container` wou
-0000ccb0: 6c64 2072 6573 756c 7420 696e 2061 2066  ld result in a f
-0000ccc0: 6169 6c75 7265 2e0a 0a23 2323 204d 6973  ailure...### Mis
-0000ccd0: 6365 6c6c 616e 656f 7573 0a0a 2a20 446f  cellaneous..* Do
-0000cce0: 6373 2066 6978 6573 0a2a 2049 6e74 6567  cs fixes.* Integ
-0000ccf0: 7261 7469 6f6e 2074 6573 7473 2061 7265  ration tests are
-0000cd00: 206e 6f77 2072 756e 2061 7320 7061 7274   now run as part
-0000cd10: 206f 6620 6f75 7220 636f 6e74 696e 756f   of our continuo
-0000cd20: 7573 2069 6e74 6567 7261 7469 6f6e 2e0a  us integration..
-0000cd30: 2a20 5570 6461 7465 6420 6465 7065 6e64  * Updated depend
-0000cd40: 656e 6379 206f 6e20 6073 6978 6020 6c69  ency on `six` li
-0000cd50: 6272 6172 790a 0a31 2e33 2e31 0a2d 2d2d  brary..1.3.1.---
-0000cd60: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
-0000cd70: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
-0000cd80: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-0000cd90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-0000cda0: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
-0000cdb0: 6973 7375 6573 3f71 3d6d 696c 6573 746f  issues?q=milesto
-0000cdc0: 6e65 2533 4131 2e33 2e31 2b69 7325 3341  ne%3A1.3.1+is%3A
-0000cdd0: 636c 6f73 6564 290a 0a23 2323 2042 7567  closed)..### Bug
-0000cde0: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
-0000cdf0: 2062 7567 2077 6865 7265 2065 6d70 7479   bug where empty
-0000ce00: 2063 6875 6e6b 7320 696e 2073 7472 6561   chunks in strea
-0000ce10: 6d73 2077 6173 206d 6973 696e 7465 7270  ms was misinterp
-0000ce20: 7265 7465 6420 6173 2045 4f46 2e0a 2a20  reted as EOF..* 
-0000ce30: 6064 6174 6574 696d 6560 2061 7267 756d  `datetime` argum
-0000ce40: 656e 7473 2070 6173 7365 6420 746f 2060  ents passed to `
-0000ce50: 436c 6965 6e74 2e65 7665 6e74 7360 2070  Client.events` p
-0000ce60: 6172 616d 6574 6572 7320 6073 696e 6365  arameters `since
-0000ce70: 6020 616e 640a 2020 6075 6e74 696c 6020  ` and.  `until` 
-0000ce80: 6172 6520 6e6f 7720 616c 7761 7973 2063  are now always c
-0000ce90: 6f6e 7369 6465 7265 6420 746f 2062 6520  onsidered to be 
-0000cea0: 5554 432e 0a2a 2046 6978 6564 2061 2062  UTC..* Fixed a b
-0000ceb0: 7567 2077 6974 6820 446f 636b 6572 2031  ug with Docker 1
-0000cec0: 2e37 2e78 2077 6865 7265 2074 6865 2077  .7.x where the w
-0000ced0: 726f 6e67 2061 7574 6820 6865 6164 6572  rong auth header
-0000cee0: 7320 7765 7265 2062 6569 6e67 2070 6173  s were being pas
-0000cef0: 7365 640a 2020 696e 2060 436c 6965 6e74  sed.  in `Client
-0000cf00: 2e62 7569 6c64 602c 2066 6169 6c69 6e67  .build`, failing
-0000cf10: 2062 7569 6c64 7320 7468 6174 2064 6570   builds that dep
-0000cf20: 656e 6465 6420 6f6e 2070 7269 7661 7465  ended on private
-0000cf30: 2069 6d61 6765 732e 0a2a 2060 436c 6965   images..* `Clie
-0000cf40: 6e74 2e65 7865 635f 6372 6561 7465 6020  nt.exec_create` 
-0000cf50: 6361 6e20 6e6f 7720 7265 7472 6965 7665  can now retrieve
-0000cf60: 2074 6865 2060 4964 6020 6b65 7920 6672   the `Id` key fr
-0000cf70: 6f6d 2061 2064 6963 7469 6f6e 6172 7920  om a dictionary 
-0000cf80: 666f 7220 6974 730a 2020 636f 6e74 6169  for its.  contai
-0000cf90: 6e65 7220 7061 7261 6d2e 0a0a 2323 2320  ner param...### 
-0000cfa0: 4d69 7363 656c 6c61 6e65 6f75 730a 0a2a  Miscellaneous..*
-0000cfb0: 2034 3034 2041 5049 2073 7461 7475 7320   404 API status 
-0000cfc0: 6e6f 7720 7261 6973 6573 2060 646f 636b  now raises `dock
-0000cfd0: 6572 2e65 7272 6f72 732e 4e6f 7446 6f75  er.errors.NotFou
-0000cfe0: 6e64 602e 2054 6869 7320 6578 6365 7074  nd`. This except
-0000cff0: 696f 6e20 696e 6865 7269 7473 0a20 2060  ion inherits.  `
-0000d000: 4150 4945 7272 6f72 6020 7768 6963 6820  APIError` which 
-0000d010: 7761 7320 7573 6564 2070 7265 7669 6f75  was used previou
-0000d020: 736c 792e 0a2a 2044 6f63 7320 6669 7865  sly..* Docs fixe
-0000d030: 730a 2a20 5465 7374 2066 6978 6573 0a0a  s.* Test fixes..
-0000d040: 312e 332e 300a 2d2d 2d2d 2d0a 0a5b 4c69  1.3.0.-----..[Li
-0000d050: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
-0000d060: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
-0000d070: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
-0000d080: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
-0000d090: 6f63 6b65 722d 7079 2f69 7373 7565 733f  ocker-py/issues?
-0000d0a0: 713d 6d69 6c65 7374 6f6e 6525 3341 312e  q=milestone%3A1.
-0000d0b0: 332e 302b 6973 2533 4163 6c6f 7365 6429  3.0+is%3Aclosed)
-0000d0c0: 0a0a 2323 2320 4465 7072 6563 6174 696f  ..### Deprecatio
-0000d0d0: 6e20 7761 726e 696e 670a 0a2a 2041 7320  n warning..* As 
-0000d0e0: 616e 6e6f 756e 6365 6420 696e 2074 6865  announced in the
-0000d0f0: 2031 2e32 2e30 2072 656c 6561 7365 2c20   1.2.0 release, 
-0000d100: 6043 6c69 656e 742e 6578 6563 7574 6560  `Client.execute`
-0000d110: 2068 6173 2062 6565 6e20 7265 6d6f 7665   has been remove
-0000d120: 6420 696e 2066 6176 6f72 0a20 206f 6620  d in favor.  of 
-0000d130: 6043 6c69 656e 742e 6578 6563 5f63 7265  `Client.exec_cre
-0000d140: 6174 6560 2061 6e64 2060 436c 6965 6e74  ate` and `Client
-0000d150: 2e65 7865 635f 7374 6172 7460 2e0a 0a23  .exec_start`...#
-0000d160: 2323 2046 6561 7475 7265 730a 0a2a 2060  ## Features..* `
-0000d170: 6578 7472 615f 686f 7374 7360 2070 6172  extra_hosts` par
-0000d180: 616d 6574 6572 2069 6e20 686f 7374 2063  ameter in host c
-0000d190: 6f6e 6669 6720 6361 6e20 6e6f 7720 616c  onfig can now al
-0000d1a0: 736f 2062 6520 7072 6f76 6964 6564 2061  so be provided a
-0000d1b0: 7320 6120 6c69 7374 2e0a 2a20 4164 6465  s a list..* Adde
-0000d1c0: 6420 7375 7070 6f72 7420 666f 7220 606d  d support for `m
-0000d1d0: 656d 6f72 795f 6c69 6d69 7460 2061 6e64  emory_limit` and
-0000d1e0: 2060 6d65 6d73 7761 705f 6c69 6d69 7460   `memswap_limit`
-0000d1f0: 2069 6e20 686f 7374 2063 6f6e 6669 6720   in host config 
-0000d200: 746f 0a20 2063 6f6d 706c 7920 7769 7468  to.  comply with
-0000d210: 2072 6563 656e 7420 6465 7072 6563 6174   recent deprecat
-0000d220: 696f 6e73 2e0a 2a20 4164 6465 6420 7375  ions..* Added su
-0000d230: 7070 6f72 7420 666f 7220 6076 6f6c 756d  pport for `volum
-0000d240: 655f 6472 6976 6572 6020 696e 2060 436c  e_driver` in `Cl
-0000d250: 6965 6e74 2e63 7265 6174 655f 636f 6e74  ient.create_cont
-0000d260: 6169 6e65 7260 0a2a 2041 6464 6564 2073  ainer`.* Added s
-0000d270: 7570 706f 7274 2066 6f72 2061 6476 616e  upport for advan
-0000d280: 6365 6420 6d6f 6465 7320 696e 2076 6f6c  ced modes in vol
-0000d290: 756d 6520 6269 6e64 7320 2875 7369 6e67  ume binds (using
-0000d2a0: 2074 6865 2060 6d6f 6465 6020 6b65 7929   the `mode` key)
-0000d2b0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-0000d2c0: 2066 6f72 2060 6465 636f 6465 6020 696e   for `decode` in
-0000d2d0: 2060 436c 6965 6e74 2e62 7569 6c64 6020   `Client.build` 
-0000d2e0: 2864 6563 6f64 6573 204a 534f 4e20 7374  (decodes JSON st
-0000d2f0: 7265 616d 206f 6e20 7468 6520 666c 7929  ream on the fly)
-0000d300: 0a2a 2064 6f63 6b65 722d 7079 2077 696c  .* docker-py wil
-0000d310: 6c20 6e6f 7720 6c6f 6f6b 2066 6f72 206c  l now look for l
-0000d320: 6f67 696e 2063 6f6e 6669 6775 7261 7469  ogin configurati
-0000d330: 6f6e 2075 6e64 6572 2074 6865 206e 6577  on under the new
-0000d340: 2063 6f6e 6669 6720 7061 7468 2c0a 2020   config path,.  
-0000d350: 616e 6420 6661 6c6c 2062 6163 6b20 746f  and fall back to
-0000d360: 2074 6865 206f 6c64 2060 7e2f 2e64 6f63   the old `~/.doc
-0000d370: 6b65 7263 6667 6020 7061 7468 2069 6620  kercfg` path if 
-0000d380: 6e6f 7420 7072 6573 656e 742e 0a0a 2323  not present...##
-0000d390: 2320 4275 6766 6978 6573 0a0a 2a20 436f  # Bugfixes..* Co
-0000d3a0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-0000d3b0: 206c 6f6f 6b75 7020 6e6f 7720 616c 736f   lookup now also
-0000d3c0: 2077 6f72 6b20 6f6e 2070 6c61 7466 6f72   work on platfor
-0000d3d0: 6d73 2074 6861 7420 646f 6e27 7420 6465  ms that don't de
-0000d3e0: 6669 6e65 2061 0a20 2060 2448 4f4d 4560  fine a.  `$HOME`
-0000d3f0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-0000d400: 6961 626c 652e 0a2a 2046 6978 6564 2061  iable..* Fixed a
-0000d410: 6e20 6973 7375 6520 7768 6572 6520 7069  n issue where pi
-0000d420: 6e67 696e 6720 6120 7632 2070 7269 7661  nging a v2 priva
-0000d430: 7465 2072 6567 6973 7472 7920 7761 736e  te registry wasn
-0000d440: 2774 2077 6f72 6b69 6e67 2070 726f 7065  't working prope
-0000d450: 726c 792c 0a20 2070 7265 7665 6e74 696e  rly,.  preventin
-0000d460: 6720 7573 6572 7320 6672 6f6d 2070 7573  g users from pus
-0000d470: 6869 6e67 2061 6e64 2070 756c 6c69 6e67  hing and pulling
-0000d480: 2e0a 2a20 6070 756c 6c60 2070 6172 616d  ..* `pull` param
-0000d490: 6574 6572 2069 6e20 6043 6c69 656e 742e  eter in `Client.
-0000d4a0: 6275 696c 6460 206e 6f77 2064 6566 6175  build` now defau
-0000d4b0: 6c74 7320 746f 2060 4661 6c73 6560 2e20  lts to `False`. 
-0000d4c0: 4669 7865 7320 6120 6275 6720 7768 6572  Fixes a bug wher
-0000d4d0: 650a 2020 7468 6520 6465 6661 756c 7420  e.  the default 
-0000d4e0: 6f70 7469 6f6e 7320 776f 756c 6420 7472  options would tr
-0000d4f0: 7920 746f 2066 6f72 6365 2061 2070 756c  y to force a pul
-0000d500: 6c20 6f66 206e 6f6e 2d72 656d 6f74 6520  l of non-remote 
-0000d510: 696d 6167 6573 2e0a 2a20 4669 7865 6420  images..* Fixed 
-0000d520: 6120 6275 6720 7768 6572 6520 6765 7474  a bug where gett
-0000d530: 696e 6720 6c6f 6773 2066 726f 6d20 7474  ing logs from tt
-0000d540: 792d 656e 6162 6c65 6420 636f 6e74 6169  y-enabled contai
-0000d550: 6e65 7273 2077 6173 6e27 7420 776f 726b  ners wasn't work
-0000d560: 696e 670a 2020 7072 6f70 6572 6c79 2077  ing.  properly w
-0000d570: 6974 6820 6d6f 7265 2072 6563 656e 7420  ith more recent 
-0000d580: 7665 7273 696f 6e73 206f 6620 446f 636b  versions of Dock
-0000d590: 6572 0a2a 2060 436c 6965 6e74 2e70 7573  er.* `Client.pus
-0000d5a0: 6860 2061 6e64 2060 436c 6965 6e74 2e70  h` and `Client.p
-0000d5b0: 756c 6c60 2077 696c 6c20 6e6f 7720 7261  ull` will now ra
-0000d5c0: 6973 6520 6578 6365 7074 696f 6e73 2069  ise exceptions i
-0000d5d0: 6620 7468 6520 4854 5450 0a20 2073 7461  f the HTTP.  sta
-0000d5e0: 7475 7320 696e 6469 6361 7465 7320 616e  tus indicates an
-0000d5f0: 2065 7272 6f72 2e0a 2a20 4669 7865 6420   error..* Fixed 
-0000d600: 6120 6275 6720 7769 7468 2061 6461 7074  a bug with adapt
-0000d610: 6572 206c 6f6f 6b75 7020 7768 656e 2075  er lookup when u
-0000d620: 7369 6e67 2074 6865 2055 6e69 7820 736f  sing the Unix so
-0000d630: 636b 6574 2061 6461 7074 6572 0a20 2028  cket adapter.  (
-0000d640: 7468 6973 2061 6666 6563 7465 6420 736f  this affected so
-0000d650: 6d65 2077 6569 7264 2065 6467 6520 6361  me weird edge ca
-0000d660: 7365 732c 2073 6565 2069 7373 7565 2023  ses, see issue #
-0000d670: 3634 3720 666f 7220 6465 7461 696c 7329  647 for details)
-0000d680: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-0000d690: 6865 7265 2070 726f 7669 6469 6e67 2060  here providing `
-0000d6a0: 7469 6d65 6f75 743d 4e6f 6e65 6020 746f  timeout=None` to
-0000d6b0: 2060 436c 6965 6e74 2e73 746f 7060 2077   `Client.stop` w
-0000d6c0: 6f75 6c64 2072 6573 756c 740a 2020 696e  ould result.  in
-0000d6d0: 2061 6e20 6578 6365 7074 696f 6e20 6465   an exception de
-0000d6e0: 7370 6974 6520 7468 6520 7573 6563 6173  spite the usecas
-0000d6f0: 6520 6265 696e 6720 7661 6c69 642e 0a2a  e being valid..*
-0000d700: 2041 6464 6564 2060 6769 7440 6020 746f   Added `git@` to
-0000d710: 2074 6865 206c 6973 7420 6f66 2076 616c   the list of val
-0000d720: 6964 2070 7265 6669 7865 7320 666f 7220  id prefixes for 
-0000d730: 7265 6d6f 7465 2062 7569 6c64 2070 6174  remote build pat
-0000d740: 6873 2e0a 0a23 2323 2044 6570 656e 6465  hs...### Depende
-0000d750: 6e63 6965 730a 0a2a 2054 6865 2077 6562  ncies..* The web
-0000d760: 736f 636b 6574 2d63 6c69 656e 7420 6465  socket-client de
-0000d770: 7065 6e64 656e 6379 2068 6173 2062 6565  pendency has bee
-0000d780: 6e20 7570 6461 7465 6420 746f 2061 206d  n updated to a m
-0000d790: 6f72 6520 7265 6365 6e74 2076 6572 7369  ore recent versi
-0000d7a0: 6f6e 2e0a 2020 5468 6973 206e 6577 2076  on..  This new v
-0000d7b0: 6572 7369 6f6e 2061 6c73 6f20 7375 7070  ersion also supp
-0000d7c0: 6f72 7473 2050 7974 686f 6e20 332e 782c  orts Python 3.x,
-0000d7d0: 206d 616b 696e 6720 6061 7474 6163 685f   making `attach_
-0000d7e0: 736f 636b 6574 6020 6176 6169 6c61 626c  socket` availabl
-0000d7f0: 650a 2020 6f6e 2074 686f 7365 2076 6572  e.  on those ver
-0000d800: 7369 6f6e 7320 6173 2077 656c 6c2e 0a0a  sions as well...
-0000d810: 2323 2320 446f 6375 6d65 6e74 6174 696f  ### Documentatio
-0000d820: 6e0a 0a2a 2056 6172 696f 7573 2066 6978  n..* Various fix
-0000d830: 6573 0a0a 312e 322e 330a 2d2d 2d2d 2d0a  es..1.2.3.-----.
-0000d840: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
-0000d850: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
-0000d860: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
-0000d870: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
-0000d880: 6572 2f64 6f63 6b65 722d 7079 2f69 7373  er/docker-py/iss
-0000d890: 7565 733f 713d 6d69 6c65 7374 6f6e 6525  ues?q=milestone%
-0000d8a0: 3341 312e 322e 332b 6973 2533 4163 6c6f  3A1.2.3+is%3Aclo
-0000d8b0: 7365 6429 0a0a 2323 2320 4465 7072 6563  sed)..### Deprec
-0000d8c0: 6174 696f 6e20 7761 726e 696e 670a 0a2a  ation warning..*
-0000d8d0: 2050 6173 7369 6e67 2068 6f73 7420 636f   Passing host co
-0000d8e0: 6e66 6967 2069 6e20 7468 6520 6043 6c69  nfig in the `Cli
-0000d8f0: 656e 742e 7374 6172 7460 206d 6574 686f  ent.start` metho
-0000d900: 6420 6973 206e 6f77 2064 6570 7265 6361  d is now depreca
-0000d910: 7465 642e 2050 6c65 6173 650a 2020 7573  ted. Please.  us
-0000d920: 6520 7468 6520 6068 6f73 745f 636f 6e66  e the `host_conf
-0000d930: 6967 6020 696e 2060 436c 6965 6e74 2e63  ig` in `Client.c
-0000d940: 7265 6174 655f 636f 6e74 6169 6e65 7260  reate_container`
-0000d950: 2069 6e73 7465 6164 2e0a 0a23 2323 2046   instead...### F
-0000d960: 6561 7475 7265 730a 0a2a 2041 6464 6564  eatures..* Added
-0000d970: 2073 7570 706f 7274 2066 6f72 2060 7072   support for `pr
-0000d980: 6976 696c 6567 6564 6020 7061 7261 6d20  ivileged` param 
-0000d990: 696e 2060 436c 6965 6e74 2e65 7865 635f  in `Client.exec_
-0000d9a0: 6372 6561 7465 600a 2020 286f 6e6c 7920  create`.  (only 
-0000d9b0: 6176 6169 6c61 626c 6520 696e 2041 5049  available in API
-0000d9c0: 203e 3d20 312e 3139 290a 2a20 566f 6c75   >= 1.19).* Volu
-0000d9d0: 6d65 2062 696e 6473 2063 616e 206e 6f77  me binds can now
-0000d9e0: 2061 6c73 6f20 6265 2073 7065 6369 6669   also be specifi
-0000d9f0: 6564 2061 7320 6120 6c69 7374 206f 6620  ed as a list of 
-0000da00: 7374 7269 6e67 732e 0a0a 2323 2320 4275  strings...### Bu
-0000da10: 6766 6978 6573 0a0a 2a20 4669 7865 6420  gfixes..* Fixed 
-0000da20: 6120 6275 6720 7768 6572 6520 7468 6520  a bug where the 
-0000da30: 6072 6561 645f 6f6e 6c79 6020 7061 7261  `read_only` para
-0000da40: 6d20 696e 2068 6f73 745f 636f 6e66 6967  m in host_config
-0000da50: 2077 6173 6e27 7420 6861 6e64 6c65 640a   wasn't handled.
-0000da60: 2020 7072 6f70 6572 6c79 2e0a 2a20 4669    properly..* Fi
-0000da70: 7865 6420 6120 6275 6720 696e 2060 436c  xed a bug in `Cl
-0000da80: 6965 6e74 2e65 7865 6375 7465 6020 2874  ient.execute` (t
-0000da90: 6869 7320 6d65 7468 6f64 2069 7320 7374  his method is st
-0000daa0: 696c 6c20 6465 7072 6563 6174 6564 292e  ill deprecated).
-0000dab0: 0a2a 2054 6865 2060 6370 7573 6574 6020  .* The `cpuset` 
-0000dac0: 7061 7261 6d20 696e 2060 436c 6965 6e74  param in `Client
-0000dad0: 2e63 7265 6174 655f 636f 6e74 6169 6e65  .create_containe
-0000dae0: 7260 2069 7320 616c 736f 2070 6173 7365  r` is also passe
-0000daf0: 6420 6173 0a20 2074 6865 2060 4370 7573  d as.  the `Cpus
-0000db00: 6574 4370 7573 6020 7061 7261 6d20 2860  etCpus` param (`
-0000db10: 4370 7573 6574 6020 6465 7072 6563 6174  Cpuset` deprecat
-0000db20: 6564 2069 6e20 7265 6365 6e74 2076 6572  ed in recent ver
-0000db30: 7369 6f6e 7320 6f66 2074 6865 2041 5049  sions of the API
-0000db40: 290a 2a20 4669 7865 6420 616e 2069 7373  ).* Fixed an iss
-0000db50: 7565 2077 6974 6820 696e 7465 6772 6174  ue with integrat
-0000db60: 696f 6e20 7465 7374 7320 6265 696e 6720  ion tests being 
-0000db70: 7275 6e20 696e 7369 6465 2061 2063 6f6e  run inside a con
-0000db80: 7461 696e 6572 0a20 2028 606d 616b 6520  tainer.  (`make 
-0000db90: 696e 7465 6772 6174 696f 6e2d 7465 7374  integration-test
-0000dba0: 6029 0a2a 2046 6978 6564 2061 2062 7567  `).* Fixed a bug
-0000dbb0: 2077 6865 7265 2061 6e20 656d 7074 7920   where an empty 
-0000dbc0: 7374 7269 6e67 2077 6f75 6c64 2062 6520  string would be 
-0000dbd0: 636f 6e73 6964 6572 6564 2061 2076 616c  considered a val
-0000dbe0: 6964 2063 6f6e 7461 696e 6572 2049 440a  id container ID.
-0000dbf0: 2020 6f72 2069 6d61 6765 2049 442e 0a2a    or image ID..*
-0000dc00: 2046 6978 6564 2061 2062 7567 2069 6e20   Fixed a bug in 
-0000dc10: 6043 6c69 656e 742e 696e 7365 7274 600a  `Client.insert`.
-0000dc20: 0a0a 2323 2320 446f 6375 6d65 6e74 6174  ..### Documentat
-0000dc30: 696f 6e0a 0a2a 2056 6172 696f 7573 2066  ion..* Various f
-0000dc40: 6978 6573 0a0a 312e 322e 320a 2d2d 2d2d  ixes..1.2.2.----
-0000dc50: 2d0a 0a23 2323 2042 7567 6669 7865 730a  -..### Bugfixes.
-0000dc60: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-0000dc70: 6865 7265 2070 6172 616d 6574 6572 7320  here parameters 
-0000dc80: 7061 7373 6564 2074 6f20 6043 6c69 656e  passed to `Clien
-0000dc90: 742e 6578 6563 5f72 6573 697a 6560 2077  t.exec_resize` w
-0000dca0: 6f75 6c64 2062 6520 6967 6e6f 7265 6420  ould be ignored 
-0000dcb0: 2823 3537 3629 0a2a 2046 6978 6564 2061  (#576).* Fixed a
-0000dcc0: 2062 7567 2077 6865 7265 2061 7574 6820   bug where auth 
-0000dcd0: 636f 6e66 6967 2077 6f75 6c64 6e27 7420  config wouldn't 
-0000dce0: 6265 2072 6573 6f6c 7665 6420 7072 6f70  be resolved prop
-0000dcf0: 6572 6c79 2069 6e20 6043 6c69 656e 742e  erly in `Client.
-0000dd00: 7075 6c6c 6020 2823 3537 3729 0a0a 312e  pull` (#577)..1.
-0000dd10: 322e 310a 2d2d 2d2d 2d0a 0a23 2323 2042  2.1.-----..### B
-0000dd20: 7567 6669 7865 730a 0a2a 2046 6978 6564  ugfixes..* Fixed
-0000dd30: 2061 2062 7567 2077 6865 7265 2074 6865   a bug where the
-0000dd40: 2063 6865 636b 5f72 6573 6f75 7263 6520   check_resource 
-0000dd50: 6465 636f 7261 746f 7220 776f 756c 6420  decorator would 
-0000dd60: 6272 6561 6b20 7769 7468 2073 6f6d 650a  break with some.
-0000dd70: 2020 6172 6775 6d65 6e74 2d70 6173 7369    argument-passi
-0000dd80: 6e67 206d 6574 686f 6473 2e20 2823 3537  ng methods. (#57
-0000dd90: 3329 0a0a 312e 322e 300a 2d2d 2d2d 2d0a  3)..1.2.0.-----.
-0000dda0: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
-0000ddb0: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
-0000ddc0: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
-0000ddd0: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
-0000dde0: 6572 2f64 6f63 6b65 722d 7079 2f69 7373  er/docker-py/iss
-0000ddf0: 7565 733f 713d 6d69 6c65 7374 6f6e 6525  ues?q=milestone%
-0000de00: 3341 312e 322e 302b 6973 2533 4163 6c6f  3A1.2.0+is%3Aclo
-0000de10: 7365 6429 0a0a 2323 2320 4465 7072 6563  sed)..### Deprec
-0000de20: 6174 696f 6e20 7761 726e 696e 670a 0a2a  ation warning..*
-0000de30: 2060 436c 6965 6e74 2e65 7865 6375 7465   `Client.execute
-0000de40: 6020 6973 2062 6569 6e67 2064 6570 7265  ` is being depre
-0000de50: 6361 7465 6420 696e 2066 6176 6f72 206f  cated in favor o
-0000de60: 6620 7468 6520 6d6f 7265 2064 6576 2d66  f the more dev-f
-0000de70: 7269 656e 646c 790a 2020 6043 6c69 656e  riendly.  `Clien
-0000de80: 742e 6578 6563 5f73 7461 7274 6020 616e  t.exec_start` an
-0000de90: 6420 6043 6c69 656e 742e 6578 6563 5f63  d `Client.exec_c
-0000dea0: 7265 6174 6560 2e20 2a2a 4974 2077 696c  reate`. **It wil
-0000deb0: 6c20 6265 2072 656d 6f76 6564 2069 6e20  l be removed in 
-0000dec0: 312e 332e 302a 2a0a 0a23 2323 2046 6561  1.3.0**..### Fea
-0000ded0: 7475 7265 730a 0a2a 2041 6464 6564 2060  tures..* Added `
-0000dee0: 6578 6563 5f63 7265 6174 6560 2c20 6065  exec_create`, `e
-0000def0: 7865 635f 7374 6172 7460 2c20 6065 7865  xec_start`, `exe
-0000df00: 635f 696e 7370 6563 7460 2061 6e64 2060  c_inspect` and `
-0000df10: 6578 6563 5f72 6573 697a 6560 2074 6f0a  exec_resize` to.
-0000df20: 2020 636c 6965 6e74 2c20 6163 6375 7261    client, accura
-0000df30: 7465 6c79 206d 6972 726f 7269 6e67 2074  tely mirroring t
-0000df40: 6865 0a20 205b 4578 6563 2041 5049 5d28  he.  [Exec API](
-0000df50: 6874 7470 733a 2f2f 646f 6373 2e64 6f63  https://docs.doc
-0000df60: 6b65 722e 636f 6d2f 7265 6665 7265 6e63  ker.com/referenc
-0000df70: 652f 6170 692f 646f 636b 6572 5f72 656d  e/api/docker_rem
-0000df80: 6f74 655f 6170 695f 7631 2e31 382f 2365  ote_api_v1.18/#e
-0000df90: 7865 632d 6372 6561 7465 290a 2a20 4164  xec-create).* Ad
-0000dfa0: 6465 6420 6061 7574 685f 636f 6e66 6967  ded `auth_config
-0000dfb0: 6020 7061 7261 6d20 746f 2060 436c 6965  ` param to `Clie
-0000dfc0: 6e74 2e70 756c 6c60 2028 616c 6c6f 7773  nt.pull` (allows
-0000dfd0: 2074 6f20 7573 6520 6f6e 652d 6f66 6620   to use one-off 
-0000dfe0: 6372 6564 656e 7469 616c 730a 2020 666f  credentials.  fo
-0000dff0: 7220 7468 6973 2070 756c 6c20 7265 7175  r this pull requ
-0000e000: 6573 7429 0a2a 2041 6464 6564 2073 7570  est).* Added sup
-0000e010: 706f 7274 2066 6f72 2060 6970 635f 6d6f  port for `ipc_mo
-0000e020: 6465 6020 696e 2068 6f73 7420 636f 6e66  de` in host conf
-0000e030: 6967 2e0a 2a20 4164 6465 6420 7375 7070  ig..* Added supp
-0000e040: 6f72 7420 666f 7220 7468 6520 606c 6f67  ort for the `log
-0000e050: 5f63 6f6e 6669 6760 2070 6172 616d 2069  _config` param i
-0000e060: 6e20 686f 7374 2063 6f6e 6669 672e 0a2a  n host config..*
-0000e070: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-0000e080: 6f72 2074 6865 2060 756c 696d 6974 6020  or the `ulimit` 
-0000e090: 7061 7261 6d20 696e 2068 6f73 7420 636f  param in host co
-0000e0a0: 6e66 6967 2e0a 2a20 4164 6465 6420 7375  nfig..* Added su
-0000e0b0: 7070 6f72 7420 666f 7220 636f 6e74 6169  pport for contai
-0000e0c0: 6e65 7220 7265 736f 7572 6365 206c 696d  ner resource lim
-0000e0d0: 6974 7320 696e 2060 436c 6965 6e74 2e62  its in `Client.b
-0000e0e0: 7569 6c64 602e 0a2a 2057 6865 6e20 6120  uild`..* When a 
-0000e0f0: 7265 736f 7572 6365 2069 6465 6e74 6966  resource identif
-0000e100: 6965 7220 2869 6d61 6765 206f 7220 636f  ier (image or co
-0000e110: 6e74 6169 6e65 7220 4944 2920 6973 2070  ntainer ID) is p
-0000e120: 6173 7365 6420 746f 2061 2043 6c69 656e  assed to a Clien
-0000e130: 740a 2020 6d65 7468 6f64 2c20 7765 206e  t.  method, we n
-0000e140: 6f77 2063 6865 636b 2066 6f72 2060 4e6f  ow check for `No
-0000e150: 6e65 6020 7661 6c75 6573 2074 6f20 6176  ne` values to av
-0000e160: 6f69 6420 6372 6173 6869 6e67 0a20 2028  oid crashing.  (
-0000e170: 6e6f 7720 7261 6973 6573 2060 646f 636b  now raises `dock
-0000e180: 6572 2e65 7272 6f72 732e 4e75 6c6c 5265  er.errors.NullRe
-0000e190: 736f 7572 6365 6029 0a2a 2041 6464 6564  source`).* Added
-0000e1a0: 2074 6f6f 6c73 2074 6f20 7061 7273 6520   tools to parse 
-0000e1b0: 706f 7274 2072 616e 6765 7320 696e 7369  port ranges insi
-0000e1c0: 6465 2074 6865 206e 6577 2060 646f 636b  de the new `dock
-0000e1d0: 6572 2e75 7469 6c73 2e70 6f72 7473 6020  er.utils.ports` 
-0000e1e0: 7061 636b 6167 652e 0a2a 2041 6464 6564  package..* Added
-0000e1f0: 2061 2060 7665 7273 696f 6e5f 696e 666f   a `version_info
-0000e200: 6020 6174 7472 6962 7574 6520 746f 2074  ` attribute to t
-0000e210: 6865 2060 646f 636b 6572 6020 7061 636b  he `docker` pack
-0000e220: 6167 652e 0a0a 2323 2320 4275 6766 6978  age...### Bugfix
-0000e230: 6573 0a0a 2a20 4669 7865 6420 6120 6275  es..* Fixed a bu
-0000e240: 6720 696e 2060 436c 6965 6e74 2e70 6f72  g in `Client.por
-0000e250: 7460 2077 6865 7265 2061 6273 656e 6365  t` where absence
-0000e260: 206f 6620 6120 6365 7274 6169 6e20 6b65   of a certain ke
-0000e270: 7920 696e 2074 6865 0a20 2063 6f6e 7461  y in the.  conta
-0000e280: 696e 6572 2773 204a 534f 4e20 776f 756c  iner's JSON woul
-0000e290: 6420 7261 6973 6520 616e 2065 7272 6f72  d raise an error
-0000e2a0: 2028 6e6f 7720 6a75 7374 2072 6574 7572   (now just retur
-0000e2b0: 6e73 2060 4e6f 6e65 6029 0a2a 2046 6978  ns `None`).* Fix
-0000e2c0: 6564 2061 2062 7567 2077 6974 6820 7468  ed a bug with th
-0000e2d0: 6520 6074 7275 6e63 6020 7061 7261 6d65  e `trunc` parame
-0000e2e0: 7465 7220 696e 2060 436c 6965 6e74 2e63  ter in `Client.c
-0000e2f0: 6f6e 7461 696e 6572 7360 2068 6176 696e  ontainers` havin
-0000e300: 6720 6e6f 0a20 2065 6666 6563 7420 286d  g no.  effect (m
-0000e310: 6f76 6564 2066 756e 6374 696f 6e61 6c69  oved functionali
-0000e320: 7479 2074 6f20 7468 6520 636c 6965 6e74  ty to the client
-0000e330: 290a 2a20 5365 7665 7261 6c20 696d 7072  ).* Several impr
-0000e340: 6f76 656d 656e 7473 2068 6176 6520 6265  ovements have be
-0000e350: 656e 206d 6164 6520 746f 2074 6865 2060  en made to the `
-0000e360: 436c 6965 6e74 2e69 6d70 6f72 745f 696d  Client.import_im
-0000e370: 6167 6560 206d 6574 686f 642e 0a2a 2046  age` method..* F
-0000e380: 6978 6564 2070 7573 6869 6e67 202f 2070  ixed pushing / p
-0000e390: 756c 6c69 6e67 2074 6f0a 2020 5b76 3220  ulling to.  [v2 
-0000e3a0: 7265 6769 7374 7269 6573 5d28 6874 7470  registries](http
-0000e3b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-0000e3c0: 6f63 6b65 722f 6469 7374 7269 6275 7469  ocker/distributi
-0000e3d0: 6f6e 290a 2a20 4669 7865 6420 6120 6275  on).* Fixed a bu
-0000e3e0: 6720 7768 6572 6520 7061 7373 696e 6720  g where passing 
-0000e3f0: 6120 636f 6e74 6169 6e65 7220 6469 6374  a container dict
-0000e400: 696f 6e61 7279 2074 6f20 6043 6c69 656e  ionary to `Clien
-0000e410: 742e 636f 6d6d 6974 600a 2020 776f 756c  t.commit`.  woul
-0000e420: 6420 6661 696c 0a0a 2323 2320 4d69 7363  d fail..### Misc
-0000e430: 656c 6c61 6e65 6f75 730a 0a2a 2044 6566  ellaneous..* Def
-0000e440: 6175 6c74 2041 5049 2076 6572 7369 6f6e  ault API version
-0000e450: 2068 6173 2062 6565 6e20 6275 6d70 6564   has been bumped
-0000e460: 2074 6f20 312e 3138 2028 446f 636b 6572   to 1.18 (Docker
-0000e470: 2045 6e67 696e 6520 312e 362e 3029 0a2a   Engine 1.6.0).*
-0000e480: 2053 6576 6572 616c 2074 6573 7469 6e67   Several testing
-0000e490: 2063 6f76 6572 6167 6520 696d 7072 6f76   coverage improv
-0000e4a0: 656d 656e 7473 0a2a 2044 6f63 7320 6669  ements.* Docs fi
-0000e4b0: 7865 7320 616e 6420 696d 7072 6f76 656d  xes and improvem
-0000e4c0: 656e 7473 0a0a 312e 312e 300a 2d2d 2d2d  ents..1.1.0.----
-0000e4d0: 2d0a 0a23 2323 2046 6561 7475 7265 730a  -..### Features.
-0000e4e0: 0a2a 2041 6464 6564 2060 646f 636b 6572  .* Added `docker
-0000e4f0: 6669 6c65 6020 7061 7261 6d20 7375 7070  file` param supp
-0000e500: 6f72 7420 746f 2060 436c 6965 6e74 2e62  ort to `Client.b
-0000e510: 7569 6c64 6020 286d 6972 726f 7273 0a20  uild` (mirrors. 
-0000e520: 2060 646f 636b 6572 2062 7569 6c64 202d   `docker build -
-0000e530: 6660 2062 6568 6176 696f 7229 0a2a 2041  f` behavior).* A
-0000e540: 6464 6564 2074 6865 2061 6269 6c69 7479  dded the ability
-0000e550: 2074 6f20 7370 6563 6966 7920 6027 6175   to specify `'au
-0000e560: 746f 2760 2061 7320 6076 6572 7369 6f6e  to'` as `version
-0000e570: 6020 696e 2060 436c 6965 6e74 2e5f 5f69  ` in `Client.__i
-0000e580: 6e69 745f 5f60 2c0a 2020 616c 6c6f 7769  nit__`,.  allowi
-0000e590: 6e67 2074 6865 2063 6f6e 7374 7275 6374  ng the construct
-0000e5a0: 6f72 2074 6f20 6175 746f 6465 7465 6374  or to autodetect
-0000e5b0: 2074 6865 2064 6165 6d6f 6e27 7320 4150   the daemon's AP
-0000e5c0: 4920 7665 7273 696f 6e2e 0a0a 2323 2320  I version...### 
-0000e5d0: 4275 6766 6978 6573 0a0a 2a20 4669 7865  Bugfixes..* Fixe
-0000e5e0: 6420 6120 6275 6720 7768 6572 6520 6465  d a bug where de
-0000e5f0: 636f 6469 6e67 2061 2072 6573 756c 7420  coding a result 
-0000e600: 7374 7265 616d 2075 7369 6e67 2074 6865  stream using the
-0000e610: 2060 6465 636f 6465 6020 7061 7261 6d65   `decode` parame
-0000e620: 7465 720a 2020 776f 756c 6420 6272 6561  ter.  would brea
-0000e630: 6b20 7768 656e 2075 7369 6e67 2050 7974  k when using Pyt
-0000e640: 686f 6e20 332e 780a 2a20 4669 7865 6420  hon 3.x.* Fixed 
-0000e650: 6120 6275 6720 7768 6572 6520 736f 6d65  a bug where some
-0000e660: 2066 696c 6573 2069 6e20 602e 646f 636b   files in `.dock
-0000e670: 6572 6967 6e6f 7265 6020 7765 7265 6e27  erignore` weren'
-0000e680: 7420 6265 696e 6720 6861 6e64 6c65 640a  t being handled.
-0000e690: 2020 7072 6f70 6572 6c79 0a2a 2046 6978    properly.* Fix
-0000e6a0: 6564 2060 7265 736f 6c76 655f 6175 7468  ed `resolve_auth
-0000e6b0: 636f 6e66 6967 6020 6973 7375 6573 2062  config` issues b
-0000e6c0: 7920 6272 696e 6769 6e67 2069 7420 636c  y bringing it cl
-0000e6d0: 6f73 6572 2074 6f20 446f 636b 6572 2045  oser to Docker E
-0000e6e0: 6e67 696e 6527 730a 2020 6265 6861 7669  ngine's.  behavi
-0000e6f0: 6f72 2e20 5468 6973 2073 686f 756c 6420  or. This should 
-0000e700: 6669 7820 616c 6c20 6973 7375 6573 2065  fix all issues e
-0000e710: 6e63 6f75 6e74 6572 6564 2077 6974 6820  ncountered with 
-0000e720: 7072 6976 6174 6520 7265 6769 7374 7279  private registry
-0000e730: 2061 7574 680a 2a20 4669 7865 6420 616e   auth.* Fixed an
-0000e740: 2069 7373 7565 2077 6865 7265 2070 6173   issue where pas
-0000e750: 7377 6f72 6473 2063 6f6e 7461 696e 696e  swords containin
-0000e760: 6720 6120 636f 6c6f 6e20 7765 7265 6e27  g a colon weren'
-0000e770: 7420 6265 696e 6720 6861 6e64 6c65 640a  t being handled.
-0000e780: 2020 7072 6f70 6572 6c79 2e0a 2a20 4275    properly..* Bu
-0000e790: 6d70 6564 2060 7265 7175 6573 7473 6020  mped `requests` 
-0000e7a0: 7665 7273 696f 6e20 7265 7175 6972 656d  version requirem
-0000e7b0: 656e 742c 2077 6869 6368 2073 686f 756c  ent, which shoul
-0000e7c0: 6420 6669 7820 6d6f 7374 206f 6620 7468  d fix most of th
-0000e7d0: 6520 5353 4c0a 2020 6973 7375 6573 2065  e SSL.  issues e
-0000e7e0: 6e63 6f75 6e74 6572 6564 2072 6563 656e  ncountered recen
-0000e7f0: 746c 792e 0a0a 2323 2320 4d69 7363 656c  tly...### Miscel
-0000e800: 6c61 6e65 6f75 730a 0a2a 2053 6576 6572  laneous..* Sever
-0000e810: 616c 2069 6e74 6567 7261 7469 6f6e 2074  al integration t
-0000e820: 6573 7420 696d 7072 6f76 656d 656e 7473  est improvements
-0000e830: 2e0a 2a20 4669 7865 6420 736f 6d65 2075  ..* Fixed some u
-0000e840: 6e63 6c6f 7365 6420 7265 736f 7572 6365  nclosed resource
-0000e850: 7320 696e 2075 6e69 7420 7465 7374 732e  s in unit tests.
-0000e860: 0a2a 2053 6576 6572 616c 2064 6f63 7320  .* Several docs 
-0000e870: 696d 7072 6f76 656d 656e 7473 2e0a 0a31  improvements...1
-0000e880: 2e30 2e30 0a2d 2d2d 2d2d 0a0a 2323 2320  .0.0.-----..### 
-0000e890: 4665 6174 7572 6573 0a0a 2a20 4164 6465  Features..* Adde
-0000e8a0: 6420 6e65 7720 6043 6c69 656e 742e 7265  d new `Client.re
-0000e8b0: 6e61 6d65 6020 6d65 7468 6f64 2028 6064  name` method (`d
-0000e8c0: 6f63 6b65 7220 7265 6e61 6d65 6029 0a2a  ocker rename`).*
-0000e8d0: 2041 6464 6564 206e 6f77 2060 436c 6965   Added now `Clie
-0000e8e0: 6e74 2e73 7461 7473 6020 6d65 7468 6f64  nt.stats` method
-0000e8f0: 2028 6064 6f63 6b65 7220 7374 6174 7360   (`docker stats`
-0000e900: 290a 2a20 4164 6465 6420 6072 6561 645f  ).* Added `read_
-0000e910: 6f6e 6c79 6020 7061 7261 6d20 7375 7070  only` param supp
-0000e920: 6f72 7420 746f 2060 7574 696c 732e 6372  ort to `utils.cr
-0000e930: 6561 7465 5f68 6f73 745f 636f 6e66 6967  eate_host_config
-0000e940: 6020 616e 640a 2020 6043 6c69 656e 742e  ` and.  `Client.
-0000e950: 7374 6172 7460 2028 6064 6f63 6b65 7220  start` (`docker 
-0000e960: 7275 6e20 2d2d 7265 6164 2d6f 6e6c 7960  run --read-only`
-0000e970: 290a 2a20 4164 6465 6420 6070 6964 5f6d  ).* Added `pid_m
-0000e980: 6f64 6560 2070 6172 616d 2073 7570 706f  ode` param suppo
-0000e990: 7274 2074 6f20 6075 7469 6c73 2e63 7265  rt to `utils.cre
-0000e9a0: 6174 655f 686f 7374 5f63 6f6e 6669 6760  ate_host_config`
-0000e9b0: 2061 6e64 0a20 2060 436c 6965 6e74 2e73   and.  `Client.s
-0000e9c0: 7461 7274 6020 2860 646f 636b 6572 2072  tart` (`docker r
-0000e9d0: 756e 202d 2d70 6964 3d27 686f 7374 2760  un --pid='host'`
-0000e9e0: 290a 2a20 4164 6465 6420 6073 696e 6365  ).* Added `since
-0000e9f0: 602c 2060 756e 7469 6c60 2061 6e64 2060  `, `until` and `
-0000ea00: 6669 6c74 6572 7360 2070 6172 616d 7320  filters` params 
-0000ea10: 746f 2060 436c 6965 6e74 2e65 7665 6e74  to `Client.event
-0000ea20: 7360 2e0a 2a20 4164 6465 6420 6064 6563  s`..* Added `dec
-0000ea30: 6f64 6560 2070 6172 616d 6574 6572 2074  ode` parameter t
-0000ea40: 6f20 6043 6c69 656e 742e 7374 6174 7360  o `Client.stats`
-0000ea50: 2061 6e64 2060 436c 6965 6e74 2e65 7665   and `Client.eve
-0000ea60: 6e74 7360 2074 6f20 6465 636f 6465 0a20  nts` to decode. 
-0000ea70: 204a 534f 4e20 6f62 6a65 6374 7320 6f6e   JSON objects on
-0000ea80: 2074 6865 2066 6c79 2028 4661 6c73 6520   the fly (False 
-0000ea90: 6279 2064 6566 6175 6c74 292e 0a0a 2323  by default)...##
-0000eaa0: 2320 4275 6766 6978 6573 0a0a 2a20 4669  # Bugfixes..* Fi
-0000eab0: 7865 6420 6120 6275 6720 7468 6174 2063  xed a bug that c
-0000eac0: 6175 7365 6420 6043 6c69 656e 742e 6275  aused `Client.bu
-0000ead0: 696c 6460 2074 6f20 6372 6173 6820 7768  ild` to crash wh
-0000eae0: 656e 2074 6865 2070 726f 7669 6465 6420  en the provided 
-0000eaf0: 736f 7572 6365 2077 6173 0a20 2061 2072  source was.  a r
-0000eb00: 656d 6f74 6520 736f 7572 6365 2e0a 0a23  emote source...#
-0000eb10: 2323 204d 6973 6365 6c6c 616e 656f 7573  ## Miscellaneous
-0000eb20: 0a0a 2a20 4465 6661 756c 7420 4150 4920  ..* Default API 
-0000eb30: 7665 7273 696f 6e20 6861 7320 6265 656e  version has been
-0000eb40: 2062 756d 7065 6420 746f 2031 2e31 3720   bumped to 1.17 
-0000eb50: 2844 6f63 6b65 7220 456e 6769 6e65 2031  (Docker Engine 1
-0000eb60: 2e35 2e30 290a 2a20 6043 6c69 656e 742e  .5.0).* `Client.
-0000eb70: 7469 6d65 6f75 7460 2069 7320 6e6f 7720  timeout` is now 
-0000eb80: 6120 7075 626c 6963 2061 7474 7269 6275  a public attribu
-0000eb90: 7465 2c20 616e 6420 7573 6572 7320 6172  te, and users ar
-0000eba0: 6520 656e 636f 7572 6167 6564 2074 6f20  e encouraged to 
-0000ebb0: 7573 6520 6974 0a20 2077 6865 6e20 7265  use it.  when re
-0000ebc0: 7175 6573 7420 7469 6d65 6f75 7473 206e  quest timeouts n
-0000ebd0: 6565 6420 746f 2062 6520 6368 616e 6765  eed to be change
-0000ebe0: 6420 6174 2072 756e 7469 6d65 2e0a 2a20  d at runtime..* 
-0000ebf0: 4164 6465 6420 6043 6c69 656e 742e 6170  Added `Client.ap
-0000ec00: 695f 7665 7273 696f 6e60 2061 7320 6120  i_version` as a 
-0000ec10: 7265 6164 2d6f 6e6c 7920 7072 6f70 6572  read-only proper
-0000ec20: 7479 2e0a 2a20 5468 6520 606d 656d 7377  ty..* The `memsw
-0000ec30: 6170 5f6c 696d 6974 6020 6172 6775 6d65  ap_limit` argume
-0000ec40: 6e74 2069 6e20 6043 6c69 656e 742e 6372  nt in `Client.cr
-0000ec50: 6561 7465 5f63 6f6e 7461 696e 6572 6020  eate_container` 
-0000ec60: 6e6f 7720 6163 6365 7074 7320 7374 7269  now accepts stri
-0000ec70: 6e67 0a20 2074 7970 6520 7661 6c75 6573  ng.  type values
-0000ec80: 2073 696d 696c 6172 2074 6f20 606d 656d   similar to `mem
-0000ec90: 5f6c 696d 6974 6020 2827 3667 272c 2027  _limit` ('6g', '
-0000eca0: 3132 3030 3030 6b27 2c20 6574 632e 290a  120000k', etc.).
-0000ecb0: 2a20 496d 7072 6f76 6564 2064 6f63 756d  * Improved docum
-0000ecc0: 656e 7461 7469 6f6e 0a0a 302e 372e 320a  entation..0.7.2.
-0000ecd0: 2d2d 2d2d 2d0a 0a23 2323 2046 6561 7475  -----..### Featu
-0000ece0: 7265 730a 0a2a 2041 6464 6564 2073 7570  res..* Added sup
-0000ecf0: 706f 7274 2066 6f72 2060 6d61 635f 6164  port for `mac_ad
-0000ed00: 6472 6573 7360 2069 6e20 6043 6c69 656e  dress` in `Clien
-0000ed10: 742e 6372 6561 7465 5f63 6f6e 7461 696e  t.create_contain
-0000ed20: 6572 600a 0a23 2323 2042 7567 6669 7865  er`..### Bugfixe
-0000ed30: 730a 0a2a 2046 6978 6564 2061 2062 7567  s..* Fixed a bug
-0000ed40: 2077 6865 7265 2073 7472 6561 6d69 6e67   where streaming
-0000ed50: 2072 6573 706f 6e73 6573 2028 6070 756c   responses (`pul
-0000ed60: 6c60 2c20 6070 7573 6860 2c20 606c 6f67  l`, `push`, `log
-0000ed70: 7360 2c20 6574 632e 2920 7765 7265 0a20  s`, etc.) were. 
-0000ed80: 2075 6e72 656c 6961 626c 6520 2823 3330   unreliable (#30
-0000ed90: 3029 0a2a 2046 6978 6564 2061 2062 7567  0).* Fixed a bug
-0000eda0: 2077 6865 7265 2072 6573 6f6c 7665 5f61   where resolve_a
-0000edb0: 7574 6863 6f6e 6669 6720 776f 756c 646e  uthconfig wouldn
-0000edc0: 2774 2070 726f 7065 726c 7920 7265 736f  't properly reso
-0000edd0: 6c76 6520 636f 6e66 6967 7572 6174 696f  lve configuratio
-0000ede0: 6e0a 2020 666f 7220 7072 6976 6174 6520  n.  for private 
-0000edf0: 7265 706f 7369 746f 7269 6573 2028 2334  repositories (#4
-0000ee00: 3638 290a 2a20 4669 7865 6420 6120 6275  68).* Fixed a bu
-0000ee10: 6720 7768 6572 6520 736f 6d65 2065 7272  g where some err
-0000ee20: 6f72 7320 776f 756c 646e 2774 2062 6520  ors wouldn't be 
-0000ee30: 7072 6f70 6572 6c79 2063 6f6e 7374 7275  properly constru
-0000ee40: 6374 6564 2069 6e0a 2020 6063 6c69 656e  cted in.  `clien
-0000ee50: 742e 7079 602c 206c 6561 6469 6e67 2074  t.py`, leading t
-0000ee60: 6f20 756e 6865 6c70 6675 6c20 6578 6365  o unhelpful exce
-0000ee70: 7074 696f 6e73 2062 7562 626c 696e 6720  ptions bubbling 
-0000ee80: 7570 2028 2334 3636 290a 2a20 4669 7865  up (#466).* Fixe
-0000ee90: 6420 6120 6275 6720 7768 6572 6520 6043  d a bug where `C
-0000eea0: 6c69 656e 742e 6275 696c 6460 2077 6f75  lient.build` wou
-0000eeb0: 6c64 2074 7279 2074 6f20 636c 6f73 6520  ld try to close 
-0000eec0: 636f 6e74 6578 7420 7768 656e 2065 7874  context when ext
-0000eed0: 6572 6e61 6c6c 790a 2020 7072 6f76 6964  ernally.  provid
-0000eee0: 6564 2028 6063 7573 746f 6d5f 636f 6e74  ed (`custom_cont
-0000eef0: 6578 7420 3d3d 2054 7275 6560 2920 2823  ext == True`) (#
-0000ef00: 3435 3829 0a2a 2046 6978 6564 2061 6e20  458).* Fixed an 
-0000ef10: 6973 7375 6520 696e 2060 6372 6561 7465  issue in `create
-0000ef20: 5f68 6f73 745f 636f 6e66 6967 6020 7768  _host_config` wh
-0000ef30: 6572 6520 656d 7074 7920 7365 7175 656e  ere empty sequen
-0000ef40: 6365 7320 776f 756c 646e 2774 2062 650a  ces wouldn't be.
-0000ef50: 2020 696e 7465 7270 7265 7465 6420 7072    interpreted pr
-0000ef60: 6f70 6572 6c79 2028 2334 3632 290a 0a23  operly (#462)..#
-0000ef70: 2323 204d 6973 6365 6c6c 616e 656f 7573  ## Miscellaneous
-0000ef80: 0a0a 2a20 4164 6465 6420 6072 6573 6f6c  ..* Added `resol
-0000ef90: 7665 5f61 7574 6863 6f6e 6669 6760 2074  ve_authconfig` t
-0000efa0: 6573 7473 2e0a 0a30 2e37 2e31 0a2d 2d2d  ests...0.7.1.---
-0000efb0: 2d2d 0a0a 2323 2320 4275 6766 6978 6573  --..### Bugfixes
-0000efc0: 0a0a 2a20 6073 6574 7570 2e70 7960 206e  ..* `setup.py` n
-0000efd0: 6f77 2069 6e64 6963 6174 6573 2061 206d  ow indicates a m
-0000efe0: 6178 696d 756d 2076 6572 7369 6f6e 206f  aximum version o
-0000eff0: 6620 7265 7175 6573 7473 2074 6f20 776f  f requests to wo
-0000f000: 726b 2061 726f 756e 6420 7468 650a 2020  rk around the.  
-0000f010: 626f 6f74 3264 6f63 6b65 7220 2f20 6061  boot2docker / `a
-0000f020: 7373 6572 745f 686f 7374 6e61 6d65 6020  ssert_hostname` 
-0000f030: 6275 672e 0a2a 2052 656d 6f76 6564 2069  bug..* Removed i
-0000f040: 6e76 616c 6964 2065 7863 6570 7469 6f6e  nvalid exception
-0000f050: 2077 6865 6e20 7573 696e 6720 7468 6520   when using the 
-0000f060: 5265 6769 7374 7279 2048 7562 2773 2046  Registry Hub's F
-0000f070: 5144 4e20 7768 656e 2070 756c 6c69 6e67  QDN when pulling
-0000f080: 2e0a 2a20 4669 7865 6420 616e 2069 7373  ..* Fixed an iss
-0000f090: 7565 2077 6865 7265 2065 6172 6c79 2048  ue where early H
-0000f0a0: 5454 5020 6572 726f 7273 2077 6572 656e  TTP errors weren
-0000f0b0: 2774 2068 616e 646c 6564 2070 726f 7065  't handled prope
-0000f0c0: 726c 7920 696e 2073 7472 6561 6d69 6e67  rly in streaming
-0000f0d0: 0a20 2072 6573 706f 6e73 6573 2e0a 2a20  .  responses..* 
-0000f0e0: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
-0000f0f0: 6520 736f 636b 6574 7320 776f 756c 6420  e sockets would 
-0000f100: 636c 6f73 6520 756e 6578 7065 6374 6564  close unexpected
-0000f110: 6c79 2075 7369 6e67 2050 7974 686f 6e20  ly using Python 
-0000f120: 332e 780a 2a20 5661 7269 6f75 7320 6669  3.x.* Various fi
-0000f130: 7865 7320 666f 7220 696e 7465 6772 6174  xes for integrat
-0000f140: 696f 6e20 7465 7374 732e 0a0a 2323 2320  ion tests...### 
-0000f150: 4d69 7363 656c 6c61 6e65 6f75 730a 0a2a  Miscellaneous..*
-0000f160: 2053 6d61 6c6c 2064 6f63 2066 6978 6573   Small doc fixes
-0000f170: 0a0a 302e 372e 300a 2d2d 2d2d 2d0a 0a23  ..0.7.0.-----..#
-0000f180: 2323 2042 7265 616b 696e 6720 6368 616e  ## Breaking chan
-0000f190: 6765 730a 0a2a 2050 6173 7369 6e67 2060  ges..* Passing `
-0000f1a0: 646e 7360 206f 7220 6076 6f6c 756d 6573  dns` or `volumes
-0000f1b0: 5f66 726f 6d60 2069 6e20 6043 6c69 656e  _from` in `Clien
-0000f1c0: 742e 7374 6172 7460 2077 6974 6820 4150  t.start` with AP
-0000f1d0: 4920 7665 7273 696f 6e20 3c20 312e 3130  I version < 1.10
-0000f1e0: 0a20 2077 696c 6c20 6e6f 7720 7261 6973  .  will now rais
-0000f1f0: 6520 616e 2065 7863 6570 7469 6f6e 2028  e an exception (
-0000f200: 7072 6576 696f 7573 6c79 206f 6e6c 7920  previously only 
-0000f210: 7472 6967 6765 7265 6420 6120 7761 726e  triggered a warn
-0000f220: 696e 6729 0a0a 2323 2320 4665 6174 7572  ing)..### Featur
-0000f230: 6573 0a0a 2a20 4164 6465 6420 7375 7070  es..* Added supp
-0000f240: 6f72 7420 666f 7220 6068 6f73 745f 636f  ort for `host_co
-0000f250: 6e66 6967 6020 696e 2060 436c 6965 6e74  nfig` in `Client
-0000f260: 2e63 7265 6174 655f 636f 6e74 6169 6e65  .create_containe
-0000f270: 7260 0a2a 2041 6464 6564 2075 7469 6c69  r`.* Added utili
-0000f280: 7479 206d 6574 686f 6420 6064 6f63 6b65  ty method `docke
-0000f290: 722e 7574 696c 732e 6372 6561 7465 5f68  r.utils.create_h
-0000f2a0: 6f73 745f 636f 6e66 6967 6020 746f 2068  ost_config` to h
-0000f2b0: 656c 7020 6275 696c 6420 610a 2020 7072  elp build a.  pr
-0000f2c0: 6f70 6572 2060 486f 7374 436f 6e66 6967  oper `HostConfig
-0000f2d0: 6020 6469 6374 696f 6e61 7279 2e0a 2a20  ` dictionary..* 
-0000f2e0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-0000f2f0: 7220 7468 6520 6070 756c 6c60 2070 6172  r the `pull` par
-0000f300: 616d 6574 6572 2069 6e20 6043 6c69 656e  ameter in `Clien
-0000f310: 742e 6275 696c 6460 0a2a 2041 6464 6564  t.build`.* Added
-0000f320: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
-0000f330: 2060 666f 7263 6572 6d60 2070 6172 616d   `forcerm` param
-0000f340: 6574 6572 2069 6e20 6043 6c69 656e 742e  eter in `Client.
-0000f350: 6275 696c 6460 0a2a 2041 6464 6564 2073  build`.* Added s
-0000f360: 7570 706f 7274 2066 6f72 2060 6578 7472  upport for `extr
-0000f370: 615f 686f 7374 7360 2069 6e20 6043 6c69  a_hosts` in `Cli
-0000f380: 656e 742e 7374 6172 7460 0a2a 2041 6464  ent.start`.* Add
-0000f390: 6564 2073 7570 706f 7274 2066 6f72 2061  ed support for a
-0000f3a0: 2063 7573 746f 6d20 6074 696d 656f 7574   custom `timeout
-0000f3b0: 6020 696e 2060 436c 6965 6e74 2e77 6169  ` in `Client.wai
-0000f3c0: 7460 0a2a 2041 6464 6564 2073 7570 706f  t`.* Added suppo
-0000f3d0: 7274 2066 6f72 2063 7573 746f 6d20 602e  rt for custom `.
-0000f3e0: 646f 636b 6572 6366 6760 206c 6f61 6469  dockercfg` loadi
-0000f3f0: 6e67 2069 6e20 6043 6c69 656e 742e 6c6f  ng in `Client.lo
-0000f400: 6769 6e60 0a20 2028 6064 6f63 6b65 7263  gin`.  (`dockerc
-0000f410: 6667 5f70 6174 6860 2061 7267 756d 656e  fg_path` argumen
-0000f420: 7429 0a0a 2323 2320 4275 6766 6978 6573  t)..### Bugfixes
-0000f430: 0a0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
-0000f440: 7768 6572 6520 736f 6d65 206f 7574 7075  where some outpu
-0000f450: 7420 776f 756c 646e 2774 2062 6520 7374  t wouldn't be st
-0000f460: 7265 616d 6564 2070 726f 7065 726c 7920  reamed properly 
-0000f470: 696e 2073 7472 6561 6d69 6e67 0a20 2063  in streaming.  c
-0000f480: 6875 6e6b 6564 2072 6573 706f 6e73 6573  hunked responses
-0000f490: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-0000f4a0: 6865 7265 2074 6865 2060 6465 7669 6365  here the `device
-0000f4b0: 7360 2070 6172 616d 2064 6964 6e27 7420  s` param didn't 
-0000f4c0: 7265 636f 676e 697a 6520 7468 6520 7072  recognize the pr
-0000f4d0: 6f70 6572 2064 656c 696d 6974 6572 0a2a  oper delimiter.*
-0000f4e0: 2060 436c 6965 6e74 2e6c 6f67 696e 6020   `Client.login` 
-0000f4f0: 6e6f 7720 7072 6f70 6572 6c79 2065 7870  now properly exp
-0000f500: 616e 6473 2074 6865 2060 7265 6769 7374  ands the `regist
-0000f510: 7279 6020 5552 4c20 6966 2070 726f 7669  ry` URL if provi
-0000f520: 6465 642e 0a2a 2046 6978 6564 2061 2062  ded..* Fixed a b
-0000f530: 7567 2077 6865 7265 2075 6e69 636f 6465  ug where unicode
-0000f540: 2063 6861 7261 6374 6572 7320 696e 2070   characters in p
-0000f550: 6173 7365 6420 666f 7220 6065 6e76 6972  assed for `envir
-0000f560: 6f6e 6d65 6e74 6020 696e 0a20 2060 6372  onment` in.  `cr
-0000f570: 6561 7465 5f63 6f6e 7461 696e 6572 6020  eate_container` 
-0000f580: 776f 756c 6420 6272 6561 6b2e 0a0a 2323  would break...##
-0000f590: 2320 4d69 7363 656c 6c61 6e65 6f75 730a  # Miscellaneous.
-0000f5a0: 0a2a 2053 6576 6572 616c 2075 6e69 7420  .* Several unit 
-0000f5b0: 7465 7374 7320 616e 6420 696e 7465 6772  tests and integr
-0000f5c0: 6174 696f 6e20 7465 7374 7320 696d 7072  ation tests impr
-0000f5d0: 6f76 656d 656e 7473 2e0a 2a20 6043 6c69  ovements..* `Cli
-0000f5e0: 656e 7460 2063 6f6e 7374 7275 6374 6f72  ent` constructor
-0000f5f0: 206e 6f77 2065 6e66 6f72 6365 7320 7061   now enforces pa
-0000f600: 7373 696e 6720 7468 6520 6076 6572 7369  ssing the `versi
-0000f610: 6f6e 6020 7061 7261 6d65 7465 7220 6173  on` parameter as
-0000f620: 2061 0a20 2073 7472 696e 672e 0a2a 2042   a.  string..* B
-0000f630: 7569 6c64 2063 6f6e 7465 7874 2066 696c  uild context fil
-0000f640: 6573 2061 7265 206e 6f77 206f 7264 6572  es are now order
-0000f650: 6564 2062 7920 6669 6c65 6e61 6d65 2077  ed by filename w
-0000f660: 6865 6e20 6372 6561 7469 6e67 2074 6865  hen creating the
-0000f670: 2061 7263 6869 7665 0a20 2028 666f 7220   archive.  (for 
-0000f680: 636f 6e73 6973 7465 6e63 7920 7769 7468  consistency with
-0000f690: 2064 6f63 6b65 7220 6d61 696e 6c69 6e65   docker mainline
-0000f6a0: 2062 6568 6176 696f 7229 0a0a 302e 362e   behavior)..0.6.
-0000f6b0: 300a 2d2d 2d2d 2d0a 2a20 2a2a 5468 6973  0.-----.* **This
-0000f6c0: 2076 6572 7369 6f6e 2069 6e74 726f 6475   version introdu
-0000f6d0: 6365 7320 6272 6561 6b69 6e67 2063 6861  ces breaking cha
-0000f6e0: 6e67 6573 212a 2a0a 0a23 2323 2042 7265  nges!**..### Bre
-0000f6f0: 616b 696e 6720 6368 616e 6765 730a 0a2a  aking changes..*
-0000f700: 2054 6865 2064 6566 6175 6c74 2053 534c   The default SSL
-0000f710: 2070 726f 746f 636f 6c20 6973 206e 6f77   protocol is now
-0000f720: 2074 6865 2068 6967 6865 7374 2054 4c53   the highest TLS
-0000f730: 2076 312e 7820 2877 6173 2053 534c 2076   v1.x (was SSL v
-0000f740: 322e 3320 6265 666f 7265 290a 2020 2850  2.3 before).  (P
-0000f750: 6f6f 646c 6520 6669 7829 0a2a 2054 6865  oodle fix).* The
-0000f760: 2060 6869 7374 6f72 7960 2063 6f6d 6d61   `history` comma
-0000f770: 6e64 206e 6f77 2072 6574 7572 6e73 2061  nd now returns a
-0000f780: 2064 6963 7420 696e 7374 6561 6420 6f66   dict instead of
-0000f790: 2061 2072 6177 204a 534f 4e20 7374 7269   a raw JSON stri
-0000f7a0: 6e67 2e0a 0a23 2323 2046 6561 7475 7265  ng...### Feature
-0000f7b0: 730a 0a2a 2041 6464 6564 2074 6865 2060  s..* Added the `
-0000f7c0: 6578 6563 7574 6560 2063 6f6d 6d61 6e64  execute` command
-0000f7d0: 2e0a 2a20 4164 6465 6420 6070 6175 7365  ..* Added `pause
-0000f7e0: 6020 616e 6420 6075 6e70 6175 7365 6020  ` and `unpause` 
-0000f7f0: 636f 6d6d 616e 6473 2e0a 2a20 4164 6465  commands..* Adde
-0000f800: 6420 7375 7070 6f72 7420 666f 2074 6865  d support fo the
-0000f810: 2060 6370 7573 6574 6020 7061 7261 6d20   `cpuset` param 
-0000f820: 696e 2060 6372 6561 7465 5f63 6f6e 7461  in `create_conta
-0000f830: 696e 6572 600a 2a20 4164 6465 6420 7375  iner`.* Added su
-0000f840: 7070 6f72 7420 666f 7220 686f 7374 2064  pport for host d
-0000f850: 6576 6963 6573 2028 6064 6576 6963 6573  evices (`devices
-0000f860: 6020 7061 7261 6d20 696e 2060 7374 6172  ` param in `star
-0000f870: 7460 290a 2a20 4164 6465 6420 7375 7070  t`).* Added supp
-0000f880: 6f72 7420 666f 7220 7468 6520 6074 6169  ort for the `tai
-0000f890: 6c60 2070 6172 616d 2069 6e20 606c 6f67  l` param in `log
-0000f8a0: 7360 2e0a 2a20 4164 6465 6420 7375 7070  s`..* Added supp
-0000f8b0: 6f72 7420 666f 7220 7468 6520 6066 696c  ort for the `fil
-0000f8c0: 7465 7273 6020 7061 7261 6d20 696e 2060  ters` param in `
-0000f8d0: 696d 6167 6573 6020 616e 6420 6063 6f6e  images` and `con
-0000f8e0: 7461 696e 6572 7360 0a2a 2054 6865 2060  tainers`.* The `
-0000f8f0: 6b77 6172 6773 5f66 726f 6d5f 656e 7660  kwargs_from_env`
-0000f900: 206d 6574 686f 6420 6973 206e 6f77 2061   method is now a
-0000f910: 7661 696c 6162 6c65 2069 6e20 7468 6520  vailable in the 
-0000f920: 6064 6f63 6b65 722e 7574 696c 7360 0a20  `docker.utils`. 
-0000f930: 206d 6f64 756c 652e 2054 6869 7320 7368   module. This sh
-0000f940: 6f75 6c64 206d 616b 6520 6974 2065 6173  ould make it eas
-0000f950: 6965 7220 666f 7220 626f 6f74 3264 6f63  ier for boot2doc
-0000f960: 6b65 7220 7573 6572 2074 6f20 636f 6e6e  ker user to conn
-0000f970: 6563 740a 2020 746f 2074 6865 6972 2064  ect.  to their d
-0000f980: 6165 6d6f 6e2e 0a0a 2323 2320 4275 6766  aemon...### Bugf
-0000f990: 6978 6573 0a0a 2a20 4669 7865 6420 6120  ixes..* Fixed a 
-0000f9a0: 6275 6720 7768 6572 6520 656d 7074 7920  bug where empty 
-0000f9b0: 6469 7265 6374 6f72 6965 7320 7765 7265  directories were
-0000f9c0: 6e27 7420 636f 7272 6563 746c 7920 696e  n't correctly in
-0000f9d0: 636c 7564 6564 2077 6865 6e0a 2020 7072  cluded when.  pr
-0000f9e0: 6f76 6964 696e 6720 6120 636f 6e74 6578  oviding a contex
-0000f9f0: 7420 746f 2060 436c 6965 6e74 2e62 7569  t to `Client.bui
-0000fa00: 6c64 602e 0a2a 2046 6978 6564 2061 2062  ld`..* Fixed a b
-0000fa10: 7567 2077 6865 7265 2055 4e49 5820 736f  ug where UNIX so
-0000fa20: 636b 6574 2063 6f6e 6e65 6374 696f 6e73  cket connections
-0000fa30: 2077 6572 656e 2774 2070 726f 7065 726c   weren't properl
-0000fa40: 7920 636c 6561 6e65 6420 7570 2c0a 2020  y cleaned up,.  
-0000fa50: 6361 7573 696e 6720 6052 6573 6f75 7263  causing `Resourc
-0000fa60: 6557 6172 6e69 6e67 6073 2074 6f20 6170  eWarning`s to ap
-0000fa70: 7065 6172 2069 6e20 736f 6d65 2063 6173  pear in some cas
-0000fa80: 6573 2e0a 2a20 4669 7865 6420 6120 6275  es..* Fixed a bu
-0000fa90: 6720 7768 6572 6520 646f 636b 6572 2d70  g where docker-p
-0000faa0: 7920 776f 756c 6420 6372 6173 6820 6966  y would crash if
-0000fab0: 2074 6865 2064 6f63 6b65 7220 6461 656d   the docker daem
-0000fac0: 6f6e 2077 6173 2073 746f 7070 6564 0a20  on was stopped. 
-0000fad0: 2077 6869 6c65 2072 6561 6469 6e67 2061   while reading a
-0000fae0: 2073 7472 6561 6d69 6e67 2072 6573 706f   streaming respo
-0000faf0: 6e73 650a 2a20 4669 7865 6420 6120 6275  nse.* Fixed a bu
-0000fb00: 6720 7769 7468 2073 7472 6561 6d69 6e67  g with streaming
-0000fb10: 2072 6573 706f 6e73 6573 2069 6e20 5079   responses in Py
-0000fb20: 7468 6f6e 2033 0a2a 2060 7265 6d6f 7665  thon 3.* `remove
-0000fb30: 5f69 6d61 6765 6020 6e6f 7720 7375 7070  _image` now supp
-0000fb40: 6f72 7473 2061 2064 6963 7420 636f 6e74  orts a dict cont
-0000fb50: 6169 6e69 6e67 2061 6e20 6049 6460 206b  aining an `Id` k
-0000fb60: 6579 2061 7320 6974 7320 6069 6460 0a20  ey as its `id`. 
-0000fb70: 2070 6172 616d 6574 6572 2028 7369 6d69   parameter (simi
-0000fb80: 6c61 7220 746f 206f 7468 6572 206d 6574  lar to other met
-0000fb90: 686f 6473 2072 6571 7569 7269 6e67 2061  hods requiring a
-0000fba0: 2072 6573 6f75 7263 6520 4944 290a 0a23   resource ID)..#
-0000fbb0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-0000fbc0: 0a0a 2a20 4164 6465 6420 6e65 7720 4d6b  ..* Added new Mk
-0000fbd0: 446f 6373 2064 6f63 756d 656e 7461 7469  Docs documentati
-0000fbe0: 6f6e 2e20 4375 7272 656e 746c 7920 686f  on. Currently ho
-0000fbf0: 7374 6564 206f 6e0a 2020 5b52 6561 6454  sted on.  [ReadT
-0000fc00: 6865 446f 6373 5d28 6874 7470 733a 2f2f  heDocs](https://
-0000fc10: 646f 636b 6572 2d70 792e 7265 6164 7468  docker-py.readth
-0000fc20: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-0000fc30: 7374 2f29 0a0a 2323 2320 4d69 7363 656c  st/)..### Miscel
-0000fc40: 6c61 6e65 6f75 730a 0a2a 2041 6464 6564  laneous..* Added
-0000fc50: 2074 6573 7473 2074 6f20 7364 6973 740a   tests to sdist.
-0000fc60: 2a20 4164 6465 6420 6120 4d61 6b65 6669  * Added a Makefi
-0000fc70: 6c65 2066 6f72 2072 756e 6e69 6e67 2074  le for running t
-0000fc80: 6573 7473 2069 6e20 446f 636b 6572 0a2a  ests in Docker.*
-0000fc90: 2055 7064 6174 6564 2044 6f63 6b65 7266   Updated Dockerf
-0000fca0: 696c 650a 0a30 2e35 2e33 0a2d 2d2d 2d2d  ile..0.5.3.-----
-0000fcb0: 0a0a 2a20 4669 7865 6420 6174 7461 6368  ..* Fixed attach
-0000fcc0: 696e 6720 7768 656e 2063 6f6e 6e65 6374  ing when connect
-0000fcd0: 696e 6720 746f 2074 6865 2064 6165 6d6f  ing to the daemo
-0000fce0: 6e20 6f76 6572 2061 2055 4e49 5820 736f  n over a UNIX so
-0000fcf0: 636b 6574 2e0a 0a30 2e35 2e32 0a2d 2d2d  cket...0.5.2.---
-0000fd00: 2d2d 0a0a 2a20 4669 7865 6420 6120 6275  --..* Fixed a bu
-0000fd10: 6720 7768 6572 6520 736f 636b 6574 7320  g where sockets 
-0000fd20: 7765 7265 2063 6c6f 7365 6420 696d 6d65  were closed imme
-0000fd30: 6469 6174 656c 7920 7768 656e 2061 7474  diately when att
-0000fd40: 6163 6869 6e67 206f 7665 720a 2020 544c  aching over.  TL
-0000fd50: 532e 0a0a 302e 352e 310a 2d2d 2d2d 2d0a  S...0.5.1.-----.
-0000fd60: 0a2a 2041 6464 6564 2061 2060 6173 7365  .* Added a `asse
-0000fd70: 7274 5f68 6f73 746e 616d 6560 206f 7074  rt_hostname` opt
-0000fd80: 696f 6e20 746f 2060 544c 5343 6f6e 6669  ion to `TLSConfi
-0000fd90: 6760 2077 6869 6368 2063 616e 2062 6520  g` which can be 
-0000fda0: 7573 6564 2074 6f0a 2020 6469 7361 626c  used to.  disabl
-0000fdb0: 6520 7665 7269 6669 6361 7469 6f6e 206f  e verification o
-0000fdc0: 6620 686f 7374 6e61 6d65 732e 0a2a 2046  f hostnames..* F
-0000fdd0: 6978 6564 2053 534c 206e 6f74 2077 6f72  ixed SSL not wor
-0000fde0: 6b69 6e67 2064 7565 2074 6f20 616e 2069  king due to an i
-0000fdf0: 6e63 6f72 7265 6374 2076 6572 7369 6f6e  ncorrect version
-0000fe00: 2063 6f6d 7061 7269 736f 6e0a 2a20 4669   comparison.* Fi
-0000fe10: 7865 6420 7374 7265 616d 7320 6e6f 7420  xed streams not 
-0000fe20: 776f 726b 696e 6720 6f6e 2057 696e 646f  working on Windo
-0000fe30: 7773 0a0a 302e 352e 300a 2d2d 2d2d 2d0a  ws..0.5.0.-----.
-0000fe40: 0a2a 202a 2a54 6869 7320 7665 7273 696f  .* **This versio
-0000fe50: 6e20 696e 7472 6f64 7563 6573 2062 7265  n introduces bre
-0000fe60: 616b 696e 6720 6368 616e 6765 7321 2a2a  aking changes!**
-0000fe70: 0a2a 2041 6464 6564 2060 696e 7365 6375  .* Added `insecu
-0000fe80: 7265 5f72 6567 6973 7472 7960 2070 6172  re_registry` par
-0000fe90: 616d 6574 6572 2069 6e20 6043 6c69 656e  ameter in `Clien
-0000fea0: 742e 7075 7368 6020 616e 6420 6043 6c69  t.push` and `Cli
-0000feb0: 656e 742e 7075 6c6c 602e 0a20 202a 4974  ent.pull`..  *It
-0000fec0: 2064 6566 6175 6c74 7320 746f 2046 616c   defaults to Fal
-0000fed0: 7365 2061 6e64 2063 6f64 6520 7075 7368  se and code push
-0000fee0: 696e 6720 746f 206e 6f6e 2d48 5454 5053  ing to non-HTTPS
-0000fef0: 2070 7269 7661 7465 2072 6567 6973 7472   private registr
-0000ff00: 6965 730a 2020 6d69 6768 7420 6272 6561  ies.  might brea
-0000ff10: 6b20 6173 2061 2072 6573 756c 742e 2a0a  k as a result.*.
-0000ff20: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-0000ff30: 666f 7220 6164 6469 6e67 2061 6e64 2064  for adding and d
-0000ff40: 726f 7070 696e 6720 6361 7061 6269 6c69  ropping capabili
-0000ff50: 7469 6573 0a2a 2041 6464 6564 2073 7570  ties.* Added sup
-0000ff60: 706f 7274 2066 6f72 2072 6573 7461 7274  port for restart
-0000ff70: 2070 6f6c 6963 790a 2a20 4164 6465 6420   policy.* Added 
-0000ff80: 7375 7070 6f72 7420 666f 7220 7374 7269  support for stri
-0000ff90: 6e67 2076 616c 7565 7320 696e 2060 436c  ng values in `Cl
-0000ffa0: 6965 6e74 2e63 7265 6174 655f 636f 6e74  ient.create_cont
-0000ffb0: 6169 6e65 7260 2773 2060 6d65 6d5f 6c69  ainer`'s `mem_li
-0000ffc0: 6d69 7460 0a2a 2041 6464 6564 2073 7570  mit`.* Added sup
-0000ffd0: 706f 7274 2066 6f72 2060 2e64 6f63 6b65  port for `.docke
-0000ffe0: 7269 676e 6f72 6560 2066 696c 6520 696e  rignore` file in
-0000fff0: 2060 436c 6965 6e74 2e62 7569 6c64 600a   `Client.build`.
-00010000: 0a23 2323 2042 7567 6669 7865 730a 0a2a  .### Bugfixes..*
-00010010: 2046 6978 6564 2074 696d 656f 7574 2062   Fixed timeout b
-00010020: 6568 6176 696f 7220 696e 2060 436c 6965  ehavior in `Clie
-00010030: 6e74 2e73 746f 7060 0a0a 2323 2320 4d69  nt.stop`..### Mi
-00010040: 7363 656c 6c61 6e65 6f75 730a 0a2a 2060  scellaneous..* `
-00010050: 436c 6965 6e74 2e63 7265 6174 655f 636f  Client.create_co
-00010060: 6e74 6169 6e65 7260 2070 726f 7669 6465  ntainer` provide
-00010070: 7320 6265 7474 6572 2076 616c 6964 6174  s better validat
-00010080: 696f 6e20 6f66 2074 6865 2060 766f 6c75  ion of the `volu
-00010090: 6d65 7360 0a20 2070 6172 616d 6574 6572  mes`.  parameter
-000100a0: 0a2a 2049 6d70 726f 7665 6420 696e 7465  .* Improved inte
-000100b0: 6772 6174 696f 6e20 7465 7374 730a 0a30  gration tests..0
-000100c0: 2e34 2e30 0a2d 2d2d 2d2d 0a0a 2a20 2a2a  .4.0.-----..* **
-000100d0: 5468 6973 2076 6572 7369 6f6e 2069 6e74  This version int
-000100e0: 726f 6475 6365 7320 6272 6561 6b69 6e67  roduces breaking
-000100f0: 2063 6861 6e67 6573 212a 2a0a 2a20 5468   changes!**.* Th
-00010100: 6520 6062 6173 655f 7572 6c60 2070 6172  e `base_url` par
-00010110: 616d 6574 6572 2069 6e20 7468 6520 6043  ameter in the `C
-00010120: 6c69 656e 7460 2063 6f6e 7374 7275 6374  lient` construct
-00010130: 6f72 2073 686f 756c 6420 6e6f 7720 616c  or should now al
-00010140: 6c6f 7720 6d6f 7374 0a20 206f 6620 7468  low most.  of th
-00010150: 6520 6044 4f43 4b45 525f 484f 5354 6020  e `DOCKER_HOST` 
-00010160: 656e 7669 726f 6e6d 656e 7420 7661 6c75  environment valu
-00010170: 6573 2028 6578 6365 7074 2066 6f72 2074  es (except for t
-00010180: 6865 2066 643a 2f2f 2070 726f 746f 636f  he fd:// protoco
-00010190: 6c29 0a20 2020 202a 2041 7320 6120 7265  l).    * As a re
-000101a0: 7375 6c74 2c20 5552 4c73 2074 6861 7420  sult, URLs that 
-000101b0: 646f 6e27 7420 7370 6563 6966 7920 6120  don't specify a 
-000101c0: 706f 7274 2061 7265 206e 6f77 2069 6e76  port are now inv
-000101d0: 616c 6964 2028 7369 6d69 6c61 720a 2020  alid (similar.  
-000101e0: 2020 746f 2074 6865 206f 6666 6963 6961    to the officia
-000101f0: 6c20 636c 6965 6e74 2773 2062 6568 6176  l client's behav
-00010200: 696f 7229 0a2a 2041 6464 6564 2054 4c53  ior).* Added TLS
-00010210: 2073 7570 706f 7274 2028 7365 6520 5b64   support (see [d
-00010220: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00010230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00010240: 2f64 6f74 636c 6f75 642f 646f 636b 6572  /dotcloud/docker
-00010250: 2d70 7923 636f 6e6e 6563 7469 6f6e 2d74  -py#connection-t
-00010260: 6f2d 6461 656d 6f6e 2d75 7369 6e67 2d68  o-daemon-using-h
-00010270: 7474 7073 2929 0a0a 2323 2320 4275 6766  ttps))..### Bugf
-00010280: 6978 6573 0a0a 2a20 4669 7865 6420 616e  ixes..* Fixed an
-00010290: 2069 7373 7565 2077 6974 6820 6043 6c69   issue with `Cli
-000102a0: 656e 742e 6275 696c 6460 2073 7472 6561  ent.build` strea
-000102b0: 6d65 6420 6c6f 6773 2069 6e20 5079 7468  med logs in Pyth
-000102c0: 6f6e 2033 0a0a 2323 2320 4d69 7363 656c  on 3..### Miscel
-000102d0: 6c61 6e65 6f75 730a 0a2a 2041 6464 6564  laneous..* Added
-000102e0: 2075 6e69 7420 7465 7374 7320 636f 7665   unit tests cove
-000102f0: 7261 6765 0a2a 2056 6172 696f 7573 2069  rage.* Various i
-00010300: 6e74 6567 7261 7469 6f6e 2074 6573 7473  ntegration tests
-00010310: 2066 6978 6573 0a0a 302e 332e 320a 2d2d   fixes..0.3.2.--
-00010320: 2d2d 2d0a 0a2a 2044 6566 6175 6c74 2041  ---..* Default A
-00010330: 5049 2076 6572 7369 6f6e 2069 7320 6e6f  PI version is no
-00010340: 7720 312e 3132 2028 7375 7070 6f72 7420  w 1.12 (support 
-00010350: 666f 7220 646f 636b 6572 2031 2e30 290a  for docker 1.0).
-00010360: 2a20 4164 6465 6420 6e65 7720 6d65 7468  * Added new meth
-00010370: 6f64 7320 6043 6c69 656e 742e 6765 745f  ods `Client.get_
-00010380: 696d 6167 6560 2061 6e64 2060 436c 6965  image` and `Clie
-00010390: 6e74 2e6c 6f61 645f 696d 6167 6560 0a20  nt.load_image`. 
-000103a0: 2028 6064 6f63 6b65 7220 7361 7665 6020   (`docker save` 
-000103b0: 616e 6420 6064 6f63 6b65 7220 6c6f 6164  and `docker load
-000103c0: 6029 0a2a 2041 6464 6564 206e 6577 206d  `).* Added new m
-000103d0: 6574 686f 6420 6043 6c69 656e 742e 7069  ethod `Client.pi
-000103e0: 6e67 600a 2a20 4164 6465 6420 6e65 7720  ng`.* Added new 
-000103f0: 6d65 7468 6f64 2060 436c 6965 6e74 2e72  method `Client.r
-00010400: 6573 697a 6560 0a2a 2060 436c 6965 6e74  esize`.* `Client
-00010410: 2e62 7569 6c64 6020 6361 6e20 6e6f 7720  .build` can now 
-00010420: 6265 2070 726f 7669 6465 6420 7769 7468  be provided with
-00010430: 2061 2063 7573 746f 6d20 636f 6e74 6578   a custom contex
-00010440: 7420 7573 696e 6720 7468 650a 2020 6063  t using the.  `c
-00010450: 7573 746f 6d5f 636f 6e74 6578 7460 2070  ustom_context` p
-00010460: 6172 616d 6574 6572 2e0a 2a20 4164 6465  arameter..* Adde
-00010470: 6420 7375 7070 6f72 7420 666f 7220 606d  d support for `m
-00010480: 656d 7377 6170 5f6c 696d 6974 6020 7061  emswap_limit` pa
-00010490: 7261 6d65 7465 7220 696e 2060 6372 6561  rameter in `crea
-000104a0: 7465 5f63 6f6e 7461 696e 6572 600a 2a20  te_container`.* 
-000104b0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-000104c0: 7220 6066 6f72 6365 6020 7061 7261 6d65  r `force` parame
-000104d0: 7465 7220 696e 2060 7265 6d6f 7665 5f63  ter in `remove_c
-000104e0: 6f6e 7461 696e 6572 600a 2a20 4164 6465  ontainer`.* Adde
-000104f0: 6420 7375 7070 6f72 7420 666f 7220 6066  d support for `f
-00010500: 6f72 6365 6020 616e 6420 606e 6f70 7275  orce` and `nopru
-00010510: 6e65 6020 7061 7261 6d65 7465 7273 2069  ne` parameters i
-00010520: 6e20 6072 656d 6f76 655f 696d 6167 6560  n `remove_image`
-00010530: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-00010540: 2066 6f72 2060 7469 6d65 7374 616d 7073   for `timestamps
-00010550: 6020 7061 7261 6d65 7465 7220 696e 2060  ` parameter in `
-00010560: 6c6f 6773 600a 2a20 4164 6465 6420 7375  logs`.* Added su
-00010570: 7070 6f72 7420 666f 7220 6064 6e73 5f73  pport for `dns_s
-00010580: 6561 7263 6860 2070 6172 616d 6574 6572  earch` parameter
-00010590: 2069 6e20 6073 7461 7274 600a 2a20 4164   in `start`.* Ad
-000105a0: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
-000105b0: 606e 6574 776f 726b 5f6d 6f64 6560 2070  `network_mode` p
-000105c0: 6172 616d 6574 6572 2069 6e20 6073 7461  arameter in `sta
-000105d0: 7274 600a 2a20 4164 6465 6420 7375 7070  rt`.* Added supp
-000105e0: 6f72 7420 666f 7220 6073 697a 6560 2070  ort for `size` p
-000105f0: 6172 616d 6574 6572 2069 6e20 6063 6f6e  arameter in `con
-00010600: 7461 696e 6572 7360 0a2a 2041 6464 6564  tainers`.* Added
-00010610: 2073 7570 706f 7274 2066 6f72 2060 766f   support for `vo
-00010620: 6c75 6d65 735f 6672 6f6d 6020 616e 6420  lumes_from` and 
-00010630: 6064 6e73 6020 7061 7261 6d65 7465 7273  `dns` parameters
-00010640: 2069 6e20 6073 7461 7274 602e 2041 7320   in `start`. As 
-00010650: 6f66 0a20 2041 5049 2076 6572 7369 6f6e  of.  API version
-00010660: 203e 3d20 312e 3130 2c20 7468 6573 6520   >= 1.10, these 
-00010670: 7061 7261 6d65 7465 7273 206e 6f20 6c6f  parameters no lo
-00010680: 6e67 6572 2062 656c 6f6e 6720 746f 2060  nger belong to `
-00010690: 6372 6561 7465 5f63 6f6e 7461 696e 6572  create_container
-000106a0: 600a 2a20 6043 6c69 656e 742e 6c6f 6773  `.* `Client.logs
-000106b0: 6020 6e6f 7720 7573 6573 2074 6865 206c  ` now uses the l
-000106c0: 6f67 7320 656e 6470 6f69 6e74 2077 6865  ogs endpoint whe
-000106d0: 6e20 4150 4920 7665 7273 696f 6e20 6973  n API version is
-000106e0: 2073 7566 6669 6369 656e 740a 0a23 2323   sufficient..###
-000106f0: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
-00010700: 6564 2061 2062 7567 2069 6e20 7075 6c6c  ed a bug in pull
-00010710: 2077 6865 7265 2074 6865 2060 7265 706f   where the `repo
-00010720: 3a74 6167 6020 6e6f 7461 7469 6f6e 2077  :tag` notation w
-00010730: 6173 6e27 7420 696e 7465 7270 7265 7465  asn't interprete
-00010740: 640a 2020 7072 6f70 6572 6c79 0a2a 2046  d.  properly.* F
-00010750: 6978 6564 2061 2062 7567 2069 6e20 7374  ixed a bug in st
-00010760: 7265 616d 696e 6720 6d65 7468 6f64 7320  reaming methods 
-00010770: 7769 7468 2070 7974 686f 6e20 3320 2875  with python 3 (u
-00010780: 6e69 636f 6465 2c20 6279 7465 732f 7374  nicode, bytes/st
-00010790: 7220 7265 6c61 7465 6429 0a2a 2046 6978  r related).* Fix
-000107a0: 6564 2061 2062 7567 2069 6e20 6043 6c69  ed a bug in `Cli
-000107b0: 656e 742e 7374 6172 7460 2077 6865 7265  ent.start` where
-000107c0: 206c 6567 6163 7920 6e6f 7461 7469 6f6e   legacy notation
-000107d0: 2066 6f72 2076 6f6c 756d 6573 2077 6173   for volumes was
-000107e0: 6e27 740a 2020 7375 7070 6f72 7465 6420  n't.  supported 
-000107f0: 616e 796d 6f72 652e 0a0a 2323 2320 4d69  anymore...### Mi
-00010800: 7363 656c 6c61 6e65 6f75 730a 0a2a 2054  scellaneous..* T
-00010810: 6865 2063 6c69 656e 7420 6e6f 7720 7261  he client now ra
-00010820: 6973 6573 2060 446f 636b 6572 4578 6365  ises `DockerExce
-00010830: 7074 696f 6e60 7320 7768 656e 2061 7070  ption`s when app
-00010840: 726f 7072 6961 7465 2e20 596f 7520 6361  ropriate. You ca
-00010850: 6e20 696d 706f 7274 0a20 2060 446f 636b  n import.  `Dock
-00010860: 6572 4578 6365 7074 696f 6e60 2028 616e  erException` (an
-00010870: 6420 6974 7320 7375 6263 6c61 7373 6573  d its subclasses
-00010880: 2920 6672 6f6d 2074 6865 2060 646f 636b  ) from the `dock
-00010890: 6572 2e65 7272 6f72 7360 206d 6f64 756c  er.errors` modul
-000108a0: 6520 746f 0a20 2063 6174 6368 2074 6865  e to.  catch the
-000108b0: 6d20 6966 206e 6565 6465 642e 0a2a 2060  m if needed..* `
-000108c0: 646f 636b 6572 2e41 5049 4572 726f 7260  docker.APIError`
-000108d0: 2068 6173 2062 6565 6e20 6d6f 7665 6420   has been moved 
-000108e0: 746f 2074 6865 206e 6577 2060 646f 636b  to the new `dock
-000108f0: 6572 2e65 7272 6f72 7360 206d 6f64 756c  er.errors` modul
-00010900: 6520 6173 2077 656c 6c2e 0a2a 2060 436c  e as well..* `Cl
-00010910: 6965 6e74 2e69 6e73 6572 7460 2069 7320  ient.insert` is 
-00010920: 6465 7072 6563 6174 6564 2069 6e20 4150  deprecated in AP
-00010930: 4920 7665 7273 696f 6e20 3e20 312e 3131  I version > 1.11
-00010940: 0a2a 2049 6d70 726f 7665 6420 696e 7465  .* Improved inte
-00010950: 6772 6174 696f 6e20 7465 7374 7320 7368  gration tests sh
-00010960: 6f75 6c64 206e 6f77 2072 756e 206d 7563  ould now run muc
-00010970: 6820 6661 7374 6572 2e0a 2a20 5468 6572  h faster..* Ther
-00010980: 6520 6973 206e 6f77 2061 2073 696e 676c  e is now a singl
-00010990: 6520 736f 7572 6365 206f 6620 7472 7574  e source of trut
-000109a0: 6820 666f 7220 7468 6520 646f 636b 6572  h for the docker
-000109b0: 2d70 7920 7665 7273 696f 6e20 6e75 6d62  -py version numb
-000109c0: 6572 2e0a 0a30 2e33 2e31 0a2d 2d2d 2d2d  er...0.3.1.-----
-000109d0: 0a0a 2a20 4465 6661 756c 7420 4150 4920  ..* Default API 
-000109e0: 7665 7273 696f 6e20 6973 206e 6f77 2031  version is now 1
-000109f0: 2e39 0a2a 2053 7472 6561 6d69 6e67 2072  .9.* Streaming r
-00010a00: 6573 706f 6e73 6573 206e 6f20 6c6f 6e67  esponses no long
-00010a10: 6572 2079 6965 6c64 2062 6c61 6e6b 206c  er yield blank l
-00010a20: 696e 6573 2e0a 2a20 6043 6c69 656e 742e  ines..* `Client.
-00010a30: 6372 6561 7465 5f63 6f6e 7461 696e 6572  create_container
-00010a40: 6020 6e6f 7720 7375 7070 6f72 7473 2074  ` now supports t
-00010a50: 6865 2060 646f 6d61 696e 6e61 6d65 6020  he `domainname` 
-00010a60: 7061 7261 6d65 7465 722e 0a2a 2060 766f  parameter..* `vo
-00010a70: 6c75 6d65 735f 6672 6f6d 6020 7061 7261  lumes_from` para
-00010a80: 6d65 7465 7220 696e 2060 436c 6965 6e74  meter in `Client
-00010a90: 2e63 7265 6174 655f 636f 6e74 6169 6e65  .create_containe
-00010aa0: 7260 206e 6f77 2073 7570 706f 7274 730a  r` now supports.
-00010ab0: 2020 6974 6572 6162 6c65 732e 0a2a 2041    iterables..* A
-00010ac0: 7574 6820 6372 6564 656e 7469 616c 7320  uth credentials 
-00010ad0: 6172 6520 7072 6f76 6964 6564 2074 6f20  are provided to 
-00010ae0: 7468 6520 646f 636b 6572 2064 6165 6d6f  the docker daemo
-00010af0: 6e20 7768 656e 2075 7369 6e67 2060 436c  n when using `Cl
-00010b00: 6965 6e74 2e62 7569 6c64 600a 2020 286e  ient.build`.  (n
-00010b10: 6577 2066 6561 7475 7265 2069 6e20 4150  ew feature in AP
-00010b20: 4920 7665 7273 696f 6e20 312e 3929 0a0a  I version 1.9)..
-00010b30: 0a23 2323 2042 7567 6669 7865 730a 0a2a  .### Bugfixes..*
-00010b40: 2056 6172 696f 7573 2066 6978 6573 2066   Various fixes f
-00010b50: 6f72 2072 6573 706f 6e73 6520 7374 7265  or response stre
-00010b60: 616d 7320 2860 6c6f 6773 602c 2060 7075  ams (`logs`, `pu
-00010b70: 6c6c 602c 2065 7463 2e29 2e0a 2a20 4669  ll`, etc.)..* Fi
-00010b80: 7865 6420 6120 6275 6720 7769 7468 2060  xed a bug with `
-00010b90: 436c 6965 6e74 2e70 7573 6860 2077 6865  Client.push` whe
-00010ba0: 6e20 7573 696e 6720 4150 4920 7665 7273  n using API vers
-00010bb0: 696f 6e20 3c20 312e 350a 2a20 4669 7865  ion < 1.5.* Fixe
-00010bc0: 6420 6120 6275 6720 7769 7468 2041 5049  d a bug with API
-00010bd0: 2076 6572 7369 6f6e 2063 6865 636b 732e   version checks.
-00010be0: 0a0a 2323 2320 4d69 7363 656c 6c61 6e65  ..### Miscellane
-00010bf0: 6f75 730a 0a2a 2060 6d6f 636b 6020 6861  ous..* `mock` ha
-00010c00: 7320 6265 656e 2072 656d 6f76 6564 2066  s been removed f
-00010c10: 726f 6d20 7468 6520 7275 6e74 696d 6520  rom the runtime 
-00010c20: 7265 7175 6972 656d 656e 7473 2e0a 2a20  requirements..* 
-00010c30: 4164 6465 6420 696e 7374 616c 6c61 7469  Added installati
-00010c40: 6f6e 2069 6e73 7472 7563 7469 6f6e 7320  on instructions 
-00010c50: 696e 2074 6865 2052 4541 444d 452e 0a0a  in the README...
-00010c60: 302e 332e 300a 2d2d 2d2d 2d0a 0a2a 202a  0.3.0.-----..* *
-00010c70: 2a54 6869 7320 7665 7273 696f 6e20 696e  *This version in
-00010c80: 7472 6f64 7563 6573 2062 7265 616b 696e  troduces breakin
-00010c90: 6720 6368 616e 6765 7321 2a2a 0a2a 2053  g changes!**.* S
-00010ca0: 7570 706f 7274 2066 6f72 2041 5049 2076  upport for API v
-00010cb0: 6572 7369 6f6e 2031 2e37 2074 6872 6f75  ersion 1.7 throu
-00010cc0: 6768 2031 2e39 2028 446f 636b 6572 2030  gh 1.9 (Docker 0
-00010cd0: 2e38 2e30 2b29 0a2a 2044 6566 6175 6c74  .8.0+).* Default
-00010ce0: 2041 5049 2076 6572 7369 6f6e 2069 7320   API version is 
-00010cf0: 6e6f 7720 312e 380a 2a20 5468 6520 636c  now 1.8.* The cl
-00010d00: 6965 6e74 2068 6173 2062 6565 6e20 7570  ient has been up
-00010d10: 6461 7465 6420 746f 2073 7570 706f 7274  dated to support
-00010d20: 2052 6571 7565 7374 7320 322e 782e 2060   Requests 2.x. `
-00010d30: 7265 7175 6573 7473 3d3d 322e 322e 3160  requests==2.2.1`
-00010d40: 0a20 2069 7320 6e6f 7720 7468 6520 7265  .  is now the re
-00010d50: 636f 6d6d 656e 6465 6420 7665 7273 696f  commended versio
-00010d60: 6e2e 0a2a 204c 696e 6b73 2063 616e 206e  n..* Links can n
-00010d70: 6f77 2062 6520 7370 6563 6966 6965 6420  ow be specified 
-00010d80: 6173 2074 7570 6c65 7320 696e 2060 436c  as tuples in `Cl
-00010d90: 6965 6e74 2e73 7461 7274 6020 2873 6565  ient.start` (see
-00010da0: 2064 6f63 7320 666f 720a 2020 6d6f 7265   docs for.  more
-00010db0: 2069 6e66 6f72 6d61 7469 6f6e 290a 2a20   information).* 
-00010dc0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
-00010dd0: 7220 7661 7269 6f75 7320 6f70 7469 6f6e  r various option
-00010de0: 7320 696e 2060 436c 6965 6e74 2e63 7265  s in `Client.cre
-00010df0: 6174 655f 636f 6e74 6169 6e65 7260 0a20  ate_container`. 
-00010e00: 2028 606e 6574 776f 726b 5f64 6973 6162   (`network_disab
-00010e10: 6c65 6460 2c20 6063 7075 5f73 6861 7265  led`, `cpu_share
-00010e20: 7360 2c20 6077 6f72 6b69 6e67 5f64 6972  s`, `working_dir
-00010e30: 6020 616e 6420 6065 6e74 7279 706f 696e  ` and `entrypoin
-00010e40: 7460 290a 2a20 6043 6c69 656e 742e 6174  t`).* `Client.at
-00010e50: 7461 6368 6020 6861 7320 6265 656e 2072  tach` has been r
-00010e60: 6577 6f72 6b65 6420 746f 2077 6f72 6b20  eworked to work 
-00010e70: 7369 6d69 6c61 726c 7920 746f 2060 436c  similarly to `Cl
-00010e80: 6965 6e74 2e6c 6f67 7360 0a20 206d 696e  ient.logs`.  min
-00010e90: 7573 2074 6865 2068 6973 746f 7269 6361  us the historica
-00010ea0: 6c20 6461 7461 2e0a 2a20 4c6f 6773 2063  l data..* Logs c
-00010eb0: 616e 206e 6f77 2062 6520 7374 7265 616d  an now be stream
-00010ec0: 6564 2075 7369 6e67 2074 6865 2060 7374  ed using the `st
-00010ed0: 7265 616d 6020 7061 7261 6d65 7465 722e  ream` parameter.
-00010ee0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
-00010ef0: 2066 6f72 2060 7463 703a 2f2f 6020 5552   for `tcp://` UR
-00010f00: 4c73 2061 7320 636c 6965 6e74 2060 6261  Ls as client `ba
-00010f10: 7365 5f75 726c 602e 0a2a 2056 6172 696f  se_url`..* Vario
-00010f20: 7573 2061 7574 6820 696d 7072 6f76 656d  us auth improvem
-00010f30: 656e 7473 2e0a 2a20 4164 6465 6420 7375  ents..* Added su
-00010f40: 7070 6f72 7420 666f 7220 6375 7374 6f6d  pport for custom
-00010f50: 2060 436c 6965 6e74 2e62 7569 6c64 6020   `Client.build` 
-00010f60: 7469 6d65 6f75 742e 0a0a 0a23 2323 2042  timeout....### B
-00010f70: 7567 6669 7865 730a 0a2a 2046 6978 6564  ugfixes..* Fixed
-00010f80: 2061 2062 7567 2077 6865 7265 2064 6574   a bug where det
-00010f90: 6572 6d69 6e69 6e67 2074 6865 2070 726f  ermining the pro
-00010fa0: 746f 636f 6c20 6f66 2061 2070 7269 7661  tocol of a priva
-00010fb0: 7465 2072 6567 6973 7472 790a 2020 776f  te registry.  wo
-00010fc0: 756c 6420 736f 6d65 7469 6d65 7320 7969  uld sometimes yi
-00010fd0: 656c 6420 7468 6520 7772 6f6e 6720 7265  eld the wrong re
-00010fe0: 7375 6c74 2e0a 2a20 4669 7865 6420 6120  sult..* Fixed a 
-00010ff0: 6275 6720 7768 6572 6520 6043 6c69 656e  bug where `Clien
-00011000: 742e 636f 7079 6020 776f 756c 646e 2774  t.copy` wouldn't
-00011010: 2061 6363 6570 7420 6120 6469 6374 2061   accept a dict a
-00011020: 7320 6172 6775 6d65 6e74 2e0a 2a20 4669  s argument..* Fi
-00011030: 7865 6420 7365 7665 7261 6c20 7374 7265  xed several stre
-00011040: 616d 696e 6720 6275 6773 2e0a 2a20 5265  aming bugs..* Re
-00011050: 6d6f 7665 6420 756e 7573 6564 2070 6172  moved unused par
-00011060: 616d 6574 6572 2069 6e20 6043 6c69 656e  ameter in `Clien
-00011070: 742e 696d 706f 7274 5f69 6d61 6765 602e  t.import_image`.
-00011080: 0a2a 2054 6865 2063 6c69 656e 7427 7320  .* The client's 
-00011090: 6062 6173 655f 7572 6c60 206e 6f77 2074  `base_url` now t
-000110a0: 6f6c 6572 6174 6573 2074 7261 696c 696e  olerates trailin
-000110b0: 6720 736c 6173 6865 732e 0a0a 2323 2323  g slashes...####
-000110c0: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
-000110d0: 2a20 5570 6461 7465 6420 696e 7465 6772  * Updated integr
-000110e0: 6174 696f 6e20 7465 7374 730a 2a20 536d  ation tests.* Sm
-000110f0: 616c 6c20 646f 6320 6669 7865 730a 0a30  all doc fixes..0
-00011100: 2e32 2e33 0a2d 2d2d 2d2d 0a0a 2a20 5375  .2.3.-----..* Su
-00011110: 7070 6f72 7420 666f 7220 4150 4920 7665  pport for API ve
-00011120: 7273 696f 6e20 312e 360a 2a20 4164 6465  rsion 1.6.* Adde
-00011130: 6420 7375 7070 6f72 7420 666f 7220 6c69  d support for li
-00011140: 6e6b 730a 2a20 4164 6465 6420 7375 7070  nks.* Added supp
-00011150: 6f72 7420 666f 7220 676c 6f62 616c 2072  ort for global r
-00011160: 6571 7565 7374 2074 696d 656f 7574 0a2a  equest timeout.*
-00011170: 2041 6464 6564 2060 7369 676e 616c 6020   Added `signal` 
-00011180: 7061 7261 6d65 7465 7220 696e 2060 436c  parameter in `Cl
-00011190: 6965 6e74 2e6b 696c 6c60 0a2a 2041 6464  ient.kill`.* Add
-000111a0: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
-000111b0: 7075 626c 6973 685f 616c 6c5f 706f 7274  publish_all_port
-000111c0: 7360 2069 6e20 6043 6c69 656e 742e 7374  s` in `Client.st
-000111d0: 6172 7460 0a2a 2060 436c 6965 6e74 2e70  art`.* `Client.p
-000111e0: 756c 6c60 2c20 6043 6c69 656e 742e 7075  ull`, `Client.pu
-000111f0: 7368 6020 616e 6420 6043 6c69 656e 742e  sh` and `Client.
-00011200: 6275 696c 6460 2063 616e 2062 6520 7374  build` can be st
-00011210: 7265 616d 6564 206e 6f77 0a2a 2041 6464  reamed now.* Add
-00011220: 6564 2073 7570 706f 7274 2066 6f72 2077  ed support for w
-00011230: 6562 736f 636b 6574 7320 696e 2060 436c  ebsockets in `Cl
-00011240: 6965 6e74 2e61 7474 6163 6860 0a2a 2046  ient.attach`.* F
-00011250: 6978 6564 2070 6f72 7473 2066 6f72 2044  ixed ports for D
-00011260: 6f63 6b65 7220 302e 362e 352b 0a2a 2041  ocker 0.6.5+.* A
-00011270: 6464 6564 2060 436c 6965 6e74 2e65 7665  dded `Client.eve
-00011280: 6e74 7360 206d 6574 686f 6420 2861 6363  nts` method (acc
-00011290: 6573 7320 746f 2074 6865 2060 2f65 7665  ess to the `/eve
-000112a0: 6e74 7360 2065 6e64 706f 696e 7429 0a2a  nts` endpoint).*
-000112b0: 2043 6861 6e67 6564 2074 6865 2077 6179   Changed the way
-000112c0: 2074 6865 2070 6f72 7473 2061 6e64 2076   the ports and v
-000112d0: 6f6c 756d 6573 2061 7265 2070 726f 7669  olumes are provi
-000112e0: 6465 6420 696e 2060 436c 6965 6e74 2e73  ded in `Client.s
-000112f0: 7461 7274 6020 616e 640a 2020 6043 6c69  tart` and.  `Cli
-00011300: 656e 742e 6372 6561 7465 5f63 6f6e 7461  ent.create_conta
-00011310: 696e 6572 cc80 6020 746f 206d 616b 6520  iner..` to make 
-00011320: 7468 656d 2073 696d 706c 6572 2061 6e64  them simpler and
-00011330: 206d 6f72 6520 696e 7475 6974 6976 652e   more intuitive.
-00011340: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
-00011350: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
-00011360: 6572 6520 7072 6976 6174 6520 7265 6769  ere private regi
-00011370: 7374 7269 6573 206f 6e20 4854 5450 5320  stries on HTTPS 
-00011380: 7765 7265 6e27 7420 6861 6e64 6c65 6420  weren't handled 
-00011390: 7072 6f70 6572 6c79 0a2a 2046 6978 6564  properly.* Fixed
-000113a0: 2061 2062 7567 2077 6865 7265 2061 7574   a bug where aut
-000113b0: 6820 776f 756c 6420 6272 6561 6b20 7769  h would break wi
-000113c0: 7468 2050 7974 686f 6e20 330a 0a23 2323  th Python 3..###
-000113d0: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
-000113e0: 2a20 5465 7374 2069 6d70 726f 7665 6d65  * Test improveme
-000113f0: 6e74 730a 2a20 536c 6967 6874 2064 6f63  nts.* Slight doc
-00011400: 2069 6d70 726f 7665 6d65 6e74 730a 0a0a   improvements...
-00011410: 302e 322e 320a 2d2d 2d2d 2d0a 0a2a 2041  0.2.2.-----..* A
-00011420: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
-00011430: 2074 6865 2060 726d 6020 7061 7261 6d65   the `rm` parame
-00011440: 7465 7220 696e 2060 436c 6965 6e74 2e62  ter in `Client.b
-00011450: 7569 6c64 600a 2a20 4164 6465 6420 7375  uild`.* Added su
-00011460: 7070 6f72 7420 666f 7220 7461 7262 616c  pport for tarbal
-00011470: 6c20 696d 706f 7274 7320 696e 2060 436c  l imports in `Cl
-00011480: 6965 6e74 2e69 6d70 6f72 745f 696d 6167  ient.import_imag
-00011490: 6560 2074 6872 6f75 6768 2060 6461 7461  e` through `data
-000114a0: 600a 2020 7061 7261 6d65 7465 722e 0a2a  `.  parameter..*
-000114b0: 2054 6865 2060 636f 6d6d 616e 6460 2070   The `command` p
-000114c0: 6172 616d 6574 6572 2069 6e20 6043 6c69  arameter in `Cli
-000114d0: 656e 742e 6372 6561 7465 5f63 6f6e 7461  ent.create_conta
-000114e0: 696e 6572 6020 6973 206e 6f77 206f 7074  iner` is now opt
-000114f0: 696f 6e61 6c20 2866 6f72 0a20 2063 6f6e  ional (for.  con
-00011500: 7461 696e 6572 7320 7468 6174 2069 6e63  tainers that inc
-00011510: 6c75 6465 2061 2064 6566 6175 6c74 2072  lude a default r
-00011520: 756e 2063 6f6d 6d61 6e64 290a 0a23 2323  un command)..###
-00011530: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
-00011540: 6564 2050 7974 686f 6e20 3320 7375 7070  ed Python 3 supp
-00011550: 6f72 740a 2a20 4669 7865 6420 6120 6275  ort.* Fixed a bu
-00011560: 6720 7768 6572 6520 616e 6f6e 796d 6f75  g where anonymou
-00011570: 7320 7075 7368 2f70 756c 6c20 776f 756c  s push/pull woul
-00011580: 6420 6272 6561 6b20 7768 656e 206e 6f20  d break when no 
-00011590: 6175 7468 636f 6e66 6967 2069 730a 2020  authconfig is.  
-000115a0: 7072 6573 656e 740a 2a20 4669 7865 6420  present.* Fixed 
-000115b0: 6120 6275 6720 7768 6572 6520 7468 6520  a bug where the 
-000115c0: 6071 7569 6574 6020 7061 7261 6d65 7465  `quiet` paramete
-000115d0: 7220 776f 756c 646e 2774 2062 6520 7461  r wouldn't be ta
-000115e0: 6b65 6e20 696e 746f 2061 6363 6f75 6e74  ken into account
-000115f0: 2069 6e0a 2020 6043 6c69 656e 742e 636f   in.  `Client.co
-00011600: 6e74 6169 6e65 7273 600a 2a20 4669 7865  ntainers`.* Fixe
-00011610: 6420 6120 6275 6720 7768 6572 6520 6043  d a bug where `C
-00011620: 6c69 656e 742e 7075 7368 6020 776f 756c  lient.push` woul
-00011630: 6420 6272 6561 6b20 7768 656e 2070 7573  d break when pus
-00011640: 6869 6e67 2074 6f20 7072 6976 6174 650a  hing to private.
-00011650: 2020 7265 6769 7374 7269 6573 2e0a 2a20    registries..* 
-00011660: 5265 6d6f 7665 6420 756e 7573 6564 2060  Removed unused `
-00011670: 7265 6769 7374 7279 6020 7061 7261 6d65  registry` parame
-00011680: 7465 7220 696e 2060 436c 6965 6e74 2e70  ter in `Client.p
-00011690: 756c 6c60 2e0a 2a20 5265 6d6f 7665 6420  ull`..* Removed 
-000116a0: 6f62 736f 6c65 7465 2063 7573 746f 6d20  obsolete custom 
-000116b0: 6572 726f 7220 6d65 7373 6167 6520 696e  error message in
-000116c0: 2060 436c 6965 6e74 2e63 7265 6174 655f   `Client.create_
-000116d0: 636f 6e74 6169 6e65 7260 2e0a 0a23 2323  container`...###
-000116e0: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
-000116f0: 2a20 646f 636b 6572 2d70 7920 6973 206e  * docker-py is n
-00011700: 6f77 2075 6e69 742d 7465 7374 6564 2c20  ow unit-tested, 
-00011710: 616e 6420 5472 6176 6973 2d43 4920 6861  and Travis-CI ha
-00011720: 7320 6265 656e 2065 6e61 626c 6564 206f  s been enabled o
-00011730: 6e20 7468 650a 2020 736f 7572 6365 2072  n the.  source r
-00011740: 6570 6f73 6974 6f72 792e 0a0a 302e 322e  epository...0.2.
-00011750: 310a 2d2d 2d2d 2d0a 0a2a 2049 6d70 726f  1.-----..* Impro
-00011760: 7665 6d65 6e74 7320 746f 2074 6865 2060  vements to the `
-00011770: 746f 782e 696e 6960 2066 696c 650a 0a23  tox.ini` file..#
-00011780: 2323 2042 7567 6669 7865 730a 0a2a 2046  ## Bugfixes..* F
-00011790: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
-000117a0: 2074 6865 2070 6163 6b61 6765 2077 6f75   the package wou
-000117b0: 6c64 2066 6169 6c20 7769 7468 2061 6e20  ld fail with an 
-000117c0: 6049 6d70 6f72 7445 7272 6f72 6020 6966  `ImportError` if
-000117d0: 2072 6571 7565 7374 730a 2020 7761 7320   requests.  was 
-000117e0: 696e 7374 616c 6c65 6420 7573 696e 6720  installed using 
-000117f0: 6061 7074 2d67 6574 600a 2a20 4669 7865  `apt-get`.* Fixe
-00011800: 6420 6120 6275 6720 7768 6572 6520 6043  d a bug where `C
-00011810: 6c69 656e 742e 6275 696c 6460 2077 6f75  lient.build` wou
-00011820: 6c64 2066 6169 6c20 6966 2067 6976 656e  ld fail if given
-00011830: 2061 2060 7061 7468 6020 7061 7261 6d65   a `path` parame
-00011840: 7465 722e 0a2a 2046 6978 6564 2073 6576  ter..* Fixed sev
-00011850: 6572 616c 2062 7567 7320 696e 2060 436c  eral bugs in `Cl
-00011860: 6965 6e74 2e6c 6f67 696e 602e 2049 7420  ient.login`. It 
-00011870: 7368 6f75 6c64 206e 6f77 2077 6f72 6b20  should now work 
-00011880: 7769 7468 2041 5049 2076 6572 7369 6f6e  with API version
-00011890: 730a 2020 312e 342c 2031 2e35 2e0a 2a20  s.  1.4, 1.5..* 
-000118a0: 506c 6561 7365 206e 6f74 6520 7468 6174  Please note that
-000118b0: 2060 436c 6965 6e74 2e6c 6f67 696e 6020   `Client.login` 
-000118c0: 6375 7272 656e 746c 7920 646f 6573 6e27  currently doesn'
-000118d0: 7420 7772 6974 6520 6175 7468 2074 6f20  t write auth to 
-000118e0: 7468 650a 2020 602e 646f 636b 6572 6366  the.  `.dockercf
-000118f0: 6760 2066 696c 652c 2074 6875 7320 2a2a  g` file, thus **
-00011900: 6175 7468 2069 7320 6e6f 7420 7065 7273  auth is not pers
-00011910: 6973 7465 6e74 2077 6865 6e20 7573 696e  istent when usin
-00011920: 6720 7468 6973 206d 6574 686f 642e 2a2a  g this method.**
-00011930: 0a0a 302e 322e 300a 2d2d 2d2d 2d0a 0a2a  ..0.2.0.-----..*
-00011940: 202a 2a54 6869 7320 7665 7273 696f 6e20   **This version 
-00011950: 696e 7472 6f64 7563 6573 2062 7265 616b  introduces break
-00011960: 696e 6720 6368 616e 6765 7321 2a2a 0a2a  ing changes!**.*
-00011970: 2060 436c 6965 6e74 2e6b 696c 6c60 2c20   `Client.kill`, 
-00011980: 6043 6c69 656e 742e 7265 6d6f 7665 5f63  `Client.remove_c
-00011990: 6f6e 7461 696e 6572 602c 2060 436c 6965  ontainer`, `Clie
-000119a0: 6e74 2e72 656d 6f76 655f 696d 6167 6560  nt.remove_image`
-000119b0: 2c0a 6043 6c69 656e 742e 7265 7374 6172  ,.`Client.restar
-000119c0: 7460 2c20 6043 6c69 656e 742e 7374 6172  t`, `Client.star
-000119d0: 7460 2c20 6043 6c69 656e 742e 7374 6f70  t`, `Client.stop
-000119e0: 6020 616e 6420 6043 6c69 656e 742e 7761  ` and `Client.wa
-000119f0: 6974 6020 646f 6e27 7420 7375 7070 6f72  it` don't suppor
-00011a00: 740a 7661 7261 7267 7320 616e 796d 6f72  t.varargs anymor
-00011a10: 652e 0a2a 2041 6464 6564 2063 6f6d 6d61  e..* Added comma
-00011a20: 6e64 7320 6043 6c69 656e 742e 746f 7060  nds `Client.top`
-00011a30: 2061 6e64 2060 436c 6965 6e74 2e63 6f70   and `Client.cop
-00011a40: 7960 0a2a 2041 6464 6564 2060 6c78 635f  y`.* Added `lxc_
-00011a50: 636f 6e66 6020 7061 7261 6d65 7465 7220  conf` parameter 
-00011a60: 746f 2060 436c 6965 6e74 2e73 7461 7274  to `Client.start
-00011a70: 600a 2a20 4164 6465 6420 7375 7070 6f72  `.* Added suppor
-00011a80: 7420 666f 7220 6175 7468 656e 7469 6361  t for authentica
-00011a90: 7469 6f6e 2069 6e20 6043 6c69 656e 742e  tion in `Client.
-00011aa0: 7075 6c6c 6020 2841 5049 2076 6572 7369  pull` (API versi
-00011ab0: 6f6e 203e 3d31 2e35 290a 2a20 4164 6465  on >=1.5).* Adde
-00011ac0: 6420 7375 7070 6f72 7420 666f 7220 7072  d support for pr
-00011ad0: 6976 696c 6567 6564 2063 6f6e 7461 696e  ivileged contain
-00011ae0: 6572 732e 0a2a 2045 7272 6f72 206d 616e  ers..* Error man
-00011af0: 6167 656d 656e 7420 6f76 6572 6861 756c  agement overhaul
-00011b00: 2e20 5468 6520 6e65 7720 7665 7273 696f  . The new versio
-00011b10: 6e20 7368 6f75 6c64 2062 6520 6d6f 7265  n should be more
-00011b20: 2063 6f6e 7369 7374 656e 7420 616e 640a   consistent and.
-00011b30: 2a20 416c 6c20 6d65 7468 6f64 7320 7468  * All methods th
-00011b40: 6174 2065 7870 6563 7465 6420 6120 636f  at expected a co
-00011b50: 6e74 6169 6e65 7220 4944 2061 7320 6172  ntainer ID as ar
-00011b60: 6775 6d65 6e74 206e 6f77 2061 6c73 6f20  gument now also 
-00011b70: 7375 7070 6f72 7420 6120 6469 6374 0a63  support a dict.c
-00011b80: 6f6e 7461 696e 696e 6720 616e 2060 4964  ontaining an `Id
-00011b90: 6020 6b65 792e 0a2a 2041 6464 6564 206c  ` key..* Added l
-00011ba0: 6963 656e 7365 2068 6561 6465 7220 746f  icense header to
-00011bb0: 2070 7974 686f 6e20 6669 6c65 732e 0a2a   python files..*
-00011bc0: 2053 6576 6572 616c 2060 5245 4144 4d45   Several `README
-00011bd0: 2e6d 6460 2075 7064 6174 6573 2e0a 0a23  .md` updates...#
-00011be0: 2323 2042 7567 6669 7865 730a 0a2a 2046  ## Bugfixes..* F
-00011bf0: 6978 6564 2073 6576 6572 616c 2062 7567  ixed several bug
-00011c00: 7320 7769 7468 2061 7574 6820 636f 6e66  s with auth conf
-00011c10: 6967 2070 6172 7369 6e67 2e0a 2a20 4669  ig parsing..* Fi
-00011c20: 7865 6420 6120 6275 6720 696e 2060 436c  xed a bug in `Cl
-00011c30: 6965 6e74 2e70 7573 6860 2077 6865 7265  ient.push` where
-00011c40: 2069 7420 776f 756c 6420 7261 6973 6520   it would raise 
-00011c50: 616e 2065 7863 6570 7469 6f6e 2069 660a  an exception if.
-00011c60: 7468 6520 6175 7468 2063 6f6e 6669 6720  the auth config 
-00011c70: 7761 736e 2774 206c 6f61 6465 642e 0a2a  wasn't loaded..*
-00011c80: 2046 6978 6564 2061 2062 7567 2069 6e20   Fixed a bug in 
-00011c90: 6043 6c69 656e 742e 7075 6c6c 6020 7768  `Client.pull` wh
-00011ca0: 6572 6520 7072 6976 6174 6520 7265 6769  ere private regi
-00011cb0: 7374 7279 2069 6d61 6765 7320 776f 756c  stry images woul
-00011cc0: 646e 2774 2062 6520 7061 7273 6564 0a70  dn't be parsed.p
-00011cd0: 726f 7065 726c 7920 6966 2069 7420 636f  roperly if it co
-00011ce0: 6e74 6169 6e65 6420 706f 7274 2069 6e66  ntained port inf
-00011cf0: 6f72 6d61 7469 6f6e 2e0a 0a0a 302e 312e  ormation....0.1.
-00011d00: 350a 2d2d 2d2d 2d0a 0a2a 2060 436c 6965  5.-----..* `Clie
-00011d10: 6e74 2e62 7569 6c64 6020 6e6f 7720 7573  nt.build` now us
-00011d20: 6573 2074 656d 7066 696c 6573 2074 6f20  es tempfiles to 
-00011d30: 7374 6f72 6520 6275 696c 6420 636f 6e74  store build cont
-00011d40: 6578 7420 696e 7374 6561 6420 6f66 2073  ext instead of s
-00011d50: 746f 7269 6e67 0a69 7420 696e 206d 656d  toring.it in mem
-00011d60: 6f72 790a 2a20 4164 6465 6420 606e 6f63  ory.* Added `noc
-00011d70: 6163 6865 6020 6f70 7469 6f6e 2074 6f20  ache` option to 
-00011d80: 6043 6c69 656e 742e 6275 696c 6460 0a2a  `Client.build`.*
-00011d90: 2060 436c 6965 6e74 2e72 656d 6f76 655f   `Client.remove_
-00011da0: 636f 6e74 6169 6e65 7260 206e 6f77 2072  container` now r
-00011db0: 6169 7365 7320 616e 2065 7863 6570 7469  aises an excepti
-00011dc0: 6f6e 2077 6865 6e20 7472 7969 6e67 2074  on when trying t
-00011dd0: 6f20 7265 6d6f 7665 2061 0a72 756e 6e69  o remove a.runni
-00011de0: 6e67 2063 6f6e 7461 696e 6572 0a2a 2060  ng container.* `
-00011df0: 436c 6965 6e74 2e63 7265 6174 655f 636f  Client.create_co
-00011e00: 6e74 6169 6e65 7260 206e 6f77 2061 6363  ntainer` now acc
-00011e10: 6570 7473 2064 6963 7473 2066 6f72 2074  epts dicts for t
-00011e20: 6865 2060 656e 7669 726f 6e6d 656e 7460  he `environment`
-00011e30: 2070 6172 616d 6574 6572 0a0a 2323 2320   parameter..### 
-00011e40: 4275 6766 6978 6573 0a0a 2a20 4669 7865  Bugfixes..* Fixe
-00011e50: 6420 6120 6275 6720 696e 2060 436c 6965  d a bug in `Clie
-00011e60: 6e74 2e63 7265 6174 655f 636f 6e74 6169  nt.create_contai
-00011e70: 6e65 7260 206f 6e20 5079 7468 6f6e 2032  ner` on Python 2
-00011e80: 2e36 2077 6865 7265 2075 6e69 636f 6465  .6 where unicode
-00011e90: 0a63 6f6d 6d61 6e64 7320 776f 756c 6420  .commands would 
-00011ea0: 6661 696c 2074 6f20 6265 2070 6172 7365  fail to be parse
-00011eb0: 640a 2a20 4669 7865 6420 6120 6275 6720  d.* Fixed a bug 
-00011ec0: 696e 2060 436c 6965 6e74 2e62 7569 6c64  in `Client.build
-00011ed0: 6020 7768 6572 6520 7468 6520 6074 6167  ` where the `tag
-00011ee0: 6020 7061 7261 6d65 7465 7220 776f 756c  ` parameter woul
-00011ef0: 6420 6e6f 7420 6265 2074 616b 656e 0a69  d not be taken.i
-00011f00: 6e74 6f20 6163 636f 756e 740a 0a30 2e31  nto account..0.1
-00011f10: 2e34 0a2d 2d2d 2d2d 0a0a 2a20 4164 6465  .4.-----..* Adde
-00011f20: 6420 7375 7070 6f72 7420 666f 7220 4150  d support for AP
-00011f30: 4920 636f 6e6e 6563 7469 6f6e 2074 6872  I connection thr
-00011f40: 6f75 6768 2055 4e49 5820 736f 636b 6574  ough UNIX socket
-00011f50: 2028 6465 6661 756c 7420 666f 7220 646f   (default for do
-00011f60: 636b 6572 2030 2e35 2e32 2b29 0a0a 302e  cker 0.5.2+)..0.
-00011f70: 312e 330a 2d2d 2d2d 2d0a 0a2a 2054 6865  1.3.-----..* The
-00011f80: 2063 6c69 656e 7420 6e6f 7720 7472 6965   client now trie
-00011f90: 7320 746f 206c 6f61 6420 7468 6520 6175  s to load the au
-00011fa0: 7468 2063 6f6e 6669 6720 6672 6f6d 2060  th config from `
-00011fb0: 7e2f 2e64 6f63 6b65 7263 6667 602e 2054  ~/.dockercfg`. T
-00011fc0: 6869 7320 6973 206e 6563 6573 7361 7279  his is necessary
-00011fd0: 2074 6f20 7573 6520 7468 6520 7075 7368   to use the push
-00011fe0: 2063 6f6d 6d61 6e64 2069 6620 4150 4920   command if API 
-00011ff0: 7665 7273 696f 6e20 6973 203e 312e 300a  version is >1.0.
-00012000: 0a30 2e31 2e32 0a2d 2d2d 2d2d 0a0a 2a20  .0.1.2.-----..* 
-00012010: 4164 6465 6420 6120 6071 7569 6574 2070  Added a `quiet p
-00012020: 6172 616d 6574 6572 6020 746f 2060 436c  arameter` to `Cl
-00012030: 6965 6e74 2e62 7569 6c64 6020 286d 6972  ient.build` (mir
-00012040: 726f 7273 2074 6865 2060 7160 2070 6172  rors the `q` par
-00012050: 616d 6574 6572 2069 6e20 7468 6520 4150  ameter in the AP
-00012060: 4929 0a0a 302e 312e 310a 2d2d 2d2d 2d0a  I)..0.1.1.-----.
-00012070: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
-00012080: 6865 7265 2074 6865 2062 7569 6c64 2063  here the build c
-00012090: 6f6d 6d61 6e64 2077 6f75 6c64 206c 6973  ommand would lis
-000120a0: 7420 7461 7220 636f 6e74 656e 7473 2062  t tar contents b
-000120b0: 6566 6f72 6520 7365 6e64 696e 6720 7468  efore sending th
-000120c0: 6520 7265 7175 6573 740a 2a20 4669 7865  e request.* Fixe
-000120d0: 6420 6120 6275 6720 696e 2060 436c 6965  d a bug in `Clie
-000120e0: 6e74 2e70 6f72 7460 0a0a 0a30 2e31 2e30  nt.port`...0.1.0
-000120f0: 0a2d 2d2d 2d2d 0a2a 202a 2a54 6869 7320  .-----.* **This 
-00012100: 7665 7273 696f 6e20 696e 7472 6f64 7563  version introduc
-00012110: 6573 2062 7265 616b 696e 6720 6368 616e  es breaking chan
-00012120: 6765 7321 2a2a 0a2a 2053 7769 7463 6865  ges!**.* Switche
-00012130: 6420 746f 2073 6572 7665 7220 7369 6465  d to server side
-00012140: 2062 7569 6c64 2073 7973 7465 6d0a 2a20   build system.* 
-00012150: 5265 6d6f 7665 6420 7468 6520 4275 696c  Removed the Buil
-00012160: 6465 7243 6c69 656e 740a 2a20 4164 6465  derClient.* Adde
-00012170: 6420 7375 7070 6f72 7420 666f 7220 636f  d support for co
-00012180: 6e74 6578 7475 616c 2062 7569 6c64 730a  ntextual builds.
-00012190: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-000121a0: 666f 7220 7265 6d6f 7465 2055 524c 2062  for remote URL b
-000121b0: 7569 6c64 730a 2a20 4164 6465 6420 7079  uilds.* Added py
-000121c0: 7468 6f6e 2033 2073 7570 706f 7274 0a2a  thon 3 support.*
-000121d0: 2041 6464 6564 2062 696e 6420 6d6f 756e   Added bind moun
-000121e0: 7473 2073 7570 706f 7274 0a2a 2041 6464  ts support.* Add
-000121f0: 6564 2041 5049 2076 6572 7369 6f6e 2073  ed API version s
-00012200: 7570 706f 7274 0a2a 2046 6978 6564 2061  upport.* Fixed a
-00012210: 2062 7567 2077 6865 7265 2060 436c 6965   bug where `Clie
-00012220: 6e74 2e70 6f72 7460 2077 6f75 6c64 2066  nt.port` would f
-00012230: 6169 6c20 6966 2070 726f 7669 6465 6420  ail if provided 
-00012240: 7769 7468 2061 2070 6f72 7420 6f66 2074  with a port of t
-00012250: 7970 6520 6e75 6d62 6572 0a2a 2046 6978  ype number.* Fix
-00012260: 6564 2061 2062 7567 2077 6865 7265 2060  ed a bug where `
-00012270: 436c 6965 6e74 2e5f 706f 7374 5f6a 736f  Client._post_jso
-00012280: 6e60 2077 6f75 6c64 6e27 7420 7365 7420  n` wouldn't set 
-00012290: 7468 6520 436f 6e74 656e 742d 5479 7065  the Content-Type
-000122a0: 2068 6561 6465 7220 746f 2060 6170 706c   header to `appl
-000122b0: 6963 6174 696f 6e2f 6a73 6f6e 600a 0a30  ication/json`..0
-000122c0: 2e30 2e36 0a2d 2d2d 2d2d 0a2a 2041 6464  .0.6.-----.* Add
-000122d0: 6564 2073 7570 706f 7274 2066 6f72 2063  ed support for c
-000122e0: 7573 746f 6d20 6c6f 6767 6572 7320 696e  ustom loggers in
-000122f0: 2060 436c 6965 6e74 2e62 7569 6c64 600a   `Client.build`.
-00012300: 2a20 4164 6465 6420 6043 6c69 656e 742e  * Added `Client.
-00012310: 6174 7461 6368 6020 636f 6d6d 616e 640a  attach` command.
-00012320: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-00012330: 666f 7220 6041 4444 6020 636f 6d6d 616e  for `ADD` comman
-00012340: 6420 696e 2062 7569 6c64 6572 0a2a 2046  d in builder.* F
-00012350: 6978 6564 2061 2062 7567 2069 6e20 6043  ixed a bug in `C
-00012360: 6c69 656e 742e 6c6f 6773 600a 2a20 496d  lient.logs`.* Im
-00012370: 7072 6f76 6564 2075 6e69 7420 7465 7374  proved unit test
-00012380: 730a 0a0a 302e 302e 350a 2d2d 2d2d 2d0a  s...0.0.5.-----.
-00012390: 2a20 4164 6465 6420 7461 6720 7375 7070  * Added tag supp
-000123a0: 6f72 7420 666f 7220 7468 6520 6275 696c  ort for the buil
-000123b0: 6465 720a 2a20 5573 6520 6073 686c 6578  der.* Use `shlex
-000123c0: 6020 746f 2070 6172 7365 2070 6c61 696e  ` to parse plain
-000123d0: 2073 7472 696e 6720 636f 6d6d 616e 6473   string commands
-000123e0: 2077 6865 6e20 6372 6561 7469 6e67 2061   when creating a
-000123f0: 2063 6f6e 7461 696e 6572 0a2a 2046 6978   container.* Fix
-00012400: 6564 2073 6576 6572 616c 2062 7567 7320  ed several bugs 
-00012410: 696e 2074 6865 2062 7569 6c64 6572 0a2a  in the builder.*
-00012420: 2046 6978 6564 2074 6865 2060 7175 6965   Fixed the `quie
-00012430: 7460 206f 7074 696f 6e20 696e 2060 436c  t` option in `Cl
-00012440: 6965 6e74 2e69 6d61 6765 7360 0a2a 2055  ient.images`.* U
-00012450: 6e69 7420 7465 7374 730a 0a30 2e30 2e34  nit tests..0.0.4
-00012460: 0a2d 2d2d 2d2d 0a2a 2049 6d70 726f 7665  .-----.* Improve
-00012470: 6420 6572 726f 7220 7265 706f 7274 696e  d error reportin
-00012480: 670a 0a30 2e30 2e33 0a2d 2d2d 2d2d 0a2a  g..0.0.3.-----.*
-00012490: 2046 6978 6564 2061 2062 7567 2069 6e20   Fixed a bug in 
-000124a0: 6043 6c69 656e 742e 7461 6760 0a2a 2046  `Client.tag`.* F
-000124b0: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
-000124c0: 2067 656e 6572 6174 6564 2069 6d61 6765   generated image
-000124d0: 7320 776f 756c 6420 6265 2072 656d 6f76  s would be remov
-000124e0: 6564 2061 6674 6572 2061 2073 7563 6365  ed after a succe
-000124f0: 7373 6675 6c20 6275 696c 640a 0a30 2e30  ssful build..0.0
-00012500: 2e32 0a2d 2d2d 2d2d 0a2a 2049 6d70 6c65  .2.-----.* Imple
-00012510: 6d65 6e74 6564 2066 6972 7374 2076 6572  mented first ver
-00012520: 7369 6f6e 206f 6620 7468 6520 6275 696c  sion of the buil
-00012530: 6465 7220 636c 6965 6e74 0a              der client.
+00000010: 3d3d 3d3d 0a0a 362e 312e 320a 2d2d 2d2d  ====..6.1.2.----
+00000020: 2d0a 0a23 2323 2320 4275 6766 6978 6573  -..#### Bugfixes
+00000030: 0a2d 2046 6978 2066 6f72 2073 6f63 6b65  .- Fix for socke
+00000040: 7420 7469 6d65 6f75 7473 206f 6e20 6c6f  t timeouts on lo
+00000050: 6e67 2060 646f 636b 6572 2065 7865 6360  ng `docker exec`
+00000060: 2063 616c 6c73 200a 0a36 2e31 2e31 0a2d   calls ..6.1.1.-
+00000070: 2d2d 2d2d 0a0a 2323 2323 2042 7567 6669  ----..#### Bugfi
+00000080: 7865 730a 2d20 4669 7820 6063 6f6e 7461  xes.- Fix `conta
+00000090: 696e 6572 732e 7374 6174 7328 2960 2068  iners.stats()` h
+000000a0: 616e 6769 6e67 2077 6974 6820 6073 7472  anging with `str
+000000b0: 6561 6d3d 5472 7565 600a 2d20 436f 7272  eam=True`.- Corr
+000000c0: 6563 7420 7265 7475 726e 2074 7970 6520  ect return type 
+000000d0: 696e 2064 6f63 7320 666f 7220 6063 6f6e  in docs for `con
+000000e0: 7461 696e 6572 732e 6469 6666 2829 6020  tainers.diff()` 
+000000f0: 6d65 7468 6f64 0a0a 0a36 2e31 2e30 0a2d  method...6.1.0.-
+00000100: 2d2d 2d2d 0a0a 2323 2320 5570 6772 6164  ----..### Upgrad
+00000110: 6520 4e6f 7465 730a 2d20 4572 726f 7273  e Notes.- Errors
+00000120: 2061 7265 206e 6f20 6c6f 6e67 6572 2072   are no longer r
+00000130: 6574 7572 6e65 6420 6475 7269 6e67 2063  eturned during c
+00000140: 6c69 656e 7420 696e 6974 6961 6c69 7a61  lient initializa
+00000150: 7469 6f6e 2069 6620 7468 6520 6372 6564  tion if the cred
+00000160: 656e 7469 616c 2068 656c 7065 7220 6361  ential helper ca
+00000170: 6e6e 6f74 2062 6520 666f 756e 642e 2041  nnot be found. A
+00000180: 2077 6172 6e69 6e67 2077 696c 6c20 6265   warning will be
+00000190: 2065 6d69 7474 6564 2069 6e73 7465 6164   emitted instead
+000001a0: 2c20 616e 6420 616e 2065 7272 6f72 2069  , and an error i
+000001b0: 7320 7265 7475 726e 6564 2069 6620 7468  s returned if th
+000001c0: 6520 6372 6564 656e 7469 616c 2068 656c  e credential hel
+000001d0: 7065 7220 6973 2075 7365 642e 0a0a 2323  per is used...##
+000001e0: 2320 4665 6174 7572 6573 0a2d 2050 7974  # Features.- Pyt
+000001f0: 686f 6e20 332e 3131 2073 7570 706f 7274  hon 3.11 support
+00000200: 0a2d 2055 7365 2060 706f 6c6c 2829 6020  .- Use `poll()` 
+00000210: 696e 7374 6561 6420 6f66 2060 7365 6c65  instead of `sele
+00000220: 6374 2829 6020 6f6e 206e 6f6e 2d57 696e  ct()` on non-Win
+00000230: 646f 7773 2070 6c61 7466 6f72 6d73 0a2d  dows platforms.-
+00000240: 204e 6577 2041 5049 2066 6965 6c64 730a   New API fields.
+00000250: 2020 2d20 606e 6574 776f 726b 5f64 7269    - `network_dri
+00000260: 7665 725f 6f70 7460 206f 6e20 636f 6e74  ver_opt` on cont
+00000270: 6169 6e65 7220 7275 6e20 2f20 6372 6561  ainer run / crea
+00000280: 7465 0a20 202d 2060 6f6e 652d 7368 6f74  te.  - `one-shot
+00000290: 6020 6f6e 2063 6f6e 7461 696e 6572 2073  ` on container s
+000002a0: 7461 7473 0a20 202d 2060 7374 6174 7573  tats.  - `status
+000002b0: 6020 6f6e 2073 6572 7669 6365 7320 6c69  ` on services li
+000002c0: 7374 0a0a 2323 2320 4275 6766 6978 6573  st..### Bugfixes
+000002d0: 0a2d 2053 7570 706f 7274 2066 6f72 2072  .- Support for r
+000002e0: 6571 7565 7374 7320 322e 3239 2e30 2b20  equests 2.29.0+ 
+000002f0: 616e 6420 7572 6c6c 6962 3320 322e 780a  and urllib3 2.x.
+00000300: 2d20 446f 206e 6f74 2073 7472 6970 2063  - Do not strip c
+00000310: 6861 7261 6374 6572 7320 6672 6f6d 2076  haracters from v
+00000320: 6f6c 756d 6520 6e61 6d65 730a 2d20 4669  olume names.- Fi
+00000330: 7820 636f 6e6e 6563 7469 6f6e 206c 6561  x connection lea
+00000340: 6b20 6f6e 2063 6f6e 7461 696e 6572 2e65  k on container.e
+00000350: 7865 635f 2a20 6f70 6572 6174 696f 6e73  xec_* operations
+00000360: 0a2d 2046 6978 2065 7272 6f72 7320 636c  .- Fix errors cl
+00000370: 6f73 696e 6720 6e61 6d65 6420 7069 7065  osing named pipe
+00000380: 7320 6f6e 2057 696e 646f 7773 0a0a 362e  s on Windows..6.
+00000390: 302e 310a 2d2d 2d2d 2d0a 0a23 2323 2042  0.1.-----..### B
+000003a0: 7567 6669 7865 730a 2d20 4669 7820 666f  ugfixes.- Fix fo
+000003b0: 7220 6054 6865 2070 6970 6520 6861 7320  r `The pipe has 
+000003c0: 6265 656e 2065 6e64 6564 2065 7272 6f72  been ended error
+000003d0: 7360 206f 6e20 5769 6e64 6f77 730a 2d20  s` on Windows.- 
+000003e0: 5375 7070 6f72 7420 666c 6f61 7473 2066  Support floats f
+000003f0: 6f72 2063 6f6e 7461 696e 6572 206c 6f67  or container log
+00000400: 2066 696c 7465 7269 6e67 2062 7920 7469   filtering by ti
+00000410: 6d65 7374 616d 7020 2860 7369 6e63 6560  mestamp (`since`
+00000420: 202f 2060 756e 7469 6c60 290a 0a36 2e30   / `until`)..6.0
+00000430: 2e30 0a2d 2d2d 2d2d 0a0a 2323 2320 5570  .0.-----..### Up
+00000440: 6772 6164 6520 4e6f 7465 730a 2d20 4d69  grade Notes.- Mi
+00000450: 6e69 6d75 6d20 7375 7070 6f72 7465 6420  nimum supported 
+00000460: 5079 7468 6f6e 2076 6572 7369 6f6e 2069  Python version i
+00000470: 7320 332e 372b 0a2d 2057 6865 6e20 696e  s 3.7+.- When in
+00000480: 7374 616c 6c69 6e67 2077 6974 6820 7069  stalling with pi
+00000490: 702c 2074 6865 2060 646f 636b 6572 5b74  p, the `docker[t
+000004a0: 6c73 5d60 2065 7874 7261 2069 7320 6465  ls]` extra is de
+000004b0: 7072 6563 6174 6564 2061 6e64 2061 206e  precated and a n
+000004c0: 6f2d 6f70 2c0a 2020 7573 6520 6064 6f63  o-op,.  use `doc
+000004d0: 6b65 7260 2066 6f72 2073 616d 6520 6675  ker` for same fu
+000004e0: 6e63 7469 6f6e 616c 6974 7920 2854 4c53  nctionality (TLS
+000004f0: 2073 7570 706f 7274 2069 7320 616c 7761   support is alwa
+00000500: 7973 2061 7661 696c 6162 6c65 206e 6f77  ys available now
+00000510: 290a 2d20 4e61 7469 7665 2050 7974 686f  ).- Native Pytho
+00000520: 6e20 5353 4820 636c 6965 6e74 2028 7573  n SSH client (us
+00000530: 6564 2062 7920 6465 6661 756c 7420 2f20  ed by default / 
+00000540: 6075 7365 5f73 7368 5f63 6c69 656e 743d  `use_ssh_client=
+00000550: 4661 6c73 6560 2920 7769 6c6c 206e 6f77  False`) will now
+00000560: 0a20 2072 656a 6563 7420 756e 6b6e 6f77  .  reject unknow
+00000570: 6e20 686f 7374 206b 6579 7320 7769 7468  n host keys with
+00000580: 2060 7061 7261 6d69 6b6f 2e73 7368 5f65   `paramiko.ssh_e
+00000590: 7863 6570 7469 6f6e 2e53 5348 4578 6365  xception.SSHExce
+000005a0: 7074 696f 6e60 0a2d 2053 686f 7274 2049  ption`.- Short I
+000005b0: 4473 2061 7265 206e 6f77 2031 3220 6368  Ds are now 12 ch
+000005c0: 6172 6163 7465 7273 2069 6e73 7465 6164  aracters instead
+000005d0: 206f 6620 3130 2063 6861 7261 6374 6572   of 10 character
+000005e0: 7320 2873 616d 6520 6173 2044 6f63 6b65  s (same as Docke
+000005f0: 7220 434c 4929 0a0a 2323 2320 4665 6174  r CLI)..### Feat
+00000600: 7572 6573 0a2d 2050 7974 686f 6e20 332e  ures.- Python 3.
+00000610: 3130 2073 7570 706f 7274 0a2d 2041 7574  10 support.- Aut
+00000620: 6f6d 6174 6963 616c 6c79 206e 6567 6f74  omatically negot
+00000630: 6961 7465 206d 6f73 7420 7365 6375 7265  iate most secure
+00000640: 2054 4c53 2076 6572 7369 6f6e 0a2d 2041   TLS version.- A
+00000650: 6464 2060 706c 6174 666f 726d 6020 2865  dd `platform` (e
+00000660: 2e67 2e20 606c 696e 7578 2f61 6d64 3634  .g. `linux/amd64
+00000670: 602c 2060 6461 7277 696e 2f61 726d 3634  `, `darwin/arm64
+00000680: 6029 2074 6f20 636f 6e74 6169 6e65 7220  `) to container 
+00000690: 6372 6561 7465 2026 2072 756e 0a2d 2041  create & run.- A
+000006a0: 6464 2073 7570 706f 7274 2066 6f72 2060  dd support for `
+000006b0: 476c 6f62 616c 4a6f 6260 2061 6e64 2060  GlobalJob` and `
+000006c0: 5265 706c 6963 6174 6564 4a6f 6273 6020  ReplicatedJobs` 
+000006d0: 666f 7220 5377 6172 6d0a 2d20 4164 6420  for Swarm.- Add 
+000006e0: 6072 656d 6f76 6528 2960 206d 6574 686f  `remove()` metho
+000006f0: 6420 6f6e 2060 496d 6167 6560 0a2d 2041  d on `Image`.- A
+00000700: 6464 2060 666f 7263 6560 2070 6172 616d  dd `force` param
+00000710: 2074 6f20 6064 6973 6162 6c65 2829 6020   to `disable()` 
+00000720: 6f6e 2060 506c 7567 696e 600a 0a23 2323  on `Plugin`..###
+00000730: 2042 7567 6669 7865 730a 2d20 4669 7820   Bugfixes.- Fix 
+00000740: 696e 7374 616c 6c20 6973 7375 6573 206f  install issues o
+00000750: 6e20 5769 6e64 6f77 7320 7265 6c61 7465  n Windows relate
+00000760: 6420 746f 2060 7079 7769 6e33 3260 0a2d  d to `pywin32`.-
+00000770: 2044 6f20 6e6f 7420 6163 6365 7074 2075   Do not accept u
+00000780: 6e6b 6e6f 776e 2053 5348 2068 6f73 7420  nknown SSH host 
+00000790: 6b65 7973 2069 6e20 6e61 7469 7665 2050  keys in native P
+000007a0: 7974 686f 6e20 5353 4820 6d6f 6465 0a2d  ython SSH mode.-
+000007b0: 2055 7365 2031 3220 6368 6172 6163 7465   Use 12 characte
+000007c0: 7220 7368 6f72 7420 4944 7320 666f 7220  r short IDs for 
+000007d0: 636f 6e73 6973 7465 6e63 7920 7769 7468  consistency with
+000007e0: 2044 6f63 6b65 7220 434c 490a 2d20 4967   Docker CLI.- Ig
+000007f0: 6e6f 7265 2074 7261 696c 696e 6720 7768  nore trailing wh
+00000800: 6974 6573 7061 6365 2069 6e20 602e 646f  itespace in `.do
+00000810: 636b 6572 6967 6e6f 7265 6020 6669 6c65  ckerignore` file
+00000820: 730a 2d20 4669 7820 4950 7636 2068 6f73  s.- Fix IPv6 hos
+00000830: 7420 7061 7273 696e 6720 7768 656e 2065  t parsing when e
+00000840: 7870 6c69 6369 7420 706f 7274 2073 7065  xplicit port spe
+00000850: 6369 6669 6564 0a2d 2046 6978 2060 5072  cified.- Fix `Pr
+00000860: 6f78 7943 6f6d 6d61 6e64 6020 6f70 7469  oxyCommand` opti
+00000870: 6f6e 2066 6f72 2053 5348 2063 6f6e 6e65  on for SSH conne
+00000880: 6374 696f 6e73 0a2d 2044 6f20 6e6f 7420  ctions.- Do not 
+00000890: 7370 6177 6e20 6578 7472 6120 7375 6273  spawn extra subs
+000008a0: 6865 6c6c 2077 6865 6e20 6c61 756e 6368  hell when launch
+000008b0: 696e 6720 6578 7465 726e 616c 2053 5348  ing external SSH
+000008c0: 2063 6c69 656e 740a 2d20 496d 7072 6f76   client.- Improv
+000008d0: 6520 6578 6365 7074 696f 6e20 7365 6d61  e exception sema
+000008e0: 6e74 6963 7320 746f 2070 7265 7365 7276  ntics to preserv
+000008f0: 6520 636f 6e74 6578 740a 2d20 446f 6375  e context.- Docu
+00000900: 6d65 6e74 6174 696f 6e20 696d 7072 6f76  mentation improv
+00000910: 656d 656e 7473 2028 666f 726d 6174 7469  ements (formatti
+00000920: 6e67 2c20 6578 616d 706c 6573 2c20 7479  ng, examples, ty
+00000930: 706f 732c 206d 6973 7369 6e67 2070 6172  pos, missing par
+00000940: 616d 7329 0a0a 2323 2320 4d69 7363 656c  ams)..### Miscel
+00000950: 6c61 6e65 6f75 730a 2d20 5570 6772 6164  laneous.- Upgrad
+00000960: 6520 6465 7065 6e64 656e 6369 6573 2069  e dependencies i
+00000970: 6e20 6072 6571 7569 7265 6d65 6e74 732e  n `requirements.
+00000980: 7478 7460 2074 6f20 6c61 7465 7374 2076  txt` to latest v
+00000990: 6572 7369 6f6e 730a 2d20 5265 6d6f 7665  ersions.- Remove
+000009a0: 2065 7874 7261 6e65 6f75 7320 7472 616e   extraneous tran
+000009b0: 7369 7469 7665 2064 6570 656e 6465 6e63  sitive dependenc
+000009c0: 6965 730a 2d20 456c 696d 696e 6174 6520  ies.- Eliminate 
+000009d0: 7573 6167 6573 206f 6620 6465 7072 6563  usages of deprec
+000009e0: 6174 6564 2066 756e 6374 696f 6e73 2f6d  ated functions/m
+000009f0: 6574 686f 6473 0a2d 2054 6573 7420 7375  ethods.- Test su
+00000a00: 6974 6520 7265 6c69 6162 696c 6974 7920  ite reliability 
+00000a10: 696d 7072 6f76 656d 656e 7473 0a2d 2047  improvements.- G
+00000a20: 6974 4875 6220 4163 7469 6f6e 7320 776f  itHub Actions wo
+00000a30: 726b 666c 6f77 7320 666f 7220 6c69 6e74  rkflows for lint
+00000a40: 696e 672c 2075 6e69 7420 7465 7374 732c  ing, unit tests,
+00000a50: 2069 6e74 6567 7261 7469 6f6e 2074 6573   integration tes
+00000a60: 7473 2c20 616e 640a 2020 7075 626c 6973  ts, and.  publis
+00000a70: 6869 6e67 2072 656c 6561 7365 730a 0a35  hing releases..5
+00000a80: 2e30 2e33 0a2d 2d2d 2d2d 0a0a 5b4c 6973  .0.3.-----..[Lis
+00000a90: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
+00000aa0: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+00000ab0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+00000ac0: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
+00000ad0: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
+00000ae0: 652f 3736 3f63 6c6f 7365 643d 3129 0a0a  e/76?closed=1)..
+00000af0: 2323 2320 4665 6174 7572 6573 0a2d 2041  ### Features.- A
+00000b00: 6464 2060 6361 705f 6164 6460 2061 6e64  dd `cap_add` and
+00000b10: 2060 6361 705f 6472 6f70 6020 7061 7261   `cap_drop` para
+00000b20: 6d65 7465 7273 2074 6f20 7365 7276 6963  meters to servic
+00000b30: 6520 6372 6561 7465 2061 6e64 2043 6f6e  e create and Con
+00000b40: 7461 696e 6572 5370 6563 0a2d 2041 6464  tainerSpec.- Add
+00000b50: 2060 7465 6d70 6c61 7469 6e67 6020 7061   `templating` pa
+00000b60: 7261 6d65 7465 7220 746f 2063 6f6e 6669  rameter to confi
+00000b70: 6720 6372 6561 7465 0a0a 2323 2320 4275  g create..### Bu
+00000b80: 6766 6978 6573 0a2d 2046 6978 2067 6574  gfixes.- Fix get
+00000b90: 7469 6e67 2061 2072 6561 6420 7469 6d65  ting a read time
+00000ba0: 6f75 7420 666f 7220 6c6f 6773 2f61 7474  out for logs/att
+00000bb0: 6163 6820 7769 7468 2061 2074 7479 2061  ach with a tty a
+00000bc0: 6e64 2073 6c6f 7720 6f75 7470 7574 0a0a  nd slow output..
+00000bd0: 2323 2320 4d69 7363 656c 6c61 6e65 6f75  ### Miscellaneou
+00000be0: 730a 2d20 4669 7820 646f 6375 6d65 6e74  s.- Fix document
+00000bf0: 6174 696f 6e20 6578 616d 706c 6573 0a0a  ation examples..
+00000c00: 352e 302e 320a 2d2d 2d2d 2d0a 0a5b 4c69  5.0.2.-----..[Li
+00000c10: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+00000c20: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+00000c30: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+00000c40: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+00000c50: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
+00000c60: 6e65 2f37 353f 636c 6f73 6564 3d31 290a  ne/75?closed=1).
+00000c70: 0a23 2323 2042 7567 6669 7865 730a 2d20  .### Bugfixes.- 
+00000c80: 4669 7820 6064 6973 6162 6c65 5f62 7566  Fix `disable_buf
+00000c90: 6665 7269 6e67 6020 7265 6772 6573 7369  fering` regressi
+00000ca0: 6f6e 0a0a 352e 302e 310a 2d2d 2d2d 2d0a  on..5.0.1.-----.
+00000cb0: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
+00000cc0: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
+00000cd0: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
+00000ce0: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
+00000cf0: 6572 2f64 6f63 6b65 722d 7079 2f6d 696c  er/docker-py/mil
+00000d00: 6573 746f 6e65 2f37 343f 636c 6f73 6564  estone/74?closed
+00000d10: 3d31 290a 0a23 2323 2042 7567 6669 7865  =1)..### Bugfixe
+00000d20: 730a 2d20 4272 696e 6720 6261 636b 2073  s.- Bring back s
+00000d30: 7570 706f 7274 2066 6f72 2073 7368 2069  upport for ssh i
+00000d40: 6465 6e74 6974 7920 6669 6c65 0a2d 2043  dentity file.- C
+00000d50: 6c65 616e 7570 2072 656d 6169 6e69 6e67  leanup remaining
+00000d60: 2070 7974 686f 6e2d 3220 6465 7065 6e64   python-2 depend
+00000d70: 656e 6369 6573 0a2d 2046 6978 2069 6d61  encies.- Fix ima
+00000d80: 6765 2073 6176 6520 6578 616d 706c 6520  ge save example 
+00000d90: 696e 2064 6f63 730a 0a23 2323 204d 6973  in docs..### Mis
+00000da0: 6365 6c6c 616e 656f 7573 0a2d 2042 756d  cellaneous.- Bum
+00000db0: 7020 7572 6c6c 6962 3320 746f 2031 2e32  p urllib3 to 1.2
+00000dc0: 362e 350a 2d20 4275 6d70 2072 6571 7565  6.5.- Bump reque
+00000dd0: 7374 7320 746f 2032 2e32 362e 300a 0a35  sts to 2.26.0..5
+00000de0: 2e30 2e30 0a2d 2d2d 2d2d 0a0a 5b4c 6973  .0.0.-----..[Lis
+00000df0: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
+00000e00: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+00000e10: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+00000e20: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
+00000e30: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
+00000e40: 652f 3730 3f63 6c6f 7365 643d 3129 0a0a  e/70?closed=1)..
+00000e50: 2323 2320 4272 6561 6b69 6e67 2063 6861  ### Breaking cha
+00000e60: 6e67 6573 0a2d 2052 656d 6f76 6520 7375  nges.- Remove su
+00000e70: 7070 6f72 7420 666f 7220 5079 7468 6f6e  pport for Python
+00000e80: 2032 2e37 0a2d 204d 616b 6520 5079 7468   2.7.- Make Pyth
+00000e90: 6f6e 2033 2e36 2074 6865 206d 696e 696d  on 3.6 the minim
+00000ea0: 756d 2076 6572 7369 6f6e 2073 7570 706f  um version suppo
+00000eb0: 7274 6564 0a0a 2323 2320 4665 6174 7572  rted..### Featur
+00000ec0: 6573 0a2d 2041 6464 2060 6c69 6d69 7460  es.- Add `limit`
+00000ed0: 2070 6172 616d 6574 6572 2074 6f20 696d   parameter to im
+00000ee0: 6167 6520 7365 6172 6368 2065 6e64 706f  age search endpo
+00000ef0: 696e 740a 0a23 2323 2042 7567 6669 7865  int..### Bugfixe
+00000f00: 730a 2d20 4669 7820 604b 6579 4572 726f  s.- Fix `KeyErro
+00000f10: 7260 2065 7863 6570 7469 6f6e 206f 6e20  r` exception on 
+00000f20: 7365 6372 6574 2063 7265 6174 650a 2d20  secret create.- 
+00000f30: 5665 7269 6679 2054 4c53 206b 6579 7320  Verify TLS keys 
+00000f40: 6c6f 6164 6564 2066 726f 6d20 646f 636b  loaded from dock
+00000f50: 6572 2063 6f6e 7465 7874 730a 2d20 5570  er contexts.- Up
+00000f60: 6461 7465 2050 4f52 545f 5350 4543 2072  date PORT_SPEC r
+00000f70: 6567 6578 2074 6f20 616c 6c6f 7720 7371  egex to allow sq
+00000f80: 7561 7265 2062 7261 636b 6574 7320 666f  uare brackets fo
+00000f90: 7220 4950 7636 2061 6464 7265 7373 6573  r IPv6 addresses
+00000fa0: 0a2d 2046 6978 2063 6f6e 7461 696e 6572  .- Fix container
+00000fb0: 7320 616e 6420 696d 6167 6573 2064 6f63  s and images doc
+00000fc0: 756d 656e 7461 7469 6f6e 2065 7861 6d70  umentation examp
+00000fd0: 6c65 730a 0a34 2e34 2e34 0a2d 2d2d 2d2d  les..4.4.4.-----
+00000fe0: 0a0a 5b4c 6973 7420 6f66 2050 5273 202f  ..[List of PRs /
+00000ff0: 2069 7373 7565 7320 666f 7220 7468 6973   issues for this
+00001000: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+00001010: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
+00001020: 6b65 722f 646f 636b 6572 2d70 792f 6d69  ker/docker-py/mi
+00001030: 6c65 7374 6f6e 652f 3733 3f63 6c6f 7365  lestone/73?close
+00001040: 643d 3129 0a0a 2323 2320 4275 6766 6978  d=1)..### Bugfix
+00001050: 6573 0a2d 2052 656d 6f76 6520 604c 445f  es.- Remove `LD_
+00001060: 4c49 4252 4152 595f 5041 5448 6020 616e  LIBRARY_PATH` an
+00001070: 6420 6053 534c 5f43 4552 545f 4649 4c45  d `SSL_CERT_FILE
+00001080: 6020 656e 7669 726f 6e6d 656e 7420 7661  ` environment va
+00001090: 7269 6162 6c65 7320 7768 656e 2073 6865  riables when she
+000010a0: 6c6c 696e 6720 6f75 7420 746f 2074 6865  lling out to the
+000010b0: 2073 7368 2063 6c69 656e 740a 0a34 2e34   ssh client..4.4
+000010c0: 2e33 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420  .3.-----..[List 
+000010d0: 6f66 2050 5273 202f 2069 7373 7565 7320  of PRs / issues 
+000010e0: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
+000010f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001100: 2e63 6f6d 2f64 6f63 6b65 722f 646f 636b  .com/docker/dock
+00001110: 6572 2d70 792f 6d69 6c65 7374 6f6e 652f  er-py/milestone/
+00001120: 3732 3f63 6c6f 7365 643d 3129 0a0a 2323  72?closed=1)..##
+00001130: 2320 4665 6174 7572 6573 0a2d 2041 6464  # Features.- Add
+00001140: 2073 7570 706f 7274 2066 6f72 2064 6f63   support for doc
+00001150: 6b65 722e 7479 7065 732e 506c 6163 656d  ker.types.Placem
+00001160: 656e 742e 4d61 7852 6570 6c69 6361 730a  ent.MaxReplicas.
+00001170: 0a23 2323 2042 7567 6669 7865 730a 2d20  .### Bugfixes.- 
+00001180: 4669 7820 5353 4820 706f 7274 2070 6172  Fix SSH port par
+00001190: 7369 6e67 2077 6865 6e20 7368 656c 6c69  sing when shelli
+000011a0: 6e67 206f 7574 2074 6f20 7468 6520 7373  ng out to the ss
+000011b0: 6820 636c 6965 6e74 0a0a 342e 342e 320a  h client..4.4.2.
+000011c0: 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f 6620  -----..[List of 
+000011d0: 5052 7320 2f20 6973 7375 6573 2066 6f72  PRs / issues for
+000011e0: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
+000011f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001200: 6d2f 646f 636b 6572 2f64 6f63 6b65 722d  m/docker/docker-
+00001210: 7079 2f6d 696c 6573 746f 6e65 2f37 313f  py/milestone/71?
+00001220: 636c 6f73 6564 3d31 290a 0a23 2323 2042  closed=1)..### B
+00001230: 7567 6669 7865 730a 2d20 4669 7820 5353  ugfixes.- Fix SS
+00001240: 4820 636f 6e6e 6563 7469 6f6e 2062 7567  H connection bug
+00001250: 2077 6865 7265 2074 6865 2068 6f73 746e   where the hostn
+00001260: 616d 6520 7761 7320 696e 636f 7272 6563  ame was incorrec
+00001270: 746c 7920 7472 696d 6d65 6420 616e 6420  tly trimmed and 
+00001280: 7468 6520 6572 726f 7220 7761 7320 6869  the error was hi
+00001290: 6464 656e 0a2d 2046 6978 2064 6f63 7320  dden.- Fix docs 
+000012a0: 6578 616d 706c 650a 0a23 2323 204d 6973  example..### Mis
+000012b0: 6365 6c6c 616e 656f 7573 0a2d 2041 6464  cellaneous.- Add
+000012c0: 2050 7974 686f 6e33 2e38 2061 6e64 2033   Python3.8 and 3
+000012d0: 2e39 2069 6e20 7365 7475 702e 7079 2063  .9 in setup.py c
+000012e0: 6c61 7373 6966 6965 7220 6c69 7374 0a0a  lassifier list..
+000012f0: 342e 342e 310a 2d2d 2d2d 2d0a 0a5b 4c69  4.4.1.-----..[Li
+00001300: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+00001310: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+00001320: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+00001330: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+00001340: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
+00001350: 6e65 2f36 393f 636c 6f73 6564 3d31 290a  ne/69?closed=1).
+00001360: 0a23 2323 2042 7567 6669 7865 730a 2d20  .### Bugfixes.- 
+00001370: 4176 6f69 6420 7365 7474 696e 6720 756e  Avoid setting un
+00001380: 7375 706f 7274 6564 2070 6172 616d 6574  suported paramet
+00001390: 6572 2066 6f72 2073 7562 7072 6f63 6573  er for subproces
+000013a0: 732e 506f 7065 6e20 6f6e 2057 696e 646f  s.Popen on Windo
+000013b0: 7773 0a2d 2052 6570 6c61 6365 2075 7365  ws.- Replace use
+000013c0: 206f 6620 6465 7072 6563 6174 6564 2022   of deprecated "
+000013d0: 6669 6c74 6572 2220 6172 6775 6d65 6e74  filter" argument
+000013e0: 206f 6e20 2222 646f 636b 6572 2f61 7069   on ""docker/api
+000013f0: 2f69 6d61 6765 220a 0a34 2e34 2e30 0a2d  /image"..4.4.0.-
+00001400: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
+00001410: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
+00001420: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+00001430: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001440: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
+00001450: 792f 6d69 6c65 7374 6f6e 652f 3637 3f63  y/milestone/67?c
+00001460: 6c6f 7365 643d 3129 0a0a 2323 2320 4665  losed=1)..### Fe
+00001470: 6174 7572 6573 0a2d 2041 6464 2061 6e20  atures.- Add an 
+00001480: 616c 7465 726e 6174 6976 6520 5353 4820  alternative SSH 
+00001490: 636f 6e6e 6563 7469 6f6e 2074 6f20 7468  connection to th
+000014a0: 6520 7061 7261 6d69 6b6f 206f 6e65 2c20  e paramiko one, 
+000014b0: 6261 7365 6420 6f6e 2073 6865 6c6c 696e  based on shellin
+000014c0: 6720 6f75 7420 746f 2074 6865 2053 5368  g out to the SSh
+000014d0: 2063 6c69 656e 742e 2053 696d 696c 6172   client. Similar
+000014e0: 2074 6f20 7468 6520 6265 6861 7669 6f75   to the behaviou
+000014f0: 7220 6f66 2044 6f63 6b65 7220 636c 690a  r of Docker cli.
+00001500: 2d20 4465 6661 756c 7420 696d 6167 6520  - Default image 
+00001510: 7461 6720 746f 2060 6c61 7465 7374 6020  tag to `latest` 
+00001520: 6f6e 2060 7075 6c6c 600a 0a23 2323 2042  on `pull`..### B
+00001530: 7567 6669 7865 730a 2d20 4669 7820 706c  ugfixes.- Fix pl
+00001540: 7567 696e 206d 6f64 656c 2075 7067 7261  ugin model upgra
+00001550: 6465 0a2d 2046 6978 2065 7861 6d70 6c65  de.- Fix example
+00001560: 7320 5552 4c20 696e 2075 6c69 6d69 7473  s URL in ulimits
+00001570: 0a0a 2323 2320 4d69 7363 656c 6c61 6e65  ..### Miscellane
+00001580: 6f75 730a 2d20 496d 7072 6f76 6520 6578  ous.- Improve ex
+00001590: 6365 7074 696f 6e20 6d65 7373 6167 6573  ception messages
+000015a0: 2066 6f72 2073 6572 7665 7220 616e 6420   for server and 
+000015b0: 636c 6965 6e74 2065 7272 6f72 730a 2d20  client errors.- 
+000015c0: 4275 6d70 2063 7279 7074 6f67 7261 7068  Bump cryptograph
+000015d0: 7920 6672 6f6d 2032 2e33 2074 6f20 332e  y from 2.3 to 3.
+000015e0: 320a 0a34 2e33 2e31 0a2d 2d2d 2d2d 0a0a  2..4.3.1.-----..
+000015f0: 5b4c 6973 7420 6f66 2050 5273 202f 2069  [List of PRs / i
+00001600: 7373 7565 7320 666f 7220 7468 6973 2072  ssues for this r
+00001610: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00001620: 6769 7468 7562 2e63 6f6d 2f64 6f63 6b65  github.com/docke
+00001630: 722f 646f 636b 6572 2d70 792f 6d69 6c65  r/docker-py/mile
+00001640: 7374 6f6e 652f 3638 3f63 6c6f 7365 643d  stone/68?closed=
+00001650: 3129 0a0a 2323 2320 4d69 7363 656c 6c61  1)..### Miscella
+00001660: 6e65 6f75 730a 2d20 5365 7420 6465 6661  neous.- Set defa
+00001670: 756c 7420 4150 4920 7665 7273 696f 6e20  ult API version 
+00001680: 746f 2060 6175 746f 600a 2d20 4669 7820  to `auto`.- Fix 
+00001690: 636f 6e76 6572 7369 6f6e 2074 6f20 6279  conversion to by
+000016a0: 7465 7320 666f 7220 6066 6c6f 6174 600a  tes for `float`.
+000016b0: 2d20 5375 7070 6f72 7420 4f70 656e 5353  - Support OpenSS
+000016c0: 4820 6069 6465 6e74 6974 7966 696c 6560  H `identityfile`
+000016d0: 206f 7074 696f 6e0a 0a34 2e33 2e30 0a2d   option..4.3.0.-
+000016e0: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
+000016f0: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
+00001700: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+00001710: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001720: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
+00001730: 792f 6d69 6c65 7374 6f6e 652f 3634 3f63  y/milestone/64?c
+00001740: 6c6f 7365 643d 3129 0a0a 2323 2320 4665  losed=1)..### Fe
+00001750: 6174 7572 6573 0a2d 2041 6464 2060 4465  atures.- Add `De
+00001760: 7669 6365 5265 7175 6573 7460 2074 7970  viceRequest` typ
+00001770: 6520 746f 2065 7870 6f73 6520 686f 7374  e to expose host
+00001780: 2072 6573 6f75 7263 6573 2073 7563 6820   resources such 
+00001790: 6173 2047 5055 730a 2d20 4164 6420 7375  as GPUs.- Add su
+000017a0: 7070 6f72 7420 666f 7220 6044 7269 7665  pport for `Drive
+000017b0: 724f 7074 7360 2069 6e20 456e 6470 6f69  rOpts` in Endpoi
+000017c0: 6e74 436f 6e66 6967 0a2d 2044 6973 6162  ntConfig.- Disab
+000017d0: 6c65 2063 6f6d 7072 6573 7369 6f6e 2062  le compression b
+000017e0: 7920 6465 6661 756c 7420 7768 656e 2075  y default when u
+000017f0: 7369 6e67 2063 6f6e 7461 696e 6572 2e67  sing container.g
+00001800: 6574 5f61 7263 6869 7665 206d 6574 686f  et_archive metho
+00001810: 640a 0a23 2323 204d 6973 6365 6c6c 616e  d..### Miscellan
+00001820: 656f 7573 0a2d 2055 7064 6174 6520 6465  eous.- Update de
+00001830: 6661 756c 7420 4150 4920 7665 7273 696f  fault API versio
+00001840: 6e20 746f 2076 312e 3339 0a2d 2055 7064  n to v1.39.- Upd
+00001850: 6174 6520 7465 7374 2065 6e67 696e 6520  ate test engine 
+00001860: 7665 7273 696f 6e20 746f 2031 392e 3033  version to 19.03
+00001870: 2e31 320a 0a34 2e32 2e32 0a2d 2d2d 2d2d  .12..4.2.2.-----
+00001880: 0a0a 5b4c 6973 7420 6f66 2050 5273 202f  ..[List of PRs /
+00001890: 2069 7373 7565 7320 666f 7220 7468 6973   issues for this
+000018a0: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+000018b0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
+000018c0: 6b65 722f 646f 636b 6572 2d70 792f 6d69  ker/docker-py/mi
+000018d0: 6c65 7374 6f6e 652f 3636 3f63 6c6f 7365  lestone/66?close
+000018e0: 643d 3129 0a0a 2323 2320 4275 6766 6978  d=1)..### Bugfix
+000018f0: 6573 0a0a 2d20 4669 7820 636f 6e74 6578  es..- Fix contex
+00001900: 7420 6c6f 6164 2066 6f72 206e 6f6e 2d64  t load for non-d
+00001910: 6f63 6b65 7220 656e 6470 6f69 6e74 730a  ocker endpoints.
+00001920: 0a34 2e32 2e31 0a2d 2d2d 2d2d 0a0a 5b4c  .4.2.1.-----..[L
+00001930: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
+00001940: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
+00001950: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
+00001960: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
+00001970: 646f 636b 6572 2d70 792f 6d69 6c65 7374  docker-py/milest
+00001980: 6f6e 652f 3635 3f63 6c6f 7365 643d 3129  one/65?closed=1)
+00001990: 0a0a 2323 2320 4665 6174 7572 6573 0a0a  ..### Features..
+000019a0: 2d20 4164 6420 6f70 7469 6f6e 206f 6e20  - Add option on 
+000019b0: 7768 656e 2074 6f20 7573 6520 6074 6c73  when to use `tls
+000019c0: 6020 6f6e 2043 6f6e 7465 7874 2063 6f6e  ` on Context con
+000019d0: 7374 7275 6374 6f72 0a2d 204d 616b 6520  structor.- Make 
+000019e0: 636f 6e74 6578 7420 6f72 6368 6573 7472  context orchestr
+000019f0: 6174 6f72 2066 6965 6c64 206f 7074 696f  ator field optio
+00001a00: 6e61 6c0a 0a34 2e32 2e30 0a2d 2d2d 2d2d  nal..4.2.0.-----
+00001a10: 0a0a 5b4c 6973 7420 6f66 2050 5273 202f  ..[List of PRs /
+00001a20: 2069 7373 7565 7320 666f 7220 7468 6973   issues for this
+00001a30: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+00001a40: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
+00001a50: 6b65 722f 646f 636b 6572 2d70 792f 6d69  ker/docker-py/mi
+00001a60: 6c65 7374 6f6e 652f 3633 3f63 6c6f 7365  lestone/63?close
+00001a70: 643d 3129 0a0a 2323 2320 4275 6766 6978  d=1)..### Bugfix
+00001a80: 6573 0a0a 2d20 4669 7820 6077 696e 3332  es..- Fix `win32
+00001a90: 7069 7065 2e57 6169 744e 616d 6564 5069  pipe.WaitNamedPi
+00001aa0: 7065 6020 7468 726f 7720 6578 6365 7074  pe` throw except
+00001ab0: 696f 6e20 696e 2057 696e 646f 7773 2063  ion in Windows c
+00001ac0: 6f6e 7461 696e 6572 730a 2d20 5573 6520  ontainers.- Use 
+00001ad0: 6048 6f73 746e 616d 6560 2c20 6055 7365  `Hostname`, `Use
+00001ae0: 726e 616d 6560 2c20 6050 6f72 7460 2061  rname`, `Port` a
+00001af0: 6e64 2060 5072 6f78 7943 6f6d 6d61 6e64  nd `ProxyCommand
+00001b00: 6020 7365 7474 696e 6773 2066 726f 6d20  ` settings from 
+00001b10: 602e 7373 682f 636f 6e66 6967 6020 7768  `.ssh/config` wh
+00001b20: 656e 206f 6e20 5353 480a 2d20 5365 7420  en on SSH.- Set 
+00001b30: 686f 7374 206b 6579 2070 6f6c 6963 7920  host key policy 
+00001b40: 666f 7220 7373 6820 7472 616e 7370 6f72  for ssh transpor
+00001b50: 7420 746f 2060 7061 7261 6d69 6b6f 2e57  t to `paramiko.W
+00001b60: 6172 6e69 6e67 506f 6c69 6379 2829 600a  arningPolicy()`.
+00001b70: 2d20 5365 7420 6c6f 6767 696e 6720 6c65  - Set logging le
+00001b80: 7665 6c20 6f66 2060 7061 7261 6d69 6b6f  vel of `paramiko
+00001b90: 6020 746f 2077 6172 6e0a 0a23 2323 2046  ` to warn..### F
+00001ba0: 6561 7475 7265 730a 0a2d 2041 6464 2073  eatures..- Add s
+00001bb0: 7570 706f 7274 2066 6f72 2064 6f63 6b65  upport for docke
+00001bc0: 7220 636f 6e74 6578 7473 2074 6872 6f75  r contexts throu
+00001bd0: 6768 2060 646f 636b 6572 2e43 6f6e 7465  gh `docker.Conte
+00001be0: 7874 4150 4960 0a0a 342e 312e 300a 2d2d  xtAPI`..4.1.0.--
+00001bf0: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
+00001c00: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
+00001c10: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+00001c20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001c30: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
+00001c40: 2f6d 696c 6573 746f 6e65 2f36 313f 636c  /milestone/61?cl
+00001c50: 6f73 6564 3d31 290a 0a23 2323 2042 7567  osed=1)..### Bug
+00001c60: 6669 7865 730a 0a2d 2043 6f72 7265 6374  fixes..- Correct
+00001c70: 2060 494e 4445 585f 5552 4c60 206c 6f67   `INDEX_URL` log
+00001c80: 6963 2069 6e20 6275 696c 642e 7079 205f  ic in build.py _
+00001c90: 7365 745f 6175 7468 5f68 6561 6465 7273  set_auth_headers
+00001ca0: 0a2d 2046 6978 2066 6f72 2065 6d70 7479  .- Fix for empty
+00001cb0: 2061 7574 6820 6b65 7973 2069 6e20 636f   auth keys in co
+00001cc0: 6e66 6967 2e6a 736f 6e0a 0a23 2323 2046  nfig.json..### F
+00001cd0: 6561 7475 7265 730a 0a2d 2041 6464 2060  eatures..- Add `
+00001ce0: 4e65 7477 6f72 6b41 7474 6163 686d 656e  NetworkAttachmen
+00001cf0: 7443 6f6e 6669 6760 2066 6f72 2073 6572  tConfig` for ser
+00001d00: 7669 6365 2063 7265 6174 652f 7570 6461  vice create/upda
+00001d10: 7465 0a0a 2323 2320 4d69 7363 656c 6c61  te..### Miscella
+00001d20: 6e65 6f75 730a 0a2d 2042 756d 7020 7079  neous..- Bump py
+00001d30: 7465 7374 2074 6f20 342e 332e 310a 2d20  test to 4.3.1.- 
+00001d40: 4164 6a75 7374 2060 2d2d 706c 6174 666f  Adjust `--platfo
+00001d50: 726d 6020 7465 7374 7320 666f 7220 6368  rm` tests for ch
+00001d60: 616e 6765 7320 696e 2064 6f63 6b65 7220  anges in docker 
+00001d70: 656e 6769 6e65 0a2d 2055 7064 6174 6520  engine.- Update 
+00001d80: 6372 6564 656e 7469 616c 732d 6865 6c70  credentials-help
+00001d90: 6572 7320 746f 2076 302e 362e 330a 0a34  ers to v0.6.3..4
+00001da0: 2e30 2e32 0a2d 2d2d 2d2d 0a0a 5b4c 6973  .0.2.-----..[Lis
+00001db0: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
+00001dc0: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+00001dd0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+00001de0: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
+00001df0: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
+00001e00: 652f 3632 3f63 6c6f 7365 643d 3129 0a0a  e/62?closed=1)..
+00001e10: 2323 2320 4275 6766 6978 6573 0a0a 2d20  ### Bugfixes..- 
+00001e20: 556e 6966 6965 6420 7468 6520 7761 7920  Unified the way 
+00001e30: 6048 6561 6c74 6843 6865 636b 6020 6973  `HealthCheck` is
+00001e40: 2063 7265 6174 6564 2f63 6f6e 6669 6775   created/configu
+00001e50: 7265 640a 0a23 2323 204d 6973 6365 6c6c  red..### Miscell
+00001e60: 616e 656f 7573 0a0a 2d20 4275 6d70 6564  aneous..- Bumped
+00001e70: 2076 6572 7369 6f6e 206f 6620 7765 6273   version of webs
+00001e80: 6f63 6b65 742d 636c 6965 6e74 0a0a 342e  ocket-client..4.
+00001e90: 302e 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374  0.1.-----..[List
+00001ea0: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
+00001eb0: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+00001ec0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00001ed0: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
+00001ee0: 6b65 722d 7079 2f6d 696c 6573 746f 6e65  ker-py/milestone
+00001ef0: 2f36 303f 636c 6f73 6564 3d31 290a 0a23  /60?closed=1)..#
+00001f00: 2323 2042 7567 6669 7865 730a 0a2d 2046  ## Bugfixes..- F
+00001f10: 6978 6564 2061 6e20 6f62 736f 6c65 7465  ixed an obsolete
+00001f20: 2069 6d70 6f72 7420 696e 2074 6865 2060   import in the `
+00001f30: 6372 6564 656e 7469 616c 7360 2073 7562  credentials` sub
+00001f40: 7061 636b 6167 6520 7468 6174 2063 6175  package that cau
+00001f50: 7365 6420 696d 706f 7274 2065 7272 6f72  sed import error
+00001f60: 7320 696e 0a20 2050 7974 686f 6e20 332e  s in.  Python 3.
+00001f70: 370a 0a23 2323 204d 6973 6365 6c6c 616e  7..### Miscellan
+00001f80: 656f 7573 0a0a 2d20 446f 6373 2062 7569  eous..- Docs bui
+00001f90: 6c64 696e 6720 6861 7320 6265 656e 2072  lding has been r
+00001fa0: 6570 6169 7265 640a 0a34 2e30 2e30 0a2d  epaired..4.0.0.-
+00001fb0: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
+00001fc0: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
+00001fd0: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+00001fe0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001ff0: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
+00002000: 792f 6d69 6c65 7374 6f6e 652f 3537 3f63  y/milestone/57?c
+00002010: 6c6f 7365 643d 3129 0a0a 2323 2320 4272  losed=1)..### Br
+00002020: 6561 6b69 6e67 2063 6861 6e67 6573 0a0a  eaking changes..
+00002030: 2d20 5375 7070 6f72 7420 666f 7220 5079  - Support for Py
+00002040: 7468 6f6e 2033 2e33 2061 6e64 2050 7974  thon 3.3 and Pyt
+00002050: 686f 6e20 332e 3420 6861 7320 6265 656e  hon 3.4 has been
+00002060: 2064 726f 7070 6564 0a2d 2060 4150 4943   dropped.- `APIC
+00002070: 6c69 656e 742e 7570 6461 7465 5f73 6572  lient.update_ser
+00002080: 7669 6365 602c 2060 4150 4943 6c69 656e  vice`, `APIClien
+00002090: 742e 696e 6974 5f73 7761 726d 602c 2061  t.init_swarm`, a
+000020a0: 6e64 0a20 2060 446f 636b 6572 436c 6965  nd.  `DockerClie
+000020b0: 6e74 2e73 7761 726d 2e69 6e69 7460 206e  nt.swarm.init` n
+000020c0: 6f77 2072 6574 7572 6e20 6120 6064 6963  ow return a `dic
+000020d0: 7460 2066 726f 6d20 7468 6520 4150 4927  t` from the API'
+000020e0: 7320 7265 7370 6f6e 7365 2062 6f64 790a  s response body.
+000020f0: 2d20 496e 2060 4150 4943 6c69 656e 742e  - In `APIClient.
+00002100: 6275 696c 6460 2061 6e64 2060 446f 636b  build` and `Dock
+00002110: 6572 436c 6965 6e74 2e69 6d61 6765 732e  erClient.images.
+00002120: 6275 696c 6460 2c20 7468 6520 6075 7365  build`, the `use
+00002130: 5f63 6f6e 6669 675f 7072 6f78 7960 0a20  _config_proxy`. 
+00002140: 2070 6172 616d 6574 6572 206e 6f77 2064   parameter now d
+00002150: 6566 6175 6c74 7320 746f 2054 7275 650a  efaults to True.
+00002160: 2d20 6069 6e69 745f 7061 7468 6020 6973  - `init_path` is
+00002170: 206e 6f20 6c6f 6e67 6572 2061 2076 616c   no longer a val
+00002180: 6964 2070 6172 616d 6574 6572 2066 6f72  id parameter for
+00002190: 2060 486f 7374 436f 6e66 6967 600a 0a23   `HostConfig`..#
+000021a0: 2323 2046 6561 7475 7265 730a 0a2d 2049  ## Features..- I
+000021b0: 7420 6973 206e 6f77 2070 6f73 7369 626c  t is now possibl
+000021c0: 6520 746f 2070 726f 7669 6465 2060 5343  e to provide `SC
+000021d0: 5450 6020 706f 7274 7320 666f 7220 706f  TP` ports for po
+000021e0: 7274 206d 6170 7069 6e67 730a 2d20 6043  rt mappings.- `C
+000021f0: 6f6e 7461 696e 6572 5370 6563 6073 206e  ontainerSpec`s n
+00002200: 6f77 2073 7570 706f 7274 2074 6865 2060  ow support the `
+00002210: 696e 6974 6020 7061 7261 6d65 7465 720a  init` parameter.
+00002220: 2d20 6044 6f63 6b65 7243 6c69 656e 742e  - `DockerClient.
+00002230: 7377 6172 6d2e 696e 6974 6020 616e 6420  swarm.init` and 
+00002240: 6041 5049 436c 6965 6e74 2e69 6e69 745f  `APIClient.init_
+00002250: 7377 6172 6d60 206e 6f77 2073 7570 706f  swarm` now suppo
+00002260: 7274 2074 6865 0a20 2060 6461 7461 5f70  rt the.  `data_p
+00002270: 6174 685f 6164 6472 6020 7061 7261 6d65  ath_addr` parame
+00002280: 7465 720a 2d20 6041 5049 436c 6965 6e74  ter.- `APIClient
+00002290: 2e75 7064 6174 655f 7377 6172 6d60 2061  .update_swarm` a
+000022a0: 6e64 2060 446f 636b 6572 436c 6965 6e74  nd `DockerClient
+000022b0: 2e73 7761 726d 2e75 7064 6174 6560 206e  .swarm.update` n
+000022c0: 6f77 2073 7570 706f 7274 2074 6865 0a20  ow support the. 
+000022d0: 2060 726f 7461 7465 5f6d 616e 6167 6572   `rotate_manager
+000022e0: 5f75 6e6c 6f63 6b5f 6b65 7960 2070 6172  _unlock_key` par
+000022f0: 616d 6574 6572 0a2d 2060 4150 4943 6c69  ameter.- `APICli
+00002300: 656e 742e 7570 6461 7465 5f73 6572 7669  ent.update_servi
+00002310: 6365 6020 7265 7475 726e 7320 7468 6520  ce` returns the 
+00002320: 4150 4927 7320 7265 7370 6f6e 7365 2062  API's response b
+00002330: 6f64 7920 6173 2061 2060 6469 6374 600a  ody as a `dict`.
+00002340: 2d20 6041 5049 436c 6965 6e74 2e69 6e69  - `APIClient.ini
+00002350: 745f 7377 6172 6d60 2c20 616e 6420 6044  t_swarm`, and `D
+00002360: 6f63 6b65 7243 6c69 656e 742e 7377 6172  ockerClient.swar
+00002370: 6d2e 696e 6974 6020 6e6f 7720 7265 7475  m.init` now retu
+00002380: 726e 2074 6865 2041 5049 2773 0a20 2072  rn the API's.  r
+00002390: 6573 706f 6e73 6520 626f 6479 2061 7320  esponse body as 
+000023a0: 6120 6064 6963 7460 0a0a 2323 2320 4275  a `dict`..### Bu
+000023b0: 6766 6978 6573 0a0a 2d20 4669 7865 6420  gfixes..- Fixed 
+000023c0: 6050 6c61 6365 6d65 6e74 5072 6566 6572  `PlacementPrefer
+000023d0: 656e 6365 6020 696e 7374 616e 6365 7320  ence` instances 
+000023e0: 746f 2070 726f 6475 6365 2061 2076 616c  to produce a val
+000023f0: 6964 2041 5049 2074 7970 650a 2d20 4669  id API type.- Fi
+00002400: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
+00002410: 6e6f 7420 7365 7474 696e 6720 6120 7661  not setting a va
+00002420: 6c75 6520 666f 7220 6062 7569 6c64 6172  lue for `buildar
+00002430: 6773 6020 696e 2060 6275 696c 6460 2063  gs` in `build` c
+00002440: 6f75 6c64 2063 6175 7365 0a20 2074 6865  ould cause.  the
+00002450: 206c 6962 7261 7279 2074 6f20 6174 7465   library to atte
+00002460: 6d70 7420 6163 6365 7373 696e 6720 6174  mpt accessing at
+00002470: 7472 6962 7574 6573 206f 6620 6120 604e  tributes of a `N
+00002480: 6f6e 6560 2076 616c 7565 0a2d 2046 6978  one` value.- Fix
+00002490: 6564 2061 2062 7567 2077 6865 7265 2073  ed a bug where s
+000024a0: 6574 7469 6e67 2074 6865 2060 766f 6c75  etting the `volu
+000024b0: 6d65 5f64 7269 7665 7260 2070 6172 616d  me_driver` param
+000024c0: 6574 6572 2069 6e0a 2020 6044 6f63 6b65  eter in.  `Docke
+000024d0: 7243 6c69 656e 742e 636f 6e74 6169 6e65  rClient.containe
+000024e0: 7273 2e63 7265 6174 6560 2077 6f75 6c64  rs.create` would
+000024f0: 2072 6573 756c 7420 696e 2061 6e20 6572   result in an er
+00002500: 726f 720a 2d20 6041 5049 436c 6965 6e74  ror.- `APIClient
+00002510: 2e69 6e73 7065 6374 5f64 6973 7472 6962  .inspect_distrib
+00002520: 7574 696f 6e60 206e 6f77 2063 6f72 7265  ution` now corre
+00002530: 6374 6c79 2073 6574 7320 7468 6520 6175  ctly sets the au
+00002540: 7468 656e 7469 6361 7469 6f6e 0a20 2068  thentication.  h
+00002550: 6561 6465 7273 206f 6e20 7468 6520 7265  eaders on the re
+00002560: 7175 6573 742c 2061 6c6c 6f77 696e 6720  quest, allowing 
+00002570: 6974 2074 6f20 6265 2075 7365 6420 7769  it to be used wi
+00002580: 7468 2070 7269 7661 7465 2072 6570 6f73  th private repos
+00002590: 6974 6f72 6965 730a 2020 5468 6973 2063  itories.  This c
+000025a0: 6861 6e67 6520 616c 736f 2061 7070 6c69  hange also appli
+000025b0: 6573 2074 6f20 6044 6f63 6b65 7243 6c69  es to `DockerCli
+000025c0: 656e 742e 6765 745f 7265 6769 7374 7279  ent.get_registry
+000025d0: 5f64 6174 6160 0a0a 332e 372e 320a 2d2d  _data`..3.7.2.--
+000025e0: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
+000025f0: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
+00002600: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+00002610: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002620: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
+00002630: 2f6d 696c 6573 746f 6e65 2f35 393f 636c  /milestone/59?cl
+00002640: 6f73 6564 3d31 290a 0a23 2323 2042 7567  osed=1)..### Bug
+00002650: 6669 7865 730a 0a2a 2046 6978 2062 6173  fixes..* Fix bas
+00002660: 655f 7572 6c20 746f 206b 6565 7020 5443  e_url to keep TC
+00002670: 5020 7072 6f74 6f63 6f6c 206f 6e20 7574  P protocol on ut
+00002680: 696c 732e 7079 2062 7920 6c65 7474 696e  ils.py by lettin
+00002690: 6720 7468 6520 7265 7370 6f6e 7369 6269  g the responsibi
+000026a0: 6c69 7479 206f 6620 6368 616e 6769 6e67  lity of changing
+000026b0: 2074 6865 0a70 726f 746f 636f 6c20 746f   the.protocol to
+000026c0: 2060 7061 7273 655f 686f 7374 6020 6166   `parse_host` af
+000026d0: 7465 7277 6172 6473 2c20 6c65 7474 696e  terwards, lettin
+000026e0: 6720 6062 6173 655f 7572 6c60 2077 6974  g `base_url` wit
+000026f0: 6820 7468 6520 6f72 6967 696e 616c 2076  h the original v
+00002700: 616c 7565 2e0a 2a20 5846 4149 4c20 7465  alue..* XFAIL te
+00002710: 7374 5f61 7474 6163 685f 7374 7265 616d  st_attach_stream
+00002720: 5f61 6e64 5f63 616e 6365 6c20 6f6e 2054  _and_cancel on T
+00002730: 4c53 0a0a 332e 372e 310a 2d2d 2d2d 2d0a  LS..3.7.1.-----.
+00002740: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
+00002750: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
+00002760: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
+00002770: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
+00002780: 6572 2f64 6f63 6b65 722d 7079 2f6d 696c  er/docker-py/mil
+00002790: 6573 746f 6e65 2f35 383f 636c 6f73 6564  estone/58?closed
+000027a0: 3d31 290a 0a23 2323 2042 7567 6669 7865  =1)..### Bugfixe
+000027b0: 730a 0a2a 2053 6574 2061 2064 6966 6665  s..* Set a diffe
+000027c0: 7265 6e74 2064 6566 6175 6c74 206e 756d  rent default num
+000027d0: 6265 7220 2877 6869 6368 2069 7320 6e6f  ber (which is no
+000027e0: 7720 3929 2066 6f72 2053 5348 2070 6f6f  w 9) for SSH poo
+000027f0: 6c73 0a2a 2041 6464 7320 6120 4261 7365  ls.* Adds a Base
+00002800: 4854 5450 4164 6170 7465 7220 7769 7468  HTTPAdapter with
+00002810: 2061 2063 6c6f 7365 206d 6574 686f 6420   a close method 
+00002820: 746f 2065 6e73 7572 6520 7468 6174 2074  to ensure that t
+00002830: 6865 0a70 6f6f 6c73 2069 7320 636c 6561  he.pools is clea
+00002840: 6e20 6f6e 2063 6c6f 7365 2829 0a2a 204d  n on close().* M
+00002850: 616b 6573 2053 5348 4854 5450 4164 6170  akes SSHHTTPAdap
+00002860: 7465 7220 7265 6f70 656e 2061 2063 6c6f  ter reopen a clo
+00002870: 7365 6420 636f 6e6e 6563 7469 6f6e 2077  sed connection w
+00002880: 6865 6e20 6e65 6564 6564 0a6c 696b 6520  hen needed.like 
+00002890: 7468 6520 6f74 6865 7273 0a0a 332e 372e  the others..3.7.
+000028a0: 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f  0.-----..[List o
+000028b0: 6620 5052 7320 2f20 6973 7375 6573 2066  f PRs / issues f
+000028c0: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
+000028d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000028e0: 636f 6d2f 646f 636b 6572 2f64 6f63 6b65  com/docker/docke
+000028f0: 722d 7079 2f6d 696c 6573 746f 6e65 2f35  r-py/milestone/5
+00002900: 363f 636c 6f73 6564 3d31 290a 0a23 2323  6?closed=1)..###
+00002910: 2046 6561 7475 7265 730a 0a2a 2041 6464   Features..* Add
+00002920: 6564 2073 7570 706f 7274 2066 6f72 206d  ed support for m
+00002930: 756c 7469 706c 6578 6564 2073 7472 6561  ultiplexed strea
+00002940: 6d73 2028 666f 7220 6061 7474 6163 6860  ms (for `attach`
+00002950: 2061 6e64 2060 6578 6563 5f73 7461 7274   and `exec_start
+00002960: 6029 2e20 4c65 6172 6e0a 2020 6d6f 7265  `). Learn.  more
+00002970: 2061 7420 6874 7470 733a 2f2f 646f 636b   at https://dock
+00002980: 6572 2d70 792e 7265 6164 7468 6564 6f63  er-py.readthedoc
+00002990: 732e 696f 2f65 6e2f 7374 6162 6c65 2f75  s.io/en/stable/u
+000029a0: 7365 725f 6775 6964 6573 2f6d 756c 7469  ser_guides/multi
+000029b0: 706c 6578 2e68 746d 6c0a 2a20 4164 6465  plex.html.* Adde
+000029c0: 6420 7468 6520 6075 7365 5f63 6f6e 6669  d the `use_confi
+000029d0: 675f 7072 6f78 7960 2070 6172 616d 6574  g_proxy` paramet
+000029e0: 6572 2074 6f20 7468 6520 666f 6c6c 6f77  er to the follow
+000029f0: 696e 6720 6d65 7468 6f64 733a 0a20 2060  ing methods:.  `
+00002a00: 4150 4943 6c69 656e 742e 6275 696c 6460  APIClient.build`
+00002a10: 2c20 6041 5049 436c 6965 6e74 2e63 7265  , `APIClient.cre
+00002a20: 6174 655f 636f 6e74 6169 6e65 7260 2c20  ate_container`, 
+00002a30: 6044 6f63 6b65 7243 6c69 656e 742e 696d  `DockerClient.im
+00002a40: 6167 6573 2e62 7569 6c64 600a 2020 616e  ages.build`.  an
+00002a50: 6420 6044 6f63 6b65 7243 6c69 656e 742e  d `DockerClient.
+00002a60: 636f 6e74 6169 6e65 7273 2e72 756e 6020  containers.run` 
+00002a70: 2860 4661 6c73 6560 2062 7920 6465 6661  (`False` by defa
+00002a80: 756c 7429 2e20 2a2a 5468 6973 2070 6172  ult). **This par
+00002a90: 616d 6574 6572 2a2a 0a20 202a 2a77 696c  ameter**.  **wil
+00002aa0: 6c20 6265 636f 6d65 2060 5472 7565 6020  l become `True` 
+00002ab0: 6279 2064 6566 6175 6c74 2069 6e20 7468  by default in th
+00002ac0: 6520 342e 302e 3020 7265 6c65 6173 652e  e 4.0.0 release.
+00002ad0: 2a2a 0a2a 2050 6c61 6365 6d65 6e74 2070  **.* Placement p
+00002ae0: 7265 6665 7265 6e63 6573 2066 6f72 2053  references for S
+00002af0: 7761 726d 2073 6572 7669 6365 7320 6172  warm services ar
+00002b00: 6520 6265 7474 6572 2076 616c 6964 6174  e better validat
+00002b10: 6564 206f 6e20 7468 6520 636c 6965 6e74  ed on the client
+00002b20: 0a20 2061 6e64 2064 6f63 756d 656e 7461  .  and documenta
+00002b30: 7469 6f6e 2068 6173 2062 6565 6e20 7570  tion has been up
+00002b40: 6461 7465 6420 6163 636f 7264 696e 676c  dated accordingl
+00002b50: 790a 0a23 2323 2042 7567 6669 7865 730a  y..### Bugfixes.
+00002b60: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00002b70: 6865 7265 2063 7265 6465 6e74 6961 6c20  here credential 
+00002b80: 7374 6f72 6573 2077 6572 656e 2774 2071  stores weren't q
+00002b90: 7565 7269 6564 2066 6f72 2072 656c 6576  ueried for relev
+00002ba0: 616e 7420 7265 6769 7374 7279 0a20 2063  ant registry.  c
+00002bb0: 7265 6465 6e74 6961 6c73 2077 6974 6820  redentials with 
+00002bc0: 6365 7274 6169 6e20 7661 7269 6174 696f  certain variatio
+00002bd0: 6e73 206f 6620 7468 6520 6063 6f6e 6669  ns of the `confi
+00002be0: 672e 6a73 6f6e 6020 6669 6c65 2e0a 2a20  g.json` file..* 
+00002bf0: 6044 6f63 6b65 7243 6c69 656e 742e 7377  `DockerClient.sw
+00002c00: 6172 6d2e 696e 6974 6020 6e6f 7720 7265  arm.init` now re
+00002c10: 7475 726e 7320 6120 626f 6f6c 6561 6e20  turns a boolean 
+00002c20: 7661 6c75 6520 6173 2061 6476 6572 7469  value as adverti
+00002c30: 7365 642e 0a0a 332e 362e 300a 2d2d 2d2d  sed...3.6.0.----
+00002c40: 2d0a 0a5b 4c69 7374 206f 6620 5052 7320  -..[List of PRs 
+00002c50: 2f20 6973 7375 6573 2066 6f72 2074 6869  / issues for thi
+00002c60: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
+00002c70: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
+00002c80: 636b 6572 2f64 6f63 6b65 722d 7079 2f6d  cker/docker-py/m
+00002c90: 696c 6573 746f 6e65 3d35 353f 636c 6f73  ilestone=55?clos
+00002ca0: 6564 3d31 290a 0a23 2323 2046 6561 7475  ed=1)..### Featu
+00002cb0: 7265 730a 0a2a 2041 6464 6564 2073 7570  res..* Added sup
+00002cc0: 706f 7274 2066 6f72 2063 6f6e 6e65 6374  port for connect
+00002cd0: 696e 6720 746f 2074 6865 2044 6f63 6b65  ing to the Docke
+00002ce0: 7220 456e 6769 6e65 206f 7665 7220 5353  r Engine over SS
+00002cf0: 482e 2041 6464 6974 696f 6e61 6c0a 2020  H. Additional.  
+00002d00: 6465 7065 6e64 656e 6369 6573 2066 6f72  dependencies for
+00002d10: 2074 6869 7320 6665 6174 7572 6520 6361   this feature ca
+00002d20: 6e20 6265 2069 6e73 7461 6c6c 6564 2077  n be installed w
+00002d30: 6974 680a 2020 6070 6970 2069 6e73 7461  ith.  `pip insta
+00002d40: 6c6c 2022 646f 636b 6572 5b73 7368 5d22  ll "docker[ssh]"
+00002d50: 600a 2a20 4164 6465 6420 7375 7070 6f72  `.* Added suppor
+00002d60: 7420 666f 7220 7468 6520 606e 616d 6564  t for the `named
+00002d70: 6020 7061 7261 6d65 7465 7220 696e 2060  ` parameter in `
+00002d80: 496d 6167 652e 7361 7665 602c 2077 6869  Image.save`, whi
+00002d90: 6368 206d 6179 2062 650a 2020 7573 6564  ch may be.  used
+00002da0: 2074 6f20 656e 7375 7265 2074 6865 2072   to ensure the r
+00002db0: 6573 756c 7469 6e67 2074 6172 6261 6c6c  esulting tarball
+00002dc0: 2072 6574 6169 6e73 2074 6865 2069 6d61   retains the ima
+00002dd0: 6765 2773 206e 616d 6520 6f6e 2073 6176  ge's name on sav
+00002de0: 652e 0a0a 2323 2320 4275 6766 6978 6573  e...### Bugfixes
+00002df0: 0a0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+00002e00: 7768 6572 6520 6275 696c 6473 206f 6e20  where builds on 
+00002e10: 5769 6e64 6f77 7320 7769 7468 2061 2063  Windows with a c
+00002e20: 6f6e 7465 7874 2070 6174 6820 7573 696e  ontext path usin
+00002e30: 6720 7468 6520 605c 5c3f 5c60 0a20 2070  g the `\\?\`.  p
+00002e40: 7265 6669 7820 776f 756c 6420 6661 696c  refix would fail
+00002e50: 2077 6974 6820 736f 6d65 2072 656c 6174   with some relat
+00002e60: 6976 6520 446f 636b 6572 6669 6c65 2070  ive Dockerfile p
+00002e70: 6174 6873 2e0a 2a20 4669 7865 6420 616e  aths..* Fixed an
+00002e80: 2069 7373 7565 2077 6865 7265 2070 756c   issue where pul
+00002e90: 6c73 206d 6164 6520 7769 7468 2074 6865  ls made with the
+00002ea0: 2060 446f 636b 6572 436c 6965 6e74 6020   `DockerClient` 
+00002eb0: 776f 756c 6420 6661 696c 2077 6865 6e0a  would fail when.
+00002ec0: 2020 7365 7474 696e 6720 7468 6520 6073    setting the `s
+00002ed0: 7472 6561 6d60 2070 6172 616d 6574 6572  tream` parameter
+00002ee0: 2074 6f20 6054 7275 6560 2e0a 0a23 2323   to `True`...###
+00002ef0: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
+00002f00: 2a20 5468 6520 6d69 6e69 6d75 6d20 7265  * The minimum re
+00002f10: 7175 6972 656d 656e 7420 666f 7220 7468  quirement for th
+00002f20: 6520 6072 6571 7565 7374 7360 2064 6570  e `requests` dep
+00002f30: 656e 6465 6e63 7920 6861 7320 6265 656e  endency has been
+00002f40: 2062 756d 7065 640a 2020 746f 2032 2e32   bumped.  to 2.2
+00002f50: 302e 300a 0a33 2e35 2e31 0a2d 2d2d 2d2d  0.0..3.5.1.-----
+00002f60: 0a0a 5b4c 6973 7420 6f66 2050 5273 202f  ..[List of PRs /
+00002f70: 2069 7373 7565 7320 666f 7220 7468 6973   issues for this
+00002f80: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+00002f90: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
+00002fa0: 6b65 722f 646f 636b 6572 2d70 792f 6d69  ker/docker-py/mi
+00002fb0: 6c65 7374 6f6e 652f 3534 3f63 6c6f 7365  lestone/54?close
+00002fc0: 643d 3129 0a0a 2323 2320 4d69 7363 656c  d=1)..### Miscel
+00002fd0: 6c61 6e65 6f75 730a 0a2a 2042 756d 7065  laneous..* Bumpe
+00002fe0: 6420 7665 7273 696f 6e20 6f66 2060 7079  d version of `py
+00002ff0: 4f70 656e 5353 4c60 2069 6e20 6072 6571  OpenSSL` in `req
+00003000: 7569 7265 6d65 6e74 732e 7478 7460 2061  uirements.txt` a
+00003010: 6e64 2060 7365 7475 702e 7079 6020 746f  nd `setup.py` to
+00003020: 2070 7265 7665 6e74 0a20 2069 6e73 7461   prevent.  insta
+00003030: 6c6c 6174 696f 6e20 6f66 2061 2076 756c  llation of a vul
+00003040: 6e65 7261 626c 6520 7665 7273 696f 6e0a  nerable version.
+00003050: 0a2a 2044 6f63 7320 6669 7865 730a 0a33  .* Docs fixes..3
+00003060: 2e35 2e30 0a2d 2d2d 2d2d 0a0a 5b4c 6973  .5.0.-----..[Lis
+00003070: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
+00003080: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+00003090: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+000030a0: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
+000030b0: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
+000030c0: 652f 3533 3f63 6c6f 7365 643d 3129 0a0a  e/53?closed=1)..
+000030d0: 2323 2320 4465 7072 6563 6174 696f 6e20  ### Deprecation 
+000030e0: 7761 726e 696e 670a 0a2a 2053 7570 706f  warning..* Suppo
+000030f0: 7274 2066 6f72 2050 7974 686f 6e20 332e  rt for Python 3.
+00003100: 3320 7769 6c6c 2062 6520 6472 6f70 7065  3 will be droppe
+00003110: 6420 696e 2074 6865 2034 2e30 2e30 2072  d in the 4.0.0 r
+00003120: 656c 6561 7365 0a0a 2323 2320 4665 6174  elease..### Feat
+00003130: 7572 6573 0a0a 2a20 5570 6461 7465 6420  ures..* Updated 
+00003140: 6465 7065 6e64 656e 6369 6573 2074 6f20  dependencies to 
+00003150: 656e 7375 7265 2073 7570 706f 7274 2066  ensure support f
+00003160: 6f72 2050 7974 686f 6e20 332e 3720 656e  or Python 3.7 en
+00003170: 7669 726f 6e6d 656e 7473 0a2a 2041 6464  vironments.* Add
+00003180: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
+00003190: 6865 2060 7574 735f 6d6f 6465 6020 7061  he `uts_mode` pa
+000031a0: 7261 6d65 7465 7220 696e 2060 486f 7374  rameter in `Host
+000031b0: 436f 6e66 6967 600a 2a20 5468 6520 6055  Config`.* The `U
+000031c0: 7064 6174 6543 6f6e 6669 6760 2063 6f6e  pdateConfig` con
+000031d0: 7374 7275 6374 6f72 206e 6f77 2061 6c6c  structor now all
+000031e0: 6f77 7320 6072 6f6c 6c62 6163 6b60 2061  ows `rollback` a
+000031f0: 7320 6120 7661 6c69 640a 2020 7661 6c75  s a valid.  valu
+00003200: 6520 666f 7220 6066 6169 6c75 7265 5f61  e for `failure_a
+00003210: 6374 696f 6e60 0a2a 2041 6464 6564 2073  ction`.* Added s
+00003220: 7570 706f 7274 2066 6f72 2060 726f 6c6c  upport for `roll
+00003230: 6261 636b 5f63 6f6e 6669 6760 2069 6e20  back_config` in 
+00003240: 6041 5049 436c 6965 6e74 2e63 7265 6174  `APIClient.creat
+00003250: 655f 7365 7276 6963 6560 2c0a 2020 6041  e_service`,.  `A
+00003260: 5049 436c 6965 6e74 2e75 7064 6174 655f  PIClient.update_
+00003270: 7365 7276 6963 6560 2c20 6044 6f63 6b65  service`, `Docke
+00003280: 7243 6c69 656e 742e 7365 7276 6963 6573  rClient.services
+00003290: 2e63 7265 6174 6560 2061 6e64 0a20 2060  .create` and.  `
+000032a0: 5365 7276 6963 652e 7570 6461 7465 602e  Service.update`.
+000032b0: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
+000032c0: 2a20 4372 6564 656e 7469 616c 2068 656c  * Credential hel
+000032d0: 7065 7273 2061 7265 206e 6f77 2070 726f  pers are now pro
+000032e0: 7065 726c 7920 6c65 7665 7261 6765 6420  perly leveraged 
+000032f0: 6279 2074 6865 2060 6275 696c 6460 206d  by the `build` m
+00003300: 6574 686f 640a 2a20 4669 7865 6420 6120  ethod.* Fixed a 
+00003310: 6275 6720 7468 6174 2063 6175 7365 6420  bug that caused 
+00003320: 706c 6163 656d 656e 7420 7072 6566 6572  placement prefer
+00003330: 656e 6365 7320 746f 2062 6520 6967 6e6f  ences to be igno
+00003340: 7265 6420 7768 656e 2070 726f 7669 6465  red when provide
+00003350: 640a 2020 746f 2060 446f 636b 6572 436c  d.  to `DockerCl
+00003360: 6965 6e74 2e73 6572 7669 6365 732e 6372  ient.services.cr
+00003370: 6561 7465 600a 2a20 4669 7865 6420 6120  eate`.* Fixed a 
+00003380: 6275 6720 7468 6174 2063 6175 7365 6420  bug that caused 
+00003390: 6120 6075 7365 7260 2076 616c 7565 206f  a `user` value o
+000033a0: 6620 6030 6020 746f 2062 6520 6967 6e6f  f `0` to be igno
+000033b0: 7265 6420 696e 0a20 2060 4150 4943 6c69  red in.  `APICli
+000033c0: 656e 742e 6372 6561 7465 5f63 6f6e 7461  ent.create_conta
+000033d0: 696e 6572 6020 616e 6420 6044 6f63 6b65  iner` and `Docke
+000033e0: 7243 6c69 656e 742e 636f 6e74 6169 6e65  rClient.containe
+000033f0: 7273 2e63 7265 6174 6560 0a0a 332e 342e  rs.create`..3.4.
+00003400: 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f  1.-----..[List o
+00003410: 6620 5052 7320 2f20 6973 7375 6573 2066  f PRs / issues f
+00003420: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
+00003430: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003440: 636f 6d2f 646f 636b 6572 2f64 6f63 6b65  com/docker/docke
+00003450: 722d 7079 2f6d 696c 6573 746f 6e65 2f35  r-py/milestone/5
+00003460: 323f 636c 6f73 6564 3d31 290a 0a23 2323  2?closed=1)..###
+00003470: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
+00003480: 6564 2061 2062 7567 2074 6861 7420 6361  ed a bug that ca
+00003490: 7573 6564 2061 7574 6820 7661 6c75 6573  used auth values
+000034a0: 2069 6e20 636f 6e66 6967 2066 696c 6573   in config files
+000034b0: 2077 7269 7474 656e 2075 7369 6e67 206f   written using o
+000034c0: 6e65 206f 6620 7468 650a 2020 6c65 6761  ne of the.  lega
+000034d0: 6379 2066 6f72 6d61 7473 2074 6f20 6265  cy formats to be
+000034e0: 2069 676e 6f72 6564 0a2a 2046 6978 6564   ignored.* Fixed
+000034f0: 2069 7373 7565 7320 7769 7468 2068 616e   issues with han
+00003500: 646c 696e 6720 6f66 2064 6f75 626c 652d  dling of double-
+00003510: 7769 6c64 6361 7264 2060 2a2a 6020 7061  wildcard `**` pa
+00003520: 7474 6572 6e73 2069 6e0a 2020 602e 646f  tterns in.  `.do
+00003530: 636b 6572 6967 6e6f 7265 6020 6669 6c65  ckerignore` file
+00003540: 730a 0a33 2e34 2e30 0a2d 2d2d 2d2d 0a0a  s..3.4.0.-----..
+00003550: 5b4c 6973 7420 6f66 2050 5273 202f 2069  [List of PRs / i
+00003560: 7373 7565 7320 666f 7220 7468 6973 2072  ssues for this r
+00003570: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00003580: 6769 7468 7562 2e63 6f6d 2f64 6f63 6b65  github.com/docke
+00003590: 722f 646f 636b 6572 2d70 792f 6d69 6c65  r/docker-py/mile
+000035a0: 7374 6f6e 652f 3531 3f63 6c6f 7365 643d  stone/51?closed=
+000035b0: 3129 0a0a 2323 2320 4665 6174 7572 6573  1)..### Features
+000035c0: 0a0a 2a20 5468 6520 6041 5049 436c 6965  ..* The `APIClie
+000035d0: 6e74 6020 616e 6420 6044 6f63 6b65 7243  nt` and `DockerC
+000035e0: 6c69 656e 7460 2063 6f6e 7374 7275 6374  lient` construct
+000035f0: 6f72 7320 6e6f 7720 6163 6365 7074 2061  ors now accept a
+00003600: 2060 6372 6564 7374 6f72 655f 656e 7660   `credstore_env`
+00003610: 0a20 2070 6172 616d 6574 6572 2e20 5768  .  parameter. Wh
+00003620: 656e 2073 6574 2c20 7661 6c75 6573 2069  en set, values i
+00003630: 6e20 7468 6973 2064 6963 7469 6f6e 6172  n this dictionar
+00003640: 7920 6172 6520 6164 6465 6420 746f 2074  y are added to t
+00003650: 6865 2065 6e76 6972 6f6e 6d65 6e74 0a20  he environment. 
+00003660: 2077 6865 6e20 6578 6563 7574 696e 6720   when executing 
+00003670: 7468 6520 6372 6564 656e 7469 616c 2073  the credential s
+00003680: 746f 7265 2070 726f 6365 7373 2e0a 0a23  tore process...#
+00003690: 2323 2042 7567 6669 7865 730a 0a2a 2060  ## Bugfixes..* `
+000036a0: 446f 636b 6572 436c 6965 6e74 2e6e 6574  DockerClient.net
+000036b0: 776f 726b 732e 7072 756e 6560 206e 6f77  works.prune` now
+000036c0: 2070 726f 7065 726c 7920 7265 7475 726e   properly return
+000036d0: 7320 7468 6520 6f70 6572 6174 696f 6e27  s the operation'
+000036e0: 7320 7265 7375 6c74 0a2a 2046 6978 6564  s result.* Fixed
+000036f0: 2061 2062 7567 2074 6861 7420 6361 7573   a bug that caus
+00003700: 6564 2063 7573 746f 6d20 446f 636b 6572  ed custom Docker
+00003710: 6669 6c65 2070 6174 6873 2069 6e20 6120  file paths in a 
+00003720: 7375 6266 6f6c 6465 7220 6f66 2074 6865  subfolder of the
+00003730: 2062 7569 6c64 0a20 2063 6f6e 7465 7874   build.  context
+00003740: 2074 6f20 6265 2069 6e76 616c 6964 6174   to be invalidat
+00003750: 6564 2c20 7072 6576 656e 7469 6e67 2074  ed, preventing t
+00003760: 6865 7365 2062 7569 6c64 7320 6672 6f6d  hese builds from
+00003770: 2077 6f72 6b69 6e67 0a2a 2054 6865 2060   working.* The `
+00003780: 706c 7567 696e 5f70 7269 7669 6c65 6765  plugin_privilege
+00003790: 7360 206d 6574 686f 6420 6361 6e20 6e6f  s` method can no
+000037a0: 7720 6265 2063 616c 6c65 6420 666f 7220  w be called for 
+000037b0: 706c 7567 696e 7320 7265 7175 6972 696e  plugins requirin
+000037c0: 670a 2020 6175 7468 656e 7469 6361 7469  g.  authenticati
+000037d0: 6f6e 2074 6f20 6163 6365 7373 0a2a 2046  on to access.* F
+000037e0: 6978 6564 2061 2062 7567 2074 6861 7420  ixed a bug that 
+000037f0: 6361 7573 6564 2061 7474 656d 7074 7320  caused attempts 
+00003800: 746f 2072 6561 6420 6120 6461 7461 2073  to read a data s
+00003810: 7472 6561 6d20 6f76 6572 2061 6e20 756e  tream over an un
+00003820: 7365 6375 7265 6420 5443 500a 2020 736f  secured TCP.  so
+00003830: 636b 6574 2074 6f20 6372 6173 6820 6f6e  cket to crash on
+00003840: 2057 696e 646f 7773 2063 6c69 656e 7473   Windows clients
+00003850: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00003860: 6865 7265 2075 7369 6e67 2074 6865 2060  here using the `
+00003870: 7265 6164 5f6f 6e6c 7960 2070 6172 616d  read_only` param
+00003880: 6574 6572 2077 6865 6e20 6372 6561 7469  eter when creati
+00003890: 6e67 2061 2073 6572 7669 6365 2075 7369  ng a service usi
+000038a0: 6e67 0a20 2074 6865 2060 446f 636b 6572  ng.  the `Docker
+000038b0: 436c 6965 6e74 6020 7761 7320 6265 696e  Client` was bein
+000038c0: 6720 6967 6e6f 7265 640a 2a20 4669 7865  g ignored.* Fixe
+000038d0: 6420 616e 2069 7373 7565 2077 6865 7265  d an issue where
+000038e0: 2060 5365 7276 6963 652e 7363 616c 6560   `Service.scale`
+000038f0: 2077 6f75 6c64 206e 6f74 2070 726f 7065   would not prope
+00003900: 726c 7920 7570 6461 7465 2074 6865 2073  rly update the s
+00003910: 6572 7669 6365 2773 0a20 206d 6f64 652c  ervice's.  mode,
+00003920: 2063 6175 7369 6e67 2074 6865 206f 7065   causing the ope
+00003930: 7261 7469 6f6e 2074 6f20 6661 696c 2073  ration to fail s
+00003940: 696c 656e 746c 790a 0a33 2e33 2e30 0a2d  ilently..3.3.0.-
+00003950: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
+00003960: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
+00003970: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+00003980: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003990: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
+000039a0: 792f 6d69 6c65 7374 6f6e 652f 3439 3f63  y/milestone/49?c
+000039b0: 6c6f 7365 643d 3129 0a0a 2323 2320 4665  losed=1)..### Fe
+000039c0: 6174 7572 6573 0a0a 2a20 4164 6465 6420  atures..* Added 
+000039d0: 7375 7070 6f72 7420 666f 7220 6070 7275  support for `pru
+000039e0: 6e65 5f62 7569 6c64 7360 2069 6e20 6041  ne_builds` in `A
+000039f0: 5049 436c 6965 6e74 6020 616e 6420 6044  PIClient` and `D
+00003a00: 6f63 6b65 7243 6c69 656e 742e 696d 6167  ockerClient.imag
+00003a10: 6573 600a 2a20 4164 6465 6420 7375 7070  es`.* Added supp
+00003a20: 6f72 7420 666f 7220 6069 676e 6f72 655f  ort for `ignore_
+00003a30: 7265 6d6f 7665 6460 2070 6172 616d 6574  removed` paramet
+00003a40: 6572 2069 6e0a 2020 6044 6f63 6b65 7243  er in.  `DockerC
+00003a50: 6c69 656e 742e 636f 6e74 6169 6e65 7273  lient.containers
+00003a60: 2e6c 6973 7460 0a0a 2323 2320 4275 6766  .list`..### Bugf
+00003a70: 6978 6573 0a0a 2a20 4669 7865 6420 616e  ixes..* Fixed an
+00003a80: 2069 7373 7565 2074 6861 7420 6361 7573   issue that caus
+00003a90: 6564 2062 7569 6c64 7320 746f 2066 6169  ed builds to fai
+00003aa0: 6c20 7768 656e 2061 6e20 696e 2d63 6f6e  l when an in-con
+00003ab0: 7465 7874 2044 6f63 6b65 7266 696c 650a  text Dockerfile.
+00003ac0: 2020 776f 756c 6420 6265 2073 7065 6369    would be speci
+00003ad0: 6669 6564 2075 7369 6e67 2069 7473 2061  fied using its a
+00003ae0: 6273 6f6c 7574 6520 7061 7468 0a2a 2049  bsolute path.* I
+00003af0: 6e73 7461 6c6c 6174 696f 6e20 7769 7468  nstallation with
+00003b00: 2070 6970 2031 302e 302e 3020 616e 6420   pip 10.0.0 and 
+00003b10: 6162 6f76 6520 6e6f 206c 6f6e 6765 7220  above no longer 
+00003b20: 6661 696c 730a 2a20 436f 6e6e 6563 7469  fails.* Connecti
+00003b30: 6f6e 2074 696d 656f 7574 2066 6f72 2060  on timeout for `
+00003b40: 7374 6f70 6020 616e 6420 6072 6573 7461  stop` and `resta
+00003b50: 7274 6020 6e6f 7720 6765 7473 2070 726f  rt` now gets pro
+00003b60: 7065 726c 7920 6164 6a75 7374 6564 2074  perly adjusted t
+00003b70: 6f0a 2020 616c 6c6f 7720 666f 7220 7468  o.  allow for th
+00003b80: 6520 6f70 6572 6174 696f 6e20 746f 2066  e operation to f
+00003b90: 696e 6973 6820 696e 2074 6865 2073 7065  inish in the spe
+00003ba0: 6369 6669 6564 2074 696d 650a 2a20 496d  cified time.* Im
+00003bb0: 7072 6f76 6564 2064 6f63 6b65 7220 6372  proved docker cr
+00003bc0: 6564 656e 7469 616c 2073 746f 7265 2073  edential store s
+00003bd0: 7570 706f 7274 206f 6e20 5769 6e64 6f77  upport on Window
+00003be0: 730a 0a33 2e32 2e31 0a2d 2d2d 2d2d 0a0a  s..3.2.1.-----..
+00003bf0: 5b4c 6973 7420 6f66 2050 5273 202f 2069  [List of PRs / i
+00003c00: 7373 7565 7320 666f 7220 7468 6973 2072  ssues for this r
+00003c10: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00003c20: 6769 7468 7562 2e63 6f6d 2f64 6f63 6b65  github.com/docke
+00003c30: 722f 646f 636b 6572 2d70 792f 6d69 6c65  r/docker-py/mile
+00003c40: 7374 6f6e 652f 3530 3f63 6c6f 7365 643d  stone/50?closed=
+00003c50: 3129 0a0a 2323 2320 4275 6766 6978 6573  1)..### Bugfixes
+00003c60: 0a0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+00003c70: 7769 7468 2062 7569 6c64 7320 6e6f 7420  with builds not 
+00003c80: 7072 6f70 6572 6c79 2069 6465 6e74 6966  properly identif
+00003c90: 7969 6e67 2044 6f63 6b65 7266 696c 6520  ying Dockerfile 
+00003ca0: 7061 7468 7320 7265 6c61 7469 7665 0a20  paths relative. 
+00003cb0: 2074 6f20 7468 6520 6275 696c 6420 636f   to the build co
+00003cc0: 6e74 6578 740a 2a20 4669 7865 6420 616e  ntext.* Fixed an
+00003cd0: 2069 7373 7565 2077 6865 7265 2062 7569   issue where bui
+00003ce0: 6c64 7320 776f 756c 6420 7261 6973 6520  lds would raise 
+00003cf0: 6120 6056 616c 7565 4572 726f 7260 2077  a `ValueError` w
+00003d00: 6865 6e20 6174 7465 6d70 7469 6e67 2074  hen attempting t
+00003d10: 6f0a 2020 6275 696c 6420 7769 7468 2061  o.  build with a
+00003d20: 2044 6f63 6b65 7266 696c 6520 6f6e 2061   Dockerfile on a
+00003d30: 2064 6966 6665 7265 6e74 2057 696e 646f   different Windo
+00003d40: 7773 2064 7269 7665 2e0a 0a33 2e32 2e30  ws drive...3.2.0
+00003d50: 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66  .-----..[List of
+00003d60: 2050 5273 202f 2069 7373 7565 7320 666f   PRs / issues fo
+00003d70: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
+00003d80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003d90: 6f6d 2f64 6f63 6b65 722f 646f 636b 6572  om/docker/docker
+00003da0: 2d70 792f 6d69 6c65 7374 6f6e 652f 3435  -py/milestone/45
+00003db0: 3f63 6c6f 7365 643d 3129 0a0a 2323 2320  ?closed=1)..### 
+00003dc0: 4665 6174 7572 6573 0a0a 2a20 4765 6e65  Features..* Gene
+00003dd0: 7261 746f 7273 2072 6574 7572 6e65 6420  rators returned 
+00003de0: 6279 2060 6174 7461 6368 2829 602c 2060  by `attach()`, `
+00003df0: 6c6f 6773 2829 6020 616e 6420 6065 7665  logs()` and `eve
+00003e00: 6e74 7328 2960 206e 6f77 2068 6176 6520  nts()` now have 
+00003e10: 610a 2020 6063 616e 6365 6c28 2960 206d  a.  `cancel()` m
+00003e20: 6574 686f 6420 746f 206c 6574 2063 6f6e  ethod to let con
+00003e30: 7375 6d65 7273 2073 746f 7020 7468 6520  sumers stop the 
+00003e40: 6974 6572 6174 696f 6e20 636c 6965 6e74  iteration client
+00003e50: 2d73 6964 652e 0a2a 2060 6275 696c 6428  -side..* `build(
+00003e60: 2960 206d 6574 686f 6473 2063 616e 206e  )` methods can n
+00003e70: 6f77 2068 616e 646c 6520 446f 636b 6572  ow handle Docker
+00003e80: 6669 6c65 7320 7375 7070 6c69 6564 206f  files supplied o
+00003e90: 7574 7369 6465 206f 6620 7468 650a 2020  utside of the.  
+00003ea0: 6275 696c 6420 636f 6e74 6578 742e 0a2a  build context..*
+00003eb0: 2041 6464 6564 2060 7370 6172 7365 6020   Added `sparse` 
+00003ec0: 6172 6775 6d65 6e74 2074 6f20 6044 6f63  argument to `Doc
+00003ed0: 6b65 7243 6c69 656e 742e 636f 6e74 6169  kerClient.contai
+00003ee0: 6e65 7273 2e6c 6973 7428 2960 0a2a 2041  ners.list()`.* A
+00003ef0: 6464 6564 2060 6973 6f6c 6174 696f 6e60  dded `isolation`
+00003f00: 2070 6172 616d 6574 6572 2074 6f20 6062   parameter to `b
+00003f10: 7569 6c64 2829 6020 6d65 7468 6f64 732e  uild()` methods.
+00003f20: 0a2a 2041 6464 6564 2060 636c 6f73 6528  .* Added `close(
+00003f30: 2960 206d 6574 686f 6420 746f 2060 446f  )` method to `Do
+00003f40: 636b 6572 436c 6965 6e74 600a 2a20 4164  ckerClient`.* Ad
+00003f50: 6465 6420 6041 5049 436c 6965 6e74 2e69  ded `APIClient.i
+00003f60: 6e73 7065 6374 5f64 6973 7472 6962 7574  nspect_distribut
+00003f70: 696f 6e28 2960 206d 6574 686f 6420 616e  ion()` method an
+00003f80: 640a 2020 6044 6f63 6b65 7243 6c69 656e  d.  `DockerClien
+00003f90: 742e 696d 6167 6573 2e67 6574 5f72 6567  t.images.get_reg
+00003fa0: 6973 7472 795f 6461 7461 2829 600a 2020  istry_data()`.  
+00003fb0: 2a20 5468 6520 6c61 7474 6572 2072 6574  * The latter ret
+00003fc0: 7572 6e73 2061 6e20 696e 7374 616e 6365  urns an instance
+00003fd0: 206f 6620 7468 6520 6e65 7720 6052 6567   of the new `Reg
+00003fe0: 6973 7472 7944 6174 6160 2063 6c61 7373  istryData` class
+00003ff0: 0a0a 332e 312e 340a 2d2d 2d2d 2d0a 0a5b  ..3.1.4.-----..[
+00004000: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
+00004010: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
+00004020: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
+00004030: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
+00004040: 2f64 6f63 6b65 722d 7079 2f6d 696c 6573  /docker-py/miles
+00004050: 746f 6e65 2f34 383f 636c 6f73 6564 3d31  tone/48?closed=1
+00004060: 290a 0a23 2323 2042 7567 6669 7865 730a  )..### Bugfixes.
+00004070: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00004080: 6865 7265 2062 7569 6c64 2063 6f6e 7465  here build conte
+00004090: 7874 7320 636f 6e74 6169 6e69 6e67 2064  xts containing d
+000040a0: 6972 6563 746f 7279 2073 796d 6c69 6e6b  irectory symlink
+000040b0: 7320 776f 756c 6420 7072 6f64 7563 650a  s would produce.
+000040c0: 2020 696e 7661 6c69 6420 7461 7220 6172    invalid tar ar
+000040d0: 6368 6976 6573 0a0a 332e 312e 330a 2d2d  chives..3.1.3.--
+000040e0: 2d2d 2d0a 0a23 2323 2042 7567 6669 7865  ---..### Bugfixe
+000040f0: 730a 0a2a 2052 6567 656e 6572 6174 6564  s..* Regenerated
+00004100: 2069 6e76 616c 6964 2077 6865 656c 2070   invalid wheel p
+00004110: 6163 6b61 6765 0a0a 332e 312e 320a 2d2d  ackage..3.1.2.--
+00004120: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
+00004130: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
+00004140: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+00004150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004160: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
+00004170: 2f6d 696c 6573 746f 6e65 2f34 373f 636c  /milestone/47?cl
+00004180: 6f73 6564 3d31 290a 0a23 2323 2042 7567  osed=1)..### Bug
+00004190: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
+000041a0: 2062 7567 2074 6861 7420 6c65 6420 746f   bug that led to
+000041b0: 2061 2044 6f63 6b65 7266 696c 6520 6e6f   a Dockerfile no
+000041c0: 7420 6265 696e 6720 696e 636c 7564 6564  t being included
+000041d0: 2069 6e20 7468 6520 6275 696c 6420 636f   in the build co
+000041e0: 6e74 6578 740a 2020 696e 2073 6f6d 6520  ntext.  in some 
+000041f0: 7369 7475 6174 696f 6e73 2077 6865 6e20  situations when 
+00004200: 7468 6520 446f 636b 6572 6669 6c65 2773  the Dockerfile's
+00004210: 2070 6174 6820 7761 7320 7072 6566 6978   path was prefix
+00004220: 6564 2077 6974 6820 602e 2f60 0a0a 332e  ed with `./`..3.
+00004230: 312e 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374  1.1.-----..[List
+00004240: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
+00004250: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+00004260: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00004270: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
+00004280: 6b65 722d 7079 2f6d 696c 6573 746f 6e65  ker-py/milestone
+00004290: 2f34 363f 636c 6f73 6564 3d31 290a 0a23  /46?closed=1)..#
+000042a0: 2323 2042 7567 6669 7865 730a 0a2a 2046  ## Bugfixes..* F
+000042b0: 6978 6564 2061 2062 7567 2074 6861 7420  ixed a bug that 
+000042c0: 6361 7573 6564 2063 6f73 746c 7920 444e  caused costly DN
+000042d0: 5320 6c6f 6f6b 7570 7320 6f6e 204d 6163  S lookups on Mac
+000042e0: 204f 5358 2077 6865 6e20 636f 6e6e 6563   OSX when connec
+000042f0: 7469 6e67 2074 6f20 7468 650a 2020 656e  ting to the.  en
+00004300: 6769 6e65 2074 6872 6f75 6768 2055 4e49  gine through UNI
+00004310: 5820 736f 636b 6574 0a2a 2046 6978 6564  X socket.* Fixed
+00004320: 2061 2062 7567 2074 6861 7420 6361 7573   a bug that caus
+00004330: 6564 2060 2e64 6f63 6b65 7269 676e 6f72  ed `.dockerignor
+00004340: 6560 2063 6f6d 6d65 6e74 7320 746f 2062  e` comments to b
+00004350: 6520 7265 6164 2061 7320 6578 636c 7573  e read as exclus
+00004360: 696f 6e0a 2020 7061 7474 6572 6e73 0a0a  ion.  patterns..
+00004370: 332e 312e 300a 2d2d 2d2d 2d0a 0a5b 4c69  3.1.0.-----..[Li
+00004380: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+00004390: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+000043a0: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+000043b0: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+000043c0: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
+000043d0: 6e65 2f34 343f 636c 6f73 6564 3d31 290a  ne/44?closed=1).
+000043e0: 0a23 2323 2046 6561 7475 7265 730a 0a2a  .### Features..*
+000043f0: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
+00004400: 6f72 2060 6465 7669 6365 5f63 6772 6f75  or `device_cgrou
+00004410: 705f 7275 6c65 7360 2069 6e20 686f 7374  p_rules` in host
+00004420: 2063 6f6e 6669 670a 2a20 4164 6465 6420   config.* Added 
+00004430: 7375 7070 6f72 7420 666f 7220 6067 656e  support for `gen
+00004440: 6572 6963 5f72 6573 6f75 7263 6573 6020  eric_resources` 
+00004450: 7768 656e 2063 7265 6174 696e 6720 6120  when creating a 
+00004460: 6052 6573 6f75 7263 6573 600a 2020 6f62  `Resources`.  ob
+00004470: 6a65 6374 2e0a 2a20 4164 6465 6420 7375  ject..* Added su
+00004480: 7070 6f72 7420 666f 7220 6120 636f 6e66  pport for a conf
+00004490: 6967 7572 6162 6c65 2060 6368 756e 6b5f  igurable `chunk_
+000044a0: 7369 7a65 6020 7061 7261 6d65 7465 7220  size` parameter 
+000044b0: 696e 2060 6578 706f 7274 602c 0a20 2060  in `export`,.  `
+000044c0: 6765 745f 6172 6368 6976 6560 2061 6e64  get_archive` and
+000044d0: 2060 6765 745f 696d 6167 6560 2028 6049   `get_image` (`I
+000044e0: 6d61 6765 2e73 6176 6560 290a 2a20 4164  mage.save`).* Ad
+000044f0: 6465 6420 6120 6066 6f72 6365 5f75 7064  ded a `force_upd
+00004500: 6174 6560 206d 6574 686f 6420 746f 2074  ate` method to t
+00004510: 6865 2060 5365 7276 6963 6560 2063 6c61  he `Service` cla
+00004520: 7373 2e0a 2a20 496e 2060 5365 7276 6963  ss..* In `Servic
+00004530: 652e 7570 6461 7465 602c 2077 6865 6e20  e.update`, when 
+00004540: 7468 6520 6066 6f72 6365 5f75 7064 6174  the `force_updat
+00004550: 6560 2070 6172 616d 6574 6572 2069 7320  e` parameter is 
+00004560: 7365 7420 746f 2060 5472 7565 602c 0a20  set to `True`,. 
+00004570: 2074 6865 2063 7572 7265 6e74 2060 666f   the current `fo
+00004580: 7263 655f 7570 6461 7465 6020 636f 756e  rce_update` coun
+00004590: 7465 7220 6973 2069 6e63 7265 6d65 6e74  ter is increment
+000045a0: 6564 2062 7920 6f6e 6520 696e 2074 6865  ed by one in the
+000045b0: 2075 7064 6174 650a 2020 7265 7175 6573   update.  reques
+000045c0: 742e 0a0a 2323 2320 4275 6766 6978 6573  t...### Bugfixes
+000045d0: 0a0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+000045e0: 7768 6572 6520 6175 7468 656e 7469 6361  where authentica
+000045f0: 7469 6f6e 2074 6872 6f75 6768 2060 6c6f  tion through `lo
+00004600: 6769 6e28 2960 2077 6173 2062 6569 6e67  gin()` was being
+00004610: 2069 676e 6f72 6564 2069 6620 7468 650a   ignored if the.
+00004620: 2020 5344 4b20 7761 7320 636f 6e66 6967    SDK was config
+00004630: 7572 6564 2074 6f20 7573 6520 6120 6372  ured to use a cr
+00004640: 6564 656e 7469 616c 2073 746f 7265 2e0a  edential store..
+00004650: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+00004660: 6572 6520 646f 776e 6c6f 6164 206d 6574  ere download met
+00004670: 686f 6473 2077 6f75 6c64 2075 7365 2061  hods would use a
+00004680: 6e20 6162 7375 7264 6c79 2073 6d61 6c6c  n absurdly small
+00004690: 2063 6875 6e6b 2073 697a 652c 0a20 206c   chunk size,.  l
+000046a0: 6561 6469 6e67 2074 6f20 736c 6f77 2064  eading to slow d
+000046b0: 6174 6120 7265 7472 6965 7661 6c0a 2a20  ata retrieval.* 
+000046c0: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+000046d0: 6520 7573 696e 6720 6044 6f63 6b65 7243  e using `DockerC
+000046e0: 6c69 656e 742e 696d 6167 6573 2e70 756c  lient.images.pul
+000046f0: 6c60 2074 6f20 7075 6c6c 2061 6e20 696d  l` to pull an im
+00004700: 6167 6520 6279 2064 6967 6573 740a 2020  age by digest.  
+00004710: 776f 756c 6420 6c65 6164 2074 6f20 616e  would lead to an
+00004720: 2065 7863 6570 7469 6f6e 2062 6569 6e67   exception being
+00004730: 2072 6169 7365 642e 0a2a 2060 2e64 6f63   raised..* `.doc
+00004740: 6b65 7269 676e 6f72 6560 2072 756c 6573  kerignore` rules
+00004750: 2073 686f 756c 6420 6e6f 7720 6265 2072   should now be r
+00004760: 6573 7065 6374 6564 2061 7320 6465 6669  espected as defi
+00004770: 6e65 6420 6279 2074 6865 2073 7065 632c  ned by the spec,
+00004780: 0a20 2069 6e63 6c75 6469 6e67 2072 6573  .  including res
+00004790: 7065 6374 2066 6f72 206c 6173 742d 6c69  pect for last-li
+000047a0: 6e65 2070 7265 6365 6465 6e63 6520 616e  ne precedence an
+000047b0: 6420 7072 6f70 6572 2068 616e 646c 696e  d proper handlin
+000047c0: 6720 6f66 2061 6273 6f6c 7574 650a 2020  g of absolute.  
+000047d0: 7061 7468 730a 2a20 5468 6520 6070 6173  paths.* The `pas
+000047e0: 7360 2063 7265 6465 6e74 6961 6c20 7374  s` credential st
+000047f0: 6f72 6520 6973 206e 6f77 2070 726f 7065  ore is now prope
+00004800: 726c 7920 7375 7070 6f72 7465 642e 0a0a  rly supported...
+00004810: 332e 302e 310a 2d2d 2d2d 2d0a 0a5b 4c69  3.0.1.-----..[Li
+00004820: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+00004830: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+00004840: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+00004850: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+00004860: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
+00004870: 6e65 2f34 333f 636c 6f73 6564 3d31 290a  ne/43?closed=1).
+00004880: 0a23 2323 2042 7567 6669 7865 730a 0a2a  .### Bugfixes..*
+00004890: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+000048a0: 7265 2060 4150 4943 6c69 656e 742e 6c6f  re `APIClient.lo
+000048b0: 6769 6e60 2064 6964 6e27 7420 706f 7075  gin` didn't popu
+000048c0: 6c61 7465 2074 6865 2060 5f61 7574 685f  late the `_auth_
+000048d0: 636f 6e66 6967 7360 0a20 2064 6963 7469  configs`.  dicti
+000048e0: 6f6e 6172 7920 7072 6f70 6572 6c79 2c20  onary properly, 
+000048f0: 6361 7573 696e 6720 7375 6273 6571 7565  causing subseque
+00004900: 6e74 2060 7075 6c6c 6020 616e 6420 6070  nt `pull` and `p
+00004910: 7573 6860 206f 7065 7261 7469 6f6e 7320  ush` operations 
+00004920: 746f 2066 6169 6c0a 2a20 4669 7865 6420  to fail.* Fixed 
+00004930: 6120 6275 6720 7768 6572 6520 736f 6d65  a bug where some
+00004940: 2062 7569 6c64 2063 6f6e 7465 7874 2066   build context f
+00004950: 696c 6573 2077 6572 6520 696e 636f 7272  iles were incorr
+00004960: 6563 746c 7920 7265 636f 676e 697a 6564  ectly recognized
+00004970: 2061 730a 2020 6265 696e 6720 696e 6163   as.  being inac
+00004980: 6365 7373 6962 6c65 2e0a 2a20 4669 7865  cessible..* Fixe
+00004990: 6420 6120 6275 6720 7768 6572 6520 6669  d a bug where fi
+000049a0: 6c65 7320 7769 7468 2061 206e 6567 6174  les with a negat
+000049b0: 6976 6520 6d74 696d 6520 7661 6c75 6520  ive mtime value 
+000049c0: 776f 756c 640a 2020 6361 7573 6520 6572  would.  cause er
+000049d0: 726f 7273 2077 6865 6e20 696e 636c 7564  rors when includ
+000049e0: 6564 2069 6e20 6120 6275 696c 6420 636f  ed in a build co
+000049f0: 6e74 6578 740a 0a33 2e30 2e30 0a2d 2d2d  ntext..3.0.0.---
+00004a00: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
+00004a10: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
+00004a20: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
+00004a30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00004a40: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
+00004a50: 6d69 6c65 7374 6f6e 652f 3339 3f63 6c6f  milestone/39?clo
+00004a60: 7365 643d 3129 0a0a 2323 2320 4272 6561  sed=1)..### Brea
+00004a70: 6b69 6e67 2063 6861 6e67 6573 0a0a 2a20  king changes..* 
+00004a80: 5375 7070 6f72 7420 666f 7220 4150 4920  Support for API 
+00004a90: 7665 7273 696f 6e20 3c20 312e 3231 2068  version < 1.21 h
+00004aa0: 6173 2062 6565 6e20 7265 6d6f 7665 642e  as been removed.
+00004ab0: 0a2a 2054 6865 2066 6f6c 6c6f 7769 6e67  .* The following
+00004ac0: 206d 6574 686f 6473 2068 6176 6520 6265   methods have be
+00004ad0: 656e 2072 656d 6f76 6564 3a0a 2020 2a20  en removed:.  * 
+00004ae0: 6041 5049 436c 6965 6e74 2e63 6f70 7960  `APIClient.copy`
+00004af0: 2068 6173 2062 6565 6e20 7265 6d6f 7665   has been remove
+00004b00: 642e 2055 7365 7273 2073 686f 756c 6420  d. Users should 
+00004b10: 7573 6520 6041 5049 436c 6965 6e74 2e67  use `APIClient.g
+00004b20: 6574 5f61 7263 6869 7665 600a 2020 2020  et_archive`.    
+00004b30: 696e 7374 6561 642e 0a20 202a 2060 4150  instead..  * `AP
+00004b40: 4943 6c69 656e 742e 696e 7365 7274 6020  IClient.insert` 
+00004b50: 6861 7320 6265 656e 2072 656d 6f76 6564  has been removed
+00004b60: 2e20 5573 6572 7320 6d61 7920 7573 6520  . Users may use 
+00004b70: 6041 5049 436c 6965 6e74 2e70 7574 5f61  `APIClient.put_a
+00004b80: 7263 6869 7665 600a 2020 2020 636f 6d62  rchive`.    comb
+00004b90: 696e 6564 2077 6974 6820 6041 5049 436c  ined with `APICl
+00004ba0: 6965 6e74 2e63 6f6d 6d69 7460 2074 6f20  ient.commit` to 
+00004bb0: 7265 706c 6963 6174 6520 7468 6520 6d65  replicate the me
+00004bc0: 7468 6f64 2773 2062 6568 6176 696f 722e  thod's behavior.
+00004bd0: 0a20 202a 2060 7574 696c 732e 7069 6e67  .  * `utils.ping
+00004be0: 5f72 6567 6973 7472 7960 2061 6e64 2060  _registry` and `
+00004bf0: 7574 696c 732e 7069 6e67 6020 6861 7665  utils.ping` have
+00004c00: 2062 6565 6e20 7265 6d6f 7665 642e 0a2a   been removed..*
+00004c10: 2054 6865 2066 6f6c 6c6f 7769 6e67 2070   The following p
+00004c20: 6172 616d 6574 6572 7320 6861 7665 2062  arameters have b
+00004c30: 6565 6e20 7265 6d6f 7665 643a 0a20 202a  een removed:.  *
+00004c40: 2060 7374 7265 616d 6020 696e 2060 4150   `stream` in `AP
+00004c50: 4943 6c69 656e 742e 6275 696c 6460 0a20  IClient.build`. 
+00004c60: 202a 2060 6370 755f 7368 6172 6573 602c   * `cpu_shares`,
+00004c70: 2060 6370 7573 6574 602c 2060 646e 7360   `cpuset`, `dns`
+00004c80: 2c20 606d 656d 5f6c 696d 6974 602c 2060  , `mem_limit`, `
+00004c90: 6d65 6d73 7761 705f 6c69 6d69 7460 2c0a  memswap_limit`,.
+00004ca0: 2020 2020 6076 6f6c 756d 655f 6472 6976      `volume_driv
+00004cb0: 6572 602c 2060 766f 6c75 6d65 735f 6672  er`, `volumes_fr
+00004cc0: 6f6d 6020 696e 2060 4150 4943 6c69 656e  om` in `APIClien
+00004cd0: 742e 6372 6561 7465 5f63 6f6e 7461 696e  t.create_contain
+00004ce0: 6572 602e 2054 6865 7365 2061 7265 0a20  er`. These are. 
+00004cf0: 2020 2061 6c6c 2072 6570 6c61 6365 6420     all replaced 
+00004d00: 6279 2074 6865 6972 2065 7175 6976 616c  by their equival
+00004d10: 656e 7420 696e 2060 6372 6561 7465 5f68  ent in `create_h
+00004d20: 6f73 745f 636f 6e66 6967 600a 2020 2a20  ost_config`.  * 
+00004d30: 6069 6e73 6563 7572 655f 7265 6769 7374  `insecure_regist
+00004d40: 7279 6020 696e 2060 4150 4943 6c69 656e  ry` in `APIClien
+00004d50: 742e 6c6f 6769 6e60 2c20 6041 5049 436c  t.login`, `APICl
+00004d60: 6965 6e74 2e70 756c 6c60 2c0a 2020 2020  ient.pull`,.    
+00004d70: 6041 5049 436c 6965 6e74 2e70 7573 6860  `APIClient.push`
+00004d80: 2c20 6044 6f63 6b65 7243 6c69 656e 742e  , `DockerClient.
+00004d90: 696d 6167 6573 2e70 7573 6860 2061 6e64  images.push` and
+00004da0: 2060 446f 636b 6572 436c 6965 6e74 2e69   `DockerClient.i
+00004db0: 6d61 6765 732e 7075 6c6c 600a 2020 2a20  mages.pull`.  * 
+00004dc0: 6076 697a 6020 696e 2060 4150 4943 6c69  `viz` in `APICli
+00004dd0: 656e 742e 696d 6167 6573 600a 2a20 5468  ent.images`.* Th
+00004de0: 6520 666f 6c6c 6f77 696e 6720 7061 7261  e following para
+00004df0: 6d65 7465 7273 2068 6176 6520 6265 656e  meters have been
+00004e00: 2072 656e 616d 6564 3a0a 2020 2a20 6065   renamed:.  * `e
+00004e10: 6e64 706f 696e 745f 636f 6e66 6967 6020  ndpoint_config` 
+00004e20: 696e 2060 4150 4943 6c69 656e 742e 6372  in `APIClient.cr
+00004e30: 6561 7465 5f73 6572 7669 6365 6020 616e  eate_service` an
+00004e40: 640a 2020 2020 6041 5049 436c 6965 6e74  d.    `APIClient
+00004e50: 2e75 7064 6174 655f 7365 7276 6963 6560  .update_service`
+00004e60: 2069 7320 6e6f 7720 6065 6e64 706f 696e   is now `endpoin
+00004e70: 745f 7370 6563 600a 2020 2a20 606e 616d  t_spec`.  * `nam
+00004e80: 6560 2069 6e20 6044 6f63 6b65 7243 6c69  e` in `DockerCli
+00004e90: 656e 742e 696d 6167 6573 2e70 756c 6c60  ent.images.pull`
+00004ea0: 2069 7320 6e6f 7720 6072 6570 6f73 6974   is now `reposit
+00004eb0: 6f72 7960 0a2a 2054 6865 2072 6574 7572  ory`.* The retur
+00004ec0: 6e20 7661 6c75 6520 666f 7220 7468 6520  n value for the 
+00004ed0: 666f 6c6c 6f77 696e 6720 6d65 7468 6f64  following method
+00004ee0: 7320 6861 7320 6368 616e 6765 643a 0a20  s has changed:. 
+00004ef0: 202a 2060 4150 4943 6c69 656e 742e 7761   * `APIClient.wa
+00004f00: 6974 6020 616e 6420 6043 6f6e 7461 696e  it` and `Contain
+00004f10: 6572 2e77 6169 7460 206e 6f77 2072 6574  er.wait` now ret
+00004f20: 7572 6e20 6120 6060 6469 6374 6060 2072  urn a ``dict`` r
+00004f30: 6570 7265 7365 6e74 696e 670a 2020 2020  epresenting.    
+00004f40: 7468 6520 4150 4927 7320 7265 7370 6f6e  the API's respon
+00004f50: 7365 2069 6e73 7465 6164 206f 6620 7265  se instead of re
+00004f60: 7475 726e 696e 6720 7468 6520 7374 6174  turning the stat
+00004f70: 7573 2063 6f64 6520 6469 7265 6374 6c79  us code directly
+00004f80: 2e0a 2020 2a20 6044 6f63 6b65 7243 6c69  ..  * `DockerCli
+00004f90: 656e 742e 696d 6167 6573 2e6c 6f61 6460  ent.images.load`
+00004fa0: 206e 6f77 2072 6574 7572 6e73 2061 206c   now returns a l
+00004fb0: 6973 7420 6f66 2060 496d 6167 6560 206f  ist of `Image` o
+00004fc0: 626a 6563 7473 2074 6861 7420 6861 7665  bjects that have
+00004fd0: 0a20 2020 2066 6f72 2074 6865 2069 6d61  .    for the ima
+00004fe0: 6765 7320 7468 6174 2077 6572 6520 6c6f  ges that were lo
+00004ff0: 6164 6564 2c20 696e 7374 6561 6420 6f66  aded, instead of
+00005000: 2061 206c 6f67 2073 7472 6561 6d2e 0a20   a log stream.. 
+00005010: 202a 2060 436f 6e74 6169 6e65 722e 6578   * `Container.ex
+00005020: 6563 5f72 756e 6020 6e6f 7720 7265 7475  ec_run` now retu
+00005030: 726e 7320 6120 7475 706c 6520 6f66 2028  rns a tuple of (
+00005040: 6578 6974 5f63 6f64 652c 206f 7574 7075  exit_code, outpu
+00005050: 7429 2069 6e73 7465 6164 206f 660a 2020  t) instead of.  
+00005060: 2020 6a75 7374 2074 6865 206f 7574 7075    just the outpu
+00005070: 742e 0a20 202a 2060 446f 636b 6572 436c  t..  * `DockerCl
+00005080: 6965 6e74 2e69 6d61 6765 732e 6275 696c  ient.images.buil
+00005090: 6460 206e 6f77 2072 6574 7572 6e73 2061  d` now returns a
+000050a0: 2074 7570 6c65 206f 6620 2869 6d61 6765   tuple of (image
+000050b0: 2c20 6275 696c 645f 6c6f 6773 290a 2020  , build_logs).  
+000050c0: 2020 696e 7374 6561 6420 6f66 206a 7573    instead of jus
+000050d0: 7420 7468 6520 696d 6167 6520 6f62 6a65  t the image obje
+000050e0: 6374 2e0a 2020 2a20 6041 5049 436c 6965  ct..  * `APIClie
+000050f0: 6e74 2e65 7870 6f72 7460 2c20 6041 5049  nt.export`, `API
+00005100: 436c 6965 6e74 2e67 6574 5f61 7263 6869  Client.get_archi
+00005110: 7665 6020 616e 6420 6041 5049 436c 6965  ve` and `APIClie
+00005120: 6e74 2e67 6574 5f69 6d61 6765 6020 6e6f  nt.get_image` no
+00005130: 770a 2020 2020 7265 7475 726e 2067 656e  w.    return gen
+00005140: 6572 6174 6f72 7320 7374 7265 616d 696e  erators streamin
+00005150: 6720 7468 6520 7261 7720 6269 6e61 7279  g the raw binary
+00005160: 2064 6174 6120 6672 6f6d 2074 6865 2073   data from the s
+00005170: 6572 7665 7227 7320 7265 7370 6f6e 7365  erver's response
+00005180: 2e0a 2020 2a20 5768 656e 206e 6f20 7461  ..  * When no ta
+00005190: 6720 6973 2070 726f 7669 6465 642c 2060  g is provided, `
+000051a0: 446f 636b 6572 436c 6965 6e74 2e69 6d61  DockerClient.ima
+000051b0: 6765 732e 7075 6c6c 6020 6e6f 7720 7265  ges.pull` now re
+000051c0: 7475 726e 7320 6120 6c69 7374 206f 660a  turns a list of.
+000051d0: 2020 2020 6049 6d61 6765 6073 2061 7373      `Image`s ass
+000051e0: 6f63 6961 7465 6420 746f 2074 6865 2070  ociated to the p
+000051f0: 756c 6c65 6420 7265 706f 7369 746f 7279  ulled repository
+00005200: 2069 6e73 7465 6164 206f 6620 6a75 7374   instead of just
+00005210: 2074 6865 2060 6c61 7465 7374 600a 2020   the `latest`.  
+00005220: 2020 696d 6167 652e 0a0a 2323 2320 4665    image...### Fe
+00005230: 6174 7572 6573 0a0a 2a20 5468 6520 446f  atures..* The Do
+00005240: 636b 6572 2050 7974 686f 6e20 5344 4b20  cker Python SDK 
+00005250: 6973 206e 6f77 206f 6666 6963 6961 6c6c  is now officiall
+00005260: 7920 7375 7070 6f72 7465 6420 6f6e 2050  y supported on P
+00005270: 7974 686f 6e20 332e 360a 2a20 4164 6465  ython 3.6.* Adde
+00005280: 6420 6073 6361 6c65 6020 6d65 7468 6f64  d `scale` method
+00005290: 2074 6f20 7468 6520 6053 6572 7669 6365   to the `Service
+000052a0: 6020 6d6f 6465 6c20 3b20 7468 6973 206d  ` model ; this m
+000052b0: 6574 686f 6420 6973 2061 2073 686f 7274  ethod is a short
+000052c0: 6861 6e64 0a20 2074 6861 7420 6361 6c6c  hand.  that call
+000052d0: 7320 6075 7064 6174 655f 7365 7276 6963  s `update_servic
+000052e0: 6560 2077 6974 6820 7468 6520 7265 7175  e` with the requ
+000052f0: 6972 6564 206e 756d 6265 7220 6f66 2072  ired number of r
+00005300: 6570 6c69 6361 730a 2a20 4164 6465 6420  eplicas.* Added 
+00005310: 7375 7070 6f72 7420 666f 7220 7468 6520  support for the 
+00005320: 6070 6c61 7466 6f72 6d60 2070 6172 616d  `platform` param
+00005330: 6574 6572 2069 6e20 6041 5049 436c 6965  eter in `APIClie
+00005340: 6e74 2e62 7569 6c64 602c 0a20 2060 446f  nt.build`,.  `Do
+00005350: 636b 6572 436c 6965 6e74 2e69 6d61 6765  ckerClient.image
+00005360: 732e 6275 696c 6460 2c20 6041 5049 436c  s.build`, `APICl
+00005370: 6965 6e74 2e70 756c 6c60 2061 6e64 2060  ient.pull` and `
+00005380: 446f 636b 6572 436c 6965 6e74 2e69 6d61  DockerClient.ima
+00005390: 6765 732e 7075 6c6c 600a 2a20 4164 6465  ges.pull`.* Adde
+000053a0: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
+000053b0: 6520 6075 6e74 696c 6020 7061 7261 6d65  e `until` parame
+000053c0: 7465 7220 696e 2060 4150 4943 6c69 656e  ter in `APIClien
+000053d0: 742e 6c6f 6773 6020 616e 640a 2020 6043  t.logs` and.  `C
+000053e0: 6f6e 7461 696e 6572 2e6c 6f67 7360 0a2a  ontainer.logs`.*
+000053f0: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
+00005400: 6f72 2074 6865 2060 776f 726b 6469 7260  or the `workdir`
+00005410: 2061 7267 756d 656e 7420 696e 2060 4150   argument in `AP
+00005420: 4943 6c69 656e 742e 6578 6563 5f63 7265  IClient.exec_cre
+00005430: 6174 6560 2061 6e64 0a20 2060 436f 6e74  ate` and.  `Cont
+00005440: 6169 6e65 722e 6578 6563 5f72 756e 600a  ainer.exec_run`.
+00005450: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+00005460: 666f 7220 7468 6520 6063 6f6e 6469 7469  for the `conditi
+00005470: 6f6e 6020 6172 6775 6d65 6e74 2069 6e20  on` argument in 
+00005480: 6041 5049 436c 6965 6e74 2e77 6169 7460  `APIClient.wait`
+00005490: 2061 6e64 0a20 2060 436f 6e74 6169 6e65   and.  `Containe
+000054a0: 722e 7761 6974 600a 2a20 5573 6572 7320  r.wait`.* Users 
+000054b0: 6361 6e20 6e6f 7720 7370 6563 6966 7920  can now specify 
+000054c0: 6120 7075 626c 6973 6820 6d6f 6465 2066  a publish mode f
+000054d0: 6f72 2070 6f72 7473 2069 6e20 6045 6e64  or ports in `End
+000054e0: 706f 696e 7453 7065 6360 2075 7369 6e67  pointSpec` using
+000054f0: 0a20 2074 6865 2060 7b70 7562 6c69 7368  .  the `{publish
+00005500: 6564 5f70 6f72 743a 2028 7461 7267 6574  ed_port: (target
+00005510: 5f70 6f72 742c 2070 726f 746f 636f 6c2c  _port, protocol,
+00005520: 2070 7562 6c69 7368 5f6d 6f64 6529 7d60   publish_mode)}`
+00005530: 2073 796e 7461 782e 0a2a 2041 6464 6564   syntax..* Added
+00005540: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
+00005550: 2060 6973 6f6c 6174 696f 6e60 2070 6172   `isolation` par
+00005560: 616d 6574 6572 2069 6e20 6043 6f6e 7461  ameter in `Conta
+00005570: 696e 6572 5370 6563 602c 0a20 2060 446f  inerSpec`,.  `Do
+00005580: 636b 6572 436c 6965 6e74 2e73 6572 7669  ckerClient.servi
+00005590: 6365 732e 6372 6561 7465 6020 616e 6420  ces.create` and 
+000055a0: 6053 6572 7669 6365 2e75 7064 6174 6560  `Service.update`
+000055b0: 0a2a 2060 4150 4943 6c69 656e 742e 6174  .* `APIClient.at
+000055c0: 7461 6368 5f73 6f63 6b65 7460 2c20 6041  tach_socket`, `A
+000055d0: 5049 436c 6965 6e74 2e65 7865 635f 6372  PIClient.exec_cr
+000055e0: 6561 7465 6020 6e6f 7720 616c 6c6f 7720  eate` now allow 
+000055f0: 7370 6563 6966 7969 6e67 2061 0a20 2060  specifying a.  `
+00005600: 6465 7461 6368 5f6b 6579 7360 2063 6f6d  detach_keys` com
+00005610: 6269 6e61 7469 6f6e 2e20 4966 2075 6e73  bination. If uns
+00005620: 7065 6369 6669 6564 2c20 7468 6520 7661  pecified, the va
+00005630: 6c75 6520 6672 6f6d 2074 6865 2060 636f  lue from the `co
+00005640: 6e66 6967 2e6a 736f 6e60 0a20 2066 696c  nfig.json`.  fil
+00005650: 6520 7769 6c6c 2062 6520 7573 6564 0a2a  e will be used.*
+00005660: 2054 4c53 2063 6f6e 6e65 6374 696f 6e73   TLS connections
+00005670: 206e 6f77 2064 6566 6175 6c74 2074 6f20   now default to 
+00005680: 7573 696e 6720 7468 6520 544c 5376 312e  using the TLSv1.
+00005690: 3220 7072 6f74 6f63 6f6c 2077 6865 6e20  2 protocol when 
+000056a0: 6176 6169 6c61 626c 650a 0a0a 2323 2320  available...### 
+000056b0: 4275 6766 6978 6573 0a0a 2a20 4669 7865  Bugfixes..* Fixe
+000056c0: 6420 6120 6275 6720 7768 6572 6520 7768  d a bug where wh
+000056d0: 6974 6573 7061 6365 2d6f 6e6c 7920 6c69  itespace-only li
+000056e0: 6e65 7320 696e 2060 2e64 6f63 6b65 7269  nes in `.dockeri
+000056f0: 676e 6f72 6560 2077 6f75 6c64 2062 7265  gnore` would bre
+00005700: 616b 2062 7569 6c64 730a 2020 6f6e 2057  ak builds.  on W
+00005710: 696e 646f 7773 0a2a 2046 6978 6564 2061  indows.* Fixed a
+00005720: 2062 7567 2077 6865 7265 2062 726f 6b65   bug where broke
+00005730: 6e20 7379 6d6c 696e 6b73 2069 6e73 6964  n symlinks insid
+00005740: 6520 6120 6275 696c 6420 636f 6e74 6578  e a build contex
+00005750: 7420 776f 756c 6420 6361 7573 6520 7468  t would cause th
+00005760: 650a 2020 6275 696c 6420 746f 2066 6169  e.  build to fai
+00005770: 6c0a 2a20 4669 7865 6420 6120 6275 6720  l.* Fixed a bug 
+00005780: 7768 6572 6520 7370 6563 6966 7969 6e67  where specifying
+00005790: 2076 6f6c 756d 6573 2077 6974 6820 5769   volumes with Wi
+000057a0: 6e64 6f77 7320 6472 6976 6573 2077 6f75  ndows drives wou
+000057b0: 6c64 2063 6175 7365 0a20 2069 6e63 6f72  ld cause.  incor
+000057c0: 7265 6374 2070 6172 7369 6e67 2069 6e20  rect parsing in 
+000057d0: 6044 6f63 6b65 7243 6c69 656e 742e 636f  `DockerClient.co
+000057e0: 6e74 6169 6e65 7273 2e72 756e 600a 2a20  ntainers.run`.* 
+000057f0: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+00005800: 6520 7468 6520 606e 6574 776f 726b 7360  e the `networks`
+00005810: 2064 6174 6120 7072 6f76 6964 6564 2074   data provided t
+00005820: 6f20 6063 7265 6174 655f 7365 7276 6963  o `create_servic
+00005830: 6560 2061 6e64 0a20 2060 7570 6461 7465  e` and.  `update
+00005840: 5f73 6572 7669 6365 6020 776f 756c 6420  _service` would 
+00005850: 6265 2073 656e 7420 696e 636f 7272 6563  be sent incorrec
+00005860: 746c 7920 746f 2074 6865 2045 6e67 696e  tly to the Engin
+00005870: 6520 7769 7468 2041 5049 203c 2031 2e32  e with API < 1.2
+00005880: 350a 2a20 5075 6c6c 696e 6720 616c 6c20  5.* Pulling all 
+00005890: 7461 6773 2066 726f 6d20 6120 7265 706f  tags from a repo
+000058a0: 7369 746f 7279 2077 6974 6820 6e6f 2060  sitory with no `
+000058b0: 6c61 7465 7374 6020 7461 6720 7573 696e  latest` tag usin
+000058c0: 6720 7468 650a 2020 6044 6f63 6b65 7243  g the.  `DockerC
+000058d0: 6c69 656e 7460 2077 696c 6c20 6e6f 206c  lient` will no l
+000058e0: 6f6e 6765 7220 7261 6973 6520 6120 604e  onger raise a `N
+000058f0: 6f74 466f 756e 6460 2065 7863 6570 7469  otFound` excepti
+00005900: 6f6e 0a0a 322e 372e 300a 2d2d 2d2d 2d0a  on..2.7.0.-----.
+00005910: 0a5b 4c69 7374 206f 6620 5052 7320 2f20  .[List of PRs / 
+00005920: 6973 7375 6573 2066 6f72 2074 6869 7320  issues for this 
+00005930: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
+00005940: 2f67 6974 6875 622e 636f 6d2f 646f 636b  /github.com/dock
+00005950: 6572 2f64 6f63 6b65 722d 7079 2f6d 696c  er/docker-py/mil
+00005960: 6573 746f 6e65 2f34 313f 636c 6f73 6564  estone/41?closed
+00005970: 3d31 290a 0a23 2323 2046 6561 7475 7265  =1)..### Feature
+00005980: 730a 0a2a 2041 6464 6564 2060 756e 6c6f  s..* Added `unlo
+00005990: 636b 5f73 7761 726d 6020 616e 6420 6067  ck_swarm` and `g
+000059a0: 6574 5f75 6e6c 6f63 6b5f 6b65 7960 206d  et_unlock_key` m
+000059b0: 6574 686f 6473 2074 6f20 7468 6520 6041  ethods to the `A
+000059c0: 5049 436c 6965 6e74 602e 0a20 2020 202a  PIClient`..    *
+000059d0: 2041 6464 6564 2060 756e 6c6f 636b 6020   Added `unlock` 
+000059e0: 616e 6420 6067 6574 5f75 6e6c 6f63 6b5f  and `get_unlock_
+000059f0: 6b65 7960 2074 6f20 6044 6f63 6b65 7243  key` to `DockerC
+00005a00: 6c69 656e 742e 7377 6172 6d60 2e0a 2a20  lient.swarm`..* 
+00005a10: 4164 6465 6420 6120 6067 7265 6564 7960  Added a `greedy`
+00005a20: 2070 6172 616d 6574 6572 2074 6f20 6044   parameter to `D
+00005a30: 6f63 6b65 7243 6c69 656e 742e 6e65 7477  ockerClient.netw
+00005a40: 6f72 6b73 2e6c 6973 7460 2c20 7969 656c  orks.list`, yiel
+00005a50: 6469 6e67 0a20 2061 6464 6974 696f 6e61  ding.  additiona
+00005a60: 6c20 6465 7461 696c 7320 6162 6f75 7420  l details about 
+00005a70: 7468 6520 6c69 7374 6564 206e 6574 776f  the listed netwo
+00005a80: 726b 732e 0a2a 2041 6464 6564 2060 6370  rks..* Added `cp
+00005a90: 755f 7274 5f72 756e 7469 6d65 6020 616e  u_rt_runtime` an
+00005aa0: 6420 6063 7075 5f72 745f 7065 7269 6f64  d `cpu_rt_period
+00005ab0: 6020 6173 2070 6172 616d 6574 6572 7320  ` as parameters 
+00005ac0: 746f 0a20 2060 4150 4943 6c69 656e 742e  to.  `APIClient.
+00005ad0: 6372 6561 7465 5f68 6f73 745f 636f 6e66  create_host_conf
+00005ae0: 6967 6020 616e 6420 6044 6f63 6b65 7243  ig` and `DockerC
+00005af0: 6c69 656e 742e 636f 6e74 6169 6e65 7273  lient.containers
+00005b00: 2e72 756e 602e 0a2a 2041 6464 6564 2074  .run`..* Added t
+00005b10: 6865 2060 6f72 6465 7260 2061 7267 756d  he `order` argum
+00005b20: 656e 7420 746f 2060 5570 6461 7465 436f  ent to `UpdateCo
+00005b30: 6e66 6967 602e 0a2a 2041 6464 6564 2060  nfig`..* Added `
+00005b40: 6665 7463 685f 6375 7272 656e 745f 7370  fetch_current_sp
+00005b50: 6563 6020 746f 2060 4150 4943 6c69 656e  ec` to `APIClien
+00005b60: 742e 7570 6461 7465 5f73 6572 7669 6365  t.update_service
+00005b70: 6020 616e 6420 6053 6572 7669 6365 2e75  ` and `Service.u
+00005b80: 7064 6174 6560 0a20 2074 6861 7420 7769  pdate`.  that wi
+00005b90: 6c6c 2072 6574 7269 6576 6520 7468 6520  ll retrieve the 
+00005ba0: 6375 7272 656e 7420 636f 6e66 6967 7572  current configur
+00005bb0: 6174 696f 6e20 6f66 2074 6865 2073 6572  ation of the ser
+00005bc0: 7669 6365 2061 6e64 206d 6572 6765 2069  vice and merge i
+00005bd0: 7420 7769 7468 0a20 2074 6865 2070 726f  t with.  the pro
+00005be0: 7669 6465 6420 7061 7261 6d65 7465 7273  vided parameters
+00005bf0: 2074 6f20 6465 7465 726d 696e 6520 7468   to determine th
+00005c00: 6520 6e65 7720 636f 6e66 6967 7572 6174  e new configurat
+00005c10: 696f 6e2e 0a0a 2323 2320 4275 6766 6978  ion...### Bugfix
+00005c20: 6573 0a0a 2a20 4669 7865 6420 6120 6275  es..* Fixed a bu
+00005c30: 6720 7768 6572 6520 7468 6520 6062 7569  g where the `bui
+00005c40: 6c64 6020 6d65 7468 6f64 2074 7269 6564  ld` method tried
+00005c50: 2074 6f20 696e 636c 7564 6520 696e 6163   to include inac
+00005c60: 6365 7373 6962 6c65 2066 696c 6573 0a20  cessible files. 
+00005c70: 2069 6e20 7468 6520 636f 6e74 6578 742c   in the context,
+00005c80: 206c 6561 6469 6e67 2074 6f20 6f62 7363   leading to obsc
+00005c90: 7572 6520 6572 726f 7273 2064 7572 696e  ure errors durin
+00005ca0: 6720 7468 6520 6275 696c 6420 7068 6173  g the build phas
+00005cb0: 650a 2020 2869 6e61 6363 6573 7369 626c  e.  (inaccessibl
+00005cc0: 6520 6669 6c65 7320 696e 7369 6465 2074  e files inside t
+00005cd0: 6865 2063 6f6e 7465 7874 206e 6f77 2072  he context now r
+00005ce0: 6169 7365 2061 6e20 6049 4f45 7272 6f72  aise an `IOError
+00005cf0: 6020 696e 7374 6561 6429 2e0a 2a20 4669  ` instead)..* Fi
+00005d00: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
+00005d10: 7468 6520 6062 7569 6c64 6020 6d65 7468  the `build` meth
+00005d20: 6f64 2077 6f75 6c64 2074 7279 2074 6f20  od would try to 
+00005d30: 7265 6164 2066 726f 6d20 4649 464f 7320  read from FIFOs 
+00005d40: 7072 6573 656e 740a 2020 696e 7369 6465  present.  inside
+00005d50: 2074 6865 2062 7569 6c64 2063 6f6e 7465   the build conte
+00005d60: 7874 2c20 6361 7573 696e 6720 6974 2074  xt, causing it t
+00005d70: 6f20 6861 6e67 2e0a 2a20 6041 5049 436c  o hang..* `APICl
+00005d80: 6965 6e74 2e73 746f 7060 2077 696c 6c20  ient.stop` will 
+00005d90: 6e6f 206c 6f6e 6765 7220 6f76 6572 7269  no longer overri
+00005da0: 6465 2074 6865 2060 7374 6f70 5f74 696d  de the `stop_tim
+00005db0: 656f 7574 6020 7661 6c75 6520 7072 6573  eout` value pres
+00005dc0: 656e 740a 2020 696e 2074 6865 2063 6f6e  ent.  in the con
+00005dd0: 7461 696e 6572 2773 2063 6f6e 6669 6775  tainer's configu
+00005de0: 7261 7469 6f6e 2e0a 2a20 4669 7865 6420  ration..* Fixed 
+00005df0: 6120 6275 6720 7072 6576 656e 7469 6e67  a bug preventing
+00005e00: 2072 656d 6f76 616c 206f 6620 6e65 7477   removal of netw
+00005e10: 6f72 6b73 2077 6974 6820 6e61 6d65 7320  orks with names 
+00005e20: 636f 6e74 6169 6e69 6e67 2061 2073 7061  containing a spa
+00005e30: 6365 2e0a 2a20 4669 7865 6420 6120 6275  ce..* Fixed a bu
+00005e40: 6720 7768 6572 6520 6044 6f63 6b65 7243  g where `DockerC
+00005e50: 6c69 656e 742e 636f 6e74 6169 6e65 7273  lient.containers
+00005e60: 2e72 756e 6020 776f 756c 6420 6372 6173  .run` would cras
+00005e70: 6820 6966 2074 6865 0a20 2060 6175 746f  h if the.  `auto
+00005e80: 5f72 656d 6f76 6560 2070 6172 616d 6574  _remove` paramet
+00005e90: 6572 2077 6173 2073 6574 2074 6f20 6054  er was set to `T
+00005ea0: 7275 6560 2e0a 2a20 4368 616e 6765 6420  rue`..* Changed 
+00005eb0: 7468 6520 6465 6661 756c 7420 7661 6c75  the default valu
+00005ec0: 6520 6f66 2060 6c69 7374 656e 5f61 6464  e of `listen_add
+00005ed0: 7260 2069 6e20 606a 6f69 6e5f 7377 6172  r` in `join_swar
+00005ee0: 6d60 2074 6f20 6d61 7463 6820 7468 650a  m` to match the.
+00005ef0: 2020 6f6e 6520 696e 2060 696e 6974 5f73    one in `init_s
+00005f00: 7761 726d 602e 0a2a 2046 6978 6564 2061  warm`..* Fixed a
+00005f10: 2062 7567 2077 6865 7265 2068 616e 646c   bug where handl
+00005f20: 696e 6720 4854 5450 2065 7272 6f72 7320  ing HTTP errors 
+00005f30: 7769 7468 206e 6f20 626f 6479 2077 6f75  with no body wou
+00005f40: 6c64 2063 6175 7365 2061 6e20 756e 6578  ld cause an unex
+00005f50: 7065 6374 6564 0a20 2065 7863 6570 7469  pected.  excepti
+00005f60: 6f6e 2074 6f20 6265 2074 6872 6f77 6e20  on to be thrown 
+00005f70: 7768 696c 6520 6765 6e65 7261 7469 6e67  while generating
+00005f80: 2061 6e20 6041 5049 4572 726f 7260 206f   an `APIError` o
+00005f90: 626a 6563 742e 0a0a 322e 362e 310a 2d2d  bject...2.6.1.--
+00005fa0: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
+00005fb0: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
+00005fc0: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+00005fd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005fe0: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
+00005ff0: 2f6d 696c 6573 746f 6e65 2f34 303f 636c  /milestone/40?cl
+00006000: 6f73 6564 3d31 290a 0a23 2323 2042 7567  osed=1)..### Bug
+00006010: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
+00006020: 2062 7567 206f 6e20 5079 7468 6f6e 2033   bug on Python 3
+00006030: 2069 6e73 7461 6c6c 6174 696f 6e73 2070   installations p
+00006040: 7265 7665 6e74 696e 6720 7468 6520 7573  reventing the us
+00006050: 6520 6f66 2074 6865 2060 6174 7461 6368  e of the `attach
+00006060: 6020 616e 640a 2020 6065 7865 635f 7275  ` and.  `exec_ru
+00006070: 6e60 206d 6574 686f 6473 2e0a 0a0a 322e  n` methods....2.
+00006080: 362e 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374  6.0.-----..[List
+00006090: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
+000060a0: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+000060b0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+000060c0: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
+000060d0: 6b65 722d 7079 2f6d 696c 6573 746f 6e65  ker-py/milestone
+000060e0: 2f33 383f 636c 6f73 6564 3d31 290a 0a23  /38?closed=1)..#
+000060f0: 2323 2046 6561 7475 7265 730a 0a2a 2041  ## Features..* A
+00006100: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+00006110: 2060 6d6f 756e 7473 6020 696e 2060 4150   `mounts` in `AP
+00006120: 4943 6c69 656e 742e 6372 6561 7465 5f68  IClient.create_h
+00006130: 6f73 745f 636f 6e66 6967 6020 616e 640a  ost_config` and.
+00006140: 2020 6044 6f63 6b65 7243 6c69 656e 742e    `DockerClient.
+00006150: 636f 6e74 6169 6e65 7273 2e72 756e 600a  containers.run`.
+00006160: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+00006170: 666f 7220 6063 6f6e 7369 7374 656e 6379  for `consistency
+00006180: 602c 2060 746d 7066 735f 7369 7a65 6020  `, `tmpfs_size` 
+00006190: 616e 6420 6074 6d70 6673 5f6d 6f64 6560  and `tmpfs_mode`
+000061a0: 2077 6865 6e0a 2020 6372 6561 7469 6e67   when.  creating
+000061b0: 206d 6f75 6e74 206f 626a 6563 7473 2e0a   mount objects..
+000061c0: 2a20 604d 6f75 6e74 6020 6f62 6a65 6374  * `Mount` object
+000061d0: 7320 6e6f 7720 7375 7070 6f72 7420 7468  s now support th
+000061e0: 6520 6074 6d70 6673 6020 616e 6420 606e  e `tmpfs` and `n
+000061f0: 7069 7065 6020 7479 7065 732e 0a2a 2041  pipe` types..* A
+00006200: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+00006210: 2060 6578 7472 615f 686f 7374 7360 2069   `extra_hosts` i
+00006220: 6e20 7468 6520 6062 7569 6c64 6020 6d65  n the `build` me
+00006230: 7468 6f64 732e 0a2a 2041 6464 6564 2073  thods..* Added s
+00006240: 7570 706f 7274 2066 6f72 2074 6865 2063  upport for the c
+00006250: 6f6e 6669 6773 2041 5049 3a0a 2020 2020  onfigs API:.    
+00006260: 2a20 496e 2060 4150 4943 6c69 656e 7460  * In `APIClient`
+00006270: 3a20 6063 7265 6174 655f 636f 6e66 6967  : `create_config
+00006280: 602c 2060 696e 7370 6563 745f 636f 6e66  `, `inspect_conf
+00006290: 6967 602c 2060 7265 6d6f 7665 5f63 6f6e  ig`, `remove_con
+000062a0: 6669 6760 2c0a 2020 2020 2020 6063 6f6e  fig`,.      `con
+000062b0: 6669 6773 600a 2020 2020 2a20 496e 2060  figs`.    * In `
+000062c0: 446f 636b 6572 436c 6965 6e74 603a 2060  DockerClient`: `
+000062d0: 636f 6e66 6967 732e 6372 6561 7465 602c  configs.create`,
+000062e0: 2060 636f 6e66 6967 732e 6765 7460 2c20   `configs.get`, 
+000062f0: 6063 6f6e 6669 6773 2e6c 6973 7460 2061  `configs.list` a
+00006300: 6e64 0a20 2020 2020 2074 6865 2060 436f  nd.      the `Co
+00006310: 6e66 6967 6020 6d6f 6465 6c2e 0a20 2020  nfig` model..   
+00006320: 202a 2041 6464 6564 2060 636f 6e66 6967   * Added `config
+00006330: 7360 2070 6172 616d 6574 6572 2074 6f20  s` parameter to 
+00006340: 6043 6f6e 7461 696e 6572 5370 6563 602e  `ContainerSpec`.
+00006350: 2045 6163 6820 6974 656d 2069 6e20 7468   Each item in th
+00006360: 6520 6063 6f6e 6669 6773 600a 2020 2020  e `configs`.    
+00006370: 2020 6c69 7374 206d 7573 7420 6265 2061    list must be a
+00006380: 2060 646f 636b 6572 2e74 7970 6573 2e43   `docker.types.C
+00006390: 6f6e 6669 6752 6566 6572 656e 6365 6020  onfigReference` 
+000063a0: 696e 7374 616e 6365 2e0a 2a20 4164 6465  instance..* Adde
+000063b0: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
+000063c0: 6520 666f 6c6c 6f77 696e 6720 7061 7261  e following para
+000063d0: 6d65 7465 7273 2077 6865 6e20 6372 6561  meters when crea
+000063e0: 7469 6e67 2061 2060 436f 6e74 6169 6e65  ting a `Containe
+000063f0: 7253 7065 6360 0a20 206f 626a 6563 743a  rSpec`.  object:
+00006400: 2060 6772 6f75 7073 602c 2060 6f70 656e   `groups`, `open
+00006410: 5f73 7464 696e 602c 2060 7265 6164 5f6f  _stdin`, `read_o
+00006420: 6e6c 7960 2c20 6073 746f 705f 7369 676e  nly`, `stop_sign
+00006430: 616c 602c 2060 6865 6c61 7468 6368 6563  al`, `helathchec
+00006440: 6b60 2c0a 2020 6068 6f73 7473 602c 2060  k`,.  `hosts`, `
+00006450: 6e73 5f63 6f6e 6669 6760 2c20 6063 6f6e  ns_config`, `con
+00006460: 6669 6773 602c 2060 7072 6976 696c 6567  figs`, `privileg
+00006470: 6573 602e 0a2a 2041 6464 6564 2074 6865  es`..* Added the
+00006480: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6669   following confi
+00006490: 6775 7261 7469 6f6e 2063 6c61 7373 6573  guration classes
+000064a0: 2074 6f20 6064 6f63 6b65 722e 7479 7065   to `docker.type
+000064b0: 7360 3a0a 2020 6043 6f6e 6669 6752 6566  s`:.  `ConfigRef
+000064c0: 6572 656e 6365 602c 2060 444e 5343 6f6e  erence`, `DNSCon
+000064d0: 6669 6760 2c20 6050 7269 7669 6c65 6765  fig`, `Privilege
+000064e0: 7360 2c20 6053 7761 726d 4578 7465 726e  s`, `SwarmExtern
+000064f0: 616c 4341 602e 0a2a 2041 6464 6564 2073  alCA`..* Added s
+00006500: 7570 706f 7274 2066 6f72 2060 6472 6976  upport for `driv
+00006510: 6572 6020 696e 2060 4150 4943 6c69 656e  er` in `APIClien
+00006520: 742e 6372 6561 7465 5f73 6563 7265 7460  t.create_secret`
+00006530: 2061 6e64 0a20 2060 446f 636b 6572 436c   and.  `DockerCl
+00006540: 6965 6e74 2e73 6563 7265 7473 2e63 7265  ient.secrets.cre
+00006550: 6174 6560 2e0a 2a20 4164 6465 6420 7375  ate`..* Added su
+00006560: 7070 6f72 7420 666f 7220 6073 636f 7065  pport for `scope
+00006570: 6020 696e 2060 4150 4943 6c69 656e 742e  ` in `APIClient.
+00006580: 696e 7370 6563 745f 6e65 7477 6f72 6b60  inspect_network`
+00006590: 2061 6e64 0a20 2060 4150 4943 6c69 656e   and.  `APIClien
+000065a0: 742e 6372 6561 7465 5f6e 6574 776f 726b  t.create_network
+000065b0: 602c 2061 6e64 2074 6865 6972 2060 446f  `, and their `Do
+000065c0: 636b 6572 436c 6965 6e74 6020 6571 7569  ckerClient` equi
+000065d0: 7661 6c65 6e74 2e0a 2a20 4164 6465 6420  valent..* Added 
+000065e0: 7375 7070 6f72 7420 666f 7220 7468 6520  support for the 
+000065f0: 666f 6c6c 6f77 696e 6720 7061 7261 6d65  following parame
+00006600: 7465 7273 2074 6f20 6063 7265 6174 655f  ters to `create_
+00006610: 7377 6172 6d5f 7370 6563 603a 0a20 2060  swarm_spec`:.  `
+00006620: 6578 7465 726e 616c 5f63 6173 602c 2060  external_cas`, `
+00006630: 6c61 6265 6c73 602c 2060 7369 676e 696e  labels`, `signin
+00006640: 675f 6361 5f63 6572 7460 2c20 6073 6967  g_ca_cert`, `sig
+00006650: 6e69 6e67 5f63 615f 6b65 7960 2c0a 2020  ning_ca_key`,.  
+00006660: 6063 615f 666f 7263 655f 726f 7461 7465  `ca_force_rotate
+00006670: 602c 2060 6175 746f 6c6f 636b 5f6d 616e  `, `autolock_man
+00006680: 6167 6572 7360 2c20 606c 6f67 5f64 7269  agers`, `log_dri
+00006690: 7665 7260 2e20 5468 6573 6520 6164 6469  ver`. These addi
+000066a0: 7469 6f6e 730a 2020 616c 736f 2061 7070  tions.  also app
+000066b0: 6c79 2074 6f20 6044 6f63 6b65 7243 6c69  ly to `DockerCli
+000066c0: 656e 742e 7377 6172 6d2e 696e 6974 602e  ent.swarm.init`.
+000066d0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+000066e0: 2066 6f72 2060 696e 7365 7274 5f64 6566   for `insert_def
+000066f0: 6175 6c74 7360 2069 6e20 6041 5049 436c  aults` in `APICl
+00006700: 6965 6e74 2e69 6e73 7065 6374 5f73 6572  ient.inspect_ser
+00006710: 7669 6365 6020 616e 640a 2020 6044 6f63  vice` and.  `Doc
+00006720: 6b65 7243 6c69 656e 742e 7365 7276 6963  kerClient.servic
+00006730: 6573 2e67 6574 602e 0a0a 2323 2320 4275  es.get`...### Bu
+00006740: 6766 6978 6573 0a0a 2a20 4669 7865 6420  gfixes..* Fixed 
+00006750: 6120 6275 6720 7768 6572 6520 7265 6164  a bug where read
+00006760: 696e 6720 6120 302d 6c65 6e67 7468 2066  ing a 0-length f
+00006770: 7261 6d65 2069 6e20 6c6f 6720 7374 7265  rame in log stre
+00006780: 616d 7320 776f 756c 6420 696e 636f 7272  ams would incorr
+00006790: 6563 746c 790a 2020 696e 7465 7272 7570  ectly.  interrup
+000067a0: 7420 7374 7265 616d 696e 672e 0a2a 2046  t streaming..* F
+000067b0: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+000067c0: 2074 6865 2060 6964 6020 6d65 6d62 6572   the `id` member
+000067d0: 206f 6e20 6053 7761 726d 6020 6f62 6a65   on `Swarm` obje
+000067e0: 6374 7320 7761 736e 2774 2062 6569 6e67  cts wasn't being
+000067f0: 2070 6f70 756c 6174 6564 2e0a 2a20 4669   populated..* Fi
+00006800: 7865 6420 6120 6275 6720 7468 6174 2077  xed a bug that w
+00006810: 6f75 6c64 2063 6175 7365 2073 6f6d 6520  ould cause some 
+00006820: 6461 7461 2061 7420 7468 6520 6265 6769  data at the begi
+00006830: 6e6e 696e 6720 6f66 2061 6e20 7570 6772  nning of an upgr
+00006840: 6164 6564 0a20 2063 6f6e 6e65 6374 696f  aded.  connectio
+00006850: 6e20 7374 7265 616d 2028 6061 7474 6163  n stream (`attac
+00006860: 6860 2c20 6065 7865 635f 7275 6e60 2920  h`, `exec_run`) 
+00006870: 746f 2064 6973 6170 7065 6172 2e0a 0a32  to disappear...2
+00006880: 2e35 2e31 0a2d 2d2d 2d2d 0a0a 5b4c 6973  .5.1.-----..[Lis
+00006890: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
+000068a0: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+000068b0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+000068c0: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
+000068d0: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
+000068e0: 652f 3337 3f63 6c6f 7365 643d 3129 0a0a  e/37?closed=1)..
+000068f0: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
+00006900: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+00006910: 6520 7061 7474 6572 6e73 2065 6e64 696e  e patterns endin
+00006920: 6720 7769 7468 2060 2a2a 6020 696e 2060  g with `**` in `
+00006930: 2e64 6f63 6b65 7269 676e 6f72 6560 2077  .dockerignore` w
+00006940: 6f75 6c64 0a20 2072 6169 7365 2061 6e20  ould.  raise an 
+00006950: 6578 6365 7074 696f 6e0a 2a20 4669 7865  exception.* Fixe
+00006960: 6420 6120 6275 6720 7768 6572 6520 7573  d a bug where us
+00006970: 696e 6720 6061 7474 6163 6860 2077 6974  ing `attach` wit
+00006980: 6820 7468 6520 6073 7472 6561 6d60 2061  h the `stream` a
+00006990: 7267 756d 656e 7420 7365 7420 746f 2060  rgument set to `
+000069a0: 4661 6c73 6560 0a20 2077 6f75 6c64 2072  False`.  would r
+000069b0: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
+000069c0: 6e0a 0a32 2e35 2e30 0a2d 2d2d 2d2d 0a0a  n..2.5.0.-----..
+000069d0: 5b4c 6973 7420 6f66 2050 5273 202f 2069  [List of PRs / i
+000069e0: 7373 7565 7320 666f 7220 7468 6973 2072  ssues for this r
+000069f0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00006a00: 6769 7468 7562 2e63 6f6d 2f64 6f63 6b65  github.com/docke
+00006a10: 722f 646f 636b 6572 2d70 792f 6d69 6c65  r/docker-py/mile
+00006a20: 7374 6f6e 652f 3334 3f63 6c6f 7365 643d  stone/34?closed=
+00006a30: 3129 0a0a 2323 2320 4665 6174 7572 6573  1)..### Features
+00006a40: 0a0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
+00006a50: 7420 666f 7220 7468 6520 6073 7175 6173  t for the `squas
+00006a60: 6860 2070 6172 616d 6574 6572 2069 6e20  h` parameter in 
+00006a70: 6041 5049 436c 6965 6e74 2e62 7569 6c64  `APIClient.build
+00006a80: 6020 616e 640a 2020 6044 6f63 6b65 7243  ` and.  `DockerC
+00006a90: 6c69 656e 742e 696d 6167 6573 2e62 7569  lient.images.bui
+00006aa0: 6c64 602e 0a2a 2057 6865 6e20 7573 696e  ld`..* When usin
+00006ab0: 6720 4150 4920 7665 7273 696f 6e20 312e  g API version 1.
+00006ac0: 3233 206f 7220 6162 6f76 652c 2060 6c6f  23 or above, `lo
+00006ad0: 6164 5f69 6d61 6765 6020 7769 6c6c 206e  ad_image` will n
+00006ae0: 6f77 2072 6574 7572 6e20 610a 2020 6765  ow return a.  ge
+00006af0: 6e65 7261 746f 7220 6f66 2070 726f 6772  nerator of progr
+00006b00: 6573 7320 6173 204a 534f 4e20 6064 6963  ess as JSON `dic
+00006b10: 7460 732e 0a2a 2060 7265 6d6f 7665 5f69  t`s..* `remove_i
+00006b20: 6d61 6765 6020 6e6f 7720 7265 7475 726e  mage` now return
+00006b30: 7320 7468 6520 636f 6e74 656e 7420 6f66  s the content of
+00006b40: 2074 6865 2041 5049 2773 2072 6573 706f   the API's respo
+00006b50: 6e73 652e 0a0a 0a23 2323 2042 7567 6669  nse....### Bugfi
+00006b60: 7865 730a 0a2a 2046 6978 6564 2061 6e20  xes..* Fixed an 
+00006b70: 6973 7375 6520 7768 6572 6520 7468 6520  issue where the 
+00006b80: 6061 7574 6f5f 7265 6d6f 7665 6020 7061  `auto_remove` pa
+00006b90: 7261 6d65 7465 7220 696e 0a20 2060 446f  rameter in.  `Do
+00006ba0: 636b 6572 436c 6965 6e74 2e63 6f6e 7461  ckerClient.conta
+00006bb0: 696e 6572 732e 7275 6e60 2077 6173 206e  iners.run` was n
+00006bc0: 6f74 2074 616b 656e 2069 6e74 6f20 6163  ot taken into ac
+00006bd0: 636f 756e 742e 0a2a 2046 6978 6564 2061  count..* Fixed a
+00006be0: 2062 7567 2077 6865 7265 2060 2e64 6f63   bug where `.doc
+00006bf0: 6b65 7269 676e 6f72 6560 2070 6174 7465  kerignore` patte
+00006c00: 726e 7320 7374 6172 7469 6e67 2077 6974  rns starting wit
+00006c10: 6820 6120 736c 6173 680a 2020 7765 7265  h a slash.  were
+00006c20: 2069 676e 6f72 6564 2e0a 2a20 4669 7865   ignored..* Fixe
+00006c30: 6420 616e 2069 7373 7565 2077 6974 6820  d an issue with 
+00006c40: 7468 6520 6861 6e64 6c69 6e67 206f 6620  the handling of 
+00006c50: 602a 2a60 2070 6174 7465 726e 7320 696e  `**` patterns in
+00006c60: 2060 2e64 6f63 6b65 7269 676e 6f72 6560   `.dockerignore`
+00006c70: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00006c80: 6865 7265 2062 7569 6c64 696e 6720 6046  here building `F
+00006c90: 524f 4d60 2061 2070 7269 7661 7465 2044  ROM` a private D
+00006ca0: 6f63 6b65 7220 4875 6220 696d 6167 6520  ocker Hub image 
+00006cb0: 7768 656e 206e 6f74 0a20 2075 7369 6e67  when not.  using
+00006cc0: 2061 2063 7265 6420 7374 6f72 6520 776f   a cred store wo
+00006cd0: 756c 6420 6661 696c 2e0a 2a20 4669 7865  uld fail..* Fixe
+00006ce0: 6420 6120 6275 6720 7768 6572 6520 6361  d a bug where ca
+00006cf0: 6c6c 696e 6720 6063 7265 6174 655f 7365  lling `create_se
+00006d00: 7276 6963 6560 206f 7220 6075 7064 6174  rvice` or `updat
+00006d10: 655f 7365 7276 6963 6560 2077 6974 680a  e_service` with.
+00006d20: 2020 6074 6173 6b5f 7465 6d70 6c61 7465    `task_template
+00006d30: 6020 6173 2061 2060 6469 6374 6020 776f  ` as a `dict` wo
+00006d40: 756c 6420 7261 6973 6520 616e 2065 7863  uld raise an exc
+00006d50: 6570 7469 6f6e 2e0a 2a20 4669 7865 6420  eption..* Fixed 
+00006d60: 7468 6520 6861 6e64 6c69 6e67 206f 6620  the handling of 
+00006d70: 5454 592d 656e 6162 6c65 6420 636f 6e74  TTY-enabled cont
+00006d80: 6169 6e65 7273 2069 6e20 6061 7474 6163  ainers in `attac
+00006d90: 6860 2061 6e64 2060 6578 6563 5f72 756e  h` and `exec_run
+00006da0: 602e 0a2a 2060 446f 636b 6572 436c 6965  `..* `DockerClie
+00006db0: 6e74 2e63 6f6e 7461 696e 6572 732e 7275  nt.containers.ru
+00006dc0: 6e60 2077 696c 6c20 6e6f 206c 6f6e 6765  n` will no longe
+00006dd0: 7220 6174 7465 6d70 7420 746f 2073 7472  r attempt to str
+00006de0: 6561 6d20 6c6f 6773 2069 6620 7468 650a  eam logs if the.
+00006df0: 2020 6c6f 6720 6472 6976 6572 2064 6f65    log driver doe
+00006e00: 736e 2774 2073 7570 706f 7274 2074 6865  sn't support the
+00006e10: 206f 7065 7261 7469 6f6e 2e0a 0a23 2323   operation...###
+00006e20: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
+00006e30: 2a20 4164 6465 6420 6578 7472 6120 7265  * Added extra re
+00006e40: 7175 6972 656d 656e 7473 2066 6f72 2062  quirements for b
+00006e50: 6574 7465 7220 544c 5320 7375 7070 6f72  etter TLS suppor
+00006e60: 7420 6f6e 2073 6f6d 6520 706c 6174 666f  t on some platfo
+00006e70: 726d 732e 0a20 2054 6865 7365 2063 616e  rms..  These can
+00006e80: 2062 6520 696e 7374 616c 6c65 6420 6f72   be installed or
+00006e90: 2072 6571 7569 7265 6420 7468 726f 7567   required throug
+00006ea0: 6820 7468 6520 6064 6f63 6b65 725b 746c  h the `docker[tl
+00006eb0: 735d 6020 6e6f 7461 7469 6f6e 2e0a 0a32  s]` notation...2
+00006ec0: 2e34 2e32 0a2d 2d2d 2d2d 0a0a 5b4c 6973  .4.2.-----..[Lis
+00006ed0: 7420 6f66 2050 5273 202f 2069 7373 7565  t of PRs / issue
+00006ee0: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+00006ef0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+00006f00: 7562 2e63 6f6d 2f64 6f63 6b65 722f 646f  ub.com/docker/do
+00006f10: 636b 6572 2d70 792f 6d69 6c65 7374 6f6e  cker-py/mileston
+00006f20: 652f 3336 3f63 6c6f 7365 643d 3129 0a0a  e/36?closed=1)..
+00006f30: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
+00006f40: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+00006f50: 6520 7468 6520 6073 706c 6974 5f70 6f72  e the `split_por
+00006f60: 7460 2075 7469 6c69 7479 2077 6f75 6c64  t` utility would
+00006f70: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
+00006f80: 696f 6e20 7768 656e 0a20 2070 6173 7365  ion when.  passe
+00006f90: 6420 6120 6e6f 6e2d 7374 7269 6e67 2061  d a non-string a
+00006fa0: 7267 756d 656e 742e 0a0a 322e 342e 300a  rgument...2.4.0.
+00006fb0: 2d2d 2d2d 2d0a 0a5b 4c69 7374 206f 6620  -----..[List of 
+00006fc0: 5052 7320 2f20 6973 7375 6573 2066 6f72  PRs / issues for
+00006fd0: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
+00006fe0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00006ff0: 6d2f 646f 636b 6572 2f64 6f63 6b65 722d  m/docker/docker-
+00007000: 7079 2f6d 696c 6573 746f 6e65 2f33 333f  py/milestone/33?
+00007010: 636c 6f73 6564 3d31 290a 0a23 2323 2046  closed=1)..### F
+00007020: 6561 7475 7265 730a 0a2a 2041 6464 6564  eatures..* Added
+00007030: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
+00007040: 2060 7461 7267 6574 6020 616e 6420 606e   `target` and `n
+00007050: 6574 776f 726b 5f6d 6f64 6560 2070 6172  etwork_mode` par
+00007060: 616d 6574 6572 7320 696e 0a20 2060 4150  ameters in.  `AP
+00007070: 4943 6c69 656e 742e 6275 696c 6460 2061  IClient.build` a
+00007080: 6e64 2060 446f 636b 6572 436c 6965 6e74  nd `DockerClient
+00007090: 2e69 6d61 6765 732e 6275 696c 6460 2e0a  .images.build`..
+000070a0: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+000070b0: 666f 7220 7468 6520 6072 756e 7469 6d65  for the `runtime
+000070c0: 6020 7061 7261 6d65 7465 7220 696e 2060  ` parameter in `
+000070d0: 4150 4943 6c69 656e 742e 6372 6561 7465  APIClient.create
+000070e0: 5f63 6f6e 7461 696e 6572 600a 2020 616e  _container`.  an
+000070f0: 6420 6044 6f63 6b65 7243 6c69 656e 742e  d `DockerClient.
+00007100: 636f 6e74 6169 6e65 7273 2e72 756e 602e  containers.run`.
+00007110: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00007120: 2066 6f72 2074 6865 2060 696e 6772 6573   for the `ingres
+00007130: 7360 2070 6172 616d 6574 6572 2069 6e20  s` parameter in 
+00007140: 6041 5049 436c 6965 6e74 2e63 7265 6174  `APIClient.creat
+00007150: 655f 6e65 7477 6f72 6b60 2061 6e64 0a20  e_network` and. 
+00007160: 2060 446f 636b 6572 436c 6965 6e74 2e6e   `DockerClient.n
+00007170: 6574 776f 726b 732e 6372 6561 7465 602e  etworks.create`.
+00007180: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00007190: 2066 6f72 2060 706c 6163 656d 656e 7460   for `placement`
+000071a0: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
+000071b0: 6e20 6064 6f63 6b65 722e 7479 7065 732e  n `docker.types.
+000071c0: 5461 736b 5465 6d70 6c61 7465 602e 0a2a  TaskTemplate`..*
+000071d0: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
+000071e0: 6f72 2060 7474 7960 2063 6f6e 6669 6775  or `tty` configu
+000071f0: 7261 7469 6f6e 2069 6e20 6064 6f63 6b65  ration in `docke
+00007200: 722e 7479 7065 732e 436f 6e74 6169 6e65  r.types.Containe
+00007210: 7253 7065 6360 2e0a 2a20 4164 6465 6420  rSpec`..* Added 
+00007220: 7375 7070 6f72 7420 666f 7220 6073 7461  support for `sta
+00007230: 7274 5f70 6572 696f 6460 2063 6f6e 6669  rt_period` confi
+00007240: 6775 7261 7469 6f6e 2069 6e20 6064 6f63  guration in `doc
+00007250: 6b65 722e 7479 7065 732e 4865 616c 7468  ker.types.Health
+00007260: 6368 6563 6b60 2e0a 2a20 5468 6520 6063  check`..* The `c
+00007270: 7265 6448 656c 7065 7273 6020 7365 6374  redHelpers` sect
+00007280: 696f 6e20 696e 2044 6f63 6b65 7227 7320  ion in Docker's 
+00007290: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+000072a0: 6c65 2069 7320 6e6f 7720 7265 636f 676e  le is now recogn
+000072b0: 697a 6564 2e0a 2a20 506f 7274 2073 7065  ized..* Port spe
+000072c0: 6369 6669 6361 7469 6f6e 7320 696e 636c  cifications incl
+000072d0: 7564 696e 6720 4950 7636 2065 6e64 706f  uding IPv6 endpo
+000072e0: 696e 7473 2061 7265 206e 6f77 2073 7570  ints are now sup
+000072f0: 706f 7274 6564 2e0a 0a23 2323 2042 7567  ported...### Bug
+00007300: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
+00007310: 2062 7567 2077 6865 7265 2069 6e73 7461   bug where insta
+00007320: 6e74 6961 7469 6e67 2061 2060 446f 636b  ntiating a `Dock
+00007330: 6572 436c 6965 6e74 6020 7573 696e 6720  erClient` using 
+00007340: 6064 6f63 6b65 722e 6672 6f6d 5f65 6e76  `docker.from_env
+00007350: 600a 2020 776f 756c 646e 2774 2063 6f72  `.  wouldn't cor
+00007360: 7265 6374 6c79 2073 6574 2074 6865 2064  rectly set the d
+00007370: 6566 6175 6c74 2074 696d 656f 7574 2076  efault timeout v
+00007380: 616c 7565 2e0a 2a20 4669 7865 6420 6120  alue..* Fixed a 
+00007390: 6275 6720 7768 6572 6520 6044 6f63 6b65  bug where `Docke
+000073a0: 7243 6c69 656e 742e 7365 6372 6574 7360  rClient.secrets`
+000073b0: 2077 6173 206e 6f74 2061 6363 6573 7369   was not accessi
+000073c0: 626c 6520 6173 2061 2070 726f 7065 7274  ble as a propert
+000073d0: 792e 0a2a 2046 6978 6564 2061 2062 7567  y..* Fixed a bug
+000073e0: 2077 6865 7265 2060 446f 636b 6572 436c   where `DockerCl
+000073f0: 6965 6e74 2e62 7569 6c64 6020 776f 756c  ient.build` woul
+00007400: 6420 736f 6d65 7469 6d65 7320 7265 7475  d sometimes retu
+00007410: 726e 2074 6865 2077 726f 6e67 0a20 2069  rn the wrong.  i
+00007420: 6d61 6765 2e0a 2a20 4669 7865 6420 6120  mage..* Fixed a 
+00007430: 6275 6720 7768 6572 6520 7661 6c75 6573  bug where values
+00007440: 2066 6f72 2060 486f 7374 436f 6e66 6967   for `HostConfig
+00007450: 2e6e 616e 6f5f 6370 7573 6020 6578 6365  .nano_cpus` exce
+00007460: 6564 696e 6720 325e 3332 2077 6f75 6c64  eding 2^32 would
+00007470: 0a20 2072 6169 7365 2061 2074 7970 6520  .  raise a type 
+00007480: 6572 726f 722e 0a2a 2060 496d 6167 652e  error..* `Image.
+00007490: 7461 6760 206e 6f77 2070 726f 7065 726c  tag` now properl
+000074a0: 7920 7265 7475 726e 7320 6054 7275 6560  y returns `True`
+000074b0: 2077 6865 6e20 7468 6520 6f70 6572 6174   when the operat
+000074c0: 696f 6e20 6973 2073 7563 6365 7373 6675  ion is successfu
+000074d0: 6c2e 0a2a 2060 4150 4943 6c69 656e 742e  l..* `APIClient.
+000074e0: 6c6f 6773 6020 616e 6420 6043 6f6e 7461  logs` and `Conta
+000074f0: 696e 6572 2e6c 6f67 7360 206e 6f77 2072  iner.logs` now r
+00007500: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
+00007510: 6e20 6966 2074 6865 2060 7369 6e63 6560  n if the `since`
+00007520: 0a20 2061 7267 756d 656e 7420 7573 6573  .  argument uses
+00007530: 2061 6e20 756e 7375 7070 6f72 7465 6420   an unsupported 
+00007540: 7479 7065 2069 6e73 7465 6164 206f 6620  type instead of 
+00007550: 6967 6e6f 7269 6e67 2074 6865 2076 616c  ignoring the val
+00007560: 7565 2e0a 2a20 4669 7865 6420 6120 6275  ue..* Fixed a bu
+00007570: 6720 7768 6572 6520 736f 6d65 206d 6574  g where some met
+00007580: 686f 6473 2077 6f75 6c64 2072 6169 7365  hods would raise
+00007590: 2061 2060 4e75 6c6c 5265 736f 7572 6365   a `NullResource
+000075a0: 6020 6578 6365 7074 696f 6e20 7768 656e  ` exception when
+000075b0: 0a20 2074 6865 2072 6573 6f75 7263 6520  .  the resource 
+000075c0: 4944 2077 6173 2070 726f 7669 6465 6420  ID was provided 
+000075d0: 7573 696e 6720 6120 6b65 7977 6f72 6420  using a keyword 
+000075e0: 6172 6775 6d65 6e74 2e0a 0a23 2323 204d  argument...### M
+000075f0: 6973 6365 6c6c 616e 656f 7573 0a0a 2a20  iscellaneous..* 
+00007600: 6041 5049 436c 6965 6e74 6020 696e 7374  `APIClient` inst
+00007610: 616e 6365 7320 6361 6e20 6e6f 7720 6265  ances can now be
+00007620: 2070 6963 6b6c 6564 2e0a 0a32 2e33 2e30   pickled...2.3.0
+00007630: 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66  .-----..[List of
+00007640: 2050 5273 202f 2069 7373 7565 7320 666f   PRs / issues fo
+00007650: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
+00007660: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00007670: 6f6d 2f64 6f63 6b65 722f 646f 636b 6572  om/docker/docker
+00007680: 2d70 792f 6d69 6c65 7374 6f6e 652f 3331  -py/milestone/31
+00007690: 3f63 6c6f 7365 643d 3129 0a0a 2323 2320  ?closed=1)..### 
+000076a0: 4665 6174 7572 6573 0a0a 2a20 4164 6465  Features..* Adde
+000076b0: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
+000076c0: 6520 666f 6c6c 6f77 696e 6720 6048 6f73  e following `Hos
+000076d0: 7443 6f6e 6669 6760 2070 6172 616d 6574  tConfig` paramet
+000076e0: 6572 733a 2060 766f 6c75 6d65 5f64 7269  ers: `volume_dri
+000076f0: 7665 7260 2c0a 2020 6063 7075 5f63 6f75  ver`,.  `cpu_cou
+00007700: 6e74 602c 2060 6370 755f 7065 7263 656e  nt`, `cpu_percen
+00007710: 7460 2c20 606e 616e 6f5f 6370 7573 602c  t`, `nano_cpus`,
+00007720: 2060 6370 7573 6574 5f6d 656d 7360 2e0a   `cpuset_mems`..
+00007730: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+00007740: 666f 7220 6076 6572 626f 7365 6020 7061  for `verbose` pa
+00007750: 7261 6d65 7465 7220 696e 2060 4150 4943  rameter in `APIC
+00007760: 6c69 656e 742e 696e 7370 6563 745f 6e65  lient.inspect_ne
+00007770: 7477 6f72 6b60 2061 6e64 0a20 2060 446f  twork` and.  `Do
+00007780: 636b 6572 436c 6965 6e74 2e6e 6574 776f  ckerClient.netwo
+00007790: 726b 732e 6765 7460 2e0a 2a20 4164 6465  rks.get`..* Adde
+000077a0: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
+000077b0: 6520 6065 6e76 6972 6f6e 6d65 6e74 6020  e `environment` 
+000077c0: 7061 7261 6d65 7465 7220 696e 2060 4150  parameter in `AP
+000077d0: 4943 6c69 656e 742e 6578 6563 5f63 7265  IClient.exec_cre
+000077e0: 6174 6560 0a20 2061 6e64 2060 436f 6e74  ate`.  and `Cont
+000077f0: 6169 6e65 722e 6578 6563 5f72 756e 600a  ainer.exec_run`.
+00007800: 2a20 4164 6465 6420 6072 656c 6f61 645f  * Added `reload_
+00007810: 636f 6e66 6967 6020 6d65 7468 6f64 2074  config` method t
+00007820: 6f20 6041 5049 436c 6965 6e74 602c 2074  o `APIClient`, t
+00007830: 6861 7420 6c65 7473 2074 6865 2075 7365  hat lets the use
+00007840: 7220 7265 6c6f 6164 0a20 2074 6865 2060  r reload.  the `
+00007850: 636f 6e66 6967 2e6a 736f 6e60 2064 6174  config.json` dat
+00007860: 6120 6672 6f6d 2064 6973 6b2e 0a2a 2041  a from disk..* A
+00007870: 6464 6564 2060 6c61 6265 6c73 6020 7072  dded `labels` pr
+00007880: 6f70 6572 7479 2074 6f20 7468 6520 6049  operty to the `I
+00007890: 6d61 6765 6020 616e 6420 6043 6f6e 7461  mage` and `Conta
+000078a0: 696e 6572 6020 636c 6173 7365 732e 0a2a  iner` classes..*
+000078b0: 2041 6464 6564 2060 696d 6167 6560 2070   Added `image` p
+000078c0: 726f 7065 7274 7920 746f 2074 6865 2060  roperty to the `
+000078d0: 436f 6e74 6169 6e65 7260 2063 6c61 7373  Container` class
+000078e0: 2e0a 0a23 2323 2042 7567 6669 7865 730a  ...### Bugfixes.
+000078f0: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00007900: 6865 7265 2073 6574 7469 6e67 2060 7265  here setting `re
+00007910: 706c 6963 6173 6020 746f 207a 6572 6f20  plicas` to zero 
+00007920: 696e 2060 5365 7276 6963 654d 6f64 6560  in `ServiceMode`
+00007930: 2077 6f75 6c64 206e 6f74 0a20 2072 6567   would not.  reg
+00007940: 6973 7465 7220 6173 2061 2076 616c 6964  ister as a valid
+00007950: 2065 6e74 7279 2e0a 2a20 4669 7865 6420   entry..* Fixed 
+00007960: 6120 6275 6720 7768 6572 6520 6044 6f63  a bug where `Doc
+00007970: 6b65 7243 6c69 656e 742e 696d 6167 6573  kerClient.images
+00007980: 2e62 7569 6c64 6020 776f 756c 6420 7265  .build` would re
+00007990: 706f 7274 2061 2066 6169 6c75 7265 2061  port a failure a
+000079a0: 6674 6572 0a20 2061 2073 7563 6365 7373  fter.  a success
+000079b0: 6675 6c20 6275 696c 6420 6966 2061 2060  ful build if a `
+000079c0: 7461 6760 2077 6173 2073 6574 2e0a 2a20  tag` was set..* 
+000079d0: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
+000079e0: 6865 7265 2060 446f 636b 6572 436c 6965  here `DockerClie
+000079f0: 6e74 2e69 6d61 6765 732e 7075 6c6c 6020  nt.images.pull` 
+00007a00: 776f 756c 6420 6661 696c 2074 6f20 7265  would fail to re
+00007a10: 7475 726e 2074 6865 0a20 2063 6f72 7265  turn the.  corre
+00007a20: 7370 6f6e 6469 6e67 2069 6d61 6765 206f  sponding image o
+00007a30: 626a 6563 7420 6966 2061 2060 7461 6760  bject if a `tag`
+00007a40: 2077 6173 2073 6574 2e0a 2a20 4669 7865   was set..* Fixe
+00007a50: 6420 6120 6275 6720 7768 6572 6520 6120  d a bug where a 
+00007a60: 6c69 7374 206f 6620 606d 6f75 6e74 7360  list of `mounts`
+00007a70: 2070 726f 7669 6465 6420 746f 2060 4150   provided to `AP
+00007a80: 4943 6c69 656e 742e 6372 6561 7465 5f73  IClient.create_s
+00007a90: 6572 7669 6365 600a 2020 776f 756c 6420  ervice`.  would 
+00007aa0: 736f 6d65 7469 6d65 7320 6265 2070 6172  sometimes be par
+00007ab0: 7365 6420 696e 636f 7272 6563 746c 792e  sed incorrectly.
+00007ac0: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00007ad0: 6865 7265 2063 616c 6c69 6e67 2060 4e65  here calling `Ne
+00007ae0: 7477 6f72 6b2e 636f 6e74 6169 6e65 7273  twork.containers
+00007af0: 6020 776f 756c 6420 6372 6173 6820 7768  ` would crash wh
+00007b00: 656e 206e 6f20 636f 6e74 6169 6e65 7273  en no containers
+00007b10: 0a20 2077 6572 6520 6173 736f 6369 6174  .  were associat
+00007b20: 6564 2077 6974 6820 7468 6520 6e65 7477  ed with the netw
+00007b30: 6f72 6b2e 0a2a 2046 6978 6564 2061 6e20  ork..* Fixed an 
+00007b40: 6973 7375 6520 7768 6572 6520 604e 6574  issue where `Net
+00007b50: 776f 726b 2e63 6f6e 6e65 6374 6020 616e  work.connect` an
+00007b60: 6420 604e 6574 776f 726b 2e64 6973 636f  d `Network.disco
+00007b70: 6e6e 6563 7460 2077 6f75 6c64 206e 6f74  nnect` would not
+00007b80: 0a20 2061 6363 6570 7420 736f 6d65 206f  .  accept some o
+00007b90: 6620 7468 6520 646f 6375 6d65 6e74 6564  f the documented
+00007ba0: 2070 6172 616d 6574 6572 732e 0a2a 2046   parameters..* F
+00007bb0: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+00007bc0: 2074 6865 2060 6370 7573 6574 5f63 7075   the `cpuset_cpu
+00007bd0: 7360 2070 6172 616d 6574 6572 2077 6f75  s` parameter wou
+00007be0: 6c64 206e 6f74 2062 6520 7072 6f70 6572  ld not be proper
+00007bf0: 6c79 2073 6574 2069 6e0a 2020 6041 5049  ly set in.  `API
+00007c00: 436c 6965 6e74 2e63 7265 6174 655f 686f  Client.create_ho
+00007c10: 7374 5f63 6f6e 6669 6760 2e0a 0a23 2323  st_config`...###
+00007c20: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
+00007c30: 2a20 5468 6520 696e 7661 6c69 6420 606e  * The invalid `n
+00007c40: 6574 776f 726b 7360 2061 7267 756d 656e  etworks` argumen
+00007c50: 7420 696e 2060 446f 636b 6572 436c 6965  t in `DockerClie
+00007c60: 6e74 2e63 6f6e 7461 696e 6572 732e 7275  nt.containers.ru
+00007c70: 6e60 2068 6173 2062 6565 6e0a 2020 7265  n` has been.  re
+00007c80: 706c 6163 6564 2077 6974 6820 6120 2877  placed with a (w
+00007c90: 6f72 6b69 6e67 2920 7369 6e67 756c 6172  orking) singular
+00007ca0: 2060 6e65 7477 6f72 6b60 2061 7267 756d   `network` argum
+00007cb0: 656e 742e 0a0a 0a32 2e32 2e31 0a2d 2d2d  ent....2.2.1.---
+00007cc0: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
+00007cd0: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
+00007ce0: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
+00007cf0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00007d00: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
+00007d10: 6d69 6c65 7374 6f6e 652f 3332 3f63 6c6f  milestone/32?clo
+00007d20: 7365 643d 3129 0a0a 2323 2320 4275 6766  sed=1)..### Bugf
+00007d30: 6978 6573 0a0a 2a20 4669 7865 6420 6120  ixes..* Fixed a 
+00007d40: 6275 6720 7768 6572 6520 7468 6520 6073  bug where the `s
+00007d50: 7461 7475 735f 636f 6465 6020 6174 7472  tatus_code` attr
+00007d60: 6962 7574 6520 6f66 2060 4150 4945 7272  ibute of `APIErr
+00007d70: 6f72 6020 6578 6365 7074 696f 6e73 2077  or` exceptions w
+00007d80: 6f75 6c64 0a20 206e 6f74 2072 6566 6c65  ould.  not refle
+00007d90: 6374 2074 6865 2065 7870 6563 7465 6420  ct the expected 
+00007da0: 7661 6c75 652e 0a2a 2046 6978 6564 2061  value..* Fixed a
+00007db0: 6e20 6973 7375 6520 7768 6572 6520 7468  n issue where th
+00007dc0: 6520 6065 7665 6e74 7360 206d 6574 686f  e `events` metho
+00007dd0: 6420 776f 756c 6420 7469 6d65 206f 7574  d would time out
+00007de0: 2075 6e65 7870 6563 7465 646c 7920 6966   unexpectedly if
+00007df0: 206e 6f0a 2020 6461 7461 2077 6173 2073   no.  data was s
+00007e00: 656e 7420 6279 2074 6865 2065 6e67 696e  ent by the engin
+00007e10: 6520 666f 7220 6120 6769 7665 6e20 616d  e for a given am
+00007e20: 6f75 6e74 206f 6620 7469 6d65 2e0a 0a0a  ount of time....
+00007e30: 322e 322e 300a 2d2d 2d2d 2d0a 0a5b 4c69  2.2.0.-----..[Li
+00007e40: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+00007e50: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+00007e60: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+00007e70: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+00007e80: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
+00007e90: 6e65 2f33 303f 636c 6f73 6564 3d31 290a  ne/30?closed=1).
+00007ea0: 0a23 2323 2046 6561 7475 7265 730a 0a2a  .### Features..*
+00007eb0: 2044 6566 6175 6c74 2041 5049 2076 6572   Default API ver
+00007ec0: 7369 6f6e 2068 6173 2062 6565 6e20 6275  sion has been bu
+00007ed0: 6d70 6564 2074 6f20 6031 2e32 3660 2028  mped to `1.26` (
+00007ee0: 456e 6769 6e65 2031 2e31 332e 312b 290a  Engine 1.13.1+).
+00007ef0: 2a20 5570 6772 6164 6520 706c 7567 696e  * Upgrade plugin
+00007f00: 3a0a 2020 2a20 4164 6465 6420 7468 6520  :.  * Added the 
+00007f10: 6075 7067 7261 6465 5f70 6c75 6769 6e60  `upgrade_plugin`
+00007f20: 206d 6574 686f 6420 746f 2074 6865 2060   method to the `
+00007f30: 4150 4943 6c69 656e 7460 2063 6c61 7373  APIClient` class
+00007f40: 0a20 202a 2041 6464 6564 2074 6865 2060  .  * Added the `
+00007f50: 7570 6772 6164 6560 206d 6574 686f 6420  upgrade` method 
+00007f60: 746f 2074 6865 2060 506c 7567 696e 6020  to the `Plugin` 
+00007f70: 636c 6173 730a 2a20 5365 7276 6963 6520  class.* Service 
+00007f80: 6c6f 6773 3a0a 2020 2a20 4164 6465 6420  logs:.  * Added 
+00007f90: 7468 6520 6073 6572 7669 6365 5f6c 6f67  the `service_log
+00007fa0: 7360 206d 6574 686f 6420 746f 2074 6865  s` method to the
+00007fb0: 2060 4150 4943 6c69 656e 7460 2063 6c61   `APIClient` cla
+00007fc0: 7373 0a20 202a 2041 6464 6564 2074 6865  ss.  * Added the
+00007fd0: 2060 6c6f 6773 6020 6d65 7468 6f64 2074   `logs` method t
+00007fe0: 6f20 7468 6520 6053 6572 7669 6365 6020  o the `Service` 
+00007ff0: 636c 6173 730a 2a20 4164 6465 6420 7468  class.* Added th
+00008000: 6520 6064 6660 206d 6574 686f 6420 746f  e `df` method to
+00008010: 2060 4150 4943 6c69 656e 7460 2061 6e64   `APIClient` and
+00008020: 2060 446f 636b 6572 436c 6965 6e74 600a   `DockerClient`.
+00008030: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+00008040: 666f 7220 6069 6e69 7460 2061 6e64 2060  for `init` and `
+00008050: 696e 6974 5f70 6174 6860 2070 6172 616d  init_path` param
+00008060: 6574 6572 7320 696e 2060 486f 7374 436f  eters in `HostCo
+00008070: 6e66 6967 600a 2020 616e 6420 6044 6f63  nfig`.  and `Doc
+00008080: 6b65 7243 6c69 656e 742e 636f 6e74 6169  kerClient.contai
+00008090: 6e65 7273 2e72 756e 600a 2a20 4164 6465  ners.run`.* Adde
+000080a0: 6420 7375 7070 6f72 7420 666f 7220 6068  d support for `h
+000080b0: 6f73 746e 616d 6560 2070 6172 616d 6574  ostname` paramet
+000080c0: 6572 2069 6e20 6043 6f6e 7461 696e 6572  er in `Container
+000080d0: 5370 6563 6020 616e 640a 2020 6044 6f63  Spec` and.  `Doc
+000080e0: 6b65 7243 6c69 656e 742e 7365 7276 6963  kerClient.servic
+000080f0: 652e 6372 6561 7465 600a 2a20 4164 6465  e.create`.* Adde
+00008100: 6420 7375 7070 6f72 7420 666f 7220 706f  d support for po
+00008110: 7274 2072 616e 6765 2074 6f20 7369 6e67  rt range to sing
+00008120: 6c65 2070 6f72 7420 696e 2070 6f72 7420  le port in port 
+00008130: 6d61 7070 696e 6773 0a20 2028 652e 672e  mappings.  (e.g.
+00008140: 2060 3830 3030 2d38 3031 303a 3830 6029   `8000-8010:80`)
+00008150: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
+00008160: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+00008170: 6572 6520 6120 6d69 7373 696e 6720 636f  ere a missing co
+00008180: 6e74 6169 6e65 7220 706f 7274 2069 6e20  ntainer port in 
+00008190: 6120 706f 7274 206d 6170 7069 6e67 2077  a port mapping w
+000081a0: 6f75 6c64 2072 6169 7365 0a20 2061 6e20  ould raise.  an 
+000081b0: 756e 6578 7065 6374 6564 2060 5479 7065  unexpected `Type
+000081c0: 4572 726f 7260 0a2a 2046 6978 6564 2061  Error`.* Fixed a
+000081d0: 2062 7567 2077 6865 7265 2074 6865 2060   bug where the `
+000081e0: 6576 656e 7473 6020 6d65 7468 6f64 2069  events` method i
+000081f0: 6e20 6041 5049 436c 6965 6e74 6020 616e  n `APIClient` an
+00008200: 6420 6044 6f63 6b65 7243 6c69 656e 7460  d `DockerClient`
+00008210: 0a20 2077 6f75 6c64 206e 6f74 2072 6573  .  would not res
+00008220: 7065 6374 2063 7573 746f 6d20 6865 6164  pect custom head
+00008230: 6572 7320 7365 7420 696e 2060 636f 6e66  ers set in `conf
+00008240: 6967 2e6a 736f 6e60 0a0a 0a32 2e31 2e30  ig.json`...2.1.0
+00008250: 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66  .-----..[List of
+00008260: 2050 5273 202f 2069 7373 7565 7320 666f   PRs / issues fo
+00008270: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
+00008280: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00008290: 6f6d 2f64 6f63 6b65 722f 646f 636b 6572  om/docker/docker
+000082a0: 2d70 792f 6d69 6c65 7374 6f6e 652f 3237  -py/milestone/27
+000082b0: 3f63 6c6f 7365 643d 3129 0a0a 2323 2320  ?closed=1)..### 
+000082c0: 4665 6174 7572 6573 0a0a 2a20 4164 6465  Features..* Adde
+000082d0: 6420 7468 6520 666f 6c6c 6f77 696e 6720  d the following 
+000082e0: 7072 756e 696e 6720 6d65 7468 6f64 733a  pruning methods:
+000082f0: 0a20 2020 202a 2049 6e20 6041 5049 436c  .    * In `APICl
+00008300: 6965 6e74 603a 2060 7072 756e 655f 636f  ient`: `prune_co
+00008310: 6e74 6169 6e65 7273 602c 2060 7072 756e  ntainers`, `prun
+00008320: 655f 696d 6167 6573 602c 2060 7072 756e  e_images`, `prun
+00008330: 655f 6e65 7477 6f72 6b73 602c 0a20 2020  e_networks`,.   
+00008340: 2020 2060 7072 756e 655f 766f 6c75 6d65     `prune_volume
+00008350: 7360 0a20 2020 202a 2049 6e20 6044 6f63  s`.    * In `Doc
+00008360: 6b65 7243 6c69 656e 7460 3a20 6063 6f6e  kerClient`: `con
+00008370: 7461 696e 6572 732e 7072 756e 6560 2c20  tainers.prune`, 
+00008380: 6069 6d61 6765 732e 7072 756e 6560 2c20  `images.prune`, 
+00008390: 606e 6574 776f 726b 732e 7072 756e 6560  `networks.prune`
+000083a0: 2c0a 2020 2020 2020 6076 6f6c 756d 6573  ,.      `volumes
+000083b0: 2e70 7275 6e65 600a 2a20 4164 6465 6420  .prune`.* Added 
+000083c0: 7375 7070 6f72 7420 666f 7220 7468 6520  support for the 
+000083d0: 706c 7567 696e 7320 4150 493a 0a20 2020  plugins API:.   
+000083e0: 202a 2049 6e20 6041 5049 436c 6965 6e74   * In `APIClient
+000083f0: 603a 2060 636f 6e66 6967 7572 655f 706c  `: `configure_pl
+00008400: 7567 696e 602c 2060 6372 6561 7465 5f70  ugin`, `create_p
+00008410: 6c75 6769 6e60 2c20 6064 6973 6162 6c65  lugin`, `disable
+00008420: 5f70 6c75 6769 6e60 2c0a 2020 2020 2020  _plugin`,.      
+00008430: 6065 6e61 626c 655f 706c 7567 696e 602c  `enable_plugin`,
+00008440: 2060 696e 7370 6563 745f 706c 7567 696e   `inspect_plugin
+00008450: 602c 2060 7075 6c6c 5f70 6c75 6769 6e60  `, `pull_plugin`
+00008460: 2c20 6070 6c75 6769 6e73 602c 0a20 2020  , `plugins`,.   
+00008470: 2020 2060 706c 7567 696e 5f70 7269 7669     `plugin_privi
+00008480: 6c65 6765 7360 2c20 6070 7573 685f 706c  leges`, `push_pl
+00008490: 7567 696e 602c 2060 7265 6d6f 7665 5f70  ugin`, `remove_p
+000084a0: 6c75 6769 6e60 0a20 2020 202a 2049 6e20  lugin`.    * In 
+000084b0: 6044 6f63 6b65 7243 6c69 656e 7460 3a20  `DockerClient`: 
+000084c0: 6070 6c75 6769 6e73 2e63 7265 6174 6560  `plugins.create`
+000084d0: 2c20 6070 6c75 6769 6e73 2e67 6574 602c  , `plugins.get`,
+000084e0: 2060 706c 7567 696e 732e 696e 7374 616c   `plugins.instal
+000084f0: 6c60 2c0a 2020 2020 2020 6070 6c75 6769  l`,.      `plugi
+00008500: 6e73 2e6c 6973 7460 2c20 616e 6420 7468  ns.list`, and th
+00008510: 6520 6050 6c75 6769 6e60 206d 6f64 656c  e `Plugin` model
+00008520: 2e0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
+00008530: 7420 666f 7220 7468 6520 7365 6372 6574  t for the secret
+00008540: 7320 4150 493a 0a20 2020 202a 2049 6e20  s API:.    * In 
+00008550: 6041 5049 436c 6965 6e74 603a 2060 6372  `APIClient`: `cr
+00008560: 6561 7465 5f73 6563 7265 7460 2c20 6069  eate_secret`, `i
+00008570: 6e73 7065 6374 5f73 6563 7265 7460 2c20  nspect_secret`, 
+00008580: 6072 656d 6f76 655f 7365 6372 6574 602c  `remove_secret`,
+00008590: 0a20 2020 2020 2060 7365 6372 6574 7360  .      `secrets`
+000085a0: 0a20 2020 202a 2049 6e20 6044 6f63 6b65  .    * In `Docke
+000085b0: 7243 6c69 656e 7460 3a20 6073 6563 7265  rClient`: `secre
+000085c0: 742e 6372 6561 7465 602c 2060 7365 6372  t.create`, `secr
+000085d0: 6574 2e67 6574 602c 2060 7365 6372 6574  et.get`, `secret
+000085e0: 2e6c 6973 7460 2061 6e64 0a20 2020 2020  .list` and.     
+000085f0: 2074 6865 2060 5365 6372 6574 6020 6d6f   the `Secret` mo
+00008600: 6465 6c2e 0a20 2020 202a 2041 6464 6564  del..    * Added
+00008610: 2060 7365 6372 6574 7360 2070 6172 616d   `secrets` param
+00008620: 6574 6572 2074 6f20 6043 6f6e 7461 696e  eter to `Contain
+00008630: 6572 5370 6563 602e 2045 6163 6820 6974  erSpec`. Each it
+00008640: 656d 2069 6e20 7468 6520 6073 6563 7265  em in the `secre
+00008650: 7473 600a 2020 2020 2020 6c69 7374 206d  ts`.      list m
+00008660: 7573 7420 6265 2061 2060 646f 636b 6572  ust be a `docker
+00008670: 2e74 7970 6573 2e53 6563 7265 7452 6566  .types.SecretRef
+00008680: 6572 656e 6365 6020 696e 7374 616e 6365  erence` instance
+00008690: 2e0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
+000086a0: 7420 666f 7220 6063 6163 6865 5f66 726f  t for `cache_fro
+000086b0: 6d60 2069 6e20 6041 5049 436c 6965 6e74  m` in `APIClient
+000086c0: 2e62 7569 6c64 6020 616e 640a 2020 6044  .build` and.  `D
+000086d0: 6f63 6b65 7243 6c69 656e 742e 696d 6167  ockerClient.imag
+000086e0: 6573 2e62 7569 6c64 602e 0a2a 2041 6464  es.build`..* Add
+000086f0: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
+00008700: 6175 746f 5f72 656d 6f76 6560 2061 6e64  auto_remove` and
+00008710: 2060 7374 6f72 6167 655f 6f70 7460 2069   `storage_opt` i
+00008720: 6e0a 2020 6041 5049 436c 6965 6e74 2e63  n.  `APIClient.c
+00008730: 7265 6174 655f 686f 7374 5f63 6f6e 6669  reate_host_confi
+00008740: 6760 2061 6e64 2060 446f 636b 6572 436c  g` and `DockerCl
+00008750: 6965 6e74 2e63 6f6e 7461 696e 6572 732e  ient.containers.
+00008760: 7275 6e60 0a2a 2041 6464 6564 2073 7570  run`.* Added sup
+00008770: 706f 7274 2066 6f72 2060 7374 6f70 5f74  port for `stop_t
+00008780: 696d 656f 7574 6020 696e 2060 4150 4943  imeout` in `APIC
+00008790: 6c69 656e 742e 6372 6561 7465 5f63 6f6e  lient.create_con
+000087a0: 7461 696e 6572 6020 616e 640a 2020 6044  tainer` and.  `D
+000087b0: 6f63 6b65 7243 6c69 656e 742e 636f 6e74  ockerClient.cont
+000087c0: 6169 6e65 7273 2e72 756e 600a 2a20 4164  ainers.run`.* Ad
+000087d0: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
+000087e0: 7468 6520 6066 6f72 6365 6020 7061 7261  the `force` para
+000087f0: 6d65 7465 7220 696e 2060 4150 4943 6c69  meter in `APICli
+00008800: 656e 742e 7265 6d6f 7665 5f76 6f6c 756d  ent.remove_volum
+00008810: 6560 2061 6e64 0a20 2060 566f 6c75 6d65  e` and.  `Volume
+00008820: 2e72 656d 6f76 6560 0a2a 2041 6464 6564  .remove`.* Added
+00008830: 2073 7570 706f 7274 2066 6f72 2060 6d61   support for `ma
+00008840: 785f 6661 696c 7572 655f 7261 7469 6f60  x_failure_ratio`
+00008850: 2061 6e64 2060 6d6f 6e69 746f 7260 2069   and `monitor` i
+00008860: 6e20 6055 7064 6174 6543 6f6e 6669 6760  n `UpdateConfig`
+00008870: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00008880: 2066 6f72 2060 666f 7263 655f 7570 6461   for `force_upda
+00008890: 7465 6020 696e 2060 5461 736b 5465 6d70  te` in `TaskTemp
+000088a0: 6c61 7465 600a 2a20 4d61 6465 2060 6e61  late`.* Made `na
+000088b0: 6d65 6020 7061 7261 6d65 7465 7220 6f70  me` parameter op
+000088c0: 7469 6f6e 616c 2069 6e20 6041 5049 436c  tional in `APICl
+000088d0: 6965 6e74 2e63 7265 6174 655f 766f 6c75  ient.create_volu
+000088e0: 6d65 6020 616e 640a 2020 6044 6f63 6b65  me` and.  `Docke
+000088f0: 7243 6c69 656e 742e 766f 6c75 6d65 732e  rClient.volumes.
+00008900: 6372 6561 7465 600a 0a23 2323 2042 7567  create`..### Bug
+00008910: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
+00008920: 2062 7567 2077 6865 7265 2062 7569 6c64   bug where build
+00008930: 696e 6720 6672 6f6d 2061 2064 6972 6563  ing from a direc
+00008940: 746f 7279 2063 6f6e 7461 696e 696e 6720  tory containing 
+00008950: 736f 636b 6574 2d74 7970 6520 6669 6c65  socket-type file
+00008960: 730a 2020 776f 756c 6420 7261 6973 6520  s.  would raise 
+00008970: 616e 2075 6e65 7870 6563 7465 6420 6041  an unexpected `A
+00008980: 7474 7269 6275 7465 4572 726f 7260 2e0a  ttributeError`..
+00008990: 2a20 4669 7865 6420 616e 2069 7373 7565  * Fixed an issue
+000089a0: 2074 6861 7420 7761 7320 7072 6576 656e   that was preven
+000089b0: 7469 6e67 2074 6865 2060 446f 636b 6572  ting the `Docker
+000089c0: 436c 6965 6e74 2e73 7761 726d 2e69 6e69  Client.swarm.ini
+000089d0: 7460 206d 6574 686f 6420 746f 0a20 2074  t` method to.  t
+000089e0: 616b 6520 696e 746f 2061 6363 6f75 6e74  ake into account
+000089f0: 2061 7267 756d 656e 7473 2070 6173 7365   arguments passe
+00008a00: 6420 746f 2069 742e 0a2a 2060 496d 6167  d to it..* `Imag
+00008a10: 652e 7461 6760 206e 6f77 2063 6f72 7265  e.tag` now corre
+00008a20: 6374 6c79 2072 6574 7572 6e73 2061 2062  ctly returns a b
+00008a30: 6f6f 6c65 616e 2076 616c 7565 2075 706f  oolean value upo
+00008a40: 6e20 636f 6d70 6c65 7469 6f6e 2e0a 2a20  n completion..* 
+00008a50: 4669 7865 6420 7365 7665 7261 6c20 6973  Fixed several is
+00008a60: 7375 6573 2072 656c 6174 6564 2074 6f20  sues related to 
+00008a70: 7061 7373 696e 6720 6076 6f6c 756d 6573  passing `volumes
+00008a80: 6020 696e 0a20 2060 446f 636b 6572 436c  ` in.  `DockerCl
+00008a90: 6965 6e74 2e63 6f6e 7461 696e 6572 732e  ient.containers.
+00008aa0: 7275 6e60 0a2a 2046 6978 6564 2061 6e20  run`.* Fixed an 
+00008ab0: 6973 7375 6520 7768 6572 6520 6044 6f63  issue where `Doc
+00008ac0: 6b65 7243 6c69 656e 742e 696d 6167 652e  kerClient.image.
+00008ad0: 6275 696c 6460 2077 6f75 6c64 6e27 7420  build` wouldn't 
+00008ae0: 7265 7475 726e 2061 6e20 6049 6d61 6765  return an `Image
+00008af0: 600a 2020 6f62 6a65 6374 2065 7665 6e20  `.  object even 
+00008b00: 7768 656e 2074 6865 2062 7569 6c64 2077  when the build w
+00008b10: 6173 2073 7563 6365 7373 6675 6c0a 0a0a  as successful...
+00008b20: 322e 302e 320a 2d2d 2d2d 2d0a 0a5b 4c69  2.0.2.-----..[Li
+00008b30: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+00008b40: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+00008b50: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+00008b60: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+00008b70: 6f63 6b65 722d 7079 2f6d 696c 6573 746f  ocker-py/milesto
+00008b80: 6e65 2f32 393f 636c 6f73 6564 3d31 290a  ne/29?closed=1).
+00008b90: 0a23 2323 2042 7567 6669 7865 730a 0a2a  .### Bugfixes..*
+00008ba0: 2049 6e73 7461 6c6c 6174 696f 6e20 6f66   Installation of
+00008bb0: 2074 6865 2070 6163 6b61 6765 206e 6f77   the package now
+00008bc0: 2066 6169 6c73 2069 6620 7468 6520 6064   fails if the `d
+00008bd0: 6f63 6b65 722d 7079 6020 7061 636b 6167  ocker-py` packag
+00008be0: 6520 6973 0a20 2069 6e73 7461 6c6c 6564  e is.  installed
+00008bf0: 2069 6e20 6f72 6465 7220 746f 2070 7265   in order to pre
+00008c00: 7665 6e74 206f 6273 6375 7265 206e 616d  vent obscure nam
+00008c10: 696e 6720 636f 6e66 6c69 6374 7320 7768  ing conflicts wh
+00008c20: 656e 2062 6f74 680a 2020 7061 636b 6167  en both.  packag
+00008c30: 6573 2063 6f2d 6578 6973 742e 0a2a 2041  es co-exist..* A
+00008c40: 6464 6564 206d 6973 7369 6e67 2060 6669  dded missing `fi
+00008c50: 6c74 6572 7360 2070 6172 616d 6574 6572  lters` parameter
+00008c60: 2074 6f20 6041 5049 436c 6965 6e74 2e6e   to `APIClient.n
+00008c70: 6574 776f 726b 7360 2e0a 2a20 5265 736f  etworks`..* Reso
+00008c80: 7572 6365 206f 626a 6563 7473 2067 656e  urce objects gen
+00008c90: 6572 6174 6564 2062 7920 7468 6520 6044  erated by the `D
+00008ca0: 6f63 6b65 7243 6c69 656e 7460 2061 7265  ockerClient` are
+00008cb0: 206e 6f77 2068 6173 6861 626c 652e 0a2a   now hashable..*
+00008cc0: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+00008cd0: 7265 2072 6574 7269 6576 696e 6720 756e  re retrieving un
+00008ce0: 7461 6767 6564 2069 6d61 6765 7320 7573  tagged images us
+00008cf0: 696e 6720 6044 6f63 6b65 7243 6c69 656e  ing `DockerClien
+00008d00: 7460 0a20 2077 6f75 6c64 2072 6169 7365  t`.  would raise
+00008d10: 2061 2060 5479 7065 4572 726f 7260 2065   a `TypeError` e
+00008d20: 7863 6570 7469 6f6e 2e0a 2a20 606d 6f64  xception..* `mod
+00008d30: 6560 2070 6172 616d 6574 6572 2069 6e20  e` parameter in 
+00008d40: 6063 7265 6174 655f 7365 7276 6963 6560  `create_service`
+00008d50: 2069 7320 6e6f 7720 7072 6f70 6572 6c79   is now properly
+00008d60: 2063 6f6e 7665 7274 6564 2074 6f0a 2020   converted to.  
+00008d70: 6120 7661 6c69 6420 6461 7461 2074 7970  a valid data typ
+00008d80: 6520 666f 7220 7468 6520 456e 6769 6e65  e for the Engine
+00008d90: 2041 5049 2e20 5573 6520 6053 6572 7669   API. Use `Servi
+00008da0: 6365 4d6f 6465 6020 666f 7220 6164 7661  ceMode` for adva
+00008db0: 6e63 6564 0a20 2063 6f6e 6669 6775 7261  nced.  configura
+00008dc0: 7469 6f6e 732e 0a2a 2046 6978 6564 2061  tions..* Fixed a
+00008dd0: 2062 7567 2077 6865 7265 2074 6865 2064   bug where the d
+00008de0: 6563 6f64 6564 2060 4150 4943 6c69 656e  ecoded `APIClien
+00008df0: 742e 6576 656e 7473 6020 7374 7265 616d  t.events` stream
+00008e00: 2077 6f75 6c64 2073 6f6d 6574 696d 6573   would sometimes
+00008e10: 2072 6169 7365 0a20 2061 6e20 6578 6365   raise.  an exce
+00008e20: 7074 696f 6e20 7768 656e 2061 2063 6f6e  ption when a con
+00008e30: 7461 696e 6572 2069 7320 7374 6f70 7065  tainer is stoppe
+00008e40: 6420 6f72 2072 6573 7461 7274 6564 2e0a  d or restarted..
+00008e50: 0a32 2e30 2e31 0a2d 2d2d 2d2d 0a0a 5b4c  .2.0.1.-----..[L
+00008e60: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
+00008e70: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
+00008e80: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
+00008e90: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
+00008ea0: 646f 636b 6572 2d70 792f 6d69 6c65 7374  docker-py/milest
+00008eb0: 6f6e 652f 3238 3f63 6c6f 7365 643d 3129  one/28?closed=1)
+00008ec0: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
+00008ed0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+00008ee0: 6572 6520 666f 7277 6172 6420 736c 6173  ere forward slas
+00008ef0: 6865 7320 696e 2073 6f6d 6520 2e64 6f63  hes in some .doc
+00008f00: 6b65 7269 676e 6f72 6520 7061 7474 6572  kerignore patter
+00008f10: 6e73 2077 6572 656e 2774 0a20 2062 6569  ns weren't.  bei
+00008f20: 6e67 2070 6172 7365 6420 636f 7272 6563  ng parsed correc
+00008f30: 746c 7920 6f6e 2057 696e 646f 7773 0a2a  tly on Windows.*
+00008f40: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+00008f50: 7265 2060 4d6f 756e 742e 7061 7273 655f  re `Mount.parse_
+00008f60: 6d6f 756e 745f 7374 7269 6e67 6020 776f  mount_string` wo
+00008f70: 756c 6420 6e65 7665 7220 7365 7420 7468  uld never set th
+00008f80: 6520 7265 6164 5f6f 6e6c 790a 2020 7061  e read_only.  pa
+00008f90: 7261 6d65 7465 7220 6f6e 2074 6865 2072  rameter on the r
+00008fa0: 6573 756c 7469 6e67 2060 4d6f 756e 7460  esulting `Mount`
+00008fb0: 2e0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+00008fc0: 7768 6572 6520 604d 6f75 6e74 2e70 6172  where `Mount.par
+00008fd0: 7365 5f6d 6f75 6e74 5f73 7472 696e 6760  se_mount_string`
+00008fe0: 2077 6f75 6c64 2069 6e63 6f72 7265 6374   would incorrect
+00008ff0: 6c79 206d 6172 6b20 686f 7374 0a20 2062  ly mark host.  b
+00009000: 696e 6473 2061 7320 6265 696e 6720 6f66  inds as being of
+00009010: 2060 766f 6c75 6d65 6020 7479 7065 2e0a   `volume` type..
+00009020: 0a32 2e30 2e30 0a2d 2d2d 2d2d 0a0a 5b4c  .2.0.0.-----..[L
+00009030: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
+00009040: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
+00009050: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
+00009060: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
+00009070: 646f 636b 6572 2d70 792f 6d69 6c65 7374  docker-py/milest
+00009080: 6f6e 652f 3232 3f63 6c6f 7365 643d 3129  one/22?closed=1)
+00009090: 0a0a 2323 2320 4272 6561 6b69 6e67 2063  ..### Breaking c
+000090a0: 6861 6e67 6573 0a0a 2a20 4472 6f70 7065  hanges..* Droppe
+000090b0: 6420 7375 7070 6f72 7420 666f 7220 5079  d support for Py
+000090c0: 7468 6f6e 2032 2e36 0a2a 2060 646f 636b  thon 2.6.* `dock
+000090d0: 6572 2e43 6c69 656e 7460 2068 6173 2062  er.Client` has b
+000090e0: 6565 6e20 7265 6e61 6d65 6420 746f 2060  een renamed to `
+000090f0: 646f 636b 6572 2e41 5049 436c 6965 6e74  docker.APIClient
+00009100: 600a 2a20 6064 6f63 6b65 722e 6672 6f6d  `.* `docker.from
+00009110: 5f65 6e76 6020 6e6f 7720 6372 6561 7465  _env` now create
+00009120: 7320 6120 6044 6f63 6b65 7243 6c69 656e  s a `DockerClien
+00009130: 7460 2069 6e73 7461 6e63 6520 696e 7374  t` instance inst
+00009140: 6561 6420 6f66 2061 6e0a 2020 6041 5049  ead of an.  `API
+00009150: 436c 6965 6e74 6020 696e 7374 616e 6365  Client` instance
+00009160: 2e0a 2a20 5265 6d6f 7665 6420 486f 7374  ..* Removed Host
+00009170: 436f 6e66 6967 2070 6172 616d 6574 6572  Config parameter
+00009180: 7320 6672 6f6d 2060 4150 4943 6c69 656e  s from `APIClien
+00009190: 742e 7374 6172 7460 0a2a 2054 6865 206d  t.start`.* The m
+000091a0: 696e 696d 756d 2073 7570 706f 7274 6564  inimum supported
+000091b0: 2041 5049 2076 6572 7369 6f6e 2069 7320   API version is 
+000091c0: 6e6f 7720 312e 3231 2028 456e 6769 6e65  now 1.21 (Engine
+000091d0: 2076 6572 7369 6f6e 2031 2e39 2e30 2b29   version 1.9.0+)
+000091e0: 0a2a 2054 6865 206e 616d 6520 6f66 2074  .* The name of t
+000091f0: 6865 2060 7069 7060 2070 6163 6b61 6765  he `pip` package
+00009200: 2069 7320 6e6f 7720 6064 6f63 6b65 7260   is now `docker`
+00009210: 2028 7761 733a 2060 646f 636b 6572 2d70   (was: `docker-p
+00009220: 7960 292e 204e 6577 0a20 2076 6572 7369  y`). New.  versi
+00009230: 6f6e 7320 6f66 2074 6869 7320 6c69 6272  ons of this libr
+00009240: 6172 7920 7769 6c6c 206f 6e6c 7920 6265  ary will only be
+00009250: 2070 7562 6c69 7368 6564 2061 7320 6064   published as `d
+00009260: 6f63 6b65 7260 2066 726f 6d20 6e6f 7720  ocker` from now 
+00009270: 6f6e 2e0a 2a20 6064 6f63 6b65 722e 7373  on..* `docker.ss
+00009280: 6c61 6461 7074 6572 6020 6973 206e 6f77  ladapter` is now
+00009290: 2060 646f 636b 6572 2e74 7261 6e73 706f   `docker.transpo
+000092a0: 7274 2e73 736c 6164 6170 7465 7260 0a2a  rt.ssladapter`.*
+000092b0: 2054 6865 2070 6163 6b61 6765 2073 7472   The package str
+000092c0: 7563 7475 7265 2068 6173 2062 6565 6e20  ucture has been 
+000092d0: 666c 6174 7465 6e65 6420 696e 2063 6572  flattened in cer
+000092e0: 7461 696e 2063 6173 6573 2c20 7768 6963  tain cases, whic
+000092f0: 6820 6d61 7920 6166 6665 6374 0a20 2069  h may affect.  i
+00009300: 6d70 6f72 7420 666f 7220 6064 6f63 6b65  mport for `docke
+00009310: 722e 6175 7468 6020 616e 6420 6064 6f63  r.auth` and `doc
+00009320: 6b65 722e 7574 696c 732e 706f 7274 7360  ker.utils.ports`
+00009330: 0a2a 2060 646f 636b 6572 2e75 7469 6c73  .* `docker.utils
+00009340: 2e74 7970 6573 6020 6861 7320 6265 656e  .types` has been
+00009350: 206d 6f76 6564 2074 6f20 6064 6f63 6b65   moved to `docke
+00009360: 722e 7479 7065 7360 0a2a 2060 6372 6561  r.types`.* `crea
+00009370: 7465 5f68 6f73 745f 636f 6e66 6967 602c  te_host_config`,
+00009380: 2060 6372 6561 7465 5f69 7061 6d5f 706f   `create_ipam_po
+00009390: 6f6c 6020 616e 6420 6063 7265 6174 655f  ol` and `create_
+000093a0: 6970 616d 5f63 6f6e 6669 6760 2068 6176  ipam_config` hav
+000093b0: 6520 6265 656e 0a20 2072 656d 6f76 6564  e been.  removed
+000093c0: 2066 726f 6d20 6064 6f63 6b65 722e 7574   from `docker.ut
+000093d0: 696c 7360 2e20 5468 6579 2068 6176 6520  ils`. They have 
+000093e0: 6265 656e 2072 6570 6c61 6365 6420 6279  been replaced by
+000093f0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00009400: 6c61 7373 6573 0a20 2069 6e20 6064 6f63  lasses.  in `doc
+00009410: 6b65 722e 7479 7065 7360 3a20 6048 6f73  ker.types`: `Hos
+00009420: 7443 6f6e 6669 6760 2c20 6049 5041 4d50  tConfig`, `IPAMP
+00009430: 6f6f 6c60 2061 6e64 2060 4950 414d 434f  ool` and `IPAMCO
+00009440: 6e66 6967 602e 0a0a 2323 2320 4665 6174  nfig`...### Feat
+00009450: 7572 6573 0a0a 2a20 4164 6465 6420 6120  ures..* Added a 
+00009460: 6869 6768 2d6c 6576 656c 2c20 7573 6572  high-level, user
+00009470: 2d66 6f63 7573 6564 2041 5049 2061 7320  -focused API as 
+00009480: 6064 6f63 6b65 722e 446f 636b 6572 436c  `docker.DockerCl
+00009490: 6965 6e74 602e 2053 6565 2074 6865 0a20  ient`. See the. 
+000094a0: 2052 4541 444d 4520 616e 6420 646f 6375   README and docu
+000094b0: 6d65 6e74 6174 696f 6e20 666f 7220 6d6f  mentation for mo
+000094c0: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0a  re information..
+000094d0: 2a20 496d 706c 656d 656e 7465 6420 6075  * Implemented `u
+000094e0: 7064 6174 655f 6e6f 6465 6020 6d65 7468  pdate_node` meth
+000094f0: 6f64 2069 6e20 6041 5049 436c 6965 6e74  od in `APIClient
+00009500: 602e 0a2a 2049 6d70 6c65 6d65 6e74 6564  `..* Implemented
+00009510: 2060 7265 6d6f 7665 5f6e 6f64 6560 206d   `remove_node` m
+00009520: 6574 686f 6420 696e 2060 4150 4943 6c69  ethod in `APICli
+00009530: 656e 7460 2e0a 2a20 4164 6465 6420 7375  ent`..* Added su
+00009540: 7070 6f72 7420 666f 7220 6072 6573 7461  pport for `resta
+00009550: 7274 5f70 6f6c 6963 7960 2069 6e20 6075  rt_policy` in `u
+00009560: 7064 6174 655f 636f 6e74 6169 6e65 7260  pdate_container`
+00009570: 2e0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
+00009580: 7420 666f 7220 606c 6162 656c 7360 2061  t for `labels` a
+00009590: 6e64 2060 7368 6d73 697a 6560 2069 6e20  nd `shmsize` in 
+000095a0: 6062 7569 6c64 602e 0a2a 2041 6464 6564  `build`..* Added
+000095b0: 2073 7570 706f 7274 2066 6f72 2060 6174   support for `at
+000095c0: 7461 6368 6162 6c65 6020 696e 2060 6372  tachable` in `cr
+000095d0: 6561 7465 5f6e 6574 776f 726b 600a 2a20  eate_network`.* 
+000095e0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+000095f0: 7220 6068 6561 6c74 6863 6865 636b 6020  r `healthcheck` 
+00009600: 696e 2060 6372 6561 7465 5f63 6f6e 7461  in `create_conta
+00009610: 696e 6572 602e 0a2a 2041 6464 6564 2073  iner`..* Added s
+00009620: 7570 706f 7274 2066 6f72 2060 6973 6f6c  upport for `isol
+00009630: 6174 696f 6e60 2069 6e20 6048 6f73 7443  ation` in `HostC
+00009640: 6f6e 6669 6760 2e0a 2a20 4578 7061 6e64  onfig`..* Expand
+00009650: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
+00009660: 7069 645f 6d6f 6465 6020 696e 2060 486f  pid_mode` in `Ho
+00009670: 7374 436f 6e66 6967 6020 286e 6f77 2073  stConfig` (now s
+00009680: 7570 706f 7274 7320 6172 6269 7472 6172  upports arbitrar
+00009690: 790a 2020 7661 6c75 6573 2066 6f72 2041  y.  values for A
+000096a0: 5049 2076 6572 7369 6f6e 203e 3d20 312e  PI version >= 1.
+000096b0: 3234 292e 0a2a 2041 6464 6564 2073 7570  24)..* Added sup
+000096c0: 706f 7274 2066 6f72 2060 6f70 7469 6f6e  port for `option
+000096d0: 7360 2069 6e20 6049 5041 4d43 6f6e 6669  s` in `IPAMConfi
+000096e0: 6760 0a2a 2041 6464 6564 2061 2060 4865  g`.* Added a `He
+000096f0: 616c 7468 4368 6563 6b60 2063 6c61 7373  althCheck` class
+00009700: 2074 6f20 6064 6f63 6b65 722e 7479 7065   to `docker.type
+00009710: 7360 2074 6f20 6265 2075 7365 6420 696e  s` to be used in
+00009720: 0a20 2060 6372 6561 7465 5f63 6f6e 7461  .  `create_conta
+00009730: 696e 6572 602e 0a2a 2041 6464 6564 2061  iner`..* Added a
+00009740: 6e20 6045 6e64 706f 696e 7453 7065 6360  n `EndpointSpec`
+00009750: 2063 6c61 7373 2074 6f20 6064 6f63 6b65   class to `docke
+00009760: 722e 7479 7065 7360 2074 6f20 6265 2075  r.types` to be u
+00009770: 7365 6420 696e 0a20 2060 6372 6561 7465  sed in.  `create
+00009780: 5f73 6572 7669 6365 6020 616e 6420 6075  _service` and `u
+00009790: 7064 6174 655f 7365 7276 6963 6560 2e0a  pdate_service`..
+000097a0: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
+000097b0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+000097c0: 6572 6520 6175 7468 2069 6e66 6f72 6d61  ere auth informa
+000097d0: 7469 6f6e 2077 6f75 6c64 206e 6f74 2062  tion would not b
+000097e0: 6520 7072 6f70 6572 6c79 2070 6173 7365  e properly passe
+000097f0: 6420 746f 2074 6865 2065 6e67 696e 650a  d to the engine.
+00009800: 2020 6475 7269 6e67 2061 2060 6275 696c    during a `buil
+00009810: 6460 2069 6620 7468 6520 636c 6965 6e74  d` if the client
+00009820: 2075 7365 6420 6120 6372 6564 656e 7469   used a credenti
+00009830: 616c 7320 7374 6f72 652e 0a2a 2046 6978  als store..* Fix
+00009840: 6564 2061 6e20 6973 7375 6520 7769 7468  ed an issue with
+00009850: 2073 6f6d 6520 6578 636c 7573 696f 6e20   some exclusion 
+00009860: 7061 7474 6572 6e73 2069 6e20 6062 7569  patterns in `bui
+00009870: 6c64 602e 0a2a 2046 6978 6564 2061 6e20  ld`..* Fixed an 
+00009880: 6973 7375 6520 7768 6572 6520 636f 6e74  issue where cont
+00009890: 6578 7420 6669 6c65 7320 7765 7265 2062  ext files were b
+000098a0: 756e 646c 6564 2077 6974 6820 7468 6520  undled with the 
+000098b0: 7772 6f6e 6720 7065 726d 6973 7369 6f6e  wrong permission
+000098c0: 730a 2020 7768 656e 2063 616c 6c69 6e67  s.  when calling
+000098d0: 2060 6275 696c 6460 206f 6e20 5769 6e64   `build` on Wind
+000098e0: 6f77 732e 0a2a 2046 6978 6564 2061 6e20  ows..* Fixed an 
+000098f0: 6973 7375 6520 7768 6572 6520 6175 7468  issue where auth
+00009900: 2069 6e66 6f20 776f 756c 6420 6e6f 7420   info would not 
+00009910: 6265 2072 6574 7269 6576 6564 2066 726f  be retrieved fro
+00009920: 6d20 6974 7320 6465 6661 756c 7420 6c6f  m its default lo
+00009930: 6361 7469 6f6e 0a20 206f 6e20 5769 6e64  cation.  on Wind
+00009940: 6f77 732e 0a2a 2046 6978 6564 2061 6e20  ows..* Fixed an 
+00009950: 6973 7375 6520 7768 6572 6520 6c69 7374  issue where list
+00009960: 7320 6f66 2060 6e65 7477 6f72 6b73 6020  s of `networks` 
+00009970: 696e 2060 6372 6561 7465 5f73 6572 7669  in `create_servi
+00009980: 6365 6020 616e 640a 2020 6075 7064 6174  ce` and.  `updat
+00009990: 655f 7365 7276 6963 6560 2077 6f75 6c64  e_service` would
+000099a0: 6e27 7420 6265 2070 726f 7065 726c 7920  n't be properly 
+000099b0: 636f 6e76 6572 7465 6420 666f 7220 7468  converted for th
+000099c0: 6520 656e 6769 6e65 2e0a 2a20 4669 7865  e engine..* Fixe
+000099d0: 6420 616e 2069 7373 7565 2077 6865 7265  d an issue where
+000099e0: 2060 656e 6470 6f69 6e74 5f63 6f6e 6669   `endpoint_confi
+000099f0: 6760 2069 6e20 6063 7265 6174 655f 7365  g` in `create_se
+00009a00: 7276 6963 6560 2061 6e64 0a20 2060 7570  rvice` and.  `up
+00009a10: 6461 7465 5f73 6572 7669 6365 6020 776f  date_service` wo
+00009a20: 756c 6420 6265 2069 676e 6f72 6564 2e0a  uld be ignored..
+00009a30: 2a20 6065 6e64 706f 696e 745f 636f 6e66  * `endpoint_conf
+00009a40: 6967 6020 696e 2060 6372 6561 7465 5f73  ig` in `create_s
+00009a50: 6572 7669 6365 6020 616e 6420 6075 7064  ervice` and `upd
+00009a60: 6174 655f 7365 7276 6963 6560 2068 6173  ate_service` has
+00009a70: 2062 6565 6e0a 2020 6465 7072 6563 6174   been.  deprecat
+00009a80: 6564 2069 6e20 6661 766f 7220 6f66 2060  ed in favor of `
+00009a90: 656e 6470 6f69 6e74 5f73 7065 6360 0a2a  endpoint_spec`.*
+00009aa0: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+00009ab0: 7265 2060 636f 6e73 7472 6169 6e74 7360  re `constraints`
+00009ac0: 2069 6e20 6120 6054 6173 6b54 656d 706c   in a `TaskTempl
+00009ad0: 6174 6560 206f 626a 6563 7420 776f 756c  ate` object woul
+00009ae0: 646e 2774 2062 650a 2020 7072 6f70 6572  dn't be.  proper
+00009af0: 6c79 2063 6f6e 7665 7274 6564 2066 6f72  ly converted for
+00009b00: 2074 6865 2065 6e67 696e 652e 0a2a 2046   the engine..* F
+00009b10: 6978 6564 2061 6e20 6973 7375 6520 7768  ixed an issue wh
+00009b20: 6572 6520 7072 6f76 6964 696e 6720 6120  ere providing a 
+00009b30: 6469 6374 696f 6e61 7279 2066 6f72 2060  dictionary for `
+00009b40: 656e 7660 2069 6e20 6043 6f6e 7461 696e  env` in `Contain
+00009b50: 6572 5370 6563 600a 2020 776f 756c 6420  erSpec`.  would 
+00009b60: 7072 6f76 6f6b 6520 616e 2060 4150 4945  provoke an `APIE
+00009b70: 7272 6f72 6020 7768 656e 2073 656e 7420  rror` when sent 
+00009b80: 746f 2074 6865 2065 6e67 696e 652e 0a2a  to the engine..*
+00009b90: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+00009ba0: 7265 2070 726f 7669 6469 6e67 2061 6e20  re providing an 
+00009bb0: 6065 6e76 5f66 696c 6560 2063 6f6e 7461  `env_file` conta
+00009bc0: 696e 696e 6720 656d 7074 7920 6c69 6e65  ining empty line
+00009bd0: 7320 696e 0a20 2060 6372 6561 7465 5f63  s in.  `create_c
+00009be0: 6f6e 7461 696e 6572 6077 6f75 6c64 2072  ontainer`would r
+00009bf0: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
+00009c00: 6e2e 0a2a 2046 6978 6564 2061 2062 7567  n..* Fixed a bug
+00009c10: 2077 6865 7265 2060 6465 7461 6368 6020   where `detach` 
+00009c20: 7761 7320 6265 696e 6720 6967 6e6f 7265  was being ignore
+00009c30: 6420 6279 2060 6578 6563 5f73 7461 7274  d by `exec_start
+00009c40: 602e 0a0a 2323 2320 446f 6375 6d65 6e74  `...### Document
+00009c50: 6174 696f 6e0a 0a2a 2044 6f63 756d 656e  ation..* Documen
+00009c60: 7461 7469 6f6e 2066 6f72 2063 6c61 7373  tation for class
+00009c70: 6573 2061 6e64 206d 6574 686f 6473 2069  es and methods i
+00009c80: 7320 6e6f 7720 696e 636c 7564 6564 2061  s now included a
+00009c90: 6c6f 6e67 7369 6465 2074 6865 2063 6f64  longside the cod
+00009ca0: 6520 6173 0a20 2064 6f63 7374 7269 6e67  e as.  docstring
+00009cb0: 732e 0a0a 312e 3130 2e36 0a2d 2d2d 2d2d  s...1.10.6.-----
+00009cc0: 2d0a 0a5b 4c69 7374 206f 6620 5052 7320  -..[List of PRs 
+00009cd0: 2f20 6973 7375 6573 2066 6f72 2074 6869  / issues for thi
+00009ce0: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
+00009cf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
+00009d00: 636b 6572 2f64 6f63 6b65 722d 7079 2f6d  cker/docker-py/m
+00009d10: 696c 6573 746f 6e65 2f32 363f 636c 6f73  ilestone/26?clos
+00009d20: 6564 3d31 290a 0a23 2323 2042 7567 6669  ed=1)..### Bugfi
+00009d30: 7865 730a 0a2a 2046 6978 6564 2061 6e20  xes..* Fixed an 
+00009d40: 6973 7375 6520 7768 6572 6520 7365 7474  issue where sett
+00009d50: 696e 6720 6120 604e 7069 7065 536f 636b  ing a `NpipeSock
+00009d60: 6574 6020 696e 7374 616e 6365 2074 6f20  et` instance to 
+00009d70: 626c 6f63 6b69 6e67 206d 6f64 6520 776f  blocking mode wo
+00009d80: 756c 640a 2020 7075 7420 6974 2069 6e20  uld.  put it in 
+00009d90: 6e6f 6e2d 626c 6f63 6b69 6e67 206d 6f64  non-blocking mod
+00009da0: 6520 616e 6420 7669 6365 2d76 6572 7361  e and vice-versa
+00009db0: 2e0a 0a0a 312e 3130 2e35 0a2d 2d2d 2d2d  ....1.10.5.-----
+00009dc0: 2d0a 0a5b 4c69 7374 206f 6620 5052 7320  -..[List of PRs 
+00009dd0: 2f20 6973 7375 6573 2066 6f72 2074 6869  / issues for thi
+00009de0: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
+00009df0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
+00009e00: 636b 6572 2f64 6f63 6b65 722d 7079 2f6d  cker/docker-py/m
+00009e10: 696c 6573 746f 6e65 2f32 353f 636c 6f73  ilestone/25?clos
+00009e20: 6564 3d31 290a 0a23 2323 2042 7567 6669  ed=1)..### Bugfi
+00009e30: 7865 730a 0a2a 2046 6978 6564 2061 6e20  xes..* Fixed an 
+00009e40: 6973 7375 6520 7768 6572 6520 636f 6e63  issue where conc
+00009e50: 7572 7265 6e74 2061 7474 656d 7074 7320  urrent attempts 
+00009e60: 746f 2061 6363 6573 7320 746f 2061 206e  to access to a n
+00009e70: 616d 6564 2070 6970 6520 6279 2074 6865  amed pipe by the
+00009e80: 0a20 2063 6c69 656e 7420 776f 756c 6420  .  client would 
+00009e90: 736f 6d65 7469 6d65 7320 6361 7573 6520  sometimes cause 
+00009ea0: 7265 636f 7665 7261 626c 6520 6578 6365  recoverable exce
+00009eb0: 7074 696f 6e73 2074 6f20 6265 2072 6169  ptions to be rai
+00009ec0: 7365 642e 0a0a 0a31 2e31 302e 340a 2d2d  sed....1.10.4.--
+00009ed0: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
+00009ee0: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
+00009ef0: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+00009f00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00009f10: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
+00009f20: 792f 6d69 6c65 7374 6f6e 652f 3234 3f63  y/milestone/24?c
+00009f30: 6c6f 7365 643d 3129 0a0a 2323 2320 4275  losed=1)..### Bu
+00009f40: 6766 6978 6573 0a0a 2a20 4669 7865 6420  gfixes..* Fixed 
+00009f50: 616e 2069 7373 7565 2077 6865 7265 2060  an issue where `
+00009f60: 5265 7374 6172 7450 6f6c 6963 792e 636f  RestartPolicy.co
+00009f70: 6e64 6974 696f 6e5f 7479 7065 732e 4f4e  ndition_types.ON
+00009f80: 5f46 4149 4c55 5245 6020 776f 756c 6420  _FAILURE` would 
+00009f90: 7969 656c 640a 2020 616e 2069 6e76 616c  yield.  an inval
+00009fa0: 6964 2076 616c 7565 2e0a 2a20 4669 7865  id value..* Fixe
+00009fb0: 6420 616e 2069 7373 7565 2077 6865 7265  d an issue where
+00009fc0: 2074 6865 2053 534c 2063 6f6e 6e65 6374   the SSL connect
+00009fd0: 696f 6e20 6164 6170 7465 7220 776f 756c  ion adapter woul
+00009fe0: 6420 7265 6365 6976 6520 616e 2069 6e76  d receive an inv
+00009ff0: 616c 6964 0a20 2061 7267 756d 656e 742e  alid.  argument.
+0000a000: 0a2a 2046 6978 6564 2061 6e20 6973 7375  .* Fixed an issu
+0000a010: 6520 7468 6174 2063 6175 7365 6420 7468  e that caused th
+0000a020: 6520 436c 6965 6e74 2074 6f20 6661 696c  e Client to fail
+0000a030: 2074 6f20 7265 6163 6820 4150 4920 656e   to reach API en
+0000a040: 6470 6f69 6e74 7320 7768 656e 0a20 2074  dpoints when.  t
+0000a050: 6865 2070 726f 7669 6465 6420 6062 6173  he provided `bas
+0000a060: 655f 7572 6c60 2068 6164 2061 2074 7261  e_url` had a tra
+0000a070: 696c 696e 6720 736c 6173 682e 0a2a 2046  iling slash..* F
+0000a080: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+0000a090: 2073 6f6d 6520 6065 6e76 6972 6f6e 6d65   some `environme
+0000a0a0: 6e74 6020 7661 6c75 6573 2069 6e20 6063  nt` values in `c
+0000a0b0: 7265 6174 655f 636f 6e74 6169 6e65 7260  reate_container`
+0000a0c0: 0a20 2063 6f6e 7461 696e 696e 6720 756e  .  containing un
+0000a0d0: 6963 6f64 6520 6368 6172 6163 7465 7273  icode characters
+0000a0e0: 2077 6f75 6c64 2072 6169 7365 2061 6e20   would raise an 
+0000a0f0: 656e 636f 6469 6e67 2065 7272 6f72 2e0a  encoding error..
+0000a100: 2a20 4669 7865 6420 6120 6e75 6d62 6572  * Fixed a number
+0000a110: 206f 6620 6973 7375 6573 2074 6965 6420   of issues tied 
+0000a120: 7769 7468 206e 616d 6564 2070 6970 6520  with named pipe 
+0000a130: 7472 616e 7370 6f72 7420 6f6e 2057 696e  transport on Win
+0000a140: 646f 7773 2e0a 2a20 4669 7865 6420 6120  dows..* Fixed a 
+0000a150: 6275 6720 7768 6572 6520 696e 636c 7573  bug where inclus
+0000a160: 696f 6e20 7061 7474 6572 6e73 2069 6e20  ion patterns in 
+0000a170: 602e 646f 636b 6572 6967 6e6f 7265 6020  `.dockerignore` 
+0000a180: 776f 756c 6420 6361 7573 6520 736f 6d65  would cause some
+0000a190: 0a20 2065 7863 6c75 6465 6420 6669 6c65  .  excluded file
+0000a1a0: 7320 746f 2061 7070 6561 7220 696e 2074  s to appear in t
+0000a1b0: 6865 2062 7569 6c64 2063 6f6e 7465 7874  he build context
+0000a1c0: 206f 6e20 5769 6e64 6f77 732e 0a0a 2323   on Windows...##
+0000a1d0: 2320 4d69 7363 656c 6c61 6e65 6f75 730a  # Miscellaneous.
+0000a1e0: 0a2a 2041 646a 7573 7465 6420 7665 7273  .* Adjusted vers
+0000a1f0: 696f 6e20 7265 7175 6972 656d 656e 7473  ion requirements
+0000a200: 2066 6f72 2074 6865 2060 7265 7175 6573   for the `reques
+0000a210: 7473 6020 6c69 6272 6172 792e 0a2a 2049  ts` library..* I
+0000a220: 7420 6973 206e 6f77 2070 6f73 7369 626c  t is now possibl
+0000a230: 6520 746f 2072 756e 2074 6865 2064 6f63  e to run the doc
+0000a240: 6b65 722d 7079 2074 6573 7420 7375 6974  ker-py test suit
+0000a250: 6520 6f6e 2057 696e 646f 7773 2e0a 0a0a  e on Windows....
+0000a260: 312e 3130 2e33 0a2d 2d2d 2d2d 2d0a 0a5b  1.10.3.------..[
+0000a270: 4c69 7374 206f 6620 5052 7320 2f20 6973  List of PRs / is
+0000a280: 7375 6573 2066 6f72 2074 6869 7320 7265  sues for this re
+0000a290: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
+0000a2a0: 6974 6875 622e 636f 6d2f 646f 636b 6572  ithub.com/docker
+0000a2b0: 2f64 6f63 6b65 722d 7079 2f69 7373 7565  /docker-py/issue
+0000a2c0: 733f 713d 6d69 6c65 7374 6f6e 6525 3341  s?q=milestone%3A
+0000a2d0: 312e 3130 2e33 2b69 7325 3341 636c 6f73  1.10.3+is%3Aclos
+0000a2e0: 6564 290a 0a23 2323 2042 7567 6669 7865  ed)..### Bugfixe
+0000a2f0: 730a 0a2a 2046 6978 6564 2061 6e20 6973  s..* Fixed an is
+0000a300: 7375 6520 7768 6572 6520 6964 656e 7469  sue where identi
+0000a310: 7479 2074 6f6b 656e 7320 696e 2063 6f6e  ty tokens in con
+0000a320: 6669 6775 7261 7469 6f6e 2066 696c 6573  figuration files
+0000a330: 2077 6572 656e 2774 2068 616e 646c 6564   weren't handled
+0000a340: 0a20 2062 7920 7468 6520 6c69 6272 6172  .  by the librar
+0000a350: 792e 0a0a 2323 2320 4d69 7363 656c 6c61  y...### Miscella
+0000a360: 6e65 6f75 730a 0a2a 2049 6e63 7265 6173  neous..* Increas
+0000a370: 6564 2074 6865 2064 6566 6175 6c74 206e  ed the default n
+0000a380: 756d 6265 7220 6f66 2063 6f6e 6e65 6374  umber of connect
+0000a390: 696f 6e20 706f 6f6c 7320 6672 6f6d 2031  ion pools from 1
+0000a3a0: 3020 746f 2032 352e 2054 6869 7320 6e75  0 to 25. This nu
+0000a3b0: 6d62 6572 0a20 2063 616e 206e 6f77 2062  mber.  can now b
+0000a3c0: 6520 636f 6e66 6967 7572 6564 2075 7369  e configured usi
+0000a3d0: 6e67 2074 6865 2060 6e75 6d5f 706f 6f6c  ng the `num_pool
+0000a3e0: 7360 2070 6172 616d 6574 6572 2069 6e20  s` parameter in 
+0000a3f0: 7468 6520 6043 6c69 656e 7460 0a20 2063  the `Client`.  c
+0000a400: 6f6e 7374 7275 6374 6f72 2e0a 0a0a 312e  onstructor....1.
+0000a410: 3130 2e32 0a2d 2d2d 2d2d 2d0a 0a5b 4c69  10.2.------..[Li
+0000a420: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+0000a430: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+0000a440: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+0000a450: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+0000a460: 6f63 6b65 722d 7079 2f69 7373 7565 733f  ocker-py/issues?
+0000a470: 713d 6d69 6c65 7374 6f6e 6525 3341 312e  q=milestone%3A1.
+0000a480: 3130 2e30 2b69 7325 3341 636c 6f73 6564  10.0+is%3Aclosed
+0000a490: 290a 0a23 2323 2042 7567 6669 7865 730a  )..### Bugfixes.
+0000a4a0: 0a2a 2055 7064 6174 6564 2074 6865 2064  .* Updated the d
+0000a4b0: 6f63 6b65 722d 7079 6372 6564 7320 6465  ocker-pycreds de
+0000a4c0: 7065 6e64 656e 6379 2061 7320 6974 2077  pendency as it w
+0000a4d0: 6173 2063 6175 7369 6e67 2069 7373 7565  as causing issue
+0000a4e0: 7320 666f 7220 736f 6d65 0a20 2075 7365  s for some.  use
+0000a4f0: 7273 2077 6974 6820 6465 7065 6e64 656e  rs with dependen
+0000a500: 6379 2072 6573 6f6c 7574 696f 6e20 696e  cy resolution in
+0000a510: 2061 7070 6c69 6361 7469 6f6e 7320 7573   applications us
+0000a520: 696e 6720 646f 636b 6572 2d70 792e 0a0a  ing docker-py...
+0000a530: 0a31 2e31 302e 310a 2d2d 2d2d 2d2d 0a0a  .1.10.1.------..
+0000a540: 5b4c 6973 7420 6f66 2050 5273 202f 2069  [List of PRs / i
+0000a550: 7373 7565 7320 666f 7220 7468 6973 2072  ssues for this r
+0000a560: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+0000a570: 6769 7468 7562 2e63 6f6d 2f64 6f63 6b65  github.com/docke
+0000a580: 722f 646f 636b 6572 2d70 792f 6973 7375  r/docker-py/issu
+0000a590: 6573 3f71 3d6d 696c 6573 746f 6e65 2533  es?q=milestone%3
+0000a5a0: 4131 2e31 302e 302b 6973 2533 4163 6c6f  A1.10.0+is%3Aclo
+0000a5b0: 7365 6429 0a0a 2323 2320 4275 6766 6978  sed)..### Bugfix
+0000a5c0: 6573 0a0a 2a20 5468 6520 646f 636b 6572  es..* The docker
+0000a5d0: 2e75 7469 6c73 2e74 7970 6573 206d 6f64  .utils.types mod
+0000a5e0: 756c 6520 7761 7320 7265 6d6f 7665 6420  ule was removed 
+0000a5f0: 696e 2066 6176 6f72 206f 6620 646f 636b  in favor of dock
+0000a600: 6572 2e74 7970 6573 2c20 6275 7420 736f  er.types, but so
+0000a610: 6d65 0a20 2061 7070 6c69 6361 7469 6f6e  me.  application
+0000a620: 7320 696d 706f 7274 6564 2069 7420 6578  s imported it ex
+0000a630: 706c 6963 6974 6c79 2e20 4974 2068 6173  plicitly. It has
+0000a640: 2062 6565 6e20 7265 2d61 6464 6564 2077   been re-added w
+0000a650: 6974 6820 616e 2069 6d70 6f72 740a 2020  ith an import.  
+0000a660: 7761 726e 696e 6720 6164 7669 7369 6e67  warning advising
+0000a670: 2074 6f20 7573 6520 7468 6520 6e65 7720   to use the new 
+0000a680: 6d6f 6475 6c65 2070 6174 682e 0a0a 312e  module path...1.
+0000a690: 3130 2e30 0a2d 2d2d 2d2d 2d0a 0a5b 4c69  10.0.------..[Li
+0000a6a0: 7374 206f 6620 5052 7320 2f20 6973 7375  st of PRs / issu
+0000a6b0: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
+0000a6c0: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+0000a6d0: 6875 622e 636f 6d2f 646f 636b 6572 2f64  hub.com/docker/d
+0000a6e0: 6f63 6b65 722d 7079 2f69 7373 7565 733f  ocker-py/issues?
+0000a6f0: 713d 6d69 6c65 7374 6f6e 6525 3341 312e  q=milestone%3A1.
+0000a700: 3130 2e30 2b69 7325 3341 636c 6f73 6564  10.0+is%3Aclosed
+0000a710: 290a 0a23 2323 2046 6561 7475 7265 730a  )..### Features.
+0000a720: 0a2a 2041 6464 6564 2073 7761 726d 206d  .* Added swarm m
+0000a730: 6f64 6520 616e 6420 7365 7276 6963 6520  ode and service 
+0000a740: 6d61 6e61 6765 6d65 6e74 206d 6574 686f  management metho
+0000a750: 6473 2e20 5365 6520 7468 6520 646f 6375  ds. See the docu
+0000a760: 6d65 6e74 6174 696f 6e20 666f 720a 2020  mentation for.  
+0000a770: 6465 7461 696c 732e 0a2a 2041 6464 6564  details..* Added
+0000a780: 2073 7570 706f 7274 2066 6f72 2049 5076   support for IPv
+0000a790: 3620 446f 636b 6572 2068 6f73 7420 6164  6 Docker host ad
+0000a7a0: 6472 6573 7365 7320 696e 2074 6865 2060  dresses in the `
+0000a7b0: 436c 6965 6e74 6020 636f 6e73 7472 7563  Client` construc
+0000a7c0: 746f 722e 0a2a 2041 6464 6564 2028 7265  tor..* Added (re
+0000a7d0: 6164 2d6f 6e6c 7929 2073 7570 706f 7274  ad-only) support
+0000a7e0: 2066 6f72 2074 6865 2044 6f63 6b65 7220   for the Docker 
+0000a7f0: 6372 6564 656e 7469 616c 7320 7374 6f72  credentials stor
+0000a800: 652e 0a2a 2041 6464 6564 2073 7570 706f  e..* Added suppo
+0000a810: 7274 2066 6f72 2063 7573 746f 6d20 6061  rt for custom `a
+0000a820: 7574 685f 636f 6e66 6967 6020 696e 2060  uth_config` in `
+0000a830: 436c 6965 6e74 2e70 7573 6860 2e0a 2a20  Client.push`..* 
+0000a840: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+0000a850: 7220 606c 6162 656c 7360 2069 6e20 6043  r `labels` in `C
+0000a860: 6c69 656e 742e 6372 6561 7465 5f76 6f6c  lient.create_vol
+0000a870: 756d 6560 2e0a 2a20 4164 6465 6420 7375  ume`..* Added su
+0000a880: 7070 6f72 7420 666f 7220 606c 6162 656c  pport for `label
+0000a890: 7360 2061 6e64 2060 656e 6162 6c65 5f69  s` and `enable_i
+0000a8a0: 7076 3660 2069 6e20 6043 6c69 656e 742e  pv6` in `Client.
+0000a8b0: 6372 6561 7465 5f6e 6574 776f 726b 602e  create_network`.
+0000a8c0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+0000a8d0: 2066 6f72 2060 666f 7263 6560 2070 6172   for `force` par
+0000a8e0: 616d 2069 6e0a 2020 6043 6c69 656e 742e  am in.  `Client.
+0000a8f0: 6469 7363 6f6e 6e65 6374 5f63 6f6e 7461  disconnect_conta
+0000a900: 696e 6572 5f66 726f 6d5f 6e65 7477 6f72  iner_from_networ
+0000a910: 6b60 2e0a 2a20 4164 6465 6420 7375 7070  k`..* Added supp
+0000a920: 6f72 7420 666f 7220 6070 6964 735f 6c69  ort for `pids_li
+0000a930: 6d69 7460 2c20 6073 7973 6374 6c73 602c  mit`, `sysctls`,
+0000a940: 2060 7573 6572 6e73 5f6d 6f64 6560 2c20   `userns_mode`, 
+0000a950: 6063 7075 7365 745f 6370 7573 602c 0a20  `cpuset_cpus`,. 
+0000a960: 2060 6370 755f 7368 6172 6573 602c 2060   `cpu_shares`, `
+0000a970: 6d65 6d5f 7265 7365 7276 6174 696f 6e60  mem_reservation`
+0000a980: 2061 6e64 2060 6b65 726e 656c 5f6d 656d   and `kernel_mem
+0000a990: 6f72 7960 2070 6172 616d 6574 6572 7320  ory` parameters 
+0000a9a0: 696e 0a20 2060 436c 6965 6e74 2e63 7265  in.  `Client.cre
+0000a9b0: 6174 655f 686f 7374 5f63 6f6e 6669 6760  ate_host_config`
+0000a9c0: 2e0a 2a20 4164 6465 6420 7375 7070 6f72  ..* Added suppor
+0000a9d0: 7420 666f 7220 606c 696e 6b5f 6c6f 6361  t for `link_loca
+0000a9e0: 6c5f 6970 7360 2069 6e20 6063 7265 6174  l_ips` in `creat
+0000a9f0: 655f 656e 6470 6f69 6e74 5f63 6f6e 6669  e_endpoint_confi
+0000aa00: 6760 2e0a 2a20 4164 6465 6420 7375 7070  g`..* Added supp
+0000aa10: 6f72 7420 666f 7220 6120 6063 6861 6e67  ort for a `chang
+0000aa20: 6573 6020 7061 7261 6d65 7465 7220 696e  es` parameter in
+0000aa30: 2060 436c 6965 6e74 2e69 6d70 6f72 745f   `Client.import_
+0000aa40: 696d 6167 6560 2e0a 2a20 4164 6465 6420  image`..* Added 
+0000aa50: 7375 7070 6f72 7420 666f 7220 6120 6076  support for a `v
+0000aa60: 6572 7369 6f6e 6020 7061 7261 6d65 7465  ersion` paramete
+0000aa70: 7220 696e 2060 436c 6965 6e74 2e66 726f  r in `Client.fro
+0000aa80: 6d5f 656e 7660 2e0a 0a23 2323 2042 7567  m_env`...### Bug
+0000aa90: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
+0000aaa0: 2062 7567 2077 6865 7265 2060 436c 6965   bug where `Clie
+0000aab0: 6e74 2e62 7569 6c64 6020 776f 756c 6420  nt.build` would 
+0000aac0: 6372 6173 6820 6966 2074 6865 2060 636f  crash if the `co
+0000aad0: 6e66 6967 2e6a 736f 6e60 2066 696c 650a  nfig.json` file.
+0000aae0: 2020 636f 6e74 6169 6e65 6420 6120 6048    contained a `H
+0000aaf0: 7474 7048 6561 6465 7273 6020 656e 7472  ttpHeaders` entr
+0000ab00: 792e 0a2a 2046 6978 6564 2061 2062 7567  y..* Fixed a bug
+0000ab10: 2077 6865 7265 2070 6173 7369 6e67 2060   where passing `
+0000ab20: 6465 636f 6465 3d54 7275 6560 2069 6e20  decode=True` in 
+0000ab30: 736f 6d65 2073 7472 6561 6d69 6e67 206d  some streaming m
+0000ab40: 6574 686f 6473 2077 6f75 6c64 0a20 2063  ethods would.  c
+0000ab50: 7261 7368 2077 6865 6e20 7468 6520 6461  rash when the da
+0000ab60: 656d 6f6e 2773 2072 6573 706f 6e73 6520  emon's response 
+0000ab70: 6861 6420 616e 2075 6e65 7870 6563 7465  had an unexpecte
+0000ab80: 6420 666f 726d 6174 2e0a 2a20 4669 7865  d format..* Fixe
+0000ab90: 6420 6120 6275 6720 7768 6572 6520 6065  d a bug where `e
+0000aba0: 6e76 6972 6f6e 6d65 6e74 6020 7661 6c75  nvironment` valu
+0000abb0: 6573 2077 6974 6820 756e 6963 6f64 6520  es with unicode 
+0000abc0: 6368 6172 6163 7465 7273 2077 6572 656e  characters weren
+0000abd0: 2774 0a20 2068 616e 646c 6564 2070 726f  't.  handled pro
+0000abe0: 7065 726c 7920 696e 2060 6372 6561 7465  perly in `create
+0000abf0: 5f63 6f6e 7461 696e 6572 602e 0a2a 2046  _container`..* F
+0000ac00: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+0000ac10: 2075 7369 6e67 2074 6865 2060 6e70 6970   using the `npip
+0000ac20: 6560 2070 726f 746f 636f 6c20 776f 756c  e` protocol woul
+0000ac30: 6420 736f 6d65 7469 6d65 7320 6272 6561  d sometimes brea
+0000ac40: 6b20 7769 7468 0a20 2060 5661 6c75 6545  k with.  `ValueE
+0000ac50: 7272 6f72 3a20 6275 6666 6572 2073 697a  rror: buffer siz
+0000ac60: 6520 6d75 7374 2062 6520 7374 7269 6374  e must be strict
+0000ac70: 6c79 2070 6f73 6974 6976 6560 2e0a 0a23  ly positive`...#
+0000ac80: 2323 204d 6973 6365 6c6c 616e 656f 7573  ## Miscellaneous
+0000ac90: 0a0a 2a20 4669 7865 6420 616e 2069 7373  ..* Fixed an iss
+0000aca0: 7565 2077 6865 7265 2055 524c 2d71 756f  ue where URL-quo
+0000acb0: 7469 6e67 2069 6e20 646f 636b 6572 2d70  ting in docker-p
+0000acc0: 7920 7761 7320 696e 636f 6e73 6973 7465  y was inconsiste
+0000acd0: 6e74 2077 6974 6820 7468 650a 2020 7175  nt with the.  qu
+0000ace0: 6f74 696e 6720 646f 6e65 2062 7920 7468  oting done by th
+0000acf0: 6520 446f 636b 6572 2043 4c49 2063 6c69  e Docker CLI cli
+0000ad00: 656e 742e 0a2a 2054 6865 2063 6c69 656e  ent..* The clien
+0000ad10: 7420 6e6f 7720 7365 6e64 7320 5443 5020  t now sends TCP 
+0000ad20: 7570 6772 6164 6520 6865 6164 6572 7320  upgrade headers 
+0000ad30: 746f 2068 696e 7420 706f 7465 6e74 6961  to hint potentia
+0000ad40: 6c20 7072 6f78 6965 7320 6162 6f75 740a  l proxies about.
+0000ad50: 2020 636f 6e6e 6563 7469 6f6e 2068 696a    connection hij
+0000ad60: 6163 6b69 6e67 2e0a 2a20 5468 6520 636c  acking..* The cl
+0000ad70: 6965 6e74 206e 6f77 2064 6566 6175 6c74  ient now default
+0000ad80: 7320 746f 2075 7369 6e67 2074 6865 2060  s to using the `
+0000ad90: 6e70 6970 6560 2070 726f 746f 636f 6c20  npipe` protocol 
+0000ada0: 6f6e 2057 696e 646f 7773 2e0a 0a0a 312e  on Windows....1.
+0000adb0: 392e 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374  9.0.-----..[List
+0000adc0: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
+0000add0: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+0000ade0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+0000adf0: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
+0000ae00: 6b65 722d 7079 2f69 7373 7565 733f 713d  ker-py/issues?q=
+0000ae10: 6d69 6c65 7374 6f6e 6525 3341 312e 392e  milestone%3A1.9.
+0000ae20: 302b 6973 2533 4163 6c6f 7365 6429 0a0a  0+is%3Aclosed)..
+0000ae30: 2323 2320 4665 6174 7572 6573 0a0a 2a20  ### Features..* 
+0000ae40: 4164 6465 6420 2a2a 6578 7065 7269 6d65  Added **experime
+0000ae50: 6e74 616c 2a2a 2073 7570 706f 7274 2066  ntal** support f
+0000ae60: 6f72 2057 696e 646f 7773 206e 616d 6564  or Windows named
+0000ae70: 2070 6970 6573 2028 606e 7069 7065 3a2f   pipes (`npipe:/
+0000ae80: 2f60 2070 726f 746f 636f 6c29 2e0a 2a20  /` protocol)..* 
+0000ae90: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+0000aea0: 7220 426c 6f63 6b20 494f 2063 6f6e 7374  r Block IO const
+0000aeb0: 7261 696e 7473 2069 6e20 6043 6c69 656e  raints in `Clien
+0000aec0: 742e 6372 6561 7465 5f68 6f73 745f 636f  t.create_host_co
+0000aed0: 6e66 6967 602e 2054 6869 730a 2020 696e  nfig`. This.  in
+0000aee0: 636c 7564 6573 2070 6172 616d 6574 6572  cludes parameter
+0000aef0: 7320 6062 6c6b 696f 5f77 6569 6768 7460  s `blkio_weight`
+0000af00: 2c20 6062 6c6b 696f 5f77 6569 6768 745f  , `blkio_weight_
+0000af10: 6465 7669 6365 602c 2060 6465 7669 6365  device`, `device
+0000af20: 5f72 6561 645f 6270 7360 2c0a 2020 6064  _read_bps`,.  `d
+0000af30: 6576 6963 655f 7772 6974 655f 6270 7360  evice_write_bps`
+0000af40: 2c20 6064 6576 6963 655f 7265 6164 5f69  , `device_read_i
+0000af50: 6f70 7360 2061 6e64 2060 6465 7669 6365  ops` and `device
+0000af60: 5f77 7269 7465 5f69 6f70 7360 2e0a 2a20  _write_iops`..* 
+0000af70: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+0000af80: 7220 7468 6520 6069 6e74 6572 6e61 6c60  r the `internal`
+0000af90: 2070 6172 616d 2069 6e20 6043 6c69 656e   param in `Clien
+0000afa0: 742e 6372 6561 7465 5f6e 6574 776f 726b  t.create_network
+0000afb0: 602e 0a2a 2041 6464 6564 2073 7570 706f  `..* Added suppo
+0000afc0: 7274 2066 6f72 2060 6970 7634 5f61 6464  rt for `ipv4_add
+0000afd0: 7265 7373 6020 616e 6420 6069 7076 365f  ress` and `ipv6_
+0000afe0: 6164 6472 6573 7360 2069 6e20 7574 696c  address` in util
+0000aff0: 7320 6675 6e63 7469 6f6e 0a20 2060 6372  s function.  `cr
+0000b000: 6561 7465 5f65 6e64 706f 696e 745f 636f  eate_endpoint_co
+0000b010: 6e66 6967 602e 0a2a 2041 6464 6564 2073  nfig`..* Added s
+0000b020: 7570 706f 7274 2066 6f72 2063 7573 746f  upport for custo
+0000b030: 6d20 7573 6572 2061 6765 6e74 2073 6574  m user agent set
+0000b040: 7469 6e67 2069 6e20 7468 6520 6043 6c69  ting in the `Cli
+0000b050: 656e 7460 2063 6f6e 7374 7275 6374 6f72  ent` constructor
+0000b060: 2e0a 2020 4279 2064 6566 6175 6c74 2c20  ..  By default, 
+0000b070: 646f 636b 6572 2d70 7920 6e6f 7720 616c  docker-py now al
+0000b080: 736f 2064 6563 6c61 7265 7320 6974 7365  so declares itse
+0000b090: 6c66 2069 6e20 7468 6520 6055 7365 722d  lf in the `User-
+0000b0a0: 4167 656e 7460 2068 6561 6465 722e 0a0a  Agent` header...
+0000b0b0: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
+0000b0c0: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
+0000b0d0: 6865 7265 2074 6865 2048 5454 5020 7469  here the HTTP ti
+0000b0e0: 6d65 6f75 7420 6f6e 2073 7472 6561 6d69  meout on streami
+0000b0f0: 6e67 2072 6573 706f 6e73 6573 2077 6f75  ng responses wou
+0000b100: 6c64 2073 6f6d 6574 696d 6573 0a20 2062  ld sometimes.  b
+0000b110: 6520 7365 7420 696e 636f 7272 6563 746c  e set incorrectl
+0000b120: 792e 0a2a 2046 6978 6564 2061 6e20 6973  y..* Fixed an is
+0000b130: 7375 6520 7768 6572 6520 6578 706c 6963  sue where explic
+0000b140: 6974 2072 656c 6174 6976 6520 7061 7468  it relative path
+0000b150: 7320 696e 2060 2e64 6f63 6b65 7269 676e  s in `.dockerign
+0000b160: 6f72 6560 2066 696c 6573 2077 6572 650a  ore` files were.
+0000b170: 2020 6e6f 7420 6265 696e 6720 7265 636f    not being reco
+0000b180: 676e 697a 6564 2e0a 0a31 2e38 2e31 0a2d  gnized...1.8.1.-
+0000b190: 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66 2050  ----..[List of P
+0000b1a0: 5273 202f 2069 7373 7565 7320 666f 7220  Rs / issues for 
+0000b1b0: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+0000b1c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000b1d0: 2f64 6f63 6b65 722f 646f 636b 6572 2d70  /docker/docker-p
+0000b1e0: 792f 6973 7375 6573 3f71 3d6d 696c 6573  y/issues?q=miles
+0000b1f0: 746f 6e65 2533 4131 2e38 2e31 2b69 7325  tone%3A1.8.1+is%
+0000b200: 3341 636c 6f73 6564 290a 0a23 2323 2042  3Aclosed)..### B
+0000b210: 7567 6669 7865 730a 0a2a 2046 6978 6564  ugfixes..* Fixed
+0000b220: 2061 2062 7567 2077 6865 7265 2063 616c   a bug where cal
+0000b230: 6c69 6e67 2060 6c6f 6769 6e28 2960 2061  ling `login()` a
+0000b240: 6761 696e 7374 2074 6865 2064 6566 6175  gainst the defau
+0000b250: 6c74 2072 6567 6973 7472 7920 776f 756c  lt registry woul
+0000b260: 6420 6661 696c 0a20 2077 6974 6820 7468  d fail.  with th
+0000b270: 6520 312e 3130 2e78 2065 6e67 696e 650a  e 1.10.x engine.
+0000b280: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+0000b290: 6572 6520 7661 6c75 6573 2069 6e20 656e  ere values in en
+0000b2a0: 7669 726f 6e6d 656e 7420 6669 6c65 7320  vironment files 
+0000b2b0: 776f 756c 6420 6265 2070 6172 7365 6420  would be parsed 
+0000b2c0: 696e 636f 7272 6563 746c 7920 6966 0a20  incorrectly if. 
+0000b2d0: 2074 6865 7920 636f 6e74 6169 6e65 6420   they contained 
+0000b2e0: 616e 2065 7175 616c 2073 6967 6e2e 0a2a  an equal sign..*
+0000b2f0: 2053 7769 7463 6865 6420 746f 2061 2062   Switched to a b
+0000b300: 6574 7465 7220 7375 7070 6f72 7465 6420  etter supported 
+0000b310: 6261 636b 706f 7274 206f 6620 7468 6520  backport of the 
+0000b320: 606d 6174 6368 5f68 6f73 746e 616d 6560  `match_hostname`
+0000b330: 2066 756e 6374 696f 6e2c 0a20 2066 6978   function,.  fix
+0000b340: 696e 6720 6465 7065 6e64 656e 6379 2069  ing dependency i
+0000b350: 7373 7565 7320 696e 2073 6f6d 6520 656e  ssues in some en
+0000b360: 7669 726f 6e6d 656e 7473 2e0a 0a0a 312e  vironments....1.
+0000b370: 382e 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374  8.0.-----..[List
+0000b380: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
+0000b390: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+0000b3a0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+0000b3b0: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
+0000b3c0: 6b65 722d 7079 2f69 7373 7565 733f 713d  ker-py/issues?q=
+0000b3d0: 6d69 6c65 7374 6f6e 6525 3341 312e 382e  milestone%3A1.8.
+0000b3e0: 302b 6973 2533 4163 6c6f 7365 6429 0a0a  0+is%3Aclosed)..
+0000b3f0: 2323 2320 4665 6174 7572 6573 0a0a 2a20  ### Features..* 
+0000b400: 4164 6465 6420 6043 6c69 656e 742e 7570  Added `Client.up
+0000b410: 6461 7465 5f63 6f6e 7461 696e 6572 6020  date_container` 
+0000b420: 6d65 7468 6f64 2028 5570 6461 7465 2072  method (Update r
+0000b430: 6573 6f75 7263 6520 636f 6e66 6967 7320  esource configs 
+0000b440: 6f66 2061 0a20 2063 6f6e 7461 696e 6572  of a.  container
+0000b450: 290a 2a20 4164 6465 6420 7375 7070 6f72  ).* Added suppor
+0000b460: 7420 666f 7220 677a 6970 7065 6420 636f  t for gzipped co
+0000b470: 6e74 6578 7420 696e 2060 436c 6965 6e74  ntext in `Client
+0000b480: 2e62 7569 6c64 600a 2a20 4164 6465 6420  .build`.* Added 
+0000b490: 6162 696c 6974 7920 746f 2073 7065 6369  ability to speci
+0000b4a0: 6679 2049 5020 6164 6472 6573 7320 7768  fy IP address wh
+0000b4b0: 656e 2063 6f6e 6e65 6374 696e 6720 6120  en connecting a 
+0000b4c0: 636f 6e74 6169 6e65 7220 746f 2061 0a20  container to a. 
+0000b4d0: 206e 6574 776f 726b 0a2a 2041 6464 6564   network.* Added
+0000b4e0: 2060 746d 7066 7360 2073 7570 706f 7274   `tmpfs` support
+0000b4f0: 2074 6f20 6043 6c69 656e 742e 6372 6561   to `Client.crea
+0000b500: 7465 5f68 6f73 745f 636f 6e66 6967 600a  te_host_config`.
+0000b510: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+0000b520: 666f 7220 7468 6520 6063 6861 6e67 6573  for the `changes
+0000b530: 6020 7061 7261 6d20 696e 2060 436c 6965  ` param in `Clie
+0000b540: 6e74 2e63 6f6d 6d69 7460 0a2a 2041 6464  nt.commit`.* Add
+0000b550: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
+0000b560: 6865 2060 666f 6c6c 6f77 6020 7061 7261  he `follow` para
+0000b570: 6d20 696e 2060 436c 6965 6e74 2e6c 6f67  m in `Client.log
+0000b580: 7360 0a2a 2041 6464 6564 2073 7570 706f  s`.* Added suppo
+0000b590: 7274 2066 6f72 2074 6865 2060 6368 6563  rt for the `chec
+0000b5a0: 6b5f 6475 706c 6963 6174 6560 2070 6172  k_duplicate` par
+0000b5b0: 616d 2069 6e20 6043 6c69 656e 742e 6372  am in `Client.cr
+0000b5c0: 6561 7465 5f6e 6574 776f 726b 600a 2a20  eate_network`.* 
+0000b5d0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+0000b5e0: 7220 7468 6520 6064 6563 6f64 6560 2070  r the `decode` p
+0000b5f0: 6172 616d 2069 6e20 6043 6c69 656e 742e  aram in `Client.
+0000b600: 7075 7368 6020 616e 6420 6043 6c69 656e  push` and `Clien
+0000b610: 742e 7075 6c6c 600a 2a20 4164 6465 6420  t.pull`.* Added 
+0000b620: 6064 6f63 6b65 722e 6672 6f6d 5f65 6e76  `docker.from_env
+0000b630: 6020 7368 6f72 7463 7574 2066 756e 6374  ` shortcut funct
+0000b640: 696f 6e2e 2049 6e73 7461 6e74 6961 7465  ion. Instantiate
+0000b650: 7320 6120 636c 6965 6e74 2077 6974 680a  s a client with.
+0000b660: 2020 606b 7761 7267 735f 6672 6f6d 5f65    `kwargs_from_e
+0000b670: 6e76 600a 2a20 606b 7761 7267 735f 6672  nv`.* `kwargs_fr
+0000b680: 6f6d 5f65 6e76 6020 6e6f 7720 7375 7070  om_env` now supp
+0000b690: 6f72 7473 2061 6e20 6f70 7469 6f6e 616c  orts an optional
+0000b6a0: 2060 656e 7669 726f 6e6d 656e 7460 2070   `environment` p
+0000b6b0: 6172 616d 6574 6572 2e0a 2020 4966 2070  arameter..  If p
+0000b6c0: 7265 7365 6e74 2c20 7661 6c75 6573 2077  resent, values w
+0000b6d0: 696c 6c20 6265 2066 6574 6368 6564 2066  ill be fetched f
+0000b6e0: 726f 6d20 7468 6973 2064 6963 7469 6f6e  rom this diction
+0000b6f0: 6172 7920 696e 7374 6561 6420 6f66 0a20  ary instead of. 
+0000b700: 2060 6f73 2e65 6e76 6972 6f6e 600a 0a0a   `os.environ`...
+0000b710: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
+0000b720: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+0000b730: 6520 544c 5320 7665 7269 6669 6361 7469  e TLS verificati
+0000b740: 6f6e 2077 6f75 6c64 2066 6169 6c20 7768  on would fail wh
+0000b750: 656e 2075 7369 6e67 2049 5020 6164 6472  en using IP addr
+0000b760: 6573 7365 730a 2020 696e 2074 6865 2063  esses.  in the c
+0000b770: 6572 7469 6669 6361 7465 2773 2060 7375  ertificate's `su
+0000b780: 626a 6563 7441 6c74 4e61 6d65 6020 6669  bjectAltName` fi
+0000b790: 656c 6473 0a2a 2046 6978 6564 2061 6e20  elds.* Fixed an 
+0000b7a0: 6973 7375 6520 7768 6572 6520 7468 6520  issue where the 
+0000b7b0: 6465 6661 756c 7420 544c 5320 7665 7273  default TLS vers
+0000b7c0: 696f 6e20 696e 2054 4c53 436f 6e66 6967  ion in TLSConfig
+0000b7d0: 2077 6f75 6c64 0a20 2062 7265 616b 2069   would.  break i
+0000b7e0: 6e20 736f 6d65 2065 6e76 6972 6f6e 6d65  n some environme
+0000b7f0: 6e74 732e 2060 646f 636b 6572 2d70 7960  nts. `docker-py`
+0000b800: 206e 6f77 2075 7365 7320 544c 5376 3120   now uses TLSv1 
+0000b810: 6279 2064 6566 6175 6c74 0a20 2054 6869  by default.  Thi
+0000b820: 7320 7365 7474 696e 6720 6361 6e20 6265  s setting can be
+0000b830: 206f 7665 7272 6964 6465 6e20 7573 696e   overridden usin
+0000b840: 6720 7468 6520 6073 736c 5f76 6572 7369  g the `ssl_versi
+0000b850: 6f6e 6020 7061 7261 6d20 696e 0a20 2060  on` param in.  `
+0000b860: 6b77 6172 6773 5f66 726f 6d5f 656e 7660  kwargs_from_env`
+0000b870: 206f 7220 7468 6520 6054 4c53 436f 6e66   or the `TLSConf
+0000b880: 6967 6020 636f 6e73 7472 7563 746f 720a  ig` constructor.
+0000b890: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+0000b8a0: 6572 6520 6074 6370 6020 686f 7374 7320  ere `tcp` hosts 
+0000b8b0: 776f 756c 6420 6661 696c 2074 6f20 636f  would fail to co
+0000b8c0: 6e6e 6563 7420 746f 2054 4c53 2d65 6e61  nnect to TLS-ena
+0000b8d0: 626c 6564 0a20 2065 6e64 706f 696e 7473  bled.  endpoints
+0000b8e0: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+0000b8f0: 6865 7265 206c 6f61 6469 6e67 2061 2076  here loading a v
+0000b900: 616c 6964 2064 6f63 6b65 7220 636f 6e66  alid docker conf
+0000b910: 6967 7572 6174 696f 6e20 6669 6c65 2077  iguration file w
+0000b920: 6f75 6c64 2066 6169 6c0a 2a20 4669 7865  ould fail.* Fixe
+0000b930: 6420 6120 6275 6720 7768 6572 6520 736f  d a bug where so
+0000b940: 6d65 2065 6e76 6972 6f6e 6d65 6e74 2076  me environment v
+0000b950: 6172 6961 626c 6573 2073 7065 6369 6669  ariables specifi
+0000b960: 6564 2074 6872 6f75 6768 0a20 2060 6372  ed through.  `cr
+0000b970: 6561 7465 5f63 6f6e 7461 696e 6572 6020  eate_container` 
+0000b980: 776f 756c 6420 6265 2069 6d70 726f 7065  would be imprope
+0000b990: 726c 7920 666f 726d 6174 7465 640a 2a20  rly formatted.* 
+0000b9a0: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+0000b9b0: 6520 7573 696e 6720 7468 6520 756e 6978  e using the unix
+0000b9c0: 2073 6f63 6b65 7420 636f 6e6e 6563 7469   socket connecti
+0000b9d0: 6f6e 2077 6f75 6c64 2072 6169 7365 0a20  on would raise. 
+0000b9e0: 2061 6e20 6572 726f 7220 696e 2073 6f6d   an error in som
+0000b9f0: 6520 6564 6765 2d63 6173 6520 7369 7475  e edge-case situ
+0000ba00: 6174 696f 6e73 0a0a 2323 2320 4d69 7363  ations..### Misc
+0000ba10: 656c 6c61 6e65 6f75 730a 0a2a 2044 6566  ellaneous..* Def
+0000ba20: 6175 6c74 2041 5049 2076 6572 7369 6f6e  ault API version
+0000ba30: 2069 7320 6e6f 7720 312e 3232 2028 696e   is now 1.22 (in
+0000ba40: 7472 6f64 7563 6564 2069 6e20 446f 636b  troduced in Dock
+0000ba50: 6572 2031 2e31 302e 3029 0a0a 0a31 2e37  er 1.10.0)...1.7
+0000ba60: 2e32 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420  .2.-----..[List 
+0000ba70: 6f66 2050 5273 202f 2069 7373 7565 7320  of PRs / issues 
+0000ba80: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
+0000ba90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000baa0: 2e63 6f6d 2f64 6f63 6b65 722f 646f 636b  .com/docker/dock
+0000bab0: 6572 2d70 792f 6973 7375 6573 3f71 3d6d  er-py/issues?q=m
+0000bac0: 696c 6573 746f 6e65 2533 4131 2e37 2e32  ilestone%3A1.7.2
+0000bad0: 2b69 7325 3341 636c 6f73 6564 290a 0a23  +is%3Aclosed)..#
+0000bae0: 2323 2042 7567 6669 7865 730a 0a2a 2046  ## Bugfixes..* F
+0000baf0: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+0000bb00: 2054 4c53 2076 6572 6966 6963 6174 696f   TLS verificatio
+0000bb10: 6e20 7761 7320 696d 7072 6f70 6572 6c79  n was improperly
+0000bb20: 2065 7865 6375 7465 6420 7768 656e 2070   executed when p
+0000bb30: 726f 7669 6469 6e67 0a20 2061 2063 7573  roviding.  a cus
+0000bb40: 746f 6d20 4341 2063 6572 7469 6669 6361  tom CA certifica
+0000bb50: 7465 2e0a 0a31 2e37 2e31 0a2d 2d2d 2d2d  te...1.7.1.-----
+0000bb60: 0a0a 5b4c 6973 7420 6f66 2050 5273 202f  ..[List of PRs /
+0000bb70: 2069 7373 7565 7320 666f 7220 7468 6973   issues for this
+0000bb80: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+0000bb90: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
+0000bba0: 6b65 722f 646f 636b 6572 2d70 792f 6973  ker/docker-py/is
+0000bbb0: 7375 6573 3f71 3d6d 696c 6573 746f 6e65  sues?q=milestone
+0000bbc0: 2533 4131 2e37 2e31 2b69 7325 3341 636c  %3A1.7.1+is%3Acl
+0000bbd0: 6f73 6564 290a 0a23 2323 2046 6561 7475  osed)..### Featu
+0000bbe0: 7265 730a 0a2a 2041 6464 6564 2073 7570  res..* Added sup
+0000bbf0: 706f 7274 2066 6f72 2060 7368 6d5f 7369  port for `shm_si
+0000bc00: 7a65 6020 696e 2060 436c 6965 6e74 2e63  ze` in `Client.c
+0000bc10: 7265 6174 655f 686f 7374 5f63 6f6e 6669  reate_host_confi
+0000bc20: 6760 0a0a 2323 2320 4275 6766 6978 6573  g`..### Bugfixes
+0000bc30: 0a0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+0000bc40: 7768 6572 6520 446f 636b 6572 6669 6c65  where Dockerfile
+0000bc50: 2077 6f75 6c64 2073 6f6d 6574 696d 6573   would sometimes
+0000bc60: 2062 6520 6578 636c 7564 6564 2066 726f   be excluded fro
+0000bc70: 6d20 7468 6520 6275 696c 640a 2020 636f  m the build.  co
+0000bc80: 6e74 6578 742e 0a2a 2046 6978 6564 2061  ntext..* Fixed a
+0000bc90: 2062 7567 2077 6865 7265 2061 2064 6f63   bug where a doc
+0000bca0: 6b65 7220 636f 6e66 6967 2066 696c 6520  ker config file 
+0000bcb0: 636f 6e74 6169 6e69 6e67 2075 6e6b 6e6f  containing unkno
+0000bcc0: 776e 206b 6579 7320 776f 756c 6420 7261  wn keys would ra
+0000bcd0: 6973 650a 2020 616e 2065 7863 6570 7469  ise.  an excepti
+0000bce0: 6f6e 2e0a 2a20 4669 7865 6420 616e 2069  on..* Fixed an i
+0000bcf0: 7373 7565 2077 6974 6820 5353 4c20 636f  ssue with SSL co
+0000bd00: 6e6e 6563 7469 6f6e 7320 6265 6861 7669  nnections behavi
+0000bd10: 6e67 2069 6d70 726f 7065 726c 7920 7768  ng improperly wh
+0000bd20: 656e 2070 794f 7065 6e53 534c 0a20 2077  en pyOpenSSL.  w
+0000bd30: 6173 2069 6e73 7461 6c6c 6564 2069 6e20  as installed in 
+0000bd40: 7468 6520 7361 6d65 2065 6e76 6972 6f6e  the same environ
+0000bd50: 6d65 6e74 2e0a 2a20 5365 7665 7261 6c20  ment..* Several 
+0000bd60: 544c 5320 636f 6e66 6967 7572 6174 696f  TLS configuratio
+0000bd70: 6e20 696d 7072 6f76 656d 656e 7473 0a0a  n improvements..
+0000bd80: 0a31 2e37 2e30 0a2d 2d2d 2d2d 0a0a 5b4c  .1.7.0.-----..[L
+0000bd90: 6973 7420 6f66 2050 5273 202f 2069 7373  ist of PRs / iss
+0000bda0: 7565 7320 666f 7220 7468 6973 2072 656c  ues for this rel
+0000bdb0: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
+0000bdc0: 7468 7562 2e63 6f6d 2f64 6f63 6b65 722f  thub.com/docker/
+0000bdd0: 646f 636b 6572 2d70 792f 6973 7375 6573  docker-py/issues
+0000bde0: 3f71 3d6d 696c 6573 746f 6e65 2533 4131  ?q=milestone%3A1
+0000bdf0: 2e37 2e30 2b69 7325 3341 636c 6f73 6564  .7.0+is%3Aclosed
+0000be00: 290a 0a23 2323 2046 6561 7475 7265 730a  )..### Features.
+0000be10: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+0000be20: 2066 6f72 2063 7573 6f6d 2049 5041 4d20   for cusom IPAM 
+0000be30: 636f 6e66 6967 7572 6174 696f 6e20 696e  configuration in
+0000be40: 2060 436c 6965 6e74 2e63 7265 6174 655f   `Client.create_
+0000be50: 6e65 7477 6f72 6b60 0a2a 2041 6464 6564  network`.* Added
+0000be60: 2069 6e70 7574 2073 7570 706f 7274 2074   input support t
+0000be70: 6f20 6043 6c69 656e 742e 6578 6563 5f63  o `Client.exec_c
+0000be80: 7265 6174 6560 0a2a 2041 6464 6564 2073  reate`.* Added s
+0000be90: 7570 706f 7274 2066 6f72 2060 7374 6f70  upport for `stop
+0000bea0: 5f73 6967 6e61 6c60 2069 6e20 6043 6c69  _signal` in `Cli
+0000beb0: 656e 742e 6372 6561 7465 5f68 6f73 745f  ent.create_host_
+0000bec0: 636f 6e66 6967 600a 2a20 4164 6465 6420  config`.* Added 
+0000bed0: 7375 7070 6f72 7420 666f 7220 6375 7374  support for cust
+0000bee0: 6f6d 2048 5454 5020 6865 6164 6572 7320  om HTTP headers 
+0000bef0: 696e 2044 6f63 6b65 7220 636f 6e66 6967  in Docker config
+0000bf00: 2066 696c 652e 0a2a 2041 6464 6564 2073   file..* Added s
+0000bf10: 7570 706f 7274 2066 6f72 2075 6e73 7065  upport for unspe
+0000bf20: 6369 6669 6564 2074 7261 6e73 6665 7220  cified transfer 
+0000bf30: 7072 6f74 6f63 6f6c 2069 6e20 6062 6173  protocol in `bas
+0000bf40: 655f 7572 6c60 2077 6865 6e20 544c 5320  e_url` when TLS 
+0000bf50: 6973 0a20 2065 6e61 626c 6564 2e0a 0a0a  is.  enabled....
+0000bf60: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
+0000bf70: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+0000bf80: 6520 7468 6520 6066 696c 7465 7273 6020  e the `filters` 
+0000bf90: 7061 7261 6d65 7465 7220 696e 2060 436c  parameter in `Cl
+0000bfa0: 6965 6e74 2e76 6f6c 756d 6573 6020 776f  ient.volumes` wo
+0000bfb0: 756c 6420 6e6f 7420 6265 0a20 2061 7070  uld not be.  app
+0000bfc0: 6c69 6564 2070 726f 7065 726c 792e 0a2a  lied properly..*
+0000bfd0: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+0000bfe0: 7265 206d 656d 6f72 7920 6c69 6d69 7473  re memory limits
+0000bff0: 2077 6f75 6c64 2070 6172 7365 2074 6f20   would parse to 
+0000c000: 696e 636f 7272 6563 7420 7661 6c75 6573  incorrect values
+0000c010: 2e0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+0000c020: 7768 6572 6520 7468 6520 6064 6576 6963  where the `devic
+0000c030: 6573 6020 7061 7261 6d65 7465 7220 696e  es` parameter in
+0000c040: 2060 436c 6965 6e74 2e63 7265 6174 655f   `Client.create_
+0000c050: 686f 7374 5f63 6f6e 6669 6760 0a20 2077  host_config`.  w
+0000c060: 6f75 6c64 2073 6f6d 6574 696d 6573 2062  ould sometimes b
+0000c070: 6520 6d69 7369 6e74 6572 7072 6574 6564  e misinterpreted
+0000c080: 2e0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+0000c090: 7768 6572 6520 696e 7374 616e 7469 6174  where instantiat
+0000c0a0: 696e 6720 6120 6043 6c69 656e 7460 206f  ing a `Client` o
+0000c0b0: 626a 6563 7420 776f 756c 6420 736f 6d65  bject would some
+0000c0c0: 7469 6d65 7320 6372 6173 6820 6966 0a20  times crash if. 
+0000c0d0: 2060 6261 7365 5f75 726c 6020 7761 7320   `base_url` was 
+0000c0e0: 756e 7370 6563 6966 6965 642e 0a2a 2046  unspecified..* F
+0000c0f0: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+0000c100: 2061 6e20 6572 726f 7220 6d65 7373 6167   an error messag
+0000c110: 6520 7265 6c61 7465 6420 746f 2054 4c53  e related to TLS
+0000c120: 2063 6f6e 6669 6775 7261 7469 6f6e 2077   configuration w
+0000c130: 6f75 6c64 206c 696e 6b0a 2020 746f 2061  ould link.  to a
+0000c140: 206e 6f6e 2d65 7869 7374 656e 7420 286f   non-existent (o
+0000c150: 7574 6461 7465 6429 2064 6f63 7320 7061  utdated) docs pa
+0000c160: 6765 2e0a 0a0a 2323 2320 4d69 7363 656c  ge....### Miscel
+0000c170: 6c61 6e65 6f75 730a 0a2a 2050 726f 6365  laneous..* Proce
+0000c180: 7373 696e 6720 6f66 2060 2e64 6f63 6b65  ssing of `.docke
+0000c190: 7269 676e 6f72 6560 2068 6173 2062 6565  rignore` has bee
+0000c1a0: 6e20 6d61 6465 2073 6967 6e69 6669 6361  n made significa
+0000c1b0: 6e74 6c79 2066 6173 7465 722e 0a2a 2044  ntly faster..* D
+0000c1c0: 726f 7070 6564 2065 7870 6c69 6369 7420  ropped explicit 
+0000c1d0: 7375 7070 6f72 7420 666f 7220 5079 7468  support for Pyth
+0000c1e0: 6f6e 2033 2e32 0a0a 312e 362e 300a 2d2d  on 3.2..1.6.0.--
+0000c1f0: 2d2d 2d0a 0a5b 4c69 7374 206f 6620 5052  ---..[List of PR
+0000c200: 7320 2f20 6973 7375 6573 2066 6f72 2074  s / issues for t
+0000c210: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+0000c220: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000c230: 646f 636b 6572 2f64 6f63 6b65 722d 7079  docker/docker-py
+0000c240: 2f69 7373 7565 733f 713d 6d69 6c65 7374  /issues?q=milest
+0000c250: 6f6e 6525 3341 312e 362e 302b 6973 2533  one%3A1.6.0+is%3
+0000c260: 4163 6c6f 7365 6429 0a0a 2323 2320 4665  Aclosed)..### Fe
+0000c270: 6174 7572 6573 0a0a 2a20 4164 6465 6420  atures..* Added 
+0000c280: 7375 7070 6f72 7420 666f 7220 7468 6520  support for the 
+0000c290: 6073 696e 6365 6020 7061 7261 6d20 696e  `since` param in
+0000c2a0: 2060 436c 6965 6e74 2e6c 6f67 7360 2028   `Client.logs` (
+0000c2b0: 696e 7472 6f64 7563 6564 2069 6e20 4150  introduced in AP
+0000c2c0: 490a 2020 7665 7273 696f 6e20 312e 3139  I.  version 1.19
+0000c2d0: 290a 2a20 4164 6465 6420 7375 7070 6f72  ).* Added suppor
+0000c2e0: 7420 666f 7220 7468 6520 6044 4f43 4b45  t for the `DOCKE
+0000c2f0: 525f 434f 4e46 4947 6020 656e 7669 726f  R_CONFIG` enviro
+0000c300: 6e6d 656e 7420 7661 7269 6162 6c65 2077  nment variable w
+0000c310: 6865 6e20 6c6f 6f6b 696e 6720 7570 0a20  hen looking up. 
+0000c320: 2061 7574 6820 636f 6e66 6967 0a2a 2041   auth config.* A
+0000c330: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+0000c340: 2074 6865 2060 7374 7265 616d 6020 7061   the `stream` pa
+0000c350: 7261 6d20 696e 2060 436c 6965 6e74 2e73  ram in `Client.s
+0000c360: 7461 7473 6020 2877 6865 6e20 7365 7420  tats` (when set 
+0000c370: 746f 2060 4661 6c73 6560 2c0a 2020 616c  to `False`,.  al
+0000c380: 6c6f 7773 2075 7365 7220 746f 2072 6574  lows user to ret
+0000c390: 7269 6576 6520 6120 7369 6e67 6c65 2073  rieve a single s
+0000c3a0: 6e61 7073 686f 7420 696e 7374 6561 6420  napshot instead 
+0000c3b0: 6f66 2061 2063 6f6e 7374 616e 7420 6461  of a constant da
+0000c3c0: 7461 2073 7472 6561 6d29 0a2a 2041 6464  ta stream).* Add
+0000c3d0: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
+0000c3e0: 6865 2060 6d65 6d5f 7377 6170 7069 6e65  he `mem_swappine
+0000c3f0: 7373 602c 2060 6f6f 6d5f 6b69 6c6c 5f64  ss`, `oom_kill_d
+0000c400: 6973 6162 6c65 6020 7061 7261 6d73 0a20  isable` params. 
+0000c410: 2069 6e20 6043 6c69 656e 742e 6372 6561   in `Client.crea
+0000c420: 7465 5f68 6f73 745f 636f 6e66 6967 600a  te_host_config`.
+0000c430: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+0000c440: 666f 7220 6275 696c 6420 6172 6775 6d65  for build argume
+0000c450: 6e74 7320 696e 2060 436c 6965 6e74 2e62  nts in `Client.b
+0000c460: 7569 6c64 6020 7468 726f 7567 6820 7468  uild` through th
+0000c470: 6520 6062 7569 6c64 6172 6773 600a 2020  e `buildargs`.  
+0000c480: 7061 7261 6d2e 0a0a 0a23 2323 2042 7567  param....### Bug
+0000c490: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
+0000c4a0: 2062 7567 2077 6865 7265 2073 7472 6561   bug where strea
+0000c4b0: 6d69 6e67 2064 6174 6120 6f76 6572 2048  ming data over H
+0000c4c0: 5454 5053 2077 6f75 6c64 2073 6f6d 6574  TTPS would somet
+0000c4d0: 696d 6573 2062 6568 6176 650a 2020 696e  imes behave.  in
+0000c4e0: 636f 7272 6563 746c 7920 7769 7468 2050  correctly with P
+0000c4f0: 7974 686f 6e20 332e 780a 2a20 4669 7865  ython 3.x.* Fixe
+0000c500: 6420 6120 6275 6720 7768 6572 6520 636f  d a bug where co
+0000c510: 6d6d 616e 6473 2063 6f6e 7461 696e 696e  mmands containin
+0000c520: 6720 756e 6963 6f64 6520 6368 6172 6163  g unicode charac
+0000c530: 7465 7273 2077 6f75 6c64 2062 6520 696e  ters would be in
+0000c540: 636f 7272 6563 746c 790a 2020 6861 6e64  correctly.  hand
+0000c550: 6c65 6420 6279 2060 436c 6965 6e74 2e63  led by `Client.c
+0000c560: 7265 6174 655f 636f 6e74 6169 6e65 7260  reate_container`
+0000c570: 2e0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+0000c580: 7768 6572 6520 6175 7468 2063 6f6e 6669  where auth confi
+0000c590: 6720 6372 6564 656e 7469 616c 7320 636f  g credentials co
+0000c5a0: 6e74 6169 6e69 6e67 2075 6e69 636f 6465  ntaining unicode
+0000c5b0: 2063 6861 7261 6374 6572 7320 776f 756c   characters woul
+0000c5c0: 640a 2020 6361 7573 6520 6661 696c 7572  d.  cause failur
+0000c5d0: 6573 2077 6865 6e20 7075 7368 696e 6720  es when pushing 
+0000c5e0: 2f20 7075 6c6c 696e 6720 696d 6167 6573  / pulling images
+0000c5f0: 2e0a 2a20 5365 7474 696e 6720 6074 6169  ..* Setting `tai
+0000c600: 6c3d 3060 2069 6e20 6043 6c69 656e 742e  l=0` in `Client.
+0000c610: 6c6f 6773 6020 6e6f 206c 6f6e 6765 7220  logs` no longer 
+0000c620: 7368 6f77 7320 7061 7374 206c 6f67 732e  shows past logs.
+0000c630: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+0000c640: 6865 7265 2060 436c 6965 6e74 2e70 756c  here `Client.pul
+0000c650: 6c60 2061 6e64 2060 436c 6965 6e74 2e70  l` and `Client.p
+0000c660: 7573 6860 2063 6f75 6c64 6e27 7420 6861  ush` couldn't ha
+0000c670: 6e64 6c65 2069 6d61 6765 206e 616d 6573  ndle image names
+0000c680: 0a20 2063 6f6e 7461 696e 696e 6720 6120  .  containing a 
+0000c690: 646f 742e 0a0a 0a23 2323 204d 6973 6365  dot....### Misce
+0000c6a0: 6c6c 616e 656f 7573 0a0a 2a20 4465 6661  llaneous..* Defa
+0000c6b0: 756c 7420 4150 4920 7665 7273 696f 6e20  ult API version 
+0000c6c0: 6973 206e 6f77 2031 2e32 3120 2869 6e74  is now 1.21 (int
+0000c6d0: 726f 6475 6365 6420 696e 2044 6f63 6b65  roduced in Docke
+0000c6e0: 7220 312e 392e 3029 0a2a 2053 6576 6572  r 1.9.0).* Sever
+0000c6f0: 616c 2074 6573 7420 696d 7072 6f76 656d  al test improvem
+0000c700: 656e 7473 2061 6e64 2063 6c65 616e 7570  ents and cleanup
+0000c710: 2074 6861 7420 7368 6f75 6c64 206d 616b   that should mak
+0000c720: 6520 7468 6520 7375 6974 6520 6561 7369  e the suite easi
+0000c730: 6572 2074 6f0a 2020 6578 7061 6e64 2061  er to.  expand a
+0000c740: 6e64 206d 6169 6e74 6169 6e20 6d6f 7669  nd maintain movi
+0000c750: 6e67 2066 6f72 7761 7264 2e0a 0a0a 312e  ng forward....1.
+0000c760: 352e 300a 2d2d 2d2d 2d0a 0a5b 4c69 7374  5.0.-----..[List
+0000c770: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
+0000c780: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+0000c790: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+0000c7a0: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
+0000c7b0: 6b65 722d 7079 2f69 7373 7565 733f 713d  ker-py/issues?q=
+0000c7c0: 6d69 6c65 7374 6f6e 6525 3341 312e 352e  milestone%3A1.5.
+0000c7d0: 302b 6973 2533 4163 6c6f 7365 6429 0a0a  0+is%3Aclosed)..
+0000c7e0: 2323 2320 4665 6174 7572 6573 0a0a 2a20  ### Features..* 
+0000c7f0: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+0000c800: 7220 7468 6520 6e65 7477 6f72 6b69 6e67  r the networking
+0000c810: 2041 5049 2069 6e74 726f 6475 6365 6420   API introduced 
+0000c820: 696e 2044 6f63 6b65 7220 312e 392e 300a  in Docker 1.9.0.
+0000c830: 2020 2860 436c 6965 6e74 2e6e 6574 776f    (`Client.netwo
+0000c840: 726b 7360 2c20 6043 6c69 656e 742e 6372  rks`, `Client.cr
+0000c850: 6561 7465 5f6e 6574 776f 726b 602c 2060  eate_network`, `
+0000c860: 436c 6965 6e74 2e72 656d 6f76 655f 6e65  Client.remove_ne
+0000c870: 7477 6f72 6b60 2c0a 2020 6043 6c69 656e  twork`,.  `Clien
+0000c880: 742e 696e 7370 6563 745f 6e65 7477 6f72  t.inspect_networ
+0000c890: 6b60 2c20 6043 6c69 656e 742e 636f 6e6e  k`, `Client.conn
+0000c8a0: 6563 745f 636f 6e74 6169 6e65 725f 746f  ect_container_to
+0000c8b0: 5f6e 6574 776f 726b 602c 0a20 2060 436c  _network`,.  `Cl
+0000c8c0: 6965 6e74 2e64 6973 636f 6e6e 6563 745f  ient.disconnect_
+0000c8d0: 636f 6e74 6169 6e65 725f 6672 6f6d 5f6e  container_from_n
+0000c8e0: 6574 776f 726b 6029 2e0a 2a20 4164 6465  etwork`)..* Adde
+0000c8f0: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
+0000c900: 6520 766f 6c75 6d65 7320 4150 4920 696e  e volumes API in
+0000c910: 7472 6f64 7563 6564 2069 6e20 446f 636b  troduced in Dock
+0000c920: 6572 2031 2e39 2e30 0a20 2028 6043 6c69  er 1.9.0.  (`Cli
+0000c930: 656e 742e 766f 6c75 6d65 7360 2c20 6043  ent.volumes`, `C
+0000c940: 6c69 656e 742e 6372 6561 7465 5f76 6f6c  lient.create_vol
+0000c950: 756d 6560 2c20 6043 6c69 656e 742e 696e  ume`, `Client.in
+0000c960: 7370 6563 745f 766f 6c75 6d65 602c 0a20  spect_volume`,. 
+0000c970: 2060 436c 6965 6e74 2e72 656d 6f76 655f   `Client.remove_
+0000c980: 766f 6c75 6d65 6029 2e0a 2a20 4164 6465  volume`)..* Adde
+0000c990: 6420 7375 7070 6f72 7420 666f 7220 7468  d support for th
+0000c9a0: 6520 6067 726f 7570 5f61 6464 6020 7061  e `group_add` pa
+0000c9b0: 7261 6d65 7465 7220 696e 2060 6372 6561  rameter in `crea
+0000c9c0: 7465 5f68 6f73 745f 636f 6e66 6967 602e  te_host_config`.
+0000c9d0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+0000c9e0: 2066 6f72 2074 6865 2043 5055 2043 4653   for the CPU CFS
+0000c9f0: 2028 6063 7075 5f71 756f 7461 6020 616e   (`cpu_quota` an
+0000ca00: 6420 6063 7075 5f70 6572 696f 6460 2920  d `cpu_period`) 
+0000ca10: 7061 7261 6d65 7465 7273 0a20 2069 6e20  parameters.  in 
+0000ca20: 6063 7265 6174 655f 686f 7374 5f63 6f6e  `create_host_con
+0000ca30: 6669 6760 2e0a 2a20 4164 6465 6420 7375  fig`..* Added su
+0000ca40: 7070 6f72 7420 666f 7220 7468 6520 6172  pport for the ar
+0000ca50: 6368 6976 6520 4150 4920 656e 6470 6f69  chive API endpoi
+0000ca60: 6e74 2028 6043 6c69 656e 742e 6765 745f  nt (`Client.get_
+0000ca70: 6172 6368 6976 6560 2c0a 2020 6043 6c69  archive`,.  `Cli
+0000ca80: 656e 742e 7075 745f 6172 6368 6976 6560  ent.put_archive`
+0000ca90: 292e 0a2a 2041 6464 6564 2073 7570 706f  )..* Added suppo
+0000caa0: 7274 2066 6f72 2060 7073 5f61 7267 7360  rt for `ps_args`
+0000cab0: 2070 6172 616d 6574 6572 2069 6e20 6043   parameter in `C
+0000cac0: 6c69 656e 742e 746f 7060 2e0a 0a0a 2323  lient.top`....##
+0000cad0: 2320 4275 6766 6978 6573 0a0a 2a20 4669  # Bugfixes..* Fi
+0000cae0: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
+0000caf0: 7370 6563 6966 7969 6e67 2076 6f6c 756d  specifying volum
+0000cb00: 6520 6269 6e64 7320 7769 7468 2075 6e69  e binds with uni
+0000cb10: 636f 6465 2063 6861 7261 6374 6572 7320  code characters 
+0000cb20: 776f 756c 640a 2020 6661 696c 2e0a 2a20  would.  fail..* 
+0000cb30: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+0000cb40: 6520 7072 6f76 6964 696e 6720 616e 2065  e providing an e
+0000cb50: 7870 6c69 6369 7420 7072 6f74 6f63 6f6c  xplicit protocol
+0000cb60: 2069 6e20 6043 6c69 656e 742e 706f 7274   in `Client.port
+0000cb70: 6020 776f 756c 6420 6661 696c 0a20 2074  ` would fail.  t
+0000cb80: 6f20 7969 656c 6420 7468 6520 6578 7065  o yield the expe
+0000cb90: 6374 6564 2072 6573 756c 742e 0a2a 2046  cted result..* F
+0000cba0: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+0000cbb0: 2074 6865 2070 7269 6f72 6974 7920 7072   the priority pr
+0000cbc0: 6f74 6f63 6f6c 2072 6574 7572 6e65 6420  otocol returned 
+0000cbd0: 6279 2060 436c 6965 6e74 2e70 6f72 7460  by `Client.port`
+0000cbe0: 2077 6f75 6c64 2062 6520 5544 500a 2020   would be UDP.  
+0000cbf0: 696e 7374 6561 6420 6f66 2074 6865 2065  instead of the e
+0000cc00: 7870 6563 7465 6420 5443 502e 0a0a 2323  xpected TCP...##
+0000cc10: 2320 4d69 7363 656c 6c61 6e65 6f75 730a  # Miscellaneous.
+0000cc20: 0a2a 2042 726f 6b65 2075 7020 436c 6965  .* Broke up Clie
+0000cc30: 6e74 2063 6f64 6520 696e 746f 2073 6576  nt code into sev
+0000cc40: 6572 616c 2066 696c 6573 2074 6f20 6661  eral files to fa
+0000cc50: 6369 6c69 7461 7465 206d 6169 6e74 656e  cilitate mainten
+0000cc60: 616e 6365 2061 6e64 0a20 2063 6f6e 7472  ance and.  contr
+0000cc70: 6962 7574 696f 6e2e 0a2a 2041 6464 6564  ibution..* Added
+0000cc80: 2063 6f6e 7472 6962 7574 696e 6720 6775   contributing gu
+0000cc90: 6964 656c 696e 6573 2074 6f20 7468 6520  idelines to the 
+0000cca0: 7265 706f 7369 746f 7279 2e0a 0a31 2e34  repository...1.4
+0000ccb0: 2e30 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420  .0.-----..[List 
+0000ccc0: 6f66 2050 5273 202f 2069 7373 7565 7320  of PRs / issues 
+0000ccd0: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
+0000cce0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000ccf0: 2e63 6f6d 2f64 6f63 6b65 722f 646f 636b  .com/docker/dock
+0000cd00: 6572 2d70 792f 6973 7375 6573 3f71 3d6d  er-py/issues?q=m
+0000cd10: 696c 6573 746f 6e65 2533 4131 2e34 2e30  ilestone%3A1.4.0
+0000cd20: 2b69 7325 3341 636c 6f73 6564 290a 0a23  +is%3Aclosed)..#
+0000cd30: 2323 2044 6570 7265 6361 7469 6f6e 2077  ## Deprecation w
+0000cd40: 6172 6e69 6e67 0a0a 2a20 6064 6f63 6b65  arning..* `docke
+0000cd50: 722e 7574 696c 732e 6372 6561 7465 5f68  r.utils.create_h
+0000cd60: 6f73 745f 636f 6e66 6967 6020 6973 2064  ost_config` is d
+0000cd70: 6570 7265 6361 7465 6420 696e 2066 6176  eprecated in fav
+0000cd80: 6f72 206f 660a 2020 6043 6c69 656e 742e  or of.  `Client.
+0000cd90: 6372 6561 7465 5f68 6f73 745f 636f 6e66  create_host_conf
+0000cda0: 6967 602e 0a0a 2323 2320 4665 6174 7572  ig`...### Featur
+0000cdb0: 6573 0a0a 2a20 4164 6465 6420 6075 7469  es..* Added `uti
+0000cdc0: 6c73 2e70 6172 7365 5f65 6e76 5f66 696c  ls.parse_env_fil
+0000cdd0: 6560 2074 6f20 7375 7070 6f72 7420 656e  e` to support en
+0000cde0: 762d 6669 6c65 732e 0a20 2053 6565 205b  v-files..  See [
+0000cdf0: 646f 6373 5d28 6874 7470 733a 2f2f 646f  docs](https://do
+0000ce00: 636b 6572 2d70 792e 7265 6164 7468 6564  cker-py.readthed
+0000ce10: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+0000ce20: 2f61 7069 2f23 6372 6561 7465 5f63 6f6e  /api/#create_con
+0000ce30: 7461 696e 6572 290a 2020 666f 7220 7573  tainer).  for us
+0000ce40: 6167 652e 0a2a 2041 6464 6564 2073 7570  age..* Added sup
+0000ce50: 706f 7274 2066 6f72 2061 7262 6974 7261  port for arbitra
+0000ce60: 7279 206c 6f67 2064 7269 7665 7273 0a2a  ry log drivers.*
+0000ce70: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
+0000ce80: 6f72 2055 524c 2070 6174 6873 2069 6e20  or URL paths in 
+0000ce90: 7468 6520 646f 636b 6572 2068 6f73 7420  the docker host 
+0000cea0: 5552 4c20 2860 6261 7365 5f75 726c 6029  URL (`base_url`)
+0000ceb0: 0a2a 2044 7261 7374 6963 616c 6c79 2069  .* Drastically i
+0000cec0: 6d70 726f 7665 6420 7375 7070 6f72 7420  mproved support 
+0000ced0: 666f 7220 2e64 6f63 6b65 7269 676e 6f72  for .dockerignor
+0000cee0: 6520 7379 6e74 6178 0a0a 2323 2320 4275  e syntax..### Bu
+0000cef0: 6766 6978 6573 0a0a 2a20 4669 7865 6420  gfixes..* Fixed 
+0000cf00: 6120 6275 6720 7768 6572 6520 6578 6563  a bug where exec
+0000cf10: 5f69 6e73 7065 6374 2077 6f75 6c64 2061  _inspect would a
+0000cf20: 6c6c 6f77 2069 6e76 6f63 6174 696f 6e20  llow invocation 
+0000cf30: 7768 656e 2074 6865 2041 5049 2076 6572  when the API ver
+0000cf40: 7369 6f6e 0a20 2077 6173 2074 6f6f 206c  sion.  was too l
+0000cf50: 6f77 2e0a 2a20 4669 7865 6420 6120 6275  ow..* Fixed a bu
+0000cf60: 6720 7768 6572 6520 6064 6f63 6b65 722e  g where `docker.
+0000cf70: 7574 696c 732e 706f 7274 732e 7370 6c69  utils.ports.spli
+0000cf80: 745f 706f 7274 6020 776f 756c 6420 6272  t_port` would br
+0000cf90: 6561 6b20 6966 2061 6e20 6f70 656e 0a20  eak if an open. 
+0000cfa0: 2072 616e 6765 2077 6173 2070 726f 7669   range was provi
+0000cfb0: 6465 642e 0a2a 2046 6978 6564 2061 2062  ded..* Fixed a b
+0000cfc0: 7567 2077 6865 7265 2069 6e76 616c 6964  ug where invalid
+0000cfd0: 2069 6d61 6765 2049 4473 202f 2063 6f6e   image IDs / con
+0000cfe0: 7461 696e 6572 2049 4473 2063 6f75 6c64  tainer IDs could
+0000cff0: 2062 6520 7072 6f76 6964 6564 2074 6f0a   be provided to.
+0000d000: 2020 6279 7061 7373 206f 7220 7265 726f    bypass or rero
+0000d010: 7574 6520 7265 7175 6573 7420 5552 4c73  ute request URLs
+0000d020: 0a2a 2044 6566 6175 6c74 2060 6261 7365  .* Default `base
+0000d030: 5f75 726c 6020 6e6f 7720 6164 6170 7473  _url` now adapts
+0000d040: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+0000d050: 6520 4f53 2028 6265 7474 6572 2057 696e  e OS (better Win
+0000d060: 646f 7773 2073 7570 706f 7274 290a 2a20  dows support).* 
+0000d070: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+0000d080: 6520 7573 696e 6720 616e 2069 6e74 6567  e using an integ
+0000d090: 6572 2061 7320 7468 6520 7573 6572 2070  er as the user p
+0000d0a0: 6172 616d 2069 6e0a 2020 6043 6c69 656e  aram in.  `Clien
+0000d0b0: 742e 6372 6561 7465 5f63 6f6e 7461 696e  t.create_contain
+0000d0c0: 6572 6020 776f 756c 6420 7265 7375 6c74  er` would result
+0000d0d0: 2069 6e20 6120 6661 696c 7572 652e 0a0a   in a failure...
+0000d0e0: 2323 2320 4d69 7363 656c 6c61 6e65 6f75  ### Miscellaneou
+0000d0f0: 730a 0a2a 2044 6f63 7320 6669 7865 730a  s..* Docs fixes.
+0000d100: 2a20 496e 7465 6772 6174 696f 6e20 7465  * Integration te
+0000d110: 7374 7320 6172 6520 6e6f 7720 7275 6e20  sts are now run 
+0000d120: 6173 2070 6172 7420 6f66 206f 7572 2063  as part of our c
+0000d130: 6f6e 7469 6e75 6f75 7320 696e 7465 6772  ontinuous integr
+0000d140: 6174 696f 6e2e 0a2a 2055 7064 6174 6564  ation..* Updated
+0000d150: 2064 6570 656e 6465 6e63 7920 6f6e 2060   dependency on `
+0000d160: 7369 7860 206c 6962 7261 7279 0a0a 312e  six` library..1.
+0000d170: 332e 310a 2d2d 2d2d 2d0a 0a5b 4c69 7374  3.1.-----..[List
+0000d180: 206f 6620 5052 7320 2f20 6973 7375 6573   of PRs / issues
+0000d190: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+0000d1a0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+0000d1b0: 622e 636f 6d2f 646f 636b 6572 2f64 6f63  b.com/docker/doc
+0000d1c0: 6b65 722d 7079 2f69 7373 7565 733f 713d  ker-py/issues?q=
+0000d1d0: 6d69 6c65 7374 6f6e 6525 3341 312e 332e  milestone%3A1.3.
+0000d1e0: 312b 6973 2533 4163 6c6f 7365 6429 0a0a  1+is%3Aclosed)..
+0000d1f0: 2323 2320 4275 6766 6978 6573 0a0a 2a20  ### Bugfixes..* 
+0000d200: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+0000d210: 6520 656d 7074 7920 6368 756e 6b73 2069  e empty chunks i
+0000d220: 6e20 7374 7265 616d 7320 7761 7320 6d69  n streams was mi
+0000d230: 7369 6e74 6572 7072 6574 6564 2061 7320  sinterpreted as 
+0000d240: 454f 462e 0a2a 2060 6461 7465 7469 6d65  EOF..* `datetime
+0000d250: 6020 6172 6775 6d65 6e74 7320 7061 7373  ` arguments pass
+0000d260: 6564 2074 6f20 6043 6c69 656e 742e 6576  ed to `Client.ev
+0000d270: 656e 7473 6020 7061 7261 6d65 7465 7273  ents` parameters
+0000d280: 2060 7369 6e63 6560 2061 6e64 0a20 2060   `since` and.  `
+0000d290: 756e 7469 6c60 2061 7265 206e 6f77 2061  until` are now a
+0000d2a0: 6c77 6179 7320 636f 6e73 6964 6572 6564  lways considered
+0000d2b0: 2074 6f20 6265 2055 5443 2e0a 2a20 4669   to be UTC..* Fi
+0000d2c0: 7865 6420 6120 6275 6720 7769 7468 2044  xed a bug with D
+0000d2d0: 6f63 6b65 7220 312e 372e 7820 7768 6572  ocker 1.7.x wher
+0000d2e0: 6520 7468 6520 7772 6f6e 6720 6175 7468  e the wrong auth
+0000d2f0: 2068 6561 6465 7273 2077 6572 6520 6265   headers were be
+0000d300: 696e 6720 7061 7373 6564 0a20 2069 6e20  ing passed.  in 
+0000d310: 6043 6c69 656e 742e 6275 696c 6460 2c20  `Client.build`, 
+0000d320: 6661 696c 696e 6720 6275 696c 6473 2074  failing builds t
+0000d330: 6861 7420 6465 7065 6e64 6564 206f 6e20  hat depended on 
+0000d340: 7072 6976 6174 6520 696d 6167 6573 2e0a  private images..
+0000d350: 2a20 6043 6c69 656e 742e 6578 6563 5f63  * `Client.exec_c
+0000d360: 7265 6174 6560 2063 616e 206e 6f77 2072  reate` can now r
+0000d370: 6574 7269 6576 6520 7468 6520 6049 6460  etrieve the `Id`
+0000d380: 206b 6579 2066 726f 6d20 6120 6469 6374   key from a dict
+0000d390: 696f 6e61 7279 2066 6f72 2069 7473 0a20  ionary for its. 
+0000d3a0: 2063 6f6e 7461 696e 6572 2070 6172 616d   container param
+0000d3b0: 2e0a 0a23 2323 204d 6973 6365 6c6c 616e  ...### Miscellan
+0000d3c0: 656f 7573 0a0a 2a20 3430 3420 4150 4920  eous..* 404 API 
+0000d3d0: 7374 6174 7573 206e 6f77 2072 6169 7365  status now raise
+0000d3e0: 7320 6064 6f63 6b65 722e 6572 726f 7273  s `docker.errors
+0000d3f0: 2e4e 6f74 466f 756e 6460 2e20 5468 6973  .NotFound`. This
+0000d400: 2065 7863 6570 7469 6f6e 2069 6e68 6572   exception inher
+0000d410: 6974 730a 2020 6041 5049 4572 726f 7260  its.  `APIError`
+0000d420: 2077 6869 6368 2077 6173 2075 7365 6420   which was used 
+0000d430: 7072 6576 696f 7573 6c79 2e0a 2a20 446f  previously..* Do
+0000d440: 6373 2066 6978 6573 0a2a 2054 6573 7420  cs fixes.* Test 
+0000d450: 6669 7865 730a 0a31 2e33 2e30 0a2d 2d2d  fixes..1.3.0.---
+0000d460: 2d2d 0a0a 5b4c 6973 7420 6f66 2050 5273  --..[List of PRs
+0000d470: 202f 2069 7373 7565 7320 666f 7220 7468   / issues for th
+0000d480: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
+0000d490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+0000d4a0: 6f63 6b65 722f 646f 636b 6572 2d70 792f  ocker/docker-py/
+0000d4b0: 6973 7375 6573 3f71 3d6d 696c 6573 746f  issues?q=milesto
+0000d4c0: 6e65 2533 4131 2e33 2e30 2b69 7325 3341  ne%3A1.3.0+is%3A
+0000d4d0: 636c 6f73 6564 290a 0a23 2323 2044 6570  closed)..### Dep
+0000d4e0: 7265 6361 7469 6f6e 2077 6172 6e69 6e67  recation warning
+0000d4f0: 0a0a 2a20 4173 2061 6e6e 6f75 6e63 6564  ..* As announced
+0000d500: 2069 6e20 7468 6520 312e 322e 3020 7265   in the 1.2.0 re
+0000d510: 6c65 6173 652c 2060 436c 6965 6e74 2e65  lease, `Client.e
+0000d520: 7865 6375 7465 6020 6861 7320 6265 656e  xecute` has been
+0000d530: 2072 656d 6f76 6564 2069 6e20 6661 766f   removed in favo
+0000d540: 720a 2020 6f66 2060 436c 6965 6e74 2e65  r.  of `Client.e
+0000d550: 7865 635f 6372 6561 7465 6020 616e 6420  xec_create` and 
+0000d560: 6043 6c69 656e 742e 6578 6563 5f73 7461  `Client.exec_sta
+0000d570: 7274 602e 0a0a 2323 2320 4665 6174 7572  rt`...### Featur
+0000d580: 6573 0a0a 2a20 6065 7874 7261 5f68 6f73  es..* `extra_hos
+0000d590: 7473 6020 7061 7261 6d65 7465 7220 696e  ts` parameter in
+0000d5a0: 2068 6f73 7420 636f 6e66 6967 2063 616e   host config can
+0000d5b0: 206e 6f77 2061 6c73 6f20 6265 2070 726f   now also be pro
+0000d5c0: 7669 6465 6420 6173 2061 206c 6973 742e  vided as a list.
+0000d5d0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+0000d5e0: 2066 6f72 2060 6d65 6d6f 7279 5f6c 696d   for `memory_lim
+0000d5f0: 6974 6020 616e 6420 606d 656d 7377 6170  it` and `memswap
+0000d600: 5f6c 696d 6974 6020 696e 2068 6f73 7420  _limit` in host 
+0000d610: 636f 6e66 6967 2074 6f0a 2020 636f 6d70  config to.  comp
+0000d620: 6c79 2077 6974 6820 7265 6365 6e74 2064  ly with recent d
+0000d630: 6570 7265 6361 7469 6f6e 732e 0a2a 2041  eprecations..* A
+0000d640: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+0000d650: 2060 766f 6c75 6d65 5f64 7269 7665 7260   `volume_driver`
+0000d660: 2069 6e20 6043 6c69 656e 742e 6372 6561   in `Client.crea
+0000d670: 7465 5f63 6f6e 7461 696e 6572 600a 2a20  te_container`.* 
+0000d680: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+0000d690: 7220 6164 7661 6e63 6564 206d 6f64 6573  r advanced modes
+0000d6a0: 2069 6e20 766f 6c75 6d65 2062 696e 6473   in volume binds
+0000d6b0: 2028 7573 696e 6720 7468 6520 606d 6f64   (using the `mod
+0000d6c0: 6560 206b 6579 290a 2a20 4164 6465 6420  e` key).* Added 
+0000d6d0: 7375 7070 6f72 7420 666f 7220 6064 6563  support for `dec
+0000d6e0: 6f64 6560 2069 6e20 6043 6c69 656e 742e  ode` in `Client.
+0000d6f0: 6275 696c 6460 2028 6465 636f 6465 7320  build` (decodes 
+0000d700: 4a53 4f4e 2073 7472 6561 6d20 6f6e 2074  JSON stream on t
+0000d710: 6865 2066 6c79 290a 2a20 646f 636b 6572  he fly).* docker
+0000d720: 2d70 7920 7769 6c6c 206e 6f77 206c 6f6f  -py will now loo
+0000d730: 6b20 666f 7220 6c6f 6769 6e20 636f 6e66  k for login conf
+0000d740: 6967 7572 6174 696f 6e20 756e 6465 7220  iguration under 
+0000d750: 7468 6520 6e65 7720 636f 6e66 6967 2070  the new config p
+0000d760: 6174 682c 0a20 2061 6e64 2066 616c 6c20  ath,.  and fall 
+0000d770: 6261 636b 2074 6f20 7468 6520 6f6c 6420  back to the old 
+0000d780: 607e 2f2e 646f 636b 6572 6366 6760 2070  `~/.dockercfg` p
+0000d790: 6174 6820 6966 206e 6f74 2070 7265 7365  ath if not prese
+0000d7a0: 6e74 2e0a 0a23 2323 2042 7567 6669 7865  nt...### Bugfixe
+0000d7b0: 730a 0a2a 2043 6f6e 6669 6775 7261 7469  s..* Configurati
+0000d7c0: 6f6e 2066 696c 6520 6c6f 6f6b 7570 206e  on file lookup n
+0000d7d0: 6f77 2061 6c73 6f20 776f 726b 206f 6e20  ow also work on 
+0000d7e0: 706c 6174 666f 726d 7320 7468 6174 2064  platforms that d
+0000d7f0: 6f6e 2774 2064 6566 696e 6520 610a 2020  on't define a.  
+0000d800: 6024 484f 4d45 6020 656e 7669 726f 6e6d  `$HOME` environm
+0000d810: 656e 7420 7661 7269 6162 6c65 2e0a 2a20  ent variable..* 
+0000d820: 4669 7865 6420 616e 2069 7373 7565 2077  Fixed an issue w
+0000d830: 6865 7265 2070 696e 6769 6e67 2061 2076  here pinging a v
+0000d840: 3220 7072 6976 6174 6520 7265 6769 7374  2 private regist
+0000d850: 7279 2077 6173 6e27 7420 776f 726b 696e  ry wasn't workin
+0000d860: 6720 7072 6f70 6572 6c79 2c0a 2020 7072  g properly,.  pr
+0000d870: 6576 656e 7469 6e67 2075 7365 7273 2066  eventing users f
+0000d880: 726f 6d20 7075 7368 696e 6720 616e 6420  rom pushing and 
+0000d890: 7075 6c6c 696e 672e 0a2a 2060 7075 6c6c  pulling..* `pull
+0000d8a0: 6020 7061 7261 6d65 7465 7220 696e 2060  ` parameter in `
+0000d8b0: 436c 6965 6e74 2e62 7569 6c64 6020 6e6f  Client.build` no
+0000d8c0: 7720 6465 6661 756c 7473 2074 6f20 6046  w defaults to `F
+0000d8d0: 616c 7365 602e 2046 6978 6573 2061 2062  alse`. Fixes a b
+0000d8e0: 7567 2077 6865 7265 0a20 2074 6865 2064  ug where.  the d
+0000d8f0: 6566 6175 6c74 206f 7074 696f 6e73 2077  efault options w
+0000d900: 6f75 6c64 2074 7279 2074 6f20 666f 7263  ould try to forc
+0000d910: 6520 6120 7075 6c6c 206f 6620 6e6f 6e2d  e a pull of non-
+0000d920: 7265 6d6f 7465 2069 6d61 6765 732e 0a2a  remote images..*
+0000d930: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+0000d940: 7265 2067 6574 7469 6e67 206c 6f67 7320  re getting logs 
+0000d950: 6672 6f6d 2074 7479 2d65 6e61 626c 6564  from tty-enabled
+0000d960: 2063 6f6e 7461 696e 6572 7320 7761 736e   containers wasn
+0000d970: 2774 2077 6f72 6b69 6e67 0a20 2070 726f  't working.  pro
+0000d980: 7065 726c 7920 7769 7468 206d 6f72 6520  perly with more 
+0000d990: 7265 6365 6e74 2076 6572 7369 6f6e 7320  recent versions 
+0000d9a0: 6f66 2044 6f63 6b65 720a 2a20 6043 6c69  of Docker.* `Cli
+0000d9b0: 656e 742e 7075 7368 6020 616e 6420 6043  ent.push` and `C
+0000d9c0: 6c69 656e 742e 7075 6c6c 6020 7769 6c6c  lient.pull` will
+0000d9d0: 206e 6f77 2072 6169 7365 2065 7863 6570   now raise excep
+0000d9e0: 7469 6f6e 7320 6966 2074 6865 2048 5454  tions if the HTT
+0000d9f0: 500a 2020 7374 6174 7573 2069 6e64 6963  P.  status indic
+0000da00: 6174 6573 2061 6e20 6572 726f 722e 0a2a  ates an error..*
+0000da10: 2046 6978 6564 2061 2062 7567 2077 6974   Fixed a bug wit
+0000da20: 6820 6164 6170 7465 7220 6c6f 6f6b 7570  h adapter lookup
+0000da30: 2077 6865 6e20 7573 696e 6720 7468 6520   when using the 
+0000da40: 556e 6978 2073 6f63 6b65 7420 6164 6170  Unix socket adap
+0000da50: 7465 720a 2020 2874 6869 7320 6166 6665  ter.  (this affe
+0000da60: 6374 6564 2073 6f6d 6520 7765 6972 6420  cted some weird 
+0000da70: 6564 6765 2063 6173 6573 2c20 7365 6520  edge cases, see 
+0000da80: 6973 7375 6520 2336 3437 2066 6f72 2064  issue #647 for d
+0000da90: 6574 6169 6c73 290a 2a20 4669 7865 6420  etails).* Fixed 
+0000daa0: 6120 6275 6720 7768 6572 6520 7072 6f76  a bug where prov
+0000dab0: 6964 696e 6720 6074 696d 656f 7574 3d4e  iding `timeout=N
+0000dac0: 6f6e 6560 2074 6f20 6043 6c69 656e 742e  one` to `Client.
+0000dad0: 7374 6f70 6020 776f 756c 6420 7265 7375  stop` would resu
+0000dae0: 6c74 0a20 2069 6e20 616e 2065 7863 6570  lt.  in an excep
+0000daf0: 7469 6f6e 2064 6573 7069 7465 2074 6865  tion despite the
+0000db00: 2075 7365 6361 7365 2062 6569 6e67 2076   usecase being v
+0000db10: 616c 6964 2e0a 2a20 4164 6465 6420 6067  alid..* Added `g
+0000db20: 6974 4060 2074 6f20 7468 6520 6c69 7374  it@` to the list
+0000db30: 206f 6620 7661 6c69 6420 7072 6566 6978   of valid prefix
+0000db40: 6573 2066 6f72 2072 656d 6f74 6520 6275  es for remote bu
+0000db50: 696c 6420 7061 7468 732e 0a0a 2323 2320  ild paths...### 
+0000db60: 4465 7065 6e64 656e 6369 6573 0a0a 2a20  Dependencies..* 
+0000db70: 5468 6520 7765 6273 6f63 6b65 742d 636c  The websocket-cl
+0000db80: 6965 6e74 2064 6570 656e 6465 6e63 7920  ient dependency 
+0000db90: 6861 7320 6265 656e 2075 7064 6174 6564  has been updated
+0000dba0: 2074 6f20 6120 6d6f 7265 2072 6563 656e   to a more recen
+0000dbb0: 7420 7665 7273 696f 6e2e 0a20 2054 6869  t version..  Thi
+0000dbc0: 7320 6e65 7720 7665 7273 696f 6e20 616c  s new version al
+0000dbd0: 736f 2073 7570 706f 7274 7320 5079 7468  so supports Pyth
+0000dbe0: 6f6e 2033 2e78 2c20 6d61 6b69 6e67 2060  on 3.x, making `
+0000dbf0: 6174 7461 6368 5f73 6f63 6b65 7460 2061  attach_socket` a
+0000dc00: 7661 696c 6162 6c65 0a20 206f 6e20 7468  vailable.  on th
+0000dc10: 6f73 6520 7665 7273 696f 6e73 2061 7320  ose versions as 
+0000dc20: 7765 6c6c 2e0a 0a23 2323 2044 6f63 756d  well...### Docum
+0000dc30: 656e 7461 7469 6f6e 0a0a 2a20 5661 7269  entation..* Vari
+0000dc40: 6f75 7320 6669 7865 730a 0a31 2e32 2e33  ous fixes..1.2.3
+0000dc50: 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66  .-----..[List of
+0000dc60: 2050 5273 202f 2069 7373 7565 7320 666f   PRs / issues fo
+0000dc70: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
+0000dc80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000dc90: 6f6d 2f64 6f63 6b65 722f 646f 636b 6572  om/docker/docker
+0000dca0: 2d70 792f 6973 7375 6573 3f71 3d6d 696c  -py/issues?q=mil
+0000dcb0: 6573 746f 6e65 2533 4131 2e32 2e33 2b69  estone%3A1.2.3+i
+0000dcc0: 7325 3341 636c 6f73 6564 290a 0a23 2323  s%3Aclosed)..###
+0000dcd0: 2044 6570 7265 6361 7469 6f6e 2077 6172   Deprecation war
+0000dce0: 6e69 6e67 0a0a 2a20 5061 7373 696e 6720  ning..* Passing 
+0000dcf0: 686f 7374 2063 6f6e 6669 6720 696e 2074  host config in t
+0000dd00: 6865 2060 436c 6965 6e74 2e73 7461 7274  he `Client.start
+0000dd10: 6020 6d65 7468 6f64 2069 7320 6e6f 7720  ` method is now 
+0000dd20: 6465 7072 6563 6174 6564 2e20 506c 6561  deprecated. Plea
+0000dd30: 7365 0a20 2075 7365 2074 6865 2060 686f  se.  use the `ho
+0000dd40: 7374 5f63 6f6e 6669 6760 2069 6e20 6043  st_config` in `C
+0000dd50: 6c69 656e 742e 6372 6561 7465 5f63 6f6e  lient.create_con
+0000dd60: 7461 696e 6572 6020 696e 7374 6561 642e  tainer` instead.
+0000dd70: 0a0a 2323 2320 4665 6174 7572 6573 0a0a  ..### Features..
+0000dd80: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+0000dd90: 666f 7220 6070 7269 7669 6c65 6765 6460  for `privileged`
+0000dda0: 2070 6172 616d 2069 6e20 6043 6c69 656e   param in `Clien
+0000ddb0: 742e 6578 6563 5f63 7265 6174 6560 0a20  t.exec_create`. 
+0000ddc0: 2028 6f6e 6c79 2061 7661 696c 6162 6c65   (only available
+0000ddd0: 2069 6e20 4150 4920 3e3d 2031 2e31 3929   in API >= 1.19)
+0000dde0: 0a2a 2056 6f6c 756d 6520 6269 6e64 7320  .* Volume binds 
+0000ddf0: 6361 6e20 6e6f 7720 616c 736f 2062 6520  can now also be 
+0000de00: 7370 6563 6966 6965 6420 6173 2061 206c  specified as a l
+0000de10: 6973 7420 6f66 2073 7472 696e 6773 2e0a  ist of strings..
+0000de20: 0a23 2323 2042 7567 6669 7865 730a 0a2a  .### Bugfixes..*
+0000de30: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+0000de40: 7265 2074 6865 2060 7265 6164 5f6f 6e6c  re the `read_onl
+0000de50: 7960 2070 6172 616d 2069 6e20 686f 7374  y` param in host
+0000de60: 5f63 6f6e 6669 6720 7761 736e 2774 2068  _config wasn't h
+0000de70: 616e 646c 6564 0a20 2070 726f 7065 726c  andled.  properl
+0000de80: 792e 0a2a 2046 6978 6564 2061 2062 7567  y..* Fixed a bug
+0000de90: 2069 6e20 6043 6c69 656e 742e 6578 6563   in `Client.exec
+0000dea0: 7574 6560 2028 7468 6973 206d 6574 686f  ute` (this metho
+0000deb0: 6420 6973 2073 7469 6c6c 2064 6570 7265  d is still depre
+0000dec0: 6361 7465 6429 2e0a 2a20 5468 6520 6063  cated)..* The `c
+0000ded0: 7075 7365 7460 2070 6172 616d 2069 6e20  puset` param in 
+0000dee0: 6043 6c69 656e 742e 6372 6561 7465 5f63  `Client.create_c
+0000def0: 6f6e 7461 696e 6572 6020 6973 2061 6c73  ontainer` is als
+0000df00: 6f20 7061 7373 6564 2061 730a 2020 7468  o passed as.  th
+0000df10: 6520 6043 7075 7365 7443 7075 7360 2070  e `CpusetCpus` p
+0000df20: 6172 616d 2028 6043 7075 7365 7460 2064  aram (`Cpuset` d
+0000df30: 6570 7265 6361 7465 6420 696e 2072 6563  eprecated in rec
+0000df40: 656e 7420 7665 7273 696f 6e73 206f 6620  ent versions of 
+0000df50: 7468 6520 4150 4929 0a2a 2046 6978 6564  the API).* Fixed
+0000df60: 2061 6e20 6973 7375 6520 7769 7468 2069   an issue with i
+0000df70: 6e74 6567 7261 7469 6f6e 2074 6573 7473  ntegration tests
+0000df80: 2062 6569 6e67 2072 756e 2069 6e73 6964   being run insid
+0000df90: 6520 6120 636f 6e74 6169 6e65 720a 2020  e a container.  
+0000dfa0: 2860 6d61 6b65 2069 6e74 6567 7261 7469  (`make integrati
+0000dfb0: 6f6e 2d74 6573 7460 290a 2a20 4669 7865  on-test`).* Fixe
+0000dfc0: 6420 6120 6275 6720 7768 6572 6520 616e  d a bug where an
+0000dfd0: 2065 6d70 7479 2073 7472 696e 6720 776f   empty string wo
+0000dfe0: 756c 6420 6265 2063 6f6e 7369 6465 7265  uld be considere
+0000dff0: 6420 6120 7661 6c69 6420 636f 6e74 6169  d a valid contai
+0000e000: 6e65 7220 4944 0a20 206f 7220 696d 6167  ner ID.  or imag
+0000e010: 6520 4944 2e0a 2a20 4669 7865 6420 6120  e ID..* Fixed a 
+0000e020: 6275 6720 696e 2060 436c 6965 6e74 2e69  bug in `Client.i
+0000e030: 6e73 6572 7460 0a0a 0a23 2323 2044 6f63  nsert`...### Doc
+0000e040: 756d 656e 7461 7469 6f6e 0a0a 2a20 5661  umentation..* Va
+0000e050: 7269 6f75 7320 6669 7865 730a 0a31 2e32  rious fixes..1.2
+0000e060: 2e32 0a2d 2d2d 2d2d 0a0a 2323 2320 4275  .2.-----..### Bu
+0000e070: 6766 6978 6573 0a0a 2a20 4669 7865 6420  gfixes..* Fixed 
+0000e080: 6120 6275 6720 7768 6572 6520 7061 7261  a bug where para
+0000e090: 6d65 7465 7273 2070 6173 7365 6420 746f  meters passed to
+0000e0a0: 2060 436c 6965 6e74 2e65 7865 635f 7265   `Client.exec_re
+0000e0b0: 7369 7a65 6020 776f 756c 6420 6265 2069  size` would be i
+0000e0c0: 676e 6f72 6564 2028 2335 3736 290a 2a20  gnored (#576).* 
+0000e0d0: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+0000e0e0: 6520 6175 7468 2063 6f6e 6669 6720 776f  e auth config wo
+0000e0f0: 756c 646e 2774 2062 6520 7265 736f 6c76  uldn't be resolv
+0000e100: 6564 2070 726f 7065 726c 7920 696e 2060  ed properly in `
+0000e110: 436c 6965 6e74 2e70 756c 6c60 2028 2335  Client.pull` (#5
+0000e120: 3737 290a 0a31 2e32 2e31 0a2d 2d2d 2d2d  77)..1.2.1.-----
+0000e130: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
+0000e140: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+0000e150: 6572 6520 7468 6520 6368 6563 6b5f 7265  ere the check_re
+0000e160: 736f 7572 6365 2064 6563 6f72 6174 6f72  source decorator
+0000e170: 2077 6f75 6c64 2062 7265 616b 2077 6974   would break wit
+0000e180: 6820 736f 6d65 0a20 2061 7267 756d 656e  h some.  argumen
+0000e190: 742d 7061 7373 696e 6720 6d65 7468 6f64  t-passing method
+0000e1a0: 732e 2028 2335 3733 290a 0a31 2e32 2e30  s. (#573)..1.2.0
+0000e1b0: 0a2d 2d2d 2d2d 0a0a 5b4c 6973 7420 6f66  .-----..[List of
+0000e1c0: 2050 5273 202f 2069 7373 7565 7320 666f   PRs / issues fo
+0000e1d0: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
+0000e1e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000e1f0: 6f6d 2f64 6f63 6b65 722f 646f 636b 6572  om/docker/docker
+0000e200: 2d70 792f 6973 7375 6573 3f71 3d6d 696c  -py/issues?q=mil
+0000e210: 6573 746f 6e65 2533 4131 2e32 2e30 2b69  estone%3A1.2.0+i
+0000e220: 7325 3341 636c 6f73 6564 290a 0a23 2323  s%3Aclosed)..###
+0000e230: 2044 6570 7265 6361 7469 6f6e 2077 6172   Deprecation war
+0000e240: 6e69 6e67 0a0a 2a20 6043 6c69 656e 742e  ning..* `Client.
+0000e250: 6578 6563 7574 6560 2069 7320 6265 696e  execute` is bein
+0000e260: 6720 6465 7072 6563 6174 6564 2069 6e20  g deprecated in 
+0000e270: 6661 766f 7220 6f66 2074 6865 206d 6f72  favor of the mor
+0000e280: 6520 6465 762d 6672 6965 6e64 6c79 0a20  e dev-friendly. 
+0000e290: 2060 436c 6965 6e74 2e65 7865 635f 7374   `Client.exec_st
+0000e2a0: 6172 7460 2061 6e64 2060 436c 6965 6e74  art` and `Client
+0000e2b0: 2e65 7865 635f 6372 6561 7465 602e 202a  .exec_create`. *
+0000e2c0: 2a49 7420 7769 6c6c 2062 6520 7265 6d6f  *It will be remo
+0000e2d0: 7665 6420 696e 2031 2e33 2e30 2a2a 0a0a  ved in 1.3.0**..
+0000e2e0: 2323 2320 4665 6174 7572 6573 0a0a 2a20  ### Features..* 
+0000e2f0: 4164 6465 6420 6065 7865 635f 6372 6561  Added `exec_crea
+0000e300: 7465 602c 2060 6578 6563 5f73 7461 7274  te`, `exec_start
+0000e310: 602c 2060 6578 6563 5f69 6e73 7065 6374  `, `exec_inspect
+0000e320: 6020 616e 6420 6065 7865 635f 7265 7369  ` and `exec_resi
+0000e330: 7a65 6020 746f 0a20 2063 6c69 656e 742c  ze` to.  client,
+0000e340: 2061 6363 7572 6174 656c 7920 6d69 7272   accurately mirr
+0000e350: 6f72 696e 6720 7468 650a 2020 5b45 7865  oring the.  [Exe
+0000e360: 6320 4150 495d 2868 7474 7073 3a2f 2f64  c API](https://d
+0000e370: 6f63 732e 646f 636b 6572 2e63 6f6d 2f72  ocs.docker.com/r
+0000e380: 6566 6572 656e 6365 2f61 7069 2f64 6f63  eference/api/doc
+0000e390: 6b65 725f 7265 6d6f 7465 5f61 7069 5f76  ker_remote_api_v
+0000e3a0: 312e 3138 2f23 6578 6563 2d63 7265 6174  1.18/#exec-creat
+0000e3b0: 6529 0a2a 2041 6464 6564 2060 6175 7468  e).* Added `auth
+0000e3c0: 5f63 6f6e 6669 6760 2070 6172 616d 2074  _config` param t
+0000e3d0: 6f20 6043 6c69 656e 742e 7075 6c6c 6020  o `Client.pull` 
+0000e3e0: 2861 6c6c 6f77 7320 746f 2075 7365 206f  (allows to use o
+0000e3f0: 6e65 2d6f 6666 2063 7265 6465 6e74 6961  ne-off credentia
+0000e400: 6c73 0a20 2066 6f72 2074 6869 7320 7075  ls.  for this pu
+0000e410: 6c6c 2072 6571 7565 7374 290a 2a20 4164  ll request).* Ad
+0000e420: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
+0000e430: 6069 7063 5f6d 6f64 6560 2069 6e20 686f  `ipc_mode` in ho
+0000e440: 7374 2063 6f6e 6669 672e 0a2a 2041 6464  st config..* Add
+0000e450: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
+0000e460: 6865 2060 6c6f 675f 636f 6e66 6967 6020  he `log_config` 
+0000e470: 7061 7261 6d20 696e 2068 6f73 7420 636f  param in host co
+0000e480: 6e66 6967 2e0a 2a20 4164 6465 6420 7375  nfig..* Added su
+0000e490: 7070 6f72 7420 666f 7220 7468 6520 6075  pport for the `u
+0000e4a0: 6c69 6d69 7460 2070 6172 616d 2069 6e20  limit` param in 
+0000e4b0: 686f 7374 2063 6f6e 6669 672e 0a2a 2041  host config..* A
+0000e4c0: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+0000e4d0: 2063 6f6e 7461 696e 6572 2072 6573 6f75   container resou
+0000e4e0: 7263 6520 6c69 6d69 7473 2069 6e20 6043  rce limits in `C
+0000e4f0: 6c69 656e 742e 6275 696c 6460 2e0a 2a20  lient.build`..* 
+0000e500: 5768 656e 2061 2072 6573 6f75 7263 6520  When a resource 
+0000e510: 6964 656e 7469 6669 6572 2028 696d 6167  identifier (imag
+0000e520: 6520 6f72 2063 6f6e 7461 696e 6572 2049  e or container I
+0000e530: 4429 2069 7320 7061 7373 6564 2074 6f20  D) is passed to 
+0000e540: 6120 436c 6965 6e74 0a20 206d 6574 686f  a Client.  metho
+0000e550: 642c 2077 6520 6e6f 7720 6368 6563 6b20  d, we now check 
+0000e560: 666f 7220 604e 6f6e 6560 2076 616c 7565  for `None` value
+0000e570: 7320 746f 2061 766f 6964 2063 7261 7368  s to avoid crash
+0000e580: 696e 670a 2020 286e 6f77 2072 6169 7365  ing.  (now raise
+0000e590: 7320 6064 6f63 6b65 722e 6572 726f 7273  s `docker.errors
+0000e5a0: 2e4e 756c 6c52 6573 6f75 7263 6560 290a  .NullResource`).
+0000e5b0: 2a20 4164 6465 6420 746f 6f6c 7320 746f  * Added tools to
+0000e5c0: 2070 6172 7365 2070 6f72 7420 7261 6e67   parse port rang
+0000e5d0: 6573 2069 6e73 6964 6520 7468 6520 6e65  es inside the ne
+0000e5e0: 7720 6064 6f63 6b65 722e 7574 696c 732e  w `docker.utils.
+0000e5f0: 706f 7274 7360 2070 6163 6b61 6765 2e0a  ports` package..
+0000e600: 2a20 4164 6465 6420 6120 6076 6572 7369  * Added a `versi
+0000e610: 6f6e 5f69 6e66 6f60 2061 7474 7269 6275  on_info` attribu
+0000e620: 7465 2074 6f20 7468 6520 6064 6f63 6b65  te to the `docke
+0000e630: 7260 2070 6163 6b61 6765 2e0a 0a23 2323  r` package...###
+0000e640: 2042 7567 6669 7865 730a 0a2a 2046 6978   Bugfixes..* Fix
+0000e650: 6564 2061 2062 7567 2069 6e20 6043 6c69  ed a bug in `Cli
+0000e660: 656e 742e 706f 7274 6020 7768 6572 6520  ent.port` where 
+0000e670: 6162 7365 6e63 6520 6f66 2061 2063 6572  absence of a cer
+0000e680: 7461 696e 206b 6579 2069 6e20 7468 650a  tain key in the.
+0000e690: 2020 636f 6e74 6169 6e65 7227 7320 4a53    container's JS
+0000e6a0: 4f4e 2077 6f75 6c64 2072 6169 7365 2061  ON would raise a
+0000e6b0: 6e20 6572 726f 7220 286e 6f77 206a 7573  n error (now jus
+0000e6c0: 7420 7265 7475 726e 7320 604e 6f6e 6560  t returns `None`
+0000e6d0: 290a 2a20 4669 7865 6420 6120 6275 6720  ).* Fixed a bug 
+0000e6e0: 7769 7468 2074 6865 2060 7472 756e 6360  with the `trunc`
+0000e6f0: 2070 6172 616d 6574 6572 2069 6e20 6043   parameter in `C
+0000e700: 6c69 656e 742e 636f 6e74 6169 6e65 7273  lient.containers
+0000e710: 6020 6861 7669 6e67 206e 6f0a 2020 6566  ` having no.  ef
+0000e720: 6665 6374 2028 6d6f 7665 6420 6675 6e63  fect (moved func
+0000e730: 7469 6f6e 616c 6974 7920 746f 2074 6865  tionality to the
+0000e740: 2063 6c69 656e 7429 0a2a 2053 6576 6572   client).* Sever
+0000e750: 616c 2069 6d70 726f 7665 6d65 6e74 7320  al improvements 
+0000e760: 6861 7665 2062 6565 6e20 6d61 6465 2074  have been made t
+0000e770: 6f20 7468 6520 6043 6c69 656e 742e 696d  o the `Client.im
+0000e780: 706f 7274 5f69 6d61 6765 6020 6d65 7468  port_image` meth
+0000e790: 6f64 2e0a 2a20 4669 7865 6420 7075 7368  od..* Fixed push
+0000e7a0: 696e 6720 2f20 7075 6c6c 696e 6720 746f  ing / pulling to
+0000e7b0: 0a20 205b 7632 2072 6567 6973 7472 6965  .  [v2 registrie
+0000e7c0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+0000e7d0: 622e 636f 6d2f 646f 636b 6572 2f64 6973  b.com/docker/dis
+0000e7e0: 7472 6962 7574 696f 6e29 0a2a 2046 6978  tribution).* Fix
+0000e7f0: 6564 2061 2062 7567 2077 6865 7265 2070  ed a bug where p
+0000e800: 6173 7369 6e67 2061 2063 6f6e 7461 696e  assing a contain
+0000e810: 6572 2064 6963 7469 6f6e 6172 7920 746f  er dictionary to
+0000e820: 2060 436c 6965 6e74 2e63 6f6d 6d69 7460   `Client.commit`
+0000e830: 0a20 2077 6f75 6c64 2066 6169 6c0a 0a23  .  would fail..#
+0000e840: 2323 204d 6973 6365 6c6c 616e 656f 7573  ## Miscellaneous
+0000e850: 0a0a 2a20 4465 6661 756c 7420 4150 4920  ..* Default API 
+0000e860: 7665 7273 696f 6e20 6861 7320 6265 656e  version has been
+0000e870: 2062 756d 7065 6420 746f 2031 2e31 3820   bumped to 1.18 
+0000e880: 2844 6f63 6b65 7220 456e 6769 6e65 2031  (Docker Engine 1
+0000e890: 2e36 2e30 290a 2a20 5365 7665 7261 6c20  .6.0).* Several 
+0000e8a0: 7465 7374 696e 6720 636f 7665 7261 6765  testing coverage
+0000e8b0: 2069 6d70 726f 7665 6d65 6e74 730a 2a20   improvements.* 
+0000e8c0: 446f 6373 2066 6978 6573 2061 6e64 2069  Docs fixes and i
+0000e8d0: 6d70 726f 7665 6d65 6e74 730a 0a31 2e31  mprovements..1.1
+0000e8e0: 2e30 0a2d 2d2d 2d2d 0a0a 2323 2320 4665  .0.-----..### Fe
+0000e8f0: 6174 7572 6573 0a0a 2a20 4164 6465 6420  atures..* Added 
+0000e900: 6064 6f63 6b65 7266 696c 6560 2070 6172  `dockerfile` par
+0000e910: 616d 2073 7570 706f 7274 2074 6f20 6043  am support to `C
+0000e920: 6c69 656e 742e 6275 696c 6460 2028 6d69  lient.build` (mi
+0000e930: 7272 6f72 730a 2020 6064 6f63 6b65 7220  rrors.  `docker 
+0000e940: 6275 696c 6420 2d66 6020 6265 6861 7669  build -f` behavi
+0000e950: 6f72 290a 2a20 4164 6465 6420 7468 6520  or).* Added the 
+0000e960: 6162 696c 6974 7920 746f 2073 7065 6369  ability to speci
+0000e970: 6679 2060 2761 7574 6f27 6020 6173 2060  fy `'auto'` as `
+0000e980: 7665 7273 696f 6e60 2069 6e20 6043 6c69  version` in `Cli
+0000e990: 656e 742e 5f5f 696e 6974 5f5f 602c 0a20  ent.__init__`,. 
+0000e9a0: 2061 6c6c 6f77 696e 6720 7468 6520 636f   allowing the co
+0000e9b0: 6e73 7472 7563 746f 7220 746f 2061 7574  nstructor to aut
+0000e9c0: 6f64 6574 6563 7420 7468 6520 6461 656d  odetect the daem
+0000e9d0: 6f6e 2773 2041 5049 2076 6572 7369 6f6e  on's API version
+0000e9e0: 2e0a 0a23 2323 2042 7567 6669 7865 730a  ...### Bugfixes.
+0000e9f0: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+0000ea00: 6865 7265 2064 6563 6f64 696e 6720 6120  here decoding a 
+0000ea10: 7265 7375 6c74 2073 7472 6561 6d20 7573  result stream us
+0000ea20: 696e 6720 7468 6520 6064 6563 6f64 6560  ing the `decode`
+0000ea30: 2070 6172 616d 6574 6572 0a20 2077 6f75   parameter.  wou
+0000ea40: 6c64 2062 7265 616b 2077 6865 6e20 7573  ld break when us
+0000ea50: 696e 6720 5079 7468 6f6e 2033 2e78 0a2a  ing Python 3.x.*
+0000ea60: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+0000ea70: 7265 2073 6f6d 6520 6669 6c65 7320 696e  re some files in
+0000ea80: 2060 2e64 6f63 6b65 7269 676e 6f72 6560   `.dockerignore`
+0000ea90: 2077 6572 656e 2774 2062 6569 6e67 2068   weren't being h
+0000eaa0: 616e 646c 6564 0a20 2070 726f 7065 726c  andled.  properl
+0000eab0: 790a 2a20 4669 7865 6420 6072 6573 6f6c  y.* Fixed `resol
+0000eac0: 7665 5f61 7574 6863 6f6e 6669 6760 2069  ve_authconfig` i
+0000ead0: 7373 7565 7320 6279 2062 7269 6e67 696e  ssues by bringin
+0000eae0: 6720 6974 2063 6c6f 7365 7220 746f 2044  g it closer to D
+0000eaf0: 6f63 6b65 7220 456e 6769 6e65 2773 0a20  ocker Engine's. 
+0000eb00: 2062 6568 6176 696f 722e 2054 6869 7320   behavior. This 
+0000eb10: 7368 6f75 6c64 2066 6978 2061 6c6c 2069  should fix all i
+0000eb20: 7373 7565 7320 656e 636f 756e 7465 7265  ssues encountere
+0000eb30: 6420 7769 7468 2070 7269 7661 7465 2072  d with private r
+0000eb40: 6567 6973 7472 7920 6175 7468 0a2a 2046  egistry auth.* F
+0000eb50: 6978 6564 2061 6e20 6973 7375 6520 7768  ixed an issue wh
+0000eb60: 6572 6520 7061 7373 776f 7264 7320 636f  ere passwords co
+0000eb70: 6e74 6169 6e69 6e67 2061 2063 6f6c 6f6e  ntaining a colon
+0000eb80: 2077 6572 656e 2774 2062 6569 6e67 2068   weren't being h
+0000eb90: 616e 646c 6564 0a20 2070 726f 7065 726c  andled.  properl
+0000eba0: 792e 0a2a 2042 756d 7065 6420 6072 6571  y..* Bumped `req
+0000ebb0: 7565 7374 7360 2076 6572 7369 6f6e 2072  uests` version r
+0000ebc0: 6571 7569 7265 6d65 6e74 2c20 7768 6963  equirement, whic
+0000ebd0: 6820 7368 6f75 6c64 2066 6978 206d 6f73  h should fix mos
+0000ebe0: 7420 6f66 2074 6865 2053 534c 0a20 2069  t of the SSL.  i
+0000ebf0: 7373 7565 7320 656e 636f 756e 7465 7265  ssues encountere
+0000ec00: 6420 7265 6365 6e74 6c79 2e0a 0a23 2323  d recently...###
+0000ec10: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
+0000ec20: 2a20 5365 7665 7261 6c20 696e 7465 6772  * Several integr
+0000ec30: 6174 696f 6e20 7465 7374 2069 6d70 726f  ation test impro
+0000ec40: 7665 6d65 6e74 732e 0a2a 2046 6978 6564  vements..* Fixed
+0000ec50: 2073 6f6d 6520 756e 636c 6f73 6564 2072   some unclosed r
+0000ec60: 6573 6f75 7263 6573 2069 6e20 756e 6974  esources in unit
+0000ec70: 2074 6573 7473 2e0a 2a20 5365 7665 7261   tests..* Severa
+0000ec80: 6c20 646f 6373 2069 6d70 726f 7665 6d65  l docs improveme
+0000ec90: 6e74 732e 0a0a 312e 302e 300a 2d2d 2d2d  nts...1.0.0.----
+0000eca0: 2d0a 0a23 2323 2046 6561 7475 7265 730a  -..### Features.
+0000ecb0: 0a2a 2041 6464 6564 206e 6577 2060 436c  .* Added new `Cl
+0000ecc0: 6965 6e74 2e72 656e 616d 6560 206d 6574  ient.rename` met
+0000ecd0: 686f 6420 2860 646f 636b 6572 2072 656e  hod (`docker ren
+0000ece0: 616d 6560 290a 2a20 4164 6465 6420 6e6f  ame`).* Added no
+0000ecf0: 7720 6043 6c69 656e 742e 7374 6174 7360  w `Client.stats`
+0000ed00: 206d 6574 686f 6420 2860 646f 636b 6572   method (`docker
+0000ed10: 2073 7461 7473 6029 0a2a 2041 6464 6564   stats`).* Added
+0000ed20: 2060 7265 6164 5f6f 6e6c 7960 2070 6172   `read_only` par
+0000ed30: 616d 2073 7570 706f 7274 2074 6f20 6075  am support to `u
+0000ed40: 7469 6c73 2e63 7265 6174 655f 686f 7374  tils.create_host
+0000ed50: 5f63 6f6e 6669 6760 2061 6e64 0a20 2060  _config` and.  `
+0000ed60: 436c 6965 6e74 2e73 7461 7274 6020 2860  Client.start` (`
+0000ed70: 646f 636b 6572 2072 756e 202d 2d72 6561  docker run --rea
+0000ed80: 642d 6f6e 6c79 6029 0a2a 2041 6464 6564  d-only`).* Added
+0000ed90: 2060 7069 645f 6d6f 6465 6020 7061 7261   `pid_mode` para
+0000eda0: 6d20 7375 7070 6f72 7420 746f 2060 7574  m support to `ut
+0000edb0: 696c 732e 6372 6561 7465 5f68 6f73 745f  ils.create_host_
+0000edc0: 636f 6e66 6967 6020 616e 640a 2020 6043  config` and.  `C
+0000edd0: 6c69 656e 742e 7374 6172 7460 2028 6064  lient.start` (`d
+0000ede0: 6f63 6b65 7220 7275 6e20 2d2d 7069 643d  ocker run --pid=
+0000edf0: 2768 6f73 7427 6029 0a2a 2041 6464 6564  'host'`).* Added
+0000ee00: 2060 7369 6e63 6560 2c20 6075 6e74 696c   `since`, `until
+0000ee10: 6020 616e 6420 6066 696c 7465 7273 6020  ` and `filters` 
+0000ee20: 7061 7261 6d73 2074 6f20 6043 6c69 656e  params to `Clien
+0000ee30: 742e 6576 656e 7473 602e 0a2a 2041 6464  t.events`..* Add
+0000ee40: 6564 2060 6465 636f 6465 6020 7061 7261  ed `decode` para
+0000ee50: 6d65 7465 7220 746f 2060 436c 6965 6e74  meter to `Client
+0000ee60: 2e73 7461 7473 6020 616e 6420 6043 6c69  .stats` and `Cli
+0000ee70: 656e 742e 6576 656e 7473 6020 746f 2064  ent.events` to d
+0000ee80: 6563 6f64 650a 2020 4a53 4f4e 206f 626a  ecode.  JSON obj
+0000ee90: 6563 7473 206f 6e20 7468 6520 666c 7920  ects on the fly 
+0000eea0: 2846 616c 7365 2062 7920 6465 6661 756c  (False by defaul
+0000eeb0: 7429 2e0a 0a23 2323 2042 7567 6669 7865  t)...### Bugfixe
+0000eec0: 730a 0a2a 2046 6978 6564 2061 2062 7567  s..* Fixed a bug
+0000eed0: 2074 6861 7420 6361 7573 6564 2060 436c   that caused `Cl
+0000eee0: 6965 6e74 2e62 7569 6c64 6020 746f 2063  ient.build` to c
+0000eef0: 7261 7368 2077 6865 6e20 7468 6520 7072  rash when the pr
+0000ef00: 6f76 6964 6564 2073 6f75 7263 6520 7761  ovided source wa
+0000ef10: 730a 2020 6120 7265 6d6f 7465 2073 6f75  s.  a remote sou
+0000ef20: 7263 652e 0a0a 2323 2320 4d69 7363 656c  rce...### Miscel
+0000ef30: 6c61 6e65 6f75 730a 0a2a 2044 6566 6175  laneous..* Defau
+0000ef40: 6c74 2041 5049 2076 6572 7369 6f6e 2068  lt API version h
+0000ef50: 6173 2062 6565 6e20 6275 6d70 6564 2074  as been bumped t
+0000ef60: 6f20 312e 3137 2028 446f 636b 6572 2045  o 1.17 (Docker E
+0000ef70: 6e67 696e 6520 312e 352e 3029 0a2a 2060  ngine 1.5.0).* `
+0000ef80: 436c 6965 6e74 2e74 696d 656f 7574 6020  Client.timeout` 
+0000ef90: 6973 206e 6f77 2061 2070 7562 6c69 6320  is now a public 
+0000efa0: 6174 7472 6962 7574 652c 2061 6e64 2075  attribute, and u
+0000efb0: 7365 7273 2061 7265 2065 6e63 6f75 7261  sers are encoura
+0000efc0: 6765 6420 746f 2075 7365 2069 740a 2020  ged to use it.  
+0000efd0: 7768 656e 2072 6571 7565 7374 2074 696d  when request tim
+0000efe0: 656f 7574 7320 6e65 6564 2074 6f20 6265  eouts need to be
+0000eff0: 2063 6861 6e67 6564 2061 7420 7275 6e74   changed at runt
+0000f000: 696d 652e 0a2a 2041 6464 6564 2060 436c  ime..* Added `Cl
+0000f010: 6965 6e74 2e61 7069 5f76 6572 7369 6f6e  ient.api_version
+0000f020: 6020 6173 2061 2072 6561 642d 6f6e 6c79  ` as a read-only
+0000f030: 2070 726f 7065 7274 792e 0a2a 2054 6865   property..* The
+0000f040: 2060 6d65 6d73 7761 705f 6c69 6d69 7460   `memswap_limit`
+0000f050: 2061 7267 756d 656e 7420 696e 2060 436c   argument in `Cl
+0000f060: 6965 6e74 2e63 7265 6174 655f 636f 6e74  ient.create_cont
+0000f070: 6169 6e65 7260 206e 6f77 2061 6363 6570  ainer` now accep
+0000f080: 7473 2073 7472 696e 670a 2020 7479 7065  ts string.  type
+0000f090: 2076 616c 7565 7320 7369 6d69 6c61 7220   values similar 
+0000f0a0: 746f 2060 6d65 6d5f 6c69 6d69 7460 2028  to `mem_limit` (
+0000f0b0: 2736 6727 2c20 2731 3230 3030 306b 272c  '6g', '120000k',
+0000f0c0: 2065 7463 2e29 0a2a 2049 6d70 726f 7665   etc.).* Improve
+0000f0d0: 6420 646f 6375 6d65 6e74 6174 696f 6e0a  d documentation.
+0000f0e0: 0a30 2e37 2e32 0a2d 2d2d 2d2d 0a0a 2323  .0.7.2.-----..##
+0000f0f0: 2320 4665 6174 7572 6573 0a0a 2a20 4164  # Features..* Ad
+0000f100: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
+0000f110: 606d 6163 5f61 6464 7265 7373 6020 696e  `mac_address` in
+0000f120: 2060 436c 6965 6e74 2e63 7265 6174 655f   `Client.create_
+0000f130: 636f 6e74 6169 6e65 7260 0a0a 2323 2320  container`..### 
+0000f140: 4275 6766 6978 6573 0a0a 2a20 4669 7865  Bugfixes..* Fixe
+0000f150: 6420 6120 6275 6720 7768 6572 6520 7374  d a bug where st
+0000f160: 7265 616d 696e 6720 7265 7370 6f6e 7365  reaming response
+0000f170: 7320 2860 7075 6c6c 602c 2060 7075 7368  s (`pull`, `push
+0000f180: 602c 2060 6c6f 6773 602c 2065 7463 2e29  `, `logs`, etc.)
+0000f190: 2077 6572 650a 2020 756e 7265 6c69 6162   were.  unreliab
+0000f1a0: 6c65 2028 2333 3030 290a 2a20 4669 7865  le (#300).* Fixe
+0000f1b0: 6420 6120 6275 6720 7768 6572 6520 7265  d a bug where re
+0000f1c0: 736f 6c76 655f 6175 7468 636f 6e66 6967  solve_authconfig
+0000f1d0: 2077 6f75 6c64 6e27 7420 7072 6f70 6572   wouldn't proper
+0000f1e0: 6c79 2072 6573 6f6c 7665 2063 6f6e 6669  ly resolve confi
+0000f1f0: 6775 7261 7469 6f6e 0a20 2066 6f72 2070  guration.  for p
+0000f200: 7269 7661 7465 2072 6570 6f73 6974 6f72  rivate repositor
+0000f210: 6965 7320 2823 3436 3829 0a2a 2046 6978  ies (#468).* Fix
+0000f220: 6564 2061 2062 7567 2077 6865 7265 2073  ed a bug where s
+0000f230: 6f6d 6520 6572 726f 7273 2077 6f75 6c64  ome errors would
+0000f240: 6e27 7420 6265 2070 726f 7065 726c 7920  n't be properly 
+0000f250: 636f 6e73 7472 7563 7465 6420 696e 0a20  constructed in. 
+0000f260: 2060 636c 6965 6e74 2e70 7960 2c20 6c65   `client.py`, le
+0000f270: 6164 696e 6720 746f 2075 6e68 656c 7066  ading to unhelpf
+0000f280: 756c 2065 7863 6570 7469 6f6e 7320 6275  ul exceptions bu
+0000f290: 6262 6c69 6e67 2075 7020 2823 3436 3629  bbling up (#466)
+0000f2a0: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+0000f2b0: 6865 7265 2060 436c 6965 6e74 2e62 7569  here `Client.bui
+0000f2c0: 6c64 6020 776f 756c 6420 7472 7920 746f  ld` would try to
+0000f2d0: 2063 6c6f 7365 2063 6f6e 7465 7874 2077   close context w
+0000f2e0: 6865 6e20 6578 7465 726e 616c 6c79 0a20  hen externally. 
+0000f2f0: 2070 726f 7669 6465 6420 2860 6375 7374   provided (`cust
+0000f300: 6f6d 5f63 6f6e 7465 7874 203d 3d20 5472  om_context == Tr
+0000f310: 7565 6029 2028 2334 3538 290a 2a20 4669  ue`) (#458).* Fi
+0000f320: 7865 6420 616e 2069 7373 7565 2069 6e20  xed an issue in 
+0000f330: 6063 7265 6174 655f 686f 7374 5f63 6f6e  `create_host_con
+0000f340: 6669 6760 2077 6865 7265 2065 6d70 7479  fig` where empty
+0000f350: 2073 6571 7565 6e63 6573 2077 6f75 6c64   sequences would
+0000f360: 6e27 7420 6265 0a20 2069 6e74 6572 7072  n't be.  interpr
+0000f370: 6574 6564 2070 726f 7065 726c 7920 2823  eted properly (#
+0000f380: 3436 3229 0a0a 2323 2320 4d69 7363 656c  462)..### Miscel
+0000f390: 6c61 6e65 6f75 730a 0a2a 2041 6464 6564  laneous..* Added
+0000f3a0: 2060 7265 736f 6c76 655f 6175 7468 636f   `resolve_authco
+0000f3b0: 6e66 6967 6020 7465 7374 732e 0a0a 302e  nfig` tests...0.
+0000f3c0: 372e 310a 2d2d 2d2d 2d0a 0a23 2323 2042  7.1.-----..### B
+0000f3d0: 7567 6669 7865 730a 0a2a 2060 7365 7475  ugfixes..* `setu
+0000f3e0: 702e 7079 6020 6e6f 7720 696e 6469 6361  p.py` now indica
+0000f3f0: 7465 7320 6120 6d61 7869 6d75 6d20 7665  tes a maximum ve
+0000f400: 7273 696f 6e20 6f66 2072 6571 7565 7374  rsion of request
+0000f410: 7320 746f 2077 6f72 6b20 6172 6f75 6e64  s to work around
+0000f420: 2074 6865 0a20 2062 6f6f 7432 646f 636b   the.  boot2dock
+0000f430: 6572 202f 2060 6173 7365 7274 5f68 6f73  er / `assert_hos
+0000f440: 746e 616d 6560 2062 7567 2e0a 2a20 5265  tname` bug..* Re
+0000f450: 6d6f 7665 6420 696e 7661 6c69 6420 6578  moved invalid ex
+0000f460: 6365 7074 696f 6e20 7768 656e 2075 7369  ception when usi
+0000f470: 6e67 2074 6865 2052 6567 6973 7472 7920  ng the Registry 
+0000f480: 4875 6227 7320 4651 444e 2077 6865 6e20  Hub's FQDN when 
+0000f490: 7075 6c6c 696e 672e 0a2a 2046 6978 6564  pulling..* Fixed
+0000f4a0: 2061 6e20 6973 7375 6520 7768 6572 6520   an issue where 
+0000f4b0: 6561 726c 7920 4854 5450 2065 7272 6f72  early HTTP error
+0000f4c0: 7320 7765 7265 6e27 7420 6861 6e64 6c65  s weren't handle
+0000f4d0: 6420 7072 6f70 6572 6c79 2069 6e20 7374  d properly in st
+0000f4e0: 7265 616d 696e 670a 2020 7265 7370 6f6e  reaming.  respon
+0000f4f0: 7365 732e 0a2a 2046 6978 6564 2061 2062  ses..* Fixed a b
+0000f500: 7567 2077 6865 7265 2073 6f63 6b65 7473  ug where sockets
+0000f510: 2077 6f75 6c64 2063 6c6f 7365 2075 6e65   would close une
+0000f520: 7870 6563 7465 646c 7920 7573 696e 6720  xpectedly using 
+0000f530: 5079 7468 6f6e 2033 2e78 0a2a 2056 6172  Python 3.x.* Var
+0000f540: 696f 7573 2066 6978 6573 2066 6f72 2069  ious fixes for i
+0000f550: 6e74 6567 7261 7469 6f6e 2074 6573 7473  ntegration tests
+0000f560: 2e0a 0a23 2323 204d 6973 6365 6c6c 616e  ...### Miscellan
+0000f570: 656f 7573 0a0a 2a20 536d 616c 6c20 646f  eous..* Small do
+0000f580: 6320 6669 7865 730a 0a30 2e37 2e30 0a2d  c fixes..0.7.0.-
+0000f590: 2d2d 2d2d 0a0a 2323 2320 4272 6561 6b69  ----..### Breaki
+0000f5a0: 6e67 2063 6861 6e67 6573 0a0a 2a20 5061  ng changes..* Pa
+0000f5b0: 7373 696e 6720 6064 6e73 6020 6f72 2060  ssing `dns` or `
+0000f5c0: 766f 6c75 6d65 735f 6672 6f6d 6020 696e  volumes_from` in
+0000f5d0: 2060 436c 6965 6e74 2e73 7461 7274 6020   `Client.start` 
+0000f5e0: 7769 7468 2041 5049 2076 6572 7369 6f6e  with API version
+0000f5f0: 203c 2031 2e31 300a 2020 7769 6c6c 206e   < 1.10.  will n
+0000f600: 6f77 2072 6169 7365 2061 6e20 6578 6365  ow raise an exce
+0000f610: 7074 696f 6e20 2870 7265 7669 6f75 736c  ption (previousl
+0000f620: 7920 6f6e 6c79 2074 7269 6767 6572 6564  y only triggered
+0000f630: 2061 2077 6172 6e69 6e67 290a 0a23 2323   a warning)..###
+0000f640: 2046 6561 7475 7265 730a 0a2a 2041 6464   Features..* Add
+0000f650: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
+0000f660: 686f 7374 5f63 6f6e 6669 6760 2069 6e20  host_config` in 
+0000f670: 6043 6c69 656e 742e 6372 6561 7465 5f63  `Client.create_c
+0000f680: 6f6e 7461 696e 6572 600a 2a20 4164 6465  ontainer`.* Adde
+0000f690: 6420 7574 696c 6974 7920 6d65 7468 6f64  d utility method
+0000f6a0: 2060 646f 636b 6572 2e75 7469 6c73 2e63   `docker.utils.c
+0000f6b0: 7265 6174 655f 686f 7374 5f63 6f6e 6669  reate_host_confi
+0000f6c0: 6760 2074 6f20 6865 6c70 2062 7569 6c64  g` to help build
+0000f6d0: 2061 0a20 2070 726f 7065 7220 6048 6f73   a.  proper `Hos
+0000f6e0: 7443 6f6e 6669 6760 2064 6963 7469 6f6e  tConfig` diction
+0000f6f0: 6172 792e 0a2a 2041 6464 6564 2073 7570  ary..* Added sup
+0000f700: 706f 7274 2066 6f72 2074 6865 2060 7075  port for the `pu
+0000f710: 6c6c 6020 7061 7261 6d65 7465 7220 696e  ll` parameter in
+0000f720: 2060 436c 6965 6e74 2e62 7569 6c64 600a   `Client.build`.
+0000f730: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+0000f740: 666f 7220 7468 6520 6066 6f72 6365 726d  for the `forcerm
+0000f750: 6020 7061 7261 6d65 7465 7220 696e 2060  ` parameter in `
+0000f760: 436c 6965 6e74 2e62 7569 6c64 600a 2a20  Client.build`.* 
+0000f770: 4164 6465 6420 7375 7070 6f72 7420 666f  Added support fo
+0000f780: 7220 6065 7874 7261 5f68 6f73 7473 6020  r `extra_hosts` 
+0000f790: 696e 2060 436c 6965 6e74 2e73 7461 7274  in `Client.start
+0000f7a0: 600a 2a20 4164 6465 6420 7375 7070 6f72  `.* Added suppor
+0000f7b0: 7420 666f 7220 6120 6375 7374 6f6d 2060  t for a custom `
+0000f7c0: 7469 6d65 6f75 7460 2069 6e20 6043 6c69  timeout` in `Cli
+0000f7d0: 656e 742e 7761 6974 600a 2a20 4164 6465  ent.wait`.* Adde
+0000f7e0: 6420 7375 7070 6f72 7420 666f 7220 6375  d support for cu
+0000f7f0: 7374 6f6d 2060 2e64 6f63 6b65 7263 6667  stom `.dockercfg
+0000f800: 6020 6c6f 6164 696e 6720 696e 2060 436c  ` loading in `Cl
+0000f810: 6965 6e74 2e6c 6f67 696e 600a 2020 2860  ient.login`.  (`
+0000f820: 646f 636b 6572 6366 675f 7061 7468 6020  dockercfg_path` 
+0000f830: 6172 6775 6d65 6e74 290a 0a23 2323 2042  argument)..### B
+0000f840: 7567 6669 7865 730a 0a2a 2046 6978 6564  ugfixes..* Fixed
+0000f850: 2061 2062 7567 2077 6865 7265 2073 6f6d   a bug where som
+0000f860: 6520 6f75 7470 7574 2077 6f75 6c64 6e27  e output wouldn'
+0000f870: 7420 6265 2073 7472 6561 6d65 6420 7072  t be streamed pr
+0000f880: 6f70 6572 6c79 2069 6e20 7374 7265 616d  operly in stream
+0000f890: 696e 670a 2020 6368 756e 6b65 6420 7265  ing.  chunked re
+0000f8a0: 7370 6f6e 7365 730a 2a20 4669 7865 6420  sponses.* Fixed 
+0000f8b0: 6120 6275 6720 7768 6572 6520 7468 6520  a bug where the 
+0000f8c0: 6064 6576 6963 6573 6020 7061 7261 6d20  `devices` param 
+0000f8d0: 6469 646e 2774 2072 6563 6f67 6e69 7a65  didn't recognize
+0000f8e0: 2074 6865 2070 726f 7065 7220 6465 6c69   the proper deli
+0000f8f0: 6d69 7465 720a 2a20 6043 6c69 656e 742e  miter.* `Client.
+0000f900: 6c6f 6769 6e60 206e 6f77 2070 726f 7065  login` now prope
+0000f910: 726c 7920 6578 7061 6e64 7320 7468 6520  rly expands the 
+0000f920: 6072 6567 6973 7472 7960 2055 524c 2069  `registry` URL i
+0000f930: 6620 7072 6f76 6964 6564 2e0a 2a20 4669  f provided..* Fi
+0000f940: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
+0000f950: 756e 6963 6f64 6520 6368 6172 6163 7465  unicode characte
+0000f960: 7273 2069 6e20 7061 7373 6564 2066 6f72  rs in passed for
+0000f970: 2060 656e 7669 726f 6e6d 656e 7460 2069   `environment` i
+0000f980: 6e0a 2020 6063 7265 6174 655f 636f 6e74  n.  `create_cont
+0000f990: 6169 6e65 7260 2077 6f75 6c64 2062 7265  ainer` would bre
+0000f9a0: 616b 2e0a 0a23 2323 204d 6973 6365 6c6c  ak...### Miscell
+0000f9b0: 616e 656f 7573 0a0a 2a20 5365 7665 7261  aneous..* Severa
+0000f9c0: 6c20 756e 6974 2074 6573 7473 2061 6e64  l unit tests and
+0000f9d0: 2069 6e74 6567 7261 7469 6f6e 2074 6573   integration tes
+0000f9e0: 7473 2069 6d70 726f 7665 6d65 6e74 732e  ts improvements.
+0000f9f0: 0a2a 2060 436c 6965 6e74 6020 636f 6e73  .* `Client` cons
+0000fa00: 7472 7563 746f 7220 6e6f 7720 656e 666f  tructor now enfo
+0000fa10: 7263 6573 2070 6173 7369 6e67 2074 6865  rces passing the
+0000fa20: 2060 7665 7273 696f 6e60 2070 6172 616d   `version` param
+0000fa30: 6574 6572 2061 7320 610a 2020 7374 7269  eter as a.  stri
+0000fa40: 6e67 2e0a 2a20 4275 696c 6420 636f 6e74  ng..* Build cont
+0000fa50: 6578 7420 6669 6c65 7320 6172 6520 6e6f  ext files are no
+0000fa60: 7720 6f72 6465 7265 6420 6279 2066 696c  w ordered by fil
+0000fa70: 656e 616d 6520 7768 656e 2063 7265 6174  ename when creat
+0000fa80: 696e 6720 7468 6520 6172 6368 6976 650a  ing the archive.
+0000fa90: 2020 2866 6f72 2063 6f6e 7369 7374 656e    (for consisten
+0000faa0: 6379 2077 6974 6820 646f 636b 6572 206d  cy with docker m
+0000fab0: 6169 6e6c 696e 6520 6265 6861 7669 6f72  ainline behavior
+0000fac0: 290a 0a30 2e36 2e30 0a2d 2d2d 2d2d 0a2a  )..0.6.0.-----.*
+0000fad0: 202a 2a54 6869 7320 7665 7273 696f 6e20   **This version 
+0000fae0: 696e 7472 6f64 7563 6573 2062 7265 616b  introduces break
+0000faf0: 696e 6720 6368 616e 6765 7321 2a2a 0a0a  ing changes!**..
+0000fb00: 2323 2320 4272 6561 6b69 6e67 2063 6861  ### Breaking cha
+0000fb10: 6e67 6573 0a0a 2a20 5468 6520 6465 6661  nges..* The defa
+0000fb20: 756c 7420 5353 4c20 7072 6f74 6f63 6f6c  ult SSL protocol
+0000fb30: 2069 7320 6e6f 7720 7468 6520 6869 6768   is now the high
+0000fb40: 6573 7420 544c 5320 7631 2e78 2028 7761  est TLS v1.x (wa
+0000fb50: 7320 5353 4c20 7632 2e33 2062 6566 6f72  s SSL v2.3 befor
+0000fb60: 6529 0a20 2028 506f 6f64 6c65 2066 6978  e).  (Poodle fix
+0000fb70: 290a 2a20 5468 6520 6068 6973 746f 7279  ).* The `history
+0000fb80: 6020 636f 6d6d 616e 6420 6e6f 7720 7265  ` command now re
+0000fb90: 7475 726e 7320 6120 6469 6374 2069 6e73  turns a dict ins
+0000fba0: 7465 6164 206f 6620 6120 7261 7720 4a53  tead of a raw JS
+0000fbb0: 4f4e 2073 7472 696e 672e 0a0a 2323 2320  ON string...### 
+0000fbc0: 4665 6174 7572 6573 0a0a 2a20 4164 6465  Features..* Adde
+0000fbd0: 6420 7468 6520 6065 7865 6375 7465 6020  d the `execute` 
+0000fbe0: 636f 6d6d 616e 642e 0a2a 2041 6464 6564  command..* Added
+0000fbf0: 2060 7061 7573 6560 2061 6e64 2060 756e   `pause` and `un
+0000fc00: 7061 7573 6560 2063 6f6d 6d61 6e64 732e  pause` commands.
+0000fc10: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+0000fc20: 2066 6f20 7468 6520 6063 7075 7365 7460   fo the `cpuset`
+0000fc30: 2070 6172 616d 2069 6e20 6063 7265 6174   param in `creat
+0000fc40: 655f 636f 6e74 6169 6e65 7260 0a2a 2041  e_container`.* A
+0000fc50: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+0000fc60: 2068 6f73 7420 6465 7669 6365 7320 2860   host devices (`
+0000fc70: 6465 7669 6365 7360 2070 6172 616d 2069  devices` param i
+0000fc80: 6e20 6073 7461 7274 6029 0a2a 2041 6464  n `start`).* Add
+0000fc90: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
+0000fca0: 6865 2060 7461 696c 6020 7061 7261 6d20  he `tail` param 
+0000fcb0: 696e 2060 6c6f 6773 602e 0a2a 2041 6464  in `logs`..* Add
+0000fcc0: 6564 2073 7570 706f 7274 2066 6f72 2074  ed support for t
+0000fcd0: 6865 2060 6669 6c74 6572 7360 2070 6172  he `filters` par
+0000fce0: 616d 2069 6e20 6069 6d61 6765 7360 2061  am in `images` a
+0000fcf0: 6e64 2060 636f 6e74 6169 6e65 7273 600a  nd `containers`.
+0000fd00: 2a20 5468 6520 606b 7761 7267 735f 6672  * The `kwargs_fr
+0000fd10: 6f6d 5f65 6e76 6020 6d65 7468 6f64 2069  om_env` method i
+0000fd20: 7320 6e6f 7720 6176 6169 6c61 626c 6520  s now available 
+0000fd30: 696e 2074 6865 2060 646f 636b 6572 2e75  in the `docker.u
+0000fd40: 7469 6c73 600a 2020 6d6f 6475 6c65 2e20  tils`.  module. 
+0000fd50: 5468 6973 2073 686f 756c 6420 6d61 6b65  This should make
+0000fd60: 2069 7420 6561 7369 6572 2066 6f72 2062   it easier for b
+0000fd70: 6f6f 7432 646f 636b 6572 2075 7365 7220  oot2docker user 
+0000fd80: 746f 2063 6f6e 6e65 6374 0a20 2074 6f20  to connect.  to 
+0000fd90: 7468 6569 7220 6461 656d 6f6e 2e0a 0a23  their daemon...#
+0000fda0: 2323 2042 7567 6669 7865 730a 0a2a 2046  ## Bugfixes..* F
+0000fdb0: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+0000fdc0: 2065 6d70 7479 2064 6972 6563 746f 7269   empty directori
+0000fdd0: 6573 2077 6572 656e 2774 2063 6f72 7265  es weren't corre
+0000fde0: 6374 6c79 2069 6e63 6c75 6465 6420 7768  ctly included wh
+0000fdf0: 656e 0a20 2070 726f 7669 6469 6e67 2061  en.  providing a
+0000fe00: 2063 6f6e 7465 7874 2074 6f20 6043 6c69   context to `Cli
+0000fe10: 656e 742e 6275 696c 6460 2e0a 2a20 4669  ent.build`..* Fi
+0000fe20: 7865 6420 6120 6275 6720 7768 6572 6520  xed a bug where 
+0000fe30: 554e 4958 2073 6f63 6b65 7420 636f 6e6e  UNIX socket conn
+0000fe40: 6563 7469 6f6e 7320 7765 7265 6e27 7420  ections weren't 
+0000fe50: 7072 6f70 6572 6c79 2063 6c65 616e 6564  properly cleaned
+0000fe60: 2075 702c 0a20 2063 6175 7369 6e67 2060   up,.  causing `
+0000fe70: 5265 736f 7572 6365 5761 726e 696e 6760  ResourceWarning`
+0000fe80: 7320 746f 2061 7070 6561 7220 696e 2073  s to appear in s
+0000fe90: 6f6d 6520 6361 7365 732e 0a2a 2046 6978  ome cases..* Fix
+0000fea0: 6564 2061 2062 7567 2077 6865 7265 2064  ed a bug where d
+0000feb0: 6f63 6b65 722d 7079 2077 6f75 6c64 2063  ocker-py would c
+0000fec0: 7261 7368 2069 6620 7468 6520 646f 636b  rash if the dock
+0000fed0: 6572 2064 6165 6d6f 6e20 7761 7320 7374  er daemon was st
+0000fee0: 6f70 7065 640a 2020 7768 696c 6520 7265  opped.  while re
+0000fef0: 6164 696e 6720 6120 7374 7265 616d 696e  ading a streamin
+0000ff00: 6720 7265 7370 6f6e 7365 0a2a 2046 6978  g response.* Fix
+0000ff10: 6564 2061 2062 7567 2077 6974 6820 7374  ed a bug with st
+0000ff20: 7265 616d 696e 6720 7265 7370 6f6e 7365  reaming response
+0000ff30: 7320 696e 2050 7974 686f 6e20 330a 2a20  s in Python 3.* 
+0000ff40: 6072 656d 6f76 655f 696d 6167 6560 206e  `remove_image` n
+0000ff50: 6f77 2073 7570 706f 7274 7320 6120 6469  ow supports a di
+0000ff60: 6374 2063 6f6e 7461 696e 696e 6720 616e  ct containing an
+0000ff70: 2060 4964 6020 6b65 7920 6173 2069 7473   `Id` key as its
+0000ff80: 2060 6964 600a 2020 7061 7261 6d65 7465   `id`.  paramete
+0000ff90: 7220 2873 696d 696c 6172 2074 6f20 6f74  r (similar to ot
+0000ffa0: 6865 7220 6d65 7468 6f64 7320 7265 7175  her methods requ
+0000ffb0: 6972 696e 6720 6120 7265 736f 7572 6365  iring a resource
+0000ffc0: 2049 4429 0a0a 2323 2320 446f 6375 6d65   ID)..### Docume
+0000ffd0: 6e74 6174 696f 6e0a 0a2a 2041 6464 6564  ntation..* Added
+0000ffe0: 206e 6577 204d 6b44 6f63 7320 646f 6375   new MkDocs docu
+0000fff0: 6d65 6e74 6174 696f 6e2e 2043 7572 7265  mentation. Curre
+00010000: 6e74 6c79 2068 6f73 7465 6420 6f6e 0a20  ntly hosted on. 
+00010010: 205b 5265 6164 5468 6544 6f63 735d 2868   [ReadTheDocs](h
+00010020: 7474 7073 3a2f 2f64 6f63 6b65 722d 7079  ttps://docker-py
+00010030: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00010040: 656e 2f6c 6174 6573 742f 290a 0a23 2323  en/latest/)..###
+00010050: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
+00010060: 2a20 4164 6465 6420 7465 7374 7320 746f  * Added tests to
+00010070: 2073 6469 7374 0a2a 2041 6464 6564 2061   sdist.* Added a
+00010080: 204d 616b 6566 696c 6520 666f 7220 7275   Makefile for ru
+00010090: 6e6e 696e 6720 7465 7374 7320 696e 2044  nning tests in D
+000100a0: 6f63 6b65 720a 2a20 5570 6461 7465 6420  ocker.* Updated 
+000100b0: 446f 636b 6572 6669 6c65 0a0a 302e 352e  Dockerfile..0.5.
+000100c0: 330a 2d2d 2d2d 2d0a 0a2a 2046 6978 6564  3.-----..* Fixed
+000100d0: 2061 7474 6163 6869 6e67 2077 6865 6e20   attaching when 
+000100e0: 636f 6e6e 6563 7469 6e67 2074 6f20 7468  connecting to th
+000100f0: 6520 6461 656d 6f6e 206f 7665 7220 6120  e daemon over a 
+00010100: 554e 4958 2073 6f63 6b65 742e 0a0a 302e  UNIX socket...0.
+00010110: 352e 320a 2d2d 2d2d 2d0a 0a2a 2046 6978  5.2.-----..* Fix
+00010120: 6564 2061 2062 7567 2077 6865 7265 2073  ed a bug where s
+00010130: 6f63 6b65 7473 2077 6572 6520 636c 6f73  ockets were clos
+00010140: 6564 2069 6d6d 6564 6961 7465 6c79 2077  ed immediately w
+00010150: 6865 6e20 6174 7461 6368 696e 6720 6f76  hen attaching ov
+00010160: 6572 0a20 2054 4c53 2e0a 0a30 2e35 2e31  er.  TLS...0.5.1
+00010170: 0a2d 2d2d 2d2d 0a0a 2a20 4164 6465 6420  .-----..* Added 
+00010180: 6120 6061 7373 6572 745f 686f 7374 6e61  a `assert_hostna
+00010190: 6d65 6020 6f70 7469 6f6e 2074 6f20 6054  me` option to `T
+000101a0: 4c53 436f 6e66 6967 6020 7768 6963 6820  LSConfig` which 
+000101b0: 6361 6e20 6265 2075 7365 6420 746f 0a20  can be used to. 
+000101c0: 2064 6973 6162 6c65 2076 6572 6966 6963   disable verific
+000101d0: 6174 696f 6e20 6f66 2068 6f73 746e 616d  ation of hostnam
+000101e0: 6573 2e0a 2a20 4669 7865 6420 5353 4c20  es..* Fixed SSL 
+000101f0: 6e6f 7420 776f 726b 696e 6720 6475 6520  not working due 
+00010200: 746f 2061 6e20 696e 636f 7272 6563 7420  to an incorrect 
+00010210: 7665 7273 696f 6e20 636f 6d70 6172 6973  version comparis
+00010220: 6f6e 0a2a 2046 6978 6564 2073 7472 6561  on.* Fixed strea
+00010230: 6d73 206e 6f74 2077 6f72 6b69 6e67 206f  ms not working o
+00010240: 6e20 5769 6e64 6f77 730a 0a30 2e35 2e30  n Windows..0.5.0
+00010250: 0a2d 2d2d 2d2d 0a0a 2a20 2a2a 5468 6973  .-----..* **This
+00010260: 2076 6572 7369 6f6e 2069 6e74 726f 6475   version introdu
+00010270: 6365 7320 6272 6561 6b69 6e67 2063 6861  ces breaking cha
+00010280: 6e67 6573 212a 2a0a 2a20 4164 6465 6420  nges!**.* Added 
+00010290: 6069 6e73 6563 7572 655f 7265 6769 7374  `insecure_regist
+000102a0: 7279 6020 7061 7261 6d65 7465 7220 696e  ry` parameter in
+000102b0: 2060 436c 6965 6e74 2e70 7573 6860 2061   `Client.push` a
+000102c0: 6e64 2060 436c 6965 6e74 2e70 756c 6c60  nd `Client.pull`
+000102d0: 2e0a 2020 2a49 7420 6465 6661 756c 7473  ..  *It defaults
+000102e0: 2074 6f20 4661 6c73 6520 616e 6420 636f   to False and co
+000102f0: 6465 2070 7573 6869 6e67 2074 6f20 6e6f  de pushing to no
+00010300: 6e2d 4854 5450 5320 7072 6976 6174 6520  n-HTTPS private 
+00010310: 7265 6769 7374 7269 6573 0a20 206d 6967  registries.  mig
+00010320: 6874 2062 7265 616b 2061 7320 6120 7265  ht break as a re
+00010330: 7375 6c74 2e2a 0a2a 2041 6464 6564 2073  sult.*.* Added s
+00010340: 7570 706f 7274 2066 6f72 2061 6464 696e  upport for addin
+00010350: 6720 616e 6420 6472 6f70 7069 6e67 2063  g and dropping c
+00010360: 6170 6162 696c 6974 6965 730a 2a20 4164  apabilities.* Ad
+00010370: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
+00010380: 7265 7374 6172 7420 706f 6c69 6379 0a2a  restart policy.*
+00010390: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
+000103a0: 6f72 2073 7472 696e 6720 7661 6c75 6573  or string values
+000103b0: 2069 6e20 6043 6c69 656e 742e 6372 6561   in `Client.crea
+000103c0: 7465 5f63 6f6e 7461 696e 6572 6027 7320  te_container`'s 
+000103d0: 606d 656d 5f6c 696d 6974 600a 2a20 4164  `mem_limit`.* Ad
+000103e0: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
+000103f0: 602e 646f 636b 6572 6967 6e6f 7265 6020  `.dockerignore` 
+00010400: 6669 6c65 2069 6e20 6043 6c69 656e 742e  file in `Client.
+00010410: 6275 696c 6460 0a0a 2323 2320 4275 6766  build`..### Bugf
+00010420: 6978 6573 0a0a 2a20 4669 7865 6420 7469  ixes..* Fixed ti
+00010430: 6d65 6f75 7420 6265 6861 7669 6f72 2069  meout behavior i
+00010440: 6e20 6043 6c69 656e 742e 7374 6f70 600a  n `Client.stop`.
+00010450: 0a23 2323 204d 6973 6365 6c6c 616e 656f  .### Miscellaneo
+00010460: 7573 0a0a 2a20 6043 6c69 656e 742e 6372  us..* `Client.cr
+00010470: 6561 7465 5f63 6f6e 7461 696e 6572 6020  eate_container` 
+00010480: 7072 6f76 6964 6573 2062 6574 7465 7220  provides better 
+00010490: 7661 6c69 6461 7469 6f6e 206f 6620 7468  validation of th
+000104a0: 6520 6076 6f6c 756d 6573 600a 2020 7061  e `volumes`.  pa
+000104b0: 7261 6d65 7465 720a 2a20 496d 7072 6f76  rameter.* Improv
+000104c0: 6564 2069 6e74 6567 7261 7469 6f6e 2074  ed integration t
+000104d0: 6573 7473 0a0a 302e 342e 300a 2d2d 2d2d  ests..0.4.0.----
+000104e0: 2d0a 0a2a 202a 2a54 6869 7320 7665 7273  -..* **This vers
+000104f0: 696f 6e20 696e 7472 6f64 7563 6573 2062  ion introduces b
+00010500: 7265 616b 696e 6720 6368 616e 6765 7321  reaking changes!
+00010510: 2a2a 0a2a 2054 6865 2060 6261 7365 5f75  **.* The `base_u
+00010520: 726c 6020 7061 7261 6d65 7465 7220 696e  rl` parameter in
+00010530: 2074 6865 2060 436c 6965 6e74 6020 636f   the `Client` co
+00010540: 6e73 7472 7563 746f 7220 7368 6f75 6c64  nstructor should
+00010550: 206e 6f77 2061 6c6c 6f77 206d 6f73 740a   now allow most.
+00010560: 2020 6f66 2074 6865 2060 444f 434b 4552    of the `DOCKER
+00010570: 5f48 4f53 5460 2065 6e76 6972 6f6e 6d65  _HOST` environme
+00010580: 6e74 2076 616c 7565 7320 2865 7863 6570  nt values (excep
+00010590: 7420 666f 7220 7468 6520 6664 3a2f 2f20  t for the fd:// 
+000105a0: 7072 6f74 6f63 6f6c 290a 2020 2020 2a20  protocol).    * 
+000105b0: 4173 2061 2072 6573 756c 742c 2055 524c  As a result, URL
+000105c0: 7320 7468 6174 2064 6f6e 2774 2073 7065  s that don't spe
+000105d0: 6369 6679 2061 2070 6f72 7420 6172 6520  cify a port are 
+000105e0: 6e6f 7720 696e 7661 6c69 6420 2873 696d  now invalid (sim
+000105f0: 696c 6172 0a20 2020 2074 6f20 7468 6520  ilar.    to the 
+00010600: 6f66 6669 6369 616c 2063 6c69 656e 7427  official client'
+00010610: 7320 6265 6861 7669 6f72 290a 2a20 4164  s behavior).* Ad
+00010620: 6465 6420 544c 5320 7375 7070 6f72 7420  ded TLS support 
+00010630: 2873 6565 205b 646f 6375 6d65 6e74 6174  (see [documentat
+00010640: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
+00010650: 6875 622e 636f 6d2f 646f 7463 6c6f 7564  hub.com/dotcloud
+00010660: 2f64 6f63 6b65 722d 7079 2363 6f6e 6e65  /docker-py#conne
+00010670: 6374 696f 6e2d 746f 2d64 6165 6d6f 6e2d  ction-to-daemon-
+00010680: 7573 696e 672d 6874 7470 7329 290a 0a23  using-https))..#
+00010690: 2323 2042 7567 6669 7865 730a 0a2a 2046  ## Bugfixes..* F
+000106a0: 6978 6564 2061 6e20 6973 7375 6520 7769  ixed an issue wi
+000106b0: 7468 2060 436c 6965 6e74 2e62 7569 6c64  th `Client.build
+000106c0: 6020 7374 7265 616d 6564 206c 6f67 7320  ` streamed logs 
+000106d0: 696e 2050 7974 686f 6e20 330a 0a23 2323  in Python 3..###
+000106e0: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
+000106f0: 2a20 4164 6465 6420 756e 6974 2074 6573  * Added unit tes
+00010700: 7473 2063 6f76 6572 6167 650a 2a20 5661  ts coverage.* Va
+00010710: 7269 6f75 7320 696e 7465 6772 6174 696f  rious integratio
+00010720: 6e20 7465 7374 7320 6669 7865 730a 0a30  n tests fixes..0
+00010730: 2e33 2e32 0a2d 2d2d 2d2d 0a0a 2a20 4465  .3.2.-----..* De
+00010740: 6661 756c 7420 4150 4920 7665 7273 696f  fault API versio
+00010750: 6e20 6973 206e 6f77 2031 2e31 3220 2873  n is now 1.12 (s
+00010760: 7570 706f 7274 2066 6f72 2064 6f63 6b65  upport for docke
+00010770: 7220 312e 3029 0a2a 2041 6464 6564 206e  r 1.0).* Added n
+00010780: 6577 206d 6574 686f 6473 2060 436c 6965  ew methods `Clie
+00010790: 6e74 2e67 6574 5f69 6d61 6765 6020 616e  nt.get_image` an
+000107a0: 6420 6043 6c69 656e 742e 6c6f 6164 5f69  d `Client.load_i
+000107b0: 6d61 6765 600a 2020 2860 646f 636b 6572  mage`.  (`docker
+000107c0: 2073 6176 6560 2061 6e64 2060 646f 636b   save` and `dock
+000107d0: 6572 206c 6f61 6460 290a 2a20 4164 6465  er load`).* Adde
+000107e0: 6420 6e65 7720 6d65 7468 6f64 2060 436c  d new method `Cl
+000107f0: 6965 6e74 2e70 696e 6760 0a2a 2041 6464  ient.ping`.* Add
+00010800: 6564 206e 6577 206d 6574 686f 6420 6043  ed new method `C
+00010810: 6c69 656e 742e 7265 7369 7a65 600a 2a20  lient.resize`.* 
+00010820: 6043 6c69 656e 742e 6275 696c 6460 2063  `Client.build` c
+00010830: 616e 206e 6f77 2062 6520 7072 6f76 6964  an now be provid
+00010840: 6564 2077 6974 6820 6120 6375 7374 6f6d  ed with a custom
+00010850: 2063 6f6e 7465 7874 2075 7369 6e67 2074   context using t
+00010860: 6865 0a20 2060 6375 7374 6f6d 5f63 6f6e  he.  `custom_con
+00010870: 7465 7874 6020 7061 7261 6d65 7465 722e  text` parameter.
+00010880: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00010890: 2066 6f72 2060 6d65 6d73 7761 705f 6c69   for `memswap_li
+000108a0: 6d69 7460 2070 6172 616d 6574 6572 2069  mit` parameter i
+000108b0: 6e20 6063 7265 6174 655f 636f 6e74 6169  n `create_contai
+000108c0: 6e65 7260 0a2a 2041 6464 6564 2073 7570  ner`.* Added sup
+000108d0: 706f 7274 2066 6f72 2060 666f 7263 6560  port for `force`
+000108e0: 2070 6172 616d 6574 6572 2069 6e20 6072   parameter in `r
+000108f0: 656d 6f76 655f 636f 6e74 6169 6e65 7260  emove_container`
+00010900: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00010910: 2066 6f72 2060 666f 7263 6560 2061 6e64   for `force` and
+00010920: 2060 6e6f 7072 756e 6560 2070 6172 616d   `noprune` param
+00010930: 6574 6572 7320 696e 2060 7265 6d6f 7665  eters in `remove
+00010940: 5f69 6d61 6765 600a 2a20 4164 6465 6420  _image`.* Added 
+00010950: 7375 7070 6f72 7420 666f 7220 6074 696d  support for `tim
+00010960: 6573 7461 6d70 7360 2070 6172 616d 6574  estamps` paramet
+00010970: 6572 2069 6e20 606c 6f67 7360 0a2a 2041  er in `logs`.* A
+00010980: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+00010990: 2060 646e 735f 7365 6172 6368 6020 7061   `dns_search` pa
+000109a0: 7261 6d65 7465 7220 696e 2060 7374 6172  rameter in `star
+000109b0: 7460 0a2a 2041 6464 6564 2073 7570 706f  t`.* Added suppo
+000109c0: 7274 2066 6f72 2060 6e65 7477 6f72 6b5f  rt for `network_
+000109d0: 6d6f 6465 6020 7061 7261 6d65 7465 7220  mode` parameter 
+000109e0: 696e 2060 7374 6172 7460 0a2a 2041 6464  in `start`.* Add
+000109f0: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
+00010a00: 7369 7a65 6020 7061 7261 6d65 7465 7220  size` parameter 
+00010a10: 696e 2060 636f 6e74 6169 6e65 7273 600a  in `containers`.
+00010a20: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+00010a30: 666f 7220 6076 6f6c 756d 6573 5f66 726f  for `volumes_fro
+00010a40: 6d60 2061 6e64 2060 646e 7360 2070 6172  m` and `dns` par
+00010a50: 616d 6574 6572 7320 696e 2060 7374 6172  ameters in `star
+00010a60: 7460 2e20 4173 206f 660a 2020 4150 4920  t`. As of.  API 
+00010a70: 7665 7273 696f 6e20 3e3d 2031 2e31 302c  version >= 1.10,
+00010a80: 2074 6865 7365 2070 6172 616d 6574 6572   these parameter
+00010a90: 7320 6e6f 206c 6f6e 6765 7220 6265 6c6f  s no longer belo
+00010aa0: 6e67 2074 6f20 6063 7265 6174 655f 636f  ng to `create_co
+00010ab0: 6e74 6169 6e65 7260 0a2a 2060 436c 6965  ntainer`.* `Clie
+00010ac0: 6e74 2e6c 6f67 7360 206e 6f77 2075 7365  nt.logs` now use
+00010ad0: 7320 7468 6520 6c6f 6773 2065 6e64 706f  s the logs endpo
+00010ae0: 696e 7420 7768 656e 2041 5049 2076 6572  int when API ver
+00010af0: 7369 6f6e 2069 7320 7375 6666 6963 6965  sion is sufficie
+00010b00: 6e74 0a0a 2323 2320 4275 6766 6978 6573  nt..### Bugfixes
+00010b10: 0a0a 2a20 4669 7865 6420 6120 6275 6720  ..* Fixed a bug 
+00010b20: 696e 2070 756c 6c20 7768 6572 6520 7468  in pull where th
+00010b30: 6520 6072 6570 6f3a 7461 6760 206e 6f74  e `repo:tag` not
+00010b40: 6174 696f 6e20 7761 736e 2774 2069 6e74  ation wasn't int
+00010b50: 6572 7072 6574 6564 0a20 2070 726f 7065  erpreted.  prope
+00010b60: 726c 790a 2a20 4669 7865 6420 6120 6275  rly.* Fixed a bu
+00010b70: 6720 696e 2073 7472 6561 6d69 6e67 206d  g in streaming m
+00010b80: 6574 686f 6473 2077 6974 6820 7079 7468  ethods with pyth
+00010b90: 6f6e 2033 2028 756e 6963 6f64 652c 2062  on 3 (unicode, b
+00010ba0: 7974 6573 2f73 7472 2072 656c 6174 6564  ytes/str related
+00010bb0: 290a 2a20 4669 7865 6420 6120 6275 6720  ).* Fixed a bug 
+00010bc0: 696e 2060 436c 6965 6e74 2e73 7461 7274  in `Client.start
+00010bd0: 6020 7768 6572 6520 6c65 6761 6379 206e  ` where legacy n
+00010be0: 6f74 6174 696f 6e20 666f 7220 766f 6c75  otation for volu
+00010bf0: 6d65 7320 7761 736e 2774 0a20 2073 7570  mes wasn't.  sup
+00010c00: 706f 7274 6564 2061 6e79 6d6f 7265 2e0a  ported anymore..
+00010c10: 0a23 2323 204d 6973 6365 6c6c 616e 656f  .### Miscellaneo
+00010c20: 7573 0a0a 2a20 5468 6520 636c 6965 6e74  us..* The client
+00010c30: 206e 6f77 2072 6169 7365 7320 6044 6f63   now raises `Doc
+00010c40: 6b65 7245 7863 6570 7469 6f6e 6073 2077  kerException`s w
+00010c50: 6865 6e20 6170 7072 6f70 7269 6174 652e  hen appropriate.
+00010c60: 2059 6f75 2063 616e 2069 6d70 6f72 740a   You can import.
+00010c70: 2020 6044 6f63 6b65 7245 7863 6570 7469    `DockerExcepti
+00010c80: 6f6e 6020 2861 6e64 2069 7473 2073 7562  on` (and its sub
+00010c90: 636c 6173 7365 7329 2066 726f 6d20 7468  classes) from th
+00010ca0: 6520 6064 6f63 6b65 722e 6572 726f 7273  e `docker.errors
+00010cb0: 6020 6d6f 6475 6c65 2074 6f0a 2020 6361  ` module to.  ca
+00010cc0: 7463 6820 7468 656d 2069 6620 6e65 6564  tch them if need
+00010cd0: 6564 2e0a 2a20 6064 6f63 6b65 722e 4150  ed..* `docker.AP
+00010ce0: 4945 7272 6f72 6020 6861 7320 6265 656e  IError` has been
+00010cf0: 206d 6f76 6564 2074 6f20 7468 6520 6e65   moved to the ne
+00010d00: 7720 6064 6f63 6b65 722e 6572 726f 7273  w `docker.errors
+00010d10: 6020 6d6f 6475 6c65 2061 7320 7765 6c6c  ` module as well
+00010d20: 2e0a 2a20 6043 6c69 656e 742e 696e 7365  ..* `Client.inse
+00010d30: 7274 6020 6973 2064 6570 7265 6361 7465  rt` is deprecate
+00010d40: 6420 696e 2041 5049 2076 6572 7369 6f6e  d in API version
+00010d50: 203e 2031 2e31 310a 2a20 496d 7072 6f76   > 1.11.* Improv
+00010d60: 6564 2069 6e74 6567 7261 7469 6f6e 2074  ed integration t
+00010d70: 6573 7473 2073 686f 756c 6420 6e6f 7720  ests should now 
+00010d80: 7275 6e20 6d75 6368 2066 6173 7465 722e  run much faster.
+00010d90: 0a2a 2054 6865 7265 2069 7320 6e6f 7720  .* There is now 
+00010da0: 6120 7369 6e67 6c65 2073 6f75 7263 6520  a single source 
+00010db0: 6f66 2074 7275 7468 2066 6f72 2074 6865  of truth for the
+00010dc0: 2064 6f63 6b65 722d 7079 2076 6572 7369   docker-py versi
+00010dd0: 6f6e 206e 756d 6265 722e 0a0a 302e 332e  on number...0.3.
+00010de0: 310a 2d2d 2d2d 2d0a 0a2a 2044 6566 6175  1.-----..* Defau
+00010df0: 6c74 2041 5049 2076 6572 7369 6f6e 2069  lt API version i
+00010e00: 7320 6e6f 7720 312e 390a 2a20 5374 7265  s now 1.9.* Stre
+00010e10: 616d 696e 6720 7265 7370 6f6e 7365 7320  aming responses 
+00010e20: 6e6f 206c 6f6e 6765 7220 7969 656c 6420  no longer yield 
+00010e30: 626c 616e 6b20 6c69 6e65 732e 0a2a 2060  blank lines..* `
+00010e40: 436c 6965 6e74 2e63 7265 6174 655f 636f  Client.create_co
+00010e50: 6e74 6169 6e65 7260 206e 6f77 2073 7570  ntainer` now sup
+00010e60: 706f 7274 7320 7468 6520 6064 6f6d 6169  ports the `domai
+00010e70: 6e6e 616d 6560 2070 6172 616d 6574 6572  nname` parameter
+00010e80: 2e0a 2a20 6076 6f6c 756d 6573 5f66 726f  ..* `volumes_fro
+00010e90: 6d60 2070 6172 616d 6574 6572 2069 6e20  m` parameter in 
+00010ea0: 6043 6c69 656e 742e 6372 6561 7465 5f63  `Client.create_c
+00010eb0: 6f6e 7461 696e 6572 6020 6e6f 7720 7375  ontainer` now su
+00010ec0: 7070 6f72 7473 0a20 2069 7465 7261 626c  pports.  iterabl
+00010ed0: 6573 2e0a 2a20 4175 7468 2063 7265 6465  es..* Auth crede
+00010ee0: 6e74 6961 6c73 2061 7265 2070 726f 7669  ntials are provi
+00010ef0: 6465 6420 746f 2074 6865 2064 6f63 6b65  ded to the docke
+00010f00: 7220 6461 656d 6f6e 2077 6865 6e20 7573  r daemon when us
+00010f10: 696e 6720 6043 6c69 656e 742e 6275 696c  ing `Client.buil
+00010f20: 6460 0a20 2028 6e65 7720 6665 6174 7572  d`.  (new featur
+00010f30: 6520 696e 2041 5049 2076 6572 7369 6f6e  e in API version
+00010f40: 2031 2e39 290a 0a0a 2323 2320 4275 6766   1.9)...### Bugf
+00010f50: 6978 6573 0a0a 2a20 5661 7269 6f75 7320  ixes..* Various 
+00010f60: 6669 7865 7320 666f 7220 7265 7370 6f6e  fixes for respon
+00010f70: 7365 2073 7472 6561 6d73 2028 606c 6f67  se streams (`log
+00010f80: 7360 2c20 6070 756c 6c60 2c20 6574 632e  s`, `pull`, etc.
+00010f90: 292e 0a2a 2046 6978 6564 2061 2062 7567  )..* Fixed a bug
+00010fa0: 2077 6974 6820 6043 6c69 656e 742e 7075   with `Client.pu
+00010fb0: 7368 6020 7768 656e 2075 7369 6e67 2041  sh` when using A
+00010fc0: 5049 2076 6572 7369 6f6e 203c 2031 2e35  PI version < 1.5
+00010fd0: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00010fe0: 6974 6820 4150 4920 7665 7273 696f 6e20  ith API version 
+00010ff0: 6368 6563 6b73 2e0a 0a23 2323 204d 6973  checks...### Mis
+00011000: 6365 6c6c 616e 656f 7573 0a0a 2a20 606d  cellaneous..* `m
+00011010: 6f63 6b60 2068 6173 2062 6565 6e20 7265  ock` has been re
+00011020: 6d6f 7665 6420 6672 6f6d 2074 6865 2072  moved from the r
+00011030: 756e 7469 6d65 2072 6571 7569 7265 6d65  untime requireme
+00011040: 6e74 732e 0a2a 2041 6464 6564 2069 6e73  nts..* Added ins
+00011050: 7461 6c6c 6174 696f 6e20 696e 7374 7275  tallation instru
+00011060: 6374 696f 6e73 2069 6e20 7468 6520 5245  ctions in the RE
+00011070: 4144 4d45 2e0a 0a30 2e33 2e30 0a2d 2d2d  ADME...0.3.0.---
+00011080: 2d2d 0a0a 2a20 2a2a 5468 6973 2076 6572  --..* **This ver
+00011090: 7369 6f6e 2069 6e74 726f 6475 6365 7320  sion introduces 
+000110a0: 6272 6561 6b69 6e67 2063 6861 6e67 6573  breaking changes
+000110b0: 212a 2a0a 2a20 5375 7070 6f72 7420 666f  !**.* Support fo
+000110c0: 7220 4150 4920 7665 7273 696f 6e20 312e  r API version 1.
+000110d0: 3720 7468 726f 7567 6820 312e 3920 2844  7 through 1.9 (D
+000110e0: 6f63 6b65 7220 302e 382e 302b 290a 2a20  ocker 0.8.0+).* 
+000110f0: 4465 6661 756c 7420 4150 4920 7665 7273  Default API vers
+00011100: 696f 6e20 6973 206e 6f77 2031 2e38 0a2a  ion is now 1.8.*
+00011110: 2054 6865 2063 6c69 656e 7420 6861 7320   The client has 
+00011120: 6265 656e 2075 7064 6174 6564 2074 6f20  been updated to 
+00011130: 7375 7070 6f72 7420 5265 7175 6573 7473  support Requests
+00011140: 2032 2e78 2e20 6072 6571 7565 7374 733d   2.x. `requests=
+00011150: 3d32 2e32 2e31 600a 2020 6973 206e 6f77  =2.2.1`.  is now
+00011160: 2074 6865 2072 6563 6f6d 6d65 6e64 6564   the recommended
+00011170: 2076 6572 7369 6f6e 2e0a 2a20 4c69 6e6b   version..* Link
+00011180: 7320 6361 6e20 6e6f 7720 6265 2073 7065  s can now be spe
+00011190: 6369 6669 6564 2061 7320 7475 706c 6573  cified as tuples
+000111a0: 2069 6e20 6043 6c69 656e 742e 7374 6172   in `Client.star
+000111b0: 7460 2028 7365 6520 646f 6373 2066 6f72  t` (see docs for
+000111c0: 0a20 206d 6f72 6520 696e 666f 726d 6174  .  more informat
+000111d0: 696f 6e29 0a2a 2041 6464 6564 2073 7570  ion).* Added sup
+000111e0: 706f 7274 2066 6f72 2076 6172 696f 7573  port for various
+000111f0: 206f 7074 696f 6e73 2069 6e20 6043 6c69   options in `Cli
+00011200: 656e 742e 6372 6561 7465 5f63 6f6e 7461  ent.create_conta
+00011210: 696e 6572 600a 2020 2860 6e65 7477 6f72  iner`.  (`networ
+00011220: 6b5f 6469 7361 626c 6564 602c 2060 6370  k_disabled`, `cp
+00011230: 755f 7368 6172 6573 602c 2060 776f 726b  u_shares`, `work
+00011240: 696e 675f 6469 7260 2061 6e64 2060 656e  ing_dir` and `en
+00011250: 7472 7970 6f69 6e74 6029 0a2a 2060 436c  trypoint`).* `Cl
+00011260: 6965 6e74 2e61 7474 6163 6860 2068 6173  ient.attach` has
+00011270: 2062 6565 6e20 7265 776f 726b 6564 2074   been reworked t
+00011280: 6f20 776f 726b 2073 696d 696c 6172 6c79  o work similarly
+00011290: 2074 6f20 6043 6c69 656e 742e 6c6f 6773   to `Client.logs
+000112a0: 600a 2020 6d69 6e75 7320 7468 6520 6869  `.  minus the hi
+000112b0: 7374 6f72 6963 616c 2064 6174 612e 0a2a  storical data..*
+000112c0: 204c 6f67 7320 6361 6e20 6e6f 7720 6265   Logs can now be
+000112d0: 2073 7472 6561 6d65 6420 7573 696e 6720   streamed using 
+000112e0: 7468 6520 6073 7472 6561 6d60 2070 6172  the `stream` par
+000112f0: 616d 6574 6572 2e0a 2a20 4164 6465 6420  ameter..* Added 
+00011300: 7375 7070 6f72 7420 666f 7220 6074 6370  support for `tcp
+00011310: 3a2f 2f60 2055 524c 7320 6173 2063 6c69  ://` URLs as cli
+00011320: 656e 7420 6062 6173 655f 7572 6c60 2e0a  ent `base_url`..
+00011330: 2a20 5661 7269 6f75 7320 6175 7468 2069  * Various auth i
+00011340: 6d70 726f 7665 6d65 6e74 732e 0a2a 2041  mprovements..* A
+00011350: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+00011360: 2063 7573 746f 6d20 6043 6c69 656e 742e   custom `Client.
+00011370: 6275 696c 6460 2074 696d 656f 7574 2e0a  build` timeout..
+00011380: 0a0a 2323 2320 4275 6766 6978 6573 0a0a  ..### Bugfixes..
+00011390: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+000113a0: 6572 6520 6465 7465 726d 696e 696e 6720  ere determining 
+000113b0: 7468 6520 7072 6f74 6f63 6f6c 206f 6620  the protocol of 
+000113c0: 6120 7072 6976 6174 6520 7265 6769 7374  a private regist
+000113d0: 7279 0a20 2077 6f75 6c64 2073 6f6d 6574  ry.  would somet
+000113e0: 696d 6573 2079 6965 6c64 2074 6865 2077  imes yield the w
+000113f0: 726f 6e67 2072 6573 756c 742e 0a2a 2046  rong result..* F
+00011400: 6978 6564 2061 2062 7567 2077 6865 7265  ixed a bug where
+00011410: 2060 436c 6965 6e74 2e63 6f70 7960 2077   `Client.copy` w
+00011420: 6f75 6c64 6e27 7420 6163 6365 7074 2061  ouldn't accept a
+00011430: 2064 6963 7420 6173 2061 7267 756d 656e   dict as argumen
+00011440: 742e 0a2a 2046 6978 6564 2073 6576 6572  t..* Fixed sever
+00011450: 616c 2073 7472 6561 6d69 6e67 2062 7567  al streaming bug
+00011460: 732e 0a2a 2052 656d 6f76 6564 2075 6e75  s..* Removed unu
+00011470: 7365 6420 7061 7261 6d65 7465 7220 696e  sed parameter in
+00011480: 2060 436c 6965 6e74 2e69 6d70 6f72 745f   `Client.import_
+00011490: 696d 6167 6560 2e0a 2a20 5468 6520 636c  image`..* The cl
+000114a0: 6965 6e74 2773 2060 6261 7365 5f75 726c  ient's `base_url
+000114b0: 6020 6e6f 7720 746f 6c65 7261 7465 7320  ` now tolerates 
+000114c0: 7472 6169 6c69 6e67 2073 6c61 7368 6573  trailing slashes
+000114d0: 2e0a 0a23 2323 2320 4d69 7363 656c 6c61  ...#### Miscella
+000114e0: 6e65 6f75 730a 0a2a 2055 7064 6174 6564  neous..* Updated
+000114f0: 2069 6e74 6567 7261 7469 6f6e 2074 6573   integration tes
+00011500: 7473 0a2a 2053 6d61 6c6c 2064 6f63 2066  ts.* Small doc f
+00011510: 6978 6573 0a0a 302e 322e 330a 2d2d 2d2d  ixes..0.2.3.----
+00011520: 2d0a 0a2a 2053 7570 706f 7274 2066 6f72  -..* Support for
+00011530: 2041 5049 2076 6572 7369 6f6e 2031 2e36   API version 1.6
+00011540: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00011550: 2066 6f72 206c 696e 6b73 0a2a 2041 6464   for links.* Add
+00011560: 6564 2073 7570 706f 7274 2066 6f72 2067  ed support for g
+00011570: 6c6f 6261 6c20 7265 7175 6573 7420 7469  lobal request ti
+00011580: 6d65 6f75 740a 2a20 4164 6465 6420 6073  meout.* Added `s
+00011590: 6967 6e61 6c60 2070 6172 616d 6574 6572  ignal` parameter
+000115a0: 2069 6e20 6043 6c69 656e 742e 6b69 6c6c   in `Client.kill
+000115b0: 600a 2a20 4164 6465 6420 7375 7070 6f72  `.* Added suppor
+000115c0: 7420 666f 7220 6070 7562 6c69 7368 5f61  t for `publish_a
+000115d0: 6c6c 5f70 6f72 7473 6020 696e 2060 436c  ll_ports` in `Cl
+000115e0: 6965 6e74 2e73 7461 7274 600a 2a20 6043  ient.start`.* `C
+000115f0: 6c69 656e 742e 7075 6c6c 602c 2060 436c  lient.pull`, `Cl
+00011600: 6965 6e74 2e70 7573 6860 2061 6e64 2060  ient.push` and `
+00011610: 436c 6965 6e74 2e62 7569 6c64 6020 6361  Client.build` ca
+00011620: 6e20 6265 2073 7472 6561 6d65 6420 6e6f  n be streamed no
+00011630: 770a 2a20 4164 6465 6420 7375 7070 6f72  w.* Added suppor
+00011640: 7420 666f 7220 7765 6273 6f63 6b65 7473  t for websockets
+00011650: 2069 6e20 6043 6c69 656e 742e 6174 7461   in `Client.atta
+00011660: 6368 600a 2a20 4669 7865 6420 706f 7274  ch`.* Fixed port
+00011670: 7320 666f 7220 446f 636b 6572 2030 2e36  s for Docker 0.6
+00011680: 2e35 2b0a 2a20 4164 6465 6420 6043 6c69  .5+.* Added `Cli
+00011690: 656e 742e 6576 656e 7473 6020 6d65 7468  ent.events` meth
+000116a0: 6f64 2028 6163 6365 7373 2074 6f20 7468  od (access to th
+000116b0: 6520 602f 6576 656e 7473 6020 656e 6470  e `/events` endp
+000116c0: 6f69 6e74 290a 2a20 4368 616e 6765 6420  oint).* Changed 
+000116d0: 7468 6520 7761 7920 7468 6520 706f 7274  the way the port
+000116e0: 7320 616e 6420 766f 6c75 6d65 7320 6172  s and volumes ar
+000116f0: 6520 7072 6f76 6964 6564 2069 6e20 6043  e provided in `C
+00011700: 6c69 656e 742e 7374 6172 7460 2061 6e64  lient.start` and
+00011710: 0a20 2060 436c 6965 6e74 2e63 7265 6174  .  `Client.creat
+00011720: 655f 636f 6e74 6169 6e65 72cc 8060 2074  e_container..` t
+00011730: 6f20 6d61 6b65 2074 6865 6d20 7369 6d70  o make them simp
+00011740: 6c65 7220 616e 6420 6d6f 7265 2069 6e74  ler and more int
+00011750: 7569 7469 7665 2e0a 0a23 2323 2042 7567  uitive...### Bug
+00011760: 6669 7865 730a 0a2a 2046 6978 6564 2061  fixes..* Fixed a
+00011770: 2062 7567 2077 6865 7265 2070 7269 7661   bug where priva
+00011780: 7465 2072 6567 6973 7472 6965 7320 6f6e  te registries on
+00011790: 2048 5454 5053 2077 6572 656e 2774 2068   HTTPS weren't h
+000117a0: 616e 646c 6564 2070 726f 7065 726c 790a  andled properly.
+000117b0: 2a20 4669 7865 6420 6120 6275 6720 7768  * Fixed a bug wh
+000117c0: 6572 6520 6175 7468 2077 6f75 6c64 2062  ere auth would b
+000117d0: 7265 616b 2077 6974 6820 5079 7468 6f6e  reak with Python
+000117e0: 2033 0a0a 2323 2320 4d69 7363 656c 6c61   3..### Miscella
+000117f0: 6e65 6f75 730a 0a2a 2054 6573 7420 696d  neous..* Test im
+00011800: 7072 6f76 656d 656e 7473 0a2a 2053 6c69  provements.* Sli
+00011810: 6768 7420 646f 6320 696d 7072 6f76 656d  ght doc improvem
+00011820: 656e 7473 0a0a 0a30 2e32 2e32 0a2d 2d2d  ents...0.2.2.---
+00011830: 2d2d 0a0a 2a20 4164 6465 6420 7375 7070  --..* Added supp
+00011840: 6f72 7420 666f 7220 7468 6520 6072 6d60  ort for the `rm`
+00011850: 2070 6172 616d 6574 6572 2069 6e20 6043   parameter in `C
+00011860: 6c69 656e 742e 6275 696c 6460 0a2a 2041  lient.build`.* A
+00011870: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+00011880: 2074 6172 6261 6c6c 2069 6d70 6f72 7473   tarball imports
+00011890: 2069 6e20 6043 6c69 656e 742e 696d 706f   in `Client.impo
+000118a0: 7274 5f69 6d61 6765 6020 7468 726f 7567  rt_image` throug
+000118b0: 6820 6064 6174 6160 0a20 2070 6172 616d  h `data`.  param
+000118c0: 6574 6572 2e0a 2a20 5468 6520 6063 6f6d  eter..* The `com
+000118d0: 6d61 6e64 6020 7061 7261 6d65 7465 7220  mand` parameter 
+000118e0: 696e 2060 436c 6965 6e74 2e63 7265 6174  in `Client.creat
+000118f0: 655f 636f 6e74 6169 6e65 7260 2069 7320  e_container` is 
+00011900: 6e6f 7720 6f70 7469 6f6e 616c 2028 666f  now optional (fo
+00011910: 720a 2020 636f 6e74 6169 6e65 7273 2074  r.  containers t
+00011920: 6861 7420 696e 636c 7564 6520 6120 6465  hat include a de
+00011930: 6661 756c 7420 7275 6e20 636f 6d6d 616e  fault run comman
+00011940: 6429 0a0a 2323 2320 4275 6766 6978 6573  d)..### Bugfixes
+00011950: 0a0a 2a20 4669 7865 6420 5079 7468 6f6e  ..* Fixed Python
+00011960: 2033 2073 7570 706f 7274 0a2a 2046 6978   3 support.* Fix
+00011970: 6564 2061 2062 7567 2077 6865 7265 2061  ed a bug where a
+00011980: 6e6f 6e79 6d6f 7573 2070 7573 682f 7075  nonymous push/pu
+00011990: 6c6c 2077 6f75 6c64 2062 7265 616b 2077  ll would break w
+000119a0: 6865 6e20 6e6f 2061 7574 6863 6f6e 6669  hen no authconfi
+000119b0: 6720 6973 0a20 2070 7265 7365 6e74 0a2a  g is.  present.*
+000119c0: 2046 6978 6564 2061 2062 7567 2077 6865   Fixed a bug whe
+000119d0: 7265 2074 6865 2060 7175 6965 7460 2070  re the `quiet` p
+000119e0: 6172 616d 6574 6572 2077 6f75 6c64 6e27  arameter wouldn'
+000119f0: 7420 6265 2074 616b 656e 2069 6e74 6f20  t be taken into 
+00011a00: 6163 636f 756e 7420 696e 0a20 2060 436c  account in.  `Cl
+00011a10: 6965 6e74 2e63 6f6e 7461 696e 6572 7360  ient.containers`
+00011a20: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00011a30: 6865 7265 2060 436c 6965 6e74 2e70 7573  here `Client.pus
+00011a40: 6860 2077 6f75 6c64 2062 7265 616b 2077  h` would break w
+00011a50: 6865 6e20 7075 7368 696e 6720 746f 2070  hen pushing to p
+00011a60: 7269 7661 7465 0a20 2072 6567 6973 7472  rivate.  registr
+00011a70: 6965 732e 0a2a 2052 656d 6f76 6564 2075  ies..* Removed u
+00011a80: 6e75 7365 6420 6072 6567 6973 7472 7960  nused `registry`
+00011a90: 2070 6172 616d 6574 6572 2069 6e20 6043   parameter in `C
+00011aa0: 6c69 656e 742e 7075 6c6c 602e 0a2a 2052  lient.pull`..* R
+00011ab0: 656d 6f76 6564 206f 6273 6f6c 6574 6520  emoved obsolete 
+00011ac0: 6375 7374 6f6d 2065 7272 6f72 206d 6573  custom error mes
+00011ad0: 7361 6765 2069 6e20 6043 6c69 656e 742e  sage in `Client.
+00011ae0: 6372 6561 7465 5f63 6f6e 7461 696e 6572  create_container
+00011af0: 602e 0a0a 2323 2320 4d69 7363 656c 6c61  `...### Miscella
+00011b00: 6e65 6f75 730a 0a2a 2064 6f63 6b65 722d  neous..* docker-
+00011b10: 7079 2069 7320 6e6f 7720 756e 6974 2d74  py is now unit-t
+00011b20: 6573 7465 642c 2061 6e64 2054 7261 7669  ested, and Travi
+00011b30: 732d 4349 2068 6173 2062 6565 6e20 656e  s-CI has been en
+00011b40: 6162 6c65 6420 6f6e 2074 6865 0a20 2073  abled on the.  s
+00011b50: 6f75 7263 6520 7265 706f 7369 746f 7279  ource repository
+00011b60: 2e0a 0a30 2e32 2e31 0a2d 2d2d 2d2d 0a0a  ...0.2.1.-----..
+00011b70: 2a20 496d 7072 6f76 656d 656e 7473 2074  * Improvements t
+00011b80: 6f20 7468 6520 6074 6f78 2e69 6e69 6020  o the `tox.ini` 
+00011b90: 6669 6c65 0a0a 2323 2320 4275 6766 6978  file..### Bugfix
+00011ba0: 6573 0a0a 2a20 4669 7865 6420 6120 6275  es..* Fixed a bu
+00011bb0: 6720 7768 6572 6520 7468 6520 7061 636b  g where the pack
+00011bc0: 6167 6520 776f 756c 6420 6661 696c 2077  age would fail w
+00011bd0: 6974 6820 616e 2060 496d 706f 7274 4572  ith an `ImportEr
+00011be0: 726f 7260 2069 6620 7265 7175 6573 7473  ror` if requests
+00011bf0: 0a20 2077 6173 2069 6e73 7461 6c6c 6564  .  was installed
+00011c00: 2075 7369 6e67 2060 6170 742d 6765 7460   using `apt-get`
+00011c10: 0a2a 2046 6978 6564 2061 2062 7567 2077  .* Fixed a bug w
+00011c20: 6865 7265 2060 436c 6965 6e74 2e62 7569  here `Client.bui
+00011c30: 6c64 6020 776f 756c 6420 6661 696c 2069  ld` would fail i
+00011c40: 6620 6769 7665 6e20 6120 6070 6174 6860  f given a `path`
+00011c50: 2070 6172 616d 6574 6572 2e0a 2a20 4669   parameter..* Fi
+00011c60: 7865 6420 7365 7665 7261 6c20 6275 6773  xed several bugs
+00011c70: 2069 6e20 6043 6c69 656e 742e 6c6f 6769   in `Client.logi
+00011c80: 6e60 2e20 4974 2073 686f 756c 6420 6e6f  n`. It should no
+00011c90: 7720 776f 726b 2077 6974 6820 4150 4920  w work with API 
+00011ca0: 7665 7273 696f 6e73 0a20 2031 2e34 2c20  versions.  1.4, 
+00011cb0: 312e 352e 0a2a 2050 6c65 6173 6520 6e6f  1.5..* Please no
+00011cc0: 7465 2074 6861 7420 6043 6c69 656e 742e  te that `Client.
+00011cd0: 6c6f 6769 6e60 2063 7572 7265 6e74 6c79  login` currently
+00011ce0: 2064 6f65 736e 2774 2077 7269 7465 2061   doesn't write a
+00011cf0: 7574 6820 746f 2074 6865 0a20 2060 2e64  uth to the.  `.d
+00011d00: 6f63 6b65 7263 6667 6020 6669 6c65 2c20  ockercfg` file, 
+00011d10: 7468 7573 202a 2a61 7574 6820 6973 206e  thus **auth is n
+00011d20: 6f74 2070 6572 7369 7374 656e 7420 7768  ot persistent wh
+00011d30: 656e 2075 7369 6e67 2074 6869 7320 6d65  en using this me
+00011d40: 7468 6f64 2e2a 2a0a 0a30 2e32 2e30 0a2d  thod.**..0.2.0.-
+00011d50: 2d2d 2d2d 0a0a 2a20 2a2a 5468 6973 2076  ----..* **This v
+00011d60: 6572 7369 6f6e 2069 6e74 726f 6475 6365  ersion introduce
+00011d70: 7320 6272 6561 6b69 6e67 2063 6861 6e67  s breaking chang
+00011d80: 6573 212a 2a0a 2a20 6043 6c69 656e 742e  es!**.* `Client.
+00011d90: 6b69 6c6c 602c 2060 436c 6965 6e74 2e72  kill`, `Client.r
+00011da0: 656d 6f76 655f 636f 6e74 6169 6e65 7260  emove_container`
+00011db0: 2c20 6043 6c69 656e 742e 7265 6d6f 7665  , `Client.remove
+00011dc0: 5f69 6d61 6765 602c 0a60 436c 6965 6e74  _image`,.`Client
+00011dd0: 2e72 6573 7461 7274 602c 2060 436c 6965  .restart`, `Clie
+00011de0: 6e74 2e73 7461 7274 602c 2060 436c 6965  nt.start`, `Clie
+00011df0: 6e74 2e73 746f 7060 2061 6e64 2060 436c  nt.stop` and `Cl
+00011e00: 6965 6e74 2e77 6169 7460 2064 6f6e 2774  ient.wait` don't
+00011e10: 2073 7570 706f 7274 0a76 6172 6172 6773   support.varargs
+00011e20: 2061 6e79 6d6f 7265 2e0a 2a20 4164 6465   anymore..* Adde
+00011e30: 6420 636f 6d6d 616e 6473 2060 436c 6965  d commands `Clie
+00011e40: 6e74 2e74 6f70 6020 616e 6420 6043 6c69  nt.top` and `Cli
+00011e50: 656e 742e 636f 7079 600a 2a20 4164 6465  ent.copy`.* Adde
+00011e60: 6420 606c 7863 5f63 6f6e 6660 2070 6172  d `lxc_conf` par
+00011e70: 616d 6574 6572 2074 6f20 6043 6c69 656e  ameter to `Clien
+00011e80: 742e 7374 6172 7460 0a2a 2041 6464 6564  t.start`.* Added
+00011e90: 2073 7570 706f 7274 2066 6f72 2061 7574   support for aut
+00011ea0: 6865 6e74 6963 6174 696f 6e20 696e 2060  hentication in `
+00011eb0: 436c 6965 6e74 2e70 756c 6c60 2028 4150  Client.pull` (AP
+00011ec0: 4920 7665 7273 696f 6e20 3e3d 312e 3529  I version >=1.5)
+00011ed0: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00011ee0: 2066 6f72 2070 7269 7669 6c65 6765 6420   for privileged 
+00011ef0: 636f 6e74 6169 6e65 7273 2e0a 2a20 4572  containers..* Er
+00011f00: 726f 7220 6d61 6e61 6765 6d65 6e74 206f  ror management o
+00011f10: 7665 7268 6175 6c2e 2054 6865 206e 6577  verhaul. The new
+00011f20: 2076 6572 7369 6f6e 2073 686f 756c 6420   version should 
+00011f30: 6265 206d 6f72 6520 636f 6e73 6973 7465  be more consiste
+00011f40: 6e74 2061 6e64 0a2a 2041 6c6c 206d 6574  nt and.* All met
+00011f50: 686f 6473 2074 6861 7420 6578 7065 6374  hods that expect
+00011f60: 6564 2061 2063 6f6e 7461 696e 6572 2049  ed a container I
+00011f70: 4420 6173 2061 7267 756d 656e 7420 6e6f  D as argument no
+00011f80: 7720 616c 736f 2073 7570 706f 7274 2061  w also support a
+00011f90: 2064 6963 740a 636f 6e74 6169 6e69 6e67   dict.containing
+00011fa0: 2061 6e20 6049 6460 206b 6579 2e0a 2a20   an `Id` key..* 
+00011fb0: 4164 6465 6420 6c69 6365 6e73 6520 6865  Added license he
+00011fc0: 6164 6572 2074 6f20 7079 7468 6f6e 2066  ader to python f
+00011fd0: 696c 6573 2e0a 2a20 5365 7665 7261 6c20  iles..* Several 
+00011fe0: 6052 4541 444d 452e 6d64 6020 7570 6461  `README.md` upda
+00011ff0: 7465 732e 0a0a 2323 2320 4275 6766 6978  tes...### Bugfix
+00012000: 6573 0a0a 2a20 4669 7865 6420 7365 7665  es..* Fixed seve
+00012010: 7261 6c20 6275 6773 2077 6974 6820 6175  ral bugs with au
+00012020: 7468 2063 6f6e 6669 6720 7061 7273 696e  th config parsin
+00012030: 672e 0a2a 2046 6978 6564 2061 2062 7567  g..* Fixed a bug
+00012040: 2069 6e20 6043 6c69 656e 742e 7075 7368   in `Client.push
+00012050: 6020 7768 6572 6520 6974 2077 6f75 6c64  ` where it would
+00012060: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
+00012070: 696f 6e20 6966 0a74 6865 2061 7574 6820  ion if.the auth 
+00012080: 636f 6e66 6967 2077 6173 6e27 7420 6c6f  config wasn't lo
+00012090: 6164 6564 2e0a 2a20 4669 7865 6420 6120  aded..* Fixed a 
+000120a0: 6275 6720 696e 2060 436c 6965 6e74 2e70  bug in `Client.p
+000120b0: 756c 6c60 2077 6865 7265 2070 7269 7661  ull` where priva
+000120c0: 7465 2072 6567 6973 7472 7920 696d 6167  te registry imag
+000120d0: 6573 2077 6f75 6c64 6e27 7420 6265 2070  es wouldn't be p
+000120e0: 6172 7365 640a 7072 6f70 6572 6c79 2069  arsed.properly i
+000120f0: 6620 6974 2063 6f6e 7461 696e 6564 2070  f it contained p
+00012100: 6f72 7420 696e 666f 726d 6174 696f 6e2e  ort information.
+00012110: 0a0a 0a30 2e31 2e35 0a2d 2d2d 2d2d 0a0a  ...0.1.5.-----..
+00012120: 2a20 6043 6c69 656e 742e 6275 696c 6460  * `Client.build`
+00012130: 206e 6f77 2075 7365 7320 7465 6d70 6669   now uses tempfi
+00012140: 6c65 7320 746f 2073 746f 7265 2062 7569  les to store bui
+00012150: 6c64 2063 6f6e 7465 7874 2069 6e73 7465  ld context inste
+00012160: 6164 206f 6620 7374 6f72 696e 670a 6974  ad of storing.it
+00012170: 2069 6e20 6d65 6d6f 7279 0a2a 2041 6464   in memory.* Add
+00012180: 6564 2060 6e6f 6361 6368 6560 206f 7074  ed `nocache` opt
+00012190: 696f 6e20 746f 2060 436c 6965 6e74 2e62  ion to `Client.b
+000121a0: 7569 6c64 600a 2a20 6043 6c69 656e 742e  uild`.* `Client.
+000121b0: 7265 6d6f 7665 5f63 6f6e 7461 696e 6572  remove_container
+000121c0: 6020 6e6f 7720 7261 6973 6573 2061 6e20  ` now raises an 
+000121d0: 6578 6365 7074 696f 6e20 7768 656e 2074  exception when t
+000121e0: 7279 696e 6720 746f 2072 656d 6f76 6520  rying to remove 
+000121f0: 610a 7275 6e6e 696e 6720 636f 6e74 6169  a.running contai
+00012200: 6e65 720a 2a20 6043 6c69 656e 742e 6372  ner.* `Client.cr
+00012210: 6561 7465 5f63 6f6e 7461 696e 6572 6020  eate_container` 
+00012220: 6e6f 7720 6163 6365 7074 7320 6469 6374  now accepts dict
+00012230: 7320 666f 7220 7468 6520 6065 6e76 6972  s for the `envir
+00012240: 6f6e 6d65 6e74 6020 7061 7261 6d65 7465  onment` paramete
+00012250: 720a 0a23 2323 2042 7567 6669 7865 730a  r..### Bugfixes.
+00012260: 0a2a 2046 6978 6564 2061 2062 7567 2069  .* Fixed a bug i
+00012270: 6e20 6043 6c69 656e 742e 6372 6561 7465  n `Client.create
+00012280: 5f63 6f6e 7461 696e 6572 6020 6f6e 2050  _container` on P
+00012290: 7974 686f 6e20 322e 3620 7768 6572 6520  ython 2.6 where 
+000122a0: 756e 6963 6f64 650a 636f 6d6d 616e 6473  unicode.commands
+000122b0: 2077 6f75 6c64 2066 6169 6c20 746f 2062   would fail to b
+000122c0: 6520 7061 7273 6564 0a2a 2046 6978 6564  e parsed.* Fixed
+000122d0: 2061 2062 7567 2069 6e20 6043 6c69 656e   a bug in `Clien
+000122e0: 742e 6275 696c 6460 2077 6865 7265 2074  t.build` where t
+000122f0: 6865 2060 7461 6760 2070 6172 616d 6574  he `tag` paramet
+00012300: 6572 2077 6f75 6c64 206e 6f74 2062 6520  er would not be 
+00012310: 7461 6b65 6e0a 696e 746f 2061 6363 6f75  taken.into accou
+00012320: 6e74 0a0a 302e 312e 340a 2d2d 2d2d 2d0a  nt..0.1.4.-----.
+00012330: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00012340: 2066 6f72 2041 5049 2063 6f6e 6e65 6374   for API connect
+00012350: 696f 6e20 7468 726f 7567 6820 554e 4958  ion through UNIX
+00012360: 2073 6f63 6b65 7420 2864 6566 6175 6c74   socket (default
+00012370: 2066 6f72 2064 6f63 6b65 7220 302e 352e   for docker 0.5.
+00012380: 322b 290a 0a30 2e31 2e33 0a2d 2d2d 2d2d  2+)..0.1.3.-----
+00012390: 0a0a 2a20 5468 6520 636c 6965 6e74 206e  ..* The client n
+000123a0: 6f77 2074 7269 6573 2074 6f20 6c6f 6164  ow tries to load
+000123b0: 2074 6865 2061 7574 6820 636f 6e66 6967   the auth config
+000123c0: 2066 726f 6d20 607e 2f2e 646f 636b 6572   from `~/.docker
+000123d0: 6366 6760 2e20 5468 6973 2069 7320 6e65  cfg`. This is ne
+000123e0: 6365 7373 6172 7920 746f 2075 7365 2074  cessary to use t
+000123f0: 6865 2070 7573 6820 636f 6d6d 616e 6420  he push command 
+00012400: 6966 2041 5049 2076 6572 7369 6f6e 2069  if API version i
+00012410: 7320 3e31 2e30 0a0a 302e 312e 320a 2d2d  s >1.0..0.1.2.--
+00012420: 2d2d 2d0a 0a2a 2041 6464 6564 2061 2060  ---..* Added a `
+00012430: 7175 6965 7420 7061 7261 6d65 7465 7260  quiet parameter`
+00012440: 2074 6f20 6043 6c69 656e 742e 6275 696c   to `Client.buil
+00012450: 6460 2028 6d69 7272 6f72 7320 7468 6520  d` (mirrors the 
+00012460: 6071 6020 7061 7261 6d65 7465 7220 696e  `q` parameter in
+00012470: 2074 6865 2041 5049 290a 0a30 2e31 2e31   the API)..0.1.1
+00012480: 0a2d 2d2d 2d2d 0a0a 2a20 4669 7865 6420  .-----..* Fixed 
+00012490: 6120 6275 6720 7768 6572 6520 7468 6520  a bug where the 
+000124a0: 6275 696c 6420 636f 6d6d 616e 6420 776f  build command wo
+000124b0: 756c 6420 6c69 7374 2074 6172 2063 6f6e  uld list tar con
+000124c0: 7465 6e74 7320 6265 666f 7265 2073 656e  tents before sen
+000124d0: 6469 6e67 2074 6865 2072 6571 7565 7374  ding the request
+000124e0: 0a2a 2046 6978 6564 2061 2062 7567 2069  .* Fixed a bug i
+000124f0: 6e20 6043 6c69 656e 742e 706f 7274 600a  n `Client.port`.
+00012500: 0a0a 302e 312e 300a 2d2d 2d2d 2d0a 2a20  ..0.1.0.-----.* 
+00012510: 2a2a 5468 6973 2076 6572 7369 6f6e 2069  **This version i
+00012520: 6e74 726f 6475 6365 7320 6272 6561 6b69  ntroduces breaki
+00012530: 6e67 2063 6861 6e67 6573 212a 2a0a 2a20  ng changes!**.* 
+00012540: 5377 6974 6368 6564 2074 6f20 7365 7276  Switched to serv
+00012550: 6572 2073 6964 6520 6275 696c 6420 7379  er side build sy
+00012560: 7374 656d 0a2a 2052 656d 6f76 6564 2074  stem.* Removed t
+00012570: 6865 2042 7569 6c64 6572 436c 6965 6e74  he BuilderClient
+00012580: 0a2a 2041 6464 6564 2073 7570 706f 7274  .* Added support
+00012590: 2066 6f72 2063 6f6e 7465 7874 7561 6c20   for contextual 
+000125a0: 6275 696c 6473 0a2a 2041 6464 6564 2073  builds.* Added s
+000125b0: 7570 706f 7274 2066 6f72 2072 656d 6f74  upport for remot
+000125c0: 6520 5552 4c20 6275 696c 6473 0a2a 2041  e URL builds.* A
+000125d0: 6464 6564 2070 7974 686f 6e20 3320 7375  dded python 3 su
+000125e0: 7070 6f72 740a 2a20 4164 6465 6420 6269  pport.* Added bi
+000125f0: 6e64 206d 6f75 6e74 7320 7375 7070 6f72  nd mounts suppor
+00012600: 740a 2a20 4164 6465 6420 4150 4920 7665  t.* Added API ve
+00012610: 7273 696f 6e20 7375 7070 6f72 740a 2a20  rsion support.* 
+00012620: 4669 7865 6420 6120 6275 6720 7768 6572  Fixed a bug wher
+00012630: 6520 6043 6c69 656e 742e 706f 7274 6020  e `Client.port` 
+00012640: 776f 756c 6420 6661 696c 2069 6620 7072  would fail if pr
+00012650: 6f76 6964 6564 2077 6974 6820 6120 706f  ovided with a po
+00012660: 7274 206f 6620 7479 7065 206e 756d 6265  rt of type numbe
+00012670: 720a 2a20 4669 7865 6420 6120 6275 6720  r.* Fixed a bug 
+00012680: 7768 6572 6520 6043 6c69 656e 742e 5f70  where `Client._p
+00012690: 6f73 745f 6a73 6f6e 6020 776f 756c 646e  ost_json` wouldn
+000126a0: 2774 2073 6574 2074 6865 2043 6f6e 7465  't set the Conte
+000126b0: 6e74 2d54 7970 6520 6865 6164 6572 2074  nt-Type header t
+000126c0: 6f20 6061 7070 6c69 6361 7469 6f6e 2f6a  o `application/j
+000126d0: 736f 6e60 0a0a 302e 302e 360a 2d2d 2d2d  son`..0.0.6.----
+000126e0: 2d0a 2a20 4164 6465 6420 7375 7070 6f72  -.* Added suppor
+000126f0: 7420 666f 7220 6375 7374 6f6d 206c 6f67  t for custom log
+00012700: 6765 7273 2069 6e20 6043 6c69 656e 742e  gers in `Client.
+00012710: 6275 696c 6460 0a2a 2041 6464 6564 2060  build`.* Added `
+00012720: 436c 6965 6e74 2e61 7474 6163 6860 2063  Client.attach` c
+00012730: 6f6d 6d61 6e64 0a2a 2041 6464 6564 2073  ommand.* Added s
+00012740: 7570 706f 7274 2066 6f72 2060 4144 4460  upport for `ADD`
+00012750: 2063 6f6d 6d61 6e64 2069 6e20 6275 696c   command in buil
+00012760: 6465 720a 2a20 4669 7865 6420 6120 6275  der.* Fixed a bu
+00012770: 6720 696e 2060 436c 6965 6e74 2e6c 6f67  g in `Client.log
+00012780: 7360 0a2a 2049 6d70 726f 7665 6420 756e  s`.* Improved un
+00012790: 6974 2074 6573 7473 0a0a 0a30 2e30 2e35  it tests...0.0.5
+000127a0: 0a2d 2d2d 2d2d 0a2a 2041 6464 6564 2074  .-----.* Added t
+000127b0: 6167 2073 7570 706f 7274 2066 6f72 2074  ag support for t
+000127c0: 6865 2062 7569 6c64 6572 0a2a 2055 7365  he builder.* Use
+000127d0: 2060 7368 6c65 7860 2074 6f20 7061 7273   `shlex` to pars
+000127e0: 6520 706c 6169 6e20 7374 7269 6e67 2063  e plain string c
+000127f0: 6f6d 6d61 6e64 7320 7768 656e 2063 7265  ommands when cre
+00012800: 6174 696e 6720 6120 636f 6e74 6169 6e65  ating a containe
+00012810: 720a 2a20 4669 7865 6420 7365 7665 7261  r.* Fixed severa
+00012820: 6c20 6275 6773 2069 6e20 7468 6520 6275  l bugs in the bu
+00012830: 696c 6465 720a 2a20 4669 7865 6420 7468  ilder.* Fixed th
+00012840: 6520 6071 7569 6574 6020 6f70 7469 6f6e  e `quiet` option
+00012850: 2069 6e20 6043 6c69 656e 742e 696d 6167   in `Client.imag
+00012860: 6573 600a 2a20 556e 6974 2074 6573 7473  es`.* Unit tests
+00012870: 0a0a 302e 302e 340a 2d2d 2d2d 2d0a 2a20  ..0.0.4.-----.* 
+00012880: 496d 7072 6f76 6564 2065 7272 6f72 2072  Improved error r
+00012890: 6570 6f72 7469 6e67 0a0a 302e 302e 330a  eporting..0.0.3.
+000128a0: 2d2d 2d2d 2d0a 2a20 4669 7865 6420 6120  -----.* Fixed a 
+000128b0: 6275 6720 696e 2060 436c 6965 6e74 2e74  bug in `Client.t
+000128c0: 6167 600a 2a20 4669 7865 6420 6120 6275  ag`.* Fixed a bu
+000128d0: 6720 7768 6572 6520 6765 6e65 7261 7465  g where generate
+000128e0: 6420 696d 6167 6573 2077 6f75 6c64 2062  d images would b
+000128f0: 6520 7265 6d6f 7665 6420 6166 7465 7220  e removed after 
+00012900: 6120 7375 6363 6573 7366 756c 2062 7569  a successful bui
+00012910: 6c64 0a0a 302e 302e 320a 2d2d 2d2d 2d0a  ld..0.0.2.-----.
+00012920: 2a20 496d 706c 656d 656e 7465 6420 6669  * Implemented fi
+00012930: 7273 7420 7665 7273 696f 6e20 6f66 2074  rst version of t
+00012940: 6865 2062 7569 6c64 6572 2063 6c69 656e  he builder clien
+00012950: 740a                                     t.
```

### Comparing `docker-6.1.1/docs/client.rst` & `docker-6.1.2/docs/client.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/conf.py` & `docker-6.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/containers.rst` & `docker-6.1.2/docs/containers.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/favicon_whale.png` & `docker-6.1.2/docs/favicon_whale.png`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/images.rst` & `docker-6.1.2/docs/images.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/index.rst` & `docker-6.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/networks.rst` & `docker-6.1.2/docs/networks.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/nodes.rst` & `docker-6.1.2/docs/nodes.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/plugins.rst` & `docker-6.1.2/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/services.rst` & `docker-6.1.2/docs/services.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/swarm.rst` & `docker-6.1.2/docs/swarm.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/tls.rst` & `docker-6.1.2/docs/tls.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/user_guides/multiplex.rst` & `docker-6.1.2/docs/user_guides/multiplex.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/user_guides/swarm_services.md` & `docker-6.1.2/docs/user_guides/swarm_services.md`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/docs/volumes.rst` & `docker-6.1.2/docs/volumes.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/scripts/release.sh` & `docker-6.1.2/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/scripts/versions.py` & `docker-6.1.2/scripts/versions.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/setup.py` & `docker-6.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/Dockerfile` & `docker-6.1.2/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/Dockerfile-dind-certs` & `docker-6.1.2/tests/Dockerfile-dind-certs`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/gpg-keys/secret` & `docker-6.1.2/tests/gpg-keys/secret`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/helpers.py` & `docker-6.1.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_build_test.py` & `docker-6.1.2/tests/integration/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_client_test.py` & `docker-6.1.2/tests/integration/api_client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_config_test.py` & `docker-6.1.2/tests/integration/api_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_container_test.py` & `docker-6.1.2/tests/integration/api_container_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_exec_test.py` & `docker-6.1.2/tests/integration/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_healthcheck_test.py` & `docker-6.1.2/tests/integration/api_healthcheck_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_image_test.py` & `docker-6.1.2/tests/integration/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_network_test.py` & `docker-6.1.2/tests/integration/api_network_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_plugin_test.py` & `docker-6.1.2/tests/integration/api_plugin_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_secret_test.py` & `docker-6.1.2/tests/integration/api_secret_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_service_test.py` & `docker-6.1.2/tests/integration/api_service_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_swarm_test.py` & `docker-6.1.2/tests/integration/api_swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/api_volume_test.py` & `docker-6.1.2/tests/integration/api_volume_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/base.py` & `docker-6.1.2/tests/integration/base.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/client_test.py` & `docker-6.1.2/tests/integration/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/conftest.py` & `docker-6.1.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/context_api_test.py` & `docker-6.1.2/tests/integration/context_api_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/credentials/store_test.py` & `docker-6.1.2/tests/integration/credentials/store_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/errors_test.py` & `docker-6.1.2/tests/integration/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_containers_test.py` & `docker-6.1.2/tests/integration/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_images_test.py` & `docker-6.1.2/tests/integration/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_networks_test.py` & `docker-6.1.2/tests/integration/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_nodes_test.py` & `docker-6.1.2/tests/integration/models_nodes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_resources_test.py` & `docker-6.1.2/tests/integration/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_services_test.py` & `docker-6.1.2/tests/integration/models_services_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_swarm_test.py` & `docker-6.1.2/tests/integration/models_swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/models_volumes_test.py` & `docker-6.1.2/tests/integration/models_volumes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/integration/regression_test.py` & `docker-6.1.2/tests/integration/regression_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/ssh/api_build_test.py` & `docker-6.1.2/tests/ssh/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/ssh/base.py` & `docker-6.1.2/tests/ssh/base.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/ssh/config/client/id_rsa` & `docker-6.1.2/tests/ssh/config/client/id_rsa`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/ssh/config/client/id_rsa.pub` & `docker-6.1.2/tests/ssh/config/client/id_rsa.pub`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/ssh/connect_test.py` & `docker-6.1.2/tests/ssh/connect_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/api_build_test.py` & `docker-6.1.2/tests/unit/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/api_container_test.py` & `docker-6.1.2/tests/unit/api_container_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/api_exec_test.py` & `docker-6.1.2/tests/unit/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/api_image_test.py` & `docker-6.1.2/tests/unit/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/api_network_test.py` & `docker-6.1.2/tests/unit/api_network_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/api_test.py` & `docker-6.1.2/tests/unit/api_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/api_volume_test.py` & `docker-6.1.2/tests/unit/api_volume_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/auth_test.py` & `docker-6.1.2/tests/unit/auth_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/client_test.py` & `docker-6.1.2/tests/unit/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/context_test.py` & `docker-6.1.2/tests/unit/context_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/dockertypes_test.py` & `docker-6.1.2/tests/unit/dockertypes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/errors_test.py` & `docker-6.1.2/tests/unit/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/fake_api.py` & `docker-6.1.2/tests/unit/fake_api.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/fake_api_client.py` & `docker-6.1.2/tests/unit/fake_api_client.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/fake_stat.py` & `docker-6.1.2/tests/unit/fake_stat.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/models_containers_test.py` & `docker-6.1.2/tests/unit/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/models_images_test.py` & `docker-6.1.2/tests/unit/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/models_networks_test.py` & `docker-6.1.2/tests/unit/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/models_resources_test.py` & `docker-6.1.2/tests/unit/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/models_services_test.py` & `docker-6.1.2/tests/unit/models_services_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/sshadapter_test.py` & `docker-6.1.2/tests/unit/sshadapter_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/ssladapter_test.py` & `docker-6.1.2/tests/unit/ssladapter_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/swarm_test.py` & `docker-6.1.2/tests/unit/swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/utils_build_test.py` & `docker-6.1.2/tests/unit/utils_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/utils_config_test.py` & `docker-6.1.2/tests/unit/utils_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/utils_json_stream_test.py` & `docker-6.1.2/tests/unit/utils_json_stream_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/utils_proxy_test.py` & `docker-6.1.2/tests/unit/utils_proxy_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.1/tests/unit/utils_test.py` & `docker-6.1.2/tests/unit/utils_test.py`

 * *Files identical despite different names*

