# Comparing `tmp/anyhedge-0.3.6.tar.gz` & `tmp/anyhedge-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyhedge-0.3.6.tar", last modified: Wed Apr 12 18:14:41 2023, max compression
+gzip compressed data, was "anyhedge-0.3.7.tar", last modified: Thu Apr 13 08:41:38 2023, max compression
```

## Comparing `anyhedge-0.3.6.tar` & `anyhedge-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/
--rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.3.6/LICENSE
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 18:14:41.786326 anyhedge-0.3.6/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.3.6/README.md
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/anyhedge/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.3.6/anyhedge/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2358 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    28401 2023-04-12 18:08:28.000000 anyhedge-0.3.6/anyhedge/contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.3.6/anyhedge/javascript.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.3.6/anyhedge/oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/role.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/anyhedge/tests/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/test_bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    33305 2023-04-12 18:09:52.000000 anyhedge-0.3.6/anyhedge/tests/test_contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/test_fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/test_oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.3.6/anyhedge/validators.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/anyhedge.egg-info/
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)      512 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/requires.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-12 18:14:17.000000 anyhedge-0.3.6/pyproject.toml
--rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-12 18:14:41.786326 anyhedge-0.3.6/setup.cfg
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-13 08:41:38.682560 anyhedge-0.3.7/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.3.7/LICENSE
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-13 08:41:38.682560 anyhedge-0.3.7/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.3.7/README.md
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-13 08:41:38.678560 anyhedge-0.3.7/anyhedge/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.3.7/anyhedge/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2358 2023-04-11 04:30:35.000000 anyhedge-0.3.7/anyhedge/bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    28784 2023-04-13 08:39:58.000000 anyhedge-0.3.7/anyhedge/contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.3.7/anyhedge/fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.3.7/anyhedge/javascript.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.3.7/anyhedge/oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.3.7/anyhedge/role.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-13 08:41:38.682560 anyhedge-0.3.7/anyhedge/tests/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.3.7/anyhedge/tests/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.3.7/anyhedge/tests/test_bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    34330 2023-04-13 08:38:14.000000 anyhedge-0.3.7/anyhedge/tests/test_contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.3.7/anyhedge/tests/test_fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.3.7/anyhedge/tests/test_oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.3.7/anyhedge/validators.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-13 08:41:38.678560 anyhedge-0.3.7/anyhedge.egg-info/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-13 08:41:38.000000 anyhedge-0.3.7/anyhedge.egg-info/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)      512 2023-04-13 08:41:38.000000 anyhedge-0.3.7/anyhedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-13 08:41:38.000000 anyhedge-0.3.7/anyhedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-13 08:41:38.000000 anyhedge-0.3.7/anyhedge.egg-info/requires.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-13 08:41:38.000000 anyhedge-0.3.7/anyhedge.egg-info/top_level.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-13 08:31:44.000000 anyhedge-0.3.7/pyproject.toml
+-rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-13 08:41:38.682560 anyhedge-0.3.7/setup.cfg
```

### Comparing `anyhedge-0.3.6/LICENSE` & `anyhedge-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/PKG-INFO` & `anyhedge-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.3.6
+Version: 0.3.7
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.3.6/README.md` & `anyhedge-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/anyhedge/bch_primitives.py` & `anyhedge-0.3.7/anyhedge/bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/anyhedge/contract.py` & `anyhedge-0.3.7/anyhedge/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,20 @@
     def other_side(self) -> Side:
         # use a lookup to ensure KeyError with unknown value
         return {Side.SHORT: Side.LONG, Side.LONG: Side.SHORT}[self]
 
     @classmethod
     def from_string(cls, side_string: str) -> Side:
         # use a lookup to ensure KeyError with unknown value
-        return {'short': cls.SHORT, 'long': cls.LONG}[side_string.lower()]
+        lookup = {
+            'short': cls.SHORT,
+            'hedge': cls.SHORT,
+            'long': cls.LONG,
+        }
+        return lookup[side_string.lower()]
 
 
 class NominalOracleUnitsXSatsPerBch(int):
     def __init__(self, value):
         super().__init__()
         validators.instance(value, int)  # i.e. don't allow silent coercion
         validators.less_equal(self, SCRIPT_INT_MAX_WHEN_JAVASCRIPT)
@@ -214,14 +219,26 @@
         #   long leverage = 1 / (1 - (long liq price / start price))
         return LongLeverage(1 / (1 - self.long_liquidation_price_oracleUnits_per_bch / self.start_price_oracleUnits_per_bch))
 
     @property
     def taker_side(self) -> Side:
         return self.maker_side.other_side
 
+    @property
+    def short_role(self) -> Role:
+        if self.maker_side == Side.SHORT:
+            return Role.MAKER
+        return Role.TAKER
+
+    @property
+    def long_role(self) -> Role:
+        if self.maker_side == Side.LONG:
+            return Role.MAKER
+        return Role.TAKER
+
     ###############
     # Property access to input sats
     ###############
     @property
     def short_input_sats(self) -> UtxoSats:
         return self.input_sats(side=Side.SHORT)
```

### Comparing `anyhedge-0.3.6/anyhedge/fee.py` & `anyhedge-0.3.7/anyhedge/fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/anyhedge/oracle.py` & `anyhedge-0.3.7/anyhedge/oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/anyhedge/tests/test_bch_primitives.py` & `anyhedge-0.3.7/anyhedge/tests/test_bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/anyhedge/tests/test_contract.py` & `anyhedge-0.3.7/anyhedge/tests/test_contract.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,16 +147,31 @@
 
     def test_long_liquidation_price_oracleUnits_per_bch(self):
         self.assertEqual(standard_contract_proposal().long_liquidation_price_oracleUnits_per_bch, LONG_LIQUIDATION_PRICE)
 
     def test_short_liquidation_price_oracleUnits_per_bch(self):
         self.assertEqual(standard_contract_proposal().short_liquidation_price_oracleUnits_per_bch, SHORT_LIQUIDATION_PRICE_AS_HEDGE)
 
-    def test_maker_side(self):
-        self.assertEqual(standard_contract_proposal().maker_side, Side.SHORT)
+    def test_maker_taker_side(self):
+        maker_short = standard_contract_proposal(maker_side=Side.SHORT)
+        self.assertEqual(maker_short.maker_side, Side.SHORT)
+        self.assertEqual(maker_short.taker_side, Side.LONG)
+
+        maker_long = standard_contract_proposal(maker_side=Side.LONG)
+        self.assertEqual(maker_long.maker_side, Side.LONG)
+        self.assertEqual(maker_long.taker_side, Side.SHORT)
+
+    def test_short_long_role(self):
+        maker_short = standard_contract_proposal(maker_side=Side.SHORT)
+        self.assertEqual(maker_short.short_role, Role.MAKER)
+        self.assertEqual(maker_short.long_role, Role.TAKER)
+
+        maker_long = standard_contract_proposal(maker_side=Side.LONG)
+        self.assertEqual(maker_long.long_role, Role.MAKER)
+        self.assertEqual(maker_long.short_role, Role.TAKER)
 
     ######################
     # Exact secondary values derived from contract parameters
     ######################
     def test_short_input_sats(self):
         self.assertEqual(standard_contract_proposal().short_input_sats, SHORT_INPUT_SATS_AS_HEDGE)
 
@@ -610,9 +625,16 @@
         self.assertEqual(hedge_redemption.cost_sats_for_nominal_value_at_redemption, hedge_redemption.short_payout_sats)
 
         # leveraged short redemption is different from short payout
         self.assertNotEqual(leveraged_short_redemption.cost_sats_for_nominal_value_at_redemption, leveraged_short_redemption.short_payout_sats)
         self.assertEqual(leveraged_short_redemption.cost_sats_for_nominal_value_at_redemption, COST_SATS_FOR_NOMINAL_VALUE_AT_REDEMPTION)
 
 
+class TestContractSide(unittest.TestCase):
+    def test_from_string_works_for_known_api_values(self):
+        self.assertEqual(Side.from_string('short'), Side.SHORT)
+        self.assertEqual(Side.from_string('hedge'), Side.SHORT)
+        self.assertEqual(Side.from_string('long'), Side.LONG)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `anyhedge-0.3.6/anyhedge/tests/test_fee.py` & `anyhedge-0.3.7/anyhedge/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/anyhedge/tests/test_oracle.py` & `anyhedge-0.3.7/anyhedge/tests/test_oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/anyhedge.egg-info/PKG-INFO` & `anyhedge-0.3.7/anyhedge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.3.6
+Version: 0.3.7
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.3.6/anyhedge.egg-info/SOURCES.txt` & `anyhedge-0.3.7/anyhedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.6/pyproject.toml` & `anyhedge-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'anyhedge'
-version = '0.3.6'
+version = '0.3.7'
 authors = [
   { name='emergent_reasons', email='emergent_reasons@gmail.com' },
 ]
 license = { file = "LICENSE" }
 description = 'Basic components of AnyHedge contracts'
 readme = 'README.md'
 requires-python = '>=3.10'
```

