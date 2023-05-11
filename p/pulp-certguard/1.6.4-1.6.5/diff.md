# Comparing `tmp/pulp-certguard-1.6.4.tar.gz` & `tmp/pulp-certguard-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-certguard-1.6.4.tar", last modified: Thu May  4 12:00:29 2023, max compression
+gzip compressed data, was "pulp-certguard-1.6.5.tar", last modified: Thu May 11 19:48:14 2023, max compression
```

## Comparing `pulp-certguard-1.6.4.tar` & `pulp-certguard-1.6.5.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.069920 pulp-certguard-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-05-04 12:00:26.000000 pulp-certguard-1.6.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-04 12:00:29.069920 pulp-certguard-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/ci_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.049920 pulp-certguard-1.6.4/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.053920 pulp-certguard-1.6.4/contrib/yum/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/contrib/yum/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/contrib/yum/README
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/contrib/yum/certguard.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/contrib/yum/certguard.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.057920 pulp-certguard-1.6.4/pulp_certguard/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.057920 pulp-certguard-1.6.4/pulp_certguard/app/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 12:00:27.000000 pulp-certguard-1.6.4/pulp_certguard/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.057920 pulp-certguard-1.6.4/pulp_certguard/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/app/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.057920 pulp-certguard-1.6.4/pulp_certguard/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.057920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.061920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/test_rhsm_certguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/test_x509_certguard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.053920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.061920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.061920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.061920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.061920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.061920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.061920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.065920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.065920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/genall.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/genca.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/genclient.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.069920 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/keys/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.069920 pulp-certguard-1.6.4/pulp_certguard/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pulp_certguard/tests/unit/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:00:29.057920 pulp-certguard-1.6.4/pulp_certguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-04 12:00:28.000000 pulp-certguard-1.6.4/pulp_certguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-04 12:00:29.000000 pulp-certguard-1.6.4/pulp_certguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:00:28.000000 pulp-certguard-1.6.4/pulp_certguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-04 12:00:28.000000 pulp-certguard-1.6.4/pulp_certguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:00:28.000000 pulp-certguard-1.6.4/pulp_certguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 12:00:28.000000 pulp-certguard-1.6.4/pulp_certguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:00:29.069920 pulp-certguard-1.6.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-05-04 12:00:27.000000 pulp-certguard-1.6.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:00:14.000000 pulp-certguard-1.6.4/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-11 19:48:12.000000 pulp-certguard-1.6.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/ci_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.858997 pulp-certguard-1.6.5/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.862997 pulp-certguard-1.6.5/contrib/yum/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/contrib/yum/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/contrib/yum/README
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/contrib/yum/certguard.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/contrib/yum/certguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.866997 pulp-certguard-1.6.5/pulp_certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.866997 pulp-certguard-1.6.5/pulp_certguard/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-11 19:48:13.000000 pulp-certguard-1.6.5/pulp_certguard/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.866997 pulp-certguard-1.6.5/pulp_certguard/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/app/migrations/0002_alter_rhsmcertguard_contentguard_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.866997 pulp-certguard-1.6.5/pulp_certguard/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.866997 pulp-certguard-1.6.5/pulp_certguard/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.866997 pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/test_rhsm_certguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/test_x509_certguard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.862997 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/genall.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/genca.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/genclient.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/pulp_certguard/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pulp_certguard/tests/unit/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:48:14.866997 pulp-certguard-1.6.5/pulp_certguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-11 19:48:14.000000 pulp-certguard-1.6.5/pulp_certguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-11 19:48:14.000000 pulp-certguard-1.6.5/pulp_certguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:48:14.000000 pulp-certguard-1.6.5/pulp_certguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 19:48:14.000000 pulp-certguard-1.6.5/pulp_certguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:48:14.000000 pulp-certguard-1.6.5/pulp_certguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 19:48:14.000000 pulp-certguard-1.6.5/pulp_certguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:48:14.870998 pulp-certguard-1.6.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-05-11 19:48:13.000000 pulp-certguard-1.6.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 19:48:01.000000 pulp-certguard-1.6.5/unittest_requirements.txt
```

### Comparing `pulp-certguard-1.6.4/CHANGES.rst` & `pulp-certguard-1.6.5/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,23 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.6.5 (2023-05-11)
+==================
+
+No significant changes.
+
+
+----
+
+
 1.6.4 (2023-05-04)
 ==================
 
 No significant changes.
 
 
 ----
```

### Comparing `pulp-certguard-1.6.4/COMMITMENT` & `pulp-certguard-1.6.5/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/COPYRIGHT` & `pulp-certguard-1.6.5/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/LICENSE` & `pulp-certguard-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/PKG-INFO` & `pulp-certguard-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-certguard
-Version: 1.6.4
+Version: 1.6.5
 Summary: Certguard plugin for the Pulp Project
 Home-page: https://docs.pulpproject.org/pulp_certguard/
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: pulp-certguard
         ==============
```

### Comparing `pulp-certguard-1.6.4/README.rst` & `pulp-certguard-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/contrib/yum/certguard.py` & `pulp-certguard-1.6.5/contrib/yum/certguard.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/app/migrations/0001_initial.py` & `pulp-certguard-1.6.5/pulp_certguard/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/app/models.py` & `pulp-certguard-1.6.5/pulp_certguard/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/app/serializers.py` & `pulp-certguard-1.6.5/pulp_certguard/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/app/utils.py` & `pulp-certguard-1.6.5/pulp_certguard/app/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/app/viewsets.py` & `pulp-certguard-1.6.5/pulp_certguard/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/__init__.py` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/base.py` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/base.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/test_rhsm_certguard.py` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/test_rhsm_certguard.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/api/test_x509_certguard.py` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/api/test_x509_certguard.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/genca.sh` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/genca.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/genclient.sh` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/genclient.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/constants.py` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard/tests/functional/utils.py` & `pulp-certguard-1.6.5/pulp_certguard/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/pulp_certguard.egg-info/PKG-INFO` & `pulp-certguard-1.6.5/pulp_certguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-certguard
-Version: 1.6.4
+Version: 1.6.5
 Summary: Certguard plugin for the Pulp Project
 Home-page: https://docs.pulpproject.org/pulp_certguard/
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: pulp-certguard
         ==============
```

### Comparing `pulp-certguard-1.6.4/pulp_certguard.egg-info/SOURCES.txt` & `pulp-certguard-1.6.5/pulp_certguard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 pulp_certguard.egg-info/top_level.txt
 pulp_certguard/app/__init__.py
 pulp_certguard/app/models.py
 pulp_certguard/app/serializers.py
 pulp_certguard/app/utils.py
 pulp_certguard/app/viewsets.py
 pulp_certguard/app/migrations/0001_initial.py
+pulp_certguard/app/migrations/0002_alter_rhsmcertguard_contentguard_ptr_and_more.py
 pulp_certguard/app/migrations/__init__.py
 pulp_certguard/tests/__init__.py
 pulp_certguard/tests/functional/__init__.py
 pulp_certguard/tests/functional/constants.py
 pulp_certguard/tests/functional/utils.py
 pulp_certguard/tests/functional/api/__init__.py
 pulp_certguard/tests/functional/api/base.py
```

### Comparing `pulp-certguard-1.6.4/pyproject.toml` & `pulp-certguard-1.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.4/setup.py` & `pulp-certguard-1.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="pulp-certguard",
-    version="1.6.4",
+    version="1.6.5",
     description="Certguard plugin for the Pulp Project",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-list@redhat.com",
     url="https://docs.pulpproject.org/pulp_certguard/",
     python_requires=">=3.8",
```

