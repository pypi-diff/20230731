# Comparing `tmp/actions_security_analyzer-1.2.3.tar.gz` & `tmp/actions_security_analyzer-1.2.4.tar.gz`

## Comparing `actions_security_analyzer-1.2.3.tar` & `actions_security_analyzer-1.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/__about__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/colors.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/requirements.txt
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/.github/workflows/asa-scan.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-that-creates-or-approves-pr.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/analyzer/__init__.py
--rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/analyzer/analyzer.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/analyzer/analyzer_test.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/images/asa-stdout.png
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/LICENSE
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/README.md
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/__about__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/colors.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/requirements.txt
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/.github/workflows/asa-scan.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-that-creates-or-approves-pr.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/analyzer/__init__.py
+-rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/analyzer/analyzer.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/images/asa-stdout.png
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/LICENSE
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/README.md
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/PKG-INFO
```

### Comparing `actions_security_analyzer-1.2.3/action.yml` & `actions_security_analyzer-1.2.4/action.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/colors.py` & `actions_security_analyzer-1.2.4/colors.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/main.py` & `actions_security_analyzer-1.2.4/main.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `actions_security_analyzer-1.2.4/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/analyzer/analyzer.py` & `actions_security_analyzer-1.2.4/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/analyzer/analyzer_test.py` & `actions_security_analyzer-1.2.4/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/images/asa-stdout.png` & `actions_security_analyzer-1.2.4/images/asa-stdout.png`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/.gitignore` & `actions_security_analyzer-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/LICENSE` & `actions_security_analyzer-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/README.md` & `actions_security_analyzer-1.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![asa-stdout](/images/asa-stdout.png)
 
 ### Installation
 
 > Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
-pip3 install actions-security-analzyer
+pip install actions-security-analzyer
 ```
 
 ### Usage
 
 ```
 asa --file action.yml
 asa -d directory-with-actions/ --verbose
@@ -27,14 +27,16 @@
 ```yaml
 name: 'RunActionsSecurityAnalzyer'
 on:
   push:
     branches:
       - main
       - dev
+    paths:
+      - '.github/workflows/**'
 jobs:
   RunAsa:
     runs-on: ubuntu-latest
     steps:
     - name: "Checkout repo"
       uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
     - name: "Run asa scanner"
```

### Comparing `actions_security_analyzer-1.2.3/pyproject.toml` & `actions_security_analyzer-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.3/PKG-INFO` & `actions_security_analyzer-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actions-security-analyzer
-Version: 1.2.3
+Version: 1.2.4
 Summary: Analyze the security posture of one or more GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/asa#readme
 Project-URL: Issues, https://github.com/bin3xish477/asa/issues
 Project-URL: Source, https://github.com/bin3xish477/asa
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -31,15 +31,15 @@
 ![asa-stdout](/images/asa-stdout.png)
 
 ### Installation
 
 > Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
-pip3 install actions-security-analzyer
+pip install actions-security-analzyer
 ```
 
 ### Usage
 
 ```
 asa --file action.yml
 asa -d directory-with-actions/ --verbose
@@ -54,14 +54,16 @@
 ```yaml
 name: 'RunActionsSecurityAnalzyer'
 on:
   push:
     branches:
       - main
       - dev
+    paths:
+      - '.github/workflows/**'
 jobs:
   RunAsa:
     runs-on: ubuntu-latest
     steps:
     - name: "Checkout repo"
       uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
     - name: "Run asa scanner"
```

