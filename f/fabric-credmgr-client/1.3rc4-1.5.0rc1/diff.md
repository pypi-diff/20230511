# Comparing `tmp/fabric-credmgr-client-1.3rc4.tar.gz` & `tmp/fabric-credmgr-client-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-credmgr-client-1.3rc4.tar", last modified: Wed Jul 13 12:54:52 2022, max compression
+gzip compressed data, was "fabric-credmgr-client-1.5.0rc1.tar", last modified: Thu May 11 18:09:36 2023, max compression
```

## Comparing `fabric-credmgr-client-1.3rc4.tar` & `fabric-credmgr-client-1.5.0rc1.tar`

### file list

```diff
@@ -1,76 +1,90 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.397238 fabric-credmgr-client-1.3rc4/
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2022-05-18 19:11:38.000000 fabric-credmgr-client-1.3rc4/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)       59 2022-05-18 19:11:38.000000 fabric-credmgr-client-1.3rc4/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)     4693 2022-07-13 12:54:52.396705 fabric-credmgr-client-1.3rc4/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     4434 2022-05-18 19:39:50.000000 fabric-credmgr-client-1.3rc4/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.344487 fabric-credmgr-client-1.3rc4/fabric_cm/
--rw-r--r--   0 kthare10   (503) staff       (20)       23 2022-07-13 12:54:40.000000 fabric-credmgr-client-1.3rc4/fabric_cm/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.345244 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-05-18 19:11:38.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     6003 2022-07-12 13:40:30.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/credmgr_proxy.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.349781 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/
--rw-r--r--   0 kthare10   (503) staff       (20)     2545 2022-05-18 19:30:51.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.353957 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/
--rw-r--r--   0 kthare10   (503) staff       (20)      301 2022-05-18 19:31:07.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3832 2022-05-18 19:31:22.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/default_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)    12548 2022-05-18 19:31:59.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/tokens_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3755 2022-05-18 19:39:11.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/version_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)    25120 2022-05-18 19:32:22.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api_client.py
--rw-r--r--   0 kthare10   (503) staff       (20)     7972 2022-05-18 19:32:36.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/configuration.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.374483 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/
--rw-r--r--   0 kthare10   (503) staff       (20)     2143 2022-05-18 19:33:01.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2964 2022-05-18 19:33:11.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/jwks.py
--rw-r--r--   0 kthare10   (503) staff       (20)     6062 2022-05-18 19:33:17.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3299 2022-05-18 19:33:25.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5011 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3844 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4265 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3175 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5783 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5075 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3882 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5006 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3843 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4983 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3831 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5236 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3975 2022-05-18 19:34:43.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4831 2022-05-18 20:01:13.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/token.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3394 2022-07-12 21:01:55.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/tokens.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3420 2022-05-18 19:49:18.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/version.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3894 2022-05-18 19:35:11.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/version_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)    13000 2022-05-18 19:33:56.000000 fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/rest.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.376859 fabric-credmgr-client-1.3rc4/fabric_credmgr_client.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)     4693 2022-07-13 12:54:52.000000 fabric-credmgr-client-1.3rc4/fabric_credmgr_client.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     2814 2022-07-13 12:54:52.000000 fabric-credmgr-client-1.3rc4/fabric_credmgr_client.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2022-07-13 12:54:52.000000 fabric-credmgr-client-1.3rc4/fabric_credmgr_client.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       99 2022-07-13 12:54:52.000000 fabric-credmgr-client-1.3rc4/fabric_credmgr_client.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       15 2022-07-13 12:54:52.000000 fabric-credmgr-client-1.3rc4/fabric_credmgr_client.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)      108 2022-05-18 19:11:38.000000 fabric-credmgr-client-1.3rc4/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2022-07-13 12:54:52.397365 fabric-credmgr-client-1.3rc4/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)     1068 2022-05-18 19:11:38.000000 fabric-credmgr-client-1.3rc4/setup.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-07-13 12:54:52.396098 fabric-credmgr-client-1.3rc4/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-05-18 19:40:51.000000 fabric-credmgr-client-1.3rc4/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)      857 2022-05-18 19:45:28.000000 fabric-credmgr-client-1.3rc4/test/test_default_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      843 2022-05-18 19:45:44.000000 fabric-credmgr-client-1.3rc4/test/test_jwks.py
--rw-r--r--   0 kthare10   (503) staff       (20)      877 2022-05-18 19:45:44.000000 fabric-credmgr-client-1.3rc4/test/test_jwks_keys.py
--rw-r--r--   0 kthare10   (503) staff       (20)      867 2022-05-18 19:45:59.000000 fabric-credmgr-client-1.3rc4/test/test_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)      977 2022-05-18 19:46:15.000000 fabric-credmgr-client-1.3rc4/test/test_status200_ok_no_content.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1011 2022-05-18 19:46:15.000000 fabric-credmgr-client-1.3rc4/test/test_status200_ok_no_content_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)      951 2022-05-18 19:46:24.000000 fabric-credmgr-client-1.3rc4/test/test_status200_ok_single.py
--rw-r--r--   0 kthare10   (503) staff       (20)      967 2022-05-18 19:46:31.000000 fabric-credmgr-client-1.3rc4/test/test_status400_bad_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1017 2022-05-18 19:46:38.000000 fabric-credmgr-client-1.3rc4/test/test_status400_bad_request_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      981 2022-05-18 19:47:23.000000 fabric-credmgr-client-1.3rc4/test/test_status401_unauthorized.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1031 2022-05-18 19:47:23.000000 fabric-credmgr-client-1.3rc4/test/test_status401_unauthorized_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      975 2022-05-18 19:47:46.000000 fabric-credmgr-client-1.3rc4/test/test_status403_forbidden.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1025 2022-05-18 19:47:46.000000 fabric-credmgr-client-1.3rc4/test/test_status403_forbidden_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      969 2022-05-18 19:47:46.000000 fabric-credmgr-client-1.3rc4/test/test_status404_not_found.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1019 2022-05-18 19:47:53.000000 fabric-credmgr-client-1.3rc4/test/test_status404_not_found_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1059 2022-05-18 19:47:59.000000 fabric-credmgr-client-1.3rc4/test/test_status500_internal_server_error.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1109 2022-05-18 19:48:08.000000 fabric-credmgr-client-1.3rc4/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      869 2022-05-18 19:48:17.000000 fabric-credmgr-client-1.3rc4/test/test_token.py
--rw-r--r--   0 kthare10   (503) staff       (20)      877 2022-05-18 19:48:25.000000 fabric-credmgr-client-1.3rc4/test/test_tokens.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1173 2022-05-18 19:48:31.000000 fabric-credmgr-client-1.3rc4/test/test_tokens_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      885 2022-05-18 19:48:38.000000 fabric-credmgr-client-1.3rc4/test/test_version.py
--rw-r--r--   0 kthare10   (503) staff       (20)      816 2022-05-18 19:48:46.000000 fabric-credmgr-client-1.3rc4/test/test_version_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      919 2022-05-18 19:48:53.000000 fabric-credmgr-client-1.3rc4/test/test_version_data.py
+-rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.5.0rc1/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.5.0rc1/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-05-11 18:03:22.616419 fabric-credmgr-client-1.5.0rc1/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.5.0rc1/.travis.yml
+-rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.5.0rc1/LICENSE
+-rw-r--r--   0        0        0     4211 2023-05-11 18:03:22.617008 fabric-credmgr-client-1.5.0rc1/README.md
+-rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.5.0rc1/docs/DefaultApi.md
+-rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.5.0rc1/docs/Jwks.md
+-rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.5.0rc1/docs/JwksKeys.md
+-rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.5.0rc1/docs/Request.md
+-rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContent.md
+-rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContentData.md
+-rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.5.0rc1/docs/Status200OkSingle.md
+-rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequest.md
+-rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequestErrors.md
+-rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.5.0rc1/docs/Status401Unauthorized.md
+-rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.5.0rc1/docs/Status401UnauthorizedErrors.md
+-rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.5.0rc1/docs/Status403Forbidden.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.5.0rc1/docs/Status403ForbiddenErrors.md
+-rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.5.0rc1/docs/Status404NotFound.md
+-rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.5.0rc1/docs/Status404NotFoundErrors.md
+-rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerError.md
+-rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerErrorErrors.md
+-rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.5.0rc1/docs/Success.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.619089 fabric-credmgr-client-1.5.0rc1/docs/Token.md
+-rw-r--r--   0        0        0      339 2023-05-11 18:03:22.619217 fabric-credmgr-client-1.5.0rc1/docs/Tokens.md
+-rw-r--r--   0        0        0     5090 2023-05-11 18:03:22.619366 fabric-credmgr-client-1.5.0rc1/docs/TokensApi.md
+-rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.5.0rc1/docs/Version.md
+-rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.5.0rc1/docs/VersionApi.md
+-rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.5.0rc1/docs/VersionData.md
+-rw-r--r--   0        0        0       50 2023-05-11 18:06:29.691397 fabric-credmgr-client-1.5.0rc1/fabric_cm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/__init__.py
+-rw-r--r--   0        0        0     6006 2023-05-11 18:03:22.620379 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/credmgr_proxy.py
+-rw-r--r--   0        0        0     2545 2023-05-11 18:03:22.620670 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/default_api.py
+-rw-r--r--   0        0        0    12548 2023-05-11 18:03:22.621635 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/tokens_api.py
+-rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25120 2023-05-11 18:03:22.622136 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api_client.py
+-rw-r--r--   0        0        0     7980 2023-05-11 18:03:22.622439 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2143 2023-05-11 18:03:22.622732 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks.py
+-rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
+-rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/request.py
+-rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     4831 2023-05-11 18:03:22.626321 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/token.py
+-rw-r--r--   0        0        0     3394 2023-05-11 18:03:22.626505 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/tokens.py
+-rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.5.0rc1/git_push.sh
+-rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.628116 fabric-credmgr-client-1.5.0rc1/test/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.5.0rc1/test/test_default_api.py
+-rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.5.0rc1/test/test_jwks.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.5.0rc1/test/test_jwks_keys.py
+-rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.5.0rc1/test/test_request.py
+-rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.5.0rc1/test/test_token.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.5.0rc1/test/test_tokens.py
+-rw-r--r--   0        0        0     1173 2023-05-11 18:03:22.632206 fabric-credmgr-client-1.5.0rc1/test/test_tokens_api.py
+-rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.5.0rc1/test/test_version.py
+-rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.5.0rc1/test/test_version_api.py
+-rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.5.0rc1/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.5.0rc1/tox.ini
+-rw-r--r--   0        0        0     5196 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.5.0rc1/PKG-INFO
```

### Comparing `fabric-credmgr-client-1.3rc4/LICENSE` & `fabric-credmgr-client-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/PKG-INFO` & `fabric-credmgr-client-1.5.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-Metadata-Version: 2.1
-Name: fabric-credmgr-client
-Version: 1.3rc4
-Summary: Fabric Credential Manager API
-Home-page: 
-Author-email: kthare10@unc.edu
-Keywords: Swagger,Fabric Credential Manager API
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Requirements Status](https://requires.io/github/fabric-testbed/fabric_credmgr_client/requirements.svg?branch=master)](https://requires.io/github/fabric-testbed/fabric_credmgr_client/requirements/?branch=master)
-
 [![PyPI](https://img.shields.io/pypi/v/fabric_credmgr_client?style=plastic)](https://pypi.org/project/fabric_credmgr_client/)
 
 # Fabric Credential Manager Client
 This is Fabric Credential Manager API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
```

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/credmgr_proxy.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/credmgr_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def __init__(self, credmgr_host: str):
         self.host = credmgr_host
         self.tokens_api = None
         if credmgr_host is not None:
             # create an instance of the API class
             configuration = swagger_client.configuration.Configuration()
-            configuration.host = f"https://{credmgr_host}/"
+            configuration.host = f"https://{credmgr_host}/credmgr/"
             api_instance = swagger_client.ApiClient(configuration)
             self.tokens_api = swagger_client.TokensApi(api_client=api_instance)
             self.default_api = swagger_client.DefaultApi(api_client=api_instance)
             self.version_api = swagger_client.VersionApi(api_client=api_instance)
 
     def refresh(self, project_id: str, scope: str, refresh_token: str,
                 file_name: str = None) -> Tuple[Status, dict]:
@@ -124,15 +124,15 @@
     def clear_token_cache(self, *, file_name: str) -> Tuple[Status, Any]:
         """
         Clear cached token
         @param file_name name of the file containing the cached token
         @return STATUS.OK for success, STATUS.FAILURE and exception in case of failure
         """
         try:
-            with open(self.file_name, 'r') as stream:
+            with open(file_name, 'r') as stream:
                 token_data = json.loads(stream.read())
             if self.ID_TOKEN in token_data:
                 token_data.pop(self.ID_TOKEN)
             with atomic_write(file_name, overwrite=True) as f:
                 json.dump(token_data, f)
         except Exception as e:
             return Status.FAILURE, e
```

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/__init__.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/default_api.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/tokens_api.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api/version_api.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/api_client.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/configuration.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
         # Default Base url
-        self.host = "http://127.0.0.1:7000/"
+        self.host = "http://127.0.0.1:7000/credmgr/"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
```

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/__init__.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/jwks.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/jwks_keys.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/request.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status404_not_found.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/token.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/tokens.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/version.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/models/version_data.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_cm/credmgr/swagger_client/rest.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/fabric_credmgr_client.egg-info/PKG-INFO` & `fabric-credmgr-client-1.5.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 Metadata-Version: 2.1
 Name: fabric-credmgr-client
-Version: 1.3rc4
-Summary: Fabric Credential Manager API
-Home-page: 
-Author-email: kthare10@unc.edu
-Keywords: Swagger,Fabric Credential Manager API
+Version: 1.5.0rc1
+Summary: Fabric Control Framework
+Keywords: Fabric Credential Manager API
+Author-email: Komal Thareja <kthare10@renci.org>
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Requirements Status](https://requires.io/github/fabric-testbed/fabric_credmgr_client/requirements.svg?branch=master)](https://requires.io/github/fabric-testbed/fabric_credmgr_client/requirements/?branch=master)
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Dist: certifi >= 14.05.14
+Requires-Dist: six >= 1.10
+Requires-Dist: python_dateutil >= 2.5.3
+Requires-Dist: urllib3 >= 1.15.1
+Requires-Dist: atomicwrites
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: coverage>=4.0.3 ; extra == "test"
+Requires-Dist: nose>=1.3.7 ; extra == "test"
+Requires-Dist: pluggy>=0.3.1 ; extra == "test"
+Requires-Dist: py>=1.4.31 ; extra == "test"
+Requires-Dist: randomize>=0.13 ; extra == "test"
+Project-URL: Home, https://fabric-testbed.net/
+Project-URL: Sources, https://github.com/fabric-testbed/fabric_credmgr_client
+Provides-Extra: test
 
 [![PyPI](https://img.shields.io/pypi/v/fabric_credmgr_client?style=plastic)](https://pypi.org/project/fabric_credmgr_client/)
 
 # Fabric Credential Manager Client
 This is Fabric Credential Manager API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
@@ -129,7 +143,8 @@
 
  All endpoints do not require authorization.
 
 
 ## Author
 
 kthare10@unc.edu
+
```

### Comparing `fabric-credmgr-client-1.3rc4/test/test_default_api.py` & `fabric-credmgr-client-1.5.0rc1/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_jwks.py` & `fabric-credmgr-client-1.5.0rc1/test/test_jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_jwks_keys.py` & `fabric-credmgr-client-1.5.0rc1/test/test_jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_request.py` & `fabric-credmgr-client-1.5.0rc1/test/test_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status200_ok_no_content.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status200_ok_no_content_data.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status200_ok_single.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status400_bad_request.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status400_bad_request_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status401_unauthorized.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status401_unauthorized_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status403_forbidden.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status403_forbidden_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status404_not_found.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status404_not_found_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status500_internal_server_error.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_token.py` & `fabric-credmgr-client-1.5.0rc1/test/test_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_tokens.py` & `fabric-credmgr-client-1.5.0rc1/test/test_tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_tokens_api.py` & `fabric-credmgr-client-1.5.0rc1/test/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_version.py` & `fabric-credmgr-client-1.5.0rc1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_version_api.py` & `fabric-credmgr-client-1.5.0rc1/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.3rc4/test/test_version_data.py` & `fabric-credmgr-client-1.5.0rc1/test/test_version_data.py`

 * *Files identical despite different names*

