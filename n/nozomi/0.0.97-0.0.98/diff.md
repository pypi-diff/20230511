# Comparing `tmp/nozomi-0.0.97.tar.gz` & `tmp/nozomi-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nozomi-0.0.97.tar", last modified: Fri Mar 27 02:55:01 2020, max compression
+gzip compressed data, was "dist/nozomi-0.0.98.tar", last modified: Fri Mar 27 03:04:32 2020, max compression
```

## Comparing `nozomi-0.0.97.tar` & `nozomi-0.0.98.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/
--rw-r--r--   0 hugh       (501) staff       (20)     1312 2020-03-27 02:55:01.000000 nozomi-0.0.97/PKG-INFO
--rw-r--r--   0 hugh       (501) staff       (20)     1575 2020-01-06 22:11:31.000000 nozomi-0.0.97/setup.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi.egg-info/
--rw-r--r--   0 hugh       (501) staff       (20)     1312 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi.egg-info/PKG-INFO
--rw-r--r--   0 hugh       (501) staff       (20)     3037 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi.egg-info/SOURCES.txt
--rw-r--r--   0 hugh       (501) staff       (20)       19 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi.egg-info/requires.txt
--rw-r--r--   0 hugh       (501) staff       (20)        7 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi.egg-info/top_level.txt
--rw-r--r--   0 hugh       (501) staff       (20)        1 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi.egg-info/dependency_links.txt
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/temporal/
--rw-r--r--   0 hugh       (501) staff       (20)     3048 2020-03-05 06:48:02.000000 nozomi-0.0.97/nozomi/temporal/time.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/temporal/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)      348 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/temporal/tz_utc.py
--rw-r--r--   0 hugh       (501) staff       (20)     3073 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/temporal/date.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/app/
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/app/security/
--rw-r--r--   0 hugh       (501) staff       (20)     7885 2020-03-06 03:17:17.000000 nozomi-0.0.97/nozomi/app/security/session.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/app/security/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)       49 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/app/__init__.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/translation/
--rw-r--r--   0 hugh       (501) staff       (20)      825 2020-03-06 07:54:14.000000 nozomi-0.0.97/nozomi/translation/translated.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-03-09 04:51:56.000000 nozomi-0.0.97/nozomi/translation/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)      620 2020-03-06 07:54:15.000000 nozomi-0.0.97/nozomi/translation/text.py
--rw-r--r--   0 hugh       (501) staff       (20)     2790 2020-03-06 07:39:48.000000 nozomi-0.0.97/nozomi/translation/language.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/security/
--rw-r--r--   0 hugh       (501) staff       (20)     1615 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/cookies.py
--rw-r--r--   0 hugh       (501) staff       (20)      713 2020-02-26 05:27:26.000000 nozomi-0.0.97/nozomi/security/abstract_session.py
--rw-r--r--   0 hugh       (501) staff       (20)      651 2020-02-27 21:50:32.000000 nozomi-0.0.97/nozomi/security/read_protected.py
--rw-r--r--   0 hugh       (501) staff       (20)      652 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/perspective.py
--rw-r--r--   0 hugh       (501) staff       (20)     1247 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/credentials.py
--rw-r--r--   0 hugh       (501) staff       (20)      845 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/salt.py
--rw-r--r--   0 hugh       (501) staff       (20)     2138 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/standalone_agent.py
--rw-r--r--   0 hugh       (501) staff       (20)      854 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/considers_perspective.py
--rw-r--r--   0 hugh       (501) staff       (20)      970 2020-03-13 05:36:43.000000 nozomi-0.0.97/nozomi/security/random_number.py
--rw-r--r--   0 hugh       (501) staff       (20)     1354 2020-02-27 21:32:33.000000 nozomi-0.0.97/nozomi/security/protected.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)       89 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/privilege.py
--rw-r--r--   0 hugh       (501) staff       (20)     1679 2020-02-27 21:32:52.000000 nozomi-0.0.97/nozomi/security/broadcastable.py
--rw-r--r--   0 hugh       (501) staff       (20)     3916 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/secret.py
--rw-r--r--   0 hugh       (501) staff       (20)      440 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/machine_agent.py
--rw-r--r--   0 hugh       (501) staff       (20)      764 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/agent.py
--rw-r--r--   0 hugh       (501) staff       (20)     1773 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/ip_address.py
--rw-r--r--   0 hugh       (501) staff       (20)     1309 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/cors_policy.py
--rw-r--r--   0 hugh       (501) staff       (20)     1555 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/request_credentials.py
--rw-r--r--   0 hugh       (501) staff       (20)     3879 2020-03-03 08:26:00.000000 nozomi-0.0.97/nozomi/security/cookie_headers.py
--rw-r--r--   0 hugh       (501) staff       (20)     2767 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/permission_record.py
--rw-r--r--   0 hugh       (501) staff       (20)     1010 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/internal_key.py
--rw-r--r--   0 hugh       (501) staff       (20)     1455 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/access_control.py
--rw-r--r--   0 hugh       (501) staff       (20)     2038 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/security/forwarded_agent.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/resources/
--rw-r--r--   0 hugh       (501) staff       (20)     3003 2020-03-24 22:53:07.000000 nozomi-0.0.97/nozomi/resources/internal.py
--rw-r--r--   0 hugh       (501) staff       (20)     5172 2020-03-24 02:42:53.000000 nozomi-0.0.97/nozomi/resources/secure.py
--rw-r--r--   0 hugh       (501) staff       (20)     2492 2020-03-24 02:37:13.000000 nozomi-0.0.97/nozomi/resources/resource.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/resources/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     3278 2020-02-26 06:18:06.000000 nozomi-0.0.97/nozomi/resources/open.py
--rw-r--r--   0 hugh       (501) staff       (20)     3812 2020-03-24 02:43:51.000000 nozomi-0.0.97/nozomi/__init__.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/ancillary/
--rw-r--r--   0 hugh       (501) staff       (20)      603 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/ancillary/immutable.py
--rw-r--r--   0 hugh       (501) staff       (20)     1357 2020-03-03 07:39:17.000000 nozomi-0.0.97/nozomi/ancillary/configuration.py
--rw-r--r--   0 hugh       (501) staff       (20)     1014 2020-03-24 04:09:24.000000 nozomi-0.0.97/nozomi/ancillary/command_line.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/ancillary/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)      501 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/ancillary/server_name.py
--rw-r--r--   0 hugh       (501) staff       (20)     2354 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/ancillary/database_credentials.py
--rw-r--r--   0 hugh       (501) staff       (20)      316 2020-03-23 22:44:18.000000 nozomi-0.0.97/nozomi/ancillary/file_content.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/http/
--rw-r--r--   0 hugh       (501) staff       (20)      853 2020-03-13 04:53:22.000000 nozomi-0.0.97/nozomi/http/user_agent.py
--rw-r--r--   0 hugh       (501) staff       (20)     1108 2020-03-05 07:34:17.000000 nozomi-0.0.97/nozomi/http/url_parameters.py
--rw-r--r--   0 hugh       (501) staff       (20)      564 2020-03-05 07:34:30.000000 nozomi-0.0.97/nozomi/http/url_parameter.py
--rw-r--r--   0 hugh       (501) staff       (20)     4830 2020-03-05 07:45:00.000000 nozomi-0.0.97/nozomi/http/redirect.py
--rw-r--r--   0 hugh       (501) staff       (20)      210 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/http/query_string.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/http/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     1768 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/http/api_request.py
--rw-r--r--   0 hugh       (501) staff       (20)      508 2020-03-19 07:05:06.000000 nozomi-0.0.97/nozomi/http/status_code.py
--rw-r--r--   0 hugh       (501) staff       (20)     7260 2020-03-27 02:54:34.000000 nozomi-0.0.97/nozomi/http/parseable_data.py
--rw-r--r--   0 hugh       (501) staff       (20)      199 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/http/method.py
--rw-r--r--   0 hugh       (501) staff       (20)     2085 2020-03-25 00:28:57.000000 nozomi-0.0.97/nozomi/http/headers.py
--rw-r--r--   0 hugh       (501) staff       (20)     3307 2020-03-06 07:31:47.000000 nozomi-0.0.97/nozomi/http/accept_language.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/api/
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/api/security/
--rw-r--r--   0 hugh       (501) staff       (20)    10848 2020-02-16 00:09:05.000000 nozomi-0.0.97/nozomi/api/security/session.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/api/security/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)       48 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/api/__init__.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/rendering/
--rw-r--r--   0 hugh       (501) staff       (20)      564 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/javascript_class.py
--rw-r--r--   0 hugh       (501) staff       (20)     2200 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/static_context.py
--rw-r--r--   0 hugh       (501) staff       (20)     1236 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/render_dependency.py
--rw-r--r--   0 hugh       (501) staff       (20)      530 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/style.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     4010 2020-03-08 04:46:25.000000 nozomi-0.0.97/nozomi/rendering/context.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/rendering/view/
--rw-r--r--   0 hugh       (501) staff       (20)     2738 2020-03-06 04:56:38.000000 nozomi-0.0.97/nozomi/rendering/view/secure.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/view/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     5397 2020-03-06 04:53:45.000000 nozomi-0.0.97/nozomi/rendering/view/view.py
--rw-r--r--   0 hugh       (501) staff       (20)     3027 2020-03-06 04:54:50.000000 nozomi-0.0.97/nozomi/rendering/view/open.py
--rw-r--r--   0 hugh       (501) staff       (20)     1806 2020-03-06 03:45:53.000000 nozomi-0.0.97/nozomi/rendering/view/base.py
--rw-r--r--   0 hugh       (501) staff       (20)     1060 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/open_graph.py
--rw-r--r--   0 hugh       (501) staff       (20)      533 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/script.py
--rw-r--r--   0 hugh       (501) staff       (20)     1718 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/rendering/view_template.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/errors/
--rw-r--r--   0 hugh       (501) staff       (20)     3022 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/errors/error.py
--rw-r--r--   0 hugh       (501) staff       (20)      479 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/errors/not_found.py
--rw-r--r--   0 hugh       (501) staff       (20)      483 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/errors/bad_request.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/errors/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)      486 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/errors/not_authenticated.py
--rw-r--r--   0 hugh       (501) staff       (20)      513 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/errors/not_authorised.py
--rw-r--r--   0 hugh       (501) staff       (20)      486 2020-02-27 21:08:33.000000 nozomi-0.0.97/nozomi/errors/already_exists.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 02:55:01.000000 nozomi-0.0.97/nozomi/data/
--rw-r--r--   0 hugh       (501) staff       (20)     2062 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/query.py
--rw-r--r--   0 hugh       (501) staff       (20)     1485 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/order.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     1942 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/format.py
--rw-r--r--   0 hugh       (501) staff       (20)      943 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/abstract_encodable.py
--rw-r--r--   0 hugh       (501) staff       (20)     1594 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/encodable.py
--rw-r--r--   0 hugh       (501) staff       (20)     1466 2020-03-14 03:27:41.000000 nozomi-0.0.97/nozomi/data/limit.py
--rw-r--r--   0 hugh       (501) staff       (20)     1347 2020-03-14 03:27:38.000000 nozomi-0.0.97/nozomi/data/offset.py
--rw-r--r--   0 hugh       (501) staff       (20)      673 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/encoder.py
--rw-r--r--   0 hugh       (501) staff       (20)     1722 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/sql_conforming.py
--rw-r--r--   0 hugh       (501) staff       (20)      696 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/index_equitable.py
--rw-r--r--   0 hugh       (501) staff       (20)     2027 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/datastore.py
--rw-r--r--   0 hugh       (501) staff       (20)     2701 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/decodable.py
--rw-r--r--   0 hugh       (501) staff       (20)      695 2020-02-15 23:04:39.000000 nozomi-0.0.97/nozomi/data/index_sql_conforming.py
--rw-r--r--   0 hugh       (501) staff       (20)       59 2020-03-27 02:55:01.000000 nozomi-0.0.97/setup.cfg
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/
+-rw-r--r--   0 hugh       (501) staff       (20)     1312 2020-03-27 03:04:32.000000 nozomi-0.0.98/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)     1575 2020-01-06 22:11:31.000000 nozomi-0.0.98/setup.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi.egg-info/
+-rw-r--r--   0 hugh       (501) staff       (20)     1312 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi.egg-info/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)     3037 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi.egg-info/SOURCES.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       19 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi.egg-info/requires.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        7 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi.egg-info/top_level.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        1 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi.egg-info/dependency_links.txt
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/temporal/
+-rw-r--r--   0 hugh       (501) staff       (20)     3048 2020-03-05 06:48:02.000000 nozomi-0.0.98/nozomi/temporal/time.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/temporal/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)      348 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/temporal/tz_utc.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3073 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/temporal/date.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/app/
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/app/security/
+-rw-r--r--   0 hugh       (501) staff       (20)     7885 2020-03-06 03:17:17.000000 nozomi-0.0.98/nozomi/app/security/session.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/app/security/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)       49 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/app/__init__.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/translation/
+-rw-r--r--   0 hugh       (501) staff       (20)      825 2020-03-06 07:54:14.000000 nozomi-0.0.98/nozomi/translation/translated.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-03-09 04:51:56.000000 nozomi-0.0.98/nozomi/translation/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)      620 2020-03-06 07:54:15.000000 nozomi-0.0.98/nozomi/translation/text.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2790 2020-03-06 07:39:48.000000 nozomi-0.0.98/nozomi/translation/language.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/security/
+-rw-r--r--   0 hugh       (501) staff       (20)     1615 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/cookies.py
+-rw-r--r--   0 hugh       (501) staff       (20)      713 2020-02-26 05:27:26.000000 nozomi-0.0.98/nozomi/security/abstract_session.py
+-rw-r--r--   0 hugh       (501) staff       (20)      651 2020-02-27 21:50:32.000000 nozomi-0.0.98/nozomi/security/read_protected.py
+-rw-r--r--   0 hugh       (501) staff       (20)      652 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/perspective.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1247 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/credentials.py
+-rw-r--r--   0 hugh       (501) staff       (20)      845 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/salt.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2138 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/standalone_agent.py
+-rw-r--r--   0 hugh       (501) staff       (20)      854 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/considers_perspective.py
+-rw-r--r--   0 hugh       (501) staff       (20)      970 2020-03-13 05:36:43.000000 nozomi-0.0.98/nozomi/security/random_number.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1354 2020-02-27 21:32:33.000000 nozomi-0.0.98/nozomi/security/protected.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)       89 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/privilege.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1679 2020-02-27 21:32:52.000000 nozomi-0.0.98/nozomi/security/broadcastable.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3916 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/secret.py
+-rw-r--r--   0 hugh       (501) staff       (20)      440 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/machine_agent.py
+-rw-r--r--   0 hugh       (501) staff       (20)      764 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/agent.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1773 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/ip_address.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1309 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/cors_policy.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1555 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/request_credentials.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3879 2020-03-03 08:26:00.000000 nozomi-0.0.98/nozomi/security/cookie_headers.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2767 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/permission_record.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1010 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/internal_key.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1455 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/access_control.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2038 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/security/forwarded_agent.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/resources/
+-rw-r--r--   0 hugh       (501) staff       (20)     3003 2020-03-24 22:53:07.000000 nozomi-0.0.98/nozomi/resources/internal.py
+-rw-r--r--   0 hugh       (501) staff       (20)     5172 2020-03-24 02:42:53.000000 nozomi-0.0.98/nozomi/resources/secure.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2492 2020-03-24 02:37:13.000000 nozomi-0.0.98/nozomi/resources/resource.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/resources/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3278 2020-02-26 06:18:06.000000 nozomi-0.0.98/nozomi/resources/open.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3812 2020-03-24 02:43:51.000000 nozomi-0.0.98/nozomi/__init__.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/ancillary/
+-rw-r--r--   0 hugh       (501) staff       (20)      603 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/ancillary/immutable.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1357 2020-03-03 07:39:17.000000 nozomi-0.0.98/nozomi/ancillary/configuration.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1014 2020-03-24 04:09:24.000000 nozomi-0.0.98/nozomi/ancillary/command_line.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/ancillary/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)      501 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/ancillary/server_name.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2354 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/ancillary/database_credentials.py
+-rw-r--r--   0 hugh       (501) staff       (20)      316 2020-03-23 22:44:18.000000 nozomi-0.0.98/nozomi/ancillary/file_content.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/http/
+-rw-r--r--   0 hugh       (501) staff       (20)      853 2020-03-13 04:53:22.000000 nozomi-0.0.98/nozomi/http/user_agent.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1108 2020-03-05 07:34:17.000000 nozomi-0.0.98/nozomi/http/url_parameters.py
+-rw-r--r--   0 hugh       (501) staff       (20)      564 2020-03-05 07:34:30.000000 nozomi-0.0.98/nozomi/http/url_parameter.py
+-rw-r--r--   0 hugh       (501) staff       (20)     4830 2020-03-05 07:45:00.000000 nozomi-0.0.98/nozomi/http/redirect.py
+-rw-r--r--   0 hugh       (501) staff       (20)      210 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/http/query_string.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/http/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1768 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/http/api_request.py
+-rw-r--r--   0 hugh       (501) staff       (20)      508 2020-03-19 07:05:06.000000 nozomi-0.0.98/nozomi/http/status_code.py
+-rw-r--r--   0 hugh       (501) staff       (20)     7321 2020-03-27 03:04:08.000000 nozomi-0.0.98/nozomi/http/parseable_data.py
+-rw-r--r--   0 hugh       (501) staff       (20)      199 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/http/method.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2085 2020-03-25 00:28:57.000000 nozomi-0.0.98/nozomi/http/headers.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3307 2020-03-06 07:31:47.000000 nozomi-0.0.98/nozomi/http/accept_language.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/api/
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/api/security/
+-rw-r--r--   0 hugh       (501) staff       (20)    10848 2020-02-16 00:09:05.000000 nozomi-0.0.98/nozomi/api/security/session.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/api/security/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)       48 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/api/__init__.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/rendering/
+-rw-r--r--   0 hugh       (501) staff       (20)      564 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/javascript_class.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2200 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/static_context.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1236 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/render_dependency.py
+-rw-r--r--   0 hugh       (501) staff       (20)      530 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/style.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     4010 2020-03-08 04:46:25.000000 nozomi-0.0.98/nozomi/rendering/context.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/rendering/view/
+-rw-r--r--   0 hugh       (501) staff       (20)     2738 2020-03-06 04:56:38.000000 nozomi-0.0.98/nozomi/rendering/view/secure.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/view/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     5397 2020-03-06 04:53:45.000000 nozomi-0.0.98/nozomi/rendering/view/view.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3027 2020-03-06 04:54:50.000000 nozomi-0.0.98/nozomi/rendering/view/open.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1806 2020-03-06 03:45:53.000000 nozomi-0.0.98/nozomi/rendering/view/base.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1060 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/open_graph.py
+-rw-r--r--   0 hugh       (501) staff       (20)      533 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/script.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1718 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/rendering/view_template.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/errors/
+-rw-r--r--   0 hugh       (501) staff       (20)     3022 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/errors/error.py
+-rw-r--r--   0 hugh       (501) staff       (20)      479 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/errors/not_found.py
+-rw-r--r--   0 hugh       (501) staff       (20)      483 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/errors/bad_request.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/errors/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)      486 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/errors/not_authenticated.py
+-rw-r--r--   0 hugh       (501) staff       (20)      513 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/errors/not_authorised.py
+-rw-r--r--   0 hugh       (501) staff       (20)      486 2020-02-27 21:08:33.000000 nozomi-0.0.98/nozomi/errors/already_exists.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2020-03-27 03:04:32.000000 nozomi-0.0.98/nozomi/data/
+-rw-r--r--   0 hugh       (501) staff       (20)     2062 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/query.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1485 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/order.py
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1942 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/format.py
+-rw-r--r--   0 hugh       (501) staff       (20)      943 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/abstract_encodable.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1594 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/encodable.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1466 2020-03-14 03:27:41.000000 nozomi-0.0.98/nozomi/data/limit.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1347 2020-03-14 03:27:38.000000 nozomi-0.0.98/nozomi/data/offset.py
+-rw-r--r--   0 hugh       (501) staff       (20)      673 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/encoder.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1722 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/sql_conforming.py
+-rw-r--r--   0 hugh       (501) staff       (20)      696 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/index_equitable.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2027 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/datastore.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2701 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/decodable.py
+-rw-r--r--   0 hugh       (501) staff       (20)      695 2020-02-15 23:04:39.000000 nozomi-0.0.98/nozomi/data/index_sql_conforming.py
+-rw-r--r--   0 hugh       (501) staff       (20)       59 2020-03-27 03:04:32.000000 nozomi-0.0.98/setup.cfg
```

### Comparing `nozomi-0.0.97/PKG-INFO` & `nozomi-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nozomi
-Version: 0.0.97
+Version: 0.0.98
 Summary: HTTP web application & API protocol library
 Home-page: https://github.com/amatino-code/nozomi
 Author: Amatino
 Author-email: hugh@blinkybeach.com
 License: UNKNOWN
 Description: # Nozomi
```

### Comparing `nozomi-0.0.97/setup.py` & `nozomi-0.0.98/setup.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi.egg-info/PKG-INFO` & `nozomi-0.0.98/nozomi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nozomi
-Version: 0.0.97
+Version: 0.0.98
 Summary: HTTP web application & API protocol library
 Home-page: https://github.com/amatino-code/nozomi
 Author: Amatino
 Author-email: hugh@blinkybeach.com
 License: UNKNOWN
 Description: # Nozomi
```

### Comparing `nozomi-0.0.97/nozomi.egg-info/SOURCES.txt` & `nozomi-0.0.98/nozomi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/temporal/time.py` & `nozomi-0.0.98/nozomi/temporal/time.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/temporal/date.py` & `nozomi-0.0.98/nozomi/temporal/date.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/app/security/session.py` & `nozomi-0.0.98/nozomi/app/security/session.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/translation/translated.py` & `nozomi-0.0.98/nozomi/translation/translated.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/translation/text.py` & `nozomi-0.0.98/nozomi/translation/text.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/translation/language.py` & `nozomi-0.0.98/nozomi/translation/language.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/cookies.py` & `nozomi-0.0.98/nozomi/security/cookies.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/abstract_session.py` & `nozomi-0.0.98/nozomi/security/abstract_session.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/read_protected.py` & `nozomi-0.0.98/nozomi/security/read_protected.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/perspective.py` & `nozomi-0.0.98/nozomi/security/perspective.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/credentials.py` & `nozomi-0.0.98/nozomi/security/credentials.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/salt.py` & `nozomi-0.0.98/nozomi/security/salt.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/standalone_agent.py` & `nozomi-0.0.98/nozomi/security/standalone_agent.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/considers_perspective.py` & `nozomi-0.0.98/nozomi/security/considers_perspective.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/random_number.py` & `nozomi-0.0.98/nozomi/security/random_number.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/protected.py` & `nozomi-0.0.98/nozomi/security/protected.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/broadcastable.py` & `nozomi-0.0.98/nozomi/security/broadcastable.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/secret.py` & `nozomi-0.0.98/nozomi/security/secret.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/agent.py` & `nozomi-0.0.98/nozomi/security/agent.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/ip_address.py` & `nozomi-0.0.98/nozomi/security/ip_address.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/cors_policy.py` & `nozomi-0.0.98/nozomi/security/cors_policy.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/request_credentials.py` & `nozomi-0.0.98/nozomi/security/request_credentials.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/cookie_headers.py` & `nozomi-0.0.98/nozomi/security/cookie_headers.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/permission_record.py` & `nozomi-0.0.98/nozomi/security/permission_record.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/internal_key.py` & `nozomi-0.0.98/nozomi/security/internal_key.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/access_control.py` & `nozomi-0.0.98/nozomi/security/access_control.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/security/forwarded_agent.py` & `nozomi-0.0.98/nozomi/security/forwarded_agent.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/resources/internal.py` & `nozomi-0.0.98/nozomi/resources/internal.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/resources/secure.py` & `nozomi-0.0.98/nozomi/resources/secure.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/resources/resource.py` & `nozomi-0.0.98/nozomi/resources/resource.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/resources/open.py` & `nozomi-0.0.98/nozomi/resources/open.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/__init__.py` & `nozomi-0.0.98/nozomi/__init__.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/ancillary/immutable.py` & `nozomi-0.0.98/nozomi/ancillary/immutable.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/ancillary/configuration.py` & `nozomi-0.0.98/nozomi/ancillary/configuration.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/ancillary/command_line.py` & `nozomi-0.0.98/nozomi/ancillary/command_line.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/ancillary/database_credentials.py` & `nozomi-0.0.98/nozomi/ancillary/database_credentials.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/http/user_agent.py` & `nozomi-0.0.98/nozomi/http/user_agent.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/http/url_parameters.py` & `nozomi-0.0.98/nozomi/http/url_parameters.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/http/url_parameter.py` & `nozomi-0.0.98/nozomi/http/url_parameter.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/http/redirect.py` & `nozomi-0.0.98/nozomi/http/redirect.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/http/api_request.py` & `nozomi-0.0.98/nozomi/http/api_request.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/http/parseable_data.py` & `nozomi-0.0.98/nozomi/http/parseable_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,12 +250,15 @@
 
     def __len__(self):
         return len(self._keys)
 
     def __getitem__(self, key):
         return self._raw[key]
 
+    def __str__(self) -> str:
+        return str(self._raw)
+
     @classmethod
     def many(cls: Type[T], data: List[Any]) -> List[T]:
         if not isinstance(data, list):
             raise BadRequest('Expected array/sequence of data in body')
         return [cls(d) for d in data]
```

### Comparing `nozomi-0.0.97/nozomi/http/headers.py` & `nozomi-0.0.98/nozomi/http/headers.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/http/accept_language.py` & `nozomi-0.0.98/nozomi/http/accept_language.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/api/security/session.py` & `nozomi-0.0.98/nozomi/api/security/session.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/javascript_class.py` & `nozomi-0.0.98/nozomi/rendering/javascript_class.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/static_context.py` & `nozomi-0.0.98/nozomi/rendering/static_context.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/render_dependency.py` & `nozomi-0.0.98/nozomi/rendering/render_dependency.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/style.py` & `nozomi-0.0.98/nozomi/rendering/style.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/context.py` & `nozomi-0.0.98/nozomi/rendering/context.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/view/secure.py` & `nozomi-0.0.98/nozomi/rendering/view/secure.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/view/view.py` & `nozomi-0.0.98/nozomi/rendering/view/view.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/view/open.py` & `nozomi-0.0.98/nozomi/rendering/view/open.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/view/base.py` & `nozomi-0.0.98/nozomi/rendering/view/base.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/open_graph.py` & `nozomi-0.0.98/nozomi/rendering/open_graph.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/script.py` & `nozomi-0.0.98/nozomi/rendering/script.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/rendering/view_template.py` & `nozomi-0.0.98/nozomi/rendering/view_template.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/errors/error.py` & `nozomi-0.0.98/nozomi/errors/error.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/errors/not_authorised.py` & `nozomi-0.0.98/nozomi/errors/not_authorised.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/query.py` & `nozomi-0.0.98/nozomi/data/query.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/order.py` & `nozomi-0.0.98/nozomi/data/order.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/format.py` & `nozomi-0.0.98/nozomi/data/format.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/abstract_encodable.py` & `nozomi-0.0.98/nozomi/data/abstract_encodable.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/encodable.py` & `nozomi-0.0.98/nozomi/data/encodable.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/limit.py` & `nozomi-0.0.98/nozomi/data/limit.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/offset.py` & `nozomi-0.0.98/nozomi/data/offset.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/encoder.py` & `nozomi-0.0.98/nozomi/data/encoder.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/sql_conforming.py` & `nozomi-0.0.98/nozomi/data/sql_conforming.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/index_equitable.py` & `nozomi-0.0.98/nozomi/data/index_equitable.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/datastore.py` & `nozomi-0.0.98/nozomi/data/datastore.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/decodable.py` & `nozomi-0.0.98/nozomi/data/decodable.py`

 * *Files identical despite different names*

### Comparing `nozomi-0.0.97/nozomi/data/index_sql_conforming.py` & `nozomi-0.0.98/nozomi/data/index_sql_conforming.py`

 * *Files identical despite different names*

