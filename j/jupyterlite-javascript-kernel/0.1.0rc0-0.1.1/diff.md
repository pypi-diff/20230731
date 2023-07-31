# Comparing `tmp/jupyterlite_javascript_kernel-0.1.0rc0.tar.gz` & `tmp/jupyterlite_javascript_kernel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr  1 06:43:15 2023, max compression
+gzip compressed data, last modified: Mon Jul 31 13:00:28 2023, max compression
```

## Comparing `jupyterlite_javascript_kernel-0.1.0rc0.tar` & `jupyterlite_javascript_kernel-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2466 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/package.json
--rw-r--r--   0        0        0      321 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/tsconfig.json
--rw-r--r--   0        0        0      124 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/__init__.py
--rw-r--r--   0        0        0     2582 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/package.json
--rw-r--r--   0        0        0     8738 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/102.c877ef340ee478be48c0.js
--rw-r--r--   0        0        0     6180 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/290.d733d9b78aec5de9e149.js
--rw-r--r--   0        0        0     6180 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/322.f988973acf64db62bd18.js
--rw-r--r--   0        0        0    27007 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/441.4368412449ba90ea9225.js
--rw-r--r--   0        0        0      621 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/568.9697b09d8959ad97cb94.js
--rw-r--r--   0        0        0     4825 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/866.1ce3c77b50c9eb671961.js
--rw-r--r--   0        0        0     8405 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/remoteEntry.aefc79022a1753a263bf.js
--rw-r--r--   0        0        0      118 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/style.js
--rw-r--r--   0        0        0    15907 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1239 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/src/index.ts
--rw-r--r--   0        0        0     2104 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/.gitignore
--rw-r--r--   0        0        0     1532 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0      667 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/README.md
--rw-r--r--   0        0        0     1493 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     3278 2023-04-01 06:43:15.000000 jupyterlite_javascript_kernel-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     2446 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/package.json
+-rw-r--r--   0        0        0      321 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0      124 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/__init__.py
+-rw-r--r--   0        0        0     2562 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/package.json
+-rw-r--r--   0        0        0     8738 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/102.c877ef340ee478be48c0.js
+-rw-r--r--   0        0        0     6180 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/290.29fb1677e9ddfbef42ef.js
+-rw-r--r--   0        0        0     6180 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/322.5488d7441d23f13faba2.js
+-rw-r--r--   0        0        0    27007 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/441.4368412449ba90ea9225.js
+-rw-r--r--   0        0        0      621 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/568.b0a688b88d43b80c014d.js
+-rw-r--r--   0        0        0     4825 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/866.1ce3c77b50c9eb671961.js
+-rw-r--r--   0        0        0     8373 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/remoteEntry.9eaa8a846d81f5b6c8be.js
+-rw-r--r--   0        0        0      118 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/style.js
+-rw-r--r--   0        0        0    15897 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1239 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/src/index.ts
+-rw-r--r--   0        0        0     2104 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1532 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/LICENSE
+-rw-r--r--   0        0        0      667 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/README.md
+-rw-r--r--   0        0        0     1490 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3275 2023-07-31 13:00:28.000000 jupyterlite_javascript_kernel-0.1.1/PKG-INFO
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/package.json` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9525462962962963%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/javascript-kernel': '^0.1.1', '@jupyterlite/kernel': '^0.1.1', "*

 * *                   "'@jupyterlite/server': '^0.1.1'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.9eaa8a846d81f5b6c8be.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterLite Contributors",
     "bugs": {
         "url": "https://github.com/jupyterlite/jupyterlite/issues"
     },
     "dependencies": {
         "@jupyterlab/coreutils": "~5.5.3",
-        "@jupyterlite/javascript-kernel": "^0.1.0-rc.0",
-        "@jupyterlite/kernel": "^0.1.0-rc.0",
-        "@jupyterlite/server": "^0.1.0-rc.0"
+        "@jupyterlite/javascript-kernel": "^0.1.1",
+        "@jupyterlite/kernel": "^0.1.1",
+        "@jupyterlite/server": "^0.1.1"
     },
     "description": "JupyterLite - JavaScript Kernel Extension",
     "devDependencies": {
         "@babel/core": "^7.11.6",
         "@babel/preset-env": "^7.12.1",
         "@jupyterlab/builder": "^3.1.0",
         "@types/jest": "^26.0.10",
@@ -26,14 +26,18 @@
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
         "lib/*.js"
     ],
     "homepage": "https://github.com/jupyterlite/jupyterlite",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.9eaa8a846d81f5b6c8be.js"
+        },
         "extension": true,
         "outputDir": "jupyterlite_javascript_kernel/labextension"
     },
     "jupyterlite": {
         "liteExtension": true
     },
     "license": "BSD-3-Clause",
@@ -66,9 +70,9 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "yarn prettier:base --check",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0-rc.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/package.json` & `jupyterlite_javascript_kernel-0.1.1/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9525462962962963%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/javascript-kernel': '^0.1.1', '@jupyterlite/kernel': '^0.1.1', "*

 * *                   "'@jupyterlite/server': '^0.1.1'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterLite Contributors",
     "bugs": {
         "url": "https://github.com/jupyterlite/jupyterlite/issues"
     },
     "dependencies": {
         "@jupyterlab/coreutils": "~5.5.3",
-        "@jupyterlite/javascript-kernel": "^0.1.0-rc.0",
-        "@jupyterlite/kernel": "^0.1.0-rc.0",
-        "@jupyterlite/server": "^0.1.0-rc.0"
+        "@jupyterlite/javascript-kernel": "^0.1.1",
+        "@jupyterlite/kernel": "^0.1.1",
+        "@jupyterlite/server": "^0.1.1"
     },
     "description": "JupyterLite - JavaScript Kernel Extension",
     "devDependencies": {
         "@babel/core": "^7.11.6",
         "@babel/preset-env": "^7.12.1",
         "@jupyterlab/builder": "^3.1.0",
         "@types/jest": "^26.0.10",
@@ -26,18 +26,14 @@
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
         "lib/*.js"
     ],
     "homepage": "https://github.com/jupyterlite/jupyterlite",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.aefc79022a1753a263bf.js"
-        },
         "extension": true,
         "outputDir": "jupyterlite_javascript_kernel/labextension"
     },
     "jupyterlite": {
         "liteExtension": true
     },
     "license": "BSD-3-Clause",
@@ -70,9 +66,9 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "yarn prettier:base --check",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0-rc.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/102.c877ef340ee478be48c0.js` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/102.c877ef340ee478be48c0.js`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/290.d733d9b78aec5de9e149.js` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/290.29fb1677e9ddfbef42ef.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
     [290, 322], {
         290: (e, t, r) => {
             r.r(t), r.d(t, {
                 JavaScriptKernel: () => E
             });
             var n = r(671),
-                a = r(180),
+                a = r(826),
                 s = r(526);
             const o = Symbol("Comlink.proxy"),
                 i = Symbol("Comlink.endpoint"),
                 c = Symbol("Comlink.releaseProxy"),
                 u = Symbol("Comlink.thrown"),
                 l = e => "object" == typeof e && null !== e || "function" == typeof e,
                 p = new Map([
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/322.f988973acf64db62bd18.js` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/322.5488d7441d23f13faba2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
     [322, 290], {
         290: (e, t, r) => {
             r.r(t), r.d(t, {
                 JavaScriptKernel: () => E
             });
             var n = r(671),
-                a = r(180),
+                a = r(826),
                 s = r(526);
             const o = Symbol("Comlink.proxy"),
                 i = Symbol("Comlink.endpoint"),
                 c = Symbol("Comlink.releaseProxy"),
                 u = Symbol("Comlink.thrown"),
                 l = e => "object" == typeof e && null !== e || "function" == typeof e,
                 p = new Map([
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/441.4368412449ba90ea9225.js` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/441.4368412449ba90ea9225.js`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/568.9697b09d8959ad97cb94.js` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/568.b0a688b88d43b80c014d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,16 @@
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
     [568], {
         568: (e, a, r) => {
             r.r(a), r.d(a, {
                 default: () => i
             });
             var t = r(671),
-                s = r(180),
-                n = r(203);
+                s = r(826),
+                n = r(765);
             const i = [{
                 id: "@jupyterlite/javascript-kernel-extension:kernel",
                 autoStart: !0,
                 requires: [s.IKernelSpecs],
                 activate: (e, a) => {
                     const r = t.PageConfig.getBaseUrl();
                     a.register({
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/866.1ce3c77b50c9eb671961.js` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/866.1ce3c77b50c9eb671961.js`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/remoteEntry.aefc79022a1753a263bf.js` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/remoteEntry.9eaa8a846d81f5b6c8be.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, a, o, i, l, u, s, f, d, c, p, h, v, b, m, y, g, j, w, k = {
             986: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(671), t.e(180), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(671), t.e(180), t.e(568)]).then((() => () => t(568)))
+                        "./index": () => Promise.all([t.e(671), t.e(826), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(671), t.e(826), t.e(568)]).then((() => () => t(568)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -42,31 +42,31 @@
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         102: "c877ef340ee478be48c0",
-        180: "63f7b1f1a77622697166",
-        290: "d733d9b78aec5de9e149",
-        322: "f988973acf64db62bd18",
+        290: "29fb1677e9ddfbef42ef",
+        322: "5488d7441d23f13faba2",
         441: "4368412449ba90ea9225",
         526: "d5312df4c55fd57dbce5",
-        568: "9697b09d8959ad97cb94",
+        568: "b0a688b88d43b80c014d",
         671: "11d0402aaed2182a5985",
+        826: "e39ede89416bd1f1fe66",
         866: "1ce3c77b50c9eb671961"
     } [e] + ".js?v=" + {
         102: "c877ef340ee478be48c0",
-        180: "63f7b1f1a77622697166",
-        290: "d733d9b78aec5de9e149",
-        322: "f988973acf64db62bd18",
+        290: "29fb1677e9ddfbef42ef",
+        322: "5488d7441d23f13faba2",
         441: "4368412449ba90ea9225",
         526: "d5312df4c55fd57dbce5",
-        568: "9697b09d8959ad97cb94",
+        568: "b0a688b88d43b80c014d",
         671: "11d0402aaed2182a5985",
+        826: "e39ede89416bd1f1fe66",
         866: "1ce3c77b50c9eb671961"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -119,15 +119,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlite/javascript-kernel-extension", "0.1.0-rc.0", (() => Promise.all([S.e(671), S.e(180), S.e(568)]).then((() => () => S(568))))), l("@jupyterlite/javascript-kernel", "0.1.0-rc.0", (() => Promise.all([S.e(526), S.e(671), S.e(180), S.e(290)]).then((() => () => S(290))))), l("@jupyterlite/kernel", "0.1.0-rc.0", (() => Promise.all([S.e(441), S.e(526), S.e(671), S.e(102)]).then((() => () => S(102)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlite/javascript-kernel-extension", "0.1.1", (() => Promise.all([S.e(671), S.e(826), S.e(568)]).then((() => () => S(568))))), l("@jupyterlite/javascript-kernel", "0.1.1", (() => Promise.all([S.e(526), S.e(671), S.e(826), S.e(290)]).then((() => () => S(290))))), l("@jupyterlite/kernel", "0.1.1", (() => Promise.all([S.e(441), S.e(526), S.e(671), S.e(102)]).then((() => () => S(102)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -233,26 +233,26 @@
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, a)) : e(r, S.S[r], t, n, a)
     })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || l(r, t))))), m = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), y = v(((e, r, t, n, a) => {
         var o = r && S.o(r, t) && d(r, t, n);
         return o ? h(o) : a()
     })), g = {}, j = {
         671: () => m("default", "@jupyterlab/coreutils", [1, 5, 5, 3]),
-        180: () => y("default", "@jupyterlite/kernel", [2, 0, 1, 0, , "rc", 0], (() => Promise.all([S.e(441), S.e(526), S.e(102)]).then((() => () => S(102))))),
-        203: () => y("default", "@jupyterlite/javascript-kernel", [2, 0, 1, 0, , "rc", 0], (() => Promise.all([S.e(526), S.e(322)]).then((() => () => S(290))))),
+        826: () => y("default", "@jupyterlite/kernel", [2, 0, 1, 1], (() => Promise.all([S.e(441), S.e(526), S.e(102)]).then((() => () => S(102))))),
+        765: () => y("default", "@jupyterlite/javascript-kernel", [2, 0, 1, 1], (() => Promise.all([S.e(526), S.e(322)]).then((() => () => S(290))))),
         526: () => m("default", "@lumino/coreutils", [1, 1, 11, 0]),
         840: () => m("default", "@lumino/signaling", [1, 1, 10, 0]),
         878: () => m("default", "@jupyterlab/services", [1, 6, 5, 3]),
         911: () => b("default", "@jupyterlab/observables", [1, 4, 5, 3])
     }, w = {
         102: [840, 878, 911],
-        180: [180],
         526: [526],
-        568: [203],
-        671: [671]
+        568: [765],
+        671: [671],
+        826: [826]
     }, S.f.consumes = (e, r) => {
         S.o(w, e) && w[e].forEach((e => {
             if (S.o(g, e)) return r.push(g[e]);
             var t = r => {
                     g[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -274,15 +274,15 @@
         var e = {
             406: 0
         };
         S.f.j = (r, t) => {
             var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(180|526|671)$/.test(r)) e[r] = 0;
+                else if (/^([58]26|671)$/.test(r)) e[r] = 0;
             else {
                 var a = new Promise(((t, a) => n = e[r] = [t, a]));
                 t.push(n[2] = a);
                 var o = S.p + S.u(r),
                     i = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json` & `jupyterlite_javascript_kernel-0.1.1/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428572%*

 * *Differences: {"'packages'": "{1: {'versionInfo': '0.1.1'}, 2: {'versionInfo': '0.1.1'}}"}*

```diff
@@ -6,21 +6,21 @@
             "name": "@jupyterlab/services",
             "versionInfo": "6.5.3"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/javascript-kernel",
-            "versionInfo": "0.1.0-rc.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/kernel",
-            "versionInfo": "0.1.0-rc.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2016 Christian Speckner <cnspeckn@googlemail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "async-mutex",
             "versionInfo": "0.3.2"
         },
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/src/index.ts` & `jupyterlite_javascript_kernel-0.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/.gitignore` & `jupyterlite_javascript_kernel-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/LICENSE` & `jupyterlite_javascript_kernel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/README.md` & `jupyterlite_javascript_kernel-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/pyproject.toml` & `jupyterlite_javascript_kernel-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling>=1.6.3,<2", "jupyterlab>=3.5.3,<3.6.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlite-javascript-kernel"
 readme = "README.md"
-version = "0.1.0rc0"
+version = "0.1.1"
 description = "JavaScript kernel for JupyterLite running in a Web Worker"
 authors = [
     { name = "JupyterLite Contributors" },
 ]
 keywords = [
     "jupyterlite",
     "jupyter",
```

### Comparing `jupyterlite_javascript_kernel-0.1.0rc0/PKG-INFO` & `jupyterlite_javascript_kernel-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlite-javascript-kernel
-Version: 0.1.0rc0
+Version: 0.1.1
 Summary: JavaScript kernel for JupyterLite running in a Web Worker
 Project-URL: Source, https://github.com/jupyterlite/jupyterlite
 Project-URL: PyPI, https://pypi.org/project/jupyterlite-javascript-kernel
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, JupyterLite Contributors
```

