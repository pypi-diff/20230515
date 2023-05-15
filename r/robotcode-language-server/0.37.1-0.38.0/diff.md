# Comparing `tmp/robotcode_language_server-0.37.1.tar.gz` & `tmp/robotcode_language_server-0.38.0.tar.gz`

## Comparing `robotcode_language_server-0.37.1.tar` & `robotcode_language_server-0.38.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9569 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18989 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    54707 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    63757 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83638 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15233 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    80441 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    40438 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11635 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/pyproject.toml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.37.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    54596 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    63744 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83635 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15233 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    80441 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    40438 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11635 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/README.md
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/__main__.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         await self.on_shutdown(self)
 
     @rpc_method(name="exit")
     @__logger.call
     async def _exit(self, *args: Any, **kwargs: Any) -> None:
         await self.on_exit(self)
 
-        raise SystemExit(0 if self.shutdown_received else 1)
+        exit(0 if self.shutdown_received else 1)
 
     @rpc_method(name="$/setTrace", param_type=SetTraceParams)
     @__logger.call
     async def _set_trace(self, value: TraceValues, *args: Any, **kwargs: Any) -> None:
         self.trace = value
 
     @rpc_method(name="$/cancelRequest", param_type=CancelParams)
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/text_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,20 +105,15 @@
     def version(self, value: Optional[int]) -> None:
         self._version = value
 
     def __str__(self) -> str:  # pragma: no cover
         return self.__repr__()
 
     def __repr__(self) -> str:  # pragma: no cover
-        return (
-            f"TextDocument(uri={repr(self.uri)}, "
-            f"language_id={repr(self.language_id)}, "
-            f"version={repr(self._version)}"
-            f")"
-        )
+        return f"TextDocument(uri={self.uri!r}, language_id={self.language_id!r}, version={self._version!r})"
 
     def text(self) -> str:
         with self._lock:
             return self._text
 
     def save(self, version: Optional[int], text: Optional[str]) -> None:
         self.apply_full_change(version, text, save=True)
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 language_id=language_id or self.detect_language_id(path),
                 text=await self.read_document_text(uri, language_id),
                 version=version,
             )
         except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
             raise
         except BaseException as e:
-            raise CantReadDocumentError(f"Error reading document '{path}': {str(e)}") from e
+            raise CantReadDocumentError(f"Error reading document '{path}': {e!s}") from e
 
     @async_event
     async def on_read_document_text(sender, uri: Uri) -> Optional[str]:  # NOSONAR
         ...
 
     @async_tasking_event
     async def did_append_document(sender, document: TextDocument) -> None:  # NOSONAR
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     async def call_childrens(self, sender: Any, changes: List[FileEvent]) -> None:
         await self.child_callbacks(sender, changes)
 
     def __str__(self) -> str:
         return self.id
 
     def __repr__(self) -> str:
-        return f"{type(self).__qualname__}(id={repr(self.id)}, watchers={repr(self.watchers)})"
+        return f"{type(self).__qualname__}(id={self.id!r}, watchers={self.watchers!r})"
 
 
 class WorkspaceFolder:
     def __init__(self, name: str, uri: Uri, document_uri: DocumentUri) -> None:
         super().__init__()
         self.name = name
         self.uri = uri
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         except RobotCodeError as e:
             raise JsonRPCErrorException(
                 JsonRPCErrors.INTERNAL_ERROR, f"Can't start language server: {e}", InitializeError(retry=False)
             ) from e
 
         self.workspace.did_change_configuration.add(self._on_did_change_configuration)
 
-        self._logger.info(lambda: f"initialized with {repr(self.options)}")
+        self._logger.info(lambda: f"initialized with {self.options!r}")
 
     async def _on_did_change_configuration(self, sender: Any, settings: Dict[str, Any]) -> None:
         pass
 
     async def _on_initialized(self, sender: Any) -> None:
         for folder in self.workspace.workspace_folders:
             config: RobotConfig = await self.workspace.get_configuration(RobotConfig, folder.uri, request=False)
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     def __hash__(self) -> int:
         return hash(self.name)
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(name={repr(self.name)})"
+        return f"{type(self).__name__}(name={self.name!r})"
 
 
 class VariableDefinitionType(Enum):
     VARIABLE = "variable"
     LOCAL_VARIABLE = "local variable"
     ARGUMENT = "argument"
     COMMAND_LINE_VARIABLE = "command line variable"
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,16 +170,16 @@
         self.base_dir = base_dir
         self._get_libdoc_coroutine = get_libdoc_coroutine
         self._lib_doc: Optional[LibraryDoc] = None
         self.ignore_reference = ignore_reference
 
     def __repr__(self) -> str:
         return (
-            f"{type(self).__qualname__}(name={repr(self.name)}, "
-            f"args={repr(self.args)}, file_watchers={repr(self.file_watchers)}, id={repr(id(self))}"
+            f"{type(self).__qualname__}(name={self.name!r}, "
+            f"args={self.args!r}, file_watchers={self.file_watchers!r}, id={id(self)!r}"
         )
 
     async def check_file_changed(self, changes: List[FileEvent]) -> Optional[FileChangeType]:
         async with self._lock:
             if self._lib_doc is None:
                 return None
 
@@ -303,18 +303,15 @@
         super().__init__(parent)
         self.name = name
         self._get_document_coroutine = get_document_coroutine
         self._document: Optional[TextDocument] = None
         self._lib_doc: Optional[LibraryDoc] = None
 
     def __repr__(self) -> str:
-        return (
-            f"{type(self).__qualname__}(name={repr(self.name)}, "
-            f"file_watchers={repr(self.file_watchers)}, id={repr(id(self))}"
-        )
+        return f"{type(self).__qualname__}(name={self.name!r}, file_watchers={self.file_watchers!r}, id={id(self)!r}"
 
     async def check_file_changed(self, changes: List[FileEvent]) -> Optional[FileChangeType]:
         async with self._lock:
             for change in changes:
                 uri = Uri(change.uri)
                 if uri.scheme != "file":
                     continue
@@ -411,16 +408,16 @@
         self.working_dir = working_dir
         self.base_dir = base_dir
         self._get_variables_doc_coroutine = get_variables_doc_coroutine
         self._lib_doc: Optional[VariablesDoc] = None
 
     def __repr__(self) -> str:
         return (
-            f"{type(self).__qualname__}(name={repr(self.name)}, "
-            f"args={repr(self.args)}, file_watchers={repr(self.file_watchers)}, id={repr(id(self))}"
+            f"{type(self).__qualname__}(name={self.name!r}, "
+            f"args={self.args!r}, file_watchers={self.file_watchers!r}, id={id(self)!r}"
         )
 
     async def check_file_changed(self, changes: List[FileEvent]) -> Optional[FileChangeType]:
         async with self._lock:
             if self._lib_doc is None:
                 return None
 
@@ -992,15 +989,15 @@
         async def _get_libdoc(name: str, args: Tuple[Any, ...], working_dir: str, base_dir: str) -> LibraryDoc:
             meta, source = await self.get_library_meta(
                 name,
                 base_dir,
                 variables,
             )
 
-            self._logger.debug(lambda: f"Load Library {source}{repr(args)}")
+            self._logger.debug(lambda: f"Load Library {source}{args!r}")
             if meta is not None:
                 meta_file = Path(self.lib_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
                 if meta_file.exists():
                     try:
                         try:
                             saved_meta = from_json(meta_file.read_text("utf-8"), LibraryMetaData)
                             spec_path = None
@@ -1033,15 +1030,15 @@
                         self.config.robot.variables if self.config.robot is not None else None,
                         variables,
                     ),
                     LOAD_LIBRARY_TIME_OUT,
                 )
 
             if result.stdout:
-                self._logger.warning(lambda: f"stdout captured at loading library {name}{repr(args)}:\n{result.stdout}")
+                self._logger.warning(lambda: f"stdout captured at loading library {name}{args!r}:\n{result.stdout}")
             try:
                 if meta is not None:
                     meta_file = Path(self.lib_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
                     spec_file = Path(self.lib_doc_cache_path, meta.filepath_base.with_suffix(".spec.json"))
                     spec_file.parent.mkdir(parents=True, exist_ok=True)
 
                     try:
@@ -1049,15 +1046,15 @@
                     except (SystemExit, KeyboardInterrupt):
                         raise
                     except BaseException as e:
                         raise RuntimeError(f"Cannot write spec file for library '{name}' to '{spec_file}'") from e
 
                     meta_file.write_text(as_json(meta), "utf-8")
                 else:
-                    self._logger.debug(lambda: f"Skip caching library {name}{repr(args)}")
+                    self._logger.debug(lambda: f"Skip caching library {name}{args!r}")
             except (SystemExit, KeyboardInterrupt):
                 raise
             except BaseException as e:
                 self._logger.exception(e)
 
             return result
 
@@ -1136,15 +1133,15 @@
         ResourceBuilder(res).visit(model)
 
         class MyUserLibrary(UserLibrary):
             current_kw: Any = None
 
             def _log_creating_failed(self, handler: UserErrorHandler, error: BaseException) -> None:
                 err = Error(
-                    message=f"Creating keyword '{handler.name}' failed: {str(error)}",
+                    message=f"Creating keyword '{handler.name}' failed: {error!s}",
                     type_name=type(error).__qualname__,
                     source=self.current_kw.source if self.current_kw is not None else None,
                     line_no=self.current_kw.lineno if self.current_kw is not None else None,
                 )
                 errors.append(err)
 
             def _create_handler(self, kw: Any) -> Any:
@@ -1232,15 +1229,15 @@
         async def _get_libdoc(name: str, args: Tuple[Any, ...], working_dir: str, base_dir: str) -> VariablesDoc:
             meta, source = await self.get_variables_meta(
                 name,
                 base_dir,
                 variables,
             )
 
-            self._logger.debug(lambda: f"Load variables {source}{repr(args)}")
+            self._logger.debug(lambda: f"Load variables {source}{args!r}")
             if meta is not None:
                 meta_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
                 if meta_file.exists():
                     try:
                         try:
                             saved_meta = from_json(meta_file.read_text("utf-8"), LibraryMetaData)
                             spec_path = None
@@ -1276,15 +1273,15 @@
                         variables,
                     ),
                     LOAD_LIBRARY_TIME_OUT,
                 )
 
                 if result.stdout:
                     self._logger.warning(
-                        lambda: f"stdout captured at loading variables {name}{repr(args)}:\n{result.stdout}"
+                        lambda: f"stdout captured at loading variables {name}{args!r}:\n{result.stdout}"
                     )
 
                 try:
                     if meta is not None:
                         meta_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
                         spec_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".spec.json"))
                         spec_file.parent.mkdir(parents=True, exist_ok=True)
@@ -1293,15 +1290,15 @@
                             spec_file.write_text(as_json(result), "utf-8")
                         except (SystemExit, KeyboardInterrupt):
                             raise
                         except BaseException as e:
                             raise RuntimeError(f"Cannot write spec file for variables '{name}' to '{spec_file}'") from e
                         meta_file.write_text(as_json(meta), "utf-8")
                     else:
-                        self._logger.debug(lambda: f"Skip caching variables {name}{repr(args)}")
+                        self._logger.debug(lambda: f"Skip caching variables {name}{args!r}")
                 except (SystemExit, KeyboardInterrupt):
                     raise
                 except BaseException as e:
                     self._logger.exception(e)
                 return result
 
         resolved_args = resolve_args(
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             else (self.normalized_name,)
         )
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(name={repr(self.name)})"
+        return f"{type(self).__name__}(name={self.name!r})"
 
 
 RUN_KEYWORD_WITH_CONDITION_MATCHERS = [KeywordMatcher(e) for e in RUN_KEYWORD_WITH_CONDITION_NAMES]
 
 RUN_KEYWORD_IF_MATCHER = KeywordMatcher(RUN_KEYWORD_IF_NAME)
 
 RUN_KEYWORDS_MATCHER = KeywordMatcher(RUN_KEYWORDS_NAME)
@@ -452,17 +452,17 @@
                 prefix = ""
                 if a.kind == KeywordArgumentKind.VAR_POSITIONAL:
                     prefix = "*"
                 elif a.kind == KeywordArgumentKind.VAR_NAMED:
                     prefix = "**"
 
                 result += (
-                    f"\n| `{prefix}{str(a.name)}`"
+                    f"\n| `{prefix}{a.name!s}`"
                     f"| {'=' if a.default_value is not None else ''}"
-                    f"| {f'`{str(a.default_value)}`' if a.default_value else ''}"
+                    f"| {f'`{a.default_value!s}`' if a.default_value else ''}"
                     f"| {' or '.join(f'`<{s}>`' for s in a.types) if a.types is not None else ''} |"
                 )
 
         if self.tags:
             if result:
                 result += "\n\n"
 
@@ -750,15 +750,15 @@
         return None
 
     def _link_inline_links(self, text: str) -> str:
         headers = [v.group(2) for v in RE_HEADERS.finditer(text)]
 
         def repl(m: re.Match) -> str:  # type: ignore
             if m.group(2) in headers:
-                return f"[{str(m.group(2))}](\\#{str(m.group(2)).lower().replace(' ', '-')})"
+                return f"[{m.group(2)!s}](\\#{str(m.group(2)).lower().replace(' ', '-')})"
             return str(m.group(0))
 
         return str(RE_INLINE_LINK.sub(repl, text))
 
     def _get_doc_for_keywords(self, header_level: int = 2) -> str:
         result = ""
         if any(v for v in self.inits.values() if v.args):
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
     alias: Optional[str] = None
     import_range: Range = field(default_factory=lambda: Range.zero())
     import_source: Optional[str] = None
 
     def __str__(self) -> str:
         result = self.import_name
         if self.args:
-            result += f"  {str(self.args)}"
+            result += f"  {self.args!s}"
         if self.alias:
             result += f"  WITH NAME  {self.alias}"
         return result
 
 
 @dataclass
 class ResourceEntry(LibraryEntry):
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                                 await self.parent.documents.get_or_open_document(f)
 
                                 if config.analysis.progress_mode != AnalysisProgressMode.OFF:
                                     name = f.relative_to(folder.uri.to_path())
 
                                     progress.begin()
                                     progress.report(
-                                        f"Load {str(name)}"
+                                        f"Load {name!s}"
                                         if config.analysis.progress_mode == AnalysisProgressMode.DETAILED
                                         else None,
                                         current=i,
                                     )
                             except (SystemExit, KeyboardInterrupt):
                                 raise
                             except BaseException as e:
@@ -145,15 +145,15 @@
                                 break
 
                             name = f.relative_to(folder.uri.to_path())
 
                             if config.analysis.progress_mode != AnalysisProgressMode.OFF:
                                 progress.begin()
                                 progress.report(
-                                    f"Initialize {str(name)}"
+                                    f"Initialize {name!s}"
                                     if config.analysis.progress_mode == AnalysisProgressMode.DETAILED
                                     else None,
                                     current=i,
                                 )
 
                             if not f.exists():
                                 continue
```

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/.gitignore` & `robotcode_language_server-0.38.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/LICENSE.txt` & `robotcode_language_server-0.38.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/README.md` & `robotcode_language_server-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.37.1/pyproject.toml` & `robotcode_language_server-0.38.0/pyproject.toml`

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
-dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.37.1"]
+dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.38.0"]
 dynamic = ["version"]
 
 [project.scripts]
 'robotcode.language_server' = 'robotcode.language_server.__main__:main'
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_language_server-0.37.1/PKG-INFO` & `robotcode_language_server-0.38.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.37.1
+Version: 0.38.0
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
-Requires-Dist: robotcode-jsonrpc2==0.37.1
+Requires-Dist: robotcode-jsonrpc2==0.38.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

