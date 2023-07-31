# Comparing `tmp/aiutil-0.80.6.tar.gz` & `tmp/aiutil-0.81.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiutil-0.80.6.tar", max compression
+gzip compressed data, was "aiutil-0.81.0.tar", max compression
```

## Comparing `aiutil-0.80.6.tar` & `aiutil-0.81.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-07-31 01:06:40.628882 aiutil-0.80.6/LICENSE
--rw-r--r--   0        0        0     1861 2023-07-31 01:06:40.628882 aiutil-0.80.6/README.md
--rw-r--r--   0        0        0       96 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/__init__.py
--rw-r--r--   0        0        0     1968 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/collections.py
--rw-r--r--   0        0        0    10716 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/cv.py
--rw-r--r--   0        0        0     3246 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/dataframe.py
--rw-r--r--   0        0        0     3501 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/datetime.py
--rw-r--r--   0        0        0     2092 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/dockerhub.py
--rw-r--r--   0        0        0    23197 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/filesystem.py
--rw-r--r--   0        0        0       81 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/__init__.py
--rw-r--r--   0        0        0     9194 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/hdfs.py
--rw-r--r--   0        0        0     5910 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/kerberos.py
--rw-r--r--   0        0        0    18754 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/log.py
--rw-r--r--   0        0        0     7473 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/logf.py
--rw-r--r--   0        0        0    16000 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/pyspark_submit.py
--rw-r--r--   0        0        0     1245 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/pyspark_submit.yaml
--rw-r--r--   0        0        0     1450 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hash.py
--rw-r--r--   0        0        0     3950 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/memory.py
--rw-r--r--   0        0        0        0 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/notebook/__init__.py
--rwxr-xr-x   0        0        0     9614 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/notebook/search.py
--rw-r--r--   0        0        0     2337 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/notebook/util.py
--rw-r--r--   0        0        0     1612 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/pdf.py
--rw-r--r--   0        0        0    10900 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/poetry.py
--rw-r--r--   0        0        0     1102 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/pypi.py
--rw-r--r--   0        0        0     2111 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/shebang.py
--rw-r--r--   0        0        0     4637 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/shell.py
--rw-r--r--   0        0        0      660 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/sql.py
--rw-r--r--   0        0        0      651 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/url.py
--rw-r--r--   0        0        0     1159 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/utils.py
--rw-r--r--   0        0        0     2541 2023-07-31 01:06:40.632882 aiutil-0.80.6/pyproject.toml
--rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 aiutil-0.80.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-31 07:27:29.369352 aiutil-0.81.0/LICENSE
+-rw-r--r--   0        0        0     1861 2023-07-31 07:27:29.369352 aiutil-0.81.0/README.md
+-rw-r--r--   0        0        0       96 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/collections.py
+-rw-r--r--   0        0        0    10716 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/cv.py
+-rw-r--r--   0        0        0     3246 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/dataframe.py
+-rw-r--r--   0        0        0     3501 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/datetime.py
+-rw-r--r--   0        0        0     2092 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/dockerhub.py
+-rw-r--r--   0        0        0    23197 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/filesystem.py
+-rw-r--r--   0        0        0     2544 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/git.py
+-rw-r--r--   0        0        0       81 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hadoop/__init__.py
+-rw-r--r--   0        0        0     9194 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hadoop/hdfs.py
+-rw-r--r--   0        0        0     5910 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hadoop/kerberos.py
+-rw-r--r--   0        0        0    18754 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hadoop/log.py
+-rw-r--r--   0        0        0     7473 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hadoop/logf.py
+-rw-r--r--   0        0        0    16000 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hadoop/pyspark_submit.py
+-rw-r--r--   0        0        0     1245 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hadoop/pyspark_submit.yaml
+-rw-r--r--   0        0        0     1450 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/hash.py
+-rw-r--r--   0        0        0     3950 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/memory.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/notebook/__init__.py
+-rwxr-xr-x   0        0        0     9614 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/notebook/search.py
+-rw-r--r--   0        0        0     2337 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/notebook/util.py
+-rw-r--r--   0        0        0     1612 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/pdf.py
+-rw-r--r--   0        0        0    10125 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/poetry.py
+-rw-r--r--   0        0        0     1102 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/pypi.py
+-rw-r--r--   0        0        0     2111 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/shebang.py
+-rw-r--r--   0        0        0     4637 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/shell.py
+-rw-r--r--   0        0        0      660 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/sql.py
+-rw-r--r--   0        0        0      651 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/url.py
+-rw-r--r--   0        0        0     1159 2023-07-31 07:27:29.369352 aiutil-0.81.0/aiutil/utils.py
+-rw-r--r--   0        0        0     2611 2023-07-31 07:27:29.373352 aiutil-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 aiutil-0.81.0/PKG-INFO
```

### Comparing `aiutil-0.80.6/LICENSE` & `aiutil-0.81.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/README.md` & `aiutil-0.81.0/README.md`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/collections.py` & `aiutil-0.81.0/aiutil/collections.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/cv.py` & `aiutil-0.81.0/aiutil/cv.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/dataframe.py` & `aiutil-0.81.0/aiutil/dataframe.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/datetime.py` & `aiutil-0.81.0/aiutil/datetime.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/dockerhub.py` & `aiutil-0.81.0/aiutil/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/filesystem.py` & `aiutil-0.81.0/aiutil/filesystem.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/hadoop/hdfs.py` & `aiutil-0.81.0/aiutil/hadoop/hdfs.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/hadoop/kerberos.py` & `aiutil-0.81.0/aiutil/hadoop/kerberos.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/hadoop/log.py` & `aiutil-0.81.0/aiutil/hadoop/log.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/hadoop/logf.py` & `aiutil-0.81.0/aiutil/hadoop/logf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/hadoop/pyspark_submit.py` & `aiutil-0.81.0/aiutil/hadoop/pyspark_submit.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/hadoop/pyspark_submit.yaml` & `aiutil-0.81.0/aiutil/hadoop/pyspark_submit.yaml`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/hash.py` & `aiutil-0.81.0/aiutil/hash.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/memory.py` & `aiutil-0.81.0/aiutil/memory.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/notebook/search.py` & `aiutil-0.81.0/aiutil/notebook/search.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/notebook/util.py` & `aiutil-0.81.0/aiutil/notebook/util.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/pdf.py` & `aiutil-0.81.0/aiutil/pdf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/poetry.py` & `aiutil-0.81.0/aiutil/poetry.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,38 +5,34 @@
 from pathlib import Path
 import os
 import shutil
 import subprocess as sp
 import toml
 from loguru import logger
 import pathspec
-import dulwich
-from dulwich.contrib.paramiko_vendor import ParamikoSSHVendor
 from .filesystem import replace_patterns
+from . import git
 
 DIST = "dist"
 README = "README.md"
 TOML = "pyproject.toml"
-dulwich.client.get_ssh_vendor = ParamikoSSHVendor
 
 
 def _project_dir() -> Path:
     """Get the root directory of the Poetry project.
 
     :return: The root directory of the Poetry project.
     :raises RuntimeError: Raises RuntimeError if the current directory is not under a Python Poetry project.
     """
     path = Path.cwd()
     while path.parent != path:
         if (path / TOML).is_file():
             return path
         path = path.parent
-    raise RuntimeError(
-        f"The current work directory {Path.cwd()} is not a (subdirectory of a) Python Poetry project."
-    )
+    return Path()
 
 
 def _project_name(proj_dir: Path) -> str:
     """Get the name of the project.
 
     :param proj_dir: The root directory of the Poetry project.
     :return: The name of the project.
@@ -114,18 +110,18 @@
     :param proj_dir: The root directory of the Poetry project.
     """
     if proj_dir is None:
         proj_dir = _project_dir()
     if ver:
         _update_version(ver=ver, proj_dir=proj_dir)
         if commit:
-            repo = dulwich.repo.Repo(proj_dir)
-            dulwich.porcelain.add(repo=repo)
-            dulwich.porcelain.commit(repo=repo, message="bump up version")
-            dulwich.porcelain.push(repo=repo)
+            repo = git.Repo(root=proj_dir)
+            repo.add()
+            repo.commit(message="bump up version")
+            repo.push()
     else:
         print(_project_version(proj_dir))
 
 
 def add_tag_release(
     proj_dir: Union[str, Path, None] = None, tag: str = "", branch_release: str = "main"
 ) -> None:
@@ -133,33 +129,31 @@
     The tag is decided based on the current version of the project.
 
     :param proj_dir: The root directory of the Poetry project.
     :param tag: The tag (defaults to the current version of the package) to use.
     :param branch_release: The branch for releasing.
     :raises ValueError: If the tag to create already exists.
     """
+    if proj_dir is None:
+        proj_dir = _project_dir()
     if not tag:
-        if proj_dir is None:
-            proj_dir = _project_dir()
         tag = "v" + _project_version(proj_dir)
-    repo = dulwich.repo.Repo(proj_dir)
-    if tag.encode() in dulwich.porcelain.tag_list(repo):
+    repo = git.Repo(proj_dir)
+    if tag.encode() in repo.tag():
         raise ValueError(
             f"The tag {tag} already exists! Please merge new changes to the {branch_release} branch first."
         )
-    branch_old = dulwich.porcelain.active_branch(repo=repo).decode()
+    branch_old = repo.active_branch()
     # add tag to the release branch
-    dulwich.porcelain.checkout_branch(repo=repo, target=branch_release)
-    dulwich.porcelain.pull(repo=repo, refspecs=branch_release)
-    dulwich.porcelain.tag_create(repo=repo, tag=tag, annotated=True)
-    remote = dulwich.porcelain.get_branch_remote(repo=repo).decode()
-    sp.run(f"git push {remote} {tag}", shell=True, check=True)
-    # dulwich.porcelain.push(repo=repo, refspecs=[f"refs/tags/{tag}"])
+    repo.checkout(branch=branch_release)
+    repo.pull(branch=branch_release)
+    repo.tag(tag=tag)
+    repo.push(branch=tag)
     # switch back to the old branch
-    dulwich.porcelain.checkout_branch(repo=repo, target=branch_old)
+    repo.checkout(branch=branch_old)
 
 
 def format_code(
     commit: bool = False,
     proj_dir: Optional[Path] = None,
     files: Iterable[Union[Path, str]] = (),
 ) -> None:
@@ -180,19 +174,19 @@
     else:
         if proj_dir is None:
             proj_dir = _project_dir()
         cmd += str(proj_dir)
     logger.info("Formatting code using black ...")
     sp.run(cmd, shell=True, check=False, stdout=sp.PIPE)
     if commit:
-        repo = dulwich.repo.Repo(proj_dir)
-        dulwich.porcelain.add(repo=repo)
-        dulwich.porcelain.commit(repo=repo, message="format code")
-        dulwich.porcelain.push(repo=repo)
-        print(dulwich.porcelain.status())
+        repo = git.Repo(proj_dir)
+        repo.add()
+        repo.commit(message="format code")
+        repo.push()
+        repo.status()
 
 
 def _lint_code(proj_dir: Union[Path, None], linter: Union[str, list[str]]):
     funcs = {
         "pylint": _lint_code_pylint,
         "flake8": _lint_code_flake8,
         "pytype": _lint_code_pytype,
```

### Comparing `aiutil-0.80.6/aiutil/pypi.py` & `aiutil-0.81.0/aiutil/pypi.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/shebang.py` & `aiutil-0.81.0/aiutil/shebang.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/shell.py` & `aiutil-0.81.0/aiutil/shell.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/sql.py` & `aiutil-0.81.0/aiutil/sql.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/url.py` & `aiutil-0.81.0/aiutil/url.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/aiutil/utils.py` & `aiutil-0.81.0/aiutil/utils.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.6/pyproject.toml` & `aiutil-0.81.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiutil"
-version = "0.80.6"
+version = "0.81.0"
 description = "A utils Python package for data scientists."
 authors = ["Benjamin Du <longendu@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/legendu-net/aiutil"
 keywords = ["AI", "Machine Learning", "tools", "utils"]
 
@@ -27,43 +27,44 @@
 loguru = ">=0.3.2"
 toml = ">=0.10.0"
 notifiers = ">=1.2.1"
 PyYAML = ">=5.3.1"
 python-magic = ">=0.4.0"
 tqdm = ">=4.59.0"
 pytest = ">=3.0"
+dulwich = ">=0.20.24"
+scikit-image = ">=0.18.3"
+paramiko = ">=3.2.0"
 # admin
 psutil = { version = ">=5.7.3", optional = true}
 # cv
 opencv-python = { version = ">=4.0.0.0", optional = true }
 pillow = { version = ">=7.0.0", optional = true }
 # docker
 networkx = { version = ">=2.5", optional = true }
 docker = { version = ">=4.4.0", optional = true }
 requests = { version = ">=2.20.0", optional = true }
 # pdf
 PyPDF2 = { version = ">=1.26.0", optional = true }
 # jupyter
 nbformat = { version = ">=5.0.7", optional = true }
 nbconvert = { version = ">=5.6.1", optional = true }
-black = {extras = ["jupyter"], version = ">=23.7.0"}
-dulwich = ">=0.20.24"
-scikit-image = ">=0.18.3"
-paramiko = ">=3.2.0"
+black = {extras = ["jupyter"], version = ">=23.7.0", optional = true}
 
 [tool.poetry.extras]
 cv = ["opencv-python", "pillow"]
 docker = ["docker", "networkx", "requests"]
 pdf = ["PyPDF2"]
 jupyter = ["nbformat", "nbconvert", "black"]
 admin = ["psutil"]
 all = ["opencv-python", "pillow", "docker", "networkx", "requests", "PyPDF2", "nbformat", "nbconvert", "black", "psutil"]
 
 [tool.poetry.group.dev.dependencies]
 pylint = ">=2.7.0"
+black = {extras = ["jupyter"], version = ">=23.7.0"}
 #pytype = {git = "https://github.com/google/pytype.git"}
 darglint = ">=1.5.8"
 
 [tool.pylint.master]
 ignore = ".venv,.ipynb_checkpoints"
 unsafe-load-any-extension = "no"
 extension-pkg-whitelist = "numpy,cv2,pyspark"
```

### Comparing `aiutil-0.80.6/PKG-INFO` & `aiutil-0.81.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiutil
-Version: 0.80.6
+Version: 0.81.0
 Summary: A utils Python package for data scientists.
 Home-page: https://github.com/legendu-net/aiutil
 License: MIT
 Keywords: AI,Machine Learning,tools,utils
 Author: Benjamin Du
 Author-email: longendu@yahoo.com
 Requires-Python: >=3.10,<3.12
```

