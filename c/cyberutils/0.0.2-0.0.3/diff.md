# Comparing `tmp/cyberutils-0.0.2.tar.gz` & `tmp/cyberutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberutils-0.0.2.tar", max compression
+gzip compressed data, was "cyberutils-0.0.3.tar", max compression
```

## Comparing `cyberutils-0.0.2.tar` & `cyberutils-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1075 2023-05-08 05:28:37.655197 cyberutils-0.0.2/LICENSE
--rw-r--r--   0        0        0     2523 2023-05-08 05:28:37.655197 cyberutils-0.0.2/README.md
--rw-r--r--   0        0        0      166 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/__init__.py
--rw-r--r--   0        0        0       77 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/bash/__init__.py
--rw-r--r--   0        0        0     2268 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/bash/execution.py
--rw-r--r--   0        0        0       40 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/contract/__init__.py
--rw-r--r--   0        0        0     1671 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/contract/execution.py
--rw-r--r--   0        0        0       39 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/graphql/__init__.py
--rw-r--r--   0        0        0      757 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/graphql/execution.py
--rw-r--r--   0        0        0     1818 2023-05-08 05:28:37.655197 cyberutils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 cyberutils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-11 06:23:14.946521 cyberutils-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3603 2023-05-11 06:23:14.946521 cyberutils-0.0.3/README.md
+-rw-r--r--   0        0        0      166 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/__init__.py
+-rw-r--r--   0        0        0       77 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/bash/__init__.py
+-rw-r--r--   0        0        0     2268 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/bash/execution.py
+-rw-r--r--   0        0        0       40 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/contract/__init__.py
+-rw-r--r--   0        0        0     1671 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/contract/execution.py
+-rw-r--r--   0        0        0       93 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/graphql/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-11 06:23:14.950521 cyberutils-0.0.3/cyberutils/graphql/execution.py
+-rw-r--r--   0        0        0     1895 2023-05-11 06:23:14.950521 cyberutils-0.0.3/cyberutils/graphql/queries.py
+-rw-r--r--   0        0        0     1818 2023-05-11 06:23:14.950521 cyberutils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 cyberutils-0.0.3/PKG-INFO
```

### Comparing `cyberutils-0.0.2/LICENSE` & `cyberutils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.2/README.md` & `cyberutils-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -92,8 +92,50 @@
             tx
           }
         }
         """,
     graphql_url='https://index.bostrom.cybernode.ai/v1/graphql')
 
 pd.DataFrame(res['contracts'])
+```
+a query with variable values
+```python
+import pandas as pd
+
+from cyberutils.graphql import execute_graphql
+
+res = await execute_graphql(
+    request="""
+        query ContractsCodeID($code_id: bigint) {
+            contracts(order_by: {tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) {
+                address
+                admin
+                creation_time
+                creator
+                fees
+                gas
+                height
+                label
+                tx
+                code_id
+            }
+        }
+        """,
+    variable_values={"code_id": "3"},
+    graphql_url='https://index.bostrom.cybernode.ai/v1/graphql')
+
+pd.DataFrame(res['contracts'])
+```
+get messages with a given address and type
+```python
+import pandas as pd
+
+from cyberutils.graphql import get_messages_by_address_and_type
+
+
+res = await get_messages_by_address_and_type(
+    address='bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw',
+    msg_type='cosmos.bank.v1beta1.MsgSend',
+    graphql_url='https://index.bostrom.cybernode.ai/v1/graphql')
+
+pd.DataFrame(res)
 ```
```

#### html2text {}

```diff
@@ -22,8 +22,20 @@
 wallet=wallet, contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client,
 gas=500_000, fee_amount=0, fee_denom='boot', memo='the first transfer') ``` ###
 execute a graphql query ```python import pandas as pd from cyberutils.graphql
 import execute_graphql res = await execute_graphql( request=""" query
 AllContracts { contracts(order_by: {tx: desc_nulls_last}) { address admin
 code_id creation_time creator fees gas height label tx } } """,
 graphql_url='https://index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res
-['contracts']) ```
+['contracts']) ``` a query with variable values ```python import pandas as pd
+from cyberutils.graphql import execute_graphql res = await execute_graphql
+( request=""" query ContractsCodeID($code_id: bigint) { contracts(order_by:
+{tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) { address admin
+creation_time creator fees gas height label tx code_id } } """,
+variable_values={"code_id": "3"}, graphql_url='https://
+index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` get
+messages with a given address and type ```python import pandas as pd from
+cyberutils.graphql import get_messages_by_address_and_type res = await
+get_messages_by_address_and_type
+( address='bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw',
+msg_type='cosmos.bank.v1beta1.MsgSend', graphql_url='https://
+index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res) ```
```

### Comparing `cyberutils-0.0.2/cyberutils/bash/execution.py` & `cyberutils-0.0.3/cyberutils/bash/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.2/cyberutils/contract/execution.py` & `cyberutils-0.0.3/cyberutils/contract/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.2/pyproject.toml` & `cyberutils-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 documentation = "https://github.com/Snedashkovsky/cyberutils"
 homepage = "https://github.com/Snedashkovsky/cyberutils"
 keywords = ["bostrom", "cyber", "knowledge-graph", "dex", "swap", "defi", "crypto", "blockchain", ]
 license = "MIT"
 packages = [{ include = "cyberutils" }]
 readme = "README.md"
 repository = "https://github.com/Snedashkovsky/cyberutils.git"
-version = "0.0.2"
+version = "0.0.3"
 
 [tool.poetry.dependencies]
 pandas = "^1.0.0"
 numpy = "^1.0.0"
 python-dotenv = "^0.20.0"
 tqdm = "^4.0.0"
 ipython = "^8.0.0"
```

### Comparing `cyberutils-0.0.2/PKG-INFO` & `cyberutils-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberutils
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Toolset for cyber protocol and cosmos ecosystem
 Home-page: https://github.com/Snedashkovsky/cyberutils
 License: MIT
 Keywords: bostrom,cyber,knowledge-graph,dex,swap,defi,crypto,blockchain
 Author: Snedashkovsky,
 Author-email: sn@cyberdrop.ai
 Requires-Python: >=3.9,<4.0
@@ -127,7 +127,49 @@
           }
         }
         """,
     graphql_url='https://index.bostrom.cybernode.ai/v1/graphql')
 
 pd.DataFrame(res['contracts'])
 ```
+a query with variable values
+```python
+import pandas as pd
+
+from cyberutils.graphql import execute_graphql
+
+res = await execute_graphql(
+    request="""
+        query ContractsCodeID($code_id: bigint) {
+            contracts(order_by: {tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) {
+                address
+                admin
+                creation_time
+                creator
+                fees
+                gas
+                height
+                label
+                tx
+                code_id
+            }
+        }
+        """,
+    variable_values={"code_id": "3"},
+    graphql_url='https://index.bostrom.cybernode.ai/v1/graphql')
+
+pd.DataFrame(res['contracts'])
+```
+get messages with a given address and type
+```python
+import pandas as pd
+
+from cyberutils.graphql import get_messages_by_address_and_type
+
+
+res = await get_messages_by_address_and_type(
+    address='bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw',
+    msg_type='cosmos.bank.v1beta1.MsgSend',
+    graphql_url='https://index.bostrom.cybernode.ai/v1/graphql')
+
+pd.DataFrame(res)
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberutils Version: 0.0.2 Summary: The Toolset for
+Metadata-Version: 2.1 Name: cyberutils Version: 0.0.3 Summary: The Toolset for
 cyber protocol and cosmos ecosystem Home-page: https://github.com/
 Snedashkovsky/cyberutils License: MIT Keywords: bostrom,cyber,knowledge-
 graph,dex,swap,defi,crypto,blockchain Author: Snedashkovsky, Author-email:
 sn@cyberdrop.ai Requires-Python: >=3.9,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -41,8 +41,20 @@
 wallet=wallet, contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client,
 gas=500_000, fee_amount=0, fee_denom='boot', memo='the first transfer') ``` ###
 execute a graphql query ```python import pandas as pd from cyberutils.graphql
 import execute_graphql res = await execute_graphql( request=""" query
 AllContracts { contracts(order_by: {tx: desc_nulls_last}) { address admin
 code_id creation_time creator fees gas height label tx } } """,
 graphql_url='https://index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res
-['contracts']) ```
+['contracts']) ``` a query with variable values ```python import pandas as pd
+from cyberutils.graphql import execute_graphql res = await execute_graphql
+( request=""" query ContractsCodeID($code_id: bigint) { contracts(order_by:
+{tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) { address admin
+creation_time creator fees gas height label tx code_id } } """,
+variable_values={"code_id": "3"}, graphql_url='https://
+index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` get
+messages with a given address and type ```python import pandas as pd from
+cyberutils.graphql import get_messages_by_address_and_type res = await
+get_messages_by_address_and_type
+( address='bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw',
+msg_type='cosmos.bank.v1beta1.MsgSend', graphql_url='https://
+index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res) ```
```

