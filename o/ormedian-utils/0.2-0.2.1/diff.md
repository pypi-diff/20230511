# Comparing `tmp/ormedian_utils-0.2.tar.gz` & `tmp/ormedian_utils-0.2.1.tar.gz`

## Comparing `ormedian_utils-0.2.tar` & `ormedian_utils-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,21 @@
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 ormedian_utils-0.2/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/.gitignore
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/modules.xml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/ormedian-utils.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ormedian_utils-0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    21725 2020-02-02 00:00:00.000000 ormedian_utils-0.2/previous_versions/ormedian_utils-0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0    22797 2020-02-02 00:00:00.000000 ormedian_utils-0.2/previous_versions/ormedian_utils-0.1.tar.gz
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/.DS_Store
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/__init__.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/.DS_Store
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/__init__.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/logger_config.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/move_spec_files.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/my_app_2022_09_07.log
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/resize_folders.py
--rw-r--r--   0        0        0    13039 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/resize_imgs.py
--rw-r--r--   0        0        0    18190 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/save_frames.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 ormedian_utils-0.2/src/ormedian_utils/video_folder.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ormedian_utils-0.2/LICENSE
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 ormedian_utils-0.2/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 ormedian_utils-0.2/pyproject.toml
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 ormedian_utils-0.2/PKG-INFO
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/requirements.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/.gitignore
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/misc.xml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/modules.xml
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/ormedian-utils.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/ormedian_utils/__init__.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/ormedian_utils/logger_config.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/ormedian_utils/move_spec_files.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/ormedian_utils/resize_folders.py
+-rw-r--r--   0        0        0    13325 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/ormedian_utils/resize_imgs.py
+-rw-r--r--   0        0        0    18637 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/ormedian_utils/save_frames.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/src/ormedian_utils/video_folder.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/README.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 ormedian_utils-0.2.1/PKG-INFO
```

### Comparing `ormedian_utils-0.2/requirements.txt` & `ormedian_utils-0.2.1/requirements.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-absl-py==0.15.0
-appdirs==1.4.4
-apturl==0.5.2
-argh==0.26.2
-argon2-cffi==21.3.0
-argon2-cffi-bindings==21.2.0
-asn1crypto==0.24.0
-astunparse==1.6.3
-async-generator==1.10
-atomicwrites==1.4.0
-attrs==22.1.0
-backcall==0.2.0
-backports.weakref==1.0.post1
-bkcharts==0.2
-black==19.10b0
-bleach==4.1.0
-boto==2.49.0
-Brlapi==0.6.6
-brotlipy==0.7.0
-build==0.8.0
-cachetools==4.2.4
-certifi==2020.12.5
-cffi==1.15.1
-chardet==3.0.4
-charset-normalizer==2.0.12
-click==6.7
-colorama==0.4.5
-command-not-found==0.3
-contextlib2==0.6.0.post1
-cryptography==2.1.4
-cupshelpers==1.0
-cycler==0.10.0
-cytoolz==0.11.0
-dataclasses==0.8
-decorator==5.1.1
-defer==1.0.6
-defusedxml==0.7.1
-distro-info===0.18ubuntu0.18.04.1
-docutils==0.18.1
-entrypoints==0.3
-et-xmlfile==1.0.1
-flatbuffers==1.12
-future==0.18.2
-gast==0.3.3
-google-auth==2.3.3
-google-auth-oauthlib==0.4.6
-google-pasta==0.2.0
-grpcio==1.32.0
-h5py==2.10.0
-HeapDict==1.0.1
-helpdev==0.7.1
-httplib2==0.9.2
-idna==2.6
-importlib-metadata==4.8.3
-importlib-resources==5.4.0
-iniconfig==1.1.1
-ipykernel==5.5.6
-ipython==7.16.3
-ipython-genutils==0.2.0
-ipywidgets==7.7.1
-jdcal==1.4.1
-jedi==0.17.2
-jeepney==0.7.1
-Jinja2==3.0.3
-joblib==1.1.0
-json5==0.9.5
-jsonschema==3.2.0
-jupyter==1.0.0
-jupyter-client==7.1.2
-jupyter-console==6.4.3
-jupyter-core==4.9.2
-jupyterlab-pygments==0.1.2
-jupyterlab-widgets==1.1.1
-Keras-Preprocessing==1.1.2
-keyring==23.4.1
-keyrings.alt==3.0
-kiwisolver==1.3.1
-language-selector==0.1
-launchpadlib==1.10.6
-lazr.restfulclient==0.13.5
-lazr.uri==1.0.3
-llvmlite==0.36.0
-locket==0.2.1
-louis==3.5.0
-macaroonbakery==1.1.3
-Mako==1.0.7
-Markdown==3.3.4
-MarkupSafe==2.0.1
-matplotlib==3.3.4
-mccabe==0.6.1
-mistune==0.8.4
-mpmath==1.2.1
-multipledispatch==0.6.0
-mypy-extensions==0.4.3
-nbclient==0.5.9
-nbconvert==6.0.7
-nbformat==5.1.3
-nest-asyncio==1.5.5
-netifaces==0.10.4
-notebook==6.4.10
-numexpr==2.8.1
-numpy==1.19.5
-oauth==1.0.1
-oauthlib==3.1.1
-olefile==0.46
-opencv-contrib-python==4.5.4.58
-opencv-python==4.5.4.58
-opt-einsum==3.3.0
-ormedian-resizer==0.0.1.4
-packaging==21.3
-pandocfilters==1.5.0
-parso==0.7.0
-pathspec==0.7.0
-patsy==0.5.1
-pbr==5.9.0
-pep517==0.13.0
-pep8==1.7.1
-pexpect==4.2.1
-pickleshare==0.7.5
-Pillow==8.4.0
-pkginfo==1.8.3
-pluggy==0.13.1
-ply==3.11
-prometheus-client==0.14.1
-prompt-toolkit==3.0.30
-protobuf==3.19.1
-ptyprocess==0.7.0
-py==1.11.0
-pyasn1==0.4.8
-pyasn1-modules==0.2.8
-pycairo==1.16.2
-pycparser==2.21
-pycrypto==2.6.1
-pycups==1.9.73
-Pygments==2.12.0
-PyGObject==3.26.1
-PyJWT==2.3.0
-pymacaroons==0.13.0
-PyNaCl==1.1.2
-pyparsing==3.0.9
-pyRFC3339==1.0
-pyrsistent==0.18.0
-pytest==6.2.3
-python-apt==1.6.5+ubuntu0.7
-python-dateutil==2.6.1
-python-debian==0.1.32
-pytz==2018.3
-pyxdg==0.25
-PyYAML==5.4.1
-pyzmq==20.0.0
-QDarkStyle==2.8.1
-qtconsole==5.2.2
-QtPy==1.9.0
-readme-renderer==34.0
-regex==2022.7.25
-reportlab==3.4.0
-requests==2.27.1
-requests-oauthlib==1.3.0
-requests-toolbelt==0.9.1
-requests-unixsocket==0.1.5
-rfc3986==1.5.0
-rsa==4.7.2
-scikit-learn==0.24.2
-scipy==1.5.4
-screen-resolution-extra==0.0.0
-SecretStorage==3.3.2
-Send2Trash==1.8.0
-simplegeneric==0.8.1
-simplejson==3.13.2
-six==1.15.0
-sklearn==0.0
-system-service==0.3
-systemd-python==234
-tables==3.6.1
-tensorboard==2.7.0
-tensorboard-data-server==0.6.1
-tensorboard-plugin-wit==1.8.0
-tensorflow==2.4.1
-tensorflow-estimator==2.4.0
-tensorflow-gpu==2.4.1
-termcolor==1.1.0
-terminado==0.9.4
-testpath==0.6.0
-testresources==2.0.1
-thop==0.0.31.post2005241907
-threadpoolctl==3.1.0
-toml==0.10.2
-tomli==1.2.3
-toolz==0.12.0
-torch==1.10.2
-tornado==6.1
-tqdm==4.64.0
-traitlets==4.3.3
-twilio==7.3.0
-twine==3.8.0
-typed-ast==1.5.4
-typing-extensions==3.7.4.3
-ubuntu-advantage-tools==27.9
-ubuntu-drivers-common==0.0.0
-ufw==0.36
-unattended-upgrades==0.1
-unicodecsv==0.14.1
-urllib3==1.26.11
-usb-creator==0.3.3
-wadllib==1.3.2
-wcwidth==0.2.5
-webencodings==0.5.1
-Werkzeug==2.0.3
-widgetsnbextension==3.5.1
-wrapt==1.12.1
-xkit==0.0.0
-xlwt==1.3.0
-xmltodict==0.12.0
-zict==2.0.0
-zipp==3.6.0
-zope.event==4.5.0
-zope.interface==4.3.2
+absl-py==0.15.0
+appdirs==1.4.4
+apturl==0.5.2
+argh==0.26.2
+argon2-cffi==21.3.0
+argon2-cffi-bindings==21.2.0
+asn1crypto==0.24.0
+astunparse==1.6.3
+async-generator==1.10
+atomicwrites==1.4.0
+attrs==22.1.0
+backcall==0.2.0
+backports.weakref==1.0.post1
+bkcharts==0.2
+black==19.10b0
+bleach==4.1.0
+boto==2.49.0
+Brlapi==0.6.6
+brotlipy==0.7.0
+build==0.8.0
+cachetools==4.2.4
+certifi==2020.12.5
+cffi==1.15.1
+chardet==3.0.4
+charset-normalizer==2.0.12
+click==6.7
+colorama==0.4.5
+command-not-found==0.3
+contextlib2==0.6.0.post1
+cryptography==2.1.4
+cupshelpers==1.0
+cycler==0.10.0
+cytoolz==0.11.0
+dataclasses==0.8
+decorator==5.1.1
+defer==1.0.6
+defusedxml==0.7.1
+distro-info===0.18ubuntu0.18.04.1
+docutils==0.18.1
+entrypoints==0.3
+et-xmlfile==1.0.1
+flatbuffers==1.12
+future==0.18.2
+gast==0.3.3
+google-auth==2.3.3
+google-auth-oauthlib==0.4.6
+google-pasta==0.2.0
+grpcio==1.32.0
+h5py==2.10.0
+HeapDict==1.0.1
+helpdev==0.7.1
+httplib2==0.9.2
+idna==2.6
+importlib-metadata==4.8.3
+importlib-resources==5.4.0
+iniconfig==1.1.1
+ipykernel==5.5.6
+ipython==7.16.3
+ipython-genutils==0.2.0
+ipywidgets==7.7.1
+jdcal==1.4.1
+jedi==0.17.2
+jeepney==0.7.1
+Jinja2==3.0.3
+joblib==1.1.0
+json5==0.9.5
+jsonschema==3.2.0
+jupyter==1.0.0
+jupyter-client==7.1.2
+jupyter-console==6.4.3
+jupyter-core==4.9.2
+jupyterlab-pygments==0.1.2
+jupyterlab-widgets==1.1.1
+Keras-Preprocessing==1.1.2
+keyring==23.4.1
+keyrings.alt==3.0
+kiwisolver==1.3.1
+language-selector==0.1
+launchpadlib==1.10.6
+lazr.restfulclient==0.13.5
+lazr.uri==1.0.3
+llvmlite==0.36.0
+locket==0.2.1
+louis==3.5.0
+macaroonbakery==1.1.3
+Mako==1.0.7
+Markdown==3.3.4
+MarkupSafe==2.0.1
+matplotlib==3.3.4
+mccabe==0.6.1
+mistune==0.8.4
+mpmath==1.2.1
+multipledispatch==0.6.0
+mypy-extensions==0.4.3
+nbclient==0.5.9
+nbconvert==6.0.7
+nbformat==5.1.3
+nest-asyncio==1.5.5
+netifaces==0.10.4
+notebook==6.4.10
+numexpr==2.8.1
+numpy==1.19.5
+oauth==1.0.1
+oauthlib==3.1.1
+olefile==0.46
+opencv-contrib-python==4.5.4.58
+opencv-python==4.5.4.58
+opt-einsum==3.3.0
+ormedian-resizer==0.0.1.4
+packaging==21.3
+pandocfilters==1.5.0
+parso==0.7.0
+pathspec==0.7.0
+patsy==0.5.1
+pbr==5.9.0
+pep517==0.13.0
+pep8==1.7.1
+pexpect==4.2.1
+pickleshare==0.7.5
+Pillow==8.4.0
+pkginfo==1.8.3
+pluggy==0.13.1
+ply==3.11
+prometheus-client==0.14.1
+prompt-toolkit==3.0.30
+protobuf==3.19.1
+ptyprocess==0.7.0
+py==1.11.0
+pyasn1==0.4.8
+pyasn1-modules==0.2.8
+pycairo==1.16.2
+pycparser==2.21
+pycrypto==2.6.1
+pycups==1.9.73
+Pygments==2.12.0
+PyGObject==3.26.1
+PyJWT==2.3.0
+pymacaroons==0.13.0
+PyNaCl==1.1.2
+pyparsing==3.0.9
+pyRFC3339==1.0
+pyrsistent==0.18.0
+pytest==6.2.3
+python-apt==1.6.5+ubuntu0.7
+python-dateutil==2.6.1
+python-debian==0.1.32
+pytz==2018.3
+pyxdg==0.25
+PyYAML==5.4.1
+pyzmq==20.0.0
+QDarkStyle==2.8.1
+qtconsole==5.2.2
+QtPy==1.9.0
+readme-renderer==34.0
+regex==2022.7.25
+reportlab==3.4.0
+requests==2.27.1
+requests-oauthlib==1.3.0
+requests-toolbelt==0.9.1
+requests-unixsocket==0.1.5
+rfc3986==1.5.0
+rsa==4.7.2
+scikit-learn==0.24.2
+scipy==1.5.4
+screen-resolution-extra==0.0.0
+SecretStorage==3.3.2
+Send2Trash==1.8.0
+simplegeneric==0.8.1
+simplejson==3.13.2
+six==1.15.0
+sklearn==0.0
+system-service==0.3
+systemd-python==234
+tables==3.6.1
+tensorboard==2.7.0
+tensorboard-data-server==0.6.1
+tensorboard-plugin-wit==1.8.0
+tensorflow==2.4.1
+tensorflow-estimator==2.4.0
+tensorflow-gpu==2.4.1
+termcolor==1.1.0
+terminado==0.9.4
+testpath==0.6.0
+testresources==2.0.1
+thop==0.0.31.post2005241907
+threadpoolctl==3.1.0
+toml==0.10.2
+tomli==1.2.3
+toolz==0.12.0
+torch==1.10.2
+tornado==6.1
+tqdm==4.64.0
+traitlets==4.3.3
+twilio==7.3.0
+twine==3.8.0
+typed-ast==1.5.4
+typing-extensions==3.7.4.3
+ubuntu-advantage-tools==27.9
+ubuntu-drivers-common==0.0.0
+ufw==0.36
+unattended-upgrades==0.1
+unicodecsv==0.14.1
+urllib3==1.26.11
+usb-creator==0.3.3
+wadllib==1.3.2
+wcwidth==0.2.5
+webencodings==0.5.1
+Werkzeug==2.0.3
+widgetsnbextension==3.5.1
+wrapt==1.12.1
+xkit==0.0.0
+xlwt==1.3.0
+xmltodict==0.12.0
+zict==2.0.0
+zipp==3.6.0
+zope.event==4.5.0
+zope.interface==4.3.2
```

### Comparing `ormedian_utils-0.2/.idea/inspectionProfiles/Project_Default.xml` & `ormedian_utils-0.2.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text*

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,129 @@
 00000000: 3c63 6f6d 706f 6e65 6e74 206e 616d 653d  <component name=
 00000010: 2249 6e73 7065 6374 696f 6e50 726f 6a65  "InspectionProje
 00000020: 6374 5072 6f66 696c 654d 616e 6167 6572  ctProfileManager
-00000030: 223e 0a20 203c 7072 6f66 696c 6520 7665  ">.  <profile ve
-00000040: 7273 696f 6e3d 2231 2e30 223e 0a20 2020  rsion="1.0">.   
-00000050: 203c 6f70 7469 6f6e 206e 616d 653d 226d   <option name="m
-00000060: 794e 616d 6522 2076 616c 7565 3d22 5072  yName" value="Pr
-00000070: 6f6a 6563 7420 4465 6661 756c 7422 202f  oject Default" /
-00000080: 3e0a 2020 2020 3c69 6e73 7065 6374 696f  >.    <inspectio
-00000090: 6e5f 746f 6f6c 2063 6c61 7373 3d22 5079  n_tool class="Py
-000000a0: 5061 636b 6167 6552 6571 7569 7265 6d65  PackageRequireme
-000000b0: 6e74 7349 6e73 7065 6374 696f 6e22 2065  ntsInspection" e
-000000c0: 6e61 626c 6564 3d22 7472 7565 2220 6c65  nabled="true" le
-000000d0: 7665 6c3d 2257 4152 4e49 4e47 2220 656e  vel="WARNING" en
-000000e0: 6162 6c65 645f 6279 5f64 6566 6175 6c74  abled_by_default
-000000f0: 3d22 7472 7565 223e 0a20 2020 2020 203c  ="true">.      <
-00000100: 6f70 7469 6f6e 206e 616d 653d 2269 676e  option name="ign
-00000110: 6f72 6564 5061 636b 6167 6573 223e 0a20  oredPackages">. 
-00000120: 2020 2020 2020 203c 7661 6c75 653e 0a20         <value>. 
-00000130: 2020 2020 2020 2020 203c 6c69 7374 2073           <list s
-00000140: 697a 653d 2232 223e 0a20 2020 2020 2020  ize="2">.       
-00000150: 2020 2020 203c 6974 656d 2069 6e64 6578       <item index
-00000160: 3d22 3022 2063 6c61 7373 3d22 6a61 7661  ="0" class="java
-00000170: 2e6c 616e 672e 5374 7269 6e67 2220 6974  .lang.String" it
-00000180: 656d 7661 6c75 653d 2264 6565 7064 6966  emvalue="deepdif
-00000190: 6622 202f 3e0a 2020 2020 2020 2020 2020  f" />.          
-000001a0: 2020 3c69 7465 6d20 696e 6465 783d 2231    <item index="1
-000001b0: 2220 636c 6173 733d 226a 6176 612e 6c61  " class="java.la
-000001c0: 6e67 2e53 7472 696e 6722 2069 7465 6d76  ng.String" itemv
-000001d0: 616c 7565 3d22 7465 7374 332d 6f72 6d65  alue="test3-orme
-000001e0: 6469 616e 2d72 6573 697a 6572 2220 2f3e  dian-resizer" />
-000001f0: 0a20 2020 2020 2020 2020 203c 2f6c 6973  .          </lis
-00000200: 743e 0a20 2020 2020 2020 203c 2f76 616c  t>.        </val
-00000210: 7565 3e0a 2020 2020 2020 3c2f 6f70 7469  ue>.      </opti
-00000220: 6f6e 3e0a 2020 2020 3c2f 696e 7370 6563  on>.    </inspec
-00000230: 7469 6f6e 5f74 6f6f 6c3e 0a20 2020 203c  tion_tool>.    <
-00000240: 696e 7370 6563 7469 6f6e 5f74 6f6f 6c20  inspection_tool 
-00000250: 636c 6173 733d 2250 7950 6570 3849 6e73  class="PyPep8Ins
-00000260: 7065 6374 696f 6e22 2065 6e61 626c 6564  pection" enabled
-00000270: 3d22 7472 7565 2220 6c65 7665 6c3d 2257  ="true" level="W
-00000280: 4541 4b20 5741 524e 494e 4722 2065 6e61  EAK WARNING" ena
-00000290: 626c 6564 5f62 795f 6465 6661 756c 743d  bled_by_default=
-000002a0: 2274 7275 6522 3e0a 2020 2020 2020 3c6f  "true">.      <o
-000002b0: 7074 696f 6e20 6e61 6d65 3d22 6967 6e6f  ption name="igno
-000002c0: 7265 6445 7272 6f72 7322 3e0a 2020 2020  redErrors">.    
-000002d0: 2020 2020 3c6c 6973 743e 0a20 2020 2020      <list>.     
-000002e0: 2020 2020 203c 6f70 7469 6f6e 2076 616c       <option val
-000002f0: 7565 3d22 5732 3922 202f 3e0a 2020 2020  ue="W29" />.    
-00000300: 2020 2020 2020 3c6f 7074 696f 6e20 7661        <option va
-00000310: 6c75 653d 2245 3530 3122 202f 3e0a 2020  lue="E501" />.  
-00000320: 2020 2020 2020 2020 3c6f 7074 696f 6e20          <option 
-00000330: 7661 6c75 653d 2257 3239 2220 2f3e 0a20  value="W29" />. 
-00000340: 2020 2020 2020 2020 203c 6f70 7469 6f6e           <option
-00000350: 2076 616c 7565 3d22 4535 3031 2220 2f3e   value="E501" />
-00000360: 0a20 2020 2020 2020 2020 203c 6f70 7469  .          <opti
-00000370: 6f6e 2076 616c 7565 3d22 5732 3922 202f  on value="W29" /
-00000380: 3e0a 2020 2020 2020 2020 2020 3c6f 7074  >.          <opt
-00000390: 696f 6e20 7661 6c75 653d 2245 3530 3122  ion value="E501"
-000003a0: 202f 3e0a 2020 2020 2020 2020 2020 3c6f   />.          <o
-000003b0: 7074 696f 6e20 7661 6c75 653d 2257 3239  ption value="W29
-000003c0: 2220 2f3e 0a20 2020 2020 2020 2020 203c  " />.          <
-000003d0: 6f70 7469 6f6e 2076 616c 7565 3d22 4535  option value="E5
-000003e0: 3031 2220 2f3e 0a20 2020 2020 2020 2020  01" />.         
-000003f0: 203c 6f70 7469 6f6e 2076 616c 7565 3d22   <option value="
-00000400: 5732 3922 202f 3e0a 2020 2020 2020 2020  W29" />.        
-00000410: 2020 3c6f 7074 696f 6e20 7661 6c75 653d    <option value=
-00000420: 2245 3530 3122 202f 3e0a 2020 2020 2020  "E501" />.      
-00000430: 2020 2020 3c6f 7074 696f 6e20 7661 6c75      <option valu
-00000440: 653d 2257 3239 2220 2f3e 0a20 2020 2020  e="W29" />.     
-00000450: 2020 2020 203c 6f70 7469 6f6e 2076 616c       <option val
-00000460: 7565 3d22 4535 3031 2220 2f3e 0a20 2020  ue="E501" />.   
-00000470: 2020 2020 2020 203c 6f70 7469 6f6e 2076         <option v
-00000480: 616c 7565 3d22 5732 3922 202f 3e0a 2020  alue="W29" />.  
-00000490: 2020 2020 2020 2020 3c6f 7074 696f 6e20          <option 
-000004a0: 7661 6c75 653d 2245 3530 3122 202f 3e0a  value="E501" />.
-000004b0: 2020 2020 2020 2020 2020 3c6f 7074 696f            <optio
-000004c0: 6e20 7661 6c75 653d 2257 3239 2220 2f3e  n value="W29" />
-000004d0: 0a20 2020 2020 2020 2020 203c 6f70 7469  .          <opti
-000004e0: 6f6e 2076 616c 7565 3d22 4535 3031 2220  on value="E501" 
-000004f0: 2f3e 0a20 2020 2020 2020 2020 203c 6f70  />.          <op
-00000500: 7469 6f6e 2076 616c 7565 3d22 5732 3922  tion value="W29"
-00000510: 202f 3e0a 2020 2020 2020 2020 2020 3c6f   />.          <o
-00000520: 7074 696f 6e20 7661 6c75 653d 2245 3530  ption value="E50
-00000530: 3122 202f 3e0a 2020 2020 2020 2020 2020  1" />.          
-00000540: 3c6f 7074 696f 6e20 7661 6c75 653d 2257  <option value="W
-00000550: 3239 2220 2f3e 0a20 2020 2020 2020 2020  29" />.         
-00000560: 203c 6f70 7469 6f6e 2076 616c 7565 3d22   <option value="
-00000570: 4535 3031 2220 2f3e 0a20 2020 2020 2020  E501" />.       
-00000580: 2020 203c 6f70 7469 6f6e 2076 616c 7565     <option value
-00000590: 3d22 5732 3922 202f 3e0a 2020 2020 2020  ="W29" />.      
-000005a0: 2020 2020 3c6f 7074 696f 6e20 7661 6c75      <option valu
-000005b0: 653d 2245 3530 3122 202f 3e0a 2020 2020  e="E501" />.    
-000005c0: 2020 2020 2020 3c6f 7074 696f 6e20 7661        <option va
-000005d0: 6c75 653d 2257 3239 2220 2f3e 0a20 2020  lue="W29" />.   
-000005e0: 2020 2020 2020 203c 6f70 7469 6f6e 2076         <option v
-000005f0: 616c 7565 3d22 4535 3031 2220 2f3e 0a20  alue="E501" />. 
-00000600: 2020 2020 2020 2020 203c 6f70 7469 6f6e           <option
-00000610: 2076 616c 7565 3d22 5732 3922 202f 3e0a   value="W29" />.
-00000620: 2020 2020 2020 2020 2020 3c6f 7074 696f            <optio
-00000630: 6e20 7661 6c75 653d 2245 3530 3122 202f  n value="E501" /
-00000640: 3e0a 2020 2020 2020 2020 2020 3c6f 7074  >.          <opt
-00000650: 696f 6e20 7661 6c75 653d 2257 3239 2220  ion value="W29" 
-00000660: 2f3e 0a20 2020 2020 2020 2020 203c 6f70  />.          <op
-00000670: 7469 6f6e 2076 616c 7565 3d22 4535 3031  tion value="E501
-00000680: 2220 2f3e 0a20 2020 2020 2020 203c 2f6c  " />.        </l
-00000690: 6973 743e 0a20 2020 2020 203c 2f6f 7074  ist>.      </opt
-000006a0: 696f 6e3e 0a20 2020 203c 2f69 6e73 7065  ion>.    </inspe
-000006b0: 6374 696f 6e5f 746f 6f6c 3e0a 2020 2020  ction_tool>.    
-000006c0: 3c69 6e73 7065 6374 696f 6e5f 746f 6f6c  <inspection_tool
-000006d0: 2063 6c61 7373 3d22 5079 5065 7038 4e61   class="PyPep8Na
-000006e0: 6d69 6e67 496e 7370 6563 7469 6f6e 2220  mingInspection" 
-000006f0: 656e 6162 6c65 643d 2274 7275 6522 206c  enabled="true" l
-00000700: 6576 656c 3d22 5745 414b 2057 4152 4e49  evel="WEAK WARNI
-00000710: 4e47 2220 656e 6162 6c65 645f 6279 5f64  NG" enabled_by_d
-00000720: 6566 6175 6c74 3d22 7472 7565 223e 0a20  efault="true">. 
-00000730: 2020 2020 203c 6f70 7469 6f6e 206e 616d       <option nam
-00000740: 653d 2269 676e 6f72 6564 4572 726f 7273  e="ignoredErrors
-00000750: 223e 0a20 2020 2020 2020 203c 6c69 7374  ">.        <list
-00000760: 3e0a 2020 2020 2020 2020 2020 3c6f 7074  >.          <opt
-00000770: 696f 6e20 7661 6c75 653d 224e 3830 3622  ion value="N806"
-00000780: 202f 3e0a 2020 2020 2020 2020 3c2f 6c69   />.        </li
-00000790: 7374 3e0a 2020 2020 2020 3c2f 6f70 7469  st>.      </opti
-000007a0: 6f6e 3e0a 2020 2020 3c2f 696e 7370 6563  on>.    </inspec
-000007b0: 7469 6f6e 5f74 6f6f 6c3e 0a20 203c 2f70  tion_tool>.  </p
-000007c0: 726f 6669 6c65 3e0a 3c2f 636f 6d70 6f6e  rofile>.</compon
-000007d0: 656e 743e                                ent>
+00000030: 223e 0d0a 2020 3c70 726f 6669 6c65 2076  ">..  <profile v
+00000040: 6572 7369 6f6e 3d22 312e 3022 3e0d 0a20  ersion="1.0">.. 
+00000050: 2020 203c 6f70 7469 6f6e 206e 616d 653d     <option name=
+00000060: 226d 794e 616d 6522 2076 616c 7565 3d22  "myName" value="
+00000070: 5072 6f6a 6563 7420 4465 6661 756c 7422  Project Default"
+00000080: 202f 3e0d 0a20 2020 203c 696e 7370 6563   />..    <inspec
+00000090: 7469 6f6e 5f74 6f6f 6c20 636c 6173 733d  tion_tool class=
+000000a0: 2250 7950 6163 6b61 6765 5265 7175 6972  "PyPackageRequir
+000000b0: 656d 656e 7473 496e 7370 6563 7469 6f6e  ementsInspection
+000000c0: 2220 656e 6162 6c65 643d 2274 7275 6522  " enabled="true"
+000000d0: 206c 6576 656c 3d22 5741 524e 494e 4722   level="WARNING"
+000000e0: 2065 6e61 626c 6564 5f62 795f 6465 6661   enabled_by_defa
+000000f0: 756c 743d 2274 7275 6522 3e0d 0a20 2020  ult="true">..   
+00000100: 2020 203c 6f70 7469 6f6e 206e 616d 653d     <option name=
+00000110: 2269 676e 6f72 6564 5061 636b 6167 6573  "ignoredPackages
+00000120: 223e 0d0a 2020 2020 2020 2020 3c76 616c  ">..        <val
+00000130: 7565 3e0d 0a20 2020 2020 2020 2020 203c  ue>..          <
+00000140: 6c69 7374 2073 697a 653d 2232 223e 0d0a  list size="2">..
+00000150: 2020 2020 2020 2020 2020 2020 3c69 7465              <ite
+00000160: 6d20 696e 6465 783d 2230 2220 636c 6173  m index="0" clas
+00000170: 733d 226a 6176 612e 6c61 6e67 2e53 7472  s="java.lang.Str
+00000180: 696e 6722 2069 7465 6d76 616c 7565 3d22  ing" itemvalue="
+00000190: 6465 6570 6469 6666 2220 2f3e 0d0a 2020  deepdiff" />..  
+000001a0: 2020 2020 2020 2020 2020 3c69 7465 6d20            <item 
+000001b0: 696e 6465 783d 2231 2220 636c 6173 733d  index="1" class=
+000001c0: 226a 6176 612e 6c61 6e67 2e53 7472 696e  "java.lang.Strin
+000001d0: 6722 2069 7465 6d76 616c 7565 3d22 7465  g" itemvalue="te
+000001e0: 7374 332d 6f72 6d65 6469 616e 2d72 6573  st3-ormedian-res
+000001f0: 697a 6572 2220 2f3e 0d0a 2020 2020 2020  izer" />..      
+00000200: 2020 2020 3c2f 6c69 7374 3e0d 0a20 2020      </list>..   
+00000210: 2020 2020 203c 2f76 616c 7565 3e0d 0a20       </value>.. 
+00000220: 2020 2020 203c 2f6f 7074 696f 6e3e 0d0a       </option>..
+00000230: 2020 2020 3c2f 696e 7370 6563 7469 6f6e      </inspection
+00000240: 5f74 6f6f 6c3e 0d0a 2020 2020 3c69 6e73  _tool>..    <ins
+00000250: 7065 6374 696f 6e5f 746f 6f6c 2063 6c61  pection_tool cla
+00000260: 7373 3d22 5079 5065 7038 496e 7370 6563  ss="PyPep8Inspec
+00000270: 7469 6f6e 2220 656e 6162 6c65 643d 2274  tion" enabled="t
+00000280: 7275 6522 206c 6576 656c 3d22 5745 414b  rue" level="WEAK
+00000290: 2057 4152 4e49 4e47 2220 656e 6162 6c65   WARNING" enable
+000002a0: 645f 6279 5f64 6566 6175 6c74 3d22 7472  d_by_default="tr
+000002b0: 7565 223e 0d0a 2020 2020 2020 3c6f 7074  ue">..      <opt
+000002c0: 696f 6e20 6e61 6d65 3d22 6967 6e6f 7265  ion name="ignore
+000002d0: 6445 7272 6f72 7322 3e0d 0a20 2020 2020  dErrors">..     
+000002e0: 2020 203c 6c69 7374 3e0d 0a20 2020 2020     <list>..     
+000002f0: 2020 2020 203c 6f70 7469 6f6e 2076 616c       <option val
+00000300: 7565 3d22 5732 3922 202f 3e0d 0a20 2020  ue="W29" />..   
+00000310: 2020 2020 2020 203c 6f70 7469 6f6e 2076         <option v
+00000320: 616c 7565 3d22 4535 3031 2220 2f3e 0d0a  alue="E501" />..
+00000330: 2020 2020 2020 2020 2020 3c6f 7074 696f            <optio
+00000340: 6e20 7661 6c75 653d 2257 3239 2220 2f3e  n value="W29" />
+00000350: 0d0a 2020 2020 2020 2020 2020 3c6f 7074  ..          <opt
+00000360: 696f 6e20 7661 6c75 653d 2245 3530 3122  ion value="E501"
+00000370: 202f 3e0d 0a20 2020 2020 2020 2020 203c   />..          <
+00000380: 6f70 7469 6f6e 2076 616c 7565 3d22 5732  option value="W2
+00000390: 3922 202f 3e0d 0a20 2020 2020 2020 2020  9" />..         
+000003a0: 203c 6f70 7469 6f6e 2076 616c 7565 3d22   <option value="
+000003b0: 4535 3031 2220 2f3e 0d0a 2020 2020 2020  E501" />..      
+000003c0: 2020 2020 3c6f 7074 696f 6e20 7661 6c75      <option valu
+000003d0: 653d 2257 3239 2220 2f3e 0d0a 2020 2020  e="W29" />..    
+000003e0: 2020 2020 2020 3c6f 7074 696f 6e20 7661        <option va
+000003f0: 6c75 653d 2245 3530 3122 202f 3e0d 0a20  lue="E501" />.. 
+00000400: 2020 2020 2020 2020 203c 6f70 7469 6f6e           <option
+00000410: 2076 616c 7565 3d22 5732 3922 202f 3e0d   value="W29" />.
+00000420: 0a20 2020 2020 2020 2020 203c 6f70 7469  .          <opti
+00000430: 6f6e 2076 616c 7565 3d22 4535 3031 2220  on value="E501" 
+00000440: 2f3e 0d0a 2020 2020 2020 2020 2020 3c6f  />..          <o
+00000450: 7074 696f 6e20 7661 6c75 653d 2257 3239  ption value="W29
+00000460: 2220 2f3e 0d0a 2020 2020 2020 2020 2020  " />..          
+00000470: 3c6f 7074 696f 6e20 7661 6c75 653d 2245  <option value="E
+00000480: 3530 3122 202f 3e0d 0a20 2020 2020 2020  501" />..       
+00000490: 2020 203c 6f70 7469 6f6e 2076 616c 7565     <option value
+000004a0: 3d22 5732 3922 202f 3e0d 0a20 2020 2020  ="W29" />..     
+000004b0: 2020 2020 203c 6f70 7469 6f6e 2076 616c       <option val
+000004c0: 7565 3d22 4535 3031 2220 2f3e 0d0a 2020  ue="E501" />..  
+000004d0: 2020 2020 2020 2020 3c6f 7074 696f 6e20          <option 
+000004e0: 7661 6c75 653d 2257 3239 2220 2f3e 0d0a  value="W29" />..
+000004f0: 2020 2020 2020 2020 2020 3c6f 7074 696f            <optio
+00000500: 6e20 7661 6c75 653d 2245 3530 3122 202f  n value="E501" /
+00000510: 3e0d 0a20 2020 2020 2020 2020 203c 6f70  >..          <op
+00000520: 7469 6f6e 2076 616c 7565 3d22 5732 3922  tion value="W29"
+00000530: 202f 3e0d 0a20 2020 2020 2020 2020 203c   />..          <
+00000540: 6f70 7469 6f6e 2076 616c 7565 3d22 4535  option value="E5
+00000550: 3031 2220 2f3e 0d0a 2020 2020 2020 2020  01" />..        
+00000560: 2020 3c6f 7074 696f 6e20 7661 6c75 653d    <option value=
+00000570: 2257 3239 2220 2f3e 0d0a 2020 2020 2020  "W29" />..      
+00000580: 2020 2020 3c6f 7074 696f 6e20 7661 6c75      <option valu
+00000590: 653d 2245 3530 3122 202f 3e0d 0a20 2020  e="E501" />..   
+000005a0: 2020 2020 2020 203c 6f70 7469 6f6e 2076         <option v
+000005b0: 616c 7565 3d22 5732 3922 202f 3e0d 0a20  alue="W29" />.. 
+000005c0: 2020 2020 2020 2020 203c 6f70 7469 6f6e           <option
+000005d0: 2076 616c 7565 3d22 4535 3031 2220 2f3e   value="E501" />
+000005e0: 0d0a 2020 2020 2020 2020 2020 3c6f 7074  ..          <opt
+000005f0: 696f 6e20 7661 6c75 653d 2257 3239 2220  ion value="W29" 
+00000600: 2f3e 0d0a 2020 2020 2020 2020 2020 3c6f  />..          <o
+00000610: 7074 696f 6e20 7661 6c75 653d 2245 3530  ption value="E50
+00000620: 3122 202f 3e0d 0a20 2020 2020 2020 2020  1" />..         
+00000630: 203c 6f70 7469 6f6e 2076 616c 7565 3d22   <option value="
+00000640: 5732 3922 202f 3e0d 0a20 2020 2020 2020  W29" />..       
+00000650: 2020 203c 6f70 7469 6f6e 2076 616c 7565     <option value
+00000660: 3d22 4535 3031 2220 2f3e 0d0a 2020 2020  ="E501" />..    
+00000670: 2020 2020 2020 3c6f 7074 696f 6e20 7661        <option va
+00000680: 6c75 653d 2257 3239 2220 2f3e 0d0a 2020  lue="W29" />..  
+00000690: 2020 2020 2020 2020 3c6f 7074 696f 6e20          <option 
+000006a0: 7661 6c75 653d 2245 3530 3122 202f 3e0d  value="E501" />.
+000006b0: 0a20 2020 2020 2020 203c 2f6c 6973 743e  .        </list>
+000006c0: 0d0a 2020 2020 2020 3c2f 6f70 7469 6f6e  ..      </option
+000006d0: 3e0d 0a20 2020 203c 2f69 6e73 7065 6374  >..    </inspect
+000006e0: 696f 6e5f 746f 6f6c 3e0d 0a20 2020 203c  ion_tool>..    <
+000006f0: 696e 7370 6563 7469 6f6e 5f74 6f6f 6c20  inspection_tool 
+00000700: 636c 6173 733d 2250 7950 6570 384e 616d  class="PyPep8Nam
+00000710: 696e 6749 6e73 7065 6374 696f 6e22 2065  ingInspection" e
+00000720: 6e61 626c 6564 3d22 7472 7565 2220 6c65  nabled="true" le
+00000730: 7665 6c3d 2257 4541 4b20 5741 524e 494e  vel="WEAK WARNIN
+00000740: 4722 2065 6e61 626c 6564 5f62 795f 6465  G" enabled_by_de
+00000750: 6661 756c 743d 2274 7275 6522 3e0d 0a20  fault="true">.. 
+00000760: 2020 2020 203c 6f70 7469 6f6e 206e 616d       <option nam
+00000770: 653d 2269 676e 6f72 6564 4572 726f 7273  e="ignoredErrors
+00000780: 223e 0d0a 2020 2020 2020 2020 3c6c 6973  ">..        <lis
+00000790: 743e 0d0a 2020 2020 2020 2020 2020 3c6f  t>..          <o
+000007a0: 7074 696f 6e20 7661 6c75 653d 224e 3830  ption value="N80
+000007b0: 3622 202f 3e0d 0a20 2020 2020 2020 203c  6" />..        <
+000007c0: 2f6c 6973 743e 0d0a 2020 2020 2020 3c2f  /list>..      </
+000007d0: 6f70 7469 6f6e 3e0d 0a20 2020 203c 2f69  option>..    </i
+000007e0: 6e73 7065 6374 696f 6e5f 746f 6f6c 3e0d  nspection_tool>.
+000007f0: 0a20 203c 2f70 726f 6669 6c65 3e0d 0a3c  .  </profile>..<
+00000800: 2f63 6f6d 706f 6e65 6e74 3e              /component>
```

### Comparing `ormedian_utils-0.2/src/ormedian_utils/logger_config.py` & `ormedian_utils-0.2.1/src/ormedian_utils/logger_config.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import logging
-import itertools
-import time
-import sys
-from colorama import Fore
-
-
-class CustomFormatter(logging.Formatter):
-    """Logging colored formatter, adapted from https://stackoverflow.com/a/56944256/3638629"""
-
-    grey = '\x1b[38;21m'
-    blue = '\x1b[38;5;39m'
-    yellow = '\x1b[38;5;226m'
-    red = '\x1b[38;5;196m'
-    bold_red = '\x1b[31;1m'
-    unk = '\x1b[38;5;40m'
-    reset = '\x1b[0m'
-
-    def __init__(self, fmt):
-        super().__init__()
-        self.fmt = fmt
-        self.FORMATS = {
-            logging.DEBUG: self.grey + self.fmt + self.reset,
-            logging.INFO: self.blue + self.fmt + self.reset,
-            logging.WARNING: self.yellow + self.fmt + self.reset,
-            logging.ERROR: self.red + self.fmt + self.reset,
-            logging.CRITICAL: self.bold_red + self.fmt + self.reset
-        }
-
-    def format(self, record):
-        log_fmt = self.FORMATS.get(record.levelno)
-        formatter = logging.Formatter(log_fmt)
-        return formatter.format(record)
-
-
-# done = False
-
-def animate(done=True):
-    for c in itertools.cycle(['||||||', '/', '-----', '\\']):
-        if done:
-            break
-        sys.stdout.write('\rloading ' + c)
-        sys.stdout.flush()
-        time.sleep(0.1)
-    sys.stdout.write('\rDone!     ')
-
-
-def animated_exit(someText):
-    print(Fore.RED + someText, end='');
-    for i in range(10):
-        print(Fore.RED + '|||||', end='')
-        time.sleep(0.1)
+import logging
+import itertools
+import time
+import sys
+from colorama import Fore
+
+
+class CustomFormatter(logging.Formatter):
+    """Logging colored formatter, adapted from https://stackoverflow.com/a/56944256/3638629"""
+
+    grey = '\x1b[38;21m'
+    blue = '\x1b[38;5;39m'
+    yellow = '\x1b[38;5;226m'
+    red = '\x1b[38;5;196m'
+    bold_red = '\x1b[31;1m'
+    unk = '\x1b[38;5;40m'
+    reset = '\x1b[0m'
+
+    def __init__(self, fmt):
+        super().__init__()
+        self.fmt = fmt
+        self.FORMATS = {
+            logging.DEBUG: self.grey + self.fmt + self.reset,
+            logging.INFO: self.blue + self.fmt + self.reset,
+            logging.WARNING: self.yellow + self.fmt + self.reset,
+            logging.ERROR: self.red + self.fmt + self.reset,
+            logging.CRITICAL: self.bold_red + self.fmt + self.reset
+        }
+
+    def format(self, record):
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = logging.Formatter(log_fmt)
+        return formatter.format(record)
+
+
+# done = False
+
+def animate(done=True):
+    for c in itertools.cycle(['||||||', '/', '-----', '\\']):
+        if done:
+            break
+        sys.stdout.write('\rloading ' + c)
+        sys.stdout.flush()
+        time.sleep(0.1)
+    sys.stdout.write('\rDone!     ')
+
+
+def animated_exit(someText):
+    print(Fore.RED + someText, end='');
+    for i in range(10):
+        print(Fore.RED + '|||||', end='')
+        time.sleep(0.1)
```

### Comparing `ormedian_utils-0.2/src/ormedian_utils/move_spec_files.py` & `ormedian_utils-0.2.1/src/ormedian_utils/move_spec_files.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import os
-import time
-from glob import glob
-import shutil
-from pathlib import Path
-from tqdm import tqdm
-from colorama import Fore
-from datetime import datetime
-
-from .logger_config import animated_exit
-from .save_frames import logger
-
-
-def filemover(folder_path: str, file_ext: str, new_folder: str):
-    """
-    :param new_folder: Name of new folder to move files to
-    :param file_ext: extension of file to move e.g csv, json
-    :param folder_path: Path to the parent folder containing files to move
-    :return:
-    """
-    if not os.path.exists(Path(folder_path)):
-        logger.error(f'{folder_path} DOES NOT EXIST PLEASE PROVIDE A VALID FOLDER PATH ')
-        exit()
-    if file_ext[0] !=0:
-        file_ext = f'.{file_ext}'
-    else:
-        pass
-    file_list = [Path(x).suffix for x in os.listdir(folder_path)]
-    if not file_ext in file_list:
-        logger.exception(f'{folder_path} does not contain any {file_ext} file\n', exc_info=False)
-        return
-
-    parent_folder = os.path.dirname(Path(folder_path))  # parent directory of input folder
-    n_folder = os.path.join(parent_folder, new_folder)  # path for files to move
-    time.sleep(1.0)
-
-    if not os.path.exists(n_folder):
-        os.mkdir(n_folder)  # make directory for folder if not already existing
-    else:
-        logger.debug(f'{n_folder} IS AN EXISTING PATH')
-        # animated_exit('CHANGING FOLDER NAME')
-        new_folder_name = f'{new_folder}_{datetime.now().strftime("%H.%M.%S")}'
-        n_folder = os.path.join(parent_folder, new_folder_name)
-        os.mkdir(n_folder)
-        animated_exit('CHANGING FOLDER NAME')
-        logger.info(f'\nNEW_FOLDER NAME: {new_folder_name}')
-    logger.info(f'YOUR FILES WILL BE MOVED to {n_folder}')
-    files_to_move = glob(os.path.join(folder_path, f'*{file_ext}'))
-    files_to_move = tqdm(files_to_move)
-
-    i = 0
-    for f in files_to_move:
-        i += 1
-        shutil.move(f, n_folder)
-        time.sleep(.05)
-        files_to_move.set_description(f'{i} {file_ext[1::]} files moved\n')
-
-    msg_print = f'==========================================================================\n' \
-                f'-------------------------MOVED FILE STATISTICS------------------------ \n' \
-                f'--------------------------------------------------------------------------\n'
-    f_moved = f'{file_ext[1::]}'
-    msg_image_path = f'files were moved from:'
-    fol_path = f'{folder_path}'
-    image_folder_print = f'\n        to     {n_folder}                           \n'
-    space_u = f'==========================================================================\n'
-    total_msg = f'Total Number of Files moved:    '
-    total_number = f'                                {i} '
-    space_b = f'\n=========================================================================='
-
-    print(Fore.CYAN, msg_print, end='')
-    print(Fore.GREEN, f_moved, end='')
-    print(Fore.LIGHTWHITE_EX, msg_image_path, end='')
-    print(Fore.RED, fol_path)
-    print(Fore.RED, image_folder_print, end='')
-    print(Fore.CYAN, space_u, end='')
-    print(Fore.GREEN, total_msg, end='')
-    print(Fore.RED, total_number, end='')
-    print(Fore.CYAN, space_b)
-
-
+import os
+import time
+from glob import glob
+import shutil
+from pathlib import Path
+from tqdm import tqdm
+from colorama import Fore
+from datetime import datetime
+
+from .logger_config import animated_exit
+from .save_frames import logger
+
+
+def filemover(folder_path: str, file_ext: str, new_folder: str):
+    """
+    :param new_folder: Name of new folder to move files to
+    :param file_ext: extension of file to move e.g csv, json
+    :param folder_path: Path to the parent folder containing files to move
+    :return:
+    """
+    if not os.path.exists(Path(folder_path)):
+        logger.error(f'{folder_path} DOES NOT EXIST PLEASE PROVIDE A VALID FOLDER PATH ')
+        exit()
+    if file_ext[0] !=0:
+        file_ext = f'.{file_ext}'
+    else:
+        pass
+    file_list = [Path(x).suffix for x in os.listdir(folder_path)]
+    if not file_ext in file_list:
+        logger.exception(f'{folder_path} does not contain any {file_ext} file\n', exc_info=False)
+        return
+
+    parent_folder = os.path.dirname(Path(folder_path))  # parent directory of input folder
+    n_folder = os.path.join(parent_folder, new_folder)  # path for files to move
+    time.sleep(1.0)
+
+    if not os.path.exists(n_folder):
+        os.mkdir(n_folder)  # make directory for folder if not already existing
+    else:
+        logger.debug(f'{n_folder} IS AN EXISTING PATH')
+        # animated_exit('CHANGING FOLDER NAME')
+        new_folder_name = f'{new_folder}_{datetime.now().strftime("%H.%M.%S")}'
+        n_folder = os.path.join(parent_folder, new_folder_name)
+        os.mkdir(n_folder)
+        animated_exit('CHANGING FOLDER NAME')
+        logger.info(f'\nNEW_FOLDER NAME: {new_folder_name}')
+    logger.info(f'YOUR FILES WILL BE MOVED to {n_folder}')
+    files_to_move = glob(os.path.join(folder_path, f'*{file_ext}'))
+    files_to_move = tqdm(files_to_move)
+
+    i = 0
+    for f in files_to_move:
+        i += 1
+        shutil.move(f, n_folder)
+        time.sleep(.05)
+        files_to_move.set_description(f'{i} {file_ext[1::]} files moved\n')
+
+    msg_print = f'==========================================================================\n' \
+                f'-------------------------MOVED FILE STATISTICS------------------------ \n' \
+                f'--------------------------------------------------------------------------\n'
+    f_moved = f'{file_ext[1::]}'
+    msg_image_path = f'files were moved from:'
+    fol_path = f'{folder_path}'
+    image_folder_print = f'\n        to     {n_folder}                           \n'
+    space_u = f'==========================================================================\n'
+    total_msg = f'Total Number of Files moved:    '
+    total_number = f'                                {i} '
+    space_b = f'\n=========================================================================='
+
+    print(Fore.CYAN, msg_print, end='')
+    print(Fore.GREEN, f_moved, end='')
+    print(Fore.LIGHTWHITE_EX, msg_image_path, end='')
+    print(Fore.RED, fol_path)
+    print(Fore.RED, image_folder_print, end='')
+    print(Fore.CYAN, space_u, end='')
+    print(Fore.GREEN, total_msg, end='')
+    print(Fore.RED, total_number, end='')
+    print(Fore.CYAN, space_b)
+
+
 # filemover('/Users/solua1/Documents/D', 'pdf', 'MovedFiles')
```

### Comparing `ormedian_utils-0.2/src/ormedian_utils/resize_folders.py` & `ormedian_utils-0.2.1/src/ormedian_utils/resize_folders.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import time
-
-import cv2
-import os
-from pathlib import Path
-
-from colorama import Fore
-
-from .logger_config import animated_exit
-from .save_frames import logger
-
-
-def resizer(new_size,
-            image_path,
-            img_ext, new_folder, img_cnt):
-    img_dirs = os.listdir(image_path)
-    total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
-    i = img_cnt
-    for img in img_dirs:
-        img_e = Path(img).suffix
-        exact_image_path = os.path.join(image_path, img)
-
-        if img_e not in img_ext:
-            # print(f'\033[1;31;40m {img} Skipped! not a supported image file ')
-            logger.debug(f'\033[1;31;40m {img} Skipped! not a supported image file ')
-            pass
-        else:
-            if not os.path.isfile(exact_image_path):
-                print(f'\033[1;31;40m {exact_image_path} Skipped! not a supported image file')
-                pass
-            imgs = cv2.imread(exact_image_path, cv2.IMREAD_UNCHANGED)
-
-            Resized_img = cv2.resize(imgs, new_size)
-            if i % 20 == 0:
-                logger.info(f'{i} Images resized; New Size: {Resized_img.shape[0]} x {Resized_img.shape[1]}')
-                # print(f'\033[1;33;40m New size of {img}: {Resized_img.size[0]} x {Resized_img.size[1]}')1
-            else:
-                pass
-
-            if not os.path.exists(new_folder):
-                os.mkdir(new_folder)
-            image_file = os.path.join(new_folder, f'{i}.jpg')
-            # print(image_file)
-            cv2.imwrite(f'{image_file}', Resized_img)
-            i += 1
-            cv2.waitKey(1)
-            if i == total_img_len or (cv2.waitKey(1) & 0xFF == 27):
-                cv2.destroyAllWindows()
-                break
-            else:
-                pass
-
-    return i
-
-
-def resize_all(new_size:tuple, folder_path:str):
-    """
-    Takes folder_path: a directory containing folders with images, resize and save the images into a single folder.
-    Images resized are in form 1.jpg, 2.jpg .....n.jpg
-    :param new_size: expected size of the new images, accepts only tuple e.g (100, 100)
-    :param folder_path: Directory containing folders with images
-    :return:
-    """
-    img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.eps', '.raw', '.svg', '.bmp', '.dib']
-    # Path cleaning section ==> 1. Check if sub folders are directories
-    # 2. create a dictionary to house folders and number of images they contain
-    folders = [f.path for f in os.scandir(folder_path) if f.is_dir() and Path(f)]
-    fold_with_img = {}
-    total_img_len = 0
-    for f in folders:
-        fold_with_img[f] = 0
-
-        for f_ in os.listdir(f):
-            if Path(f_).suffix in img_ext:
-                fold_with_img[f] += 1
-                total_img_len += 1
-            else:
-                pass
-
-    logger.debug(f'TOTAL IMAGES to RESIZE: {total_img_len}')
-    msg_print = f'\n==========================================================================\n' \
-                f'-------------------------FOLDER STATISTICS-------------------------------- \n' \
-                f'--------------------------------------------------------------------------\n'
-    folder_path_print = f'FOLDERS with IMAGES:\n'
-    space_u = f'\n==========================================================================\n'
-    #
-    total_msg = f'Total Images in Sub Folders  : '
-    total_number = f'               {total_img_len} '
-    space_b = f'\n=========================================================================='
-
-    print(Fore.LIGHTBLUE_EX, msg_print, end='')
-    print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-    for fold, d in fold_with_img.items():
-        print(Fore.RED, f'                {fold} ', end='')
-        print(Fore.GREEN, f'{d} Images')
-    print(Fore.LIGHTBLUE_EX, space_u, end='')
-    print(Fore.LIGHTBLUE_EX, total_msg, end='')
-    print(Fore.GREEN, total_number, end='')
-    print(Fore.LIGHTBLUE_EX, space_b)
-    time.sleep(2.0)
-    animated_exit('STARTING RESIZE')
-    print('')
-
-    path_dirname = os.listdir(folder_path)
-    parent_name = Path(folder_path).parent
-    img_count = 0
-    Resized_folder = os.path.join(parent_name, 'Resized')
-    # print(f'RESIZED FOLDER: {Resized_folder}')
-    for folder in path_dirname:
-        folder_resizer = os.path.join(folder_path, folder)
-        if not os.path.isdir(folder_resizer):
-            animated_exit(f'{folder_resizer} NOT A DIRECTORY, IGNORING')
-            print('')
-            pass
-        else:
-            logger.info(f'RESIZING IMAGES in {folder}')
-            img_count = resizer(new_size, folder_resizer, img_ext, Resized_folder, img_count)
-            img_count += 0
-            print(f'{img_count} IMAGES RESIZED')
-    #
-    msg_print = f'\n==========================================================================\n' \
-                f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
-                f'--------------------------------------------------------------------------\n'
-    folder_path_print = f'Resized Images Folder:\n'
-    new_image_size = f'New Image Size:'
-
-    space_u = f'\n==========================================================================\n'
-
-    total_msg = f'Total Resized Images  : '
-    total_number = f'             {img_count} '
-    space_b = f'\n=========================================================================='
-    print(Fore.LIGHTBLUE_EX, msg_print, end='')
-    print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-    # for fold in Resized_folder:
-    #     print(Fore.RED, f'      {fold}')
-    print(Fore.GREEN, f'                {Resized_folder}')
-    print(Fore.LIGHTBLUE_EX, f'{new_image_size}', end='')
-    print(Fore.YELLOW, new_size, end='')
-    print(Fore.LIGHTBLUE_EX, space_u, end='')
-    print(Fore.LIGHTBLUE_EX, total_msg, end='')
-    print(Fore.YELLOW, total_number, end='')
-    print(Fore.LIGHTBLUE_EX, space_b)
-    cv2.destroyAllWindows()
-    cv2.waitKey(1)
-
-
+import time
+
+import cv2
+import os
+from pathlib import Path
+
+from colorama import Fore
+
+from .logger_config import animated_exit
+from .save_frames import logger
+
+
+def resizer(new_size,
+            image_path,
+            img_ext, new_folder, img_cnt):
+    img_dirs = os.listdir(image_path)
+    total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
+    i = img_cnt
+    for img in img_dirs:
+        img_e = Path(img).suffix
+        exact_image_path = os.path.join(image_path, img)
+
+        if img_e not in img_ext:
+            # print(f'\033[1;31;40m {img} Skipped! not a supported image file ')
+            logger.debug(f'\033[1;31;40m {img} Skipped! not a supported image file ')
+            pass
+        else:
+            if not os.path.isfile(exact_image_path):
+                print(f'\033[1;31;40m {exact_image_path} Skipped! not a supported image file')
+                pass
+            imgs = cv2.imread(exact_image_path, cv2.IMREAD_UNCHANGED)
+
+            Resized_img = cv2.resize(imgs, new_size)
+            if i % 20 == 0:
+                logger.info(f'{i} Images resized; New Size: {Resized_img.shape[0]} x {Resized_img.shape[1]}')
+                # print(f'\033[1;33;40m New size of {img}: {Resized_img.size[0]} x {Resized_img.size[1]}')1
+            else:
+                pass
+
+            if not os.path.exists(new_folder):
+                os.mkdir(new_folder)
+            image_file = os.path.join(new_folder, f'{i}.jpg')
+            # print(image_file)
+            cv2.imwrite(f'{image_file}', Resized_img)
+            i += 1
+            cv2.waitKey(1)
+            if i == total_img_len or (cv2.waitKey(1) & 0xFF == 27):
+                cv2.destroyAllWindows()
+                break
+            else:
+                pass
+
+    return i
+
+
+def resize_all(new_size:tuple, folder_path:str):
+    """
+    Takes folder_path: a directory containing folders with images, resize and save the images into a single folder.
+    Images resized are in form 1.jpg, 2.jpg .....n.jpg
+    :param new_size: expected size of the new images, accepts only tuple e.g (100, 100)
+    :param folder_path: Directory containing folders with images
+    :return:
+    """
+    img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.eps', '.raw', '.svg', '.bmp', '.dib']
+    # Path cleaning section ==> 1. Check if sub folders are directories
+    # 2. create a dictionary to house folders and number of images they contain
+    folders = [f.path for f in os.scandir(folder_path) if f.is_dir() and Path(f)]
+    fold_with_img = {}
+    total_img_len = 0
+    for f in folders:
+        fold_with_img[f] = 0
+
+        for f_ in os.listdir(f):
+            if Path(f_).suffix in img_ext:
+                fold_with_img[f] += 1
+                total_img_len += 1
+            else:
+                pass
+
+    logger.debug(f'TOTAL IMAGES to RESIZE: {total_img_len}')
+    msg_print = f'\n==========================================================================\n' \
+                f'-------------------------FOLDER STATISTICS-------------------------------- \n' \
+                f'--------------------------------------------------------------------------\n'
+    folder_path_print = f'FOLDERS with IMAGES:\n'
+    space_u = f'\n==========================================================================\n'
+    #
+    total_msg = f'Total Images in Sub Folders  : '
+    total_number = f'               {total_img_len} '
+    space_b = f'\n=========================================================================='
+
+    print(Fore.LIGHTBLUE_EX, msg_print, end='')
+    print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+    for fold, d in fold_with_img.items():
+        print(Fore.RED, f'                {fold} ', end='')
+        print(Fore.GREEN, f'{d} Images')
+    print(Fore.LIGHTBLUE_EX, space_u, end='')
+    print(Fore.LIGHTBLUE_EX, total_msg, end='')
+    print(Fore.GREEN, total_number, end='')
+    print(Fore.LIGHTBLUE_EX, space_b)
+    time.sleep(2.0)
+    animated_exit('STARTING RESIZE')
+    print('')
+
+    path_dirname = os.listdir(folder_path)
+    parent_name = Path(folder_path).parent
+    img_count = 0
+    Resized_folder = os.path.join(parent_name, 'Resized')
+    # print(f'RESIZED FOLDER: {Resized_folder}')
+    for folder in path_dirname:
+        folder_resizer = os.path.join(folder_path, folder)
+        if not os.path.isdir(folder_resizer):
+            animated_exit(f'{folder_resizer} NOT A DIRECTORY, IGNORING')
+            print('')
+            pass
+        else:
+            logger.info(f'RESIZING IMAGES in {folder}')
+            img_count = resizer(new_size, folder_resizer, img_ext, Resized_folder, img_count)
+            img_count += 0
+            print(f'{img_count} IMAGES RESIZED')
+    #
+    msg_print = f'\n==========================================================================\n' \
+                f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
+                f'--------------------------------------------------------------------------\n'
+    folder_path_print = f'Resized Images Folder:\n'
+    new_image_size = f'New Image Size:'
+
+    space_u = f'\n==========================================================================\n'
+
+    total_msg = f'Total Resized Images  : '
+    total_number = f'             {img_count} '
+    space_b = f'\n=========================================================================='
+    print(Fore.LIGHTBLUE_EX, msg_print, end='')
+    print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+    # for fold in Resized_folder:
+    #     print(Fore.RED, f'      {fold}')
+    print(Fore.GREEN, f'                {Resized_folder}')
+    print(Fore.LIGHTBLUE_EX, f'{new_image_size}', end='')
+    print(Fore.YELLOW, new_size, end='')
+    print(Fore.LIGHTBLUE_EX, space_u, end='')
+    print(Fore.LIGHTBLUE_EX, total_msg, end='')
+    print(Fore.YELLOW, total_number, end='')
+    print(Fore.LIGHTBLUE_EX, space_b)
+    cv2.destroyAllWindows()
+    cv2.waitKey(1)
+
+
```

### Comparing `ormedian_utils-0.2/src/ormedian_utils/resize_imgs.py` & `ormedian_utils-0.2.1/src/ormedian_utils/resize_imgs.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-import time
-
-import os
-from pathlib import Path
-import cv2
-from colorama import Fore
-
-from .logger_config import animated_exit
-from .save_frames import logger
-
-
-def image_resizer(new_size: tuple,
-                  image_path: str,
-                  n_f=True, new_folder='ResizedImages',
-                  view=True, multiple_folders=False):
-    """
-    :param multiple_folders: Set True if the image path contains multiple folders containing images
-    :param view: if True, there would display window showing resized images
-    :param new_size: New Image size e.g (224, 224)
-    :param image_path: '/path/to/where/images/are
-    :param new_folder: '/Specify/new/folder
-    :param args: at the moment you can specify either jpg or png
-    :return: New image resized to new_size
-    """
-    Resized_folder = ""
-    img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.eps', '.raw', '.svg', '.bmp', '.dib']
-
-    path_dirname = os.path.dirname(image_path)
-    if n_f and not multiple_folders:
-        total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
-        logger.critical(f'{total_img_len} total Images found in \033[1;34;40m {image_path}\n')
-        time.sleep(0.5)
-        Resized_folder = os.path.join(path_dirname, new_folder)
-        if not os.path.exists(Resized_folder):
-            os.mkdir(Resized_folder)
-        image_path = Path(image_path)
-
-        Resized_folder = os.path.join(path_dirname, new_folder)
-        if not os.path.exists(Resized_folder):
-            os.mkdir(Resized_folder)
-        else:
-            print('WARNING!!! IMAGE FOLDER ALREADY EXISTS, OVERRIDING')
-            pass
-        tot_img = resizer(new_size, image_path, img_ext, Resized_folder, view)
-        logger.info('IMAGES RESIZE DONE!!!')
-        animated_exit('COMPUTING STATS')
-
-        msg_print = f'\n==========================================================================\n' \
-                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
-                    f'--------------------------------------------------------------------------\n'
-        folder_path_print = f'Resized Images Folder:\n'
-        new_image_size = f'New Image Size:'
-
-        space_u = f'\n==========================================================================\n'
-
-        total_msg = f'Total Resized Images  : '
-        total_number = f'               {tot_img} '
-        space_b = f'\n=========================================================================='
-        print(Fore.LIGHTBLUE_EX, msg_print, end='')
-        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-        # for new_fol in Resized_folder:
-        print(Fore.RED, f'      {Resized_folder}')
-        # print(Fore.RED, f'{Resized_folder}', end='')
-        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
-        print(Fore.RED, new_size, end='')
-        # print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
-        # print(Fore.MAGENTA, image_folder_print, end='')
-        print(Fore.LIGHTBLUE_EX, space_u, end='')
-        print(Fore.LIGHTBLUE_EX, total_msg, end='')
-        print(Fore.RED, total_number, end='')
-        print(Fore.LIGHTBLUE_EX, space_b)
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
-
-        # tot_img = resizer(new_size, image_path, Resized_folder, view, )
-
-    elif not n_f and not multiple_folders:
-
-        total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
-        logger.critical(f'{total_img_len} total Images found in \033[1;34;40m {image_path}\n')
-        time.sleep(0.5)
-
-        Resized_folder = image_path
-
-        tot_img = resizer(new_size, image_path, img_ext, Resized_folder, view)
-        logger.info('IMAGES RESIZE DONE!!!')
-        animated_exit('COMPUTING STATS')
-
-        msg_print = f'\n==========================================================================\n' \
-                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
-                    f'--------------------------------------------------------------------------\n'
-        folder_path_print = f'Resized Images Folder:\n'
-        new_image_size = f'New Image Size:'
-
-        space_u = f'\n==========================================================================\n'
-
-        total_msg = f'Total Resized Images  : '
-        total_number = f'               {tot_img} '
-        space_b = f'\n=========================================================================='
-        print(Fore.LIGHTBLUE_EX, msg_print, end='')
-        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-
-        print(Fore.RED, f'      {Resized_folder}')
-        # print(Fore.RED, f'{Resized_folder}', end='')
-        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
-        print(Fore.RED, new_size, end='')
-        # print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
-        # print(Fore.MAGENTA, image_folder_print, end='')
-        print(Fore.LIGHTBLUE_EX, space_u, end='')
-        print(Fore.LIGHTBLUE_EX, total_msg, end='')
-        print(Fore.RED, total_number, end='')
-        print(Fore.LIGHTBLUE_EX, space_b)
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
-
-    elif not n_f and multiple_folders:
-        image_subfolders = [f.path for f in os.scandir(image_path) if f.is_dir()]  # prints out paths/subfolders
-        total_img_len = len([x for y in image_subfolders for x in os.listdir(y) if Path(x).suffix in img_ext])
-        logger.warning(f'THIS WILL OVERWRITE IMAGES IN THE CURRENT FOLDERS')
-        logger.critical(f'{total_img_len} total Images found in {(Fore.BLUE, image_path)}\n')
-
-        Resized_folder = image_subfolders
-        image_subfolders = [f.path for f in os.scandir(image_path) if f.is_dir()]  # prints out paths/subfolders
-
-        list_indx = 0
-        tot_img = 0
-        for img_fold in image_subfolders:
-            logger.critical(f'RESIZING {img_fold} FOLDER')
-            logger.critical(f'SAVING RESIZED IMAGES into EXISTING folder {img_fold}')
-            tot_img_ = resizer(new_size, img_fold, img_ext, img_fold, view)
-
-            # tot_img_ = resizer(new_size, img_fold, img_fold, view, )
-            time.sleep(0.5)
-            list_indx += 1
-            tot_img += tot_img_
-            if list_indx >= len(image_subfolders):
-                break
-        logger.info('IMAGES RESIZE DONE!!!')
-        animated_exit('COMPUTING STATS')
-
-        msg_print = f'\n==========================================================================\n' \
-                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
-                    f'--------------------------------------------------------------------------\n'
-        folder_path_print = f'Resized Images Folder:\n'
-        new_image_size = f'New Image Size:'
-
-        space_u = f'\n==========================================================================\n'
-
-        total_msg = f'Total Resized Images  : '
-        total_number = f'               {tot_img} '
-        space_b = f'\n=========================================================================='
-        print(Fore.LIGHTBLUE_EX, msg_print, end='')
-        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-        # for new_fol in Resized_folder:
-        for fold in Resized_folder:
-            print(Fore.RED, f'      {fold}')
-        # print(Fore.RED, f'{Resized_folder}', end='')
-        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
-        print(Fore.RED, new_size, end='')
-        # print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
-        # print(Fore.MAGENTA, image_folder_print, end='')
-        print(Fore.LIGHTBLUE_EX, space_u, end='')
-        print(Fore.LIGHTBLUE_EX, total_msg, end='')
-        print(Fore.RED, total_number, end='')
-        print(Fore.LIGHTBLUE_EX, space_b)
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
-    else:
-        Resized_folder = os.path.join(path_dirname, new_folder)
-        if not os.path.exists(Resized_folder):
-            os.mkdir(Resized_folder)
-        else:
-            print(f'WARNING! {Resized_folder} ALREADY EXISTS, USING EXISTING FOLDER PRESS ESC TO STOP');
-            time.sleep(2.0)
-            if cv2.waitKey(1) & 0xFF == 27: exit()
-
-        image_subfolders = [f.path for f in os.scandir(image_path) if f.is_dir()]  # prints out paths/subfolders
-        total_img_len = len([x for y in image_subfolders for x in os.listdir(y) if Path(x).suffix in img_ext])
-        logger.critical(f'{total_img_len} total Images found in \033[1;34;40m {image_path}\n')
-        subfolder_names = [f.name for f in os.scandir(image_path) if f.is_dir()]  # outputs only the subfolder names
-
-        list_indx = 0
-        tot_img = 0
-        Res_folders = []
-        for img_fold in image_subfolders:
-            logger.critical(f'NOW RESIZING {img_fold}')
-            Resized_folder_ = os.path.join(Resized_folder, subfolder_names[list_indx])
-
-            Res_folders.append(Resized_folder_)
-            if not os.path.exists(Resized_folder_):
-                os.mkdir(Resized_folder_)
-            else:
-                animated_exit(
-                    f'IMAGE FOLDER ALREADY EXISTS,\n OVERRIDING EXISTING FILES IN {Resized_folder_}\n PRESS Esc to Exit');
-                time.sleep(2.0)
-                if cv2.waitKey(1) & 0xFF == 27:
-                    break
-                else:
-                    pass
-            logger.info(f'SAVING INTO {Resized_folder_} FOLDER')
-            tot_img_ = resizer(new_size, img_fold, img_ext, Resized_folder_, view)
-
-            # tot_img_ = resizer(new_size, img_fold, Resized_folder_, view, )
-            list_indx += 1
-            tot_img += tot_img_
-            if list_indx >= len(image_subfolders):
-                cv2.destroyAllWindows()
-                cv2.waitKey(1)
-                break
-        Resized_folder = Res_folders
-        logger.info('IMAGES RESIZE DONE!!!')
-        animated_exit('COMPUTING STATS')
-
-        msg_print = f'\n==========================================================================\n' \
-                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
-                    f'--------------------------------------------------------------------------\n'
-        folder_path_print = f'Resized Images Folder:\n'
-        new_image_size = f'New Image Size:'
-
-        space_u = f'\n==========================================================================\n'
-
-        total_msg = f'Total Resized Images  : '
-        total_number = f'               {tot_img} '
-        space_b = f'\n=========================================================================='
-        print(Fore.LIGHTBLUE_EX, msg_print, end='')
-        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-        for fold in Resized_folder:
-            print(Fore.RED, f'      {fold}')
-        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
-        print(Fore.RED, new_size, end='')
-        print(Fore.LIGHTBLUE_EX, space_u, end='')
-        print(Fore.LIGHTBLUE_EX, total_msg, end='')
-        print(Fore.RED, total_number, end='')
-        print(Fore.LIGHTBLUE_EX, space_b)
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
-
-
-def resizer(new_size,
-            image_path,
-            img_ext, new_folder,
-            view):
-    img_dirs = os.listdir(image_path)
-    # img_extend = [x for x in os.listdir(image_path) if Path(x).suffix in img_ext]
-    total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
-    i = 0
-    for img in img_dirs:
-        img_e = Path(img).suffix
-        exact_image_path = os.path.join(image_path, img)
-
-        if img_e not in img_ext:
-            print(f'\033[1;31;40m {img} Skipped! not a supported image file ')
-            pass
-        else:
-            if not os.path.isfile(exact_image_path):
-                print(f'\033[1;31;40m {exact_image_path} Skipped! not a supported image file')
-                pass
-            imgs = cv2.imread(exact_image_path, cv2.IMREAD_UNCHANGED)
-
-            Resized_img = cv2.resize(imgs, new_size)
-            if i % 20 == 0:
-                logger.info(f'{i} Images resized; New Size: {Resized_img.shape[0]} x {Resized_img.shape[1]}')
-                # print(f'\033[1;33;40m New size of {img}: {Resized_img.size[0]} x {Resized_img.size[1]}')1
-            else:
-                pass
-            image_path = Path(image_path)
-            n_folder = os.path.join(image_path.parent, new_folder)
-
-            if not os.path.exists(n_folder):
-                os.mkdir(n_folder)
-            cv2.imwrite(f'{os.path.join(n_folder, img)}', Resized_img)
-            if view == False:
-                pass
-            else:
-                cv2.imshow('Resizing Image', Resized_img)  # cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
-                i += 1
-                cv2.waitKey(1)
-                if i == total_img_len or (cv2.waitKey(1) & 0xFF == 27):
-                    cv2.destroyAllWindows()
-                    break
-                else:
-                    pass
-    cv2.destroyAllWindows()
-    cv2.waitKey(1)
-    return i
-
+import time
+
+import os
+from pathlib import Path
+import cv2
+from colorama import Fore
+
+from .logger_config import animated_exit
+from .save_frames import logger
+
+
+def image_resizer(new_size: tuple,
+                  image_path: str,
+                  n_f=True, new_folder='ResizedImages',
+                  view=True, multiple_folders=False):
+    """
+    :param multiple_folders: Set True if the image path contains multiple folders containing images
+    :param view: if True, there would display window showing resized images
+    :param new_size: New Image size e.g (224, 224)
+    :param image_path: '/path/to/where/images/are
+    :param new_folder: '/Specify/new/folder
+    :param args: at the moment you can specify either jpg or png
+    :return: New image resized to new_size
+    """
+    Resized_folder = ""
+    img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.eps', '.raw', '.svg', '.bmp', '.dib']
+
+    path_dirname = os.path.dirname(image_path)
+    if n_f and not multiple_folders:
+        total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
+        logger.critical(f'{total_img_len} total Images found in \033[1;34;40m {image_path}\n')
+        time.sleep(0.5)
+        Resized_folder = os.path.join(path_dirname, new_folder)
+        if not os.path.exists(Resized_folder):
+            os.mkdir(Resized_folder)
+        image_path = Path(image_path)
+
+        Resized_folder = os.path.join(path_dirname, new_folder)
+        if not os.path.exists(Resized_folder):
+            os.mkdir(Resized_folder)
+        else:
+            print('WARNING!!! IMAGE FOLDER ALREADY EXISTS, OVERRIDING')
+            pass
+        tot_img = resizer(new_size, image_path, img_ext, Resized_folder, view)
+        logger.info('IMAGES RESIZE DONE!!!')
+        animated_exit('COMPUTING STATS')
+
+        msg_print = f'\n==========================================================================\n' \
+                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
+                    f'--------------------------------------------------------------------------\n'
+        folder_path_print = f'Resized Images Folder:\n'
+        new_image_size = f'New Image Size:'
+
+        space_u = f'\n==========================================================================\n'
+
+        total_msg = f'Total Resized Images  : '
+        total_number = f'               {tot_img} '
+        space_b = f'\n=========================================================================='
+        print(Fore.LIGHTBLUE_EX, msg_print, end='')
+        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+        # for new_fol in Resized_folder:
+        print(Fore.RED, f'      {Resized_folder}')
+        # print(Fore.RED, f'{Resized_folder}', end='')
+        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
+        print(Fore.RED, new_size, end='')
+        # print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
+        # print(Fore.MAGENTA, image_folder_print, end='')
+        print(Fore.LIGHTBLUE_EX, space_u, end='')
+        print(Fore.LIGHTBLUE_EX, total_msg, end='')
+        print(Fore.RED, total_number, end='')
+        print(Fore.LIGHTBLUE_EX, space_b)
+        cv2.destroyAllWindows()
+        cv2.waitKey(1)
+
+        # tot_img = resizer(new_size, image_path, Resized_folder, view, )
+
+    elif not n_f and not multiple_folders:
+
+        total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
+        logger.critical(f'{total_img_len} total Images found in \033[1;34;40m {image_path}\n')
+        time.sleep(0.5)
+
+        Resized_folder = image_path
+
+        tot_img = resizer(new_size, image_path, img_ext, Resized_folder, view)
+        logger.info('IMAGES RESIZE DONE!!!')
+        animated_exit('COMPUTING STATS')
+
+        msg_print = f'\n==========================================================================\n' \
+                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
+                    f'--------------------------------------------------------------------------\n'
+        folder_path_print = f'Resized Images Folder:\n'
+        new_image_size = f'New Image Size:'
+
+        space_u = f'\n==========================================================================\n'
+
+        total_msg = f'Total Resized Images  : '
+        total_number = f'               {tot_img} '
+        space_b = f'\n=========================================================================='
+        print(Fore.LIGHTBLUE_EX, msg_print, end='')
+        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+
+        print(Fore.RED, f'      {Resized_folder}')
+        # print(Fore.RED, f'{Resized_folder}', end='')
+        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
+        print(Fore.RED, new_size, end='')
+        # print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
+        # print(Fore.MAGENTA, image_folder_print, end='')
+        print(Fore.LIGHTBLUE_EX, space_u, end='')
+        print(Fore.LIGHTBLUE_EX, total_msg, end='')
+        print(Fore.RED, total_number, end='')
+        print(Fore.LIGHTBLUE_EX, space_b)
+        cv2.destroyAllWindows()
+        cv2.waitKey(1)
+
+    elif not n_f and multiple_folders:
+        image_subfolders = [f.path for f in os.scandir(image_path) if f.is_dir()]  # prints out paths/subfolders
+        total_img_len = len([x for y in image_subfolders for x in os.listdir(y) if Path(x).suffix in img_ext])
+        logger.warning(f'THIS WILL OVERWRITE IMAGES IN THE CURRENT FOLDERS')
+        logger.critical(f'{total_img_len} total Images found in {(Fore.BLUE, image_path)}\n')
+
+        Resized_folder = image_subfolders
+        image_subfolders = [f.path for f in os.scandir(image_path) if f.is_dir()]  # prints out paths/subfolders
+
+        list_indx = 0
+        tot_img = 0
+        for img_fold in image_subfolders:
+            logger.critical(f'RESIZING {img_fold} FOLDER')
+            logger.critical(f'SAVING RESIZED IMAGES into EXISTING folder {img_fold}')
+            tot_img_ = resizer(new_size, img_fold, img_ext, img_fold, view)
+
+            # tot_img_ = resizer(new_size, img_fold, img_fold, view, )
+            time.sleep(0.5)
+            list_indx += 1
+            tot_img += tot_img_
+            if list_indx >= len(image_subfolders):
+                break
+        logger.info('IMAGES RESIZE DONE!!!')
+        animated_exit('COMPUTING STATS')
+
+        msg_print = f'\n==========================================================================\n' \
+                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
+                    f'--------------------------------------------------------------------------\n'
+        folder_path_print = f'Resized Images Folder:\n'
+        new_image_size = f'New Image Size:'
+
+        space_u = f'\n==========================================================================\n'
+
+        total_msg = f'Total Resized Images  : '
+        total_number = f'               {tot_img} '
+        space_b = f'\n=========================================================================='
+        print(Fore.LIGHTBLUE_EX, msg_print, end='')
+        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+        # for new_fol in Resized_folder:
+        for fold in Resized_folder:
+            print(Fore.RED, f'      {fold}')
+        # print(Fore.RED, f'{Resized_folder}', end='')
+        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
+        print(Fore.RED, new_size, end='')
+        # print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
+        # print(Fore.MAGENTA, image_folder_print, end='')
+        print(Fore.LIGHTBLUE_EX, space_u, end='')
+        print(Fore.LIGHTBLUE_EX, total_msg, end='')
+        print(Fore.RED, total_number, end='')
+        print(Fore.LIGHTBLUE_EX, space_b)
+        cv2.destroyAllWindows()
+        cv2.waitKey(1)
+    else:
+        Resized_folder = os.path.join(path_dirname, new_folder)
+        if not os.path.exists(Resized_folder):
+            os.mkdir(Resized_folder)
+        else:
+            print(f'WARNING! {Resized_folder} ALREADY EXISTS, USING EXISTING FOLDER PRESS ESC TO STOP');
+            time.sleep(2.0)
+            if cv2.waitKey(1) & 0xFF == 27: exit()
+
+        image_subfolders = [f.path for f in os.scandir(image_path) if f.is_dir()]  # prints out paths/subfolders
+        total_img_len = len([x for y in image_subfolders for x in os.listdir(y) if Path(x).suffix in img_ext])
+        logger.critical(f'{total_img_len} total Images found in \033[1;34;40m {image_path}\n')
+        subfolder_names = [f.name for f in os.scandir(image_path) if f.is_dir()]  # outputs only the subfolder names
+
+        list_indx = 0
+        tot_img = 0
+        Res_folders = []
+        for img_fold in image_subfolders:
+            logger.critical(f'NOW RESIZING {img_fold}')
+            Resized_folder_ = os.path.join(Resized_folder, subfolder_names[list_indx])
+
+            Res_folders.append(Resized_folder_)
+            if not os.path.exists(Resized_folder_):
+                os.mkdir(Resized_folder_)
+            else:
+                animated_exit(
+                    f'IMAGE FOLDER ALREADY EXISTS,\n OVERRIDING EXISTING FILES IN {Resized_folder_}\n PRESS Esc to Exit');
+                time.sleep(2.0)
+                if cv2.waitKey(1) & 0xFF == 27:
+                    break
+                else:
+                    pass
+            logger.info(f'SAVING INTO {Resized_folder_} FOLDER')
+            tot_img_ = resizer(new_size, img_fold, img_ext, Resized_folder_, view)
+
+            # tot_img_ = resizer(new_size, img_fold, Resized_folder_, view, )
+            list_indx += 1
+            tot_img += tot_img_
+            if list_indx >= len(image_subfolders):
+                cv2.destroyAllWindows()
+                cv2.waitKey(1)
+                break
+        Resized_folder = Res_folders
+        logger.info('IMAGES RESIZE DONE!!!')
+        animated_exit('COMPUTING STATS')
+
+        msg_print = f'\n==========================================================================\n' \
+                    f'-------------------------IMAGE  RESIZE  STATISTICS---------------------- \n' \
+                    f'--------------------------------------------------------------------------\n'
+        folder_path_print = f'Resized Images Folder:\n'
+        new_image_size = f'New Image Size:'
+
+        space_u = f'\n==========================================================================\n'
+
+        total_msg = f'Total Resized Images  : '
+        total_number = f'               {tot_img} '
+        space_b = f'\n=========================================================================='
+        print(Fore.LIGHTBLUE_EX, msg_print, end='')
+        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+        for fold in Resized_folder:
+            print(Fore.RED, f'      {fold}')
+        print(Fore.LIGHTBLUE_EX, new_image_size, end='')
+        print(Fore.RED, new_size, end='')
+        print(Fore.LIGHTBLUE_EX, space_u, end='')
+        print(Fore.LIGHTBLUE_EX, total_msg, end='')
+        print(Fore.RED, total_number, end='')
+        print(Fore.LIGHTBLUE_EX, space_b)
+        cv2.destroyAllWindows()
+        cv2.waitKey(1)
+
+
+def resizer(new_size,
+            image_path,
+            img_ext, new_folder,
+            view):
+    img_dirs = os.listdir(image_path)
+    # img_extend = [x for x in os.listdir(image_path) if Path(x).suffix in img_ext]
+    total_img_len = len([x for x in os.listdir(image_path) if Path(x).suffix in img_ext])
+    i = 0
+    for img in img_dirs:
+        img_e = Path(img).suffix
+        exact_image_path = os.path.join(image_path, img)
+
+        if img_e not in img_ext:
+            print(f'\033[1;31;40m {img} Skipped! not a supported image file ')
+            pass
+        else:
+            if not os.path.isfile(exact_image_path):
+                print(f'\033[1;31;40m {exact_image_path} Skipped! not a supported image file')
+                pass
+            imgs = cv2.imread(exact_image_path, cv2.IMREAD_UNCHANGED)
+
+            Resized_img = cv2.resize(imgs, new_size)
+            if i % 20 == 0:
+                logger.info(f'{i} Images resized; New Size: {Resized_img.shape[0]} x {Resized_img.shape[1]}')
+                # print(f'\033[1;33;40m New size of {img}: {Resized_img.size[0]} x {Resized_img.size[1]}')1
+            else:
+                pass
+            image_path = Path(image_path)
+            n_folder = os.path.join(image_path.parent, new_folder)
+
+            if not os.path.exists(n_folder):
+                os.mkdir(n_folder)
+            cv2.imwrite(f'{os.path.join(n_folder, img)}', Resized_img)
+            if view == False:
+                pass
+            else:
+                cv2.imshow('Resizing Image', Resized_img)  # cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
+                i += 1
+                cv2.waitKey(1)
+                if i == total_img_len or (cv2.waitKey(1) & 0xFF == 27):
+                    cv2.destroyAllWindows()
+                    break
+                else:
+                    pass
+    cv2.destroyAllWindows()
+    cv2.waitKey(1)
+    return i
+
```

### Comparing `ormedian_utils-0.2/src/ormedian_utils/save_frames.py` & `ormedian_utils-0.2.1/src/ormedian_utils/save_frames.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,447 +1,447 @@
-import json
-import os.path
-import re
-from pathlib import Path
-import cv2
-from datetime import datetime
-import logging
-from tqdm import tqdm
-from colorama import Fore
-
-import time
-from .logger_config import CustomFormatter, animated_exit
-
-import datetime as dt
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
-
-# Define format for logs
-fmt = '%(asctime)s | %(levelname)8s | %(message)s'
-
-# Create stdout handler for logging to the console (logs all five levels)
-stdout_handler = logging.StreamHandler()
-stdout_handler.setLevel(logging.DEBUG)
-stdout_handler.setFormatter(CustomFormatter(fmt))
-
-# Create file handler for logging to a file (logs all five levels)
-today = dt.date.today()
-file_handler = logging.FileHandler('my_app_{}.log'.format(today.strftime('%Y_%m_%d')))
-file_handler.setLevel(logging.DEBUG)
-file_handler.setFormatter(logging.Formatter(fmt))
-
-# Add both handlers to the logger
-logger.addHandler(stdout_handler)
-logger.addHandler(file_handler)
-
-
-def frame_capture(file, image_format, new_folder, videos, view):
-    frames_folder = os.path.join(new_folder, videos[0:-len(Path(videos).suffix)])
-    if os.path.exists(frames_folder):
-        pass
-    else:
-        os.mkdir(frames_folder)
-
-    cap = cv2.VideoCapture(file)
-    i = 0
-    while True:
-        ret, frame = cap.read()
-        if ret:
-            if view:
-                cv2.imshow('Output Video', frame)
-            else:
-                pass
-            cv2.imwrite(f'{frames_folder}/image_{i}.{image_format}', frame)
-            i += 1
-            if not i % 20 == 0:
-                pass
-            else:
-                logger.info(f'Frames collected into {frames_folder} : {i}')
-            if cv2.waitKey(1) & 0xFF == 27:
-                logger.critical('EXITING FRAME COLLECTION.....');
-                time.sleep(0.5)
-                logger.critical(f'SUBTOTAL IMAGES SAVED: {i}')
-                return i
-
-        else:
-            cap.release()
-            cv2.destroyAllWindows()
-            logger.critical(f'SUBTOTAL IMAGES SAVED for {file}: {i}')
-            return i
-        cv2.waitKey(1)
-    cap.release
-    cv2.destroyAllWindows()
-    cv2.waitKey(1)
-
-
-def save_video_frames(cap_input, folder, image_name, video_format, view):
-    video_name = os.path.join(folder, image_name)
-    if not os.path.exists(video_name):
-        pass
-    else:
-        logger.error('Video name already exist, please choose a different name')
-    # camera = cv2.VideoCapture(cv2.CAP_V4L2)
-    camera = cv2.VideoCapture(cap_input)
-
-    fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-    width, height = camera.get(cv2.CAP_PROP_FRAME_WIDTH), camera.get(cv2.CAP_PROP_FRAME_HEIGHT)
-    video_ = cv2.VideoWriter(f'{video_name}.{video_format}', fourcc, 20.0, (int(width), int(height)))
-
-    i = 0
-    while camera.isOpened():
-        ret, frame = camera.read()
-        if ret == True:
-            frame = cv2.flip(frame, 1)
-            video_.write(frame)
-            cv2.imwrite(f'{video_name}_{i}.jpg', frame)
-
-            if view:
-
-                cv2.imshow(f'{video_name}', frame)
-            else:
-                pass
-            if i % 20 == 0:
-                logger.info(f'NUMBER OF IMAGES SAVED: {i}')
-            else:
-                pass
-            i += 1
-
-            # if cv2.waitKey(1) & 0xFF == ord('q'):
-            if cv2.waitKey(1) & 0xFF == 27:
-                camera.release()
-                video_.release()
-                cv2.destroyAllWindows()
-                cv2.waitKey(1)
-                animated_exit('EXITING FRAME COLLECTION')
-                break
-    msg_print = f'\n==========================================================================\n' \
-                f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
-                f'--------------------------------------------------------------------------\n'
-    folder_path_print = f'Saved Video'' Path:'
-
-    msg_image_path = f'\n Saved Images Folder:'
-    image_folder_print = f'{folder}                           \n'
-    space_u = f'==========================================================================\n'
-
-    total_msg = f'Total Number of Images saved:    '
-    total_number = f'                {i} '
-    space_b = f'\n=========================================================================='
-    print(Fore.LIGHTBLUE_EX, msg_print, end='')
-    print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-    print(Fore.RED, f'{video_name}{video_format}', end='')
-    print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
-    print(Fore.MAGENTA, image_folder_print, end='')
-    print(Fore.LIGHTBLUE_EX, space_u, end='')
-    print(Fore.LIGHTBLUE_EX, total_msg, end='')
-    print(Fore.RED, total_number, end='')
-    print(Fore.LIGHTBLUE_EX, space_b)
-    camera.release()
-    video_.release()
-    cv2.destroyAllWindows()
-    cv2.waitKey(1)
-
-
-def save_frames_only(cap_input, folder, image_name, image_format, view):
-    video_name = os.path.join(folder, image_name)
-    camera = cv2.VideoCapture(cap_input)
-    i = 0
-    while camera.isOpened():
-        ret, frame = camera.read()
-        if ret == True:
-            frame = cv2.flip(frame, 1)
-            cv2.imwrite(f'{video_name}_{i}.{image_format}', frame)
-            if view:
-
-                cv2.imshow(f'Output {image_name} Video', frame)
-            else:
-                pass
-            if i % 20 == 0:
-                logger.info(f'NUMBER OF IMAGES SAVED: {i}')
-            else:
-                pass
-            i += 1
-
-            if cv2.waitKey(1) & 0xFF == ord('q'):
-                camera.release()
-                cv2.destroyAllWindows()
-                cv2.waitKey(1)
-                animated_exit(f'EXITING FRAME COLLECTION')
-                break
-
-    msg_print = f'\n==========================================================================\n' \
-                f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
-                f'--------------------------------------------------------------------------\n'
-    # folder_path_print = f'Saved Video'' Path:'
-
-    msg_image_path = f'\n Saved Images Folder:'
-    image_folder_print = f'{folder}                           \n'
-    space_u = f'==========================================================================\n'
-
-    total_msg = f'Total Number of Images saved:    '
-    total_number = f'                {i} '
-    space_b = f'\n=========================================================================='
-    print(Fore.LIGHTBLUE_EX, msg_print, end='')
-    print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
-    print(Fore.MAGENTA, image_folder_print, end='')
-    print(Fore.LIGHTBLUE_EX, space_u, end='')
-    print(Fore.LIGHTBLUE_EX, total_msg, end='')
-    print(Fore.RED, total_number, end='')
-    print(Fore.LIGHTBLUE_EX, space_b)
-    camera.release()
-    cv2.destroyAllWindows()
-    cv2.waitKey(1)
-
-
-class collect_frames:
-    def __init__(self, num, video_format='mp4', image_name='frame', image_format='jpg', view=True):
-        super(collect_frames, self).__init__()
-        self.img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.pdf', '.eps', '.raw', '.svg', '.bmp',
-                        '.dib']
-        self.vid_ext = ['.avi', '.flv', '.mpg', '.mpeg', '.mpe', '.mpv', '.mp2', '.mp4', '.3gp', '.m4p', '.m4v', '.ogg',
-                        '.webm', '.mov', '.wmv']
-        # self.videos_path = videos_path
-        self.cap_input = num
-        if image_format[0] != '.':
-            image_format = f'.{image_format}'
-        self.image_format = image_format
-        self.image_name = image_name
-        if video_format[0] != '.':
-            video_format = f'.{video_format}'
-        self.video_format = video_format
-        self.view = view
-
-    def camera(self, folder_path, save_video=True):
-        """
-        Press q to stop collecting frames
-        :param folder_path: Path to save images and video into
-        :param save_video:
-        :param num: integer values between 0 - as many cameras you have
-        :return:
-        """
-        # folder_name = datetime.now().strftime("%H.%M.%S")
-        if self.image_format not in self.img_ext:
-            logger.exception(f'{self.image_format} not a supported image '
-                             f'file, please provide any of the following '
-                             f'images {self.img_ext}', exc_info=False)
-            exit()
-        else:
-            pass
-        if self.video_format not in self.vid_ext:
-            logger.exception(f'Unsupported Video extension provided, '
-                             f'please provide any of the following video format: '
-                             f'{self.video_format}', exc_info=False)
-            exit()
-        else:
-            pass
-
-        self.cap_input = int(self.cap_input)
-        assert isinstance(self.cap_input, int), logger.error('Please provide an Integer value', exc_info=False)
-
-        folder_path = os.path.join(folder_path, datetime.now().strftime("%H.%M.%S"))
-        if os.path.exists(folder_path):
-            logger.warning(f'OVERWRITING! Folder path {folder_path} already exists')
-            pass
-        else:
-            os.makedirs(folder_path)
-        logger.info(f'IMAGES AND VIDEO RECORDED WILL BE SAVED IN {folder_path}')
-        logger.debug('YOU MAY PRESS ESC TO STOP COLLECTION ONCE YOU ARE DONE')
-
-        if save_video:
-            save_video_frames(self.cap_input, folder_path, self.image_name, self.video_format, self.view)
-
-        else:
-            save_frames_only(self.cap_input, folder_path, self.image_name, self.image_format, self.view)
-
-    def videofile(self):
-        """
-
-        :return: used for collecting frames from videofile provided a path, return a new folder in
-        a parent directory with frames from video file
-        """
-        self.cap_input = self.cap_input
-        v_path = self.cap_input
-        assert os.path.exists(self.cap_input), print(f'\033[1;31;40m {self.cap_input}  PATH does not exists'
-                                                     f'Please provide an existing path to a video file'
-                                                     )
-        assert Path(self.cap_input).suffix in self.vid_ext, (f'\033[1;31;40m {self.cap_input} not a video file '
-                                                             f'Please provide any of the following images {self.vid_ext}'
-                                                             )
-        if self.image_format not in self.img_ext:
-            logger.exception(f'{self.image_format} not a supported image '
-                             f'file please provide any of the following images {self.img_ext}', exc_info=False)
-            exit()
-        else:
-            pass
-
-        self.cap_input = os.path.split(self.cap_input)[1]
-
-        video_input = str(self.cap_input)[0:-len(Path(self.cap_input).suffix)]
-        image_folder = os.path.join(Path(v_path).parent, video_input)
-        if os.path.exists(image_folder):
-            logger.warning(f'OVERWRITING! IMage Folder {image_folder} Already exists')
-            pass
-        else:
-            os.mkdir(image_folder)
-        print(video_input)
-        camera = cv2.VideoCapture(v_path)
-        i = 0
-        while camera.isOpened():
-            ret, frame = camera.read()
-            if ret == True:
-                cv2.imwrite(f'{image_folder}/{self.image_name}_{i}.{self.image_format}', frame)
-                if self.view:
-                    cv2.imshow(f'Output {video_input} Video', frame)
-                else:
-                    pass
-                if not i % 20 == 0:
-                    pass
-                else:
-                    logger.info(f'Frames collected into {image_folder} : {i}')
-
-                i += 1
-                if cv2.waitKey(1) & 0xFF == 27:
-                    camera.release()
-
-                    cv2.destroyAllWindows()
-                    cv2.waitKey(1)
-
-                    # logger.critical('EXITING FRAME COLLECTION.....')
-
-                    # done=True
-                    print(Fore.RED + 'FRAME COLLECTION STOPPED ABRUPTLY!');
-                    time.sleep(1.5)
-                    cv2.destroyAllWindows()
-                    cv2.waitKey(1)
-                    break
-
-            else:
-                camera.release()
-
-                cv2.destroyAllWindows()
-                cv2.waitKey(1)
-                animated_exit('EXITING FRAME COLLECTION')
-                break
-        # camera.release()
-        msg_print = f'==========================================================================\n' \
-                    f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
-                    f'--------------------------------------------------------------------------\n'
-        msg_image_path = f'Saved Images Folder:'
-        image_folder_print = f'         {image_folder}                           \n'
-        space_u = f'==========================================================================\n'
-        total_msg = f'Total Number of Images saved:    '
-        total_number = f'                                {i} '
-        space_b = f'\n=========================================================================='
-        print(Fore.CYAN, msg_print, end='')
-        print(Fore.GREEN, msg_image_path, end='')
-        print(Fore.RED, image_folder_print, end='')
-        print(Fore.CYAN, space_u, end='')
-        print(Fore.GREEN, total_msg, end='')
-        print(Fore.RED, total_number, end='')
-        print(Fore.CYAN, space_b)
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
-
-    def videofolder(self, Image_folder='Image Folder'):
-        """
-
-        :param cap_input: path to feed cv2.VideoCapture
-        :param image_format:  format of output image, refer to img_ext
-        :param Image_folder: name of folder to save images to
-        :return:
-        """
-
-        vid_ext = ['.avi', '.flv', '.mpg', '.mpeg', '.mpe', '.mpv', '.mp2', '.mp4', '.3gp', '.m4p', '.m4v', '.ogg',
-                   '.webm', '.mov', '.wmv']
-        img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.pdf', '.eps', '.raw', '.svg', '.bmp',
-                   '.dib']
-        img_ext_ = ['jpg', 'jpeg', 'png', 'gif', 'tiff', 'psd', 'pdf', 'eps', 'raw', 'svg', 'bmp',
-                    'dib']
-
-        assert os.path.isdir(self.cap_input), (f'\033[1;31;40m {self.cap_input} not a directory '
-                                               f'Please provide a directory with video files')
-        assert f'{self.image_format}' in img_ext, print(
-            f'\033[1;31;40m {self.image_format} not a supported image file '
-            f'Please provide any of the following images {img_ext_}'
-        )
-        new_folder = os.path.join(Path(self.cap_input).parent, Image_folder)
-
-        if os.path.exists(new_folder):
-            pass
-        else:
-            os.makedirs(new_folder)
-
-        vids_path = os.listdir(self.cap_input)
-        videos = []
-
-        def returnTrue(file_in):
-            if Path(file_in).suffix in vid_ext:
-                return True
-
-            return False
-
-        assert any([returnTrue(file_in) for file_in in vids_path]) is True, print(
-            (f'\033[1;31;40m {self.cap_input} contains no video file '
-             f'Please provide a directory with video files'
-             ))
-
-        [videos.append(ext) for ext in vids_path if Path(ext).suffix in vid_ext]
-        videos = tqdm(videos)
-        total = 0
-        to_log = {}
-        for vid in videos:
-            videos.set_description(f'{total} Images have been saved')
-            time.sleep(0.05)
-            tot_image = frame_capture(os.path.join(self.cap_input, vid), self.image_format, new_folder, vid, self.view)
-            to_log[f'{vid}'] = f'{tot_image} Images'
-            total += tot_image
-
-            if cv2.waitKey(1) & 0xFF == 27:
-                logger.critical('FRAME COLLECTION STOPPED ABRUPTLY');
-                time.sleep(0.5)
-                logger.critical(f'TOTAL IMAGES SAVED: {total}')
-                cv2.destroyAllWindows()
-                cv2.waitKey(1)
-                break
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
-        to_log = json.dumps(to_log, indent=20, sort_keys=True, default=dict)
-        total = json.dumps(total, indent=20, sort_keys=True, default=int)
-        to_log = re.sub(r"^{\s*", "{", to_log)
-        folder_list = os.listdir(new_folder)
-        # response_text = re.sub(r"\s*}$", "}", total)
-        animated_exit('EXITING FRAME COLLECTION')
-        animated_exit('COMPUTING STATS')
-
-        msg_print = f'==========================================================================\n' \
-                    f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
-                    f'--------------------------------------------------------------------------\n'
-        folder_path_print = f'Folders'' Path:\n'
-
-        msg_image_path = f'\n Saved Images Folder:'
-        image_folder_print = f'                 {to_log}                           \n'
-        space_u = f'==========================================================================\n'
-
-        total_msg = f'Total Number of Images saved:    '
-        total_number = f'                                {total} '
-        space_b = f'\n=========================================================================='
-        print(Fore.LIGHTBLUE_EX, msg_print, end='')
-        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
-        for paths_ in folder_list:
-            print(Fore.MAGENTA, f'              {os.path.join(new_folder, paths_)}')
-
-        print(Fore.LIGHTBLUE_EX, msg_image_path, )
-        print(Fore.MAGENTA, image_folder_print, end='')
-        print(Fore.LIGHTBLUE_EX, space_u, end='')
-        print(Fore.LIGHTBLUE_EX, total_msg, end='')
-        print(Fore.RED, total_number, end='')
-        print(Fore.LIGHTBLUE_EX, space_b)
-
-
-# video_path = '/Users/solua1/Documents/TestVideos/video.mp4'
-# video_path = '/Users/solua1/Documents/TestVideos'
-# collect_frames(video_path).videofolder()
-# collect_frames(video_path).videofile()
-# collect_frames(0).camera('/Users/solua1/Documents/', save_video=True)
-
-# print('back to normal now')
-# print('\033[31m' + 'some red text')
+import json
+import os.path
+import re
+from pathlib import Path
+import cv2
+from datetime import datetime
+import logging
+from tqdm import tqdm
+from colorama import Fore
+
+import time
+from .logger_config import CustomFormatter, animated_exit
+
+import datetime as dt
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
+# Define format for logs
+fmt = '%(asctime)s | %(levelname)8s | %(message)s'
+
+# Create stdout handler for logging to the console (logs all five levels)
+stdout_handler = logging.StreamHandler()
+stdout_handler.setLevel(logging.DEBUG)
+stdout_handler.setFormatter(CustomFormatter(fmt))
+
+# Create file handler for logging to a file (logs all five levels)
+today = dt.date.today()
+file_handler = logging.FileHandler('my_app_{}.log'.format(today.strftime('%Y_%m_%d')))
+file_handler.setLevel(logging.DEBUG)
+file_handler.setFormatter(logging.Formatter(fmt))
+
+# Add both handlers to the logger
+logger.addHandler(stdout_handler)
+logger.addHandler(file_handler)
+
+
+def frame_capture(file, image_format, new_folder, videos, view):
+    frames_folder = os.path.join(new_folder, videos[0:-len(Path(videos).suffix)])
+    if os.path.exists(frames_folder):
+        pass
+    else:
+        os.mkdir(frames_folder)
+
+    cap = cv2.VideoCapture(file)
+    i = 0
+    while True:
+        ret, frame = cap.read()
+        if ret:
+            if view:
+                cv2.imshow('Output Video', frame)
+            else:
+                pass
+            cv2.imwrite(f'{frames_folder}/image_{i}.{image_format}', frame)
+            i += 1
+            if not i % 20 == 0:
+                pass
+            else:
+                logger.info(f'Frames collected into {frames_folder} : {i}')
+            if cv2.waitKey(1) & 0xFF == 27:
+                logger.critical('EXITING FRAME COLLECTION.....');
+                time.sleep(0.5)
+                logger.critical(f'SUBTOTAL IMAGES SAVED: {i}')
+                return i
+
+        else:
+            cap.release()
+            cv2.destroyAllWindows()
+            logger.critical(f'SUBTOTAL IMAGES SAVED for {file}: {i}')
+            return i
+        cv2.waitKey(1)
+    cap.release
+    cv2.destroyAllWindows()
+    cv2.waitKey(1)
+
+
+def save_video_frames(cap_input, folder, image_name, video_format, view):
+    video_name = os.path.join(folder, image_name)
+    if not os.path.exists(video_name):
+        pass
+    else:
+        logger.error('Video name already exist, please choose a different name')
+    # camera = cv2.VideoCapture(cv2.CAP_V4L2)
+    camera = cv2.VideoCapture(cap_input)
+
+    fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+    width, height = camera.get(cv2.CAP_PROP_FRAME_WIDTH), camera.get(cv2.CAP_PROP_FRAME_HEIGHT)
+    video_ = cv2.VideoWriter(f'{video_name}.{video_format}', fourcc, 20.0, (int(width), int(height)))
+
+    i = 0
+    while camera.isOpened():
+        ret, frame = camera.read()
+        if ret == True:
+            frame = cv2.flip(frame, 1)
+            video_.write(frame)
+            cv2.imwrite(f'{video_name}_{i}.jpg', frame)
+
+            if view:
+
+                cv2.imshow(f'{video_name}', frame)
+            else:
+                pass
+            if i % 20 == 0:
+                logger.info(f'NUMBER OF IMAGES SAVED: {i}')
+            else:
+                pass
+            i += 1
+
+            # if cv2.waitKey(1) & 0xFF == ord('q'):
+            if cv2.waitKey(1) & 0xFF == 27:
+                camera.release()
+                video_.release()
+                cv2.destroyAllWindows()
+                cv2.waitKey(1)
+                animated_exit('EXITING FRAME COLLECTION')
+                break
+    msg_print = f'\n==========================================================================\n' \
+                f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
+                f'--------------------------------------------------------------------------\n'
+    folder_path_print = f'Saved Video'' Path:'
+
+    msg_image_path = f'\n Saved Images Folder:'
+    image_folder_print = f'{folder}                           \n'
+    space_u = f'==========================================================================\n'
+
+    total_msg = f'Total Number of Images saved:    '
+    total_number = f'                {i} '
+    space_b = f'\n=========================================================================='
+    print(Fore.LIGHTBLUE_EX, msg_print, end='')
+    print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+    print(Fore.RED, f'{video_name}{video_format}', end='')
+    print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
+    print(Fore.MAGENTA, image_folder_print, end='')
+    print(Fore.LIGHTBLUE_EX, space_u, end='')
+    print(Fore.LIGHTBLUE_EX, total_msg, end='')
+    print(Fore.RED, total_number, end='')
+    print(Fore.LIGHTBLUE_EX, space_b)
+    camera.release()
+    video_.release()
+    cv2.destroyAllWindows()
+    cv2.waitKey(1)
+
+
+def save_frames_only(cap_input, folder, image_name, image_format, view):
+    video_name = os.path.join(folder, image_name)
+    camera = cv2.VideoCapture(cap_input)
+    i = 0
+    while camera.isOpened():
+        ret, frame = camera.read()
+        if ret == True:
+            frame = cv2.flip(frame, 1)
+            cv2.imwrite(f'{video_name}_{i}.{image_format}', frame)
+            if view:
+
+                cv2.imshow(f'Output {image_name} Video', frame)
+            else:
+                pass
+            if i % 20 == 0:
+                logger.info(f'NUMBER OF IMAGES SAVED: {i}')
+            else:
+                pass
+            i += 1
+
+            if cv2.waitKey(1) & 0xFF == ord('q'):
+                camera.release()
+                cv2.destroyAllWindows()
+                cv2.waitKey(1)
+                animated_exit(f'EXITING FRAME COLLECTION')
+                break
+
+    msg_print = f'\n==========================================================================\n' \
+                f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
+                f'--------------------------------------------------------------------------\n'
+    # folder_path_print = f'Saved Video'' Path:'
+
+    msg_image_path = f'\n Saved Images Folder:'
+    image_folder_print = f'{folder}                           \n'
+    space_u = f'==========================================================================\n'
+
+    total_msg = f'Total Number of Images saved:    '
+    total_number = f'                {i} '
+    space_b = f'\n=========================================================================='
+    print(Fore.LIGHTBLUE_EX, msg_print, end='')
+    print(Fore.LIGHTBLUE_EX, msg_image_path, end='')
+    print(Fore.MAGENTA, image_folder_print, end='')
+    print(Fore.LIGHTBLUE_EX, space_u, end='')
+    print(Fore.LIGHTBLUE_EX, total_msg, end='')
+    print(Fore.RED, total_number, end='')
+    print(Fore.LIGHTBLUE_EX, space_b)
+    camera.release()
+    cv2.destroyAllWindows()
+    cv2.waitKey(1)
+
+
+class collect_frames:
+    def __init__(self, num, video_format='mp4', image_name='frame', image_format='jpg', view=True):
+        super(collect_frames, self).__init__()
+        self.img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.pdf', '.eps', '.raw', '.svg', '.bmp',
+                        '.dib']
+        self.vid_ext = ['.avi', '.flv', '.mpg', '.mpeg', '.mpe', '.mpv', '.mp2', '.mp4', '.3gp', '.m4p', '.m4v', '.ogg',
+                        '.webm', '.mov', '.wmv']
+        # self.videos_path = videos_path
+        self.cap_input = num
+        if image_format[0] != '.':
+            image_format = f'.{image_format}'
+        self.image_format = image_format
+        self.image_name = image_name
+        if video_format[0] != '.':
+            video_format = f'.{video_format}'
+        self.video_format = video_format
+        self.view = view
+
+    def camera(self, folder_path, save_video=True):
+        """
+        Press q to stop collecting frames
+        :param folder_path: Path to save images and video into
+        :param save_video:
+        :param num: integer values between 0 - as many cameras you have
+        :return:
+        """
+        # folder_name = datetime.now().strftime("%H.%M.%S")
+        if self.image_format not in self.img_ext:
+            logger.exception(f'{self.image_format} not a supported image '
+                             f'file, please provide any of the following '
+                             f'images {self.img_ext}', exc_info=False)
+            exit()
+        else:
+            pass
+        if self.video_format not in self.vid_ext:
+            logger.exception(f'Unsupported Video extension provided, '
+                             f'please provide any of the following video format: '
+                             f'{self.video_format}', exc_info=False)
+            exit()
+        else:
+            pass
+
+        self.cap_input = int(self.cap_input)
+        assert isinstance(self.cap_input, int), logger.error('Please provide an Integer value', exc_info=False)
+
+        folder_path = os.path.join(folder_path, datetime.now().strftime("%H.%M.%S"))
+        if os.path.exists(folder_path):
+            logger.warning(f'OVERWRITING! Folder path {folder_path} already exists')
+            pass
+        else:
+            os.makedirs(folder_path)
+        logger.info(f'IMAGES AND VIDEO RECORDED WILL BE SAVED IN {folder_path}')
+        logger.debug('YOU MAY PRESS ESC TO STOP COLLECTION ONCE YOU ARE DONE')
+
+        if save_video:
+            save_video_frames(self.cap_input, folder_path, self.image_name, self.video_format, self.view)
+
+        else:
+            save_frames_only(self.cap_input, folder_path, self.image_name, self.image_format, self.view)
+
+    def videofile(self):
+        """
+
+        :return: used for collecting frames from videofile provided a path, return a new folder in
+        a parent directory with frames from video file
+        """
+        self.cap_input = self.cap_input
+        v_path = self.cap_input
+        assert os.path.exists(self.cap_input), print(f'\033[1;31;40m {self.cap_input}  PATH does not exists'
+                                                     f'Please provide an existing path to a video file'
+                                                     )
+        assert Path(self.cap_input).suffix in self.vid_ext, (f'\033[1;31;40m {self.cap_input} not a video file '
+                                                             f'Please provide any of the following images {self.vid_ext}'
+                                                             )
+        if self.image_format not in self.img_ext:
+            logger.exception(f'{self.image_format} not a supported image '
+                             f'file please provide any of the following images {self.img_ext}', exc_info=False)
+            exit()
+        else:
+            pass
+
+        self.cap_input = os.path.split(self.cap_input)[1]
+
+        video_input = str(self.cap_input)[0:-len(Path(self.cap_input).suffix)]
+        image_folder = os.path.join(Path(v_path).parent, video_input)
+        if os.path.exists(image_folder):
+            logger.warning(f'OVERWRITING! IMage Folder {image_folder} Already exists')
+            pass
+        else:
+            os.mkdir(image_folder)
+        print(video_input)
+        camera = cv2.VideoCapture(v_path)
+        i = 0
+        while camera.isOpened():
+            ret, frame = camera.read()
+            if ret == True:
+                cv2.imwrite(f'{image_folder}/{self.image_name}_{i}.{self.image_format}', frame)
+                if self.view:
+                    cv2.imshow(f'Output {video_input} Video', frame)
+                else:
+                    pass
+                if not i % 20 == 0:
+                    pass
+                else:
+                    logger.info(f'Frames collected into {image_folder} : {i}')
+
+                i += 1
+                if cv2.waitKey(1) & 0xFF == 27:
+                    camera.release()
+
+                    cv2.destroyAllWindows()
+                    cv2.waitKey(1)
+
+                    # logger.critical('EXITING FRAME COLLECTION.....')
+
+                    # done=True
+                    print(Fore.RED + 'FRAME COLLECTION STOPPED ABRUPTLY!');
+                    time.sleep(1.5)
+                    cv2.destroyAllWindows()
+                    cv2.waitKey(1)
+                    break
+
+            else:
+                camera.release()
+
+                cv2.destroyAllWindows()
+                cv2.waitKey(1)
+                animated_exit('EXITING FRAME COLLECTION')
+                break
+        # camera.release()
+        msg_print = f'==========================================================================\n' \
+                    f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
+                    f'--------------------------------------------------------------------------\n'
+        msg_image_path = f'Saved Images Folder:'
+        image_folder_print = f'         {image_folder}                           \n'
+        space_u = f'==========================================================================\n'
+        total_msg = f'Total Number of Images saved:    '
+        total_number = f'                                {i} '
+        space_b = f'\n=========================================================================='
+        print(Fore.CYAN, msg_print, end='')
+        print(Fore.GREEN, msg_image_path, end='')
+        print(Fore.RED, image_folder_print, end='')
+        print(Fore.CYAN, space_u, end='')
+        print(Fore.GREEN, total_msg, end='')
+        print(Fore.RED, total_number, end='')
+        print(Fore.CYAN, space_b)
+        cv2.destroyAllWindows()
+        cv2.waitKey(1)
+
+    def videofolder(self, Image_folder='Image Folder'):
+        """
+
+        :param cap_input: path to feed cv2.VideoCapture
+        :param image_format:  format of output image, refer to img_ext
+        :param Image_folder: name of folder to save images to
+        :return:
+        """
+
+        vid_ext = ['.avi', '.flv', '.mpg', '.mpeg', '.mpe', '.mpv', '.mp2', '.mp4', '.3gp', '.m4p', '.m4v', '.ogg',
+                   '.webm', '.mov', '.wmv']
+        img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.pdf', '.eps', '.raw', '.svg', '.bmp',
+                   '.dib']
+        img_ext_ = ['jpg', 'jpeg', 'png', 'gif', 'tiff', 'psd', 'pdf', 'eps', 'raw', 'svg', 'bmp',
+                    'dib']
+
+        assert os.path.isdir(self.cap_input), (f'\033[1;31;40m {self.cap_input} not a directory '
+                                               f'Please provide a directory with video files')
+        assert f'{self.image_format}' in img_ext, print(
+            f'\033[1;31;40m {self.image_format} not a supported image file '
+            f'Please provide any of the following images {img_ext_}'
+        )
+        new_folder = os.path.join(Path(self.cap_input).parent, Image_folder)
+
+        if os.path.exists(new_folder):
+            pass
+        else:
+            os.makedirs(new_folder)
+
+        vids_path = os.listdir(self.cap_input)
+        videos = []
+
+        def returnTrue(file_in):
+            if Path(file_in).suffix in vid_ext:
+                return True
+
+            return False
+
+        assert any([returnTrue(file_in) for file_in in vids_path]) is True, print(
+            (f'\033[1;31;40m {self.cap_input} contains no video file '
+             f'Please provide a directory with video files'
+             ))
+
+        [videos.append(ext) for ext in vids_path if Path(ext).suffix in vid_ext]
+        videos = tqdm(videos)
+        total = 0
+        to_log = {}
+        for vid in videos:
+            videos.set_description(f'{total} Images have been saved')
+            time.sleep(0.05)
+            tot_image = frame_capture(os.path.join(self.cap_input, vid), self.image_format, new_folder, vid, self.view)
+            to_log[f'{vid}'] = f'{tot_image} Images'
+            total += tot_image
+
+            if cv2.waitKey(1) & 0xFF == 27:
+                logger.critical('FRAME COLLECTION STOPPED ABRUPTLY');
+                time.sleep(0.5)
+                logger.critical(f'TOTAL IMAGES SAVED: {total}')
+                cv2.destroyAllWindows()
+                cv2.waitKey(1)
+                break
+        cv2.destroyAllWindows()
+        cv2.waitKey(1)
+        to_log = json.dumps(to_log, indent=20, sort_keys=True, default=dict)
+        total = json.dumps(total, indent=20, sort_keys=True, default=int)
+        to_log = re.sub(r"^{\s*", "{", to_log)
+        folder_list = os.listdir(new_folder)
+        # response_text = re.sub(r"\s*}$", "}", total)
+        animated_exit('EXITING FRAME COLLECTION')
+        animated_exit('COMPUTING STATS')
+
+        msg_print = f'==========================================================================\n' \
+                    f'-------------------------SAVED FRAME STATISTICS------------------------ \n' \
+                    f'--------------------------------------------------------------------------\n'
+        folder_path_print = f'Folders'' Path:\n'
+
+        msg_image_path = f'\n Saved Images Folder:'
+        image_folder_print = f'                 {to_log}                           \n'
+        space_u = f'==========================================================================\n'
+
+        total_msg = f'Total Number of Images saved:    '
+        total_number = f'                                {total} '
+        space_b = f'\n=========================================================================='
+        print(Fore.LIGHTBLUE_EX, msg_print, end='')
+        print(Fore.LIGHTBLUE_EX, folder_path_print, end='')
+        for paths_ in folder_list:
+            print(Fore.MAGENTA, f'              {os.path.join(new_folder, paths_)}')
+
+        print(Fore.LIGHTBLUE_EX, msg_image_path, )
+        print(Fore.MAGENTA, image_folder_print, end='')
+        print(Fore.LIGHTBLUE_EX, space_u, end='')
+        print(Fore.LIGHTBLUE_EX, total_msg, end='')
+        print(Fore.RED, total_number, end='')
+        print(Fore.LIGHTBLUE_EX, space_b)
+
+
+# video_path = '/Users/solua1/Documents/TestVideos/video.mp4'
+# video_path = '/Users/solua1/Documents/TestVideos'
+# collect_frames(video_path).videofolder()
+# collect_frames(video_path).videofile()
+# collect_frames(0).camera('/Users/solua1/Documents/', save_video=True)
+
+# print('back to normal now')
+# print('\033[31m' + 'some red text')
```

### Comparing `ormedian_utils-0.2/src/ormedian_utils/video_folder.py` & `ormedian_utils-0.2.1/src/ormedian_utils/video_folder.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import os
-import time
-from pathlib import Path
-import cv2
-from tqdm import tqdm
-
-
-def frame_capture(file, image_format, new_folder, videos):
-    frames_folder = os.path.join(new_folder, videos[0:-len(Path(videos).suffix)])
-    if os.path.exists(frames_folder):
-        pass
-    else:
-        os.mkdir(frames_folder)
-
-    cap = cv2.VideoCapture(file)
-    i = 0
-    while True:
-        ret, frame = cap.read()
-        if ret:
-            cv2.imshow('name', frame)
-            cv2.imwrite(f'{frames_folder}/image_{i}.{image_format}', frame)
-            print(f'image{i} saved into: {frames_folder}/image_{i}.jpg')
-            i += 1
-        else:
-            break
-        cv2.waitKey(25)
-    cap.release()
-
-
-def video_folder(cap_input, Image_folder = 'Image Folder', image_format='jpg'):
-    """
-
-    :param cap_input: path to feed cv2.VideoCapture
-    :param image_format:  format of output image, refer to img_ext
-    :param Image_folder: name of folder to save images to
-    :return:
-    """
-    vid_ext = ['.avi', '.flv', '.mpg', '.mpeg', '.mpe', '.mpv', '.mp2', '.mp4', '.3gp', '.m4p', '.m4v', '.ogg',
-               '.webm', '.mov', '.wmv']
-    img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.pdf', '.eps', '.raw', '.svg', '.bmp',
-               '.dib']
-    img_ext_ = ['jpg', 'jpeg', 'png', 'gif', 'tiff', 'psd', 'pdf', 'eps', 'raw', 'svg', 'bmp',
-                'dib']
-
-    assert os.path.isdir(cap_input), (f'\033[1;31;40m {cap_input} not a directory '
-                                               f'Please provide a directory with video files')
-    assert f'.{image_format}' in img_ext, print(
-        f'\033[1;31;40m {image_format} not a supported image file '
-        f'Please provide any of the following images {img_ext_}'
-    )
-    new_folder = os.path.join(Path(cap_input).parent, Image_folder)
-
-    if os.path.exists(new_folder):
-        pass
-    else:
-        os.makedirs(new_folder)
-
-    vids_path = os.listdir(cap_input)
-    videos = []
-    def returnTrue(file_in):
-        if Path(file_in).suffix in vid_ext:
-            return True
-
-        return False
-    """
-    prints 
-    ['2.jpg', '360_360-0882_preview.mp4', '360_360-0809_preview.mp4', '1.jpg', '16.jpg', '8.jpg', '7.jpg', '9.jpg', 
-    '14.jpg', '10.jpg', 'istock-887357848_preview.mp4', '170609_E_Varanasi_010.mp4', '5.jpg', '20.jpg', '17.jpg', 
-    '18.jpg', '19.jpg', '15.jpg', '3.jpg', '11.jpg', '4.jpg', '13.jpg', '6.jpg', '360_360-0383_preview.mp4', '12.jpg']"""
-
-    assert any([returnTrue(file_in) for file_in in vids_path]) is True, print((f'\033[1;31;40m {cap_input} contains no video file '
-                   f'Please provide a directory with video files'
-                   ))
-
-    [videos.append(ext) for ext in vids_path if Path(ext).suffix in vid_ext]
-
-    videos = tqdm(videos)
-    for vid in videos:
-        time.sleep(0.1)
-        frame_capture(os.path.join(cap_input, vid), image_format, new_folder, vid)
-        videos.set_description(f'Saving frames from {vid} Video')
-
-# video_path = '/home/iamshri/Videos'
-# # video_path = '/home/iamshri/new_videos/170609_E_Varanasi_010'
-# images_folder = 'Images'
-# video_folder(video_path)
+import os
+import time
+from pathlib import Path
+import cv2
+from tqdm import tqdm
+
+
+def frame_capture(file, image_format, new_folder, videos):
+    frames_folder = os.path.join(new_folder, videos[0:-len(Path(videos).suffix)])
+    if os.path.exists(frames_folder):
+        pass
+    else:
+        os.mkdir(frames_folder)
+
+    cap = cv2.VideoCapture(file)
+    i = 0
+    while True:
+        ret, frame = cap.read()
+        if ret:
+            cv2.imshow('name', frame)
+            cv2.imwrite(f'{frames_folder}/image_{i}.{image_format}', frame)
+            print(f'image{i} saved into: {frames_folder}/image_{i}.jpg')
+            i += 1
+        else:
+            break
+        cv2.waitKey(25)
+    cap.release()
+
+
+def video_folder(cap_input, Image_folder = 'Image Folder', image_format='jpg'):
+    """
+
+    :param cap_input: path to feed cv2.VideoCapture
+    :param image_format:  format of output image, refer to img_ext
+    :param Image_folder: name of folder to save images to
+    :return:
+    """
+    vid_ext = ['.avi', '.flv', '.mpg', '.mpeg', '.mpe', '.mpv', '.mp2', '.mp4', '.3gp', '.m4p', '.m4v', '.ogg',
+               '.webm', '.mov', '.wmv']
+    img_ext = ['.jpg', '.jpeg', '.png', '.gif', '.tiff', '.psd', '.pdf', '.eps', '.raw', '.svg', '.bmp',
+               '.dib']
+    img_ext_ = ['jpg', 'jpeg', 'png', 'gif', 'tiff', 'psd', 'pdf', 'eps', 'raw', 'svg', 'bmp',
+                'dib']
+
+    assert os.path.isdir(cap_input), (f'\033[1;31;40m {cap_input} not a directory '
+                                               f'Please provide a directory with video files')
+    assert f'.{image_format}' in img_ext, print(
+        f'\033[1;31;40m {image_format} not a supported image file '
+        f'Please provide any of the following images {img_ext_}'
+    )
+    new_folder = os.path.join(Path(cap_input).parent, Image_folder)
+
+    if os.path.exists(new_folder):
+        pass
+    else:
+        os.makedirs(new_folder)
+
+    vids_path = os.listdir(cap_input)
+    videos = []
+    def returnTrue(file_in):
+        if Path(file_in).suffix in vid_ext:
+            return True
+
+        return False
+    """
+    prints 
+    ['2.jpg', '360_360-0882_preview.mp4', '360_360-0809_preview.mp4', '1.jpg', '16.jpg', '8.jpg', '7.jpg', '9.jpg', 
+    '14.jpg', '10.jpg', 'istock-887357848_preview.mp4', '170609_E_Varanasi_010.mp4', '5.jpg', '20.jpg', '17.jpg', 
+    '18.jpg', '19.jpg', '15.jpg', '3.jpg', '11.jpg', '4.jpg', '13.jpg', '6.jpg', '360_360-0383_preview.mp4', '12.jpg']"""
+
+    assert any([returnTrue(file_in) for file_in in vids_path]) is True, print((f'\033[1;31;40m {cap_input} contains no video file '
+                   f'Please provide a directory with video files'
+                   ))
+
+    [videos.append(ext) for ext in vids_path if Path(ext).suffix in vid_ext]
+
+    videos = tqdm(videos)
+    for vid in videos:
+        time.sleep(0.1)
+        frame_capture(os.path.join(cap_input, vid), image_format, new_folder, vid)
+        videos.set_description(f'Saving frames from {vid} Video')
+
+# video_path = '/home/iamshri/Videos'
+# # video_path = '/home/iamshri/new_videos/170609_E_Varanasi_010'
+# images_folder = 'Images'
+# video_folder(video_path)
```

### Comparing `ormedian_utils-0.2/README.md` & `ormedian_utils-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,166 +1,168 @@
-https://user-images.githubusercontent.com/73752977/188218332-96f6766d-3f7f-4eb0-89f2-c2b58a08c375.mp4
-
-
-This package contains the following utilities
-
-**🚀Frame Saver** - save frames from video, folders containing videos or camera feed/livefeed.\
-**🚀Image Resizer** - Resize image while retaining the quality\
-**🚀File mover** - move specific file types from thousands/myriads of files.
-
-
-More utility functions to be added subsequently.
-
-
-
-I hope you find this package useful
-
-
-To install:
-
-``
-pip3 install ormedian-utils
-``
-
-<br>
-
-> ### FRAME SAVER                   ``collect_frames()``
-Save frames from video, camera feed, video folder containing multiple videos.
-
-```
-collect_frames(num, video_format='mp4', image_name='frame', image_format='jpg', view=True)
-```
-`num`: **could be camera id, path to video, or a folder contain a number of videos**\
-`video_format`: **format of output video if saving video, default format is set to mp4**\
-`image_name`: **name of frame files, numbers will be appended at the back in the form of frames_1, frames_2...frames_n, could be changed to wheveter you want**\
-`image_format`: **extension of image/frames to be saved, default format is 'jpg', could be any image format, e.g 'png', 'bmp' etc**
-
-This package has 3 methods:
-
-<br>
-
-> 1. **camera** 
-    
-for saving frames from camera feed
-   
- **USAGE**:
-
-````
-from ormedian_utils import collect_frames
-camera_id =0
-frames = collect_frames(camera_id)
-frames.camera(camera_id, save_video=True)
-````
-``save_video=True`` saves video from camera feed into the same folder as the collected frames. You may set ``save_video`` to ``False`` to not save video. 
-<br>
-
-> 2. **videofolder** 
-
-for saving frames from videos in a folder(s)
-
-**USAGE**:
-````
-from ormedian_utils import collect_frames
-video_folder_path ='path/to/foldercontaining/videos
-frames = collect_frames(video_folder_path)
-Image_folder = 'Image Folder' 
-frames.videofolder(video_folder_path, Image_folder=Image_folder)
-````
-
-``Image_folder``: Where Frames will be saved. defaults to ``Image Folder`` unless otherwise changed\
-A new folder will be created for each video, and corresponding frames will be saved in this folder.
-
-<br>
-
-> 3. **videofile** 
-
-for saving frames from a single video file
-
-**USAGE**:
-````
-from ormedian_utils import collect_frames
-video_path = 'path/to/a/singlevideo'
-frames = collect_frames(video_path)
-frames.videofile()
-````
-
-<br>
-
-> ### IMAGE RESIZER ``image_resizer()``
-
-
-Resize images in a folder or in multiple folders 
-
-
-https://user-images.githubusercontent.com/73752977/187389467-3e4c8e8f-bab9-433f-9e0a-e80dca32037b.mp4
-
-
-```
-image_resizer (new_size: tuple,
-                  image_path: str,
-                  n_f=True, new_folder='ResizedImages',
-                  view=True, multiple_folders=False):
-```
-```new_size:``` **expected New Image size e.g (224, 224)**
-
-```image_path:``` **'/path/to/where/images/are**
-
-```n_f: ``` **set to True if resized images be saved in new_folder, set to True by default**
-NOTE: if resizing multiple folders (``multiple_folders=True``) and  ``n_f`` is set ``True`` 
-This will create a separate folder for each folder (``Parent_folder of image_path/ResizedImages/subfolders``) in the parent directory of ``image_path``.
-Setting ``n_f`` to ``False`` when resizing ``multiple_folders`` will override the existing ``image_path`` and overwrite the images in the subfolders.
-
-```new_folder:``` **Name of new folder to save resized images, accepts strings, default value is set to 'ResizedImages'**
-
-```view:``` **default value is set to True, this would display window showing resized images**
-
-```multiple_folders:``` **Set to True if image_path contains more than one image folder, default is False**
-
-
-**USAGE:**
-```
-from ormedian_utils import  image_resizer
-
-new_size = (100, 100)
-images_folder = '/path/to/images/folder' 
-quality =100
-```
-In this case ``images_folder contains multiple image folders``. Hence we set ``multiple_folders`` to ``True`` below.
-```
-image_resizer(new_size,
-              images_folder,
-              n_f=True,
-              quality, multiple_folders=True)
-```
-
-<br>
-
-> ### FILE MOVER ``filemover()``
-
-
-Move files from one folder to another 
-
-```filemover(folder_path: str, file_ext: str, new_folder: str)```
-
-``folder_path:`` **path to files, e.g /path/to/folder/files/**
-
-``file_ext:`` **file extension of files to move e.g 'json'**
-
-``new_folder:`` **folder name of where to move files to, creates directory in parent directory if it does not already exist**
-
-
-**USAGE:** 
-```
-from ormedian_utils import filemover
-
-folder_path = /path/to/different/files     #contains json, csv, jpg, and docs files
-file_ext = 'json'
-new_folder = 'MovedFiles'
-
-filemover(folder_path, file_ext, new_folder)
-
-```
-
-### Todo
-- [ ] **Image Converter**
-- [ ] **Video Converter**
-- [ ] **Audio Parser**
+`requires >= Python 3.6`
+
+https://user-images.githubusercontent.com/73752977/188218332-96f6766d-3f7f-4eb0-89f2-c2b58a08c375.mp4
+
+
+This package contains the following utilities
+
+**🚀Frame Saver** - save frames from video, folders containing videos or camera feed/livefeed.\
+**🚀Image Resizer** - Resize image while retaining the quality\
+**🚀File mover** - move specific file types from thousands/myriads of files.
+
+
+More utility functions to be added subsequently.
+
+
+
+I hope you find this package useful
+
+
+To install:
+
+``
+pip3 install ormedian-utils
+``
+
+<br>
+
+> ### FRAME SAVER                   ``collect_frames()``
+Save frames from video, camera feed, video folder containing multiple videos.
+
+```
+collect_frames(num, video_format='mp4', image_name='frame', image_format='jpg', view=True)
+```
+`num`: **could be camera id, path to video, or a folder contain a number of videos**\
+`video_format`: **format of output video if saving video, default format is set to mp4**\
+`image_name`: **name of frame files, numbers will be appended at the back in the form of frames_1, frames_2...frames_n, could be changed to wheveter you want**\
+`image_format`: **extension of image/frames to be saved, default format is 'jpg', could be any image format, e.g 'png', 'bmp' etc**
+
+This package has 3 methods:
+
+<br>
+
+> 1. **camera** 
+    
+for saving frames from camera feed
+   
+ **USAGE**:
+
+````
+from ormedian_utils import collect_frames
+camera_id =0
+frames = collect_frames(camera_id)
+frames.camera(camera_id, save_video=True)
+````
+``save_video=True`` saves video from camera feed into the same folder as the collected frames. You may set ``save_video`` to ``False`` to not save video. 
+<br>
+
+> 2. **videofolder** 
+
+for saving frames from videos in a folder(s)
+
+**USAGE**:
+````
+from ormedian_utils import collect_frames
+video_folder_path ='path/to/foldercontaining/videos
+frames = collect_frames(video_folder_path)
+Image_folder = 'Image Folder' 
+frames.videofolder(video_folder_path, Image_folder=Image_folder)
+````
+
+``Image_folder``: Where Frames will be saved. defaults to ``Image Folder`` unless otherwise changed\
+A new folder will be created for each video, and corresponding frames will be saved in this folder.
+
+<br>
+
+> 3. **videofile** 
+
+for saving frames from a single video file
+
+**USAGE**:
+````
+from ormedian_utils import collect_frames
+video_path = 'path/to/a/singlevideo'
+frames = collect_frames(video_path)
+frames.videofile()
+````
+
+<br>
+
+> ### IMAGE RESIZER ``image_resizer()``
+
+
+Resize images in a folder or in multiple folders 
+
+
+https://user-images.githubusercontent.com/73752977/187389467-3e4c8e8f-bab9-433f-9e0a-e80dca32037b.mp4
+
+
+```
+image_resizer (new_size: tuple,
+                  image_path: str,
+                  n_f=True, new_folder='ResizedImages',
+                  view=True, multiple_folders=False):
+```
+```new_size:``` **expected New Image size e.g (224, 224)**
+
+```image_path:``` **'/path/to/where/images/are**
+
+```n_f: ``` **set to True if resized images be saved in new_folder, set to True by default**
+NOTE: if resizing multiple folders (``multiple_folders=True``) and  ``n_f`` is set ``True`` 
+This will create a separate folder for each folder (``Parent_folder of image_path/ResizedImages/subfolders``) in the parent directory of ``image_path``.
+Setting ``n_f`` to ``False`` when resizing ``multiple_folders`` will override the existing ``image_path`` and overwrite the images in the subfolders.
+
+```new_folder:``` **Name of new folder to save resized images, accepts strings, default value is set to 'ResizedImages'**
+
+```view:``` **default value is set to True, this would display window showing resized images**
+
+```multiple_folders:``` **Set to True if image_path contains more than one image folder, default is False**
+
+
+**USAGE:**
+```
+from ormedian_utils import  image_resizer
+
+new_size = (100, 100)
+images_folder = '/path/to/images/folder' 
+quality =100
+```
+In this case ``images_folder contains multiple image folders``. Hence we set ``multiple_folders`` to ``True`` below.
+```
+image_resizer(new_size,
+              images_folder,
+              n_f=True,
+              quality, multiple_folders=True)
+```
+
+<br>
+
+> ### FILE MOVER ``filemover()``
+
+
+Move files from one folder to another 
+
+```filemover(folder_path: str, file_ext: str, new_folder: str)```
+
+``folder_path:`` **path to files, e.g /path/to/folder/files/**
+
+``file_ext:`` **file extension of files to move e.g 'json'**
+
+``new_folder:`` **folder name of where to move files to, creates directory in parent directory if it does not already exist**
+
+
+**USAGE:** 
+```
+from ormedian_utils import filemover
+
+folder_path = /path/to/different/files     #contains json, csv, jpg, and docs files
+file_ext = 'json'
+new_folder = 'MovedFiles'
+
+filemover(folder_path, file_ext, new_folder)
+
+```
+
+### Todo
+- [ ] **Image Converter**
+- [ ] **Video Converter**
+- [ ] **Audio Parser**
```

### Comparing `ormedian_utils-0.2/pyproject.toml` & `ormedian_utils-0.2.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = 'ormedian_utils'
-version = '0.2'
-authors = [
-    {name='Samuel Adebayo', email='samueladebayo@ieee.org'},
-]
-description = 'Utilities for Computer Vision Tasks'
-readme = 'README.md'
-license = {file='LICENSE'}
-requires-python = '<=3.10.0'
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent"
-]
-dependencies = [
-    "opencv-python==4.5.4.58", "colorama", "tqdm"
-]
-
-[project.urls]
-'Homepage' = 'https://github.com/exponentialR/ormedian-utils'
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = 'ormedian_utils'
+version = '0.2.1'
+authors = [
+    {name='Samuel Adebayo', email='samueladebayo@ieee.org'},
+]
+description = 'Utilities for Computer Vision Tasks'
+readme = 'README.md'
+license = {file='LICENSE'}
+requires-python = '>=3.6'
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent"
+]
+dependencies = [
+    "opencv-python>=4.5.5.62", "colorama", "Pillow", "tqdm"
+]
+
+[project.urls]
+'Homepage' = 'https://github.com/exponentialR/ormedian-utils'
 'Bug Tracker' = 'https://github.com/exponentialR/ormedian-utils/issues'
```

### Comparing `ormedian_utils-0.2/PKG-INFO` & `ormedian_utils-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: ormedian_utils
-Version: 0.2
+Version: 0.2.1
 Summary: Utilities for Computer Vision Tasks
 Project-URL: Homepage, https://github.com/exponentialR/ormedian-utils
 Project-URL: Bug Tracker, https://github.com/exponentialR/ormedian-utils/issues
 Author-email: Samuel Adebayo <samueladebayo@ieee.org>
 License: AIN'T NO LICENSE BRUV!
         USE AS IS
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <=3.10.0
+Requires-Python: >=3.6
 Requires-Dist: colorama
-Requires-Dist: opencv-python==4.5.4.58
+Requires-Dist: opencv-python>=4.5.5.62
+Requires-Dist: pillow
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
+`requires >= Python 3.6`
+
 https://user-images.githubusercontent.com/73752977/188218332-96f6766d-3f7f-4eb0-89f2-c2b58a08c375.mp4
 
 
 This package contains the following utilities
 
 **🚀Frame Saver** - save frames from video, folders containing videos or camera feed/livefeed.\
 **🚀Image Resizer** - Resize image while retaining the quality\
```

