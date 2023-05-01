# Comparing `tmp/robotcode_language_server-0.35.0.tar.gz` & `tmp/robotcode_language_server-0.36.0.tar.gz`

## Comparing `robotcode_language_server-0.35.0.tar` & `robotcode_language_server-0.36.0.tar`

### file list

```diff
@@ -1,89 +1,88 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/lsp_types.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21125 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    19025 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38217 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    54371 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    63728 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83656 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    80273 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/discovering.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    40456 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/pyproject.toml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9569 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18989 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    54353 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83638 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15233 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    80255 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/discovering.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19259 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23499 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    40438 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11635 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/README.md
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/pyproject.toml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.36.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/__main__.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 from typing import Any, ClassVar, Final, List, NamedTuple, Optional, Set, Union
 
 from robotcode.core.async_tools import Event, async_event
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import (
-    JsonRPCErrorException,
-    JsonRPCErrors,
-    JsonRPCException,
-    JsonRPCProtocol,
-    ProtocolPartDescriptor,
-    rpc_method,
-)
-from robotcode.jsonrpc2.server import JsonRPCServer
-
-from .has_extend_capabilities import HasExtendCapabilities
-from .lsp_types import (
+from robotcode.core.lsp.types import (
     CancelParams,
     ClientCapabilities,
     InitializedParams,
     InitializeError,
     InitializeParams,
     InitializeParamsClientInfoType,
     InitializeResult,
@@ -35,14 +24,25 @@
     TextDocumentSyncKind,
     TextDocumentSyncOptions,
     TraceValues,
     Unregistration,
     UnregistrationParams,
     WorkspaceFolder,
 )
+from robotcode.jsonrpc2.protocol import (
+    JsonRPCErrorException,
+    JsonRPCErrors,
+    JsonRPCException,
+    JsonRPCProtocol,
+    ProtocolPartDescriptor,
+    rpc_method,
+)
+from robotcode.jsonrpc2.server import JsonRPCServer
+
+from .has_extend_capabilities import HasExtendCapabilities
 from .parts.code_action import CodeActionProtocolPart
 from .parts.code_lens import CodeLensProtocolPart
 from .parts.commands import CommandsProtocolPart
 from .parts.completion import CompletionProtocolPart
 from .parts.declaration import DeclarationProtocolPart
 from .parts.definition import DefinitionProtocolPart
 from .parts.diagnostics import DiagnosticsProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/text_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import io
 import threading
 import weakref
 from typing import Any, Awaitable, Callable, Dict, Final, List, Optional, TypeVar, Union, cast
 
 from robotcode.core.async_tools import async_event, create_sub_task
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import DocumentUri, Position, Range
 from robotcode.core.uri import Uri
 
-from .lsp_types import DocumentUri, Position, Range
-
 
 def is_multibyte_char(char: str) -> bool:
     return ord(char) > 0xFFFF
 
 
 def position_from_utf16(lines: List[str], position: Position) -> Position:
     if position.line >= len(lines):
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from asyncio import CancelledError
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Final, List, Optional, Union, cast
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import HasCodeActionKinds, language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     CodeAction,
     CodeActionContext,
     CodeActionOptions,
     CodeActionParams,
     Command,
     Range,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import HasCodeActionKinds, language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import asyncio
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, create_sub_task, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     CodeLens,
     CodeLensOptions,
     CodeLensParams,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.text_document import TextDocument
 
 from .protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import uuid
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Dict, Final, List, Optional, cast
 
 from robotcode.core.async_tools import threaded
 from robotcode.core.dataclasses import from_dict
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
-from robotcode.language_server.common.decorators import IsCommand, get_command_name
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     ErrorCodes,
     ExecuteCommandOptions,
     ExecuteCommandParams,
     LSPAny,
     ServerCapabilities,
 )
+from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
+from robotcode.language_server.common.decorators import IsCommand, get_command_name
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 
 _FUNC_TYPE = Callable[..., Awaitable[Optional[LSPAny]]]
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from asyncio import CancelledError
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Final, List, Optional, Union, cast
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import HasAllCommitCharacters, HasTriggerCharacters, language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     CompletionContext,
     CompletionItem,
     CompletionList,
     CompletionOptions,
     CompletionParams,
     InsertReplaceEdit,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
     TextEdit,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import HasAllCommitCharacters, HasTriggerCharacters, language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional, Union
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DeclarationParams,
     Location,
     LocationLink,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional, Union
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DefinitionParams,
     Location,
     LocationLink,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,15 @@
     async_tasking_event,
     async_tasking_event_iterator,
     check_canceled,
     create_sub_task,
     threaded,
 )
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.uri import Uri
-from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Diagnostic,
     DiagnosticOptions,
     DiagnosticServerCancellationData,
     DocumentDiagnosticParams,
     DocumentDiagnosticReport,
     LSPErrorCodes,
     PreviousResultId,
@@ -36,14 +32,18 @@
     PublishDiagnosticsParams,
     RelatedFullDocumentDiagnosticReport,
     ServerCapabilities,
     TextDocumentIdentifier,
     WorkspaceDiagnosticParams,
     WorkspaceDiagnosticReport,
 )
+from robotcode.core.uri import Uri
+from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 __all__ = ["DiagnosticsProtocolPart", "DiagnosticsResult"]
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DocumentHighlight,
     DocumentHighlightOptions,
     DocumentHighlightParams,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     Union,
     cast,
     runtime_checkable,
 )
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DocumentSymbol,
     DocumentSymbolClientCapabilitiesSymbolKindType,
     DocumentSymbolClientCapabilitiesTagSupportType,
     DocumentSymbolOptions,
     DocumentSymbolParams,
     ServerCapabilities,
     SymbolInformation,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,15 @@
     Optional,
     Union,
     cast,
 )
 
 from robotcode.core.async_tools import Lock, async_event, async_tasking_event, create_sub_task
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.uri import Uri
-from robotcode.jsonrpc2.protocol import JsonRPCException, rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DidChangeTextDocumentParams,
     DidCloseTextDocumentParams,
     DidOpenTextDocumentParams,
     DidSaveTextDocumentParams,
     DocumentUri,
     FileChangeType,
     FileEvent,
@@ -39,14 +36,17 @@
     TextDocumentSyncKind,
     TextDocumentSyncOptions,
     TextEdit,
     VersionedTextDocumentIdentifier,
     WatchKind,
     WillSaveTextDocumentParams,
 )
+from robotcode.core.uri import Uri
+from robotcode.jsonrpc2.protocol import JsonRPCException, rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
 from robotcode.language_server.common.text_document import TextDocument
 
 from .protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     FoldingRange,
     FoldingRangeParams,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol  # pragma: no cover
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DocumentFormattingOptions,
     DocumentFormattingParams,
     DocumentRangeFormattingOptions,
     DocumentRangeFormattingParams,
     FormattingOptions,
     ProgressToken,
     Range,
     ServerCapabilities,
     TextDocumentIdentifier,
     TextEdit,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.parts.protocol_part import (
     LanguageServerProtocolPart,
 )
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Hover,
     HoverOptions,
     HoverParams,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.parts.protocol_part import (
     LanguageServerProtocolPart,
 )
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional, Union
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     ImplementationParams,
     Location,
     LocationLink,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 from .protocol_part import LanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     InlayHint,
     InlayHintOptions,
     InlayHintParams,
     Range,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 from .protocol_part import LanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import (
-    HasLanguageId,
-    language_id_filter,
-)
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DocumentSelector,
     InlineValue,
     InlineValueContext,
     InlineValueParams,
     InlineValueRegistrationOptions,
     Range,
     ServerCapabilities,
     TextDocumentFilterType1,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import (
+    HasLanguageId,
+    language_id_filter,
+)
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.parts.protocol_part import (
     LanguageServerProtocolPart,
 )
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol  # pragma: no cover
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     LinkedEditingRangeOptions,
     LinkedEditingRangeParams,
     LinkedEditingRanges,
     Position,
     Range,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 from .protocol_part import LanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/references.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Location,
     Position,
     ReferenceContext,
     ReferenceOptions,
     ReferenceParams,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 from .protocol_part import LanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     ErrorCodes,
     Position,
     PrepareRenameParams,
     PrepareRenameResult,
     PrepareRenameResultType1,
     Range,
     RenameOptions,
     RenameParams,
     ServerCapabilities,
     TextDocumentEdit,
     TextDocumentIdentifier,
     WorkspaceEdit,
 )
+from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 from .protocol_part import LanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Position,
     SelectionRange,
     SelectionRangeOptions,
     SelectionRangeParams,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 from .protocol_part import LanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 
 from asyncio import CancelledError
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Final, List, Union
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Range,
     SemanticTokenModifiers,
     SemanticTokens,
     SemanticTokensDelta,
     SemanticTokensDeltaParams,
     SemanticTokensDeltaPartialResult,
     SemanticTokensLegend,
@@ -24,14 +19,19 @@
     SemanticTokensParams,
     SemanticTokensPartialResult,
     SemanticTokensRangeParams,
     SemanticTokenTypes,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 from .protocol_part import LanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from asyncio import CancelledError
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Final, List, Optional, cast
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import HasRetriggerCharacters, HasTriggerCharacters, language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Position,
     ServerCapabilities,
     SignatureHelp,
     SignatureHelpContext,
     SignatureHelpOptions,
     SignatureHelpParams,
     TextDocumentIdentifier,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import HasRetriggerCharacters, HasTriggerCharacters, language_id_filter
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.text_document import TextDocument
 
 from .protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import contextlib
 import uuid
 from typing import TYPE_CHECKING, Any, AsyncIterator, Dict, List, Optional
 
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     URI,
     LogMessageParams,
     MessageActionItem,
     MessageType,
     ProgressParams,
     ProgressToken,
     Range,
@@ -17,14 +16,15 @@
     ShowMessageRequestParams,
     WorkDoneProgressBegin,
     WorkDoneProgressCancelParams,
     WorkDoneProgressCreateParams,
     WorkDoneProgressEnd,
     WorkDoneProgressReport,
 )
+from robotcode.jsonrpc2.protocol import rpc_method
 
 from .protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,15 @@
     Lock,
     async_tasking_event,
     create_sub_task,
     threaded,
 )
 from robotcode.core.dataclasses import CamelSnakeMixin, from_dict
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.uri import Uri
-from robotcode.core.utils.path import path_is_relative_to
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     ApplyWorkspaceEditParams,
     ApplyWorkspaceEditResult,
     ConfigurationItem,
     ConfigurationParams,
     CreateFilesParams,
     DeleteFilesParams,
     DidChangeConfigurationParams,
@@ -65,17 +59,23 @@
     TextDocumentEdit,
     TextEdit,
     WatchKind,
     WorkspaceEdit,
     WorkspaceFoldersChangeEvent,
     WorkspaceFoldersServerCapabilities,
 )
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     WorkspaceFolder as TypesWorkspaceFolder,
 )
+from robotcode.core.uri import Uri
+from robotcode.core.utils.path import path_is_relative_to
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 
 from .protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 __all__ = [
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Final, List, Optional
 
 from robotcode.core.dataclasses import CamelSnakeMixin, from_dict
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import InitializeError
 from robotcode.jsonrpc2.protocol import JsonRPCErrorException, JsonRPCErrors, ProtocolPartDescriptor
-from robotcode.language_server.common.lsp_types import InitializeError
 from robotcode.language_server.common.parts.document_symbols import symbol_information_label
 from robotcode.language_server.common.protocol import LanguageDefinition, LanguageServerProtocol
 
 from ..__version__ import __version__
 from .configuration import RobotConfig
 from .parts.code_action_documentation import RobotCodeActionDocumentationProtocolPart
 from .parts.code_action_fixes import RobotCodeActionFixesProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import asyncio
 import itertools
 import os
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union, cast
 
-from robotcode.core.uri import Uri
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     CodeDescription,
     Diagnostic,
     DiagnosticRelatedInformation,
     DiagnosticSeverity,
     DiagnosticTag,
     Location,
     Position,
     Range,
 )
+from robotcode.core.uri import Uri
 from robotcode.language_server.robotframework.parts.model_helper import ModelHelperMixin
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HasTokens,
     Statement,
     Token,
     is_not_variable_token,
     iter_over_keyword_names_and_owners,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, TypeVar, cast
 
-from robotcode.language_server.common.lsp_types import Position, Range
+from robotcode.core.lsp.types import Position, Range
 from robotcode.language_server.robotframework.utils.ast_utils import Token, range_from_token
 
 if TYPE_CHECKING:
     from .library_doc import KeywordDoc
 
 _F = TypeVar("_F", bound=Callable[..., Any])
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     final,
 )
 
 from robotcode.core.async_cache import AsyncSimpleLRUCache
 from robotcode.core.async_tools import Lock, async_tasking_event, create_sub_task
 from robotcode.core.dataclasses import as_json, from_json
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import DocumentUri, FileChangeType, FileEvent
 from robotcode.core.uri import Uri
 from robotcode.core.utils.glob_path import Pattern, iter_files
 from robotcode.core.utils.path import path_is_relative_to
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import DocumentUri, FileChangeType, FileEvent
 from robotcode.language_server.common.parts.workspace import FileWatcherEntry, Workspace
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import CacheSaveLocation, RobotCodeConfig
 from robotcode.language_server.robotframework.utils.ast_utils import HasError, HasErrors, Token
 from robotcode.language_server.robotframework.utils.robot_path import find_file_ex
 from robotcode.language_server.robotframework.utils.version import get_robot_version, get_robot_version_str
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Optional,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
-from robotcode.language_server.common.lsp_types import Position, Range
+from robotcode.core.lsp.types import Position, Range
 from robotcode.language_server.robotframework.utils.ast_utils import (
     Token,
     range_from_token,
 )
 from robotcode.language_server.robotframework.utils.markdownformatter import (
     MarkDownFormatter,
 )
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     Tuple,
     Union,
     cast,
 )
 
 from robotcode.core.async_tools import Lock, async_event
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.uri import Uri
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     CodeDescription,
     Diagnostic,
     DiagnosticRelatedInformation,
     DiagnosticSeverity,
     DiagnosticTag,
     DocumentUri,
     Location,
     Position,
     Range,
 )
+from robotcode.core.uri import Uri
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.languages import Languages
 from robotcode.language_server.robotframework.utils.ast_utils import (
     Token,
     range_from_node,
     range_from_token,
     strip_variable_token,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 from threading import Thread
 from typing import TYPE_CHECKING, Any, List, Optional, Tuple, Union, cast
 from urllib.parse import parse_qs, urlparse
 
 from robotcode.core.async_tools import threaded
 from robotcode.core.dataclasses import CamelSnakeMixin
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.uri import Uri
-from robotcode.core.utils.net import find_free_port
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import code_action_kinds, language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     CodeAction,
     CodeActionContext,
     CodeActionKind,
     Command,
     Range,
 )
+from robotcode.core.uri import Uri
+from robotcode.core.utils.net import find_free_port
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import code_action_kinds, language_id
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import (
     DocumentationServerConfig,
 )
 from robotcode.language_server.robotframework.diagnostics.library_doc import (
     get_library_doc,
     get_robot_library_html_doc_str,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
 import ast
 from string import Template
 from typing import TYPE_CHECKING, Any, List, Optional, Union, cast
 
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.language_server.common.decorators import code_action_kinds, command, language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     AnnotatedTextEdit,
     ChangeAnnotation,
     CodeAction,
     CodeActionContext,
     CodeActionKind,
     CodeActionTriggerKind,
     Command,
     DocumentUri,
     OptionalVersionedTextDocumentIdentifier,
     Position,
     Range,
     TextDocumentEdit,
     WorkspaceEdit,
 )
+from robotcode.language_server.common.decorators import code_action_kinds, command, language_id
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.ast_utils import Token, get_node_at_position, range_from_node
 from robotcode.language_server.robotframework.utils.async_ast import AsyncVisitor
 
 from .model_helper import ModelHelperMixin
 from .protocol_part import RobotLanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import ast
 from typing import TYPE_CHECKING, Any, List, Optional, Set, Tuple, cast
 
 from robotcode.core.async_tools import create_sub_task
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import CodeLens, Command
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import CodeLens, Command
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import AnalysisConfig
 from robotcode.language_server.robotframework.diagnostics.library_doc import KeywordDoc
 from robotcode.language_server.robotframework.utils.ast_utils import range_from_token
 from robotcode.language_server.robotframework.utils.async_ast import AsyncVisitor
 
 from .model_helper import ModelHelperMixin
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
     TypedDict,
     Union,
     cast,
 )
 
 from robotcode.core.async_itertools import async_chain, async_chain_iterator
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.language_server.common.decorators import language_id, trigger_characters
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     CompletionContext,
     CompletionItem,
     CompletionItemKind,
     CompletionList,
     CompletionTriggerKind,
     InsertTextFormat,
     MarkupContent,
     MarkupKind,
     Position,
     Range,
     TextEdit,
 )
+from robotcode.language_server.common.decorators import language_id, trigger_characters
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import CompletionConfig
 from robotcode.language_server.robotframework.diagnostics.entities import VariableDefinitionType
 from robotcode.language_server.robotframework.diagnostics.library_doc import (
     CompleteResultKind,
     KeywordArgumentKind,
     KeywordDoc,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Optional
 
 from robotcode.core.async_itertools import async_next
 from robotcode.core.async_tools import run_coroutine_in_thread, threaded
 from robotcode.core.dataclasses import CamelSnakeMixin
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import Position, Range, TextDocumentIdentifier
 from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.lsp_types import Position, Range, TextDocumentIdentifier
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HasTokens,
     get_nodes_at_position,
     get_tokens_at_position,
     range_from_token,
 )
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import ast
 import asyncio
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from robotcode.core.async_tools import check_canceled, create_sub_task, threaded
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import Diagnostic, DiagnosticSeverity, DiagnosticTag, Position, Range
 from robotcode.core.uri import Uri
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import Diagnostic, DiagnosticSeverity, DiagnosticTag, Position, Range
 from robotcode.language_server.common.parts.diagnostics import DiagnosticsResult
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import AnalysisConfig
 from robotcode.language_server.robotframework.diagnostics.entities import ArgumentDefinition
 from robotcode.language_server.robotframework.diagnostics.namespace import Namespace
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HeaderAndBodyBlock,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/discovering.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/discovering.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterator, List, Optional, cast
 
 from robotcode.core.async_tools import check_canceled, check_canceled_sync, threaded
 from robotcode.core.dataclasses import CamelSnakeMixin
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.uri import Uri
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     DocumentUri,
     Position,
     Range,
     TextDocumentIdentifier,
 )
+from robotcode.core.uri import Uri
+from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.language_server.robotframework.configuration import RobotConfig
 from robotcode.language_server.robotframework.utils.async_ast import AsyncVisitor
 
 from .protocol_part import RobotLanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.robotframework.protocol import (
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import DocumentHighlight, DocumentHighlightKind, Position
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import DocumentHighlight, DocumentHighlightKind, Position
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.robotframework.protocol import RobotLanguageServerProtocol
 
 from .model_helper import ModelHelperMixin
 from .protocol_part import RobotLanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import ast
 import itertools
 from typing import TYPE_CHECKING, Any, List, Optional, Union, cast
 
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import DocumentSymbol, SymbolInformation, SymbolKind
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import DocumentSymbol, SymbolInformation, SymbolKind
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.ast_utils import (
     Token,
     range_from_node,
     range_from_token,
     tokenize_variables,
 )
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     Optional,
     Tuple,
     Union,
     cast,
 )
 
 from robotcode.core.async_tools import Lock, async_tasking_event, check_canceled_sync
+from robotcode.core.lsp.types import MessageType
 from robotcode.core.uri import Uri
 from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.lsp_types import MessageType
 from robotcode.language_server.common.parts.workspace import WorkspaceFolder
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import RobotCodeConfig, RobotConfig
 from robotcode.language_server.robotframework.diagnostics.imports_manager import ImportsManager
 from robotcode.language_server.robotframework.diagnostics.namespace import DocumentType, Namespace
 from robotcode.language_server.robotframework.utils.ast_utils import Token
 from robotcode.language_server.robotframework.utils.version import get_robot_version
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import ast
 from typing import TYPE_CHECKING, Any, List, Optional, cast
 
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import FoldingRange
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import FoldingRange
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.async_ast import AsyncVisitor
 
 from .protocol_part import RobotLanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.robotframework.protocol import (
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import asyncio
 import io
 import os
 import re
 from typing import TYPE_CHECKING, Any, List, Optional, cast
 
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     FormattingOptions,
     MessageType,
     Position,
     Range,
     TextEdit,
 )
+from robotcode.language_server.common.decorators import language_id
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.version import get_robot_version
 
 if TYPE_CHECKING:
     from robotcode.language_server.robotframework.protocol import (
         RobotLanguageServerProtocol,
     )
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     Type,
     Union,
     cast,
 )
 
 from robotcode.core.async_itertools import async_next
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import Location, LocationLink, Position
 from robotcode.core.uri import Uri
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import Location, LocationLink, Position
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HasTokens,
     Token,
     get_nodes_at_position,
     get_tokens_at_position,
     range_from_token,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     Type,
     Union,
     cast,
 )
 
 from robotcode.core.async_itertools import async_next
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import Hover, MarkupContent, MarkupKind, Position
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import Hover, MarkupContent, MarkupKind, Position
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HasTokens,
     Token,
     get_nodes_at_position,
     get_tokens_at_position,
     range_from_node,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import ast
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, List, Optional, Type, cast
 
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import InlayHint, InlayHintKind, Range
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import InlayHint, InlayHintKind, Range
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import InlayHintsConfig
 from robotcode.language_server.robotframework.diagnostics.library_doc import KeywordArgumentKind
 from robotcode.language_server.robotframework.diagnostics.namespace import Namespace
 from robotcode.language_server.robotframework.utils.ast_utils import Token, range_from_node, range_from_token
 from robotcode.language_server.robotframework.utils.async_ast import iter_nodes
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import ast
 from typing import TYPE_CHECKING, Any, Iterator, List, Optional, Tuple
 
 from robotcode.core.async_itertools import async_dropwhile, async_takewhile
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     InlineValue,
     InlineValueContext,
     InlineValueEvaluatableExpression,
     Range,
 )
+from robotcode.language_server.common.decorators import language_id
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HasTokens,
     Token,
     get_nodes_at_position,
     iter_nodes,
     range_from_node,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Optional,
     Set,
     Tuple,
     Type,
     Union,
 )
 
-from robotcode.language_server.common.lsp_types import Position
+from robotcode.core.lsp.types import Position
 from robotcode.language_server.robotframework.diagnostics.entities import (
     VariableDefinition,
     VariableNotFoundDefinition,
 )
 from robotcode.language_server.robotframework.diagnostics.library_doc import (
     KeywordDoc,
     KeywordMatcher,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     Type,
     cast,
 )
 
 from robotcode.core.async_cache import AsyncSimpleLRUCache
 from robotcode.core.async_tools import async_event, threaded
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import FileEvent, Location, Position, ReferenceContext, WatchKind
 from robotcode.core.uri import Uri
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import FileEvent, Location, Position, ReferenceContext, WatchKind
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.diagnostics.entities import LocalVariableDefinition, VariableDefinition
 from robotcode.language_server.robotframework.diagnostics.library_doc import (
     RESOURCE_FILE_EXTENSION,
     ROBOT_FILE_EXTENSION,
     KeywordDoc,
     LibraryDoc,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     TypeVar,
     Union,
     cast,
 )
 
 from robotcode.core.async_itertools import async_next
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     AnnotatedTextEdit,
     ChangeAnnotation,
     CreateFile,
     DeleteFile,
     OptionalVersionedTextDocumentIdentifier,
     Position,
     PrepareRenameResult,
     PrepareRenameResultType1,
     RenameFile,
     TextDocumentEdit,
     WorkspaceEdit,
 )
+from robotcode.language_server.common.decorators import language_id
 from robotcode.language_server.common.parts.rename import CantRenameError
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.diagnostics.entities import (
     VariableDefinition,
     VariableDefinitionType,
 )
 from robotcode.language_server.robotframework.diagnostics.library_doc import KeywordDoc
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import io
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from robotcode.core.async_tools import check_canceled, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.utils.version import create_version_from_str
-from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Diagnostic,
     DiagnosticSeverity,
     Position,
     Range,
 )
+from robotcode.core.utils.version import create_version_from_str
+from robotcode.language_server.common.decorators import language_id
 from robotcode.language_server.common.parts.diagnostics import DiagnosticsResult
 from robotcode.language_server.common.parts.workspace import WorkspaceFolder
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.configuration import RoboCopConfig
 
 from .protocol_part import RobotLanguageServerProtocolPart
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import asyncio
 import time
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from robotcode.core.async_tools import Event, threaded
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.uri import InvalidUriError, Uri
-from robotcode.core.utils.glob_path import iter_files
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     FileChangeType,
     FileEvent,
     WatchKind,
 )
+from robotcode.core.uri import InvalidUriError, Uri
+from robotcode.core.utils.glob_path import iter_files
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.language_server.common.decorators import language_id
 from robotcode.language_server.common.parts.diagnostics import (
     AnalysisProgressMode,
     DiagnosticsMode,
     WorkspaceDocumentsResult,
 )
 from robotcode.language_server.robotframework.configuration import (
     AnalysisConfig,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.lsp.types import Position, SelectionRange
 from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import Position, SelectionRange
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HasTokens,
     get_nodes_at_position,
     get_tokens_at_position,
     range_from_node,
     range_from_token,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     Tuple,
     Union,
     cast,
 )
 
 from robotcode.core.async_itertools import async_dropwhile, async_takewhile
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.language_server.common.decorators import language_id
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     Position,
     Range,
     SemanticTokenModifiers,
     SemanticTokens,
     SemanticTokensDelta,
     SemanticTokensDeltaPartialResult,
     SemanticTokensPartialResult,
     SemanticTokenTypes,
 )
+from robotcode.language_server.common.decorators import language_id
 from robotcode.language_server.common.text_document import TextDocument, range_to_utf16
 from robotcode.language_server.robotframework.diagnostics.library_doc import (
     ALL_RUN_KEYWORDS_MATCHERS,
     BUILTIN_LIBRARY_NAME,
     KeywordArgumentKind,
     KeywordDoc,
     KeywordMatcher,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     Optional,
     Tuple,
     Type,
     cast,
 )
 
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.language_server.common.decorators import language_id, retrigger_characters, trigger_characters
-from robotcode.language_server.common.lsp_types import (
+from robotcode.core.lsp.types import (
     MarkupContent,
     MarkupKind,
     ParameterInformation,
     Position,
     SignatureHelp,
     SignatureHelpContext,
     SignatureInformation,
 )
+from robotcode.language_server.common.decorators import language_id, retrigger_characters, trigger_characters
 from robotcode.language_server.common.text_document import TextDocument
 from robotcode.language_server.robotframework.diagnostics.library_doc import KeywordDoc, LibraryDoc
 from robotcode.language_server.robotframework.parts.model_helper import ModelHelperMixin
 from robotcode.language_server.robotframework.parts.protocol_part import RobotLanguageServerProtocolPart
 from robotcode.language_server.robotframework.utils.ast_utils import (
     Token,
     get_node_at_position,
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Protocol,
     Set,
     Tuple,
     cast,
     runtime_checkable,
 )
 
-from robotcode.language_server.common.lsp_types import Position, Range
+from robotcode.core.lsp.types import Position, Range
 
 from . import async_ast
 
 
 def iter_nodes(node: ast.AST) -> Iterator[ast.AST]:
     for _field, value in ast.iter_fields(node):
         if isinstance(value, list):
```

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.36.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/.gitignore` & `robotcode_language_server-0.36.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/LICENSE.txt` & `robotcode_language_server-0.36.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/README.md` & `robotcode_language_server-0.36.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.35.0/pyproject.toml` & `robotcode_language_server-0.36.0/pyproject.toml`

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
-dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.35.0"]
+dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.36.0"]
 dynamic = ["version"]
 
 [project.scripts]
 'robotcode.language_server' = 'robotcode.language_server.__main__:main'
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_language_server-0.35.0/PKG-INFO` & `robotcode_language_server-0.36.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.35.0
+Version: 0.36.0
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
-Requires-Dist: robotcode-jsonrpc2==0.35.0
+Requires-Dist: robotcode-jsonrpc2==0.36.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

