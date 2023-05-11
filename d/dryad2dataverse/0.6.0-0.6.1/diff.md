# Comparing `tmp/dryad2dataverse-0.6.0.tar.gz` & `tmp/dryad2dataverse-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dryad2dataverse-0.6.0.tar", last modified: Wed May  3 20:16:20 2023, max compression
+gzip compressed data, was "dryad2dataverse-0.6.1.tar", last modified: Thu May 11 16:04:13 2023, max compression
```

## Comparing `dryad2dataverse-0.6.0.tar` & `dryad2dataverse-0.6.1.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.537736 dryad2dataverse-0.6.0/
--rw-r--r--   0 paul       (501) staff       (20)      485 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/.gitignore
--rw-r--r--   0 paul       (501) staff       (20)     3019 2023-05-03 20:16:20.536926 dryad2dataverse-0.6.0/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     2033 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/README.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.843413 dryad2dataverse-0.6.0/docs/
--rw-r--r--   0 paul       (501) staff       (20)      442 2021-11-29 23:23:23.000000 dryad2dataverse-0.6.0/docs/_config.yml
--rw-r--r--   0 paul       (501) staff       (20)    26768 2022-12-07 22:06:06.000000 dryad2dataverse-0.6.0/docs/api_reference.md
--rw-r--r--   0 paul       (501) staff       (20)     4855 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/changelog.md
--rw-r--r--   0 paul       (501) staff       (20)     1631 2022-04-14 21:51:21.000000 dryad2dataverse-0.6.0/docs/compiling.md
--rw-r--r--   0 paul       (501) staff       (20)     1152 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/credits.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.845434 dryad2dataverse-0.6.0/docs/css/
--rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.6.0/docs/css/extra.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.888738 dryad2dataverse-0.6.0/docs/dbase_structure/
--rw-r--r--   0 paul       (501) staff       (20)    19355 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/anomalies.html
--rw-r--r--   0 paul       (501) staff       (20)        0 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/anomalies.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.804285 dryad2dataverse-0.6.0/docs/dbase_structure/bower/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.779803 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.779338 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.909380 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/
--rw-r--r--   0 paul       (501) staff       (20)    26132 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css
--rw-r--r--   0 paul       (501) staff       (20)    47706 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map
--rw-r--r--   0 paul       (501) staff       (20)    23409 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 paul       (501) staff       (20)    25648 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map
--rw-r--r--   0 paul       (501) staff       (20)   146010 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css
--rw-r--r--   0 paul       (501) staff       (20)   389287 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 paul       (501) staff       (20)   121200 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 paul       (501) staff       (20)   542194 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.923999 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/
--rw-r--r--   0 paul       (501) staff       (20)    20127 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 paul       (501) staff       (20)   108738 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 paul       (501) staff       (20)    45404 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 paul       (501) staff       (20)    23424 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 paul       (501) staff       (20)    18028 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.929932 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/js/
--rw-r--r--   0 paul       (501) staff       (20)    69707 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js
--rw-r--r--   0 paul       (501) staff       (20)    37045 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 paul       (501) staff       (20)      484 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/js/npm.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.781351 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.932647 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/fastclick/
--rw-r--r--   0 paul       (501) staff       (20)    25965 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js
--rw-r--r--   0 paul       (501) staff       (20)     8776 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.933609 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQuery/
--rw-r--r--   0 paul       (501) staff       (20)    85659 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.945270 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/
--rw-r--r--   0 paul       (501) staff       (20)   470596 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js
--rw-r--r--   0 paul       (501) staff       (20)   240427 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.950859 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/
--rw-r--r--   0 paul       (501) staff       (20)    13832 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js
--rw-r--r--   0 paul       (501) staff       (20)     4724 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.952013 dryad2dataverse-0.6.0/docs/dbase_structure/bower/anchor-js/
--rw-r--r--   0 paul       (501) staff       (20)     5332 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/anchor-js/anchor.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.960034 dryad2dataverse-0.6.0/docs/dbase_structure/bower/codemirror/
--rw-r--r--   0 paul       (501) staff       (20)     8241 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/codemirror/codemirror.css
--rw-r--r--   0 paul       (501) staff       (20)   365757 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/codemirror/codemirror.js
--rw-r--r--   0 paul       (501) staff       (20)    37494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/codemirror/sql.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.961896 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net/
--rw-r--r--   0 paul       (501) staff       (20)    83268 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.783330 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.966183 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/css/
--rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css
--rw-r--r--   0 paul       (501) staff       (20)     4188 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.968515 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/js/
--rw-r--r--   0 paul       (501) staff       (20)     4559 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js
--rw-r--r--   0 paul       (501) staff       (20)     1966 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.984418 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/
--rw-r--r--   0 paul       (501) staff       (20)     5156 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js
--rw-r--r--   0 paul       (501) staff       (20)     2704 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js
--rw-r--r--   0 paul       (501) staff       (20)    45617 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js
--rw-r--r--   0 paul       (501) staff       (20)    25454 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js
--rw-r--r--   0 paul       (501) staff       (20)    42036 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js
--rw-r--r--   0 paul       (501) staff       (20)    23418 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js
--rw-r--r--   0 paul       (501) staff       (20)     4446 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js
--rw-r--r--   0 paul       (501) staff       (20)     1950 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js
--rw-r--r--   0 paul       (501) staff       (20)    40956 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js
--rw-r--r--   0 paul       (501) staff       (20)    16520 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.784950 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.987346 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/css/
--rw-r--r--   0 paul       (501) staff       (20)     3425 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css
--rw-r--r--   0 paul       (501) staff       (20)     2867 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.996069 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/js/
--rw-r--r--   0 paul       (501) staff       (20)     1400 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js
--rw-r--r--   0 paul       (501) staff       (20)      939 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.800553 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.016592 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/css/
--rw-r--r--   0 paul       (501) staff       (20)    37414 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/css/font-awesome.css
--rw-r--r--   0 paul       (501) staff       (20)    21778 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 paul       (501) staff       (20)    31000 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.165111 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/
--rw-r--r--   0 paul       (501) staff       (20)   134808 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 paul       (501) staff       (20)   165742 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 paul       (501) staff       (20)   444379 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 paul       (501) staff       (20)   165548 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 paul       (501) staff       (20)    98024 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 paul       (501) staff       (20)    77160 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.167554 dryad2dataverse-0.6.0/docs/dbase_structure/bower/html5shiv/
--rw-r--r--   0 paul       (501) staff       (20)     2730 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/html5shiv/html5shiv.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.802091 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.170743 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/css/
--rw-r--r--   0 paul       (501) staff       (20)    57193 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/css/ionicons.css
--rw-r--r--   0 paul       (501) staff       (20)    51284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/css/ionicons.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.186510 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/
--rw-r--r--   0 paul       (501) staff       (20)   120724 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot
--rw-r--r--   0 paul       (501) staff       (20)   333834 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg
--rw-r--r--   0 paul       (501) staff       (20)   188508 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf
--rw-r--r--   0 paul       (501) staff       (20)    67904 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.189319 dryad2dataverse-0.6.0/docs/dbase_structure/bower/jquery/
--rw-r--r--   0 paul       (501) staff       (20)   268039 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/jquery/jquery.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.194365 dryad2dataverse-0.6.0/docs/dbase_structure/bower/js-xlsx/
--rw-r--r--   0 paul       (501) staff       (20)   889680 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.217470 dryad2dataverse-0.6.0/docs/dbase_structure/bower/pdfmake/
--rw-r--r--   0 paul       (501) staff       (20)   971544 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/pdfmake/pdfmake.min.js
--rw-r--r--   0 paul       (501) staff       (20)   870284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/pdfmake/vfs_fonts.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.228499 dryad2dataverse-0.6.0/docs/dbase_structure/bower/respond/
--rw-r--r--   0 paul       (501) staff       (20)     4377 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/respond/respond.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.232171 dryad2dataverse-0.6.0/docs/dbase_structure/bower/salvattore/
--rw-r--r--   0 paul       (501) staff       (20)     1010 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/salvattore/salvattore.css
--rw-r--r--   0 paul       (501) staff       (20)     7493 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/bower/salvattore/salvattore.min.js
--rw-r--r--   0 paul       (501) staff       (20)     3176 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/column.js
--rw-r--r--   0 paul       (501) staff       (20)    16507 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/columns.html
--rw-r--r--   0 paul       (501) staff       (20)      380 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/constraint.js
--rw-r--r--   0 paul       (501) staff       (20)    15861 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/constraints.html
--rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.6.0/docs/dbase_structure/deletionOrder.txt
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.805770 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.234744 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/orphans/
--rw-r--r--   0 paul       (501) staff       (20)     1179 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/orphans/orphans.dot
--rw-r--r--   0 paul       (501) staff       (20)     6317 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/orphans/orphans.png
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.242029 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/
--rw-r--r--   0 paul       (501) staff       (20)     5456 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot
--rw-r--r--   0 paul       (501) staff       (20)    36361 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.compact.png
--rw-r--r--   0 paul       (501) staff       (20)     8661 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.large.dot
--rw-r--r--   0 paul       (501) staff       (20)    47530 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.large.png
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.289241 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/
--rw-r--r--   0 paul       (501) staff       (20)     2669 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    17276 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    43300 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     6778 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    47100 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     3965 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    24110 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     6134 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    48156 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     2633 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    15977 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     4802 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    41663 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     3001 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    19748 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     5135 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    44662 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     1247 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)     8986 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     4925 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml
--rw-r--r--   0 paul       (501) staff       (20)     1411 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/favicon.png
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.806904 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.303743 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/
--rw-r--r--   0 paul       (501) staff       (20)    20885 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot
--rw-r--r--   0 paul       (501) staff       (20)   133421 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg
--rw-r--r--   0 paul       (501) staff       (20)    34336 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf
--rw-r--r--   0 paul       (501) staff       (20)    22020 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff
--rw-r--r--   0 paul       (501) staff       (20)    19348 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2
--rw-r--r--   0 paul       (501) staff       (20)      678 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.463839 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/
--rw-r--r--   0 paul       (501) staff       (20)    17228 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot
--rw-r--r--   0 paul       (501) staff       (20)    60850 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg
--rw-r--r--   0 paul       (501) staff       (20)    37012 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff
--rw-r--r--   0 paul       (501) staff       (20)    14588 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2
--rw-r--r--   0 paul       (501) staff       (20)    16121 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot
--rw-r--r--   0 paul       (501) staff       (20)    61886 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg
--rw-r--r--   0 paul       (501) staff       (20)    34424 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf
--rw-r--r--   0 paul       (501) staff       (20)    17524 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff
--rw-r--r--   0 paul       (501) staff       (20)    13856 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2
--rw-r--r--   0 paul       (501) staff       (20)    17220 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot
--rw-r--r--   0 paul       (501) staff       (20)    58839 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg
--rw-r--r--   0 paul       (501) staff       (20)    36492 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff
--rw-r--r--   0 paul       (501) staff       (20)    14508 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2
--rw-r--r--   0 paul       (501) staff       (20)    16137 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot
--rw-r--r--   0 paul       (501) staff       (20)    61170 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg
--rw-r--r--   0 paul       (501) staff       (20)    34044 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf
--rw-r--r--   0 paul       (501) staff       (20)    17368 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff
--rw-r--r--   0 paul       (501) staff       (20)    13688 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2
--rw-r--r--   0 paul       (501) staff       (20)    16896 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot
--rw-r--r--   0 paul       (501) staff       (20)    58483 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg
--rw-r--r--   0 paul       (501) staff       (20)    36516 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18056 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff
--rw-r--r--   0 paul       (501) staff       (20)    14440 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2
--rw-r--r--   0 paul       (501) staff       (20)    17231 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot
--rw-r--r--   0 paul       (501) staff       (20)    60072 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg
--rw-r--r--   0 paul       (501) staff       (20)    36828 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff
--rw-r--r--   0 paul       (501) staff       (20)    14624 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2
--rw-r--r--   0 paul       (501) staff       (20)     4561 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.472407 dryad2dataverse-0.6.0/docs/dbase_structure/images/
--rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/images/foreignKey.png
--rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/images/foreignKeys.png
--rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/images/primaryKey.png
--rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/images/primaryKeys.png
--rw-r--r--   0 paul       (501) staff       (20)    19325 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/index.html
--rw-r--r--   0 paul       (501) staff       (20)      147 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/info-html.txt
--rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.6.0/docs/dbase_structure/insertionOrder.txt
--rw-r--r--   0 paul       (501) staff       (20)     1593 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/main.js
--rw-r--r--   0 paul       (501) staff       (20)     8284 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/orphans.html
--rw-r--r--   0 paul       (501) staff       (20)    10931 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/relationships.html
--rw-r--r--   0 paul       (501) staff       (20)      410 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/relationships.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.473801 dryad2dataverse-0.6.0/docs/dbase_structure/routines/
--rw-r--r--   0 paul       (501) staff       (20)      750 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/routines/routine.js
--rw-r--r--   0 paul       (501) staff       (20)     9154 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/routines.html
--rw-r--r--   0 paul       (501) staff       (20)     2069 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/routines.js
--rw-r--r--   0 paul       (501) staff       (20)     2535 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/schemaSpy.css
--rw-r--r--   0 paul       (501) staff       (20)     1622 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.0/docs/dbase_structure/schemaSpy.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.486591 dryad2dataverse-0.6.0/docs/dbase_structure/tables/
--rw-r--r--   0 paul       (501) staff       (20)    15902 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/tables/dryadFiles.html
--rw-r--r--   0 paul       (501) staff       (20)    21507 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/tables/dryadStudy.html
--rw-r--r--   0 paul       (501) staff       (20)    19567 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/tables/dvFiles.html
--rw-r--r--   0 paul       (501) staff       (20)    15866 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/tables/dvStudy.html
--rw-r--r--   0 paul       (501) staff       (20)    16840 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/tables/failed_uploads.html
--rw-r--r--   0 paul       (501) staff       (20)    12927 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/tables/lastcheck.html
--rw-r--r--   0 paul       (501) staff       (20)     1963 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/dbase_structure/tables/table.js
--rw-r--r--   0 paul       (501) staff       (20)     8840 2022-12-07 23:40:02.000000 dryad2dataverse-0.6.0/docs/faq.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.507339 dryad2dataverse-0.6.0/docs/images/
--rw-r--r--   0 paul       (501) staff       (20)    30150 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.0/docs/images/dryad2dataverseLogo.png
--rw-r--r--   0 paul       (501) staff       (20)    11191 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.0/docs/images/dryad2dataverseLogo.svg
--rw-r--r--   0 paul       (501) staff       (20)     5538 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/index.md
--rw-r--r--   0 paul       (501) staff       (20)     2518 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/installation.md
--rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.6.0/docs/other_utils.md
--rw-r--r--   0 paul       (501) staff       (20)     1132 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/pydoc-markdown.yml
--rw-r--r--   0 paul       (501) staff       (20)     5219 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.0/docs/reference.md
--rw-r--r--   0 paul       (501) staff       (20)     8280 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/docs/script.md
--rw-r--r--   0 paul       (501) staff       (20)      294 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.0/docs/track.md
--rw-r--r--   0 paul       (501) staff       (20)     1136 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.0/license.md
--rw-r--r--   0 paul       (501) staff       (20)      705 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/mkdocs.yml
--rw-r--r--   0 paul       (501) staff       (20)     1933 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/pyproject.toml
--rw-r--r--   0 paul       (501) staff       (20)      129 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-05-03 20:16:20.537931 dryad2dataverse-0.6.0/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)      450 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:19.809451 dryad2dataverse-0.6.0/src/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.519985 dryad2dataverse-0.6.0/src/dryad2dataverse/
--rw-r--r--   0 paul       (501) staff       (20)      712 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     1430 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/constants.py
--rw-r--r--   0 paul       (501) staff       (20)     1008 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/exceptions.py
--rw-r--r--   0 paul       (501) staff       (20)     1487 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/handlers.py
--rw-r--r--   0 paul       (501) staff       (20)    26267 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/monitor.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.525844 dryad2dataverse-0.6.0/src/dryad2dataverse/scripts/
--rw-r--r--   0 paul       (501) staff       (20)    26291 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/scripts/dryadd.py
--rw-r--r--   0 paul       (501) staff       (20)    33476 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/serializer.py
--rw-r--r--   0 paul       (501) staff       (20)    34125 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/src/dryad2dataverse/transfer.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.525046 dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     3019 2023-05-03 20:16:19.000000 dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)    11378 2023-05-03 20:16:19.000000 dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-03 20:16:19.000000 dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 20:16:19.000000 dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/entry_points.txt
--rw-r--r--   0 paul       (501) staff       (20)      129 2023-05-03 20:16:19.000000 dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       16 2023-05-03 20:16:19.000000 dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/top_level.txt
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 20:16:20.535560 dryad2dataverse-0.6.0/tests/
--rw-r--r--   0 paul       (501) staff       (20)        0 2021-09-22 18:45:47.000000 dryad2dataverse-0.6.0/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     8799 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.0/tests/badURL.json
--rw-r--r--   0 paul       (501) staff       (20)     6281 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/tests/tests_monitor.py
--rw-r--r--   0 paul       (501) staff       (20)    12401 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/tests/tests_serializer.py
--rw-r--r--   0 paul       (501) staff       (20)     2466 2023-05-03 18:51:22.000000 dryad2dataverse-0.6.0/tests/tests_transfer.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.963090 dryad2dataverse-0.6.1/
+-rw-r--r--   0 paul       (501) staff       (20)      485 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/.gitignore
+-rw-r--r--   0 paul       (501) staff       (20)     3019 2023-05-11 16:04:13.961567 dryad2dataverse-0.6.1/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     2033 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.518020 dryad2dataverse-0.6.1/docs/
+-rw-r--r--   0 paul       (501) staff       (20)      442 2021-11-29 23:23:23.000000 dryad2dataverse-0.6.1/docs/_config.yml
+-rw-r--r--   0 paul       (501) staff       (20)    26768 2022-12-07 22:06:06.000000 dryad2dataverse-0.6.1/docs/api_reference.md
+-rw-r--r--   0 paul       (501) staff       (20)     4855 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/changelog.md
+-rw-r--r--   0 paul       (501) staff       (20)     1631 2022-04-14 21:51:21.000000 dryad2dataverse-0.6.1/docs/compiling.md
+-rw-r--r--   0 paul       (501) staff       (20)     1152 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/credits.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.518994 dryad2dataverse-0.6.1/docs/css/
+-rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.6.1/docs/css/extra.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.579989 dryad2dataverse-0.6.1/docs/dbase_structure/
+-rw-r--r--   0 paul       (501) staff       (20)    19355 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/anomalies.html
+-rw-r--r--   0 paul       (501) staff       (20)        0 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/anomalies.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.480185 dryad2dataverse-0.6.1/docs/dbase_structure/bower/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.471047 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.470828 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.602235 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/
+-rw-r--r--   0 paul       (501) staff       (20)    26132 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css
+-rw-r--r--   0 paul       (501) staff       (20)    47706 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map
+-rw-r--r--   0 paul       (501) staff       (20)    23409 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 paul       (501) staff       (20)    25648 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 paul       (501) staff       (20)   146010 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css
+-rw-r--r--   0 paul       (501) staff       (20)   389287 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 paul       (501) staff       (20)   121200 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 paul       (501) staff       (20)   542194 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.618268 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/
+-rw-r--r--   0 paul       (501) staff       (20)    20127 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 paul       (501) staff       (20)   108738 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 paul       (501) staff       (20)    45404 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    23424 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 paul       (501) staff       (20)    18028 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.624345 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/
+-rw-r--r--   0 paul       (501) staff       (20)    69707 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js
+-rw-r--r--   0 paul       (501) staff       (20)    37045 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 paul       (501) staff       (20)      484 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/npm.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.471859 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.627079 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/
+-rw-r--r--   0 paul       (501) staff       (20)    25965 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js
+-rw-r--r--   0 paul       (501) staff       (20)     8776 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.632969 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQuery/
+-rw-r--r--   0 paul       (501) staff       (20)    85659 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.642166 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/
+-rw-r--r--   0 paul       (501) staff       (20)   470596 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js
+-rw-r--r--   0 paul       (501) staff       (20)   240427 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.647577 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/
+-rw-r--r--   0 paul       (501) staff       (20)    13832 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js
+-rw-r--r--   0 paul       (501) staff       (20)     4724 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.648998 dryad2dataverse-0.6.1/docs/dbase_structure/bower/anchor-js/
+-rw-r--r--   0 paul       (501) staff       (20)     5332 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/anchor-js/anchor.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.661098 dryad2dataverse-0.6.1/docs/dbase_structure/bower/codemirror/
+-rw-r--r--   0 paul       (501) staff       (20)     8241 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/codemirror/codemirror.css
+-rw-r--r--   0 paul       (501) staff       (20)   365757 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/codemirror/codemirror.js
+-rw-r--r--   0 paul       (501) staff       (20)    37494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/codemirror/sql.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.662840 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net/
+-rw-r--r--   0 paul       (501) staff       (20)    83268 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.474096 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.666283 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/css/
+-rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css
+-rw-r--r--   0 paul       (501) staff       (20)     4188 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.667965 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/js/
+-rw-r--r--   0 paul       (501) staff       (20)     4559 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js
+-rw-r--r--   0 paul       (501) staff       (20)     1966 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.687729 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/
+-rw-r--r--   0 paul       (501) staff       (20)     5156 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js
+-rw-r--r--   0 paul       (501) staff       (20)     2704 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js
+-rw-r--r--   0 paul       (501) staff       (20)    45617 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js
+-rw-r--r--   0 paul       (501) staff       (20)    25454 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js
+-rw-r--r--   0 paul       (501) staff       (20)    42036 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js
+-rw-r--r--   0 paul       (501) staff       (20)    23418 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js
+-rw-r--r--   0 paul       (501) staff       (20)     4446 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js
+-rw-r--r--   0 paul       (501) staff       (20)     1950 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js
+-rw-r--r--   0 paul       (501) staff       (20)    40956 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js
+-rw-r--r--   0 paul       (501) staff       (20)    16520 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.475585 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.689641 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/
+-rw-r--r--   0 paul       (501) staff       (20)     3425 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css
+-rw-r--r--   0 paul       (501) staff       (20)     2867 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.691261 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/
+-rw-r--r--   0 paul       (501) staff       (20)     1400 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js
+-rw-r--r--   0 paul       (501) staff       (20)      939 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.476594 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.708604 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/css/
+-rw-r--r--   0 paul       (501) staff       (20)    37414 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css
+-rw-r--r--   0 paul       (501) staff       (20)    21778 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 paul       (501) staff       (20)    31000 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.727526 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/
+-rw-r--r--   0 paul       (501) staff       (20)   134808 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 paul       (501) staff       (20)   165742 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 paul       (501) staff       (20)   444379 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 paul       (501) staff       (20)   165548 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    98024 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 paul       (501) staff       (20)    77160 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.729972 dryad2dataverse-0.6.1/docs/dbase_structure/bower/html5shiv/
+-rw-r--r--   0 paul       (501) staff       (20)     2730 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/html5shiv/html5shiv.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.478119 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.732637 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/css/
+-rw-r--r--   0 paul       (501) staff       (20)    57193 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/css/ionicons.css
+-rw-r--r--   0 paul       (501) staff       (20)    51284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/css/ionicons.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.745034 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/
+-rw-r--r--   0 paul       (501) staff       (20)   120724 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot
+-rw-r--r--   0 paul       (501) staff       (20)   333834 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg
+-rw-r--r--   0 paul       (501) staff       (20)   188508 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    67904 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.747719 dryad2dataverse-0.6.1/docs/dbase_structure/bower/jquery/
+-rw-r--r--   0 paul       (501) staff       (20)   268039 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/jquery/jquery.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.751349 dryad2dataverse-0.6.1/docs/dbase_structure/bower/js-xlsx/
+-rw-r--r--   0 paul       (501) staff       (20)   889680 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.767423 dryad2dataverse-0.6.1/docs/dbase_structure/bower/pdfmake/
+-rw-r--r--   0 paul       (501) staff       (20)   971544 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/pdfmake/pdfmake.min.js
+-rw-r--r--   0 paul       (501) staff       (20)   870284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/pdfmake/vfs_fonts.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.778369 dryad2dataverse-0.6.1/docs/dbase_structure/bower/respond/
+-rw-r--r--   0 paul       (501) staff       (20)     4377 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/respond/respond.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.781710 dryad2dataverse-0.6.1/docs/dbase_structure/bower/salvattore/
+-rw-r--r--   0 paul       (501) staff       (20)     1010 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/salvattore/salvattore.css
+-rw-r--r--   0 paul       (501) staff       (20)     7493 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/bower/salvattore/salvattore.min.js
+-rw-r--r--   0 paul       (501) staff       (20)     3176 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/column.js
+-rw-r--r--   0 paul       (501) staff       (20)    16507 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/columns.html
+-rw-r--r--   0 paul       (501) staff       (20)      380 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/constraint.js
+-rw-r--r--   0 paul       (501) staff       (20)    15861 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/constraints.html
+-rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.6.1/docs/dbase_structure/deletionOrder.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.481704 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.783950 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/orphans/
+-rw-r--r--   0 paul       (501) staff       (20)     1179 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/orphans/orphans.dot
+-rw-r--r--   0 paul       (501) staff       (20)     6317 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/orphans/orphans.png
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.788290 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/
+-rw-r--r--   0 paul       (501) staff       (20)     5456 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot
+-rw-r--r--   0 paul       (501) staff       (20)    36361 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.png
+-rw-r--r--   0 paul       (501) staff       (20)     8661 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.large.dot
+-rw-r--r--   0 paul       (501) staff       (20)    47530 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.large.png
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.824447 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/
+-rw-r--r--   0 paul       (501) staff       (20)     2669 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    17276 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    43300 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     6778 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    47100 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     3965 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    24110 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     6134 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    48156 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     2633 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    15977 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     4802 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    41663 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     3001 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    19748 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     5135 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    44662 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     1247 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)     8986 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     4925 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml
+-rw-r--r--   0 paul       (501) staff       (20)     1411 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/favicon.png
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.482848 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.837923 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/
+-rw-r--r--   0 paul       (501) staff       (20)    20885 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot
+-rw-r--r--   0 paul       (501) staff       (20)   133421 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg
+-rw-r--r--   0 paul       (501) staff       (20)    34336 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    22020 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff
+-rw-r--r--   0 paul       (501) staff       (20)    19348 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2
+-rw-r--r--   0 paul       (501) staff       (20)      678 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.908191 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/
+-rw-r--r--   0 paul       (501) staff       (20)    17228 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot
+-rw-r--r--   0 paul       (501) staff       (20)    60850 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg
+-rw-r--r--   0 paul       (501) staff       (20)    37012 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14588 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    16121 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot
+-rw-r--r--   0 paul       (501) staff       (20)    61886 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg
+-rw-r--r--   0 paul       (501) staff       (20)    34424 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    17524 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff
+-rw-r--r--   0 paul       (501) staff       (20)    13856 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    17220 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot
+-rw-r--r--   0 paul       (501) staff       (20)    58839 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg
+-rw-r--r--   0 paul       (501) staff       (20)    36492 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14508 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    16137 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot
+-rw-r--r--   0 paul       (501) staff       (20)    61170 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg
+-rw-r--r--   0 paul       (501) staff       (20)    34044 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    17368 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff
+-rw-r--r--   0 paul       (501) staff       (20)    13688 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    16896 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot
+-rw-r--r--   0 paul       (501) staff       (20)    58483 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg
+-rw-r--r--   0 paul       (501) staff       (20)    36516 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18056 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14440 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    17231 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot
+-rw-r--r--   0 paul       (501) staff       (20)    60072 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg
+-rw-r--r--   0 paul       (501) staff       (20)    36828 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14624 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2
+-rw-r--r--   0 paul       (501) staff       (20)     4561 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.913476 dryad2dataverse-0.6.1/docs/dbase_structure/images/
+-rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/images/foreignKey.png
+-rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/images/foreignKeys.png
+-rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/images/primaryKey.png
+-rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/images/primaryKeys.png
+-rw-r--r--   0 paul       (501) staff       (20)    19325 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/index.html
+-rw-r--r--   0 paul       (501) staff       (20)      147 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/info-html.txt
+-rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.6.1/docs/dbase_structure/insertionOrder.txt
+-rw-r--r--   0 paul       (501) staff       (20)     1593 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/main.js
+-rw-r--r--   0 paul       (501) staff       (20)     8284 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/orphans.html
+-rw-r--r--   0 paul       (501) staff       (20)    10931 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/relationships.html
+-rw-r--r--   0 paul       (501) staff       (20)      410 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/relationships.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.914755 dryad2dataverse-0.6.1/docs/dbase_structure/routines/
+-rw-r--r--   0 paul       (501) staff       (20)      750 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/routines/routine.js
+-rw-r--r--   0 paul       (501) staff       (20)     9154 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/routines.html
+-rw-r--r--   0 paul       (501) staff       (20)     2069 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/routines.js
+-rw-r--r--   0 paul       (501) staff       (20)     2535 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/schemaSpy.css
+-rw-r--r--   0 paul       (501) staff       (20)     1622 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.1/docs/dbase_structure/schemaSpy.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.923647 dryad2dataverse-0.6.1/docs/dbase_structure/tables/
+-rw-r--r--   0 paul       (501) staff       (20)    15902 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/tables/dryadFiles.html
+-rw-r--r--   0 paul       (501) staff       (20)    21507 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/tables/dryadStudy.html
+-rw-r--r--   0 paul       (501) staff       (20)    19567 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/tables/dvFiles.html
+-rw-r--r--   0 paul       (501) staff       (20)    15866 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/tables/dvStudy.html
+-rw-r--r--   0 paul       (501) staff       (20)    16840 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/tables/failed_uploads.html
+-rw-r--r--   0 paul       (501) staff       (20)    12927 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/tables/lastcheck.html
+-rw-r--r--   0 paul       (501) staff       (20)     1963 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/dbase_structure/tables/table.js
+-rw-r--r--   0 paul       (501) staff       (20)     8840 2022-12-07 23:40:02.000000 dryad2dataverse-0.6.1/docs/faq.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.929400 dryad2dataverse-0.6.1/docs/images/
+-rw-r--r--   0 paul       (501) staff       (20)    30150 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.1/docs/images/dryad2dataverseLogo.png
+-rw-r--r--   0 paul       (501) staff       (20)    11191 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.1/docs/images/dryad2dataverseLogo.svg
+-rw-r--r--   0 paul       (501) staff       (20)     5538 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/index.md
+-rw-r--r--   0 paul       (501) staff       (20)     2518 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/installation.md
+-rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.6.1/docs/other_utils.md
+-rw-r--r--   0 paul       (501) staff       (20)     1132 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/pydoc-markdown.yml
+-rw-r--r--   0 paul       (501) staff       (20)     5219 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.1/docs/reference.md
+-rw-r--r--   0 paul       (501) staff       (20)     8280 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/docs/script.md
+-rw-r--r--   0 paul       (501) staff       (20)      294 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.1/docs/track.md
+-rw-r--r--   0 paul       (501) staff       (20)     1136 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.1/license.md
+-rw-r--r--   0 paul       (501) staff       (20)      705 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/mkdocs.yml
+-rw-r--r--   0 paul       (501) staff       (20)     1933 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/pyproject.toml
+-rw-r--r--   0 paul       (501) staff       (20)      129 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-05-11 16:04:13.963463 dryad2dataverse-0.6.1/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)      450 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.490454 dryad2dataverse-0.6.1/src/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.949196 dryad2dataverse-0.6.1/src/dryad2dataverse/
+-rw-r--r--   0 paul       (501) staff       (20)      712 2023-05-11 15:55:58.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     1429 2023-05-11 15:52:57.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/constants.py
+-rw-r--r--   0 paul       (501) staff       (20)     1008 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/exceptions.py
+-rw-r--r--   0 paul       (501) staff       (20)     1487 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/handlers.py
+-rw-r--r--   0 paul       (501) staff       (20)    26267 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/monitor.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.954590 dryad2dataverse-0.6.1/src/dryad2dataverse/scripts/
+-rw-r--r--   0 paul       (501) staff       (20)    26291 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/scripts/dryadd.py
+-rw-r--r--   0 paul       (501) staff       (20)    33476 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/serializer.py
+-rw-r--r--   0 paul       (501) staff       (20)    34125 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse/transfer.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.954142 dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     3019 2023-05-11 16:04:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)    11378 2023-05-11 16:04:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-11 16:04:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-11 16:04:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/entry_points.txt
+-rw-r--r--   0 paul       (501) staff       (20)      129 2023-05-11 16:04:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       16 2023-05-11 16:04:13.000000 dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/top_level.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 16:04:13.960182 dryad2dataverse-0.6.1/tests/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2021-09-22 18:45:47.000000 dryad2dataverse-0.6.1/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     8799 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.1/tests/badURL.json
+-rw-r--r--   0 paul       (501) staff       (20)     6281 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/tests/tests_monitor.py
+-rw-r--r--   0 paul       (501) staff       (20)    12401 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/tests/tests_serializer.py
+-rw-r--r--   0 paul       (501) staff       (20)     2466 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.1/tests/tests_transfer.py
```

### Comparing `dryad2dataverse-0.6.0/PKG-INFO` & `dryad2dataverse-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dryad2dataverse
-Version: 0.6.0
+Version: 0.6.1
 Summary: Utility for copying and syncing data from a Dryad data repository to a Dataverse repository
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dryad2dataverse
 Project-URL: Documentation, https://ubc-library-rc.github.io/dryad2dataverse
 Project-URL: Repository, https://github.com/ubc-library-rc/dryad2dataverse.git
 Project-URL: Tracker, https://github.com/ubc-library-rc/dryad2dataverse/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository,Dryad,datadryad.org,dataverse.org
```

### Comparing `dryad2dataverse-0.6.0/README.md` & `dryad2dataverse-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/api_reference.md` & `dryad2dataverse-0.6.1/docs/api_reference.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/changelog.md` & `dryad2dataverse-0.6.1/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/compiling.md` & `dryad2dataverse-0.6.1/docs/compiling.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/credits.md` & `dryad2dataverse-0.6.1/docs/credits.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/anomalies.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/anomalies.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/anchor-js/anchor.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/anchor-js/anchor.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/codemirror/codemirror.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/codemirror/codemirror.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/codemirror/sql.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/codemirror/sql.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/css/font-awesome.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/html5shiv/html5shiv.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/html5shiv/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/css/ionicons.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/css/ionicons.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/css/ionicons.min.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/css/ionicons.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/jquery/jquery.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/pdfmake/pdfmake.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/pdfmake/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/pdfmake/vfs_fonts.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/pdfmake/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/respond/respond.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/respond/respond.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/salvattore/salvattore.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/salvattore/salvattore.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/bower/salvattore/salvattore.min.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/bower/salvattore/salvattore.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/column.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/column.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/columns.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/columns.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/constraints.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/constraints.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/orphans/orphans.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/orphans/orphans.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/orphans/orphans.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/orphans/orphans.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.compact.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.large.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.large.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/summary/relationships.real.large.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/summary/relationships.real.large.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml` & `dryad2dataverse-0.6.1/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/favicon.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/favicon.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/indieflower/indie-flower.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/indieflower/indie-flower.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/images/foreignKey.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/images/foreignKey.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/images/foreignKeys.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/images/foreignKeys.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/images/primaryKey.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/images/primaryKey.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/images/primaryKeys.png` & `dryad2dataverse-0.6.1/docs/dbase_structure/images/primaryKeys.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/index.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/index.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/main.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/main.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/orphans.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/orphans.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/relationships.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/relationships.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/routines/routine.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/routines/routine.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/routines.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/routines.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/routines.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/routines.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/schemaSpy.css` & `dryad2dataverse-0.6.1/docs/dbase_structure/schemaSpy.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/schemaSpy.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/schemaSpy.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/tables/dryadFiles.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/tables/dryadFiles.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/tables/dryadStudy.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/tables/dryadStudy.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/tables/dvFiles.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/tables/dvFiles.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/tables/dvStudy.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/tables/dvStudy.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/tables/failed_uploads.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/tables/failed_uploads.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/tables/lastcheck.html` & `dryad2dataverse-0.6.1/docs/dbase_structure/tables/lastcheck.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/dbase_structure/tables/table.js` & `dryad2dataverse-0.6.1/docs/dbase_structure/tables/table.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/faq.md` & `dryad2dataverse-0.6.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/images/dryad2dataverseLogo.png` & `dryad2dataverse-0.6.1/docs/images/dryad2dataverseLogo.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/images/dryad2dataverseLogo.svg` & `dryad2dataverse-0.6.1/docs/images/dryad2dataverseLogo.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/index.md` & `dryad2dataverse-0.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/installation.md` & `dryad2dataverse-0.6.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/pydoc-markdown.yml` & `dryad2dataverse-0.6.1/docs/pydoc-markdown.yml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/reference.md` & `dryad2dataverse-0.6.1/docs/reference.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/docs/script.md` & `dryad2dataverse-0.6.1/docs/script.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/license.md` & `dryad2dataverse-0.6.1/license.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/mkdocs.yml` & `dryad2dataverse-0.6.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/pyproject.toml` & `dryad2dataverse-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/__init__.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,10 +19,10 @@
     dryad2dataverse.monitor : Monitoring and database tools
     for maintaining a pipeline to Dataverse without unnecessary
     downloading and file duplication.
 
     dryad2dataverse.exceptions : Custom exceptions.
 '''
 
-VERSION = (0, 6, 0)
+VERSION = (0, 6, 1)
 
 __version__ = '.'.join([str(x) for x in VERSION])
```

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/constants.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #See :https://findwork.dev/blog/
 #advanced-usage-python-requests-timeouts-retries-hooks/#retry-on-failure
 #also
 #https://stackoverflow.com/questions/15431044/
 #can-i-set-max-retries-for-requests-request
 RETRY_STRATEGY = Retry(total=10,
                        status_forcelist=[429, 500, 502, 503, 504],
-                       method_whitelist=['HEAD', 'GET', 'OPTIONS',
+                       allowed_methods=['HEAD', 'GET', 'OPTIONS',
                                          'POST', 'PUT'],
                        backoff_factor=1)
 
 #used in dryad2dataverse.serializer
 DRYURL = 'https://datadryad.org'
 TMP = '/tmp'
```

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/exceptions.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/exceptions.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/handlers.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/handlers.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/monitor.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/monitor.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/scripts/dryadd.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/scripts/dryadd.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/serializer.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/serializer.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse/transfer.py` & `dryad2dataverse-0.6.1/src/dryad2dataverse/transfer.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/PKG-INFO` & `dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dryad2dataverse
-Version: 0.6.0
+Version: 0.6.1
 Summary: Utility for copying and syncing data from a Dryad data repository to a Dataverse repository
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dryad2dataverse
 Project-URL: Documentation, https://ubc-library-rc.github.io/dryad2dataverse
 Project-URL: Repository, https://github.com/ubc-library-rc/dryad2dataverse.git
 Project-URL: Tracker, https://github.com/ubc-library-rc/dryad2dataverse/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository,Dryad,datadryad.org,dataverse.org
```

### Comparing `dryad2dataverse-0.6.0/src/dryad2dataverse.egg-info/SOURCES.txt` & `dryad2dataverse-0.6.1/src/dryad2dataverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/tests/badURL.json` & `dryad2dataverse-0.6.1/tests/badURL.json`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/tests/tests_monitor.py` & `dryad2dataverse-0.6.1/tests/tests_monitor.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/tests/tests_serializer.py` & `dryad2dataverse-0.6.1/tests/tests_serializer.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.0/tests/tests_transfer.py` & `dryad2dataverse-0.6.1/tests/tests_transfer.py`

 * *Files identical despite different names*

