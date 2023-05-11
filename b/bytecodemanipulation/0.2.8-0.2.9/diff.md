# Comparing `tmp/bytecodemanipulation-0.2.8.tar.gz` & `tmp/bytecodemanipulation-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecodemanipulation-0.2.8.tar", last modified: Sat May  6 15:08:32 2023, max compression
+gzip compressed data, was "bytecodemanipulation-0.2.9.tar", last modified: Thu May 11 11:41:26 2023, max compression
```

## Comparing `bytecodemanipulation-0.2.8.tar` & `bytecodemanipulation-0.2.9.tar`

### file list

```diff
@@ -1,127 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.974570 bytecodemanipulation-0.2.8/bytecodemanipulation/
--rw-r--r--   0 runner    (1001) docker     (123)    21892 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    55947 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunctionHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Specialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/annotated_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/AbstractBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/syntax_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/CommonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/builtin_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.982570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.986570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    22643 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.986570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/specialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_11/specialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/mixin_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/optimise_self.py
--rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/optimiser_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-06 15:08:26.000000 bytecodemanipulation-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    50336 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_Assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_MutableFunctionHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_StandardLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_optimiser_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.735894 bytecodemanipulation-0.2.9/bytecodemanipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    21892 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56164 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/MutableFunctionHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Specialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/TypeEnforcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/annotated_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.735894 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/AbstractBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/syntax_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.739894 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/CommonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.739894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.739894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/builtin_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.743894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.751894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22643 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/RawAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.751894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.755894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.755894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/specialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/mixin_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/optimise_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/optimiser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.735894 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-11 11:41:17.000000 bytecodemanipulation-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    50753 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_InlineSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Specializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_StandardLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_issues.py
```

### Comparing `bytecodemanipulation-0.2.8/LICENSE` & `bytecodemanipulation-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/PKG-INFO` & `bytecodemanipulation-0.2.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,19 @@
-Metadata-Version: 2.1
-Name: bytecodemanipulation
-Version: 0.2.8
-Summary: High level python bytecode manipulation
-Home-page: https://github.com/uuk0/PyBytecodeManipulator
-Author: uuk
-Author-email: uuk1301@gmail.com
-Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyBytecodeManipulator
-A high level cross-version python bytecode manipulation library build ontop 
-of 'dis' and 'inspect' 
+A high level cross-version python bytecode manipulation library build ontop
+of 'dis' and 'inspect'
 
-Supports code inlining, branch removing and arbitrary code injection into 
+Supports code inlining, branch removing and arbitrary code injection into
 existing functions.
 
-WARNING: using bytecode manipulation on a so low level as we do can break 
-the python runtime at any point without a warning. We circumvent a lot of 
-safety checks normally done. 
+WARNING: using bytecode manipulation on a so low level as we do can break
+the python runtime at any point without a warning. We circumvent a lot of
+safety checks normally done.
 
-WARNING: We cannot make sure that everything works as it should, expect broken code 
+WARNING: We cannot make sure that everything works as it should, expect broken code
 at runtime!
 
 
 Supported python versions:
 
 - 3.10 (main development)
 - 3.11.0[b3] (forward porting; WIP; Currently not working)
@@ -39,92 +21,129 @@
 Other versions will not work as a lot of config is stored in .json files per-version,
 so you may need to provide your own .json config files for the version you need.
 
 (Some versions might be plug-and-play, but most will require code changes additionally)
 
 ## Why are there so many print()-s?
 
-Due to the breaking nature of anything this code touches, and the absents of any traces 
-in the function itself, we decided to add a lot of "debug" statements indicating 
-mostly the who-has-done-what-to-which-method for the runtime. 
+Due to the breaking nature of anything this code touches, and the absents of any traces
+in the function itself, we decided to add a lot of "debug" statements indicating
+mostly the who-has-done-what-to-which-method for the runtime.
 This makes debugging broken code easier, as it is more clear what happened to each transformed function.
 
 If you want them removed, create your own Fork of this and remove them, on your own risk.
 
-We may use in the future the logging library, so you can disable our logger instance, but we 
+We may use in the future the logging library, so you can disable our logger instance, but we
 are currently in an inter-stage of the code, so other stuff has priority.
 
-## Compatibility with other libraries 
+## Compatibility with other libraries
 
-- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
+- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute
   we modify
 - Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
   results which might contain internal instructions
 
 
-## Debugging your injections 
+## Debugging your injections
 
 There is the possibility to "debug" functions using the execution emulator.
 It will be able to give you more information about a crash than the python core interpreter,
-but will be a lot slower than it. 
+but will be a lot slower than it.
 
-It comes also with the possibility to run your bytecode in another interpreter version, so 
+It comes also with the possibility to run your bytecode in another interpreter version, so
 you can experiment with some stuff.
-In theory, it is also possible to run in python versions not supported by the 
+In theory, it is also possible to run in python versions not supported by the
 bytecode manipulation system, but it is not recommended.
 
 TransformationHandler() takes as an arg debug_code and debug_further_calls
-for activating it for all accessed methods. 
+for activating it for all accessed methods.
 
-BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
+BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on
 that exact method.
 
 
 # Examples
 
-TODO
+Replacing global access with constant value
+
+```python
+from bytecodemanipulation.Optimiser import cache_global_name, apply_now
+
+@cache_global_name("min", lambda: min)
+def test(x, y):
+    return min(x, y)
+
+apply_now(test)
+```
+
+Inlining method calls
+
+```python
+from bytecodemanipulation.Optimiser import cache_global_name, inline_calls, apply_now
+
+@inline_calls
+def call(a, b):
+    return a + b
+
+@cache_global_name("call", lambda: call)
+def test(x, y):
+    return call(x, y)
+
+apply_now(test)
+```
+
+will result in bytecode which could be represented with:
+
+```python
+def test(x, y):
+    return x + y
+```
 
+(there might be extra local variables generated for parameters)
 
 # Applied Optimisations
 
 - Constant Expression inlining (can be declared for custom functions to be constant)
 - LOAD_GLOBAL for builtins (if enabled)
 - standard library inlining (if enabled)
 - specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
 - branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
-- local variable elimination
+- local variable elimination (TODO: add more cases)
 
 
 # Currently Limitations
 
 - Line Numbers get mixed up, we need some way to assign meaningful line numbers
-- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
+- With python 3.11, exception table exists, and this breaks our current concept of one big flow diagram,
   as exception handling code might exist outside the default flow
-- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
-- Method inlining is not working properly and needs a lot more testing
+- Also python 3.11 introduces CACHE-s for instructions, which will require some work in order to work
+- During optimization, a lot of stuff is being recomputed each optimization pass, we need to cache that drastically
+- Method inlining is not working properly and needs a lot more testing (WIP)
 - If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
   inline method accesses for further optimisation
 - Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
   parent instruction, using the arg to switch between modes
 
 
 # Assembly Code
 
 - The library provides also a way to use some "python-assembly" for writing code
 - This is only python bytecode, so no fancy stuff can be done
 - See ASSEMBLY.md for more information on instructions
 - We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
 - You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
+    - assembly(\<code>) can be used for inline assembly
+    - this also includes macro, which may be also created from python-defined methods
 
 
-## Code Formatting
+# Code Formatting
 
 We use the python formatting library "black" on our code
 
 # TODO's
 
 - abstract opcode affect away into a .json file describing all opcodes
 - create a json file for defining certain bytecode sequences
 - write more library-specific optimisations
 - write generating bytecode system for emulator, constructing a function pointing to the
-.json file for exception printing, and optimizing wherever possible
+  .json file for exception printing, and optimizing wherever possible
```

### Comparing `bytecodemanipulation-0.2.8/README.md` & `bytecodemanipulation-0.2.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,37 @@
+Metadata-Version: 2.1
+Name: bytecodemanipulation
+Version: 0.2.9
+Summary: High level python bytecode manipulation
+Home-page: https://github.com/uuk0/PyBytecodeManipulator
+Author: uuk
+Author-email: uuk1301@gmail.com
+Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyBytecodeManipulator
-A high level cross-version python bytecode manipulation library build ontop 
-of 'dis' and 'inspect' 
+A high level cross-version python bytecode manipulation library build ontop
+of 'dis' and 'inspect'
 
-Supports code inlining, branch removing and arbitrary code injection into 
+Supports code inlining, branch removing and arbitrary code injection into
 existing functions.
 
-WARNING: using bytecode manipulation on a so low level as we do can break 
-the python runtime at any point without a warning. We circumvent a lot of 
-safety checks normally done. 
+WARNING: using bytecode manipulation on a so low level as we do can break
+the python runtime at any point without a warning. We circumvent a lot of
+safety checks normally done.
 
-WARNING: We cannot make sure that everything works as it should, expect broken code 
+WARNING: We cannot make sure that everything works as it should, expect broken code
 at runtime!
 
 
 Supported python versions:
 
 - 3.10 (main development)
 - 3.11.0[b3] (forward porting; WIP; Currently not working)
@@ -21,92 +39,129 @@
 Other versions will not work as a lot of config is stored in .json files per-version,
 so you may need to provide your own .json config files for the version you need.
 
 (Some versions might be plug-and-play, but most will require code changes additionally)
 
 ## Why are there so many print()-s?
 
-Due to the breaking nature of anything this code touches, and the absents of any traces 
-in the function itself, we decided to add a lot of "debug" statements indicating 
-mostly the who-has-done-what-to-which-method for the runtime. 
+Due to the breaking nature of anything this code touches, and the absents of any traces
+in the function itself, we decided to add a lot of "debug" statements indicating
+mostly the who-has-done-what-to-which-method for the runtime.
 This makes debugging broken code easier, as it is more clear what happened to each transformed function.
 
 If you want them removed, create your own Fork of this and remove them, on your own risk.
 
-We may use in the future the logging library, so you can disable our logger instance, but we 
+We may use in the future the logging library, so you can disable our logger instance, but we
 are currently in an inter-stage of the code, so other stuff has priority.
 
-## Compatibility with other libraries 
+## Compatibility with other libraries
 
-- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
+- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute
   we modify
 - Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
   results which might contain internal instructions
 
 
-## Debugging your injections 
+## Debugging your injections
 
 There is the possibility to "debug" functions using the execution emulator.
 It will be able to give you more information about a crash than the python core interpreter,
-but will be a lot slower than it. 
+but will be a lot slower than it.
 
-It comes also with the possibility to run your bytecode in another interpreter version, so 
+It comes also with the possibility to run your bytecode in another interpreter version, so
 you can experiment with some stuff.
-In theory, it is also possible to run in python versions not supported by the 
+In theory, it is also possible to run in python versions not supported by the
 bytecode manipulation system, but it is not recommended.
 
 TransformationHandler() takes as an arg debug_code and debug_further_calls
-for activating it for all accessed methods. 
+for activating it for all accessed methods.
 
-BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
+BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on
 that exact method.
 
 
 # Examples
 
-TODO
+Replacing global access with constant value
+
+```python
+from bytecodemanipulation.Optimiser import cache_global_name, apply_now
+
+@cache_global_name("min", lambda: min)
+def test(x, y):
+    return min(x, y)
+
+apply_now(test)
+```
+
+Inlining method calls
+
+```python
+from bytecodemanipulation.Optimiser import cache_global_name, inline_calls, apply_now
+
+@inline_calls
+def call(a, b):
+    return a + b
+
+@cache_global_name("call", lambda: call)
+def test(x, y):
+    return call(x, y)
+
+apply_now(test)
+```
+
+will result in bytecode which could be represented with:
+
+```python
+def test(x, y):
+    return x + y
+```
 
+(there might be extra local variables generated for parameters)
 
 # Applied Optimisations
 
 - Constant Expression inlining (can be declared for custom functions to be constant)
 - LOAD_GLOBAL for builtins (if enabled)
 - standard library inlining (if enabled)
 - specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
 - branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
-- local variable elimination
+- local variable elimination (TODO: add more cases)
 
 
 # Currently Limitations
 
 - Line Numbers get mixed up, we need some way to assign meaningful line numbers
-- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
+- With python 3.11, exception table exists, and this breaks our current concept of one big flow diagram,
   as exception handling code might exist outside the default flow
-- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
-- Method inlining is not working properly and needs a lot more testing
+- Also python 3.11 introduces CACHE-s for instructions, which will require some work in order to work
+- During optimization, a lot of stuff is being recomputed each optimization pass, we need to cache that drastically
+- Method inlining is not working properly and needs a lot more testing (WIP)
 - If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
   inline method accesses for further optimisation
 - Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
   parent instruction, using the arg to switch between modes
 
 
 # Assembly Code
 
 - The library provides also a way to use some "python-assembly" for writing code
 - This is only python bytecode, so no fancy stuff can be done
 - See ASSEMBLY.md for more information on instructions
 - We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
 - You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
+    - assembly(\<code>) can be used for inline assembly
+    - this also includes macro, which may be also created from python-defined methods
 
 
-## Code Formatting
+# Code Formatting
 
 We use the python formatting library "black" on our code
 
 # TODO's
 
 - abstract opcode affect away into a .json file describing all opcodes
 - create a json file for defining certain bytecode sequences
 - write more library-specific optimisations
 - write generating bytecode system for emulator, constructing a function pointing to the
-.json file for exception printing, and optimizing wherever possible
+  .json file for exception printing, and optimizing wherever possible
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/Emulator.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/Emulator.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/Mixin.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunction.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/MutableFunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -822,14 +822,17 @@
 
         if self.opcode == Opcodes.RAISE_VARARGS:
             return 0, self.arg, None
 
         if self.opcode == Opcodes.DUP_TOP_TWO:
             return 2, 4, None
 
+        if self.opcode == Opcodes.ROT_THREE:
+            return 3, 3, None
+
         raise RuntimeError(self)
 
     def special_stack_affect_when_followed_by(self, instr: "Instruction") -> int:
         if self.opcode == Opcodes.FOR_ITER and instr == self.arg_value:
             return -2
 
         return 0
@@ -1523,14 +1526,21 @@
                         [Opcodes.EXTENDED_ARG, iarg]
                     )
                     offset += 1
 
             if not (0 <= arg <= 255 and 0 <= instruction.opcode <= 255):
                 print("error", instruction)
 
+                print("----")
+
+                for ins in instructions:
+                    print(repr(ins))
+
+                print("----")
+
             self.__raw_code += bytes([instruction.opcode, arg])
 
     def get_raw_code(self):
         if self.__instructions is not None:
             self.assemble_instructions()
 
         return self.__raw_code
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunctionHelpers.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/MutableFunctionHelpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,30 +127,43 @@
 
         self.print_recursive(root.next_instruction, visited, level)
 
         if root.has_jump():
             self.print_recursive(root.arg_value, visited, level + 1)
 
 
-def prefix_all_locals_with(
+def prefix_all_locals_with_all(
+    mutable: MutableFunction | MutableFunctionWithTree,
+    prefix: str,
+):
+    if isinstance(mutable, MutableFunctionWithTree):
+        mutable.mutable.assemble_instructions_from_tree(mutable.root)
+        mutable = mutable.mutable
+
+    mutable.shared_variable_names = [prefix + e for e in mutable.shared_variable_names]
+
+    for instruction in mutable.instructions:
+        if instruction.has_local():
+            instruction.change_arg(instruction.arg)
+
+
+def prefix_all_locals_with_specified(
     mutable: MutableFunction | MutableFunctionWithTree,
     prefix: str,
     protected_locals: typing.List[str] = tuple(),
 ):
     if isinstance(mutable, MutableFunctionWithTree):
         mutable.mutable.assemble_instructions_from_tree(mutable.root)
         mutable = mutable.mutable
 
     mutable.shared_variable_names = [
         prefix + e if e not in protected_locals else e
         for e in mutable.shared_variable_names
     ]
 
-    print(mutable.shared_variable_names)
-
     for instruction in mutable.instructions:
         if instruction.has_local():
             instruction.update_owner(mutable, instruction.offset)
 
 
 def replace_opcode_with_other(
     mutable: MutableFunction | MutableFunctionWithTree,
@@ -262,14 +275,15 @@
 
 
 def insert_method_into(
     body: MutableFunction | MutableFunctionWithTree,
     offset: typing.Union[Instruction, int],
     to_insert: MutableFunction | MutableFunctionWithTree,
     protected_locals: typing.List[str] = tuple(),
+    drop_return_result=True,
 ):
     """
     Inserts the function AFTER the given offset / Instruction.
     If wanted at HEAD, set offset to -1
     """
 
     if isinstance(to_insert, MutableFunctionWithTree):
@@ -289,15 +303,21 @@
         HEAD_INSTRUCTION = body.mutable.instructions[offset]
     else:
         HEAD_INSTRUCTION = offset
 
     for instr in to_insert.instructions:
         instr.offset = -1
 
-    prefix_all_locals_with(to_insert, to_insert.function_name + ":", protected_locals)
+    if protected_locals is not None:
+        prefix_all_locals_with_specified(
+            to_insert, to_insert.function_name + ":", protected_locals
+        )
+    else:
+        prefix_all_locals_with_all(to_insert, to_insert.function_name + ":")
+
     replace_opcode_with_other(
         to_insert, Opcodes.RETURN_VALUE, Opcodes.INTERMEDIATE_INNER_RETURN
     )
     inline_access_to_global(to_insert, "capture_local", capture_local)
     inline_access_to_global(to_insert, "outer_return", outer_return)
 
     # MutableFunctionWithTree(to_insert).print_recursive()
@@ -305,20 +325,20 @@
     instr = None
     previous = None
     for instr in to_insert.instructions:
         if previous is not None:
             previous.next_instruction = instr
 
         if instr.opcode == Opcodes.INTERMEDIATE_INNER_RETURN:
-            previous.next_instruction = Instruction.create(Opcodes.POP_TOP)
-            previous.next_instruction.update_owner(to_insert, -1)
-            previous.next_instruction.next_instruction = instr
+            if drop_return_result:
+                previous.insert_after(Instruction(to_insert, -1, Opcodes.POP_TOP))
 
-            instr.change_opcode(Opcodes.JUMP_ABSOLUTE)
-            instr.change_arg_value(HEAD_INSTRUCTION.next_instruction)
+            instr.change_opcode(
+                Opcodes.JUMP_ABSOLUTE, HEAD_INSTRUCTION.next_instruction
+            )
 
         previous = instr
 
     if instr is not None and instr.next_instruction is None:
         instr.next_instruction = HEAD_INSTRUCTION.next_instruction
 
     to_insert.assemble_instructions_from_tree(
@@ -376,7 +396,34 @@
     body.visitor(visit)
 
     # body.print_recursive()
 
     body.mutable.assemble_instructions_from_tree(body.root)
 
     # body.print_recursive()
+
+
+def inline_calls_to_const_functions(mutable: MutableFunction):
+    from bytecodemanipulation.Optimiser import _OptimisationContainer
+
+    for instr in mutable.instructions[:]:
+        if instr.opcode == Opcodes.CALL_FUNCTION:
+            source = next(instr.trace_stack_position(instr.arg))
+
+            if source.opcode != Opcodes.LOAD_CONST:
+                continue
+
+            target = source.arg_value
+
+            container = _OptimisationContainer.get_for_target(target)
+            if not container.try_inline_calls:
+                continue
+
+            instr.change_opcode(Opcodes.NOP)
+            insert_method_into(
+                mutable,
+                instr.offset,
+                MutableFunction(target),
+                drop_return_result=False,
+                protected_locals=None,
+            )
+            source.change_opcode(Opcodes.NOP)
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/Opcodes.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/Opcodes.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/Optimiser.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/Optimiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,16 @@
         self.side_effect_alternative: typing.Callable = None
 
         # attributes are never mutated
         self.is_static = False
 
         self.static_attributes: typing.Set[str] = set()
 
+        self.try_inline_calls = False
+
         # Exceptions that can be raised from here
         self.may_raise_exceptions: typing.Set[
             typing.Type[Exception] | Exception
         ] | None = None
 
         self.specializations: typing.List[
             typing.Callable[[SpecializationContainer], None]
@@ -227,14 +229,17 @@
         self.is_optimized = True
 
         if DISABLE_OPTIMISATION_APPLY:
             return
 
         # print("opt", self.target)
         from bytecodemanipulation.optimiser_util import apply_specializations
+        from bytecodemanipulation.MutableFunctionHelpers import (
+            inline_calls_to_const_functions,
+        )
 
         if self.children:
             self._walk_children_and_copy_attributes()
 
             for child in self.children:
                 child.run_optimisers()
 
@@ -298,14 +303,17 @@
             if inline_constant_method_invokes(mutable):
                 continue
 
             # Remove conditional jumps no longer required
             if remove_branch_on_constant(mutable):
                 continue
 
+            if inline_calls_to_const_functions(mutable):
+                continue
+
             break
 
         mutable.assemble_instructions_from_tree(mutable.instructions[0].optimise_tree())
 
         mutable.reassign_to_function()
 
         # print(mutable)
@@ -722,27 +730,40 @@
             container.static_attributes |= set(attributes)
 
         return target
 
     return annotate
 
 
-def apply_now():
+def inline_calls(target: typing.Callable = None):
+    def annot(tar):
+        container = _OptimisationContainer.get_for_target(target)
+        container.try_inline_calls = True
+        return tar
+
+    if target:
+        return annot(target)
+    return annot
+
+
+def apply_now(target: typing.Callable = None):
     """
     Applies the optimisations NOW
     """
 
-    def annotate(target):
+    def annotate(tar):
         # dis.dis(target)
 
-        container = _OptimisationContainer.get_for_target(target)
+        container = _OptimisationContainer.get_for_target(tar)
         container.run_optimisers()
 
-        return target
+        return tar
 
+    if target:
+        return annotate(target)
     return annotate
 
 
 class IOptimised:
     """
     Implement this to apply optimisation on parts of the class
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/Specialization.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/Specialization.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/AbstractBase.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/AbstractBase.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             scope.global_scope = GLOBAL_SCOPE_CACHE[target.__module__]
         else:
             GLOBAL_SCOPE_CACHE[target.__module__] = scope.global_scope
 
         return scope
 
     def __init__(self):
-        self.labels: typing.Set[str] = set()
+        self.labels: typing.Set["IIdentifierAccessor"] = set()
         self.global_scope = {}
         self.scope_path: typing.List[str] = []
         self._name_counter = 1
         self.globals_dict = {}
         self.module_file: str = None
         self.last_base_token: AbstractToken = None
         self.macro_parameter_namespace: typing.Dict[str] = {}
@@ -98,15 +98,19 @@
                     scope = scope[e]
                 else:
                     return
 
             return scope
 
     def exists_label(self, name: str) -> bool:
-        return name in self.labels
+        for entry in self.labels:
+            if entry == name:
+                return True
+
+        return False
 
     def copy(
         self,
         sub_scope_name: str | list = None,
         copy_labels=False,
         keep_scope_name_generator: bool = None,
     ):
@@ -192,25 +196,25 @@
 
 class AbstractAccessExpression(AbstractSourceExpression, ABC):
     PREFIX: str | None = None
     IS_STATIC = False
 
     def __init__(
         self,
-        name: typing.Callable[[ParsingScope], str] | str,
+        name: "IIdentifierAccessor | str",
         token: AbstractToken | typing.List[AbstractToken] = None,
     ):
         self.name = name
         self.token = token
 
     def __eq__(self, other):
-        return type(self) == type(other) and self.get_name(None) == other.get_name(None)
+        return type(self) == type(other) and self.name == other.name
 
     def __repr__(self):
-        return f"{self.PREFIX}{self.get_name(None)}"
+        return f"{self.PREFIX}{self.name}"
 
     def copy(self) -> "AbstractAccessExpression":
         return type(self)(
             self.name, self.token.copy() if isinstance(self.token, list) else self.token
         )
 
     def get_static_value(self, scope: ParsingScope) -> typing.Any:
@@ -222,7 +226,107 @@
 
 class JumpToLabel:
     def __init__(self, name: str):
         self.name = name
 
     def __repr__(self):
         return f"-> Label('{self.name}')"
+
+
+class IIdentifierAccessor:
+    def __call__(self, scope: ParsingScope):
+        raise NotImplementedError
+
+
+class MacroExpandedIdentifier(IIdentifierAccessor):
+    def __init__(
+        self,
+        macro_name: typing.Union[str, "IIdentifierAccessor"],
+        token: typing.List[AbstractToken] = None,
+    ):
+        self.macro_name = macro_name
+        self.token = token
+
+    def __hash__(self):
+        return hash(self.macro_name)
+
+    def __eq__(self, other):
+        if isinstance(other, MacroExpandedIdentifier):
+            return self.macro_name == other.macro_name
+        return False
+
+    def __repr__(self):
+        return f"&{self.macro_name}"
+
+    def __call__(self, scope: ParsingScope):
+        from bytecodemanipulation.assembler.syntax_errors import (
+            throw_positioned_syntax_error,
+        )
+        from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
+            ConstantAccessExpression,
+        )
+        from bytecodemanipulation.data.shared.expressions.DerefAccessExpression import (
+            DerefAccessExpression,
+        )
+        from bytecodemanipulation.data.shared.expressions.GlobalAccessExpression import (
+            GlobalAccessExpression,
+        )
+        from bytecodemanipulation.data.shared.expressions.LocalAccessExpression import (
+            LocalAccessExpression,
+        )
+
+        if scope is None:
+            raise SyntaxError("no scope provided")
+
+        if self.token[1].text not in scope.macro_parameter_namespace:
+            raise throw_positioned_syntax_error(
+                scope,
+                self.token,
+                "Could not find name in macro parameter space",
+            )
+
+        value = scope.macro_parameter_namespace[self.token[1].text]
+
+        if isinstance(value, ConstantAccessExpression):
+            if not isinstance(value.value, str):
+                raise throw_positioned_syntax_error(
+                    scope,
+                    self.token,
+                    f"Expected 'string' for name de-referencing, got {value}",
+                )
+
+            return value.value
+
+        if isinstance(
+            value,
+            (
+                GlobalAccessExpression,
+                LocalAccessExpression,
+                DerefAccessExpression,
+            ),
+        ):
+            return value.get_name(scope)
+
+        raise throw_positioned_syntax_error(
+            scope,
+            self.token,
+            f"Expected <static evaluated expression> for getting the name for storing, got {value}",
+        )
+
+
+class StaticIdentifier(IIdentifierAccessor):
+    def __init__(self, name: str):
+        self.name = name
+
+    def __eq__(self, other):
+        return (
+            isinstance(other, StaticIdentifier) and self.name == other.name
+        ) or self.name == other
+
+    def __hash__(self):
+        return hash(self.name)
+
+    def __repr__(self):
+        return repr(self.name)
+
+    def __call__(self, scope: ParsingScope):
+        return self.name
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Emitter.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dis
 import string
 import types
 import typing
 
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import Lexer
 from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
 from bytecodemanipulation.Opcodes import Opcodes
 from bytecodemanipulation.assembler.Parser import (
     Parser as AssemblyParser,
 )
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
@@ -108,15 +109,15 @@
             elif value == assembly_targets.label:
                 invoke = next(instr.trace_stack_position_use(0))
                 arg = next(invoke.trace_stack_position(0))
                 assert (
                     arg.opcode == Opcodes.LOAD_CONST
                 ), "only constant label names are allowed!"
 
-                labels.add(arg.arg_value)
+                labels.add(StaticIdentifier(arg.arg_value))
                 invoke.change_opcode(Opcodes.BYTECODE_LABEL, arg.arg_value)
                 invoke.insert_after(Instruction(target, -1, Opcodes.LOAD_CONST, None))
                 instr.change_opcode(Opcodes.NOP)
                 # print(type(arg))
                 arg.change_opcode(Opcodes.NOP)
 
     if not insertion_points:
@@ -136,15 +137,15 @@
             Lexer(code).add_line_offset(instr.source_location[0] + 1).lex(),
             scope.scope_path.clear() or scope,
         ).parse()
         for code, instr in insertion_points
     ]
 
     for asm in assemblies:
-        labels.update(asm.collect_label_info())
+        labels.update(asm.collect_label_info(scope))
 
     scope.labels |= labels
 
     max_stack_effects = []
 
     label_targets: typing.Dict[str, Instruction] = {}
 
@@ -279,15 +280,15 @@
 
     if module.__name__ in GLOBAL_SCOPE_CACHE:
         scope.global_scope = GLOBAL_SCOPE_CACHE[module.__name__]
     else:
         GLOBAL_SCOPE_CACHE[module.__name__] = scope.global_scope
 
     asm = AssemblyParser(asm_code, scope).parse()
-    scope.labels = asm.get_labels()
+    scope.labels = asm.get_labels(scope)
     # asm.fill_scope_complete(scope)
     scope.scope_path.clear()
     create_function = lambda m: None
     target = MutableFunction(create_function)
     target.shared_variable_names[0] = "$module$"
     bytecode = asm.create_bytecode(target, scope)
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Lexer.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Lexer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Parser.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import typing
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
+from bytecodemanipulation.assembler.AbstractBase import (
+    IIdentifierAccessor,
+    MacroExpandedIdentifier,
+    StaticIdentifier,
+)
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import _syntax_wrapper
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.expressions.AttributeAccessExpression import (
@@ -49,16 +54,15 @@
 )
 from bytecodemanipulation.data.shared.expressions.SubscriptionAccessExpression import (
     SubscriptionAccessExpression,
 )
 from bytecodemanipulation.data.shared.expressions.TopOfStackAccessExpression import (
     TopOfStackAccessExpression,
 )
-
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
 
 from bytecodemanipulation.MutableFunction import Instruction
 
 from bytecodemanipulation.assembler.Lexer import (
     Lexer,
     SpecialToken,
     StringLiteralToken,
@@ -180,15 +184,15 @@
             lambda: not self.try_consume(SpecialToken("}")),
             eof_error="Expected '}', got EOF",
             scope=scope,
         )
 
         if namespace_part:
             if isinstance(namespace_part, str):
-                if self.scope.scope_path.pop() != namespace_part:
+                if self.scope.scope_path.pop(-1) != namespace_part:
                     raise RuntimeError
             else:
                 if self.scope.scope_path[-len(namespace_part) :] != namespace_part:
                     raise RuntimeError
 
                 del self.scope.scope_path[-len(namespace_part) :]
 
@@ -277,15 +281,15 @@
 
         if isinstance(target, MacroAssembly.MacroOverloadPage):
             for macro in typing.cast(
                 MacroAssembly.MacroOverloadPage, target
             ).assemblies:
                 if macro.allow_assembly_instr:
                     self.rollback()
-                    print(name)
+                    # print(name)
                     return AbstractCallAssembly.IMPLEMENTATION.consume_macro_call(
                         self, scope
                     )
 
         self.rollback()
 
     def try_consume_access_to_value(
@@ -304,14 +308,15 @@
         todo: make it extendable
 
         :param allow_tos: if TOS (%) is allowed
         :param allow_primitives: if primitives are allowed, e.g. numeric literals
         :param allow_op: if operations are allowed, starting with OP
         :param allow_advanced_access: if expressions like @global[$index].attribute are allowed
         :param scope: the parsing scope instance
+        :param allow_calls: if True, calls will be allowed as expressions
         """
         start_token = self.try_inspect()
 
         if start_token is None:
             return
 
         if allow_primitives:
@@ -322,14 +327,22 @@
                 return ConstantAccessExpression(
                     int(integer.text)
                     if "." not in integer.text
                     else float(integer.text),
                     integer,
                 )
 
+            if isinstance(start_token, IdentifierToken):
+                if start_token.text == "None":
+                    return ConstantAccessExpression(None, start_token)
+                elif start_token.text == "True":
+                    return ConstantAccessExpression(True, start_token)
+                elif start_token.text == "False":
+                    return ConstantAccessExpression(False, start_token)
+
         if not isinstance(start_token, (SpecialToken, IdentifierToken)):
             return
 
         if start_token.text == "@":
             self.consume(SpecialToken("@"), err_arg=scope)
 
             if self.try_consume(SpecialToken("!")):
@@ -353,31 +366,55 @@
             self.consume(SpecialToken("&"), err_arg=scope)
             expr = MacroParameterAccessExpression(
                 self.parse_identifier_like(scope), start_token
             )
 
         elif start_token.text == "%" and allow_tos:
             self.consume(SpecialToken("%"), err_arg=scope)
-            expr = TopOfStackAccessExpression()
+
+            offset = self.try_consume(IntegerToken)
+
+            if offset is not None:
+                return TopOfStackAccessExpression(start_token, int(offset.text))
+
+            expr = TopOfStackAccessExpression(start_token)
 
         elif start_token.text == "~":
             self.consume(SpecialToken("~"), err_arg=scope)
             expr = ModuleAccessExpression(
                 self.parse_identifier_like(scope), start_token
             )
 
         elif start_token.text == "\\":
             self.consume(SpecialToken("\\"), err_arg=scope)
             expr = DiscardValueExpression()
 
-        elif start_token.text == "OP" and allow_op and "OP" in self.INSTRUCTIONS:
-            self.consume(start_token)
-            self.consume(SpecialToken("("), err_arg=scope)
-            expr = self.INSTRUCTIONS["OP"].consume(self, scope)
-            self.consume(SpecialToken(")"), err_arg=scope)
+        elif (
+            start_token.text == "OP"
+            and allow_op
+            and "OP" in self.INSTRUCTIONS
+            and AbstractOpAssembly.IMPLEMENTATION is not None
+        ):
+            self.consume(start_token, err_arg=scope)
+
+            if not (opening := self.try_consume(SpecialToken("("))):
+                raise throw_positioned_syntax_error(
+                    scope,
+                    self[-1:1],
+                    "expected '(' after OP when used in expressions",
+                )
+
+            expr = AbstractOpAssembly.IMPLEMENTATION.consume(self, scope)
+
+            if not self.try_consume(SpecialToken(")")):
+                raise throw_positioned_syntax_error(
+                    scope,
+                    [opening, self[0]],
+                    "expected ')' after operation",
+                )
 
         else:
             return
 
         if allow_advanced_access:
             while True:
                 if self.try_consume(SpecialToken("[")):
@@ -408,21 +445,22 @@
 
                     expr = SubscriptionAccessExpression(
                         expr,
                         index,
                     )
 
                 elif self.try_consume(SpecialToken(".")):
-                    if self.try_consume(SpecialToken("(")):
+                    if opening_bracket := self.try_consume(SpecialToken("(")):
                         if not (
                             index := self.try_consume_access_to_value(
                                 allow_primitives=True,
                                 allow_tos=allow_tos,
                                 allow_op=allow_op,
                                 scope=scope,
+                                allow_calls=allow_calls,
                             )
                         ):
                             raise throw_positioned_syntax_error(
                                 scope,
                                 self.try_inspect() or self[-1],
                                 "expected <expression>"
                                 + (
@@ -432,23 +470,27 @@
                                     )
                                     else " (did you forget a prefix?)"
                                 ),
                             )
 
                         if not self.try_consume(SpecialToken(")")):
                             raise throw_positioned_syntax_error(
-                                scope, self.try_inspect() or self[-1], "expected ')'"
+                                scope,
+                                [opening_bracket, self.try_inspect()],
+                                "expected ')'",
                             )
 
                         expr = DynamicAttributeAccessExpression(expr, index)
+
                     elif self.try_consume(SpecialToken("!")):
-                        name = self.try_consume(IdentifierToken)
+                        name = self.parse_identifier_like(scope)
                         expr = StaticAttributeAccessExpression(expr, name)
+
                     else:
-                        name = self.try_consume(IdentifierToken)
+                        name = self.parse_identifier_like(scope)
                         expr = AttributeAccessExpression(expr, name)
 
                 elif self.try_inspect() == SpecialToken("(") and allow_calls:
                     expr = AbstractCallAssembly.IMPLEMENTATION.construct_from_partial(
                         expr, self, scope
                     )
 
@@ -496,65 +538,22 @@
             ):
                 return ConstantAccessExpression(boolean.text == "True", boolean)
 
         # print("failed", self.try_inspect())
 
         self.rollback()
 
-    def try_parse_identifier_like(self) -> typing.Callable[[ParsingScope], str] | None:
+    def try_parse_identifier_like(self) -> IIdentifierAccessor | None:
         if expr := self.try_consume_multi([SpecialToken("&"), IdentifierToken]):
-
-            def get(scope: ParsingScope):
-                # If this is None, we are only inspecting
-                if scope is None:
-                    return str(get)
-
-                if expr[1].text not in scope.macro_parameter_namespace:
-                    raise throw_positioned_syntax_error(
-                        scope,
-                        expr,
-                        "Could not find name in macro parameter space",
-                    )
-
-                value = scope.macro_parameter_namespace[expr[1].text]
-
-                if isinstance(value, ConstantAccessExpression):
-                    if not isinstance(value.value, str):
-                        raise throw_positioned_syntax_error(
-                            scope,
-                            expr,
-                            f"Expected 'string' for name de-referencing, got {value}",
-                        )
-
-                    return value.value
-
-                if isinstance(
-                    value,
-                    (
-                        GlobalAccessExpression,
-                        LocalAccessExpression,
-                        DerefAccessExpression,
-                    ),
-                ):
-                    return value.get_name(scope)
-
-                raise throw_positioned_syntax_error(
-                    scope,
-                    expr,
-                    f"Expected <static evaluated expression> for getting the name for storing, got {value}",
-                )
-
-            return get
+            return MacroExpandedIdentifier(expr[1].text, expr)
 
         if expr := self.try_consume(IdentifierToken):
-            return lambda scope: expr.text
+            return StaticIdentifier(expr.text)
 
-    def parse_identifier_like(
-        self, scope: ParsingScope
-    ) -> typing.Callable[[ParsingScope], str]:
+    def parse_identifier_like(self, scope: ParsingScope) -> IIdentifierAccessor:
         identifier = self.try_parse_identifier_like()
 
         if identifier is None:
             raise throw_positioned_syntax_error(
                 scope,
                 self[0],
                 "expected <identifier> or &<identifier>",
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/hook.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/hook.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/syntax_errors.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/syntax_errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import sys
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
-from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
-from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 
 
 def _print_complex_token_location(
     scope: ParsingScope,
     tokens: typing.List[AbstractToken | None],
     exc_type: typing.Type[Exception] = SyntaxError,
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/target.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,7 +113,17 @@
     :param config_pattern: the type of parameter
     """
 
     def annotation(function):
         return function
 
     return annotation
+
+
+def apply_operations(target: typing.Callable):
+    from bytecodemanipulation.MutableFunction import MutableFunction
+    from bytecodemanipulation.assembler.Emitter import apply_inline_assemblies
+
+    mutable = MutableFunction(target)
+    apply_inline_assemblies(mutable)
+    mutable.reassign_to_function()
+    return target
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/parser.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
         return token
 
     T = typing.TypeVar(
         "T", AbstractToken, typing.List[typing.Type[AbstractToken] | AbstractToken]
     )
 
-    def consume(self, expected: T | typing.Type[T], err_arg=None) -> T:
+    def consume(self, expected: T | typing.Type[T] = None, err_arg=None) -> T:
         """
         Consumes a token and compares it against the 'expected' (which is an instance or the expected type of token)
 
         :return: the parsed token
         :raises SyntaxError: if it failed to parse the token (either invalid type or end of stream)
         """
         token: AbstractToken = self.inspect()
@@ -299,15 +299,15 @@
                         f"Expected type {expected.__name__}, got {token} (type: {type(token).__name__})"
                     )
 
         self.cursor += 1
 
         return token
 
-    def try_consume(self, expected: T | typing.Type[T]) -> T | None:
+    def try_consume(self, expected: T | typing.Type[T] = None) -> T | None:
         """
         Tries to consume a token from the token stream
 
         :param expected: the expected type of token, either instance or type
         :return: the consumed token or None
         """
         token: AbstractToken = self.try_inspect()
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/tokenizer.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import typing
+from collections import namedtuple
 
 from .CommonUtil import AbstractCursorStateItem
 
 
 class AbstractToken(abc.ABC):
     __slots__ = ("text", "line", "column", "span")
 
@@ -15,14 +16,17 @@
 
     def __eq__(self, other):
         return type(other) == type(self) and self.text == other.text
 
     def __repr__(self):
         return f"{type(self).__name__}({repr(self.text)})"
 
+    def __hash__(self):
+        return hash((type(self).__name__, self.text))
+
 
 class IntegerToken(AbstractToken):
     pass
 
 
 class FloatToken(AbstractToken):
     pass
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/compiler.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/compiler.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/builtin_spec.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/builtin_spec.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,16 +12,50 @@
 
 @register(typing.cast)
 def specialize_typing_cast(container: SpecializationContainer):
     # typing.cast(<type>, <obj>) -> <obj>
     data_type, value = container.get_arg_specifications()
 
     if ASSERT_TYPE_CASTS:
-        # todo: add check type
-        pass
+        nop = Instruction(container.target, -1, Opcodes.NOP)
+
+        bytecode = [
+            value,
+            Instruction(container.target, -1, Opcodes.DUP_TOP),
+            Instruction(container.target, -1, Opcodes.LOAD_CONST, isinstance),
+            Instruction(container.target, -1, Opcodes.ROT_TWO),
+            data_type,
+            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=2),
+            Instruction(container.target, -1, Opcodes.POP_JUMP_IF_TRUE, nop),
+            Instruction(
+                container.target, -1, Opcodes.LOAD_CONST, "expected data type '"
+            ),
+            Instruction(container.target, -1, Opcodes.LOAD_CONST, repr),
+            data_type,
+            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(container.target, -1, Opcodes.BINARY_ADD),
+            Instruction(container.target, -1, Opcodes.LOAD_CONST, "', but got '"),
+            Instruction(container.target, -1, Opcodes.BINARY_ADD),
+            Instruction(container.target, -1, Opcodes.LOAD_CONST, repr),
+            Instruction(container.target, -1, Opcodes.LOAD_CONST, type),
+            value,
+            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(container.target, -1, Opcodes.BINARY_ADD),
+            Instruction(container.target, -1, Opcodes.LOAD_CONST, "'"),
+            Instruction(container.target, -1, Opcodes.BINARY_ADD),
+            Instruction(container.target, -1, Opcodes.LOAD_CONST, ValueError),
+            Instruction(container.target, -1, Opcodes.ROT_TWO),
+            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(container.target, -1, Opcodes.RAISE_VARARGS, arg=1),
+            nop,
+        ]
+
+        container.replace_call_with_opcodes(bytecode)
+        return
 
     container.replace_call_with_arg(value)
 
 
 @register(min)
 def specialize_min(container: SpecializationContainer):
     # remove when constants are mixed with no constant all but the smallest constant
@@ -48,39 +82,39 @@
         for arg in args:
             norm_instr = arg.get_normalized_data_instr()
             if norm_instr and norm_instr != min_const and norm_instr.has_constant():
                 arg.discard()
 
 
 @register(max)
-def specialize_min(container: SpecializationContainer):
-    # remove when constants are mixed with no constant all but the smallest constant
+def specialize_max(container: SpecializationContainer):
+    # remove when constants are mixed with no constant all but the biggest constant
     args = container.get_arg_specifications()
 
     if args[0].is_self:
         self = args.pop(0)
     else:
         self = None
 
-    min_const: Instruction = None
+    max_const: Instruction = None
 
     # todo: catch compare exceptions
     for arg in args:
         instr: Instruction = arg.get_normalized_data_instr()
 
         if instr and instr.has_constant():
-            if min_const is None or min_const.arg_value < instr.arg_value:
-                min_const = instr
+            if max_const is None or max_const.arg_value < instr.arg_value:
+                max_const = instr
 
-    if min_const is not None:
+    if max_const is not None:
         # todo: for non constants, do a clever try-eval-ahead with the type if arrival
 
         for arg in args:
             norm_instr = arg.get_normalized_data_instr()
-            if norm_instr and norm_instr != min_const and norm_instr.has_constant():
+            if norm_instr and norm_instr != max_const and norm_instr.has_constant():
                 arg.discard()
 
 
 @register(tuple)
 def create_empty_tuple(container: SpecializationContainer):
     if len(container.get_arg_specifications()) == 0:
         container.replace_with_constant_value(tuple())
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,57 +3,60 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.MutableFunction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor, StaticIdentifier
 
 
-class AttributeAccessExpression(AbstractAccessExpression):
+class StaticAttributeAccessExpression(AbstractAccessExpression):
+    IS_STATIC = True
+
     def __init__(
-        self, root: AbstractAccessExpression, name_token: IdentifierToken | str
+        self, root: AbstractAccessExpression, name: typing.Union["IIdentifierAccessor", str],
     ):
         self.root = root
-        self.name_token = (
-            name_token
-            if isinstance(name_token, IdentifierToken)
-            else IdentifierToken(name_token)
+        self.name = (
+            name
+            if not isinstance(name, str)
+            else StaticIdentifier(name)
         )
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.root == other.root
-            and self.name_token == other.name_token
+            and self.name == other.name
         )
 
     def __repr__(self):
-        return f"{self.root}.{self.name_token.text}"
+        return f"{self.root}.!{self.name(None)}"
 
-    def copy(self) -> "AttributeAccessExpression":
-        return AttributeAccessExpression(self.root.copy(), self.name_token)
+    def copy(self) -> "StaticAttributeAccessExpression":
+        return StaticAttributeAccessExpression(self.root.copy(), self.name)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.root.emit_bytecodes(function, scope) + [
             Instruction.create_with_token(
-                self.name_token, function, -1, "LOAD_ATTR", self.name_token.text
+                self.name(scope),
+                function,
+                -1,
+                "STATIC_ATTRIBUTE_ACCESS",
+                self.name(scope),
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        return self.root.emit_bytecodes(function, scope) + [
-            Instruction.create_with_token(
-                self.name_token, function, -1, "STORE_ATTR", self.name_token.text
-            )
-        ]
+        raise RuntimeError
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/CompoundExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/CompoundExpression.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,20 +88,20 @@
         return visitor(
             self,
             tuple(
                 [child.visit_assembly_instructions(visitor) for child in self.children]
             ),
         )
 
-    def collect_label_info(self) -> typing.Set[str]:
-        return self.get_labels()
+    def collect_label_info(self, scope: ParsingScope) -> typing.Set[str]:
+        return self.get_labels(scope)
 
-    def get_labels(self) -> typing.Set[str]:
+    def get_labels(self, scope: ParsingScope) -> typing.Set[str]:
         result = set()
 
         for instr in self.children:
-            result.update(instr.get_labels())
+            result.update(instr.get_labels(scope))
 
         return result
 
     def create_bytecode(self, target: MutableFunction, scope: ParsingScope):
         return self.emit_bytecodes(target, scope)
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import builtins
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.MutableFunction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,59 +3,58 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.MutableFunction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor, StaticIdentifier
 
 
-class StaticAttributeAccessExpression(AbstractAccessExpression):
-    IS_STATIC = True
-
+class AttributeAccessExpression(AbstractAccessExpression):
     def __init__(
-        self, root: AbstractAccessExpression, name_token: IdentifierToken | str
+        self, root: AbstractAccessExpression, name: IIdentifierAccessor | str
     ):
         self.root = root
-        self.name_token = (
-            name_token
-            if isinstance(name_token, IdentifierToken)
-            else IdentifierToken(name_token)
+        self.name = (
+            name
+            if not isinstance(name, str)
+            else StaticIdentifier(name)
         )
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.root == other.root
-            and self.name_token == other.name_token
+            and self.name == other.name
         )
 
     def __repr__(self):
-        return f"{self.root}.!{self.name_token.text}"
+        return f"{self.root}.{self.name(None)}"
 
-    def copy(self) -> "StaticAttributeAccessExpression":
-        return StaticAttributeAccessExpression(self.root.copy(), self.name_token)
+    def copy(self) -> "AttributeAccessExpression":
+        return AttributeAccessExpression(self.root.copy(), self.name)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.root.emit_bytecodes(function, scope) + [
-            Instruction.create_with_token(
-                self.name_token,
-                function,
-                -1,
-                "STATIC_ATTRIBUTE_ACCESS",
-                self.name_token.text,
+            Instruction(
+                function, -1, "LOAD_ATTR", self.name(scope)
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        raise RuntimeError
+        return self.root.emit_bytecodes(function, scope) + [
+            Instruction(
+                function, -1, "STORE_ATTR", self.name(scope)
+            )
+        ]
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 import typing
 
+from bytecodemanipulation.Opcodes import Opcodes
+
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.MutableFunction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class TopOfStackAccessExpression(AbstractAccessExpression):
     PREFIX = "%"
 
-    def __init__(self, token=None):
+    def __init__(self, token=None, offset=0):
         self.token = token
+        self.offset = offset
 
     def __eq__(self, other):
         return type(self) == type(other)
 
     def __repr__(self):
         return f"%"
 
     def copy(self) -> "AbstractAccessExpression":
         return type(self)(self.token)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
+        if self.offset != 0:
+            return [
+                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset)
+                for _ in range(self.offset - 1)
+            ] + [
+                Instruction(function, -1, Opcodes.DUP_TOP),
+                Instruction(function, -1, Opcodes.ROT_TWO),
+                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset),
+            ]
+
         return []
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
+        if self.offset != 0:
+            raise NotImplementedError("%<n> as store target")
+
         return []
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,74 @@
+import abc
 import typing
-from abc import ABC
 
+from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.Lexer import SpecialToken
+from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
+from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
+from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
+    AbstractAssemblyInstruction,
+)
 
 
-if typing.TYPE_CHECKING:
-    from bytecodemanipulation.assembler.Parser import Parser
+class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # STORE_GLOBAL <name> [<source>]
+    NAME = "STORE_GLOBAL"
 
-
-class AbstractAssemblyInstruction(AbstractExpression, IAssemblyStructureVisitable, ABC):
-    NAME: str | None = None
-    IMPLEMENTATION: typing.Type["AbstractAssemblyInstruction"] | None = None
-
-    @classmethod
-    def __init_subclass__(cls, **kwargs):
-        # copy the class definition into all superclasses inheriting from AbstractAssemblyInstruction
-        if ABC not in cls.__bases__:
-            for base in cls.__bases__:
-                if (
-                    issubclass(base, AbstractAssemblyInstruction)
-                    and base != AbstractAssemblyInstruction
-                ):
-                    base.IMPLEMENTATION = cls
-
-            cls.IMPLEMENTATION = cls
+    def __init__(
+        self,
+        name_token: IdentifierToken | IntegerToken | str | int,
+        source: AbstractSourceExpression | None = None,
+    ):
+        self.name_token = (
+            name_token
+            if not isinstance(name_token, (str, int))
+            else (
+                IdentifierToken(name_token)
+                if isinstance(name_token, str)
+                else IntegerToken(str(name_token))
+            )
+        )
+        self.source = source
 
     @classmethod
-    def consume(
-        cls, parser: "Parser", scope: ParsingScope
-    ) -> "AbstractAssemblyInstruction":
-        raise NotImplementedError
-
-    def __init__(self, *_, **__):
-        raise NotImplementedError
-
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        raise NotImplementedError
-
-    def fill_scope_complete(self, scope: ParsingScope):
-        self.visit_parts(
-            lambda e, _: e.fill_scope(scope) if hasattr(e, "fill_scope") else None
+    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
+        parser.try_consume(SpecialToken("@"))
+        name = parser.try_consume([IdentifierToken, IntegerToken])
+
+        if name is None:
+            raise throw_positioned_syntax_error(
+                scope, parser.try_inspect(), "expected <name> or <integer>"
+            )
+
+        source = parser.try_parse_data_source()
+
+        return cls(name, source)
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.name_token == other.name_token
+            and self.source == other.source
         )
-        return scope
 
-    def fill_scope(self, scope: ParsingScope):
-        pass
+    def __repr__(self):
+        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
+
+    def copy(self) -> "AbstractStoreGlobalAssembly":
+        return type(self)(self.name_token, self.source.copy() if self.source else None)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
-        return visitor(self, tuple(), parents)
-
-    def visit_assembly_instructions(
-        self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
-    ):
-        return visitor(self, tuple())
-
-    def get_labels(self) -> typing.Set[str]:
-        return set()
+        return visitor(
+            self, (self.source.visit_parts(visitor, []) if self.source else None,)
+        )
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/CallAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/CallAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,33 +115,35 @@
 
     class KwArgStar(IArg):
         pass
 
     @classmethod
     def construct_from_partial(
         cls, access: AbstractAccessExpression, parser: "Parser", scope: ParsingScope
-    ):
+    ) -> "AbstractCallAssembly":
         """
         Constructs an CallAssembly from an already parsed access expression.
         Used by the Parser when parsing an call as a expression to be used inline
         """
         return cls.consume_inner(
             parser, False, False, scope, call_target=access, allow_target=False
         )
 
     @classmethod
-    def consume_macro_call(cls, parser: "Parser", scope: ParsingScope):
+    def consume_macro_call(
+        cls, parser: "Parser", scope: ParsingScope
+    ) -> "AbstractCallAssembly":
         """
         Consumes a call to a macro
         Used by the Parser when finding macros to be used like assembly instructions
         """
         return cls.consume_inner(parser, False, True, scope)
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "CallAssembly":
+    def consume(cls, parser: "Parser", scope) -> "AbstractCallAssembly":
         """
         The normal consumer for the instruction
         Optionally consumes the PARTIAL and MACRO prefixes
         """
         is_partial = bool(parser.try_consume(IdentifierToken("PARTIAL")))
         is_macro = not is_partial and bool(parser.try_consume(IdentifierToken("MACRO")))
         return cls.consume_inner(parser, is_partial, is_macro, scope)
@@ -281,15 +283,15 @@
             target = None
 
         return cls(call_target, args, target, is_partial, is_macro)
 
     def __init__(
         self,
         call_target: AbstractSourceExpression,
-        args: typing.List["CallAssembly.IArg"],
+        args: typing.List["AbstractCallAssembly.IArg"],
         target: AbstractAccessExpression | None = None,
         is_partial: bool = False,
         is_macro: bool = False,
     ):
         self.call_target = call_target
         self.args = args
         self.target = target
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import abc
 
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+import typing
+
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
+from bytecodemanipulation.assembler.AbstractBase import (
+    ParsingScope,
+    IAssemblyStructureVisitable,
+    AbstractExpression,
+)
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
     ConstantAccessExpression,
 )
@@ -13,22 +20,32 @@
 )
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 
 
 class AbstractClassDefinitionAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # CLASS <name> ['(' [<parent> {',' <parent>}] ')'] '{' ... '}'
+    # CLASS <name> '<' <exposed namespace> '>' ['(' [<parent> {',' <parent>}] ')'] '{' ... '}'
     NAME = "CLASS"
 
     @classmethod
     def consume(
         cls, parser: "Parser", scope: ParsingScope
     ) -> "AbstractClassDefinitionAssembly":
-        name_token = parser.consume(IdentifierToken, err_arg=scope)
+        name = parser.parse_identifier_like(scope)
+
+        namespace = None
+
+        if parser.try_consume(SpecialToken("<")):
+            namespace = [parser.consume(IdentifierToken, err_arg=scope).text]
+
+            while parser.try_consume(SpecialToken(":")):
+                namespace.append(parser.consume(IdentifierToken, err_arg=scope).text)
+
+            parser.consume(SpecialToken(">"), err_arg=scope)
 
         parents = []
 
         if parser.try_consume(SpecialToken("(")):
             if parent := parser.try_consume_access_to_value():
                 parents.append(parent)
 
@@ -47,38 +64,38 @@
 
             if not parser.try_consume(SpecialToken(")")):
                 raise throw_positioned_syntax_error(scope, parser[0], "Expected ')'")
 
         if not parents:
             parents = [ConstantAccessExpression(object)]
 
-        code_block = parser.parse_body(namespace_part=name_token.text, scope=scope)
+        code_block = parser.parse_body(scope=scope, namespace_part=namespace)
         return cls(
-            name_token,
+            name,
             parents,
             code_block,
         )
 
     def __init__(
-        self, name_token: IdentifierToken, parents, code_block: CompoundExpression
+        self, name: IIdentifierAccessor, parents, code_block: CompoundExpression
     ):
-        self.name_token = name_token
+        self.name = name
         self.parents = parents
         self.code_block = code_block
 
     def __repr__(self):
-        return f"ClassAssembly::'{self.name_token.text}'({','.join(map(repr, self.parents))}){{{self.code_block}}}"
+        return f"ClassAssembly::'{self.name}'({','.join(map(repr, self.parents))}){{{self.code_block}}}"
 
     def copy(self):
         return AbstractClassDefinitionAssembly(
-            self.name_token,
+            self.name,
             [parent.copy() for parent in self.parents],
             self.code_block.copy(),
         )
 
     def __eq__(self, other):
         return (
             isinstance(other, type(self))
-            and self.name_token == other.name_token
+            and self.name == other.name
             and self.parents == other.parents
             and self.code_block == other.code_block
         )
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
@@ -17,25 +19,24 @@
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 
 
 class AbstractFunctionDefinitionAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # DEF [<func name>] ['<' ['!'] <bound variables\> '>'] '(' <signature> ')' ['->' <target>] '{' <body> '}'
+    # DEF [<func name>] ['<' ['!'] <bound variables> '>'] '(' <signature> ')' ['->' <target>] '{' <body> '}'
     NAME = "DEF"
 
     @classmethod
     def consume(
         cls, parser: "Parser", scope: ParsingScope
     ) -> "AbstractFunctionDefinitionAssembly":
-        func_name = parser.try_consume(IdentifierToken)
-        bound_variables: typing.List[
-            typing.Tuple[typing.Callable[[ParsingScope], str], bool]
-        ] = []
+        func_name = parser.parse_identifier_like(scope)
+
+        bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool]] = []
         args = []
 
         if parser.try_consume(SpecialToken("<")):
             is_static = bool(parser.try_consume(SpecialToken("!")))
 
             expr = parser.try_parse_identifier_like()
 
@@ -122,46 +123,42 @@
                 "Respect ordering (got 'code' before 'target'): DEF ['name'] ['captured'] ('args') [-> 'target'] { code }",
             )
 
         return cls(func_name, bound_variables, args, body, target)
 
     def __init__(
         self,
-        func_name: IdentifierToken | str | None,
-        bound_variables: typing.List[
-            typing.Tuple[typing.Callable[[ParsingScope], str], bool] | str
-        ],
+        func_name: IIdentifierAccessor | str | None,
+        bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool] | str],
         args: typing.List[AbstractCallAssembly.IArg],
         body: CompoundExpression,
         target: AbstractAccessExpression | None = None,
     ):
         self.func_name = (
-            func_name if not isinstance(func_name, str) else IdentifierToken(func_name)
+            func_name if not isinstance(func_name, str) else StaticIdentifier(func_name)
         )
-        self.bound_variables: typing.List[
-            typing.Tuple[typing.Callable[[ParsingScope], str], bool]
-        ] = []
+        self.bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool]] = []
         # var if isinstance(var, IdentifierToken) else IdentifierToken(var) for var in bound_variables]
 
         def _create_lazy(name: str):
             return lambda scope: name
 
         for element in bound_variables:
             if isinstance(element, str):
                 self.bound_variables.append(
                     (
-                        _create_lazy(element.removeprefix("!")),
+                        StaticIdentifier(element.removeprefix("!")),
                         element.startswith("!"),
                     )
                 )
             elif isinstance(element, tuple):
                 token, is_static = element
 
                 if isinstance(token, str):
-                    self.bound_variables.append((_create_lazy(token), is_static))
+                    self.bound_variables.append((StaticIdentifier(token), is_static))
                 else:
                     self.bound_variables.append(element)
             else:
                 raise ValueError(element)
 
         self.args = args
         self.body = body
@@ -184,28 +181,22 @@
             ),
         )
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.func_name == other.func_name
-            and len(self.bound_variables) == len(other.bound_variables)
-            and all(
-                (
-                    a[0](None) == b[0](None) and a[1] == b[1]
-                    for a, b in zip(self.bound_variables, other.bound_variables)
-                )
-            )
+            and self.bound_variables == other.bound_variables
             and self.args == other.args
             and self.body == other.body
             and self.target == other.target
         )
 
     def __repr__(self):
-        return f"DEF({self.func_name.text}<{repr([(name[0](None), name[1]) for name in self.bound_variables])[1:-1]}>({repr(self.args)[1:-1]}){'-> ' + repr(self.target) if self.target else ''} {{ {self.body} }})"
+        return f"DEF({self.func_name}<{repr([(name[0](None), name[1]) for name in self.bound_variables])[1:-1]}>({repr(self.args)[1:-1]}){'-> ' + repr(self.target) if self.target else ''} {{ {self.body} }})"
 
     def copy(self) -> "AbstractFunctionDefinitionAssembly":
         return type(self)(
             self.func_name,
             self.bound_variables.copy(),
             [arg.copy() for arg in self.args],
             self.body.copy(),
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/IfAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/WhileAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractIFAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # IF <expression> ['\'' <label name> '\''] '{' <body> '}'
-    NAME = "IF"
+class AbstractWhileAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # # WHILE <expression> ['\'' <label name> '\''] '{' <body> '}'
+    NAME = "WHILE"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractIFAssembly":
-        source = parser.try_parse_data_source(
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractWhileAssembly":
+        condition = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False, scope=scope
         )
 
-        if source is None:
+        if condition is None:
             raise throw_positioned_syntax_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         if parser.try_consume(SpecialToken("'")):
-            label_name = parser.consume(IdentifierToken)
+            label_name = parser.parse_identifier_like(scope)
             if not parser.try_consume(SpecialToken("'")):
                 raise throw_positioned_syntax_error(
                     scope, parser.try_inspect(), "expected '"
                 )
         else:
             label_name = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
-            source,
+            condition,
             body,
             label_name,
         )
 
     def __init__(
         self,
         source: AbstractSourceExpression,
         body: CompoundExpression,
-        label_name: IdentifierToken | str | None = None,
+        label_name: IIdentifierAccessor | None = None,
     ):
         self.source = source
         self.body = body
         self.label_name = (
             label_name
             if not isinstance(label_name, str)
-            else IdentifierToken(label_name)
+            else StaticIdentifier(label_name)
         )
 
     def copy(self):
         return type(self)(self.source.copy(), self.body.copy(), self.label_name)
 
     def __eq__(self, other):
         return (
@@ -72,15 +74,15 @@
             and self.source == other.source
             and self.body == other.body
             and self.label_name == other.label_name
         )
 
     def __repr__(self):
         c = "'"
-        return f"IF({self.source}{'' if self.label_name is None else ', label='+c+self.label_name.text+c}) -> {{{self.body}}}"
+        return f"WHILE({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
@@ -91,17 +93,17 @@
         )
 
     def visit_assembly_instructions(
         self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
     ):
         return visitor(self, (self.body.visit_assembly_instructions(visitor),))
 
-    def get_labels(self) -> typing.Set[str]:
+    def get_labels(self, scope: ParsingScope):
         return (
             set()
             if self.label_name is None
             else {
-                self.label_name.text,
-                self.label_name.text + "_END",
-                self.label_name.text + "_HEAD",
+                self.label_name(scope),
+                self.label_name(scope) + "_END",
+                self.label_name(scope) + "_INNER",
             }
-        ) | self.body.get_labels()
+        ) | self.body.get_labels(scope)
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/JumpAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/JumpAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,11 +84,11 @@
             and self.label_name_token == other.label_name_token
             and self.condition == other.condition
         )
 
     def __repr__(self):
         return f"JUMP({self.label_name_token.text}{'' if self.condition is None else ', IF '+repr(self.condition)})"
 
-    def copy(self) -> "JumpAssembly":
-        return JumpAssembly(
+    def copy(self) -> "AbstractJumpAssembly":
+        return type(self)(
             self.label_name_token, self.condition.copy() if self.condition else None
         )
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LabelAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LabelAssembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import typing
 
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.MutableFunction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.Opcodes import Opcodes
 
@@ -14,32 +16,35 @@
 @Parser.register
 class LabelAssembly(AbstractAssemblyInstruction):
     # LABEL <name>
     NAME = "LABEL"
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "LabelAssembly":
-        return cls(parser.consume(IdentifierToken))
+        name = parser.try_parse_identifier_like()
 
-    def __init__(self, name_token: IdentifierToken | str):
-        self.name_token = (
-            name_token
-            if isinstance(name_token, IdentifierToken)
-            else IdentifierToken(name_token)
-        )
+        if name is None:
+            raise throw_positioned_syntax_error(
+                scope, parser[0], "expected <identifier like>"
+            )
+
+        return cls(name)
+
+    def __init__(self, name: IIdentifierAccessor | str):
+        self.name = name if not isinstance(name, str) else StaticIdentifier(name)
 
     def __repr__(self):
-        return f"LABEL({self.name_token.text})"
+        return f"LABEL({self.name})"
 
     def __eq__(self, other):
-        return type(self) == type(other) and self.name_token == other.name_token
+        return type(self) == type(other) and self.name == other.name
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        return [Instruction(function, -1, Opcodes.BYTECODE_LABEL, self.name_token.text)]
+        return [Instruction(function, -1, Opcodes.BYTECODE_LABEL, self.name(scope))]
 
     def copy(self) -> "LabelAssembly":
-        return type(self)(self.name_token)
+        return type(self)(self.name)
 
-    def get_labels(self) -> typing.Set[str]:
-        return {self.name_token.text}
+    def get_labels(self, scope: ParsingScope) -> typing.Set[StaticIdentifier]:
+        return {StaticIdentifier(self.name(scope))}
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 @Parser.register
 class MacroReturnAssembly(AbstractAssemblyInstruction):
     NAME = "MACRO_RETURN"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "ReturnAssembly":
+    def consume(cls, parser: "Parser", scope) -> "MacroReturnAssembly":
         return cls(
             parser.try_parse_data_source(
                 allow_primitives=True, allow_op=True, include_bracket=False
             )
         )
 
     def __init__(self, expr: AbstractSourceExpression | None = None):
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
 class AbstractRaiseAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # # RAISE [<source>]
+    # RAISE [<source>]
     NAME = "RAISE"
 
     def __init__(self, source):
         self.source = source
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractRaiseAssembly":
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, expr: AbstractSourceExpression | None = None):
         self.expr = expr
 
     @classmethod
     def consume(cls, parser: "Parser", scope) -> "AbstractReturnAssembly":
         return cls(
             parser.try_parse_data_source(
-                allow_primitives=True, allow_op=True, include_bracket=False
+                allow_primitives=True, allow_op=True, include_bracket=False, scope=scope
             )
         )
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/YieldAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,72 +3,90 @@
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # STORE_GLOBAL <name> [<source>]
-    NAME = "STORE_GLOBAL"
+class AbstractYieldAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # YIELD [*] [<expr>] [-> <target>]
+    NAME = "YIELD"
 
     def __init__(
         self,
-        name_token: IdentifierToken | IntegerToken | str | int,
-        source: AbstractSourceExpression | None = None,
+        expr: AbstractSourceExpression | None = None,
+        is_star: bool = False,
+        target: AbstractSourceExpression | None = None,
     ):
-        self.name_token = (
-            name_token
-            if not isinstance(name_token, (str, int))
-            else (
-                IdentifierToken(name_token)
-                if isinstance(name_token, str)
-                else IntegerToken(str(name_token))
-            )
-        )
-        self.source = source
+        self.expr = expr
+        self.is_star = is_star
+        self.target = target
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
-        parser.try_consume(SpecialToken("@"))
-        name = parser.try_consume([IdentifierToken, IntegerToken])
-
-        if name is None:
-            raise throw_positioned_syntax_error(
-                scope, parser.try_inspect(), "expected <name> or <integer>"
-            )
+    def consume(cls, parser: "Parser", scope) -> "AbstractYieldAssembly":
+        is_star = bool(parser.try_consume(SpecialToken("*")))
 
-        source = parser.try_parse_data_source()
+        expr = parser.try_parse_data_source(
+            allow_primitives=True, allow_op=True, include_bracket=False
+        )
 
-        return cls(name, source)
+        if parser.try_consume(SpecialToken("-")) and parser.try_consume(
+            SpecialToken(">")
+        ):
+            target = parser.try_parse_data_source(
+                allow_primitives=True, allow_op=True, include_bracket=False
+            )
 
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.name_token == other.name_token
-            and self.source == other.source
-        )
+            if target is None:
+                raise throw_positioned_syntax_error(
+                    scope, parser.try_inspect(), "expected <expression>"
+                )
 
-    def __repr__(self):
-        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
+        else:
+            target = None
 
-    def copy(self) -> "AbstractStoreGlobalAssembly":
-        return type(self)(self.name_token, self.source.copy() if self.source else None)
+        return cls(expr, is_star, target)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor, []) if self.source else None,)
+            self,
+            (
+                self.expr.visit_parts(visitor, parents + [self]) if self.expr else None,
+                self.target.visit_parts(
+                    visitor,
+                    parents + [self],
+                )
+                if self.target
+                else None,
+            ),
+            parents,
+        )
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.expr == other.expr
+            and self.is_star == other.is_star
+            and self.target == other.target
+        )
+
+    def __repr__(self):
+        return f"YIELD{'' if not self.is_star else '*'}({self.expr if self.expr else ''}{(', ' if self.expr else '->') + repr(self.target) if self.target else ''})"
+
+    def copy(self) -> "AbstractYieldAssembly":
+        return type(self)(
+            self.expr.copy() if self.expr else None,
+            self.is_star,
+            self.target.copy() if self.target else None,
         )
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/WhileAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/IfAssembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,113 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractWhileAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # # WHILE <expression> ['\'' <label name> '\''] '{' <body> '}'
-    NAME = "WHILE"
-
-    def __init__(
-        self,
-        source: AbstractSourceExpression,
-        body: CompoundExpression,
-        label_name: IdentifierToken | str | None = None,
-    ):
-        self.source = source
-        self.body = body
-        self.label_name = (
-            label_name
-            if not isinstance(label_name, str)
-            else IdentifierToken(label_name)
-        )
+class AbstractIFAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # IF <expression> ['\'' <label name> '\''] '{' <body> '}'
+    NAME = "IF"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractWhileAssembly":
-        condition = parser.try_parse_data_source(
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractIFAssembly":
+        source = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False, scope=scope
         )
 
-        if condition is None:
+        if source is None:
             raise throw_positioned_syntax_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         if parser.try_consume(SpecialToken("'")):
-            label_name = parser.consume(IdentifierToken)
+            label_name = parser.parse_identifier_like(scope)
             if not parser.try_consume(SpecialToken("'")):
                 raise throw_positioned_syntax_error(
                     scope, parser.try_inspect(), "expected '"
                 )
         else:
             label_name = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
-            condition,
+            source,
             body,
             label_name,
         )
 
+    def __init__(
+        self,
+        source: AbstractSourceExpression,
+        body: CompoundExpression,
+        label_name: IIdentifierAccessor | str = None,
+    ):
+        self.source = source
+        self.body = body
+        self.label_name = (
+            label_name
+            if not isinstance(label_name, str)
+            else StaticIdentifier(label_name)
+        )
+
     def copy(self):
         return type(self)(self.source.copy(), self.body.copy(), self.label_name)
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.source == other.source
             and self.body == other.body
             and self.label_name == other.label_name
         )
 
     def __repr__(self):
         c = "'"
-        return f"WHILE({self.source}{'' if self.label_name is None else ', label='+c+self.label_name.text+c}) -> {{{self.body}}}"
+        return f"IF({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor), self.body.visit_parts(visitor))
+            self,
+            (
+                self.source.visit_parts(visitor, parents + [self]),
+                self.body.visit_parts(visitor, parents + [self]),
+            ),
+            parents,
         )
 
     def visit_assembly_instructions(
         self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
     ):
         return visitor(self, (self.body.visit_assembly_instructions(visitor),))
 
-    def get_labels(self):
+    def get_labels(self, scope: ParsingScope) -> typing.Set[str]:
         return (
             set()
             if self.label_name is None
             else {
-                self.label_name.text,
-                self.label_name.text + "_END",
-                self.label_name.text + "_INNER",
+                self.label_name(scope),
+                self.label_name(scope) + "_END",
+                self.label_name(scope) + "_HEAD",
             }
-        ) | self.body.get_labels()
+        ) | self.body.get_labels(scope)
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/assembly_instructions.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/assembly_instructions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,17 @@
     MacroAssembly,
     MacroPasteAssembly,
     NamespaceAssembly,
     MacroImportAssembly,
     LoadAssembly,
     StoreAssembly,
     MacroReturnAssembly,
+    RawAssembly,
 )
-from bytecodemanipulation.data.v3_10.instructions import (
+from bytecodemanipulation.data.v3_11.instructions import (
     CallAssembly,
     ClassDefinitionAssembly,
     ForEachAssembly,
     FunctionDefinitionAssembly,
     IfAssembly,
     JumpAssembly,
     LoadConstAssembly,
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 
 @Parser.register
 class ClassDefinitionAssembly(AbstractClassDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        inner_scope = scope.copy(sub_scope_name=self.name_token.text)
+        inner_scope = scope.copy(sub_scope_name=self.name(scope))
 
         target = MutableFunction(lambda: None)
 
         inner_bytecode = [
             Instruction(target, -1, Opcodes.LOAD_NAME, "__name__"),
             Instruction(target, -1, Opcodes.STORE_NAME, "__module__"),
-            Instruction(target, -1, Opcodes.LOAD_CONST, self.name_token.text),
+            Instruction(target, -1, Opcodes.LOAD_CONST, self.name(scope)),
             Instruction(target, -1, Opcodes.STORE_NAME, "__qualname__"),
         ]
 
         raw_inner_code = self.code_block.emit_bytecodes(target, inner_scope)
 
         for instr in raw_inner_code:
             if instr.opcode == Opcodes.LOAD_FAST:
@@ -48,23 +48,23 @@
         target.reassign_to_function()
 
         code_obj = target.target.__code__
 
         bytecode = [
             Instruction(function, -1, Opcodes.LOAD_BUILD_CLASS),
             Instruction(function, -1, Opcodes.LOAD_CONST, code_obj),
-            Instruction(function, -1, Opcodes.LOAD_CONST, self.name_token.text),
+            Instruction(function, -1, Opcodes.LOAD_CONST, self.name(scope)),
             Instruction(function, -1, Opcodes.MAKE_FUNCTION, arg=0),
-            Instruction(function, -1, Opcodes.LOAD_CONST, self.name_token.text),
+            Instruction(function, -1, Opcodes.LOAD_CONST, self.name(scope)),
         ]
 
         for parent in self.parents:
             bytecode += parent.emit_bytecodes(
                 function,
                 scope,
             )
 
         bytecode += [
             Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2 + len(self.parents)),
-            Instruction(function, -1, Opcodes.STORE_FAST, self.name_token.text),
+            Instruction(function, -1, Opcodes.STORE_FAST, self.name(scope)),
         ]
         return bytecode
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class FunctionDefinitionAssembly(AbstractFunctionDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         flags = 0
         bytecode = []
 
-        inner_labels = self.body.collect_label_info()
+        inner_labels = self.body.collect_label_info(scope)
         label_targets = {}
 
         inner_scope = scope.copy()
 
         if self.bound_variables:
             if any(map(lambda e: e[1], self.bound_variables)):
                 raise NotImplementedError("Static variables")
@@ -42,15 +42,15 @@
             tar = lambda: None
 
         target = MutableFunction(tar)
         inner_bytecode = []
 
         if self.bound_variables:
             for name, is_static in self.bound_variables:
-                print(name, name(scope), is_static)
+                # print(name, name(scope), is_static)
                 inner_bytecode += [
                     Instruction(target, -1, Opcodes.LOAD_DEREF, name(scope) + "%inner"),
                     Instruction(target, -1, Opcodes.STORE_DEREF, name(scope)),
                 ]
 
         inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
         inner_bytecode[-1].next_instruction = target.instructions[0]
@@ -118,20 +118,20 @@
 
         bytecode += [
             Instruction(function, -1, "LOAD_CONST", code_object),
             Instruction(
                 function,
                 -1,
                 "LOAD_CONST",
-                self.func_name.text if self.func_name else "<lambda>",
+                self.func_name(scope) if self.func_name else "<lambda>",
             ),
             Instruction(function, -1, "MAKE_FUNCTION", arg=flags),
         ]
 
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
         else:
             bytecode += [
-                Instruction(function, -1, Opcodes.STORE_FAST, self.func_name.text),
+                Instruction(function, -1, Opcodes.STORE_FAST, self.func_name(scope)),
             ]
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/data_loader.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/data_loader.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/mixin_util.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/mixin_util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/optimiser_util.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/optimiser_util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation/util.py` & `bytecodemanipulation-0.2.9/bytecodemanipulation/util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/PKG-INFO` & `bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.2.8
+Version: 0.2.9
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,25 +13,25 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyBytecodeManipulator
-A high level cross-version python bytecode manipulation library build ontop 
-of 'dis' and 'inspect' 
+A high level cross-version python bytecode manipulation library build ontop
+of 'dis' and 'inspect'
 
-Supports code inlining, branch removing and arbitrary code injection into 
+Supports code inlining, branch removing and arbitrary code injection into
 existing functions.
 
-WARNING: using bytecode manipulation on a so low level as we do can break 
-the python runtime at any point without a warning. We circumvent a lot of 
-safety checks normally done. 
+WARNING: using bytecode manipulation on a so low level as we do can break
+the python runtime at any point without a warning. We circumvent a lot of
+safety checks normally done.
 
-WARNING: We cannot make sure that everything works as it should, expect broken code 
+WARNING: We cannot make sure that everything works as it should, expect broken code
 at runtime!
 
 
 Supported python versions:
 
 - 3.10 (main development)
 - 3.11.0[b3] (forward porting; WIP; Currently not working)
@@ -39,92 +39,129 @@
 Other versions will not work as a lot of config is stored in .json files per-version,
 so you may need to provide your own .json config files for the version you need.
 
 (Some versions might be plug-and-play, but most will require code changes additionally)
 
 ## Why are there so many print()-s?
 
-Due to the breaking nature of anything this code touches, and the absents of any traces 
-in the function itself, we decided to add a lot of "debug" statements indicating 
-mostly the who-has-done-what-to-which-method for the runtime. 
+Due to the breaking nature of anything this code touches, and the absents of any traces
+in the function itself, we decided to add a lot of "debug" statements indicating
+mostly the who-has-done-what-to-which-method for the runtime.
 This makes debugging broken code easier, as it is more clear what happened to each transformed function.
 
 If you want them removed, create your own Fork of this and remove them, on your own risk.
 
-We may use in the future the logging library, so you can disable our logger instance, but we 
+We may use in the future the logging library, so you can disable our logger instance, but we
 are currently in an inter-stage of the code, so other stuff has priority.
 
-## Compatibility with other libraries 
+## Compatibility with other libraries
 
-- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
+- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute
   we modify
 - Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
   results which might contain internal instructions
 
 
-## Debugging your injections 
+## Debugging your injections
 
 There is the possibility to "debug" functions using the execution emulator.
 It will be able to give you more information about a crash than the python core interpreter,
-but will be a lot slower than it. 
+but will be a lot slower than it.
 
-It comes also with the possibility to run your bytecode in another interpreter version, so 
+It comes also with the possibility to run your bytecode in another interpreter version, so
 you can experiment with some stuff.
-In theory, it is also possible to run in python versions not supported by the 
+In theory, it is also possible to run in python versions not supported by the
 bytecode manipulation system, but it is not recommended.
 
 TransformationHandler() takes as an arg debug_code and debug_further_calls
-for activating it for all accessed methods. 
+for activating it for all accessed methods.
 
-BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
+BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on
 that exact method.
 
 
 # Examples
 
-TODO
+Replacing global access with constant value
 
+```python
+from bytecodemanipulation.Optimiser import cache_global_name, apply_now
+
+@cache_global_name("min", lambda: min)
+def test(x, y):
+    return min(x, y)
+
+apply_now(test)
+```
+
+Inlining method calls
+
+```python
+from bytecodemanipulation.Optimiser import cache_global_name, inline_calls, apply_now
+
+@inline_calls
+def call(a, b):
+    return a + b
+
+@cache_global_name("call", lambda: call)
+def test(x, y):
+    return call(x, y)
+
+apply_now(test)
+```
+
+will result in bytecode which could be represented with:
+
+```python
+def test(x, y):
+    return x + y
+```
+
+(there might be extra local variables generated for parameters)
 
 # Applied Optimisations
 
 - Constant Expression inlining (can be declared for custom functions to be constant)
 - LOAD_GLOBAL for builtins (if enabled)
 - standard library inlining (if enabled)
 - specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
 - branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
-- local variable elimination
+- local variable elimination (TODO: add more cases)
 
 
 # Currently Limitations
 
 - Line Numbers get mixed up, we need some way to assign meaningful line numbers
-- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
+- With python 3.11, exception table exists, and this breaks our current concept of one big flow diagram,
   as exception handling code might exist outside the default flow
-- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
-- Method inlining is not working properly and needs a lot more testing
+- Also python 3.11 introduces CACHE-s for instructions, which will require some work in order to work
+- During optimization, a lot of stuff is being recomputed each optimization pass, we need to cache that drastically
+- Method inlining is not working properly and needs a lot more testing (WIP)
 - If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
   inline method accesses for further optimisation
 - Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
   parent instruction, using the arg to switch between modes
 
 
 # Assembly Code
 
 - The library provides also a way to use some "python-assembly" for writing code
 - This is only python bytecode, so no fancy stuff can be done
 - See ASSEMBLY.md for more information on instructions
 - We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
 - You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
+    - assembly(\<code>) can be used for inline assembly
+    - this also includes macro, which may be also created from python-defined methods
 
 
-## Code Formatting
+# Code Formatting
 
 We use the python formatting library "black" on our code
 
 # TODO's
 
 - abstract opcode affect away into a .json file describing all opcodes
 - create a json file for defining certain bytecode sequences
 - write more library-specific optimisations
 - write generating bytecode system for emulator, constructing a function pointing to the
-.json file for exception printing, and optimizing wherever possible
+  .json file for exception printing, and optimizing wherever possible
```

### Comparing `bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/SOURCES.txt` & `bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 bytecodemanipulation/Emulator.py
 bytecodemanipulation/Mixin.py
 bytecodemanipulation/MutableFunction.py
 bytecodemanipulation/MutableFunctionHelpers.py
 bytecodemanipulation/Opcodes.py
 bytecodemanipulation/Optimiser.py
 bytecodemanipulation/Specialization.py
+bytecodemanipulation/TypeEnforcer.py
 bytecodemanipulation/__init__.py
 bytecodemanipulation/annotated_std.py
 bytecodemanipulation/compiler.py
 bytecodemanipulation/data_loader.py
 bytecodemanipulation/mixin_util.py
 bytecodemanipulation/optimise_self.py
 bytecodemanipulation/optimiser_util.py
@@ -49,14 +50,15 @@
 bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
 bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
 bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
 bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
 bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
 bytecodemanipulation/data/shared/expressions/__init__.py
 bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
+bytecodemanipulation/data/shared/instructions/AssertAssembly.py
 bytecodemanipulation/data/shared/instructions/CallAssembly.py
 bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
 bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
 bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
 bytecodemanipulation/data/shared/instructions/IfAssembly.py
 bytecodemanipulation/data/shared/instructions/JumpAssembly.py
 bytecodemanipulation/data/shared/instructions/LabelAssembly.py
@@ -69,24 +71,26 @@
 bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
 bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
 bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
 bytecodemanipulation/data/shared/instructions/OpAssembly.py
 bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
 bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
 bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
+bytecodemanipulation/data/shared/instructions/RawAssembly.py
 bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
 bytecodemanipulation/data/shared/instructions/StoreAssembly.py
 bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
 bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
 bytecodemanipulation/data/shared/instructions/WhileAssembly.py
 bytecodemanipulation/data/shared/instructions/YieldAssembly.py
 bytecodemanipulation/data/shared/instructions/__init__.py
 bytecodemanipulation/data/v3_10/__init__.py
 bytecodemanipulation/data/v3_10/assembly_instructions.py
 bytecodemanipulation/data/v3_10/specialize.py
+bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
 bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
 bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
 bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
 bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
 bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
 bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
 bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
@@ -98,15 +102,36 @@
 bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
 bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
 bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
 bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
 bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
 bytecodemanipulation/data/v3_10/instructions/__init__.py
 bytecodemanipulation/data/v3_11/__init__.py
+bytecodemanipulation/data/v3_11/assembly_instructions.py
 bytecodemanipulation/data/v3_11/specialize.py
+bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
+bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
+bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
+bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
+bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
+bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
+bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
+bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
+bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
+bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
+bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
+bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
+bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
+bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
+bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
+bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
+bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
+bytecodemanipulation/data/v3_11/instructions/__init__.py
 tests/test_Assembly.py
+tests/test_InlineSystem.py
 tests/test_Mixin.py
 tests/test_MutableFunction.py
-tests/test_MutableFunctionHelper.py
+tests/test_Operators.py
+tests/test_Optimiser.py
+tests/test_Specializations.py
 tests/test_StandardLibrary.py
-tests/test_issues.py
-tests/test_optimiser_util.py
+tests/test_issues.py
```

### Comparing `bytecodemanipulation-0.2.8/setup.py` & `bytecodemanipulation-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="bytecodemanipulation",
-    version="0.2.8",
+    version="0.2.9",
     author="uuk",
     author_email="uuk1301@gmail.com",
     description="High level python bytecode manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uuk0/PyBytecodeManipulator",
     project_urls={
```

### Comparing `bytecodemanipulation-0.2.8/tests/test_Assembly.py` & `bytecodemanipulation-0.2.9/tests/test_Assembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,58 @@
+import dis
 import functools
 import itertools
 from unittest import TestCase
 
 import bytecodemanipulation.data_loader
 from bytecodemanipulation.data.shared.instructions.LabelAssembly import LabelAssembly
 from bytecodemanipulation.data.shared.instructions.PythonCodeAssembly import (
     PythonCodeAssembly,
 )
 
 from bytecodemanipulation.data.shared.instructions.FunctionDefinitionAssembly import (
     AbstractFunctionDefinitionAssembly,
 )
 from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
-from bytecodemanipulation.data.shared.instructions.JumpAssembly import AbstractJumpAssembly
+from bytecodemanipulation.data.shared.instructions.JumpAssembly import (
+    AbstractJumpAssembly,
+)
 from bytecodemanipulation.data.shared.instructions.LoadAssembly import LoadAssembly
 from bytecodemanipulation.data.shared.instructions.LoadConstAssembly import (
     AbstractLoadConstAssembly,
 )
 from bytecodemanipulation.data.shared.instructions.LoadFastAssembly import (
     AbstractLoadFastAssembly,
 )
 from bytecodemanipulation.data.shared.instructions.LoadGlobalAssembly import (
     AbstractLoadGlobalAssembly,
 )
 from bytecodemanipulation.data.shared.instructions.PopElementAssembly import (
     AbstractPopElementAssembly,
 )
-from bytecodemanipulation.data.shared.instructions.ReturnAssembly import AbstractReturnAssembly
+from bytecodemanipulation.data.shared.instructions.ReturnAssembly import (
+    AbstractReturnAssembly,
+)
 from bytecodemanipulation.data.shared.instructions.StoreAssembly import StoreAssembly
 from bytecodemanipulation.data.shared.instructions.StoreFastAssembly import (
     AbstractStoreFastAssembly,
 )
 from bytecodemanipulation.data.shared.instructions.StoreGlobalAssembly import (
     AbstractStoreGlobalAssembly,
 )
-from bytecodemanipulation.data.shared.instructions.WhileAssembly import AbstractWhileAssembly
-from bytecodemanipulation.data.shared.instructions.YieldAssembly import AbstractYieldAssembly
+from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
+    AbstractWhileAssembly,
+)
+from bytecodemanipulation.data.shared.instructions.YieldAssembly import (
+    AbstractYieldAssembly,
+)
 from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
-from bytecodemanipulation.data.shared.instructions.CallAssembly import AbstractCallAssembly
+from bytecodemanipulation.data.shared.instructions.CallAssembly import (
+    AbstractCallAssembly,
+)
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 bytecodemanipulation.data_loader.INIT_ASSEMBLY = False
 from bytecodemanipulation.assembler.Parser import *
 from bytecodemanipulation.assembler.target import (
     assembly,
     label,
@@ -58,28 +69,31 @@
     from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 
 bytecodemanipulation.data_loader.load_assembly_instructions()
 
 if typing.TYPE_CHECKING:
     pass
 
-from tests.test_issues import compare_optimized_results
+from tests.util import compare_optimized_results
 from bytecodemanipulation.Optimiser import cache_global_name, _OptimisationContainer
 
 
 if bytecodemanipulation.data_loader.version == "3_10":
     import bytecodemanipulation.data.v3_10.assembly_instructions
 elif bytecodemanipulation.data_loader.version == "3_11":
     import bytecodemanipulation.data.v3_11.assembly_instructions
 else:
     raise RuntimeError(
         f"Found not supported version: '{bytecodemanipulation.data_loader.version}'"
     )
 
 
+from bytecodemanipulation.assembler.target import apply_operations
+
+
 GLOBAL = None
 
 
 class TestParser(TestCase):
     def assertEqualList(
         self, correct: CompoundExpression, to_check: CompoundExpression
     ):
@@ -116,15 +130,17 @@
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractLoadGlobalAssembly.IMPLEMENTATION("test"),
                     AbstractLoadGlobalAssembly.IMPLEMENTATION(10),
                     AbstractLoadGlobalAssembly.IMPLEMENTATION("test"),
                     AbstractLoadGlobalAssembly.IMPLEMENTATION(10),
-                    AbstractLoadGlobalAssembly.IMPLEMENTATION("hello", LocalAccessExpression("test")),
+                    AbstractLoadGlobalAssembly.IMPLEMENTATION(
+                        "hello", LocalAccessExpression("test")
+                    ),
                 ]
             ),
             expr,
         )
 
     def test_store_global(self):
         expr = Parser(
@@ -140,15 +156,17 @@
                         "test",
                         GlobalAccessExpression("test"),
                     ),
                     AbstractStoreGlobalAssembly.IMPLEMENTATION(
                         "test",
                         LocalAccessExpression("test"),
                     ),
-                    AbstractStoreGlobalAssembly.IMPLEMENTATION("test", TopOfStackAccessExpression()),
+                    AbstractStoreGlobalAssembly.IMPLEMENTATION(
+                        "test", TopOfStackAccessExpression()
+                    ),
                 ]
             ),
             expr,
         )
 
     def test_load_fast(self):
         expr = Parser(
@@ -158,15 +176,17 @@
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractLoadFastAssembly.IMPLEMENTATION("test"),
                     AbstractLoadFastAssembly.IMPLEMENTATION(10),
                     AbstractLoadFastAssembly.IMPLEMENTATION("test"),
                     AbstractLoadFastAssembly.IMPLEMENTATION(10),
-                    AbstractLoadFastAssembly.IMPLEMENTATION("test", GlobalAccessExpression("test")),
+                    AbstractLoadFastAssembly.IMPLEMENTATION(
+                        "test", GlobalAccessExpression("test")
+                    ),
                 ]
             ),
             expr,
         )
 
     def test_store_fast(self):
         expr = Parser(
@@ -174,17 +194,23 @@
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractStoreFastAssembly.IMPLEMENTATION("test"),
                     AbstractStoreFastAssembly.IMPLEMENTATION("test"),
-                    AbstractStoreFastAssembly.IMPLEMENTATION("test", GlobalAccessExpression("test")),
-                    AbstractStoreFastAssembly.IMPLEMENTATION("test", LocalAccessExpression("test")),
-                    AbstractStoreFastAssembly.IMPLEMENTATION("test", TopOfStackAccessExpression()),
+                    AbstractStoreFastAssembly.IMPLEMENTATION(
+                        "test", GlobalAccessExpression("test")
+                    ),
+                    AbstractStoreFastAssembly.IMPLEMENTATION(
+                        "test", LocalAccessExpression("test")
+                    ),
+                    AbstractStoreFastAssembly.IMPLEMENTATION(
+                        "test", TopOfStackAccessExpression()
+                    ),
                 ]
             ),
             expr,
         )
 
     def test_load_const(self):
         expr = Parser(
@@ -192,16 +218,20 @@
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractLoadConstAssembly.IMPLEMENTATION(10),
                     AbstractLoadConstAssembly.IMPLEMENTATION("Hello World!"),
-                    AbstractLoadConstAssembly.IMPLEMENTATION(10, GlobalAccessExpression("test")),
-                    AbstractLoadConstAssembly.IMPLEMENTATION(GlobalAccessExpression("global")),
+                    AbstractLoadConstAssembly.IMPLEMENTATION(
+                        10, GlobalAccessExpression("test")
+                    ),
+                    AbstractLoadConstAssembly.IMPLEMENTATION(
+                        GlobalAccessExpression("global")
+                    ),
                     AbstractLoadConstAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("global"), LocalAccessExpression("test")
                     ),
                 ]
             ),
             expr,
         )
@@ -303,25 +333,35 @@
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractCallAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("print"),
-                        [AbstractCallAssembly.Arg(ConstantAccessExpression("Hello World!"))],
+                        [
+                            AbstractCallAssembly.Arg(
+                                ConstantAccessExpression("Hello World!")
+                            )
+                        ],
                     ),
                     AbstractCallAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("print"),
-                        [AbstractCallAssembly.Arg(ConstantAccessExpression("Hello World!"))],
+                        [
+                            AbstractCallAssembly.Arg(
+                                ConstantAccessExpression("Hello World!")
+                            )
+                        ],
                         LocalAccessExpression("result"),
                     ),
                     AbstractCallAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("print"),
                         [
-                            AbstractCallAssembly.Arg(ConstantAccessExpression("Hello World!")),
+                            AbstractCallAssembly.Arg(
+                                ConstantAccessExpression("Hello World!")
+                            ),
                             AbstractCallAssembly.Arg(ConstantAccessExpression("test")),
                         ],
                         LocalAccessExpression("result"),
                     ),
                     AbstractCallAssembly.IMPLEMENTATION(
                         SubscriptionAccessExpression(
                             LocalAccessExpression("print"),
@@ -331,34 +371,42 @@
                             AbstractCallAssembly.Arg(GlobalAccessExpression("test")),
                             AbstractCallAssembly.Arg(GlobalAccessExpression("hello")),
                         ],
                         TopOfStackAccessExpression(),
                     ),
                     AbstractCallAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("test"),
-                        [AbstractCallAssembly.KwArg("key", GlobalAccessExpression("value"))],
+                        [
+                            AbstractCallAssembly.KwArg(
+                                "key", GlobalAccessExpression("value")
+                            )
+                        ],
                         GlobalAccessExpression("result"),
                     ),
                     AbstractCallAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("test"),
                         [
                             AbstractCallAssembly.Arg(LocalAccessExpression("direct")),
-                            AbstractCallAssembly.KwArg("key", GlobalAccessExpression("value")),
+                            AbstractCallAssembly.KwArg(
+                                "key", GlobalAccessExpression("value")
+                            ),
                         ],
                         GlobalAccessExpression("result"),
                     ),
                     AbstractCallAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("test"),
                         [
                             AbstractCallAssembly.Arg(
                                 AttributeAccessExpression(
                                     LocalAccessExpression("direct"), "test"
                                 )
                             ),
-                            AbstractCallAssembly.KwArg("key", GlobalAccessExpression("value")),
+                            AbstractCallAssembly.KwArg(
+                                "key", GlobalAccessExpression("value")
+                            ),
                         ],
                         GlobalAccessExpression("result"),
                     ),
                     AbstractCallAssembly.IMPLEMENTATION(
                         AttributeAccessExpression(GlobalAccessExpression("test"), "x"),
                         [
                             AbstractCallAssembly.StarArg(LocalAccessExpression("x")),
@@ -381,27 +429,29 @@
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractOpAssembly.IMPLEMENTATION(
                         AbstractOpAssembly.BinaryOperation(
                             GlobalAccessExpression("lhs"),
                             "+",
+                            [SpecialToken("+")],
                             GlobalAccessExpression("rhs"),
                         ),
                         GlobalAccessExpression("result"),
                     ),
                     AbstractOpAssembly.IMPLEMENTATION(
                         AbstractOpAssembly.BinaryOperation(
                             SubscriptionAccessExpression(
                                 GlobalAccessExpression("lhs"),
                                 AttributeAccessExpression(
                                     LocalAccessExpression("local"), "attr"
                                 ),
                             ),
                             "**",
+                            [SpecialToken("*"), SpecialToken("*")],
                             GlobalAccessExpression("rhs"),
                         )
                     ),
                 ]
             ),
             expr,
         )
@@ -422,33 +472,41 @@
     def test_return(self):
         expr = Parser("RETURN\nRETURN @global").parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractReturnAssembly.IMPLEMENTATION(),
-                    AbstractReturnAssembly.IMPLEMENTATION(GlobalAccessExpression("global")),
+                    AbstractReturnAssembly.IMPLEMENTATION(
+                        GlobalAccessExpression("global")
+                    ),
                 ]
             ),
             expr,
         )
 
     def test_yield(self):
         expr = Parser(
             "YIELD\nYIELD @global\nYIELD *\nYIELD* $local\nYIELD -> %\nYIELD @global -> $local\n YIELD* -> @global\nYIELD* @global -> $local"
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractYieldAssembly.IMPLEMENTATION(),
-                    AbstractYieldAssembly.IMPLEMENTATION(GlobalAccessExpression("global")),
+                    AbstractYieldAssembly.IMPLEMENTATION(
+                        GlobalAccessExpression("global")
+                    ),
                     AbstractYieldAssembly.IMPLEMENTATION(is_star=True),
-                    AbstractYieldAssembly.IMPLEMENTATION(LocalAccessExpression("local"), is_star=True),
-                    AbstractYieldAssembly.IMPLEMENTATION(target=TopOfStackAccessExpression()),
+                    AbstractYieldAssembly.IMPLEMENTATION(
+                        LocalAccessExpression("local"), is_star=True
+                    ),
+                    AbstractYieldAssembly.IMPLEMENTATION(
+                        target=TopOfStackAccessExpression()
+                    ),
                     AbstractYieldAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("global"),
                         target=LocalAccessExpression("local"),
                     ),
                     AbstractYieldAssembly.IMPLEMENTATION(
                         is_star=True, target=GlobalAccessExpression("global")
                     ),
@@ -497,24 +555,27 @@
                         ),
                     ),
                     AbstractIFAssembly.IMPLEMENTATION(
                         AbstractOpAssembly.IMPLEMENTATION(
                             AbstractOpAssembly.BinaryOperation(
                                 LocalAccessExpression("a"),
                                 "==",
+                                [SpecialToken("="), SpecialToken("=")],
                                 LocalAccessExpression("b"),
                             )
                         ),
                         CompoundExpression(
                             [StoreAssembly(GlobalAccessExpression("global"))]
                         ),
                     ),
                     AbstractIFAssembly.IMPLEMENTATION(
                         GlobalAccessExpression("global"),
-                        CompoundExpression([AbstractJumpAssembly.IMPLEMENTATION("test")]),
+                        CompoundExpression(
+                            [AbstractJumpAssembly.IMPLEMENTATION("test")]
+                        ),
                         "test",
                     ),
                 ]
             ),
             expr,
         )
 
@@ -552,14 +613,15 @@
                         ),
                     ),
                     AbstractWhileAssembly.IMPLEMENTATION(
                         AbstractOpAssembly.IMPLEMENTATION(
                             AbstractOpAssembly.BinaryOperation(
                                 LocalAccessExpression("a"),
                                 "==",
+                                [SpecialToken("="), SpecialToken("=")],
                                 LocalAccessExpression("b"),
                             )
                         ),
                         CompoundExpression(
                             [StoreAssembly(GlobalAccessExpression("global"))]
                         ),
                     ),
@@ -581,42 +643,49 @@
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
                     LabelAssembly("test"),
                     AbstractJumpAssembly.IMPLEMENTATION("test"),
-                    AbstractJumpAssembly.IMPLEMENTATION("test", GlobalAccessExpression("global")),
+                    AbstractJumpAssembly.IMPLEMENTATION(
+                        "test", GlobalAccessExpression("global")
+                    ),
                     AbstractJumpAssembly.IMPLEMENTATION(
                         "test",
                         AbstractOpAssembly.IMPLEMENTATION(
                             AbstractOpAssembly.BinaryOperation(
                                 GlobalAccessExpression("a"),
                                 "==",
+                                [SpecialToken("="), SpecialToken("=")],
                                 GlobalAccessExpression("b"),
                             )
                         ),
                     ),
-                    AbstractJumpAssembly.IMPLEMENTATION("test", GlobalAccessExpression("global")),
+                    AbstractJumpAssembly.IMPLEMENTATION(
+                        "test", GlobalAccessExpression("global")
+                    ),
                     AbstractJumpAssembly.IMPLEMENTATION(
                         "test",
                         AbstractOpAssembly.IMPLEMENTATION(
                             AbstractOpAssembly.BinaryOperation(
                                 GlobalAccessExpression("a"),
                                 "==",
+                                [SpecialToken("="), SpecialToken("=")],
                                 GlobalAccessExpression("b"),
                             )
                         ),
                     ),
                     AbstractJumpAssembly.IMPLEMENTATION(
                         "test",
                         AbstractOpAssembly.IMPLEMENTATION(
                             AbstractOpAssembly.BinaryOperation(
                                 GlobalAccessExpression("a"),
                                 "==",
+                                [SpecialToken("="), SpecialToken("=")],
                                 GlobalAccessExpression("b"),
                             )
                         ),
                     ),
                 ]
             ),
             expr,
@@ -635,15 +704,17 @@
 DEF test <test> () -> @target {}
 """
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
-                    AbstractFunctionDefinitionAssembly.IMPLEMENTATION("test", [], [], CompoundExpression([])),
+                    AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
+                        "test", [], [], CompoundExpression([])
+                    ),
                     AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
                         "test", ["test"], [], CompoundExpression([])
                     ),
                     AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
                         "test", [("test", True)], [], CompoundExpression([])
                     ),
                     AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
@@ -900,152 +971,28 @@
         bytecodemanipulation.assembler.hook.hook()
 
         code = "import tests.test\nself.assertEqual(10, tests.test.test)"
         exec(code, {"self": self})
 
         bytecodemanipulation.assembler.hook.unhook()
 
-    def test_walrus_assigment(self):
-        def target():
-            assembly(
-                """
-OP $local := 10
-STORE $test
-RETURN OP ($local + $test)
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        def compare():
-            test = (local := 10)
-            return local + test
-
-        compare_optimized_results(self, target, compare, opt_ideal=0)
-
     def test_dynamic_attribute_access(self):
         def target(t):
             assembly(
                 """
 RETURN $t.("test_dynamic_attribute_access")
 """
             )
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(self), self.test_dynamic_attribute_access)
 
-    def test_isinstance_check(self):
-        def target():
-            assembly(
-                """
-RETURN OP (10 isinstance @int)
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertTrue(target())
-
-    def test_not_isinstance_check(self):
-        def target():
-            assembly(
-                """
-RETURN OP (10 isinstance @float)
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        # dis.dis(target)
-
-        self.assertFalse(target())
-
-    def test_issubclass_check(self):
-        def target():
-            assembly(
-                """
-RETURN OP (@int issubclass @object)
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertTrue(target())
-
-    def test_not_issubclass_check(self):
-        def target():
-            assembly(
-                """
-RETURN OP (@int issubclass @float)
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        # dis.dis(target)
-
-        self.assertFalse(target())
-
-    def test_hasattr_check(self):
-        def target(t):
-            assembly(
-                """
-RETURN OP ($t hasattr "test_hasattr_check")
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertTrue(target(self))
-
-    def test_not_hasattr_check(self):
-        def target(t):
-            assembly(
-                """
-RETURN OP ($t hasattr "no attr")
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        # dis.dis(target)
-
-        self.assertFalse(target(self))
-
-    def test_getattr_check(self):
-        def target(t):
-            assembly(
-                """
-RETURN OP ($t getattr "test_getattr_check")
-"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertEqual(target(self), self.test_getattr_check)
-
 
 class TestMacro(TestCase):
     def test_basic(self):
         def target():
             assembly(
                 """
     LOAD 1 -> $x
@@ -1485,15 +1432,15 @@
         cls = target()
         self.assertEqual(cls.test(), 42)
 
     def test_class_assembly_namespace_macro(self):
         def target():
             assembly(
                 """
-CLASS test
+CLASS test<test>
 {
     MACRO test_macro()
     {
         RETURN 1
     }
 }
 
@@ -1646,14 +1593,16 @@
             )
             return result
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
+        # dis.dis(target)
+
         self.assertEqual(target(), [1, 2, 3, 4])
 
     def test_for_loop_double(self):
         def target():
             iterable = [0, 1, 2, 3]
             iterable_2 = [1, 2, 3, 4]
             result = []
@@ -1689,7 +1638,72 @@
             return result
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), [0, 0, 1, 2])
+
+    def test_raw_assembly_by_id(self):
+        def target():
+            assembly(
+                """
+LOAD 10
+LOAD 5
+RAW 2
+RETURN %
+"""
+            )
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertEqual(target(), 10)
+
+    def test_raw_assembly_by_name(self):
+        def target():
+            assembly(
+                """
+LOAD 10
+LOAD 5
+RAW ROT_TWO
+RETURN %
+"""
+            )
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertEqual(target(), 10)
+
+    def test_assert(self):
+        @apply_operations
+        def target(x):
+            assembly(
+                """
+ASSERT $x
+"""
+            )
+
+        target(1)
+        self.assertRaises(AssertionError, lambda: target(0))
+
+    def test_assert_with_message(self):
+        @apply_operations
+        def target(x):
+            assembly(
+                """
+ASSERT $x \"Test Message\"
+"""
+            )
+
+        target(1)
+        self.assertRaises(AssertionError, lambda: target(0))
+
+        try:
+            target(0)
+        except AssertionError as e:
+            self.assertEqual(e.args, ("Test Message",))
+        else:
+            self.assertTrue(False)
```

### Comparing `bytecodemanipulation-0.2.8/tests/test_Mixin.py` & `bytecodemanipulation-0.2.9/tests/test_Mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import dis
 import unittest
 from unittest import TestCase
 
 
 from bytecodemanipulation.Mixin import *
-from tests.test_issues import compare_optimized_results
-
+from tests.util import compare_optimized_results
 
 FLAG = False
 
 
 class TestMixinBasic(unittest.TestCase):
     def setUp(self) -> None:
         Mixin._reset()
```

### Comparing `bytecodemanipulation-0.2.8/tests/test_MutableFunction.py` & `bytecodemanipulation-0.2.9/tests/test_MutableFunction.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.8/tests/test_StandardLibrary.py` & `bytecodemanipulation-0.2.9/tests/test_StandardLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,26 +144,30 @@
             data = (0, 1, 2)
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
 std:stream:extend($stream, $data)
+std:print($stream)
 std:stream:filter($stream, $var, {
     OP $var < 2 -> %
 })
+std:print($stream)
 std:stream:to_list($stream, $output)
 """
             )
             return output
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
+        # dis.dis(target)
+
         self.assertEqual(target(), [0, 1])
 
     def test_stream_simple_map(self):
         def target():
             data = (0, 1, 2)
             stream = None
             output = None
```

