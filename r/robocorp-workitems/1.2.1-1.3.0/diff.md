# Comparing `tmp/robocorp_workitems-1.2.1.tar.gz` & `tmp/robocorp_workitems-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_workitems-1.2.1.tar", max compression
+gzip compressed data, was "robocorp_workitems-1.3.0.tar", max compression
```

## Comparing `robocorp_workitems-1.2.1.tar` & `robocorp_workitems-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     5629 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/README.md
--rw-r--r--   0        0        0      893 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4839 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/__init__.py
--rw-r--r--   0        0        0    17330 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/_adapters.py
--rw-r--r--   0        0        0     2380 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/_context.py
--rw-r--r--   0        0        0      958 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/_exceptions.py
--rw-r--r--   0        0        0     6520 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/_requests.py
--rw-r--r--   0        0        0     1613 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/_types.py
--rw-r--r--   0        0        0     2401 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/_utils.py
--rw-r--r--   0        0        0     8789 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/_workitem.py
--rw-r--r--   0        0        0        0 2023-06-28 14:28:15.623515 robocorp_workitems-1.2.1/src/robocorp/workitems/py.typed
--rw-r--r--   0        0        0     6452 1970-01-01 00:00:00.000000 robocorp_workitems-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2648 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/docs/README.md
+-rw-r--r--   0        0        0      893 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4868 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/__init__.py
+-rw-r--r--   0        0        0     2792 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_adapters/__init__.py
+-rw-r--r--   0        0        0     1831 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_adapters/_base.py
+-rw-r--r--   0        0        0     8119 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_adapters/_file.py
+-rw-r--r--   0        0        0     8966 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_adapters/_robocorp.py
+-rw-r--r--   0        0        0     1423 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_context.py
+-rw-r--r--   0        0        0      958 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_exceptions.py
+-rw-r--r--   0        0        0     6520 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_requests.py
+-rw-r--r--   0        0        0     1613 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_types.py
+-rw-r--r--   0        0        0     2401 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_utils.py
+-rw-r--r--   0        0        0    16208 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/_workitem.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:48:37.315022 robocorp_workitems-1.3.0/src/robocorp/workitems/py.typed
+-rw-r--r--   0        0        0     3471 1970-01-01 00:00:00.000000 robocorp_workitems-1.3.0/PKG-INFO
```

### Comparing `robocorp_workitems-1.2.1/pyproject.toml` & `robocorp_workitems-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-workitems"
-version = "1.2.1"
+version = "1.3.0"
 description = "Robocorp Work Items library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
     "Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
```

### Comparing `robocorp_workitems-1.2.1/src/robocorp/workitems/__init__.py` & `robocorp_workitems-1.3.0/src/robocorp/workitems/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     BusinessException,
     EmptyQueue,
     to_exception_type,
 )
 from ._types import ExceptionType, JSONType, State
 from ._workitem import Input, Output
 
-__version__ = "1.2.1"
+__version__ = "1.3.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 LOGGER = logging.getLogger(__name__)
 
 
 @task_cache
 def __ctx():
@@ -171,20 +171,22 @@
         return item
 
 
 inputs = Inputs()
 outputs = Outputs()
 
 __all__ = [
-    "BaseAdapter",
-    "FileAdapter",
-    "RobocorpAdapter",
+    "inputs",
+    "outputs",
+    "Inputs",
+    "Outputs",
+    "Input",
+    "Output",
+    "State",
+    "ExceptionType",
     "EmptyQueue",
     "BusinessException",
     "ApplicationException",
-    "State",
-    "ExceptionType",
-    "Input",
-    "Output",
-    "inputs",
-    "outputs",
+    "RobocorpAdapter",
+    "FileAdapter",
+    "BaseAdapter",
 ]
```

### Comparing `robocorp_workitems-1.2.1/src/robocorp/workitems/_adapters.py` & `robocorp_workitems-1.3.0/src/robocorp/workitems/_workitem.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,489 +1,536 @@
+import fnmatch
 import json
 import logging
 import os
-from abc import ABC, abstractmethod
+import warnings
+from glob import glob
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Optional, Union
 
-from ._exceptions import EmptyQueue
-from ._requests import Requests
-from ._types import State
-from ._utils import JSONType, json_dumps, required_env, resolve_path, url_join
+from ._adapters import BaseAdapter
+from ._exceptions import ApplicationException, BusinessException, to_exception_type
+from ._types import Email, ExceptionType, JSONType, PathType, State
+from ._utils import truncate
 
-UNDEFINED = object()  # Undefined default value
-ENCODING = "utf-8"
 LOGGER = logging.getLogger(__name__)
 
 
-class BaseAdapter(ABC):
-    """Abstract base class for work item adapters."""
-
-    @abstractmethod
-    def reserve_input(self) -> str:
-        """Get next work item ID from the input queue and reserve it."""
-        raise NotImplementedError
-
-    @abstractmethod
-    def release_input(
-        self, item_id: str, state: State, exception: Optional[dict] = None
+class WorkItem:
+    def __init__(
+        self,
+        adapter: BaseAdapter,
+        item_id: Optional[str] = None,
+        parent_id: Optional[str] = None,
     ):
-        """Release the lastly retrieved input work item and set state."""
-        raise NotImplementedError
+        #: API client adpater
+        self._adapter = adapter
+        #: Current work item ID
+        self._id: Optional[str] = item_id
+        #: Parent work item ID (output only)
+        self._parent_id: Optional[str] = parent_id
+        #: Work item payload (JSON)
+        self._payload: JSONType = None
+        #: Current work item files
+        self._files: list[str] = []
+        #: Files queued for upload
+        self._files_to_add: dict[str, Path] = {}
+        #: Files queued for removal
+        self._files_to_remove: set[str] = set()
+        #: Flag for saved/dirty state
+        self._saved = False
 
-    @abstractmethod
-    def create_output(self, parent_id: str, payload: Optional[JSONType] = None) -> str:
-        """Create new output for work item, and return created ID."""
-        raise NotImplementedError
-
-    @abstractmethod
-    def load_payload(self, item_id: str) -> JSONType:
-        """Load JSON payload from work item."""
-        raise NotImplementedError
-
-    @abstractmethod
-    def save_payload(self, item_id: str, payload: JSONType):
-        """Save JSON payload to work item."""
-        raise NotImplementedError
-
-    @abstractmethod
-    def list_files(self, item_id: str) -> List[str]:
-        """List attached files in work item."""
-        raise NotImplementedError
-
-    @abstractmethod
-    def get_file(self, item_id: str, name: str) -> bytes:
-        """Read file's contents from work item."""
-        raise NotImplementedError
-
-    @abstractmethod
-    def add_file(self, item_id: str, name: str, *, original_name: str, content: bytes):
-        """Attach file to work item."""
-        raise NotImplementedError
-
-    @abstractmethod
-    def remove_file(self, item_id: str, name: str):
-        """Remove attached file from work item."""
-        raise NotImplementedError
-
-
-class RobocorpAdapter(BaseAdapter):
-    """Adapter for saving/loading work items from Robocorp Control Room.
-
-    Required environment variables:
-
-    * RC_API_WORKITEM_HOST:     Work item API hostname
-    * RC_API_WORKITEM_TOKEN:    Work item API access token
-
-    * RC_API_PROCESS_HOST:      Process API hostname
-    * RC_API_PROCESS_TOKEN:     Process API access token
-
-    * RC_WORKSPACE_ID:          Control room workspace ID
-    * RC_PROCESS_ID:            Control room process ID
-    * RC_PROCESS_RUN_ID:        Control room process run ID
-    * RC_ROBOT_RUN_ID:          Control room robot run ID
+    @property
+    def id(self) -> Optional[str]:
+        """Current ID for work item."""
+        return self._id
 
-    * RC_WORKITEM_ID:           Control room work item ID (input)
-    """
+    @property
+    def parent_id(self) -> Optional[str]:
+        """Current parent work item ID (output only)."""
+        return self._parent_id
 
-    def __init__(self) -> None:
-        # IDs identifying the current robot run and its input.
-        self._workspace_id: str = required_env("RC_WORKSPACE_ID")
-        self._process_run_id: str = required_env("RC_PROCESS_RUN_ID")
-        self._step_run_id: str = required_env("RC_ACTIVITY_RUN_ID")
-        self._initial_item_id: Optional[str] = required_env("RC_WORKITEM_ID")
-
-        self._workitem_requests = self._init_workitem_requests()
-        self._process_requests = self._init_process_requests()
-
-    def _init_workitem_requests(self) -> Requests:
-        # Endpoint for old work items API.
-        workitem_host = required_env("RC_API_WORKITEM_HOST")
-        workitem_token = required_env("RC_API_WORKITEM_TOKEN")
-        route_prefix = (
-            url_join(
-                workitem_host, "json-v1", "workspaces", self._workspace_id, "workitems"
-            )
-            + "/"
-        )
-        default_headers = {
-            "Authorization": f"Bearer {workitem_token}",
-            "Content-Type": "application/json",
-        }
-        LOGGER.info("Work item API route prefix: %s", route_prefix)
-        return Requests(route_prefix, default_headers=default_headers)
+    @property
+    def payload(self) -> JSONType:
+        """Current JSON payload."""
+        return self._payload
+
+    @payload.setter
+    def payload(self, value: JSONType):
+        self._saved = False
+        self._payload = value
+
+    @property
+    def files(self) -> list[str]:
+        """Names of attached files."""
+        return self._files
 
-    def _init_process_requests(self) -> Requests:
-        # Endpoint for the new process API.
-        process_host = required_env("RC_API_PROCESS_HOST")
-        process_token = required_env("RC_API_PROCESS_TOKEN")
-        process_id = required_env("RC_PROCESS_ID")
-        route_prefix = (
-            url_join(
-                process_host,
-                "process-v1",
-                "workspaces",
-                self._workspace_id,
-                "processes",
-                process_id,
+    @property
+    def saved(self) -> bool:
+        """Is the current item saved."""
+        return self._saved
+
+    def load(self) -> None:
+        """Load work item payload and file listing from Control Room."""
+        if self.id is None:
+            raise RuntimeError("Unable to load unsaved item")
+
+        self._payload = self._adapter.load_payload(self.id)
+        self._files = self._adapter.list_files(self.id)
+        self._saved = True
+
+    def save(self):
+        """Save the current work item.
+
+        Updates the work item payload and adds/removes all pending files.
+        """
+        if self.id is not None:
+            self._adapter.save_payload(self.id, payload=self.payload)
+        elif self.parent_id is not None:
+            self._id = self._adapter.create_output(
+                self.parent_id,
+                payload=self.payload,
             )
-            + "/"
-        )
-        default_headers = {
-            "Authorization": f"Bearer {process_token}",
-            "Content-Type": "application/json",
-        }
-        LOGGER.info("Process API route prefix: %s", route_prefix)
-        return Requests(route_prefix, default_headers=default_headers)
+        else:
+            raise RuntimeError("Invalid work item state (no id or parent_id)")
 
-    def _pop_item(self):
-        # Get the next input work item from the cloud queue.
-        url = url_join(
-            "runs",
-            self._process_run_id,
-            "robotRuns",
-            self._step_run_id,
-            "reserve-next-work-item",
-        )
-        LOGGER.info("Reserving new input work item from: %s", url)
-        response = self._process_requests.post(url)
-        return response.json()["workItemId"]
-
-    def reserve_input(self) -> str:
-        if self._initial_item_id:
-            item_id = self._initial_item_id
-            self._initial_item_id = None
-            return item_id
-
-        item_id = self._pop_item()
-        if not item_id:
-            raise EmptyQueue("No work items in the input queue")
-        return item_id
+        assert self.id is not None
 
-    def release_input(
-        self, item_id: str, state: State, exception: Optional[dict] = None
-    ):
-        # Release the current input work item in the cloud queue.
-        url = url_join(
-            "runs",
-            self._process_run_id,
-            "robotRuns",
-            self._step_run_id,
-            "release-work-item",
-        )
-        body: dict[str, Any] = {"workItemId": item_id, "state": state.value}
-        if exception:
-            for key, value in list(exception.items()):
-                # All values are (and should be) strings (if not `None`).
-                value = value.strip() if value else value
-                if value:
-                    exception[key] = value  # keep the stripped string value
-                else:
-                    # Exclude `None` & empty string values.
-                    del exception[key]
-            body["exception"] = exception
-
-        log_func = LOGGER.error if state == State.FAILED else LOGGER.info
-        log_func(
-            "Releasing %s input work item %r into %r with exception: %s",
-            state.value,
-            item_id,
-            url,
-            exception,
-        )
-        self._process_requests.post(url, json=body)
+        for name, path in self._files_to_add.items():
+            with open(path, "rb") as fd:
+                self._adapter.add_file(
+                    item_id=self.id,
+                    name=name,
+                    content=fd.read(),
+                )
 
-    def create_output(self, parent_id: str, payload: Optional[JSONType] = None) -> str:
-        # Putting "output" for the current input work item identified by `parent_id`.
-        url = url_join("work-items", parent_id, "output")
-        body = {"payload": payload}
-
-        LOGGER.info("Creating output item: %s", url)
-        response = self._process_requests.post(url, json=body)
-        return response.json()["id"]
-
-    def load_payload(self, item_id: str) -> JSONType:
-        url = url_join(item_id, "data")
-
-        def handle_error(resp):
-            # NOTE: The API might return 404 if no payload is attached to the work
-            # item.
-            if not (resp.ok or resp.status_code == 404):
-                self._workitem_requests.handle_error(resp)
-
-        LOGGER.info("Loading work item payload from: %s", url)
-        response = self._workitem_requests.get(url, _handle_error=handle_error)
-        return response.json() if response.ok else {}
-
-    def save_payload(self, item_id: str, payload: JSONType):
-        url = url_join(item_id, "data")
-
-        LOGGER.info("Saving work item payload to: %s", url)
-        self._workitem_requests.put(url, json=payload)
-
-    def list_files(self, item_id: str) -> List[str]:
-        url = url_join(item_id, "files")
-
-        LOGGER.info("Listing work item files at: %s", url)
-        response = self._workitem_requests.get(url)
-
-        return [item["fileName"] for item in response.json()]
-
-    def get_file(self, item_id: str, name: str) -> bytes:
-        # Robocorp API returns URL for S3 download.
-        file_id = self.file_id(item_id, name)
-        url = url_join(item_id, "files", file_id)
-
-        LOGGER.info("Downloading work item file at: %s", url)
-        response = self._workitem_requests.get(url)
-        file_url = response.json()["url"]
-
-        # Perform the actual file download.
-        response = self._workitem_requests.get(
-            file_url,
-            _handle_error=lambda resp: resp.raise_for_status(),
-            _sensitive=True,
-            headers={},
-        )
-        return response.content
+        for name in self._files_to_remove:
+            self._adapter.remove_file(self.id, name)
 
-    def add_file(self, item_id: str, name: str, *, original_name: str, content: bytes):
-        # Note that here the `original_name` is useless here. (used with `FileAdapter`
-        #   only)
-        del original_name
-
-        # Robocorp API returns pre-signed POST details for S3 upload.
-        url = url_join(item_id, "files")
-        body = {"fileName": str(name), "fileSize": len(content)}
-        LOGGER.info(
-            "Adding work item file into: %s (name: %s, size: %d)",
-            url,
-            body["fileName"],
-            body["fileSize"],
+        self._files = list(
+            set(self._files) - set(self._files_to_remove) | set(self._files_to_add)
         )
-        response = self._workitem_requests.post(url, json=body)
-        data = response.json()
+        self._files_to_add = {}
+        self._files_to_remove = set()
 
-        # Perform the actual file upload.
-        url = data["url"]
-        fields = data["fields"]
-        files = {"file": (name, content)}
-        self._workitem_requests.post(
-            url,
-            _handle_error=lambda resp: resp.raise_for_status(),
-            _sensitive=True,
-            headers={},
-            data=fields,
-            files=files,
-        )
+        self._saved = True
+
+    def add_file(self, path: Union[Path, str], name: Optional[str] = None) -> Path:
+        """Attach a file from the local machine to the work item.
+
+        Note: Files are not uploaded until the item is saved.
+
+        Args:
+            path: Path to attached file
+            name: Custom name for file in work item
+
+        Returns:
+            Resolved path to added file
+        """
+        path = Path(path).resolve()
+        name = name or path.name
+
+        if not path.is_file():
+            raise FileNotFoundError(f"Not a valid file: {path}")
+
+        if name in self._files:
+            LOGGER.warning('File with name "%s" already exists', name)
+
+        self._saved = False
+        self._files_to_add[name] = path
+        LOGGER.info("Added file: %s", name)
+
+        return path
+
+    def add_files(self, pattern: str) -> list[Path]:
+        """Attach files from the local machine to the work item that
+        match the given pattern.
+
+        Note: Files are not uploaded until the item is saved.
+
+        Args:
+            pattern: Glob pattern for attached file paths
+
+        Returns:
+            List of added paths
+        """
+        matches = glob(pattern, recursive=False)
+
+        paths = []
+        for match in matches:
+            path = self.add_file(match)
+            paths.append(path)
+
+        LOGGER.info("Added %d file(s)", len(paths))
+        return paths
+
+    def remove_file(self, name: str, missing_ok: bool = False):
+        """Remove attached file with given name.
+
+        Note: Files are not removed from Control Room until the item is saved.
 
-    def remove_file(self, item_id: str, name: str):
-        file_id = self.file_id(item_id, name)
-        url = url_join(item_id, "files", file_id)
-        self._workitem_requests.delete(url)
+        Args:
+            name: Name of file
+            missing_ok: Do nothing if given file does not exist
+        """
+        if name not in self._files:
+            if missing_ok:
+                return
+            else:
+                raise FileNotFoundError(f"No such file in work item: {name}")
 
-    def file_id(self, item_id: str, name: str) -> str:
-        url = url_join(item_id, "files")
-        response = self._workitem_requests.get(url)
+        LOGGER.info("Removing file: %s", name)
+        self._files_to_remove.add(name)
+        self._saved = False
 
-        files = response.json()
-        if not files:
-            raise FileNotFoundError("No files in work item")
+    def remove_files(self, pattern: str) -> list[str]:
+        """Remove attached files that match the given pattern.
 
-        matches = [item for item in files if item["fileName"] == name]
-        if not matches:
-            names = ", ".join(item["fileName"] for item in files)
-            raise FileNotFoundError(f"File with name '{name}' not in: {names}")
+        Note: Files are not removed from Control Room until the item is saved.
 
-        # Duplicate filenames should never exist,
-        # but use last item just in case
-        return matches[-1]["fileId"]
+        Args:
+            pattern: Glob pattern for file names
 
+        Returns:
+            List of matched names
+        """
+        names = []
+        for name in self._files:
+            if fnmatch.fnmatch(name, pattern):
+                self.remove_file(name)
+                names.append(name)
 
-class FileAdapter(BaseAdapter):
-    """Adapter for simulating work item input queues.
+        LOGGER.info("Removing %d file(s)", len(names))
+        return names
 
-    Reads inputs from the given database file, and writes
-    all created output items into an adjacent file
-    with the suffix ``<filename>.output.json``. If the output path is provided by an
-    env var explicitly, then the file will be saved with the provided path and name.
 
-    Reads and writes all work item files from/to the same parent
-    folder as the given input database.
+class Input(WorkItem):
+    """Container for an input work item.
 
-    Optional environment variables:
+    An input work item can contain arbitrary JSON data in the `payload` section,
+    and optionally attached files that are stored in Control Room.
 
-    * RPA_INPUT_WORKITEM_PATH:  Path to work items input database file
-    * RPA_OUTPUT_WORKITEM_PATH:  Path to work items output database file
+    Each step run of a process in Control Room has at least one input
+    work item associated with it, but the step's input queue can have
+    multiple input items in it.
+
+    There can only be one input work item reserved at a time. To reserve
+    the next item, the current item needs to be released as either
+    passed or failed.
     """
 
-    def __init__(self) -> None:
-        self._input_path: Optional[Path] = None
-        self._output_path: Optional[Path] = None
-
-        self._inputs: List[Dict[str, Any]] = self.load_database()
-        self._outputs: List[Dict[str, Any]] = []
-        self._index: int = 0
+    def __init__(self, adapter: BaseAdapter, item_id: str):
+        super().__init__(adapter, item_id=item_id)
+        self._state: Optional[State] = None
+        self._outputs: list[Output] = []
+        self._saved = True
+
+    def __repr__(self):
+        payload = truncate(json.dumps(self._payload), 64)
+        return (
+            "Input["
+            + f"id={self.id},"
+            + f"payload={payload},"
+            + f"files={self.files},"
+            + f"state={self.state},"
+            + f"saved={self.saved}]"
+        )
 
-    @property
-    def input_path(self) -> Path:
-        if self._input_path is None:
-            path = os.getenv("RC_WORKITEM_INPUT_PATH") or os.getenv(
-                "RPA_INPUT_WORKITEM_PATH"
-            )
-            if not path:
-                raise RuntimeError(
-                    "No input path defined, "
-                    + "set environment variable 'RC_WORKITEM_INPUT_PATH'"
-                )
+    def __enter__(self):
+        return self
 
-            self._input_path = resolve_path(path)
+    def __exit__(self, exc_type, exc_value, traceback):
+        if self.released:
+            return False
 
-        return self._input_path
+        if exc_type is None:
+            self.done()
+            return False
+
+        exception_type = to_exception_type(exc_type)
+        code = getattr(exc_value, "code", None)
+        message = getattr(exc_value, "message", str(exc_value))
+
+        self.fail(exception_type=exception_type, code=code, message=message)
+
+        # Do not propagate library-specific exceptions
+        return exc_type in (ApplicationException, BusinessException)
 
     @property
-    def output_path(self) -> Path:
-        if self._output_path is None:
-            path = os.getenv("RC_WORKITEM_OUTPUT_PATH") or os.getenv(
-                "RPA_OUTPUT_WORKITEM_PATH"
-            )
-            if not path:
-                raise RuntimeError(
-                    "No output path defined, "
-                    + "set environment variable 'RC_WORKITEM_OUTPUT_PATH'"
-                )
+    def state(self) -> Optional[State]:
+        """Current release state."""
+        return self._state
 
-            self._output_path = resolve_path(path)
-            self._output_path.parent.mkdir(parents=True, exist_ok=True)
+    @property
+    def released(self) -> bool:
+        """Is the current item released."""
+        return self._state is not None
 
-        return self._output_path
+    @property
+    def outputs(self) -> list["Output"]:
+        """Child output work items."""
+        return list(self._outputs)
+
+    def save(self):
+        """Save the current input work item.
+
+        Updates the work item payload and adds/removes all pending files.
+
+        **Note:** Modifying input work items is not recommended, as it will
+         make traceability after execution difficult, and potentially make
+         the process behave in unexpected ways.
+        """
+        super().save()
+
+    def email(
+        self,
+        html=True,
+        encoding="utf-8",
+        ignore_errors=False,
+    ) -> Optional[Email]:
+        """Parse an email attachment from the work item.
+
+        Args:
+            html: Parse the HTML content into the `html` attribute
+            encoding: Text encoding of the email
+            ignore_errors: Ignore possible parsing errors from Control Room
+
+        Returns:
+            An email container with metadata and content
+
+        Raises:
+            ValueError: No email attached or content is malformed
+        """
+        assert self.id is not None
+
+        email = self._parse_email()
+
+        if email.errors and not ignore_errors:
+            raise ValueError("\n".join(email.errors))
+
+        if html and "__mail.html" in self._files:
+            content = self._adapter.get_file(self.id, "__mail.html")
+            email.html = content.decode(encoding)
+
+        return email
+
+    def _parse_email(self) -> Email:
+        if not isinstance(self._payload, dict):
+            typename = type(self._payload).__name__
+            raise ValueError(f"Expected 'dict' payload, was '{typename}'")
 
-    def _get_item(self, item_id: str) -> Tuple[str, Dict[str, Any]]:
-        # The work item ID is analogue to inputs/outputs list queues index.
-        idx = int(item_id)
-        if idx < len(self._inputs):
-            return "input", self._inputs[idx]
-
-        if idx < (len(self._inputs) + len(self._outputs)):
-            return "output", self._outputs[idx - len(self._inputs)]
-
-        raise ValueError(f"Unknown work item ID: {item_id}")
-
-    def _save_to_disk(self, source: str) -> None:
-        if source == "input":
-            path = self.input_path
-            data = self._inputs
+        def _try_parse(fields):
+            try:
+                email = Email.from_dict(fields)  # type: ignore
+                return email
+            except KeyError as err:
+                raise ValueError(f"Missing key in 'email' field: {err}") from err
+            except Exception as err:
+                raise ValueError(f"Malformed 'email' field: {err}") from err
+
+        # Email was successfully parsed by Control Room
+        if "email" in self._payload:
+            fields = self._payload["email"]
+            email = _try_parse(fields)
+            return email
+
+        # Email parsing by Control Room failed (payload or attachments too big)
+        if "failedEmail" in self._payload:
+            fields = self._payload["failedEmail"]
+            email = _try_parse(fields)
+            email.errors = self._parse_email_errors(self._payload)
+            return email
+
+        # No email fields in payload
+        raise ValueError("No email in work item")
+
+    def _parse_email_errors(self, payload: dict[str, Any]) -> list[str]:
+        errors = payload.get("errors", [])
+        if not isinstance(errors, list):
+            LOGGER.warning("Expected 'errors' as 'list', was '%s'", type(errors))
+            return []
+
+        result = []
+        for err in errors:
+            msg = err["message"]
+            if files := err.get("files"):
+                names = ", ".join(f["name"] for f in files)
+                msg += f" ({names})"
+            result.append(msg)
+
+        return result
+
+    def get_file(self, name: str, path: Optional[PathType] = None) -> Path:
+        """Download file with given name.
+
+        If a `path` is not defined, uses the Robot root or current working
+        directory.
+
+        Args:
+            name: Name of file
+            path: Path to created file
+
+        Returns:
+            Path to created file
+        """
+        assert self.id is not None
+
+        if name not in self.files:
+            raise FileNotFoundError(f"No file with name: {name}")
+
+        if path is None:
+            root = os.getenv("ROBOT_ROOT", "")
+            path = Path(root) / name
         else:
-            path = self.output_path
-            data = self._outputs
+            path = Path(path)
 
-        with open(path, "w", encoding=ENCODING) as fd:
-            fd.write(json_dumps(data, indent=4))
+        content = self._adapter.get_file(self.id, name)
+        with open(path, "wb") as fd:
+            fd.write(content)
 
-        LOGGER.info("Saved into %s file: %s", source, path)
+        return path.absolute()
 
-    def reserve_input(self) -> str:
-        if self._index >= len(self._inputs):
-            raise EmptyQueue("No work items in the input queue")
+    def get_files(self, pattern: str, path: Optional[Path] = None) -> list[Path]:
+        """Download all files attached to this work item that match
+        the given pattern.
+
+        If a `path` is not defined, uses the Robot root or current working
+        directory.
+
+        Args:
+            pattern: Glob pattern for file names
+            path: Directory to store files in
+
+        Returns:
+            List of created file paths
+        """
+        assert self.id is not None
+
+        if path is None:
+            root = os.getenv("ROBOT_ROOT", "")
+            path = Path(root)
+        else:
+            path = Path(path)
 
-        try:
-            return str(self._index)
-        finally:
-            self._index += 1
+        path.mkdir(parents=True, exist_ok=True)
 
-    def release_input(
-        self, item_id: str, state: State, exception: Optional[dict] = None
-    ):
-        # Nothing happens for now on releasing local dev input Work Items.
-        log_func = LOGGER.error if state == State.FAILED else LOGGER.info
-        log_func(
-            "Releasing item %r with %s state and exception: %s",
-            item_id,
-            state.value,
-            exception,
-        )
+        paths = []
+        for name in self.files:
+            if not fnmatch.fnmatch(name, pattern):
+                continue
+
+            filepath = (path / name).absolute()
+            paths.append(filepath)
 
-    def create_output(self, _: str, payload: Optional[JSONType] = None) -> str:
-        # Note that the `parent_id` is not used during local development.
-        item: Dict[str, Any] = {"payload": payload, "files": {}}
+            content = self._adapter.get_file(self.id, name)
+            with open(filepath, "wb") as fd:
+                fd.write(content)
+
+        return paths
+
+    def create_output(self) -> "Output":
+        """Create an output work item that is a child of this item."""
+        assert self.id is not None
+
+        item = Output(adapter=self._adapter, parent_id=self.id)
         self._outputs.append(item)
+        return item
 
-        self._save_to_disk("output")
-        item_id = str(len(self._inputs) + len(self._outputs) - 1)
-        return item_id
-
-    def load_payload(self, item_id: str) -> JSONType:
-        _, item = self._get_item(item_id)
-        return item.get("payload", {})
-
-    def save_payload(self, item_id: str, payload: JSONType):
-        source, item = self._get_item(item_id)
-        item["payload"] = payload
-        self._save_to_disk(source)
-
-    def list_files(self, item_id: str) -> List[str]:
-        _, item = self._get_item(item_id)
-        files = item.get("files", {})
-        return list(files.keys())
-
-    def get_file(self, item_id: str, name: str) -> bytes:
-        source, item = self._get_item(item_id)
-        files = item.get("files", {})
-
-        path = files[name]
-        if not Path(path).is_absolute():
-            parent = (
-                self.input_path.parent if source == "input" else self.output_path.parent
-            )
-            path = parent / path
+    def done(self):
+        """Mark this work item as done, and release it."""
+        assert self.id is not None
+
+        if self.state is not None:
+            raise RuntimeError("Work item already released")
+
+        state = State.DONE
+        self._adapter.release_input(self.id, state, exception=None)
+        self._state = state
+
+    def fail(
+        self,
+        exception_type: Union[ExceptionType, str] = ExceptionType.APPLICATION,
+        code: Optional[str] = None,
+        message: Optional[str] = None,
+    ):
+        """Mark this work item as failed, and release it.
 
-        with open(path, "rb") as infile:
-            return infile.read()
+        Args:
+            exception_type: Type of failure (APPLICATION or BUSINESS)
+            code: Custom error code for the failure
+            message: Human-readable error message
+        """
+        assert self.id is not None
+
+        if self.state is not None:
+            raise RuntimeError("Work item already released")
+
+        type_ = (
+            exception_type
+            if isinstance(exception_type, ExceptionType)
+            else ExceptionType(exception_type.upper())
+        )
 
-    def add_file(self, item_id: str, name: str, *, original_name: str, content: bytes):
-        source, item = self._get_item(item_id)
-        files = item.setdefault("files", {})
+        exception = {
+            "type": type_.value,
+            "code": code,
+            "message": message,
+        }
 
-        parent = (
-            self.input_path.parent if source == "input" else self.output_path.parent
+        state = State.FAILED
+        self._adapter.release_input(self.id, state, exception=exception)
+        self._state = state
+
+    # Backwards compatibility
+    def download_file(self, name: str, path: Optional[PathType] = None) -> Path:
+        """Deprecated method, use `get_file` instead.
+
+        lazydocs: ignore
+        """
+        warnings.warn(
+            "download_file() will be removed in version 2.x, use get_file()",
+            DeprecationWarning,
         )
-        path = parent / original_name  # the file on disk will keep its original name
-        with open(path, "wb") as fd:
-            fd.write(content)
-        LOGGER.info("Created file: %s", path)
-        files[name] = original_name  # file path relative to the work item
+        return self.get_file(name, path)
 
-        self._save_to_disk(source)
+    def download_files(self, pattern: str, path: Optional[Path] = None) -> list[Path]:
+        """Deprecated method, use `get_files` instead.
 
-    def remove_file(self, item_id: str, name: str):
-        source, item = self._get_item(item_id)
-        files = item.get("files", {})
+        lazydocs: ignore
+        """
+        warnings.warn(
+            "download_files() will be removed in version 2.x, use get_files()",
+            DeprecationWarning,
+        )
+        return self.get_files(pattern, path)
 
-        path = files[name]
-        LOGGER.info("Would remove file: %s", path)
-        # Note that the file doesn't get removed from disk as well.
-        del files[name]
 
-        self._save_to_disk(source)
+class Output(WorkItem):
+    """Container for an output work item.
 
-    def load_database(self) -> List:
-        try:
-            try:
-                with open(self.input_path, "r", encoding=ENCODING) as infile:
-                    data = json.load(infile)
-            except (TypeError, FileNotFoundError):
-                LOGGER.warning("No input work items file found: %s", self.input_path)
-                data = []
-
-            if not isinstance(data, list):
-                raise ValueError("Expected list of items")
-
-            if any(not isinstance(d, dict) for d in data):
-                raise ValueError("Items should be dictionaries")
-
-            if len(data) == 0:
-                data.append({"payload": {}})
-
-            return data
-        except Exception as exc:
-            LOGGER.exception("Invalid work items file because of: %s", exc)
-            return [{"payload": {}}]
+    Created output items are added to an output queue, and released
+    to the next step of a process when the current run ends.
+
+    Note: An output item always has an input item as a parent,
+    which is used for traceability in a work item's history.
+    """
+
+    def __init__(self, adapter: BaseAdapter, parent_id: str):
+        super().__init__(adapter, parent_id=parent_id)
+
+    def __repr__(self):
+        payload = truncate(str(self.payload), 64)
+        return (
+            "Output["
+            + f"id={self.id},"
+            + f"parent={self.parent_id},"
+            + f"payload={payload},"
+            + f"files={self.files},"
+            + f"saved={self.saved}]"
+        )
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        if exc_type is not None:
+            self.save()
```

### Comparing `robocorp_workitems-1.2.1/src/robocorp/workitems/_exceptions.py` & `robocorp_workitems-1.3.0/src/robocorp/workitems/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.2.1/src/robocorp/workitems/_requests.py` & `robocorp_workitems-1.3.0/src/robocorp/workitems/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.2.1/src/robocorp/workitems/_types.py` & `robocorp_workitems-1.3.0/src/robocorp/workitems/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.2.1/src/robocorp/workitems/_utils.py` & `robocorp_workitems-1.3.0/src/robocorp/workitems/_utils.py`

 * *Files identical despite different names*

