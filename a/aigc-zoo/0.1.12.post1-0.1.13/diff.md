# Comparing `tmp/aigc_zoo-0.1.12.post1-py3-none-any.whl.zip` & `tmp/aigc_zoo-0.1.13-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 73205 bytes, number of entries: 46
+Zip file size: 73580 bytes, number of entries: 48
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-26 02:52 aigc_zoo/.gitignore
 -rw-rw-rw-  2.0 fat       80 b- defN 23-Jun-26 02:52 aigc_zoo/__init__.py
+-rw-rw-rw-  2.0 fat      105 b- defN 23-Jul-31 06:56 aigc_zoo/requirements.txt
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-26 02:52 aigc_zoo/model_zoo/__init__.py
 -rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-26 02:52 aigc_zoo/model_zoo/baichuan/__init__.py
 -rw-rw-rw-  2.0 fat     5578 b- defN 23-Jul-10 04:30 aigc_zoo/model_zoo/baichuan/llm_model.py
 -rw-rw-rw-  2.0 fat     9574 b- defN 23-Jun-26 02:52 aigc_zoo/model_zoo/baichuan/tokenization_baichuan.py
 -rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-26 02:52 aigc_zoo/model_zoo/baichuan2/__init__.py
 -rw-rw-rw-  2.0 fat     5575 b- defN 23-Jul-11 04:15 aigc_zoo/model_zoo/baichuan2/llm_model.py
 -rw-rw-rw-  2.0 fat     8720 b- defN 23-Jul-11 03:13 aigc_zoo/model_zoo/baichuan2/tokenization_baichuan.py
@@ -36,13 +38,13 @@
 -rw-rw-rw-  2.0 fat     5848 b- defN 23-Jul-10 04:30 aigc_zoo/model_zoo/t5/ppo_model.py
 -rw-rw-rw-  2.0 fat     9098 b- defN 23-Jul-10 04:30 aigc_zoo/model_zoo/t5/reward_model.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-26 02:52 aigc_zoo/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2664 b- defN 23-Jul-12 07:02 aigc_zoo/utils/llm_generate.py
 -rw-rw-rw-  2.0 fat    13198 b- defN 23-Jul-14 00:27 aigc_zoo/utils/moss_generate.py
 -rw-rw-rw-  2.0 fat     3429 b- defN 23-Jul-17 03:15 aigc_zoo/utils/rwkv4_generate.py
 -rw-rw-rw-  2.0 fat      748 b- defN 23-Jul-26 05:46 aigc_zoo/utils/streamgenerator.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-26 08:20 aigc_zoo-0.1.12.post1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      357 b- defN 23-Jul-26 08:20 aigc_zoo-0.1.12.post1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 08:20 aigc_zoo-0.1.12.post1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-26 08:20 aigc_zoo-0.1.12.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     4296 b- defN 23-Jul-26 08:20 aigc_zoo-0.1.12.post1.dist-info/RECORD
-46 files, 224047 bytes uncompressed, 66177 bytes compressed:  70.5%
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-31 07:00 aigc_zoo-0.1.13.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      351 b- defN 23-Jul-31 07:00 aigc_zoo-0.1.13.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 07:00 aigc_zoo-0.1.13.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-31 07:00 aigc_zoo-0.1.13.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     4420 b- defN 23-Jul-31 07:00 aigc_zoo-0.1.13.dist-info/RECORD
+48 files, 224277 bytes uncompressed, 66372 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -1,10 +1,16 @@
+Filename: aigc_zoo/.gitignore
+Comment: 
+
 Filename: aigc_zoo/__init__.py
 Comment: 
 
+Filename: aigc_zoo/requirements.txt
+Comment: 
+
 Filename: aigc_zoo/model_zoo/__init__.py
 Comment: 
 
 Filename: aigc_zoo/model_zoo/baichuan/__init__.py
 Comment: 
 
 Filename: aigc_zoo/model_zoo/baichuan/llm_model.py
@@ -117,23 +123,23 @@
 
 Filename: aigc_zoo/utils/rwkv4_generate.py
 Comment: 
 
 Filename: aigc_zoo/utils/streamgenerator.py
 Comment: 
 
-Filename: aigc_zoo-0.1.12.post1.dist-info/LICENSE
+Filename: aigc_zoo-0.1.13.dist-info/LICENSE
 Comment: 
 
-Filename: aigc_zoo-0.1.12.post1.dist-info/METADATA
+Filename: aigc_zoo-0.1.13.dist-info/METADATA
 Comment: 
 
-Filename: aigc_zoo-0.1.12.post1.dist-info/WHEEL
+Filename: aigc_zoo-0.1.13.dist-info/WHEEL
 Comment: 
 
-Filename: aigc_zoo-0.1.12.post1.dist-info/top_level.txt
+Filename: aigc_zoo-0.1.13.dist-info/top_level.txt
 Comment: 
 
-Filename: aigc_zoo-0.1.12.post1.dist-info/RECORD
+Filename: aigc_zoo-0.1.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `aigc_zoo-0.1.12.post1.dist-info/LICENSE` & `aigc_zoo-0.1.13.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aigc_zoo-0.1.12.post1.dist-info/RECORD` & `aigc_zoo-0.1.13.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+aigc_zoo/.gitignore,sha256=WMWRJLHvEkjvi4h1Yem_XEBDutffhQXAiaW1vlgFlv8,7
 aigc_zoo/__init__.py,sha256=mmJF0EECVZ_Bj8ul8zq9hou9n4ktDZLo7dUa8vX32g8,80
+aigc_zoo/requirements.txt,sha256=jjyqI-79blp4Xp2VambtFTc7GajPfyXEmUF6ELnx9oI,105
 aigc_zoo/model_zoo/__init__.py,sha256=hab96oKzPI-gzccPWfe8027s99Z7zELBE5D0DVKSTnU,77
 aigc_zoo/model_zoo/baichuan/__init__.py,sha256=2WFhbzYihC48B1ZSY2a42c1l8F8gIxxWh8slLoxGEt0,66
 aigc_zoo/model_zoo/baichuan/llm_model.py,sha256=9vqXeEyvqgjdQmviJnPylFqNtqNR3hyMLnmb1t1VNUI,5578
 aigc_zoo/model_zoo/baichuan/tokenization_baichuan.py,sha256=ZUGfjVTCcNiKfG_JV8TaZsdw7acnUXXxkOpH-wGwht4,9574
 aigc_zoo/model_zoo/baichuan2/__init__.py,sha256=2WFhbzYihC48B1ZSY2a42c1l8F8gIxxWh8slLoxGEt0,66
 aigc_zoo/model_zoo/baichuan2/llm_model.py,sha256=-MYekAWzGJO9FX9e79LJTcisgY-kOA7aSwKNvhjT94o,5575
 aigc_zoo/model_zoo/baichuan2/tokenization_baichuan.py,sha256=15HCHJatue1VgvRZ86HbnaYMgodHt0MHZsi2pIUBYTY,8720
@@ -35,12 +37,12 @@
 aigc_zoo/model_zoo/t5/ppo_model.py,sha256=eXm5sKi4WgISU95r25OCJhrP_ziYy3wRwALn1bf6_24,5848
 aigc_zoo/model_zoo/t5/reward_model.py,sha256=YhWq_Q6zNgQYlyrR3R79NDUkf4BZZiSB8gMzjS2n9kY,9098
 aigc_zoo/utils/__init__.py,sha256=Oc9cllKC2z1rKpYMLkfRj01Jud2WLQaZ_Dd89t4sreY,77
 aigc_zoo/utils/llm_generate.py,sha256=92TvTXISdU7GSrBgMYJoFyicWxkXrm_-02O4jcDnMp0,2664
 aigc_zoo/utils/moss_generate.py,sha256=NYcvqjm3NbutslYlF8_7_BiHNBMPPI0mZzVui4nmkIU,13198
 aigc_zoo/utils/rwkv4_generate.py,sha256=y0HzEYG5Wu9r4NIoFE8rhealv_KJriV8rlhEV-tJpnU,3429
 aigc_zoo/utils/streamgenerator.py,sha256=C1HLeanS0JUokFJIQpY90BKEOlvh8TZvPPCHut-q2EU,748
-aigc_zoo-0.1.12.post1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-aigc_zoo-0.1.12.post1.dist-info/METADATA,sha256=4O_14PqrQ3nR57VkXQ-Rb226xA0yDrSLlwt_rSQFQGw,357
-aigc_zoo-0.1.12.post1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-aigc_zoo-0.1.12.post1.dist-info/top_level.txt,sha256=dl7_T4oT72ShHHM2khyOXJL4Kyvq0u_TdVolu-lKbnY,9
-aigc_zoo-0.1.12.post1.dist-info/RECORD,,
+aigc_zoo-0.1.13.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+aigc_zoo-0.1.13.dist-info/METADATA,sha256=luprLn-vqsVtC9k5-ZQHPDTfd5QkWOpotxo9PcLkLWE,351
+aigc_zoo-0.1.13.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+aigc_zoo-0.1.13.dist-info/top_level.txt,sha256=dl7_T4oT72ShHHM2khyOXJL4Kyvq0u_TdVolu-lKbnY,9
+aigc_zoo-0.1.13.dist-info/RECORD,,
```

