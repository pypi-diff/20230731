# Comparing `tmp/alphawave-0.3.97.tar.gz` & `tmp/alphawave-0.3.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.97.tar", last modified: Wed Jul 26 15:20:25 2023, max compression
+gzip compressed data, was "alphawave-0.3.98.tar", last modified: Sun Jul 30 23:35:33 2023, max compression
```

## Comparing `alphawave-0.3.97.tar` & `alphawave-0.3.98.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.97/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-26 15:20:25.443503 alphawave-0.3.97/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.97/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1038 2023-07-26 15:19:59.000000 alphawave-0.3.97/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-26 15:20:25.443503 alphawave-0.3.97/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.435503 alphawave-0.3.97/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.435503 alphawave-0.3.97/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9760 2023-07-26 01:49:42.000000 alphawave-0.3.97/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-07-25 20:51:35.000000 alphawave-0.3.97/src/alphawave/ChoiceResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.97/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.97/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8202 2023-07-25 03:45:02.000000 alphawave-0.3.97/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.97/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6803 2023-07-23 02:16:38.000000 alphawave-0.3.97/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5920 2023-07-23 02:28:01.000000 alphawave-0.3.97/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-16 20:12:02.000000 alphawave-0.3.97/src/alphawave/PythonResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.97/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.97/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8938 2023-07-25 17:23:29.000000 alphawave-0.3.97/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.97/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.97/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.97/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.97/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.97/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.97/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.435503 alphawave-0.3.97/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2175 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      209 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.439503 alphawave-0.3.97/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    17577 2023-07-23 03:33:26.000000 alphawave-0.3.97/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.97/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7197 2023-07-21 01:51:42.000000 alphawave-0.3.97/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-07-23 03:31:47.000000 alphawave-0.3.97/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.97/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.97/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-23 03:32:25.000000 alphawave-0.3.97/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-23 03:32:00.000000 alphawave-0.3.97/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3236 2023-07-24 16:02:13.000000 alphawave-0.3.97/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7932 2023-07-23 03:32:46.000000 alphawave-0.3.97/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.97/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.97/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.97/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.97/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.97/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6403 2023-07-23 02:20:11.000000 alphawave-0.3.97/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2897 2023-07-23 03:22:29.000000 alphawave-0.3.97/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10249 2023-07-20 20:27:59.000000 alphawave-0.3.97/src/alphawave_pyexts/agentChat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10823 2023-07-20 20:44:34.000000 alphawave-0.3.97/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-07-20 20:28:15.000000 alphawave-0.3.97/src/alphawave_pyexts/chatglm2.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.97/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    26601 2023-07-25 21:05:22.000000 alphawave-0.3.97/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      742 2023-07-20 20:28:29.000000 alphawave-0.3.97/src/alphawave_pyexts/falcon7.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.97/src/alphawave_pyexts/handler.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1094 2023-07-20 20:29:07.000000 alphawave-0.3.97/src/alphawave_pyexts/llama-2-13b-chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1387 2023-07-20 20:29:07.000000 alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b-chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      894 2023-07-20 20:29:07.000000 alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13634 2023-07-23 02:23:28.000000 alphawave-0.3.97/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      941 2023-07-23 02:25:16.000000 alphawave-0.3.97/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.97/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.97/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8664 2023-07-23 02:19:51.000000 alphawave-0.3.97/src/alphawave_pyexts/utilityV2.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      831 2023-07-20 20:29:42.000000 alphawave-0.3.97/src/alphawave_pyexts/vicuna13.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      813 2023-07-20 20:29:35.000000 alphawave-0.3.97/src/alphawave_pyexts/vicuna7.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1121 2023-07-20 20:29:58.000000 alphawave-0.3.97/src/alphawave_pyexts/wvicuna30.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.97/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.97/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.120965 alphawave-0.3.98/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.98/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-30 23:35:33.120965 alphawave-0.3.98/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.98/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1038 2023-07-30 23:35:23.000000 alphawave-0.3.98/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-30 23:35:33.120965 alphawave-0.3.98/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.112965 alphawave-0.3.98/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.116965 alphawave-0.3.98/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9760 2023-07-26 01:49:42.000000 alphawave-0.3.98/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2567 2023-07-27 19:27:45.000000 alphawave-0.3.98/src/alphawave/ChoiceResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.98/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.98/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8202 2023-07-25 03:45:02.000000 alphawave-0.3.98/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.98/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6557 2023-07-27 01:30:23.000000 alphawave-0.3.98/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5920 2023-07-23 02:28:01.000000 alphawave-0.3.98/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-16 20:12:02.000000 alphawave-0.3.98/src/alphawave/PythonResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.98/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.98/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8938 2023-07-25 17:23:29.000000 alphawave-0.3.98/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.98/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.98/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.98/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1403 2023-07-27 01:09:56.000000 alphawave-0.3.98/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.98/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.98/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.116965 alphawave-0.3.98/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-30 23:35:33.000000 alphawave-0.3.98/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2175 2023-07-30 23:35:33.000000 alphawave-0.3.98/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-30 23:35:33.000000 alphawave-0.3.98/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      209 2023-07-30 23:35:33.000000 alphawave-0.3.98/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-30 23:35:33.000000 alphawave-0.3.98/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.116965 alphawave-0.3.98/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17577 2023-07-23 03:33:26.000000 alphawave-0.3.98/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.98/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7197 2023-07-21 01:51:42.000000 alphawave-0.3.98/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-07-23 03:31:47.000000 alphawave-0.3.98/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.98/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.98/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-23 03:32:25.000000 alphawave-0.3.98/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-23 03:32:00.000000 alphawave-0.3.98/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3236 2023-07-24 16:02:13.000000 alphawave-0.3.98/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7932 2023-07-23 03:32:46.000000 alphawave-0.3.98/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.98/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.98/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.98/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.98/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.120965 alphawave-0.3.98/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.98/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6576 2023-07-27 02:39:06.000000 alphawave-0.3.98/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2897 2023-07-23 03:22:29.000000 alphawave-0.3.98/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10249 2023-07-20 20:27:59.000000 alphawave-0.3.98/src/alphawave_pyexts/agentChat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10823 2023-07-20 20:44:34.000000 alphawave-0.3.98/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-07-20 20:28:15.000000 alphawave-0.3.98/src/alphawave_pyexts/chatglm2.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.98/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    26601 2023-07-25 21:05:22.000000 alphawave-0.3.98/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      742 2023-07-20 20:28:29.000000 alphawave-0.3.98/src/alphawave_pyexts/falcon7.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.98/src/alphawave_pyexts/handler.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1094 2023-07-20 20:29:07.000000 alphawave-0.3.98/src/alphawave_pyexts/llama-2-13b-chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1387 2023-07-20 20:29:07.000000 alphawave-0.3.98/src/alphawave_pyexts/llama-2-70b-chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      894 2023-07-20 20:29:07.000000 alphawave-0.3.98/src/alphawave_pyexts/llama-2-70b.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.120965 alphawave-0.3.98/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13634 2023-07-23 02:23:28.000000 alphawave-0.3.98/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      941 2023-07-23 02:25:16.000000 alphawave-0.3.98/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.98/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.98/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8750 2023-07-30 23:32:23.000000 alphawave-0.3.98/src/alphawave_pyexts/utilityV2.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      831 2023-07-20 20:29:42.000000 alphawave-0.3.98/src/alphawave_pyexts/vicuna13.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      813 2023-07-20 20:29:35.000000 alphawave-0.3.98/src/alphawave_pyexts/vicuna7.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1121 2023-07-20 20:29:58.000000 alphawave-0.3.98/src/alphawave_pyexts/wvicuna30.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-30 23:35:33.120965 alphawave-0.3.98/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.98/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.98/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.97/LICENSE` & `alphawave-0.3.98/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/PKG-INFO` & `alphawave-0.3.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.97
+Version: 0.3.98
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.97/README.md` & `alphawave-0.3.98/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/pyproject.toml` & `alphawave-0.3.98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.97"
+version = "0.3.98"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
```

### Comparing `alphawave-0.3.97/src/alphawave/AlphaWave.py` & `alphawave-0.3.98/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/ChoiceResponseValidator.py` & `alphawave-0.3.98/src/alphawave/ChoiceResponseValidator.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,32 +6,50 @@
 class ChoiceResponseValidator(PromptResponseValidator):
     def __init__(self, choices=None, missing_choice_feedback="Response did not contain a choice from "):
         self.choices = []
         if choices is None or type(choices) != list:
             print(f' ChoiceResponseValidator init must be provided a list of string choices')
         else:
             for choice in choices:
-                self.choices.append(choice.lower())
+                self.choices.append(choice)
         self.missing_choice_feedback = missing_choice_feedback+str(self.choices)
         
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts) -> Validation:
-        message = response['message']
+        message = response['message']['content']
         if type(message) != str:
             text = str(message)
         else:
             text = message
+        min_find = 99999
+        found_choice = ''
+        # find first choice in first few chars of returned text. first look for matched case
+        for choice in self.choices:
+            c = choice
+            i = text.find(c)
+            if i >=0:
+                if i < min_find or i == min_find and len(c) > len(found_choice):
+                    # this will make sure 'does not' beats 'does' in same start pos!
+                    min_find = i
+                    found_choice = choice # return choice as capitalized in spec
+        if min_find < 15:
+            return {
+                'type': 'Validation',
+                'valid': True,
+                'value': found_choice
+            }
+                
+        min_find = 99999
         text = text.lower()
-        min_find = 9999
-        # find first choice in returned text. Sloppy, could check for multiple choice matches.
         for choice in self.choices:
-            if choice in text:
-                if text.find(choice) < min_find or (text.find(choice) == min_find and len(choice) > len(found_choice)):
+            c = choice.lower()
+            if c in text:
+                if text.find(c) < min_find or (text.find(c) == min_find and len(c) > len(found_choice)):
                     # this will make sure 'does not' beats 'does' in same start pos!
-                    min_find = text.find(choice)
-                    found_choice = choice
+                    min_find = text.find(c) # ignore case in match
+                    found_choice = choice # return choice as capitalized in spec
         if min_find < 9999:
             return {
                 'type': 'Validation',
                 'valid': True,
                 'value': found_choice
             }
```

### Comparing `alphawave-0.3.97/src/alphawave/Colorize.py` & `alphawave-0.3.98/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.98/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.98/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/MemoryFork.py` & `alphawave-0.3.98/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/OSClient.py` & `alphawave-0.3.98/src/alphawave/OSClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,46 +66,44 @@
             if self.options.endpoint.endswith('/'):
                 self.options.endpoint = self.options.endpoint[:-1]
 
         self._session = requests.Session()
 
     def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
         if isinstance(options, dict):
+            # convert to PCO object
             argoptions = options
             options = PromptCompletionOptions(completion_type = argoptions['completion_type'],
                                               model = argoptions['model'],
                                               max_input_tokens = argoptions['max_input_tokens'],
                                               temperature = argoptions['temperature'],
                                               top_p = argoptions['top_p'],
                                               max_tokens = argoptions['max_tokens'],
                                               stop = argoptions['stop'],
-                                              presence_penalty = argoptions['presence_penalty'],
-                                              frequency_penalty = argoptions['frequency_penalty']
+                                              choice_set = argoptions['choice_set']
                                               )
         startTime = time.time()
         max_input_tokens = 1500
         if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
             max_input_tokens = options.max_input_tokens
         
-        result = prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
+        rendered_prompt = prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
         
-        if result.tooLong:
+        if rendered_prompt.tooLong:
             return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
         if self.options.logRequests:
             print(Colorize.title('CHAT PROMPT:'))
-            for msg in result.output:
+            for msg in rendered_prompt.output:
                 if not isinstance(msg, dict):
                     print(Colorize.output(msg))
                     msg = msg.__dict__
                 print(Colorize.output(json.dumps(msg, indent=2)), end='')
             print()
 
-        request = self.copyOptionsToRequest(CreateChatCompletionRequest(model = options.model, messages =  result.output), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
-
-        response = self.createChatCompletion(request)
+        response = self.createChatCompletion(rendered_prompt.output, options)
         if self.options.logRequests:
             print(Colorize.title('CHAT RESPONSE:'))
             print(Colorize.value('status', response.status))
             print(Colorize.value('duration', time.time() - startTime, 'ms'))
             print(Colorize.output(response.message))
         
         if response.status == 'success':
@@ -121,26 +119,27 @@
 
     def copyOptionsToRequest(self, target: Dict[str, Any], src: Any, fields: list) -> Dict[str, Any]:
         for field in fields:
             if hasattr(src, field) and getattr(src, field) is not None:
                 setattr(target,field, getattr(src,field))
         return target
 
-    def createChatCompletion(self, request: CreateChatCompletionRequest) -> requests.Response:
+    def createChatCompletion(self, messages, options) -> requests.Response:
         url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/chat/completions"
         requestHeaders = {
             'Content-Type': 'application/json',
             'User-Agent': self.UserAgent
         }
         result = ''
         try:
-            result = ut.ask_LLM(request.model,
-                                request.messages,
-                                request.max_tokens,
-                                request.temperature,
-                                request.top_p,
-                                self.options.endpoint,
-                                self.options.port
+            result = ut.ask_LLM(options.model,
+                                messages,
+                                max_tokens=options.max_tokens,
+                                temp=options.temperature,
+                                top_p=options.top_p,
+                                host=self.options.endpoint,
+                                port=self.options.port,
+                                choice_set=options.choice_set
                                 )
         except Exception as e:
             return PromptResponse(status='error',message=str(e))
         return PromptResponse(status='success', message=result)
```

### Comparing `alphawave-0.3.97/src/alphawave/OpenAIClient.py` & `alphawave-0.3.98/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/PythonResponseValidator.py` & `alphawave-0.3.98/src/alphawave/PythonResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/RepairTestClient.py` & `alphawave-0.3.98/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/Response.py` & `alphawave-0.3.98/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.98/src/alphawave/TOMLResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/TestClient.py` & `alphawave-0.3.98/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/TestClientTest.py` & `alphawave-0.3.98/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.98/src/alphawave/alphawaveTypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     completion_type: str  = 'chat' # 'text' | 'chat'
     model: str = ''
     max_input_tokens: int =8000
     temperature: float = 0.7
     top_p: float = 1.0
     max_tokens: int = 500
     stop: str = None
+    choice_set: list=None
     #presence_penalty: float = 1.0
     #frequency_penalty: float = 1.0
     #logit_bias = None
     #best_of = None
 
 PromptResponseStatus = ['success', 'error', 'rate_limited', 'invalid_response', 'too_long']
```

### Comparing `alphawave-0.3.97/src/alphawave/internalTypes.py` & `alphawave-0.3.98/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave/jsonParser.py` & `alphawave-0.3.98/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.98/src/alphawave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.97
+Version: 0.3.98
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.97/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.98/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/Agent.py` & `alphawave-0.3.98/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.98/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.98/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.98/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.98/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.98/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.98/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.98/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.98/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.98/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.98/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.98/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.98/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.98/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.98/src/alphawave_pyexts/LLMClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 host='192.168.1.195'
 port = 5004
 
 
 def get_available_models():
     return list(cv.conv_templates.keys())
 
-def run_query(model, messages, max_tokens, temp, top_p, host = host, port = port, tkroot = None, tkdisplay=None, format=True): 
+def run_query(model, messages, max_tokens, temp, top_p, host = host, port = port, choice_set=None, tkroot = None, tkdisplay=None, format=True): 
     global USER_PREFIX, ASSISTANT_PREFIX, SYSTEM_PREFIX
 
     conv=cv.get_conv_template(model)
     user_prompt = conv.roles[0]
     asst_prompt = conv.roles[1]
     system_prompt = conv.roles[1]
     
@@ -64,20 +64,24 @@
         if len(prime) > 0:
             prompt = prime+conv.sep+prompt
     else:
         prompt = messages
     prompt = re.sub('\n{3,}', '\n\n', prompt)
     #print(f'***** llm output prompt string {prompt}')
     server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens, 'user_prompt':USER_PREFIX}
+    if choice_set:
+        server_message['choice_set']=choice_set
     smj = json.dumps(server_message)
     try:
         client_socket = socket.socket()  # instantiate
         client_socket.connect((host, port))  # connect to the server
         client_socket.settimeout(240)
         server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens, 'user':user_prompt, 'asst':asst_prompt}
+        if choice_set is not None:
+            server_message['choice_set'] = choice_set
         smj = json.dumps(server_message)
         client_socket.sendall(smj.encode('utf-8'))
         client_socket.sendall(b'x00xff')
         response = ''
         while True:
             s = client_socket.recv(1024) # break every 32 chars to stream output
             if s is None or not s:
```

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.98/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/agentChat.py` & `alphawave-0.3.98/src/alphawave_pyexts/agentChat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/chat.py` & `alphawave-0.3.98/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/chatglm2.py` & `alphawave-0.3.98/src/alphawave_pyexts/chatglm2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.98/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.98/src/alphawave_pyexts/conversation.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/falcon7.py` & `alphawave-0.3.98/src/alphawave_pyexts/falcon7.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/handler.py` & `alphawave-0.3.98/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/llama-2-13b-chat.py` & `alphawave-0.3.98/src/alphawave_pyexts/llama-2-13b-chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b-chat.py` & `alphawave-0.3.98/src/alphawave_pyexts/llama-2-70b-chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b.py` & `alphawave-0.3.98/src/alphawave_pyexts/llama-2-70b.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.98/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.98/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.98/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.98/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.98/src/alphawave_pyexts/utilityV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 from alphawave.alphawaveTypes import PromptCompletionOptions
 from alphawave_agents.PromptCommand import CommandSchema, PromptCommandOptions
 from alphawave.AlphaWave import AlphaWave
 from alphawave.DefaultResponseValidator import DefaultResponseValidator
 from alphawave.JSONResponseValidator import JSONResponseValidator
 from alphawave.TOMLResponseValidator import TOMLResponseValidator
 from alphawave.MemoryFork import MemoryFork
-
+import tkinter as tk
 openai.api_key = os.getenv("OPENAI_API_KEY")
 google_key = os.getenv("GOOGLE_KEY")
 google_cx = os.getenv("GOOGLE_CX")
 GOOGLE = 'google'
 
-def ask_LLM(model, gpt_message, max_tokens=100, temp=0.7, top_p=1.0, host = None, port = None, tkroot = None, tkdisplay=None):
+def ask_LLM(model, gpt_message, max_tokens=100, temp=0.7, top_p=1.0, host = None, port = None, choice_set=None, tkroot = None, tkdisplay=None):
     completion = None
     response = ''
     #print(f'***** utility ask_LLL temperature {temp}')
     try:
       if not model.lower().startswith('gpt'):
-        completion = llm.run_query(model, gpt_message, max_tokens, temp, top_p, host, port, tkroot, tkdisplay )
+        completion = llm.run_query(model, gpt_message, max_tokens, temp, top_p, choice_set=choice_set, host=host, port=port, tkroot=tkroot, tkdisplay=tkdisplay)
         if completion is not None:
           response = completion
 
       else:
         stream= openai.ChatCompletion.create(
             model=model, messages=gpt_message, max_tokens=max_tokens, temperature=temp, top_p=1, stop='STOP', stream=True)
         response = ''
```

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/vicuna13.py` & `alphawave-0.3.98/src/alphawave_pyexts/vicuna13.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/vicuna7.py` & `alphawave-0.3.98/src/alphawave_pyexts/vicuna7.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/src/alphawave_pyexts/wvicuna30.py` & `alphawave-0.3.98/src/alphawave_pyexts/wvicuna30.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/tests/testOSClient.py` & `alphawave-0.3.98/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.97/tests/testOpenAiClient.py` & `alphawave-0.3.98/tests/testOpenAiClient.py`

 * *Files identical despite different names*

