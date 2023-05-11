# Comparing `tmp/linux-tools-0.2.4.tar.gz` & `tmp/linux-tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linux-tools-0.2.4.tar", last modified: Sun Apr  2 16:57:54 2023, max compression
+gzip compressed data, was "linux-tools-0.2.5.tar", last modified: Thu May 11 15:23:37 2023, max compression
```

## Comparing `linux-tools-0.2.4.tar` & `linux-tools-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-04-02 16:57:54.758190 linux-tools-0.2.4/
--rw-r--r--   0 build     (1000) build     (1000)     1558 2023-04-02 16:57:26.000000 linux-tools-0.2.4/LICENSE
--rw-r--r--   0 build     (1000) build     (1000)    20173 2023-04-02 16:57:54.758190 linux-tools-0.2.4/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)    19849 2023-04-02 16:57:26.000000 linux-tools-0.2.4/README.md
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-04-02 16:57:54.758190 linux-tools-0.2.4/linux_tools/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-04-02 16:57:26.000000 linux-tools-0.2.4/linux_tools/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     3214 2023-04-02 16:57:26.000000 linux-tools-0.2.4/linux_tools/bits.py
--rw-r--r--   0 build     (1000) build     (1000)     8793 2023-04-02 16:57:26.000000 linux-tools-0.2.4/linux_tools/irqstat.py
--rw-r--r--   0 build     (1000) build     (1000)    10625 2023-04-02 16:57:26.000000 linux-tools-0.2.4/linux_tools/netgraph.py
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-04-02 16:57:54.758190 linux-tools-0.2.4/linux_tools.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)    20173 2023-04-02 16:57:54.000000 linux-tools-0.2.4/linux_tools.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)      320 2023-04-02 16:57:54.000000 linux-tools-0.2.4/linux_tools.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-04-02 16:57:54.000000 linux-tools-0.2.4/linux_tools.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)      119 2023-04-02 16:57:54.000000 linux-tools-0.2.4/linux_tools.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)       12 2023-04-02 16:57:54.000000 linux-tools-0.2.4/linux_tools.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)      235 2023-04-02 16:57:26.000000 linux-tools-0.2.4/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1000)      352 2023-04-02 16:57:54.758190 linux-tools-0.2.4/setup.cfg
--rw-r--r--   0 build     (1000) build     (1000)      779 2023-04-02 16:57:26.000000 linux-tools-0.2.4/setup.py
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-05-11 15:23:37.069933 linux-tools-0.2.5/
+-rw-r--r--   0 build     (1000) build     (1000)     1558 2023-05-11 15:22:48.000000 linux-tools-0.2.5/LICENSE
+-rw-r--r--   0 build     (1000) build     (1000)    20173 2023-05-11 15:23:37.069933 linux-tools-0.2.5/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)    19849 2023-05-11 15:22:48.000000 linux-tools-0.2.5/README.md
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-05-11 15:23:37.069933 linux-tools-0.2.5/linux_tools/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     3214 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/bits.py
+-rw-r--r--   0 build     (1000) build     (1000)     8312 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/irqstat.py
+-rw-r--r--   0 build     (1000) build     (1000)    11038 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/netgraph.py
+-rw-r--r--   0 build     (1000) build     (1000)     1697 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/table.py
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-05-11 15:23:37.069933 linux-tools-0.2.5/linux_tools.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)    20173 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)      341 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)      119 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)       12 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)      235 2023-05-11 15:22:48.000000 linux-tools-0.2.5/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1000)      352 2023-05-11 15:23:37.069933 linux-tools-0.2.5/setup.cfg
+-rw-r--r--   0 build     (1000) build     (1000)      779 2023-05-11 15:22:48.000000 linux-tools-0.2.5/setup.py
```

### Comparing `linux-tools-0.2.4/LICENSE` & `linux-tools-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.4/PKG-INFO` & `linux-tools-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linux-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: Various command line utilities for Linux written in python
 Home-page: https://git.sr.ht/~rjarry/linux-tools
 Author: Robin Jarry
 Author-email: ~rjarry/public-inbox@lists.sr.ht
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linux-tools-0.2.4/README.md` & `linux-tools-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.4/linux_tools/bits.py` & `linux-tools-0.2.5/linux_tools/bits.py`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.4/linux_tools/irqstat.py` & `linux-tools-0.2.5/linux_tools/irqstat.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 import argparse
 import os
 import re
 import sys
 
-from . import bits
+from . import bits, table
 
 
 # ------------------------------------------------------------------------------
 def main() -> int:
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
         "-r",
@@ -147,88 +147,74 @@
         per_irq = True
         cpu_ids = sorted(cpu_ids)
     else:
         per_irq = False
         cpu_ids = sorted(cpus.keys())
     irq_ids.sort(key=lambda i: f"{int(i):04d}" if i.isdigit() else i)
 
+    t = table.Table()
+
     if args.stats:
         if per_cpu:
-            header = ["CPU"] + [f"IRQ-{i}" if i.isdigit() else i for i in irq_ids]
-            align = [1] * len(header)
-            align[0] = -1
-            rows = [tuple(header)]
+            t.add_column("CPU")
+            for i in irq_ids:
+                t.add_column(
+                    f"IRQ-{i}" if i.isdigit() else i, table.ALIGN_RIGHT, num_format
+                )
             for cpu in sorted(cpus.keys()):
                 if cpu_ids and cpu not in cpu_ids:
                     continue
                 nums = [irqs[i]["counters"][cpu] for i in irq_ids]
                 if not any(nums) and not args.display_zeroes:
                     continue
-                nums = [num_format(n) for n in nums]
-                rows.append(tuple([str(cpu)] + nums))
+                t.add_row([cpu] + nums)
 
         elif per_irq:
-            header = ["IRQ"] + [f"CPU-{c}" for c in cpu_ids] + ["DESCRIPTION"]
-            align = [1] * len(header)
-            align[0] = -1
-            align[-1] = -1
-            rows = [tuple(header)]
+            t.add_column("IRQ")
+            for c in cpu_ids:
+                t.add_column(f"CPU-{c}", table.ALIGN_RIGHT, num_format)
+            t.add_column("DESCRIPTION")
             for irq in irq_ids:
                 i = irqs[irq]
                 nums = [i["counters"][c] for c in cpu_ids]
                 if not any(nums) and not args.display_zeroes:
                     continue
-                nums = [num_format(n) for n in nums]
-                rows.append(tuple([irq] + nums + [i["desc"]]))
+                t.add_row([irq] + nums + [i["desc"]])
 
         else:
-            rows = [("IRQ", "TOTAL", "DESCRIPTION")]
-            align = [-1, 1, -1]
+            t.add_column("IRQ")
+            t.add_column("TOTAL", table.ALIGN_RIGHT, num_format)
+            t.add_column("DESCRIPTION")
             for irq in irq_ids:
                 i = irqs[irq]
-                total = sum(i["counters"][c] for c in sorted(cpus.keys()))
+                total = sum(i["counters"][c] for c in cpu_ids)
                 if total == 0 and not args.display_zeroes:
                     continue
-                rows.append((irq, num_format(total), i["desc"]))
+                t.add_row([irq, total, i["desc"]])
 
     elif args.num_per_cpu:
-        rows = [("CPU", "AFFINITY-IRQs", "EFFECTIVE-IRQs")]
-        align = [-1, 1, 1]
+        t.add_column("CPU")
+        t.add_column("AFFINITY-IRQs", table.ALIGN_RIGHT)
+        t.add_column("EFFECTIVE-IRQs", table.ALIGN_RIGHT)
         for cpu in cpu_ids:
             c = cpus[cpu]
-            rows.append((str(cpu), str(c["affinity"]), str(c["effective"])))
+            t.add_row([cpu, c["affinity"], c["effective"]])
 
     else:
-        rows = [("IRQ", "AFFINITY", "EFFECTIVE-CPU", "DESCRIPTION")]
-        align = [-1, 1, 1, -1]
+        t.add_column("IRQ")
+        t.add_column("AFFINITY", table.ALIGN_RIGHT, bits.bit_list)
+        t.add_column("EFFECTIVE-CPU", table.ALIGN_RIGHT, bits.bit_list)
+        t.add_column("DESCRIPTION")
         for irq in irq_ids:
             i = irqs[irq]
             if cpu_ids and not i["effective"].intersection(cpu_ids):
                 continue
-            rows.append(
-                (
-                    irq,
-                    bits.bit_list(i["affinity"]),
-                    bits.bit_list(i["effective"]),
-                    i["desc"],
-                )
-            )
+            t.add_row([irq, i["affinity"], i["effective"], i["desc"]])
 
-    widths = [len(c) for c in rows[0]]
-    for row in rows:
-        for c, _ in enumerate(widths):
-            if len(row[c]) > widths[c]:
-                widths[c] = len(row[c])
-    for w, _ in enumerate(widths):
-        widths[w] = align[w] * widths[w]
-    if widths[-1] < 0:
-        widths[-1] = ""
-    fmt = "  ".join(f"%{w}s" for w in widths)
-    for row in rows:
-        print(fmt % row)
+    t.print(sys.stdout)
 
     return 0
 
 
 # ------------------------------------------------------------------------------
 INTERRUPT_RE = re.compile(r"^\s*(\w+):\s+([\s\d]+)\s+([A-Za-z].+)$")
 SOFTIRQS_RE = re.compile(r"^\s*(\w+):\s+([\s\d]+)\s*$")
```

### Comparing `linux-tools-0.2.4/linux_tools/netgraph.py` & `linux-tools-0.2.5/linux_tools/netgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,17 +145,24 @@
     attrs = {}
     color = COLORS.get(link["kind"], "gray")
     attrs["tooltip"] = '"' + "\\n".join(link["tip"]) + '"'
     attrs["color"] = color
     attrs["shape"] = SHAPES.get(link["kind"], "oval")
     if attrs["shape"] == "rectangle":
         attrs.setdefault("margin", "0.05")
-    labels = (
+    labels = [
+        f"<b>{link['name']}</b>",
+    ]
+    if "alias" in link:
+        alias = link["alias"]
+        if len(alias) > 16:
+            alias = alias[:15] + "…"
+        labels.append(f'<font color="slategray"><i>&quot;{alias}&quot;</i></font>')
+    labels += (
         [
-            f"<b>{link['name']}</b>",
             f'<font color="{color}">{link["kind"]}</font>',
         ]
         + [
             f'<font color="{color}">{key} {value}</font>'
             for key, value in link["attributes"].items()
         ]
         + [f'<font color="orange">{mac}</font>' for mac in link["l2"]]
@@ -282,15 +289,18 @@
                             # ignore access private vlans
                             continue
                         if "vlanEnd" in v:
                             vlans.update(range(v["vlan"], v["vlanEnd"] + 1))
                         else:
                             vlans.add(v["vlan"])
 
-            tip = [f"{k} {v}" for k, v in data.items()]
+            tip = []
+            if "ifalias" in addr:
+                tip.append(f"alias {addr['ifalias']}")
+            tip += [f"{k} {v}" for k, v in data.items()]
             l2 = []
             if "address" in addr:
                 if args.l2_addresses:
                     l2.append(addr["address"])
                 else:
                     tip.append(f"lladdr {addr['address']}")
 
@@ -321,14 +331,16 @@
                 "ipv6": ipv6,
                 "tip": tip,
             }
             if "master" in addr:
                 a["master"] = safe(f"{ns}_{addr['master']}")
             if link_dev is not None:
                 a["link"] = safe(f"{link_ns}_{link_dev}")
+            if "ifalias" in addr:
+                a["alias"] = addr["ifalias"]
 
             out.setdefault(ns, []).append(a)
 
     return out
 
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linux-tools-0.2.4/linux_tools.egg-info/PKG-INFO` & `linux-tools-0.2.5/linux_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linux-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: Various command line utilities for Linux written in python
 Home-page: https://git.sr.ht/~rjarry/linux-tools
 Author: Robin Jarry
 Author-email: ~rjarry/public-inbox@lists.sr.ht
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linux-tools-0.2.4/setup.py` & `linux-tools-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 setuptools.setup(
     name="linux-tools",
     description="Various command line utilities for Linux written in python",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text("utf-8"),
     long_description_content_type="text/markdown",
     license="BSD-3-Clause",
-    version="0.2.4",
+    version="0.2.5",
     author="Robin Jarry",
     author_email="~rjarry/public-inbox@lists.sr.ht",
     url="https://git.sr.ht/~rjarry/linux-tools",
     packages=setuptools.find_packages("."),
     entry_points="""
     [console_scripts]
     bits = linux_tools.bits:main
```

