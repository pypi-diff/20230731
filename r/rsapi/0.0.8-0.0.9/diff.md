# Comparing `tmp/rsapi-0.0.8.tar.gz` & `tmp/rsapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rsapi-0.0.8.tar", last modified: Sat Aug  1 21:37:17 2020, max compression
+gzip compressed data, was "dist/rsapi-0.0.9.tar", last modified: Sun Aug  2 11:55:14 2020, max compression
```

## Comparing `rsapi-0.0.8.tar` & `rsapi-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-01 21:37:17.589908 rsapi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      329 2020-08-01 21:37:17.589908 rsapi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      222 2020-08-01 21:37:09.000000 rsapi-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-01 21:37:17.589908 rsapi-0.0.8/rsapi/
--rw-r--r--   0 runner    (1001) docker     (116)     1164 2020-08-01 21:37:09.000000 rsapi-0.0.8/rsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10050 2020-08-01 21:37:09.000000 rsapi-0.0.8/rsapi/osrs.py
--rw-r--r--   0 runner    (1001) docker     (116)     1334 2020-08-01 21:37:09.000000 rsapi-0.0.8/rsapi/test_osrs.py
--rw-r--r--   0 runner    (1001) docker     (116)     3302 2020-08-01 21:37:09.000000 rsapi-0.0.8/rsapi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-01 21:37:17.589908 rsapi-0.0.8/rsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      329 2020-08-01 21:37:17.000000 rsapi-0.0.8/rsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      227 2020-08-01 21:37:17.000000 rsapi-0.0.8/rsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-01 21:37:17.000000 rsapi-0.0.8/rsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       78 2020-08-01 21:37:17.000000 rsapi-0.0.8/rsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-08-01 21:37:17.000000 rsapi-0.0.8/rsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-01 21:37:17.589908 rsapi-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      489 2020-08-01 21:37:09.000000 rsapi-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-02 11:55:14.473523 rsapi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      329 2020-08-02 11:55:14.473523 rsapi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      222 2020-08-02 11:55:06.000000 rsapi-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-02 11:55:14.473523 rsapi-0.0.9/rsapi/
+-rw-r--r--   0 runner    (1001) docker     (116)     1164 2020-08-02 11:55:06.000000 rsapi-0.0.9/rsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12439 2020-08-02 11:55:06.000000 rsapi-0.0.9/rsapi/osrs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1334 2020-08-02 11:55:06.000000 rsapi-0.0.9/rsapi/test_osrs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3302 2020-08-02 11:55:06.000000 rsapi-0.0.9/rsapi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-02 11:55:14.473523 rsapi-0.0.9/rsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      329 2020-08-02 11:55:14.000000 rsapi-0.0.9/rsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      227 2020-08-02 11:55:14.000000 rsapi-0.0.9/rsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-02 11:55:14.000000 rsapi-0.0.9/rsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       94 2020-08-02 11:55:14.000000 rsapi-0.0.9/rsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-08-02 11:55:14.000000 rsapi-0.0.9/rsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-02 11:55:14.473523 rsapi-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      489 2020-08-02 11:55:06.000000 rsapi-0.0.9/setup.py
```

### Comparing `rsapi-0.0.8/rsapi/__init__.py` & `rsapi-0.0.9/rsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rsapi-0.0.8/rsapi/osrs.py` & `rsapi-0.0.9/rsapi/osrs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+import re
+import typing
+
+from osrsbox import items_api
+from osrsbox.items_api.item_properties import ItemProperties
+
 import rsapi.util
 
 
+ITEMS = items_api.load()
 SKILLS = [
     ("Overall",                 "Overall", "data:image/gif;base64,R0lGODlhEAAQAIcAAAAAAP///wgICNEYGnYPEXYQEZcVGHsSE8dUVaYXG4QTGIQTF3YRFWoPElQMD00LDYoUGIMTF3oSFn8TF3IRFGMPElAMD08MDm8RFFsOEZopLGpAQcR3eqGFhksLDkQKDTcIC0gLDkAKDUQLDlQOEpQkKsBJT/zr7NEaKKUYJSsHCogdJbU6RFE1OHwWIndoauhMYtElQ+QxUNOPn8IhS6mdoYd+grujrm9iaV1YW8m0yZSPlMjEzHVyeREXQUZSpi4/nzA/kzE1TBojTygtRCQsP0JHURgfKz5KXSsxO4CMnR8oNCgyQCo0QUlWaCs2RDRBUSw3RD5MXUBOX0dWaUlYa11rfbzP5nJ7hiY0RB8qNh8oMi05RzdFVTZEU0dYazE9Skpbbk1ecVxvhTtHVVRleG2DmyY2RyQyQD5OX0NUZU5hdHWFlhgjLS9CUyUxPDlJWD5OXWuCmIuapr7W50VTXL7a677Y6b3X6LvV5r3Y6HaDikJMUGyDi6S5wWmFii03OF1pY3SDe32Ngz1FQHKAd0FKREdQSnuKgISXiY6ikqKtpG+EchpZISJnKzN5PHCpdw9JFBtcIiJjKCpvMS1yM0aPTUSHS16hZQo9DhVSGj2FQ1pxW3mPeqi6qWl1aMPFvv/3cf/eIf/nWP/oaP/XBP/aKP/dO//pef/pif/aTvm4Av/IJd+2RP/VV//FOee1O/+1CP+2GP+8J9moOP/JTP/LXP/QY//WfbqTQcabRuCxVf/NZf/+/P+hAP+oFP/Nfv/Ujf+2SPSOBt6BC9d/FP+nN//Dd//FfM9vAJNNAP+pR7pkE/+LIP+2df+gVaFDAMlPAKM+AOhlFc5dFZNSKdpTD9dZFfV7PB0QCsNMGRgHAXgqDNFbL29OQkgUBOBQHug2AM82DSsSC7tWOKNONVgUAzkVDGMVBO5QLNg+IJ0sF2wOAKU9M+ZjV7JDPN3JyKc3M7BYVFAMDJ4nJ6ErKqEuLsNFRM5eXsi0tO7a2pyUlJaOjv/+/gEBAf///yH5BAMAAP8ALAAAAAAQABAAAAitAP8JHEiwoEGBAhImPDhQACRIni4JYPhPgKeLlyRSFIAJU0SNBRUKsGRJUaVKEwkKuHcP38iSlRylRIivZj0BmzYlciRT5bt3COjh1OlI0syKP4MKePSokySjKuPFM1FiaVNJmkRWlEpVACVKjDRlBQLkR0J79kys8Ao264+3Q86mXTtp0qdIAoQI+RFXgAYNLNY2asQpkwAiRIL0LVGChQt/gwsLKFIkiA8BAQEAOw=="),
     ("Attack",                  "Att",     "data:image/gif;base64,R0lGODlhEAAQALMAAEY8L7u5A3huYVpQQ1BGOWRaTYJ4a3d7CXd3dwAAAP///wAAAAAAAAAAAAAAAAAAACH5BAEAAAoALAAAAAAQABAAAAQ+UMlJZbqp6otQ1hPXfaDokZV5gQpnnCwnwGWCFPRmD3mIIYRe6HAIHIS+YmAVAwCIqFTCmThEKYkl5urjaiIAOw=="),
     ("Defence",                 "Def",     "data:image/gif;base64,R0lGODlhEAAQAKIAAFtbVZCQkHd3dwAAAP///wAAAAAAAAAAACH5BAEAAAQALAAAAAAQABAAAANBSLrcOzBKyAa4IovAR8Xa1n1ABomB94Anl5LmgKqKNUXvekN5zcouGsFSErRGq+KxN7TERJSKU5MSPqZVx1XSSAAAOw=="),
     ("Strength",                "Str",     "data:image/gif;base64,R0lGODlhDQAQAKIFAEY8L9CyhAAAAQAAAKGSev///wAAAAAAACH5BAEAAAUALAAAAAANABAAAANEWFois1C10BwcjRAQgJXBBnCchYXaSDoCqqUb1YovEE+baNvOGbgjgkDhe2kai5breFEahxCnhhKR/qDJn5Z6GXi/0AQAOw=="),
     ("Hitpoints",               "HP",      "data:image/gif;base64,R0lGODlhEAAQAKIFAHo9CbM5AwAAAQAAAN1PAf///wAAAAAAACH5BAEAAAUALAAAAAAQABAAAANEWCUso6MJtQa5joUAxmNX6BEb0IFhepWn6nKtm8KRPJu1TdKazDILQeDFASo0m5XJSEFuihNKU2BaRqVTK3Yr2Xo93gQAOw=="),
     ("Ranged",                  "Range",   "data:image/gif;base64,R0lGODlhEgASAKIGAAlsAjUvG3V7fHo9CQAAAQAAAP///wAAACH5BAEAAAYALAAAAAASABIAAANoaLrcW6QYSGp0hoyoh9+SpXTd53GbUkDCFkGnUDGFIKyqF1x0LUuQwEnSs60Kuw/v4SMEjh1io7YjFjzSyTFgBGIfBADg2YQNpAVxAHA0RheVNVtrGzIqAN7KtoTjmBp9GA9fg1NHBgkAOw=="),
@@ -80,17 +87,98 @@
     "Vorkath",
     "Wintertodt",
     "Zalcano",
     "Zulrah",
 ]
 HISCORES_PATH = "m=hiscore_oldschool/index_lite.ws"
 NEWS_PATH = "m=news/latest_news.rss"
+GE_PATH = "m=itemdb_oldschool/api/catalogue/detail.json"
+
 
+class ItemNotFound(Exception):
+    def __init__(self, msg, query):
+        self.msg = msg
+        self.query = query
 
-def hiscores(player):
+
+def hiscores(player: str) -> dict:
     with rsapi.util.request(HISCORES_PATH, player=player) as resp:
         return rsapi.util.parse_scores(resp.text, SKILLS)
 
 
-def news():
+def news() -> dict:
     with rsapi.util.request(NEWS_PATH, oldschool=True) as resp:
         return rsapi.util.parse_news(resp.text)
+
+
+def items(item_q: typing.Union[int, str],
+          maxitems: int = 10) -> typing.List[ItemProperties]:
+    ret = []
+
+    if isinstance(item_q, int):
+        ret = [i for i in ITEMS if i.id == item_q]
+    elif isinstance(item_q, str):
+        r = re.compile(item_q, re.IGNORECASE)
+        ret = [
+            i for i in ITEMS if r.search(i.name) and \
+                                i.linked_id_item is None and \
+                                not i.duplicate
+        ]
+        # Maybe there is an exact match
+        exact = [i for i in ret if i.name.lower() == item_q.lower()]
+        if exact:
+            ret = exact
+    else:
+        raise Exception("Bad argument type")
+
+    if not ret:
+        raise ItemNotFound(f"No items found", item_q)
+
+    return ret[:maxitems]
+
+
+def alch(item_q: typing.Union[int, str], maxitems: int = 10) -> dict:
+    return {
+        i.id: {
+            "name": i.name,
+            "highalch": i.highalch,
+            "lowalch": i.lowalch,
+        } for i in items(item_q, maxitems=maxitems)
+    }
+
+
+def _ge_parse(data):
+    item = data["item"]
+    return {
+        "current": item["current"],
+        "today": item["today"],
+        "day30": item["day30"],
+        "day90": item["day90"],
+        "day180": item["day180"],
+    }
+
+
+def _ge_get(id_):
+    with rsapi.util.request(GE_PATH, item=id_) as resp:
+        return _ge_parse(resp.json())
+
+
+def ge(item_q: typing.Union[int, str], maxitems: int = 10) -> dict:
+    return {i.id: _ge_get(i.id) for i in items(item_q, maxitems=maxitems)}
+
+
+def price(item_q: typing.Union[int, str], maxitems=10) -> dict:
+    ret = {}
+    for item in items(item_q, maxitems=maxitems):
+        entry = {
+            "name": item.name,
+            "tradeable": item.tradeable,
+            "tradeable_on_ge": item.tradeable_on_ge,
+            "alch": {
+                "highalch": item.highalch,
+                "lowalch": item.lowalch,
+            },
+        }
+        if item.tradeable_on_ge:
+            entry["ge"] = _ge_get(item.id)
+        ret[item.id] = entry
+    return ret
```

### Comparing `rsapi-0.0.8/rsapi/test_osrs.py` & `rsapi-0.0.9/rsapi/test_osrs.py`

 * *Files identical despite different names*

### Comparing `rsapi-0.0.8/rsapi/util.py` & `rsapi-0.0.9/rsapi/util.py`

 * *Files identical despite different names*

