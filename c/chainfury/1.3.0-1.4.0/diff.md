# Comparing `tmp/chainfury-1.3.0.tar.gz` & `tmp/chainfury-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainfury-1.3.0.tar", max compression
+gzip compressed data, was "chainfury-1.4.0.tar", max compression
```

## Comparing `chainfury-1.3.0.tar` & `chainfury-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-1.3.0/LICENSE
--rw-r--r--   0        0        0     4500 2023-07-26 10:48:59.407812 chainfury-1.3.0/README.md
--rw-r--r--   0        0        0      361 2023-07-26 11:58:05.957831 chainfury-1.3.0/chainfury/__init__.py
--rw-r--r--   0        0        0       39 2023-07-26 05:41:33.286898 chainfury-1.3.0/chainfury/__main__.py
--rw-r--r--   0        0        0    27439 2023-07-27 04:10:46.158868 chainfury-1.3.0/chainfury/agent.py
--rw-r--r--   0        0        0    47544 2023-07-27 04:28:09.607193 chainfury-1.3.0/chainfury/base.py
--rw-r--r--   0        0        0     3570 2023-07-26 05:41:33.288177 chainfury-1.3.0/chainfury/cli.py
--rw-r--r--   0        0        0    13266 2023-07-20 12:08:00.208542 chainfury-1.3.0/chainfury/client.py
--rw-r--r--   0        0        0     1699 2023-07-20 12:08:00.208666 chainfury-1.3.0/chainfury/components/README.md
--rw-r--r--   0        0        0      608 2023-07-26 05:41:33.288471 chainfury-1.3.0/chainfury/components/__init__.py
--rw-r--r--   0        0        0     1146 2023-07-20 12:08:00.209196 chainfury-1.3.0/chainfury/components/ai_actions/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-26 10:43:07.571250 chainfury-1.3.0/chainfury/components/const.py
--rw-r--r--   0        0        0     6836 2023-07-25 12:00:51.905993 chainfury-1.3.0/chainfury/components/functional/__init__.py
--rw-r--r--   0        0        0      419 2023-07-21 11:05:44.530297 chainfury-1.3.0/chainfury/components/milvus/__init__.py
--rw-r--r--   0        0        0     4603 2023-07-20 12:08:00.210177 chainfury-1.3.0/chainfury/components/nbx/__init__.py
--rw-r--r--   0        0        0    12708 2023-07-26 05:41:33.289125 chainfury-1.3.0/chainfury/components/openai/__init__.py
--rw-r--r--   0        0        0     2831 2023-07-24 11:27:34.882593 chainfury-1.3.0/chainfury/components/pinecone_db/__init__.py
--rw-r--r--   0        0        0     9326 2023-07-27 04:41:40.506974 chainfury-1.3.0/chainfury/components/qdrant/__init__.py
--rw-r--r--   0        0        0       78 2023-07-20 12:08:00.210514 chainfury-1.3.0/chainfury/components/redis/__init__.py
--rw-r--r--   0        0        0     8659 2023-07-20 12:08:00.210779 chainfury-1.3.0/chainfury/components/serper/__init__.py
--rw-r--r--   0        0        0     6637 2023-07-20 12:08:00.211018 chainfury-1.3.0/chainfury/components/stability/__init__.py
--rw-r--r--   0        0        0     1013 2023-07-20 12:08:00.211166 chainfury-1.3.0/chainfury/types.py
--rw-r--r--   0        0        0     3556 2023-07-26 05:41:33.289789 chainfury-1.3.0/chainfury/utils.py
--rw-r--r--   0        0        0      135 2023-07-26 05:41:33.290061 chainfury-1.3.0/chainfury/version.py
--rw-r--r--   0        0        0      935 2023-07-26 07:03:35.791974 chainfury-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 chainfury-1.3.0/setup.py
--rw-r--r--   0        0        0     5655 1970-01-01 00:00:00.000000 chainfury-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4500 2023-07-26 10:48:59.407812 chainfury-1.4.0/README.md
+-rw-r--r--   0        0        0      361 2023-07-26 11:58:05.957831 chainfury-1.4.0/chainfury/__init__.py
+-rw-r--r--   0        0        0       39 2023-07-26 05:41:33.286898 chainfury-1.4.0/chainfury/__main__.py
+-rw-r--r--   0        0        0    27439 2023-07-31 07:12:21.933415 chainfury-1.4.0/chainfury/agent.py
+-rw-r--r--   0        0        0    47810 2023-07-31 08:05:23.320930 chainfury-1.4.0/chainfury/base.py
+-rw-r--r--   0        0        0     3570 2023-07-26 05:41:33.288177 chainfury-1.4.0/chainfury/cli.py
+-rw-r--r--   0        0        0    13266 2023-07-20 12:08:00.208542 chainfury-1.4.0/chainfury/client.py
+-rw-r--r--   0        0        0     1699 2023-07-20 12:08:00.208666 chainfury-1.4.0/chainfury/components/README.md
+-rw-r--r--   0        0        0      608 2023-07-26 05:41:33.288471 chainfury-1.4.0/chainfury/components/__init__.py
+-rw-r--r--   0        0        0     1146 2023-07-20 12:08:00.209196 chainfury-1.4.0/chainfury/components/ai_actions/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-26 10:43:07.571250 chainfury-1.4.0/chainfury/components/const.py
+-rw-r--r--   0        0        0     6836 2023-07-25 12:00:51.905993 chainfury-1.4.0/chainfury/components/functional/__init__.py
+-rw-r--r--   0        0        0      419 2023-07-21 11:05:44.530297 chainfury-1.4.0/chainfury/components/milvus/__init__.py
+-rw-r--r--   0        0        0     4603 2023-07-20 12:08:00.210177 chainfury-1.4.0/chainfury/components/nbx/__init__.py
+-rw-r--r--   0        0        0    13853 2023-07-31 07:07:02.390566 chainfury-1.4.0/chainfury/components/openai/__init__.py
+-rw-r--r--   0        0        0     2831 2023-07-24 11:27:34.882593 chainfury-1.4.0/chainfury/components/pinecone_db/__init__.py
+-rw-r--r--   0        0        0     9326 2023-07-27 04:41:40.506974 chainfury-1.4.0/chainfury/components/qdrant/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-20 12:08:00.210514 chainfury-1.4.0/chainfury/components/redis/__init__.py
+-rw-r--r--   0        0        0     8659 2023-07-20 12:08:00.210779 chainfury-1.4.0/chainfury/components/serper/__init__.py
+-rw-r--r--   0        0        0     6637 2023-07-20 12:08:00.211018 chainfury-1.4.0/chainfury/components/stability/__init__.py
+-rw-r--r--   0        0        0     1013 2023-07-20 12:08:00.211166 chainfury-1.4.0/chainfury/types.py
+-rw-r--r--   0        0        0     3556 2023-07-26 05:41:33.289789 chainfury-1.4.0/chainfury/utils.py
+-rw-r--r--   0        0        0      135 2023-07-31 08:25:26.086496 chainfury-1.4.0/chainfury/version.py
+-rw-r--r--   0        0        0      935 2023-07-31 08:25:28.079516 chainfury-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 chainfury-1.4.0/setup.py
+-rw-r--r--   0        0        0     5655 1970-01-01 00:00:00.000000 chainfury-1.4.0/PKG-INFO
```

### Comparing `chainfury-1.3.0/LICENSE` & `chainfury-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/README.md` & `chainfury-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/agent.py` & `chainfury-1.4.0/chainfury/agent.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/base.py` & `chainfury-1.4.0/chainfury/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -744,23 +744,19 @@
         fn = data["fn"]
         if not fn:
             raise ValueError(f"Invalid fn: {fn}")
 
         from chainfury.agent import AIAction, Memory
 
         node_type = data["type"]
-        print("----->>>>>", node_type)
-        print("#######", fn)
         if node_type == NodeType.AI:
             fn = AIAction.from_dict(fn)
         elif node_type == NodeType.MEMORY:
             fn = Memory.from_dict(fn)
 
-            print("ASDFASDFADSFADSFASFD", fn)
-
         return cls(
             id=data["id"],
             type=node_type,
             fn=fn,
             description=data["description"],
             fields=fields,
             outputs=outputs,
@@ -805,16 +801,17 @@
             if not data_keys.issubset(template_keys):
                 raise ValueError(f"Invalid keys passed to node '{self.id}': {data_keys - template_keys}")
             if print_thoughts:
                 print(terminal_top_with_text(f"Node: {self.id}"))
                 print("Inputs:\n------")
                 print(pformat(data))
 
-            print("ASSSSSSSSSSS:", self.fn)
-            out, err = self.fn(**data)  # type: ignore
+            _out = self.fn(**data)  # type: ignore
+            out = _out[0] if isinstance(_out, tuple) else _out
+            err = _out[1] if isinstance(_out, tuple) and len(_out) > 1 else None
             if err:
                 raise err
 
             # this is where we have to polish this outgoing result into the structure as configured in self.outputs
             logger.debug(f"> fn_out: {out}")
             logger.debug(f"> OUTPUTS: {self.outputs}")
             for o in self.outputs:
@@ -826,14 +823,19 @@
                 print("Outputs:\n-------")
                 print(pformat(fout))
             return fout, None
         except Exception as e:
             tb = traceback.format_exc()
             return tb, e
 
+    def forward(self, *args, **kwargs):
+        """This is a convinience method so users can subclass this and implement their own forward method while the
+        underlying processing implemented within __call__ method remain intact."""
+        return self(*args, **kwargs)
+
 
 #
 # Edge: Each connection between two boxes on the UI is called an Edge, it is only a dataclass without any methods.
 #
 
 
 class Edge:
@@ -1061,15 +1063,15 @@
             # need to check if this information is available in the IR buffer, if it is not then this is an error
             ir_value = pre_data.get(req_key, None) or full_ir.get(req_key, {}).get("value", None)
             if ir_value is None:
                 raise ValueError(f"Missing value for {req_key}")
             _data[edge.trg_node_var] = ir_value
 
         # then run the node
-        out, err = node(_data, print_thoughts=print_thoughts)
+        out, err = node.forward(_data, print_thoughts=print_thoughts)
         if err:
             logger.error(f"TRACE: {out}")
             raise err
 
         yield_dict = {}
         for k, v in out.items():
             key = f"{node_id}/{k}"
```

### Comparing `chainfury-1.3.0/chainfury/cli.py` & `chainfury-1.4.0/chainfury/cli.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/client.py` & `chainfury-1.4.0/chainfury/client.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/README.md` & `chainfury-1.4.0/chainfury/components/README.md`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/__init__.py` & `chainfury-1.4.0/chainfury/components/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/ai_actions/__init__.py` & `chainfury-1.4.0/chainfury/components/ai_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/const.py` & `chainfury-1.4.0/chainfury/components/const.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/functional/__init__.py` & `chainfury-1.4.0/chainfury/components/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/nbx/__init__.py` & `chainfury-1.4.0/chainfury/components/nbx/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/openai/__init__.py` & `chainfury-1.4.0/chainfury/components/openai/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
-from typing import Any, List, Union, Dict
+from pydantic import BaseModel
+from typing import Any, List, Union, Dict, Optional
 
 from chainfury import Secret, model_registry, exponential_backoff, Model, UnAuthException
 from chainfury.components.const import Env
 
 
 def openai_completion(
     model: str,
@@ -107,14 +108,44 @@
         fn=openai_completion,
         description="Given a prompt, the model will return one or more predicted completions, and can also return the probabilities of alternative tokens at each position.",
         usage=["usage", "total_tokens"],
     ),
 )
 
 
+class OpenAIChat(BaseModel):
+    """This model is used to chat with the OpenAI API"""
+
+    class Message(BaseModel):
+        role: str
+        content: str
+        name: Optional[str] = None
+        function_call: Optional[Union[str, Dict[str, str]]] = None
+
+    class Function(BaseModel):
+        name: str
+        description: Optional[str] = None
+        parameters: Dict[str, str]
+        function_call: Optional[str] = None
+
+    model: str
+    messages: List[Message]
+    functions: Optional[List[Function]] = None
+    temperature: Optional[float] = 1
+    top_p: Optional[float] = 1
+    n: Optional[int] = 1
+    stream: Optional[bool] = False
+    stop: Optional[Union[str, List[str]]] = None
+    max_tokens: Optional[int] = 2 << 32 - 1
+    presence_penalty: Optional[float] = 0
+    frequency_penalty: Optional[float] = 0
+    logit_bias: Optional[Dict[str, int]] = None
+    user: Optional[str] = None
+
+
 def openai_chat(
     model: str,
     messages: List[Dict[str, str]],
     openai_api_key: Secret = Secret(""),
     temperature: float = 1.0,
     top_p: float = 1.0,
     n: int = 1,
@@ -154,14 +185,19 @@
         Any: The completion(s) generated by the API.
     """
     if not openai_api_key:
         openai_api_key = Secret(Env.OPENAI_TOKEN("")).value
     if not openai_api_key:
         raise Exception("OpenAI API key not found. Please set OPENAI_TOKEN environment variable or pass through function")
 
+    if not len(messages):
+        raise Exception("Messages cannot be empty")
+    if isinstance(messages[0], OpenAIChat.Message):
+        messages = [x.dict(skip_defaults=True) for x in messages]
+
     def _fn():
         r = requests.post(
             "https://api.openai.com/v1/chat/completions",
             headers={
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {openai_api_key}",
             },
```

### Comparing `chainfury-1.3.0/chainfury/components/pinecone_db/__init__.py` & `chainfury-1.4.0/chainfury/components/pinecone_db/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/qdrant/__init__.py` & `chainfury-1.4.0/chainfury/components/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/serper/__init__.py` & `chainfury-1.4.0/chainfury/components/serper/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/components/stability/__init__.py` & `chainfury-1.4.0/chainfury/components/stability/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/types.py` & `chainfury-1.4.0/chainfury/types.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/chainfury/utils.py` & `chainfury-1.4.0/chainfury/utils.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.3.0/pyproject.toml` & `chainfury-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainfury"
-version = "1.3.0"
+version = "1.4.0"
 description = "ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs."
 authors = ["NimbleBox Engineering <engineering@nimblebox.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/ChainFury"
 
 [tool.poetry.dependencies]
```

### Comparing `chainfury-1.3.0/setup.py` & `chainfury-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 entry_points = \
 {'console_scripts': ['cf = chainfury.cli:main',
                      'chainfury = chainfury.cli:main']}
 
 setup_kwargs = {
     'name': 'chainfury',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs.',
     'long_description': '# 🦋 NimbleBox ChainFury\n\n[![linkcheck](https://img.shields.io/badge/Workflow-Passing-darkgreen)](https://github.com/NimbleBoxAI/ChainFury/actions)\n[![Downloads](https://static.pepy.tech/badge/chainfury)](https://pepy.tech/project/chainfury)\n[![linkcheck](https://img.shields.io/badge/Site-🦋ChainFury-lightblue)](https://chainfury.nbox.ai)\n[![License: Apache](https://img.shields.io/badge/License-Apache%20v2.0-red)](https://github.com/NimbleBoxAI/ChainFury/blob/main/LICENSE) \n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/NimbleBoxAI.svg?style=social&label=Follow%20%40NimbleBoxAI)](https://twitter.com/NimbleBoxAI)\n[![](https://dcbadge.vercel.app/api/server/KhF38hrAJ2?compact=true&style=flat)](https://discord.com/invite/KhF38hrAJ2)\n\n🦋 Build complex chat apps using LLMs in 4 clicks ⚡️ [Try it out here](https://chainfury.nbox.ai/). Used in production by [chat.nbox.ai](https://chat.nbox.ai).\n\n# Read the [Docs](https://nimbleboxai.github.io/ChainFury/index.html)\n\nThe documentation page contains all the information on using `chainfury` and `chainfury_server`.\n\n# Installation\n\nThere are two separate packages built into this repository, first is `chainfury` which contains the fury-engine for running\nthe DAGs and `chainfury_server` which contains the self hosted server for the GUI.\n\n``` bash\npip install chainfury\npip install chainfury_server\n\n# to launch the server\npython3 -m chainfury_server\n```\n\n### Run Docker\n\nEasiest way to run the server is to use docker. You can use the following command to run ChainFury:\n\n```bash\ndocker build . -f Dockerfile -t chainfury:latest\ndocker run -p 8000:8000 chainfury:latest\n```\n\nTo pass any env variables you can use the command:\n\n```bash\ndocker run --env ENV_KEY=ENV_VALUE -p 8000:8000 chainfury:latest\n```\n\nCheckout all the:\n- `component` environment variables [here](https://nimbleboxai.github.io/ChainFury/source/chainfury.components.const.html#chainfury.components.const.Env)\n- `chainfury` specific variables [here](https://nimbleboxai.github.io/ChainFury/source/chainfury.utils.html#chainfury.utils.CFEnv)\n- `chainfury_server` specific variables [here](https://nimbleboxai.github.io/ChainFury/cf_server/chainfury_server.commons.config.html#chainfury_server.commons.config.Env)\n\n### From Source\n\nHere\'s a breakdown of folder:\n\n- `chainfury/` contains the chainfury engine\n- `server/` contains the chainfury server\n- `client/` contains the frontend code for the GUI\n- `api_docs/` contains the documentation\n\nTo build the entire system from scratch follow these steps:\n\n```bash\ngit clone https://github.com/NimbleBoxAI/ChainFury\ncd ChainFury\npython3 -m venv venv\nsource venv/bin/activate\n```\n\nYou will need to have `yarn` installed to build the frontend and move it to the correct location on the server\n\n```bash\nsh stories/build_and_copy.sh\n```\n\nOnce the static files are copied we can now proceed to install dependecies:\n\n```bash\npip install setuptools\npip install -e .          # editable install the chainfury\ncd server\npip install -e .          # editable install the chainfury_server\n```\n\nTo start you can now do:\n\n```bash\ncd chainfury_server\npython3 server.py\n```\n\nYou can now visit [localhost:8000](http://localhost:8000/ui/) to see the GUI.\n\n# Contibutions\n\nChainFury is an open-source project used in production. We are open to contributions to the project in the form of features,\ninfrastructure or documentation.\n\n- Our [issues](https://github.com/NimbleBoxAI/ChainFury/issues) page is kept up to date with bugs, improvements, and feature requests.\n\n- If you\'re looking for help with your code, hop onto [GitHub Discussions board](https://github.com/NimbleBoxAI/ChainFury/discussions) or\n[Discord](https://discord.com/invite/KhF38hrAJ2), so that more people can benefit from it.\n\n- **Describing your issue:** Try to provide as many details as possible. What exactly goes wrong? How is it failing?\nIs there an error? "XY doesn\'t work" usually isn\'t that helpful for tracking down problems. Always remember to include\nthe code you ran and if possible, extract only the relevant parts and don\'t just dump your entire script. This will make\nit easier for us to reproduce the error.\n\n- **Sharing long blocks of code or logs:** If you need to include long code, logs or tracebacks, you can wrap them in\n`<details>` and `</details>`. This [collapses the content](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details)\nso it only becomes visible on click, making the issue easier to read and follow.\n\n',
     'author': 'NimbleBox Engineering',
     'author_email': 'engineering@nimblebox.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NimbleBoxAI/ChainFury',
```

### Comparing `chainfury-1.3.0/PKG-INFO` & `chainfury-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainfury
-Version: 1.3.0
+Version: 1.4.0
 Summary: ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs.
 Home-page: https://github.com/NimbleBoxAI/ChainFury
 License: Apache 2.0
 Author: NimbleBox Engineering
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

