# Comparing `tmp/robotcode_language_server-0.36.0.tar.gz` & `tmp/robotcode_language_server-0.37.0.tar.gz`

## Comparing `robotcode_language_server-0.36.0.tar` & `robotcode_language_server-0.37.0.tar`

### file list

```diff
@@ -1,88 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9569 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18989 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    54353 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83638 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15233 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    80255 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/discovering.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19259 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23499 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    40438 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11635 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/pyproject.toml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9569 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18989 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    54707 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    63757 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83638 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15233 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    80441 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    40438 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11635 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/README.md
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/pyproject.toml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/__main__.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from .configuration import RobotConfig
 from .parts.code_action_documentation import RobotCodeActionDocumentationProtocolPart
 from .parts.code_action_fixes import RobotCodeActionFixesProtocolPart
 from .parts.codelens import RobotCodeLensProtocolPart
 from .parts.completion import RobotCompletionProtocolPart
 from .parts.debugging_utils import RobotDebuggingUtilsProtocolPart
 from .parts.diagnostics import RobotDiagnosticsProtocolPart
-from .parts.discovering import DiscoveringProtocolPart
 from .parts.document_highlight import RobotDocumentHighlightProtocolPart
 from .parts.document_symbols import RobotDocumentSymbolsProtocolPart
 from .parts.documents_cache import DocumentsCache
 from .parts.folding_range import RobotFoldingRangeProtocolPart
 from .parts.formatting import RobotFormattingProtocolPart
 from .parts.goto import RobotGotoProtocolPart
 from .parts.hover import RobotHoverProtocolPart
@@ -96,22 +95,21 @@
     robot_rename = ProtocolPartDescriptor(RobotRenameProtocolPart)
     robot_inline_value = ProtocolPartDescriptor(RobotInlineValueProtocolPart)
     robot_inlay_hint = ProtocolPartDescriptor(RobotInlayHintProtocolPart)
     robot_code_action_documentation = ProtocolPartDescriptor(RobotCodeActionDocumentationProtocolPart)
     robot_code_action_fixes = ProtocolPartDescriptor(RobotCodeActionFixesProtocolPart)
     robot_workspace = ProtocolPartDescriptor(RobotWorkspaceProtocolPart)
 
-    robot_discovering = ProtocolPartDescriptor(DiscoveringProtocolPart)
     robot_debugging_utils = ProtocolPartDescriptor(RobotDebuggingUtilsProtocolPart)
 
     name = "RobotCode Language Server"
     short_name = "RobotCode"
     version = __version__
 
-    file_extensions = {"robot", "resource", "py", "yaml", "yml", "feature"}
+    file_extensions = {"robot", "resource", "py", "yaml", "yml"}
 
     languages = [
         LanguageDefinition(
             id="robotframework",
             extensions=[".robot", ".resource"],
             aliases=["Robot Framework", "robotframework"],
         ),
```

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,20 +396,24 @@
 
 
 class _VariablesEntry(_ImportEntry):
     def __init__(
         self,
         name: str,
         args: Tuple[Any, ...],
+        working_dir: str,
+        base_dir: str,
         parent: ImportsManager,
-        get_variables_doc_coroutine: Callable[[], Coroutine[Any, Any, VariablesDoc]],
+        get_variables_doc_coroutine: Callable[[str, Tuple[Any, ...], str, str], Coroutine[Any, Any, VariablesDoc]],
     ) -> None:
         super().__init__(parent)
         self.name = name
         self.args = args
+        self.working_dir = working_dir
+        self.base_dir = base_dir
         self._get_variables_doc_coroutine = get_variables_doc_coroutine
         self._lib_doc: Optional[VariablesDoc] = None
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__qualname__}(name={repr(self.name)}, "
             f"args={repr(self.args)}, file_watchers={repr(self.file_watchers)}, id={repr(id(self))}"
@@ -434,15 +438,15 @@
                     await self._invalidate()
 
                     return change.type
 
             return None
 
     async def _update(self) -> None:
-        self._lib_doc = await self._get_variables_doc_coroutine()
+        self._lib_doc = await self._get_variables_doc_coroutine(self.name, self.args, self.working_dir, self.base_dir)
 
         if self._lib_doc is not None:
             self.file_watchers.append(
                 await self.parent.parent_protocol.workspace.add_file_watchers(
                     self.parent.did_change_watched_files,
                     [str(self._lib_doc.source)],
                 )
@@ -1221,15 +1225,15 @@
     ) -> VariablesDoc:
         source = await self.find_variables(
             name,
             base_dir,
             variables,
         )
 
-        async def _get_libdoc() -> VariablesDoc:
+        async def _get_libdoc(name: str, args: Tuple[Any, ...], working_dir: str, base_dir: str) -> VariablesDoc:
             meta, source = await self.get_variables_meta(
                 name,
                 base_dir,
                 variables,
             )
 
             self._logger.debug(lambda: f"Load variables {source}{repr(args)}")
@@ -1307,15 +1311,17 @@
             self.config.robot.variables if self.config.robot is not None else None,
             variables,
         )
         entry_key = _VariablesEntryKey(source, resolved_args)
 
         async with self._variables_lock:
             if entry_key not in self._variables:
-                self._variables[entry_key] = _VariablesEntry(name, args, self, _get_libdoc)
+                self._variables[entry_key] = _VariablesEntry(
+                    name, resolved_args, str(self.folder.to_path()), base_dir, self, _get_libdoc
+                )
 
         entry = self._variables[entry_key]
 
         if sentinel is not None and sentinel not in entry.references:
             entry.references.add(sentinel)
             weakref.finalize(sentinel, self.__remove_variables_entry, entry_key, entry)
```

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                 self.positional_or_named,
                 self.var_positional,
                 self.named_only,
                 self.var_named,
                 self.defaults,
                 self.types,
             )
-
+        self.__robot_arguments.name = self.name
         resolver = ArgumentResolver(
             self.__robot_arguments,
             resolve_named=resolve_named,
             resolve_variables_until=resolve_variables_until,
             dict_to_kwargs=dict_to_kwargs,
         )
         resolver.resolve(arguments, variables)
```

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,20 +481,24 @@
             if s.name is not None and (s.name_token is None or not position.is_in_range(range_from_token(s.name_token)))
         ]
 
     async def create_settings_completion_items(self, range: Optional[Range]) -> List[CompletionItem]:
         from robot.parsing.lexer.settings import (
             InitFileSettings,
             ResourceFileSettings,
-            TestCaseFileSettings,
         )
 
+        if get_robot_version() >= (6, 1):
+            from robot.parsing.lexer.settings import SuiteFileSettings
+        else:
+            from robot.parsing.lexer.settings import TestCaseFileSettings as SuiteFileSettings
+
         doc_type = await self.parent.documents_cache.get_document_type(self.document)
 
-        settings_class = TestCaseFileSettings
+        settings_class = SuiteFileSettings
         if doc_type == DocumentType.RESOURCE:
             settings_class = ResourceFileSettings
         elif doc_type == DocumentType.INIT:
             settings_class = InitFileSettings
 
         settings = {*settings_class.names, *settings_class.aliases.keys()}
```

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self._default_imports_manager: Optional[ImportsManager] = None
         self._workspace_languages: weakref.WeakKeyDictionary[WorkspaceFolder, Languages] = weakref.WeakKeyDictionary()
 
     async def get_workspace_languages(self, document_or_uri: Union[TextDocument, Uri, str]) -> Optional[Languages]:
         if get_robot_version() < (6, 0):
             return None
 
-        from robot.conf.languages import Languages as RobotLanguages  # pyright: reportMissingImports=false
+        from robot.conf.languages import Languages as RobotLanguages  # pyright: ignore[reportMissingImports]
 
         uri: Union[Uri, str]
 
         if isinstance(document_or_uri, TextDocument):
             uri = document_or_uri.uri
         else:
             uri = document_or_uri
@@ -94,15 +94,15 @@
 
     async def build_languages_from_model(
         self, document: TextDocument, model: ast.AST
     ) -> Tuple[Optional[Languages], Optional[Languages]]:
         if get_robot_version() < (6, 0):
             return (None, None)
 
-        from robot.conf.languages import Languages as RobotLanguages
+        from robot.conf.languages import Languages as RobotLanguages  # pyright: ignore[reportMissingImports]
         from robot.parsing.model.blocks import File
 
         workspace_langs = await self.get_workspace_languages(document)
 
         return (
             cast(
                 Languages,
@@ -294,15 +294,18 @@
 
         def get_tokens(source: str, data_only: bool = False, lang: Any = None) -> Iterator[Token]:
             for t in tokens:
                 check_canceled_sync()
 
                 yield t
 
-        model = _get_model(get_tokens, document.uri.to_path())
+        if get_robot_version() >= (6, 0):
+            model = _get_model(get_tokens, document.uri.to_path(), False, None, None)
+        else:
+            model = _get_model(get_tokens, document.uri.to_path(), False, None)
 
         setattr(model, "source", str(document.uri.to_path()))
         setattr(model, "model_type", document_type)
 
         return cast(ast.AST, model)
 
     async def get_general_model(self, document: TextDocument, data_only: bool = True) -> ast.AST:
```

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,15 +495,15 @@
 
                 try:
                     libdoc = await namespace.get_imported_variables_libdoc(variables_node.name, variables_node.args)
 
                     if libdoc is None or libdoc.errors:
                         libdoc = await namespace.imports_manager.get_libdoc_for_variables_import(
                             str(variables_node.name),
-                            (),
+                            variables_node.args,
                             str(document.uri.to_path().parent),
                             variables=await namespace.get_resolvable_variables(),
                         )
 
                     if libdoc is None or libdoc.errors:
                         return None
```

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.37.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/.gitignore` & `robotcode_language_server-0.37.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/LICENSE.txt` & `robotcode_language_server-0.37.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/README.md` & `robotcode_language_server-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.36.0/pyproject.toml` & `robotcode_language_server-0.37.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.36.0"]
+dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.37.0"]
 dynamic = ["version"]
 
 [project.scripts]
 'robotcode.language_server' = 'robotcode.language_server.__main__:main'
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_language_server-0.36.0/PKG-INFO` & `robotcode_language_server-0.37.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.36.0
+Version: 0.37.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.36.0
+Requires-Dist: robotcode-jsonrpc2==0.37.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

