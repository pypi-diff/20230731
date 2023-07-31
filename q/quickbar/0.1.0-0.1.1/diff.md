# Comparing `tmp/quickbar-0.1.0.tar.gz` & `tmp/quickbar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbar-0.1.0.tar", max compression
+gzip compressed data, was "quickbar-0.1.1.tar", max compression
```

## Comparing `quickbar-0.1.0.tar` & `quickbar-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-27 18:17:51.248528 quickbar-0.1.0/README.md
--rw-r--r--   0        0        0      475 2023-07-28 00:30:47.999308 quickbar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       26 2023-07-28 00:29:14.936031 quickbar-0.1.0/quickbar/.git/COMMIT_EDITMSG
--rw-r--r--   0        0        0       23 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/HEAD
--rw-r--r--   0        0        0      268 2023-07-28 00:29:25.056953 quickbar-0.1.0/quickbar/.git/config
--rw-r--r--   0        0        0       73 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/description
--rwxr-xr-x   0        0        0      482 2023-07-28 00:27:42.983746 quickbar-0.1.0/quickbar/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      900 2023-07-28 00:27:42.983746 quickbar-0.1.0/quickbar/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2023-07-28 00:27:42.983746 quickbar-0.1.0/quickbar/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      193 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      428 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1647 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      420 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1378 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4902 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      548 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1496 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2787 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     2312 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0        0        0     3654 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/hooks/update.sample
--rw-r--r--   0        0        0      709 2023-07-28 00:29:14.936031 quickbar-0.1.0/quickbar/.git/index
--rw-r--r--   0        0        0      240 2023-07-28 00:27:42.984746 quickbar-0.1.0/quickbar/.git/info/exclude
--rw-r--r--   0        0        0      188 2023-07-28 00:29:14.936031 quickbar-0.1.0/quickbar/.git/logs/HEAD
--rw-r--r--   0        0        0      188 2023-07-28 00:29:14.937031 quickbar-0.1.0/quickbar/.git/logs/refs/heads/master
--rw-r--r--   0        0        0      159 2023-07-28 00:29:25.056953 quickbar-0.1.0/quickbar/.git/logs/refs/remotes/origin/master
--rw-r--r--   0        0        0      144 2023-07-28 00:29:14.936031 quickbar-0.1.0/quickbar/.git/objects/5e/84af76c069e856e654433eaf4a00d6d566bcb2
--rw-r--r--   0        0        0       49 2023-07-28 00:27:45.077730 quickbar-0.1.0/quickbar/.git/objects/89/ffb730f9a508076ba131bfdccbb27174638459
--rw-r--r--   0        0        0      127 2023-07-28 00:29:14.936031 quickbar-0.1.0/quickbar/.git/objects/9e/f1ba3d989a5b7d7a79a12b6497aa6304eb075f
--rw-r--r--   0        0        0      762 2023-07-28 00:27:45.078730 quickbar-0.1.0/quickbar/.git/objects/ad/36fc1152f6debade1936f749579ff09ea7fb35
--rw-r--r--   0        0        0      174 2023-07-28 00:27:45.077730 quickbar-0.1.0/quickbar/.git/objects/b8/5c913348442ec3f91f62079d6e5a576df3e2f2
--rw-r--r--   0        0        0     1235 2023-07-28 00:27:45.078730 quickbar-0.1.0/quickbar/.git/objects/bc/e598075e1253af2d0a0f9fd950843f3d5f652b
--rw-r--r--   0        0        0     1302 2023-07-28 00:27:45.078730 quickbar-0.1.0/quickbar/.git/objects/d1/ff9ba4be424b0f370c9c32fa6c2811af750be2
--rw-r--r--   0        0        0      187 2023-07-28 00:29:14.936031 quickbar-0.1.0/quickbar/.git/objects/e5/abf7201000050917e38d176f74f1f0bcde2eb6
--rw-r--r--   0        0        0      192 2023-07-28 00:27:45.077730 quickbar-0.1.0/quickbar/.git/objects/ea/f291868a89d7bfabca461b9fe7e2186d1d26a4
--rw-r--r--   0        0        0      853 2023-07-28 00:27:45.077730 quickbar-0.1.0/quickbar/.git/objects/fb/b42972d3a0eceba9797456c04f75c45861e54b
--rw-r--r--   0        0        0       41 2023-07-28 00:29:14.936031 quickbar-0.1.0/quickbar/.git/refs/heads/master
--rw-r--r--   0        0        0       41 2023-07-28 00:29:25.056953 quickbar-0.1.0/quickbar/.git/refs/remotes/origin/master
--rw-r--r--   0        0        0      234 2023-07-28 00:27:29.256852 quickbar-0.1.0/quickbar/README.md
--rw-r--r--   0        0        0       41 2023-07-27 18:42:44.521026 quickbar-0.1.0/quickbar/__init__.py
--rw-r--r--   0        0        0     1962 2023-07-28 00:25:31.648766 quickbar-0.1.0/quickbar/__main__.py
--rw-r--r--   0        0        0     2436 2023-07-27 23:56:26.028876 quickbar-0.1.0/quickbar/core.py
--rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 quickbar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-07-28 00:37:36.475223 quickbar-0.1.1/README.md
+-rw-r--r--   0        0        0      564 2023-07-31 02:21:17.669618 quickbar-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-07-28 00:27:29.256852 quickbar-0.1.1/quickbar/README.md
+-rw-r--r--   0        0        0       41 2023-07-27 18:42:44.521026 quickbar-0.1.1/quickbar/__init__.py
+-rw-r--r--   0        0        0     1962 2023-07-28 00:25:31.648766 quickbar-0.1.1/quickbar/__main__.py
+-rw-r--r--   0        0        0     2596 2023-07-31 02:02:48.808892 quickbar-0.1.1/quickbar/core.py
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 quickbar-0.1.1/PKG-INFO
```

### Comparing `quickbar-0.1.0/quickbar/__main__.py` & `quickbar-0.1.1/quickbar/__main__.py`

 * *Files identical despite different names*

### Comparing `quickbar-0.1.0/quickbar/core.py` & `quickbar-0.1.1/quickbar/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,19 +59,22 @@
         
     
     @staticmethod
     def track(iterable: Union[Sequence, Iterable] = ..., message: str = 'Working ..'):
         qbar = Quickbar('spin-bar')
         if hasattr(iterable, '__len__'):
             qbar.total = len(iterable)
-
         
         qbar.message = message or qbar.message
         task_id = qbar.bar.add_task(qbar.message, total=qbar.total)
         def callback():
             qbar.bar.start()
-            for item in iterable:
-                qbar.bar.advance(task_id=task_id)
-                yield item
-            qbar.bar.stop()
-            qbar.bar.remove_task(task_id=task_id)
-        return callback()
+            try:
+                for item in iterable:
+                    qbar.bar.advance(task_id=task_id)
+                    yield item
+                qbar.bar.stop()
+                qbar.bar.remove_task(task_id=task_id)
+            except Exception as err:
+                qbar.bar.stop()
+                qbar.bar.remove_task(task_id=task_id)
+        return callback()
```

