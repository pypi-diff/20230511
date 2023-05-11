# Comparing `tmp/devapps-2023.5.13.tar.gz` & `tmp/devapps-2023.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devapps-2023.5.13.tar", max compression
+gzip compressed data, was "devapps-2023.5.14.tar", max compression
```

## Comparing `devapps-2023.5.13.tar` & `devapps-2023.5.14.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.5.13/LICENSE
--rw-r--r--   0        0        0      992 2023-05-10 02:47:33.968713 devapps-2023.5.13/README.md
--rw-r--r--   0        0        0     5914 2023-05-10 12:49:47.080762 devapps-2023.5.13/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.5.13/src/ax/utils/__init__.py
--rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.5.13/src/ax/utils/ax_tree/__init__.py
--rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.5.13/src/ax/utils/ax_tree/_ax_tree.so
--rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.5.13/src/ax/utils/ax_tree/ax_tree.py
--rwxr-xr-x   0        0        0      491 2023-05-02 12:47:20.238964 devapps-2023.5.13/src/devapp/__init__.py
--rwxr-xr-x   0        0        0    19220 2023-05-02 12:47:20.238964 devapps-2023.5.13/src/devapp/app.py
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.238964 devapps-2023.5.13/src/devapp/app_token/__init__.py
--rwxr-xr-x   0        0        0     1201 2023-05-02 12:47:20.238964 devapps-2023.5.13/src/devapp/app_token/create_tokens.py
--rwxr-xr-x   0        0        0     2230 2023-05-02 12:47:20.238964 devapps-2023.5.13/src/devapp/app_token/read_tokens.py
--rwxr-xr-x   0        0        0      151 2023-05-02 12:47:20.239964 devapps-2023.5.13/src/devapp/app_token/verify_token
--rwxr-xr-x   0        0        0      297 2023-05-02 12:47:20.239964 devapps-2023.5.13/src/devapp/components/__init__.py
--rwxr-xr-x   0        0        0     6980 2023-05-02 12:47:20.239964 devapps-2023.5.13/src/devapp/components/cloudfoundry.py
--rwxr-xr-x   0        0        0     5956 2023-05-02 12:47:20.239964 devapps-2023.5.13/src/devapp/components/gitlab.py
--rwxr-xr-x   0        0        0     4828 2023-05-02 12:47:20.239964 devapps-2023.5.13/src/devapp/components/gitlab_runner.py
--rwxr-xr-x   0        0        0      150 2023-05-02 12:47:20.239964 devapps-2023.5.13/src/devapp/da.py
--rwxr-xr-x   0        0        0     1321 2023-05-02 12:47:20.239964 devapps-2023.5.13/src/devapp/dev_mode.py
--rwxr-xr-x   0        0        0     1636 2023-05-02 12:47:20.240964 devapps-2023.5.13/src/devapp/gevent_patched.py
--rwxr-xr-x   0        0        0     1549 2023-05-02 12:47:20.240964 devapps-2023.5.13/src/devapp/layer.py
--rwxr-xr-x   0        0        0      188 2023-05-02 12:47:20.240964 devapps-2023.5.13/src/devapp/lib/README.md
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.240964 devapps-2023.5.13/src/devapp/lib/__init__.py
--rwxr-xr-x   0        0        0   123141 2023-05-02 12:47:20.241964 devapps-2023.5.13/src/devapp/lib/sh.py
--rwxr-xr-x   0        0        0     2343 2023-05-02 12:47:20.241964 devapps-2023.5.13/src/devapp/load.py
--rwxr-xr-x   0        0        0      655 2023-05-02 12:47:20.241964 devapps-2023.5.13/src/devapp/logo
--rwxr-xr-x   0        0        0     1671 2023-05-02 12:47:20.241964 devapps-2023.5.13/src/devapp/max.py
--rw-r--r--   0        0        0     1933 2023-05-10 12:37:52.980662 devapps-2023.5.13/src/devapp/operations/resources.py
--rwxr-xr-x   0        0        0     1551 2023-05-02 12:47:20.241964 devapps-2023.5.13/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
--rwxr-xr-x   0        0        0     6445 2023-05-02 12:47:20.241964 devapps-2023.5.13/src/devapp/plugins/dev_devapp/repo_sym_links.py
--rw-r--r--   0        0        0     3090 2023-05-02 12:47:20.242964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resource_install.py
--rw-r--r--   0        0        0     4577 2023-05-02 12:47:20.242964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resource_run.py
--rw-r--r--   0        0        0     8983 2023-05-02 12:47:20.242964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resources.py.dis
--rw-r--r--   0        0        0      671 2023-05-02 12:47:20.242964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resources_list.py
--rw-r--r--   0        0        0      879 2023-05-02 12:47:20.242964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
--rwxr-xr-x   0        0        0     8688 2023-05-02 12:47:20.242964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/container_build.py
--rwxr-xr-x   0        0        0    10257 2023-05-02 12:47:20.242964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/container_pull.py
--rwxr-xr-x   0        0        0    28013 2023-05-02 12:47:20.243964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/fs_build.py
--rwxr-xr-x   0        0        0    13318 2023-05-02 12:47:20.243964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
--rwxr-xr-x   0        0        0     9232 2023-05-02 12:47:20.243964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
--rwxr-xr-x   0        0        0    12668 2023-05-02 12:47:20.243964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
--rwxr-xr-x   0        0        0     8750 2023-05-02 12:47:20.244964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/kubectl/__init__.py
--rwxr-xr-x   0        0        0     2975 2023-05-02 12:47:20.244964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/life_cycle.py
--rw-r--r--   0        0        0     1573 2023-05-02 12:47:20.244964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/log_view.py
--rwxr-xr-x   0        0        0    11773 2023-05-10 02:43:35.060661 devapps-2023.5.13/src/devapp/plugins/ops_devapp/project/__init__.py
--rw-r--r--   0        0        0     9960 2023-05-02 12:47:20.244964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
--rw-r--r--   0        0        0     4994 2023-05-02 12:47:20.245964 devapps-2023.5.13/src/devapp/plugins/ops_devapp/run.py
--rwxr-xr-x   0        0        0    28235 2023-05-02 12:47:20.245964 devapps-2023.5.13/src/devapp/run.py
--rwxr-xr-x   0        0        0    25984 2023-05-02 12:47:20.245964 devapps-2023.5.13/src/devapp/spec/build.py
--rwxr-xr-x   0        0        0     2929 2023-05-02 12:47:20.246964 devapps-2023.5.13/src/devapp/spec/find_paths_in_fs_components.py
--rwxr-xr-x   0        0        0    16176 2023-05-02 12:47:20.246964 devapps-2023.5.13/src/devapp/spec/fs_components.py
--rwxr-xr-x   0        0        0     1715 2023-05-02 12:47:20.246964 devapps-2023.5.13/src/devapp/spec/links.py
--rwxr-xr-x   0        0        0     2481 2023-05-02 12:47:20.246964 devapps-2023.5.13/src/devapp/spec/os_tools.py
--rwxr-xr-x   0        0        0     7913 2023-05-02 12:47:20.246964 devapps-2023.5.13/src/devapp/spec/templ.py
--rwxr-xr-x   0        0        0     1600 2023-05-02 12:47:20.246964 devapps-2023.5.13/src/devapp/spec/templates/unit
--rwxr-xr-x   0        0        0     7586 2023-05-02 12:47:20.247964 devapps-2023.5.13/src/devapp/spec/tools.py
--rwxr-xr-x   0        0        0    30671 2023-05-02 12:47:20.247964 devapps-2023.5.13/src/devapp/t
--rw-r--r--   0        0        0     3559 2023-05-02 12:47:20.247964 devapps-2023.5.13/src/devapp/testing/auto_docs.py
--rw-r--r--   0        0        0      443 2023-05-02 12:47:20.247964 devapps-2023.5.13/src/devapp/tests/test_unit_devapp.py
--rwxr-xr-x   0        0        0    13808 2023-05-02 12:47:20.247964 devapps-2023.5.13/src/devapp/third/rpl
--rwxr-xr-x   0        0        0    50010 2023-05-02 12:47:20.248964 devapps-2023.5.13/src/devapp/tools/__init__.py
--rw-r--r--   0        0        0     4025 2023-05-02 12:47:20.248964 devapps-2023.5.13/src/devapp/tools/flag.py
--rw-r--r--   0        0        0      731 2023-05-02 12:47:20.248964 devapps-2023.5.13/src/devapp/tools/http.py
--rw-r--r--   0        0        0    35701 2023-05-02 12:47:20.248964 devapps-2023.5.13/src/devapp/tools/infra/__init__.py
--rw-r--r--   0        0        0    16618 2023-05-02 12:47:20.248964 devapps-2023.5.13/src/devapp/tools/infra/actions.py
--rw-r--r--   0        0        0     3089 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/000:functions.sh
--rwxr-xr-x   0        0        0      375 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
--rwxr-xr-x   0        0        0     1521 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
--rwxr-xr-x   0        0        0      448 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/100:docker.sh
--rwxr-xr-x   0        0        0      324 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/200:tools.sh
--rwxr-xr-x   0        0        0      760 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/300:dns.sh
--rwxr-xr-x   0        0        0     4375 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/500:k3s.sh
--rwxr-xr-x   0        0        0      943 2023-05-02 12:47:20.249964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/501:kind.sh
--rwxr-xr-x   0        0        0    17210 2023-05-02 12:47:20.250964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/502:k3s.sh
--rw-r--r--   0        0        0      276 2023-05-02 12:47:20.250964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/510:label_workers.sh
--rwxr-xr-x   0        0        0      661 2023-05-02 12:47:20.250964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/600:longhorn.sh
--rw-r--r--   0        0        0     1737 2023-05-02 12:47:20.250964 devapps-2023.5.13/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
--rw-r--r--   0        0        0    26850 2023-05-10 05:18:44.984532 devapps-2023.5.13/src/devapp/tools/old.py
--rw-r--r--   0        0        0     4415 2023-05-03 12:55:53.147915 devapps-2023.5.13/src/devapp/tools/plugin.py
--rw-r--r--   0        0        0    27608 2023-05-10 12:44:20.346704 devapps-2023.5.13/src/devapp/tools/resource.py
--rw-r--r--   0        0        0     1861 2023-05-02 12:47:20.251964 devapps-2023.5.13/src/devapp/tools/times.py
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.251964 devapps-2023.5.13/src/devapp/utils/__init__.py
--rwxr-xr-x   0        0        0    15787 2023-05-02 12:47:20.251964 devapps-2023.5.13/src/devapp/utils/os_.py
--rwxr-xr-x   0        0        0     1871 2023-05-02 12:47:20.251964 devapps-2023.5.13/src/devapp/utils/py_source_env.py
--rwxr-xr-x   0        0        0     9335 2023-05-02 12:47:20.252964 devapps-2023.5.13/src/devapp/utils/rx_tools.py
--rwxr-xr-x   0        0        0    11529 2023-05-02 12:47:20.252964 devapps-2023.5.13/src/devapp/utils/vault.py
--rwxr-xr-x   0        0        0     2107 2023-05-02 12:47:20.252964 devapps-2023.5.13/src/devapp/utils/watch_dog.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.5.13/src/mdvl/__init__.py
--rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.5.13/src/mdvl/mdvl.py
--rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.5.13/src/mdvl/tools.py
--rwxr-xr-x   0        0        0      519 2023-03-22 14:30:25.735939 devapps-2023.5.13/src/structlogging/__init__.py
--rwxr-xr-x   0        0        0     1559 2023-03-22 14:30:25.735939 devapps-2023.5.13/src/structlogging/adapters.py
--rwxr-xr-x   0        0        0       88 2023-03-22 14:30:25.735939 devapps-2023.5.13/src/structlogging/common.py
--rwxr-xr-x   0        0        0     5503 2023-03-22 14:30:25.735939 devapps-2023.5.13/src/structlogging/config.py
--rwxr-xr-x   0        0        0     1618 2023-03-22 14:30:25.735939 devapps-2023.5.13/src/structlogging/formatters.py
--rwxr-xr-x   0        0        0     2640 2023-03-22 14:30:25.736939 devapps-2023.5.13/src/structlogging/processors.py
--rwxr-xr-x   0        0        0     5472 2023-03-22 14:30:25.736939 devapps-2023.5.13/src/structlogging/renderers.py
--rwxr-xr-x   0        0        0    11172 2023-05-02 12:28:38.054778 devapps-2023.5.13/src/structlogging/sl.py
--rw-r--r--   0        0        0     4022 2023-03-22 14:30:25.736939 devapps-2023.5.13/src/structlogging/stacktrace.py
--rwxr-xr-x   0        0        0     1355 2023-03-22 14:30:25.736939 devapps-2023.5.13/src/structlogging/tests/test_structlogging.py
--rwxr-xr-x   0        0        0      886 2023-05-02 12:47:20.254964 devapps-2023.5.13/src/theming/__init__.py
--rwxr-xr-x   0        0        0    14865 2023-05-02 12:47:20.254964 devapps-2023.5.13/src/theming/absl_color_help.py
--rwxr-xr-x   0        0        0     4345 2023-05-02 12:47:20.255964 devapps-2023.5.13/src/theming/ansi2html.py
--rwxr-xr-x   0        0        0    11888 2023-05-02 12:47:20.255964 devapps-2023.5.13/src/theming/ansi2html.sh
--rwxr-xr-x   0        0        0     3030 2023-05-02 12:47:20.255964 devapps-2023.5.13/src/theming/ansistrm.py
--rwxr-xr-x   0        0        0    10066 2023-05-02 12:47:20.255964 devapps-2023.5.13/src/theming/ax_xml.py
--rwxr-xr-x   0        0        0    10495 2023-05-02 12:47:20.255964 devapps-2023.5.13/src/theming/camel_snake.py
--rwxr-xr-x   0        0        0     7517 2023-05-02 12:47:20.256964 devapps-2023.5.13/src/theming/charting.py
--rwxr-xr-x   0        0        0     3392 2023-05-02 12:47:20.256964 devapps-2023.5.13/src/theming/colorhilite.py
--rwxr-xr-x   0        0        0     1113 2023-05-02 12:47:20.256964 devapps-2023.5.13/src/theming/filesize/README.txt
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.256964 devapps-2023.5.13/src/theming/filesize/__init__.py
--rwxr-xr-x   0        0        0     2549 2023-05-02 12:47:20.256964 devapps-2023.5.13/src/theming/filesize/filesize.py
--rwxr-xr-x   0        0        0     3756 2023-05-02 12:47:20.257964 devapps-2023.5.13/src/theming/formatters.py
--rw-r--r--   0        0        0     3807 2023-05-02 12:47:20.257964 devapps-2023.5.13/src/theming/formatting/markdown.py
--rw-r--r--   0        0        0     1241 2023-05-02 12:47:20.257964 devapps-2023.5.13/src/theming/formatting/viz_sequence.py
--rwxr-xr-x   0        0        0     3410 2023-05-02 12:47:20.257964 devapps-2023.5.13/src/theming/html_tools.py
--rwxr-xr-x   0        0        0    11409 2023-05-02 12:47:20.257964 devapps-2023.5.13/src/theming/inflect.py
--rwxr-xr-x   0        0        0      460 2023-05-02 12:47:20.258964 devapps-2023.5.13/src/theming/msgs.py
--rwxr-xr-x   0        0        0     9864 2023-05-02 12:47:20.258964 devapps-2023.5.13/src/theming/pretty_print.py
--rwxr-xr-x   0        0        0    55699 2023-05-02 12:47:20.258964 devapps-2023.5.13/src/theming/tablepretty.py
--rwxr-xr-x   0        0        0    13998 2023-05-02 12:47:20.259964 devapps-2023.5.13/src/theming/term.py
--rwxr-xr-x   0        0        0     1468 2023-05-02 12:47:20.259964 devapps-2023.5.13/src/theming/term_struct_hilite.py
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.13/src/theming/test
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.13/src/theming/tests/__init__.py
--rwxr-xr-x   0        0        0     9454 2023-05-02 12:47:20.260964 devapps-2023.5.13/src/theming/tests/test_text_formatting.py
--rwxr-xr-x   0        0        0     1063 2023-05-02 12:47:20.260964 devapps-2023.5.13/src/theming/tracebacks.py
--rwxr-xr-x   0        0        0     3011 2023-05-02 12:47:20.260964 devapps-2023.5.13/src/theming/unicode_chars.py
--rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.5.13/src/tree_builder/__init__.py
--rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.5.13/src/tree_builder/arch/__init__.py.bak
--rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.5.13/src/tree_builder/arch/links.py.bak
--rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.5.13/src/tree_builder/arch/o.py
--rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.5.13/src/tree_builder/arch/old
--rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.5.13/src/tree_builder/arch/olinit
--rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.5.13/src/tree_builder/arch/oo
--rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.5.13/src/tree_builder/arch/py2.py
--rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.5.13/src/tree_builder/arch/render.py.bak
--rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.5.13/src/tree_builder/chrome_reload.sh
--rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.5.13/src/tree_builder/delivery2.py
--rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.5.13/src/tree_builder/links.py
--rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.5.13/src/tree_builder/py3.py
--rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.5.13/src/tree_builder/render.py
--rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.5.13/src/tree_builder/version.py
--rw-r--r--   0        0        0     3038 2023-05-10 12:49:48.285171 devapps-2023.5.13/setup.py
--rw-r--r--   0        0        0     1805 2023-05-10 12:49:48.285487 devapps-2023.5.13/PKG-INFO
+-rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.5.14/LICENSE
+-rw-r--r--   0        0        0      992 2023-05-10 02:47:33.968713 devapps-2023.5.14/README.md
+-rw-r--r--   0        0        0     5914 2023-05-11 05:44:42.398839 devapps-2023.5.14/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.5.14/src/ax/utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.5.14/src/ax/utils/ax_tree/__init__.py
+-rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.5.14/src/ax/utils/ax_tree/_ax_tree.so
+-rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.5.14/src/ax/utils/ax_tree/ax_tree.py
+-rwxr-xr-x   0        0        0      491 2023-05-02 12:47:20.238964 devapps-2023.5.14/src/devapp/__init__.py
+-rwxr-xr-x   0        0        0    19220 2023-05-02 12:47:20.238964 devapps-2023.5.14/src/devapp/app.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.238964 devapps-2023.5.14/src/devapp/app_token/__init__.py
+-rwxr-xr-x   0        0        0     1201 2023-05-02 12:47:20.238964 devapps-2023.5.14/src/devapp/app_token/create_tokens.py
+-rwxr-xr-x   0        0        0     2230 2023-05-02 12:47:20.238964 devapps-2023.5.14/src/devapp/app_token/read_tokens.py
+-rwxr-xr-x   0        0        0      151 2023-05-02 12:47:20.239964 devapps-2023.5.14/src/devapp/app_token/verify_token
+-rwxr-xr-x   0        0        0      297 2023-05-02 12:47:20.239964 devapps-2023.5.14/src/devapp/components/__init__.py
+-rwxr-xr-x   0        0        0     6980 2023-05-02 12:47:20.239964 devapps-2023.5.14/src/devapp/components/cloudfoundry.py
+-rwxr-xr-x   0        0        0     5956 2023-05-02 12:47:20.239964 devapps-2023.5.14/src/devapp/components/gitlab.py
+-rwxr-xr-x   0        0        0     4828 2023-05-02 12:47:20.239964 devapps-2023.5.14/src/devapp/components/gitlab_runner.py
+-rwxr-xr-x   0        0        0      150 2023-05-02 12:47:20.239964 devapps-2023.5.14/src/devapp/da.py
+-rwxr-xr-x   0        0        0     1321 2023-05-02 12:47:20.239964 devapps-2023.5.14/src/devapp/dev_mode.py
+-rwxr-xr-x   0        0        0     1636 2023-05-02 12:47:20.240964 devapps-2023.5.14/src/devapp/gevent_patched.py
+-rwxr-xr-x   0        0        0     1549 2023-05-02 12:47:20.240964 devapps-2023.5.14/src/devapp/layer.py
+-rwxr-xr-x   0        0        0      188 2023-05-02 12:47:20.240964 devapps-2023.5.14/src/devapp/lib/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.240964 devapps-2023.5.14/src/devapp/lib/__init__.py
+-rwxr-xr-x   0        0        0   123141 2023-05-02 12:47:20.241964 devapps-2023.5.14/src/devapp/lib/sh.py
+-rwxr-xr-x   0        0        0     2343 2023-05-02 12:47:20.241964 devapps-2023.5.14/src/devapp/load.py
+-rwxr-xr-x   0        0        0      655 2023-05-02 12:47:20.241964 devapps-2023.5.14/src/devapp/logo
+-rwxr-xr-x   0        0        0     1671 2023-05-02 12:47:20.241964 devapps-2023.5.14/src/devapp/max.py
+-rw-r--r--   0        0        0     1933 2023-05-10 12:37:52.980662 devapps-2023.5.14/src/devapp/operations/resources.py
+-rwxr-xr-x   0        0        0     1551 2023-05-02 12:47:20.241964 devapps-2023.5.14/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     6445 2023-05-02 12:47:20.241964 devapps-2023.5.14/src/devapp/plugins/dev_devapp/repo_sym_links.py
+-rw-r--r--   0        0        0     3090 2023-05-02 12:47:20.242964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resource_install.py
+-rw-r--r--   0        0        0     4577 2023-05-02 12:47:20.242964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resource_run.py
+-rw-r--r--   0        0        0     8983 2023-05-02 12:47:20.242964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resources.py.dis
+-rw-r--r--   0        0        0      671 2023-05-02 12:47:20.242964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resources_list.py
+-rw-r--r--   0        0        0      879 2023-05-02 12:47:20.242964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
+-rwxr-xr-x   0        0        0     8688 2023-05-02 12:47:20.242964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/container_build.py
+-rwxr-xr-x   0        0        0    10257 2023-05-02 12:47:20.242964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/container_pull.py
+-rwxr-xr-x   0        0        0    28013 2023-05-02 12:47:20.243964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/fs_build.py
+-rwxr-xr-x   0        0        0    13318 2023-05-02 12:47:20.243964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
+-rwxr-xr-x   0        0        0     9232 2023-05-02 12:47:20.243964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
+-rwxr-xr-x   0        0        0    12668 2023-05-02 12:47:20.243964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
+-rwxr-xr-x   0        0        0     8750 2023-05-02 12:47:20.244964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/kubectl/__init__.py
+-rwxr-xr-x   0        0        0     2975 2023-05-02 12:47:20.244964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/life_cycle.py
+-rw-r--r--   0        0        0     1573 2023-05-02 12:47:20.244964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/log_view.py
+-rwxr-xr-x   0        0        0    11773 2023-05-10 02:43:35.060661 devapps-2023.5.14/src/devapp/plugins/ops_devapp/project/__init__.py
+-rw-r--r--   0        0        0     9960 2023-05-02 12:47:20.244964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
+-rw-r--r--   0        0        0     4994 2023-05-02 12:47:20.245964 devapps-2023.5.14/src/devapp/plugins/ops_devapp/run.py
+-rwxr-xr-x   0        0        0    28235 2023-05-02 12:47:20.245964 devapps-2023.5.14/src/devapp/run.py
+-rwxr-xr-x   0        0        0    25984 2023-05-02 12:47:20.245964 devapps-2023.5.14/src/devapp/spec/build.py
+-rwxr-xr-x   0        0        0     2929 2023-05-02 12:47:20.246964 devapps-2023.5.14/src/devapp/spec/find_paths_in_fs_components.py
+-rwxr-xr-x   0        0        0    16176 2023-05-02 12:47:20.246964 devapps-2023.5.14/src/devapp/spec/fs_components.py
+-rwxr-xr-x   0        0        0     1715 2023-05-02 12:47:20.246964 devapps-2023.5.14/src/devapp/spec/links.py
+-rwxr-xr-x   0        0        0     2481 2023-05-02 12:47:20.246964 devapps-2023.5.14/src/devapp/spec/os_tools.py
+-rwxr-xr-x   0        0        0     7913 2023-05-02 12:47:20.246964 devapps-2023.5.14/src/devapp/spec/templ.py
+-rwxr-xr-x   0        0        0     1600 2023-05-02 12:47:20.246964 devapps-2023.5.14/src/devapp/spec/templates/unit
+-rwxr-xr-x   0        0        0     7586 2023-05-02 12:47:20.247964 devapps-2023.5.14/src/devapp/spec/tools.py
+-rwxr-xr-x   0        0        0    30671 2023-05-02 12:47:20.247964 devapps-2023.5.14/src/devapp/t
+-rw-r--r--   0        0        0     3559 2023-05-02 12:47:20.247964 devapps-2023.5.14/src/devapp/testing/auto_docs.py
+-rw-r--r--   0        0        0      443 2023-05-02 12:47:20.247964 devapps-2023.5.14/src/devapp/tests/test_unit_devapp.py
+-rwxr-xr-x   0        0        0    13808 2023-05-02 12:47:20.247964 devapps-2023.5.14/src/devapp/third/rpl
+-rwxr-xr-x   0        0        0    50010 2023-05-02 12:47:20.248964 devapps-2023.5.14/src/devapp/tools/__init__.py
+-rw-r--r--   0        0        0     4025 2023-05-02 12:47:20.248964 devapps-2023.5.14/src/devapp/tools/flag.py
+-rw-r--r--   0        0        0      731 2023-05-02 12:47:20.248964 devapps-2023.5.14/src/devapp/tools/http.py
+-rw-r--r--   0        0        0    35701 2023-05-02 12:47:20.248964 devapps-2023.5.14/src/devapp/tools/infra/__init__.py
+-rw-r--r--   0        0        0    16618 2023-05-02 12:47:20.248964 devapps-2023.5.14/src/devapp/tools/infra/actions.py
+-rw-r--r--   0        0        0     3089 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/000:functions.sh
+-rwxr-xr-x   0        0        0      375 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
+-rwxr-xr-x   0        0        0     1521 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
+-rwxr-xr-x   0        0        0      448 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/100:docker.sh
+-rwxr-xr-x   0        0        0      324 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/200:tools.sh
+-rwxr-xr-x   0        0        0      760 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/300:dns.sh
+-rwxr-xr-x   0        0        0     4375 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/500:k3s.sh
+-rwxr-xr-x   0        0        0      943 2023-05-02 12:47:20.249964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/501:kind.sh
+-rwxr-xr-x   0        0        0    17210 2023-05-02 12:47:20.250964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/502:k3s.sh
+-rw-r--r--   0        0        0      276 2023-05-02 12:47:20.250964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/510:label_workers.sh
+-rwxr-xr-x   0        0        0      661 2023-05-02 12:47:20.250964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/600:longhorn.sh
+-rw-r--r--   0        0        0     1737 2023-05-02 12:47:20.250964 devapps-2023.5.14/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
+-rw-r--r--   0        0        0    26850 2023-05-10 05:18:44.984532 devapps-2023.5.14/src/devapp/tools/old.py
+-rw-r--r--   0        0        0     4415 2023-05-03 12:55:53.147915 devapps-2023.5.14/src/devapp/tools/plugin.py
+-rw-r--r--   0        0        0    27830 2023-05-11 05:25:28.444663 devapps-2023.5.14/src/devapp/tools/resource.py
+-rw-r--r--   0        0        0     1861 2023-05-02 12:47:20.251964 devapps-2023.5.14/src/devapp/tools/times.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.251964 devapps-2023.5.14/src/devapp/utils/__init__.py
+-rwxr-xr-x   0        0        0    15787 2023-05-02 12:47:20.251964 devapps-2023.5.14/src/devapp/utils/os_.py
+-rwxr-xr-x   0        0        0     1871 2023-05-02 12:47:20.251964 devapps-2023.5.14/src/devapp/utils/py_source_env.py
+-rwxr-xr-x   0        0        0     9335 2023-05-02 12:47:20.252964 devapps-2023.5.14/src/devapp/utils/rx_tools.py
+-rwxr-xr-x   0        0        0    11529 2023-05-02 12:47:20.252964 devapps-2023.5.14/src/devapp/utils/vault.py
+-rwxr-xr-x   0        0        0     2107 2023-05-02 12:47:20.252964 devapps-2023.5.14/src/devapp/utils/watch_dog.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.5.14/src/mdvl/__init__.py
+-rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.5.14/src/mdvl/mdvl.py
+-rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.5.14/src/mdvl/tools.py
+-rwxr-xr-x   0        0        0      519 2023-03-22 14:30:25.735939 devapps-2023.5.14/src/structlogging/__init__.py
+-rwxr-xr-x   0        0        0     1559 2023-03-22 14:30:25.735939 devapps-2023.5.14/src/structlogging/adapters.py
+-rwxr-xr-x   0        0        0       88 2023-03-22 14:30:25.735939 devapps-2023.5.14/src/structlogging/common.py
+-rwxr-xr-x   0        0        0     5503 2023-03-22 14:30:25.735939 devapps-2023.5.14/src/structlogging/config.py
+-rwxr-xr-x   0        0        0     1618 2023-03-22 14:30:25.735939 devapps-2023.5.14/src/structlogging/formatters.py
+-rwxr-xr-x   0        0        0     2640 2023-03-22 14:30:25.736939 devapps-2023.5.14/src/structlogging/processors.py
+-rwxr-xr-x   0        0        0     5472 2023-03-22 14:30:25.736939 devapps-2023.5.14/src/structlogging/renderers.py
+-rwxr-xr-x   0        0        0    11172 2023-05-02 12:28:38.054778 devapps-2023.5.14/src/structlogging/sl.py
+-rw-r--r--   0        0        0     4022 2023-03-22 14:30:25.736939 devapps-2023.5.14/src/structlogging/stacktrace.py
+-rwxr-xr-x   0        0        0     1355 2023-03-22 14:30:25.736939 devapps-2023.5.14/src/structlogging/tests/test_structlogging.py
+-rwxr-xr-x   0        0        0      886 2023-05-02 12:47:20.254964 devapps-2023.5.14/src/theming/__init__.py
+-rwxr-xr-x   0        0        0    14865 2023-05-02 12:47:20.254964 devapps-2023.5.14/src/theming/absl_color_help.py
+-rwxr-xr-x   0        0        0     4345 2023-05-02 12:47:20.255964 devapps-2023.5.14/src/theming/ansi2html.py
+-rwxr-xr-x   0        0        0    11888 2023-05-02 12:47:20.255964 devapps-2023.5.14/src/theming/ansi2html.sh
+-rwxr-xr-x   0        0        0     3030 2023-05-02 12:47:20.255964 devapps-2023.5.14/src/theming/ansistrm.py
+-rwxr-xr-x   0        0        0    10066 2023-05-02 12:47:20.255964 devapps-2023.5.14/src/theming/ax_xml.py
+-rwxr-xr-x   0        0        0    10495 2023-05-02 12:47:20.255964 devapps-2023.5.14/src/theming/camel_snake.py
+-rwxr-xr-x   0        0        0     7517 2023-05-02 12:47:20.256964 devapps-2023.5.14/src/theming/charting.py
+-rwxr-xr-x   0        0        0     3392 2023-05-02 12:47:20.256964 devapps-2023.5.14/src/theming/colorhilite.py
+-rwxr-xr-x   0        0        0     1113 2023-05-02 12:47:20.256964 devapps-2023.5.14/src/theming/filesize/README.txt
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.256964 devapps-2023.5.14/src/theming/filesize/__init__.py
+-rwxr-xr-x   0        0        0     2549 2023-05-02 12:47:20.256964 devapps-2023.5.14/src/theming/filesize/filesize.py
+-rwxr-xr-x   0        0        0     3756 2023-05-02 12:47:20.257964 devapps-2023.5.14/src/theming/formatters.py
+-rw-r--r--   0        0        0     3807 2023-05-02 12:47:20.257964 devapps-2023.5.14/src/theming/formatting/markdown.py
+-rw-r--r--   0        0        0     1241 2023-05-02 12:47:20.257964 devapps-2023.5.14/src/theming/formatting/viz_sequence.py
+-rwxr-xr-x   0        0        0     3410 2023-05-02 12:47:20.257964 devapps-2023.5.14/src/theming/html_tools.py
+-rwxr-xr-x   0        0        0    11409 2023-05-02 12:47:20.257964 devapps-2023.5.14/src/theming/inflect.py
+-rwxr-xr-x   0        0        0      460 2023-05-02 12:47:20.258964 devapps-2023.5.14/src/theming/msgs.py
+-rwxr-xr-x   0        0        0     9864 2023-05-02 12:47:20.258964 devapps-2023.5.14/src/theming/pretty_print.py
+-rwxr-xr-x   0        0        0    55699 2023-05-02 12:47:20.258964 devapps-2023.5.14/src/theming/tablepretty.py
+-rwxr-xr-x   0        0        0    13998 2023-05-02 12:47:20.259964 devapps-2023.5.14/src/theming/term.py
+-rwxr-xr-x   0        0        0     1468 2023-05-02 12:47:20.259964 devapps-2023.5.14/src/theming/term_struct_hilite.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.14/src/theming/test
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.14/src/theming/tests/__init__.py
+-rwxr-xr-x   0        0        0     9454 2023-05-02 12:47:20.260964 devapps-2023.5.14/src/theming/tests/test_text_formatting.py
+-rwxr-xr-x   0        0        0     1063 2023-05-02 12:47:20.260964 devapps-2023.5.14/src/theming/tracebacks.py
+-rwxr-xr-x   0        0        0     3011 2023-05-02 12:47:20.260964 devapps-2023.5.14/src/theming/unicode_chars.py
+-rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.5.14/src/tree_builder/__init__.py
+-rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.5.14/src/tree_builder/arch/__init__.py.bak
+-rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.5.14/src/tree_builder/arch/links.py.bak
+-rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.5.14/src/tree_builder/arch/o.py
+-rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.5.14/src/tree_builder/arch/old
+-rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.5.14/src/tree_builder/arch/olinit
+-rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.5.14/src/tree_builder/arch/oo
+-rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.5.14/src/tree_builder/arch/py2.py
+-rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.5.14/src/tree_builder/arch/render.py.bak
+-rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.5.14/src/tree_builder/chrome_reload.sh
+-rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.5.14/src/tree_builder/delivery2.py
+-rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.5.14/src/tree_builder/links.py
+-rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.5.14/src/tree_builder/py3.py
+-rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.5.14/src/tree_builder/render.py
+-rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.5.14/src/tree_builder/version.py
+-rw-r--r--   0        0        0     3038 2023-05-11 05:44:43.560822 devapps-2023.5.14/setup.py
+-rw-r--r--   0        0        0     1805 2023-05-11 05:44:43.561086 devapps-2023.5.14/PKG-INFO
```

### Comparing `devapps-2023.5.13/LICENSE` & `devapps-2023.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/README.md` & `devapps-2023.5.14/README.md`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/pyproject.toml` & `devapps-2023.5.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "devapps"
-version = "2023.05.13"
+version = "2023.05.14"
 description = "Apps - End to End."
 authors = ["Gunther Klessinger <g_kle_ss_ing_er@gmx.de>"]
 license = "BSD"
 readme = "README.md"
 repository = "https://github.com/AXGKl/devapps"
 homepage = "https://axgkl.github.io/devapps"
 keywords = []
```

### Comparing `devapps-2023.5.13/src/ax/utils/ax_tree/_ax_tree.so` & `devapps-2023.5.14/src/ax/utils/ax_tree/_ax_tree.so`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/ax/utils/ax_tree/ax_tree.py` & `devapps-2023.5.14/src/ax/utils/ax_tree/ax_tree.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/app.py` & `devapps-2023.5.14/src/devapp/app.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/app_token/create_tokens.py` & `devapps-2023.5.14/src/devapp/app_token/create_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/app_token/read_tokens.py` & `devapps-2023.5.14/src/devapp/app_token/read_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/components/cloudfoundry.py` & `devapps-2023.5.14/src/devapp/components/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/components/gitlab.py` & `devapps-2023.5.14/src/devapp/components/gitlab.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/components/gitlab_runner.py` & `devapps-2023.5.14/src/devapp/components/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/dev_mode.py` & `devapps-2023.5.14/src/devapp/dev_mode.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/gevent_patched.py` & `devapps-2023.5.14/src/devapp/gevent_patched.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/layer.py` & `devapps-2023.5.14/src/devapp/layer.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/lib/sh.py` & `devapps-2023.5.14/src/devapp/lib/sh.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/load.py` & `devapps-2023.5.14/src/devapp/load.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/logo` & `devapps-2023.5.14/src/devapp/logo`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/max.py` & `devapps-2023.5.14/src/devapp/max.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/operations/resources.py` & `devapps-2023.5.14/src/devapp/operations/resources.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py` & `devapps-2023.5.14/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/dev_devapp/repo_sym_links.py` & `devapps-2023.5.14/src/devapp/plugins/dev_devapp/repo_sym_links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resource_install.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resource_install.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resource_run.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resource_run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resources.py.dis` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resources.py.dis`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/resources_list.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/resources_list.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/arch/wait_for_port.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/arch/wait_for_port.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/container_build.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/container_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/container_pull.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/container_pull.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/fs_build.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/fs_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/kubectl/__init__.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/kubectl/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/life_cycle.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/life_cycle.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/log_view.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/log_view.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/project/__init__.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/project/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/plugins/ops_devapp/run.py` & `devapps-2023.5.14/src/devapp/plugins/ops_devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/run.py` & `devapps-2023.5.14/src/devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/build.py` & `devapps-2023.5.14/src/devapp/spec/build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/find_paths_in_fs_components.py` & `devapps-2023.5.14/src/devapp/spec/find_paths_in_fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/fs_components.py` & `devapps-2023.5.14/src/devapp/spec/fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/links.py` & `devapps-2023.5.14/src/devapp/spec/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/os_tools.py` & `devapps-2023.5.14/src/devapp/spec/os_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/templ.py` & `devapps-2023.5.14/src/devapp/spec/templ.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/templates/unit` & `devapps-2023.5.14/src/devapp/spec/templates/unit`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/spec/tools.py` & `devapps-2023.5.14/src/devapp/spec/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/t` & `devapps-2023.5.14/src/devapp/t`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/testing/auto_docs.py` & `devapps-2023.5.14/src/devapp/testing/auto_docs.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/third/rpl` & `devapps-2023.5.14/src/devapp/third/rpl`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/__init__.py` & `devapps-2023.5.14/src/devapp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/flag.py` & `devapps-2023.5.14/src/devapp/tools/flag.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/http.py` & `devapps-2023.5.14/src/devapp/tools/http.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/__init__.py` & `devapps-2023.5.14/src/devapp/tools/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/actions.py` & `devapps-2023.5.14/src/devapp/tools/infra/actions.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/000:functions.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/000:functions.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/300:dns.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/300:dns.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/500:k3s.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/500:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/501:kind.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/501:kind.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/502:k3s.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/502:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/600:longhorn.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/600:longhorn.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh` & `devapps-2023.5.14/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/old.py` & `devapps-2023.5.14/src/devapp/tools/old.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/plugin.py` & `devapps-2023.5.14/src/devapp/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/tools/resource.py` & `devapps-2023.5.14/src/devapp/tools/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     repl_dollar_var_with_env_val,
     dirname,
     write_file,
     read_file,
 )
 
 # mamba support hack
-os.environ['CONDA_PREFIX'] = os.environ.get(
-    'CONDA_PREFIX', os.environ.get('MAMBA_ROOT_PREFIX')
-)
+MRP = os.environ.get('MAMBA_ROOT_PREFIX')
+os.environ['CONDA_PREFIX'] = os.environ.get('CONDA_PREFIX', MRP or '')
+
 
 T_unit = """
 [Unit]
 Description      = %(descr)s %(name)s
 Wants            = network-online.target
 StopWhenUnneeded = false
 
@@ -87,15 +87,16 @@
     m[k] = v
 
 
 environ = os.environ
 
 
 def cur_prefix():
-    cli = os.environ.get('CONDA_PREFIX', '').split('/envs/', 1)[0]
+    m = MRP
+    cli = os.environ.get('CONDA_PREFIX', m).split('/envs/', 1)[0]
     if not cli:
         app.die('No $CONDA_PREFIX currently set')
     return cli
 
 
 def set_conda_prefix():
     """
@@ -138,27 +139,29 @@
         cli = S.conda_prefix + '/fs'
     elif cli in ('conda', 'c'):
         cli = cur_prefix() + '/fs'
     cli = os.path.abspath(cli)
     S.fs_dir = cli
 
 
-conda_prefix = lambda: S.conda_prefix or [set_conda_prefix(), S.conda_prefix][1]
+conda_prefix = (
+    lambda: S.conda_prefix or [set_conda_prefix(), S.conda_prefix][1]
+)
 
 
 class CommonFlags:
     autoshort = ''
 
     class install_state:
         n = 'show install state infos'
         d = False
 
     class conda_prefix:
         n = set_conda_prefix.__doc__
-        d = 'default'
+        d = MRP or 'default'
 
     class fs_dir:
         n = set_fs_dir.__doc__
         d = 'default'
 
     class log_resources_fully:
         n = 'Always output all settings of resources when logging'
@@ -235,15 +238,17 @@
 def dir_rsc_cfg(rsc):
     """configured directory of the resource"""
     if is_no_pkg_rsc(rsc):
         return project.root() + '/bin'
     elif is_fs(rsc):
         return S.fs_dir + '/' + rsc.name
     else:
-        return S.conda_prefix + '/envs/%s/bin' % (g(rsc, 'conda_env', rsc.name))
+        return S.conda_prefix + '/envs/%s/bin' % (
+            g(rsc, 'conda_env', rsc.name)
+        )
 
 
 def rsc_path(rsc, verify_present=False):
     """
     Find path of resource (e.g. /home/joe/miniconda3/envs/myrsc/bin)
     Return nothing if not present
 
@@ -358,15 +363,18 @@
         def filesystem(rsc):
             if not rsc_path(rsc, verify_present=True):
                 pass
             d = S.fs_dir + '/%s' % rsc.name
             img = rsc.pkg.split('layers:', 1)[1]
             system('ops container_pull --repo "%s" --dir "%s.img"' % (img, d))
             s = '--skip_filesystem_adaptions'
-            system('ops container_build --dirs "%s.img" --target_dir "%s" %s' % (d, d, s))
+            system(
+                'ops container_build --dirs "%s.img" --target_dir "%s" %s'
+                % (d, d, s)
+            )
 
     def write_unit_file(name, fn, rsc, instance):
         pn = project.root().rsplit('/', 1)[-1]
         inst_name = f'{name}-{instance}' if instance else name
         m = {
             'name': inst_name,
             'descr': '%s %s ' % (g(rsc, 'n', inst_name), pn),
@@ -456,15 +464,17 @@
                 add(deindent(s))
 
             # env['PATH'] = '%s:$PATH' % g(rsc, 'path')
             add('')
             add("H='__HOME__'")
             add('export PROJECT_ROOT="%s"' % project.root())
             add('# set e.g. in unit files:')
-            add('test -n "$INSTANCE" && inst_postfix="-$INSTANCE" || inst_postfix=""')
+            add(
+                'test -n "$INSTANCE" && inst_postfix="-$INSTANCE" || inst_postfix=""'
+            )
             add('')
             add('# Resource settings:')
             # for whoever needs that:
             allk = set()
             for m in to_dict(rsc), spec, spec_env:
                 for k, v in sorted(m.items()):
                     if k == 'cmd_pre':
@@ -546,22 +556,21 @@
             if str(rsc.path).startswith(D):
                 return app.debug('already installed - skipping', rsc=rsc)
 
             env = g(rsc, 'conda_env', rsc.name)
             ctx = dict(D=D, name=env, yes=interactive())
             mamba = os.environ.get('MAMBA_EXE')
             # if os.system('type micromamba') == 0 or 1:
-            if mamba and os.environ.get('MAMBA_ROOT_PREFIX'):
+            if mamba and MRP:
                 ctx['conda'] = mamba
                 # FIXME: The activate during docker build is a problem in micromamba which runs as subprocess
                 # Better create the env via micromamba create -n foo -f <yaml file> first
-                f = os.environ.get('MAMBA_ROOT_PREFIX')
                 cmd = [
                     '%(conda)s create %(yes)s -n "%(name)s"',
-                    f'. "{f}/etc/profile.d/micromamba.sh"',
+                    f'. "{MRP}/etc/profile.d/micromamba.sh"',
                     'micromamba activate "%(name)s"',
                 ]
 
             elif mamba:
                 ctx['conda'] = mamba
                 # FIXME: The activate during docker build is a problem in micromamba which runs as subprocess
                 # Better create the env via micromamba create -n foo -f <yaml file> first
@@ -586,21 +595,27 @@
                     % pth
                 ]
             else:
                 icmd = g(rsc, 'conda_inst', '')
                 if icmd:
                     cmd += [icmd]
                 else:
-                    p = g(rsc, 'conda_pkg') or g(rsc, 'pkg') or ' '.join(rsc.provides)
+                    p = (
+                        g(rsc, 'conda_pkg')
+                        or g(rsc, 'pkg')
+                        or ' '.join(rsc.provides)
+                    )
                     chan = g(rsc, 'conda_chan', '')
                     if chan:
                         chan = '-c ' + chan
                     ctx['chan'] = chan
                     ctx['pkg'] = p
-                    cmd += ['%(conda)s install %(yes)s -c conda-forge %(chan)s %(pkg)s']
+                    cmd += [
+                        '%(conda)s install %(yes)s -c conda-forge %(chan)s %(pkg)s'
+                    ]
             cmd = ' && '.join(cmd) % ctx
             rsc.path = g(rsc, 'path') or pth
 
             # app.info('cmd', cmd=cmd)
             # import subprocess
             # s = subprocess.run(cmd, shell=True, executable='/bin/bash')
             # will run under dash, sh, bash -> problem e.g. for conda activate
@@ -739,15 +754,19 @@
     rsc.module = rsc.__module__.replace('.operations.resources', '')
     rsc.__repr__ = lambda r: str(to_dict(r))
     rsc.__str__ = lambda r: to_str(r)
     rsc.module_dir = S.rsc_dirs[fn]
     rsc.host_conf_dir = '$PROJECT_ROOT/conf/${host:-$HOSTNAME}/' + rsc.name
     rsc.disabled = g(rsc, 'disabled', g(rsc, 'd', False))
     rsc.installed = g(rsc, 'installed', False)
-    [repl_callable(rsc, k, getattr(rsc, k)) for k in dir(rsc) if not k.startswith('_')]
+    [
+        repl_callable(rsc, k, getattr(rsc, k))
+        for k in dir(rsc)
+        if not k.startswith('_')
+    ]
 
 
 def to_str(rsc):
     svc = g(rsc, 'systemd')
     i = 'i' if g(rsc, 'installed') else ' '
     d = 'd' if rsc.disabled else ' '
     s = 's' if svc else ' '
@@ -837,7 +856,8 @@
     rscs = sorted([r for r in rscs], key=lambda x: x.name)
     # now we make singletons for __repr__ w/o metaclass hacks
     rscs = [r() for r in rscs]
     for k in rscs:
         app.debug(k.name, **to_dict(k))
     S.rscs_defined = rscs
     return rscs
+
```

### Comparing `devapps-2023.5.13/src/devapp/tools/times.py` & `devapps-2023.5.14/src/devapp/tools/times.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/utils/os_.py` & `devapps-2023.5.14/src/devapp/utils/os_.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/utils/py_source_env.py` & `devapps-2023.5.14/src/devapp/utils/py_source_env.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/utils/rx_tools.py` & `devapps-2023.5.14/src/devapp/utils/rx_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/utils/vault.py` & `devapps-2023.5.14/src/devapp/utils/vault.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/devapp/utils/watch_dog.py` & `devapps-2023.5.14/src/devapp/utils/watch_dog.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/mdvl/mdvl.py` & `devapps-2023.5.14/src/mdvl/mdvl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/mdvl/tools.py` & `devapps-2023.5.14/src/mdvl/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/__init__.py` & `devapps-2023.5.14/src/structlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/adapters.py` & `devapps-2023.5.14/src/structlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/config.py` & `devapps-2023.5.14/src/structlogging/config.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/formatters.py` & `devapps-2023.5.14/src/structlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/processors.py` & `devapps-2023.5.14/src/structlogging/processors.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/renderers.py` & `devapps-2023.5.14/src/structlogging/renderers.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/sl.py` & `devapps-2023.5.14/src/structlogging/sl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/stacktrace.py` & `devapps-2023.5.14/src/structlogging/stacktrace.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/structlogging/tests/test_structlogging.py` & `devapps-2023.5.14/src/structlogging/tests/test_structlogging.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/__init__.py` & `devapps-2023.5.14/src/theming/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/absl_color_help.py` & `devapps-2023.5.14/src/theming/absl_color_help.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/ansi2html.py` & `devapps-2023.5.14/src/theming/ansi2html.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/ansi2html.sh` & `devapps-2023.5.14/src/theming/ansi2html.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/ansistrm.py` & `devapps-2023.5.14/src/theming/ansistrm.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/ax_xml.py` & `devapps-2023.5.14/src/theming/ax_xml.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/camel_snake.py` & `devapps-2023.5.14/src/theming/camel_snake.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/charting.py` & `devapps-2023.5.14/src/theming/charting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/colorhilite.py` & `devapps-2023.5.14/src/theming/colorhilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/filesize/README.txt` & `devapps-2023.5.14/src/theming/filesize/README.txt`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/filesize/filesize.py` & `devapps-2023.5.14/src/theming/filesize/filesize.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/formatters.py` & `devapps-2023.5.14/src/theming/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/formatting/markdown.py` & `devapps-2023.5.14/src/theming/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/formatting/viz_sequence.py` & `devapps-2023.5.14/src/theming/formatting/viz_sequence.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/html_tools.py` & `devapps-2023.5.14/src/theming/html_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/inflect.py` & `devapps-2023.5.14/src/theming/inflect.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/pretty_print.py` & `devapps-2023.5.14/src/theming/pretty_print.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/tablepretty.py` & `devapps-2023.5.14/src/theming/tablepretty.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/term.py` & `devapps-2023.5.14/src/theming/term.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/term_struct_hilite.py` & `devapps-2023.5.14/src/theming/term_struct_hilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/tests/test_text_formatting.py` & `devapps-2023.5.14/src/theming/tests/test_text_formatting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/tracebacks.py` & `devapps-2023.5.14/src/theming/tracebacks.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/theming/unicode_chars.py` & `devapps-2023.5.14/src/theming/unicode_chars.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/__init__.py` & `devapps-2023.5.14/src/tree_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/arch/__init__.py.bak` & `devapps-2023.5.14/src/tree_builder/arch/__init__.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/arch/links.py.bak` & `devapps-2023.5.14/src/tree_builder/arch/links.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/arch/o.py` & `devapps-2023.5.14/src/tree_builder/arch/o.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/arch/old` & `devapps-2023.5.14/src/tree_builder/arch/old`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/arch/olinit` & `devapps-2023.5.14/src/tree_builder/arch/olinit`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/arch/oo` & `devapps-2023.5.14/src/tree_builder/arch/oo`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/arch/render.py.bak` & `devapps-2023.5.14/src/tree_builder/arch/render.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/chrome_reload.sh` & `devapps-2023.5.14/src/tree_builder/chrome_reload.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/delivery2.py` & `devapps-2023.5.14/src/tree_builder/delivery2.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/links.py` & `devapps-2023.5.14/src/tree_builder/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/src/tree_builder/render.py` & `devapps-2023.5.14/src/tree_builder/render.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.13/setup.py` & `devapps-2023.5.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                      'dev = devapp.tools.plugin:main',
                      'fui = interactive.cli:main',
                      'myapp = devapp.tools.plugin:main',
                      'ops = devapp.tools.plugin:main']}
 
 setup_kwargs = {
     'name': 'devapps',
-    'version': '2023.5.13',
+    'version': '2023.5.14',
     'description': 'Apps - End to End.',
     'long_description': '# devapps\n\n\n<!-- badges -->\n[![docs pages][docs pages_img]][docs pages] [![gh-ci][gh-ci_img]][gh-ci] [![pkg][pkg_img]][pkg] [![code_style][code_style_img]][code_style] \n\n[docs pages]: https://axgkl.github.io/devapps/\n[docs pages_img]: https://axgkl.github.io/devapps/img/badge_docs.svg\n[gh-ci]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml\n[gh-ci_img]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml/badge.svg\n[pkg]: https://pypi.com/\n[pkg_img]: https://axgkl.github.io/devapps/img/badge_pypi.svg\n[code_style]: https://pypi.org/project/axblack/\n[code_style_img]: https://axgkl.github.io/devapps/img/badge_axblack.svg\n<!-- badges -->\n\n\nEnabler repo for dev *and* ops friendly apps, in a normalized way.\n\nIncludes:\n\n- logging (structlog)\n- cli flags handling (abseil, with addons)\n- docutools (mkdocs-material)\n- project setup\n- (test) resources management, including daemons and container filesystem layers\n\nand more.\n\n\n\n\nDocumentation: https://axgkl.github.io/devapps/',
     'author': 'Gunther Klessinger',
     'author_email': 'g_kle_ss_ing_er@gmx.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://axgkl.github.io/devapps',
```

### Comparing `devapps-2023.5.13/PKG-INFO` & `devapps-2023.5.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devapps
-Version: 2023.5.13
+Version: 2023.5.14
 Summary: Apps - End to End.
 Home-page: https://axgkl.github.io/devapps
 License: BSD
 Author: Gunther Klessinger
 Author-email: g_kle_ss_ing_er@gmx.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

