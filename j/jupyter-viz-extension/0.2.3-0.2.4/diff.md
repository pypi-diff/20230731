# Comparing `tmp/jupyter_viz_extension-0.2.3.tar.gz` & `tmp/jupyter_viz_extension-0.2.4.tar.gz`

## Comparing `jupyter_viz_extension-0.2.3.tar` & `jupyter_viz_extension-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/.yarnrc.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/install.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/tsconfig.json
--rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/yarn.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter-config/nb-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter-config/server-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/_version.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/trame_model.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/cmd.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/paraview.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/trame.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/user.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/package.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/759.b87504abaef54983a24e.js
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/remoteEntry.e49408fc099f9436f8e2.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/style.js
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/share/launch_paraview.in
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/schema/plugin.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/components.tsx
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/dialogs.tsx
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/handler.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/index.tsx
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/paraview.tsx
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/trame.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/base.css
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/collapsible.css
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/index.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/LICENSE
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/.yarnrc.yml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/install.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/tsconfig.json
+-rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/yarn.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter-config/nb-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter-config/server-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/_version.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/trame_model.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/cmd.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/paraview.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/trame.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/user.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/package.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/759.31e0c66cf5e4357de249.js
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/remoteEntry.f31b28d3ff5c024fc221.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/share/launch_paraview.in
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/schema/plugin.json
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/components.tsx
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/dialogs.tsx
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/handler.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/index.tsx
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/paraview.tsx
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/trame.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/base.css
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/collapsible.css
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/index.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/README.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/PKG-INFO
```

### Comparing `jupyter_viz_extension-0.2.3/package.json` & `jupyter_viz_extension-0.2.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.4'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.2.4"
 }
```

### Comparing `jupyter_viz_extension-0.2.3/tsconfig.json` & `jupyter_viz_extension-0.2.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/yarn.lock` & `jupyter_viz_extension-0.2.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/__init__.py` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/trame_model.py` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/trame_model.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/cmd.py` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/cmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 
 
-async def run(programm: str, *args: str, logger=None, **kwargs):
+async def run(programm: str, *args: str, logger=None, **kwargs) -> int:
     command = " ".join([programm, *args])
     
     proccess = await asyncio.create_subprocess_shell(
         command,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
         **kwargs
@@ -19,20 +19,25 @@
             logger.info(f"[stdout]\n{stdout.decode()}")
         if stderr:
             logger.info(f"[stderr]\n{stderr.decode()}")
     
     return proccess.returncode
 
 
-async def output(programm: str, *args: str, **kwargs):
+async def output(programm: str, *args: str, logger=None, **kwargs) -> tuple[int, str]:
     command = " ".join([programm, *args])
     
     proccess = await asyncio.create_subprocess_shell(
         command,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.STDOUT,
         **kwargs
     )
     
     stdout, _ = await proccess.communicate()
 
-    return stdout.decode()
+    if logger:
+        logger.info(f"{command!r} exited with {proccess.returncode}")
+        if stdout:
+            logger.info(f"[stdout]\n{stdout.decode()}")
+
+    return proccess.returncode, stdout.decode()
```

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/paraview.py` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/paraview.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from jinja2 import Template
 from jupyter_server.base.handlers import APIHandler
 from tornado.web import authenticated
-from .cmd import run, output
+
+from .cmd import output
 
 
 class ParaViewHandler(APIHandler):
     async def get_running_servers(self):
-        out = await output("squeue", "--me", "--noheader", "--Format='Partition,Account,NumNodes,TimeUsed,TimeLimit,State,NodeList'")
+        _, out = await output("squeue", "--me", "--noheader", "--Format='Partition,Account,NumNodes,TimeUsed,TimeLimit,State,NodeList'")
 
         servers = []
         for server in out.splitlines():
             self.log.info(f"Found Server: {server}")
             partition, account, nodes, time_used, time_limit, state, *nodelist = server.split()
             servers.append({
                 "partition": partition,
@@ -35,25 +36,25 @@
 
         # Create a tempfile and write the SLURM Config into it
         with NamedTemporaryFile("w", delete=False) as tmp:
             path = tmp.name
             tmp.write(template.render(options))
 
         self.log.info(f"Job script in {path!r}")
-        await run("sbatch", path, logger=self.log)
+        return await output("sbatch", path, logger=self.log)
 
     @authenticated
     async def get(self):
         servers = await self.get_running_servers()
         await self.finish(json.dumps(servers))
         
     @authenticated
     async def post(self):
         try:
-            await self.launch_paraview(json.loads(self.request.body))
+            return_code, message = await self.launch_paraview(json.loads(self.request.body))
             self.set_status(200)
-            await self.finish()
+            await self.finish({"returnCode": return_code, "message": message})
             
         except Exception as e:
             self.log.error(str(e))
             self.set_status(400)
             await self.finish(str(e))
```

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/trame.py` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/trame.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/user.py` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 from jupyter_server.base.handlers import APIHandler
 from tornado.web import authenticated
 from .cmd import output
 
 
 async def _get_accounts():
-    out = await output("jutil", "user", "projects", "--format='json'")
+    _, out = await output("jutil", "user", "projects", "--format='json'")
     return [group["unixgroup"] for group in json.loads(out)] if out else []
 
 
 async def _get_partitions():
     return ["booster", "develbooster"]
```

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/package.json` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f31b28d3ff5c024fc221.js'}}",*

 * * "'version'": "'0.2.4'"}*

```diff
@@ -106,15 +106,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/jupyter-viz-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e49408fc099f9436f8e2.js",
+            "load": "static/remoteEntry.f31b28d3ff5c024fc221.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_viz_extension"
                 },
@@ -183,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.2.4"
 }
```

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.4'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.2.4"
 }
```

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/759.b87504abaef54983a24e.js` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/759.31e0c66cf5e4357de249.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 "use strict";
 (self.webpackChunkjupyter_viz_extension = self.webpackChunkjupyter_viz_extension || []).push([
     [759], {
         759: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => x
+                default: () => S
             });
             var a = n(303),
                 s = n(832),
                 i = n(271),
-                r = n.n(i),
-                l = n(628),
-                o = n.n(l),
-                c = n(344),
+                o = n.n(i),
+                r = n(628),
+                c = n.n(r),
+                l = n(344),
                 p = n(139);
             async function u(e, t = {}) {
                 const n = p.ServerConnection.makeSettings(),
-                    a = c.URLExt.join(n.baseUrl, "jupyter-viz-extension", e);
+                    a = l.URLExt.join(n.baseUrl, "jupyter-viz-extension", e);
                 let s;
                 try {
                     s = await p.ServerConnection.makeRequest(a, t, n)
                 } catch (e) {
                     throw new p.ServerConnection.NetworkError(e)
                 }
                 let i = await s.text();
@@ -109,15 +109,15 @@
                     }), i.createElement(v, {
                         label: "Status",
                         value: this.props.state
                     }), i.createElement(v, {
                         label: "Time",
                         value: `${this.props.timeUsed} / ${this.props.timeLimit}`
                     }));
-                    return i.createElement(i.Fragment, null, i.createElement(o(), {
+                    return i.createElement(i.Fragment, null, i.createElement(c(), {
                         trigger: t
                     }, i.createElement(v, {
                         label: "Project",
                         value: this.props.account
                     }), i.createElement(v, {
                         label: "Partition",
                         value: this.props.partition
@@ -130,44 +130,49 @@
                     })))
                 }
             }
             class C extends i.Component {
                 constructor() {
                     super({}), this.fetchData = async () => {
                         this.setState({
-                            instaces: await u("paraview")
+                            instances: await u("paraview")
                         })
                     }, this.newInstance = async () => {
                         const e = await (0, a.showDialog)({
                             title: "Launch a new ParaView instance",
                             body: new E
                         });
-                        console.log(e.value), await u("paraview", {
+                        console.log(e.value);
+                        const t = await u("paraview", {
                             method: "POST",
                             body: JSON.stringify(e.value)
-                        }), await this.fetchData()
+                        });
+                        await Promise.all([(0, a.showErrorMessage)(0 === t.returnCode ? "Success" : "Error", t.message), this.fetchData()])
                     }, this.state = {
-                        instaces: []
-                    }, this.fetchData()
+                        instances: []
+                    }
+                }
+                async componentDidMount() {
+                    await this.fetchData()
                 }
                 render() {
                     return i.createElement(i.Fragment, null, i.createElement("h3", null, "Running ParaView backends:", i.createElement("button", {
                         className: "launch-button",
                         onClick: this.newInstance
                     }, "Launch")), i.createElement("div", {
                         id: "paraview-instances",
                         className: "instance-list"
-                    }, this.state.instaces.map((e => i.createElement(g, Object.assign({}, e))))))
+                    }, this.state.instances.map((e => i.createElement(g, Object.assign({}, e))))))
                 }
             }
             class b extends i.Component {
                 constructor(e) {
                     super(e), this.openInstance = () => {
                         const e = p.ServerConnection.makeSettings(),
-                            t = c.URLExt.join(e.baseUrl, "proxy", String(this.props.port), "index.html");
+                            t = l.URLExt.join(e.baseUrl, "proxy", String(this.props.port), "index.html");
                         window.open(t, "_blank", "noreferrer")
                     }
                 }
                 render() {
                     return i.createElement("li", null, i.createElement("div", {
                         style: {
                             flexGrow: 1
@@ -199,15 +204,15 @@
                         }), await (0, a.showErrorMessage)("Success", `Launched new trame instance on port ${e.port}`)
                     }, this.state = {
                         instances: this.props.instances
                     }
                 }
                 render() {
                     const e = i.createElement("div", null, i.createElement("b", null, " ", this.props.name, " "), i.createElement("br", null), "Running Instances: ", this.state.instances.length);
-                    return i.createElement(i.Fragment, null, i.createElement(o(), {
+                    return i.createElement(i.Fragment, null, i.createElement(c(), {
                         trigger: e
                     }, i.createElement(v, {
                         label: "Path",
                         value: this.props.path
                     }), i.createElement("h4", null, "Instances:", i.createElement("button", {
                         className: "launch-button",
                         onClick: this.launchInstance
@@ -216,35 +221,38 @@
                     }, this.state.instances.map((e => i.createElement(b, Object.assign({}, e)))))))
                 }
             }
             class f extends i.Component {
                 constructor() {
                     super({}), this.fetchData = async () => {
                         this.setState({
-                            apps: await u("trame")
+                            instances: await u("trame")
                         })
                     }, this.state = {
-                        apps: []
-                    }, this.fetchData()
+                        instances: []
+                    }
+                }
+                async componentDidMount() {
+                    await this.fetchData()
                 }
                 render() {
                     return i.createElement(i.Fragment, null, i.createElement("h3", null, "trame Apps:"), i.createElement("div", {
                         id: "trame-instances",
                         className: "instance-list"
-                    }, this.state.apps.map((e => i.createElement(w, Object.assign({}, e))))))
+                    }, this.state.instances.map((e => i.createElement(w, Object.assign({}, e))))))
                 }
             }
-            const x = {
+            const S = {
                 id: "juviz-extension",
                 autoStart: !0,
                 activate: e => {
                     const t = new s.SplitPanel;
                     t.orientation = "vertical", t.id = "juviz-sidepanel", t.title.iconClass = "jp-ExtensionIcon jp-SideBar-tabIcon", t.title.caption = "JuWiz";
-                    const n = a.ReactWidget.create(r().createElement(C, null));
+                    const n = a.ReactWidget.create(o().createElement(C, null));
                     n.addClass("juviz-sidepanel-segment"), t.addWidget(n);
-                    const i = a.ReactWidget.create(r().createElement(f, null));
+                    const i = a.ReactWidget.create(o().createElement(f, null));
                     i.addClass("juviz-sidepanel-segment"), t.addWidget(i), e.shell.add(t, "left")
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/remoteEntry.e49408fc099f9436f8e2.js` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/remoteEntry.f31b28d3ff5c024fc221.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, d, f, c, p, h, v, b, g, m, y = {
+    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v, b, g, m, y = {
             299: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./extension": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -46,21 +46,21 @@
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         187: "f44cc496302e8c70c5db",
         271: "624d1e1a34fcab02d699",
         747: "e893f2b2bb7591fde94c",
-        759: "b87504abaef54983a24e",
+        759: "31e0c66cf5e4357de249",
         893: "b4c09f80424627b87fe3"
     } [e] + ".js?v=" + {
         187: "f44cc496302e8c70c5db",
         271: "624d1e1a34fcab02d699",
         747: "e893f2b2bb7591fde94c",
-        759: "b87504abaef54983a24e",
+        759: "31e0c66cf5e4357de249",
         893: "b4c09f80424627b87fe3"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -75,19 +75,19 @@
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
                         i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyter-viz-extension", "0.2.3", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyter-viz-extension", "0.2.4", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -192,42 +192,42 @@
                     l = !1, u--
                 } else {
                     if (u <= n || d < f != o) return !1;
                     l = !1
                 } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || f(l(e, t, o, n)), c(e[t][o])
+        return a(n, o) || f(l(e, t, o, n)), p(e[t][o])
     }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
         var a = j.I(r);
         return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
         var a = r && j.o(r, t) && d(r, t, n);
-        return a ? c(a) : o()
+        return a ? p(a) : o()
     })), b = {}, g = {
         271: () => h("default", "react", [1, 17, 0, 1]),
         139: () => h("default", "@jupyterlab/services", [1, 6, 6, 5]),
         303: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
         344: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
         628: () => v("default", "react-collapsible", [1, 2, 10, 0], (() => j.e(187).then((() => () => j(893))))),
         832: () => h("default", "@lumino/widgets", [1, 1, 37, 2])
```

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/third-party-licenses.json` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/jupyter_viz_extension/share/launch_paraview.in` & `jupyter_viz_extension-0.2.4/jupyter_viz_extension/share/launch_paraview.in`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/src/dialogs.tsx` & `jupyter_viz_extension-0.2.4/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/src/handler.ts` & `jupyter_viz_extension-0.2.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/src/index.tsx` & `jupyter_viz_extension-0.2.4/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/src/paraview.tsx` & `jupyter_viz_extension-0.2.4/src/paraview.tsx`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import * as React from 'react';
 import Collapsible from 'react-collapsible';
-import { showDialog } from '@jupyterlab/apputils';
+import { showDialog, showErrorMessage } from '@jupyterlab/apputils';
 
 import { requestAPI } from './handler';
 import { ParaViewLauncherDialog } from './dialogs';
-import { Info } from './components';
+import { Info, Empty, InstanceList } from './components';
 
 
 export type ParaViewLaunchOptions = {
   account: string;
   partition: string;
   nodes: number;
   timeLimit: string;
 };
 
-export type ParaViewInstanceOptions = ParaViewLaunchOptions & {
+type ParaViewInstanceOptions = ParaViewLaunchOptions & {
   state: string;
   timeUsed: string;
   url?: string;
 };
 
+type ParaViewReturnStatus = {
+  returnCode: number;
+  message: string;
+}
+
 
 class ParaViewInstance extends React.Component<ParaViewInstanceOptions> {
   constructor(props: ParaViewInstanceOptions) {
     super(props);
   }
 
   render() {
@@ -45,51 +50,57 @@
         </Collapsible>
       </>
     );
   }
 }
 
 
-export class ParaViewSidepanelSegment extends React.Component<Record<string, never>, { instaces: ParaViewInstanceOptions[] }> {
+export class ParaViewSidepanelSegment extends React.Component<Empty, InstanceList<ParaViewInstanceOptions>> {
   constructor() {
     super({});
-    this.state = { instaces: [] };
+    this.state = { instances: [] };
+  }
 
-    this.fetchData();
+  async componentDidMount() {
+    await this.fetchData()
   }
 
   fetchData = async () => {
     this.setState({
-      instaces: await requestAPI<ParaViewInstanceOptions[]>('paraview')
+      instances: await requestAPI<ParaViewInstanceOptions[]>('paraview')
     });
   };
 
   newInstance = async () => {
     const options = await showDialog({
       title: 'Launch a new ParaView instance',
       body: new ParaViewLauncherDialog()
     });
     console.log(options.value);
 
-    await requestAPI<Record<string, never>>('paraview', {
+    const status = await requestAPI<ParaViewReturnStatus>('paraview', {
       method: 'POST',
       body: JSON.stringify(options.value)
     });
-    await this.fetchData();
+
+    await Promise.all([
+      showErrorMessage(status.returnCode === 0 ? 'Success' : 'Error', status.message),
+      this.fetchData(),
+    ])
   };
 
   render() {
     return (
       <>
         <h3>
           Running ParaView backends:
           <button className='launch-button' onClick={this.newInstance}>Launch</button>
         </h3>
         <div id='paraview-instances' className='instance-list'>
-          {this.state.instaces.map((instance) => (
+          {this.state.instances.map((instance) => (
             <ParaViewInstance {...instance} />
           ))}
         </div>
       </>
     );
   }
 }
```

### Comparing `jupyter_viz_extension-0.2.3/src/trame.tsx` & `jupyter_viz_extension-0.2.4/src/trame.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import { URLExt } from '@jupyterlab/coreutils';
 import { ServerConnection } from '@jupyterlab/services';
 import { showErrorMessage } from '@jupyterlab/apputils';
 import * as React from 'react';
 import Collapsible from 'react-collapsible';
-import { Info } from './components';
+
+import { Info, Empty, InstanceList } from './components';
 import { requestAPI } from './handler';
 
 
 type TrameAppOptions = {
   name: string;
   displayName: string;
   path: string;
@@ -42,15 +43,15 @@
         <button className='open-button' onClick={this.openInstance}>Open</button>
       </li>
     );
   }
 }
 
 
-class TrameApp extends React.Component<TrameAppOptions, { instances: TrameInstanceOptions[] }> {
+class TrameApp extends React.Component<TrameAppOptions, InstanceList<TrameInstanceOptions>> {
   constructor(props: TrameAppOptions) {
     super(props);
     this.state = {
       instances: this.props.instances  // Initialize with existing instances. ToDo: Improve?
     };
   }
 
@@ -95,33 +96,36 @@
         </Collapsible>
       </>
     );
   }
 }
 
 
-export class TrameSidepanelSegment extends React.Component<Record<string, never>, { apps: TrameAppOptions[] }> {
+export class TrameSidepanelSegment extends React.Component<Empty, InstanceList<TrameAppOptions>> {
   constructor() {
     super({});
-    this.state = { apps: [] };
-    this.fetchData();
+    this.state = { instances: [] };
+  }
+
+  async componentDidMount() {
+    await this.fetchData();
   }
 
   fetchData = async () => {
     this.setState({
-      apps: await requestAPI<TrameAppOptions[]>('trame')
+      instances: await requestAPI<TrameAppOptions[]>('trame')
     });
   };
 
   render() {
     return (
       <>
         <h3>trame Apps:</h3>
         <div id='trame-instances' className='instance-list'>
-          {this.state.apps.map((app) => (
+          {this.state.instances.map((app) => (
             <TrameApp {...app} />
           ))}
         </div>
       </>
     );
   }
 }
```

### Comparing `jupyter_viz_extension-0.2.3/style/base.css` & `jupyter_viz_extension-0.2.4/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/style/collapsible.css` & `jupyter_viz_extension-0.2.4/style/collapsible.css`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/.gitignore` & `jupyter_viz_extension-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/LICENSE` & `jupyter_viz_extension-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/README.md` & `jupyter_viz_extension-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/pyproject.toml` & `jupyter_viz_extension-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.3/PKG-INFO` & `jupyter_viz_extension-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_viz_extension
-Version: 0.2.3
+Version: 0.2.4
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyter-viz-extension
 Project-URL: Bug Tracker, https://github.com/github_username/jupyter-viz-extension/issues
 Project-URL: Repository, https://github.com/github_username/jupyter-viz-extension.git
 Author-email: Jonathan Windgassen <j.windgassen@fz-juelich.de>
 License: BSD 3-Clause License
```

