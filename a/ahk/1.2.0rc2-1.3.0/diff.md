# Comparing `tmp/ahk-1.2.0rc2.tar.gz` & `tmp/ahk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.2.0rc2.tar", last modified: Sun Jul  9 19:18:37 2023, max compression
+gzip compressed data, was "ahk-1.3.0.tar", last modified: Mon Jul 31 02:06:09 2023, max compression
```

## Comparing `ahk-1.2.0rc2.tar` & `ahk-1.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.629729 ahk-1.2.0rc2/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   180681 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    44691 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    83807 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174928 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.629729 ahk-1.2.0rc2/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:06:09.067969 ahk-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 02:05:53.000000 ahk-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-07-31 02:06:09.067969 ahk-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:06:09.063969 ahk-1.3.0/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:06:09.067969 ahk-1.3.0/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   191361 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45795 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86604 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:06:09.067969 ahk-1.3.0/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   185359 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41393 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26345 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:06:09.067969 ahk-1.3.0/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    81832 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-31 02:05:53.000000 ahk-1.3.0/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:06:09.063969 ahk-1.3.0/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-07-31 02:06:09.000000 ahk-1.3.0/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-31 02:06:09.000000 ahk-1.3.0/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 02:06:09.000000 ahk-1.3.0/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 02:06:09.000000 ahk-1.3.0/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 02:06:09.000000 ahk-1.3.0/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-31 02:05:53.000000 ahk-1.3.0/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:06:09.067969 ahk-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19101 2023-07-31 02:05:53.000000 ahk-1.3.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 02:05:53.000000 ahk-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 02:06:09.067969 ahk-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 02:05:53.000000 ahk-1.3.0/setup.py
```

### Comparing `ahk-1.2.0rc2/PKG-INFO` & `ahk-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.2.0rc2
+Version: 1.3.0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -310,27 +310,42 @@
 ahk.set_volume(50, device_number=1)  # Set volume of a device
 ahk.sound_get(device_number=1, component_type='MASTER', control_type='VOLUME') # Get sound device property
 ahk.sound_set(50, device_number=1, component_type='MASTER', control_type='VOLUME') # Set sound device property
 ```
 
 ## GUI
 
+
+Tooltips/traytips
+
 ```python
 import time
 from ahk import AHK
 
 ahk = AHK()
 ahk.show_tooltip("hello4", x=10, y=10)
 time.sleep(2)
 ahk.hide_tooltip() # hide the tooltip
 ahk.show_info_traytip("Info", "It's also info", silent=False, blocking=True)  # Default info traytip
 ahk.show_warning_traytip("Warning", "It's a warning")                           # Warning traytip
 ahk.show_error_traytip("Error", "It's an error")                                 # Error trytip
 ```
 
+Dialog boxes
+
+```python
+from ahk import AHK, MsgBoxButtons
+ahk = AHK()
+
+ahk.msg_box(text='Do you like message boxes?', title='My Title', buttons=MsgBoxButtons.YES_NO)
+ahk.input_box(prompt='Password', title='Enter your password', hide=True)
+ahk.file_select_box(title='Select one or more mp3 files', multi=True, filter='*.mp3', file_must_exist=True)
+ahk.folder_select_box(prompt='Select a folder')
+```
+
 ## Global state changes
 
 You can change various global states such as `CoordMode`, `DetectHiddenWindows`, etc. so you don't have to pass
 these parameters directly to function calls
 
 ```python
 from ahk import AHK
@@ -356,14 +371,28 @@
 from ahk.directives import NoTrayIcon
 
 ahk = AHK(directives=[NoTrayIcon])
 ```
 
 By default, some directives are automatically added to ensure functionality and are merged with any user-provided directives.
 
+Directives are not applied for the AHK process used for handling hotkeys and hotstrings (discussed below) by default. To apply a directive
+to the hotkeys process using the keyword argument `apply_to_hotkeys_process=True`:
+
+```python
+from ahk import AHK
+from ahk.directives import NoTrayIcon
+
+directives = [
+    NoTrayIcon(apply_to_hotkeys_process=True)
+]
+
+ahk = AHK(directives=directives)
+```
+
 ## Menu tray icon
 
 As discussed above, you can hide the tray icon if you wish. Additionally, there are some methods available for
 customizing the tray icon.
 
 
 ```python
```

### Comparing `ahk-1.2.0rc2/ahk/_async/engine.py` & `ahk-1.3.0/ahk/_async/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,38 @@
 from typing import overload
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 from .._hotkey import Hotkey
 from .._hotkey import Hotstring
+from .._utils import MsgBoxButtons
+from .._utils import MsgBoxDefaultButton
+from .._utils import MsgBoxIcon
+from .._utils import MsgBoxModality
+from .._utils import MsgBoxOtherOptions
 from .._utils import type_escape
 from ..directives import Directive
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
 from ..keys import Key
 from .transport import AsyncDaemonProcessTransport
 from .transport import AsyncFutureResult
 from .transport import AsyncTransport
 from .window import AsyncControl
 from .window import AsyncWindow
+
+# from .window import AsyncGui
 from ahk.message import Position
 
+
 async_sleep = asyncio.sleep  # unasync: remove
 sleep = time.sleep
 
 AsyncFilterFunc: TypeAlias = Callable[[AsyncWindow], Awaitable[bool]]  # unasync: remove
 SyncFilterFunc: TypeAlias = Callable[[AsyncWindow], bool]
 
 CoordModeTargets: TypeAlias = Union[
@@ -3482,13 +3490,190 @@
         Analog for `RegRead <https://www.autohotkey.com/docs/commands/RegRead.htm>`_
         """
         args = [key_name]
         if value_name is not None:
             args.append(value_name)
         return await self._transport.function_call('AHKRegRead', args, blocking=blocking)
 
+    # fmt: off
+    @overload
+    async def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None) -> str: ...
+    @overload
+    async def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None, *, blocking: Literal[False]) -> AsyncFutureResult[str]: ...
+    @overload
+    async def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None, *, blocking: Literal[True]) -> str: ...
+    @overload
+    async def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None, *, blocking: bool = True) -> Union[str, AsyncFutureResult[str]]: ...
+    # fmt: on
+    async def msg_box(
+        self,
+        text: str = '',
+        title: str = 'Message',
+        buttons: MsgBoxButtons = MsgBoxButtons.OK,
+        icon: Optional[MsgBoxIcon] = None,
+        default_button: Optional[MsgBoxDefaultButton] = None,
+        modality: Optional[MsgBoxModality] = None,
+        help_button: bool = False,
+        text_right_justified: bool = False,
+        right_to_left_reading: bool = False,
+        timeout: Optional[int] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[str, AsyncFutureResult[str]]:
+        options: int = int(buttons)
+        for opt in (icon, default_button, modality):
+            if opt is not None:
+                options += opt
+        if help_button:
+            options += MsgBoxOtherOptions.HELP_BUTTON
+        if text_right_justified:
+            options += MsgBoxOtherOptions.TEXT_RIGHT_JUSTIFIED
+        if right_to_left_reading:
+            options += MsgBoxOtherOptions.RIGHT_TO_LEFT_READING_ORDER
+
+        args = [str(options), title, text]
+        if timeout is not None:
+            args.append(str(timeout))
+        return await self._transport.function_call('AHKMsgBox', args, blocking=blocking)
+
+    # fmt: off
+    @overload
+    async def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None) -> Union[None, str]: ...
+    @overload
+    async def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: Literal[False]) -> Union[AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    @overload
+    async def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: Literal[True]) -> Union[str, None]: ...
+    @overload
+    async def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: bool = True) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    # fmt: on
+    async def input_box(
+        self,
+        prompt: str = '',
+        title: str = 'Input',
+        default: str = '',
+        hide: bool = False,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        x: Optional[int] = None,
+        y: Optional[int] = None,
+        locale: bool = True,
+        timeout: Optional[int] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[None, str, AsyncFutureResult[str], AsyncFutureResult[None]]:
+        """
+        Like AHK's ``InputBox``
+
+        If the user presses Cancel or closes the box, ``None`` is returned.
+        Otherwise, the user's input is returned.
+        Raises a ``TimeoutError`` if a timeout is specified and expires.
+        """
+        args = [title, prompt]
+        if hide:
+            args.append('hide')
+        else:
+            args.append('')
+        for opt in (width, height, x, y):
+            if opt is not None:
+                args.append(str(opt))
+            else:
+                args.append('')
+        if locale:
+            args.append('Locale')
+        else:
+            args.append('')
+        if timeout is not None:
+            args.append(str(timeout))
+        else:
+            args.append('')
+        args.append(default)
+        return await self._transport.function_call('AHKInputBox', args, blocking=blocking)
+
+    # fmt: off
+    @overload
+    async def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True) -> Union[None, str]: ...
+    @overload
+    async def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True, *, blocking: Literal[False]) -> Union[AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    @overload
+    async def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True, *, blocking: Literal[True]) -> Union[str, None]: ...
+    @overload
+    async def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True, *, blocking: bool = True) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    # fmt: on
+    async def file_select_box(
+        self,
+        title: str = 'Select File',
+        multi: bool = False,
+        root: str = '',
+        filter: str = '',
+        save_button: bool = False,
+        file_must_exist: bool = False,
+        path_must_exist: bool = False,
+        prompt_create_new_file: bool = False,
+        prompt_override_file: bool = False,
+        follow_shortcuts: bool = True,
+        *,
+        blocking: bool = True,
+    ) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]:
+        opts = 0
+        if file_must_exist:
+            opts += 1
+        if path_must_exist:
+            opts += 2
+        if prompt_create_new_file:
+            opts += 8
+        if prompt_override_file:
+            opts += 8
+        if not follow_shortcuts:
+            opts += 32
+        options = ''
+        if multi:
+            options += 'M'
+        if save_button:
+            options += 'S'
+        if opts:
+            options += str(opts)
+        args = [options, root, title, filter]
+        return await self._transport.function_call('AHKFileSelectFile', args, blocking=blocking)
+
+    # fmt: off
+    @overload
+    async def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False) -> Union[None, str]: ...
+    @overload
+    async def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False, *, blocking: Literal[False]) -> Union[AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    @overload
+    async def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False, *, blocking: Literal[True]) -> Union[str, None]: ...
+    @overload
+    async def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False, *, blocking: bool = True) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    # fmt: on
+    async def folder_select_box(
+        self,
+        prompt: str = 'Select Folder',
+        root: str = '',
+        chroot: bool = False,
+        enable_new_directories: bool = True,
+        edit_field: bool = False,
+        new_dialog_style: bool = False,
+        *,
+        blocking: bool = True,
+    ) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]:
+        if not chroot:
+            starting_folder = '*'
+        else:
+            starting_folder = ''
+        starting_folder += root
+        if enable_new_directories:
+            opts = 1
+        else:
+            opts = 0
+        if edit_field:
+            opts += 2
+        if new_dialog_style:
+            opts += 4
+        args = [starting_folder, str(opts), prompt]
+        return await self._transport.function_call('AHKFileSelectFolder', args, blocking=blocking)
+
     async def block_forever(self) -> NoReturn:
         """
         Blocks (sleeps) forever. Utility method to prevent script from exiting.
         """
         while True:
             await async_sleep(1)
```

### Comparing `ahk-1.2.0rc2/ahk/_async/transport.py` & `ahk-1.3.0/ahk/_async/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,27 +82,32 @@
 FunctionName = Literal[
     'AHKBlockInput',
     'AHKClipWait',
     'AHKControlClick',
     'AHKControlGetPos',
     'AHKControlGetText',
     'AHKControlSend',
+    'AHKFileSelectFile',
+    'AHKFileSelectFolder',
     'AHKGetClipboard',
     'AHKGetClipboardAll',
     'AHKGetCoordMode',
     'AHKGetSendLevel',
     'AHKGetTitleMatchMode',
     'AHKGetTitleMatchSpeed',
     'AHKGetVolume',
+    'AHKGuiNew',
     'AHKImageSearch',
+    'AHKInputBox',
     'AHKKeyState',
     'AHKKeyWait',
     'AHKMenuTrayIcon',
     'AHKMenuTrayShow',
     'AHKMenuTrayTip',
+    'AHKMsgBox',
     'AHKMouseClickDrag',
     'AHKMouseGetPos',
     'AHKMouseMove',
     'AHKPixelGetColor',
     'AHKPixelSearch',
     'AHKRegRead',
     'AHKRegWrite',
@@ -587,15 +592,24 @@
     async def function_call(self, function_name: Literal['AHKRegDelete'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKMenuTrayTip'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKMenuTrayIcon'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKMenuTrayShow'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
-
+    @overload
+    async def function_call(self, function_name: Literal['AHKGuiNew'], args: List[str], *, engine: AsyncAHK) -> str: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKMsgBox'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, AsyncFutureResult[str]]: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKInputBox'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKFileSelectFile'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKFileSelectFolder'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, None, AsyncFutureResult[str], AsyncFutureResult[None]]: ...
     # fmt: on
 
     async def function_call(
         self,
         function_name: FunctionName,
         args: Optional[List[str]] = None,
         blocking: bool = True,
```

### Comparing `ahk-1.2.0rc2/ahk/_async/window.py` & `ahk-1.3.0/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc2/ahk/_constants.py` & `ahk-1.3.0/ahk/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -2640,14 +2640,109 @@
     filename := command[2]
     icon_number := command[3]
     freeze := command[4]
     Menu, Tray, Icon, %filename%, %icon_number%,%freeze%
     return FormatNoValueResponse()
 }
 
+AHKGuiNew(ByRef command) {
+    global STRINGRESPONSEMESSAGE
+    options := command[2]
+    title := command[3]
+    Gui, New, %options%, %title%
+    return FormatResponse(STRINGRESPONSEMESSAGE, hwnd)
+}
+
+AHKMsgBox(ByRef command) {
+    global TIMEOUTRESPONSEMESSAGE
+    global STRINGRESPONSEMESSAGE
+    options := command[2]
+    title := command[3]
+    text := command[4]
+    timeout := command[5]
+    MsgBox,% options, %title%, %text%, %timeout%
+    IfMsgBox, Yes
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Yes")
+    IfMsgBox, No
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "No")
+    IfMsgBox, OK
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "OK")
+    IfMsgBox, Cancel
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Cancel")
+    IfMsgBox, Abort
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Abort")
+    IfMsgBox, Ignore
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Ignore")
+    IfMsgBox, Retry
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Retry")
+    IfMsgBox, Continue
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Continue")
+    IfMsgBox, TryAgain
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "TryAgain")
+    IfMsgBox, Timeout
+        ret := FormatResponse(TIMEOUTRESPONSEMESSAGE, "MsgBox timed out")
+    return ret
+}
+
+AHKInputBox(ByRef command) {
+    global STRINGRESPONSEMESSAGE
+    global TIMEOUTRESPONSEMESSAGE
+    title := command[2]
+    prompt := command[3]
+    hide := command[4]
+    width := command[5]
+    height := command[6]
+    x := command[7]
+    y := command[8]
+    locale := command[9]
+    timeout := command[10]
+    default := command[11]
+
+    InputBox, output, %title%, %prompt%, %hide%, %width%, %height%, %x%, %y%, %locale%, %timeout%, %default%
+    if (ErrorLevel = 2) {
+        ret := FormatResponse(TIMEOUTRESPONSEMESSAGE, "Input box timed out")
+    } else if (ErrorLevel = 1) {
+        ret := FormatNoValueResponse()
+    } else {
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, output)
+    }
+    return ret
+}
+
+AHKFileSelectFile(byRef command) {
+    global STRINGRESPONSEMESSAGE
+    options := command[2]
+    root := command[3]
+    title := command[4]
+    filter := command[5]
+    FileSelectFile, output, %options%, %root%, %title%, %filter%
+    if (ErrorLevel = 1) {
+        ret := FormatNoValueResponse()
+    } else {
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, output)
+    }
+    return ret
+}
+
+AHKFileSelectFolder(byRef command) {
+    global STRINGRESPONSEMESSAGE
+    starting_folder := command[2]
+    options := command[3]
+    prompt := command[4]
+
+    FileSelectFolder, output, %starting_folder%, %options%, %prompt%
+
+    if (ErrorLevel = 1) {
+        ret := FormatNoValueResponse()
+    } else {
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, output)
+    }
+    return ret
+}
+
 b64decode(ByRef pszString) {
     ; TODO load DLL globally for performance
     ; REF: https://docs.microsoft.com/en-us/windows/win32/api/wincrypt/nf-wincrypt-cryptstringtobinaryw
     ;  [in]      LPCSTR pszString,  A pointer to a string that contains the formatted string to be converted.
     ;  [in]      DWORD  cchString,  The number of characters of the formatted string to be converted, not including the terminating NULL character. If this parameter is zero, pszString is considered to be a null-terminated string.
     ;  [in]      DWORD  dwFlags,    Indicates the format of the string to be converted. (see table in link above)
     ;  [in]      BYTE   *pbBinary,  A pointer to a buffer that receives the returned sequence of bytes. If this parameter is NULL, the function calculates the length of the buffer needed and returns the size, in bytes, of required memory in the DWORD pointed to by pcbBinary.
```

### Comparing `ahk-1.2.0rc2/ahk/_hotkey.py` & `ahk-1.3.0/ahk/_hotkey.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._hotstrings: Dict[str, Hotstring] = {}
         self._running: bool = False
         self._get_callback_registry = functools.lru_cache(maxsize=None)(self._callback_registry_uncached)
         self._clipboard_callback: Optional[Callable[[int], Any]] = None
         self._clipboard_ex_handler: Optional[Callable[[int, Exception], Any]] = None
         if directives is None:
             directives = []
-        self._directives: list[Directive | Type[Directive]] = directives
+        self._directives: list[Directive | Type[Directive]] = [d for d in directives if d.apply_to_hotkeys_process]
 
     @property
     def _callback_registry(self) -> Dict[str, Union[Hotkey, Hotstring]]:
         return self._get_callback_registry()
 
     def _callback_registry_uncached(self) -> Dict[str, Union[Hotkey, Hotstring]]:
         registry: Dict[str, Union[Hotkey, Hotstring]] = dict(self._hotkeys)
@@ -420,15 +420,15 @@
     def _validate(self) -> None:
         if not isinstance(self.trigger, str):
             raise TypeError(f'trigger must be a string. Got {self.trigger!r}')
         if self.options:
             assert '\n' not in self.options, 'Newlines not allowed in options'
             assert 'x' not in self.options.lower(), 'X is not an allowed option. Use a callback instead.'
             assert re.fullmatch(
-                r'(\?|C|C1|K\d+|O|P\d+|S[IPE]|T|Z)+', self.options.upper()
+                r'(\*|\?|C|C1|K\d+|O|P\d+|S[IPE]|T|Z)+', self.options.upper()
             ), f'Invalid options: {self.options!r}'
         return None
 
 
 @runtime_checkable
 class Killable(Protocol):
     def kill(self) -> None:
```

### Comparing `ahk-1.2.0rc2/ahk/_sync/engine.py` & `ahk-1.3.0/ahk/_sync/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,38 @@
 from typing import overload
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 from .._hotkey import Hotkey
 from .._hotkey import Hotstring
+from .._utils import MsgBoxButtons
+from .._utils import MsgBoxDefaultButton
+from .._utils import MsgBoxIcon
+from .._utils import MsgBoxModality
+from .._utils import MsgBoxOtherOptions
 from .._utils import type_escape
 from ..directives import Directive
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
 from ..keys import Key
 from .transport import DaemonProcessTransport
 from .transport import FutureResult
 from .transport import Transport
 from .window import Control
 from .window import Window
+
+# from .window import AsyncGui
 from ahk.message import Position
 
+
 sleep = time.sleep
 
 SyncFilterFunc: TypeAlias = Callable[[Window], bool]
 
 CoordModeTargets: TypeAlias = Union[
     Literal['ToolTip'], Literal['Pixel'], Literal['Mouse'], Literal['Caret'], Literal['Menu']
 ]
@@ -184,14 +192,15 @@
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return None
 
     def remove_hotkey(self, keyname: str) -> None:
         def _() -> None:
             return None
+
         h = Hotkey(keyname=keyname, callback=_)  # XXX: this can probably be avoided
         self._transport.remove_hotkey(hotkey=h)
         return None
 
     def clear_hotkeys(self) -> None:
         self._transport.clear_hotkeys()
         return None
@@ -201,15 +210,14 @@
         self._transport.remove_hotstring(hs)
         return None
 
     def clear_hotstrings(self) -> None:
         self._transport.clear_hotstrings()
         return None
 
-
     def set_title_match_mode(self, title_match_mode: TitleMatchMode, /) -> None:
         """
         Sets the default title match mode
 
         Does not affect methods called with ``blocking=True`` (because these run in a separate AHK process)
 
         Reference: https://www.autohotkey.com/docs/commands/SetTitleMatchMode.htm
@@ -3471,13 +3479,190 @@
         Analog for `RegRead <https://www.autohotkey.com/docs/commands/RegRead.htm>`_
         """
         args = [key_name]
         if value_name is not None:
             args.append(value_name)
         return self._transport.function_call('AHKRegRead', args, blocking=blocking)
 
+    # fmt: off
+    @overload
+    def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None) -> str: ...
+    @overload
+    def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None, *, blocking: Literal[False]) -> FutureResult[str]: ...
+    @overload
+    def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None, *, blocking: Literal[True]) -> str: ...
+    @overload
+    def msg_box(self, text: str = '', title: str = 'Message', buttons: MsgBoxButtons = MsgBoxButtons.OK, icon: Optional[MsgBoxIcon] = None, default_button: Optional[MsgBoxDefaultButton] = None, modality: Optional[MsgBoxModality] = None, help_button: bool = False, text_right_justified: bool = False, right_to_left_reading: bool = False, timeout: Optional[int] = None, *, blocking: bool = True) -> Union[str, FutureResult[str]]: ...
+    # fmt: on
+    def msg_box(
+        self,
+        text: str = '',
+        title: str = 'Message',
+        buttons: MsgBoxButtons = MsgBoxButtons.OK,
+        icon: Optional[MsgBoxIcon] = None,
+        default_button: Optional[MsgBoxDefaultButton] = None,
+        modality: Optional[MsgBoxModality] = None,
+        help_button: bool = False,
+        text_right_justified: bool = False,
+        right_to_left_reading: bool = False,
+        timeout: Optional[int] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[str, FutureResult[str]]:
+        options: int = int(buttons)
+        for opt in (icon, default_button, modality):
+            if opt is not None:
+                options += opt
+        if help_button:
+            options += MsgBoxOtherOptions.HELP_BUTTON
+        if text_right_justified:
+            options += MsgBoxOtherOptions.TEXT_RIGHT_JUSTIFIED
+        if right_to_left_reading:
+            options += MsgBoxOtherOptions.RIGHT_TO_LEFT_READING_ORDER
+
+        args = [str(options), title, text]
+        if timeout is not None:
+            args.append(str(timeout))
+        return self._transport.function_call('AHKMsgBox', args, blocking=blocking)
+
+    # fmt: off
+    @overload
+    def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None) -> Union[None, str]: ...
+    @overload
+    def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: Literal[False]) -> Union[FutureResult[str], FutureResult[None]]: ...
+    @overload
+    def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: Literal[True]) -> Union[str, None]: ...
+    @overload
+    def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: bool = True) -> Union[str, None, FutureResult[str], FutureResult[None]]: ...
+    # fmt: on
+    def input_box(
+        self,
+        prompt: str = '',
+        title: str = 'Input',
+        default: str = '',
+        hide: bool = False,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        x: Optional[int] = None,
+        y: Optional[int] = None,
+        locale: bool = True,
+        timeout: Optional[int] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[None, str, FutureResult[str], FutureResult[None]]:
+        """
+        Like AHK's ``InputBox``
+
+        If the user presses Cancel or closes the box, ``None`` is returned.
+        Otherwise, the user's input is returned.
+        Raises a ``TimeoutError`` if a timeout is specified and expires.
+        """
+        args = [title, prompt]
+        if hide:
+            args.append('hide')
+        else:
+            args.append('')
+        for opt in (width, height, x, y):
+            if opt is not None:
+                args.append(str(opt))
+            else:
+                args.append('')
+        if locale:
+            args.append('Locale')
+        else:
+            args.append('')
+        if timeout is not None:
+            args.append(str(timeout))
+        else:
+            args.append('')
+        args.append(default)
+        return self._transport.function_call('AHKInputBox', args, blocking=blocking)
+
+    # fmt: off
+    @overload
+    def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True) -> Union[None, str]: ...
+    @overload
+    def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True, *, blocking: Literal[False]) -> Union[FutureResult[str], FutureResult[None]]: ...
+    @overload
+    def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True, *, blocking: Literal[True]) -> Union[str, None]: ...
+    @overload
+    def file_select_box(self, title: str = 'Select File', multi: bool = False, root: str = '', filter: str = '', save_button: bool = False, file_must_exist: bool = False, path_must_exist: bool = False, prompt_create_new_file: bool = False, prompt_override_file: bool = False, follow_shortcuts: bool = True, *, blocking: bool = True) -> Union[str, None, FutureResult[str], FutureResult[None]]: ...
+    # fmt: on
+    def file_select_box(
+        self,
+        title: str = 'Select File',
+        multi: bool = False,
+        root: str = '',
+        filter: str = '',
+        save_button: bool = False,
+        file_must_exist: bool = False,
+        path_must_exist: bool = False,
+        prompt_create_new_file: bool = False,
+        prompt_override_file: bool = False,
+        follow_shortcuts: bool = True,
+        *,
+        blocking: bool = True,
+    ) -> Union[str, None, FutureResult[str], FutureResult[None]]:
+        opts = 0
+        if file_must_exist:
+            opts += 1
+        if path_must_exist:
+            opts += 2
+        if prompt_create_new_file:
+            opts += 8
+        if prompt_override_file:
+            opts += 8
+        if not follow_shortcuts:
+            opts += 32
+        options = ''
+        if multi:
+            options += 'M'
+        if save_button:
+            options += 'S'
+        if opts:
+            options += str(opts)
+        args = [options, root, title, filter]
+        return self._transport.function_call('AHKFileSelectFile', args, blocking=blocking)
+
+    # fmt: off
+    @overload
+    def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False) -> Union[None, str]: ...
+    @overload
+    def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False, *, blocking: Literal[False]) -> Union[FutureResult[str], FutureResult[None]]: ...
+    @overload
+    def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False, *, blocking: Literal[True]) -> Union[str, None]: ...
+    @overload
+    def folder_select_box(self, prompt: str = 'Select Folder', root: str = '', chroot: bool = False, enable_new_directories: bool = True, edit_field: bool = False, new_dialog_style: bool = False, *, blocking: bool = True) -> Union[str, None, FutureResult[str], FutureResult[None]]: ...
+    # fmt: on
+    def folder_select_box(
+        self,
+        prompt: str = 'Select Folder',
+        root: str = '',
+        chroot: bool = False,
+        enable_new_directories: bool = True,
+        edit_field: bool = False,
+        new_dialog_style: bool = False,
+        *,
+        blocking: bool = True,
+    ) -> Union[str, None, FutureResult[str], FutureResult[None]]:
+        if not chroot:
+            starting_folder = '*'
+        else:
+            starting_folder = ''
+        starting_folder += root
+        if enable_new_directories:
+            opts = 1
+        else:
+            opts = 0
+        if edit_field:
+            opts += 2
+        if new_dialog_style:
+            opts += 4
+        args = [starting_folder, str(opts), prompt]
+        return self._transport.function_call('AHKFileSelectFolder', args, blocking=blocking)
+
     def block_forever(self) -> NoReturn:
         """
         Blocks (sleeps) forever. Utility method to prevent script from exiting.
         """
         while True:
             sleep(1)
```

### Comparing `ahk-1.2.0rc2/ahk/_sync/transport.py` & `ahk-1.3.0/ahk/_sync/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,27 +74,32 @@
 FunctionName = Literal[
     'AHKBlockInput',
     'AHKClipWait',
     'AHKControlClick',
     'AHKControlGetPos',
     'AHKControlGetText',
     'AHKControlSend',
+    'AHKFileSelectFile',
+    'AHKFileSelectFolder',
     'AHKGetClipboard',
     'AHKGetClipboardAll',
     'AHKGetCoordMode',
     'AHKGetSendLevel',
     'AHKGetTitleMatchMode',
     'AHKGetTitleMatchSpeed',
     'AHKGetVolume',
+    'AHKGuiNew',
     'AHKImageSearch',
+    'AHKInputBox',
     'AHKKeyState',
     'AHKKeyWait',
     'AHKMenuTrayIcon',
     'AHKMenuTrayShow',
     'AHKMenuTrayTip',
+    'AHKMsgBox',
     'AHKMouseClickDrag',
     'AHKMouseGetPos',
     'AHKMouseMove',
     'AHKPixelGetColor',
     'AHKPixelSearch',
     'AHKRegRead',
     'AHKRegWrite',
@@ -568,15 +573,24 @@
     def function_call(self, function_name: Literal['AHKRegDelete'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKMenuTrayTip'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKMenuTrayIcon'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKMenuTrayShow'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
-
+    @overload
+    def function_call(self, function_name: Literal['AHKGuiNew'], args: List[str], *, engine: AHK) -> str: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKMsgBox'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, FutureResult[str]]: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKInputBox'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, None, FutureResult[str], FutureResult[None]]: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKFileSelectFile'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, None, FutureResult[str], FutureResult[None]]: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKFileSelectFolder'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, None, FutureResult[str], FutureResult[None]]: ...
     # fmt: on
 
     def function_call(
         self,
         function_name: FunctionName,
         args: Optional[List[str]] = None,
         blocking: bool = True,
```

### Comparing `ahk-1.2.0rc2/ahk/_sync/window.py` & `ahk-1.3.0/ahk/_sync/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,14 +631,15 @@
     def from_pid(cls, engine: AHK, pid: int) -> Optional[Window]:
         return engine.win_get(title=f'ahk_pid {pid}')
 
     @classmethod
     def from_mouse_position(cls, engine: AHK) -> Optional[Window]:
         return engine.win_get_from_mouse_position()
 
+
 class Control:
     def __init__(self, window: Window, hwnd: str, control_class: str):
         self.window: Window = window
         self.hwnd: str = hwnd
         self.control_class: str = control_class
         self._engine = window._engine
```

### Comparing `ahk-1.2.0rc2/ahk/directives.py` & `ahk-1.3.0/ahk/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
     def __hash__(self) -> int:
         return hash(str(self))
 
     def __eq__(cls, other: Any) -> bool:
         return bool(str(cls) == other)
 
+    @property
+    def apply_to_hotkeys_process(cls) -> bool:
+        return False
+
 
 class Directive(SimpleNamespace, metaclass=DirectiveMeta):
     """
     Simple directive class
     They are designed to be hashable and comparable with string equivalent of AHK directive.
     Directives that don't require arguments do not need to be instantiated.
     """
```

### Comparing `ahk-1.2.0rc2/ahk/keys.py` & `ahk-1.3.0/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc2/ahk/message.py` & `ahk-1.3.0/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc2/ahk/templates/daemon.ahk` & `ahk-1.3.0/ahk/templates/daemon.ahk`

 * *Files 7% similar despite different names*

```diff
@@ -2637,14 +2637,109 @@
     filename := command[2]
     icon_number := command[3]
     freeze := command[4]
     Menu, Tray, Icon, %filename%, %icon_number%,%freeze%
     return FormatNoValueResponse()
 }
 
+AHKGuiNew(ByRef command) {
+    global STRINGRESPONSEMESSAGE
+    options := command[2]
+    title := command[3]
+    Gui, New, %options%, %title%
+    return FormatResponse(STRINGRESPONSEMESSAGE, hwnd)
+}
+
+AHKMsgBox(ByRef command) {
+    global TIMEOUTRESPONSEMESSAGE
+    global STRINGRESPONSEMESSAGE
+    options := command[2]
+    title := command[3]
+    text := command[4]
+    timeout := command[5]
+    MsgBox,% options, %title%, %text%, %timeout%
+    IfMsgBox, Yes
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Yes")
+    IfMsgBox, No
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "No")
+    IfMsgBox, OK
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "OK")
+    IfMsgBox, Cancel
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Cancel")
+    IfMsgBox, Abort
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Abort")
+    IfMsgBox, Ignore
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Ignore")
+    IfMsgBox, Retry
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Retry")
+    IfMsgBox, Continue
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "Continue")
+    IfMsgBox, TryAgain
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, "TryAgain")
+    IfMsgBox, Timeout
+        ret := FormatResponse(TIMEOUTRESPONSEMESSAGE, "MsgBox timed out")
+    return ret
+}
+
+AHKInputBox(ByRef command) {
+    global STRINGRESPONSEMESSAGE
+    global TIMEOUTRESPONSEMESSAGE
+    title := command[2]
+    prompt := command[3]
+    hide := command[4]
+    width := command[5]
+    height := command[6]
+    x := command[7]
+    y := command[8]
+    locale := command[9]
+    timeout := command[10]
+    default := command[11]
+
+    InputBox, output, %title%, %prompt%, %hide%, %width%, %height%, %x%, %y%, %locale%, %timeout%, %default%
+    if (ErrorLevel = 2) {
+        ret := FormatResponse(TIMEOUTRESPONSEMESSAGE, "Input box timed out")
+    } else if (ErrorLevel = 1) {
+        ret := FormatNoValueResponse()
+    } else {
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, output)
+    }
+    return ret
+}
+
+AHKFileSelectFile(byRef command) {
+    global STRINGRESPONSEMESSAGE
+    options := command[2]
+    root := command[3]
+    title := command[4]
+    filter := command[5]
+    FileSelectFile, output, %options%, %root%, %title%, %filter%
+    if (ErrorLevel = 1) {
+        ret := FormatNoValueResponse()
+    } else {
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, output)
+    }
+    return ret
+}
+
+AHKFileSelectFolder(byRef command) {
+    global STRINGRESPONSEMESSAGE
+    starting_folder := command[2]
+    options := command[3]
+    prompt := command[4]
+
+    FileSelectFolder, output, %starting_folder%, %options%, %prompt%
+
+    if (ErrorLevel = 1) {
+        ret := FormatNoValueResponse()
+    } else {
+        ret := FormatResponse(STRINGRESPONSEMESSAGE, output)
+    }
+    return ret
+}
+
 b64decode(ByRef pszString) {
     ; TODO load DLL globally for performance
     ; REF: https://docs.microsoft.com/en-us/windows/win32/api/wincrypt/nf-wincrypt-cryptstringtobinaryw
     ;  [in]      LPCSTR pszString,  A pointer to a string that contains the formatted string to be converted.
     ;  [in]      DWORD  cchString,  The number of characters of the formatted string to be converted, not including the terminating NULL character. If this parameter is zero, pszString is considered to be a null-terminated string.
     ;  [in]      DWORD  dwFlags,    Indicates the format of the string to be converted. (see table in link above)
     ;  [in]      BYTE   *pbBinary,  A pointer to a buffer that receives the returned sequence of bytes. If this parameter is NULL, the function calculates the length of the buffer needed and returns the size, in bytes, of required memory in the DWORD pointed to by pcbBinary.
```

### Comparing `ahk-1.2.0rc2/ahk/templates/hotkeys.ahk` & `ahk-1.3.0/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc2/ahk.egg-info/PKG-INFO` & `ahk-1.3.0/ahk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.2.0rc2
+Version: 1.3.0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -310,27 +310,42 @@
 ahk.set_volume(50, device_number=1)  # Set volume of a device
 ahk.sound_get(device_number=1, component_type='MASTER', control_type='VOLUME') # Get sound device property
 ahk.sound_set(50, device_number=1, component_type='MASTER', control_type='VOLUME') # Set sound device property
 ```
 
 ## GUI
 
+
+Tooltips/traytips
+
 ```python
 import time
 from ahk import AHK
 
 ahk = AHK()
 ahk.show_tooltip("hello4", x=10, y=10)
 time.sleep(2)
 ahk.hide_tooltip() # hide the tooltip
 ahk.show_info_traytip("Info", "It's also info", silent=False, blocking=True)  # Default info traytip
 ahk.show_warning_traytip("Warning", "It's a warning")                           # Warning traytip
 ahk.show_error_traytip("Error", "It's an error")                                 # Error trytip
 ```
 
+Dialog boxes
+
+```python
+from ahk import AHK, MsgBoxButtons
+ahk = AHK()
+
+ahk.msg_box(text='Do you like message boxes?', title='My Title', buttons=MsgBoxButtons.YES_NO)
+ahk.input_box(prompt='Password', title='Enter your password', hide=True)
+ahk.file_select_box(title='Select one or more mp3 files', multi=True, filter='*.mp3', file_must_exist=True)
+ahk.folder_select_box(prompt='Select a folder')
+```
+
 ## Global state changes
 
 You can change various global states such as `CoordMode`, `DetectHiddenWindows`, etc. so you don't have to pass
 these parameters directly to function calls
 
 ```python
 from ahk import AHK
@@ -356,14 +371,28 @@
 from ahk.directives import NoTrayIcon
 
 ahk = AHK(directives=[NoTrayIcon])
 ```
 
 By default, some directives are automatically added to ensure functionality and are merged with any user-provided directives.
 
+Directives are not applied for the AHK process used for handling hotkeys and hotstrings (discussed below) by default. To apply a directive
+to the hotkeys process using the keyword argument `apply_to_hotkeys_process=True`:
+
+```python
+from ahk import AHK
+from ahk.directives import NoTrayIcon
+
+directives = [
+    NoTrayIcon(apply_to_hotkeys_process=True)
+]
+
+ahk = AHK(directives=directives)
+```
+
 ## Menu tray icon
 
 As discussed above, you can hide the tray icon if you wish. Additionally, there are some methods available for
 customizing the tray icon.
 
 
 ```python
```

### Comparing `ahk-1.2.0rc2/ahk.egg-info/SOURCES.txt` & `ahk-1.3.0/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc2/buildunasync.py` & `ahk-1.3.0/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc2/docs/README.md` & `ahk-1.3.0/docs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -287,27 +287,42 @@
 ahk.set_volume(50, device_number=1)  # Set volume of a device
 ahk.sound_get(device_number=1, component_type='MASTER', control_type='VOLUME') # Get sound device property
 ahk.sound_set(50, device_number=1, component_type='MASTER', control_type='VOLUME') # Set sound device property
 ```
 
 ## GUI
 
+
+Tooltips/traytips
+
 ```python
 import time
 from ahk import AHK
 
 ahk = AHK()
 ahk.show_tooltip("hello4", x=10, y=10)
 time.sleep(2)
 ahk.hide_tooltip() # hide the tooltip
 ahk.show_info_traytip("Info", "It's also info", silent=False, blocking=True)  # Default info traytip
 ahk.show_warning_traytip("Warning", "It's a warning")                           # Warning traytip
 ahk.show_error_traytip("Error", "It's an error")                                 # Error trytip
 ```
 
+Dialog boxes
+
+```python
+from ahk import AHK, MsgBoxButtons
+ahk = AHK()
+
+ahk.msg_box(text='Do you like message boxes?', title='My Title', buttons=MsgBoxButtons.YES_NO)
+ahk.input_box(prompt='Password', title='Enter your password', hide=True)
+ahk.file_select_box(title='Select one or more mp3 files', multi=True, filter='*.mp3', file_must_exist=True)
+ahk.folder_select_box(prompt='Select a folder')
+```
+
 ## Global state changes
 
 You can change various global states such as `CoordMode`, `DetectHiddenWindows`, etc. so you don't have to pass
 these parameters directly to function calls
 
 ```python
 from ahk import AHK
@@ -333,14 +348,28 @@
 from ahk.directives import NoTrayIcon
 
 ahk = AHK(directives=[NoTrayIcon])
 ```
 
 By default, some directives are automatically added to ensure functionality and are merged with any user-provided directives.
 
+Directives are not applied for the AHK process used for handling hotkeys and hotstrings (discussed below) by default. To apply a directive
+to the hotkeys process using the keyword argument `apply_to_hotkeys_process=True`:
+
+```python
+from ahk import AHK
+from ahk.directives import NoTrayIcon
+
+directives = [
+    NoTrayIcon(apply_to_hotkeys_process=True)
+]
+
+ahk = AHK(directives=directives)
+```
+
 ## Menu tray icon
 
 As discussed above, you can hide the tray icon if you wish. Additionally, there are some methods available for
 customizing the tray icon.
 
 
 ```python
```

### Comparing `ahk-1.2.0rc2/setup.cfg` & `ahk-1.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.2.0rc2
+version = 1.3.0
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords =
```

