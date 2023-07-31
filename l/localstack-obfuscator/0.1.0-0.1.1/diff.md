# Comparing `tmp/localstack_obfuscator-0.1.0.tar.gz` & `tmp/localstack_obfuscator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack_obfuscator-0.1.0.tar", last modified: Fri Jul 28 19:07:27 2023, max compression
+gzip compressed data, was "localstack_obfuscator-0.1.1.tar", last modified: Mon Jul 31 17:23:25 2023, max compression
```

## Comparing `localstack_obfuscator-0.1.0.tar` & `localstack_obfuscator-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cristopher  (1000) cristopher  (1000)        0 2023-07-28 19:07:27.121249 localstack_obfuscator-0.1.0/
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)      252 2023-07-28 19:07:27.121249 localstack_obfuscator-0.1.0/PKG-INFO
-drwxr-xr-x   0 cristopher  (1000) cristopher  (1000)        0 2023-07-28 19:07:27.121249 localstack_obfuscator-0.1.0/localstack_obfuscator/
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)        0 2023-07-28 19:01:24.000000 localstack_obfuscator-0.1.0/localstack_obfuscator/__init__.py
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)     2669 2023-07-28 19:01:24.000000 localstack_obfuscator-0.1.0/localstack_obfuscator/localstack_obfuscator.py
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)     1552 2023-07-28 19:01:24.000000 localstack_obfuscator-0.1.0/localstack_obfuscator/ls_patches.py
-drwxr-xr-x   0 cristopher  (1000) cristopher  (1000)        0 2023-07-28 19:07:27.121249 localstack_obfuscator-0.1.0/localstack_obfuscator.egg-info/
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)      252 2023-07-28 19:07:26.000000 localstack_obfuscator-0.1.0/localstack_obfuscator.egg-info/PKG-INFO
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)      363 2023-07-28 19:07:27.000000 localstack_obfuscator-0.1.0/localstack_obfuscator.egg-info/SOURCES.txt
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)        1 2023-07-28 19:07:26.000000 localstack_obfuscator-0.1.0/localstack_obfuscator.egg-info/dependency_links.txt
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)       91 2023-07-28 19:07:26.000000 localstack_obfuscator-0.1.0/localstack_obfuscator.egg-info/entry_points.txt
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)       22 2023-07-28 19:07:26.000000 localstack_obfuscator-0.1.0/localstack_obfuscator.egg-info/top_level.txt
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)      442 2023-07-28 19:07:27.121249 localstack_obfuscator-0.1.0/setup.cfg
--rw-r--r--   0 cristopher  (1000) cristopher  (1000)       52 2023-07-28 19:01:55.000000 localstack_obfuscator-0.1.0/setup.py
+drwxr-xr-x   0 cristopher  (1000) cristopher  (1000)        0 2023-07-31 17:23:25.696265 localstack_obfuscator-0.1.1/
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)      252 2023-07-31 17:23:25.696265 localstack_obfuscator-0.1.1/PKG-INFO
+drwxr-xr-x   0 cristopher  (1000) cristopher  (1000)        0 2023-07-31 17:23:25.696265 localstack_obfuscator-0.1.1/localstack_obfuscator/
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)        0 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator/__init__.py
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)     2729 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator/localstack_obfuscator.py
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)     1552 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator/ls_patches.py
+drwxr-xr-x   0 cristopher  (1000) cristopher  (1000)        0 2023-07-31 17:23:25.696265 localstack_obfuscator-0.1.1/localstack_obfuscator.egg-info/
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)      252 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator.egg-info/PKG-INFO
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)      363 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator.egg-info/SOURCES.txt
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)        1 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator.egg-info/dependency_links.txt
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)       91 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator.egg-info/entry_points.txt
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)       22 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/localstack_obfuscator.egg-info/top_level.txt
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)      442 2023-07-31 17:23:25.696265 localstack_obfuscator-0.1.1/setup.cfg
+-rw-r--r--   0 cristopher  (1000) cristopher  (1000)       52 2023-07-31 17:23:25.000000 localstack_obfuscator-0.1.1/setup.py
```

### Comparing `localstack_obfuscator-0.1.0/localstack_obfuscator/localstack_obfuscator.py` & `localstack_obfuscator-0.1.1/localstack_obfuscator/localstack_obfuscator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 _A=False
 import os,sys,yaml,python_minifier
 from localstack_obfuscator.ls_patches import patch
 CONFIG_FILE_NAME='obfuscator.yml'
 def root_code_dir():dir=os.path.dirname(os.path.realpath(__file__));return os.path.realpath(os.path.join(dir,''))
 def mkdir(path):
 	if not os.path.exists(path):os.makedirs(path)
-def run(cmd):print(cmd);os.system(cmd)
-def copy_target_code(target_dir,output_dir_name):B=target_dir;A=os.path.realpath(os.path.join(B,'..',output_dir_name));mkdir(A);C='cp -r "%s" "%s/"'%(B,A);run(C);return A
+def run(cmd):os.system(cmd)
+def copy_target_code(target_dir,output_dir_name):B=target_dir;A=os.path.realpath(os.path.join(B,'..',output_dir_name));mkdir(A);C='cp -r "%s" "%s/"'%(B,A);print(f"Copying target code to {A}");run(C);return A
 def apply_python_minifier_patches():
 	'Idempotent operation that applies required patches to python-minifier';C=True;import ast as B;from python_minifier.transforms.remove_annotations import RemoveAnnotations as A
 	def F(node):
 		E='dataclasses';D='dataclass';A=node
 		if not isinstance(A.parent,B.ClassDef):return _A
 		if len(A.parent.decorator_list)==0:return _A
 		for A in A.parent.decorator_list:
@@ -33,23 +33,24 @@
 def load_file(path):
 	with open(path,'r')as A:return A.read()
 def save_file(path,content):
 	with open(path,'w')as A:return A.write(content)
 def load_config(target):
 	A=os.path.join(target,CONFIG_FILE_NAME)
 	try:B=open(A,'r');return yaml.safe_load(B)
-	except FileNotFoundError:print('No localstack_obfuscator.yml file found in target directory');return{}
+	except FileNotFoundError:print(f"No {CONFIG_FILE_NAME} file found in target directory");return{}
 def obfuscate(dirpath):
-	F='target_dir';A=dirpath;A=os.path.realpath(A);B=load_config(A)
+	G='target_dir';A=dirpath;A=os.path.realpath(A);B=load_config(A)
 	if B.get('custom_patches',_A):apply_python_minifier_patches()
-	if B.get(F):D=os.path.join(A,B.get(F))
-	else:G=os.path.basename(A);D=os.path.join(A,G)
-	H=copy_target_code(D,B.get('output_dir','build'));I=B.get('minify',{});J=B.get('exclude',[])
-	for(K,N,L)in os.walk(os.path.join(H)):
+	if B.get(G):D=os.path.join(A,B.get(G))
+	else:H=os.path.basename(A);D=os.path.join(A,H)
+	E=copy_target_code(D,B.get('output_dir','build'));I=B.get('minify',{});J=B.get('exclude',[]);print(f"Obfuscating code in {E}")
+	for(K,N,L)in os.walk(os.path.join(E)):
 		for C in L:
 			if C in J or not C.endswith('.py'):continue
-			E=os.path.join(K,C);M=python_minifier.minify(load_file(E),**I);save_file(E,M)
+			F=os.path.join(K,C);M=python_minifier.minify(load_file(F),**I);save_file(F,M)
+	print('Done!')
 def main():
 	A=sys.argv[1:]
-	if len(A)!=1:print('Usage: python localstack_obfuscator.py <dirpath>');sys.exit(1)
+	if len(A)!=1:print('Usage: localstack-obfuscator <dirpath>');sys.exit(1)
 	B=A[0];obfuscate(B)
 if __name__=='__main__':main()
```

### Comparing `localstack_obfuscator-0.1.0/localstack_obfuscator/ls_patches.py` & `localstack_obfuscator-0.1.1/localstack_obfuscator/ls_patches.py`

 * *Files identical despite different names*

