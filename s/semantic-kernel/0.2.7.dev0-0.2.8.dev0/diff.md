# Comparing `tmp/semantic_kernel-0.2.7.dev0.tar.gz` & `tmp/semantic_kernel-0.2.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.7.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.8.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.7.dev0.tar` & `semantic_kernel-0.2.8.dev0.tar`

### file list

```diff
@@ -1,91 +1,93 @@
--rw-r--r--   0        0        0     1186 2023-05-08 22:48:20.447102 semantic_kernel-0.2.7.dev0/pip/README.md
--rw-r--r--   0        0        0      771 2023-05-08 22:53:10.954241 semantic_kernel-0.2.7.dev0/pyproject.toml
--rw-r--r--   0        0        0     1227 2023-05-07 18:39:02.913641 semantic_kernel-0.2.7.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-29 00:21:18.081250 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0      506 2023-04-29 00:21:18.081609 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-29 00:21:18.081920 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-29 00:21:18.082190 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-29 00:21:18.082773 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 23:48:28.652652 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     3837 2023-05-08 22:53:10.956135 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 22:53:10.957061 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-29 00:21:18.084928 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2782 2023-04-29 00:21:18.085471 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2774 2023-04-29 00:21:18.085835 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2769 2023-04-29 00:21:18.086154 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     5227 2023-04-30 23:48:28.654055 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4471 2023-04-30 23:48:28.654520 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2572 2023-05-02 00:49:03.449515 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      497 2023-04-30 23:48:28.654940 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      500 2023-05-07 18:39:02.916522 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-14 03:36:09.239029 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-26 22:16:44.328276 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 03:36:09.239829 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-14 03:36:09.240512 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5849 2023-04-29 00:21:18.088108 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    22020 2023-05-08 22:53:10.957924 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2099 2023-05-07 18:39:02.918601 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     1626 2023-04-29 00:21:18.089839 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-14 03:36:09.245082 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-14 03:36:09.245483 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     3822 2023-04-29 00:21:18.090797 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-14 03:36:09.246857 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1483 2023-05-07 18:39:02.919392 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-14 03:36:09.247903 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-30 23:48:28.656559 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3090 2023-05-07 18:39:02.920199 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2004 2023-05-07 18:39:02.921208 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-14 03:36:09.249612 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6045 2023-05-02 00:49:03.451205 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1196 2023-04-30 23:48:28.662481 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-04-30 23:48:28.664620 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-20 17:10:26.995186 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 03:36:09.253302 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-14 03:36:09.253662 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-14 03:36:09.254004 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 03:36:09.254344 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15915 2023-05-07 18:39:02.921883 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 23:48:28.668178 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-07 18:39:02.922653 semantic_kernel-0.2.7.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7275 2023-05-07 18:39:02.923105 semantic_kernel-0.2.7.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0      396 2023-05-07 18:39:02.923447 semantic_kernel-0.2.7.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      919 2023-04-14 03:36:09.255908 semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-14 03:36:09.256522 semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-14 03:36:09.256949 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 03:36:09.257319 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-14 03:36:09.257703 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-29 00:21:18.098358 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 03:36:09.258593 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 03:36:09.259027 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 03:36:09.259911 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-14 03:36:09.260336 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 03:36:09.261065 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 03:36:09.261495 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 03:36:09.261836 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-14 03:36:09.262309 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 03:36:09.262723 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 03:36:09.263484 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-14 03:36:09.263900 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-14 03:36:09.264367 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 03:36:09.264992 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 03:36:09.265522 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-29 00:21:18.098851 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-14 03:36:09.267164 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-14 03:36:09.267627 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 03:36:09.268042 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-14 03:36:09.268607 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 03:36:09.269045 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-14 03:36:09.269480 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 03:36:09.269880 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-14 03:36:09.270280 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-14 03:36:09.270855 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-14 03:36:09.271313 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-14 03:36:09.271775 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 23:48:28.669001 semantic_kernel-0.2.7.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 23:48:28.669455 semantic_kernel-0.2.7.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     6466 2023-04-30 23:48:28.670502 semantic_kernel-0.2.7.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-14 03:36:09.272351 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-14 03:36:09.272775 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-14 03:36:09.273176 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-14 03:36:09.274119 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.2.7.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-09 16:56:59.338396 semantic_kernel-0.2.8.dev0/pip/README.md
+-rw-r--r--   0        0        0      771 2023-05-15 18:37:29.801042 semantic_kernel-0.2.8.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1227 2023-05-09 16:56:59.344375 semantic_kernel-0.2.8.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-29 00:21:18.081250 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0      506 2023-04-29 00:21:18.081609 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-29 00:21:18.081920 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-29 00:21:18.082190 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-29 00:21:18.082773 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 23:48:28.652652 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3837 2023-05-09 16:56:59.345779 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-09 16:56:59.347133 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-29 00:21:18.084928 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-12 22:12:56.286732 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-12 22:12:56.289589 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-12 22:12:56.291500 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     5502 2023-05-12 22:12:56.293123 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4746 2023-05-12 22:12:56.294808 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-12 22:12:56.296394 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      497 2023-04-30 23:48:28.654940 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      711 2023-05-14 22:39:43.859053 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-14 22:39:43.859324 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2072 2023-04-14 03:36:09.239029 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-26 22:16:44.328276 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3164 2023-05-12 22:12:56.299298 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 03:36:09.239829 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-14 03:36:09.240512 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5849 2023-04-29 00:21:18.088108 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    22020 2023-05-09 16:56:59.349187 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2099 2023-05-09 16:56:59.349735 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0     1626 2023-04-29 00:21:18.089839 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-14 03:36:09.245082 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-14 03:36:09.245483 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     3822 2023-04-29 00:21:18.090797 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-14 03:36:09.246857 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1483 2023-05-09 16:56:59.350243 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-14 03:36:09.247903 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-30 23:48:28.656559 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3090 2023-05-09 16:56:59.350763 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2004 2023-05-09 16:56:59.351286 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-14 03:36:09.249612 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6045 2023-05-02 00:49:03.451205 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1196 2023-04-30 23:48:28.662481 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-12 22:12:56.301028 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-20 17:10:26.995186 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 03:36:09.253302 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-14 03:36:09.253662 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-14 03:36:09.254004 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 03:36:09.254344 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15915 2023-05-09 16:56:59.351884 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 23:48:28.668178 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-09 16:56:59.352379 semantic_kernel-0.2.8.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7275 2023-05-09 16:56:59.352682 semantic_kernel-0.2.8.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0      396 2023-05-09 16:56:59.352963 semantic_kernel-0.2.8.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      919 2023-04-14 03:36:09.255908 semantic_kernel-0.2.8.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-14 03:36:09.256522 semantic_kernel-0.2.8.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-14 03:36:09.256949 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 03:36:09.257319 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-14 03:36:09.257703 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-29 00:21:18.098358 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 03:36:09.258593 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 03:36:09.259027 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 03:36:09.259911 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-14 03:36:09.260336 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 03:36:09.261065 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 03:36:09.261495 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 03:36:09.261836 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-14 03:36:09.262309 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 03:36:09.262723 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 03:36:09.263484 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-14 03:36:09.263900 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-14 03:36:09.264367 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 03:36:09.264992 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 03:36:09.265522 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-29 00:21:18.098851 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-14 03:36:09.267164 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-14 03:36:09.267627 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 03:36:09.268042 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-14 03:36:09.268607 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 03:36:09.269045 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-14 03:36:09.269480 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 03:36:09.269880 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-14 03:36:09.270280 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-14 03:36:09.270855 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-14 03:36:09.271313 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-14 03:36:09.271775 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 23:48:28.669001 semantic_kernel-0.2.8.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 23:48:28.669455 semantic_kernel-0.2.8.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     6467 2023-05-12 22:13:00.910173 semantic_kernel-0.2.8.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-14 03:36:09.272351 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-14 03:36:09.272775 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-14 03:36:09.273176 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-14 03:36:09.274119 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.2.8.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.7.dev0/pip/README.md` & `semantic_kernel-0.2.8.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/pyproject.toml` & `semantic_kernel-0.2.8.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.2.7.dev"
+version = "0.2.8.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 from logging import Logger
-from typing import Any, Optional
+from typing import Optional
 
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion import (
-    OpenAIChatCompletion,
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion import (
+    OpenAITextCompletion,
 )
 
 
-class AzureChatCompletion(OpenAIChatCompletion):
+class AzureTextCompletion(OpenAITextCompletion):
     _endpoint: str
     _api_version: str
     _api_type: str
 
     def __init__(
         self,
         deployment_name: str,
         endpoint: Optional[str] = None,
         api_key: Optional[str] = None,
-        api_version: str = "2023-03-15-preview",
+        api_version: str = "2022-12-01",
         logger: Optional[Logger] = None,
         ad_auth=False,
     ) -> None:
         """
-        Initialize an AzureChatCompletion service.
+        Initialize an AzureTextCompletion service.
 
         You must provide:
         - A deployment_name, endpoint, and api_key (plus, optionally: ad_auth)
 
         :param deployment_name: The name of the Azure deployment. This value
             will correspond to the custom name you chose for your deployment
             when you deployed a model. This value can be found under
@@ -51,22 +51,18 @@
         if not api_key:
             raise ValueError("The Azure API key cannot be `None` or empty`")
         if not endpoint:
             raise ValueError("The Azure endpoint cannot be `None` or empty")
         if not endpoint.startswith("https://"):
             raise ValueError("The Azure endpoint must start with https://")
 
-        self._endpoint = endpoint
-        self._api_version = api_version
         self._api_type = "azure_ad" if ad_auth else "azure"
 
-        super().__init__(deployment_name, api_key, org_id=None, log=logger)
-
-    def _setup_open_ai(self) -> Any:
-        import openai
-
-        openai.api_type = self._api_type
-        openai.api_key = self._api_key
-        openai.api_base = self._endpoint
-        openai.api_version = self._api_version
-
-        return openai
+        super().__init__(
+            deployment_name,
+            api_key,
+            api_type=self._api_type,
+            api_version=api_version,
+            endpoint=endpoint,
+            org_id=None,
+            log=logger,
+        )
```

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 from logging import Logger
-from typing import Any, Optional
+from typing import Optional
 
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding import (
     OpenAITextEmbedding,
 )
 
 
 class AzureTextEmbedding(OpenAITextEmbedding):
@@ -51,22 +51,18 @@
         if not api_key:
             raise ValueError("The Azure API key cannot be `None` or empty`")
         if not endpoint:
             raise ValueError("The Azure endpoint cannot be `None` or empty")
         if not endpoint.startswith("https://"):
             raise ValueError("The Azure endpoint must start with https://")
 
-        self._endpoint = endpoint
-        self._api_version = api_version
         self._api_type = "azure_ad" if ad_auth else "azure"
 
-        super().__init__(deployment_name, api_key, org_id=None, log=logger)
-
-    def _setup_open_ai(self) -> Any:
-        import openai
-
-        openai.api_type = self._api_type
-        openai.api_key = self._api_key
-        openai.api_base = self._endpoint
-        openai.api_version = self._api_version
-
-        return openai
+        super().__init__(
+            deployment_name,
+            api_key,
+            api_type=self._api_type,
+            api_version=api_version,
+            endpoint=endpoint,
+            org_id=None,
+            log=logger,
+        )
```

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import Any, List, Optional, Tuple
 
+import openai
+
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.chat_completion_client_base import (
     ChatCompletionClientBase,
 )
 from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
@@ -17,21 +19,27 @@
 from semantic_kernel.utils.null_logger import NullLogger
 
 
 class OpenAIChatCompletion(ChatCompletionClientBase, TextCompletionClientBase):
     _model_id: str
     _api_key: str
     _org_id: Optional[str] = None
+    _api_type: Optional[str] = None
+    _api_version: Optional[str] = None
+    _endpoint: Optional[str] = None
     _log: Logger
 
     def __init__(
         self,
         model_id: str,
         api_key: str,
         org_id: Optional[str] = None,
+        api_type: Optional[str] = None,
+        api_version: Optional[str] = None,
+        endpoint: Optional[str] = None,
         log: Optional[Logger] = None,
     ) -> None:
         """
         Initializes a new instance of the OpenAIChatCompletion class.
 
         Arguments:
             model_id {str} -- OpenAI model name, see
@@ -41,28 +49,20 @@
             org_id {Optional[str]} -- OpenAI organization ID.
                 This is usually optional unless your
                 account belongs to multiple organizations.
         """
         self._model_id = model_id
         self._api_key = api_key
         self._org_id = org_id
+        self._api_type = api_type
+        self._api_version = api_version
+        self._endpoint = endpoint
         self._log = log if log is not None else NullLogger()
         self._messages = []
 
-        self.open_ai_instance = self._setup_open_ai()
-
-    def _setup_open_ai(self) -> Any:
-        import openai
-
-        openai.api_key = self._api_key
-        if self._org_id is not None:
-            openai.organization = self._org_id
-
-        return openai
-
     async def complete_chat_async(
         self, messages: List[Tuple[str, str]], request_settings: ChatRequestSettings
     ) -> str:
         """
         Completes the given user message. Returns a single string completion.
 
         Arguments:
@@ -91,26 +91,31 @@
         if messages[-1][0] != "user":
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
                 "The last message must be from the user",
             )
 
         model_args = {}
-        if self.open_ai_instance.api_type in ["azure", "azure_ad"]:
+        if self._api_type in ["azure", "azure_ad"]:
             model_args["engine"] = self._model_id
         else:
             model_args["model"] = self._model_id
 
         formatted_messages = [
             {"role": role, "content": message} for role, message in messages
         ]
 
         try:
-            response: Any = await self.open_ai_instance.ChatCompletion.acreate(
+            response: Any = await openai.ChatCompletion.acreate(
                 **model_args,
+                api_key=self._api_key,
+                api_type=self._api_type,
+                api_base=self._endpoint,
+                api_version=self._api_version,
+                organization=self._org_id,
                 messages=formatted_messages,
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
             )
```

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import Any, Optional
 
+import openai
+
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
 )
 from semantic_kernel.connectors.ai.text_completion_client_base import (
     TextCompletionClientBase,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 
 
 class OpenAITextCompletion(TextCompletionClientBase):
     _model_id: str
     _api_key: str
+    _api_type: Optional[str] = None
+    _api_version: Optional[str] = None
+    _endpoint: Optional[str] = None
     _org_id: Optional[str] = None
     _log: Logger
 
     def __init__(
         self,
         model_id: str,
         api_key: str,
         org_id: Optional[str] = None,
+        api_type: Optional[str] = None,
+        api_version: Optional[str] = None,
+        endpoint: Optional[str] = None,
         log: Optional[Logger] = None,
     ) -> None:
         """
         Initializes a new instance of the OpenAITextCompletion class.
 
         Arguments:
             model_id {str} -- OpenAI model name, see
@@ -36,28 +44,20 @@
                 https://platform.openai.com/account/api-keys
             org_id {Optional[str]} -- OpenAI organization ID.
                 This is usually optional unless your
                 account belongs to multiple organizations.
         """
         self._model_id = model_id
         self._api_key = api_key
+        self._api_type = api_type
+        self._api_version = api_version
+        self._endpoint = endpoint
         self._org_id = org_id
         self._log = log if log is not None else NullLogger()
 
-        self.open_ai_instance = self._setup_open_ai()
-
-    def _setup_open_ai(self) -> Any:
-        import openai
-
-        openai.api_key = self._api_key
-        if self._org_id is not None:
-            openai.organization = self._org_id
-
-        return openai
-
     async def complete_async(
         self, prompt: str, request_settings: CompleteRequestSettings
     ) -> str:
         """
         Completes the given prompt. Returns a single string completion.
         Cannot return multiple completions. Cannot return logprobs.
 
@@ -91,22 +91,27 @@
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
                 "complete_async does not support logprobs, "
                 f"but logprobs={request_settings.logprobs} was requested",
             )
 
         model_args = {}
-        if self.open_ai_instance.api_type in ["azure", "azure_ad"]:
+        if self._api_type in ["azure", "azure_ad"]:
             model_args["engine"] = self._model_id
         else:
             model_args["model"] = self._model_id
 
         try:
-            response: Any = await self.open_ai_instance.Completion.acreate(
+            response: Any = await openai.Completion.acreate(
                 **model_args,
+                api_key=self._api_key,
+                api_type=self._api_type,
+                api_base=self._endpoint,
+                api_version=self._api_version,
+                organization=self._org_id,
                 prompt=prompt,
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
                 stop=(
```

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/import_skills.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/import_skills.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         """Upserts a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the record into.
             record {MemoryRecord} -- The record to upsert.
 
         Returns:
-            str -- The unqiue database key of the record.
+            str -- The unique database key of the record.
         """
         if collection_name not in self._store:
             raise Exception(f"Collection '{collection_name}' does not exist")
 
         record._key = record._id
         self._store[collection_name][record._key] = record
         return record._key
@@ -94,15 +94,15 @@
         """Upserts a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
-            List[str] -- The unqiue database keys of the records.
+            List[str] -- The unique database keys of the records.
         """
         if collection_name not in self._store:
             raise Exception(f"Collection '{collection_name}' does not exist")
 
         for record in records:
             record._key = record._id
             self._store[collection_name][record._key] = record
```

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/text/text_chunker.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     return lines, input_was_split
 
 
 def _split_list(
     text: List[str], max_tokens: int, separators: List[str], trim: bool
 ) -> List[str]:
     """
-    Split list of sring into lines.
+    Split list of string into lines.
     """
     if not text:
         return []
 
     lines = []
     input_was_split = False
     for line in text:
```

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.8.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.7.dev0/PKG-INFO` & `semantic_kernel-0.2.8.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.2.7.dev0
+Version: 0.2.8.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

