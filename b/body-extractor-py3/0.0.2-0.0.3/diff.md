# Comparing `tmp/body-extractor-py3-0.0.2.tar.gz` & `tmp/body-extractor-py3-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "body-extractor-py3-0.0.2.tar", last modified: Mon Jul 31 02:38:18 2023, max compression
+gzip compressed data, was "body-extractor-py3-0.0.3.tar", last modified: Mon Jul 31 09:24:31 2023, max compression
```

## Comparing `body-extractor-py3-0.0.2.tar` & `body-extractor-py3-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yubin      (501) staff       (20)        0 2023-07-31 02:38:18.799154 body-extractor-py3-0.0.2/
--rw-r--r--   0 yubin      (501) staff       (20)      247 2023-07-31 02:38:18.799056 body-extractor-py3-0.0.2/PKG-INFO
-drwxr-xr-x   0 yubin      (501) staff       (20)        0 2023-07-31 02:38:18.798226 body-extractor-py3-0.0.2/body_extractor/
--rw-r--r--   0 yubin      (501) staff       (20)       74 2023-07-28 03:39:30.000000 body-extractor-py3-0.0.2/body_extractor/__init__.py
--rw-r--r--   0 yubin      (501) staff       (20)     5097 2023-07-31 02:34:53.000000 body-extractor-py3-0.0.2/body_extractor/extractor.py
-drwxr-xr-x   0 yubin      (501) staff       (20)        0 2023-07-31 02:38:18.798910 body-extractor-py3-0.0.2/body_extractor_py3.egg-info/
--rw-r--r--   0 yubin      (501) staff       (20)      247 2023-07-31 02:38:18.000000 body-extractor-py3-0.0.2/body_extractor_py3.egg-info/PKG-INFO
--rw-r--r--   0 yubin      (501) staff       (20)      272 2023-07-31 02:38:18.000000 body-extractor-py3-0.0.2/body_extractor_py3.egg-info/SOURCES.txt
--rw-r--r--   0 yubin      (501) staff       (20)        1 2023-07-31 02:38:18.000000 body-extractor-py3-0.0.2/body_extractor_py3.egg-info/dependency_links.txt
--rw-r--r--   0 yubin      (501) staff       (20)       51 2023-07-31 02:38:18.000000 body-extractor-py3-0.0.2/body_extractor_py3.egg-info/requires.txt
--rw-r--r--   0 yubin      (501) staff       (20)       15 2023-07-31 02:38:18.000000 body-extractor-py3-0.0.2/body_extractor_py3.egg-info/top_level.txt
--rw-r--r--   0 yubin      (501) staff       (20)       38 2023-07-31 02:38:18.799186 body-extractor-py3-0.0.2/setup.cfg
--rw-r--r--   0 yubin      (501) staff       (20)      459 2023-07-31 02:37:47.000000 body-extractor-py3-0.0.2/setup.py
+drwxr-xr-x   0 yubin      (501) staff       (20)        0 2023-07-31 09:24:31.362872 body-extractor-py3-0.0.3/
+-rw-r--r--   0 yubin      (501) staff       (20)      247 2023-07-31 09:24:31.362768 body-extractor-py3-0.0.3/PKG-INFO
+drwxr-xr-x   0 yubin      (501) staff       (20)        0 2023-07-31 09:24:31.362011 body-extractor-py3-0.0.3/body_extractor/
+-rw-r--r--   0 yubin      (501) staff       (20)       74 2023-07-28 03:39:30.000000 body-extractor-py3-0.0.3/body_extractor/__init__.py
+-rw-r--r--   0 yubin      (501) staff       (20)     5305 2023-07-31 09:22:43.000000 body-extractor-py3-0.0.3/body_extractor/extractor.py
+drwxr-xr-x   0 yubin      (501) staff       (20)        0 2023-07-31 09:24:31.362628 body-extractor-py3-0.0.3/body_extractor_py3.egg-info/
+-rw-r--r--   0 yubin      (501) staff       (20)      247 2023-07-31 09:24:31.000000 body-extractor-py3-0.0.3/body_extractor_py3.egg-info/PKG-INFO
+-rw-r--r--   0 yubin      (501) staff       (20)      272 2023-07-31 09:24:31.000000 body-extractor-py3-0.0.3/body_extractor_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 yubin      (501) staff       (20)        1 2023-07-31 09:24:31.000000 body-extractor-py3-0.0.3/body_extractor_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 yubin      (501) staff       (20)       51 2023-07-31 09:24:31.000000 body-extractor-py3-0.0.3/body_extractor_py3.egg-info/requires.txt
+-rw-r--r--   0 yubin      (501) staff       (20)       15 2023-07-31 09:24:31.000000 body-extractor-py3-0.0.3/body_extractor_py3.egg-info/top_level.txt
+-rw-r--r--   0 yubin      (501) staff       (20)       38 2023-07-31 09:24:31.362909 body-extractor-py3-0.0.3/setup.cfg
+-rw-r--r--   0 yubin      (501) staff       (20)      459 2023-07-31 09:24:11.000000 body-extractor-py3-0.0.3/setup.py
```

### Comparing `body-extractor-py3-0.0.2/body_extractor/extractor.py` & `body-extractor-py3-0.0.3/body_extractor/extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 class BodyExtractor():
     def __init__(self, html, lang='CN', encoding='utf-8'):
         if type(html) == bytes:
             self.html = html.decode(encoding)
         else:
             self.html = html
-        if lang == 'CN':
-            self.splitter = ''
-        else:
-            self.splitter = ' '
+        # if lang == 'CN':
+        #     self.splitter = ''
+        # else:
+        self.splitter = ' '
         self.pureText = ''  # 去除标签后的
         self.THRESHOLD = 50  # 骤升点阈值
         self.K = 3  # 行块中行数
         self.wordCount = []  # 每个行块中的字符个数
         self.lines = []
         self.content = ''  # 抽取的正文
         self.title = ''
@@ -59,17 +59,23 @@
         # print(self.pureText)
 
         self.lines = list(map(lambda s: re.sub(r'\s+', self.splitter, s), self.pureText.splitlines()))
         if lang == 'CN':
             count = list(map(lambda s: len(s), self.lines))
         else:
             count = list(map(lambda s: len(s.split()), self.lines))
-        for i in range(len(count) - self.K + 1):
-            self.wordCount.append(count[i] + count[i + 1] + count[i + 2])
-        self.maxIndex = self.wordCount.index(max(self.wordCount))
+
+        if len(count) <= self.K - 1:
+            self.wordCount = [sum(count)]
+            self.maxIndex = 0
+        else:
+            for i in range(len(count) - self.K + 1):
+                self.wordCount.append(count[i] + count[i + 1] + count[i + 2])
+
+            self.maxIndex = self.wordCount.index(max(self.wordCount))
 
     def html_escape(self, text):
         """
         html转义
         """
         text = (text.replace("&quot;", "\"").replace("&ldquo;", "“").replace("&rdquo;", "”")
                 .replace("&middot;", "·").replace("&#8217;", "’").replace("&#8220;", "“")
@@ -79,14 +85,15 @@
                 .replace("&lt;", "<").replace("&#60;", "<").replace("&gt;", ">")
                 .replace("&#62;", ">").replace("&nbsp;", " ").replace("&#160;", " ")
                 .replace("&tilde;", "~").replace("&mdash;", "—").replace("&copy;", "@")
                 .replace("&#169;", "@").replace("♂", "").replace("\r\n|\r", "\n"))
         return text
 
     def _start(self):
+        i = -1
         for i in [-x - 1 + self.maxIndex for x in range(self.maxIndex)]:
             gap = min(self.maxIndex - i, self.K)
             if sum(self.wordCount[i + 1:i + 1 + gap]) > 0:
                 if self.wordCount[i] > self.THRESHOLD:
                     continue
                 else:
                     break
@@ -115,11 +122,12 @@
     # url = 'https://executivegov.com/articles/pfizer-inc-leaders-founders-and-executives-who-are-they/'
     url = 'https://www.pfizer.com/about/people/executives'
 
     res = requests.get(url)
     # if res.encoding != 'ISO-8859-1' or res.encoding != 'utf-8':
     #     extractor = BodyExtractor(res.content, encoding=res.encoding)
     # else:
-    extractor = BodyExtractor(res.content, lang='EN')
+    # extractor = BodyExtractor(res.content, lang='EN')
+    extractor = BodyExtractor('This is', lang='EN')
     print(extractor.content)
     # print(extractor.lines)
     print(extractor.title)
```

