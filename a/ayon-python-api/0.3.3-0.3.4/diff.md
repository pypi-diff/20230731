# Comparing `tmp/ayon-python-api-0.3.3.tar.gz` & `tmp/ayon-python-api-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.3.3.tar", last modified: Fri Jul 21 13:39:19 2023, max compression
+gzip compressed data, was "ayon-python-api-0.3.4.tar", last modified: Mon Jul 31 12:28:44 2023, max compression
```

## Comparing `ayon-python-api-0.3.3.tar` & `ayon-python-api-0.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30310 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)   192441 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:28:44.663769 ayon-python-api-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-07-31 12:28:44.663769 ayon-python-api-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:28:44.663769 ayon-python-api-0.3.4/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30310 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80376 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193221 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:28:44.663769 ayon-python-api-0.3.4/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-07-31 12:28:44.000000 ayon-python-api-0.3.4/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-31 12:28:44.000000 ayon-python-api-0.3.4/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:28:44.000000 ayon-python-api-0.3.4/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 12:28:44.000000 ayon-python-api-0.3.4/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 12:28:44.000000 ayon-python-api-0.3.4/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:28:44.663769 ayon-python-api-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-31 12:28:38.000000 ayon-python-api-0.3.4/setup.py
```

### Comparing `ayon-python-api-0.3.3/LICENSE` & `ayon-python-api-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/PKG-INFO` & `ayon-python-api-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -269,15 +269,14 @@
 - Add folder and task changes to operations
 - Enhance entity hub
   - Missing docstrings in EntityHub -> especially entity arguments are missing
   - Better order of arguments for entity classes
     - Move entity hub to first place
     - Skip those which are invalid for the entity and fake it for base or remove it from base
   - Entity hub should use operations session to do changes
-  - Entity hub could also handle 'subset', 'version' and 'representation' entities
-  - Missing 'statuses' on project
+  - Entity hub could also handle 'product', 'version' and 'representation' entities
   - Missing 'status' on folders
   - Missing assignees on tasks
   - Pass docstrings and arguments definitions from `ServerAPI` methods to global functions
 - Split `ServerAPI` into smaller chunks (somehow), the class has 4k+ lines of code
 - Add .pyi stub for ServerAPI 
 - Missing websockets connection
```

### Comparing `ayon-python-api-0.3.3/README.md` & `ayon-python-api-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 - Add folder and task changes to operations
 - Enhance entity hub
   - Missing docstrings in EntityHub -> especially entity arguments are missing
   - Better order of arguments for entity classes
     - Move entity hub to first place
     - Skip those which are invalid for the entity and fake it for base or remove it from base
   - Entity hub should use operations session to do changes
-  - Entity hub could also handle 'subset', 'version' and 'representation' entities
-  - Missing 'statuses' on project
+  - Entity hub could also handle 'product', 'version' and 'representation' entities
   - Missing 'status' on folders
   - Missing assignees on tasks
   - Pass docstrings and arguments definitions from `ServerAPI` methods to global functions
 - Split `ServerAPI` into smaller chunks (somehow), the class has 4k+ lines of code
 - Add .pyi stub for ServerAPI 
 - Missing websockets connection
```

### Comparing `ayon-python-api-0.3.3/ayon_api/__init__.py` & `ayon-python-api-0.3.4/ayon_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/_api.py` & `ayon-python-api-0.3.4/ayon_api/_api.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/constants.py` & `ayon-python-api-0.3.4/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/entity_hub.py` & `ayon-python-api-0.3.4/ayon_api/entity_hub.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import re
 import copy
 import collections
 from abc import ABCMeta, abstractmethod
 
 import six
 from ._api import get_server_api_connection
-from .utils import create_entity_id, convert_entity_id
+from .utils import create_entity_id, convert_entity_id, slugify_string
 
 UNKNOWN_VALUE = object()
 PROJECT_PARENT_ID = object()
 _NOT_SET = object()
 
 
 class EntityHub(object):
@@ -541,14 +542,15 @@
         self._project_entity = ProjectEntity(
             project["code"],
             parent_id=PROJECT_PARENT_ID,
             entity_id=project["name"],
             library=project["library"],
             folder_types=project["folderTypes"],
             task_types=project["taskTypes"],
+            statuses=project["statuses"],
             name=project["name"],
             attribs=project["ownAttrib"],
             data=project["data"],
             active=project["active"],
             entity_hub=self
         )
         self.add_entity(self._project_entity)
@@ -771,16 +773,15 @@
 
         project_changes = self.project_entity.changes
         if project_changes:
             response = self._connection.patch(
                 "projects/{}".format(self.project_name),
                 **project_changes
             )
-            if response.status_code != 204:
-                raise ValueError("Failed to update project")
+            response.raise_for_status()
 
         self.project_entity.lock()
 
         operations_body = []
 
         created_entity_ids, other_entity_ids, removed_entity_ids = (
             self._split_entities()
@@ -1481,14 +1482,730 @@
         Warning:
             This is not an api call but is called from entity hub.
         """
 
         self._children_ids = set(children_ids)
 
 
+class ProjectStatus:
+    """Project status class.
+
+    Args:
+        name (str): Name of the status. e.g. 'In progress'
+        short_name (Optional[str]): Short name of the status. e.g. 'IP'
+        state (Optional[Literal[not_started, in_progress, done, blocked]]): A
+            state of the status.
+        icon (Optional[str]): Icon of the status. e.g. 'play_arrow'.
+        color (Optional[str]): Color of the status. e.g. '#eeeeee'.
+        index (Optional[int]): Index of the status.
+        project_statuses (Optional[_ProjectStatuses]): Project statuses
+            wrapper.
+    """
+
+    valid_states = ("not_started", "in_progress", "done", "blocked")
+    color_regex = re.compile(r"#([a-f0-9]{6})$")
+    default_state = "in_progress"
+    default_color = "#eeeeee"
+
+    def __init__(
+        self,
+        name,
+        short_name=None,
+        state=None,
+        icon=None,
+        color=None,
+        index=None,
+        project_statuses=None,
+        is_new=None,
+    ):
+        short_name = short_name or ""
+        icon = icon or ""
+        state = state or self.default_state
+        color = color or self.default_color
+        self._name = name
+        self._short_name = short_name
+        self._icon = icon
+        self._slugified_name = None
+        self._state = None
+        self._color = None
+        self.set_state(state)
+        self.set_color(color)
+
+        self._original_name = name
+        self._original_short_name = short_name
+        self._original_icon = icon
+        self._original_state = state
+        self._original_color = color
+        self._original_index = index
+
+        self._index = index
+        self._project_statuses = project_statuses
+        if is_new is None:
+            is_new = index is None or project_statuses is None
+        self._is_new = is_new
+
+    def __str__(self):
+        short_name = ""
+        if self.short_name:
+            short_name = "({})".format(self.short_name)
+        return "<{} {}{}>".format(
+            self.__class__.__name__, self.name, short_name
+        )
+
+    def __repr__(self):
+        return str(self)
+
+    def __getitem__(self, key):
+        if key in {
+            "name", "short_name", "icon", "state", "color", "slugified_name"
+        }:
+            return getattr(self, key)
+        raise KeyError(key)
+
+    def __setitem__(self, key, value):
+        if key in {"name", "short_name", "icon", "state", "color"}:
+            return setattr(self, key, value)
+        raise KeyError(key)
+
+    def lock(self):
+        """Lock status.
+
+        Changes were commited and current values are now the original values.
+        """
+
+        self._is_new = False
+        self._original_name = self.name
+        self._original_short_name = self.short_name
+        self._original_icon = self.icon
+        self._original_state = self.state
+        self._original_color = self.color
+        self._original_index = self.index
+
+    @staticmethod
+    def slugify_name(name):
+        """Slugify status name for name comparison.
+
+        Args:
+            name (str): Name of the status.
+
+        Returns:
+            str: Slugified name.
+        """
+
+        return slugify_string(name.lower())
+
+    def get_project_statuses(self):
+        """Internal logic method.
+
+        Returns:
+            _ProjectStatuses: Project statuses object.
+        """
+
+        return self._project_statuses
+
+    def set_project_statuses(self, project_statuses):
+        """Internal logic method to change parent object.
+
+        Args:
+            project_statuses (_ProjectStatuses): Project statuses object.
+        """
+
+        self._project_statuses = project_statuses
+
+    def unset_project_statuses(self, project_statuses):
+        """Internal logic method to unset parent object.
+
+        Args:
+            project_statuses (_ProjectStatuses): Project statuses object.
+        """
+
+        if self._project_statuses is project_statuses:
+            self._project_statuses = None
+            self._index = None
+
+    @property
+    def changed(self):
+        """Status has changed.
+
+        Returns:
+            bool: Status has changed.
+        """
+
+        return (
+            self._is_new
+            or self._original_name != self._name
+            or self._original_short_name != self._short_name
+            or self._original_index != self._index
+            or self._original_state != self._state
+            or self._original_icon != self._icon
+            or self._original_color != self._color
+        )
+
+    def delete(self):
+        """Remove status from project statuses object."""
+
+        if self._project_statuses is not None:
+            self._project_statuses.remove(self)
+
+    def get_index(self):
+        """Get index of status.
+
+        Returns:
+            Union[int, None]: Index of status or None if status is not under
+                project.
+        """
+
+        return self._index
+
+    def set_index(self, index, **kwargs):
+        """Change status index.
+
+        Returns:
+            Union[int, None]: Index of status or None if status is not under
+                project.
+        """
+
+        if kwargs.get("from_parent"):
+            self._index = index
+        else:
+            self._project_statuses.set_status_index(self, index)
+
+    def get_name(self):
+        """Status name.
+
+        Returns:
+            str: Status name.
+        """
+
+        return self._name
+
+    def set_name(self, name):
+        """Change status name.
+
+        Args:
+            name (str): New status name.
+        """
+
+        if not isinstance(name, six.string_types):
+            raise TypeError("Name must be a string.")
+        if name == self._name:
+            return
+        self._name = name
+        self._slugified_name = None
+
+    def get_short_name(self):
+        """Status short name 3 letters tops.
+
+        Returns:
+            str: Status short name.
+        """
+
+        return self._short_name
+
+    def set_short_name(self, short_name):
+        """Change status short name.
+
+        Args:
+            short_name (str): New status short name. 3 letters tops.
+        """
+
+        if not isinstance(short_name, six.string_types):
+            raise TypeError("Short name must be a string.")
+        self._short_name = short_name
+
+    def get_icon(self):
+        """Name of icon to use for status.
+
+        Returns:
+            str: Name of the icon.
+        """
+
+        return self._icon
+
+    def set_icon(self, icon):
+        """Change status icon name.
+
+        Args:
+            icon (str): Name of the icon.
+        """
+
+        if icon is None:
+            icon = ""
+        if not isinstance(icon, six.string_types):
+            raise TypeError("Icon name must be a string.")
+        self._icon = icon
+
+    @property
+    def slugified_name(self):
+        """Slugified and lowere status name.
+
+        Can be used for comparison of existing statuses. e.g. 'In Progress'
+            vs. 'in-progress'.
+
+        Returns:
+            str: Slugified and lower status name.
+        """
+
+        if self._slugified_name is None:
+            self._slugified_name = self.slugify_name(self.name)
+        return self._slugified_name
+
+    def get_state(self):
+        """Get state of project status.
+
+        Return:
+            Literal[not_started, in_progress, done, blocked]: General
+                state of status.
+        """
+
+        return self._state
+
+    def set_state(self, state):
+        """Set color of project status.
+
+        Args:
+            state (Literal[not_started, in_progress, done, blocked]): General
+                state of status.
+        """
+
+        if state not in self.valid_states:
+            raise ValueError("Invalid state '{}'".format(str(state)))
+        self._state = state
+
+    def get_color(self):
+        """Get color of project status.
+
+        Returns:
+            str: Status color.
+        """
+
+        return self._color
+
+    def set_color(self, color):
+        """Set color of project status.
+
+        Args:
+            color (str): Color in hex format. Example: '#ff0000'.
+        """
+
+        if not isinstance(color, six.string_types):
+            raise TypeError(
+                "Color must be string got '{}'".format(type(color)))
+        color = color.lower()
+        if self.color_regex.fullmatch(color) is None:
+            raise ValueError("Invalid color value '{}'".format(color))
+        self._color = color
+
+    name = property(get_name, set_name)
+    short_name = property(get_short_name, set_short_name)
+    project_statuses = property(get_project_statuses, set_project_statuses)
+    index = property(get_index, set_index)
+    state = property(get_state, set_state)
+    color = property(get_color, set_color)
+    icon = property(get_icon, set_icon)
+
+    def _validate_other_p_statuses(self, other):
+        """Validate if other status can be used for move.
+
+        To be able to work with other status, and position them in relation,
+        they must belong to same existing object of '_ProjectStatuses'.
+
+        Args:
+            other (ProjectStatus): Other status to validate.
+        """
+
+        o_project_statuses = other.project_statuses
+        m_project_statuses = self.project_statuses
+        if o_project_statuses is None and m_project_statuses is None:
+            raise ValueError("Both statuses are not assigned to a project.")
+
+        missing_status = None
+        if o_project_statuses is None:
+            missing_status = other
+        elif m_project_statuses is None:
+            missing_status = self
+        if missing_status is not None:
+            raise ValueError(
+                "Status '{}' is not assigned to a project.".format(
+                    missing_status.name))
+        if m_project_statuses is not o_project_statuses:
+            raise ValueError(
+                "Statuse are assigned to different projects."
+                " Cannot execute move."
+            )
+
+    def move_before(self, other):
+        """Move status before other status.
+
+        Args:
+            other (ProjectStatus): Status to move before.
+        """
+
+        self._validate_other_p_statuses(other)
+        self._project_statuses.set_status_index(self, other.index)
+
+    def move_after(self, other):
+        """Move status after other status.
+
+        Args:
+            other (ProjectStatus): Status to move after.
+        """
+
+        self._validate_other_p_statuses(other)
+        self._project_statuses.set_status_index(self, other.index + 1)
+
+    def to_data(self):
+        """Convert status to data.
+
+        Returns:
+            dict[str, str]: Status data.
+        """
+
+        output = {
+            "name": self.name,
+            "shortName": self.short_name,
+            "state": self.state,
+            "icon": self.icon,
+            "color": self.color,
+        }
+        if (
+            not self._is_new
+            and self._original_name
+            and self.name != self._original_name
+        ):
+            output["original_name"] = self._original_name
+        return output
+
+    @classmethod
+    def from_data(cls, data, index=None, project_statuses=None):
+        """Create project status from data.
+
+        Args:
+            data (dict[str, str]): Status data.
+            index (Optional[int]): Status index.
+            project_statuses (Optional[ProjectStatuses]): Project statuses
+                object which wraps the status for a project.
+        """
+
+        return cls(
+            data["name"],
+            data.get("shortName", data.get("short_name")),
+            data.get("state"),
+            data.get("icon"),
+            data.get("color"),
+            index=index,
+            project_statuses=project_statuses
+        )
+
+
+class _ProjectStatuses:
+    """Wrapper for project statuses.
+
+    Supports basic methods to add, change or remove statuses from a project.
+
+    To add new statuses use 'create' or 'add_status' methods. To change
+        statuses receive them by one of the getter methods and change their
+        values.
+
+    Todos:
+        Validate if statuses are duplicated.
+    """
+
+    def __init__(self, statuses):
+        self._statuses = [
+            ProjectStatus.from_data(status, idx, self)
+            for idx, status in enumerate(statuses)
+        ]
+        self._orig_status_length = len(self._statuses)
+        self._set_called = False
+
+    def __len__(self):
+        return len(self._statuses)
+
+    def __iter__(self):
+        """Iterate over statuses.
+
+        Yields:
+            ProjectStatus: Project status.
+        """
+
+        for status in self._statuses:
+            yield status
+
+    def create(
+        self,
+        name,
+        short_name=None,
+        state=None,
+        icon=None,
+        color=None,
+    ):
+        """Create project status.
+
+        Args:
+            name (str): Name of the status. e.g. 'In progress'
+            short_name (Optional[str]): Short name of the status. e.g. 'IP'
+            state (Optional[Literal[not_started, in_progress, done, blocked]]): A
+                state of the status.
+            icon (Optional[str]): Icon of the status. e.g. 'play_arrow'.
+            color (Optional[str]): Color of the status. e.g. '#eeeeee'.
+
+        Returns:
+            ProjectStatus: Created project status.
+        """
+
+        status = ProjectStatus(
+            name, short_name, state, icon, color, is_new=True
+        )
+        self.append(status)
+        return status
+
+    def lock(self):
+        """Lock statuses.
+
+        Changes were commited and current values are now the original values.
+        """
+
+        self._orig_status_length = len(self._statuses)
+        self._set_called = False
+        for status in self._statuses:
+            status.lock()
+
+    def to_data(self):
+        """Convert to project statuses data."""
+
+        return [
+            status.to_data()
+            for status in self._statuses
+        ]
+
+    def set(self, statuses):
+        """Explicitly override statuses.
+
+        This method does not handle if statuses changed or not.
+
+        Args:
+            statuses (list[dict[str, str]]): List of statuses data.
+        """
+
+        self._set_called = True
+        self._statuses = [
+            ProjectStatus.from_data(status, idx, self)
+            for idx, status in enumerate(statuses)
+        ]
+
+    @property
+    def changed(self):
+        """Statuses have changed.
+
+        Returns:
+            bool: True if statuses changed, False otherwise.
+        """
+
+        if self._set_called:
+            return True
+
+        # Check if status length changed
+        #   - when all statuses are removed it is a changed
+        if self._orig_status_length != len(self._statuses):
+            return True
+        # Go through all statuses and check if any of them changed
+        for status in self._statuses:
+            if status.changed:
+                return True
+        return False
+
+    def get(self, name, default=None):
+        """Get status by name.
+
+        Args:
+            name (str): Status name.
+            default (Any): Default value of status is not found.
+
+        Returns:
+            Union[ProjectStatus, Any]: Status or default value.
+        """
+
+        return next(
+            (
+                status
+                for status in self._statuses
+                if status.name == name
+            ),
+            default
+        )
+
+    get_status_by_name = get
+
+    def index(self, status, **kwargs):
+        """Get status index.
+
+        Args:
+            status (ProjectStatus): Status to get index of.
+            default (Optional[Any]): Default value if status is not found.
+
+        Returns:
+            Union[int, Any]: Status index.
+
+        Raises:
+            ValueError: If status is not found and default value is not
+                defined.
+        """
+
+        output = next(
+            (
+                idx
+                for idx, st in enumerate(self._statuses)
+                if st is status
+            ),
+            None
+        )
+        if output is not None:
+            return output
+
+        if "default" in kwargs:
+            return kwargs["default"]
+        raise ValueError("Status '{}' not found".format(status.name))
+
+    def get_status_by_slugified_name(self, name):
+        """Get status by slugified name.
+
+        Args:
+            name (str): Status name. Is slugified before search.
+
+        Returns:
+            Union[ProjectStatus, None]: Status or None if not found.
+        """
+
+        slugified_name = ProjectStatus.slugify_name(name)
+        return next(
+            (
+                status
+                for status in self._statuses
+                if status.slugified_name == slugified_name
+            ),
+            None
+        )
+
+    def remove_by_name(self, name, ignore_missing=False):
+        """Remove status by name.
+
+        Args:
+            name (str): Status name.
+            ignore_missing (Optional[bool]): If True, no error is raised if
+                status is not found.
+
+        Returns:
+            ProjectStatus: Removed status.
+        """
+
+        matching_status = self.get(name)
+        if matching_status is None:
+            if ignore_missing:
+                return
+            raise ValueError(
+                "Status '{}' not found in project".format(name))
+        return self.remove(matching_status)
+
+    def remove(self, status, ignore_missing=False):
+        """Remove status.
+
+        Args:
+            status (ProjectStatus): Status to remove.
+            ignore_missing (Optional[bool]): If True, no error is raised if
+                status is not found.
+
+        Returns:
+            Union[ProjectStatus, None]: Removed status.
+        """
+
+        index = self.index(status, default=None)
+        if index is None:
+            if ignore_missing:
+                return None
+            raise ValueError("Status '{}' not in project".format(status))
+
+        return self.pop(index)
+
+    def pop(self, index):
+        """Remove status by index.
+
+        Args:
+            index (int): Status index.
+
+        Returns:
+            ProjectStatus: Removed status.
+        """
+
+        status = self._statuses.pop(index)
+        status.unset_project_statuses(self)
+        for st in self._statuses[index:]:
+            st.set_index(st.index - 1, from_parent=True)
+        return status
+
+    def insert(self, index, status):
+        """Insert status at index.
+
+        Args:
+            index (int): Status index.
+            status (Union[ProjectStatus, dict[str, str]]): Status to insert.
+                Can be either status object or status data.
+
+        Returns:
+            ProjectStatus: Inserted status.
+        """
+
+        if not isinstance(status, ProjectStatus):
+            status = ProjectStatus.from_data(status)
+
+        start_index = index
+        end_index = len(self._statuses) + 1
+        matching_index = self.index(status, default=None)
+        if matching_index is not None:
+            if matching_index == index:
+                status.set_index(index, from_parent=True)
+                return
+
+            self._statuses.pop(matching_index)
+            if matching_index < index:
+                start_index = matching_index
+                end_index = index + 1
+            else:
+                end_index -= 1
+
+        status.set_project_statuses(self)
+        self._statuses.insert(index, status)
+        for idx, st in enumerate(self._statuses[start_index:end_index]):
+            st.set_index(start_index + idx, from_parent=True)
+        return status
+
+    def append(self, status):
+        """Add new status to the end of the list.
+
+        Args:
+            status (Union[ProjectStatus, dict[str, str]]): Status to insert.
+                Can be either status object or status data.
+
+        Returns:
+            ProjectStatus: Inserted status.
+        """
+
+        return self.insert(len(self._statuses), status)
+
+    def set_status_index(self, status, index):
+        """Set status index.
+
+        Args:
+            status (ProjectStatus): Status to set index.
+            index (int): New status index.
+        """
+
+        return self.insert(index, status)
+
+
 class ProjectEntity(BaseEntity):
     """Entity representing project on AYON server.
 
     Args:
         project_code (str): Project code.
         library (bool): Is project library project.
         folder_types (list[dict[str, Any]]): Folder types definition.
@@ -1510,27 +2227,36 @@
     entity_type = "project"
     parent_entity_types = []
     # TODO These are hardcoded but maybe should be used from server???
     default_folder_type_icon = "folder"
     default_task_type_icon = "task_alt"
 
     def __init__(
-        self, project_code, library, folder_types, task_types, *args, **kwargs
+        self,
+        project_code,
+        library,
+        folder_types,
+        task_types,
+        statuses,
+        *args,
+        **kwargs
     ):
         super(ProjectEntity, self).__init__(*args, **kwargs)
 
         self._project_code = project_code
         self._library_project = library
         self._folder_types = folder_types
         self._task_types = task_types
+        self._statuses_obj = _ProjectStatuses(statuses)
 
         self._orig_project_code = project_code
         self._orig_library_project = library
         self._orig_folder_types = copy.deepcopy(folder_types)
         self._orig_task_types = copy.deepcopy(task_types)
+        self._orig_statuses = copy.deepcopy(statuses)
 
     def _prepare_entity_id(self, entity_id):
         if entity_id != self.project_name:
             raise ValueError(
                 "Unexpected entity id value \"{}\". Expected \"{}\"".format(
                     entity_id, self.project_name))
         return entity_id
@@ -1569,31 +2295,45 @@
         new_task_types = []
         for task_type in task_types:
             if "icon" not in task_type:
                 task_type["icon"] = self.default_task_type_icon
             new_task_types.append(task_type)
         self._task_types = new_task_types
 
+    def get_orig_statuses(self):
+        return copy.deepcopy(self._orig_statuses)
+
+    def get_statuses(self):
+        return self._statuses_obj
+
+    def set_statuses(self, statuses):
+        self._statuses_obj.set(statuses)
+
     folder_types = property(get_folder_types, set_folder_types)
     task_types = property(get_task_types, set_task_types)
+    statuses = property(get_statuses, set_statuses)
 
     def lock(self):
         super(ProjectEntity, self).lock()
         self._orig_folder_types = copy.deepcopy(self._folder_types)
         self._orig_task_types = copy.deepcopy(self._task_types)
+        self._statuses_obj.lock()
 
     @property
     def changes(self):
         changes = self._get_default_changes()
         if self._orig_folder_types != self._folder_types:
             changes["folderTypes"] = self.get_folder_types()
 
         if self._orig_task_types != self._task_types:
             changes["taskTypes"] = self.get_task_types()
 
+        if self._statuses_obj.changed:
+            changes["statuses"] = self._statuses_obj.to_data()
+
         return changes
 
     @classmethod
     def from_entity_data(cls, project, entity_hub):
         return cls(
             project["code"],
             parent_id=PROJECT_PARENT_ID,
```

### Comparing `ayon-python-api-0.3.3/ayon_api/events.py` & `ayon-python-api-0.3.4/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/exceptions.py` & `ayon-python-api-0.3.4/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/graphql.py` & `ayon-python-api-0.3.4/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/graphql_queries.py` & `ayon-python-api-0.3.4/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/operations.py` & `ayon-python-api-0.3.4/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/server_api.py` & `ayon-python-api-0.3.4/ayon_api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,24 @@
 from contextlib import contextmanager
 try:
     from http import HTTPStatus
 except ImportError:
     HTTPStatus = None
 
 import requests
-from requests.exceptions import JSONDecodeError as RequestsJSONDecodeError
+try:
+    # This should be used if 'requests' have it available
+    from requests.exceptions import JSONDecodeError as RequestsJSONDecodeError
+except ImportError:
+    # Older versions of 'requests' don't have custom exception for json
+    #   decode error
+    try:
+        from simplejson import JSONDecodeError as RequestsJSONDecodeError
+    except ImportError:
+        from json import JSONDecodeError as RequestsJSONDecodeError
 
 from .constants import (
     DEFAULT_PRODUCT_TYPE_FIELDS,
     DEFAULT_PROJECT_FIELDS,
     DEFAULT_FOLDER_FIELDS,
     DEFAULT_TASK_FIELDS,
     DEFAULT_PRODUCT_FIELDS,
@@ -896,26 +905,32 @@
                     self.create_session()
                 return
 
         self.reset_token()
 
         self.validate_server_availability()
 
-        response = self.post(
-            "auth/login",
-            name=username,
-            password=password
-        )
-        if response.status_code != 200:
-            _detail = response.data.get("detail")
-            details = ""
-            if _detail:
-                details = " {}".format(_detail)
+        self._token_validation_started = True
 
-            raise AuthenticationError("Login failed {}".format(details))
+        try:
+            response = self.post(
+                "auth/login",
+                name=username,
+                password=password
+            )
+            if response.status_code != 200:
+                _detail = response.data.get("detail")
+                details = ""
+                if _detail:
+                    details = " {}".format(_detail)
+
+                raise AuthenticationError("Login failed {}".format(details))
+
+        finally:
+            self._token_validation_started = False
 
         self._access_token = response["token"]
 
         if not self.has_valid_token:
             raise AuthenticationError("Invalid credentials")
 
         if create_session:
@@ -1224,15 +1239,16 @@
 
     def enroll_event_job(
         self,
         source_topic,
         target_topic,
         sender,
         description=None,
-        sequential=None
+        sequential=None,
+        events_filter=None,
     ):
         """Enroll job based on events.
 
         Enroll will find first unprocessed event with 'source_topic' and will
         create new event with 'target_topic' for it and return the new event
         data.
 
@@ -1266,14 +1282,16 @@
             source_topic (str): Source topic to enroll.
             target_topic (str): Topic of dependent event.
             sender (str): Identifier of sender (e.g. service name or username).
             description (Optional[str]): Human readable text shown
                 in target event.
             sequential (Optional[bool]): The source topic must be processed
                 in sequence.
+            events_filter (Optional[ayon_server.sqlfilter.Filter]): A dict-like
+                with conditions to filter the source event.
 
         Returns:
             Union[None, dict[str, Any]]: None if there is no event matching
                 filters. Created event with 'target_topic'.
         """
 
         kwargs = {
@@ -1281,14 +1299,16 @@
             "targetTopic": target_topic,
             "sender": sender,
         }
         if sequential is not None:
             kwargs["sequential"] = sequential
         if description is not None:
             kwargs["description"] = description
+        if events_filter is not None:
+            kwargs["filter"] = events_filter
         response = self.post("enroll", **kwargs)
         if response.status_code == 204:
             return None
         elif response.status_code >= 400:
             self.log.error(response.text)
             return None
```

### Comparing `ayon-python-api-0.3.3/ayon_api/thumbnails.py` & `ayon-python-api-0.3.4/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_api/utils.py` & `ayon-python-api-0.3.4/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.3.4/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -269,15 +269,14 @@
 - Add folder and task changes to operations
 - Enhance entity hub
   - Missing docstrings in EntityHub -> especially entity arguments are missing
   - Better order of arguments for entity classes
     - Move entity hub to first place
     - Skip those which are invalid for the entity and fake it for base or remove it from base
   - Entity hub should use operations session to do changes
-  - Entity hub could also handle 'subset', 'version' and 'representation' entities
-  - Missing 'statuses' on project
+  - Entity hub could also handle 'product', 'version' and 'representation' entities
   - Missing 'status' on folders
   - Missing assignees on tasks
   - Pass docstrings and arguments definitions from `ServerAPI` methods to global functions
 - Split `ServerAPI` into smaller chunks (somehow), the class has 4k+ lines of code
 - Add .pyi stub for ServerAPI 
 - Missing websockets connection
```

### Comparing `ayon-python-api-0.3.3/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.3.4/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.3/pyproject.toml` & `ayon-python-api-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayon-python-api"
-version = "0.3.3"
+version = "0.3.4"
 description = "AYON Python API"
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "ynput.io", email = "info@ynput.io"}
 ]
 keywords = ["AYON", "ynput", "OpenPype", "vfx"]
```

### Comparing `ayon-python-api-0.3.3/setup.py` & `ayon-python-api-0.3.4/setup.py`

 * *Files identical despite different names*

