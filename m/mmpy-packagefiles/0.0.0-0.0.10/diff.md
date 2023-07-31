# Comparing `tmp/mmpy_packagefiles-0.0.0.tar.gz` & `tmp/mmpy_packagefiles-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmpy_packagefiles-0.0.0.tar", last modified: Thu Jun 29 20:07:33 2023, max compression
+gzip compressed data, was "mmpy_packagefiles-0.0.10.tar", last modified: Mon Jul 31 01:57:57 2023, max compression
```

## Comparing `mmpy_packagefiles-0.0.0.tar` & `mmpy_packagefiles-0.0.10.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:07:33.023908 mmpy_packagefiles-0.0.0/
--rw-rw-rw-   0        0        0     1094 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       87 2023-06-29 20:07:33.022907 mmpy_packagefiles-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/README.md
--rw-rw-rw-   0        0        0        0 2023-06-29 19:47:53.000000 mmpy_packagefiles-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 20:07:33.023908 mmpy_packagefiles-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 20:07:32.988621 mmpy_packagefiles-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 20:07:33.011454 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/
--rw-rw-rw-   0        0        0        0 2023-06-29 19:00:37.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/__init__.py
--rw-rw-rw-   0        0        0     6867 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/database.py
--rw-rw-rw-   0        0        0     2603 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/obvious.py
--rw-rw-rw-   0        0        0     7644 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/parse.py
--rw-rw-rw-   0        0        0    10491 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/proof.py
--rw-rw-rw-   0        0        0     1052 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/scratch.py
--rw-rw-rw-   0        0        0     6522 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/theory.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:07:33.020907 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles.egg-info/
--rw-rw-rw-   0        0        0       87 2023-06-29 20:07:32.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-06-29 20:07:32.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:07:32.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-29 20:07:32.000000 mmpy_packagefiles-0.0.0/src/mmpy_packagefiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 01:57:57.449877 mmpy_packagefiles-0.0.10/
+-rw-rw-rw-   0        0        0     1094 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.10/LICENSE
+-rw-rw-rw-   0        0        0      541 2023-07-31 01:57:57.447837 mmpy_packagefiles-0.0.10/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.10/README.md
+-rw-rw-rw-   0        0        0      632 2023-07-31 01:57:33.000000 mmpy_packagefiles-0.0.10/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 01:57:57.450891 mmpy_packagefiles-0.0.10/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 01:57:57.393300 mmpy_packagefiles-0.0.10/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 01:57:57.426889 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/
+-rw-rw-rw-   0        0        0        0 2023-06-29 19:00:37.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/__init__.py
+-rw-rw-rw-   0        0        0     6867 2023-07-31 01:45:36.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/database.py
+-rw-rw-rw-   0        0        0     2603 2023-06-30 19:50:05.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/obvious.py
+-rw-rw-rw-   0        0        0     7644 2023-07-31 01:45:38.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/parse.py
+-rw-rw-rw-   0        0        0    10647 2023-07-21 19:35:26.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/proof.py
+-rw-rw-rw-   0        0        0     1052 2023-06-29 18:33:43.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/scratch.py
+-rw-rw-rw-   0        0        0     6522 2023-07-10 19:38:26.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/theory.py
+-rw-rw-rw-   0        0        0      922 2023-07-31 01:45:43.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/training_data.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:57:57.442613 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-07-31 01:57:57.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-07-31 01:57:57.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 01:57:57.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-31 01:57:57.000000 mmpy_packagefiles-0.0.10/src/mmpy_packagefiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 01:57:57.444796 mmpy_packagefiles-0.0.10/tests/
+-rw-rw-rw-   0        0        0     2915 2023-07-13 22:22:40.000000 mmpy_packagefiles-0.0.10/tests/tests.py
```

### Comparing `mmpy_packagefiles-0.0.0/LICENSE` & `mmpy_packagefiles-0.0.10/LICENSE`

 * *Files identical despite different names*

### Comparing `mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/database.py` & `mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/database.py`

 * *Files identical despite different names*

### Comparing `mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/obvious.py` & `mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/obvious.py`

 * *Files identical despite different names*

### Comparing `mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/parse.py` & `mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/parse.py`

 * *Files identical despite different names*

### Comparing `mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/proof.py` & `mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/proof.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,22 @@
     profile = lambda x: x
 
 """
 symbols[n]: nth token in symbol string
 substitution[v]: symbol string to put in place of symbol v
 returns result[n]: nth token after substitutions applied
 """
-@profile
+# @profile
 def substitute(symbols, substitution):
     result = ()
     for symbol in symbols:
         if symbol in substitution: result += substitution[symbol]
         else: result += (symbol,)
     return result
+# from substitute import substitute # cython version
 
 """
 Proof step: represents one step of a proof
 conclusion: the symbol string that is concluded by applying an inference rule
 rule: the rule object that was applied
 dependencies[h]: another inference object, whose conclusion met the rule hypothesis with label h
 substitution: the substitution that transforms the rule's consequent and hypotheses into the conclusion and dependencies
@@ -206,39 +207,41 @@
     for hypothesis in claim.hypotheses:
         conclusion, rule = tuple(hypothesis.tokens), database.rules[hypothesis.label]
         proof_steps.append(ProofStep(conclusion, rule, {}, {}))
     # step labels
     proof_steps += step_labels
 
     # process each step in proof
+    proof_step_dict = {}
     for step, pointer in enumerate(step_pointers):
 
         # tag previous step if requested
         if pointer < 0: proof_steps.append(stack[-1])
 
         # otherwise handle current proof step
         else:
 
             # retrieve current step
             proof_step = proof_steps[pointer]
 
             # replace labels by associated step
             if type(proof_step) is str:
                 proof_step = conduct(database.rules[proof_step], stack, claim)
+                proof_step_dict[proof_step.conclusion] = proof_step
 
             # push current proof step onto stack
             stack.append(proof_step)
 
     # check that original claim has been proved
     assert stack[0].conclusion == tuple(claim.consequent.tokens), \
            f"proved statement {' '.join(stack[0].conclusion)} does not match theorem {' '.join(claim.consequent.tokens)}"
     assert len(stack) == 1, f"non-singleton stack {stack} after proof"
 
     # return root of proof graph and dictionary of nodes
-    return stack[0], proof_steps
+    return stack[0], proof_step_dict
 
 def verify_proof(database, claim):
     # compressed proofs start with "(" token
     if claim.consequent.proof[0] == "(":
         return verify_compressed_proof(database, claim)
     else:
         return verify_normal_proof(database, claim)
@@ -281,11 +284,11 @@
     #     print(k, " ".join(conclusion), step.rule.consequent.label, edges)
 
     import os
     fpath = os.path.join(os.environ["HOME"], "metamath", "set.mm")
     db = parse(fpath)
     print("parsed.")
 
-    verify_all(db)
-    # verify_all(db, stop=5000)
+    # verify_all(db)
+    verify_all(db, stop=20000)
     # verify_compressed_proof(db, db.rules['ax5d'])
```

### Comparing `mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/scratch.py` & `mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/scratch.py`

 * *Files identical despite different names*

### Comparing `mmpy_packagefiles-0.0.0/src/mmpy_packagefiles/theory.py` & `mmpy_packagefiles-0.0.10/src/mmpy_packagefiles/theory.py`

 * *Files identical despite different names*

