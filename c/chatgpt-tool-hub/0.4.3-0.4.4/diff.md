# Comparing `tmp/chatgpt-tool-hub-0.4.3.tar.gz` & `tmp/chatgpt-tool-hub-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-tool-hub-0.4.3.tar", last modified: Tue Apr 25 17:39:22 2023, max compression
+gzip compressed data, was "chatgpt-tool-hub-0.4.4.tar", last modified: Mon May 15 15:53:25 2023, max compression
```

## Comparing `chatgpt-tool-hub-0.4.3.tar` & `chatgpt-tool-hub-0.4.4.tar`

### file list

```diff
@@ -1,157 +1,163 @@
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.793435 chatgpt-tool-hub-0.4.3/
--rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.3/LICENSE
--rw-r--r--   0 goldfish   (502) staff       (20)    14090 2023-04-25 17:39:22.793220 chatgpt-tool-hub-0.4.3/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)    13295 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/README.md
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.770038 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.772043 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/
--rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2517 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2661 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/app_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/lite_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/victorinox.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.772419 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/
--rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/all_bot_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.772875 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    11283 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1935 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.773255 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4981 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.773961 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/
--rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.774633 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/
--rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/llm.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.777465 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/cache.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/calculate_token.py
--rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/callbacks.py
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/config.py
--rw-r--r--   0 goldfish   (502) staff       (20)      168 2023-04-16 00:10:23.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/constants.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/document.py
--rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/formatting.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/input.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/json_utils.py
--rw-r--r--   0 goldfish   (502) staff       (20)      640 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/log.py
--rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/schema.py
--rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/singleton.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/text_splitter.py
--rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.778330 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/
--rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/chat_memory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/token_buffer.py
--rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.779193 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/
--rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12841 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/bot.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/initialize.py
--rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/tool_engine.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.780048 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/
--rw-r--r--   0 goldfish   (502) staff       (20)     2142 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/base.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.781690 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5393 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15107 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/chatgpt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      521 2023-04-08 08:53:56.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/model_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)    28103 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/openai.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.782602 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/
--rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/chat.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.783656 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/
--rw-r--r--   0 goldfish   (502) staff       (20)     1396 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/all_tool_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.784246 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/
--rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2892 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/base_tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.784869 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.785412 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/load_tools.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.786033 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/
--rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5158 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1922 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.786306 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/
--rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.786692 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.787391 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3205 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.787800 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/
--rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2277 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.788053 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.788542 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.789124 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/
--rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/map_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/reduce_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7354 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.789710 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/
--rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/answer_user.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/debug.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.790078 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)      784 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool_register.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.790488 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/
--rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2349 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/text2image.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.791941 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/
--rw-r--r--   0 goldfish   (502) staff       (20)     2365 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5094 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/browser.py
--rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/delete.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/get.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/patch.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/post.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/put.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.792497 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/
--rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.792993 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/
--rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/version.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.770817 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/
--rw-r--r--   0 goldfish   (502) staff       (20)    14090 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)     4862 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/SOURCES.txt
--rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/dependency_links.txt
--rw-r--r--   0 goldfish   (502) staff       (20)      250 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/requires.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/top_level.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-04-25 17:39:22.793477 chatgpt-tool-hub-0.4.3/setup.cfg
--rw-r--r--   0 goldfish   (502) staff       (20)     1977 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.3/setup.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.545026 chatgpt-tool-hub-0.4.4/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.4/LICENSE
+-rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-05-15 15:53:25.544794 chatgpt-tool-hub-0.4.4/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)    13902 2023-05-04 15:37:21.000000 chatgpt-tool-hub-0.4.4/README.md
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.516544 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.518368 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/
+-rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2516 2023-05-04 17:20:51.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2874 2023-05-12 01:12:49.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/app_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/lite_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/victorinox.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.519129 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/
+-rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/all_bot_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.519780 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    11410 2023-05-15 14:37:49.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2310 2023-05-15 15:34:09.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.520303 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4988 2023-05-15 14:37:53.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.521413 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/
+-rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.521952 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/
+-rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-05-15 15:34:57.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/llm.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.525100 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/cache.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/calculate_token.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/callbacks.py
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/config.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      359 2023-05-12 01:00:31.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/constants.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/document.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/formatting.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/input.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/json_utils.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      859 2023-05-13 16:15:44.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/log.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/schema.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/singleton.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/text_splitter.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.526044 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/
+-rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/chat_memory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/token_buffer.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.526973 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/
+-rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12786 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/bot.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/initialize.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-27 15:08:27.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/tool_engine.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.528001 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2456 2023-05-13 15:52:05.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/base.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.528927 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4872 2023-05-04 10:03:38.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15985 2023-05-04 12:49:56.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/chatgpt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.529220 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/dashscope/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:59:11.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/dashscope/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      903 2023-05-04 10:14:15.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/model_factory.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.529326 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/moss/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:58:43.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/moss/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.530159 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/
+-rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/chat.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.531510 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1395 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/all_tool_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.532469 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2937 2023-05-05 15:15:58.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/base_tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.533105 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.533676 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.534052 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/hello_tool/
+-rw-r--r--   0 goldfish   (502) staff       (20)       60 2023-05-04 14:00:20.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/hello_tool/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1070 2023-05-04 13:53:09.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/hello_tool/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/load_tools.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.534792 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/
+-rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5263 2023-04-26 16:51:21.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1965 2023-05-06 18:07:09.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.535241 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/
+-rw-r--r--   0 goldfish   (502) staff       (20)      884 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.535660 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.536800 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3142 2023-05-12 01:24:50.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.537356 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/
+-rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2257 2023-05-12 01:22:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.537750 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.538310 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.538903 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/
+-rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/map_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/reduce_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7304 2023-05-15 14:53:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.539570 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/
+-rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/answer_user.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/debug.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.540198 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-28 11:33:01.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      916 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool_register.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.540716 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/
+-rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2377 2023-04-28 11:33:15.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/text2image.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.542687 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2397 2023-04-26 15:57:51.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5173 2023-05-05 16:21:45.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/browser.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/delete.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/get.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/patch.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/post.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/put.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.543869 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/
+-rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.544430 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/
+-rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-05-15 15:02:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/version.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.517210 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/
+-rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)     5003 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)      250 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/requires.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/top_level.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-05-15 15:53:25.545071 chatgpt-tool-hub-0.4.4/setup.cfg
+-rw-r--r--   0 goldfish   (502) staff       (20)     1977 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.4/setup.py
```

### Comparing `chatgpt-tool-hub-0.4.3/LICENSE` & `chatgpt-tool-hub-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/PKG-INFO` & `chatgpt-tool-hub-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.3
+Version: 0.4.4
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -37,21 +37,30 @@
 
 ---
 
 简体中文 | [English](./docs/README_en.md)
 
 > 大语言模型涌现能力让人惊艳，ChatGPT出现给NLP技术带来革命，除此之外还让我意识到一种新的人机交互的可能性
 
-## 🌱 4.23 新增LLM-OS demo - [快速上手](#llm-os_jump)
-
-
-
-https://user-images.githubusercontent.com/24581028/233855116-ecbc5ea8-246b-46c6-8a1a-67ea6d970077.mp4
-
+<div>
+    <h2 style="display:inline; margin:0; padding:0;">🌱 5.4 LLM-OS demo在线演示</h2>
+    <a style="display:inline-block; align:center" src="https://colab.research.google.com/assets/colab-badge.svg" href="https://colab.research.google.com/drive/11nYPGFCYiaZ73H8nTHSN8ifbo0u3W_8p">
+        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="demo in Colab"/>
+    </a>
+</div>
+
+<br/>
+
+<div align="center">
+    <a style="text-decoration:none" href="https://www.bilibili.com/video/BV1eL411h7Nk/" target="_blank">
+        <img src="https://i.328888.xyz/2023/04/29/iJQNi3.jpeg" width = "659" height = "410" alt="LLM-OS" align=center />
+    </a>
+</div>
 
+<br/>
 
 #### [更新日志](./docs/update_log.md) | [Q&A](./docs/q_and_a.md)
 
 ## 简介
 
 ---
 
@@ -84,16 +93,14 @@
 
 ## ✈️ 快速开始
 
 ---
 
 ### 1.  LLM-OS demo
 
-<span id="llm-os_jump"></span>
-
 #### (1). 克隆仓库
 
 ```bash
 git clone https://github.com/goldfishh/chatgpt-tool-hub.git
 cd chatgpt-tool-hub
 ```
 
@@ -103,15 +110,15 @@
 pip3 install -r requirements.txt
 ```
 
 #### (3). 重命名.env.template 和 config.json.template文件，去掉.template后缀 打开文件填入配置参数 
 
 `.env` 用于配置全局参数 文件配置示例
 ```text
-OPENAI_API_KEY=sk-xx          // 必填，你的OPENAI API Key, 如何申请请见Q&A
+LLM_API_KEY=sk-xx          // 必填，你的OPENAI API Key, 如何申请请见Q&A
 MODEL_NAME=gpt-3.5-turbo      // 选填，OPENAI LLM模型
 THINK_DEPTH=3                 // 选填，默认为3，控制LLM-OS的最大调用工具次数，过大不一定能提高回复质量
 REQUEST_TIMEOUT=90            // 选填，默认120，等待openai api回复的最大时间
 PROXY=http://192.168.7.1:7890 // 选填，当你需要代理访问openai时可填
 DEBUG=false                   // 选填，debug模式
 ```
 
@@ -133,15 +140,15 @@
 
 ```bash
 python3 terminal_io.py
 ```
 
 #### (5). 进入LLM-OS后你可以自行探索 或者进一步浏览详细教程：[LLM_OS demo使用说明](https://github.com/goldfishh/llm-os/blob/main/README.md)
 
---- 
+---
 
 ### 2. 我给[chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat)开发了tool插件
 
 > 使用本方法，你将可以用微信作为前端更方便地使用tool-hub
 
 #### 查阅chatgpt-on-wechat文档中的[项目简介](https://github.com/zhayujie/chatgpt-on-wechat#%E7%AE%80%E4%BB%8B) 和 [快速开始](https://github.com/zhayujie/chatgpt-on-wechat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
 
@@ -162,60 +169,48 @@
 ```
 
 #### (2). 快速开始
 
 ```python
 import os
 from chatgpt_tool_hub.apps import AppFactory
-os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"  # 必填
+os.environ["LLM_API_KEY"] = "YOUR_LLM_API_KEY"  # 必填
 os.environ["PROXY"] = "YOUR_PROXY_ADDRESS"            # 选填
 app = AppFactory().create_app(tools_list=[], **{})
 reply = app.ask("YOUR_QUESTION_TO_HERE")
 print(reply)
 ```
 
 #### (3). 以插件形式接入tool-hub可参考tool插件实现
 
 [tool.py](https://github.com/goldfishh/chatgpt-on-wechat/blob/master/plugins/tool/tool.py)
 
 > 如果有需求，我会更新更详细接入的文档，欢迎提issue
 
 ---
 
-## ☕ 宣传
-
-#### 如果你想支持本项目，欢迎给项目点个star、提issue和pr
-#### 如果你想进一步支持项目作者少掉头发，努力开发，可以给和我一起开发项目的伙伴 或 单独给我来杯 ☕
-
-<table><tr>
-<td><a href="https://public.zsxq.com/groups/88885848842852.html"><img src="https://github.com/zhayujie/chatgpt-on-wechat/blob/master/docs/images/planet.jpg?raw=true" width="400" height="200" border=0></a></td>
-<td><img src="./assets/buy_me_a_coffee.jpg" width="200" height="200" border=0 /></td>
-</tr></table> 
-
----
-
 ## 工具指南 
 
 ### 🚀 [工具指南 工具快速开发中](./docs/tool_tutorial.md)
 
 ---
 
 ## 原理
 
 ---
 
 工具引擎的实现原理本质是**Chain-of-Thought**：[Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)
-  
+
 我将通过用6个自问自答的问题解释chatgpt-tool-hub的工作原理  
 
 #### 1. 事务型工具（如terminal、python）是在哪运行，以及如何执行的
 
 事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、url-get工具分别用到了封装调用subprocess库、python解释器和requests库的函数
 
---- 
+---
 
 #### 2. ChatGPT是如何触发调用这些函数
 
 借助ChatGPT api提供的temperature参数，该参数越低，ChatGPT输出的结果会更集中和确定，当temperature为0时，相同的问题会得到统一回答  
 我在prompt构建时会提供给ChatGPT此时用到的工具列表信息，每个工具信息包含：工具名 和 工具描述：
 
 ```text
@@ -254,25 +249,25 @@
 
 ```text
 Observation: 当事务函数执行完成返回时的内容
 ```
 
 带Observation前缀的内容往往是使用事务型工具的用户想知道的答案
 
---- 
-  
+---
+
 #### 3. ChatGPT怎么知道该用的工具和输入，是否每次都严格按照prompt生成格式化内容
 
 ChatGPT微调时进行大量Q&A、CoT预料的学习和RLHF调优，目前ChatGPT对于工具和内容生成的质量是有保证的  
 但是目前不是100%，因为会有低质量prompt或者不合适工具的输入，这些问题在工具引擎会进行鲁棒性的处理来保证生成内容的稳定性  
 
 我创建一个issue，可以方便大家来获取和分享使用tool过程解决的有趣问题和思路、每个tool使用时prompt技巧、遇到问题的处理办法：
 [更好的使用tool的技巧交流](https://github.com/goldfishh/chatgpt-tool-hub/issues/3)
 
---- 
+---
 
 #### 4. 如果需要多个工具交替配合解决某个问题，引擎是怎么做的？
 
 当事务函数处理完成返回结果后，默认不会直接返回给用户，而是根据结果内容CoT，在整个prompt中，还有两个子prompt负责用户对话历史记录和中间结果
 
 用户对话历史记录：
 ```text
@@ -287,51 +282,51 @@
 Action: Wolfram Alpha
 Action Input: gdp china vs. usa
 Observation: China\nUnited States | GDP | nominal \nAnswer: China | $14.72 trillion per year\nUnited States | $20.95 trillion per year\n(2020 estimates)
 Thought:
 ```
 
 每轮工具CoT过程均会作为下次推理判断工具的依据，由此迭代地进行工具判断、执行，最后当识别到特定前缀时，CoT结果将返回给用户    
-  
+
 CoT结束prompt：
 ```text
 When you have a response to say to the Human, or if you do not need to use a tool, you MUST use the format:
 
 Thought: Do I need to use a tool? No
 AI: the response to the original input question in chinese
 
 ```
 
 
 ChatGPT使用工具过程并不顺利：当遇到迭代次数到达预设值时，会根据历史过程，返回给用户最后结果    
 
---- 
+---
 
 #### 5. 事务性工具交给ChatGPT是否具有不可预料的危险性？
 
 是的，当你用事务性工具时，你就给予了ChatGPT在你本地运行程序的权利，你需要权限限制来规避可能的风险      
 如果无法信任ChatGPT主导你的机器，请不要使用  
 
---- 
+---
 
 #### 6. 非事务型工具的实现原理是什么
 
 参考[ChatGPT 官方插件](https://github.com/openai/chatgpt-retrieval-plugin)，非事务性工具也称为插件型工具，该工具可视为开放性的ChatGPT插件
 
 ---
 
 
 ## 🎯 计划
 
 <span id="plan"></span>
 
 ---
- 
+
 ### feature todolist
-  
+
 [✓] 结果可解释性输出 -> LLM-OS的内心独白  
 [✓] 一个前端demo  -> LLM-OS  
 [✓] 长文本场景 -> summary工具  
 [✓] 长工具顺序控制 -> 实现了toolintool机制    
 [✓] 粒度配置 -> 每个tool封装的LLM可独立配置  
 [○] tokens计算，精确管理    
 [○] gpt_index长文本(pdf、html)检索   
@@ -339,46 +334,62 @@
 [○] 接入国内LLM  
 [○] 兼容不使用tool的场景  
 [○] 互斥tool控制  
 [○] subtree 动态注册&反注册  
 [○] 工具中断  
 [○] 定时调度  
 [○] 语音输入、输出  
-  
+
 ### tool todolist  
-   
+
 [○] stable-diffusion 中文prompt翻译    
 [✓] ImageCaptioning    
 [○] 小米智能家居控制    
 [○] 支持ChatGPT官方插件  
 [○] 让LLM来实现tool  
 [○] 支持图片处理工具    
 [○] 支持视频处理工具   
 [✗] Wechat  
 
 ## 工具开发指南
 
 ---
- 
+
 目前工具分为两类：事务型工具、插件型工具   
- 
-我等待有需求之后更新这部分内容    
 
 [工具开发教程](./docs/tool_development_guide.md)
 
 ## 背景
 
 我将很快更新这部分内容   
 
 ---
 
+## ☕ 宣传
+
+#### 如果你想支持本项目，欢迎给项目点个star、提issue和pr
+#### 如果你想进一步支持项目作者少掉头发，努力开发，可以给和我一起开发项目的伙伴 或 单独给我来杯 ☕
+
+<table><tr>
+<td><a href="https://public.zsxq.com/groups/88885848842852.html"><img src="https://github.com/zhayujie/chatgpt-on-wechat/blob/master/docs/images/planet.jpg?raw=true" width="400" height="200" border=0></a></td>
+<td><img src="./assets/buy_me_a_coffee.jpg" width="200" height="200" border=0 /></td>
+</tr></table> 
+
+---
+
 ## 感谢
 
 感谢以下项目对本项目提供的有力支持：
 
-#### 1. [langchain](https://github.com/hwchase17/langchain)
+#### 1. [langchain](https://github.com/hwchase17/langchain) 
+
+受langchain的启发，本项目重写了langchain v0.0.123 工具有关的实现
 
 #### 2. [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
+启发了browser tool跨平台的实现、tool engine的json通信、部分prompt描述
+
 #### 3. [chatgpt-in-terminal](https://github.com/xiaoxx970/chatgpt-in-terminal)
 
+llm-os demo 改写自该项目
+
 ---
```

### Comparing `chatgpt-tool-hub-0.4.3/README.md` & `chatgpt-tool-hub-0.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,30 @@
 
 ---
 
 简体中文 | [English](./docs/README_en.md)
 
 > 大语言模型涌现能力让人惊艳，ChatGPT出现给NLP技术带来革命，除此之外还让我意识到一种新的人机交互的可能性
 
-## 🌱 4.23 新增LLM-OS demo - [快速上手](#llm-os_jump)
-
-
-
-https://user-images.githubusercontent.com/24581028/233855116-ecbc5ea8-246b-46c6-8a1a-67ea6d970077.mp4
-
+<div>
+    <h2 style="display:inline; margin:0; padding:0;">🌱 5.4 LLM-OS demo在线演示</h2>
+    <a style="display:inline-block; align:center" src="https://colab.research.google.com/assets/colab-badge.svg" href="https://colab.research.google.com/drive/11nYPGFCYiaZ73H8nTHSN8ifbo0u3W_8p">
+        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="demo in Colab"/>
+    </a>
+</div>
+
+<br/>
+
+<div align="center">
+    <a style="text-decoration:none" href="https://www.bilibili.com/video/BV1eL411h7Nk/" target="_blank">
+        <img src="https://i.328888.xyz/2023/04/29/iJQNi3.jpeg" width = "659" height = "410" alt="LLM-OS" align=center />
+    </a>
+</div>
 
+<br/>
 
 #### [更新日志](./docs/update_log.md) | [Q&A](./docs/q_and_a.md)
 
 ## 简介
 
 ---
 
@@ -65,16 +74,14 @@
 
 ## ✈️ 快速开始
 
 ---
 
 ### 1.  LLM-OS demo
 
-<span id="llm-os_jump"></span>
-
 #### (1). 克隆仓库
 
 ```bash
 git clone https://github.com/goldfishh/chatgpt-tool-hub.git
 cd chatgpt-tool-hub
 ```
 
@@ -84,15 +91,15 @@
 pip3 install -r requirements.txt
 ```
 
 #### (3). 重命名.env.template 和 config.json.template文件，去掉.template后缀 打开文件填入配置参数 
 
 `.env` 用于配置全局参数 文件配置示例
 ```text
-OPENAI_API_KEY=sk-xx          // 必填，你的OPENAI API Key, 如何申请请见Q&A
+LLM_API_KEY=sk-xx          // 必填，你的OPENAI API Key, 如何申请请见Q&A
 MODEL_NAME=gpt-3.5-turbo      // 选填，OPENAI LLM模型
 THINK_DEPTH=3                 // 选填，默认为3，控制LLM-OS的最大调用工具次数，过大不一定能提高回复质量
 REQUEST_TIMEOUT=90            // 选填，默认120，等待openai api回复的最大时间
 PROXY=http://192.168.7.1:7890 // 选填，当你需要代理访问openai时可填
 DEBUG=false                   // 选填，debug模式
 ```
 
@@ -114,15 +121,15 @@
 
 ```bash
 python3 terminal_io.py
 ```
 
 #### (5). 进入LLM-OS后你可以自行探索 或者进一步浏览详细教程：[LLM_OS demo使用说明](https://github.com/goldfishh/llm-os/blob/main/README.md)
 
---- 
+---
 
 ### 2. 我给[chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat)开发了tool插件
 
 > 使用本方法，你将可以用微信作为前端更方便地使用tool-hub
 
 #### 查阅chatgpt-on-wechat文档中的[项目简介](https://github.com/zhayujie/chatgpt-on-wechat#%E7%AE%80%E4%BB%8B) 和 [快速开始](https://github.com/zhayujie/chatgpt-on-wechat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
 
@@ -143,60 +150,48 @@
 ```
 
 #### (2). 快速开始
 
 ```python
 import os
 from chatgpt_tool_hub.apps import AppFactory
-os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"  # 必填
+os.environ["LLM_API_KEY"] = "YOUR_LLM_API_KEY"  # 必填
 os.environ["PROXY"] = "YOUR_PROXY_ADDRESS"            # 选填
 app = AppFactory().create_app(tools_list=[], **{})
 reply = app.ask("YOUR_QUESTION_TO_HERE")
 print(reply)
 ```
 
 #### (3). 以插件形式接入tool-hub可参考tool插件实现
 
 [tool.py](https://github.com/goldfishh/chatgpt-on-wechat/blob/master/plugins/tool/tool.py)
 
 > 如果有需求，我会更新更详细接入的文档，欢迎提issue
 
 ---
 
-## ☕ 宣传
-
-#### 如果你想支持本项目，欢迎给项目点个star、提issue和pr
-#### 如果你想进一步支持项目作者少掉头发，努力开发，可以给和我一起开发项目的伙伴 或 单独给我来杯 ☕
-
-<table><tr>
-<td><a href="https://public.zsxq.com/groups/88885848842852.html"><img src="https://github.com/zhayujie/chatgpt-on-wechat/blob/master/docs/images/planet.jpg?raw=true" width="400" height="200" border=0></a></td>
-<td><img src="./assets/buy_me_a_coffee.jpg" width="200" height="200" border=0 /></td>
-</tr></table> 
-
----
-
 ## 工具指南 
 
 ### 🚀 [工具指南 工具快速开发中](./docs/tool_tutorial.md)
 
 ---
 
 ## 原理
 
 ---
 
 工具引擎的实现原理本质是**Chain-of-Thought**：[Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)
-  
+
 我将通过用6个自问自答的问题解释chatgpt-tool-hub的工作原理  
 
 #### 1. 事务型工具（如terminal、python）是在哪运行，以及如何执行的
 
 事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、url-get工具分别用到了封装调用subprocess库、python解释器和requests库的函数
 
---- 
+---
 
 #### 2. ChatGPT是如何触发调用这些函数
 
 借助ChatGPT api提供的temperature参数，该参数越低，ChatGPT输出的结果会更集中和确定，当temperature为0时，相同的问题会得到统一回答  
 我在prompt构建时会提供给ChatGPT此时用到的工具列表信息，每个工具信息包含：工具名 和 工具描述：
 
 ```text
@@ -235,25 +230,25 @@
 
 ```text
 Observation: 当事务函数执行完成返回时的内容
 ```
 
 带Observation前缀的内容往往是使用事务型工具的用户想知道的答案
 
---- 
-  
+---
+
 #### 3. ChatGPT怎么知道该用的工具和输入，是否每次都严格按照prompt生成格式化内容
 
 ChatGPT微调时进行大量Q&A、CoT预料的学习和RLHF调优，目前ChatGPT对于工具和内容生成的质量是有保证的  
 但是目前不是100%，因为会有低质量prompt或者不合适工具的输入，这些问题在工具引擎会进行鲁棒性的处理来保证生成内容的稳定性  
 
 我创建一个issue，可以方便大家来获取和分享使用tool过程解决的有趣问题和思路、每个tool使用时prompt技巧、遇到问题的处理办法：
 [更好的使用tool的技巧交流](https://github.com/goldfishh/chatgpt-tool-hub/issues/3)
 
---- 
+---
 
 #### 4. 如果需要多个工具交替配合解决某个问题，引擎是怎么做的？
 
 当事务函数处理完成返回结果后，默认不会直接返回给用户，而是根据结果内容CoT，在整个prompt中，还有两个子prompt负责用户对话历史记录和中间结果
 
 用户对话历史记录：
 ```text
@@ -268,51 +263,51 @@
 Action: Wolfram Alpha
 Action Input: gdp china vs. usa
 Observation: China\nUnited States | GDP | nominal \nAnswer: China | $14.72 trillion per year\nUnited States | $20.95 trillion per year\n(2020 estimates)
 Thought:
 ```
 
 每轮工具CoT过程均会作为下次推理判断工具的依据，由此迭代地进行工具判断、执行，最后当识别到特定前缀时，CoT结果将返回给用户    
-  
+
 CoT结束prompt：
 ```text
 When you have a response to say to the Human, or if you do not need to use a tool, you MUST use the format:
 
 Thought: Do I need to use a tool? No
 AI: the response to the original input question in chinese
 
 ```
 
 
 ChatGPT使用工具过程并不顺利：当遇到迭代次数到达预设值时，会根据历史过程，返回给用户最后结果    
 
---- 
+---
 
 #### 5. 事务性工具交给ChatGPT是否具有不可预料的危险性？
 
 是的，当你用事务性工具时，你就给予了ChatGPT在你本地运行程序的权利，你需要权限限制来规避可能的风险      
 如果无法信任ChatGPT主导你的机器，请不要使用  
 
---- 
+---
 
 #### 6. 非事务型工具的实现原理是什么
 
 参考[ChatGPT 官方插件](https://github.com/openai/chatgpt-retrieval-plugin)，非事务性工具也称为插件型工具，该工具可视为开放性的ChatGPT插件
 
 ---
 
 
 ## 🎯 计划
 
 <span id="plan"></span>
 
 ---
- 
+
 ### feature todolist
-  
+
 [✓] 结果可解释性输出 -> LLM-OS的内心独白  
 [✓] 一个前端demo  -> LLM-OS  
 [✓] 长文本场景 -> summary工具  
 [✓] 长工具顺序控制 -> 实现了toolintool机制    
 [✓] 粒度配置 -> 每个tool封装的LLM可独立配置  
 [○] tokens计算，精确管理    
 [○] gpt_index长文本(pdf、html)检索   
@@ -320,46 +315,62 @@
 [○] 接入国内LLM  
 [○] 兼容不使用tool的场景  
 [○] 互斥tool控制  
 [○] subtree 动态注册&反注册  
 [○] 工具中断  
 [○] 定时调度  
 [○] 语音输入、输出  
-  
+
 ### tool todolist  
-   
+
 [○] stable-diffusion 中文prompt翻译    
 [✓] ImageCaptioning    
 [○] 小米智能家居控制    
 [○] 支持ChatGPT官方插件  
 [○] 让LLM来实现tool  
 [○] 支持图片处理工具    
 [○] 支持视频处理工具   
 [✗] Wechat  
 
 ## 工具开发指南
 
 ---
- 
+
 目前工具分为两类：事务型工具、插件型工具   
- 
-我等待有需求之后更新这部分内容    
 
 [工具开发教程](./docs/tool_development_guide.md)
 
 ## 背景
 
 我将很快更新这部分内容   
 
 ---
 
+## ☕ 宣传
+
+#### 如果你想支持本项目，欢迎给项目点个star、提issue和pr
+#### 如果你想进一步支持项目作者少掉头发，努力开发，可以给和我一起开发项目的伙伴 或 单独给我来杯 ☕
+
+<table><tr>
+<td><a href="https://public.zsxq.com/groups/88885848842852.html"><img src="https://github.com/zhayujie/chatgpt-on-wechat/blob/master/docs/images/planet.jpg?raw=true" width="400" height="200" border=0></a></td>
+<td><img src="./assets/buy_me_a_coffee.jpg" width="200" height="200" border=0 /></td>
+</tr></table> 
+
+---
+
 ## 感谢
 
 感谢以下项目对本项目提供的有力支持：
 
-#### 1. [langchain](https://github.com/hwchase17/langchain)
+#### 1. [langchain](https://github.com/hwchase17/langchain) 
+
+受langchain的启发，本项目重写了langchain v0.0.123 工具有关的实现
 
 #### 2. [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
+启发了browser tool跨平台的实现、tool engine的json通信、部分prompt描述
+
 #### 3. [chatgpt-in-terminal](https://github.com/xiaoxx970/chatgpt-in-terminal)
 
+llm-os demo 改写自该项目
+
 ---
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/app.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     def init_tool_engine(self, tools: List[BaseTool] = list):
         raise ValueError("init_tool_engine not implemented for this app.")
 
     def load_tools_into_bot(self, **tools_kwargs):
         raise ValueError("load_tools_into_bot not implemented for this app.")
 
-
     def update_tool_args(self, tools_list: list, is_del: bool = False, **tools_kwargs):
         if is_del:
             for tool in tools_list:
                 self.tools.remove(tool)
             return
 
         for tool in tools_list:
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/lite_app.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/lite_app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/victorinox.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/victorinox.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     def get_full_inputs(
         self, intermediate_steps: List[Tuple[BotAction, str]], **kwargs: Any
     ) -> Dict[str, Any]:
         """Create the full inputs for the LLMChain from intermediate steps."""
         thoughts = self._construct_scratchpad(intermediate_steps)
         # todo remove stop
-        new_inputs = {"bot_scratchpad": self._crop_full_input(thoughts), "stop": self._stop}
+        new_inputs = {"bot_scratchpad": self._crop_full_input(thoughts)}
         return {**kwargs, **new_inputs}
 
     def _get_next_action(self, full_inputs: Dict[str, str]) -> BotAction:
         llm_answer_str = self.llm_chain.predict(**full_inputs)
 
         action, action_input = self._extract_tool_and_input(llm_answer_str)
 
@@ -171,15 +171,15 @@
         if action.lower() not in self.allowed_tools:
             return "answer-user", action_input
 
         if action.lower() != "answer-user":
             self.console.print(f"√ 我在用 [bold cyan]{action}[/] 工具...")
 
         LOG.info(f"执行Tool: {action}中...")
-        return action.strip(), action_input.strip()
+        return str(action).strip(), str(action_input).strip()
 
     def parse_reply_json(self, assistant_reply) -> dict:
         """Prints the assistant's thoughts to the console"""
         try:
             try:
                 # Parse and print Assistant response
                 assistant_reply_json = json_utils.fix_and_parse_json(assistant_reply)
@@ -214,20 +214,21 @@
             thoughts_text = ""
             if assistant_thoughts_reasoning:
                 thoughts_text += f"推理：{assistant_thoughts_reasoning}\n"
             if assistant_thoughts_text:
                 thoughts_text += f"思考：{assistant_thoughts_text}\n"
             if assistant_thoughts_criticism:
                 thoughts_text += f"反思：{assistant_thoughts_criticism}\n"
-
+            if assistant_thoughts_speak:
+                LOG.info(f"{self.ai_prefix.upper()}想和你说：{assistant_thoughts_speak}")
             self.console.print(Panel(thoughts_text,
                                      title=f"{self.ai_prefix.upper()}的内心独白",
                                      highlight=True, style='dim'))
             # it's useful for avoid splitting Panel
-            LOG.info(f"{self.ai_prefix.upper()}的内心独白: {thoughts_text}")
+            LOG.info(f"{self.ai_prefix.upper()}的内心独白: \n{thoughts_text}")
             
             return assistant_reply_json
         except json.decoder.JSONDecodeError as e:
             call_stack = traceback.format_exc()
             LOG.error(f"Error: Invalid JSON: {assistant_reply}\n")
             LOG.error(f"Traceback: {repr(call_stack)}, error: {repr(e)}")
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,12 +119,12 @@
         if FINAL_ANSWER_ACTION in text:
             return "Final Answer", text.split(FINAL_ANSWER_ACTION)[-1].strip()
         regex = r"Action: (.*?)[\n]*Action Input: (.*)"
         match = re.search(regex, text, re.DOTALL)
         if not match:
             return None
 
-        action = match[1].strip()
-        action_input = match[2]
+        action = str(match[1]).strip()
+        action_input = str(match[2]).strip()
         LOG.info(f"执行Tool: {action}中...")
 
-        return action, action_input.strip(" ")
+        return action, action_input
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/llm.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/llm.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/cache.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/cache.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/calculate_token.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/calculate_token.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/callbacks.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/document.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/document.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/formatting.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/formatting.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/input.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/input.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/json_utils.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/json_utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/schema.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/schema.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/singleton.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/singleton.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/text_splitter.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/utils.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/chat_memory.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/chat_memory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/token_buffer.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/token_buffer.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/utils.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/bot.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,17 +67,18 @@
         ]
 
     def _construct_scratchpad(
         self, intermediate_steps: List[Tuple[BotAction, str]]
     ) -> Union[str, List[BaseMessage]]:
         """Construct the scratchpad that lets the bot continue its thought process."""
         thoughts = ""
+        # todo 区分当前对话和历史对话的scratchpad描述
         for action, observation in intermediate_steps:
-            thoughts += f"The JSON you responded me: \n{action.log}\n\n"
-            thoughts += f"The content returned after invoking the tool: \n{observation}\n\n"
+            thoughts += f"previous constructed JSON: {action.log}\n"
+            thoughts += f"{action.tool} tool was called and it returned: {observation}\n\n"
         return thoughts
 
     def _crop_full_input(self, inputs: str) -> str:
         """ crop too long text """
         if not inputs:
             return inputs
         _input = inputs
@@ -87,15 +88,15 @@
             # compress text size
             temp_file = tempfile.mkstemp()
             file_path = temp_file[1]
 
             with open(file_path, "w") as f:
                 f.write(_input + "\n")
             # 总结
-            _input = SummaryTool(max_segment_length=2000).run(f"{str(file_path)}, 0")
+            _input = SummaryTool(self.console, max_segment_length=2000).run(f"{str(file_path)}, 0")
             try:
                 os.remove(file_path)
             except Exception as e:
                 LOG.debug(f"remove {file_path} failed... error_info: {repr(e)}")
 
         return _input
 
@@ -227,38 +228,33 @@
         **kwargs: Any,
     ) -> BotFinish:
         """Return response when bot has been stopped due to max iterations."""
         if early_stopping_method == "force":
             # `force` just returns a constant string
             return BotFinish({"output": "Bot stopped due to max iterations."}, "")
         elif early_stopping_method == "generate":
-            # Generate does one final forward pass
-            thoughts = ""
-            for action, observation in intermediate_steps:
-                thoughts += action.log
-                thoughts += (
-                    f"\n{self.observation_prefix}{observation}\n{self.llm_prefix}"
-                )
             # Adding to the previous steps, we now tell the LLM to make a final pred
+            thoughts = self._construct_scratchpad(intermediate_steps)
             thoughts += (
                 f"你超过了tool使用次数限制: 最多{max_iterations}次。"
-                "你现在需要总结当前你了解到的所有信息，来反馈给人类。"
+                "你现在需要总结当前你了解到的所有信息，来反馈给人类，本次你必须使用answer-user工具!"
                 "你需要生成一个final answer:"
             )
-            new_inputs = {"bot_scratchpad": thoughts, "stop": self._stop}
+
+            new_inputs = {"bot_scratchpad": self._crop_full_input(thoughts), "stop": self._stop}
             full_inputs = {**kwargs, **new_inputs}
             full_output = self.llm_chain.predict(**full_inputs)
             # We try to extract a final answer
             action, action_input = self._extract_tool_and_input(full_output)
 
             if action:
                 return (
                     BotFinish({"output": action_input}, full_output)
                     if action.lower() in ['answer-user']
-                    else BotFinish({"output": full_output}, full_output)
+                    else BotFinish({"output": "受think_depth限制，系统强制终止了LLM-OS"}, full_output)
                 )
             else:
                 # If we cannot extract, we just return the full output
                 return BotFinish({"output": full_output}, full_output)
 
         else:
             raise ValueError(
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/initialize.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/initialize.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/tool_engine.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/tool_engine.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/__init__.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from typing import Optional
 
 from chatgpt_tool_hub.common.cache import BaseCache
+from chatgpt_tool_hub.common.constants import openai_default_api_base
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 
 verbose: bool = False
 llm_cache: Optional[BaseCache] = None
 
 # default for gpt-3.5
 ALL_MAX_TOKENS_NUM = 4000
@@ -19,45 +20,48 @@
 def change_memory_max_tokens(memory_max_tokens_num: int):
     global MEMORY_MAX_TOKENS_NUM, BOT_SCRATCHPAD_MAX_TOKENS_NUM
     MEMORY_MAX_TOKENS_NUM = memory_max_tokens_num
     BOT_SCRATCHPAD_MAX_TOKENS_NUM = ALL_MAX_TOKENS_NUM - BOT_PROMPT - MEMORY_MAX_TOKENS_NUM - 200
 
 
 def build_model_params(kwargs: dict) -> dict:
-    _api_key = get_from_dict_or_env(kwargs, "openai_api_key", "OPENAI_API_KEY")
+    _api_key = get_from_dict_or_env(kwargs, "llm_api_key", "LLM_API_KEY")
     _proxy = get_from_dict_or_env(kwargs, "proxy", "PROXY", "")
     _model = get_from_dict_or_env(kwargs, "model_name", "MODEL_NAME", "gpt-3.5-turbo")
     _timeout = get_from_dict_or_env(kwargs, "request_timeout", "REQUEST_TIMEOUT", 120)
+    _llm_api_base_url = get_from_dict_or_env(kwargs, "llm_api_base_url", "LLM_API_BASE_URL", openai_default_api_base)
+
     # tool llm need them
-    os.environ["OPENAI_API_KEY"] = str(_api_key)
+    os.environ["LLM_API_KEY"] = str(_api_key)
+    if _proxy and not _proxy.startswith("http://") and not _proxy.startswith("https://"):
+        _proxy = "http://" + _proxy
     os.environ["PROXY"] = str(_proxy)
     os.environ["MODEL_NAME"] = str(_model)
     os.environ["REQUEST_TIMEOUT"] = str(_timeout)
+    os.environ["LLM_API_BASE_URL"] = str(_llm_api_base_url)
     return {
         "temperature": get_from_dict_or_env(kwargs, "temperature", "TEMPERATURE", 0),
-        "openai_api_key": _api_key,
+        "llm_api_key": _api_key,
+        "llm_api_base_url": _llm_api_base_url,
         "proxy": _proxy,
         "model_name": _model,  # 对话模型的名称
         "top_p": 1,
         "frequency_penalty": 0.0,  # [-2,2]之间，该值越大则更倾向于产生不同的内容
         "presence_penalty": 0.0,  # [-2,2]之间，该值越大则更倾向于产生不同的内容
         "request_timeout": _timeout,
         "max_retries": 2
     }
 
 
 from chatgpt_tool_hub.models.base import BaseLLM, LLM
 from chatgpt_tool_hub.models.chatgpt.chatgpt import ChatOpenAI
-from chatgpt_tool_hub.models.openai import OpenAI, AzureOpenAI
 
 
 __all__ = [
     "ALL_MAX_TOKENS_NUM",
     "MEMORY_MAX_TOKENS_NUM",
     "BOT_SCRATCHPAD_MAX_TOKENS_NUM",
 
     "BaseLLM",
     "LLM",
-    "OpenAI",
-    "AzureOpenAI",
     "ChatOpenAI"
 ]
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,23 +122,7 @@
         self, messages: List[BaseMessage], stop: Optional[List[str]] = None
     ) -> BaseMessage:
         return self._generate(messages, stop=stop).generations[0].message
 
     def call_as_llm(self, message: str, stop: Optional[List[str]] = None) -> str:
         result = self([HumanMessage(content=message)], stop=stop)
         return result.content
-
-
-class SimpleChatModel(BaseChatModel):
-    def _generate(
-        self, messages: List[BaseMessage], stop: Optional[List[str]] = None
-    ) -> ChatResult:
-        output_str = self._call(messages, stop=stop)
-        message = AIMessage(content=output_str)
-        generation = ChatGeneration(message=message)
-        return ChatResult(generations=[generation])
-
-    @abstractmethod
-    def _call(
-        self, messages: List[BaseMessage], stop: Optional[List[str]] = None
-    ) -> str:
-        """Simpler interface."""
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/chatgpt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/chatgpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
+from chatgpt_tool_hub.common.constants import openai_default_api_base
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.schema import (
     AIMessage,
     BaseMessage,
     ChatGeneration,
     ChatMessage,
     ChatResult,
@@ -100,44 +101,48 @@
     return ChatResult(generations=generations, llm_output=llm_output)
 
 
 class ChatOpenAI(BaseChatModel, BaseModel):
     """Wrapper around OpenAI Chat large language models.
 
     To use, you should have the ``openai`` python package installed, and the
-    environment variable ``OPENAI_API_KEY`` set with your API key.
+    environment variable ``LLM_API_KEY`` set with your API key.
 
     Any parameters that are valid to be passed to the openai.create call can be passed
     in, even if not explicitly saved on this class.
 
     Example:
         .. code-block:: python
 
             from lib.chat_models import ChatOpenAI
             openai = ChatOpenAI(model_name="gpt-3.5-turbo")
     """
 
     client: Any  #: :meta private:
-    model_name: str = "gpt-3.5-turbo"
     """Model name to use."""
-    model_kwargs: Dict[str, Any] = Field(default_factory=dict)
+    model_name: str = "gpt-3.5-turbo"
     """Holds any model parameters valid for `create` call not explicitly specified."""
-    openai_api_key: Optional[str] = None
-    request_timeout: int = 60
+    model_kwargs: Dict[str, Any] = Field(default_factory=dict)
+    """llm api base url"""
+    llm_api_base_url: str = openai_default_api_base
+    """a key to call llm api server"""
+    llm_api_key: Optional[str] = None
     """Timeout in seconds for the OpenAPI request."""
-    max_retries: int = 6
+    request_timeout: int = 60
     """Maximum number of retries to make when generating."""
-    streaming: bool = False
+    max_retries: int = 6
     """Whether to stream the results or not."""
-    n: int = 1
+    streaming: bool = False
     """Number of chat completions to generate for each prompt."""
-    max_tokens: Optional[int] = None
+    n: int = 1
     """Maximum number of tokens to generate."""
-    proxy: str = None
+    max_tokens: Optional[int] = None
     """the proxy to use"""
+    proxy: Optional[str] = None
+    """"""
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.ignore
 
     @root_validator(pre=True)
@@ -153,33 +158,50 @@
                 extra[field_name] = values.pop(field_name)
         values["model_kwargs"] = extra
         return values
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
-        openai_api_key = get_from_dict_or_env(
-            values, "openai_api_key", "OPENAI_API_KEY"
+        _llm_api_key = get_from_dict_or_env(
+            values, "llm_api_key", "LLM_API_KEY"
+        )
+        _llm_api_base_url = get_from_dict_or_env(
+            values, "llm_api_base_url", "LLM_API_BASE_URL",
+            openai_default_api_base)
+        _proxy = get_from_dict_or_env(
+            values, "proxy", "PROXY", ""
         )
         try:
             import openai
 
-            if not openai.proxy:
-                if values.get('proxy'):
-                    openai.proxy = values['proxy']
-                    LOG.info(f"success use proxy: {values['proxy']}")
+            if openai.proxy != _proxy:
+                if _proxy:
+                    openai.proxy = _proxy
+                    values["proxy"] = _proxy
+                    LOG.info(f"success use proxy: {_proxy}")
                 else:
-                    LOG.warning("proxy no find, directly request to chatgpt instead")
+                    LOG.info("proxy no find, directly request to chatgpt instead")
+
+            if openai.api_base != _llm_api_base_url:
+                openai.api_base = _llm_api_base_url
+                values["llm_api_base_url"] = _llm_api_base_url
+                LOG.info(f"success use customized api base url: {_llm_api_base_url}")
+
+            if openai.api_key != _llm_api_key:
+                openai.api_key = _llm_api_key
+                values["llm_api_key"] = _llm_api_key
+                LOG.debug(f"success use llm api key: {_llm_api_key}")
 
-            openai.api_key = openai_api_key
         except ImportError:
             raise ValueError(
                 "Could not import openai python package. "
                 "Please it install it with `pip install openai`."
             )
+
         try:
             values["client"] = openai.ChatCompletion
         except AttributeError:
             raise ValueError(
                 "`openai` has no `ChatCompletion` attribute, this is likely "
                 "due to an old version of the openai package. Try upgrading it "
                 "with `pip install --upgrade openai`."
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/__init__.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/chat.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/__init__.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def dynamic_tool_loader():
     try:
         all_tool_package_list = get_packages(f"{os.path.dirname(os.path.abspath(__file__))}")
     except Exception as e:
         LOG.debug(f"get_packages error: {repr(e)}")
         all_tool_package_list = ["meteo", "system", "web_requests", "wikipedia"]
-        LOG.debug(f"Detected main tool package: {repr(all_tool_package_list)}")
+        LOG.info(f"Detected main tool package: {repr(all_tool_package_list)}")
 
     for package_name in all_tool_package_list:
         try:
             import importlib
             importlib.import_module(f"chatgpt_tool_hub.tools.{package_name}")
         except Exception as e:
             LOG.info(f"[{package_name}] init failed, error_info: {repr(e)}")
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "Useful for when you need to answer questions about scientific research or search for papers "
         "Like: which papers has a certain author published? "
         "Input should be the title or abstract keywords or author names of a paper you want to search. "
     )
     bot: Any = None
 
     api_wrapper: ArxivAPIWrapper = None
+    arxiv_summary: bool = True
 
     def __init__(self, console: Console = Console(), **tool_kwargs: Any):
         super().__init__(console=console, return_direct=True)
 
         self.api_wrapper = ArxivAPIWrapper(**tool_kwargs)
         self.arxiv_summary = get_from_dict_or_env(tool_kwargs, "arxiv_summary", "ARXIV_SUMMARY", True)
 
@@ -57,15 +58,15 @@
             return _api_response
 
         temp_file = tempfile.mkstemp()
         file_path = temp_file[1]
         with open(file_path, "w") as f:
             f.write(_api_response + "\n")
 
-        _input = SummaryTool(max_segment_length=2400).run(f"{str(file_path)}, 0")
+        _input = SummaryTool(self.console, max_segment_length=2400).run(f"{str(file_path)}, 0")
         try:
             os.remove(file_path)
         except Exception as e:
             LOG.debug(f"remove {file_path} failed... error_info: {repr(e)}")
 
         return _input
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/wrapper.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/base_tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/wrapper.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/wrapper.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/load_tools.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/load_tools.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/docs_prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/docs_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 61, 63, 65	Rain: Slight, moderate and heavy intensity
 66, 67	Freezing Rain: Light and heavy intensity
 71, 73, 75	Snow fall: Slight, moderate, and heavy intensity
 77	Snow grains
 80, 81, 82	Rain showers: Slight, moderate, and violent
 85, 86	Snow showers slight and heavy
 
-Pay attention: 
+Think step by step: 
 1. You should only use the parameters described in this document to construct the API URL, 
 and should not make up parameters. If there is no parameter for daily granularity, 
 you can use the parameter for hourly granularity instead.
-2. If daily weather variables are specified, parameter timezone is required.
+2. Access weather information for no more than 3 days using the parameters start_date, or end_date.
 3. Parameter past_days is mutually exclusive with start_date and end_date.
-4. Your output can only be a URL, no need for explanation.
+4. If daily weather variables are specified, parameter timezone is required.
+5. Your output can only be a URL, no need for explanation.
 
 URL: """
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/tool.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 default_tool_name = "meteo-weather"
 
 
 class MeteoWeatherTool(BaseTool):
     name: str = default_tool_name
     description: str = (
-        "当你想要获取天气信息时应该使用本工具。"
-        "你需要分析用户想要哪些天气信息，严谨地用自然语言描述问题，然后将该问题传入本工具。"
-        "你最好能在输入末尾添加返回天气信息的粒度，支持：按时 或 按天，查询某天的天气优先用按时，遇到错误可以更换粒度"
+        "When you want to obtain weather information, use this tool. Analyze which weather information the user wants, "
+        "describe the problem rigorously in natural language, and then pass it on to this tool."
+        "It's best to append the weather granularity to the end of the input, such as 'by hour' or 'by day', "
+        "with priority given to 'by hour' when querying the weather on a specific day."
     )
     api_chain: APIChain = None
 
     def __init__(self, console: Console = Console(), **tool_kwargs):
         super().__init__(console=console, return_direct=False)
         llm = ModelFactory().create_llm_model(**build_model_params(tool_kwargs))
         self.api_chain = APIChain.from_llm_and_api_docs(llm, OPEN_METEO_DOCS, console=console)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/__init__.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.tools import get_packages
 from chatgpt_tool_hub.tools.tool_register import ToolRegister
 
 news_tool_register = ToolRegister()
+
 try:
     all_tool_package_list = get_packages(f"{os.path.dirname(os.path.abspath(__file__))}")
 except Exception as e:
     LOG.debug(f"get_packages error: {repr(e)}")
     all_tool_package_list = ["finance_news", "morning_news", "news_api"]
     LOG.debug(f"Detected main tool package: {repr(all_tool_package_list)}")
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 default_tool_name = "morning-news"
 
 
 class MorningNewsTool(BaseTool):
     name: str = default_tool_name
     description: str = (
-        "Use this tool when you want to get information about Daily 60 seconds morning news today. "
+        "Use this tool when you want to get information about Daily 60 seconds Chinese morning news today. "
         "no input."
     )
     bot: Any = None
     morning_news_api_key: str = ""
     morning_news_use_llm: bool = False
 
     def __init__(self, console: Console = Console(), **tool_kwargs: Any):
@@ -38,17 +38,14 @@
             input_variables=["morning_news"],
             template=SUMMARY_DOCS,
         )
         self.bot = LLMChain(llm=llm, prompt=prompt)
 
     def _run(self, query: str) -> str:
         """Use the tool."""
-        if not query:
-            return "the input of tool is empty"
-
         morning_news_url = f"https://v2.alapi.cn/api/zaobao?token={self.morning_news_api_key}&format=json"
         _response = RequestsWrapper().get(morning_news_url)
         _response_json = json.loads(_response)
         if self.morning_news_use_llm:
             return self.bot.run(_response)
         elif _response_json.get("code") == 200 or _response_json.get("msg") == "success":
             # 不使用llm，表明人类具有先天的优越性
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 
 class NewsTool(BaseTool):
     name: str = default_tool_name
     description: str = (
         "当你想要获取实时新闻资讯时可以使用该工具，你能获取任何与新闻有关的信息。"
         "该工具包含了金融、早报和news-api三个子工具，访问这些工具前你需要先访问本工具。"
-        "工具输入：你目前了解到的所有信息的总结 和 用户想获取的新闻内容。"
+        "工具输入：草稿的总结, 用户想获取的新闻内容"
     )
-    engine: ToolEngine = Any
+    engine: ToolEngine = None
 
     def __init__(self, console: Console = Console(), **tool_kwargs: Any):
         # 这个工具直接返回内容
         super().__init__(console=console, return_direct=True)
-
-        tools = load_tools(news_tool_register.get_registered_tool_names(), news_tool_register, console, **tool_kwargs)
+        # todo
+        tools = load_tools(["finance-news", "morning-news", "news-api"], news_tool_register, console, **tool_kwargs)
         llm = ModelFactory().create_llm_model(**build_model_params(tool_kwargs))
 
         # subtool 思考深度暂时固定为2
         self.engine = init_tool_engine(tools, llm, bot="qa-bot", verbose=True, console=self.console,
                                        max_iterations=2, early_stopping_method="force")
 
     def _run(self, query: str) -> str:
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/wrapper.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/map_prompt.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/map_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,17 @@
 default_tool_name = "summary"
 
 
 class SummaryTool(BaseTool):
     name = default_tool_name
     description = (
         "Useful when you want to summarize the content of a file. "
-        "The input is a comma-separated of file_path and a number. "
-        "The number represents summarizing only the first N lines of the file, "
-        "and when the number is 0, it means summarizing the entire file. "
-        "If you don't know what the file path is, you cannot use this tool."
+        "The input is a comma-separated of absolute path of the file and a number, like 'fakepath, 0'."
+        "The number indicates how many lines to summarize, with 0 meaning the entire file."
+        "You must know the file path to use this tool."
     )
 
     message_num: int = 100
     max_segment_length: int = 2500
 
     map_bot: Any = None
     reduce_bot: Any = None
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/answer_user.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/answer_user.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/debug.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/debug.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/base.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool_register.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool_register.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import List
 
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.common.singleton import Singleton
 
 
-class ToolRegister:
+class ToolRegister(Singleton):
+    REGISTER_TOOLS = {}
+
     def __init__(self):
-        self.REGISTER_TOOLS = {}
+        if not self.REGISTER_TOOLS:
+            self.REGISTER_TOOLS = {}
 
     def register_tool(self, name: str, function: callable, tool_input_keys: list):
         self.REGISTER_TOOLS[name] = (function, tool_input_keys)
 
     def unregister_tool(self, name: str) -> bool:
         if self.REGISTER_TOOLS.get(name):
             self.REGISTER_TOOLS.pop(name)
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/text2image.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/text2image.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class ImageCaptionTool(BaseTool):
     """Tool for get image captioning from image_path or url"""
 
     name = default_tool_name
     description = (
         "useful when you want to know what is inside the photo. receives image_path as input."
-        "The input to this tool should be a string, representing the image_path."
+        "The input to this tool should be a string, representing the image_path, you MUST use absolute path."
     )
     device: str = "cpu"
     torch_dtype: torch.dtype = torch.float32
     processor: Any = None
     model: Any = None
 
     def __init__(self, console: Console = Console(), **tool_kwargs):
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/__init__.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     # compress text size
     temp_file = tempfile.mkstemp()
     file_path = temp_file[1]
 
     with open(file_path, "w") as f:
         f.write(text + "\n")
+    # todo should input console
     _summary = SummaryTool().run(f"{str(file_path)}, 0")
     try:
         os.remove(file_path)
     except Exception as e:
         LOG.debug(f"remove {file_path} failed... error_info: {repr(e)}")
 
     return _summary.encode('utf-8').decode()
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/browser.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
+import time
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, Extra, root_validator
 from rich.console import Console
 
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.web_requests import filter_text
-
 default_tool_name = "browser"
 
 
 browser: Any = None  # ChromeWebDriver or None
 
 
 class ChromeBrowser(BaseModel):
@@ -64,19 +64,21 @@
 
         options = Options()
         options.add_argument(
             "user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
             "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.5615.49 Safari/537.36"
         )
         options.add_argument("--headless")
+        options.add_argument('blink-settings=imagesEnabled=false')
         options.add_argument("--disable-gpu")
         options.add_argument("--disable-extensions")
         options.add_argument("--ignore-certificate-errors")
         options.add_argument("--no-sandbox")
         options.add_argument(f"--proxy-server={proxy}")
+
         # 设置代理
         from webdriver_manager.chrome import ChromeDriverManager
         return webdriver.Chrome(
             executable_path=ChromeDriverManager().install(), options=options
         )
 
     def get(self, url: str, **kwargs) -> str:
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/delete.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/delete.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/get.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/get.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/patch.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/patch.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/post.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/post.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/put.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/put.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/wrapper.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wikipedia.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wrapper.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/PKG-INFO` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.3
+Version: 0.4.4
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -37,21 +37,30 @@
 
 ---
 
 简体中文 | [English](./docs/README_en.md)
 
 > 大语言模型涌现能力让人惊艳，ChatGPT出现给NLP技术带来革命，除此之外还让我意识到一种新的人机交互的可能性
 
-## 🌱 4.23 新增LLM-OS demo - [快速上手](#llm-os_jump)
-
-
-
-https://user-images.githubusercontent.com/24581028/233855116-ecbc5ea8-246b-46c6-8a1a-67ea6d970077.mp4
-
+<div>
+    <h2 style="display:inline; margin:0; padding:0;">🌱 5.4 LLM-OS demo在线演示</h2>
+    <a style="display:inline-block; align:center" src="https://colab.research.google.com/assets/colab-badge.svg" href="https://colab.research.google.com/drive/11nYPGFCYiaZ73H8nTHSN8ifbo0u3W_8p">
+        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="demo in Colab"/>
+    </a>
+</div>
+
+<br/>
+
+<div align="center">
+    <a style="text-decoration:none" href="https://www.bilibili.com/video/BV1eL411h7Nk/" target="_blank">
+        <img src="https://i.328888.xyz/2023/04/29/iJQNi3.jpeg" width = "659" height = "410" alt="LLM-OS" align=center />
+    </a>
+</div>
 
+<br/>
 
 #### [更新日志](./docs/update_log.md) | [Q&A](./docs/q_and_a.md)
 
 ## 简介
 
 ---
 
@@ -84,16 +93,14 @@
 
 ## ✈️ 快速开始
 
 ---
 
 ### 1.  LLM-OS demo
 
-<span id="llm-os_jump"></span>
-
 #### (1). 克隆仓库
 
 ```bash
 git clone https://github.com/goldfishh/chatgpt-tool-hub.git
 cd chatgpt-tool-hub
 ```
 
@@ -103,15 +110,15 @@
 pip3 install -r requirements.txt
 ```
 
 #### (3). 重命名.env.template 和 config.json.template文件，去掉.template后缀 打开文件填入配置参数 
 
 `.env` 用于配置全局参数 文件配置示例
 ```text
-OPENAI_API_KEY=sk-xx          // 必填，你的OPENAI API Key, 如何申请请见Q&A
+LLM_API_KEY=sk-xx          // 必填，你的OPENAI API Key, 如何申请请见Q&A
 MODEL_NAME=gpt-3.5-turbo      // 选填，OPENAI LLM模型
 THINK_DEPTH=3                 // 选填，默认为3，控制LLM-OS的最大调用工具次数，过大不一定能提高回复质量
 REQUEST_TIMEOUT=90            // 选填，默认120，等待openai api回复的最大时间
 PROXY=http://192.168.7.1:7890 // 选填，当你需要代理访问openai时可填
 DEBUG=false                   // 选填，debug模式
 ```
 
@@ -133,15 +140,15 @@
 
 ```bash
 python3 terminal_io.py
 ```
 
 #### (5). 进入LLM-OS后你可以自行探索 或者进一步浏览详细教程：[LLM_OS demo使用说明](https://github.com/goldfishh/llm-os/blob/main/README.md)
 
---- 
+---
 
 ### 2. 我给[chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat)开发了tool插件
 
 > 使用本方法，你将可以用微信作为前端更方便地使用tool-hub
 
 #### 查阅chatgpt-on-wechat文档中的[项目简介](https://github.com/zhayujie/chatgpt-on-wechat#%E7%AE%80%E4%BB%8B) 和 [快速开始](https://github.com/zhayujie/chatgpt-on-wechat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
 
@@ -162,60 +169,48 @@
 ```
 
 #### (2). 快速开始
 
 ```python
 import os
 from chatgpt_tool_hub.apps import AppFactory
-os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"  # 必填
+os.environ["LLM_API_KEY"] = "YOUR_LLM_API_KEY"  # 必填
 os.environ["PROXY"] = "YOUR_PROXY_ADDRESS"            # 选填
 app = AppFactory().create_app(tools_list=[], **{})
 reply = app.ask("YOUR_QUESTION_TO_HERE")
 print(reply)
 ```
 
 #### (3). 以插件形式接入tool-hub可参考tool插件实现
 
 [tool.py](https://github.com/goldfishh/chatgpt-on-wechat/blob/master/plugins/tool/tool.py)
 
 > 如果有需求，我会更新更详细接入的文档，欢迎提issue
 
 ---
 
-## ☕ 宣传
-
-#### 如果你想支持本项目，欢迎给项目点个star、提issue和pr
-#### 如果你想进一步支持项目作者少掉头发，努力开发，可以给和我一起开发项目的伙伴 或 单独给我来杯 ☕
-
-<table><tr>
-<td><a href="https://public.zsxq.com/groups/88885848842852.html"><img src="https://github.com/zhayujie/chatgpt-on-wechat/blob/master/docs/images/planet.jpg?raw=true" width="400" height="200" border=0></a></td>
-<td><img src="./assets/buy_me_a_coffee.jpg" width="200" height="200" border=0 /></td>
-</tr></table> 
-
----
-
 ## 工具指南 
 
 ### 🚀 [工具指南 工具快速开发中](./docs/tool_tutorial.md)
 
 ---
 
 ## 原理
 
 ---
 
 工具引擎的实现原理本质是**Chain-of-Thought**：[Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)
-  
+
 我将通过用6个自问自答的问题解释chatgpt-tool-hub的工作原理  
 
 #### 1. 事务型工具（如terminal、python）是在哪运行，以及如何执行的
 
 事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、url-get工具分别用到了封装调用subprocess库、python解释器和requests库的函数
 
---- 
+---
 
 #### 2. ChatGPT是如何触发调用这些函数
 
 借助ChatGPT api提供的temperature参数，该参数越低，ChatGPT输出的结果会更集中和确定，当temperature为0时，相同的问题会得到统一回答  
 我在prompt构建时会提供给ChatGPT此时用到的工具列表信息，每个工具信息包含：工具名 和 工具描述：
 
 ```text
@@ -254,25 +249,25 @@
 
 ```text
 Observation: 当事务函数执行完成返回时的内容
 ```
 
 带Observation前缀的内容往往是使用事务型工具的用户想知道的答案
 
---- 
-  
+---
+
 #### 3. ChatGPT怎么知道该用的工具和输入，是否每次都严格按照prompt生成格式化内容
 
 ChatGPT微调时进行大量Q&A、CoT预料的学习和RLHF调优，目前ChatGPT对于工具和内容生成的质量是有保证的  
 但是目前不是100%，因为会有低质量prompt或者不合适工具的输入，这些问题在工具引擎会进行鲁棒性的处理来保证生成内容的稳定性  
 
 我创建一个issue，可以方便大家来获取和分享使用tool过程解决的有趣问题和思路、每个tool使用时prompt技巧、遇到问题的处理办法：
 [更好的使用tool的技巧交流](https://github.com/goldfishh/chatgpt-tool-hub/issues/3)
 
---- 
+---
 
 #### 4. 如果需要多个工具交替配合解决某个问题，引擎是怎么做的？
 
 当事务函数处理完成返回结果后，默认不会直接返回给用户，而是根据结果内容CoT，在整个prompt中，还有两个子prompt负责用户对话历史记录和中间结果
 
 用户对话历史记录：
 ```text
@@ -287,51 +282,51 @@
 Action: Wolfram Alpha
 Action Input: gdp china vs. usa
 Observation: China\nUnited States | GDP | nominal \nAnswer: China | $14.72 trillion per year\nUnited States | $20.95 trillion per year\n(2020 estimates)
 Thought:
 ```
 
 每轮工具CoT过程均会作为下次推理判断工具的依据，由此迭代地进行工具判断、执行，最后当识别到特定前缀时，CoT结果将返回给用户    
-  
+
 CoT结束prompt：
 ```text
 When you have a response to say to the Human, or if you do not need to use a tool, you MUST use the format:
 
 Thought: Do I need to use a tool? No
 AI: the response to the original input question in chinese
 
 ```
 
 
 ChatGPT使用工具过程并不顺利：当遇到迭代次数到达预设值时，会根据历史过程，返回给用户最后结果    
 
---- 
+---
 
 #### 5. 事务性工具交给ChatGPT是否具有不可预料的危险性？
 
 是的，当你用事务性工具时，你就给予了ChatGPT在你本地运行程序的权利，你需要权限限制来规避可能的风险      
 如果无法信任ChatGPT主导你的机器，请不要使用  
 
---- 
+---
 
 #### 6. 非事务型工具的实现原理是什么
 
 参考[ChatGPT 官方插件](https://github.com/openai/chatgpt-retrieval-plugin)，非事务性工具也称为插件型工具，该工具可视为开放性的ChatGPT插件
 
 ---
 
 
 ## 🎯 计划
 
 <span id="plan"></span>
 
 ---
- 
+
 ### feature todolist
-  
+
 [✓] 结果可解释性输出 -> LLM-OS的内心独白  
 [✓] 一个前端demo  -> LLM-OS  
 [✓] 长文本场景 -> summary工具  
 [✓] 长工具顺序控制 -> 实现了toolintool机制    
 [✓] 粒度配置 -> 每个tool封装的LLM可独立配置  
 [○] tokens计算，精确管理    
 [○] gpt_index长文本(pdf、html)检索   
@@ -339,46 +334,62 @@
 [○] 接入国内LLM  
 [○] 兼容不使用tool的场景  
 [○] 互斥tool控制  
 [○] subtree 动态注册&反注册  
 [○] 工具中断  
 [○] 定时调度  
 [○] 语音输入、输出  
-  
+
 ### tool todolist  
-   
+
 [○] stable-diffusion 中文prompt翻译    
 [✓] ImageCaptioning    
 [○] 小米智能家居控制    
 [○] 支持ChatGPT官方插件  
 [○] 让LLM来实现tool  
 [○] 支持图片处理工具    
 [○] 支持视频处理工具   
 [✗] Wechat  
 
 ## 工具开发指南
 
 ---
- 
+
 目前工具分为两类：事务型工具、插件型工具   
- 
-我等待有需求之后更新这部分内容    
 
 [工具开发教程](./docs/tool_development_guide.md)
 
 ## 背景
 
 我将很快更新这部分内容   
 
 ---
 
+## ☕ 宣传
+
+#### 如果你想支持本项目，欢迎给项目点个star、提issue和pr
+#### 如果你想进一步支持项目作者少掉头发，努力开发，可以给和我一起开发项目的伙伴 或 单独给我来杯 ☕
+
+<table><tr>
+<td><a href="https://public.zsxq.com/groups/88885848842852.html"><img src="https://github.com/zhayujie/chatgpt-on-wechat/blob/master/docs/images/planet.jpg?raw=true" width="400" height="200" border=0></a></td>
+<td><img src="./assets/buy_me_a_coffee.jpg" width="200" height="200" border=0 /></td>
+</tr></table> 
+
+---
+
 ## 感谢
 
 感谢以下项目对本项目提供的有力支持：
 
-#### 1. [langchain](https://github.com/hwchase17/langchain)
+#### 1. [langchain](https://github.com/hwchase17/langchain) 
+
+受langchain的启发，本项目重写了langchain v0.0.123 工具有关的实现
 
 #### 2. [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
+启发了browser tool跨平台的实现、tool engine的json通信、部分prompt描述
+
 #### 3. [chatgpt-in-terminal](https://github.com/xiaoxx970/chatgpt-in-terminal)
 
+llm-os demo 改写自该项目
+
 ---
```

### Comparing `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/SOURCES.txt` & `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,19 @@
 chatgpt_tool_hub/engine/__init__.py
 chatgpt_tool_hub/engine/bot.py
 chatgpt_tool_hub/engine/initialize.py
 chatgpt_tool_hub/engine/tool_engine.py
 chatgpt_tool_hub/models/__init__.py
 chatgpt_tool_hub/models/base.py
 chatgpt_tool_hub/models/model_factory.py
-chatgpt_tool_hub/models/openai.py
 chatgpt_tool_hub/models/chatgpt/__init__.py
 chatgpt_tool_hub/models/chatgpt/base.py
 chatgpt_tool_hub/models/chatgpt/chatgpt.py
+chatgpt_tool_hub/models/dashscope/__init__.py
+chatgpt_tool_hub/models/moss/__init__.py
 chatgpt_tool_hub/prompts/__init__.py
 chatgpt_tool_hub/prompts/base.py
 chatgpt_tool_hub/prompts/chat.py
 chatgpt_tool_hub/prompts/prompt.py
 chatgpt_tool_hub/tools/__init__.py
 chatgpt_tool_hub/tools/all_tool_list.py
 chatgpt_tool_hub/tools/base_tool.py
@@ -73,14 +74,16 @@
 chatgpt_tool_hub/tools/arxiv_search/wrapper.py
 chatgpt_tool_hub/tools/bing_search/__init__.py
 chatgpt_tool_hub/tools/bing_search/tool.py
 chatgpt_tool_hub/tools/bing_search/wrapper.py
 chatgpt_tool_hub/tools/google_search/__init__.py
 chatgpt_tool_hub/tools/google_search/tool.py
 chatgpt_tool_hub/tools/google_search/wrapper.py
+chatgpt_tool_hub/tools/hello_tool/__init__.py
+chatgpt_tool_hub/tools/hello_tool/tool.py
 chatgpt_tool_hub/tools/meteo/__init__.py
 chatgpt_tool_hub/tools/meteo/docs_prompt.py
 chatgpt_tool_hub/tools/meteo/tool.py
 chatgpt_tool_hub/tools/news/__init__.py
 chatgpt_tool_hub/tools/news/tool.py
 chatgpt_tool_hub/tools/news/finance_news/__init__.py
 chatgpt_tool_hub/tools/news/finance_news/tool.py
```

### Comparing `chatgpt-tool-hub-0.4.3/setup.py` & `chatgpt-tool-hub-0.4.4/setup.py`

 * *Files identical despite different names*

