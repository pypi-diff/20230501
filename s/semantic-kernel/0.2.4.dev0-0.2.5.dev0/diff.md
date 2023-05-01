# Comparing `tmp/semantic_kernel-0.2.4.dev0.tar.gz` & `tmp/semantic_kernel-0.2.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.4.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.5.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.4.dev0.tar` & `semantic_kernel-0.2.5.dev0.tar`

### file list

```diff
@@ -1,87 +1,89 @@
--rw-r--r--   0        0        0     4562 2023-04-19 21:51:48.404232 semantic_kernel-0.2.4.dev0/README.md
--rw-r--r--   0        0        0      644 2023-04-24 18:00:09.400940 semantic_kernel-0.2.4.dev0/pyproject.toml
--rw-r--r--   0        0        0     1302 2023-04-19 06:06:19.926015 semantic_kernel-0.2.4.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-14 03:36:09.230039 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/ai_exception.py
--rw-r--r--   0        0        0      495 2023-04-14 03:36:09.230576 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-14 03:36:09.231022 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-14 03:36:09.231429 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-14 03:36:09.232144 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      479 2023-04-14 03:36:09.232562 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
--rw-r--r--   0        0        0      817 2023-04-14 03:36:09.232970 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2771 2023-04-14 03:36:09.233875 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2763 2023-04-14 03:36:09.234689 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2758 2023-04-14 03:36:09.235471 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4007 2023-04-14 03:36:09.236270 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4441 2023-04-14 03:36:09.236952 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2427 2023-04-14 03:36:09.237661 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      476 2023-04-14 03:36:09.238119 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      457 2023-04-21 23:16:53.100030 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-14 03:36:09.239029 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-21 23:16:53.100412 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 03:36:09.239829 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-14 03:36:09.240512 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5613 2023-04-14 03:36:09.240911 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    12421 2023-04-21 23:16:53.101120 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2240 2023-04-20 17:10:26.993745 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     9134 2023-04-14 03:36:09.243870 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_config.py
--rw-r--r--   0        0        0     1626 2023-04-14 03:36:09.244661 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-14 03:36:09.245082 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-14 03:36:09.245483 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     3826 2023-04-21 23:16:53.101795 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-14 03:36:09.246857 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1531 2023-04-14 03:36:09.247527 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-14 03:36:09.247903 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-14 03:36:09.248433 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     1598 2023-04-14 03:36:09.248824 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0      299 2023-04-14 03:36:09.249224 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-14 03:36:09.249612 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     2499 2023-04-14 03:36:09.250068 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1237 2023-04-14 03:36:09.250457 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0      836 2023-04-14 03:36:09.250950 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/data_entry.py
--rw-r--r--   0        0        0      953 2023-04-14 03:36:09.251369 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/data_store_base.py
--rw-r--r--   0        0        0     1989 2023-04-14 03:36:09.251740 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/volatile_data_store.py
--rw-r--r--   0        0        0     4050 2023-04-14 03:36:09.252125 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-20 17:10:26.995186 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 03:36:09.253302 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-14 03:36:09.253662 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-14 03:36:09.254004 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 03:36:09.254344 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15963 2023-04-24 01:56:59.028969 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6164 2023-04-24 01:56:59.029417 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      919 2023-04-14 03:36:09.255908 semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-14 03:36:09.256522 semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-14 03:36:09.256949 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 03:36:09.257319 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-14 03:36:09.257703 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-14 03:36:09.258212 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 03:36:09.258593 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 03:36:09.259027 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 03:36:09.259911 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-14 03:36:09.260336 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 03:36:09.261065 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 03:36:09.261495 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 03:36:09.261836 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-14 03:36:09.262309 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 03:36:09.262723 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 03:36:09.263484 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-14 03:36:09.263900 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-14 03:36:09.264367 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 03:36:09.264992 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 03:36:09.265522 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-24 01:56:59.029930 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-14 03:36:09.267164 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-14 03:36:09.267627 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 03:36:09.268042 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-14 03:36:09.268607 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 03:36:09.269045 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-14 03:36:09.269480 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 03:36:09.269880 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-14 03:36:09.270280 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-14 03:36:09.270855 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-14 03:36:09.271313 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-14 03:36:09.271775 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      403 2023-04-14 03:36:09.272351 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-14 03:36:09.272775 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-14 03:36:09.273176 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-14 03:36:09.274119 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5136 1970-01-01 00:00:00.000000 semantic_kernel-0.2.4.dev0/PKG-INFO
+-rw-r--r--   0        0        0     4573 2023-04-30 18:57:02.979916 semantic_kernel-0.2.5.dev0/README.md
+-rw-r--r--   0        0        0      719 2023-05-01 18:50:34.098615 semantic_kernel-0.2.5.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1302 2023-04-18 17:46:11.883057 semantic_kernel-0.2.5.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0      506 2023-04-30 18:57:02.983999 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3463 2023-04-30 18:57:02.987541 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2093 2023-04-30 18:57:02.988126 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2782 2023-04-30 18:57:02.989002 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2774 2023-04-30 18:57:02.989380 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2769 2023-04-30 18:57:02.990041 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     5227 2023-04-30 18:57:02.990444 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4471 2023-04-30 18:57:02.990953 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2449 2023-04-30 18:57:02.991301 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      497 2023-04-30 18:57:02.991644 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      457 2023-04-22 04:06:40.780007 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5849 2023-04-30 18:57:02.992220 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    12503 2023-04-30 18:57:02.992677 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2240 2023-04-22 04:06:40.781294 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0     9401 2023-04-30 18:57:02.993097 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_config.py
+-rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-14 00:51:57.196637 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-13 23:12:46.171776 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     3822 2023-04-30 18:57:02.994407 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-13 23:12:46.172614 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1481 2023-04-30 18:57:02.995123 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3089 2023-04-30 18:57:02.996701 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2012 2023-04-30 18:57:02.997202 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6036 2023-04-30 18:57:02.997638 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-04-30 18:57:02.998486 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-14 00:51:57.200548 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15917 2023-04-30 18:57:02.998992 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      919 2023-04-13 23:12:46.181682 semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-13 23:12:46.182155 semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.2.5.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.2.5.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     6466 2023-05-01 18:36:22.039798 semantic_kernel-0.2.5.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 semantic_kernel-0.2.5.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.4.dev0/README.md` & `semantic_kernel-0.2.5.dev0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Get Started with Semantic Kernel ⚡
 
 Install the latest package:
 
     python -m pip install --upgrade semantic-kernel
 
 
-# AI backends
+# AI Services
 
 ## OpenAI / Azure OpenAI API keys
 
 Make sure you have an
 [Open AI API Key](https://openai.com/api/) or
 [Azure Open AI service key](https://learn.microsoft.com/azure/cognitive-services/openai/quickstart?pivots=rest-api)
 
@@ -23,25 +23,25 @@
 AZURE_OPENAI_API_KEY=""
 ```
 
 # Running a prompt
 
 ```python
 import semantic_kernel as sk
-from semantic_kernel.ai.open_ai import OpenAITextCompletion, AzureTextCompletion
+from semantic_kernel.connectors.ai.open_ai import OpenAITextCompletion, AzureTextCompletion
 
 kernel = sk.Kernel()
 
-# Prepare OpenAI backend using credentials stored in the `.env` file
+# Prepare OpenAI service using credentials stored in the `.env` file
 api_key, org_id = sk.openai_settings_from_dot_env()
-kernel.config.add_text_backend("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
+kernel.config.add_text_service("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
 
 # Alternative using Azure:
 # deployment, api_key, endpoint = sk.azure_openai_settings_from_dot_env()
-# kernel.config.add_text_backend("dv", AzureTextCompletion(deployment, endpoint, api_key))
+# kernel.config.add_text_service("dv", AzureTextCompletion(deployment, endpoint, api_key))
 
 # Wrap your prompt in a function
 prompt = kernel.create_semantic_function("""
 1) A robot may not injure a human being or, through inaction,
 allow a human being to come to harm.
 
 2) A robot must obey orders given it by human beings except where
```

### Comparing `semantic_kernel-0.2.4.dev0/pyproject.toml` & `semantic_kernel-0.2.5.dev0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.2.4.dev"
+version = "0.2.5.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
 openai = "^0.27.0"
 aiofiles = "^23.1.0"
+transformers = "^4.28.1"
+torch = "^2.0.0"
+sentence-transformers = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.21.0"
 black = {version = "^23.1.0", allow-prereleases = true}
 ipykernel = "^6.21.1"
 pytest = "7.2.0"
 ruff = "^0.0.257"
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/ai_exception.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/chat_request_settings.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/complete_request_settings.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 from logging import Logger
 from typing import Any, Optional
 
-from semantic_kernel.ai.open_ai.services.open_ai_chat_completion import (
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion import (
     OpenAIChatCompletion,
 )
 
 
 class AzureChatCompletion(OpenAIChatCompletion):
     _endpoint: str
     _api_version: str
@@ -20,15 +20,15 @@
         endpoint: Optional[str] = None,
         api_key: Optional[str] = None,
         api_version: str = "2023-03-15-preview",
         logger: Optional[Logger] = None,
         ad_auth=False,
     ) -> None:
         """
-        Initialize an AzureChatCompletion backend.
+        Initialize an AzureChatCompletion service.
 
         You must provide:
         - A deployment_name, endpoint, and api_key (plus, optionally: ad_auth)
 
         :param deployment_name: The name of the Azure deployment. This value
             will correspond to the custom name you chose for your deployment
             when you deployed a model. This value can be found under
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 from logging import Logger
 from typing import Any, Optional
 
-from semantic_kernel.ai.open_ai.services.open_ai_text_completion import (
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion import (
     OpenAITextCompletion,
 )
 
 
 class AzureTextCompletion(OpenAITextCompletion):
     _endpoint: str
     _api_version: str
@@ -20,15 +20,15 @@
         endpoint: Optional[str] = None,
         api_key: Optional[str] = None,
         api_version: str = "2022-12-01",
         logger: Optional[Logger] = None,
         ad_auth=False,
     ) -> None:
         """
-        Initialize an AzureTextCompletion backend.
+        Initialize an AzureTextCompletion service.
 
         You must provide:
         - A deployment_name, endpoint, and api_key (plus, optionally: ad_auth)
 
         :param deployment_name: The name of the Azure deployment. This value
             will correspond to the custom name you chose for your deployment
             when you deployed a model. This value can be found under
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 from logging import Logger
 from typing import Any, Optional
 
-from semantic_kernel.ai.open_ai.services.open_ai_text_embedding import (
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding import (
     OpenAITextEmbedding,
 )
 
 
 class AzureTextEmbedding(OpenAITextEmbedding):
     _endpoint: str
     _api_version: str
@@ -20,15 +20,15 @@
         endpoint: Optional[str] = None,
         api_key: Optional[str] = None,
         api_version: str = "2022-12-01",
         logger: Optional[Logger] = None,
         ad_auth=False,
     ) -> None:
         """
-        Initialize an AzureTextEmbedding backend.
+        Initialize an AzureTextEmbedding service.
 
         You must provide:
         - A deployment_name, endpoint, and api_key (plus, optionally: ad_auth)
 
         :param deployment_name: The name of the Azure deployment. This value
             will correspond to the custom name you chose for your deployment
             when you deployed a model. This value can be found under
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,130 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
-from typing import Any, List, Optional, Tuple
+from typing import Any, Optional
 
-from semantic_kernel.ai.ai_exception import AIException
-from semantic_kernel.ai.chat_completion_client_base import ChatCompletionClientBase
-from semantic_kernel.ai.chat_request_settings import ChatRequestSettings
+from semantic_kernel.connectors.ai.ai_exception import AIException
+from semantic_kernel.connectors.ai.complete_request_settings import (
+    CompleteRequestSettings,
+)
+from semantic_kernel.connectors.ai.text_completion_client_base import (
+    TextCompletionClientBase,
+)
 from semantic_kernel.utils.null_logger import NullLogger
 
 
-class OpenAIChatCompletion(ChatCompletionClientBase):
+class OpenAITextCompletion(TextCompletionClientBase):
     _model_id: str
     _api_key: str
     _org_id: Optional[str] = None
     _log: Logger
 
     def __init__(
         self,
         model_id: str,
         api_key: str,
         org_id: Optional[str] = None,
         log: Optional[Logger] = None,
     ) -> None:
         """
-        Initializes a new instance of the OpenAIChatCompletion class.
+        Initializes a new instance of the OpenAITextCompletion class.
 
         Arguments:
             model_id {str} -- OpenAI model name, see
                 https://platform.openai.com/docs/models
             api_key {str} -- OpenAI API key, see
                 https://platform.openai.com/account/api-keys
             org_id {Optional[str]} -- OpenAI organization ID.
                 This is usually optional unless your
                 account belongs to multiple organizations.
         """
         self._model_id = model_id
         self._api_key = api_key
         self._org_id = org_id
         self._log = log if log is not None else NullLogger()
-        self._messages = []
 
         self.open_ai_instance = self._setup_open_ai()
 
     def _setup_open_ai(self) -> Any:
         import openai
 
         openai.api_key = self._api_key
         if self._org_id is not None:
             openai.organization = self._org_id
 
         return openai
 
-    async def complete_chat_async(
-        self, messages: List[Tuple[str, str]], request_settings: ChatRequestSettings
+    async def complete_async(
+        self, prompt: str, request_settings: CompleteRequestSettings
     ) -> str:
         """
-        Completes the given user message. Returns a single string completion.
+        Completes the given prompt. Returns a single string completion.
+        Cannot return multiple completions. Cannot return logprobs.
 
         Arguments:
-            user_message {str} -- The message (from a user) to respond to.
-            request_settings {ChatRequestSettings} -- The request settings.
+            prompt {str} -- The prompt to complete.
+            request_settings {CompleteRequestSettings} -- The request settings.
 
         Returns:
             str -- The completed text.
         """
+        if not prompt:
+            raise ValueError("The prompt cannot be `None` or empty")
         if request_settings is None:
             raise ValueError("The request settings cannot be `None`")
 
         if request_settings.max_tokens < 1:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
                 "The max tokens must be greater than 0, "
                 f"but was {request_settings.max_tokens}",
             )
 
-        if len(messages) <= 0:
+        if request_settings.number_of_responses != 1:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
-                "To complete a chat you need at least one message",
+                "complete_async only supports a single completion, "
+                f"but {request_settings.number_of_responses} were requested",
             )
 
-        if messages[-1][0] != "user":
+        if request_settings.logprobs != 0:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
-                "The last message must be from the user",
+                "complete_async does not support logprobs, "
+                f"but logprobs={request_settings.logprobs} was requested",
             )
 
         model_args = {}
         if self.open_ai_instance.api_type in ["azure", "azure_ad"]:
             model_args["engine"] = self._model_id
         else:
             model_args["model"] = self._model_id
 
-        formatted_messages = [
-            {"role": role, "content": message} for role, message in messages
-        ]
-
         try:
-            response: Any = await self.open_ai_instance.ChatCompletion.acreate(
+            response: Any = await self.open_ai_instance.Completion.acreate(
                 **model_args,
-                messages=formatted_messages,
+                prompt=prompt,
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
+                stop=(
+                    request_settings.stop_sequences
+                    if request_settings.stop_sequences is not None
+                    and len(request_settings.stop_sequences) > 0
+                    else None
+                ),
             )
         except Exception as ex:
             raise AIException(
                 AIException.ErrorCodes.ServiceError,
-                "OpenAI service failed to complete the chat",
+                "OpenAI service failed to complete the prompt",
                 ex,
             )
 
         # TODO: tracking on token counts/etc.
 
-        return response.choices[0].message.content
+        return response.choices[0].text
+
+    # TODO: complete w/ multiple...
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,150 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
-from typing import Any, Optional
+from typing import Any, List, Optional, Tuple
 
-from semantic_kernel.ai.ai_exception import AIException
-from semantic_kernel.ai.complete_request_settings import CompleteRequestSettings
-from semantic_kernel.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.connectors.ai.ai_exception import AIException
+from semantic_kernel.connectors.ai.chat_completion_client_base import (
+    ChatCompletionClientBase,
+)
+from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
+from semantic_kernel.connectors.ai.complete_request_settings import (
+    CompleteRequestSettings,
+)
+from semantic_kernel.connectors.ai.text_completion_client_base import (
+    TextCompletionClientBase,
+)
 from semantic_kernel.utils.null_logger import NullLogger
 
 
-class OpenAITextCompletion(TextCompletionClientBase):
+class OpenAIChatCompletion(ChatCompletionClientBase, TextCompletionClientBase):
     _model_id: str
     _api_key: str
     _org_id: Optional[str] = None
     _log: Logger
 
     def __init__(
         self,
         model_id: str,
         api_key: str,
         org_id: Optional[str] = None,
         log: Optional[Logger] = None,
     ) -> None:
         """
-        Initializes a new instance of the OpenAITextCompletion class.
+        Initializes a new instance of the OpenAIChatCompletion class.
 
         Arguments:
             model_id {str} -- OpenAI model name, see
                 https://platform.openai.com/docs/models
             api_key {str} -- OpenAI API key, see
                 https://platform.openai.com/account/api-keys
             org_id {Optional[str]} -- OpenAI organization ID.
                 This is usually optional unless your
                 account belongs to multiple organizations.
         """
         self._model_id = model_id
         self._api_key = api_key
         self._org_id = org_id
         self._log = log if log is not None else NullLogger()
+        self._messages = []
 
         self.open_ai_instance = self._setup_open_ai()
 
     def _setup_open_ai(self) -> Any:
         import openai
 
         openai.api_key = self._api_key
         if self._org_id is not None:
             openai.organization = self._org_id
 
         return openai
 
-    async def complete_simple_async(
-        self, prompt: str, request_settings: CompleteRequestSettings
+    async def complete_chat_async(
+        self, messages: List[Tuple[str, str]], request_settings: ChatRequestSettings
     ) -> str:
         """
-        Completes the given prompt. Returns a single string completion.
-        Cannot return multiple completions. Cannot return logprobs.
+        Completes the given user message. Returns a single string completion.
 
         Arguments:
-            prompt {str} -- The prompt to complete.
-            request_settings {CompleteRequestSettings} -- The request settings.
+            user_message {str} -- The message (from a user) to respond to.
+            request_settings {ChatRequestSettings} -- The request settings.
 
         Returns:
             str -- The completed text.
         """
-        if not prompt:
-            raise ValueError("The prompt cannot be `None` or empty")
         if request_settings is None:
             raise ValueError("The request settings cannot be `None`")
 
         if request_settings.max_tokens < 1:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
                 "The max tokens must be greater than 0, "
                 f"but was {request_settings.max_tokens}",
             )
 
-        if request_settings.number_of_responses != 1:
+        if len(messages) <= 0:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
-                "complete_simple_async only supports a single completion, "
-                f"but {request_settings.number_of_responses} were requested",
+                "To complete a chat you need at least one message",
             )
 
-        if request_settings.logprobs != 0:
+        if messages[-1][0] != "user":
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
-                "complete_simple_async does not support logprobs, "
-                f"but logprobs={request_settings.logprobs} was requested",
+                "The last message must be from the user",
             )
 
         model_args = {}
         if self.open_ai_instance.api_type in ["azure", "azure_ad"]:
             model_args["engine"] = self._model_id
         else:
             model_args["model"] = self._model_id
 
+        formatted_messages = [
+            {"role": role, "content": message} for role, message in messages
+        ]
+
         try:
-            response: Any = await self.open_ai_instance.Completion.acreate(
+            response: Any = await self.open_ai_instance.ChatCompletion.acreate(
                 **model_args,
-                prompt=prompt,
+                messages=formatted_messages,
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
-                stop=(
-                    request_settings.stop_sequences
-                    if request_settings.stop_sequences is not None
-                    and len(request_settings.stop_sequences) > 0
-                    else None
-                ),
             )
         except Exception as ex:
             raise AIException(
                 AIException.ErrorCodes.ServiceError,
-                "OpenAI service failed to complete the prompt",
+                "OpenAI service failed to complete the chat",
                 ex,
             )
 
         # TODO: tracking on token counts/etc.
 
-        return response.choices[0].text
+        return response.choices[0].message.content
 
-    # TODO: complete w/ multiple...
+    async def complete_async(
+        self, prompt: str, request_settings: CompleteRequestSettings
+    ) -> str:
+        """
+        Completes the given prompt. Returns a single string completion.
+        Cannot return multiple completions. Cannot return logprobs.
+
+        Arguments:
+            prompt {str} -- The prompt to complete.
+            request_settings {CompleteRequestSettings} -- The request settings.
+
+        Returns:
+            str -- The completed text.
+        """
+        prompt_to_message = [("user", prompt)]
+        chat_settings = ChatRequestSettings(
+            temperature=request_settings.temperature,
+            top_p=request_settings.top_p,
+            presence_penalty=request_settings.presence_penalty,
+            frequency_penalty=request_settings.frequency_penalty,
+            max_tokens=request_settings.max_tokens,
+        )
+        return await self.complete_chat_async(prompt_to_message, chat_settings)
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import Any, List, Optional
 
 from numpy import array, ndarray
 
-from semantic_kernel.ai.ai_exception import AIException
-from semantic_kernel.ai.embeddings.embedding_generator_base import (
+from semantic_kernel.connectors.ai.ai_exception import AIException
+from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
     EmbeddingGeneratorBase,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 
 
 class OpenAITextEmbedding(EmbeddingGeneratorBase):
     _model_id: str
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,35 @@
         {{time.minutes}}         => 15
         {{time.second}}          => 7
         {{time.seconds}}         => 7
         {{time.timeZoneOffset}}  => -0800
         {{time.timeZoneName}}    => PST
     """
 
-    @sk_function(description="Get the current time.")
+    @sk_function(description="Get the current date.")
     def date(self) -> str:
         """
         Get the current date
 
         Example:
             {{time.date}} => Sunday, 12 January, 2031
         """
         now = datetime.datetime.now()
         return now.strftime("%A, %d %B, %Y")
 
+    @sk_function(description="Get the current date.")
+    def today(self) -> str:
+        """
+        Get the current date
+
+        Example:
+            {{time.today}} => Sunday, 12 January, 2031
+        """
+        return self.date()
+
     @sk_function(description="Get the current date and time in the local time zone")
     def now(self) -> str:
         """
         Get the current date and time in the local time zone"
 
         Example:
             {{time.now}} => Sunday, January 12, 2031 9:15 PM
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import inspect
 from logging import Logger
 from typing import Any, Dict, Optional
 
-from semantic_kernel.ai.ai_exception import AIException
-from semantic_kernel.ai.chat_completion_client_base import ChatCompletionClientBase
-from semantic_kernel.ai.chat_request_settings import ChatRequestSettings
-from semantic_kernel.ai.complete_request_settings import CompleteRequestSettings
-from semantic_kernel.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.connectors.ai.ai_exception import AIException
+from semantic_kernel.connectors.ai.chat_completion_client_base import (
+    ChatCompletionClientBase,
+)
+from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
+from semantic_kernel.connectors.ai.complete_request_settings import (
+    CompleteRequestSettings,
+)
+from semantic_kernel.connectors.ai.text_completion_client_base import (
+    TextCompletionClientBase,
+)
 from semantic_kernel.kernel_base import KernelBase
 from semantic_kernel.kernel_config import KernelConfig
 from semantic_kernel.kernel_exception import KernelException
 from semantic_kernel.kernel_extensions import KernelExtensions
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.memory.null_memory import NullMemory
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
@@ -264,54 +270,54 @@
 
         # Connect the function to the current kernel skill
         # collection, in case the function is invoked manually
         # without a context and without a way to find other functions.
         function.set_default_skill_collection(self.skills)
 
         if function_config.has_chat_prompt:
-            backend = self._config.get_ai_backend(
+            service = self._config.get_ai_service(
                 ChatCompletionClientBase,
-                function_config.prompt_template_config.default_backends[0]
-                if len(function_config.prompt_template_config.default_backends) > 0
+                function_config.prompt_template_config.default_services[0]
+                if len(function_config.prompt_template_config.default_services) > 0
                 else None,
             )
 
             function.set_chat_configuration(
                 ChatRequestSettings.from_completion_config(
                     function_config.prompt_template_config.completion
                 )
             )
 
-            if backend is None:
+            if service is None:
                 raise AIException(
                     AIException.ErrorCodes.InvalidConfiguration,
-                    "Could not load chat backend, unable to prepare semantic function. "
+                    "Could not load chat service, unable to prepare semantic function. "
                     "Function description: "
                     "{function_config.prompt_template_config.description}",
                 )
 
-            function.set_chat_backend(lambda: backend(self))
+            function.set_chat_service(lambda: service(self))
         else:
-            backend = self._config.get_ai_backend(
+            service = self._config.get_ai_service(
                 TextCompletionClientBase,
-                function_config.prompt_template_config.default_backends[0]
-                if len(function_config.prompt_template_config.default_backends) > 0
+                function_config.prompt_template_config.default_services[0]
+                if len(function_config.prompt_template_config.default_services) > 0
                 else None,
             )
 
             function.set_ai_configuration(
                 CompleteRequestSettings.from_completion_config(
                     function_config.prompt_template_config.completion
                 )
             )
 
-            if backend is None:
+            if service is None:
                 raise AIException(
                     AIException.ErrorCodes.InvalidConfiguration,
-                    "Could not load text backend, unable to prepare semantic function. "
+                    "Could not load text service, unable to prepare semantic function. "
                     "Function description: "
                     "{function_config.prompt_template_config.description}",
                 )
 
-            function.set_ai_backend(lambda: backend(self))
+            function.set_ai_service(lambda: service(self))
 
         return function
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_config.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,260 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Type, TypeVar, Union
 
-from semantic_kernel.ai.chat_completion_client_base import ChatCompletionClientBase
-from semantic_kernel.ai.embeddings.embedding_generator_base import (
+from semantic_kernel.connectors.ai.chat_completion_client_base import (
+    ChatCompletionClientBase,
+)
+from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
     EmbeddingGeneratorBase,
 )
-from semantic_kernel.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.connectors.ai.text_completion_client_base import (
+    TextCompletionClientBase,
+)
 from semantic_kernel.reliability.pass_through_without_retry import (
     PassThroughWithoutRetry,
 )
 from semantic_kernel.reliability.retry_mechanism import RetryMechanism
 
 if TYPE_CHECKING:
     from semantic_kernel.kernel_base import KernelBase
 
 
 T = TypeVar("T")
 
 
 class KernelConfig:
     def __init__(self) -> None:
-        self._text_backends: Dict[
+        self._text_services: Dict[
             str, Callable[["KernelBase"], TextCompletionClientBase]
         ] = {}
-        self._chat_backends: Dict[
+        self._chat_services: Dict[
             str, Callable[["KernelBase"], ChatCompletionClientBase]
         ] = {}
-        self._embedding_backends: Dict[
+        self._embedding_services: Dict[
             str, Callable[["KernelBase"], EmbeddingGeneratorBase]
         ] = {}
 
-        self._default_text_backend: Optional[str] = None
-        self._default_chat_backend: Optional[str] = None
-        self._default_embedding_backend: Optional[str] = None
+        self._default_text_service: Optional[str] = None
+        self._default_chat_service: Optional[str] = None
+        self._default_embedding_service: Optional[str] = None
 
         self._retry_mechanism: RetryMechanism = PassThroughWithoutRetry()
 
-    def get_ai_backend(
+    def get_ai_service(
         self, type: Type[T], service_id: Optional[str] = None
     ) -> Callable[["KernelBase"], T]:
         matching_type = {}
         if type == TextCompletionClientBase:
-            service_id = service_id or self._default_text_backend
-            matching_type = self._text_backends
+            service_id = service_id or self._default_text_service
+            matching_type = self._text_services
         elif type == ChatCompletionClientBase:
-            service_id = service_id or self._default_chat_backend
-            matching_type = self._chat_backends
+            service_id = service_id or self._default_chat_service
+            matching_type = self._chat_services
         elif type == EmbeddingGeneratorBase:
-            service_id = service_id or self._default_embedding_backend
-            matching_type = self._embedding_backends
+            service_id = service_id or self._default_embedding_service
+            matching_type = self._embedding_services
         else:
-            raise ValueError(f"Unknown backend type: {type.__name__}")
+            raise ValueError(f"Unknown AI service type: {type.__name__}")
 
         if service_id not in matching_type:
             raise ValueError(
-                f"{type.__name__} backend with service_id '{service_id}' not found"
+                f"{type.__name__} service with service_id '{service_id}' not found"
             )
 
         return matching_type[service_id]
 
-    def all_text_backends(self) -> List[str]:
-        return list(self._text_backends.keys())
+    def all_text_services(self) -> List[str]:
+        return list(self._text_services.keys())
 
-    def all_chat_backends(self) -> List[str]:
-        return list(self._chat_backends.keys())
+    def all_chat_services(self) -> List[str]:
+        return list(self._chat_services.keys())
 
-    def all_embedding_backends(self) -> List[str]:
-        return list(self._embedding_backends.keys())
+    def all_embedding_services(self) -> List[str]:
+        return list(self._embedding_services.keys())
 
-    def add_text_backend(
+    def add_text_service(
         self,
         service_id: str,
-        backend: Union[
+        service: Union[
             TextCompletionClientBase, Callable[["KernelBase"], TextCompletionClientBase]
         ],
         overwrite: bool = True,
     ) -> "KernelConfig":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
-        if not overwrite and service_id in self._text_backends:
+        if not overwrite and service_id in self._text_services:
             raise ValueError(
-                f"Text backend with service_id '{service_id}' already exists"
+                f"Text service with service_id '{service_id}' already exists"
             )
 
-        self._text_backends[service_id] = (
-            backend if isinstance(backend, Callable) else lambda _: backend
+        self._text_services[service_id] = (
+            service if isinstance(service, Callable) else lambda _: service
         )
-        if self._default_text_backend is None:
-            self._default_text_backend = service_id
+        if self._default_text_service is None:
+            self._default_text_service = service_id
 
         return self
 
-    def add_chat_backend(
+    def add_chat_service(
         self,
         service_id: str,
-        backend: Union[
+        service: Union[
             ChatCompletionClientBase, Callable[["KernelBase"], ChatCompletionClientBase]
         ],
         overwrite: bool = True,
     ) -> "KernelConfig":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
-        if not overwrite and service_id in self._chat_backends:
+        if not overwrite and service_id in self._chat_services:
             raise ValueError(
-                f"Chat backend with service_id '{service_id}' already exists"
+                f"Chat service with service_id '{service_id}' already exists"
             )
 
-        self._chat_backends[service_id] = (
-            backend if isinstance(backend, Callable) else lambda _: backend
+        self._chat_services[service_id] = (
+            service if isinstance(service, Callable) else lambda _: service
         )
-        if self._default_chat_backend is None:
-            self._default_chat_backend = service_id
+        if self._default_chat_service is None:
+            self._default_chat_service = service_id
+
+        if isinstance(service, TextCompletionClientBase):
+            self.add_text_service(service_id, service)
+            if self._default_text_service is None:
+                self._default_text_service = service_id
 
         return self
 
-    def add_embedding_backend(
+    def add_embedding_service(
         self,
         service_id: str,
-        backend: Union[
+        service: Union[
             EmbeddingGeneratorBase, Callable[["KernelBase"], EmbeddingGeneratorBase]
         ],
         overwrite: bool = False,
     ) -> "KernelConfig":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
-        if not overwrite and service_id in self._embedding_backends:
+        if not overwrite and service_id in self._embedding_services:
             raise ValueError(
-                f"Embedding backend with service_id '{service_id}' already exists"
+                f"Embedding service with service_id '{service_id}' already exists"
             )
 
-        self._embedding_backends[service_id] = (
-            backend if isinstance(backend, Callable) else lambda _: backend
+        self._embedding_services[service_id] = (
+            service if isinstance(service, Callable) else lambda _: service
         )
-        if self._default_embedding_backend is None:
-            self._default_embedding_backend = service_id
+        if self._default_embedding_service is None:
+            self._default_embedding_service = service_id
 
         return self
 
     # TODO: look harder at retry stuff
 
-    def set_default_text_backend(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._text_backends:
+    def set_default_text_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._text_services:
             raise ValueError(
-                f"AI backend with service_id '{service_id}' does not exist"
+                f"AI service with service_id '{service_id}' does not exist"
             )
 
-        self._default_text_backend = service_id
+        self._default_text_service = service_id
         return self
 
-    def set_default_chat_backend(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._chat_backends:
+    def set_default_chat_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._chat_services:
             raise ValueError(
-                f"AI backend with service_id '{service_id}' does not exist"
+                f"AI service with service_id '{service_id}' does not exist"
             )
 
-        self._default_chat_backend = service_id
+        self._default_chat_service = service_id
         return self
 
-    def set_default_embedding_backend(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._embedding_backends:
+    def set_default_embedding_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._embedding_services:
             raise ValueError(
-                f"AI backend with service_id '{service_id}' does not exist"
+                f"AI service with service_id '{service_id}' does not exist"
             )
 
-        self._default_embedding_backend = service_id
+        self._default_embedding_service = service_id
         return self
 
-    def get_text_backend_service_id(self, service_id: Optional[str] = None) -> str:
-        if service_id is None or service_id not in self._text_backends:
-            if self._default_text_backend is None:
-                raise ValueError("No default text backend is set")
-            return self._default_text_backend
+    def get_text_service_service_id(self, service_id: Optional[str] = None) -> str:
+        if service_id is None or service_id not in self._text_services:
+            if self._default_text_service is None:
+                raise ValueError("No default text service is set")
+            return self._default_text_service
 
         return service_id
 
-    def get_chat_backend_service_id(self, service_id: Optional[str] = None) -> str:
-        if service_id is None or service_id not in self._chat_backends:
-            if self._default_chat_backend is None:
-                raise ValueError("No default chat backend is set")
-            return self._default_chat_backend
+    def get_chat_service_service_id(self, service_id: Optional[str] = None) -> str:
+        if service_id is None or service_id not in self._chat_services:
+            if self._default_chat_service is None:
+                raise ValueError("No default chat service is set")
+            return self._default_chat_service
 
         return service_id
 
-    def get_embedding_backend_service_id(self, service_id: Optional[str] = None) -> str:
-        if service_id is None or service_id not in self._embedding_backends:
-            if self._default_embedding_backend is None:
-                raise ValueError("No default embedding backend is set")
-            return self._default_embedding_backend
+    def get_embedding_service_id(self, service_id: Optional[str] = None) -> str:
+        if service_id is None or service_id not in self._embedding_services:
+            if self._default_embedding_service is None:
+                raise ValueError("No default embedding service is set")
+            return self._default_embedding_service
 
         return service_id
 
-    def remove_text_backend(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._text_backends:
+    def remove_text_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._text_services:
             raise ValueError(
-                f"AI backend with service_id '{service_id}' does not exist"
+                f"AI service with service_id '{service_id}' does not exist"
             )
 
-        del self._text_backends[service_id]
-        if self._default_text_backend == service_id:
-            self._default_text_backend = next(iter(self._text_backends), None)
+        del self._text_services[service_id]
+        if self._default_text_service == service_id:
+            self._default_text_service = next(iter(self._text_services), None)
         return self
 
-    def remove_chat_backend(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._chat_backends:
+    def remove_chat_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._chat_services:
             raise ValueError(
-                f"AI backend with service_id '{service_id}' does not exist"
+                f"AI service with service_id '{service_id}' does not exist"
             )
 
-        del self._chat_backends[service_id]
-        if self._default_chat_backend == service_id:
-            self._default_chat_backend = next(iter(self._chat_backends), None)
+        del self._chat_services[service_id]
+        if self._default_chat_service == service_id:
+            self._default_chat_service = next(iter(self._chat_services), None)
         return self
 
-    def remove_embedding_backend(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._embedding_backends:
+    def remove_embedding_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._embedding_services:
             raise ValueError(
-                f"AI backend with service_id '{service_id}' does not exist"
+                f"AI service with service_id '{service_id}' does not exist"
             )
 
-        del self._embedding_backends[service_id]
-        if self._default_embedding_backend == service_id:
-            self._default_embedding_backend = next(iter(self._embedding_backends), None)
+        del self._embedding_services[service_id]
+        if self._default_embedding_service == service_id:
+            self._default_embedding_service = next(iter(self._embedding_services), None)
         return self
 
-    def clear_all_text_backends(self) -> "KernelConfig":
-        self._text_backends = {}
-        self._default_text_backend = None
+    def clear_all_text_services(self) -> "KernelConfig":
+        self._text_services = {}
+        self._default_text_service = None
         return self
 
-    def clear_all_chat_backends(self) -> "KernelConfig":
-        self._chat_backends = {}
-        self._default_chat_backend = None
+    def clear_all_chat_services(self) -> "KernelConfig":
+        self._chat_services = {}
+        self._default_chat_service = None
         return self
 
-    def clear_all_embedding_backends(self) -> "KernelConfig":
-        self._embedding_backends = {}
-        self._default_embedding_backend = None
+    def clear_all_embedding_services(self) -> "KernelConfig":
+        self._embedding_services = {}
+        self._default_embedding_service = None
         return self
 
-    def clear_all_backends(self) -> "KernelConfig":
-        self._text_backends = {}
-        self._chat_backends = {}
-        self._embedding_backends = {}
+    def clear_all_services(self) -> "KernelConfig":
+        self._text_services = {}
+        self._chat_services = {}
+        self._embedding_services = {}
 
-        self._default_text_backend = None
-        self._default_chat_backend = None
-        self._default_embedding_backend = None
+        self._default_text_service = None
+        self._default_chat_service = None
+        self._default_embedding_service = None
 
         return self
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_exception.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         FunctionOverloadNotSupported = 1
         # Function not available.
         FunctionNotAvailable = 2
         # Function type not supported.
         FunctionTypeNotSupported = 3
         # Invalid function type.
         InvalidFunctionType = 4
-        # Invalid backend configuration.
-        InvalidBackendConfiguration = 5
-        # Backend not found.
-        BackendNotFound = 6
+        # Invalid service configuration.
+        InvalidServiceConfiguration = 5
+        # Service not found.
+        ServiceNotFound = 6
         # Skill collection not set.
         SkillCollectionNotSet = 7
         # Ambiguous implementation.
         AmbiguousImplementation = 8
 
     # The error code.
     _error_code: ErrorCodes
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/import_skills.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/import_skills.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import glob
 import importlib
 import inspect
 import os
-import sys
 from typing import Dict
 
 from semantic_kernel.kernel_extensions.extends_kernel import ExtendsKernel
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.semantic_functions.prompt_template import PromptTemplate
 from semantic_kernel.semantic_functions.prompt_template_config import (
     PromptTemplateConfig,
@@ -19,51 +18,52 @@
 from semantic_kernel.utils.validation import validate_skill_name
 
 
 class ImportSkills(ExtendsKernel):
     def import_native_skill_from_directory(
         self, parent_directory: str, skill_directory_name: str
     ) -> Dict[str, SKFunctionBase]:
-        PYTHON_FILE = "native_function.py"
-
+        MODULE_NAME = "native_function"
         kernel = self.kernel()
 
         validate_skill_name(skill_directory_name)
 
         skill_directory = os.path.abspath(
             os.path.join(parent_directory, skill_directory_name)
         )
-        native_py_file_path = os.path.join(skill_directory, PYTHON_FILE)
+        native_py_file_path = os.path.join(skill_directory, f"{MODULE_NAME}.py")
 
         if not os.path.exists(native_py_file_path):
             raise ValueError(
                 f"Native Skill Python File does not exist: {native_py_file_path}"
             )
 
         skill_name = os.path.basename(skill_directory)
         try:
-            sys.path.append(skill_directory)
-            module_name = os.path.splitext(os.path.basename(native_py_file_path))[0]
-            module = importlib.import_module(module_name)
+            spec = importlib.util.spec_from_file_location(
+                MODULE_NAME, native_py_file_path
+            )
+            module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(module)
+
+            class_name = next(
+                (
+                    name
+                    for name, cls in inspect.getmembers(module, inspect.isclass)
+                    if cls.__module__ == MODULE_NAME
+                ),
+                None,
+            )
+            if class_name:
+                skill_obj = getattr(module, class_name)()
+                return kernel.import_skill(skill_obj, skill_name)
         except Exception:
-            return {}
-        finally:
-            sys.path.remove(skill_directory)
-
-        # Find the class in the module
-        classes = inspect.getmembers(module, inspect.isclass)
-        class_name = next(
-            (name for name, cls in classes if inspect.getmodule(cls) == module), None
-        )
+            pass
 
-        if class_name:
-            skill_obj = getattr(module, class_name)()
-            return kernel.import_skill(skill_obj, skill_name)
-        else:
-            return {}
+        return {}
 
     def import_semantic_skill_from_directory(
         self, parent_directory: str, skill_directory_name: str
     ) -> Dict[str, SKFunctionBase]:
         CONFIG_FILE = "config.json"
         PROMPT_FILE = "skprompt.txt"
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import Optional
 
-from semantic_kernel.ai.embeddings.embedding_generator_base import (
+from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
     EmbeddingGeneratorBase,
 )
 from semantic_kernel.kernel_extensions.extends_kernel import ExtendsKernel
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.memory.semantic_text_memory import SemanticTextMemory
 
 
@@ -15,27 +15,25 @@
         self,
         storage: MemoryStoreBase,
         embeddings_generator: Optional[EmbeddingGeneratorBase] = None,
     ) -> None:
         kernel = self.kernel()
 
         if embeddings_generator is None:
-            backend_label = kernel.config.get_embedding_backend_service_id()
-            if not backend_label:
-                raise ValueError(
-                    "The embedding backend label cannot be `None` or empty"
-                )
+            service_id = kernel.config.get_embedding_service_id()
+            if not service_id:
+                raise ValueError("The embedding service id cannot be `None` or empty")
 
-            embeddings_backend = kernel.config.get_ai_backend(
-                EmbeddingGeneratorBase, backend_label
+            embeddings_service = kernel.config.get_ai_service(
+                EmbeddingGeneratorBase, service_id
             )
-            if not embeddings_backend:
-                raise ValueError(f"AI configuration is missing for: {backend_label}")
+            if not embeddings_service:
+                raise ValueError(f"AI configuration is missing for: {service_id}")
 
-            embeddings_generator = embeddings_backend(kernel)
+            embeddings_generator = embeddings_service(kernel)
 
         if storage is None:
             raise ValueError("The storage instance provided cannot be `None`")
         if embeddings_generator is None:
             raise ValueError("The embedding generator cannot be `None`")
 
         kernel.register_memory(SemanticTextMemory(storage, embeddings_generator))
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,23 +22,22 @@
     async def save_reference_async(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
         description: Optional[str] = None,
-        # TODO: ctoken?
     ) -> None:
         pass
 
     @abstractmethod
     async def get_async(
         self,
         collection: str,
-        query: str,  # TODO: ctoken?
+        query: str,
     ) -> Optional[MemoryQueryResult]:
         pass
 
     @abstractmethod
     async def search_async(
         self,
         collection: str,
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 
 import asyncio
 import threading
 from enum import Enum
 from logging import Logger
 from typing import Any, Callable, List, Optional, cast
 
-from semantic_kernel.ai.chat_completion_client_base import ChatCompletionClientBase
-from semantic_kernel.ai.chat_request_settings import ChatRequestSettings
-from semantic_kernel.ai.complete_request_settings import CompleteRequestSettings
-from semantic_kernel.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.connectors.ai.chat_completion_client_base import (
+    ChatCompletionClientBase,
+)
+from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
+from semantic_kernel.connectors.ai.complete_request_settings import (
+    CompleteRequestSettings,
+)
+from semantic_kernel.connectors.ai.text_completion_client_base import (
+    TextCompletionClientBase,
+)
 from semantic_kernel.kernel_exception import KernelException
 from semantic_kernel.memory.null_memory import NullMemory
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.delegate_handlers import DelegateHandlers
 from semantic_kernel.orchestration.delegate_inference import DelegateInference
 from semantic_kernel.orchestration.delegate_types import DelegateTypes
@@ -37,17 +43,17 @@
     """
 
     _parameters: List[ParameterView]
     _delegate_type: DelegateTypes
     _function: Callable[..., Any]
     _skill_collection: Optional[ReadOnlySkillCollectionBase]
     _log: Logger
-    _ai_backend: Optional[TextCompletionClientBase]
+    _ai_service: Optional[TextCompletionClientBase]
     _ai_request_settings: CompleteRequestSettings
-    _chat_backend: Optional[ChatCompletionClientBase]
+    _chat_service: Optional[ChatCompletionClientBase]
     _chat_request_settings: ChatRequestSettings
 
     @staticmethod
     def from_native_method(method, skill_name="", log=None) -> "SKFunction":
         if method is None:
             raise ValueError("Method cannot be `None`")
 
@@ -95,15 +101,15 @@
         log: Optional[Logger] = None,
     ) -> "SKFunction":
         if function_config is None:
             raise ValueError("Function configuration cannot be `None`")
 
         async def _local_func(client, request_settings, context):
             if client is None:
-                raise ValueError("AI LLM backend cannot be `None`")
+                raise ValueError("AI LLM service cannot be `None`")
 
             try:
                 if function_config.has_chat_prompt:
                     as_chat_prompt = cast(
                         ChatPromptTemplate, function_config.prompt_template
                     )
 
@@ -121,17 +127,15 @@
                     as_chat_prompt.add_user_message(content)
                     as_chat_prompt.add_assistant_message(completion)
 
                     # Update context
                     context.variables.update(completion)
                 else:
                     prompt = await function_config.prompt_template.render_async(context)
-                    completion = await client.complete_simple_async(
-                        prompt, request_settings
-                    )
+                    completion = await client.complete_async(prompt, request_settings)
                     context.variables.update(completion)
             except Exception as e:
                 # TODO: "critical exceptions"
                 context.fail(str(e), e)
 
             return context
 
@@ -190,41 +194,41 @@
         self._parameters = parameters
         self._description = description
         self._skill_name = skill_name
         self._name = function_name
         self._is_semantic = is_semantic
         self._log = log if log is not None else NullLogger()
         self._skill_collection = None
-        self._ai_backend = None
+        self._ai_service = None
         self._ai_request_settings = CompleteRequestSettings()
-        self._chat_backend = None
+        self._chat_service = None
         self._chat_request_settings = ChatRequestSettings()
 
     def set_default_skill_collection(
         self, skills: ReadOnlySkillCollectionBase
     ) -> "SKFunction":
         self._skill_collection = skills
         return self
 
-    def set_ai_backend(
-        self, ai_backend: Callable[[], TextCompletionClientBase]
+    def set_ai_service(
+        self, ai_service: Callable[[], TextCompletionClientBase]
     ) -> "SKFunction":
-        if ai_backend is None:
-            raise ValueError("AI LLM backend factory cannot be `None`")
+        if ai_service is None:
+            raise ValueError("AI LLM service factory cannot be `None`")
         self._verify_is_semantic()
-        self._ai_backend = ai_backend()
+        self._ai_service = ai_service()
         return self
 
-    def set_chat_backend(
-        self, chat_backend: Callable[[], ChatCompletionClientBase]
+    def set_chat_service(
+        self, chat_service: Callable[[], ChatCompletionClientBase]
     ) -> "SKFunction":
-        if chat_backend is None:
-            raise ValueError("Chat LLM backend factory cannot be `None`")
+        if chat_service is None:
+            raise ValueError("Chat LLM service factory cannot be `None`")
         self._verify_is_semantic()
-        self._chat_backend = chat_backend()
+        self._chat_service = chat_service()
         return self
 
     def set_ai_configuration(self, settings: CompleteRequestSettings) -> "SKFunction":
         if settings is None:
             raise ValueError("AI LLM request settings cannot be `None`")
         self._verify_is_semantic()
         self._ai_request_settings = settings
@@ -275,15 +279,14 @@
     ) -> SKContext:
         if context is None:
             context = SKContext(
                 variables=ContextVariables("") if variables is None else variables,
                 skill_collection=self._skill_collection,
                 memory=memory if memory is not None else NullMemory.instance,
                 logger=log if log is not None else self._log,
-                # TODO: ctoken?
             )
         else:
             # If context is passed, we need to merge the variables
             if variables is not None:
                 context._variables = variables.merge_or_overwrite(
                     new_vars=context._variables, overwrite=False
                 )
@@ -322,15 +325,14 @@
     ) -> SKContext:
         if context is None:
             context = SKContext(
                 variables=ContextVariables("") if variables is None else variables,
                 skill_collection=self._skill_collection,
                 memory=memory if memory is not None else NullMemory.instance,
                 logger=log if log is not None else self._log,
-                # TODO: ctoken?
             )
         else:
             # If context is passed, we need to merge the variables
             if variables is not None:
                 context._variables = variables.merge_or_overwrite(
                     new_vars=context._variables, overwrite=False
                 )
@@ -351,28 +353,28 @@
 
     async def _invoke_semantic_async(self, context, settings):
         self._verify_is_semantic()
 
         self._ensure_context_has_skills(context)
 
         if settings is None:
-            if self._ai_backend is not None:
+            if self._ai_service is not None:
                 settings = self._ai_request_settings
-            elif self._chat_backend is not None:
+            elif self._chat_service is not None:
                 settings = self._chat_request_settings
             else:
                 raise KernelException(
                     KernelException.ErrorCodes.UnknownError,
-                    "Semantic functions must have either an AI backend or Chat backend",
+                    "Semantic functions must have either an AI service or Chat service",
                 )
 
-        backend = (
-            self._ai_backend if self._ai_backend is not None else self._chat_backend
+        service = (
+            self._ai_service if self._ai_service is not None else self._chat_service
         )
-        new_context = await self._function(backend, settings, context)
+        new_context = await self._function(service, settings, context)
         context.variables.merge_or_overwrite(new_context.variables)
         return context
 
     async def _invoke_native_async(self, context):
         self._verify_is_native()
 
         self._ensure_context_has_skills(context)
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import ABC, abstractmethod
 from logging import Logger
 from typing import TYPE_CHECKING, Callable, Optional
 
-from semantic_kernel.ai.complete_request_settings import CompleteRequestSettings
-from semantic_kernel.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.connectors.ai.complete_request_settings import (
+    CompleteRequestSettings,
+)
+from semantic_kernel.connectors.ai.text_completion_client_base import (
+    TextCompletionClientBase,
+)
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.skill_definition.function_view import FunctionView
 
 if TYPE_CHECKING:
     from semantic_kernel.skill_definition.read_only_skill_collection_base import (
@@ -76,15 +80,15 @@
         the function might still involve AI calls.
         """
         pass
 
     @property
     @abstractmethod
     def request_settings(self) -> CompleteRequestSettings:
-        """AI backend settings"""
+        """AI service settings"""
         pass
 
     @abstractmethod
     def describe() -> FunctionView:
         """
         Returns a description of the function,
         including its parameters
@@ -99,15 +103,14 @@
         self,
         input: Optional[str] = None,
         variables: ContextVariables = None,
         context: Optional[SKContext] = None,
         memory: Optional[SemanticTextMemoryBase] = None,
         settings: Optional[CompleteRequestSettings] = None,
         log: Optional[Logger] = None,
-        # TODO: ctoken
     ) -> SKContext:
         """
         Invokes the function with an explicit string input
         Keyword Arguments:
             input {str} -- The explicit string input (default: {None})
             variables {ContextVariables} -- The custom input
             context {SKContext} -- The context to use
@@ -125,15 +128,14 @@
         self,
         input: Optional[str] = None,
         variables: ContextVariables = None,
         context: Optional[SKContext] = None,
         memory: Optional[SemanticTextMemoryBase] = None,
         settings: Optional[CompleteRequestSettings] = None,
         log: Optional[Logger] = None,
-        # TODO: ctoken
     ) -> SKContext:
         """
         Invokes the function with an explicit string input
         Keyword Arguments:
             input {str} -- The explicit string input (default: {None})
             variables {ContextVariables} -- The custom input
             context {SKContext} -- The context to use
@@ -161,24 +163,24 @@
 
         Returns:
             SKFunctionBase -- The function instance
         """
         pass
 
     @abstractmethod
-    def set_ai_backend(
-        self, backend_factory: Callable[[], TextCompletionClientBase]
+    def set_ai_service(
+        self, service_factory: Callable[[], TextCompletionClientBase]
     ) -> "SKFunctionBase":
         """
-        Sets the AI backend used by the semantic function, passing in a factory
+        Sets the AI service used by the semantic function, passing in a factory
         method. The factory allows us to lazily instantiate the client and to
         properly handle its disposal
 
         Arguments:
-            backend_factory -- AI backend factory
+            service_factory -- AI service factory
 
         Returns:
             SKFunctionBase -- The function instance
         """
         pass
 
     @abstractmethod
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     schema: int = 1
     type: str = "completion"
     description: str = ""
     completion: "PromptTemplateConfig.CompletionConfig" = field(
         default_factory=CompletionConfig
     )
-    default_backends: List[str] = field(default_factory=list)
+    default_services: List[str] = field(default_factory=list)
     input: "PromptTemplateConfig.InputConfig" = field(default_factory=InputConfig)
 
     @staticmethod
     def from_dict(data: dict) -> "PromptTemplateConfig":
         config = PromptTemplateConfig()
         config.schema = data.get("schema")
         config.type = data.get("type")
@@ -48,15 +48,15 @@
         completion_dict = data["completion"]
         config.completion.temperature = completion_dict.get("temperature")
         config.completion.top_p = completion_dict.get("top_p")
         config.completion.presence_penalty = completion_dict.get("presence_penalty")
         config.completion.frequency_penalty = completion_dict.get("frequency_penalty")
         config.completion.max_tokens = completion_dict.get("max_tokens")
         config.completion.stop_sequences = completion_dict.get("stop_sequences", [])
-        config.default_backends = data.get("default_backends", [])
+        config.default_services = data.get("default_services", [])
 
         # Some skills may not have input parameters defined
         config.input = PromptTemplateConfig.InputConfig()
         config.input.parameters = []
         if data.get("input") is not None:
             for parameter in data["input"]["parameters"]:
                 if "name" in parameter:
```

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.5.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.4.dev0/PKG-INFO` & `semantic_kernel-0.2.5.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.2.4.dev0
+Version: 0.2.5.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: transformers (>=4.28.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Get Started with Semantic Kernel ⚡
 
 Install the latest package:
 
     python -m pip install --upgrade semantic-kernel
 
 
-# AI backends
+# AI Services
 
 ## OpenAI / Azure OpenAI API keys
 
 Make sure you have an
 [Open AI API Key](https://openai.com/api/) or
 [Azure Open AI service key](https://learn.microsoft.com/azure/cognitive-services/openai/quickstart?pivots=rest-api)
 
@@ -40,25 +43,25 @@
 AZURE_OPENAI_API_KEY=""
 ```
 
 # Running a prompt
 
 ```python
 import semantic_kernel as sk
-from semantic_kernel.ai.open_ai import OpenAITextCompletion, AzureTextCompletion
+from semantic_kernel.connectors.ai.open_ai import OpenAITextCompletion, AzureTextCompletion
 
 kernel = sk.Kernel()
 
-# Prepare OpenAI backend using credentials stored in the `.env` file
+# Prepare OpenAI service using credentials stored in the `.env` file
 api_key, org_id = sk.openai_settings_from_dot_env()
-kernel.config.add_text_backend("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
+kernel.config.add_text_service("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
 
 # Alternative using Azure:
 # deployment, api_key, endpoint = sk.azure_openai_settings_from_dot_env()
-# kernel.config.add_text_backend("dv", AzureTextCompletion(deployment, endpoint, api_key))
+# kernel.config.add_text_service("dv", AzureTextCompletion(deployment, endpoint, api_key))
 
 # Wrap your prompt in a function
 prompt = kernel.create_semantic_function("""
 1) A robot may not injure a human being or, through inaction,
 allow a human being to come to harm.
 
 2) A robot must obey orders given it by human beings except where
```

