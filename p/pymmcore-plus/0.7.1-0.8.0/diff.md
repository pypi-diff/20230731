# Comparing `tmp/pymmcore_plus-0.7.1.tar.gz` & `tmp/pymmcore_plus-0.8.0.tar.gz`

## Comparing `pymmcore_plus-0.7.1.tar` & `pymmcore_plus-0.8.0.tar`

### file list

```diff
@@ -1,83 +1,49 @@
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/codecov.yml
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/mkdocs.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/_hooks.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/contributing.md
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/index.md
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/install.md
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/cmmcoreplus.md
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/configuration.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/constants.md
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/device.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/events.md
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/mda.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/metadata.md
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/utils.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/context-set.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/following_changes_in_core.md
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/integration-with-qt.md
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/mda.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/napari-micromanager.md
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/guides/logging.md
--rw-r--r--   0        0        0    79333 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/images/components.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/images/favicon.ico
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/napari.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/properties_and_state_events.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/qt_integration.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/run_mda.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/set_as_context.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/__init__.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_build.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_cli.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_logger.py
--rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_version.py
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/install.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/py.typed
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_adapter.py
--rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config_group.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_constants.py
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_device.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_metadata.py
--rw-r--r--   0        0        0    76552 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_mmcore_plus.py
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_property.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_sequencing.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/__init__.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_device_signal_view.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_norm_slot.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_prop_event_mixin.py
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_protocol.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_psygnal.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_qsignals.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/__init__.py
--rw-r--r--   0        0        0    11051 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_engine.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_protocol.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_runner.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_protocol.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_psygnal.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_qsignals.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/local_config.cfg
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_adapter_class.py
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_cli.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_config_group_class.py
--rw-r--r--   0        0        0    17063 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_core.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_device_class.py
--rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_events.py
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_mda.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_misc.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_property_class.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_sequencing.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/LICENSE
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/README.md
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/__init__.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/_build.py
+-rw-r--r--   0        0        0    12220 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/_cli.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/_logger.py
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/_util.py
+-rw-r--r--   0        0        0     7991 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/install.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/py.typed
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_adapter.py
+-rw-r--r--   0        0        0    10596 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_config.py
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_config_group.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_constants.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_device.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_metadata.py
+-rw-r--r--   0        0        0    76899 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_mmcore_plus.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_property.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/_sequencing.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_device_signal_view.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_norm_slot.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_prop_event_mixin.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_protocol.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_psygnal.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_qsignals.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/__init__.py
+-rw-r--r--   0        0        0    14838 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/_engine.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/_protocol.py
+-rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/_runner.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/events/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/events/_protocol.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/events/_psygnal.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/src/pymmcore_plus/mda/events/_qsignals.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/local_config.cfg
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_adapter_class.py
+-rw-r--r--   0        0        0     9839 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_cli.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_config_group_class.py
+-rw-r--r--   0        0        0    17076 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_core.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_device_class.py
+-rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_events.py
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_mda.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_misc.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_property_class.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/tests/test_sequencing.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/README.md
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 pymmcore_plus-0.8.0/PKG-INFO
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/__init__.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from importlib.metadata import PackageNotFoundError, version
+
 try:
-    from ._version import version as __version__
-except ImportError:
+    __version__ = version("pymmcore-plus")
+except PackageNotFoundError:
     __version__ = "unknown"
 
 
 from ._logger import configure_logging
 from ._util import find_micromanager
 from .core import (
     CMMCorePlus,
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/_build.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/_build.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/_cli.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     release: str = typer.Option(
         "latest", "-r", "--release", help="Release date. e.g. 20210201"
     ),
 ) -> None:
     """Install Micro-Manager Device adapters."""
     import pymmcore_plus.install
 
-    pymmcore_plus.install._install(dest, release)
+    pymmcore_plus.install.install(dest, release)
 
 
 @app.command()
 def run(
     useq: Optional[Path] = typer.Argument(
         None,
         dir_okay=False,
@@ -203,15 +203,19 @@
 ) -> None:
     """Run a Micro-Manager acquisition from a useq-schema MDASequence file."""
     import json
 
     from useq import MDASequence
 
     # load from file if provided...
-    mda = {} if useq is None else MDASequence.parse_file(useq).dict()
+    if useq is None:
+        mda = {}
+    else:
+        _mda = MDASequence.from_file(useq)
+        mda = _mda.model_dump() if hasattr(_mda, "model_dump") else _mda.dict()
 
     # Any command line arguments take precedence over useq file
     # note that useq-schema itself will handle any conflicts between z plans
     # (the first correct Union of keyword arguments will win.)
     _zmap = (
         ("go_up", z_go_up),
         ("top", z_top),
@@ -220,29 +224,27 @@
         ("above", z_above),
         ("below", z_below),
         ("step", z_step),
         ("relative", z_relative),
         ("absolute", z_absolute),
     )
     if z_plan := {k: v for k, v in _zmap if v not in (None, [])}:
-        field = MDASequence.__fields__["z_plan"]
-        if field.validate(z_plan, {}, loc="")[0]:
+        try:
             # the field is valid on its own. overwrite:
-            mda["z_plan"] = z_plan
-        else:
+            mda["z_plan"] = MDASequence(z_plan=z_plan).z_plan
+        except Exception:
             # the field is not valid on its own. update existing:
             mda.setdefault("z_plan", {}).update(z_plan)
 
     _tmap = (("interval", t_interval), ("duration", t_duration), ("loops", t_loops))
     if time_plan := {k: v for k, v in _tmap if v is not None}:
-        field = MDASequence.__fields__["time_plan"]
-        if field.validate(time_plan, {}, loc="")[0]:
+        try:
             # the field is valid on its own. overwrite:
-            mda["time_plan"] = time_plan
-        else:
+            mda["time_plan"] = MDASequence(time_plan=time_plan).time_plan
+        except Exception:
             # the field is not valid on its own. update existing:
             mda.setdefault("time_plan", {}).update(time_plan)
 
     if axis_order is not None:
         mda["axis_order"] = axis_order
 
     for c in channel or []:
@@ -261,15 +263,15 @@
             cast(dict, c)["group"] = channel_group
 
     # this will raise if anything has gone wrong.
     _mda = MDASequence(**mda)
 
     if dry_run:
         print(":eyes: [bold green]Would run\n")
-        print(_mda.dict())
+        print(_mda.model_dump() if hasattr(_mda, "model_dump") else _mda.dict())
         raise typer.Exit(0)
 
     core = pymmcore_plus.CMMCorePlus.instance()
     core.loadSystemConfiguration(config or "MMConfig_demo.cfg")
     core.run_mda(_mda)
 
 
@@ -289,17 +291,17 @@
         None,
         "-y",
         help="Overwrite existing if git sha is already built. "
         "If not specified, will prompt.",
     ),
 ) -> None:  # pragma: no cover
     """Build DemoCamera and Utility adapters from source for apple silicon."""
-    import pymmcore_plus._build
+    from pymmcore_plus._build import build
 
-    pymmcore_plus._build.build(dest, overwrite=overwrite)
+    build(dest, overwrite=overwrite)
 
 
 @app.command()
 def logs(
     num: Optional[int] = typer.Option(
         None, "-n", "--num", help="Number of lines to display."
     ),
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/_logger.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import atexit
 import contextlib
 import os
 import sys
+import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 try:
     from typing_extensions import deprecated
 except ImportError:
 
@@ -153,15 +154,22 @@
     )
     configure_logging(strerr_level=level)
 
 
 def current_logfile(logger: Any) -> Path | None:
     """Hacky way to return the current log file."""
     # sourcery skip: use-next
-    for h in logger._core.handlers.values():
-        if hasattr(h, "_sink") and getattr(h._sink, "_path", None):
-            return Path(h._sink._path)
+    try:
+        for h in logger._core.handlers.values():  # noqa: SLF001
+            if hasattr(h, "_sink") and getattr(h._sink, "_path", None):  # noqa: SLF001
+                return Path(h._sink._path)  # noqa: SLF001
+    except AttributeError as e:  # pragma: no cover
+        warnings.warn(
+            f"Error determining current log file {e}. Please check loguru version.",
+            RuntimeWarning,
+            stacklevel=1,
+        )
     return None
 
 
 configure_logging()
 atexit.register(logger.remove)
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/_util.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from time import sleep
 from typing import TYPE_CHECKING, Literal, overload
 
 import appdirs
 
 if TYPE_CHECKING:
-    from typing import TYPE_CHECKING, Any, Callable, TypeVar
+    from typing import Any, Callable, TypeVar
 
     from typing_extensions import ParamSpec
 
     P = ParamSpec("P")
     R = TypeVar("R")
 
 
@@ -241,16 +241,16 @@
     for i, col in enumerate(data.values()):
         for val in col:
             col_widths[i] = max(col_widths[i], len(str(val)))
     fmt = " | ".join(f"{{:<{w}s}}" for w in col_widths)
 
     print(fmt.format(*data.keys()))
 
-    dashs = ["-" * w for w in col_widths]
-    print(fmt.format(*dashs))
+    dashes = ["-" * w for w in col_widths]
+    print(fmt.format(*dashes))
 
     for row in _sorted_rows(data, sort=sort):
         print(fmt.format(*(str(x) for x in row)))
 
 
 def _rich_print_table(data: dict[str, list[str]], sort: str | None = None) -> None:
     """Print pretty table with rich."""
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/install.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,16 @@
         pbar.update(task_id, advance=block_size)
 
     print(f"[bold blue]Downloading {url} ...")
     with pbar:
         urlretrieve(url=url, filename=output_path, reporthook=hook)
 
 
-def _install(dest: Path, release: str) -> None:
+def install(dest: Path, release: str) -> None:
+    """Install Micro-Manager to `dest`."""
     if PLATFORM not in ("Darwin", "Windows"):  # pragma: no cover
         print(f":x: [bold red]Unsupported platform: {PLATFORM!r}")
         raise sys.exit(1)
 
     if release == "latest":
         plat = {
             "Darwin": "macos/Micro-Manager-x86_64-latest.dmg",
@@ -238,12 +239,12 @@
         "--yes",
         action="store_true",
         default=False,
         help="Say yes to all prompts. (no input mode).",
     )
 
     args = parser.parse_args()
-    _install(Path(args.dest), args.release)
+    install(Path(args.dest), args.release)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/__init__.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_adapter.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, NamedTuple
 
 from pymmcore_plus.core._constants import DeviceType
-from pymmcore_plus.core._device import Device
 
 if TYPE_CHECKING:
+    from pymmcore_plus.core._device import Device
+
     from ._mmcore_plus import CMMCorePlus
 
 
 class AvailableDevice(NamedTuple):
     adapter_name: str
     device_name: str
     type: DeviceType
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """pythonic wrapper on pymmcore.Configuration object."""
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import Any, Iterable, Iterator, Tuple, overload
+from typing import TYPE_CHECKING, Any, Iterable, Iterator, Tuple, overload
 
 import pymmcore
-from typing_extensions import TypeAlias
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
 
 DevPropValueTuple: TypeAlias = Tuple[str, str, str]
 DevPropTuple: TypeAlias = Tuple[str, str]
 
 
 class Configuration(pymmcore.Configuration):
     """Encapsulation of configuration information.
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config_group.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pymmcore
 
 from ._config import Configuration
 from ._property import DeviceProperty
 
 if TYPE_CHECKING:
-    from ..core._mmcore_plus import CMMCorePlus
+    from pymmcore_plus.core._mmcore_plus import CMMCorePlus
 
 
 class ConfigGroup(MutableMapping[str, Configuration]):
     """Convenience object for dealing with a set of related Configuration objects.
 
     This object behaves as a [`collections.abc.MutableMapping`][] of `str`
     (configuration group name) to [`Configuration`][pymmcore_plus.Configuration]
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_constants.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_constants.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_device.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,14 @@
     def wait(self) -> None:
         """Block the calling thread until device becomes non-busy."""
         self._mmc.waitForDevice(self.label)
 
     def __repr__(self) -> str:
         if self.isLoaded():
             n = len(self.propertyNames())
-            props = f'{n} propertie{"s" if n>1 else ""}'
+            props = f'{n} {"properties" if n>1 else "property"}'
             lib = f"({self.library()}::{self.name()}) "
         else:
             props = "NOT LOADED"
             lib = ""
         core = repr(self._mmc).strip("<>")
         return f"<Device {self.label!r} {lib}on {core}: {props}>"
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_metadata.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_metadata.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_mmcore_plus.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_mmcore_plus.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,4758 +28,4780 @@
 000001b0: 5365 7175 656e 6365 2c0d 0a20 2020 2054  Sequence,..    T
 000001c0: 7970 6556 6172 2c0d 0a20 2020 2063 6173  ypeVar,..    cas
 000001d0: 742c 0d0a 2020 2020 6f76 6572 6c6f 6164  t,..    overload
 000001e0: 2c0d 0a29 0d0a 0d0a 696d 706f 7274 2070  ,..)....import p
 000001f0: 796d 6d63 6f72 650d 0a66 726f 6d20 7073  ymmcore..from ps
 00000200: 7967 6e61 6c20 696d 706f 7274 2053 6967  ygnal import Sig
 00000210: 6e61 6c49 6e73 7461 6e63 650d 0a0d 0a66  nalInstance....f
-00000220: 726f 6d20 2e2e 5f6c 6f67 6765 7220 696d  rom .._logger im
-00000230: 706f 7274 2063 7572 7265 6e74 5f6c 6f67  port current_log
-00000240: 6669 6c65 2c20 6c6f 6767 6572 0d0a 6672  file, logger..fr
-00000250: 6f6d 202e 2e5f 7574 696c 2069 6d70 6f72  om .._util impor
-00000260: 7420 6669 6e64 5f6d 6963 726f 6d61 6e61  t find_micromana
-00000270: 6765 722c 2070 7269 6e74 5f74 6162 756c  ger, print_tabul
-00000280: 6172 5f64 6174 610d 0a66 726f 6d20 2e2e  ar_data..from ..
-00000290: 6d64 6120 696d 706f 7274 204d 4441 456e  mda import MDAEn
-000002a0: 6769 6e65 2c20 4d44 4152 756e 6e65 722c  gine, MDARunner,
-000002b0: 2050 4d44 4145 6e67 696e 650d 0a66 726f   PMDAEngine..fro
-000002c0: 6d20 2e5f 6164 6170 7465 7220 696d 706f  m ._adapter impo
-000002d0: 7274 2044 6576 6963 6541 6461 7074 6572  rt DeviceAdapter
-000002e0: 0d0a 6672 6f6d 202e 5f63 6f6e 6669 6720  ..from ._config 
-000002f0: 696d 706f 7274 2043 6f6e 6669 6775 7261  import Configura
-00000300: 7469 6f6e 0d0a 6672 6f6d 202e 5f63 6f6e  tion..from ._con
-00000310: 6669 675f 6772 6f75 7020 696d 706f 7274  fig_group import
-00000320: 2043 6f6e 6669 6747 726f 7570 0d0a 6672   ConfigGroup..fr
-00000330: 6f6d 202e 5f63 6f6e 7374 616e 7473 2069  om ._constants i
-00000340: 6d70 6f72 7420 4465 7669 6365 4465 7465  mport DeviceDete
-00000350: 6374 696f 6e53 7461 7475 732c 2044 6576  ctionStatus, Dev
-00000360: 6963 6554 7970 652c 2050 726f 7065 7274  iceType, Propert
-00000370: 7954 7970 650d 0a66 726f 6d20 2e5f 6465  yType..from ._de
-00000380: 7669 6365 2069 6d70 6f72 7420 4465 7669  vice import Devi
-00000390: 6365 0d0a 6672 6f6d 202e 5f6d 6574 6164  ce..from ._metad
-000003a0: 6174 6120 696d 706f 7274 204d 6574 6164  ata import Metad
-000003b0: 6174 610d 0a66 726f 6d20 2e5f 7072 6f70  ata..from ._prop
-000003c0: 6572 7479 2069 6d70 6f72 7420 4465 7669  erty import Devi
-000003d0: 6365 5072 6f70 6572 7479 0d0a 6672 6f6d  ceProperty..from
-000003e0: 202e 5f73 6571 7565 6e63 696e 6720 696d   ._sequencing im
-000003f0: 706f 7274 2063 616e 5f73 6571 7565 6e63  port can_sequenc
-00000400: 655f 6576 656e 7473 0d0a 6672 6f6d 202e  e_events..from .
-00000410: 6576 656e 7473 2069 6d70 6f72 7420 434d  events import CM
-00000420: 4d43 6f72 6553 6967 6e61 6c65 722c 2050  MCoreSignaler, P
-00000430: 436f 7265 5369 676e 616c 6572 2c20 5f67  CoreSignaler, _g
-00000440: 6574 5f61 7574 6f5f 636f 7265 5f63 616c  et_auto_core_cal
-00000450: 6c62 6163 6b5f 636c 6173 730d 0a0d 0a69  lback_class....i
-00000460: 6620 5459 5045 5f43 4845 434b 494e 473a  f TYPE_CHECKING:
-00000470: 0d0a 2020 2020 696d 706f 7274 206e 756d  ..    import num
-00000480: 7079 2061 7320 6e70 0d0a 2020 2020 6672  py as np..    fr
-00000490: 6f6d 2074 7970 696e 675f 6578 7465 6e73  om typing_extens
-000004a0: 696f 6e73 2069 6d70 6f72 7420 4c69 7465  ions import Lite
-000004b0: 7261 6c2c 2054 7970 6564 4469 6374 0d0a  ral, TypedDict..
-000004c0: 2020 2020 6672 6f6d 2075 7365 7120 696d      from useq im
-000004d0: 706f 7274 204d 4441 4576 656e 740d 0a0d  port MDAEvent...
-000004e0: 0a20 2020 205f 5420 3d20 5479 7065 5661  .    _T = TypeVa
-000004f0: 7228 225f 5422 290d 0a20 2020 205f 4620  r("_T")..    _F 
-00000500: 3d20 5479 7065 5661 7228 225f 4622 2c20  = TypeVar("_F", 
-00000510: 626f 756e 643d 4361 6c6c 6162 6c65 5b2e  bound=Callable[.
-00000520: 2e2e 2c20 416e 795d 290d 0a20 2020 204c  .., Any])..    L
-00000530: 6973 744f 7254 7570 6c65 203d 206c 6973  istOrTuple = lis
-00000540: 745b 5f54 5d20 7c20 7475 706c 655b 5f54  t[_T] | tuple[_T
-00000550: 2c20 2e2e 2e5d 0d0a 0d0a 2020 2020 636c  , ...]....    cl
-00000560: 6173 7320 5374 6174 6544 6963 7428 5479  ass StateDict(Ty
-00000570: 7065 6444 6963 742c 2074 6f74 616c 3d46  pedDict, total=F
-00000580: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
-00000590: 2222 2244 6963 7469 6f6e 6172 7920 6f66  """Dictionary of
-000005a0: 2073 7461 7465 2076 616c 7565 7320 666f   state values fo
-000005b0: 7220 6120 6465 7669 6365 2e0d 0a0d 0a20  r a device..... 
-000005c0: 2020 2020 2020 2054 6869 7320 6f62 6a65         This obje
-000005d0: 6374 2073 686f 756c 6420 6f6e 6c79 2062  ct should only b
-000005e0: 6520 696d 706f 7274 6564 2069 6e73 6964  e imported insid
-000005f0: 6520 6120 6054 5950 455f 4348 4543 4b49  e a `TYPE_CHECKI
-00000600: 4e47 6020 626c 6f63 6b2e 0d0a 2020 2020  NG` block...    
-00000610: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
-00000620: 2020 2041 7574 6f46 6f63 7573 4465 7669     AutoFocusDevi
-00000630: 6365 3a20 7374 720d 0a20 2020 2020 2020  ce: str..       
-00000640: 2042 7974 6573 5065 7250 6978 656c 3a20   BytesPerPixel: 
-00000650: 696e 740d 0a20 2020 2020 2020 2043 616d  int..        Cam
-00000660: 6572 6143 6861 6e6e 656c 4e61 6d65 733a  eraChannelNames:
-00000670: 2074 7570 6c65 5b73 7472 2c20 2e2e 2e5d   tuple[str, ...]
-00000680: 0d0a 2020 2020 2020 2020 4361 6d65 7261  ..        Camera
-00000690: 4465 7669 6365 3a20 7374 720d 0a20 2020  Device: str..   
-000006a0: 2020 2020 2044 6174 6574 696d 653a 2073       Datetime: s
-000006b0: 7472 0d0a 2020 2020 2020 2020 4578 706f  tr..        Expo
-000006c0: 7375 7265 3a20 666c 6f61 740d 0a20 2020  sure: float..   
-000006d0: 2020 2020 2046 6f63 7573 4465 7669 6365       FocusDevice
-000006e0: 3a20 7374 720d 0a20 2020 2020 2020 2047  : str..        G
-000006f0: 616c 766f 4465 7669 6365 3a20 7374 720d  alvoDevice: str.
-00000700: 0a20 2020 2020 2020 2049 6d61 6765 4269  .        ImageBi
-00000710: 7444 6570 7468 3a20 696e 740d 0a20 2020  tDepth: int..   
-00000720: 2020 2020 2049 6d61 6765 4865 6967 6874       ImageHeight
-00000730: 3a20 696e 740d 0a20 2020 2020 2020 2049  : int..        I
-00000740: 6d61 6765 5072 6f63 6573 736f 7244 6576  mageProcessorDev
-00000750: 6963 653a 2073 7472 0d0a 2020 2020 2020  ice: str..      
-00000760: 2020 496d 6167 6557 6964 7468 3a20 696e    ImageWidth: in
-00000770: 740d 0a20 2020 2020 2020 2050 6978 656c  t..        Pixel
-00000780: 5369 7a65 556d 3a20 666c 6f61 740d 0a20  SizeUm: float.. 
-00000790: 2020 2020 2020 2053 6875 7474 6572 4465         ShutterDe
-000007a0: 7669 6365 3a20 7374 720d 0a20 2020 2020  vice: str..     
-000007b0: 2020 2053 4c4d 4465 7669 6365 3a20 7374     SLMDevice: st
-000007c0: 720d 0a20 2020 2020 2020 2058 5950 6f73  r..        XYPos
-000007d0: 6974 696f 6e3a 2074 7570 6c65 5b66 6c6f  ition: tuple[flo
-000007e0: 6174 2c20 666c 6f61 745d 0d0a 2020 2020  at, float]..    
-000007f0: 2020 2020 5859 5374 6167 6544 6576 6963      XYStageDevic
-00000800: 653a 2073 7472 0d0a 2020 2020 2020 2020  e: str..        
-00000810: 5a50 6f73 6974 696f 6e3a 2066 6c6f 6174  ZPosition: float
-00000820: 0d0a 0d0a 2020 2020 636c 6173 7320 5072  ....    class Pr
-00000830: 6f70 6572 7479 5363 6865 6d61 2854 7970  opertySchema(Typ
-00000840: 6564 4469 6374 2c20 746f 7461 6c3d 4661  edDict, total=Fa
-00000850: 6c73 6529 3a0d 0a20 2020 2020 2020 2022  lse):..        "
-00000860: 2222 4a53 4f4e 2073 6368 656d 6120 6064  ""JSON schema `d
-00000870: 6963 7460 2064 6573 6372 6962 696e 6720  ict` describing 
-00000880: 6120 6465 7669 6365 2070 726f 7065 7274  a device propert
-00000890: 792e 2222 220d 0a0d 0a20 2020 2020 2020  y."""....       
-000008a0: 2074 7970 653a 2073 7472 0d0a 2020 2020   type: str..    
-000008b0: 2020 2020 6d61 7869 6d75 6d3a 2066 6c6f      maximum: flo
-000008c0: 6174 0d0a 2020 2020 2020 2020 6d69 6e69  at..        mini
-000008d0: 6d75 6d3a 2066 6c6f 6174 0d0a 2020 2020  mum: float..    
-000008e0: 2020 2020 656e 756d 3a20 6c69 7374 0d0a      enum: list..
-000008f0: 2020 2020 2020 2020 7265 6164 4f6e 6c79          readOnly
-00000900: 3a20 626f 6f6c 0d0a 2020 2020 2020 2020  : bool..        
-00000910: 6465 6661 756c 743a 2041 6e79 0d0a 2020  default: Any..  
-00000920: 2020 2020 2020 7365 7175 656e 6365 6162        sequenceab
-00000930: 6c65 3a20 626f 6f6c 0d0a 2020 2020 2020  le: bool..      
-00000940: 2020 7365 7175 656e 6365 4d61 784c 656e    sequenceMaxLen
-00000950: 6774 683a 2069 6e74 0d0a 2020 2020 2020  gth: int..      
-00000960: 2020 7072 6549 6e69 743a 2062 6f6f 6c0d    preInit: bool.
-00000970: 0a0d 0a20 2020 2063 6c61 7373 2044 6576  ...    class Dev
-00000980: 6963 6553 6368 656d 6128 5479 7065 6444  iceSchema(TypedD
-00000990: 6963 7429 3a0d 0a20 2020 2020 2020 2022  ict):..        "
-000009a0: 2222 4a53 4f4e 2073 6368 656d 6120 6064  ""JSON schema `d
-000009b0: 6963 7460 2064 6573 6372 6962 696e 6720  ict` describing 
-000009c0: 6120 6465 7669 6365 2e22 2222 0d0a 0d0a  a device."""....
-000009d0: 2020 2020 2020 2020 7469 746c 653a 2073          title: s
-000009e0: 7472 0d0a 2020 2020 2020 2020 6465 7363  tr..        desc
-000009f0: 7269 7074 696f 6e3a 2073 7472 0d0a 2020  ription: str..  
-00000a00: 2020 2020 2020 7479 7065 3a20 7374 720d        type: str.
-00000a10: 0a20 2020 2020 2020 2070 726f 7065 7274  .        propert
-00000a20: 6965 733a 2064 6963 745b 7374 722c 2050  ies: dict[str, P
-00000a30: 726f 7065 7274 7953 6368 656d 615d 0d0a  ropertySchema]..
-00000a40: 0d0a 2020 2020 6465 6620 7379 6e63 6872  ..    def synchr
-00000a50: 6f6e 697a 6564 286c 6f63 6b3a 2052 4c6f  onized(lock: RLo
-00000a60: 636b 2920 2d3e 2043 616c 6c61 626c 655b  ck) -> Callable[
-00000a70: 5b5f 465d 2c20 5f46 5d3a 0d0a 2020 2020  [_F], _F]:..    
-00000a80: 2020 2020 2e2e 2e0d 0a0d 0a65 6c73 653a      .......else:
-00000a90: 0d0a 2020 2020 6672 6f6d 2077 7261 7074  ..    from wrapt
-00000aa0: 2069 6d70 6f72 7420 7379 6e63 6872 6f6e   import synchron
-00000ab0: 697a 6564 0d0a 0d0a 5f4f 424a 4445 565f  ized...._OBJDEV_
-00000ac0: 5245 4745 5820 3d20 7265 2e63 6f6d 7069  REGEX = re.compi
-00000ad0: 6c65 2822 282e 2b29 3f28 6e6f 7365 7069  le("(.+)?(nosepi
-00000ae0: 6563 657c 6f62 6a28 6563 7469 7665 293f  ece|obj(ective)?
-00000af0: 2928 7475 7272 6574 293f 733f 222c 2072  )(turret)?s?", r
-00000b00: 652e 4947 4e4f 5245 4341 5345 290d 0a5f  e.IGNORECASE).._
-00000b10: 4348 414e 4e45 4c5f 5245 4745 5820 3d20  CHANNEL_REGEX = 
-00000b20: 7265 2e63 6f6d 7069 6c65 2822 2863 6861  re.compile("(cha
-00000b30: 6e7b 312c 327d 2865 6c29 3f7c 6669 6c74  n{1,2}(el)?|filt
-00000b40: 2865 7229 3f29 733f 222c 2072 652e 4947  (er)?)s?", re.IG
-00000b50: 4e4f 5245 4341 5345 290d 0a0d 0a53 5441  NORECASE)....STA
-00000b60: 5445 203d 2070 796d 6d63 6f72 652e 675f  TE = pymmcore.g_
-00000b70: 4b65 7977 6f72 645f 5374 6174 650d 0a4c  Keyword_State..L
-00000b80: 4142 454c 203d 2070 796d 6d63 6f72 652e  ABEL = pymmcore.
-00000b90: 675f 4b65 7977 6f72 645f 4c61 6265 6c0d  g_Keyword_Label.
-00000ba0: 0a53 5441 5445 5f50 524f 5053 203d 2028  .STATE_PROPS = (
-00000bb0: 5354 4154 452c 204c 4142 454c 290d 0a55  STATE, LABEL)..U
-00000bc0: 4e4e 414d 4544 5f50 5245 5345 5420 3d20  NNAMED_PRESET = 
-00000bd0: 224e 6577 5072 6573 6574 220d 0a0d 0a0d  "NewPreset".....
-00000be0: 0a40 636f 6e74 6578 746d 616e 6167 6572  .@contextmanager
-00000bf0: 0d0a 6465 6620 5f62 6c6f 636b 5369 676e  ..def _blockSign
-00000c00: 616c 286f 626a 3a20 416e 792c 2073 6967  al(obj: Any, sig
-00000c10: 6e61 6c3a 2041 6e79 2920 2d3e 2049 7465  nal: Any) -> Ite
-00000c20: 7261 746f 725b 4e6f 6e65 5d3a 0d0a 2020  rator[None]:..  
-00000c30: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00000c40: 7369 676e 616c 2c20 5369 676e 616c 496e  signal, SignalIn
-00000c50: 7374 616e 6365 293a 0d0a 2020 2020 2020  stance):..      
-00000c60: 2020 7369 676e 616c 2e62 6c6f 636b 2829    signal.block()
-00000c70: 0d0a 2020 2020 2020 2020 7969 656c 640d  ..        yield.
-00000c80: 0a20 2020 2020 2020 2073 6967 6e61 6c2e  .        signal.
-00000c90: 756e 626c 6f63 6b28 290d 0a20 2020 2065  unblock()..    e
-00000ca0: 6c73 653a 0d0a 2020 2020 2020 2020 6f62  lse:..        ob
-00000cb0: 6a2e 626c 6f63 6b53 6967 6e61 6c73 2854  j.blockSignals(T
-00000cc0: 7275 6529 0d0a 2020 2020 2020 2020 7969  rue)..        yi
-00000cd0: 656c 640d 0a20 2020 2020 2020 206f 626a  eld..        obj
-00000ce0: 2e62 6c6f 636b 5369 676e 616c 7328 4661  .blockSignals(Fa
-00000cf0: 6c73 6529 0d0a 0d0a 0d0a 5f69 6e73 7461  lse)......_insta
-00000d00: 6e63 6520 3d20 4e6f 6e65 0d0a 0d0a 0d0a  nce = None......
-00000d10: 636c 6173 7320 434d 4d43 6f72 6550 6c75  class CMMCorePlu
-00000d20: 7328 7079 6d6d 636f 7265 2e43 4d4d 436f  s(pymmcore.CMMCo
-00000d30: 7265 293a 0d0a 2020 2020 2222 2257 7261  re):..    """Wra
-00000d40: 7070 6572 2066 6f72 2043 4d4d 436f 7265  pper for CMMCore
-00000d50: 2077 6974 6820 6578 7465 6e64 6564 2066   with extended f
-00000d60: 756e 6374 696f 6e61 6c69 7479 2e0d 0a0d  unctionality....
-00000d70: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
-00000d80: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
-00000d90: 0a20 2020 206d 6d5f 7061 7468 203a 2073  .    mm_path : s
-00000da0: 7472 207c 204e 6f6e 652c 206f 7074 696f  tr | None, optio
-00000db0: 6e61 6c0d 0a20 2020 2020 2020 2050 6174  nal..        Pat
-00000dc0: 6820 746f 2074 6865 204d 6963 726f 2d4d  h to the Micro-M
-00000dd0: 616e 6167 6572 2069 6e73 7461 6c6c 6174  anager installat
-00000de0: 696f 6e2e 2049 6620 604e 6f6e 6560 2028  ion. If `None` (
-00000df0: 6465 6661 756c 7429 2c20 7769 6c6c 2075  default), will u
-00000e00: 7365 2074 6865 0d0a 2020 2020 2020 2020  se the..        
-00000e10: 7265 7475 726e 2076 616c 7565 206f 6620  return value of 
-00000e20: 5b60 7079 6d6d 636f 7265 5f70 6c75 732e  [`pymmcore_plus.
-00000e30: 6669 6e64 5f6d 6963 726f 6d61 6e61 6765  find_micromanage
-00000e40: 7260 5d5b 5d2e 0d0a 2020 2020 6164 6170  r`][]...    adap
-00000e50: 7465 725f 7061 7468 7320 3a20 5365 7175  ter_paths : Sequ
-00000e60: 656e 6365 5b73 7472 5d2c 206f 7074 696f  ence[str], optio
-00000e70: 6e61 6c0d 0a20 2020 2020 2020 2050 6174  nal..        Pat
-00000e80: 6873 2074 6f20 7365 6172 6368 2066 6f72  hs to search for
-00000e90: 2064 6576 6963 6520 6164 6170 7465 7273   device adapters
-00000ea0: 2c20 6279 2064 6566 6175 6c74 2028 290d  , by default ().
-00000eb0: 0a20 2020 2022 2222 0d0a 0d0a 2020 2020  .    """....    
-00000ec0: 5f6c 6f63 6b20 3d20 524c 6f63 6b28 290d  _lock = RLock().
-00000ed0: 0a0d 0a20 2020 2040 636c 6173 736d 6574  ...    @classmet
-00000ee0: 686f 640d 0a20 2020 2064 6566 2069 6e73  hod..    def ins
-00000ef0: 7461 6e63 6528 636c 7329 202d 3e20 434d  tance(cls) -> CM
-00000f00: 4d43 6f72 6550 6c75 733a 0d0a 2020 2020  MCorePlus:..    
-00000f10: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-00000f20: 6520 676c 6f62 616c 2073 696e 676c 6574  e global singlet
-00000f30: 6f6e 2069 6e73 7461 6e63 6520 6f66 2060  on instance of `
-00000f40: 434d 4d43 6f72 6550 6c75 7360 2e0d 0a0d  CMMCorePlus`....
-00000f50: 0a20 2020 2020 2020 203a 7370 6172 6b6c  .        :sparkl
-00000f60: 6573 3a20 2a54 6869 7320 6d65 7468 6f64  es: *This method
-00000f70: 2069 7320 6e65 7720 696e 2060 434d 4d43   is new in `CMMC
-00000f80: 6f72 6550 6c75 7360 2e2a 0d0a 0d0a 2020  orePlus`.*....  
-00000f90: 2020 2020 2020 496e 206d 616e 7920 6361        In many ca
-00000fa0: 7365 732c 2061 2073 696e 676c 6520 696e  ses, a single in
-00000fb0: 7374 616e 6365 206f 6620 6043 4d4d 436f  stance of `CMMCo
-00000fc0: 7265 506c 7573 6020 6973 2061 6c6c 2074  rePlus` is all t
-00000fd0: 6861 7420 7769 6c6c 2062 6520 6372 6561  hat will be crea
-00000fe0: 7465 640d 0a20 2020 2020 2020 2069 6e20  ted..        in 
-00000ff0: 6120 6769 7665 6e20 7365 7373 696f 6e2e  a given session.
-00001000: 2020 5468 6973 2063 6c61 7373 206d 6574    This class met
-00001010: 686f 6420 7072 6f76 6964 6573 2061 2063  hod provides a c
-00001020: 6f6e 7665 6e69 656e 7420 7761 7920 746f  onvenient way to
-00001030: 2061 6363 6573 730d 0a20 2020 2020 2020   access..       
-00001040: 2074 6861 7420 696e 7374 616e 6365 2e0d   that instance..
-00001050: 0a0d 0a20 2020 2020 2020 2021 2121 2074  ...        !!! t
-00001060: 6970 0d0a 0d0a 2020 2020 2020 2020 2020  ip....          
-00001070: 2020 4372 6561 7469 6e67 2f61 6363 6573    Creating/acces
-00001080: 7369 6e67 2061 2060 434d 4d43 6f72 6550  sing a `CMMCoreP
-00001090: 6c75 7360 206f 626a 6563 7420 7573 696e  lus` object usin
-000010a0: 6720 6043 4d4d 436f 7265 506c 7573 2e69  g `CMMCorePlus.i
-000010b0: 6e73 7461 6e63 6528 2960 2069 730d 0a20  nstance()` is.. 
-000010c0: 2020 2020 2020 2020 2020 2061 2063 6f6e             a con
-000010d0: 7665 6e69 656e 7420 7761 7920 746f 2061  venient way to a
-000010e0: 6363 6573 7320 7468 6520 7361 6d65 2063  ccess the same c
-000010f0: 6f72 6520 696e 7374 616e 6365 2066 726f  ore instance fro
-00001100: 6d20 6d75 6c74 6970 6c65 2070 6c61 6365  m multiple place
-00001110: 7320 696e 0d0a 2020 2020 2020 2020 2020  s in..          
-00001120: 2020 796f 7572 2063 6f64 652e 2041 6c6c    your code. All
-00001130: 2077 6964 6765 7473 2069 6e0d 0a20 2020   widgets in..   
-00001140: 2020 2020 2020 2020 205b 6070 796d 6d63           [`pymmc
-00001150: 6f72 652d 7769 6467 6574 7360 5d28 6874  ore-widgets`](ht
-00001160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001170: 2f70 796d 6d63 6f72 652d 706c 7573 2f70  /pymmcore-plus/p
-00001180: 796d 6d63 6f72 652d 7769 6467 6574 7329  ymmcore-widgets)
-00001190: 2061 6c73 6f0d 0a20 2020 2020 2020 2020   also..         
-000011a0: 2020 2075 7365 2060 434d 4d43 6f72 6550     use `CMMCoreP
-000011b0: 6c75 732e 696e 7374 616e 6365 2829 6020  lus.instance()` 
-000011c0: 6279 2064 6566 6175 6c74 2c20 736f 2061  by default, so a
-000011d0: 6e79 2077 6964 6765 7473 2079 6f75 2075  ny widgets you u
-000011e0: 7365 2077 696c 6c0d 0a20 2020 2020 2020  se will..       
-000011f0: 2020 2020 2061 7574 6f6d 6174 6963 616c       automatical
-00001200: 6c79 2063 6f6e 6e65 6374 2074 6f20 7468  ly connect to th
-00001210: 6520 7361 6d65 2063 6f72 6520 696e 7374  e same core inst
-00001220: 616e 6365 2077 6974 686f 7574 2061 6e79  ance without any
-00001230: 2061 6464 6974 696f 6e61 6c0d 0a20 2020   additional..   
-00001240: 2020 2020 2020 2020 2063 6f6e 6669 6775           configu
-00001250: 7261 7469 6f6e 2e0d 0a0d 0a20 2020 2020  ration.....     
-00001260: 2020 2020 2020 2041 7474 656d 7074 7320         Attempts 
-00001270: 2a61 7265 2a20 6d61 6465 2074 6f20 6d61  *are* made to ma
-00001280: 6b65 2069 7420 7468 7265 6164 2d73 6166  ke it thread-saf
-00001290: 652e 2020 4275 7420 706c 6561 7365 206f  e.  But please o
-000012a0: 7065 6e20 616e 2069 7373 7565 0d0a 2020  pen an issue..  
-000012b0: 2020 2020 2020 2020 2020 6966 2079 6f75            if you
-000012c0: 2066 696e 6420 616e 7920 7072 6f62 6c65   find any proble
-000012d0: 6d73 2e0d 0a0d 0a0d 0a20 2020 2020 2020  ms.......       
-000012e0: 2022 2222 0d0a 2020 2020 2020 2020 676c   """..        gl
-000012f0: 6f62 616c 205f 696e 7374 616e 6365 0d0a  obal _instance..
-00001300: 2020 2020 2020 2020 6966 205f 696e 7374          if _inst
-00001310: 616e 6365 2069 7320 4e6f 6e65 3a0d 0a20  ance is None:.. 
-00001320: 2020 2020 2020 2020 2020 205f 696e 7374             _inst
-00001330: 616e 6365 203d 2063 6c73 2829 0d0a 2020  ance = cls()..  
-00001340: 2020 2020 2020 7265 7475 726e 205f 696e        return _in
-00001350: 7374 616e 6365 0d0a 0d0a 2020 2020 6465  stance....    de
-00001360: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00001370: 206d 6d5f 7061 7468 3a20 7374 7220 7c20   mm_path: str | 
-00001380: 4e6f 6e65 203d 204e 6f6e 652c 2061 6461  None = None, ada
-00001390: 7074 6572 5f70 6174 6873 3a20 5365 7175  pter_paths: Sequ
-000013a0: 656e 6365 5b73 7472 5d20 3d20 2829 293a  ence[str] = ()):
-000013b0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-000013c0: 292e 5f5f 696e 6974 5f5f 2829 0d0a 0d0a  ).__init__()....
-000013d0: 2020 2020 2020 2020 6966 206c 6f67 6669          if logfi
-000013e0: 6c65 203a 3d20 6375 7272 656e 745f 6c6f  le := current_lo
-000013f0: 6766 696c 6528 6c6f 6767 6572 293a 0d0a  gfile(logger):..
-00001400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001410: 2e73 6574 5072 696d 6172 794c 6f67 4669  .setPrimaryLogFi
-00001420: 6c65 2873 7472 286c 6f67 6669 6c65 2929  le(str(logfile))
-00001430: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-00001440: 6767 6572 2e64 6562 7567 2822 496e 6974  gger.debug("Init
-00001450: 6961 6c69 7a65 6420 636f 7265 207b 7d22  ialized core {}"
-00001460: 2c20 7365 6c66 290d 0a0d 0a20 2020 2020  , self)....     
-00001470: 2020 2073 656c 662e 5f6d 6d5f 7061 7468     self._mm_path
-00001480: 203d 206d 6d5f 7061 7468 206f 7220 6669   = mm_path or fi
-00001490: 6e64 5f6d 6963 726f 6d61 6e61 6765 7228  nd_micromanager(
-000014a0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-000014b0: 7420 6164 6170 7465 725f 7061 7468 7320  t adapter_paths 
-000014c0: 616e 6420 7365 6c66 2e5f 6d6d 5f70 6174  and self._mm_pat
-000014d0: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-000014e0: 6164 6170 7465 725f 7061 7468 7320 3d20  adapter_paths = 
-000014f0: 5b73 656c 662e 5f6d 6d5f 7061 7468 5d0d  [self._mm_path].
-00001500: 0a20 2020 2020 2020 2069 6620 6164 6170  .        if adap
-00001510: 7465 725f 7061 7468 733a 0d0a 2020 2020  ter_paths:..    
-00001520: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00001530: 4465 7669 6365 4164 6170 7465 7253 6561  DeviceAdapterSea
-00001540: 7263 6850 6174 6873 2861 6461 7074 6572  rchPaths(adapter
-00001550: 5f70 6174 6873 290d 0a0d 0a20 2020 2020  _paths)....     
-00001560: 2020 2073 656c 662e 5f65 7665 6e74 7320     self._events 
-00001570: 3d20 5f67 6574 5f61 7574 6f5f 636f 7265  = _get_auto_core
-00001580: 5f63 616c 6c62 6163 6b5f 636c 6173 7328  _callback_class(
-00001590: 2928 290d 0a20 2020 2020 2020 2073 656c  )()..        sel
-000015a0: 662e 5f63 616c 6c62 6163 6b5f 7265 6c61  f._callback_rela
-000015b0: 7920 3d20 4d4d 4361 6c6c 6261 636b 5265  y = MMCallbackRe
-000015c0: 6c61 7928 7365 6c66 2e65 7665 6e74 7329  lay(self.events)
-000015d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-000015e0: 6567 6973 7465 7243 616c 6c62 6163 6b28  egisterCallback(
-000015f0: 7365 6c66 2e5f 6361 6c6c 6261 636b 5f72  self._callback_r
-00001600: 656c 6179 290d 0a0d 0a20 2020 2020 2020  elay)....       
-00001610: 2073 656c 662e 5f6d 6461 5f72 756e 6e65   self._mda_runne
-00001620: 7220 3d20 4d44 4152 756e 6e65 7228 290d  r = MDARunner().
-00001630: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
-00001640: 6461 5f72 756e 6e65 722e 7365 745f 656e  da_runner.set_en
-00001650: 6769 6e65 284d 4441 456e 6769 6e65 2873  gine(MDAEngine(s
-00001660: 656c 6629 290d 0a0d 0a20 2020 2020 2020  elf))....       
-00001670: 2073 656c 662e 5f6f 626a 6563 7469 7665   self._objective
-00001680: 5f72 6567 6578 3a20 5061 7474 6572 6e20  _regex: Pattern 
-00001690: 3d20 5f4f 424a 4445 565f 5245 4745 580d  = _OBJDEV_REGEX.
-000016a0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-000016b0: 6861 6e6e 656c 5f67 726f 7570 5f72 6567  hannel_group_reg
-000016c0: 6578 3a20 5061 7474 6572 6e20 3d20 5f43  ex: Pattern = _C
-000016d0: 4841 4e4e 454c 5f52 4547 4558 0d0a 0d0a  HANNEL_REGEX....
-000016e0: 2020 2020 2020 2020 2320 7573 6520 7765          # use we
-000016f0: 616b 7265 6620 746f 2061 766f 6964 2061  akref to avoid a
-00001700: 7465 7869 7420 6b65 6570 696e 6720 7573  texit keeping us
-00001710: 2066 726f 6d20 6265 696e 670d 0a20 2020   from being..   
-00001720: 2020 2020 2023 2067 6172 6261 6765 2063       # garbage c
-00001730: 6f6c 6c65 6374 6564 0d0a 2020 2020 2020  ollected..      
-00001740: 2020 7365 6c66 2e5f 7765 616b 5f63 6c65    self._weak_cle
-00001750: 616e 203d 2077 6561 6b72 6566 2e57 6561  an = weakref.Wea
-00001760: 6b4d 6574 686f 6428 7365 6c66 2e75 6e6c  kMethod(self.unl
-00001770: 6f61 6441 6c6c 4465 7669 6365 7329 0d0a  oadAllDevices)..
-00001780: 2020 2020 2020 2020 6174 6578 6974 2e72          atexit.r
-00001790: 6567 6973 7465 7228 7365 6c66 2e5f 7765  egister(self._we
-000017a0: 616b 5f63 6c65 616e 290d 0a0d 0a20 2020  ak_clean)....   
-000017b0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-000017c0: 6465 6620 6576 656e 7473 2873 656c 6629  def events(self)
-000017d0: 202d 3e20 5043 6f72 6553 6967 6e61 6c65   -> PCoreSignale
-000017e0: 723a 0d0a 2020 2020 2020 2020 2222 2253  r:..        """S
-000017f0: 6967 6e61 6c65 7220 666f 7220 636f 7265  ignaler for core
-00001800: 2065 7665 6e74 732e 0d0a 0d0a 2020 2020   events.....    
-00001810: 2020 2020 3a73 7061 726b 6c65 733a 202a      :sparkles: *
-00001820: 5468 6973 206d 6574 686f 6420 6973 206e  This method is n
-00001830: 6577 2069 6e20 6043 4d4d 436f 7265 506c  ew in `CMMCorePl
-00001840: 7573 602e 2a0d 0a0d 0a20 2020 2020 2020  us`.*....       
-00001850: 2054 6869 7320 6174 7472 6962 7574 6520   This attribute 
-00001860: 616c 6c6f 7773 2063 6f6e 6e65 6374 696e  allows connectin
-00001870: 6720 6361 6c6c 6261 636b 7320 746f 2076  g callbacks to v
-00001880: 6172 696f 7573 2065 7665 6e74 7320 7468  arious events th
-00001890: 6174 206f 6363 7572 2077 6974 6869 6e0d  at occur within.
-000018a0: 0a20 2020 2020 2020 2074 6865 2063 6f72  .        the cor
-000018b0: 652e 2053 6565 205b 6070 796d 6d63 6f72  e. See [`pymmcor
-000018c0: 655f 706c 7573 2e63 6f72 652e 6576 656e  e_plus.core.even
-000018d0: 7473 2e50 436f 7265 5369 676e 616c 6572  ts.PCoreSignaler
-000018e0: 605d 5b5d 2064 6f63 756d 656e 7461 7469  `][] documentati
-000018f0: 6f6e 2066 6f72 0d0a 2020 2020 2020 2020  on for..        
-00001900: 6465 7461 696c 7320 6f66 2074 6865 2061  details of the a
-00001910: 7661 696c 6162 6c65 2073 6967 6e61 6c73  vailable signals
-00001920: 2c20 616e 6420 686f 7720 746f 2063 6f6e  , and how to con
-00001930: 6e65 6374 2074 6f20 7468 656d 2e0d 0a20  nect to them... 
-00001940: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001950: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001960: 5f65 7665 6e74 730d 0a0d 0a20 2020 2064  _events....    d
-00001970: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
-00001980: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00001990: 2020 2072 6574 7572 6e20 6622 3c7b 7479     return f"<{ty
-000019a0: 7065 2873 656c 6629 2e5f 5f6e 616d 655f  pe(self).__name_
-000019b0: 5f7d 2061 7420 7b68 6578 2869 6428 7365  _} at {hex(id(se
-000019c0: 6c66 2929 7d3e 220d 0a0d 0a20 2020 2064  lf))}>"....    d
-000019d0: 6566 205f 5f64 656c 5f5f 2873 656c 6629  ef __del__(self)
-000019e0: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-000019f0: 2020 2061 7465 7869 742e 756e 7265 6769     atexit.unregi
-00001a00: 7374 6572 2873 656c 662e 5f77 6561 6b5f  ster(self._weak_
-00001a10: 636c 6561 6e29 0d0a 2020 2020 2020 2020  clean)..        
-00001a20: 7365 6c66 2e75 6e6c 6f61 6441 6c6c 4465  self.unloadAllDe
-00001a30: 7669 6365 7328 290d 0a0d 0a20 2020 2023  vices()....    #
-00001a40: 2052 652d 696d 706c 656d 656e 7465 6420   Re-implemented 
-00001a50: 6d65 7468 6f64 7320 6672 6f6d 2074 6865  methods from the
-00001a60: 2043 4d4d 436f 7265 2041 5049 0d0a 0d0a   CMMCore API....
-00001a70: 2020 2020 4073 796e 6368 726f 6e69 7a65      @synchronize
-00001a80: 6428 5f6c 6f63 6b29 0d0a 2020 2020 6465  d(_lock)..    de
-00001a90: 6620 7365 7450 726f 7065 7274 7928 0d0a  f setProperty(..
-00001aa0: 2020 2020 2020 2020 7365 6c66 2c20 6c61          self, la
-00001ab0: 6265 6c3a 2073 7472 2c20 7072 6f70 4e61  bel: str, propNa
-00001ac0: 6d65 3a20 7374 722c 2070 726f 7056 616c  me: str, propVal
-00001ad0: 7565 3a20 626f 6f6c 207c 2066 6c6f 6174  ue: bool | float
-00001ae0: 207c 2069 6e74 207c 2073 7472 0d0a 2020   | int | str..  
-00001af0: 2020 2920 2d3e 204e 6f6e 653a 0d0a 2020    ) -> None:..  
-00001b00: 2020 2020 2020 2222 2253 6574 2070 726f        """Set pro
-00001b10: 7065 7274 7920 6e61 6d65 6420 6070 726f  perty named `pro
-00001b20: 704e 616d 6560 206f 6e20 6465 7669 6365  pName` on device
-00001b30: 2060 6c61 6265 6c60 2074 6f20 6070 726f   `label` to `pro
-00001b40: 7056 616c 7565 602e 0d0a 0d0a 2020 2020  pValue`.....    
-00001b50: 2020 2020 2a2a 5768 7920 4f76 6572 7269      **Why Overri
-00001b60: 6465 3f2a 2a20 2049 6e20 604d 4d43 6f72  de?**  In `MMCor
-00001b70: 6560 2c20 7468 6520 6361 6c6c 696e 6720  e`, the calling 
-00001b80: 6f66 2074 6865 2060 6f6e 5072 6f70 6572  of the `onProper
-00001b90: 7479 4368 616e 6765 6460 0d0a 2020 2020  tyChanged`..    
-00001ba0: 2020 2020 6361 6c6c 6261 636b 2069 7320      callback is 
-00001bb0: 6c65 6674 2074 6f20 7468 6520 756e 6465  left to the unde
-00001bc0: 726c 7969 6e67 2064 6576 6963 6520 6164  rlying device ad
-00001bd0: 6170 7465 722c 2077 6869 6368 206d 6561  apter, which mea
-00001be0: 6e73 2069 7420 6973 206e 6f74 2061 6c77  ns it is not alw
-00001bf0: 6179 730d 0a20 2020 2020 2020 2063 616c  ays..        cal
-00001c00: 6c65 642e 2020 5468 6973 206d 6574 686f  led.  This metho
-00001c10: 6420 6f76 6572 7269 6465 7320 7468 6520  d overrides the 
-00001c20: 6465 6661 756c 7420 696d 706c 656d 656e  default implemen
-00001c30: 7461 7469 6f6e 2074 6f20 656e 7375 7265  tation to ensure
-00001c40: 2074 6861 740d 0a20 2020 2020 2020 2060   that..        `
-00001c50: 6576 656e 7473 2e70 726f 7065 7274 7943  events.propertyC
-00001c60: 6861 6e67 6564 6020 6973 202a 616c 7761  hanged` is *alwa
-00001c70: 7973 2a20 656d 6974 7465 6420 7768 656e  ys* emitted when
-00001c80: 2060 7365 7450 726f 7065 7274 7960 2068   `setProperty` h
-00001c90: 6173 2062 6565 6e20 6361 6c6c 6564 0d0a  as been called..
-00001ca0: 2020 2020 2020 2020 616e 6420 7468 6520          and the 
-00001cb0: 7072 6f70 6572 7479 2056 616c 7565 2068  property Value h
-00001cc0: 6173 2061 6374 7561 6c6c 7920 6368 616e  as actually chan
-00001cd0: 6765 642e 0d0a 2020 2020 2020 2020 2222  ged...        ""
-00001ce0: 220d 0a20 2020 2020 2020 2077 6974 6820  "..        with 
-00001cf0: 7365 6c66 2e5f 7072 6f70 6572 7479 5f63  self._property_c
-00001d00: 6861 6e67 655f 656d 6973 7369 6f6e 5f65  hange_emission_e
-00001d10: 6e73 7572 6564 286c 6162 656c 2c20 2870  nsured(label, (p
-00001d20: 726f 704e 616d 652c 2929 3a0d 0a20 2020  ropName,)):..   
-00001d30: 2020 2020 2020 2020 2073 7570 6572 2829           super()
-00001d40: 2e73 6574 5072 6f70 6572 7479 286c 6162  .setProperty(lab
-00001d50: 656c 2c20 7072 6f70 4e61 6d65 2c20 7072  el, propName, pr
-00001d60: 6f70 5661 6c75 6529 0d0a 0d0a 2020 2020  opValue)....    
-00001d70: 4073 796e 6368 726f 6e69 7a65 6428 5f6c  @synchronized(_l
-00001d80: 6f63 6b29 0d0a 2020 2020 6465 6620 7365  ock)..    def se
-00001d90: 7453 7461 7465 2873 656c 662c 2073 7461  tState(self, sta
-00001da0: 7465 4465 7669 6365 4c61 6265 6c3a 2073  teDeviceLabel: s
-00001db0: 7472 2c20 7374 6174 653a 2069 6e74 2920  tr, state: int) 
-00001dc0: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-00001dd0: 2020 2222 2253 6574 2073 7461 7465 2028    """Set state (
-00001de0: 6279 2070 6f73 6974 696f 6e29 206f 6e20  by position) on 
-00001df0: 6073 7461 7465 4465 7669 6365 4c61 6265  `stateDeviceLabe
-00001e00: 6c60 2c20 7769 7468 2072 656c 6961 626c  l`, with reliabl
-00001e10: 6520 6576 656e 7420 656d 6973 7369 6f6e  e event emission
-00001e20: 2e0d 0a0d 0a20 2020 2020 2020 202a 2a57  .....        **W
-00001e30: 6879 204f 7665 7272 6964 653f 2a2a 2020  hy Override?**  
-00001e40: 496e 2060 4d4d 436f 7265 602c 2074 6865  In `MMCore`, the
-00001e50: 2063 616c 6c69 6e67 206f 6620 7468 6520   calling of the 
-00001e60: 606f 6e50 726f 7065 7274 7943 6861 6e67  `onPropertyChang
-00001e70: 6564 600d 0a20 2020 2020 2020 2063 616c  ed`..        cal
-00001e80: 6c62 6163 6b20 6973 206c 6566 7420 746f  lback is left to
-00001e90: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-00001ea0: 6465 7669 6365 2061 6461 7074 6572 2c20  device adapter, 
-00001eb0: 7768 6963 6820 6d65 616e 7320 6974 2069  which means it i
-00001ec0: 7320 6e6f 7420 616c 7761 7973 0d0a 2020  s not always..  
-00001ed0: 2020 2020 2020 6361 6c6c 6564 2e20 2054        called.  T
-00001ee0: 6869 7320 6d65 7468 6f64 206f 7665 7272  his method overr
-00001ef0: 6964 6573 2074 6865 2064 6566 6175 6c74  ides the default
-00001f00: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00001f10: 746f 2065 6e73 7572 6520 7468 6174 0d0a  to ensure that..
-00001f20: 2020 2020 2020 2020 6065 7665 6e74 732e          `events.
-00001f30: 7072 6f70 6572 7479 4368 616e 6765 6460  propertyChanged`
-00001f40: 2069 7320 2a61 6c77 6179 732a 2065 6d69   is *always* emi
-00001f50: 7474 6564 2077 6865 6e20 6073 6574 5072  tted when `setPr
-00001f60: 6f70 6572 7479 6020 6861 7320 6265 656e  operty` has been
-00001f70: 2063 616c 6c65 640d 0a20 2020 2020 2020   called..       
-00001f80: 2061 6e64 2074 6865 2070 726f 7065 7274   and the propert
-00001f90: 7920 5661 6c75 6520 6861 7320 6163 7475  y Value has actu
-00001fa0: 616c 6c79 2063 6861 6e67 6564 2e0d 0a20  ally changed... 
-00001fb0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001fc0: 2020 2020 7769 7468 2073 656c 662e 5f70      with self._p
-00001fd0: 726f 7065 7274 795f 6368 616e 6765 5f65  roperty_change_e
-00001fe0: 6d69 7373 696f 6e5f 656e 7375 7265 6428  mission_ensured(
-00001ff0: 7374 6174 6544 6576 6963 654c 6162 656c  stateDeviceLabel
-00002000: 2c20 5354 4154 455f 5052 4f50 5329 3a0d  , STATE_PROPS):.
-00002010: 0a20 2020 2020 2020 2020 2020 2073 7570  .            sup
-00002020: 6572 2829 2e73 6574 5374 6174 6528 7374  er().setState(st
-00002030: 6174 6544 6576 6963 654c 6162 656c 2c20  ateDeviceLabel, 
-00002040: 7374 6174 6529 0d0a 0d0a 2020 2020 4073  state)....    @s
-00002050: 796e 6368 726f 6e69 7a65 6428 5f6c 6f63  ynchronized(_loc
-00002060: 6b29 0d0a 2020 2020 6465 6620 7365 7453  k)..    def setS
-00002070: 7461 7465 4c61 6265 6c28 7365 6c66 2c20  tateLabel(self, 
-00002080: 7374 6174 6544 6576 6963 654c 6162 656c  stateDeviceLabel
-00002090: 3a20 7374 722c 2073 7461 7465 4c61 6265  : str, stateLabe
-000020a0: 6c3a 2073 7472 2920 2d3e 204e 6f6e 653a  l: str) -> None:
-000020b0: 0d0a 2020 2020 2020 2020 2222 2253 6574  ..        """Set
-000020c0: 2073 7461 7465 2028 6279 206c 6162 656c   state (by label
-000020d0: 2920 6f6e 2060 7374 6174 6544 6576 6963  ) on `stateDevic
-000020e0: 654c 6162 656c 602c 2077 6974 6820 7265  eLabel`, with re
-000020f0: 6c69 6162 6c65 2065 7665 6e74 2065 6d69  liable event emi
-00002100: 7373 696f 6e2e 0d0a 0d0a 2020 2020 2020  ssion.....      
-00002110: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
-00002120: 3f2a 2a20 2049 6e20 604d 4d43 6f72 6560  ?**  In `MMCore`
-00002130: 2c20 7468 6520 6361 6c6c 696e 6720 6f66  , the calling of
-00002140: 2074 6865 2060 6f6e 5072 6f70 6572 7479   the `onProperty
-00002150: 4368 616e 6765 6460 0d0a 2020 2020 2020  Changed`..      
-00002160: 2020 6361 6c6c 6261 636b 2069 7320 6c65    callback is le
-00002170: 6674 2074 6f20 7468 6520 756e 6465 726c  ft to the underl
-00002180: 7969 6e67 2064 6576 6963 6520 6164 6170  ying device adap
-00002190: 7465 722c 2077 6869 6368 206d 6561 6e73  ter, which means
-000021a0: 2069 7420 6973 206e 6f74 2061 6c77 6179   it is not alway
-000021b0: 730d 0a20 2020 2020 2020 2063 616c 6c65  s..        calle
-000021c0: 642e 2020 5468 6973 206d 6574 686f 6420  d.  This method 
-000021d0: 6f76 6572 7269 6465 7320 7468 6520 6465  overrides the de
-000021e0: 6661 756c 7420 696d 706c 656d 656e 7461  fault implementa
-000021f0: 7469 6f6e 2074 6f20 656e 7375 7265 2074  tion to ensure t
-00002200: 6861 740d 0a20 2020 2020 2020 2060 6576  hat..        `ev
-00002210: 656e 7473 2e70 726f 7065 7274 7943 6861  ents.propertyCha
-00002220: 6e67 6564 6020 6973 202a 616c 7761 7973  nged` is *always
-00002230: 2a20 656d 6974 7465 6420 7768 656e 2060  * emitted when `
-00002240: 7365 7450 726f 7065 7274 7960 2068 6173  setProperty` has
-00002250: 2062 6565 6e20 6361 6c6c 6564 0d0a 2020   been called..  
-00002260: 2020 2020 2020 616e 6420 7468 6520 7072        and the pr
-00002270: 6f70 6572 7479 2056 616c 7565 2068 6173  operty Value has
-00002280: 2061 6374 7561 6c6c 7920 6368 616e 6765   actually change
-00002290: 642e 0d0a 2020 2020 2020 2020 2222 220d  d...        """.
-000022a0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000022b0: 6c66 2e5f 7072 6f70 6572 7479 5f63 6861  lf._property_cha
-000022c0: 6e67 655f 656d 6973 7369 6f6e 5f65 6e73  nge_emission_ens
-000022d0: 7572 6564 2873 7461 7465 4465 7669 6365  ured(stateDevice
-000022e0: 4c61 6265 6c2c 2053 5441 5445 5f50 524f  Label, STATE_PRO
-000022f0: 5053 293a 0d0a 2020 2020 2020 2020 2020  PS):..          
-00002300: 2020 7375 7065 7228 292e 7365 7453 7461    super().setSta
-00002310: 7465 4c61 6265 6c28 7374 6174 6544 6576  teLabel(stateDev
-00002320: 6963 654c 6162 656c 2c20 7374 6174 654c  iceLabel, stateL
-00002330: 6162 656c 290d 0a0d 0a20 2020 2064 6566  abel)....    def
-00002340: 2073 6574 4465 7669 6365 4164 6170 7465   setDeviceAdapte
-00002350: 7253 6561 7263 6850 6174 6873 2873 656c  rSearchPaths(sel
-00002360: 662c 2070 6174 6873 3a20 5365 7175 656e  f, paths: Sequen
-00002370: 6365 5b73 7472 5d29 202d 3e20 4e6f 6e65  ce[str]) -> None
-00002380: 3a0d 0a20 2020 2020 2020 2022 2222 5365  :..        """Se
-00002390: 7420 7468 6520 6465 7669 6365 2061 6461  t the device ada
-000023a0: 7074 6572 2073 6561 7263 6820 7061 7468  pter search path
-000023b0: 732e 0d0a 0d0a 2020 2020 2020 2020 2a2a  s.....        **
-000023c0: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
-000023d0: 2049 6e20 6361 7365 7320 7768 6572 6520   In cases where 
-000023e0: 4d4d 2064 6576 6963 6520 6164 6170 7465  MM device adapte
-000023f0: 7273 2075 7365 2064 796e 616d 6963 616c  rs use dynamical
-00002400: 6c79 206c 6f61 6465 640d 0a20 2020 2020  ly loaded..     
-00002410: 2020 206c 6962 7261 7269 6573 2c20 7468     libraries, th
-00002420: 6520 6465 7669 6365 2061 6461 7074 6572  e device adapter
-00002430: 2073 6561 7263 6820 7061 7468 7320 6d75   search paths mu
-00002440: 7374 2061 6c73 6f20 6265 2061 6464 6564  st also be added
-00002450: 2074 6f20 7468 6520 6050 4154 4860 0d0a   to the `PATH`..
-00002460: 2020 2020 2020 2020 656e 7669 726f 6e6d          environm
-00002470: 656e 7420 7661 7269 6162 6c65 2028 652e  ent variable (e.
-00002480: 672e 0d0a 2020 2020 2020 2020 3c68 7474  g...        <htt
-00002490: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000024a0: 6d69 6372 6f2d 6d61 6e61 6765 722f 7079  micro-manager/py
-000024b0: 6d6d 636f 7265 2f69 7373 7565 732f 3238  mmcore/issues/28
-000024c0: 3e29 2e20 5468 6973 206d 6574 686f 6420  >). This method 
-000024d0: 6f76 6572 7269 6465 730d 0a20 2020 2020  overrides..     
-000024e0: 2020 2074 6865 2064 6566 6175 6c74 2069     the default i
-000024f0: 6d70 6c65 6d65 6e74 6174 696f 6e20 746f  mplementation to
-00002500: 2065 6e73 7572 6520 7468 6174 2074 6865   ensure that the
-00002510: 2060 5041 5448 6020 656e 7669 726f 6e6d   `PATH` environm
-00002520: 656e 7420 7661 7269 6162 6c65 2069 730d  ent variable is.
-00002530: 0a20 2020 2020 2020 2075 7064 6174 6564  .        updated
-00002540: 2077 6865 6e20 7468 6520 6465 7669 6365   when the device
-00002550: 2061 6461 7074 6572 2073 6561 7263 6820   adapter search 
-00002560: 7061 7468 7320 6172 6520 6368 616e 6765  paths are change
-00002570: 642e 0d0a 2020 2020 2020 2020 2222 220d  d...        """.
-00002580: 0a20 2020 2020 2020 2023 2061 6464 2074  .        # add t
-00002590: 6f20 5041 5448 2061 7320 7765 6c6c 2066  o PATH as well f
-000025a0: 6f72 2064 796e 616d 6963 2064 6c6c 730d  or dynamic dlls.
-000025b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000025c0: 7061 7468 733a 0d0a 2020 2020 2020 2020  paths:..        
-000025d0: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
-000025e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000025f0: 6528 7061 7468 732c 2073 7472 2920 6f72  e(paths, str) or
-00002600: 2061 6e79 286e 6f74 2069 7369 6e73 7461   any(not isinsta
-00002610: 6e63 6528 702c 2073 7472 2920 666f 7220  nce(p, str) for 
-00002620: 7020 696e 2070 6174 6873 293a 0d0a 2020  p in paths):..  
-00002630: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00002640: 5479 7065 4572 726f 7228 2270 6174 6873  TypeError("paths
-00002650: 206d 7573 7420 6265 2061 2073 6571 7565   must be a seque
-00002660: 6e63 6520 6f66 2073 7472 696e 6773 2229  nce of strings")
-00002670: 0d0a 2020 2020 2020 2020 656e 765f 7061  ..        env_pa
-00002680: 7468 203d 206f 732e 656e 7669 726f 6e5b  th = os.environ[
-00002690: 2250 4154 4822 5d0d 0a20 2020 2020 2020  "PATH"]..       
-000026a0: 2066 6f72 2070 2069 6e20 7061 7468 733a   for p in paths:
-000026b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000026c0: 2070 206e 6f74 2069 6e20 656e 765f 7061   p not in env_pa
-000026d0: 7468 3a0d 0a20 2020 2020 2020 2020 2020  th:..           
-000026e0: 2020 2020 2065 6e76 5f70 6174 6820 3d20       env_path = 
-000026f0: 7020 2b20 6f73 2e70 6174 6873 6570 202b  p + os.pathsep +
-00002700: 2065 6e76 5f70 6174 680d 0a20 2020 2020   env_path..     
-00002710: 2020 206f 732e 656e 7669 726f 6e5b 2250     os.environ["P
-00002720: 4154 4822 5d20 3d20 656e 765f 7061 7468  ATH"] = env_path
-00002730: 0d0a 2020 2020 2020 2020 6c6f 6767 6572  ..        logger
-00002740: 2e64 6562 7567 2866 2273 6574 7469 6e67  .debug(f"setting
-00002750: 2061 6461 7074 6572 2073 6561 7263 6820   adapter search 
-00002760: 7061 7468 733a 207b 7061 7468 737d 2229  paths: {paths}")
-00002770: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00002780: 292e 7365 7444 6576 6963 6541 6461 7074  ).setDeviceAdapt
-00002790: 6572 5365 6172 6368 5061 7468 7328 7061  erSearchPaths(pa
-000027a0: 7468 7329 0d0a 0d0a 2020 2020 6465 6620  ths)....    def 
-000027b0: 6c6f 6164 4465 7669 6365 2873 656c 662c  loadDevice(self,
-000027c0: 206c 6162 656c 3a20 7374 722c 206d 6f64   label: str, mod
-000027d0: 756c 654e 616d 653a 2073 7472 2c20 6465  uleName: str, de
-000027e0: 7669 6365 4e61 6d65 3a20 7374 7229 202d  viceName: str) -
-000027f0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-00002800: 2022 2222 4c6f 6164 2061 2064 6576 6963   """Load a devic
-00002810: 6520 6672 6f6d 2074 6865 2070 6c75 6769  e from the plugi
-00002820: 6e20 6c69 6272 6172 792e 0d0a 0d0a 2020  n library.....  
-00002830: 2020 2020 2020 2a2a 5768 7920 4f76 6572        **Why Over
-00002840: 7269 6465 3f2a 2a20 546f 2061 6464 206d  ride?** To add m
-00002850: 7563 6820 6265 7474 6572 2065 7272 6f72  uch better error
-00002860: 206d 6573 7361 6765 7320 696e 2074 6865   messages in the
-00002870: 2063 6173 6520 6f66 2066 6169 6c75 7265   case of failure
-00002880: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00002890: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-000028a0: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-000028b0: 2020 2020 206c 6162 656c 3a20 7374 720d       label: str.
-000028c0: 0a20 2020 2020 2020 2020 2020 204e 616d  .            Nam
-000028d0: 6520 746f 2062 6520 6173 7369 676e 6564  e to be assigned
-000028e0: 2074 6f20 7468 6520 6465 7669 6365 2064   to the device d
-000028f0: 7572 696e 6720 7468 6973 2063 6f72 6520  uring this core 
-00002900: 7365 7373 696f 6e2e 0d0a 2020 2020 2020  session...      
-00002910: 2020 6d6f 6475 6c65 4e61 6d65 3a20 7374    moduleName: st
-00002920: 720d 0a20 2020 2020 2020 2020 2020 2054  r..            T
-00002930: 6865 206e 616d 6520 6f66 2074 6865 2064  he name of the d
-00002940: 6576 6963 6520 6164 6170 7465 7220 6d6f  evice adapter mo
-00002950: 6475 6c65 2028 7368 6f72 7420 6e61 6d65  dule (short name
-00002960: 2c20 6e6f 7420 6675 6c6c 2066 696c 6520  , not full file 
-00002970: 6e61 6d65 292e 0d0a 2020 2020 2020 2020  name)...        
-00002980: 2020 2020 5365 6520 5b60 7079 6d6d 636f      See [`pymmco
-00002990: 7265 2e43 4d4d 436f 7265 2e67 6574 4465  re.CMMCore.getDe
-000029a0: 7669 6365 4164 6170 7465 724e 616d 6573  viceAdapterNames
-000029b0: 605d 5b5d 2066 6f72 2061 206c 6973 7420  `][] for a list 
-000029c0: 6f66 2076 616c 6964 0d0a 2020 2020 2020  of valid..      
-000029d0: 2020 2020 2020 6d6f 6475 6c65 206e 616d        module nam
-000029e0: 6573 2e0d 0a20 2020 2020 2020 2064 6576  es...        dev
-000029f0: 6963 654e 616d 653a 2073 7472 0d0a 2020  iceName: str..  
-00002a00: 2020 2020 2020 2020 2020 7468 6520 6e61            the na
-00002a10: 6d65 206f 6620 7468 6520 6465 7669 6365  me of the device
-00002a20: 2e20 5468 6520 6e61 6d65 206d 7573 7420  . The name must 
-00002a30: 636f 7272 6573 706f 6e64 2074 6f20 6f6e  correspond to on
-00002a40: 6520 6f66 2074 6865 206e 616d 6573 0d0a  e of the names..
-00002a50: 2020 2020 2020 2020 2020 2020 7265 636f              reco
-00002a60: 676e 697a 6564 2062 7920 7468 6520 7370  gnized by the sp
-00002a70: 6563 6966 6963 2070 6c75 6769 6e20 6c69  ecific plugin li
-00002a80: 6272 6172 792e 2053 6565 0d0a 2020 2020  brary. See..    
-00002a90: 2020 2020 2020 2020 5b60 7079 6d6d 636f          [`pymmco
-00002aa0: 7265 2e43 4d4d 436f 7265 2e67 6574 4176  re.CMMCore.getAv
-00002ab0: 6169 6c61 626c 6544 6576 6963 6573 605d  ailableDevices`]
-00002ac0: 5b5d 2066 6f72 2061 206c 6973 7420 6f66  [] for a list of
-00002ad0: 2076 616c 6964 2064 6576 6963 6520 6e61   valid device na
-00002ae0: 6d65 732e 0d0a 2020 2020 2020 2020 2222  mes...        ""
-00002af0: 220d 0a20 2020 2020 2020 2074 7279 3a0d  "..        try:.
-00002b00: 0a20 2020 2020 2020 2020 2020 2073 7570  .            sup
-00002b10: 6572 2829 2e6c 6f61 6444 6576 6963 6528  er().loadDevice(
-00002b20: 6c61 6265 6c2c 206d 6f64 756c 654e 616d  label, moduleNam
-00002b30: 652c 2064 6576 6963 654e 616d 6529 0d0a  e, deviceName)..
-00002b40: 2020 2020 2020 2020 6578 6365 7074 2052          except R
-00002b50: 756e 7469 6d65 4572 726f 7220 6173 2065  untimeError as e
-00002b60: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
-00002b70: 7367 203d 2073 7472 2865 290d 0a20 2020  sg = str(e)..   
-00002b80: 2020 2020 2020 2020 2069 6620 6c61 6265           if labe
-00002b90: 6c20 696e 2073 656c 662e 6765 744c 6f61  l in self.getLoa
-00002ba0: 6465 6444 6576 6963 6573 2829 3a0d 0a20  dedDevices():.. 
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002bc0: 6962 203d 2073 7570 6572 2829 2e67 6574  ib = super().get
-00002bd0: 4465 7669 6365 4c69 6272 6172 7928 6c61  DeviceLibrary(la
-00002be0: 6265 6c29 0d0a 2020 2020 2020 2020 2020  bel)..          
-00002bf0: 2020 2020 2020 6e61 6d65 203d 2073 7570        name = sup
-00002c00: 6572 2829 2e67 6574 4465 7669 6365 4e61  er().getDeviceNa
-00002c10: 6d65 286c 6162 656c 290d 0a20 2020 2020  me(label)..     
-00002c20: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-00002c30: 6475 6c65 4e61 6d65 203d 3d20 6c69 6220  duleName == lib 
-00002c40: 616e 6420 6465 7669 6365 4e61 6d65 203d  and deviceName =
-00002c50: 3d20 6e61 6d65 3a0d 0a20 2020 2020 2020  = name:..       
-00002c60: 2020 2020 2020 2020 2020 2020 206d 7367               msg
-00002c70: 202b 3d20 6622 2e20 4465 7669 6365 207b   += f". Device {
-00002c80: 6c61 6265 6c21 727d 2061 7070 6561 7273  label!r} appears
-00002c90: 2074 6f20 6265 206c 6f61 6465 6420 616c   to be loaded al
-00002ca0: 7265 6164 792e 220d 0a20 2020 2020 2020  ready."..       
-00002cb0: 2020 2020 2020 2020 2020 2020 2077 6172               war
-00002cc0: 6e69 6e67 732e 7761 726e 286d 7367 2c20  nings.warn(msg, 
-00002cd0: 7374 6163 6b6c 6576 656c 3d32 290d 0a20  stacklevel=2).. 
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cf0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-00002d00: 2020 2020 2020 2020 2020 2020 206d 7367               msg
-00002d10: 202b 3d20 6622 2e20 4465 7669 6365 207b   += f". Device {
-00002d20: 6c61 6265 6c21 727d 2069 7320 616c 7265  label!r} is alre
-00002d30: 6164 7920 7461 6b65 6e20 6279 207b 6c69  ady taken by {li
-00002d40: 627d 3a3a 7b6e 616d 657d 220d 0a20 2020  b}::{name}"..   
-00002d50: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 6164 6170 7465 7273 203d 2073 7570 6572  adapters = super
-00002d80: 2829 2e67 6574 4465 7669 6365 4164 6170  ().getDeviceAdap
-00002d90: 7465 724e 616d 6573 2829 0d0a 2020 2020  terNames()..    
-00002da0: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00002db0: 6f64 756c 654e 616d 6520 6e6f 7420 696e  oduleName not in
-00002dc0: 2061 6461 7074 6572 733a 0d0a 2020 2020   adapters:..    
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 6d73 6720 2b3d 2028 0d0a 2020 2020 2020  msg += (..      
-00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e00: 2020 6622 2e20 4164 6170 7465 7220 6e61    f". Adapter na
-00002e10: 6d65 207b 6d6f 6475 6c65 4e61 6d65 2172  me {moduleName!r
-00002e20: 7d20 6e6f 7420 696e 206c 6973 7420 6f66  } not in list of
-00002e30: 206b 6e6f 776e 2061 6461 7074 6572 2022   known adapter "
-00002e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e50: 2020 2020 2020 2020 2020 6622 6e61 6d65            f"name
-00002e60: 733a 207b 6164 6170 7465 7273 7d2e 220d  s: {adapters}.".
-00002e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e80: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00002e90: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002eb0: 2020 2064 6576 6963 6573 203d 2073 7570     devices = sup
-00002ec0: 6572 2829 2e67 6574 4176 6169 6c61 626c  er().getAvailabl
-00002ed0: 6544 6576 6963 6573 286d 6f64 756c 654e  eDevices(moduleN
-00002ee0: 616d 6529 0d0a 2020 2020 2020 2020 2020  ame)..          
-00002ef0: 2020 2020 2020 2020 2020 6966 2064 6576            if dev
-00002f00: 6963 654e 616d 6520 6e6f 7420 696e 2064  iceName not in d
-00002f10: 6576 6963 6573 3a0d 0a20 2020 2020 2020  evices:..       
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 206d 7367 202b 3d20 280d 0a20 2020 2020   msg += (..     
+00000220: 726f 6d20 7079 6d6d 636f 7265 5f70 6c75  rom pymmcore_plu
+00000230: 732e 5f6c 6f67 6765 7220 696d 706f 7274  s._logger import
+00000240: 2063 7572 7265 6e74 5f6c 6f67 6669 6c65   current_logfile
+00000250: 2c20 6c6f 6767 6572 0d0a 6672 6f6d 2070  , logger..from p
+00000260: 796d 6d63 6f72 655f 706c 7573 2e5f 7574  ymmcore_plus._ut
+00000270: 696c 2069 6d70 6f72 7420 6669 6e64 5f6d  il import find_m
+00000280: 6963 726f 6d61 6e61 6765 722c 2070 7269  icromanager, pri
+00000290: 6e74 5f74 6162 756c 6172 5f64 6174 610d  nt_tabular_data.
+000002a0: 0a66 726f 6d20 7079 6d6d 636f 7265 5f70  .from pymmcore_p
+000002b0: 6c75 732e 6d64 6120 696d 706f 7274 204d  lus.mda import M
+000002c0: 4441 456e 6769 6e65 2c20 4d44 4152 756e  DAEngine, MDARun
+000002d0: 6e65 722c 2050 4d44 4145 6e67 696e 650d  ner, PMDAEngine.
+000002e0: 0a0d 0a66 726f 6d20 2e5f 6164 6170 7465  ...from ._adapte
+000002f0: 7220 696d 706f 7274 2044 6576 6963 6541  r import DeviceA
+00000300: 6461 7074 6572 0d0a 6672 6f6d 202e 5f63  dapter..from ._c
+00000310: 6f6e 6669 6720 696d 706f 7274 2043 6f6e  onfig import Con
+00000320: 6669 6775 7261 7469 6f6e 0d0a 6672 6f6d  figuration..from
+00000330: 202e 5f63 6f6e 6669 675f 6772 6f75 7020   ._config_group 
+00000340: 696d 706f 7274 2043 6f6e 6669 6747 726f  import ConfigGro
+00000350: 7570 0d0a 6672 6f6d 202e 5f63 6f6e 7374  up..from ._const
+00000360: 616e 7473 2069 6d70 6f72 7420 4465 7669  ants import Devi
+00000370: 6365 4465 7465 6374 696f 6e53 7461 7475  ceDetectionStatu
+00000380: 732c 2044 6576 6963 6554 7970 652c 2050  s, DeviceType, P
+00000390: 726f 7065 7274 7954 7970 650d 0a66 726f  ropertyType..fro
+000003a0: 6d20 2e5f 6465 7669 6365 2069 6d70 6f72  m ._device impor
+000003b0: 7420 4465 7669 6365 0d0a 6672 6f6d 202e  t Device..from .
+000003c0: 5f6d 6574 6164 6174 6120 696d 706f 7274  _metadata import
+000003d0: 204d 6574 6164 6174 610d 0a66 726f 6d20   Metadata..from 
+000003e0: 2e5f 7072 6f70 6572 7479 2069 6d70 6f72  ._property impor
+000003f0: 7420 4465 7669 6365 5072 6f70 6572 7479  t DeviceProperty
+00000400: 0d0a 6672 6f6d 202e 5f73 6571 7565 6e63  ..from ._sequenc
+00000410: 696e 6720 696d 706f 7274 2063 616e 5f73  ing import can_s
+00000420: 6571 7565 6e63 655f 6576 656e 7473 0d0a  equence_events..
+00000430: 6672 6f6d 202e 6576 656e 7473 2069 6d70  from .events imp
+00000440: 6f72 7420 434d 4d43 6f72 6553 6967 6e61  ort CMMCoreSigna
+00000450: 6c65 722c 2050 436f 7265 5369 676e 616c  ler, PCoreSignal
+00000460: 6572 2c20 5f67 6574 5f61 7574 6f5f 636f  er, _get_auto_co
+00000470: 7265 5f63 616c 6c62 6163 6b5f 636c 6173  re_callback_clas
+00000480: 730d 0a0d 0a69 6620 5459 5045 5f43 4845  s....if TYPE_CHE
+00000490: 434b 494e 473a 0d0a 2020 2020 696d 706f  CKING:..    impo
+000004a0: 7274 206e 756d 7079 2061 7320 6e70 0d0a  rt numpy as np..
+000004b0: 2020 2020 6672 6f6d 2074 7970 696e 675f      from typing_
+000004c0: 6578 7465 6e73 696f 6e73 2069 6d70 6f72  extensions impor
+000004d0: 7420 4c69 7465 7261 6c2c 2054 7970 6564  t Literal, Typed
+000004e0: 4469 6374 0d0a 2020 2020 6672 6f6d 2075  Dict..    from u
+000004f0: 7365 7120 696d 706f 7274 204d 4441 4576  seq import MDAEv
+00000500: 656e 740d 0a0d 0a20 2020 205f 5420 3d20  ent....    _T = 
+00000510: 5479 7065 5661 7228 225f 5422 290d 0a20  TypeVar("_T").. 
+00000520: 2020 205f 4620 3d20 5479 7065 5661 7228     _F = TypeVar(
+00000530: 225f 4622 2c20 626f 756e 643d 4361 6c6c  "_F", bound=Call
+00000540: 6162 6c65 5b2e 2e2e 2c20 416e 795d 290d  able[..., Any]).
+00000550: 0a20 2020 204c 6973 744f 7254 7570 6c65  .    ListOrTuple
+00000560: 203d 206c 6973 745b 5f54 5d20 7c20 7475   = list[_T] | tu
+00000570: 706c 655b 5f54 2c20 2e2e 2e5d 0d0a 0d0a  ple[_T, ...]....
+00000580: 2020 2020 636c 6173 7320 5374 6174 6544      class StateD
+00000590: 6963 7428 5479 7065 6444 6963 742c 2074  ict(TypedDict, t
+000005a0: 6f74 616c 3d46 616c 7365 293a 0d0a 2020  otal=False):..  
+000005b0: 2020 2020 2020 2222 2244 6963 7469 6f6e        """Diction
+000005c0: 6172 7920 6f66 2073 7461 7465 2076 616c  ary of state val
+000005d0: 7565 7320 666f 7220 6120 6465 7669 6365  ues for a device
+000005e0: 2e0d 0a0d 0a20 2020 2020 2020 2054 6869  .....        Thi
+000005f0: 7320 6f62 6a65 6374 2073 686f 756c 6420  s object should 
+00000600: 6f6e 6c79 2062 6520 696d 706f 7274 6564  only be imported
+00000610: 2069 6e73 6964 6520 6120 6054 5950 455f   inside a `TYPE_
+00000620: 4348 4543 4b49 4e47 6020 626c 6f63 6b2e  CHECKING` block.
+00000630: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+00000640: 0a20 2020 2020 2020 2041 7574 6f46 6f63  .        AutoFoc
+00000650: 7573 4465 7669 6365 3a20 7374 720d 0a20  usDevice: str.. 
+00000660: 2020 2020 2020 2042 7974 6573 5065 7250         BytesPerP
+00000670: 6978 656c 3a20 696e 740d 0a20 2020 2020  ixel: int..     
+00000680: 2020 2043 616d 6572 6143 6861 6e6e 656c     CameraChannel
+00000690: 4e61 6d65 733a 2074 7570 6c65 5b73 7472  Names: tuple[str
+000006a0: 2c20 2e2e 2e5d 0d0a 2020 2020 2020 2020  , ...]..        
+000006b0: 4361 6d65 7261 4465 7669 6365 3a20 7374  CameraDevice: st
+000006c0: 720d 0a20 2020 2020 2020 2044 6174 6574  r..        Datet
+000006d0: 696d 653a 2073 7472 0d0a 2020 2020 2020  ime: str..      
+000006e0: 2020 4578 706f 7375 7265 3a20 666c 6f61    Exposure: floa
+000006f0: 740d 0a20 2020 2020 2020 2046 6f63 7573  t..        Focus
+00000700: 4465 7669 6365 3a20 7374 720d 0a20 2020  Device: str..   
+00000710: 2020 2020 2047 616c 766f 4465 7669 6365       GalvoDevice
+00000720: 3a20 7374 720d 0a20 2020 2020 2020 2049  : str..        I
+00000730: 6d61 6765 4269 7444 6570 7468 3a20 696e  mageBitDepth: in
+00000740: 740d 0a20 2020 2020 2020 2049 6d61 6765  t..        Image
+00000750: 4865 6967 6874 3a20 696e 740d 0a20 2020  Height: int..   
+00000760: 2020 2020 2049 6d61 6765 5072 6f63 6573       ImageProces
+00000770: 736f 7244 6576 6963 653a 2073 7472 0d0a  sorDevice: str..
+00000780: 2020 2020 2020 2020 496d 6167 6557 6964          ImageWid
+00000790: 7468 3a20 696e 740d 0a20 2020 2020 2020  th: int..       
+000007a0: 2050 6978 656c 5369 7a65 556d 3a20 666c   PixelSizeUm: fl
+000007b0: 6f61 740d 0a20 2020 2020 2020 2053 6875  oat..        Shu
+000007c0: 7474 6572 4465 7669 6365 3a20 7374 720d  tterDevice: str.
+000007d0: 0a20 2020 2020 2020 2053 4c4d 4465 7669  .        SLMDevi
+000007e0: 6365 3a20 7374 720d 0a20 2020 2020 2020  ce: str..       
+000007f0: 2058 5950 6f73 6974 696f 6e3a 2074 7570   XYPosition: tup
+00000800: 6c65 5b66 6c6f 6174 2c20 666c 6f61 745d  le[float, float]
+00000810: 0d0a 2020 2020 2020 2020 5859 5374 6167  ..        XYStag
+00000820: 6544 6576 6963 653a 2073 7472 0d0a 2020  eDevice: str..  
+00000830: 2020 2020 2020 5a50 6f73 6974 696f 6e3a        ZPosition:
+00000840: 2066 6c6f 6174 0d0a 0d0a 2020 2020 636c   float....    cl
+00000850: 6173 7320 5072 6f70 6572 7479 5363 6865  ass PropertySche
+00000860: 6d61 2854 7970 6564 4469 6374 2c20 746f  ma(TypedDict, to
+00000870: 7461 6c3d 4661 6c73 6529 3a0d 0a20 2020  tal=False):..   
+00000880: 2020 2020 2022 2222 4a53 4f4e 2073 6368       """JSON sch
+00000890: 656d 6120 6064 6963 7460 2064 6573 6372  ema `dict` descr
+000008a0: 6962 696e 6720 6120 6465 7669 6365 2070  ibing a device p
+000008b0: 726f 7065 7274 792e 2222 220d 0a0d 0a20  roperty.""".... 
+000008c0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+000008d0: 0d0a 2020 2020 2020 2020 6d61 7869 6d75  ..        maximu
+000008e0: 6d3a 2066 6c6f 6174 0d0a 2020 2020 2020  m: float..      
+000008f0: 2020 6d69 6e69 6d75 6d3a 2066 6c6f 6174    minimum: float
+00000900: 0d0a 2020 2020 2020 2020 656e 756d 3a20  ..        enum: 
+00000910: 6c69 7374 0d0a 2020 2020 2020 2020 7265  list..        re
+00000920: 6164 4f6e 6c79 3a20 626f 6f6c 0d0a 2020  adOnly: bool..  
+00000930: 2020 2020 2020 6465 6661 756c 743a 2041        default: A
+00000940: 6e79 0d0a 2020 2020 2020 2020 7365 7175  ny..        sequ
+00000950: 656e 6365 6162 6c65 3a20 626f 6f6c 0d0a  enceable: bool..
+00000960: 2020 2020 2020 2020 7365 7175 656e 6365          sequence
+00000970: 4d61 784c 656e 6774 683a 2069 6e74 0d0a  MaxLength: int..
+00000980: 2020 2020 2020 2020 7072 6549 6e69 743a          preInit:
+00000990: 2062 6f6f 6c0d 0a0d 0a20 2020 2063 6c61   bool....    cla
+000009a0: 7373 2044 6576 6963 6553 6368 656d 6128  ss DeviceSchema(
+000009b0: 5479 7065 6444 6963 7429 3a0d 0a20 2020  TypedDict):..   
+000009c0: 2020 2020 2022 2222 4a53 4f4e 2073 6368       """JSON sch
+000009d0: 656d 6120 6064 6963 7460 2064 6573 6372  ema `dict` descr
+000009e0: 6962 696e 6720 6120 6465 7669 6365 2e22  ibing a device."
+000009f0: 2222 0d0a 0d0a 2020 2020 2020 2020 7469  ""....        ti
+00000a00: 746c 653a 2073 7472 0d0a 2020 2020 2020  tle: str..      
+00000a10: 2020 6465 7363 7269 7074 696f 6e3a 2073    description: s
+00000a20: 7472 0d0a 2020 2020 2020 2020 7479 7065  tr..        type
+00000a30: 3a20 7374 720d 0a20 2020 2020 2020 2070  : str..        p
+00000a40: 726f 7065 7274 6965 733a 2064 6963 745b  roperties: dict[
+00000a50: 7374 722c 2050 726f 7065 7274 7953 6368  str, PropertySch
+00000a60: 656d 615d 0d0a 0d0a 2020 2020 6465 6620  ema]....    def 
+00000a70: 7379 6e63 6872 6f6e 697a 6564 286c 6f63  synchronized(loc
+00000a80: 6b3a 2052 4c6f 636b 2920 2d3e 2043 616c  k: RLock) -> Cal
+00000a90: 6c61 626c 655b 5b5f 465d 2c20 5f46 5d3a  lable[[_F], _F]:
+00000aa0: 0d0a 2020 2020 2020 2020 2e2e 2e0d 0a0d  ..        ......
+00000ab0: 0a65 6c73 653a 0d0a 2020 2020 6672 6f6d  .else:..    from
+00000ac0: 2077 7261 7074 2069 6d70 6f72 7420 7379   wrapt import sy
+00000ad0: 6e63 6872 6f6e 697a 6564 0d0a 0d0a 5f4f  nchronized...._O
+00000ae0: 424a 4445 565f 5245 4745 5820 3d20 7265  BJDEV_REGEX = re
+00000af0: 2e63 6f6d 7069 6c65 2822 282e 2b29 3f28  .compile("(.+)?(
+00000b00: 6e6f 7365 7069 6563 657c 6f62 6a28 6563  nosepiece|obj(ec
+00000b10: 7469 7665 293f 2928 7475 7272 6574 293f  tive)?)(turret)?
+00000b20: 733f 222c 2072 652e 4947 4e4f 5245 4341  s?", re.IGNORECA
+00000b30: 5345 290d 0a5f 4348 414e 4e45 4c5f 5245  SE).._CHANNEL_RE
+00000b40: 4745 5820 3d20 7265 2e63 6f6d 7069 6c65  GEX = re.compile
+00000b50: 2822 2863 6861 6e7b 312c 327d 2865 6c29  ("(chan{1,2}(el)
+00000b60: 3f7c 6669 6c74 2865 7229 3f29 733f 222c  ?|filt(er)?)s?",
+00000b70: 2072 652e 4947 4e4f 5245 4341 5345 290d   re.IGNORECASE).
+00000b80: 0a0d 0a53 5441 5445 203d 2070 796d 6d63  ...STATE = pymmc
+00000b90: 6f72 652e 675f 4b65 7977 6f72 645f 5374  ore.g_Keyword_St
+00000ba0: 6174 650d 0a4c 4142 454c 203d 2070 796d  ate..LABEL = pym
+00000bb0: 6d63 6f72 652e 675f 4b65 7977 6f72 645f  mcore.g_Keyword_
+00000bc0: 4c61 6265 6c0d 0a53 5441 5445 5f50 524f  Label..STATE_PRO
+00000bd0: 5053 203d 2028 5354 4154 452c 204c 4142  PS = (STATE, LAB
+00000be0: 454c 290d 0a55 4e4e 414d 4544 5f50 5245  EL)..UNNAMED_PRE
+00000bf0: 5345 5420 3d20 224e 6577 5072 6573 6574  SET = "NewPreset
+00000c00: 220d 0a0d 0a0d 0a40 636f 6e74 6578 746d  "......@contextm
+00000c10: 616e 6167 6572 0d0a 6465 6620 5f62 6c6f  anager..def _blo
+00000c20: 636b 5369 676e 616c 286f 626a 3a20 416e  ckSignal(obj: An
+00000c30: 792c 2073 6967 6e61 6c3a 2041 6e79 2920  y, signal: Any) 
+00000c40: 2d3e 2049 7465 7261 746f 725b 4e6f 6e65  -> Iterator[None
+00000c50: 5d3a 0d0a 2020 2020 6966 2069 7369 6e73  ]:..    if isins
+00000c60: 7461 6e63 6528 7369 676e 616c 2c20 5369  tance(signal, Si
+00000c70: 676e 616c 496e 7374 616e 6365 293a 0d0a  gnalInstance):..
+00000c80: 2020 2020 2020 2020 7369 676e 616c 2e62          signal.b
+00000c90: 6c6f 636b 2829 0d0a 2020 2020 2020 2020  lock()..        
+00000ca0: 7969 656c 640d 0a20 2020 2020 2020 2073  yield..        s
+00000cb0: 6967 6e61 6c2e 756e 626c 6f63 6b28 290d  ignal.unblock().
+00000cc0: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
+00000cd0: 2020 2020 6f62 6a2e 626c 6f63 6b53 6967      obj.blockSig
+00000ce0: 6e61 6c73 2854 7275 6529 0d0a 2020 2020  nals(True)..    
+00000cf0: 2020 2020 7969 656c 640d 0a20 2020 2020      yield..     
+00000d00: 2020 206f 626a 2e62 6c6f 636b 5369 676e     obj.blockSign
+00000d10: 616c 7328 4661 6c73 6529 0d0a 0d0a 0d0a  als(False)......
+00000d20: 5f69 6e73 7461 6e63 6520 3d20 4e6f 6e65  _instance = None
+00000d30: 0d0a 0d0a 0d0a 636c 6173 7320 434d 4d43  ......class CMMC
+00000d40: 6f72 6550 6c75 7328 7079 6d6d 636f 7265  orePlus(pymmcore
+00000d50: 2e43 4d4d 436f 7265 293a 0d0a 2020 2020  .CMMCore):..    
+00000d60: 2222 2257 7261 7070 6572 2066 6f72 2043  """Wrapper for C
+00000d70: 4d4d 436f 7265 2077 6974 6820 6578 7465  MMCore with exte
+00000d80: 6e64 6564 2066 756e 6374 696f 6e61 6c69  nded functionali
+00000d90: 7479 2e0d 0a0d 0a20 2020 2050 6172 616d  ty.....    Param
+00000da0: 6574 6572 730d 0a20 2020 202d 2d2d 2d2d  eters..    -----
+00000db0: 2d2d 2d2d 2d0d 0a20 2020 206d 6d5f 7061  -----..    mm_pa
+00000dc0: 7468 203a 2073 7472 207c 204e 6f6e 652c  th : str | None,
+00000dd0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00000de0: 2020 2050 6174 6820 746f 2074 6865 204d     Path to the M
+00000df0: 6963 726f 2d4d 616e 6167 6572 2069 6e73  icro-Manager ins
+00000e00: 7461 6c6c 6174 696f 6e2e 2049 6620 604e  tallation. If `N
+00000e10: 6f6e 6560 2028 6465 6661 756c 7429 2c20  one` (default), 
+00000e20: 7769 6c6c 2075 7365 2074 6865 0d0a 2020  will use the..  
+00000e30: 2020 2020 2020 7265 7475 726e 2076 616c        return val
+00000e40: 7565 206f 6620 5b60 7079 6d6d 636f 7265  ue of [`pymmcore
+00000e50: 5f70 6c75 732e 6669 6e64 5f6d 6963 726f  _plus.find_micro
+00000e60: 6d61 6e61 6765 7260 5d5b 5d2e 0d0a 2020  manager`][]...  
+00000e70: 2020 6164 6170 7465 725f 7061 7468 7320    adapter_paths 
+00000e80: 3a20 5365 7175 656e 6365 5b73 7472 5d2c  : Sequence[str],
+00000e90: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00000ea0: 2020 2050 6174 6873 2074 6f20 7365 6172     Paths to sear
+00000eb0: 6368 2066 6f72 2064 6576 6963 6520 6164  ch for device ad
+00000ec0: 6170 7465 7273 2c20 6279 2064 6566 6175  apters, by defau
+00000ed0: 6c74 2028 290d 0a20 2020 2022 2222 0d0a  lt ()..    """..
+00000ee0: 0d0a 2020 2020 5f6c 6f63 6b20 3d20 524c  ..    _lock = RL
+00000ef0: 6f63 6b28 290d 0a0d 0a20 2020 2040 636c  ock()....    @cl
+00000f00: 6173 736d 6574 686f 640d 0a20 2020 2064  assmethod..    d
+00000f10: 6566 2069 6e73 7461 6e63 6528 636c 7329  ef instance(cls)
+00000f20: 202d 3e20 434d 4d43 6f72 6550 6c75 733a   -> CMMCorePlus:
+00000f30: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00000f40: 7572 6e20 7468 6520 676c 6f62 616c 2073  urn the global s
+00000f50: 696e 676c 6574 6f6e 2069 6e73 7461 6e63  ingleton instanc
+00000f60: 6520 6f66 2060 434d 4d43 6f72 6550 6c75  e of `CMMCorePlu
+00000f70: 7360 2e0d 0a0d 0a20 2020 2020 2020 203a  s`.....        :
+00000f80: 7370 6172 6b6c 6573 3a20 2a54 6869 7320  sparkles: *This 
+00000f90: 6d65 7468 6f64 2069 7320 6e65 7720 696e  method is new in
+00000fa0: 2060 434d 4d43 6f72 6550 6c75 7360 2e2a   `CMMCorePlus`.*
+00000fb0: 0d0a 0d0a 2020 2020 2020 2020 496e 206d  ....        In m
+00000fc0: 616e 7920 6361 7365 732c 2061 2073 696e  any cases, a sin
+00000fd0: 676c 6520 696e 7374 616e 6365 206f 6620  gle instance of 
+00000fe0: 6043 4d4d 436f 7265 506c 7573 6020 6973  `CMMCorePlus` is
+00000ff0: 2061 6c6c 2074 6861 7420 7769 6c6c 2062   all that will b
+00001000: 6520 6372 6561 7465 640d 0a20 2020 2020  e created..     
+00001010: 2020 2069 6e20 6120 6769 7665 6e20 7365     in a given se
+00001020: 7373 696f 6e2e 2020 5468 6973 2063 6c61  ssion.  This cla
+00001030: 7373 206d 6574 686f 6420 7072 6f76 6964  ss method provid
+00001040: 6573 2061 2063 6f6e 7665 6e69 656e 7420  es a convenient 
+00001050: 7761 7920 746f 2061 6363 6573 730d 0a20  way to access.. 
+00001060: 2020 2020 2020 2074 6861 7420 696e 7374         that inst
+00001070: 616e 6365 2e0d 0a0d 0a20 2020 2020 2020  ance.....       
+00001080: 2021 2121 2074 6970 0d0a 0d0a 2020 2020   !!! tip....    
+00001090: 2020 2020 2020 2020 4372 6561 7469 6e67          Creating
+000010a0: 2f61 6363 6573 7369 6e67 2061 2060 434d  /accessing a `CM
+000010b0: 4d43 6f72 6550 6c75 7360 206f 626a 6563  MCorePlus` objec
+000010c0: 7420 7573 696e 6720 6043 4d4d 436f 7265  t using `CMMCore
+000010d0: 506c 7573 2e69 6e73 7461 6e63 6528 2960  Plus.instance()`
+000010e0: 2069 730d 0a20 2020 2020 2020 2020 2020   is..           
+000010f0: 2061 2063 6f6e 7665 6e69 656e 7420 7761   a convenient wa
+00001100: 7920 746f 2061 6363 6573 7320 7468 6520  y to access the 
+00001110: 7361 6d65 2063 6f72 6520 696e 7374 616e  same core instan
+00001120: 6365 2066 726f 6d20 6d75 6c74 6970 6c65  ce from multiple
+00001130: 2070 6c61 6365 7320 696e 0d0a 2020 2020   places in..    
+00001140: 2020 2020 2020 2020 796f 7572 2063 6f64          your cod
+00001150: 652e 2041 6c6c 2077 6964 6765 7473 2069  e. All widgets i
+00001160: 6e0d 0a20 2020 2020 2020 2020 2020 205b  n..            [
+00001170: 6070 796d 6d63 6f72 652d 7769 6467 6574  `pymmcore-widget
+00001180: 7360 5d28 6874 7470 733a 2f2f 6769 7468  s`](https://gith
+00001190: 7562 2e63 6f6d 2f70 796d 6d63 6f72 652d  ub.com/pymmcore-
+000011a0: 706c 7573 2f70 796d 6d63 6f72 652d 7769  plus/pymmcore-wi
+000011b0: 6467 6574 7329 2061 6c73 6f0d 0a20 2020  dgets) also..   
+000011c0: 2020 2020 2020 2020 2075 7365 2060 434d           use `CM
+000011d0: 4d43 6f72 6550 6c75 732e 696e 7374 616e  MCorePlus.instan
+000011e0: 6365 2829 6020 6279 2064 6566 6175 6c74  ce()` by default
+000011f0: 2c20 736f 2061 6e79 2077 6964 6765 7473  , so any widgets
+00001200: 2079 6f75 2075 7365 2077 696c 6c0d 0a20   you use will.. 
+00001210: 2020 2020 2020 2020 2020 2061 7574 6f6d             autom
+00001220: 6174 6963 616c 6c79 2063 6f6e 6e65 6374  atically connect
+00001230: 2074 6f20 7468 6520 7361 6d65 2063 6f72   to the same cor
+00001240: 6520 696e 7374 616e 6365 2077 6974 686f  e instance witho
+00001250: 7574 2061 6e79 2061 6464 6974 696f 6e61  ut any additiona
+00001260: 6c0d 0a20 2020 2020 2020 2020 2020 2063  l..            c
+00001270: 6f6e 6669 6775 7261 7469 6f6e 2e0d 0a0d  onfiguration....
+00001280: 0a20 2020 2020 2020 2020 2020 2041 7474  .            Att
+00001290: 656d 7074 7320 2a61 7265 2a20 6d61 6465  empts *are* made
+000012a0: 2074 6f20 6d61 6b65 2069 7420 7468 7265   to make it thre
+000012b0: 6164 2d73 6166 652e 2020 4275 7420 706c  ad-safe.  But pl
+000012c0: 6561 7365 206f 7065 6e20 616e 2069 7373  ease open an iss
+000012d0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+000012e0: 6966 2079 6f75 2066 696e 6420 616e 7920  if you find any 
+000012f0: 7072 6f62 6c65 6d73 2e0d 0a0d 0a0d 0a20  problems....... 
+00001300: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00001310: 2020 2020 676c 6f62 616c 205f 696e 7374      global _inst
+00001320: 616e 6365 0d0a 2020 2020 2020 2020 6966  ance..        if
+00001330: 205f 696e 7374 616e 6365 2069 7320 4e6f   _instance is No
+00001340: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00001350: 205f 696e 7374 616e 6365 203d 2063 6c73   _instance = cls
+00001360: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
+00001370: 726e 205f 696e 7374 616e 6365 0d0a 0d0a  rn _instance....
+00001380: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001390: 2873 656c 662c 206d 6d5f 7061 7468 3a20  (self, mm_path: 
+000013a0: 7374 7220 7c20 4e6f 6e65 203d 204e 6f6e  str | None = Non
+000013b0: 652c 2061 6461 7074 6572 5f70 6174 6873  e, adapter_paths
+000013c0: 3a20 5365 7175 656e 6365 5b73 7472 5d20  : Sequence[str] 
+000013d0: 3d20 2829 293a 0d0a 2020 2020 2020 2020  = ()):..        
+000013e0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+000013f0: 2829 0d0a 0d0a 2020 2020 2020 2020 6966  ()....        if
+00001400: 206c 6f67 6669 6c65 203a 3d20 6375 7272   logfile := curr
+00001410: 656e 745f 6c6f 6766 696c 6528 6c6f 6767  ent_logfile(logg
+00001420: 6572 293a 0d0a 2020 2020 2020 2020 2020  er):..          
+00001430: 2020 7365 6c66 2e73 6574 5072 696d 6172    self.setPrimar
+00001440: 794c 6f67 4669 6c65 2873 7472 286c 6f67  yLogFile(str(log
+00001450: 6669 6c65 2929 0d0a 2020 2020 2020 2020  file))..        
+00001460: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00001470: 2822 496e 6974 6961 6c69 7a65 6420 636f  ("Initialized co
+00001480: 7265 207b 7d22 2c20 7365 6c66 290d 0a0d  re {}", self)...
+00001490: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+000014a0: 6d5f 7061 7468 203d 206d 6d5f 7061 7468  m_path = mm_path
+000014b0: 206f 7220 6669 6e64 5f6d 6963 726f 6d61   or find_microma
+000014c0: 6e61 6765 7228 290d 0a20 2020 2020 2020  nager()..       
+000014d0: 2069 6620 6e6f 7420 6164 6170 7465 725f   if not adapter_
+000014e0: 7061 7468 7320 616e 6420 7365 6c66 2e5f  paths and self._
+000014f0: 6d6d 5f70 6174 683a 0d0a 2020 2020 2020  mm_path:..      
+00001500: 2020 2020 2020 6164 6170 7465 725f 7061        adapter_pa
+00001510: 7468 7320 3d20 5b73 656c 662e 5f6d 6d5f  ths = [self._mm_
+00001520: 7061 7468 5d0d 0a20 2020 2020 2020 2069  path]..        i
+00001530: 6620 6164 6170 7465 725f 7061 7468 733a  f adapter_paths:
+00001540: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00001550: 6c66 2e73 6574 4465 7669 6365 4164 6170  lf.setDeviceAdap
+00001560: 7465 7253 6561 7263 6850 6174 6873 2861  terSearchPaths(a
+00001570: 6461 7074 6572 5f70 6174 6873 290d 0a0d  dapter_paths)...
+00001580: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
+00001590: 7665 6e74 7320 3d20 5f67 6574 5f61 7574  vents = _get_aut
+000015a0: 6f5f 636f 7265 5f63 616c 6c62 6163 6b5f  o_core_callback_
+000015b0: 636c 6173 7328 2928 290d 0a20 2020 2020  class()()..     
+000015c0: 2020 2073 656c 662e 5f63 616c 6c62 6163     self._callbac
+000015d0: 6b5f 7265 6c61 7920 3d20 4d4d 4361 6c6c  k_relay = MMCall
+000015e0: 6261 636b 5265 6c61 7928 7365 6c66 2e65  backRelay(self.e
+000015f0: 7665 6e74 7329 0d0a 2020 2020 2020 2020  vents)..        
+00001600: 7365 6c66 2e72 6567 6973 7465 7243 616c  self.registerCal
+00001610: 6c62 6163 6b28 7365 6c66 2e5f 6361 6c6c  lback(self._call
+00001620: 6261 636b 5f72 656c 6179 290d 0a0d 0a20  back_relay).... 
+00001630: 2020 2020 2020 2073 656c 662e 5f6d 6461         self._mda
+00001640: 5f72 756e 6e65 7220 3d20 4d44 4152 756e  _runner = MDARun
+00001650: 6e65 7228 290d 0a20 2020 2020 2020 2073  ner()..        s
+00001660: 656c 662e 5f6d 6461 5f72 756e 6e65 722e  elf._mda_runner.
+00001670: 7365 745f 656e 6769 6e65 284d 4441 456e  set_engine(MDAEn
+00001680: 6769 6e65 2873 656c 6629 290d 0a0d 0a20  gine(self)).... 
+00001690: 2020 2020 2020 2073 656c 662e 5f6f 626a         self._obj
+000016a0: 6563 7469 7665 5f72 6567 6578 3a20 5061  ective_regex: Pa
+000016b0: 7474 6572 6e20 3d20 5f4f 424a 4445 565f  ttern = _OBJDEV_
+000016c0: 5245 4745 580d 0a20 2020 2020 2020 2073  REGEX..        s
+000016d0: 656c 662e 5f63 6861 6e6e 656c 5f67 726f  elf._channel_gro
+000016e0: 7570 5f72 6567 6578 3a20 5061 7474 6572  up_regex: Patter
+000016f0: 6e20 3d20 5f43 4841 4e4e 454c 5f52 4547  n = _CHANNEL_REG
+00001700: 4558 0d0a 0d0a 2020 2020 2020 2020 2320  EX....        # 
+00001710: 7573 6520 7765 616b 7265 6620 746f 2061  use weakref to a
+00001720: 766f 6964 2061 7465 7869 7420 6b65 6570  void atexit keep
+00001730: 696e 6720 7573 2066 726f 6d20 6265 696e  ing us from bein
+00001740: 670d 0a20 2020 2020 2020 2023 2067 6172  g..        # gar
+00001750: 6261 6765 2063 6f6c 6c65 6374 6564 0d0a  bage collected..
+00001760: 2020 2020 2020 2020 7365 6c66 2e5f 7765          self._we
+00001770: 616b 5f63 6c65 616e 203d 2077 6561 6b72  ak_clean = weakr
+00001780: 6566 2e57 6561 6b4d 6574 686f 6428 7365  ef.WeakMethod(se
+00001790: 6c66 2e75 6e6c 6f61 6441 6c6c 4465 7669  lf.unloadAllDevi
+000017a0: 6365 7329 0d0a 2020 2020 2020 2020 6174  ces)..        at
+000017b0: 6578 6974 2e72 6567 6973 7465 7228 7365  exit.register(se
+000017c0: 6c66 2e5f 7765 616b 5f63 6c65 616e 290d  lf._weak_clean).
+000017d0: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+000017e0: 0d0a 2020 2020 6465 6620 6576 656e 7473  ..    def events
+000017f0: 2873 656c 6629 202d 3e20 5043 6f72 6553  (self) -> PCoreS
+00001800: 6967 6e61 6c65 723a 0d0a 2020 2020 2020  ignaler:..      
+00001810: 2020 2222 2253 6967 6e61 6c65 7220 666f    """Signaler fo
+00001820: 7220 636f 7265 2065 7665 6e74 732e 0d0a  r core events...
+00001830: 0d0a 2020 2020 2020 2020 3a73 7061 726b  ..        :spark
+00001840: 6c65 733a 202a 5468 6973 206d 6574 686f  les: *This metho
+00001850: 6420 6973 206e 6577 2069 6e20 6043 4d4d  d is new in `CMM
+00001860: 436f 7265 506c 7573 602e 2a0d 0a0d 0a20  CorePlus`.*.... 
+00001870: 2020 2020 2020 2054 6869 7320 6174 7472         This attr
+00001880: 6962 7574 6520 616c 6c6f 7773 2063 6f6e  ibute allows con
+00001890: 6e65 6374 696e 6720 6361 6c6c 6261 636b  necting callback
+000018a0: 7320 746f 2076 6172 696f 7573 2065 7665  s to various eve
+000018b0: 6e74 7320 7468 6174 206f 6363 7572 2077  nts that occur w
+000018c0: 6974 6869 6e0d 0a20 2020 2020 2020 2074  ithin..        t
+000018d0: 6865 2063 6f72 652e 2053 6565 205b 6070  he core. See [`p
+000018e0: 796d 6d63 6f72 655f 706c 7573 2e63 6f72  ymmcore_plus.cor
+000018f0: 652e 6576 656e 7473 2e50 436f 7265 5369  e.events.PCoreSi
+00001900: 676e 616c 6572 605d 5b5d 2064 6f63 756d  gnaler`][] docum
+00001910: 656e 7461 7469 6f6e 2066 6f72 0d0a 2020  entation for..  
+00001920: 2020 2020 2020 6465 7461 696c 7320 6f66        details of
+00001930: 2074 6865 2061 7661 696c 6162 6c65 2073   the available s
+00001940: 6967 6e61 6c73 2c20 616e 6420 686f 7720  ignals, and how 
+00001950: 746f 2063 6f6e 6e65 6374 2074 6f20 7468  to connect to th
+00001960: 656d 2e0d 0a20 2020 2020 2020 2022 2222  em...        """
+00001970: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001980: 2073 656c 662e 5f65 7665 6e74 730d 0a0d   self._events...
+00001990: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
+000019a0: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0d  _(self) -> str:.
+000019b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000019c0: 6622 3c7b 7479 7065 2873 656c 6629 2e5f  f"<{type(self)._
+000019d0: 5f6e 616d 655f 5f7d 2061 7420 7b68 6578  _name__} at {hex
+000019e0: 2869 6428 7365 6c66 2929 7d3e 220d 0a0d  (id(self))}>"...
+000019f0: 0a20 2020 2064 6566 205f 5f64 656c 5f5f  .    def __del__
+00001a00: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
+00001a10: 0a20 2020 2020 2020 2061 7465 7869 742e  .        atexit.
+00001a20: 756e 7265 6769 7374 6572 2873 656c 662e  unregister(self.
+00001a30: 5f77 6561 6b5f 636c 6561 6e29 0d0a 2020  _weak_clean)..  
+00001a40: 2020 2020 2020 7365 6c66 2e75 6e6c 6f61        self.unloa
+00001a50: 6441 6c6c 4465 7669 6365 7328 290d 0a0d  dAllDevices()...
+00001a60: 0a20 2020 2023 2052 652d 696d 706c 656d  .    # Re-implem
+00001a70: 656e 7465 6420 6d65 7468 6f64 7320 6672  ented methods fr
+00001a80: 6f6d 2074 6865 2043 4d4d 436f 7265 2041  om the CMMCore A
+00001a90: 5049 0d0a 0d0a 2020 2020 4073 796e 6368  PI....    @synch
+00001aa0: 726f 6e69 7a65 6428 5f6c 6f63 6b29 0d0a  ronized(_lock)..
+00001ab0: 2020 2020 6465 6620 7365 7450 726f 7065      def setPrope
+00001ac0: 7274 7928 0d0a 2020 2020 2020 2020 7365  rty(..        se
+00001ad0: 6c66 2c20 6c61 6265 6c3a 2073 7472 2c20  lf, label: str, 
+00001ae0: 7072 6f70 4e61 6d65 3a20 7374 722c 2070  propName: str, p
+00001af0: 726f 7056 616c 7565 3a20 626f 6f6c 207c  ropValue: bool |
+00001b00: 2066 6c6f 6174 207c 2069 6e74 207c 2073   float | int | s
+00001b10: 7472 0d0a 2020 2020 2920 2d3e 204e 6f6e  tr..    ) -> Non
+00001b20: 653a 0d0a 2020 2020 2020 2020 2222 2253  e:..        """S
+00001b30: 6574 2070 726f 7065 7274 7920 6e61 6d65  et property name
+00001b40: 6420 6070 726f 704e 616d 6560 206f 6e20  d `propName` on 
+00001b50: 6465 7669 6365 2060 6c61 6265 6c60 2074  device `label` t
+00001b60: 6f20 6070 726f 7056 616c 7565 602e 0d0a  o `propValue`...
+00001b70: 0d0a 2020 2020 2020 2020 2a2a 5768 7920  ..        **Why 
+00001b80: 4f76 6572 7269 6465 3f2a 2a20 2049 6e20  Override?**  In 
+00001b90: 604d 4d43 6f72 6560 2c20 7468 6520 6361  `MMCore`, the ca
+00001ba0: 6c6c 696e 6720 6f66 2074 6865 2060 6f6e  lling of the `on
+00001bb0: 5072 6f70 6572 7479 4368 616e 6765 6460  PropertyChanged`
+00001bc0: 0d0a 2020 2020 2020 2020 6361 6c6c 6261  ..        callba
+00001bd0: 636b 2069 7320 6c65 6674 2074 6f20 7468  ck is left to th
+00001be0: 6520 756e 6465 726c 7969 6e67 2064 6576  e underlying dev
+00001bf0: 6963 6520 6164 6170 7465 722c 2077 6869  ice adapter, whi
+00001c00: 6368 206d 6561 6e73 2069 7420 6973 206e  ch means it is n
+00001c10: 6f74 2061 6c77 6179 730d 0a20 2020 2020  ot always..     
+00001c20: 2020 2063 616c 6c65 642e 2020 5468 6973     called.  This
+00001c30: 206d 6574 686f 6420 6f76 6572 7269 6465   method override
+00001c40: 7320 7468 6520 6465 6661 756c 7420 696d  s the default im
+00001c50: 706c 656d 656e 7461 7469 6f6e 2074 6f20  plementation to 
+00001c60: 656e 7375 7265 2074 6861 740d 0a20 2020  ensure that..   
+00001c70: 2020 2020 2060 6576 656e 7473 2e70 726f       `events.pro
+00001c80: 7065 7274 7943 6861 6e67 6564 6020 6973  pertyChanged` is
+00001c90: 202a 616c 7761 7973 2a20 656d 6974 7465   *always* emitte
+00001ca0: 6420 7768 656e 2060 7365 7450 726f 7065  d when `setPrope
+00001cb0: 7274 7960 2068 6173 2062 6565 6e20 6361  rty` has been ca
+00001cc0: 6c6c 6564 0d0a 2020 2020 2020 2020 616e  lled..        an
+00001cd0: 6420 7468 6520 7072 6f70 6572 7479 2056  d the property V
+00001ce0: 616c 7565 2068 6173 2061 6374 7561 6c6c  alue has actuall
+00001cf0: 7920 6368 616e 6765 642e 0d0a 2020 2020  y changed...    
+00001d00: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001d10: 2077 6974 6820 7365 6c66 2e5f 7072 6f70   with self._prop
+00001d20: 6572 7479 5f63 6861 6e67 655f 656d 6973  erty_change_emis
+00001d30: 7369 6f6e 5f65 6e73 7572 6564 286c 6162  sion_ensured(lab
+00001d40: 656c 2c20 2870 726f 704e 616d 652c 2929  el, (propName,))
+00001d50: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00001d60: 7570 6572 2829 2e73 6574 5072 6f70 6572  uper().setProper
+00001d70: 7479 286c 6162 656c 2c20 7072 6f70 4e61  ty(label, propNa
+00001d80: 6d65 2c20 7072 6f70 5661 6c75 6529 0d0a  me, propValue)..
+00001d90: 0d0a 2020 2020 4073 796e 6368 726f 6e69  ..    @synchroni
+00001da0: 7a65 6428 5f6c 6f63 6b29 0d0a 2020 2020  zed(_lock)..    
+00001db0: 6465 6620 7365 7453 7461 7465 2873 656c  def setState(sel
+00001dc0: 662c 2073 7461 7465 4465 7669 6365 4c61  f, stateDeviceLa
+00001dd0: 6265 6c3a 2073 7472 2c20 7374 6174 653a  bel: str, state:
+00001de0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0d0a   int) -> None:..
+00001df0: 2020 2020 2020 2020 2222 2253 6574 2073          """Set s
+00001e00: 7461 7465 2028 6279 2070 6f73 6974 696f  tate (by positio
+00001e10: 6e29 206f 6e20 6073 7461 7465 4465 7669  n) on `stateDevi
+00001e20: 6365 4c61 6265 6c60 2c20 7769 7468 2072  ceLabel`, with r
+00001e30: 656c 6961 626c 6520 6576 656e 7420 656d  eliable event em
+00001e40: 6973 7369 6f6e 2e0d 0a0d 0a20 2020 2020  ission.....     
+00001e50: 2020 202a 2a57 6879 204f 7665 7272 6964     **Why Overrid
+00001e60: 653f 2a2a 2020 496e 2060 4d4d 436f 7265  e?**  In `MMCore
+00001e70: 602c 2074 6865 2063 616c 6c69 6e67 206f  `, the calling o
+00001e80: 6620 7468 6520 606f 6e50 726f 7065 7274  f the `onPropert
+00001e90: 7943 6861 6e67 6564 600d 0a20 2020 2020  yChanged`..     
+00001ea0: 2020 2063 616c 6c62 6163 6b20 6973 206c     callback is l
+00001eb0: 6566 7420 746f 2074 6865 2075 6e64 6572  eft to the under
+00001ec0: 6c79 696e 6720 6465 7669 6365 2061 6461  lying device ada
+00001ed0: 7074 6572 2c20 7768 6963 6820 6d65 616e  pter, which mean
+00001ee0: 7320 6974 2069 7320 6e6f 7420 616c 7761  s it is not alwa
+00001ef0: 7973 0d0a 2020 2020 2020 2020 6361 6c6c  ys..        call
+00001f00: 6564 2e20 2054 6869 7320 6d65 7468 6f64  ed.  This method
+00001f10: 206f 7665 7272 6964 6573 2074 6865 2064   overrides the d
+00001f20: 6566 6175 6c74 2069 6d70 6c65 6d65 6e74  efault implement
+00001f30: 6174 696f 6e20 746f 2065 6e73 7572 6520  ation to ensure 
+00001f40: 7468 6174 0d0a 2020 2020 2020 2020 6065  that..        `e
+00001f50: 7665 6e74 732e 7072 6f70 6572 7479 4368  vents.propertyCh
+00001f60: 616e 6765 6460 2069 7320 2a61 6c77 6179  anged` is *alway
+00001f70: 732a 2065 6d69 7474 6564 2077 6865 6e20  s* emitted when 
+00001f80: 6073 6574 5072 6f70 6572 7479 6020 6861  `setProperty` ha
+00001f90: 7320 6265 656e 2063 616c 6c65 640d 0a20  s been called.. 
+00001fa0: 2020 2020 2020 2061 6e64 2074 6865 2070         and the p
+00001fb0: 726f 7065 7274 7920 5661 6c75 6520 6861  roperty Value ha
+00001fc0: 7320 6163 7475 616c 6c79 2063 6861 6e67  s actually chang
+00001fd0: 6564 2e0d 0a20 2020 2020 2020 2022 2222  ed...        """
+00001fe0: 0d0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+00001ff0: 656c 662e 5f70 726f 7065 7274 795f 6368  elf._property_ch
+00002000: 616e 6765 5f65 6d69 7373 696f 6e5f 656e  ange_emission_en
+00002010: 7375 7265 6428 7374 6174 6544 6576 6963  sured(stateDevic
+00002020: 654c 6162 656c 2c20 5354 4154 455f 5052  eLabel, STATE_PR
+00002030: 4f50 5329 3a0d 0a20 2020 2020 2020 2020  OPS):..         
+00002040: 2020 2073 7570 6572 2829 2e73 6574 5374     super().setSt
+00002050: 6174 6528 7374 6174 6544 6576 6963 654c  ate(stateDeviceL
+00002060: 6162 656c 2c20 7374 6174 6529 0d0a 0d0a  abel, state)....
+00002070: 2020 2020 4073 796e 6368 726f 6e69 7a65      @synchronize
+00002080: 6428 5f6c 6f63 6b29 0d0a 2020 2020 6465  d(_lock)..    de
+00002090: 6620 7365 7453 7461 7465 4c61 6265 6c28  f setStateLabel(
+000020a0: 7365 6c66 2c20 7374 6174 6544 6576 6963  self, stateDevic
+000020b0: 654c 6162 656c 3a20 7374 722c 2073 7461  eLabel: str, sta
+000020c0: 7465 4c61 6265 6c3a 2073 7472 2920 2d3e  teLabel: str) ->
+000020d0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+000020e0: 2222 2253 6574 2073 7461 7465 2028 6279  """Set state (by
+000020f0: 206c 6162 656c 2920 6f6e 2060 7374 6174   label) on `stat
+00002100: 6544 6576 6963 654c 6162 656c 602c 2077  eDeviceLabel`, w
+00002110: 6974 6820 7265 6c69 6162 6c65 2065 7665  ith reliable eve
+00002120: 6e74 2065 6d69 7373 696f 6e2e 0d0a 0d0a  nt emission.....
+00002130: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
+00002140: 6572 7269 6465 3f2a 2a20 2049 6e20 604d  erride?**  In `M
+00002150: 4d43 6f72 6560 2c20 7468 6520 6361 6c6c  MCore`, the call
+00002160: 696e 6720 6f66 2074 6865 2060 6f6e 5072  ing of the `onPr
+00002170: 6f70 6572 7479 4368 616e 6765 6460 0d0a  opertyChanged`..
+00002180: 2020 2020 2020 2020 6361 6c6c 6261 636b          callback
+00002190: 2069 7320 6c65 6674 2074 6f20 7468 6520   is left to the 
+000021a0: 756e 6465 726c 7969 6e67 2064 6576 6963  underlying devic
+000021b0: 6520 6164 6170 7465 722c 2077 6869 6368  e adapter, which
+000021c0: 206d 6561 6e73 2069 7420 6973 206e 6f74   means it is not
+000021d0: 2061 6c77 6179 730d 0a20 2020 2020 2020   always..       
+000021e0: 2063 616c 6c65 642e 2020 5468 6973 206d   called.  This m
+000021f0: 6574 686f 6420 6f76 6572 7269 6465 7320  ethod overrides 
+00002200: 7468 6520 6465 6661 756c 7420 696d 706c  the default impl
+00002210: 656d 656e 7461 7469 6f6e 2074 6f20 656e  ementation to en
+00002220: 7375 7265 2074 6861 740d 0a20 2020 2020  sure that..     
+00002230: 2020 2060 6576 656e 7473 2e70 726f 7065     `events.prope
+00002240: 7274 7943 6861 6e67 6564 6020 6973 202a  rtyChanged` is *
+00002250: 616c 7761 7973 2a20 656d 6974 7465 6420  always* emitted 
+00002260: 7768 656e 2060 7365 7450 726f 7065 7274  when `setPropert
+00002270: 7960 2068 6173 2062 6565 6e20 6361 6c6c  y` has been call
+00002280: 6564 0d0a 2020 2020 2020 2020 616e 6420  ed..        and 
+00002290: 7468 6520 7072 6f70 6572 7479 2056 616c  the property Val
+000022a0: 7565 2068 6173 2061 6374 7561 6c6c 7920  ue has actually 
+000022b0: 6368 616e 6765 642e 0d0a 2020 2020 2020  changed...      
+000022c0: 2020 2222 220d 0a20 2020 2020 2020 2077    """..        w
+000022d0: 6974 6820 7365 6c66 2e5f 7072 6f70 6572  ith self._proper
+000022e0: 7479 5f63 6861 6e67 655f 656d 6973 7369  ty_change_emissi
+000022f0: 6f6e 5f65 6e73 7572 6564 2873 7461 7465  on_ensured(state
+00002300: 4465 7669 6365 4c61 6265 6c2c 2053 5441  DeviceLabel, STA
+00002310: 5445 5f50 524f 5053 293a 0d0a 2020 2020  TE_PROPS):..    
+00002320: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00002330: 7365 7453 7461 7465 4c61 6265 6c28 7374  setStateLabel(st
+00002340: 6174 6544 6576 6963 654c 6162 656c 2c20  ateDeviceLabel, 
+00002350: 7374 6174 654c 6162 656c 290d 0a0d 0a20  stateLabel).... 
+00002360: 2020 2064 6566 2073 6574 4465 7669 6365     def setDevice
+00002370: 4164 6170 7465 7253 6561 7263 6850 6174  AdapterSearchPat
+00002380: 6873 2873 656c 662c 2070 6174 6873 3a20  hs(self, paths: 
+00002390: 5365 7175 656e 6365 5b73 7472 5d29 202d  Sequence[str]) -
+000023a0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+000023b0: 2022 2222 5365 7420 7468 6520 6465 7669   """Set the devi
+000023c0: 6365 2061 6461 7074 6572 2073 6561 7263  ce adapter searc
+000023d0: 6820 7061 7468 732e 0d0a 0d0a 2020 2020  h paths.....    
+000023e0: 2020 2020 2a2a 5768 7920 4f76 6572 7269      **Why Overri
+000023f0: 6465 3f2a 2a20 2049 6e20 6361 7365 7320  de?**  In cases 
+00002400: 7768 6572 6520 4d4d 2064 6576 6963 6520  where MM device 
+00002410: 6164 6170 7465 7273 2075 7365 2064 796e  adapters use dyn
+00002420: 616d 6963 616c 6c79 206c 6f61 6465 640d  amically loaded.
+00002430: 0a20 2020 2020 2020 206c 6962 7261 7269  .        librari
+00002440: 6573 2c20 7468 6520 6465 7669 6365 2061  es, the device a
+00002450: 6461 7074 6572 2073 6561 7263 6820 7061  dapter search pa
+00002460: 7468 7320 6d75 7374 2061 6c73 6f20 6265  ths must also be
+00002470: 2061 6464 6564 2074 6f20 7468 6520 6050   added to the `P
+00002480: 4154 4860 0d0a 2020 2020 2020 2020 656e  ATH`..        en
+00002490: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+000024a0: 6c65 2028 652e 672e 0d0a 2020 2020 2020  le (e.g...      
+000024b0: 2020 3c68 7474 7073 3a2f 2f67 6974 6875    <https://githu
+000024c0: 622e 636f 6d2f 6d69 6372 6f2d 6d61 6e61  b.com/micro-mana
+000024d0: 6765 722f 7079 6d6d 636f 7265 2f69 7373  ger/pymmcore/iss
+000024e0: 7565 732f 3238 3e29 2e20 5468 6973 206d  ues/28>). This m
+000024f0: 6574 686f 6420 6f76 6572 7269 6465 730d  ethod overrides.
+00002500: 0a20 2020 2020 2020 2074 6865 2064 6566  .        the def
+00002510: 6175 6c74 2069 6d70 6c65 6d65 6e74 6174  ault implementat
+00002520: 696f 6e20 746f 2065 6e73 7572 6520 7468  ion to ensure th
+00002530: 6174 2074 6865 2060 5041 5448 6020 656e  at the `PATH` en
+00002540: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00002550: 6c65 2069 730d 0a20 2020 2020 2020 2075  le is..        u
+00002560: 7064 6174 6564 2077 6865 6e20 7468 6520  pdated when the 
+00002570: 6465 7669 6365 2061 6461 7074 6572 2073  device adapter s
+00002580: 6561 7263 6820 7061 7468 7320 6172 6520  earch paths are 
+00002590: 6368 616e 6765 642e 0d0a 2020 2020 2020  changed...      
+000025a0: 2020 2222 220d 0a20 2020 2020 2020 2023    """..        #
+000025b0: 2061 6464 2074 6f20 5041 5448 2061 7320   add to PATH as 
+000025c0: 7765 6c6c 2066 6f72 2064 796e 616d 6963  well for dynamic
+000025d0: 2064 6c6c 730d 0a20 2020 2020 2020 2069   dlls..        i
+000025e0: 6620 6e6f 7420 7061 7468 733a 0d0a 2020  f not paths:..  
+000025f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002600: 0d0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+00002610: 6e73 7461 6e63 6528 7061 7468 732c 2073  nstance(paths, s
+00002620: 7472 2920 6f72 2061 6e79 286e 6f74 2069  tr) or any(not i
+00002630: 7369 6e73 7461 6e63 6528 702c 2073 7472  sinstance(p, str
+00002640: 2920 666f 7220 7020 696e 2070 6174 6873  ) for p in paths
+00002650: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00002660: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00002670: 2270 6174 6873 206d 7573 7420 6265 2061  "paths must be a
+00002680: 2073 6571 7565 6e63 6520 6f66 2073 7472   sequence of str
+00002690: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
+000026a0: 656e 765f 7061 7468 203d 206f 732e 656e  env_path = os.en
+000026b0: 7669 726f 6e5b 2250 4154 4822 5d0d 0a20  viron["PATH"].. 
+000026c0: 2020 2020 2020 2066 6f72 2070 2069 6e20         for p in 
+000026d0: 7061 7468 733a 0d0a 2020 2020 2020 2020  paths:..        
+000026e0: 2020 2020 6966 2070 206e 6f74 2069 6e20      if p not in 
+000026f0: 656e 765f 7061 7468 3a0d 0a20 2020 2020  env_path:..     
+00002700: 2020 2020 2020 2020 2020 2065 6e76 5f70             env_p
+00002710: 6174 6820 3d20 7020 2b20 6f73 2e70 6174  ath = p + os.pat
+00002720: 6873 6570 202b 2065 6e76 5f70 6174 680d  hsep + env_path.
+00002730: 0a20 2020 2020 2020 206f 732e 656e 7669  .        os.envi
+00002740: 726f 6e5b 2250 4154 4822 5d20 3d20 656e  ron["PATH"] = en
+00002750: 765f 7061 7468 0d0a 2020 2020 2020 2020  v_path..        
+00002760: 6c6f 6767 6572 2e64 6562 7567 2866 2273  logger.debug(f"s
+00002770: 6574 7469 6e67 2061 6461 7074 6572 2073  etting adapter s
+00002780: 6561 7263 6820 7061 7468 733a 207b 7061  earch paths: {pa
+00002790: 7468 737d 2229 0d0a 2020 2020 2020 2020  ths}")..        
+000027a0: 7375 7065 7228 292e 7365 7444 6576 6963  super().setDevic
+000027b0: 6541 6461 7074 6572 5365 6172 6368 5061  eAdapterSearchPa
+000027c0: 7468 7328 7061 7468 7329 0d0a 0d0a 2020  ths(paths)....  
+000027d0: 2020 6465 6620 6c6f 6164 4465 7669 6365    def loadDevice
+000027e0: 2873 656c 662c 206c 6162 656c 3a20 7374  (self, label: st
+000027f0: 722c 206d 6f64 756c 654e 616d 653a 2073  r, moduleName: s
+00002800: 7472 2c20 6465 7669 6365 4e61 6d65 3a20  tr, deviceName: 
+00002810: 7374 7229 202d 3e20 4e6f 6e65 3a0d 0a20  str) -> None:.. 
+00002820: 2020 2020 2020 2022 2222 4c6f 6164 2061         """Load a
+00002830: 2064 6576 6963 6520 6672 6f6d 2074 6865   device from the
+00002840: 2070 6c75 6769 6e20 6c69 6272 6172 792e   plugin library.
+00002850: 0d0a 0d0a 2020 2020 2020 2020 2a2a 5768  ....        **Wh
+00002860: 7920 4f76 6572 7269 6465 3f2a 2a20 546f  y Override?** To
+00002870: 2061 6464 206d 7563 6820 6265 7474 6572   add much better
+00002880: 2065 7272 6f72 206d 6573 7361 6765 7320   error messages 
+00002890: 696e 2074 6865 2063 6173 6520 6f66 2066  in the case of f
+000028a0: 6169 6c75 7265 2e0d 0a0d 0a20 2020 2020  ailure.....     
+000028b0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+000028c0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000028d0: 2d0d 0a20 2020 2020 2020 206c 6162 656c  -..        label
+000028e0: 3a20 7374 720d 0a20 2020 2020 2020 2020  : str..         
+000028f0: 2020 204e 616d 6520 746f 2062 6520 6173     Name to be as
+00002900: 7369 676e 6564 2074 6f20 7468 6520 6465  signed to the de
+00002910: 7669 6365 2064 7572 696e 6720 7468 6973  vice during this
+00002920: 2063 6f72 6520 7365 7373 696f 6e2e 0d0a   core session...
+00002930: 2020 2020 2020 2020 6d6f 6475 6c65 4e61          moduleNa
+00002940: 6d65 3a20 7374 720d 0a20 2020 2020 2020  me: str..       
+00002950: 2020 2020 2054 6865 206e 616d 6520 6f66       The name of
+00002960: 2074 6865 2064 6576 6963 6520 6164 6170   the device adap
+00002970: 7465 7220 6d6f 6475 6c65 2028 7368 6f72  ter module (shor
+00002980: 7420 6e61 6d65 2c20 6e6f 7420 6675 6c6c  t name, not full
+00002990: 2066 696c 6520 6e61 6d65 292e 0d0a 2020   file name)...  
+000029a0: 2020 2020 2020 2020 2020 5365 6520 5b60            See [`
+000029b0: 7079 6d6d 636f 7265 2e43 4d4d 436f 7265  pymmcore.CMMCore
+000029c0: 2e67 6574 4465 7669 6365 4164 6170 7465  .getDeviceAdapte
+000029d0: 724e 616d 6573 605d 5b5d 2066 6f72 2061  rNames`][] for a
+000029e0: 206c 6973 7420 6f66 2076 616c 6964 0d0a   list of valid..
+000029f0: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
+00002a00: 6c65 206e 616d 6573 2e0d 0a20 2020 2020  le names...     
+00002a10: 2020 2064 6576 6963 654e 616d 653a 2073     deviceName: s
+00002a20: 7472 0d0a 2020 2020 2020 2020 2020 2020  tr..            
+00002a30: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+00002a40: 6465 7669 6365 2e20 5468 6520 6e61 6d65  device. The name
+00002a50: 206d 7573 7420 636f 7272 6573 706f 6e64   must correspond
+00002a60: 2074 6f20 6f6e 6520 6f66 2074 6865 206e   to one of the n
+00002a70: 616d 6573 0d0a 2020 2020 2020 2020 2020  ames..          
+00002a80: 2020 7265 636f 676e 697a 6564 2062 7920    recognized by 
+00002a90: 7468 6520 7370 6563 6966 6963 2070 6c75  the specific plu
+00002aa0: 6769 6e20 6c69 6272 6172 792e 2053 6565  gin library. See
+00002ab0: 0d0a 2020 2020 2020 2020 2020 2020 5b60  ..            [`
+00002ac0: 7079 6d6d 636f 7265 2e43 4d4d 436f 7265  pymmcore.CMMCore
+00002ad0: 2e67 6574 4176 6169 6c61 626c 6544 6576  .getAvailableDev
+00002ae0: 6963 6573 605d 5b5d 2066 6f72 2061 206c  ices`][] for a l
+00002af0: 6973 7420 6f66 2076 616c 6964 2064 6576  ist of valid dev
+00002b00: 6963 6520 6e61 6d65 732e 0d0a 2020 2020  ice names...    
+00002b10: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00002b20: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00002b30: 2020 2073 7570 6572 2829 2e6c 6f61 6444     super().loadD
+00002b40: 6576 6963 6528 6c61 6265 6c2c 206d 6f64  evice(label, mod
+00002b50: 756c 654e 616d 652c 2064 6576 6963 654e  uleName, deviceN
+00002b60: 616d 6529 0d0a 2020 2020 2020 2020 6578  ame)..        ex
+00002b70: 6365 7074 2052 756e 7469 6d65 4572 726f  cept RuntimeErro
+00002b80: 7220 6173 2065 3a0d 0a20 2020 2020 2020  r as e:..       
+00002b90: 2020 2020 206d 7367 203d 2073 7472 2865       msg = str(e
+00002ba0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00002bb0: 6620 6c61 6265 6c20 696e 2073 656c 662e  f label in self.
+00002bc0: 6765 744c 6f61 6465 6444 6576 6963 6573  getLoadedDevices
+00002bd0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00002be0: 2020 2020 206c 6962 203d 2073 7570 6572       lib = super
+00002bf0: 2829 2e67 6574 4465 7669 6365 4c69 6272  ().getDeviceLibr
+00002c00: 6172 7928 6c61 6265 6c29 0d0a 2020 2020  ary(label)..    
+00002c10: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00002c20: 203d 2073 7570 6572 2829 2e67 6574 4465   = super().getDe
+00002c30: 7669 6365 4e61 6d65 286c 6162 656c 290d  viceName(label).
+00002c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c50: 2069 6620 6d6f 6475 6c65 4e61 6d65 203d   if moduleName =
+00002c60: 3d20 6c69 6220 616e 6420 6465 7669 6365  = lib and device
+00002c70: 4e61 6d65 203d 3d20 6e61 6d65 3a0d 0a20  Name == name:.. 
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 206d 7367 202b 3d20 6622 2e20 4465     msg += f". De
+00002ca0: 7669 6365 207b 6c61 6265 6c21 727d 2061  vice {label!r} a
+00002cb0: 7070 6561 7273 2074 6f20 6265 206c 6f61  ppears to be loa
+00002cc0: 6465 6420 616c 7265 6164 792e 220d 0a20  ded already.".. 
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
+00002cf0: 286d 7367 2c20 7374 6163 6b6c 6576 656c  (msg, stacklevel
+00002d00: 3d32 290d 0a20 2020 2020 2020 2020 2020  =2)..           
+00002d10: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+00002d20: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00002d30: 2020 206d 7367 202b 3d20 6622 2e20 4465     msg += f". De
+00002d40: 7669 6365 207b 6c61 6265 6c21 727d 2069  vice {label!r} i
+00002d50: 7320 616c 7265 6164 7920 7461 6b65 6e20  s already taken 
+00002d60: 6279 207b 6c69 627d 3a3a 7b6e 616d 657d  by {lib}::{name}
+00002d70: 220d 0a20 2020 2020 2020 2020 2020 2065  "..            e
+00002d80: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00002d90: 2020 2020 2020 6164 6170 7465 7273 203d        adapters =
+00002da0: 2073 7570 6572 2829 2e67 6574 4465 7669   super().getDevi
+00002db0: 6365 4164 6170 7465 724e 616d 6573 2829  ceAdapterNames()
+00002dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002dd0: 2020 6966 206d 6f64 756c 654e 616d 6520    if moduleName 
+00002de0: 6e6f 7420 696e 2061 6461 7074 6572 733a  not in adapters:
+00002df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002e00: 2020 2020 2020 6d73 6720 2b3d 2028 0d0a        msg += (..
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e20: 2020 2020 2020 2020 6622 2e20 4164 6170          f". Adap
+00002e30: 7465 7220 6e61 6d65 207b 6d6f 6475 6c65  ter name {module
+00002e40: 4e61 6d65 2172 7d20 6e6f 7420 696e 206c  Name!r} not in l
+00002e50: 6973 7420 6f66 206b 6e6f 776e 2061 6461  ist of known ada
+00002e60: 7074 6572 2022 0d0a 2020 2020 2020 2020  pter "..        
+00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e80: 6622 6e61 6d65 733a 207b 6164 6170 7465  f"names: {adapte
+00002e90: 7273 7d2e 220d 0a20 2020 2020 2020 2020  rs}."..         
+00002ea0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00002eb0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00002ec0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002ed0: 2020 2020 2020 2020 2064 6576 6963 6573           devices
+00002ee0: 203d 2073 7570 6572 2829 2e67 6574 4176   = super().getAv
+00002ef0: 6169 6c61 626c 6544 6576 6963 6573 286d  ailableDevices(m
+00002f00: 6f64 756c 654e 616d 6529 0d0a 2020 2020  oduleName)..    
+00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f20: 6966 2064 6576 6963 654e 616d 6520 6e6f  if deviceName no
+00002f30: 7420 696e 2064 6576 6963 6573 3a0d 0a20  t in devices:.. 
 00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 2020 2066 222e 2044 6576 6963         f". Devic
-00002f60: 6520 6e61 6d65 207b 6465 7669 6365 4e61  e name {deviceNa
-00002f70: 6d65 2172 7d20 6e6f 7420 696e 2064 6576  me!r} not in dev
-00002f80: 6963 6573 2070 726f 7669 6465 6420 6279  ices provided by
-00002f90: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 6622 6164 6170 7465 7220 7b6d 6f64 756c  f"adapter {modul
-00002fc0: 654e 616d 6521 727d 3a20 7b64 6576 6963  eName!r}: {devic
-00002fd0: 6573 7d22 0d0a 2020 2020 2020 2020 2020  es}"..          
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00002ff0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00003000: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
-00003010: 6d73 6729 2066 726f 6d20 650d 0a0d 0a20  msg) from e.... 
-00003020: 2020 2040 7379 6e63 6872 6f6e 697a 6564     @synchronized
-00003030: 285f 6c6f 636b 290d 0a20 2020 2064 6566  (_lock)..    def
-00003040: 206c 6f61 6453 7973 7465 6d43 6f6e 6669   loadSystemConfi
-00003050: 6775 7261 7469 6f6e 280d 0a20 2020 2020  guration(..     
-00003060: 2020 2073 656c 662c 2066 696c 654e 616d     self, fileNam
-00003070: 653a 2073 7472 207c 2050 6174 6820 3d20  e: str | Path = 
-00003080: 224d 4d43 6f6e 6669 675f 6465 6d6f 2e63  "MMConfig_demo.c
-00003090: 6667 220d 0a20 2020 2029 202d 3e20 4e6f  fg"..    ) -> No
-000030a0: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
-000030b0: 4c6f 6164 2061 2073 7973 7465 6d20 636f  Load a system co
-000030c0: 6e66 6967 2066 696c 6520 636f 6e66 6f72  nfig file confor
-000030d0: 6d69 6e67 2074 6f20 7468 6520 4d4d 2060  ming to the MM `
-000030e0: 2e63 6667 6020 666f 726d 6174 2e0d 0a0d  .cfg` format....
-000030f0: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
-00003100: 2f6d 6963 726f 2d6d 616e 6167 6572 2e6f  /micro-manager.o
-00003110: 7267 2f4d 6963 726f 2d4d 616e 6167 6572  rg/Micro-Manager
-00003120: 5f43 6f6e 6669 6775 7261 7469 6f6e 5f47  _Configuration_G
-00003130: 7569 6465 2363 6f6e 6669 6775 7261 7469  uide#configurati
-00003140: 6f6e 2d66 696c 652d 7379 6e74 6178 0d0a  on-file-syntax..
-00003150: 0d0a 2020 2020 2020 2020 466f 7220 7265  ..        For re
-00003160: 6c61 7469 7665 2070 6174 6873 2c20 7468  lative paths, th
-00003170: 6520 6375 7272 656e 7420 776f 726b 696e  e current workin
-00003180: 6720 6469 7265 6374 6f72 7920 6973 2066  g directory is f
-00003190: 6972 7374 2063 6865 636b 6564 2c20 7468  irst checked, th
-000031a0: 656e 2074 6865 0d0a 2020 2020 2020 2020  en the..        
-000031b0: 7468 656e 2064 6576 6963 6520 6164 6170  then device adap
-000031c0: 7465 7220 7061 7468 2069 7320 6368 6563  ter path is chec
-000031d0: 6b65 642e 0d0a 0d0a 2020 2020 2020 2020  ked.....        
-000031e0: 2a2a 5768 7920 4f76 6572 7269 6465 3f2a  **Why Override?*
-000031f0: 2a20 5468 6973 206d 6574 686f 6420 6f76  * This method ov
-00003200: 6572 7269 6465 7320 7468 6520 6465 6661  errides the defa
-00003210: 756c 7420 696d 706c 656d 656e 7461 7469  ult implementati
-00003220: 6f6e 2074 6f20 4129 2061 6c6c 6f77 0d0a  on to A) allow..
-00003230: 2020 2020 2020 2020 6c6f 6164 696e 6720          loading 
-00003240: 7468 6520 604d 4d43 6f6e 6669 675f 6465  the `MMConfig_de
-00003250: 6d6f 2e63 6667 6020 6669 6c65 2062 7920  mo.cfg` file by 
-00003260: 6465 6661 756c 742c 2042 2920 746f 2070  default, B) to p
-00003270: 726f 7669 6465 206d 6f72 6520 666c 6578  rovide more flex
-00003280: 6962 6c65 0d0a 2020 2020 2020 2020 7061  ible..        pa
-00003290: 7468 2064 6563 6c61 7261 7469 6f6e 7320  th declarations 
-000032a0: 616e 6420 4329 2062 6574 7465 7220 6572  and C) better er
-000032b0: 726f 7220 6d65 7373 6167 6573 2077 6865  ror messages whe
-000032c0: 6e20 7468 6520 6669 6c65 2063 616e 6e6f  n the file canno
-000032d0: 7420 6265 2066 6f75 6e64 2e0d 0a20 2020  t be found...   
-000032e0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000032f0: 2020 6670 6174 6820 3d20 5061 7468 2866    fpath = Path(f
-00003300: 696c 654e 616d 6529 2e65 7870 616e 6475  ileName).expandu
-00003310: 7365 7228 290d 0a20 2020 2020 2020 2069  ser()..        i
-00003320: 6620 6e6f 7420 6670 6174 682e 6578 6973  f not fpath.exis
-00003330: 7473 2829 2061 6e64 206e 6f74 2066 7061  ts() and not fpa
-00003340: 7468 2e69 735f 6162 736f 6c75 7465 2829  th.is_absolute()
-00003350: 2061 6e64 2073 656c 662e 5f6d 6d5f 7061   and self._mm_pa
-00003360: 7468 3a0d 0a20 2020 2020 2020 2020 2020  th:..           
-00003370: 2066 7061 7468 203d 2050 6174 6828 7365   fpath = Path(se
-00003380: 6c66 2e5f 6d6d 5f70 6174 6829 202f 2066  lf._mm_path) / f
-00003390: 696c 654e 616d 650d 0a20 2020 2020 2020  ileName..       
-000033a0: 2069 6620 6e6f 7420 6670 6174 682e 6578   if not fpath.ex
-000033b0: 6973 7473 2829 3a0d 0a20 2020 2020 2020  ists():..       
-000033c0: 2020 2020 2072 6169 7365 2046 696c 654e       raise FileN
-000033d0: 6f74 466f 756e 6445 7272 6f72 2866 2250  otFoundError(f"P
-000033e0: 6174 6820 646f 6573 206e 6f74 2065 7869  ath does not exi
-000033f0: 7374 3a20 7b66 7061 7468 7d22 290d 0a20  st: {fpath}").. 
-00003400: 2020 2020 2020 2073 7570 6572 2829 2e6c         super().l
-00003410: 6f61 6453 7973 7465 6d43 6f6e 6669 6775  oadSystemConfigu
-00003420: 7261 7469 6f6e 2873 7472 2866 7061 7468  ration(str(fpath
-00003430: 2e72 6573 6f6c 7665 2829 2929 0d0a 0d0a  .resolve()))....
-00003440: 2020 2020 6465 6620 756e 6c6f 6164 416c      def unloadAl
-00003450: 6c44 6576 6963 6573 2873 656c 6629 202d  lDevices(self) -
-00003460: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-00003470: 2022 2222 556e 6c6f 6164 2061 6c6c 2064   """Unload all d
-00003480: 6576 6963 6573 2066 726f 6d20 7468 6520  evices from the 
-00003490: 636f 7265 2061 6e64 2072 6573 6574 2061  core and reset a
-000034a0: 6c6c 2063 6f6e 6669 6775 7261 7469 6f6e  ll configuration
-000034b0: 2064 6174 612e 0d0a 0d0a 2020 2020 2020   data.....      
-000034c0: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
-000034d0: 3f2a 2a20 546f 2061 6464 206c 6f67 6769  ?** To add loggi
-000034e0: 6e67 2e0d 0a20 2020 2020 2020 2022 2222  ng...        """
-000034f0: 0d0a 2020 2020 2020 2020 2320 7468 6973  ..        # this
-00003500: 206c 6f67 2077 6f6e 2774 2061 7070 6561   log won't appea
-00003510: 7220 7768 656e 2065 7869 7469 6e67 2069  r when exiting i
-00003520: 7079 7468 6f6e 2c20 6275 7420 7468 6520  python, but the 
-00003530: 6d65 7468 6f64 2069 7320 7374 696c 6c20  method is still 
-00003540: 6361 6c6c 6564 0d0a 2020 2020 2020 2020  called..        
-00003550: 6c6f 6767 6572 2e64 6562 7567 2822 556e  logger.debug("Un
-00003560: 6c6f 6164 696e 6720 616c 6c20 6465 7669  loading all devi
-00003570: 6365 7322 290d 0a20 2020 2020 2020 2072  ces")..        r
-00003580: 6574 7572 6e20 7375 7065 7228 292e 756e  eturn super().un
-00003590: 6c6f 6164 416c 6c44 6576 6963 6573 2829  loadAllDevices()
-000035a0: 0d0a 0d0a 2020 2020 6465 6620 6765 7444  ....    def getD
-000035b0: 6576 6963 6554 7970 6528 7365 6c66 2c20  eviceType(self, 
-000035c0: 6c61 6265 6c3a 2073 7472 2920 2d3e 2044  label: str) -> D
-000035d0: 6576 6963 6554 7970 653a 0d0a 2020 2020  eviceType:..    
-000035e0: 2020 2020 2222 2252 6574 7572 6e20 6465      """Return de
-000035f0: 7669 6365 2074 7970 6520 666f 7220 6120  vice type for a 
-00003600: 6769 7665 6e20 6465 7669 6365 2e0d 0a0d  given device....
-00003610: 0a20 2020 2020 2020 202a 2a57 6879 204f  .        **Why O
-00003620: 7665 7272 6964 653f 2a2a 2054 6865 2072  verride?** The r
-00003630: 6574 7572 6e65 6420 5b60 7079 6d6d 636f  eturned [`pymmco
-00003640: 7265 5f70 6c75 732e 4465 7669 6365 605d  re_plus.Device`]
-00003650: 5b5d 2065 6e75 6d20 6973 206d 6f72 650d  [] enum is more.
-00003660: 0a20 2020 2020 2020 2069 6e74 6572 7072  .        interpr
-00003670: 6574 6162 6c65 2074 6861 6e20 7468 6520  etable than the 
-00003680: 7261 7720 6069 6e74 6020 7265 7475 726e  raw `int` return
-00003690: 6564 2062 7920 6070 796d 6d63 6f72 6560  ed by `pymmcore`
-000036a0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000036b0: 2020 2020 2020 2072 6574 7572 6e20 4465         return De
-000036c0: 7669 6365 5479 7065 2873 7570 6572 2829  viceType(super()
-000036d0: 2e67 6574 4465 7669 6365 5479 7065 286c  .getDeviceType(l
-000036e0: 6162 656c 2929 0d0a 0d0a 2020 2020 6465  abel))....    de
-000036f0: 6620 6765 7450 726f 7065 7274 7954 7970  f getPropertyTyp
-00003700: 6528 7365 6c66 2c20 6c61 6265 6c3a 2073  e(self, label: s
-00003710: 7472 2c20 7072 6f70 4e61 6d65 3a20 7374  tr, propName: st
-00003720: 7229 202d 3e20 5072 6f70 6572 7479 5479  r) -> PropertyTy
-00003730: 7065 3a0d 0a20 2020 2020 2020 2022 2222  pe:..        """
-00003740: 5265 7475 726e 2074 6865 2069 6e74 7269  Return the intri
-00003750: 6e73 6963 2070 726f 7065 7274 7920 7479  nsic property ty
-00003760: 7065 2066 6f72 2061 2067 6976 656e 2064  pe for a given d
-00003770: 6576 6963 6520 616e 6420 7072 6f70 6572  evice and proper
-00003780: 7479 2e0d 0a0d 0a20 2020 2020 2020 202a  ty.....        *
-00003790: 2a57 6879 204f 7665 7272 6964 653f 2a2a  *Why Override?**
-000037a0: 2054 6865 2072 6574 7572 6e65 6420 5b60   The returned [`
-000037b0: 7079 6d6d 636f 7265 5f70 6c75 732e 5072  pymmcore_plus.Pr
-000037c0: 6f70 6572 7479 5479 7065 605d 5b5d 2065  opertyType`][] e
-000037d0: 6e75 6d20 6973 206d 6f72 650d 0a20 2020  num is more..   
-000037e0: 2020 2020 2069 6e74 6572 7072 6574 6162       interpretab
-000037f0: 6c65 2074 6861 6e20 7468 6520 7261 7720  le than the raw 
-00003800: 6069 6e74 6020 7265 7475 726e 6564 2062  `int` returned b
-00003810: 7920 6070 796d 6d63 6f72 6560 0d0a 2020  y `pymmcore`..  
-00003820: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00003830: 2020 2072 6574 7572 6e20 5072 6f70 6572     return Proper
-00003840: 7479 5479 7065 2873 7570 6572 2829 2e67  tyType(super().g
-00003850: 6574 5072 6f70 6572 7479 5479 7065 286c  etPropertyType(l
-00003860: 6162 656c 2c20 7072 6f70 4e61 6d65 2929  abel, propName))
-00003870: 0d0a 0d0a 2020 2020 6465 6620 6465 7465  ....    def dete
-00003880: 6374 4465 7669 6365 2873 656c 662c 2064  ctDevice(self, d
-00003890: 6576 6963 654c 6162 656c 3a20 7374 7229  eviceLabel: str)
-000038a0: 202d 3e20 4465 7669 6365 4465 7465 6374   -> DeviceDetect
-000038b0: 696f 6e53 7461 7475 733a 0d0a 2020 2020  ionStatus:..    
-000038c0: 2020 2020 2222 2254 7269 6573 2074 6f20      """Tries to 
-000038d0: 636f 6d6d 756e 6963 6174 6520 746f 2061  communicate to a
-000038e0: 2064 6576 6963 6520 7468 726f 7567 6820   device through 
-000038f0: 6120 6769 7665 6e20 7365 7269 616c 2070  a given serial p
-00003900: 6f72 742e 0d0a 0d0a 2020 2020 2020 2020  ort.....        
-00003910: 5573 6564 2074 6f20 6175 746f 6d61 7465  Used to automate
-00003920: 2064 6973 636f 7665 7279 206f 6620 636f   discovery of co
-00003930: 7272 6563 7420 7365 7269 616c 2070 6f72  rrect serial por
-00003940: 742e 0d0a 2020 2020 2020 2020 416c 736f  t...        Also
-00003950: 2063 6f6e 6669 6775 7265 7320 7468 6520   configures the 
-00003960: 7365 7269 616c 2070 6f72 7420 636f 7272  serial port corr
-00003970: 6563 746c 792e 0d0a 0d0a 2020 2020 2020  ectly.....      
-00003980: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
-00003990: 3f2a 2a20 5468 6520 7265 7475 726e 6564  ?** The returned
-000039a0: 205b 6070 796d 6d63 6f72 655f 706c 7573   [`pymmcore_plus
-000039b0: 2e44 6576 6963 6544 6574 6563 7469 6f6e  .DeviceDetection
-000039c0: 5374 6174 7573 605d 5b5d 2065 6e75 6d0d  Status`][] enum.
-000039d0: 0a20 2020 2020 2020 2069 7320 6d6f 7265  .        is more
-000039e0: 2069 6e74 6572 7072 6574 6162 6c65 2074   interpretable t
-000039f0: 6861 6e20 7468 6520 7261 7720 6069 6e74  han the raw `int
-00003a00: 6020 7265 7475 726e 6564 2062 7920 6070  ` returned by `p
-00003a10: 796d 6d63 6f72 6560 0d0a 2020 2020 2020  ymmcore`..      
-00003a20: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00003a30: 6574 7572 6e20 4465 7669 6365 4465 7465  eturn DeviceDete
-00003a40: 6374 696f 6e53 7461 7475 7328 7375 7065  ctionStatus(supe
-00003a50: 7228 292e 6465 7465 6374 4465 7669 6365  r().detectDevice
-00003a60: 2864 6576 6963 654c 6162 656c 2929 0d0a  (deviceLabel))..
-00003a70: 0d0a 2020 2020 2320 636f 6e66 6967 206f  ..    # config o
-00003a80: 7665 7272 6964 6573 0d0a 0d0a 2020 2020  verrides....    
-00003a90: 406f 7665 726c 6f61 640d 0a20 2020 2064  @overload..    d
-00003aa0: 6566 2067 6574 436f 6e66 6967 4461 7461  ef getConfigData
-00003ab0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-00003ac0: 2063 6f6e 6669 6747 726f 7570 3a20 7374   configGroup: st
-00003ad0: 722c 2063 6f6e 6669 674e 616d 653a 2073  r, configName: s
-00003ae0: 7472 2c20 2a2c 206e 6174 6976 653a 204c  tr, *, native: L
-00003af0: 6974 6572 616c 5b54 7275 655d 0d0a 2020  iteral[True]..  
-00003b00: 2020 2920 2d3e 2070 796d 6d63 6f72 652e    ) -> pymmcore.
-00003b10: 436f 6e66 6967 7572 6174 696f 6e3a 0d0a  Configuration:..
-00003b20: 2020 2020 2020 2020 2e2e 2e0d 0a0d 0a20          ....... 
-00003b30: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
-00003b40: 2020 6465 6620 6765 7443 6f6e 6669 6744    def getConfigD
-00003b50: 6174 6128 0d0a 2020 2020 2020 2020 7365  ata(..        se
-00003b60: 6c66 2c20 636f 6e66 6967 4772 6f75 703a  lf, configGroup:
-00003b70: 2073 7472 2c20 636f 6e66 6967 4e61 6d65   str, configName
-00003b80: 3a20 7374 722c 202a 2c20 6e61 7469 7665  : str, *, native
-00003b90: 3a20 4c69 7465 7261 6c5b 4661 6c73 655d  : Literal[False]
-00003ba0: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
-00003bb0: 2d3e 2043 6f6e 6669 6775 7261 7469 6f6e  -> Configuration
-00003bc0: 3a0d 0a20 2020 2020 2020 202e 2e2e 0d0a  :..        .....
-00003bd0: 0d0a 2020 2020 6465 6620 6765 7443 6f6e  ..    def getCon
-00003be0: 6669 6744 6174 6128 0d0a 2020 2020 2020  figData(..      
-00003bf0: 2020 7365 6c66 2c20 636f 6e66 6967 4772    self, configGr
-00003c00: 6f75 703a 2073 7472 2c20 636f 6e66 6967  oup: str, config
-00003c10: 4e61 6d65 3a20 7374 722c 202a 2c20 6e61  Name: str, *, na
-00003c20: 7469 7665 3a20 626f 6f6c 203d 2046 616c  tive: bool = Fal
-00003c30: 7365 0d0a 2020 2020 2920 2d3e 2043 6f6e  se..    ) -> Con
-00003c40: 6669 6775 7261 7469 6f6e 207c 2070 796d  figuration | pym
-00003c50: 6d63 6f72 652e 436f 6e66 6967 7572 6174  mcore.Configurat
-00003c60: 696f 6e3a 0d0a 2020 2020 2020 2020 2222  ion:..        ""
-00003c70: 2252 6574 7572 6e20 7468 6520 636f 6e66  "Return the conf
-00003c80: 6967 7572 6174 696f 6e20 6f62 6a65 6374  iguration object
-00003c90: 2066 6f72 2061 2067 6976 656e 2060 636f   for a given `co
-00003ca0: 6e66 6967 4772 6f75 7060 2061 6e64 2060  nfigGroup` and `
-00003cb0: 636f 6e66 6967 4e61 6d65 602e 0d0a 0d0a  configName`.....
-00003cc0: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
-00003cd0: 6572 7269 6465 3f2a 2a20 5468 6520 5b60  erride?** The [`
-00003ce0: 7079 6d6d 636f 7265 5f70 6c75 732e 436f  pymmcore_plus.Co
-00003cf0: 6e66 6967 7572 6174 696f 6e60 5d5b 5d20  nfiguration`][] 
-00003d00: 6f62 6a65 6374 2072 6574 7572 6e65 640d  object returned.
-00003d10: 0a20 2020 2020 2020 2077 6865 6e20 606e  .        when `n
-00003d20: 6174 6976 653d 4661 6c73 6560 2028 7468  ative=False` (th
-00003d30: 6520 6465 6661 756c 7429 2070 726f 7669  e default) provi
-00003d40: 6465 7320 6120 6e69 6365 7220 604d 6170  des a nicer `Map
-00003d50: 7069 6e67 6020 696e 7465 7266 6163 652e  ping` interface.
-00003d60: 2050 6173 730d 0a20 2020 2020 2020 2060   Pass..        `
-00003d70: 6e61 7469 7665 3d54 7275 6560 2074 6f20  native=True` to 
-00003d80: 6765 7420 7468 6520 6f72 6967 696e 616c  get the original
-00003d90: 2060 7079 6d6d 636f 7265 2e43 6f6e 6669   `pymmcore.Confi
-00003da0: 6775 7261 7469 6f6e 6020 6f62 6a65 6374  guration` object
-00003db0: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00003dc0: 2020 2020 2020 2020 6366 6720 3d20 7375          cfg = su
-00003dd0: 7065 7228 292e 6765 7443 6f6e 6669 6744  per().getConfigD
-00003de0: 6174 6128 636f 6e66 6967 4772 6f75 702c  ata(configGroup,
-00003df0: 2063 6f6e 6669 674e 616d 6529 0d0a 2020   configName)..  
-00003e00: 2020 2020 2020 7265 7475 726e 2063 6667        return cfg
-00003e10: 2069 6620 6e61 7469 7665 2065 6c73 6520   if native else 
-00003e20: 436f 6e66 6967 7572 6174 696f 6e2e 6672  Configuration.fr
-00003e30: 6f6d 5f63 6f6e 6669 6775 7261 7469 6f6e  om_configuration
-00003e40: 2863 6667 290d 0a0d 0a20 2020 2040 6f76  (cfg)....    @ov
-00003e50: 6572 6c6f 6164 0d0a 2020 2020 6465 6620  erload..    def 
-00003e60: 6765 7450 6978 656c 5369 7a65 436f 6e66  getPixelSizeConf
-00003e70: 6967 4461 7461 280d 0a20 2020 2020 2020  igData(..       
-00003e80: 2073 656c 662c 2063 6f6e 6669 674e 616d   self, configNam
-00003e90: 653a 2073 7472 2c20 2a2c 206e 6174 6976  e: str, *, nativ
-00003ea0: 653a 204c 6974 6572 616c 5b54 7275 655d  e: Literal[True]
-00003eb0: 0d0a 2020 2020 2920 2d3e 2070 796d 6d63  ..    ) -> pymmc
-00003ec0: 6f72 652e 436f 6e66 6967 7572 6174 696f  ore.Configuratio
-00003ed0: 6e3a 0d0a 2020 2020 2020 2020 2e2e 2e0d  n:..        ....
-00003ee0: 0a0d 0a20 2020 2040 6f76 6572 6c6f 6164  ...    @overload
-00003ef0: 0d0a 2020 2020 6465 6620 6765 7450 6978  ..    def getPix
-00003f00: 656c 5369 7a65 436f 6e66 6967 4461 7461  elSizeConfigData
-00003f10: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-00003f20: 2063 6f6e 6669 674e 616d 653a 2073 7472   configName: str
-00003f30: 2c20 2a2c 206e 6174 6976 653a 204c 6974  , *, native: Lit
-00003f40: 6572 616c 5b46 616c 7365 5d20 3d20 4661  eral[False] = Fa
-00003f50: 6c73 650d 0a20 2020 2029 202d 3e20 436f  lse..    ) -> Co
-00003f60: 6e66 6967 7572 6174 696f 6e3a 0d0a 2020  nfiguration:..  
-00003f70: 2020 2020 2020 2e2e 2e0d 0a0d 0a20 2020        .......   
-00003f80: 2064 6566 2067 6574 5069 7865 6c53 697a   def getPixelSiz
-00003f90: 6543 6f6e 6669 6744 6174 6128 0d0a 2020  eConfigData(..  
-00003fa0: 2020 2020 2020 7365 6c66 2c20 636f 6e66        self, conf
-00003fb0: 6967 4e61 6d65 3a20 7374 722c 202a 2c20  igName: str, *, 
-00003fc0: 6e61 7469 7665 3a20 626f 6f6c 203d 2046  native: bool = F
-00003fd0: 616c 7365 0d0a 2020 2020 2920 2d3e 2043  alse..    ) -> C
-00003fe0: 6f6e 6669 6775 7261 7469 6f6e 207c 2070  onfiguration | p
-00003ff0: 796d 6d63 6f72 652e 436f 6e66 6967 7572  ymmcore.Configur
-00004000: 6174 696f 6e3a 0d0a 2020 2020 2020 2020  ation:..        
-00004010: 2222 2252 6574 7572 6e20 7468 6520 636f  """Return the co
-00004020: 6e66 6967 7572 6174 696f 6e20 6f62 6a65  nfiguration obje
-00004030: 6374 2066 6f72 2061 2067 6976 656e 2070  ct for a given p
-00004040: 6978 656c 2073 697a 6520 7072 6573 6574  ixel size preset
-00004050: 2060 636f 6e66 6967 4e61 6d65 602e 0d0a   `configName`...
-00004060: 0d0a 2020 2020 2020 2020 2a2a 5768 7920  ..        **Why 
-00004070: 4f76 6572 7269 6465 3f2a 2a20 5468 6520  Override?** The 
-00004080: 5b60 7079 6d6d 636f 7265 5f70 6c75 732e  [`pymmcore_plus.
-00004090: 436f 6e66 6967 7572 6174 696f 6e60 5d5b  Configuration`][
-000040a0: 5d20 6f62 6a65 6374 2072 6574 7572 6e65  ] object returne
-000040b0: 640d 0a20 2020 2020 2020 2077 6865 6e20  d..        when 
-000040c0: 606e 6174 6976 653d 4661 6c73 6560 2028  `native=False` (
-000040d0: 7468 6520 6465 6661 756c 7429 2070 726f  the default) pro
-000040e0: 7669 6465 7320 6120 6e69 6365 7220 604d  vides a nicer `M
-000040f0: 6170 7069 6e67 6020 696e 7465 7266 6163  apping` interfac
-00004100: 652e 2050 6173 730d 0a20 2020 2020 2020  e. Pass..       
-00004110: 2060 6e61 7469 7665 3d54 7275 6560 2074   `native=True` t
-00004120: 6f20 6765 7420 7468 6520 6f72 6967 696e  o get the origin
-00004130: 616c 2060 7079 6d6d 636f 7265 2e43 6f6e  al `pymmcore.Con
-00004140: 6669 6775 7261 7469 6f6e 6020 6f62 6a65  figuration` obje
-00004150: 6374 2e0d 0a20 2020 2020 2020 2022 2222  ct...        """
-00004160: 0d0a 2020 2020 2020 2020 6366 6720 3d20  ..        cfg = 
-00004170: 7375 7065 7228 292e 6765 7450 6978 656c  super().getPixel
-00004180: 5369 7a65 436f 6e66 6967 4461 7461 2863  SizeConfigData(c
-00004190: 6f6e 6669 674e 616d 6529 0d0a 2020 2020  onfigName)..    
-000041a0: 2020 2020 7265 7475 726e 2063 6667 2069      return cfg i
-000041b0: 6620 6e61 7469 7665 2065 6c73 6520 436f  f native else Co
-000041c0: 6e66 6967 7572 6174 696f 6e2e 6672 6f6d  nfiguration.from
-000041d0: 5f63 6f6e 6669 6775 7261 7469 6f6e 2863  _configuration(c
-000041e0: 6667 290d 0a0d 0a20 2020 2040 6f76 6572  fg)....    @over
-000041f0: 6c6f 6164 0d0a 2020 2020 6465 6620 6765  load..    def ge
-00004200: 7443 6f6e 6669 6747 726f 7570 5374 6174  tConfigGroupStat
-00004210: 6528 0d0a 2020 2020 2020 2020 7365 6c66  e(..        self
-00004220: 2c20 6772 6f75 703a 2073 7472 2c20 2a2c  , group: str, *,
-00004230: 206e 6174 6976 653a 204c 6974 6572 616c   native: Literal
-00004240: 5b54 7275 655d 0d0a 2020 2020 2920 2d3e  [True]..    ) ->
-00004250: 2070 796d 6d63 6f72 652e 436f 6e66 6967   pymmcore.Config
-00004260: 7572 6174 696f 6e3a 0d0a 2020 2020 2020  uration:..      
-00004270: 2020 2e2e 2e0d 0a0d 0a20 2020 2040 6f76    .......    @ov
-00004280: 6572 6c6f 6164 0d0a 2020 2020 6465 6620  erload..    def 
-00004290: 6765 7443 6f6e 6669 6747 726f 7570 5374  getConfigGroupSt
-000042a0: 6174 6528 0d0a 2020 2020 2020 2020 7365  ate(..        se
-000042b0: 6c66 2c20 6772 6f75 703a 2073 7472 2c20  lf, group: str, 
-000042c0: 2a2c 206e 6174 6976 653a 204c 6974 6572  *, native: Liter
-000042d0: 616c 5b46 616c 7365 5d20 3d20 4661 6c73  al[False] = Fals
-000042e0: 650d 0a20 2020 2029 202d 3e20 436f 6e66  e..    ) -> Conf
-000042f0: 6967 7572 6174 696f 6e3a 0d0a 2020 2020  iguration:..    
-00004300: 2020 2020 2e2e 2e0d 0a0d 0a20 2020 2064      .......    d
-00004310: 6566 2067 6574 436f 6e66 6967 4772 6f75  ef getConfigGrou
-00004320: 7053 7461 7465 280d 0a20 2020 2020 2020  pState(..       
-00004330: 2073 656c 662c 2067 726f 7570 3a20 7374   self, group: st
-00004340: 722c 202a 2c20 6e61 7469 7665 3a20 626f  r, *, native: bo
-00004350: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
-00004360: 2920 2d3e 2043 6f6e 6669 6775 7261 7469  ) -> Configurati
-00004370: 6f6e 207c 2070 796d 6d63 6f72 652e 436f  on | pymmcore.Co
-00004380: 6e66 6967 7572 6174 696f 6e3a 0d0a 2020  nfiguration:..  
-00004390: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-000043a0: 7468 6520 7374 6174 6520 6f66 2074 6865  the state of the
-000043b0: 2064 6576 6963 6573 2069 6e63 6c75 6465   devices include
-000043c0: 6420 696e 2074 6865 2073 7065 6369 6669  d in the specifi
-000043d0: 6564 2060 6772 6f75 7060 2e0d 0a0d 0a20  ed `group`..... 
-000043e0: 2020 2020 2020 202a 2a57 6879 204f 7665         **Why Ove
-000043f0: 7272 6964 653f 2a2a 2054 6865 205b 6070  rride?** The [`p
-00004400: 796d 6d63 6f72 655f 706c 7573 2e43 6f6e  ymmcore_plus.Con
-00004410: 6669 6775 7261 7469 6f6e 605d 5b5d 206f  figuration`][] o
-00004420: 626a 6563 7420 7265 7475 726e 6564 0d0a  bject returned..
-00004430: 2020 2020 2020 2020 7768 656e 2060 6e61          when `na
-00004440: 7469 7665 3d46 616c 7365 6020 2874 6865  tive=False` (the
-00004450: 2064 6566 6175 6c74 2920 7072 6f76 6964   default) provid
-00004460: 6573 2061 206e 6963 6572 2060 4d61 7070  es a nicer `Mapp
-00004470: 696e 6760 2069 6e74 6572 6661 6365 2e20  ing` interface. 
-00004480: 5061 7373 0d0a 2020 2020 2020 2020 606e  Pass..        `n
-00004490: 6174 6976 653d 5472 7565 6020 746f 2067  ative=True` to g
-000044a0: 6574 2074 6865 206f 7269 6769 6e61 6c20  et the original 
-000044b0: 6070 796d 6d63 6f72 652e 436f 6e66 6967  `pymmcore.Config
-000044c0: 7572 6174 696f 6e60 206f 626a 6563 742e  uration` object.
-000044d0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000044e0: 2020 2020 2020 2063 6667 203d 2073 7570         cfg = sup
-000044f0: 6572 2829 2e67 6574 436f 6e66 6967 4772  er().getConfigGr
-00004500: 6f75 7053 7461 7465 2867 726f 7570 290d  oupState(group).
-00004510: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004520: 6366 6720 6966 206e 6174 6976 6520 656c  cfg if native el
-00004530: 7365 2043 6f6e 6669 6775 7261 7469 6f6e  se Configuration
-00004540: 2e66 726f 6d5f 636f 6e66 6967 7572 6174  .from_configurat
-00004550: 696f 6e28 6366 6729 0d0a 0d0a 2020 2020  ion(cfg)....    
-00004560: 6465 6620 6765 7443 6f6e 6669 6747 726f  def getConfigGro
-00004570: 7570 5374 6174 6546 726f 6d43 6163 6865  upStateFromCache
-00004580: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-00004590: 2067 726f 7570 3a20 7374 722c 202a 2c20   group: str, *, 
-000045a0: 6e61 7469 7665 3a20 626f 6f6c 203d 2046  native: bool = F
-000045b0: 616c 7365 0d0a 2020 2020 2920 2d3e 2043  alse..    ) -> C
-000045c0: 6f6e 6669 6775 7261 7469 6f6e 207c 2070  onfiguration | p
-000045d0: 796d 6d63 6f72 652e 436f 6e66 6967 7572  ymmcore.Configur
-000045e0: 6174 696f 6e3a 0d0a 2020 2020 2020 2020  ation:..        
-000045f0: 2222 2252 6574 7572 6e20 7468 6520 7374  """Return the st
-00004600: 6174 6520 6f66 2074 6865 2073 7973 7465  ate of the syste
-00004610: 6d20 6361 6368 652c 2066 6f72 2074 6865  m cache, for the
-00004620: 2064 6576 6963 6573 2069 6e20 7468 6520   devices in the 
-00004630: 7370 6563 6966 6965 6420 6772 6f75 702e  specified group.
-00004640: 0d0a 0d0a 2020 2020 2020 2020 2a2a 5768  ....        **Wh
-00004650: 7920 4f76 6572 7269 6465 3f2a 2a20 5468  y Override?** Th
-00004660: 6520 5b60 7079 6d6d 636f 7265 5f70 6c75  e [`pymmcore_plu
-00004670: 732e 436f 6e66 6967 7572 6174 696f 6e60  s.Configuration`
-00004680: 5d5b 5d20 6f62 6a65 6374 2072 6574 7572  ][] object retur
-00004690: 6e65 640d 0a20 2020 2020 2020 2077 6865  ned..        whe
-000046a0: 6e20 606e 6174 6976 653d 4661 6c73 6560  n `native=False`
-000046b0: 2028 7468 6520 6465 6661 756c 7429 2070   (the default) p
-000046c0: 726f 7669 6465 7320 6120 6e69 6365 7220  rovides a nicer 
-000046d0: 604d 6170 7069 6e67 6020 696e 7465 7266  `Mapping` interf
-000046e0: 6163 652e 2050 6173 730d 0a20 2020 2020  ace. Pass..     
-000046f0: 2020 2060 6e61 7469 7665 3d54 7275 6560     `native=True`
-00004700: 2074 6f20 6765 7420 7468 6520 6f72 6967   to get the orig
-00004710: 696e 616c 2060 7079 6d6d 636f 7265 2e43  inal `pymmcore.C
-00004720: 6f6e 6669 6775 7261 7469 6f6e 6020 6f62  onfiguration` ob
-00004730: 6a65 6374 2e0d 0a20 2020 2020 2020 2022  ject...        "
-00004740: 2222 0d0a 2020 2020 2020 2020 6366 6720  ""..        cfg 
-00004750: 3d20 7375 7065 7228 292e 6765 7443 6f6e  = super().getCon
-00004760: 6669 6747 726f 7570 5374 6174 6546 726f  figGroupStateFro
-00004770: 6d43 6163 6865 2867 726f 7570 290d 0a20  mCache(group).. 
-00004780: 2020 2020 2020 2072 6574 7572 6e20 6366         return cf
-00004790: 6720 6966 206e 6174 6976 6520 656c 7365  g if native else
-000047a0: 2043 6f6e 6669 6775 7261 7469 6f6e 2e66   Configuration.f
-000047b0: 726f 6d5f 636f 6e66 6967 7572 6174 696f  rom_configuratio
-000047c0: 6e28 6366 6729 0d0a 0d0a 2020 2020 6465  n(cfg)....    de
-000047d0: 6620 6765 7443 6f6e 6669 6753 7461 7465  f getConfigState
-000047e0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-000047f0: 2067 726f 7570 3a20 7374 722c 2063 6f6e   group: str, con
-00004800: 6669 673a 2073 7472 2c20 2a2c 206e 6174  fig: str, *, nat
-00004810: 6976 653a 2062 6f6f 6c20 3d20 4661 6c73  ive: bool = Fals
-00004820: 650d 0a20 2020 2029 202d 3e20 436f 6e66  e..    ) -> Conf
-00004830: 6967 7572 6174 696f 6e20 7c20 7079 6d6d  iguration | pymm
-00004840: 636f 7265 2e43 6f6e 6669 6775 7261 7469  core.Configurati
-00004850: 6f6e 3a0d 0a20 2020 2020 2020 2022 2222  on:..        """
-00004860: 5265 7475 726e 2073 7461 7465 206f 6620  Return state of 
-00004870: 6465 7669 6365 7320 696e 636c 7564 6564  devices included
-00004880: 2069 6e20 7468 6520 7370 6563 6966 6965   in the specifie
-00004890: 6420 636f 6e66 6967 7572 6174 696f 6e2e  d configuration.
-000048a0: 0d0a 0d0a 2020 2020 2020 2020 2a2a 5768  ....        **Wh
-000048b0: 7920 4f76 6572 7269 6465 3f2a 2a20 5468  y Override?** Th
-000048c0: 6520 5b60 7079 6d6d 636f 7265 5f70 6c75  e [`pymmcore_plu
-000048d0: 732e 436f 6e66 6967 7572 6174 696f 6e60  s.Configuration`
-000048e0: 5d5b 5d20 6f62 6a65 6374 2072 6574 7572  ][] object retur
-000048f0: 6e65 640d 0a20 2020 2020 2020 2077 6865  ned..        whe
-00004900: 6e20 606e 6174 6976 653d 4661 6c73 6560  n `native=False`
-00004910: 2028 7468 6520 6465 6661 756c 7429 2070   (the default) p
-00004920: 726f 7669 6465 7320 6120 6e69 6365 7220  rovides a nicer 
-00004930: 604d 6170 7069 6e67 6020 696e 7465 7266  `Mapping` interf
-00004940: 6163 652e 2050 6173 730d 0a20 2020 2020  ace. Pass..     
-00004950: 2020 2060 6e61 7469 7665 3d54 7275 6560     `native=True`
-00004960: 2074 6f20 6765 7420 7468 6520 6f72 6967   to get the orig
-00004970: 696e 616c 2060 7079 6d6d 636f 7265 2e43  inal `pymmcore.C
-00004980: 6f6e 6669 6775 7261 7469 6f6e 6020 6f62  onfiguration` ob
-00004990: 6a65 6374 2e0d 0a20 2020 2020 2020 2022  ject...        "
-000049a0: 2222 0d0a 2020 2020 2020 2020 6366 6720  ""..        cfg 
-000049b0: 3d20 7375 7065 7228 292e 6765 7443 6f6e  = super().getCon
-000049c0: 6669 6753 7461 7465 2867 726f 7570 2c20  figState(group, 
-000049d0: 636f 6e66 6967 290d 0a20 2020 2020 2020  config)..       
-000049e0: 2072 6574 7572 6e20 6366 6720 6966 206e   return cfg if n
-000049f0: 6174 6976 6520 656c 7365 2043 6f6e 6669  ative else Confi
-00004a00: 6775 7261 7469 6f6e 2e66 726f 6d5f 636f  guration.from_co
-00004a10: 6e66 6967 7572 6174 696f 6e28 6366 6729  nfiguration(cfg)
-00004a20: 0d0a 0d0a 2020 2020 6465 6620 6765 7453  ....    def getS
-00004a30: 7973 7465 6d53 7461 7465 280d 0a20 2020  ystemState(..   
-00004a40: 2020 2020 2073 656c 662c 202a 2c20 6e61       self, *, na
-00004a50: 7469 7665 3a20 626f 6f6c 203d 2046 616c  tive: bool = Fal
-00004a60: 7365 0d0a 2020 2020 2920 2d3e 2043 6f6e  se..    ) -> Con
-00004a70: 6669 6775 7261 7469 6f6e 207c 2070 796d  figuration | pym
-00004a80: 6d63 6f72 652e 436f 6e66 6967 7572 6174  mcore.Configurat
-00004a90: 696f 6e3a 0d0a 2020 2020 2020 2020 2222  ion:..        ""
-00004aa0: 2252 6574 7572 6e20 7468 6520 656e 7469  "Return the enti
-00004ab0: 7265 2073 7973 7465 6d20 7374 6174 652e  re system state.
-00004ac0: 0d0a 0d0a 2020 2020 2020 2020 2a2a 5768  ....        **Wh
-00004ad0: 7920 4f76 6572 7269 6465 3f2a 2a20 5468  y Override?** Th
-00004ae0: 6520 5b60 7079 6d6d 636f 7265 5f70 6c75  e [`pymmcore_plu
-00004af0: 732e 436f 6e66 6967 7572 6174 696f 6e60  s.Configuration`
-00004b00: 5d5b 5d20 6f62 6a65 6374 2072 6574 7572  ][] object retur
-00004b10: 6e65 640d 0a20 2020 2020 2020 2077 6865  ned..        whe
-00004b20: 6e20 606e 6174 6976 653d 4661 6c73 6560  n `native=False`
-00004b30: 2028 7468 6520 6465 6661 756c 7429 2070   (the default) p
-00004b40: 726f 7669 6465 7320 6120 6e69 6365 7220  rovides a nicer 
-00004b50: 604d 6170 7069 6e67 6020 696e 7465 7266  `Mapping` interf
-00004b60: 6163 652e 2050 6173 730d 0a20 2020 2020  ace. Pass..     
-00004b70: 2020 2060 6e61 7469 7665 3d54 7275 6560     `native=True`
-00004b80: 2074 6f20 6765 7420 7468 6520 6f72 6967   to get the orig
-00004b90: 696e 616c 2060 7079 6d6d 636f 7265 2e43  inal `pymmcore.C
-00004ba0: 6f6e 6669 6775 7261 7469 6f6e 6020 6f62  onfiguration` ob
-00004bb0: 6a65 6374 2e0d 0a20 2020 2020 2020 2022  ject...        "
-00004bc0: 2222 0d0a 2020 2020 2020 2020 6366 6720  ""..        cfg 
-00004bd0: 3d20 7375 7065 7228 292e 6765 7453 7973  = super().getSys
-00004be0: 7465 6d53 7461 7465 2829 0d0a 2020 2020  temState()..    
-00004bf0: 2020 2020 7265 7475 726e 2063 6667 2069      return cfg i
-00004c00: 6620 6e61 7469 7665 2065 6c73 6520 436f  f native else Co
-00004c10: 6e66 6967 7572 6174 696f 6e2e 6672 6f6d  nfiguration.from
-00004c20: 5f63 6f6e 6669 6775 7261 7469 6f6e 2863  _configuration(c
-00004c30: 6667 290d 0a0d 0a20 2020 2064 6566 2067  fg)....    def g
-00004c40: 6574 5379 7374 656d 5374 6174 6543 6163  etSystemStateCac
-00004c50: 6865 280d 0a20 2020 2020 2020 2073 656c  he(..        sel
-00004c60: 662c 202a 2c20 6e61 7469 7665 3a20 626f  f, *, native: bo
-00004c70: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
-00004c80: 2920 2d3e 2043 6f6e 6669 6775 7261 7469  ) -> Configurati
-00004c90: 6f6e 207c 2070 796d 6d63 6f72 652e 436f  on | pymmcore.Co
-00004ca0: 6e66 6967 7572 6174 696f 6e3a 0d0a 2020  nfiguration:..  
-00004cb0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00004cc0: 7468 6520 656e 7469 7265 2073 7973 7465  the entire syste
-00004cd0: 6d20 7374 6174 6520 6672 6f6d 2063 6163  m state from cac
-00004ce0: 6865 2e0d 0a0d 0a20 2020 2020 2020 202a  he.....        *
-00004cf0: 2a57 6879 204f 7665 7272 6964 653f 2a2a  *Why Override?**
-00004d00: 2054 6865 205b 6070 796d 6d63 6f72 655f   The [`pymmcore_
-00004d10: 706c 7573 2e43 6f6e 6669 6775 7261 7469  plus.Configurati
-00004d20: 6f6e 605d 5b5d 206f 626a 6563 7420 7265  on`][] object re
-00004d30: 7475 726e 6564 0d0a 2020 2020 2020 2020  turned..        
-00004d40: 7768 656e 2060 6e61 7469 7665 3d46 616c  when `native=Fal
-00004d50: 7365 6020 2874 6865 2064 6566 6175 6c74  se` (the default
-00004d60: 2920 7072 6f76 6964 6573 2061 206e 6963  ) provides a nic
-00004d70: 6572 2060 4d61 7070 696e 6760 2069 6e74  er `Mapping` int
-00004d80: 6572 6661 6365 2e20 5061 7373 0d0a 2020  erface. Pass..  
-00004d90: 2020 2020 2020 606e 6174 6976 653d 5472        `native=Tr
-00004da0: 7565 6020 746f 2067 6574 2074 6865 206f  ue` to get the o
-00004db0: 7269 6769 6e61 6c20 6070 796d 6d63 6f72  riginal `pymmcor
-00004dc0: 652e 436f 6e66 6967 7572 6174 696f 6e60  e.Configuration`
-00004dd0: 206f 626a 6563 742e 0d0a 2020 2020 2020   object...      
-00004de0: 2020 2222 220d 0a20 2020 2020 2020 2063    """..        c
-00004df0: 6667 203d 2073 7570 6572 2829 2e67 6574  fg = super().get
-00004e00: 5379 7374 656d 5374 6174 6543 6163 6865  SystemStateCache
-00004e10: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
-00004e20: 726e 2063 6667 2069 6620 6e61 7469 7665  rn cfg if native
-00004e30: 2065 6c73 6520 436f 6e66 6967 7572 6174   else Configurat
-00004e40: 696f 6e2e 6672 6f6d 5f63 6f6e 6669 6775  ion.from_configu
-00004e50: 7261 7469 6f6e 2863 6667 290d 0a0d 0a20  ration(cfg).... 
-00004e60: 2020 2023 206d 6574 6164 6174 6120 6d65     # metadata me
-00004e70: 7468 6f64 7320 7468 6174 2064 6f6e 2774  thods that don't
-00004e80: 2072 6571 7569 7265 2069 6e73 7461 6e74   require instant
-00004e90: 6961 7469 6e67 206d 6574 6164 6174 6120  iating metadata 
-00004ea0: 6669 7273 740d 0a0d 0a20 2020 2040 6f76  first....    @ov
-00004eb0: 6572 6c6f 6164 0d0a 2020 2020 6465 6620  erload..    def 
-00004ec0: 6765 744c 6173 7449 6d61 6765 416e 644d  getLastImageAndM
-00004ed0: 4428 0d0a 2020 2020 2020 2020 7365 6c66  D(..        self
-00004ee0: 2c20 6368 616e 6e65 6c3a 2069 6e74 2c20  , channel: int, 
-00004ef0: 736c 6963 653a 2069 6e74 2c20 2a2c 2066  slice: int, *, f
-00004f00: 6978 3a20 626f 6f6c 203d 2054 7275 650d  ix: bool = True.
-00004f10: 0a20 2020 2029 202d 3e20 7475 706c 655b  .    ) -> tuple[
-00004f20: 6e70 2e6e 6461 7272 6179 2c20 4d65 7461  np.ndarray, Meta
-00004f30: 6461 7461 5d3a 0d0a 2020 2020 2020 2020  data]:..        
-00004f40: 2e2e 2e0d 0a0d 0a20 2020 2040 6f76 6572  .......    @over
-00004f50: 6c6f 6164 0d0a 2020 2020 6465 6620 6765  load..    def ge
-00004f60: 744c 6173 7449 6d61 6765 416e 644d 4428  tLastImageAndMD(
-00004f70: 7365 6c66 2c20 2a2c 2066 6978 3a20 626f  self, *, fix: bo
-00004f80: 6f6c 203d 2054 7275 6529 202d 3e20 7475  ol = True) -> tu
-00004f90: 706c 655b 6e70 2e6e 6461 7272 6179 2c20  ple[np.ndarray, 
-00004fa0: 4d65 7461 6461 7461 5d3a 0d0a 2020 2020  Metadata]:..    
-00004fb0: 2020 2020 2e2e 2e0d 0a0d 0a20 2020 2040      .......    @
-00004fc0: 7379 6e63 6872 6f6e 697a 6564 285f 6c6f  synchronized(_lo
-00004fd0: 636b 290d 0a20 2020 2064 6566 2067 6574  ck)..    def get
-00004fe0: 4c61 7374 496d 6167 6541 6e64 4d44 280d  LastImageAndMD(.
-00004ff0: 0a20 2020 2020 2020 2073 656c 662c 2063  .        self, c
-00005000: 6861 6e6e 656c 3a20 696e 7420 7c20 4e6f  hannel: int | No
-00005010: 6e65 203d 204e 6f6e 652c 2073 6c69 6365  ne = None, slice
-00005020: 3a20 696e 7420 7c20 4e6f 6e65 203d 204e  : int | None = N
-00005030: 6f6e 652c 202a 2c20 6669 783a 2062 6f6f  one, *, fix: boo
-00005040: 6c20 3d20 5472 7565 0d0a 2020 2020 2920  l = True..    ) 
-00005050: 2d3e 2074 7570 6c65 5b6e 702e 6e64 6172  -> tuple[np.ndar
-00005060: 7261 792c 204d 6574 6164 6174 615d 3a0d  ray, Metadata]:.
-00005070: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00005080: 726e 206c 6173 7420 696d 6167 6520 6672  rn last image fr
-00005090: 6f6d 2074 6865 2063 6972 6375 6c61 7220  om the circular 
-000050a0: 6275 6666 6572 2061 6c6f 6e67 2077 6974  buffer along wit
-000050b0: 6820 6d65 7461 6461 7461 2e0d 0a0d 0a20  h metadata..... 
-000050c0: 2020 2020 2020 203a 7370 6172 6b6c 6573         :sparkles
-000050d0: 3a20 2a54 6869 7320 6d65 7468 6f64 2069  : *This method i
-000050e0: 7320 6e65 7720 696e 2060 434d 4d43 6f72  s new in `CMMCor
-000050f0: 6550 6c75 7360 2e2a 0d0a 0d0a 2020 2020  ePlus`.*....    
-00005100: 2020 2020 5468 6973 2069 7320 6120 636f      This is a co
-00005110: 6e76 656e 6965 6e63 6520 6d65 7468 6f64  nvenience method
-00005120: 2074 6861 7420 6973 2076 6572 7920 7369   that is very si
-00005130: 6d69 6c61 7220 746f 2060 6765 744c 6173  milar to `getLas
-00005140: 7449 6d61 6765 4d44 602c 2065 7863 6570  tImageMD`, excep
-00005150: 740d 0a20 2020 2020 2020 2074 6861 7420  t..        that 
-00005160: 6974 2064 6f65 736e 2774 2072 6571 7569  it doesn't requi
-00005170: 7265 2069 6e73 7461 6e74 6961 7469 6e67  re instantiating
-00005180: 2061 2060 4d65 7461 4461 7461 6020 6f62   a `MetaData` ob
-00005190: 6a65 6374 2066 6972 7374 2e20 4974 2072  ject first. It r
-000051a0: 6574 7572 6e73 2061 0d0a 2020 2020 2020  eturns a..      
-000051b0: 2020 7475 706c 6520 636f 6e74 6169 6e69    tuple containi
-000051c0: 6e67 2074 6865 2069 6d61 6765 2061 6e64  ng the image and
-000051d0: 2061 205b 6070 796d 6d63 6f72 655f 706c   a [`pymmcore_pl
-000051e0: 7573 2e4d 6574 6164 6174 6160 5d5b 5d20  us.Metadata`][] 
-000051f0: 6f62 6a65 6374 2e0d 0a0d 0a20 2020 2020  object.....     
-00005200: 2020 2049 7420 616c 736f 2061 6464 7320     It also adds 
-00005210: 6120 6066 6978 6020 7061 7261 6d65 7465  a `fix` paramete
-00005220: 722c 2077 6869 6368 2072 6573 6861 7065  r, which reshape
-00005230: 7320 6d75 6c74 692d 636f 6d70 6f6e 656e  s multi-componen
-00005240: 740d 0a20 2020 2020 2020 2069 6d61 6765  t..        image
-00005250: 7320 286c 696b 6520 5247 4220 696d 6167  s (like RGB imag
-00005260: 6573 2920 746f 2028 772c 2068 2c20 6e5f  es) to (w, h, n_
-00005270: 636f 6d70 6f6e 656e 7473 2920 7573 696e  components) usin
-00005280: 670d 0a20 2020 2020 2020 205b 6066 6978  g..        [`fix
-00005290: 496d 6167 6560 5d5b 7079 6d6d 636f 7265  Image`][pymmcore
-000052a0: 5f70 6c75 732e 434d 4d43 6f72 6550 6c75  _plus.CMMCorePlu
-000052b0: 732e 6669 7849 6d61 6765 5d20 6279 2064  s.fixImage] by d
-000052c0: 6566 6175 6c74 2e0d 0a0d 0a20 2020 2020  efault.....     
-000052d0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-000052e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000052f0: 2d0d 0a20 2020 2020 2020 2063 6861 6e6e  -..        chann
-00005300: 656c 203a 2069 6e74 2c20 6f70 7469 6f6e  el : int, option
-00005310: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
-00005320: 4368 616e 6e65 6c20 696e 6465 782c 2062  Channel index, b
-00005330: 7920 6465 6661 756c 7420 4e6f 6e65 0d0a  y default None..
-00005340: 2020 2020 2020 2020 736c 6963 6520 3a20          slice : 
-00005350: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
-00005360: 2020 2020 2020 2020 2020 2053 6c69 6365             Slice
-00005370: 2069 6e64 6578 2c20 6279 2064 6566 6175   index, by defau
-00005380: 6c74 204e 6f6e 650d 0a20 2020 2020 2020  lt None..       
-00005390: 2066 6978 203a 2062 6f6f 6c2c 2064 6566   fix : bool, def
-000053a0: 6175 6c74 3a20 5472 7565 0d0a 2020 2020  ault: True..    
-000053b0: 2020 2020 2020 2020 4966 2060 5472 7565          If `True
-000053c0: 6020 2874 6865 2064 6566 6175 6c74 292c  ` (the default),
-000053d0: 2074 6865 6e20 696d 6167 6573 2077 6974   then images wit
-000053e0: 6820 6e5f 636f 6d70 6f6e 656e 7473 203e  h n_components >
-000053f0: 2031 2028 6c69 6b65 2052 4742 2069 6d61   1 (like RGB ima
-00005400: 6765 7329 0d0a 2020 2020 2020 2020 2020  ges)..          
-00005410: 2020 7769 6c6c 2062 6520 7265 7368 6170    will be reshap
-00005420: 6564 2074 6f20 2877 2c20 682c 206e 5f63  ed to (w, h, n_c
-00005430: 6f6d 706f 6e65 6e74 7329 2075 7369 6e67  omponents) using
-00005440: 2060 6669 7849 6d61 6765 602e 0d0a 0d0a   `fixImage`.....
-00005450: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
-00005460: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00005470: 0d0a 2020 2020 2020 2020 7475 706c 655b  ..        tuple[
-00005480: 6e70 2e6e 6461 7272 6179 2c20 4d65 7461  np.ndarray, Meta
-00005490: 6461 7461 5d0d 0a20 2020 2020 2020 2020  data]..         
-000054a0: 2020 2049 6d61 6765 2061 6e64 206d 6574     Image and met
-000054b0: 6164 6174 610d 0a20 2020 2020 2020 2022  adata..        "
-000054c0: 2222 0d0a 2020 2020 2020 2020 6d64 203d  ""..        md =
-000054d0: 204d 6574 6164 6174 6128 290d 0a20 2020   Metadata()..   
-000054e0: 2020 2020 2069 6620 6368 616e 6e65 6c20       if channel 
-000054f0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00005500: 736c 6963 6520 6973 206e 6f74 204e 6f6e  slice is not Non
-00005510: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00005520: 696d 6720 3d20 7375 7065 7228 292e 6765  img = super().ge
-00005530: 744c 6173 7449 6d61 6765 4d44 2863 6861  tLastImageMD(cha
-00005540: 6e6e 656c 2c20 736c 6963 652c 206d 6429  nnel, slice, md)
-00005550: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00005560: 0a20 2020 2020 2020 2020 2020 2069 6d67  .            img
-00005570: 203d 2073 7570 6572 2829 2e67 6574 4c61   = super().getLa
-00005580: 7374 496d 6167 654d 4428 6d64 290d 0a20  stImageMD(md).. 
-00005590: 2020 2020 2020 2072 6574 7572 6e20 2873         return (s
-000055a0: 656c 662e 6669 7849 6d61 6765 2869 6d67  elf.fixImage(img
-000055b0: 2920 6966 2066 6978 2065 6c73 6520 696d  ) if fix else im
-000055c0: 672c 206d 6429 0d0a 0d0a 2020 2020 406f  g, md)....    @o
-000055d0: 7665 726c 6f61 640d 0a20 2020 2064 6566  verload..    def
-000055e0: 2070 6f70 4e65 7874 496d 6167 6541 6e64   popNextImageAnd
-000055f0: 4d44 2873 656c 662c 2063 6861 6e6e 656c  MD(self, channel
-00005600: 3a20 696e 742c 2073 6c69 6365 3a20 696e  : int, slice: in
-00005610: 742c 202a 2c20 6669 783a 2062 6f6f 6c20  t, *, fix: bool 
-00005620: 3d20 5472 7565 2920 2d3e 2041 6e79 3a0d  = True) -> Any:.
-00005630: 0a20 2020 2020 2020 202e 2e2e 0d0a 0d0a  .        .......
-00005640: 2020 2020 406f 7665 726c 6f61 640d 0a20      @overload.. 
-00005650: 2020 2064 6566 2070 6f70 4e65 7874 496d     def popNextIm
-00005660: 6167 6541 6e64 4d44 2873 656c 662c 202a  ageAndMD(self, *
-00005670: 2c20 6669 783a 2062 6f6f 6c20 3d20 5472  , fix: bool = Tr
-00005680: 7565 2920 2d3e 2041 6e79 3a0d 0a20 2020  ue) -> Any:..   
-00005690: 2020 2020 202e 2e2e 0d0a 0d0a 2020 2020       .......    
-000056a0: 4073 796e 6368 726f 6e69 7a65 6428 5f6c  @synchronized(_l
-000056b0: 6f63 6b29 0d0a 2020 2020 6465 6620 706f  ock)..    def po
-000056c0: 704e 6578 7449 6d61 6765 416e 644d 4428  pNextImageAndMD(
-000056d0: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
-000056e0: 6368 616e 6e65 6c3a 2069 6e74 207c 204e  channel: int | N
-000056f0: 6f6e 6520 3d20 4e6f 6e65 2c20 736c 6963  one = None, slic
-00005700: 653a 2069 6e74 207c 204e 6f6e 6520 3d20  e: int | None = 
-00005710: 4e6f 6e65 2c20 2a2c 2066 6978 3a20 626f  None, *, fix: bo
-00005720: 6f6c 203d 2054 7275 650d 0a20 2020 2029  ol = True..    )
-00005730: 202d 3e20 7475 706c 655b 6e70 2e6e 6461   -> tuple[np.nda
-00005740: 7272 6179 2c20 4d65 7461 6461 7461 5d3a  rray, Metadata]:
-00005750: 0d0a 2020 2020 2020 2020 2222 2247 6574  ..        """Get
-00005760: 7320 616e 6420 7265 6d6f 7665 7320 7468  s and removes th
-00005770: 6520 6e65 7874 2069 6d61 6765 2028 616e  e next image (an
-00005780: 6420 6d65 7461 6461 7461 2920 6672 6f6d  d metadata) from
-00005790: 2074 6865 2063 6972 6375 6c61 7220 6275   the circular bu
-000057a0: 6666 6572 2e0d 0a0d 0a20 2020 2020 2020  ffer.....       
-000057b0: 203a 7370 6172 6b6c 6573 3a20 2a54 6869   :sparkles: *Thi
-000057c0: 7320 6d65 7468 6f64 2069 7320 6e65 7720  s method is new 
-000057d0: 696e 2060 434d 4d43 6f72 6550 6c75 7360  in `CMMCorePlus`
-000057e0: 2e2a 0d0a 0d0a 2020 2020 2020 2020 5468  .*....        Th
-000057f0: 6973 2069 7320 6120 636f 6e76 656e 6965  is is a convenie
-00005800: 6e63 6520 6d65 7468 6f64 2074 6861 7420  nce method that 
-00005810: 6973 2076 6572 7920 7369 6d69 6c61 7220  is very similar 
-00005820: 746f 2060 706f 704e 6578 7449 6d61 6765  to `popNextImage
-00005830: 4d44 602c 2065 7863 6570 740d 0a20 2020  MD`, except..   
-00005840: 2020 2020 2074 6861 7420 6974 2064 6f65       that it doe
-00005850: 736e 2774 2072 6571 7569 7265 2069 6e73  sn't require ins
-00005860: 7461 6e74 6961 7469 6e67 2061 2060 4d65  tantiating a `Me
-00005870: 7461 4461 7461 6020 6f62 6a65 6374 2066  taData` object f
-00005880: 6972 7374 2e20 4974 2072 6574 7572 6e73  irst. It returns
-00005890: 2061 0d0a 2020 2020 2020 2020 7475 706c   a..        tupl
-000058a0: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-000058b0: 2069 6d61 6765 2061 6e64 2061 205b 6070   image and a [`p
-000058c0: 796d 6d63 6f72 655f 706c 7573 2e4d 6574  ymmcore_plus.Met
-000058d0: 6164 6174 6160 5d5b 5d20 6f62 6a65 6374  adata`][] object
-000058e0: 2e0d 0a0d 0a20 2020 2020 2020 2049 7420  .....        It 
-000058f0: 616c 736f 2061 6464 7320 6120 6066 6978  also adds a `fix
-00005900: 6020 7061 7261 6d65 7465 722c 2077 6869  ` parameter, whi
-00005910: 6368 2072 6573 6861 7065 7320 6d75 6c74  ch reshapes mult
-00005920: 692d 636f 6d70 6f6e 656e 740d 0a20 2020  i-component..   
-00005930: 2020 2020 2069 6d61 6765 7320 286c 696b       images (lik
-00005940: 6520 5247 4220 696d 6167 6573 2920 746f  e RGB images) to
-00005950: 2028 772c 2068 2c20 6e5f 636f 6d70 6f6e   (w, h, n_compon
-00005960: 656e 7473 2920 7573 696e 670d 0a20 2020  ents) using..   
-00005970: 2020 2020 205b 6066 6978 496d 6167 6560       [`fixImage`
-00005980: 5d5b 7079 6d6d 636f 7265 5f70 6c75 732e  ][pymmcore_plus.
-00005990: 434d 4d43 6f72 6550 6c75 732e 6669 7849  CMMCorePlus.fixI
-000059a0: 6d61 6765 5d20 6279 2064 6566 6175 6c74  mage] by default
-000059b0: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-000059c0: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-000059d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-000059e0: 2020 2020 2063 6861 6e6e 656c 203a 2069       channel : i
-000059f0: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
-00005a00: 2020 2020 2020 2020 2020 4368 616e 6e65            Channe
-00005a10: 6c20 696e 6465 782c 2062 7920 6465 6661  l index, by defa
-00005a20: 756c 7420 4e6f 6e65 0d0a 2020 2020 2020  ult None..      
-00005a30: 2020 736c 6963 6520 3a20 696e 742c 206f    slice : int, o
-00005a40: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00005a50: 2020 2020 2053 6c69 6365 2069 6e64 6578       Slice index
-00005a60: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-00005a70: 650d 0a20 2020 2020 2020 2066 6978 203a  e..        fix :
-00005a80: 2062 6f6f 6c2c 2064 6566 6175 6c74 3a20   bool, default: 
-00005a90: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
-00005aa0: 2020 4966 2060 5472 7565 6020 2874 6865    If `True` (the
-00005ab0: 2064 6566 6175 6c74 292c 2074 6865 6e20   default), then 
-00005ac0: 696d 6167 6573 2077 6974 6820 6e5f 636f  images with n_co
-00005ad0: 6d70 6f6e 656e 7473 203e 2031 2028 6c69  mponents > 1 (li
-00005ae0: 6b65 2052 4742 2069 6d61 6765 7329 0d0a  ke RGB images)..
-00005af0: 2020 2020 2020 2020 2020 2020 7769 6c6c              will
-00005b00: 2062 6520 7265 7368 6170 6564 2074 6f20   be reshaped to 
-00005b10: 2877 2c20 682c 206e 5f63 6f6d 706f 6e65  (w, h, n_compone
-00005b20: 6e74 7329 2075 7369 6e67 2060 6669 7849  nts) using `fixI
-00005b30: 6d61 6765 602e 0d0a 0d0a 2020 2020 2020  mage`.....      
-00005b40: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
-00005b50: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-00005b60: 2020 2020 7475 706c 655b 6e70 2e6e 6461      tuple[np.nda
-00005b70: 7272 6179 2c20 4d65 7461 6461 7461 5d0d  rray, Metadata].
-00005b80: 0a20 2020 2020 2020 2020 2020 2049 6d61  .            Ima
-00005b90: 6765 2061 6e64 206d 6574 6164 6174 610d  ge and metadata.
-00005ba0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005bb0: 2020 2020 2020 6d64 203d 204d 6574 6164        md = Metad
-00005bc0: 6174 6128 290d 0a20 2020 2020 2020 2069  ata()..        i
-00005bd0: 6620 6368 616e 6e65 6c20 6973 206e 6f74  f channel is not
-00005be0: 204e 6f6e 6520 616e 6420 736c 6963 6520   None and slice 
-00005bf0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00005c00: 2020 2020 2020 2020 2020 696d 6720 3d20            img = 
-00005c10: 7375 7065 7228 292e 706f 704e 6578 7449  super().popNextI
-00005c20: 6d61 6765 4d44 2863 6861 6e6e 656c 2c20  mageMD(channel, 
-00005c30: 736c 6963 652c 206d 6429 0d0a 2020 2020  slice, md)..    
-00005c40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00005c50: 2020 2020 2020 2069 6d67 203d 2073 7570         img = sup
-00005c60: 6572 2829 2e70 6f70 4e65 7874 496d 6167  er().popNextImag
-00005c70: 654d 4428 6d64 290d 0a20 2020 2020 2020  eMD(md)..       
-00005c80: 2072 6574 7572 6e20 2873 656c 662e 6669   return (self.fi
-00005c90: 7849 6d61 6765 2869 6d67 2920 6966 2066  xImage(img) if f
-00005ca0: 6978 2065 6c73 6520 696d 672c 206d 6429  ix else img, md)
-00005cb0: 0d0a 0d0a 2020 2020 4073 796e 6368 726f  ....    @synchro
-00005cc0: 6e69 7a65 6428 5f6c 6f63 6b29 0d0a 2020  nized(_lock)..  
-00005cd0: 2020 6465 6620 706f 704e 6578 7449 6d61    def popNextIma
-00005ce0: 6765 2873 656c 662c 202a 2c20 6669 783a  ge(self, *, fix:
-00005cf0: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
-00005d00: 206e 702e 6e64 6172 7261 793a 0d0a 2020   np.ndarray:..  
-00005d10: 2020 2020 2020 2222 2247 6574 7320 616e        """Gets an
-00005d20: 6420 7265 6d6f 7665 7320 7468 6520 6e65  d removes the ne
-00005d30: 7874 2069 6d61 6765 2066 726f 6d20 7468  xt image from th
-00005d40: 6520 6369 7263 756c 6172 2062 7566 6665  e circular buffe
-00005d50: 722e 0d0a 0d0a 2020 2020 2020 2020 2a2a  r.....        **
-00005d60: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
-00005d70: 746f 2061 6464 2074 6865 2060 6669 7860  to add the `fix`
-00005d80: 2070 6172 616d 6574 6572 2c20 7768 6963   parameter, whic
-00005d90: 6820 7265 7368 6170 6573 206d 756c 7469  h reshapes multi
-00005da0: 2d63 6f6d 706f 6e65 6e74 0d0a 2020 2020  -component..    
-00005db0: 2020 2020 696d 6167 6573 2028 6c69 6b65      images (like
-00005dc0: 2052 4742 2069 6d61 6765 7329 2074 6f20   RGB images) to 
-00005dd0: 2877 2c20 682c 206e 5f63 6f6d 706f 6e65  (w, h, n_compone
-00005de0: 6e74 7329 2075 7369 6e67 0d0a 2020 2020  nts) using..    
-00005df0: 2020 2020 5b60 6669 7849 6d61 6765 605d      [`fixImage`]
-00005e00: 5b70 796d 6d63 6f72 655f 706c 7573 2e43  [pymmcore_plus.C
-00005e10: 4d4d 436f 7265 506c 7573 2e66 6978 496d  MMCorePlus.fixIm
-00005e20: 6167 655d 2062 7920 6465 6661 756c 742e  age] by default.
-00005e30: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-00005e40: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
-00005e50: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-00005e60: 2020 2020 6669 7820 3a20 626f 6f6c 2c20      fix : bool, 
-00005e70: 6465 6661 756c 743a 2054 7275 650d 0a20  default: True.. 
-00005e80: 2020 2020 2020 2020 2020 2049 6620 6054             If `T
-00005e90: 7275 6560 2028 7468 6520 6465 6661 756c  rue` (the defaul
-00005ea0: 7429 2c20 7468 656e 2069 6d61 6765 7320  t), then images 
-00005eb0: 7769 7468 206e 5f63 6f6d 706f 6e65 6e74  with n_component
-00005ec0: 7320 3e20 3120 286c 696b 6520 5247 4220  s > 1 (like RGB 
-00005ed0: 696d 6167 6573 290d 0a20 2020 2020 2020  images)..       
-00005ee0: 2020 2020 2077 696c 6c20 6265 2072 6573       will be res
-00005ef0: 6861 7065 6420 746f 2028 772c 2068 2c20  haped to (w, h, 
-00005f00: 6e5f 636f 6d70 6f6e 656e 7473 2920 7573  n_components) us
-00005f10: 696e 6720 6066 6978 496d 6167 6560 2e0d  ing `fixImage`..
-00005f20: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005f30: 2020 2020 2020 696d 673a 206e 702e 6e64        img: np.nd
-00005f40: 6172 7261 7920 3d20 7375 7065 7228 292e  array = super().
-00005f50: 706f 704e 6578 7449 6d61 6765 2829 0d0a  popNextImage()..
-00005f60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005f70: 656c 662e 6669 7849 6d61 6765 2869 6d67  elf.fixImage(img
-00005f80: 2920 6966 2066 6978 2065 6c73 6520 696d  ) if fix else im
-00005f90: 670d 0a0d 0a20 2020 2040 7379 6e63 6872  g....    @synchr
-00005fa0: 6f6e 697a 6564 285f 6c6f 636b 290d 0a20  onized(_lock).. 
-00005fb0: 2020 2064 6566 2067 6574 4e42 6566 6f72     def getNBefor
-00005fc0: 654c 6173 7449 6d61 6765 416e 644d 4428  eLastImageAndMD(
-00005fd0: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
-00005fe0: 6e3a 2069 6e74 2c20 2a2c 2066 6978 3a20  n: int, *, fix: 
-00005ff0: 626f 6f6c 203d 2054 7275 650d 0a20 2020  bool = True..   
-00006000: 2029 202d 3e20 7475 706c 655b 6e70 2e6e   ) -> tuple[np.n
-00006010: 6461 7272 6179 2c20 4d65 7461 6461 7461  darray, Metadata
-00006020: 5d3a 0d0a 2020 2020 2020 2020 2222 2252  ]:..        """R
-00006030: 6574 7572 6e20 696d 6167 6520 7461 6b65  eturn image take
-00006040: 6e20 606e 6020 696d 6167 6573 2061 676f  n `n` images ago
-00006050: 2061 6c6f 6e67 2077 6974 6820 6173 736f   along with asso
-00006060: 6369 6174 6564 206d 6574 6164 6174 612e  ciated metadata.
-00006070: 0d0a 0d0a 2020 2020 2020 2020 3a73 7061  ....        :spa
-00006080: 726b 6c65 733a 202a 5468 6973 206d 6574  rkles: *This met
-00006090: 686f 6420 6973 206e 6577 2069 6e20 6043  hod is new in `C
-000060a0: 4d4d 436f 7265 506c 7573 602e 2a0d 0a0d  MMCorePlus`.*...
-000060b0: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
-000060c0: 2061 2063 6f6e 7665 6e69 656e 6365 206d   a convenience m
-000060d0: 6574 686f 6420 7468 6174 2069 7320 7665  ethod that is ve
-000060e0: 7279 2073 696d 696c 6172 2074 6f20 6067  ry similar to `g
-000060f0: 6574 4e42 6566 6f72 654c 6173 7449 6d61  etNBeforeLastIma
-00006100: 6765 4d44 602c 0d0a 2020 2020 2020 2020  geMD`,..        
-00006110: 6578 6365 7074 2074 6861 7420 6974 2064  except that it d
-00006120: 6f65 736e 2774 2072 6571 7569 7265 2069  oesn't require i
-00006130: 6e73 7461 6e74 6961 7469 6e67 2061 2060  nstantiating a `
-00006140: 4d65 7461 4461 7461 6020 6f62 6a65 6374  MetaData` object
-00006150: 2066 6972 7374 2e20 4974 0d0a 2020 2020   first. It..    
-00006160: 2020 2020 7265 7475 726e 7320 6120 7475      returns a tu
-00006170: 706c 6520 636f 6e74 6169 6e69 6e67 2074  ple containing t
-00006180: 6865 2069 6d61 6765 2061 6e64 2061 205b  he image and a [
-00006190: 6070 796d 6d63 6f72 655f 706c 7573 2e4d  `pymmcore_plus.M
-000061a0: 6574 6164 6174 6160 5d5b 5d20 6f62 6a65  etadata`][] obje
-000061b0: 6374 2e0d 0a0d 0a20 2020 2020 2020 2049  ct.....        I
-000061c0: 7420 616c 736f 2061 6464 7320 6120 6066  t also adds a `f
-000061d0: 6978 6020 7061 7261 6d65 7465 722c 2077  ix` parameter, w
-000061e0: 6869 6368 2072 6573 6861 7065 7320 6d75  hich reshapes mu
-000061f0: 6c74 692d 636f 6d70 6f6e 656e 740d 0a20  lti-component.. 
-00006200: 2020 2020 2020 2069 6d61 6765 7320 286c         images (l
-00006210: 696b 6520 5247 4220 696d 6167 6573 2920  ike RGB images) 
-00006220: 746f 2028 772c 2068 2c20 6e5f 636f 6d70  to (w, h, n_comp
-00006230: 6f6e 656e 7473 2920 7573 696e 670d 0a20  onents) using.. 
-00006240: 2020 2020 2020 205b 6066 6978 496d 6167         [`fixImag
-00006250: 6560 5d5b 7079 6d6d 636f 7265 5f70 6c75  e`][pymmcore_plu
-00006260: 732e 434d 4d43 6f72 6550 6c75 732e 6669  s.CMMCorePlus.fi
-00006270: 7849 6d61 6765 5d20 6279 2064 6566 6175  xImage] by defau
-00006280: 6c74 2e0d 0a0d 0a20 2020 2020 2020 2050  lt.....        P
-00006290: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-000062a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-000062b0: 2020 2020 2020 206e 203a 2069 6e74 0d0a         n : int..
-000062c0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000062d0: 6e75 6d62 6572 206f 6620 696d 6167 6573  number of images
-000062e0: 2061 676f 2074 6f20 7265 7472 6965 7665   ago to retrieve
-000062f0: 2e20 3020 6973 2074 6865 206c 6173 7420  . 0 is the last 
-00006300: 696d 6167 652c 2031 2069 7320 7468 650d  image, 1 is the.
-00006310: 0a20 2020 2020 2020 2020 2020 2069 6d61  .            ima
-00006320: 6765 2062 6566 6f72 6520 7468 6174 2c20  ge before that, 
-00006330: 6574 632e 0d0a 2020 2020 2020 2020 6669  etc...        fi
-00006340: 7820 3a20 626f 6f6c 2c20 6465 6661 756c  x : bool, defaul
-00006350: 743a 2054 7275 650d 0a20 2020 2020 2020  t: True..       
-00006360: 2020 2020 2049 6620 6054 7275 6560 2028       If `True` (
-00006370: 7468 6520 6465 6661 756c 7429 2c20 7468  the default), th
-00006380: 656e 2069 6d61 6765 7320 7769 7468 206e  en images with n
-00006390: 5f63 6f6d 706f 6e65 6e74 7320 3e20 3120  _components > 1 
-000063a0: 286c 696b 6520 5247 4220 696d 6167 6573  (like RGB images
-000063b0: 290d 0a20 2020 2020 2020 2020 2020 2077  )..            w
-000063c0: 696c 6c20 6265 2072 6573 6861 7065 6420  ill be reshaped 
-000063d0: 746f 2028 772c 2068 2c20 6e5f 636f 6d70  to (w, h, n_comp
-000063e0: 6f6e 656e 7473 2920 7573 696e 6720 6066  onents) using `f
-000063f0: 6978 496d 6167 6560 2e0d 0a20 2020 2020  ixImage`...     
-00006400: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00006410: 6d64 203d 204d 6574 6164 6174 6128 290d  md = Metadata().
-00006420: 0a20 2020 2020 2020 2069 6d67 203d 2073  .        img = s
-00006430: 7570 6572 2829 2e67 6574 4e42 6566 6f72  uper().getNBefor
-00006440: 654c 6173 7449 6d61 6765 4d44 286e 2c20  eLastImageMD(n, 
-00006450: 6d64 290d 0a20 2020 2020 2020 2072 6574  md)..        ret
-00006460: 7572 6e20 7365 6c66 2e66 6978 496d 6167  urn self.fixImag
-00006470: 6528 696d 6729 2069 6620 6669 7820 656c  e(img) if fix el
-00006480: 7365 2069 6d67 2c20 6d64 0d0a 0d0a 2020  se img, md....  
-00006490: 2020 6465 6620 7365 7443 6f6e 6669 6728    def setConfig(
-000064a0: 7365 6c66 2c20 6772 6f75 704e 616d 653a  self, groupName:
-000064b0: 2073 7472 2c20 636f 6e66 6967 4e61 6d65   str, configName
-000064c0: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0d  : str) -> None:.
-000064d0: 0a20 2020 2020 2020 2022 2222 4170 706c  .        """Appl
-000064e0: 6965 7320 6120 636f 6e66 6967 7572 6174  ies a configurat
-000064f0: 696f 6e20 746f 2061 2067 726f 7570 2e0d  ion to a group..
-00006500: 0a0d 0a20 2020 2020 2020 202a 2a57 6879  ...        **Why
-00006510: 204f 7665 7272 6964 653f 2a2a 2054 6865   Override?** The
-00006520: 206e 6174 6976 6520 606f 6e43 6f6e 6669   native `onConfi
-00006530: 6747 726f 7570 4368 616e 6765 6460 2063  gGroupChanged` c
-00006540: 616c 6c62 6163 6b20 6973 206e 6f74 2061  allback is not a
-00006550: 6c77 6179 730d 0a20 2020 2020 2020 2063  lways..        c
-00006560: 616c 6c65 6420 7768 656e 6576 6572 2060  alled whenever `
-00006570: 434d 4d43 6f72 652e 7365 7443 6f6e 6669  CMMCore.setConfi
-00006580: 6760 2068 6173 2062 6565 6e20 6361 6c6c  g` has been call
-00006590: 6564 2e20 5765 206f 7665 7272 6964 6520  ed. We override 
-000065a0: 6865 7265 2074 6f20 656d 6974 0d0a 2020  here to emit..  
-000065b0: 2020 2020 2020 6120 6063 6f6e 6669 6753        a `configS
-000065c0: 6574 6020 6576 656e 7420 7768 656e 6576  et` event whenev
-000065d0: 6572 2060 7365 7443 6f6e 6669 6760 2069  er `setConfig` i
-000065e0: 7320 6361 6c6c 6564 2e0d 0a20 2020 2020  s called...     
-000065f0: 2020 2053 6565 203c 6874 7470 733a 2f2f     See <https://
-00006600: 6769 7468 7562 2e63 6f6d 2f6d 6963 726f  github.com/micro
-00006610: 2d6d 616e 6167 6572 2f6d 6d43 6f72 6541  -manager/mmCoreA
-00006620: 6e64 4465 7669 6365 732f 6973 7375 6573  ndDevices/issues
-00006630: 2f32 353e 2066 6f72 2064 6574 6169 6c73  /25> for details
-00006640: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00006650: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00006660: 7365 7443 6f6e 6669 6728 6772 6f75 704e  setConfig(groupN
-00006670: 616d 652c 2063 6f6e 6669 674e 616d 6529  ame, configName)
-00006680: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-00006690: 7665 6e74 732e 636f 6e66 6967 5365 742e  vents.configSet.
-000066a0: 656d 6974 2867 726f 7570 4e61 6d65 2c20  emit(groupName, 
-000066b0: 636f 6e66 6967 4e61 6d65 290d 0a0d 0a20  configName).... 
-000066c0: 2020 2023 204e 4557 206d 6574 686f 6473     # NEW methods
-000066d0: 0d0a 0d0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
-000066e0: 640d 0a20 2020 2064 6566 2069 7465 7244  d..    def iterD
-000066f0: 6576 6963 6541 6461 7074 6572 7328 0d0a  eviceAdapters(..
-00006700: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00006710: 2020 2020 2020 2061 6461 7074 6572 5f70         adapter_p
-00006720: 6174 7465 726e 3a20 7374 7220 7c20 7265  attern: str | re
-00006730: 2e50 6174 7465 726e 207c 204e 6f6e 6520  .Pattern | None 
-00006740: 3d20 2e2e 2e2c 0d0a 2020 2020 2020 2020  = ...,..        
-00006750: 2a2c 0d0a 2020 2020 2020 2020 6173 5f6f  *,..        as_o
-00006760: 626a 6563 743a 204c 6974 6572 616c 5b54  bject: Literal[T
-00006770: 7275 655d 203d 202e 2e2e 2c0d 0a20 2020  rue] = ...,..   
-00006780: 2029 202d 3e20 4974 6572 6174 6f72 5b44   ) -> Iterator[D
-00006790: 6576 6963 6541 6461 7074 6572 5d3a 0d0a  eviceAdapter]:..
-000067a0: 2020 2020 2020 2020 2e2e 2e0d 0a0d 0a20          ....... 
-000067b0: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
-000067c0: 2020 6465 6620 6974 6572 4465 7669 6365    def iterDevice
-000067d0: 4164 6170 7465 7273 280d 0a20 2020 2020  Adapters(..     
-000067e0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-000067f0: 2020 6164 6170 7465 725f 7061 7474 6572    adapter_patter
-00006800: 6e3a 2073 7472 207c 2072 652e 5061 7474  n: str | re.Patt
-00006810: 6572 6e20 7c20 4e6f 6e65 203d 202e 2e2e  ern | None = ...
-00006820: 2c0d 0a20 2020 2020 2020 202a 2c0d 0a20  ,..        *,.. 
-00006830: 2020 2020 2020 2061 735f 6f62 6a65 6374         as_object
-00006840: 3a20 4c69 7465 7261 6c5b 4661 6c73 655d  : Literal[False]
-00006850: 2c0d 0a20 2020 2029 202d 3e20 4974 6572  ,..    ) -> Iter
-00006860: 6174 6f72 5b73 7472 5d3a 0d0a 2020 2020  ator[str]:..    
-00006870: 2020 2020 2e2e 2e0d 0a0d 0a20 2020 2064      .......    d
-00006880: 6566 2069 7465 7244 6576 6963 6541 6461  ef iterDeviceAda
-00006890: 7074 6572 7328 0d0a 2020 2020 2020 2020  pters(..        
-000068a0: 7365 6c66 2c0d 0a20 2020 2020 2020 2061  self,..        a
-000068b0: 6461 7074 6572 5f70 6174 7465 726e 3a20  dapter_pattern: 
-000068c0: 7374 7220 7c20 7265 2e50 6174 7465 726e  str | re.Pattern
-000068d0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0d   | None = None,.
-000068e0: 0a20 2020 2020 2020 202a 2c0d 0a20 2020  .        *,..   
-000068f0: 2020 2020 2061 735f 6f62 6a65 6374 3a20       as_object: 
-00006900: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
-00006910: 2020 2920 2d3e 2049 7465 7261 746f 725b    ) -> Iterator[
-00006920: 4465 7669 6365 4164 6170 7465 725d 207c  DeviceAdapter] |
-00006930: 2049 7465 7261 746f 725b 7374 725d 3a0d   Iterator[str]:.
-00006940: 0a20 2020 2020 2020 2022 2222 4974 6572  .        """Iter
-00006950: 6174 6520 6f76 6572 2061 6c6c 2061 7661  ate over all ava
-00006960: 696c 6162 6c65 2064 6576 6963 6520 6164  ilable device ad
-00006970: 6170 7465 7273 2e0d 0a0d 0a20 2020 2020  apters.....     
-00006980: 2020 203a 7370 6172 6b6c 6573 3a20 2a54     :sparkles: *T
-00006990: 6869 7320 6d65 7468 6f64 2069 7320 6e65  his method is ne
-000069a0: 7720 696e 2060 434d 4d43 6f72 6550 6c75  w in `CMMCorePlu
-000069b0: 7360 2e2a 0d0a 0d0a 2020 2020 2020 2020  s`.*....        
-000069c0: 4974 206f 6666 6572 7320 6120 636f 6e76  It offers a conv
-000069d0: 656e 6965 6e74 2077 6179 2074 6f20 6974  enient way to it
-000069e0: 6572 6174 6520 6f76 6572 2061 7661 696c  erate over avail
-000069f0: 6162 6520 6465 7669 6365 2061 6461 7074  abe device adapt
-00006a00: 6f72 206c 6962 7261 7269 6573 2c0d 0a20  or libraries,.. 
-00006a10: 2020 2020 2020 206f 7074 696f 6e61 6c6c         optionall
-00006a20: 7920 6669 6c74 6572 696e 6720 6164 6170  y filtering adap
-00006a30: 7465 7220 6c69 6272 6172 7920 6e61 6d65  ter library name
-00006a40: 2e20 4974 2063 616e 2061 6c73 6f20 7969  . It can also yi
-00006a50: 656c 640d 0a20 2020 2020 2020 205b 6041  eld..        [`A
-00006a60: 6461 7074 6572 605d 5b70 796d 6d63 6f72  dapter`][pymmcor
-00006a70: 655f 706c 7573 2e44 6576 6963 6541 6461  e_plus.DeviceAda
-00006a80: 7074 6572 5d20 6f62 6a65 6374 7320 6966  pter] objects if
-00006a90: 2060 6173 5f6f 626a 6563 7460 2069 7320   `as_object` is 
-00006aa0: 6054 7275 6560 2028 7468 650d 0a20 2020  `True` (the..   
-00006ab0: 2020 2020 2064 6566 6175 6c74 290d 0a0d       default)...
-00006ac0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00006ad0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-00006ae0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-00006af0: 2061 6461 7074 6572 5f70 6174 7465 726e   adapter_pattern
-00006b00: 203a 2073 7472 207c 204e 6f6e 650d 0a20   : str | None.. 
-00006b10: 2020 2020 2020 2020 2020 2044 6576 6963             Devic
-00006b20: 6520 6164 6170 7465 7220 6e61 6d65 206f  e adapter name o
-00006b30: 7220 7061 7474 6572 6e20 746f 2066 696c  r pattern to fil
-00006b40: 7465 7220 6279 2c20 6279 2064 6566 6175  ter by, by defau
-00006b50: 6c74 2061 6c6c 2064 6576 6963 6520 6164  lt all device ad
-00006b60: 6170 7465 7273 0d0a 2020 2020 2020 2020  apters..        
-00006b70: 2020 2020 7769 6c6c 2062 6520 7969 656c      will be yiel
-00006b80: 6465 642e 0d0a 2020 2020 2020 2020 6173  ded...        as
-00006b90: 5f6f 626a 6563 7420 3a20 626f 6f6c 2c20  _object : bool, 
-00006ba0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00006bb0: 2020 2020 2020 4966 2060 5472 7565 602c        If `True`,
-00006bc0: 2060 4164 6170 7465 7260 206f 626a 6563   `Adapter` objec
-00006bd0: 7473 2077 696c 6c20 6265 2079 6965 6c64  ts will be yield
-00006be0: 6564 2069 6e73 7465 6164 206f 660d 0a20  ed instead of.. 
-00006bf0: 2020 2020 2020 2020 2020 206c 6962 7261             libra
-00006c00: 7279 206e 616d 6520 7374 7269 6e67 732e  ry name strings.
-00006c10: 2042 7920 6465 6661 756c 7420 5472 7565   By default True
-00006c20: 0d0a 0d0a 2020 2020 2020 2020 5969 656c  ....        Yiel
-00006c30: 6473 0d0a 2020 2020 2020 2020 2d2d 2d2d  ds..        ----
-00006c40: 2d2d 0d0a 2020 2020 2020 2020 4465 7669  --..        Devi
-00006c50: 6365 207c 2073 7472 0d0a 2020 2020 2020  ce | str..      
-00006c60: 2020 2020 2020 6044 6576 6963 6560 206f        `Device` o
-00006c70: 626a 6563 7473 2028 6966 2060 6173 5f6f  bjects (if `as_o
-00006c80: 626a 6563 743d 3d54 7275 6560 2920 6f72  bject==True`) or
-00006c90: 2064 6576 6963 6520 6c61 6265 6c20 7374   device label st
-00006ca0: 7269 6e67 732e 0d0a 2020 2020 2020 2020  rings...        
-00006cb0: 2222 220d 0a20 2020 2020 2020 2061 6461  """..        ada
-00006cc0: 7074 6572 733a 2053 6571 7565 6e63 655b  pters: Sequence[
-00006cd0: 7374 725d 203d 2073 7570 6572 2829 2e67  str] = super().g
-00006ce0: 6574 4465 7669 6365 4164 6170 7465 724e  etDeviceAdapterN
-00006cf0: 616d 6573 2829 0d0a 0d0a 2020 2020 2020  ames()....      
-00006d00: 2020 6966 2061 6461 7074 6572 5f70 6174    if adapter_pat
-00006d10: 7465 726e 3a0d 0a20 2020 2020 2020 2020  tern:..         
-00006d20: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00006d30: 2861 6461 7074 6572 5f70 6174 7465 726e  (adapter_pattern
-00006d40: 2c20 7374 7229 3a0d 0a20 2020 2020 2020  , str):..       
-00006d50: 2020 2020 2020 2020 2070 7472 6e20 3d20           ptrn = 
-00006d60: 7265 2e63 6f6d 7069 6c65 2861 6461 7074  re.compile(adapt
-00006d70: 6572 5f70 6174 7465 726e 2c20 7265 2e49  er_pattern, re.I
-00006d80: 474e 4f52 4543 4153 4529 0d0a 2020 2020  GNORECASE)..    
-00006d90: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00006da0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006db0: 7472 6e20 3d20 6164 6170 7465 725f 7061  trn = adapter_pa
-00006dc0: 7474 6572 6e0d 0a20 2020 2020 2020 2020  ttern..         
-00006dd0: 2020 2061 6461 7074 6572 7320 3d20 5b64     adapters = [d
-00006de0: 2066 6f72 2064 2069 6e20 6164 6170 7465   for d in adapte
-00006df0: 7273 2069 6620 7074 726e 2e73 6561 7263  rs if ptrn.searc
-00006e00: 6828 6429 5d0d 0a0d 0a20 2020 2020 2020  h(d)]....       
-00006e10: 2066 6f72 2061 6461 7074 6572 2069 6e20   for adapter in 
-00006e20: 6164 6170 7465 7273 3a0d 0a20 2020 2020  adapters:..     
-00006e30: 2020 2020 2020 2079 6965 6c64 2044 6576         yield Dev
-00006e40: 6963 6541 6461 7074 6572 2861 6461 7074  iceAdapter(adapt
-00006e50: 6572 2c20 6d6d 636f 7265 3d73 656c 6629  er, mmcore=self)
-00006e60: 2069 6620 6173 5f6f 626a 6563 7420 656c   if as_object el
-00006e70: 7365 2061 6461 7074 6572 0d0a 0d0a 2020  se adapter....  
-00006e80: 2020 406f 7665 726c 6f61 640d 0a20 2020    @overload..   
-00006e90: 2064 6566 2069 7465 7244 6576 6963 6573   def iterDevices
-00006ea0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-00006eb0: 0d0a 2020 2020 2020 2020 6465 7669 6365  ..        device
-00006ec0: 5f74 7970 653a 2069 6e74 207c 2049 7465  _type: int | Ite
-00006ed0: 7261 626c 655b 696e 745d 207c 204e 6f6e  rable[int] | Non
-00006ee0: 6520 3d20 2e2e 2e2c 0d0a 2020 2020 2020  e = ...,..      
-00006ef0: 2020 6465 7669 6365 5f6c 6162 656c 3a20    device_label: 
-00006f00: 7374 7220 7c20 7265 2e50 6174 7465 726e  str | re.Pattern
-00006f10: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0d0a   | None = ...,..
-00006f20: 2020 2020 2020 2020 6465 7669 6365 5f61          device_a
-00006f30: 6461 7074 6572 3a20 7374 7220 7c20 7265  dapter: str | re
-00006f40: 2e50 6174 7465 726e 207c 204e 6f6e 6520  .Pattern | None 
-00006f50: 3d20 2e2e 2e2c 0d0a 2020 2020 2020 2020  = ...,..        
-00006f60: 2a2c 0d0a 2020 2020 2020 2020 6173 5f6f  *,..        as_o
-00006f70: 626a 6563 743a 204c 6974 6572 616c 5b46  bject: Literal[F
-00006f80: 616c 7365 5d2c 0d0a 2020 2020 2920 2d3e  alse],..    ) ->
-00006f90: 2049 7465 7261 746f 725b 7374 725d 3a0d   Iterator[str]:.
-00006fa0: 0a20 2020 2020 2020 202e 2e2e 0d0a 0d0a  .        .......
-00006fb0: 2020 2020 406f 7665 726c 6f61 640d 0a20      @overload.. 
-00006fc0: 2020 2064 6566 2069 7465 7244 6576 6963     def iterDevic
-00006fd0: 6573 280d 0a20 2020 2020 2020 2073 656c  es(..        sel
-00006fe0: 662c 0d0a 2020 2020 2020 2020 6465 7669  f,..        devi
-00006ff0: 6365 5f74 7970 653a 2069 6e74 207c 2049  ce_type: int | I
-00007000: 7465 7261 626c 655b 696e 745d 207c 204e  terable[int] | N
-00007010: 6f6e 6520 3d20 2e2e 2e2c 0d0a 2020 2020  one = ...,..    
-00007020: 2020 2020 6465 7669 6365 5f6c 6162 656c      device_label
-00007030: 3a20 7374 7220 7c20 7265 2e50 6174 7465  : str | re.Patte
-00007040: 726e 207c 204e 6f6e 6520 3d20 2e2e 2e2c  rn | None = ...,
-00007050: 0d0a 2020 2020 2020 2020 6465 7669 6365  ..        device
-00007060: 5f61 6461 7074 6572 3a20 7374 7220 7c20  _adapter: str | 
-00007070: 7265 2e50 6174 7465 726e 207c 204e 6f6e  re.Pattern | Non
-00007080: 6520 3d20 2e2e 2e2c 0d0a 2020 2020 2020  e = ...,..      
-00007090: 2020 2a2c 0d0a 2020 2020 2020 2020 6173    *,..        as
-000070a0: 5f6f 626a 6563 743a 204c 6974 6572 616c  _object: Literal
-000070b0: 5b54 7275 655d 203d 202e 2e2e 2c0d 0a20  [True] = ...,.. 
-000070c0: 2020 2029 202d 3e20 4974 6572 6174 6f72     ) -> Iterator
-000070d0: 5b44 6576 6963 655d 3a0d 0a20 2020 2020  [Device]:..     
-000070e0: 2020 202e 2e2e 0d0a 0d0a 2020 2020 6465     .......    de
-000070f0: 6620 6974 6572 4465 7669 6365 7328 0d0a  f iterDevices(..
-00007100: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00007110: 2020 2020 2020 2064 6576 6963 655f 7479         device_ty
-00007120: 7065 3a20 696e 7420 7c20 4974 6572 6162  pe: int | Iterab
-00007130: 6c65 5b69 6e74 5d20 7c20 4e6f 6e65 203d  le[int] | None =
-00007140: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00007150: 6465 7669 6365 5f6c 6162 656c 3a20 7374  device_label: st
-00007160: 7220 7c20 7265 2e50 6174 7465 726e 207c  r | re.Pattern |
-00007170: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
-00007180: 2020 2020 2020 2064 6576 6963 655f 6164         device_ad
-00007190: 6170 7465 723a 2073 7472 207c 2072 652e  apter: str | re.
-000071a0: 5061 7474 6572 6e20 7c20 4e6f 6e65 203d  Pattern | None =
-000071b0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-000071c0: 2a2c 0d0a 2020 2020 2020 2020 6173 5f6f  *,..        as_o
-000071d0: 626a 6563 743a 2062 6f6f 6c20 3d20 5472  bject: bool = Tr
-000071e0: 7565 2c0d 0a20 2020 2029 202d 3e20 4974  ue,..    ) -> It
-000071f0: 6572 6174 6f72 5b44 6576 6963 655d 207c  erator[Device] |
-00007200: 2049 7465 7261 746f 725b 7374 725d 3a0d   Iterator[str]:.
-00007210: 0a20 2020 2020 2020 2022 2222 4974 6572  .        """Iter
-00007220: 6174 6520 6f76 6572 2063 7572 7265 6e74  ate over current
-00007230: 6c79 206c 6f61 6465 6420 6465 7669 6365  ly loaded device
-00007240: 732e 0d0a 0d0a 2020 2020 2020 2020 3a73  s.....        :s
-00007250: 7061 726b 6c65 733a 202a 5468 6973 206d  parkles: *This m
-00007260: 6574 686f 6420 6973 206e 6577 2069 6e20  ethod is new in 
-00007270: 6043 4d4d 436f 7265 506c 7573 602e 2a0d  `CMMCorePlus`.*.
-00007280: 0a0d 0a20 2020 2020 2020 2049 7420 6f66  ...        It of
-00007290: 6665 7273 2061 2063 6f6e 7665 6e69 656e  fers a convenien
-000072a0: 7420 7761 7920 746f 2069 7465 7261 7465  t way to iterate
-000072b0: 206f 7665 7220 6c6f 6164 6564 2064 6576   over loaded dev
-000072c0: 6963 6573 2c20 6f70 7469 6f6e 616c 6c79  ices, optionally
-000072d0: 2066 696c 7465 7269 6e67 0d0a 2020 2020   filtering..    
-000072e0: 2020 2020 6279 205b 6044 6576 6963 6554      by [`DeviceT
-000072f0: 7970 6560 5d5b 7079 6d6d 636f 7265 5f70  ype`][pymmcore_p
-00007300: 6c75 732e 4465 7669 6365 5479 7065 5d20  lus.DeviceType] 
-00007310: 616e 642f 6f72 2064 6576 6963 6520 6c61  and/or device la
-00007320: 6265 6c2e 2049 7420 6361 6e20 616c 736f  bel. It can also
-00007330: 0d0a 2020 2020 2020 2020 7969 656c 6420  ..        yield 
-00007340: 5b60 4465 7669 6365 605d 5b70 796d 6d63  [`Device`][pymmc
-00007350: 6f72 655f 706c 7573 2e44 6576 6963 655d  ore_plus.Device]
-00007360: 206f 626a 6563 7473 2069 6620 6061 735f   objects if `as_
-00007370: 6f62 6a65 6374 6020 6973 0d0a 2020 2020  object` is..    
-00007380: 2020 2020 6054 7275 6560 2028 7468 6520      `True` (the 
-00007390: 6465 6661 756c 7429 2e0d 0a0d 0a20 2020  default).....   
-000073a0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-000073b0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000073c0: 2d2d 2d0d 0a20 2020 2020 2020 2064 6576  ---..        dev
-000073d0: 6963 655f 7479 7065 203a 2044 6576 6963  ice_type : Devic
-000073e0: 6554 7970 6520 7c20 4e6f 6e65 0d0a 2020  eType | None..  
-000073f0: 2020 2020 2020 2020 2020 4465 7669 6365            Device
-00007400: 5479 7065 2074 6f20 6669 6c74 6572 2062  Type to filter b
-00007410: 792c 2062 7920 6465 6661 756c 7420 616c  y, by default al
-00007420: 6c20 6465 7669 6365 2074 7970 6573 2077  l device types w
-00007430: 696c 6c20 6265 2079 6965 6c64 6564 2e0d  ill be yielded..
-00007440: 0a20 2020 2020 2020 2064 6576 6963 655f  .        device_
-00007450: 6c61 6265 6c20 3a20 7374 7220 7c20 4e6f  label : str | No
-00007460: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00007470: 4465 7669 6365 206c 6162 656c 2074 6f20  Device label to 
-00007480: 6669 6c74 6572 2062 792c 2062 7920 6465  filter by, by de
-00007490: 6661 756c 7420 616c 6c20 6465 7669 6365  fault all device
-000074a0: 206c 6162 656c 7320 7769 6c6c 2062 6520   labels will be 
-000074b0: 7969 656c 6465 642e 0d0a 2020 2020 2020  yielded...      
-000074c0: 2020 6465 7669 6365 5f61 6461 7074 6572    device_adapter
-000074d0: 203a 2073 7472 207c 204e 6f6e 650d 0a20   : str | None.. 
-000074e0: 2020 2020 2020 2020 2020 2044 6576 6963             Devic
-000074f0: 6520 6164 6170 7465 7220 6c69 6272 6172  e adapter librar
-00007500: 7920 746f 2066 696c 7465 7220 6279 2c20  y to filter by, 
-00007510: 6279 2064 6566 6175 6c74 2064 6576 6963  by default devic
-00007520: 6573 2066 726f 6d20 616c 6c20 6c69 6272  es from all libr
-00007530: 6172 6965 730d 0a20 2020 2020 2020 2020  aries..         
-00007540: 2020 2077 696c 6c20 6265 2079 6965 6c64     will be yield
-00007550: 6564 2e0d 0a20 2020 2020 2020 2061 735f  ed...        as_
-00007560: 6f62 6a65 6374 203a 2062 6f6f 6c2c 206f  object : bool, o
-00007570: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00007580: 2020 2020 2049 6620 6054 7275 6560 2c20       If `True`, 
-00007590: 6044 6576 6963 6560 206f 626a 6563 7473  `Device` objects
-000075a0: 2077 696c 6c20 6265 2079 6965 6c64 6564   will be yielded
-000075b0: 2069 6e73 7465 6164 206f 660d 0a20 2020   instead of..   
-000075c0: 2020 2020 2020 2020 2064 6576 6963 6520           device 
-000075d0: 6c61 6265 6c20 7374 7269 6e67 732e 2042  label strings. B
-000075e0: 7920 6465 6661 756c 7420 5472 7565 0d0a  y default True..
-000075f0: 0d0a 2020 2020 2020 2020 5969 656c 6473  ..        Yields
-00007600: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00007610: 0d0a 2020 2020 2020 2020 4465 7669 6365  ..        Device
-00007620: 207c 2073 7472 0d0a 2020 2020 2020 2020   | str..        
-00007630: 2020 2020 6044 6576 6963 6560 206f 626a      `Device` obj
-00007640: 6563 7473 2028 6966 2060 6173 5f6f 626a  ects (if `as_obj
-00007650: 6563 743d 3d54 7275 6560 2920 6f72 2064  ect==True`) or d
-00007660: 6576 6963 6520 6c61 6265 6c20 7374 7269  evice label stri
-00007670: 6e67 732e 0d0a 2020 2020 2020 2020 2222  ngs...        ""
-00007680: 220d 0a20 2020 2020 2020 2069 6620 6465  "..        if de
-00007690: 7669 6365 5f74 7970 6520 6973 204e 6f6e  vice_type is Non
-000076a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000076b0: 6465 7669 6365 733a 2053 6571 7565 6e63  devices: Sequenc
-000076c0: 655b 7374 725d 203d 2073 656c 662e 6765  e[str] = self.ge
-000076d0: 744c 6f61 6465 6444 6576 6963 6573 2829  tLoadedDevices()
-000076e0: 0d0a 2020 2020 2020 2020 656c 6966 2069  ..        elif i
-000076f0: 7369 6e73 7461 6e63 6528 6465 7669 6365  sinstance(device
-00007700: 5f74 7970 652c 2069 6e74 293a 0d0a 2020  _type, int):..  
-00007710: 2020 2020 2020 2020 2020 6465 7669 6365            device
-00007720: 7320 3d20 7365 6c66 2e67 6574 4c6f 6164  s = self.getLoad
-00007730: 6564 4465 7669 6365 734f 6654 7970 6528  edDevicesOfType(
-00007740: 6465 7669 6365 5f74 7970 6529 0d0a 2020  device_type)..  
-00007750: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00007760: 2020 2020 2020 2020 205f 6465 7669 6365           _device
-00007770: 733a 2073 6574 5b73 7472 5d20 3d20 7365  s: set[str] = se
-00007780: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-00007790: 2066 6f72 2064 7479 7065 2069 6e20 6465   for dtype in de
-000077a0: 7669 6365 5f74 7970 653a 0d0a 2020 2020  vice_type:..    
-000077b0: 2020 2020 2020 2020 2020 2020 5f64 6576              _dev
-000077c0: 6963 6573 2e75 7064 6174 6528 7365 6c66  ices.update(self
-000077d0: 2e67 6574 4c6f 6164 6564 4465 7669 6365  .getLoadedDevice
-000077e0: 734f 6654 7970 6528 6474 7970 6529 290d  sOfType(dtype)).
-000077f0: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
-00007800: 6963 6573 203d 206c 6973 7428 5f64 6576  ices = list(_dev
-00007810: 6963 6573 290d 0a0d 0a20 2020 2020 2020  ices)....       
-00007820: 2069 6620 6465 7669 6365 5f6c 6162 656c   if device_label
-00007830: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00007840: 6620 6973 696e 7374 616e 6365 2864 6576  f isinstance(dev
-00007850: 6963 655f 6c61 6265 6c2c 2073 7472 293a  ice_label, str):
-00007860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007870: 2020 7074 726e 203d 2072 652e 636f 6d70    ptrn = re.comp
-00007880: 696c 6528 6465 7669 6365 5f6c 6162 656c  ile(device_label
-00007890: 2c20 7265 2e49 474e 4f52 4543 4153 4529  , re.IGNORECASE)
-000078a0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000078b0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000078c0: 2020 2020 2070 7472 6e20 3d20 6465 7669       ptrn = devi
-000078d0: 6365 5f6c 6162 656c 0d0a 2020 2020 2020  ce_label..      
-000078e0: 2020 2020 2020 6465 7669 6365 7320 3d20        devices = 
-000078f0: 5b64 2066 6f72 2064 2069 6e20 6465 7669  [d for d in devi
-00007900: 6365 7320 6966 2070 7472 6e2e 7365 6172  ces if ptrn.sear
-00007910: 6368 2864 295d 0d0a 0d0a 2020 2020 2020  ch(d)]....      
-00007920: 2020 6966 2064 6576 6963 655f 6164 6170    if device_adap
-00007930: 7465 723a 0d0a 2020 2020 2020 2020 2020  ter:..          
-00007940: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00007950: 6465 7669 6365 5f61 6461 7074 6572 2c20  device_adapter, 
-00007960: 7374 7229 3a0d 0a20 2020 2020 2020 2020  str):..         
-00007970: 2020 2020 2020 2070 7472 6e20 3d20 7265         ptrn = re
-00007980: 2e63 6f6d 7069 6c65 2864 6576 6963 655f  .compile(device_
-00007990: 6164 6170 7465 722c 2072 652e 4947 4e4f  adapter, re.IGNO
-000079a0: 5245 4341 5345 290d 0a20 2020 2020 2020  RECASE)..       
-000079b0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000079c0: 2020 2020 2020 2020 2020 2020 7074 726e              ptrn
-000079d0: 203d 2064 6576 6963 655f 6164 6170 7465   = device_adapte
-000079e0: 720d 0a20 2020 2020 2020 2020 2020 2064  r..            d
-000079f0: 6576 6963 6573 203d 205b 6420 666f 7220  evices = [d for 
-00007a00: 6420 696e 2064 6576 6963 6573 2069 6620  d in devices if 
-00007a10: 7074 726e 2e73 6561 7263 6828 7365 6c66  ptrn.search(self
-00007a20: 2e67 6574 4465 7669 6365 4c69 6272 6172  .getDeviceLibrar
-00007a30: 7928 6429 295d 0d0a 0d0a 2020 2020 2020  y(d))]....      
-00007a40: 2020 666f 7220 6465 7620 696e 2064 6576    for dev in dev
-00007a50: 6963 6573 3a0d 0a20 2020 2020 2020 2020  ices:..         
-00007a60: 2020 2079 6965 6c64 2044 6576 6963 6528     yield Device(
-00007a70: 6465 762c 206d 6d63 6f72 653d 7365 6c66  dev, mmcore=self
-00007a80: 2920 6966 2061 735f 6f62 6a65 6374 2065  ) if as_object e
-00007a90: 6c73 6520 6465 760d 0a0d 0a20 2020 2040  lse dev....    @
-00007aa0: 6f76 6572 6c6f 6164 0d0a 2020 2020 6465  overload..    de
-00007ab0: 6620 6974 6572 5072 6f70 6572 7469 6573  f iterProperties
-00007ac0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-00007ad0: 0d0a 2020 2020 2020 2020 7072 6f70 6572  ..        proper
-00007ae0: 7479 5f74 7970 653a 2069 6e74 207c 2049  ty_type: int | I
-00007af0: 7465 7261 626c 655b 696e 745d 207c 204e  terable[int] | N
-00007b00: 6f6e 6520 3d20 2e2e 2e2c 0d0a 2020 2020  one = ...,..    
-00007b10: 2020 2020 7072 6f70 6572 7479 5f6e 616d      property_nam
-00007b20: 655f 7061 7474 6572 6e3a 2073 7472 207c  e_pattern: str |
-00007b30: 2072 652e 5061 7474 6572 6e20 7c20 4e6f   re.Pattern | No
-00007b40: 6e65 203d 202e 2e2e 2c0d 0a20 2020 2020  ne = ...,..     
-00007b50: 2020 202a 2c0d 0a20 2020 2020 2020 2064     *,..        d
-00007b60: 6576 6963 655f 7479 7065 3a20 696e 7420  evice_type: int 
-00007b70: 7c20 4974 6572 6162 6c65 5b69 6e74 5d20  | Iterable[int] 
-00007b80: 7c20 4e6f 6e65 203d 202e 2e2e 2c0d 0a20  | None = ...,.. 
-00007b90: 2020 2020 2020 2064 6576 6963 655f 6c61         device_la
-00007ba0: 6265 6c3a 2073 7472 207c 2072 652e 5061  bel: str | re.Pa
-00007bb0: 7474 6572 6e20 7c20 4e6f 6e65 203d 202e  ttern | None = .
-00007bc0: 2e2e 2c0d 0a20 2020 2020 2020 2068 6173  ..,..        has
-00007bd0: 5f6c 696d 6974 733a 2062 6f6f 6c20 7c20  _limits: bool | 
-00007be0: 4e6f 6e65 203d 204e 6f6e 652c 0d0a 2020  None = None,..  
-00007bf0: 2020 2020 2020 6973 5f72 6561 645f 6f6e        is_read_on
-00007c00: 6c79 3a20 626f 6f6c 207c 204e 6f6e 6520  ly: bool | None 
-00007c10: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-00007c20: 2069 735f 7365 7175 656e 6365 6162 6c65   is_sequenceable
-00007c30: 3a20 626f 6f6c 207c 204e 6f6e 6520 3d20  : bool | None = 
-00007c40: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2061  None,..        a
-00007c50: 735f 6f62 6a65 6374 3a20 4c69 7465 7261  s_object: Litera
-00007c60: 6c5b 4661 6c73 655d 2c0d 0a20 2020 2029  l[False],..    )
-00007c70: 202d 3e20 4974 6572 6174 6f72 5b74 7570   -> Iterator[tup
-00007c80: 6c65 5b73 7472 2c20 7374 725d 5d3a 0d0a  le[str, str]]:..
-00007c90: 2020 2020 2020 2020 2e2e 2e0d 0a0d 0a20          ....... 
-00007ca0: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
-00007cb0: 2020 6465 6620 6974 6572 5072 6f70 6572    def iterProper
-00007cc0: 7469 6573 280d 0a20 2020 2020 2020 2073  ties(..        s
-00007cd0: 656c 662c 0d0a 2020 2020 2020 2020 7072  elf,..        pr
-00007ce0: 6f70 6572 7479 5f74 7970 653a 2069 6e74  operty_type: int
-00007cf0: 207c 2049 7465 7261 626c 655b 696e 745d   | Iterable[int]
-00007d00: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0d0a   | None = ...,..
-00007d10: 2020 2020 2020 2020 7072 6f70 6572 7479          property
-00007d20: 5f6e 616d 655f 7061 7474 6572 6e3a 2073  _name_pattern: s
-00007d30: 7472 207c 2072 652e 5061 7474 6572 6e20  tr | re.Pattern 
-00007d40: 7c20 4e6f 6e65 203d 202e 2e2e 2c0d 0a20  | None = ...,.. 
-00007d50: 2020 2020 2020 202a 2c0d 0a20 2020 2020         *,..     
-00007d60: 2020 2064 6576 6963 655f 7479 7065 3a20     device_type: 
-00007d70: 696e 7420 7c20 4974 6572 6162 6c65 5b69  int | Iterable[i
-00007d80: 6e74 5d20 7c20 4e6f 6e65 203d 202e 2e2e  nt] | None = ...
-00007d90: 2c0d 0a20 2020 2020 2020 2064 6576 6963  ,..        devic
-00007da0: 655f 6c61 6265 6c3a 2073 7472 207c 2072  e_label: str | r
-00007db0: 652e 5061 7474 6572 6e20 7c20 4e6f 6e65  e.Pattern | None
-00007dc0: 203d 202e 2e2e 2c0d 0a20 2020 2020 2020   = ...,..       
-00007dd0: 2068 6173 5f6c 696d 6974 733a 2062 6f6f   has_limits: boo
-00007de0: 6c20 7c20 4e6f 6e65 203d 204e 6f6e 652c  l | None = None,
-00007df0: 0d0a 2020 2020 2020 2020 6973 5f72 6561  ..        is_rea
-00007e00: 645f 6f6e 6c79 3a20 626f 6f6c 207c 204e  d_only: bool | N
-00007e10: 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20 2020  one = None,..   
-00007e20: 2020 2020 2069 735f 7365 7175 656e 6365       is_sequence
-00007e30: 6162 6c65 3a20 626f 6f6c 207c 204e 6f6e  able: bool | Non
-00007e40: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
-00007e50: 2020 2061 735f 6f62 6a65 6374 3a20 4c69     as_object: Li
-00007e60: 7465 7261 6c5b 5472 7565 5d20 3d20 2e2e  teral[True] = ..
-00007e70: 2e2c 0d0a 2020 2020 2920 2d3e 2049 7465  .,..    ) -> Ite
-00007e80: 7261 746f 725b 4465 7669 6365 5072 6f70  rator[DeviceProp
-00007e90: 6572 7479 5d3a 0d0a 2020 2020 2020 2020  erty]:..        
-00007ea0: 2e2e 2e0d 0a0d 0a20 2020 2064 6566 2069  .......    def i
-00007eb0: 7465 7250 726f 7065 7274 6965 7328 0d0a  terProperties(..
-00007ec0: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00007ed0: 2020 2020 2020 2070 726f 7065 7274 795f         property_
-00007ee0: 7479 7065 3a20 696e 7420 7c20 4974 6572  type: int | Iter
-00007ef0: 6162 6c65 5b69 6e74 5d20 7c20 4e6f 6e65  able[int] | None
-00007f00: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00007f10: 2020 7072 6f70 6572 7479 5f6e 616d 655f    property_name_
-00007f20: 7061 7474 6572 6e3a 2073 7472 207c 2072  pattern: str | r
-00007f30: 652e 5061 7474 6572 6e20 7c20 4e6f 6e65  e.Pattern | None
-00007f40: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00007f50: 2020 2a2c 0d0a 2020 2020 2020 2020 6465    *,..        de
-00007f60: 7669 6365 5f74 7970 653a 2069 6e74 207c  vice_type: int |
-00007f70: 2049 7465 7261 626c 655b 696e 745d 207c   Iterable[int] |
-00007f80: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
-00007f90: 2020 2020 2020 2064 6576 6963 655f 6c61         device_la
-00007fa0: 6265 6c3a 2073 7472 207c 2072 652e 5061  bel: str | re.Pa
-00007fb0: 7474 6572 6e20 7c20 4e6f 6e65 203d 204e  ttern | None = N
-00007fc0: 6f6e 652c 0d0a 2020 2020 2020 2020 6861  one,..        ha
-00007fd0: 735f 6c69 6d69 7473 3a20 626f 6f6c 207c  s_limits: bool |
-00007fe0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
-00007ff0: 2020 2020 2020 2069 735f 7265 6164 5f6f         is_read_o
-00008000: 6e6c 793a 2062 6f6f 6c20 7c20 4e6f 6e65  nly: bool | None
-00008010: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00008020: 2020 6973 5f73 6571 7565 6e63 6561 626c    is_sequenceabl
-00008030: 653a 2062 6f6f 6c20 7c20 4e6f 6e65 203d  e: bool | None =
-00008040: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00008050: 6173 5f6f 626a 6563 743a 2062 6f6f 6c20  as_object: bool 
-00008060: 3d20 5472 7565 2c0d 0a20 2020 2029 202d  = True,..    ) -
-00008070: 3e20 4974 6572 6174 6f72 5b44 6576 6963  > Iterator[Devic
-00008080: 6550 726f 7065 7274 795d 207c 2049 7465  eProperty] | Ite
-00008090: 7261 746f 725b 7475 706c 655b 7374 722c  rator[tuple[str,
-000080a0: 2073 7472 5d5d 3a0d 0a20 2020 2020 2020   str]]:..       
-000080b0: 2022 2222 4974 6572 6174 6520 6f76 6572   """Iterate over
-000080c0: 2063 7572 7265 6e74 6c79 206c 6f61 6465   currently loade
-000080d0: 6420 2864 6576 6963 655f 6c61 6265 6c2c  d (device_label,
-000080e0: 2070 726f 7065 7274 795f 6e61 6d65 2920   property_name) 
-000080f0: 7061 6972 732e 0d0a 0d0a 2020 2020 2020  pairs.....      
-00008100: 2020 3a73 7061 726b 6c65 733a 202a 5468    :sparkles: *Th
-00008110: 6973 206d 6574 686f 6420 6973 206e 6577  is method is new
-00008120: 2069 6e20 6043 4d4d 436f 7265 506c 7573   in `CMMCorePlus
-00008130: 602e 2a0d 0a0d 0a20 2020 2020 2020 2049  `.*....        I
-00008140: 7420 6f66 6665 7273 2061 2063 6f6e 7665  t offers a conve
-00008150: 6e69 656e 7420 7761 7920 746f 2069 7465  nient way to ite
-00008160: 7261 7465 206f 7665 7220 6c6f 6164 6564  rate over loaded
-00008170: 2064 6576 6963 6573 2c20 6f70 7469 6f6e   devices, option
-00008180: 616c 6c79 2066 696c 7465 7269 6e67 0d0a  ally filtering..
-00008190: 2020 2020 2020 2020 6279 205b 6044 6576          by [`Dev
-000081a0: 6963 6554 7970 6560 5d5b 7079 6d6d 636f  iceType`][pymmco
-000081b0: 7265 5f70 6c75 732e 4465 7669 6365 5479  re_plus.DeviceTy
-000081c0: 7065 5d20 616e 642f 6f72 2064 6576 6963  pe] and/or devic
-000081d0: 6520 6c61 6265 6c2e 2049 7420 6361 6e20  e label. It can 
-000081e0: 616c 736f 0d0a 2020 2020 2020 2020 7969  also..        yi
-000081f0: 656c 6473 205b 6044 6576 6963 6550 726f  elds [`DevicePro
-00008200: 7065 7274 7960 5d5b 7079 6d6d 636f 7265  perty`][pymmcore
-00008210: 5f70 6c75 732e 4465 7669 6365 5072 6f70  _plus.DeviceProp
-00008220: 6572 7479 5d20 6f62 6a65 6374 7320 6966  erty] objects if
-00008230: 0d0a 2020 2020 2020 2020 6061 735f 6f62  ..        `as_ob
-00008240: 6a65 6374 6020 6973 2060 5472 7565 6020  ject` is `True` 
-00008250: 2874 6865 2064 6566 6175 6c74 292e 0d0a  (the default)...
-00008260: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00008270: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00008280: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00008290: 2020 7072 6f70 6572 7479 5f74 7970 6520    property_type 
-000082a0: 3a20 696e 7420 7c20 5365 7175 656e 6365  : int | Sequence
-000082b0: 5b69 6e74 5d20 7c20 4e6f 6e65 0d0a 2020  [int] | None..  
-000082c0: 2020 2020 2020 2020 2020 5072 6f70 6572            Proper
-000082d0: 7479 5479 7065 2028 6f72 2074 7970 6573  tyType (or types
-000082e0: 2920 746f 2066 696c 7465 7220 6279 2c20  ) to filter by, 
-000082f0: 6279 2064 6566 6175 6c74 2061 6c6c 2070  by default all p
-00008300: 726f 7065 7274 7920 7479 7065 7320 7769  roperty types wi
-00008310: 6c6c 0d0a 2020 2020 2020 2020 2020 2020  ll..            
-00008320: 6265 2079 6965 6c64 6564 2e0d 0a20 2020  be yielded...   
-00008330: 2020 2020 2070 726f 7065 7274 795f 6e61       property_na
-00008340: 6d65 5f70 6174 7465 726e 203a 2073 7472  me_pattern : str
-00008350: 207c 2072 652e 5061 7474 6572 6e20 7c20   | re.Pattern | 
-00008360: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
-00008370: 2020 5072 6f70 6572 7479 206e 616d 6520    Property name 
-00008380: 746f 2066 696c 7465 7220 6279 2c20 6279  to filter by, by
-00008390: 2064 6566 6175 6c74 2061 6c6c 2070 726f   default all pro
-000083a0: 7065 7274 7920 6e61 6d65 7320 7769 6c6c  perty names will
-000083b0: 2062 6520 7969 656c 6465 642e 0d0a 2020   be yielded...  
-000083c0: 2020 2020 2020 2020 2020 4d61 7920 6265            May be
-000083d0: 2061 2063 6f6d 7069 6c65 6420 7265 6775   a compiled regu
-000083e0: 6c61 7220 6578 7072 6573 7369 6f6e 206f  lar expression o
-000083f0: 7220 6120 7374 7269 6e67 2c20 696e 2077  r a string, in w
-00008400: 6869 6368 2063 6173 6520 6974 2077 696c  hich case it wil
-00008410: 6c20 6265 0d0a 2020 2020 2020 2020 2020  l be..          
-00008420: 2020 636f 6d70 696c 6564 2077 6974 6820    compiled with 
-00008430: 6072 652e 4947 4e4f 5245 4341 5345 602e  `re.IGNORECASE`.
-00008440: 0d0a 2020 2020 2020 2020 6465 7669 6365  ..        device
-00008450: 5f74 7970 6520 3a20 4465 7669 6365 5479  _type : DeviceTy
-00008460: 7065 207c 204e 6f6e 650d 0a20 2020 2020  pe | None..     
-00008470: 2020 2020 2020 2044 6576 6963 6554 7970         DeviceTyp
-00008480: 6520 746f 2066 696c 7465 7220 6279 2c20  e to filter by, 
-00008490: 6279 2064 6566 6175 6c74 2061 6c6c 2064  by default all d
-000084a0: 6576 6963 6520 7479 7065 7320 7769 6c6c  evice types will
-000084b0: 2062 6520 7969 656c 6465 642e 0d0a 2020   be yielded...  
-000084c0: 2020 2020 2020 6465 7669 6365 5f6c 6162        device_lab
-000084d0: 656c 203a 2073 7472 207c 204e 6f6e 650d  el : str | None.
-000084e0: 0a20 2020 2020 2020 2020 2020 2044 6576  .            Dev
-000084f0: 6963 6520 6c61 6265 6c20 746f 2066 696c  ice label to fil
-00008500: 7465 7220 6279 2c20 6279 2064 6566 6175  ter by, by defau
-00008510: 6c74 2061 6c6c 2064 6576 6963 6520 6c61  lt all device la
-00008520: 6265 6c73 2077 696c 6c20 6265 2079 6965  bels will be yie
-00008530: 6c64 6564 2e0d 0a20 2020 2020 2020 2068  lded...        h
-00008540: 6173 5f6c 696d 6974 7320 3a20 626f 6f6c  as_limits : bool
-00008550: 207c 204e 6f6e 650d 0a20 2020 2020 2020   | None..       
-00008560: 2020 2020 2049 6620 7072 6f76 6964 6564       If provided
-00008570: 2c20 6f6e 6c79 2070 726f 7065 7274 6965  , only propertie
-00008580: 7320 7769 7468 2060 6861 7350 726f 7065  s with `hasPrope
-00008590: 7274 794c 696d 6974 7360 206d 6174 6368  rtyLimits` match
-000085a0: 696e 6720 7468 6973 2076 616c 7565 0d0a  ing this value..
-000085b0: 2020 2020 2020 2020 2020 2020 7769 6c6c              will
-000085c0: 2062 6520 7969 656c 6465 642e 0d0a 2020   be yielded...  
-000085d0: 2020 2020 2020 6973 5f72 6561 645f 6f6e        is_read_on
-000085e0: 6c79 203a 2062 6f6f 6c20 7c20 4e6f 6e65  ly : bool | None
-000085f0: 0d0a 2020 2020 2020 2020 2020 2020 4966  ..            If
-00008600: 2070 726f 7669 6465 642c 206f 6e6c 7920   provided, only 
-00008610: 7072 6f70 6572 7469 6573 2077 6974 6820  properties with 
-00008620: 6069 7350 726f 7065 7274 7952 6561 644f  `isPropertyReadO
-00008630: 6e6c 7960 206d 6174 6368 696e 6720 7468  nly` matching th
-00008640: 6973 2076 616c 7565 0d0a 2020 2020 2020  is value..      
-00008650: 2020 2020 2020 7769 6c6c 2062 6520 7969        will be yi
-00008660: 656c 6465 642e 0d0a 2020 2020 2020 2020  elded...        
-00008670: 6973 5f73 6571 7565 6e63 6561 626c 6520  is_sequenceable 
-00008680: 3a20 626f 6f6c 207c 204e 6f6e 650d 0a20  : bool | None.. 
-00008690: 2020 2020 2020 2020 2020 2049 6620 7072             If pr
-000086a0: 6f76 6964 6564 206f 6e6c 7920 7072 6f70  ovided only prop
-000086b0: 6572 7469 6573 2077 6974 6820 6069 7350  erties with `isP
-000086c0: 726f 7065 7274 7953 6571 7565 6e63 6561  ropertySequencea
-000086d0: 626c 6560 206d 6174 6368 696e 6720 7468  ble` matching th
-000086e0: 6973 0d0a 2020 2020 2020 2020 2020 2020  is..            
-000086f0: 7661 6c75 6520 7769 6c6c 2062 6520 7969  value will be yi
-00008700: 656c 6465 642e 0d0a 2020 2020 2020 2020  elded...        
-00008710: 6173 5f6f 626a 6563 7420 3a20 626f 6f6c  as_object : bool
-00008720: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00008730: 2020 2020 2020 2020 4966 2060 5472 7565          If `True
-00008740: 602c 2060 4465 7669 6365 5072 6f70 6572  `, `DeviceProper
-00008750: 7479 6020 6f62 6a65 6374 7320 7769 6c6c  ty` objects will
-00008760: 2062 6520 7969 656c 6465 6420 696e 7374   be yielded inst
-00008770: 6561 6420 6f66 0d0a 2020 2020 2020 2020  ead of..        
-00008780: 2020 2020 6028 6465 7669 6365 5f6c 6162      `(device_lab
-00008790: 656c 2c20 7072 6f70 6572 7479 5f6e 616d  el, property_nam
-000087a0: 6529 6020 7475 706c 6573 2e20 4279 2064  e)` tuples. By d
-000087b0: 6566 6175 6c74 2054 7275 650d 0a0d 0a20  efault True.... 
-000087c0: 2020 2020 2020 2059 6965 6c64 730d 0a20         Yields.. 
-000087d0: 2020 2020 2020 202d 2d2d 2d2d 2d0d 0a20         ------.. 
-000087e0: 2020 2020 2020 2044 6576 6963 6550 726f         DevicePro
-000087f0: 7065 7274 7920 7c20 7475 706c 655b 7374  perty | tuple[st
-00008800: 722c 2073 7472 5d0d 0a20 2020 2020 2020  r, str]..       
-00008810: 2020 2020 2060 4465 7669 6365 5072 6f70       `DeviceProp
-00008820: 6572 7479 6020 6f62 6a65 6374 7320 2869  erty` objects (i
-00008830: 6620 6061 735f 6f62 6a65 6374 3d3d 5472  f `as_object==Tr
-00008840: 7565 6029 206f 7220 322d 7475 706c 6573  ue`) or 2-tuples
-00008850: 206f 6620 2864 6576 6963 655f 6e61 6d65   of (device_name
-00008860: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
-00008870: 726f 7065 7274 795f 6e61 6d65 290d 0a20  roperty_name).. 
-00008880: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00008890: 2020 2020 6966 2070 726f 7065 7274 795f      if property_
-000088a0: 6e61 6d65 5f70 6174 7465 726e 3a0d 0a20  name_pattern:.. 
-000088b0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000088c0: 696e 7374 616e 6365 2870 726f 7065 7274  instance(propert
-000088d0: 795f 6e61 6d65 5f70 6174 7465 726e 2c20  y_name_pattern, 
-000088e0: 7374 7229 3a0d 0a20 2020 2020 2020 2020  str):..         
-000088f0: 2020 2020 2020 2070 7472 6e20 3d20 7265         ptrn = re
-00008900: 2e63 6f6d 7069 6c65 2870 726f 7065 7274  .compile(propert
-00008910: 795f 6e61 6d65 5f70 6174 7465 726e 2c20  y_name_pattern, 
-00008920: 7265 2e49 474e 4f52 4543 4153 4529 0d0a  re.IGNORECASE)..
-00008930: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00008940: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00008950: 2020 2070 7472 6e20 3d20 7072 6f70 6572     ptrn = proper
-00008960: 7479 5f6e 616d 655f 7061 7474 6572 6e0d  ty_name_pattern.
-00008970: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00008980: 2020 2020 2020 2020 2020 2020 7074 726e              ptrn
-00008990: 203d 204e 6f6e 650d 0a0d 0a20 2020 2020   = None....     
-000089a0: 2020 2069 6620 7072 6f70 6572 7479 5f74     if property_t
-000089b0: 7970 6520 6973 204e 6f6e 653a 0d0a 2020  ype is None:..  
-000089c0: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
-000089d0: 7479 5f74 7970 6573 203d 2073 6574 2829  ty_types = set()
-000089e0: 0d0a 2020 2020 2020 2020 656c 6966 2069  ..        elif i
-000089f0: 7369 6e73 7461 6e63 6528 7072 6f70 6572  sinstance(proper
-00008a00: 7479 5f74 7970 652c 2069 6e74 293a 0d0a  ty_type, int):..
-00008a10: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
-00008a20: 6572 7479 5f74 7970 6573 203d 207b 7072  erty_types = {pr
-00008a30: 6f70 6572 7479 5f74 7970 657d 0d0a 2020  operty_type}..  
-00008a40: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00008a50: 2020 2020 2020 2020 2070 726f 7065 7274           propert
-00008a60: 795f 7479 7065 7320 3d20 7365 7428 7072  y_types = set(pr
-00008a70: 6f70 6572 7479 5f74 7970 6529 0d0a 0d0a  operty_type)....
-00008a80: 2020 2020 2020 2020 666f 7220 6465 7620          for dev 
-00008a90: 696e 2073 656c 662e 6974 6572 4465 7669  in self.iterDevi
-00008aa0: 6365 7328 6465 7669 6365 5f74 7970 652c  ces(device_type,
-00008ab0: 2064 6576 6963 655f 6c61 6265 6c2c 2061   device_label, a
-00008ac0: 735f 6f62 6a65 6374 3d46 616c 7365 293a  s_object=False):
-00008ad0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00008ae0: 7220 7072 6f70 2069 6e20 7365 6c66 2e67  r prop in self.g
-00008af0: 6574 4465 7669 6365 5072 6f70 6572 7479  etDeviceProperty
-00008b00: 4e61 6d65 7328 6465 7629 3a0d 0a20 2020  Names(dev):..   
-00008b10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00008b20: 7074 726e 2061 6e64 206e 6f74 2070 7472  ptrn and not ptr
-00008b30: 6e2e 7365 6172 6368 2870 726f 7029 3a0d  n.search(prop):.
-00008b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b50: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00008b60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008b70: 6620 280d 0a20 2020 2020 2020 2020 2020  f (..           
-00008b80: 2020 2020 2020 2020 2070 726f 7065 7274           propert
-00008b90: 795f 7479 7065 2069 7320 6e6f 7420 4e6f  y_type is not No
-00008ba0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00008bb0: 2020 2020 2020 2020 616e 6420 7375 7065          and supe
-00008bc0: 7228 292e 6765 7450 726f 7065 7274 7954  r().getPropertyT
-00008bd0: 7970 6528 6465 762c 2070 726f 7029 206e  ype(dev, prop) n
-00008be0: 6f74 2069 6e20 7072 6f70 6572 7479 5f74  ot in property_t
-00008bf0: 7970 6573 0d0a 2020 2020 2020 2020 2020  ypes..          
-00008c00: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
-00008c10: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00008c20: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00008c30: 2020 2020 2020 2020 6966 2028 0d0a 2020          if (..  
-00008c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c50: 2020 6861 735f 6c69 6d69 7473 2069 7320    has_limits is 
-00008c60: 6e6f 7420 4e6f 6e65 0d0a 2020 2020 2020  not None..      
-00008c70: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00008c80: 6420 7365 6c66 2e68 6173 5072 6f70 6572  d self.hasProper
-00008c90: 7479 4c69 6d69 7473 2864 6576 2c20 7072  tyLimits(dev, pr
-00008ca0: 6f70 2920 213d 2068 6173 5f6c 696d 6974  op) != has_limit
-00008cb0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00008cc0: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00008cd0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00008ce0: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
-00008cf0: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-00008d00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008d10: 735f 7265 6164 5f6f 6e6c 7920 6973 206e  s_read_only is n
-00008d20: 6f74 204e 6f6e 650d 0a20 2020 2020 2020  ot None..       
-00008d30: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00008d40: 2073 656c 662e 6973 5072 6f70 6572 7479   self.isProperty
-00008d50: 5265 6164 4f6e 6c79 2864 6576 2c20 7072  ReadOnly(dev, pr
-00008d60: 6f70 2920 213d 2069 735f 7265 6164 5f6f  op) != is_read_o
-00008d70: 6e6c 790d 0a20 2020 2020 2020 2020 2020  nly..           
-00008d80: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-00008d90: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00008da0: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
-00008db0: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dd0: 2069 735f 7365 7175 656e 6365 6162 6c65   is_sequenceable
-00008de0: 2069 7320 6e6f 7420 4e6f 6e65 0d0a 2020   is not None..  
-00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e00: 2020 616e 6420 7365 6c66 2e69 7350 726f    and self.isPro
-00008e10: 7065 7274 7953 6571 7565 6e63 6561 626c  pertySequenceabl
-00008e20: 6528 6465 762c 2070 726f 7029 2021 3d20  e(dev, prop) != 
-00008e30: 6973 5f73 6571 7565 6e63 6561 626c 650d  is_sequenceable.
-00008e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008e50: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-00008e60: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00008e70: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00008e80: 2020 2020 2079 6965 6c64 2044 6576 6963       yield Devic
-00008e90: 6550 726f 7065 7274 7928 6465 762c 2070  eProperty(dev, p
-00008ea0: 726f 702c 2073 656c 6629 2069 6620 6173  rop, self) if as
-00008eb0: 5f6f 626a 6563 7420 656c 7365 2028 6465  _object else (de
-00008ec0: 762c 2070 726f 7029 0d0a 0d0a 2020 2020  v, prop)....    
-00008ed0: 6465 6620 6765 7450 726f 7065 7274 794f  def getPropertyO
-00008ee0: 626a 6563 7428 0d0a 2020 2020 2020 2020  bject(..        
-00008ef0: 7365 6c66 2c20 6465 7669 6365 5f6c 6162  self, device_lab
-00008f00: 656c 3a20 7374 722c 2070 726f 7065 7274  el: str, propert
-00008f10: 795f 6e61 6d65 3a20 7374 720d 0a20 2020  y_name: str..   
-00008f20: 2029 202d 3e20 4465 7669 6365 5072 6f70   ) -> DeviceProp
-00008f30: 6572 7479 3a0d 0a20 2020 2020 2020 2022  erty:..        "
-00008f40: 2222 5265 7475 726e 2061 2044 6576 6963  ""Return a Devic
-00008f50: 6550 726f 7065 7274 7920 6f62 6a65 6374  eProperty object
-00008f60: 2062 6f75 6e64 2074 6f20 6120 6465 7669   bound to a devi
-00008f70: 6365 2f70 726f 7065 7274 7920 6f6e 2074  ce/property on t
-00008f80: 6869 7320 636f 7265 2e0d 0a0d 0a20 2020  his core.....   
-00008f90: 2020 2020 203a 7370 6172 6b6c 6573 3a20       :sparkles: 
-00008fa0: 2a54 6869 7320 6d65 7468 6f64 2069 7320  *This method is 
-00008fb0: 6e65 7720 696e 2060 434d 4d43 6f72 6550  new in `CMMCoreP
-00008fc0: 6c75 7360 2e2a 0d0a 0d0a 2020 2020 2020  lus`.*....      
-00008fd0: 2020 5b60 4465 7669 6365 5072 6f70 6572    [`DeviceProper
-00008fe0: 7479 605d 5b70 796d 6d63 6f72 655f 706c  ty`][pymmcore_pl
-00008ff0: 7573 2e44 6576 6963 6550 726f 7065 7274  us.DevicePropert
-00009000: 795d 206f 626a 6563 7473 2061 7265 2061  y] objects are a
-00009010: 2063 6f6e 7665 6e69 656e 7420 6f62 6a65   convenient obje
-00009020: 6374 0d0a 2020 2020 2020 2020 6f72 6965  ct..        orie
-00009030: 6e74 6564 2077 6179 2074 6f20 696e 7465  nted way to inte
-00009040: 7261 6374 2077 6974 6820 6120 7370 6563  ract with a spec
-00009050: 6966 6963 2064 6576 6963 6520 7072 6f70  ific device prop
-00009060: 6572 7469 6573 2e20 5468 6579 2061 6c6c  erties. They all
-00009070: 6f77 2079 6f75 2074 6f0d 0a20 2020 2020  ow you to..     
-00009080: 2020 2063 616c 6c20 616e 7920 6d65 7468     call any meth
-00009090: 6f64 206f 6e20 6043 4d4d 436f 7265 6020  od on `CMMCore` 
-000090a0: 7468 6174 206e 6f72 6d61 6c6c 7920 7265  that normally re
-000090b0: 7175 6972 6573 2061 2060 6465 7669 6365  quires a `device
-000090c0: 4c61 6265 6c60 2061 6e64 0d0a 2020 2020  Label` and..    
-000090d0: 2020 2020 6070 726f 7065 7274 794e 616d      `propertyNam
-000090e0: 6560 2061 7320 7468 6520 6669 7273 7420  e` as the first 
-000090f0: 7477 6f20 6172 6775 6d65 6e74 7320 6173  two arguments as
-00009100: 2061 6e20 6172 6775 6d65 6e74 2d66 7265   an argument-fre
-00009110: 6520 6d65 7468 6f64 206f 6e20 7468 650d  e method on the.
-00009120: 0a20 2020 2020 2020 2060 4465 7669 6365  .        `Device
-00009130: 5072 6f70 6572 7479 6020 6f62 6a65 6374  Property` object
-00009140: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00009150: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-00009160: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-00009170: 2020 2020 2064 6576 6963 655f 6c61 6265       device_labe
-00009180: 6c20 3a20 7374 720d 0a20 2020 2020 2020  l : str..       
-00009190: 2020 2020 2044 6576 6963 6520 6c61 6265       Device labe
-000091a0: 6c20 746f 2067 6574 2061 2070 726f 7065  l to get a prope
-000091b0: 7274 7920 6f62 6a65 6374 2066 6f72 2e0d  rty object for..
-000091c0: 0a20 2020 2020 2020 2070 726f 7065 7274  .        propert
-000091d0: 795f 6e61 6d65 203a 2073 7472 0d0a 2020  y_name : str..  
-000091e0: 2020 2020 2020 2020 2020 5072 6f70 6572            Proper
-000091f0: 7479 206e 616d 6520 746f 2067 6574 2061  ty name to get a
-00009200: 2070 726f 7065 7274 7920 6f62 6a65 6374   property object
-00009210: 2066 6f72 2e0d 0a0d 0a20 2020 2020 2020   for.....       
-00009220: 2045 7861 6d70 6c65 730d 0a20 2020 2020   Examples..     
-00009230: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-00009240: 2020 2020 203e 3e3e 2063 6f72 6520 3d20       >>> core = 
-00009250: 434d 4d43 6f72 6550 6c75 7328 290d 0a20  CMMCorePlus().. 
-00009260: 2020 2020 2020 203e 3e3e 2063 6f72 652e         >>> core.
-00009270: 6c6f 6164 4465 7669 6365 2822 4465 6d6f  loadDevice("Demo
-00009280: 4361 6d65 7261 222c 2022 4465 6d6f 4361  Camera", "DemoCa
-00009290: 6d65 7261 222c 2022 4443 616d 2229 0d0a  mera", "DCam")..
-000092a0: 2020 2020 2020 2020 3e3e 3e20 636f 7265          >>> core
-000092b0: 2e69 6e69 7469 616c 697a 6544 6576 6963  .initializeDevic
-000092c0: 6528 2244 656d 6f43 616d 6572 6122 290d  e("DemoCamera").
-000092d0: 0a20 2020 2020 2020 203e 3e3e 2063 6f72  .        >>> cor
-000092e0: 652e 7365 7443 616d 6572 6144 6576 6963  e.setCameraDevic
-000092f0: 6528 2244 656d 6f43 616d 6572 6122 290d  e("DemoCamera").
-00009300: 0a20 2020 2020 2020 203e 3e3e 2065 7870  .        >>> exp
-00009310: 6f73 7572 6520 3d20 636f 7265 2e67 6574  osure = core.get
-00009320: 5072 6f70 6572 7479 4f62 6a65 6374 2822  PropertyObject("
-00009330: 4465 6d6f 4361 6d65 7261 222c 2022 4578  DemoCamera", "Ex
-00009340: 706f 7375 7265 2229 0d0a 2020 2020 2020  posure")..      
-00009350: 2020 3e3e 3e20 6578 706f 7375 7265 2e74    >>> exposure.t
-00009360: 7970 6528 290d 0a20 2020 2020 2020 203c  ype()..        <
-00009370: 5072 6f70 6572 7479 5479 7065 2e46 6c6f  PropertyType.Flo
-00009380: 6174 3a20 323e 0d0a 2020 2020 2020 2020  at: 2>..        
-00009390: 3e3e 3e20 6578 706f 7375 7265 2e75 7070  >>> exposure.upp
-000093a0: 6572 4c69 6d69 7428 290d 0a20 2020 2020  erLimit()..     
-000093b0: 2020 2031 3030 3030 2e30 0d0a 0d0a 2020     10000.0....  
-000093c0: 2020 2020 2020 6765 742f 7365 7420 7072        get/set pr
-000093d0: 6f70 6572 7920 7661 6c75 6573 2065 6173  opery values eas
-000093e0: 696c 793a 0d0a 0d0a 2020 2020 2020 2020  ily:....        
-000093f0: 3e3e 3e20 6578 706f 7375 7265 2e76 616c  >>> exposure.val
-00009400: 7565 0d0a 2020 2020 2020 2020 3130 2e30  ue..        10.0
-00009410: 0d0a 2020 2020 2020 2020 3e3e 3e20 6578  ..        >>> ex
-00009420: 706f 7375 7265 2e76 616c 7565 203d 2035  posure.value = 5
-00009430: 2e30 0d0a 2020 2020 2020 2020 3e3e 3e20  .0..        >>> 
-00009440: 6578 706f 7375 7265 2e76 616c 7565 0d0a  exposure.value..
-00009450: 2020 2020 2020 2020 352e 300d 0a20 2020          5.0..   
-00009460: 2020 2020 203e 3e3e 2063 6f72 652e 6765       >>> core.ge
-00009470: 7445 7870 6f73 7572 6528 2920 2023 2063  tExposure()  # c
-00009480: 6861 6e67 6573 2072 6566 6c65 6374 6564  hanges reflected
-00009490: 2069 6e20 636f 7265 0d0a 2020 2020 2020   in core..      
-000094a0: 2020 352e 300d 0a20 2020 2020 2020 2022    5.0..        "
-000094b0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-000094c0: 726e 2044 6576 6963 6550 726f 7065 7274  rn DevicePropert
-000094d0: 7928 6465 7669 6365 5f6c 6162 656c 2c20  y(device_label, 
-000094e0: 7072 6f70 6572 7479 5f6e 616d 652c 2073  property_name, s
-000094f0: 656c 6629 0d0a 0d0a 2020 2020 6465 6620  elf)....    def 
-00009500: 6765 7441 6461 7074 6572 4f62 6a65 6374  getAdapterObject
-00009510: 2873 656c 662c 206c 6962 7261 7279 5f6e  (self, library_n
-00009520: 616d 653a 2073 7472 2920 2d3e 2044 6576  ame: str) -> Dev
-00009530: 6963 6541 6461 7074 6572 3a0d 0a20 2020  iceAdapter:..   
-00009540: 2020 2020 2022 2222 5265 7475 726e 2061       """Return a
-00009550: 6e20 6041 6461 7074 6572 6020 6f62 6a65  n `Adapter` obje
-00009560: 6374 2062 6f75 6e64 2074 6f20 6c69 6272  ct bound to libr
-00009570: 6172 795f 6e61 6d65 206f 6e20 7468 6973  ary_name on this
-00009580: 2063 6f72 652e 0d0a 0d0a 2020 2020 2020   core.....      
-00009590: 2020 3a73 7061 726b 6c65 733a 202a 5468    :sparkles: *Th
-000095a0: 6973 206d 6574 686f 6420 6973 206e 6577  is method is new
-000095b0: 2069 6e20 6043 4d4d 436f 7265 506c 7573   in `CMMCorePlus
-000095c0: 602e 2a0d 0a0d 0a20 2020 2020 2020 205b  `.*....        [
-000095d0: 6041 6461 7074 6572 605d 5b70 796d 6d63  `Adapter`][pymmc
-000095e0: 6f72 655f 706c 7573 2e44 6576 6963 6541  ore_plus.DeviceA
-000095f0: 6461 7074 6572 5d20 6f62 6a65 6374 7320  dapter] objects 
-00009600: 6172 6520 6120 636f 6e76 656e 6965 6e74  are a convenient
-00009610: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
-00009620: 206f 7269 656e 7465 6420 7761 7920 746f   oriented way to
-00009630: 2069 6e74 6572 6163 7420 7769 7468 2064   interact with d
-00009640: 6576 6963 6520 6164 6170 7465 7273 2e20  evice adapters. 
-00009650: 5468 6579 2061 6c6c 6f77 2079 6f75 2074  They allow you t
-00009660: 6f20 6361 6c6c 2061 6e79 206d 6574 686f  o call any metho
-00009670: 640d 0a20 2020 2020 2020 206f 6e20 6043  d..        on `C
-00009680: 4d4d 436f 7265 6020 7468 6174 206e 6f72  MMCore` that nor
-00009690: 6d61 6c6c 7920 7265 7175 6972 6573 2061  mally requires a
-000096a0: 2060 6c69 6272 6172 795f 6e61 6d65 6020   `library_name` 
-000096b0: 6173 2074 6865 2066 6972 7374 2061 7267  as the first arg
-000096c0: 756d 656e 7420 6173 2061 6e0d 0a20 2020  ument as an..   
-000096d0: 2020 2020 2061 7267 756d 656e 742d 6672       argument-fr
-000096e0: 6565 206d 6574 686f 6420 6f6e 2074 6865  ee method on the
-000096f0: 2060 4164 6170 7465 7260 206f 626a 6563   `Adapter` objec
-00009700: 742e 0d0a 2020 2020 2020 2020 2222 220d  t...        """.
-00009710: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009720: 4465 7669 6365 4164 6170 7465 7228 6c69  DeviceAdapter(li
-00009730: 6272 6172 795f 6e61 6d65 2c20 6d6d 636f  brary_name, mmco
-00009740: 7265 3d73 656c 6629 0d0a 0d0a 2020 2020  re=self)....    
-00009750: 6465 6620 6765 7444 6576 6963 654f 626a  def getDeviceObj
-00009760: 6563 7428 7365 6c66 2c20 6465 7669 6365  ect(self, device
-00009770: 5f6c 6162 656c 3a20 7374 7229 202d 3e20  _label: str) -> 
-00009780: 4465 7669 6365 3a0d 0a20 2020 2020 2020  Device:..       
-00009790: 2022 2222 5265 7475 726e 2061 2060 4465   """Return a `De
-000097a0: 7669 6365 6020 6f62 6a65 6374 2062 6f75  vice` object bou
-000097b0: 6e64 2074 6f20 6465 7669 6365 5f6c 6162  nd to device_lab
-000097c0: 656c 206f 6e20 7468 6973 2063 6f72 652e  el on this core.
-000097d0: 0d0a 0d0a 2020 2020 2020 2020 3a73 7061  ....        :spa
-000097e0: 726b 6c65 733a 202a 5468 6973 206d 6574  rkles: *This met
-000097f0: 686f 6420 6973 206e 6577 2069 6e20 6043  hod is new in `C
-00009800: 4d4d 436f 7265 506c 7573 602e 2a0d 0a0d  MMCorePlus`.*...
-00009810: 0a20 2020 2020 2020 205b 6044 6576 6963  .        [`Devic
-00009820: 6560 5d5b 7079 6d6d 636f 7265 5f70 6c75  e`][pymmcore_plu
-00009830: 732e 4465 7669 6365 5d20 6f62 6a65 6374  s.Device] object
-00009840: 7320 6172 6520 6120 636f 6e76 656e 6965  s are a convenie
-00009850: 6e74 206f 626a 6563 7420 6f72 6965 6e74  nt object orient
-00009860: 6564 2077 6179 2074 6f0d 0a20 2020 2020  ed way to..     
-00009870: 2020 2069 6e74 6572 6163 7420 7769 7468     interact with
-00009880: 2064 6576 6963 6573 2e20 5468 6579 2061   devices. They a
-00009890: 6c6c 6f77 2079 6f75 2074 6f20 6361 6c6c  llow you to call
-000098a0: 2061 6e79 206d 6574 686f 6420 6f6e 2060   any method on `
-000098b0: 434d 4d43 6f72 6560 2074 6861 740d 0a20  CMMCore` that.. 
-000098c0: 2020 2020 2020 206e 6f72 6d61 6c6c 7920         normally 
-000098d0: 7265 7175 6972 6573 2061 2060 6465 7669  requires a `devi
-000098e0: 6365 4c61 6265 6c60 2061 7320 7468 6520  ceLabel` as the 
-000098f0: 6669 7273 7420 6172 6775 6d65 6e74 2061  first argument a
-00009900: 7320 616e 2061 7267 756d 656e 742d 6672  s an argument-fr
-00009910: 6565 0d0a 2020 2020 2020 2020 6d65 7468  ee..        meth
-00009920: 6f64 206f 6e20 7468 6520 6044 6576 6963  od on the `Devic
-00009930: 6560 206f 626a 6563 742e 0d0a 0d0a 2020  e` object.....  
-00009940: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00009950: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00009960: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6465  ----..        de
-00009970: 7669 6365 5f6c 6162 656c 203a 2073 7472  vice_label : str
-00009980: 0d0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-00009990: 7669 6365 206c 6162 656c 2074 6f20 6765  vice label to ge
-000099a0: 7420 6120 6465 7669 6365 206f 626a 6563  t a device objec
-000099b0: 7420 666f 722e 0d0a 0d0a 2020 2020 2020  t for.....      
-000099c0: 2020 4578 616d 706c 6573 0d0a 2020 2020    Examples..    
-000099d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
-000099e0: 2020 2020 2020 3e3e 3e20 636f 7265 203d        >>> core =
-000099f0: 2043 4d4d 436f 7265 506c 7573 2829 0d0a   CMMCorePlus()..
-00009a00: 2020 2020 2020 2020 3e3e 3e20 6361 6d20          >>> cam 
-00009a10: 3d20 636f 7265 2e67 6574 4465 7669 6365  = core.getDevice
-00009a20: 4f62 6a65 6374 2822 4465 6d6f 4361 6d65  Object("DemoCame
-00009a30: 7261 2229 0d0a 2020 2020 2020 2020 3e3e  ra")..        >>
-00009a40: 3e20 6361 6d2e 6973 4c6f 6164 6564 2829  > cam.isLoaded()
-00009a50: 0d0a 2020 2020 2020 2020 4661 6c73 650d  ..        False.
-00009a60: 0a20 2020 2020 2020 203e 3e3e 2063 616d  .        >>> cam
-00009a70: 2e6c 6f61 6428 2244 656d 6f43 616d 6572  .load("DemoCamer
-00009a80: 6122 2c20 2244 4361 6d22 290d 0a20 2020  a", "DCam")..   
-00009a90: 2020 2020 203e 3e3e 2063 616d 2e69 734c       >>> cam.isL
-00009aa0: 6f61 6465 6428 290d 0a20 2020 2020 2020  oaded()..       
-00009ab0: 2054 7275 650d 0a20 2020 2020 2020 203e   True..        >
-00009ac0: 3e3e 2063 616d 2e69 6e69 7469 616c 697a  >> cam.initializ
-00009ad0: 6528 290d 0a0d 0a20 2020 2020 2020 2067  e()....        g
-00009ae0: 6574 2074 6865 2064 6576 6963 6520 7363  et the device sc
-00009af0: 6865 6d61 0d0a 0d0a 2020 2020 2020 2020  hema....        
-00009b00: 3e3e 3e20 6361 6d2e 7363 6865 6d61 2829  >>> cam.schema()
-00009b10: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00009b20: 2020 2020 2020 2020 2027 7469 746c 6527           'title'
-00009b30: 3a20 2744 4361 6d27 2c0d 0a20 2020 2020  : 'DCam',..     
-00009b40: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
-00009b50: 696f 6e27 3a20 2744 656d 6f20 6361 6d65  ion': 'Demo came
-00009b60: 7261 272c 0d0a 2020 2020 2020 2020 2020  ra',..          
-00009b70: 2020 2774 7970 6527 3a20 276f 626a 6563    'type': 'objec
-00009b80: 7427 2c0d 0a20 2020 2020 2020 2020 2020  t',..           
-00009b90: 2027 7072 6f70 6572 7469 6573 273a 207b   'properties': {
-00009ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009bb0: 2020 2748 7562 4944 273a 207b 2774 7970    'HubID': {'typ
-00009bc0: 6527 3a20 2773 7472 696e 6727 2c20 2772  e': 'string', 'r
-00009bd0: 6561 644f 6e6c 7927 3a20 5472 7565 2c20  eadOnly': True, 
-00009be0: 2764 6566 6175 6c74 273a 2027 277d 2c0d  'default': ''},.
-00009bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c00: 2027 4d61 7869 6d75 6d45 7870 6f73 7572   'MaximumExposur
-00009c10: 654d 7327 3a20 7b27 7479 7065 273a 2027  eMs': {'type': '
-00009c20: 6e75 6d62 6572 272c 2027 7072 6549 6e69  number', 'preIni
-00009c30: 7427 3a20 5472 7565 7d2c 0d0a 2020 2020  t': True},..    
-00009c40: 2020 2020 2020 2020 2020 2020 2754 7261              'Tra
-00009c50: 6e73 706f 7365 436f 7272 6563 7469 6f6e  nsposeCorrection
-00009c60: 273a 207b 2774 7970 6527 3a20 2762 6f6f  ': {'type': 'boo
-00009c70: 6c65 616e 277d 2c0d 0a20 2020 2020 2020  lean'},..       
-00009c80: 2020 2020 2020 2020 2027 5472 616e 7370           'Transp
-00009c90: 6f73 654d 6972 726f 7258 273a 207b 2774  oseMirrorX': {'t
-00009ca0: 7970 6527 3a20 2762 6f6f 6c65 616e 277d  ype': 'boolean'}
-00009cb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009cc0: 2020 2027 5472 616e 7370 6f73 654d 6972     'TransposeMir
-00009cd0: 726f 7259 273a 207b 2774 7970 6527 3a20  rorY': {'type': 
-00009ce0: 2762 6f6f 6c65 616e 277d 2c0d 0a20 2020  'boolean'},..   
-00009cf0: 2020 2020 2020 2020 2020 2020 2027 5472               'Tr
-00009d00: 616e 7370 6f73 6558 5927 3a20 7b27 7479  ansposeXY': {'ty
-00009d10: 7065 273a 2027 626f 6f6c 6561 6e27 7d0d  pe': 'boolean'}.
-00009d20: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-00009d30: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00009d40: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00009d50: 7265 7475 726e 2044 6576 6963 6528 6465  return Device(de
-00009d60: 7669 6365 5f6c 6162 656c 2c20 6d6d 636f  vice_label, mmco
-00009d70: 7265 3d73 656c 6629 0d0a 0d0a 2020 2020  re=self)....    
-00009d80: 6465 6620 6765 7443 6f6e 6669 6747 726f  def getConfigGro
-00009d90: 7570 4f62 6a65 6374 280d 0a20 2020 2020  upObject(..     
-00009da0: 2020 2073 656c 662c 2067 726f 7570 5f6e     self, group_n
-00009db0: 616d 653a 2073 7472 2c20 616c 6c6f 775f  ame: str, allow_
-00009dc0: 6d69 7373 696e 673a 2062 6f6f 6c20 3d20  missing: bool = 
-00009dd0: 4661 6c73 650d 0a20 2020 2029 202d 3e20  False..    ) -> 
-00009de0: 436f 6e66 6967 4772 6f75 703a 0d0a 2020  ConfigGroup:..  
-00009df0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00009e00: 6120 6043 6f6e 6669 6747 726f 7570 6020  a `ConfigGroup` 
-00009e10: 6f62 6a65 6374 2062 6f75 6e64 2074 6f20  object bound to 
-00009e20: 6772 6f75 705f 6e61 6d65 206f 6e20 7468  group_name on th
-00009e30: 6973 2063 6f72 652e 0d0a 0d0a 2020 2020  is core.....    
-00009e40: 2020 2020 3a73 7061 726b 6c65 733a 202a      :sparkles: *
-00009e50: 5468 6973 206d 6574 686f 6420 6973 206e  This method is n
-00009e60: 6577 2069 6e20 6043 4d4d 436f 7265 506c  ew in `CMMCorePl
-00009e70: 7573 602e 2a0d 0a0d 0a20 2020 2020 2020  us`.*....       
-00009e80: 205b 6043 6f6e 6669 6747 726f 7570 605d   [`ConfigGroup`]
-00009e90: 5b70 796d 6d63 6f72 655f 706c 7573 2e43  [pymmcore_plus.C
-00009ea0: 6f6e 6669 6747 726f 7570 5d20 6f62 6a65  onfigGroup] obje
-00009eb0: 6374 7320 6172 6520 6120 636f 6e76 656e  cts are a conven
-00009ec0: 6965 6e74 206f 626a 6563 740d 0a20 2020  ient object..   
-00009ed0: 2020 2020 206f 7269 656e 7465 6420 7761       oriented wa
-00009ee0: 7920 746f 2069 6e74 6572 6163 7420 7769  y to interact wi
-00009ef0: 7468 2063 6f6e 6669 6775 7261 7469 6f6e  th configuration
-00009f00: 2067 726f 7570 7320 2869 2e65 2e20 6772   groups (i.e. gr
-00009f10: 6f75 7073 206f 660d 0a20 2020 2020 2020  oups of..       
-00009f20: 205b 436f 6e66 6967 7572 6174 696f 6e0d   [Configuration.
-00009f30: 0a20 2020 2020 2020 2050 7265 7365 7473  .        Presets
-00009f40: 5d28 6874 7470 733a 2f2f 6d69 6372 6f2d  ](https://micro-
-00009f50: 6d61 6e61 6765 722e 6f72 672f 4d69 6372  manager.org/Micr
-00009f60: 6f2d 4d61 6e61 6765 725f 436f 6e66 6967  o-Manager_Config
-00009f70: 7572 6174 696f 6e5f 4775 6964 6523 636f  uration_Guide#co
-00009f80: 6e66 6967 7572 6174 696f 6e2d 7072 6573  nfiguration-pres
-00009f90: 6574 7329 0d0a 2020 2020 2020 2020 696e  ets)..        in
-00009fa0: 204d 6963 726f 2d4d 616e 6167 6572 292e   Micro-Manager).
-00009fb0: 2054 6865 7920 616c 6c6f 7720 796f 7520   They allow you 
-00009fc0: 746f 2063 616c 6c20 616e 7920 6d65 7468  to call any meth
-00009fd0: 6f64 206f 6e20 6043 4d4d 436f 7265 6020  od on `CMMCore` 
-00009fe0: 7468 6174 206e 6f72 6d61 6c6c 790d 0a20  that normally.. 
-00009ff0: 2020 2020 2020 2072 6571 7569 7265 7320         requires 
-0000a000: 6120 6067 726f 7570 4e61 6d65 6020 6173  a `groupName` as
-0000a010: 2074 6865 2066 6972 7374 2061 7267 756d   the first argum
-0000a020: 656e 7420 6173 2061 6e20 6172 6775 6d65  ent as an argume
-0000a030: 6e74 2d66 7265 6520 6d65 7468 6f64 206f  nt-free method o
-0000a040: 6e20 7468 650d 0a20 2020 2020 2020 2060  n the..        `
-0000a050: 436f 6e66 6967 4772 6f75 7060 206f 626a  ConfigGroup` obj
-0000a060: 6563 742e 0d0a 0d0a 2020 2020 2020 2020  ect.....        
-0000a070: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-0000a080: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-0000a090: 2020 2020 2020 2020 6772 6f75 705f 6e61          group_na
-0000a0a0: 6d65 203a 2073 7472 0d0a 2020 2020 2020  me : str..      
-0000a0b0: 2020 2020 2020 436f 6e66 6967 7572 6174        Configurat
-0000a0c0: 696f 6e20 6772 6f75 7020 6e61 6d65 2074  ion group name t
-0000a0d0: 6f20 6765 7420 6120 636f 6e66 6967 2067  o get a config g
-0000a0e0: 726f 7570 206f 626a 6563 7420 666f 722e  roup object for.
-0000a0f0: 0d0a 0d0a 2020 2020 2020 2020 4578 616d  ....        Exam
-0000a100: 706c 6573 0d0a 2020 2020 2020 2020 2d2d  ples..        --
-0000a110: 2d2d 2d2d 2d2d 0d0a 0d0a 2020 2020 2020  ------....      
-0000a120: 2020 2222 220d 0a20 2020 2020 2020 2067    """..        g
-0000a130: 726f 7570 203d 2043 6f6e 6669 6747 726f  roup = ConfigGro
-0000a140: 7570 2867 726f 7570 5f6e 616d 652c 206d  up(group_name, m
-0000a150: 6d63 6f72 653d 7365 6c66 290d 0a20 2020  mcore=self)..   
-0000a160: 2020 2020 2069 6620 6e6f 7420 616c 6c6f       if not allo
-0000a170: 775f 6d69 7373 696e 6720 616e 6420 6e6f  w_missing and no
-0000a180: 7420 6772 6f75 702e 6578 6973 7473 2829  t group.exists()
-0000a190: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0000a1a0: 6169 7365 204b 6579 4572 726f 7228 0d0a  aise KeyError(..
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 6622 436f 6e66 6967 7572 6174 696f 6e20  f"Configuration 
-0000a1d0: 6772 6f75 7020 7b67 726f 7570 5f6e 616d  group {group_nam
-0000a1e0: 6521 727d 2064 6f65 7320 6e6f 7420 6578  e!r} does not ex
-0000a1f0: 6973 742e 2022 0d0a 2020 2020 2020 2020  ist. "..        
-0000a200: 2020 2020 2020 2020 2255 7365 2060 616c          "Use `al
-0000a210: 6c6f 775f 6d69 7373 696e 673d 5472 7565  low_missing=True
-0000a220: 6020 746f 2063 7265 6174 6520 6372 6561  ` to create crea
-0000a230: 7465 206e 6f6e 2d65 7869 7374 656e 7420  te non-existent 
-0000a240: 636f 6e66 6967 2067 726f 7570 732e 220d  config groups.".
-0000a250: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-0000a260: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-0000a270: 726f 7570 0d0a 0d0a 2020 2020 6465 6620  roup....    def 
-0000a280: 6974 6572 436f 6e66 6967 4772 6f75 7073  iterConfigGroups
-0000a290: 2873 656c 6629 202d 3e20 4974 6572 6174  (self) -> Iterat
-0000a2a0: 6f72 5b43 6f6e 6669 6747 726f 7570 5d3a  or[ConfigGroup]:
-0000a2b0: 0d0a 2020 2020 2020 2020 2222 2249 7465  ..        """Ite
-0000a2c0: 7261 7465 2060 436f 6e66 6967 4772 6f75  rate `ConfigGrou
-0000a2d0: 7060 206f 626a 6563 7473 2066 6f72 2061  p` objects for a
-0000a2e0: 6c6c 2063 6f6e 6669 6773 2e0d 0a0d 0a20  ll configs..... 
-0000a2f0: 2020 2020 2020 203a 7370 6172 6b6c 6573         :sparkles
-0000a300: 3a20 2a54 6869 7320 6d65 7468 6f64 2069  : *This method i
-0000a310: 7320 6e65 7720 696e 2060 434d 4d43 6f72  s new in `CMMCor
-0000a320: 6550 6c75 7360 2e2a 0d0a 0d0a 2020 2020  ePlus`.*....    
-0000a330: 2020 2020 5969 656c 6473 0d0a 2020 2020      Yields..    
-0000a340: 2020 2020 2d2d 2d2d 2d2d 0d0a 2020 2020      ------..    
-0000a350: 2020 2020 436f 6e66 6967 4772 6f75 700d      ConfigGroup.
-0000a360: 0a20 2020 2020 2020 2020 2020 2060 436f  .            `Co
-0000a370: 6e66 6967 4772 6f75 7060 206f 626a 6563  nfigGroup` objec
-0000a380: 7473 0d0a 2020 2020 2020 2020 2222 220d  ts..        """.
-0000a390: 0a20 2020 2020 2020 2066 6f72 2067 726f  .        for gro
-0000a3a0: 7570 2069 6e20 7365 6c66 2e67 6574 4176  up in self.getAv
-0000a3b0: 6169 6c61 626c 6543 6f6e 6669 6747 726f  ailableConfigGro
-0000a3c0: 7570 7328 293a 0d0a 2020 2020 2020 2020  ups():..        
-0000a3d0: 2020 2020 7969 656c 6420 436f 6e66 6967      yield Config
-0000a3e0: 4772 6f75 7028 6772 6f75 702c 206d 6d63  Group(group, mmc
-0000a3f0: 6f72 653d 7365 6c66 290d 0a0d 0a20 2020  ore=self)....   
-0000a400: 2064 6566 2067 6574 4465 7669 6365 5363   def getDeviceSc
-0000a410: 6865 6d61 2873 656c 662c 2064 6576 6963  hema(self, devic
-0000a420: 655f 6c61 6265 6c3a 2073 7472 2920 2d3e  e_label: str) ->
-0000a430: 2044 6576 6963 6553 6368 656d 613a 0d0a   DeviceSchema:..
-0000a440: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-0000a450: 6e20 4a53 4f4e 2d73 6368 656d 6120 6465  n JSON-schema de
-0000a460: 7363 7269 6269 6e67 2064 6576 6963 6520  scribing device 
-0000a470: 6064 6576 6963 655f 6c61 6265 6c60 2061  `device_label` a
-0000a480: 6e64 2069 7473 2070 726f 7065 7274 6965  nd its propertie
-0000a490: 732e 0d0a 0d0a 2020 2020 2020 2020 3a73  s.....        :s
-0000a4a0: 7061 726b 6c65 733a 202a 5468 6973 206d  parkles: *This m
-0000a4b0: 6574 686f 6420 6973 206e 6577 2069 6e20  ethod is new in 
-0000a4c0: 6043 4d4d 436f 7265 506c 7573 602e 2049  `CMMCorePlus`. I
-0000a4d0: 7420 7072 6f76 6964 6573 2061 2063 6f6e  t provides a con
-0000a4e0: 7665 6e69 656e 7420 7761 7920 746f 0d0a  venient way to..
-0000a4f0: 2020 2020 2020 2020 6765 7420 616c 6c20          get all 
-0000a500: 6f66 2074 6865 2069 6e66 6f72 6d61 7469  of the informati
-0000a510: 6f6e 2061 626f 7574 2061 2064 6576 6963  on about a devic
-0000a520: 6520 696e 2061 2073 696e 676c 6520 6361  e in a single ca
-0000a530: 6c6c 2e2a 0d0a 0d0a 2020 2020 2020 2020  ll.*....        
-0000a540: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
-0000a550: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-0000a560: 2020 4465 7669 6365 5363 6865 6d61 0d0a    DeviceSchema..
-0000a570: 2020 2020 2020 2020 2020 2020 4a53 4f4e              JSON
-0000a580: 2d73 6368 656d 6120 6465 7363 7269 6269  -schema describi
-0000a590: 6e67 2064 6576 6963 6520 6064 6576 6963  ng device `devic
-0000a5a0: 655f 6c61 6265 6c60 2061 6e64 2069 7473  e_label` and its
-0000a5b0: 2070 726f 7065 7274 6965 732e 0d0a 0d0a   properties.....
-0000a5c0: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-0000a5d0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-0000a5e0: 2d2d 0d0a 2020 2020 2020 2020 3e3e 3e20  --..        >>> 
-0000a5f0: 636f 7265 203d 2043 4d4d 436f 7265 506c  core = CMMCorePl
-0000a600: 7573 2829 0d0a 2020 2020 2020 2020 3e3e  us()..        >>
-0000a610: 3e20 636f 7265 2e6c 6f61 6444 6576 6963  > core.loadDevic
-0000a620: 6528 2244 656d 6f43 616d 6572 6122 2c20  e("DemoCamera", 
-0000a630: 2244 656d 6f43 616d 6572 6122 2c20 2244  "DemoCamera", "D
-0000a640: 4361 6d22 290d 0a20 2020 2020 2020 203e  Cam")..        >
-0000a650: 3e3e 2063 6f72 652e 6765 7444 6576 6963  >> core.getDevic
-0000a660: 6553 6368 656d 6128 2244 656d 6f43 616d  eSchema("DemoCam
-0000a670: 6572 6122 290d 0a20 2020 2020 2020 207b  era")..        {
-0000a680: 0d0a 2020 2020 2020 2020 2020 2020 2774  ..            't
-0000a690: 6974 6c65 273a 2027 4443 616d 272c 0d0a  itle': 'DCam',..
-0000a6a0: 2020 2020 2020 2020 2020 2020 2764 6573              'des
-0000a6b0: 6372 6970 7469 6f6e 273a 2027 4465 6d6f  cription': 'Demo
-0000a6c0: 2063 616d 6572 6127 2c0d 0a20 2020 2020   camera',..     
-0000a6d0: 2020 2020 2020 2027 7479 7065 273a 2027         'type': '
-0000a6e0: 6f62 6a65 6374 272c 0d0a 2020 2020 2020  object',..      
-0000a6f0: 2020 2020 2020 2770 726f 7065 7274 6965        'propertie
-0000a700: 7327 3a20 7b0d 0a20 2020 2020 2020 2020  s': {..         
-0000a710: 2020 2020 2020 2027 4875 6249 4427 3a20         'HubID': 
-0000a720: 7b27 7479 7065 273a 2027 7374 7269 6e67  {'type': 'string
-0000a730: 272c 2027 7265 6164 4f6e 6c79 273a 2054  ', 'readOnly': T
-0000a740: 7275 652c 2027 6465 6661 756c 7427 3a20  rue, 'default': 
-0000a750: 2727 7d2c 0d0a 2020 2020 2020 2020 2020  ''},..          
-0000a760: 2020 2020 2020 274d 6178 696d 756d 4578        'MaximumEx
-0000a770: 706f 7375 7265 4d73 273a 207b 2774 7970  posureMs': {'typ
-0000a780: 6527 3a20 276e 756d 6265 7227 2c20 2770  e': 'number', 'p
-0000a790: 7265 496e 6974 273a 2054 7275 657d 2c0d  reInit': True},.
-0000a7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7b0: 2027 5472 616e 7370 6f73 6543 6f72 7265   'TransposeCorre
-0000a7c0: 6374 696f 6e27 3a20 7b27 7479 7065 273a  ction': {'type':
-0000a7d0: 2027 626f 6f6c 6561 6e27 7d2c 0d0a 2020   'boolean'},..  
-0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2754                'T
-0000a7f0: 7261 6e73 706f 7365 4d69 7272 6f72 5827  ransposeMirrorX'
-0000a800: 3a20 7b27 7479 7065 273a 2027 626f 6f6c  : {'type': 'bool
-0000a810: 6561 6e27 7d2c 0d0a 2020 2020 2020 2020  ean'},..        
-0000a820: 2020 2020 2020 2020 2754 7261 6e73 706f          'Transpo
-0000a830: 7365 4d69 7272 6f72 5927 3a20 7b27 7479  seMirrorY': {'ty
-0000a840: 7065 273a 2027 626f 6f6c 6561 6e27 7d2c  pe': 'boolean'},
-0000a850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a860: 2020 2754 7261 6e73 706f 7365 5859 273a    'TransposeXY':
-0000a870: 207b 2774 7970 6527 3a20 2762 6f6f 6c65   {'type': 'boole
-0000a880: 616e 277d 0d0a 2020 2020 2020 2020 2020  an'}..          
-0000a890: 2020 7d0d 0a20 2020 2020 2020 207d 0d0a    }..        }..
-0000a8a0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000a8b0: 2020 2020 2064 3a20 4465 7669 6365 5363       d: DeviceSc
-0000a8c0: 6865 6d61 203d 207b 0d0a 2020 2020 2020  hema = {..      
-0000a8d0: 2020 2020 2020 2274 6974 6c65 223a 2073        "title": s
-0000a8e0: 656c 662e 6765 7444 6576 6963 654e 616d  elf.getDeviceNam
-0000a8f0: 6528 6465 7669 6365 5f6c 6162 656c 292c  e(device_label),
-0000a900: 0d0a 2020 2020 2020 2020 2020 2020 2264  ..            "d
-0000a910: 6573 6372 6970 7469 6f6e 223a 2073 656c  escription": sel
-0000a920: 662e 6765 7444 6576 6963 6544 6573 6372  f.getDeviceDescr
-0000a930: 6970 7469 6f6e 2864 6576 6963 655f 6c61  iption(device_la
-0000a940: 6265 6c29 2c0d 0a20 2020 2020 2020 2020  bel),..         
-0000a950: 2020 2022 7479 7065 223a 2022 6f62 6a65     "type": "obje
-0000a960: 6374 222c 0d0a 2020 2020 2020 2020 2020  ct",..          
-0000a970: 2020 2270 726f 7065 7274 6965 7322 3a20    "properties": 
-0000a980: 7b7d 2c0d 0a20 2020 2020 2020 207d 0d0a  {},..        }..
-0000a990: 2020 2020 2020 2020 666f 7220 7072 6f70          for prop
-0000a9a0: 2069 6e20 7365 6c66 2e69 7465 7250 726f   in self.iterPro
-0000a9b0: 7065 7274 6965 7328 6465 7669 6365 5f6c  perties(device_l
-0000a9c0: 6162 656c 3d64 6576 6963 655f 6c61 6265  abel=device_labe
-0000a9d0: 6c2c 2061 735f 6f62 6a65 6374 3d54 7275  l, as_object=Tru
-0000a9e0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-0000a9f0: 2070 3a20 5072 6f70 6572 7479 5363 6865   p: PropertySche
-0000aa00: 6d61 0d0a 2020 2020 2020 2020 2020 2020  ma..            
-0000aa10: 645b 2270 726f 7065 7274 6965 7322 5d5b  d["properties"][
-0000aa20: 7072 6f70 2e6e 616d 655d 203d 2070 203d  prop.name] = p =
-0000aa30: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-0000aa40: 2069 6620 7072 6f70 2e74 7970 6528 292e   if prop.type().
-0000aa50: 746f 5f6a 736f 6e28 2920 213d 2022 6e75  to_json() != "nu
-0000aa60: 6c6c 223a 0d0a 2020 2020 2020 2020 2020  ll":..          
-0000aa70: 2020 2020 2020 705b 2274 7970 6522 5d20        p["type"] 
-0000aa80: 3d20 7072 6f70 2e74 7970 6528 292e 746f  = prop.type().to
-0000aa90: 5f6a 736f 6e28 290d 0a20 2020 2020 2020  _json()..       
-0000aaa0: 2020 2020 2069 6620 7072 6f70 2e68 6173       if prop.has
-0000aab0: 4c69 6d69 7473 2829 3a0d 0a20 2020 2020  Limits():..     
-0000aac0: 2020 2020 2020 2020 2020 2070 5b22 6d69             p["mi
-0000aad0: 6e69 6d75 6d22 5d20 3d20 7072 6f70 2e6c  nimum"] = prop.l
-0000aae0: 6f77 6572 4c69 6d69 7428 290d 0a20 2020  owerLimit()..   
-0000aaf0: 2020 2020 2020 2020 2020 2020 2070 5b22               p["
-0000ab00: 6d61 7869 6d75 6d22 5d20 3d20 7072 6f70  maximum"] = prop
-0000ab10: 2e75 7070 6572 4c69 6d69 7428 290d 0a20  .upperLimit().. 
-0000ab20: 2020 2020 2020 2020 2020 2069 6620 616c             if al
-0000ab30: 6c6f 7765 6420 3a3d 2070 726f 702e 616c  lowed := prop.al
-0000ab40: 6c6f 7765 6456 616c 7565 7328 293a 0d0a  lowedValues():..
-0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab60: 6966 2073 6574 2861 6c6c 6f77 6564 2920  if set(allowed) 
-0000ab70: 3d3d 207b 2230 222c 2022 3122 7d20 616e  == {"0", "1"} an
-0000ab80: 6420 7072 6f70 2e74 7970 6528 2920 3d3d  d prop.type() ==
-0000ab90: 2050 726f 7065 7274 7954 7970 652e 496e   PropertyType.In
-0000aba0: 7465 6765 723a 0d0a 2020 2020 2020 2020  teger:..        
-0000abb0: 2020 2020 2020 2020 2020 2020 705b 2274              p["t
-0000abc0: 7970 6522 5d20 3d20 2262 6f6f 6c65 616e  ype"] = "boolean
-0000abd0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000abe0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-0000ac00: 7320 3d20 7072 6f70 2e74 7970 6528 292e  s = prop.type().
-0000ac10: 746f 5f70 7974 686f 6e28 290d 0a20 2020  to_python()..   
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac30: 2070 5b22 656e 756d 225d 203d 205b 636c   p["enum"] = [cl
-0000ac40: 7328 6929 2069 6620 636c 7320 656c 7365  s(i) if cls else
-0000ac50: 2069 2066 6f72 2069 2069 6e20 616c 6c6f   i for i in allo
-0000ac60: 7765 645d 0d0a 2020 2020 2020 2020 2020  wed]..          
-0000ac70: 2020 6966 2070 726f 702e 6973 5265 6164    if prop.isRead
-0000ac80: 4f6e 6c79 2829 3a0d 0a20 2020 2020 2020  Only():..       
-0000ac90: 2020 2020 2020 2020 2070 5b22 7265 6164           p["read
-0000aca0: 4f6e 6c79 225d 203d 2054 7275 650d 0a20  Only"] = True.. 
-0000acb0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000acc0: 5b22 6465 6661 756c 7422 5d20 3d20 7072  ["default"] = pr
-0000acd0: 6f70 2e76 616c 7565 0d0a 2020 2020 2020  op.value..      
-0000ace0: 2020 2020 2020 6966 2070 726f 702e 6973        if prop.is
-0000acf0: 5365 7175 656e 6365 6162 6c65 2829 3a0d  Sequenceable():.
-0000ad00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ad10: 2070 5b22 7365 7175 656e 6365 6162 6c65   p["sequenceable
-0000ad20: 225d 203d 2054 7275 650d 0a20 2020 2020  "] = True..     
-0000ad30: 2020 2020 2020 2020 2020 2070 5b22 7365             p["se
-0000ad40: 7175 656e 6365 4d61 784c 656e 6774 6822  quenceMaxLength"
-0000ad50: 5d20 3d20 7072 6f70 2e73 6571 7565 6e63  ] = prop.sequenc
-0000ad60: 654d 6178 4c65 6e67 7468 2829 0d0a 2020  eMaxLength()..  
-0000ad70: 2020 2020 2020 2020 2020 6966 2070 726f            if pro
-0000ad80: 702e 6973 5072 6549 6e69 7428 293a 0d0a  p.isPreInit():..
-0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ada0: 705b 2270 7265 496e 6974 225d 203d 2054  p["preInit"] = T
-0000adb0: 7275 650d 0a20 2020 2020 2020 2072 6574  rue..        ret
-0000adc0: 7572 6e20 640d 0a0d 0a20 2020 2040 7072  urn d....    @pr
-0000add0: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-0000ade0: 6f62 6a65 6374 6976 655f 6465 7669 6365  objective_device
-0000adf0: 5f70 6174 7465 726e 2873 656c 6629 202d  _pattern(self) -
-0000ae00: 3e20 5061 7474 6572 6e3a 0d0a 2020 2020  > Pattern:..    
-0000ae10: 2020 2020 2222 2250 6174 7465 726e 2075      """Pattern u
-0000ae20: 7365 6420 746f 2067 7565 7373 206f 626a  sed to guess obj
-0000ae30: 6563 7469 7665 2064 6576 6963 6520 6c61  ective device la
-0000ae40: 6265 6c73 2e0d 0a0d 0a20 2020 2020 2020  bels.....       
-0000ae50: 203a 7370 6172 6b6c 6573 3a20 2a54 6869   :sparkles: *Thi
-0000ae60: 7320 7072 6f70 6572 7479 2069 7320 6e65  s property is ne
-0000ae70: 7720 696e 2060 434d 4d43 6f72 6550 6c75  w in `CMMCorePlu
-0000ae80: 7360 2e0d 0a0d 0a20 2020 2020 2020 2049  s`.....        I
-0000ae90: 7420 6973 2074 6865 2072 6567 6578 2075  t is the regex u
-0000aea0: 7365 6420 6279 0d0a 2020 2020 2020 2020  sed by..        
-0000aeb0: 5b60 6775 6573 734f 626a 6563 7469 7665  [`guessObjective
-0000aec0: 4465 7669 6365 7360 5d5b 7079 6d6d 636f  Devices`][pymmco
-0000aed0: 7265 5f70 6c75 732e 434d 4d43 6f72 6550  re_plus.CMMCoreP
-0000aee0: 6c75 732e 6775 6573 734f 626a 6563 7469  lus.guessObjecti
-0000aef0: 7665 4465 7669 6365 735d 2074 6f0d 0a20  veDevices] to.. 
-0000af00: 2020 2020 2020 2066 696e 6420 616e 7920         find any 
-0000af10: 6465 7669 6365 7320 7468 6174 2061 7265  devices that are
-0000af20: 206c 696b 656c 7920 746f 2062 6520 6f62   likely to be ob
-0000af30: 6a65 6374 6976 6520 6465 7669 6365 732e  jective devices.
-0000af40: 0d0a 0d0a 2020 2020 2020 2020 4279 2064  ....        By d
-0000af50: 6566 6175 6c74 3a0d 0a0d 0a20 2020 2020  efault:....     
-0000af60: 2020 2020 2020 2072 652e 636f 6d70 696c         re.compil
-0000af70: 6528 2228 2e2b 293f 286e 6f73 6570 6965  e("(.+)?(nosepie
-0000af80: 6365 7c6f 626a 2865 6374 6976 6529 3f29  ce|obj(ective)?)
-0000af90: 2874 7572 7265 7429 3f73 3f22 2c20 7265  (turret)?s?", re
-0000afa0: 2e49 474e 4f52 4543 4153 4529 0d0a 2020  .IGNORECASE)..  
-0000afb0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0000afc0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000afd0: 6f62 6a65 6374 6976 655f 7265 6765 780d  objective_regex.
-0000afe0: 0a0d 0a20 2020 2040 6f62 6a65 6374 6976  ...    @objectiv
-0000aff0: 655f 6465 7669 6365 5f70 6174 7465 726e  e_device_pattern
-0000b000: 2e73 6574 7465 720d 0a20 2020 2064 6566  .setter..    def
-0000b010: 206f 626a 6563 7469 7665 5f64 6576 6963   objective_devic
-0000b020: 655f 7061 7474 6572 6e28 7365 6c66 2c20  e_pattern(self, 
-0000b030: 7661 6c75 653a 2050 6174 7465 726e 207c  value: Pattern |
-0000b040: 2073 7472 2920 2d3e 204e 6f6e 653a 0d0a   str) -> None:..
-0000b050: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000b060: 7461 6e63 6528 7661 6c75 652c 2073 7472  tance(value, str
-0000b070: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000b080: 7661 6c75 6520 3d20 7265 2e63 6f6d 7069  value = re.compi
-0000b090: 6c65 2876 616c 7565 2c20 7265 2e49 474e  le(value, re.IGN
-0000b0a0: 4f52 4543 4153 4529 0d0a 2020 2020 2020  ORECASE)..      
-0000b0b0: 2020 656c 6966 206e 6f74 2069 7369 6e73    elif not isins
-0000b0c0: 7461 6e63 6528 7661 6c75 652c 2050 6174  tance(value, Pat
-0000b0d0: 7465 726e 293a 0d0a 2020 2020 2020 2020  tern):..        
-0000b0e0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-0000b0f0: 726f 7228 0d0a 2020 2020 2020 2020 2020  ror(..          
-0000b100: 2020 2020 2020 224f 626a 6563 7469 7665        "Objective
-0000b110: 2050 6174 7465 726e 206d 7573 7420 6265   Pattern must be
-0000b120: 2061 2073 7472 696e 6720 6f72 2063 6f6d   a string or com
-0000b130: 7069 6c65 6420 7265 6765 7822 0d0a 2020  piled regex"..  
-0000b140: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000b150: 2062 7574 2069 7320 7479 7065 207b 7479   but is type {ty
-0000b160: 7065 2876 616c 7565 297d 220d 0a20 2020  pe(value)}"..   
-0000b170: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0000b180: 2020 2020 7365 6c66 2e5f 6f62 6a65 6374      self._object
-0000b190: 6976 655f 7265 6765 7820 3d20 7661 6c75  ive_regex = valu
-0000b1a0: 650d 0a0d 0a20 2020 2040 7072 6f70 6572  e....    @proper
-0000b1b0: 7479 0d0a 2020 2020 6465 6620 6368 616e  ty..    def chan
-0000b1c0: 6e65 6c47 726f 7570 5f70 6174 7465 726e  nelGroup_pattern
-0000b1d0: 2873 656c 6629 202d 3e20 5061 7474 6572  (self) -> Patter
-0000b1e0: 6e3a 0d0a 2020 2020 2020 2020 2222 2254  n:..        """T
-0000b1f0: 6865 2072 6567 6578 2070 6174 7465 726e  he regex pattern
-0000b200: 2075 7365 6420 746f 2069 6465 6e74 6966   used to identif
-0000b210: 7920 6368 616e 6e65 6c20 6772 6f75 7073  y channel groups
-0000b220: 2e0d 0a0d 0a20 2020 2020 2020 203a 7370  .....        :sp
-0000b230: 6172 6b6c 6573 3a20 2a54 6869 7320 7072  arkles: *This pr
-0000b240: 6f70 6572 7479 2069 7320 6e65 7720 696e  operty is new in
-0000b250: 2060 434d 4d43 6f72 6550 6c75 7360 2e0d   `CMMCorePlus`..
-0000b260: 0a0d 0a20 2020 2020 2020 2049 7420 6973  ...        It is
-0000b270: 2074 6865 2072 6567 6578 2075 7365 6420   the regex used 
-0000b280: 6279 0d0a 2020 2020 2020 2020 5b60 6765  by..        [`ge
-0000b290: 744f 7247 7565 7373 4368 616e 6e65 6c47  tOrGuessChannelG
-0000b2a0: 726f 7570 605d 5b70 796d 6d63 6f72 655f  roup`][pymmcore_
-0000b2b0: 706c 7573 2e43 4d4d 436f 7265 506c 7573  plus.CMMCorePlus
-0000b2c0: 2e67 6574 4f72 4775 6573 7343 6861 6e6e  .getOrGuessChann
-0000b2d0: 656c 4772 6f75 705d 2074 6f0d 0a20 2020  elGroup] to..   
-0000b2e0: 2020 2020 2066 696e 6420 6120 636f 6e66       find a conf
-0000b2f0: 6967 2067 726f 7570 206c 696b 656c 7920  ig group likely 
-0000b300: 746f 2062 6520 6120 6368 616e 6e65 6c20  to be a channel 
-0000b310: 6772 6f75 7020 696e 2060 6765 7441 7661  group in `getAva
-0000b320: 696c 6162 6c65 436f 6e66 6967 4772 6f75  ilableConfigGrou
-0000b330: 7073 600d 0a20 2020 2020 2020 2069 6620  ps`..        if 
-0000b340: 6067 6574 4368 616e 6e65 6c47 726f 7570  `getChannelGroup
-0000b350: 6020 7265 7475 726e 7320 604e 6f6e 6560  ` returns `None`
-0000b360: 2e0d 0a0d 0a20 2020 2020 2020 2042 7920  .....        By 
-0000b370: 6465 6661 756c 743a 0d0a 0d0a 2020 2020  default:....    
-0000b380: 2020 2020 2020 2020 7265 2e63 6f6d 7069          re.compi
-0000b390: 6c65 2822 2863 6861 6e7b 312c 327d 2865  le("(chan{1,2}(e
-0000b3a0: 6c29 3f7c 6669 6c74 2865 7229 3f29 733f  l)?|filt(er)?)s?
-0000b3b0: 222c 2072 652e 4947 4e4f 5245 4341 5345  ", re.IGNORECASE
-0000b3c0: 290d 0a20 2020 2020 2020 2022 2222 0d0a  )..        """..
-0000b3d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000b3e0: 656c 662e 5f63 6861 6e6e 656c 5f67 726f  elf._channel_gro
-0000b3f0: 7570 5f72 6567 6578 0d0a 0d0a 2020 2020  up_regex....    
-0000b400: 4063 6861 6e6e 656c 4772 6f75 705f 7061  @channelGroup_pa
-0000b410: 7474 6572 6e2e 7365 7474 6572 0d0a 2020  ttern.setter..  
-0000b420: 2020 6465 6620 6368 616e 6e65 6c47 726f    def channelGro
-0000b430: 7570 5f70 6174 7465 726e 2873 656c 662c  up_pattern(self,
-0000b440: 2076 616c 7565 3a20 5061 7474 6572 6e20   value: Pattern 
-0000b450: 7c20 7374 7229 202d 3e20 4e6f 6e65 3a0d  | str) -> None:.
-0000b460: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000b470: 7374 616e 6365 2876 616c 7565 2c20 7374  stance(value, st
-0000b480: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
-0000b490: 2076 616c 7565 203d 2072 652e 636f 6d70   value = re.comp
-0000b4a0: 696c 6528 7661 6c75 652c 2072 652e 4947  ile(value, re.IG
-0000b4b0: 4e4f 5245 4341 5345 290d 0a20 2020 2020  NORECASE)..     
-0000b4c0: 2020 2065 6c69 6620 6e6f 7420 6973 696e     elif not isin
-0000b4d0: 7374 616e 6365 2876 616c 7565 2c20 5061  stance(value, Pa
-0000b4e0: 7474 6572 6e29 3a0d 0a20 2020 2020 2020  ttern):..       
-0000b4f0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-0000b500: 7272 6f72 280d 0a20 2020 2020 2020 2020  rror(..         
-0000b510: 2020 2020 2020 2022 6368 616e 6e65 6c47         "channelG
-0000b520: 726f 7570 2050 6174 7465 726e 206d 7573  roup Pattern mus
-0000b530: 7420 6265 2061 2073 7472 696e 6720 6f72  t be a string or
-0000b540: 2063 6f6d 7069 6c65 6420 7265 6765 7822   compiled regex"
-0000b550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b560: 2020 6622 6275 7420 6973 2074 7970 6520    f"but is type 
-0000b570: 7b74 7970 6528 7661 6c75 6529 7d22 0d0a  {type(value)}"..
-0000b580: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-0000b590: 2020 2020 2020 2073 656c 662e 5f63 6861         self._cha
-0000b5a0: 6e6e 656c 5f67 726f 7570 5f72 6567 6578  nnel_group_regex
-0000b5b0: 203d 2076 616c 7565 0d0a 0d0a 2020 2020   = value....    
-0000b5c0: 6465 6620 6775 6573 734f 626a 6563 7469  def guessObjecti
-0000b5d0: 7665 4465 7669 6365 7328 7365 6c66 2920  veDevices(self) 
-0000b5e0: 2d3e 206c 6973 745b 7374 725d 3a0d 0a20  -> list[str]:.. 
-0000b5f0: 2020 2020 2020 2022 2222 4669 6e64 2061         """Find a
-0000b600: 6e79 206c 6f61 6465 6420 6465 7669 6365  ny loaded device
-0000b610: 7320 7468 6174 2061 7265 206c 696b 656c  s that are likel
-0000b620: 7920 746f 2062 6520 616e 204f 626a 6563  y to be an Objec
-0000b630: 7469 7665 2f4e 6f73 6570 6965 6365 2e0d  tive/Nosepiece..
-0000b640: 0a0d 0a20 2020 2020 2020 203a 7370 6172  ...        :spar
-0000b650: 6b6c 6573 3a20 2a54 6869 7320 6d65 7468  kles: *This meth
-0000b660: 6f64 2069 7320 6e65 7720 696e 2060 434d  od is new in `CM
-0000b670: 4d43 6f72 6550 6c75 7360 2e2a 0d0a 0d0a  MCorePlus`.*....
-0000b680: 2020 2020 2020 2020 4c69 6b65 6c79 206d          Likely m
-0000b690: 6174 6368 6573 2061 7265 206c 6f61 6465  atches are loade
-0000b6a0: 6420 5374 6174 6544 6576 6963 6573 2077  d StateDevices w
-0000b6b0: 6974 6820 6e61 6d65 7320 7468 6174 206d  ith names that m
-0000b6c0: 6174 6368 2074 6869 7320 6f62 6a65 6374  atch this object
-0000b6d0: 2773 0d0a 2020 2020 2020 2020 606f 626a  's..        `obj
-0000b6e0: 6563 7469 7665 5f64 6576 6963 655f 7061  ective_device_pa
-0000b6f0: 7474 6572 6e60 2070 726f 7065 7274 792e  ttern` property.
-0000b700: 2054 6869 7320 6973 2061 2073 6574 7461   This is a setta
-0000b710: 626c 6520 7072 6f70 6572 7479 0d0a 2020  ble property..  
-0000b720: 2020 2020 2020 7769 7468 2061 2064 6566        with a def
-0000b730: 6175 6c74 2076 616c 7565 206f 663a 3a0d  ault value of::.
-0000b740: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-0000b750: 652e 636f 6d70 696c 6528 2228 2e2b 293f  e.compile("(.+)?
-0000b760: 286e 6f73 6570 6965 6365 7c6f 626a 2865  (nosepiece|obj(e
-0000b770: 6374 6976 6529 3f29 2874 7572 7265 7429  ctive)?)(turret)
-0000b780: 3f73 3f22 2c20 7265 2e49 474e 4f52 4543  ?s?", re.IGNOREC
-0000b790: 4153 4529 0d0a 2020 2020 2020 2020 2222  ASE)..        ""
-0000b7a0: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0000b7b0: 6e20 5b0d 0a20 2020 2020 2020 2020 2020  n [..           
-0000b7c0: 2064 6576 6963 650d 0a20 2020 2020 2020   device..       
-0000b7d0: 2020 2020 2066 6f72 2064 6576 6963 6520       for device 
-0000b7e0: 696e 2073 656c 662e 6765 744c 6f61 6465  in self.getLoade
-0000b7f0: 6444 6576 6963 6573 4f66 5479 7065 2844  dDevicesOfType(D
-0000b800: 6576 6963 6554 7970 652e 5374 6174 6544  eviceType.StateD
-0000b810: 6576 6963 6529 0d0a 2020 2020 2020 2020  evice)..        
-0000b820: 2020 2020 6966 2073 656c 662e 5f6f 626a      if self._obj
-0000b830: 6563 7469 7665 5f72 6567 6578 2e6d 6174  ective_regex.mat
-0000b840: 6368 2864 6576 6963 6529 0d0a 2020 2020  ch(device)..    
-0000b850: 2020 2020 5d0d 0a0d 0a20 2020 2064 6566      ]....    def
-0000b860: 2067 6574 4f72 4775 6573 7343 6861 6e6e   getOrGuessChann
-0000b870: 656c 4772 6f75 7028 7365 6c66 2920 2d3e  elGroup(self) ->
-0000b880: 206c 6973 745b 7374 725d 3a0d 0a20 2020   list[str]:..   
-0000b890: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
-0000b8a0: 6368 616e 6e65 6c47 726f 7570 206f 7220  channelGroup or 
-0000b8b0: 6669 6e64 2061 206c 696b 656c 7920 7365  find a likely se
-0000b8c0: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
-0000b8d0: 0d0a 0d0a 2020 2020 2020 2020 3a73 7061  ....        :spa
-0000b8e0: 726b 6c65 733a 202a 5468 6973 206d 6574  rkles: *This met
-0000b8f0: 686f 6420 6973 206e 6577 2069 6e20 6043  hod is new in `C
-0000b900: 4d4d 436f 7265 506c 7573 602e 2a0d 0a0d  MMCorePlus`.*...
-0000b910: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
-0000b920: 6772 6f75 7020 6973 206e 6f74 2064 6566  group is not def
-0000b930: 696e 6564 2076 6961 2060 2e67 6574 4368  ined via `.getCh
-0000b940: 616e 6e65 6c47 726f 7570 6020 7468 656e  annelGroup` then
-0000b950: 206c 696b 656c 7920 6361 6e64 6964 6174   likely candidat
-0000b960: 6573 0d0a 2020 2020 2020 2020 7769 6c6c  es..        will
-0000b970: 2062 6520 666f 756e 6420 6279 2073 6561   be found by sea
-0000b980: 7263 6869 6e67 2066 6f72 2063 6f6e 6669  rching for confi
-0000b990: 6720 6772 6f75 7073 2077 6974 6820 6e61  g groups with na
-0000b9a0: 6d65 7320 7468 6174 206d 6174 6368 2074  mes that match t
-0000b9b0: 6869 730d 0a20 2020 2020 2020 206f 626a  his..        obj
-0000b9c0: 6563 7427 7320 6063 6861 6e6e 656c 4772  ect's `channelGr
-0000b9d0: 6f75 705f 7061 7474 6572 6e60 2070 726f  oup_pattern` pro
-0000b9e0: 7065 7274 792e 2054 6869 7320 6973 2061  perty. This is a
-0000b9f0: 2073 6574 7461 626c 6520 7072 6f70 6572   settable proper
-0000ba00: 7479 0d0a 2020 2020 2020 2020 7769 7468  ty..        with
-0000ba10: 2061 2064 6566 6175 6c74 2076 616c 7565   a default value
-0000ba20: 206f 663a 0d0a 0d0a 2020 2020 2020 2020   of:....        
-0000ba30: 2020 2020 7265 6720 3d20 7265 2e63 6f6d      reg = re.com
-0000ba40: 7069 6c65 2822 2863 6861 6e7b 312c 327d  pile("(chan{1,2}
-0000ba50: 2865 6c29 3f7c 6669 6c74 2865 7229 3f29  (el)?|filt(er)?)
-0000ba60: 733f 222c 2072 652e 4947 4e4f 5245 4341  s?", re.IGNORECA
-0000ba70: 5345 290d 0a0d 0a20 2020 2020 2020 2022  SE)....        "
-0000ba80: 2222 0d0a 2020 2020 2020 2020 2320 736f  ""..        # so
-0000ba90: 7572 6365 7279 2073 6b69 703a 2075 7365  urcery skip: use
-0000baa0: 2d6e 616d 6564 2d65 7870 7265 7373 696f  -named-expressio
-0000bab0: 6e0d 0a20 2020 2020 2020 2063 6861 6e5f  n..        chan_
-0000bac0: 6772 6f75 7020 3d20 7365 6c66 2e67 6574  group = self.get
-0000bad0: 4368 616e 6e65 6c47 726f 7570 2829 0d0a  ChannelGroup()..
-0000bae0: 2020 2020 2020 2020 6966 2063 6861 6e5f          if chan_
-0000baf0: 6772 6f75 703a 0d0a 2020 2020 2020 2020  group:..        
-0000bb00: 2020 2020 7265 7475 726e 205b 6368 616e      return [chan
-0000bb10: 5f67 726f 7570 5d0d 0a20 2020 2020 2020  _group]..       
-0000bb20: 2023 206e 6f74 2073 6574 2069 6e20 636f   # not set in co
-0000bb30: 7265 2e20 5472 7920 2243 6861 6e6e 656c  re. Try "Channel
-0000bb40: 2220 616e 6420 6f74 6865 7220 7661 7269  " and other vari
-0000bb50: 6174 696f 6e73 2061 7320 6661 6c6c 6261  ations as fallba
-0000bb60: 636b 730d 0a20 2020 2020 2020 2072 6574  cks..        ret
-0000bb70: 7572 6e20 5b0d 0a20 2020 2020 2020 2020  urn [..         
-0000bb80: 2020 2067 726f 7570 0d0a 2020 2020 2020     group..      
-0000bb90: 2020 2020 2020 666f 7220 6772 6f75 7020        for group 
-0000bba0: 696e 2073 656c 662e 6765 7441 7661 696c  in self.getAvail
-0000bbb0: 6162 6c65 436f 6e66 6967 4772 6f75 7073  ableConfigGroups
-0000bbc0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000bbd0: 6966 2073 656c 662e 5f63 6861 6e6e 656c  if self._channel
-0000bbe0: 5f67 726f 7570 5f72 6567 6578 2e6d 6174  _group_regex.mat
-0000bbf0: 6368 2867 726f 7570 290d 0a20 2020 2020  ch(group)..     
-0000bc00: 2020 205d 0d0a 0d0a 2020 2020 6465 6620     ]....    def 
-0000bc10: 7365 7452 656c 6174 6976 6558 595a 506f  setRelativeXYZPo
-0000bc20: 7369 7469 6f6e 280d 0a20 2020 2020 2020  sition(..       
-0000bc30: 2073 656c 662c 2064 783a 2066 6c6f 6174   self, dx: float
-0000bc40: 203d 2030 2c20 6479 3a20 666c 6f61 7420   = 0, dy: float 
-0000bc50: 3d20 302c 2064 7a3a 2066 6c6f 6174 203d  = 0, dz: float =
-0000bc60: 2030 0d0a 2020 2020 2920 2d3e 204e 6f6e   0..    ) -> Non
-0000bc70: 653a 0d0a 2020 2020 2020 2020 2222 2253  e:..        """S
-0000bc80: 6574 7320 7468 6520 7265 6c61 7469 7665  ets the relative
-0000bc90: 2058 595a 2070 6f73 6974 696f 6e20 696e   XYZ position in
-0000bca0: 206d 6963 726f 6e73 2e0d 0a0d 0a20 2020   microns.....   
-0000bcb0: 2020 2020 203a 7370 6172 6b6c 6573 3a20       :sparkles: 
-0000bcc0: 2a54 6869 7320 6d65 7468 6f64 2069 7320  *This method is 
-0000bcd0: 6e65 7720 696e 2060 434d 4d43 6f72 6550  new in `CMMCoreP
-0000bce0: 6c75 7360 2e2a 0d0a 0d0a 2020 2020 2020  lus`.*....      
-0000bcf0: 2020 5468 6973 2069 7320 6120 636f 6e76    This is a conv
-0000bd00: 656e 6965 6e63 6520 6d65 7468 6f64 2074  enience method t
-0000bd10: 6861 7420 6361 6c6c 7320 6073 6574 5859  hat calls `setXY
-0000bd20: 506f 7369 7469 6f6e 6020 616e 6420 6073  Position` and `s
-0000bd30: 6574 5a50 6f73 6974 696f 6e60 0d0a 2020  etZPosition`..  
-0000bd40: 2020 2020 2020 7769 7468 2074 6865 2063        with the c
-0000bd50: 7572 7265 6e74 2070 6f73 6974 696f 6e20  urrent position 
-0000bd60: 6173 2074 6865 2073 7461 7274 696e 6720  as the starting 
-0000bd70: 706f 696e 742e 0d0a 0d0a 2020 2020 2020  point.....      
-0000bd80: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-0000bd90: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000bda0: 0d0a 2020 2020 2020 2020 6478 203a 2066  ..        dx : f
-0000bdb0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0d0a  loat, optional..
-0000bdc0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000bdd0: 7265 6c61 7469 7665 2063 6861 6e67 6520  relative change 
-0000bde0: 696e 2058 2070 6f73 6974 696f 6e2c 2062  in X position, b
-0000bdf0: 7920 6465 6661 756c 7420 300d 0a20 2020  y default 0..   
-0000be00: 2020 2020 2064 7920 3a20 666c 6f61 742c       dy : float,
-0000be10: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-0000be20: 2020 2020 2020 2054 6865 2072 656c 6174         The relat
-0000be30: 6976 6520 6368 616e 6765 2069 6e20 5920  ive change in Y 
-0000be40: 706f 7369 7469 6f6e 2c20 6279 2064 6566  position, by def
-0000be50: 6175 6c74 2030 0d0a 2020 2020 2020 2020  ault 0..        
-0000be60: 647a 203a 2066 6c6f 6174 2c20 6f70 7469  dz : float, opti
-0000be70: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
-0000be80: 2020 5468 6520 7265 6c61 7469 7665 2063    The relative c
-0000be90: 6861 6e67 6520 696e 205a 2070 6f73 6974  hange in Z posit
-0000bea0: 696f 6e2c 2062 7920 6465 6661 756c 7420  ion, by default 
-0000beb0: 300d 0a20 2020 2020 2020 2022 2222 0d0a  0..        """..
-0000bec0: 2020 2020 2020 2020 6966 2064 7820 6f72          if dx or
-0000bed0: 2064 793a 0d0a 2020 2020 2020 2020 2020   dy:..          
-0000bee0: 2020 782c 2079 203d 2073 656c 662e 6765    x, y = self.ge
-0000bef0: 7458 506f 7369 7469 6f6e 2829 2c20 7365  tXPosition(), se
-0000bf00: 6c66 2e67 6574 5950 6f73 6974 696f 6e28  lf.getYPosition(
-0000bf10: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000bf20: 656c 662e 7365 7458 5950 6f73 6974 696f  elf.setXYPositio
-0000bf30: 6e28 7820 2b20 6478 2c20 7920 2b20 6479  n(x + dx, y + dy
-0000bf40: 290d 0a20 2020 2020 2020 2069 6620 647a  )..        if dz
-0000bf50: 3a0d 0a20 2020 2020 2020 2020 2020 207a  :..            z
-0000bf60: 203d 2073 656c 662e 6765 7450 6f73 6974   = self.getPosit
-0000bf70: 696f 6e28 7365 6c66 2e67 6574 466f 6375  ion(self.getFocu
-0000bf80: 7344 6576 6963 6528 2929 0d0a 2020 2020  sDevice())..    
-0000bf90: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000bfa0: 5a50 6f73 6974 696f 6e28 7a20 2b20 647a  ZPosition(z + dz
-0000bfb0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000bfc0: 7761 6974 466f 7244 6576 6963 6528 7365  waitForDevice(se
-0000bfd0: 6c66 2e67 6574 5859 5374 6167 6544 6576  lf.getXYStageDev
-0000bfe0: 6963 6528 2929 0d0a 2020 2020 2020 2020  ice())..        
-0000bff0: 7365 6c66 2e77 6169 7446 6f72 4465 7669  self.waitForDevi
-0000c000: 6365 2873 656c 662e 6765 7446 6f63 7573  ce(self.getFocus
-0000c010: 4465 7669 6365 2829 290d 0a0d 0a20 2020  Device())....   
-0000c020: 2064 6566 2067 6574 5a50 6f73 6974 696f   def getZPositio
-0000c030: 6e28 7365 6c66 2920 2d3e 2066 6c6f 6174  n(self) -> float
-0000c040: 3a0d 0a20 2020 2020 2020 2022 2222 4f62  :..        """Ob
-0000c050: 7461 696e 7320 7468 6520 6375 7272 656e  tains the curren
-0000c060: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
-0000c070: 6520 5a20 6178 6973 206f 6620 7468 6520  e Z axis of the 
-0000c080: 5a20 7374 6167 6520 696e 206d 6963 726f  Z stage in micro
-0000c090: 6e73 2e0d 0a0d 0a20 2020 2020 2020 203a  ns.....        :
-0000c0a0: 7370 6172 6b6c 6573 3a20 2a54 6869 7320  sparkles: *This 
-0000c0b0: 6d65 7468 6f64 2069 7320 6e65 7720 696e  method is new in
-0000c0c0: 2060 434d 4d43 6f72 6550 6c75 7360 3a0d   `CMMCorePlus`:.
-0000c0d0: 0a20 2020 2020 2020 2061 6464 6564 2074  .        added t
-0000c0e0: 6f20 636f 6d70 6c65 6d65 6e74 2060 6765  o complement `ge
-0000c0f0: 7458 506f 7369 7469 6f6e 6020 616e 6420  tXPosition` and 
-0000c100: 6067 6574 5950 6f73 6974 696f 6e60 2a0d  `getYPosition`*.
-0000c110: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000c120: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000c130: 662e 6765 7450 6f73 6974 696f 6e28 7365  f.getPosition(se
-0000c140: 6c66 2e67 6574 466f 6375 7344 6576 6963  lf.getFocusDevic
-0000c150: 6528 2929 0d0a 0d0a 2020 2020 6465 6620  e())....    def 
-0000c160: 7365 745a 506f 7369 7469 6f6e 2873 656c  setZPosition(sel
-0000c170: 662c 2076 616c 3a20 666c 6f61 7429 202d  f, val: float) -
-0000c180: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-0000c190: 2022 2222 5365 7420 7468 6520 706f 7369   """Set the posi
-0000c1a0: 7469 6f6e 206f 6620 7468 6520 6375 7272  tion of the curr
-0000c1b0: 656e 7420 666f 6375 7320 6465 7669 6365  ent focus device
-0000c1c0: 2069 6e20 6d69 6372 6f6e 732e 0d0a 0d0a   in microns.....
-0000c1d0: 2020 2020 2020 2020 3a73 7061 726b 6c65          :sparkle
-0000c1e0: 733a 202a 5468 6973 206d 6574 686f 6420  s: *This method 
-0000c1f0: 6973 206e 6577 2069 6e20 6043 4d4d 436f  is new in `CMMCo
-0000c200: 7265 506c 7573 603a 0d0a 2020 2020 2020  rePlus`:..      
-0000c210: 2020 6164 6465 6420 746f 2063 6f6d 706c    added to compl
-0000c220: 656d 656e 7420 6073 6574 5859 506f 7369  ement `setXYPosi
-0000c230: 7469 6f6e 602a 0d0a 2020 2020 2020 2020  tion`*..        
-0000c240: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-0000c250: 7572 6e20 7365 6c66 2e73 6574 506f 7369  urn self.setPosi
-0000c260: 7469 6f6e 2873 656c 662e 6765 7446 6f63  tion(self.getFoc
-0000c270: 7573 4465 7669 6365 2829 2c20 7661 6c29  usDevice(), val)
-0000c280: 0d0a 0d0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
-0000c290: 640d 0a20 2020 2064 6566 2073 6574 506f  d..    def setPo
-0000c2a0: 7369 7469 6f6e 2873 656c 662c 2070 6f73  sition(self, pos
-0000c2b0: 6974 696f 6e3a 2066 6c6f 6174 2920 2d3e  ition: float) ->
-0000c2c0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000c2d0: 2e2e 2e0d 0a0d 0a20 2020 2040 6f76 6572  .......    @over
-0000c2e0: 6c6f 6164 0d0a 2020 2020 6465 6620 7365  load..    def se
-0000c2f0: 7450 6f73 6974 696f 6e28 7365 6c66 2c20  tPosition(self, 
-0000c300: 7374 6167 654c 6162 656c 3a20 7374 722c  stageLabel: str,
-0000c310: 2070 6f73 6974 696f 6e3a 2066 6c6f 6174   position: float
-0000c320: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-0000c330: 2020 2020 2e2e 2e0d 0a0d 0a20 2020 2040      .......    @
-0000c340: 7379 6e63 6872 6f6e 697a 6564 285f 6c6f  synchronized(_lo
-0000c350: 636b 290d 0a20 2020 2064 6566 2073 6574  ck)..    def set
-0000c360: 506f 7369 7469 6f6e 2873 656c 662c 202a  Position(self, *
-0000c370: 6172 6773 3a20 416e 792c 202a 2a6b 7761  args: Any, **kwa
-0000c380: 7267 733a 2041 6e79 2920 2d3e 204e 6f6e  rgs: Any) -> Non
-0000c390: 653a 0d0a 2020 2020 2020 2020 2222 2253  e:..        """S
-0000c3a0: 6574 2070 6f73 6974 696f 6e20 6f66 2074  et position of t
-0000c3b0: 6865 2073 7461 6765 2069 6e20 6d69 6372  he stage in micr
-0000c3c0: 6f6e 732e 0d0a 0d0a 2020 2020 2020 2020  ons.....        
-0000c3d0: 2a2a 5768 7920 4f76 6572 7269 6465 3f2a  **Why Override?*
-0000c3e0: 2a20 546f 2061 6464 2061 206c 6f63 6b20  * To add a lock 
-0000c3f0: 746f 2070 7265 7665 6e74 2063 6f6e 6375  to prevent concu
-0000c400: 7272 656e 7420 6361 6c6c 7320 6163 726f  rrent calls acro
-0000c410: 7373 2074 6872 6561 6473 2e0d 0a20 2020  ss threads...   
-0000c420: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000c430: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-0000c440: 2e73 6574 506f 7369 7469 6f6e 282a 6172  .setPosition(*ar
-0000c450: 6773 2c20 2a2a 6b77 6172 6773 290d 0a0d  gs, **kwargs)...
-0000c460: 0a20 2020 2040 6f76 6572 6c6f 6164 0d0a  .    @overload..
-0000c470: 2020 2020 6465 6620 7365 7458 5950 6f73      def setXYPos
-0000c480: 6974 696f 6e28 7365 6c66 2c20 783a 2066  ition(self, x: f
-0000c490: 6c6f 6174 2c20 793a 2066 6c6f 6174 2920  loat, y: float) 
-0000c4a0: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-0000c4b0: 2020 2e2e 2e0d 0a0d 0a20 2020 2040 6f76    .......    @ov
-0000c4c0: 6572 6c6f 6164 0d0a 2020 2020 6465 6620  erload..    def 
-0000c4d0: 7365 7458 5950 6f73 6974 696f 6e28 7365  setXYPosition(se
-0000c4e0: 6c66 2c20 7879 5374 6167 654c 6162 656c  lf, xyStageLabel
-0000c4f0: 3a20 7374 722c 2078 3a20 666c 6f61 742c  : str, x: float,
-0000c500: 2079 3a20 666c 6f61 7429 202d 3e20 4e6f   y: float) -> No
-0000c510: 6e65 3a0d 0a20 2020 2020 2020 202e 2e2e  ne:..        ...
-0000c520: 0d0a 0d0a 2020 2020 4073 796e 6368 726f  ....    @synchro
-0000c530: 6e69 7a65 6428 5f6c 6f63 6b29 0d0a 2020  nized(_lock)..  
-0000c540: 2020 6465 6620 7365 7458 5950 6f73 6974    def setXYPosit
-0000c550: 696f 6e28 7365 6c66 2c20 2a61 7267 733a  ion(self, *args:
-0000c560: 2041 6e79 2c20 2a2a 6b77 6172 6773 3a20   Any, **kwargs: 
-0000c570: 416e 7929 202d 3e20 4e6f 6e65 3a0d 0a20  Any) -> None:.. 
-0000c580: 2020 2020 2020 2022 2222 5365 7473 2074         """Sets t
-0000c590: 6865 2070 6f73 6974 696f 6e20 6f66 2074  he position of t
-0000c5a0: 6865 2058 5920 7374 6167 6520 696e 206d  he XY stage in m
-0000c5b0: 6963 726f 6e73 2e0d 0a0d 0a20 2020 2020  icrons.....     
-0000c5c0: 2020 202a 2a57 6879 204f 7665 7272 6964     **Why Overrid
-0000c5d0: 653f 2a2a 2054 6f20 6164 6420 6120 6c6f  e?** To add a lo
-0000c5e0: 636b 2074 6f20 7072 6576 656e 7420 636f  ck to prevent co
-0000c5f0: 6e63 7572 7265 6e74 2063 616c 6c73 2061  ncurrent calls a
-0000c600: 6372 6f73 7320 7468 7265 6164 732e 0d0a  cross threads...
-0000c610: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000c620: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-0000c630: 7228 292e 7365 7458 5950 6f73 6974 696f  r().setXYPositio
-0000c640: 6e28 2a61 7267 732c 202a 2a6b 7761 7267  n(*args, **kwarg
-0000c650: 7329 0d0a 0d0a 2020 2020 4073 796e 6368  s)....    @synch
-0000c660: 726f 6e69 7a65 6428 5f6c 6f63 6b29 0d0a  ronized(_lock)..
-0000c670: 2020 2020 6465 6620 6765 7443 616d 6572      def getCamer
-0000c680: 6143 6861 6e6e 656c 4e61 6d65 7328 7365  aChannelNames(se
-0000c690: 6c66 2920 2d3e 2074 7570 6c65 5b73 7472  lf) -> tuple[str
-0000c6a0: 2c20 2e2e 2e5d 3a0d 0a20 2020 2020 2020  , ...]:..       
-0000c6b0: 2022 2222 436f 6e76 656e 6965 6e63 6520   """Convenience 
-0000c6c0: 6d65 7468 6f64 2074 6f20 6361 6c6c 2060  method to call `
-0000c6d0: 6765 7443 616d 6572 6143 6861 6e6e 656c  getCameraChannel
-0000c6e0: 4e61 6d65 6020 666f 7220 616c 6c20 6361  Name` for all ca
-0000c6f0: 6d65 7261 2063 6861 6e6e 656c 732e 0d0a  mera channels...
-0000c700: 0d0a 2020 2020 2020 2020 3a73 7061 726b  ..        :spark
-0000c710: 6c65 733a 202a 5468 6973 206d 6574 686f  les: *This metho
-0000c720: 6420 6973 206e 6577 2069 6e20 6043 4d4d  d is new in `CMM
-0000c730: 436f 7265 506c 7573 602e 2a0d 0a20 2020  CorePlus`.*..   
-0000c740: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000c750: 2020 7265 7475 726e 2074 7570 6c65 280d    return tuple(.
-0000c760: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c770: 662e 6765 7443 616d 6572 6143 6861 6e6e  f.getCameraChann
-0000c780: 656c 4e61 6d65 2869 290d 0a20 2020 2020  elName(i)..     
-0000c790: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0000c7a0: 7261 6e67 6528 7365 6c66 2e67 6574 4e75  range(self.getNu
-0000c7b0: 6d62 6572 4f66 4361 6d65 7261 4368 616e  mberOfCameraChan
-0000c7c0: 6e65 6c73 2829 290d 0a20 2020 2020 2020  nels())..       
-0000c7d0: 2029 0d0a 0d0a 2020 2020 4073 796e 6368   )....    @synch
-0000c7e0: 726f 6e69 7a65 6428 5f6c 6f63 6b29 0d0a  ronized(_lock)..
-0000c7f0: 2020 2020 6465 6620 736e 6170 496d 6167      def snapImag
-0000c800: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-0000c810: 0d0a 2020 2020 2020 2020 2222 2241 6371  ..        """Acq
-0000c820: 7569 7265 7320 6120 7369 6e67 6c65 2069  uires a single i
-0000c830: 6d61 6765 2077 6974 6820 6375 7272 656e  mage with curren
-0000c840: 7420 7365 7474 696e 6773 2e0d 0a0d 0a20  t settings..... 
-0000c850: 2020 2020 2020 202a 2a57 6879 204f 7665         **Why Ove
-0000c860: 7272 6964 653f 2a2a 2054 6f20 6164 6420  rride?** To add 
-0000c870: 6120 6c6f 636b 2074 6f20 7072 6576 656e  a lock to preven
-0000c880: 7420 636f 6e63 7572 7265 6e74 2063 616c  t concurrent cal
-0000c890: 6c73 2061 6372 6f73 7320 7468 7265 6164  ls across thread
-0000c8a0: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
-0000c8b0: 0a20 2020 2020 2020 2061 7574 6f73 6875  .        autoshu
-0000c8c0: 7474 6572 203d 2073 656c 662e 6765 7441  tter = self.getA
-0000c8d0: 7574 6f53 6875 7474 6572 2829 0d0a 2020  utoShutter()..  
-0000c8e0: 2020 2020 2020 6966 2061 7574 6f73 6875        if autoshu
-0000c8f0: 7474 6572 3a0d 0a20 2020 2020 2020 2020  tter:..         
-0000c900: 2020 2073 656c 662e 6576 656e 7473 2e70     self.events.p
-0000c910: 726f 7065 7274 7943 6861 6e67 6564 2e65  ropertyChanged.e
-0000c920: 6d69 7428 7365 6c66 2e67 6574 5368 7574  mit(self.getShut
-0000c930: 7465 7244 6576 6963 6528 292c 2022 5374  terDevice(), "St
-0000c940: 6174 6522 2c20 5472 7565 290d 0a20 2020  ate", True)..   
-0000c950: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-0000c960: 2020 2020 2020 2073 7570 6572 2829 2e73         super().s
-0000c970: 6e61 7049 6d61 6765 2829 0d0a 2020 2020  napImage()..    
-0000c980: 2020 2020 6669 6e61 6c6c 793a 0d0a 2020      finally:..  
-0000c990: 2020 2020 2020 2020 2020 6966 2061 7574            if aut
-0000c9a0: 6f73 6875 7474 6572 3a0d 0a20 2020 2020  oshutter:..     
-0000c9b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c9c0: 6576 656e 7473 2e70 726f 7065 7274 7943  events.propertyC
-0000c9d0: 6861 6e67 6564 2e65 6d69 7428 0d0a 2020  hanged.emit(..  
-0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9f0: 2020 7365 6c66 2e67 6574 5368 7574 7465    self.getShutte
-0000ca00: 7244 6576 6963 6528 292c 2022 5374 6174  rDevice(), "Stat
-0000ca10: 6522 2c20 4661 6c73 650d 0a20 2020 2020  e", False..     
-0000ca20: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
-0000ca30: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-0000ca40: 2020 2064 6566 206d 6461 2873 656c 6629     def mda(self)
-0000ca50: 202d 3e20 4d44 4152 756e 6e65 723a 0d0a   -> MDARunner:..
-0000ca60: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-0000ca70: 6e20 7468 6520 604d 4441 5275 6e6e 6572  n the `MDARunner
-0000ca80: 6020 666f 7220 7468 6973 2060 434d 4d43  ` for this `CMMC
-0000ca90: 6f72 6550 6c75 7360 2069 6e73 7461 6e63  orePlus` instanc
-0000caa0: 652e 0d0a 0d0a 2020 2020 2020 2020 3a73  e.....        :s
-0000cab0: 7061 726b 6c65 733a 202a 5468 6973 206d  parkles: *This m
-0000cac0: 6574 686f 6420 6973 206e 6577 2069 6e20  ethod is new in 
-0000cad0: 6043 4d4d 436f 7265 506c 7573 602e 2a0d  `CMMCorePlus`.*.
-0000cae0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000caf0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000cb00: 662e 5f6d 6461 5f72 756e 6e65 720d 0a0d  f._mda_runner...
-0000cb10: 0a20 2020 2064 6566 2072 756e 5f6d 6461  .    def run_mda
-0000cb20: 2873 656c 662c 2065 7665 6e74 733a 2049  (self, events: I
-0000cb30: 7465 7261 626c 655b 4d44 4145 7665 6e74  terable[MDAEvent
-0000cb40: 5d2c 2062 6c6f 636b 3a20 626f 6f6c 203d  ], block: bool =
-0000cb50: 2046 616c 7365 2920 2d3e 2054 6872 6561   False) -> Threa
-0000cb60: 643a 0d0a 2020 2020 2020 2020 2222 2252  d:..        """R
-0000cb70: 756e 2061 2073 6571 7565 6e63 6520 6f66  un a sequence of
-0000cb80: 205b 7573 6571 2e4d 4441 4576 656e 745d   [useq.MDAEvent]
-0000cb90: 5b5d 206f 6e20 6120 6e65 7720 7468 7265  [] on a new thre
-0000cba0: 6164 2e0d 0a0d 0a20 2020 2020 2020 203a  ad.....        :
-0000cbb0: 7370 6172 6b6c 6573 3a20 2a54 6869 7320  sparkles: *This 
-0000cbc0: 6d65 7468 6f64 2069 7320 6e65 7720 696e  method is new in
-0000cbd0: 2060 434d 4d43 6f72 6550 6c75 7360 2e2a   `CMMCorePlus`.*
-0000cbe0: 0d0a 0d0a 2020 2020 2020 2020 5468 6520  ....        The 
-0000cbf0: 6375 7272 656e 746c 7920 7265 6769 7374  currently regist
-0000cc00: 6572 6564 204d 4441 456e 6769 6e65 2028  ered MDAEngine (
-0000cc10: 6063 6f72 652e 6d64 612e 656e 6769 6e65  `core.mda.engine
-0000cc20: 6029 2077 696c 6c20 6265 2072 6573 706f  `) will be respo
-0000cc30: 6e73 6962 6c65 2066 6f72 0d0a 2020 2020  nsible for..    
-0000cc40: 2020 2020 6578 6563 7574 696e 6720 7468      executing th
-0000cc50: 6520 6163 7175 6973 6974 696f 6e2e 0d0a  e acquisition...
-0000cc60: 0d0a 2020 2020 2020 2020 4166 7465 7220  ..        After 
-0000cc70: 7374 6172 7469 6e67 2074 6865 2073 6571  starting the seq
-0000cc80: 7565 6e63 6520 796f 7520 6361 6e20 7061  uence you can pa
-0000cc90: 7573 6520 6f72 2063 616e 6365 6c20 7769  use or cancel wi
-0000cca0: 7468 2074 6865 206d 6461 2077 6974 680d  th the mda with.
-0000ccb0: 0a20 2020 2020 2020 2074 6865 206d 6461  .        the mda
-0000ccc0: 206f 626a 6563 7427 7320 6074 6f67 676c   object's `toggl
-0000ccd0: 655f 7061 7573 6560 2061 6e64 2060 6361  e_pause` and `ca
-0000cce0: 6e63 656c 6020 6d65 7468 6f64 732e 0d0a  ncel` methods...
-0000ccf0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000cd00: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-0000cd10: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-0000cd20: 2020 6576 656e 7473 203a 2049 7465 7261    events : Itera
-0000cd30: 626c 655b 7573 6571 2e4d 4441 4576 656e  ble[useq.MDAEven
-0000cd40: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
-0000cd50: 416e 2069 7465 7261 626c 6520 6f66 205b  An iterable of [
-0000cd60: 7573 6571 2e4d 4441 4576 656e 745d 5b5d  useq.MDAEvent][]
-0000cd70: 2074 6f20 6578 6563 7574 652e 2020 5468   to execute.  Th
-0000cd80: 6973 206d 6179 2062 6520 616e 2069 6e73  is may be an ins
-0000cd90: 7461 6e63 650d 0a20 2020 2020 2020 2020  tance..         
-0000cda0: 2020 206f 6620 5b75 7365 712e 4d44 4153     of [useq.MDAS
-0000cdb0: 6571 7565 6e63 655d 5b5d 2c20 6f72 2061  equence][], or a
-0000cdc0: 6e79 206f 7468 6572 2069 7465 7261 626c  ny other iterabl
-0000cdd0: 6520 6f66 205b 7573 6571 2e4d 4441 4576  e of [useq.MDAEv
-0000cde0: 656e 745d 5b5d 2e0d 0a20 2020 2020 2020  ent][]...       
-0000cdf0: 2062 6c6f 636b 203a 2062 6f6f 6c2c 206f   block : bool, o
-0000ce00: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-0000ce10: 2020 2020 2049 6620 5472 7565 2c20 626c       If True, bl
-0000ce20: 6f63 6b20 756e 7469 6c20 7468 6520 7365  ock until the se
-0000ce30: 7175 656e 6365 2069 7320 636f 6d70 6c65  quence is comple
-0000ce40: 7465 2c20 6279 2064 6566 6175 6c74 2046  te, by default F
-0000ce50: 616c 7365 2e0d 0a0d 0a20 2020 2020 2020  alse.....       
-0000ce60: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-0000ce70: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-0000ce80: 2020 2054 6872 6561 640d 0a20 2020 2020     Thread..     
-0000ce90: 2020 2020 2020 2054 6865 2074 6872 6561         The threa
-0000cea0: 6420 7468 6520 7365 7175 656e 6365 2069  d the sequence i
-0000ceb0: 7320 7275 6e6e 696e 6720 6f6e 2e20 2055  s running on.  U
-0000cec0: 7365 2060 7468 7265 6164 2e6a 6f69 6e28  se `thread.join(
-0000ced0: 2960 2074 6f20 626c 6f63 6b20 756e 7469  )` to block unti
-0000cee0: 6c0d 0a20 2020 2020 2020 2020 2020 2064  l..            d
-0000cef0: 6f6e 652c 206f 7220 6074 6872 6561 642e  one, or `thread.
-0000cf00: 6973 5f61 6c69 7665 2829 6020 746f 2063  is_alive()` to c
-0000cf10: 6865 636b 2069 6620 7468 6520 7365 7175  heck if the sequ
-0000cf20: 656e 6365 2069 7320 636f 6d70 6c65 7465  ence is complete
-0000cf30: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-0000cf40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000cf50: 6d64 612e 6973 5f72 756e 6e69 6e67 2829  mda.is_running()
-0000cf60: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0000cf70: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000cf80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cf90: 2020 2243 616e 6e6f 7420 7374 6172 7420    "Cannot start 
-0000cfa0: 616e 204d 4441 2077 6869 6c65 2074 6865  an MDA while the
-0000cfb0: 2070 7265 7669 6f75 7320 4d44 4120 6973   previous MDA is
-0000cfc0: 2073 7469 6c6c 2072 756e 6e69 6e67 2e22   still running."
-0000cfd0: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-0000cfe0: 0a20 2020 2020 2020 2074 6820 3d20 5468  .        th = Th
-0000cff0: 7265 6164 2874 6172 6765 743d 7365 6c66  read(target=self
-0000d000: 2e6d 6461 2e72 756e 2c20 6172 6773 3d28  .mda.run, args=(
-0000d010: 6576 656e 7473 2c29 290d 0a20 2020 2020  events,))..     
-0000d020: 2020 2074 682e 7374 6172 7428 290d 0a20     th.start().. 
-0000d030: 2020 2020 2020 2069 6620 626c 6f63 6b3a         if block:
-0000d040: 0d0a 2020 2020 2020 2020 2020 2020 7468  ..            th
-0000d050: 2e6a 6f69 6e28 290d 0a20 2020 2020 2020  .join()..       
-0000d060: 2072 6574 7572 6e20 7468 0d0a 0d0a 2020   return th....  
-0000d070: 2020 6465 6620 7265 6769 7374 6572 5f6d    def register_m
-0000d080: 6461 5f65 6e67 696e 6528 7365 6c66 2c20  da_engine(self, 
-0000d090: 656e 6769 6e65 3a20 504d 4441 456e 6769  engine: PMDAEngi
-0000d0a0: 6e65 2920 2d3e 204e 6f6e 653a 0d0a 2020  ne) -> None:..  
-0000d0b0: 2020 2020 2020 2222 2253 6574 2074 6865        """Set the
-0000d0c0: 204d 4441 2045 6e67 696e 6520 746f 2062   MDA Engine to b
-0000d0d0: 6520 7573 6564 206f 6e20 6072 756e 5f6d  e used on `run_m
-0000d0e0: 6461 602e 0d0a 0d0a 2020 2020 2020 2020  da`.....        
-0000d0f0: 3a73 7061 726b 6c65 733a 202a 5468 6973  :sparkles: *This
-0000d100: 206d 6574 686f 6420 6973 206e 6577 2069   method is new i
-0000d110: 6e20 6043 4d4d 436f 7265 506c 7573 602e  n `CMMCorePlus`.
-0000d120: 2a0d 0a0d 0a20 2020 2020 2020 2054 6869  *....        Thi
-0000d130: 7320 7769 6c6c 2075 6e72 6567 6973 7465  s will unregiste
-0000d140: 7220 7468 6520 7072 6576 696f 7573 2065  r the previous e
-0000d150: 6e67 696e 6520 616e 6420 656d 6974 2061  ngine and emit a
-0000d160: 6e20 606d 6461 456e 6769 6e65 5265 6769  n `mdaEngineRegi
-0000d170: 7374 6572 6564 600d 0a20 2020 2020 2020  stered`..       
-0000d180: 2073 6967 6e61 6c2e 2054 6865 2063 7572   signal. The cur
-0000d190: 7265 6e74 2045 6e67 696e 6520 6d75 7374  rent Engine must
-0000d1a0: 206e 6f74 2062 6520 7275 6e6e 696e 6720   not be running 
-0000d1b0: 616e 204d 4441 2069 6e20 6f72 6465 7220  an MDA in order 
-0000d1c0: 746f 2072 6567 6973 7465 7220 6120 6e65  to register a ne
-0000d1d0: 770d 0a20 2020 2020 2020 2065 6e67 696e  w..        engin
-0000d1e0: 652e 0d0a 0d0a 2020 2020 2020 2020 5061  e.....        Pa
-0000d1f0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-0000d200: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-0000d210: 2020 2020 2020 656e 6769 6e65 203a 2050        engine : P
-0000d220: 4d44 4145 6e67 696e 650d 0a20 2020 2020  MDAEngine..     
-0000d230: 2020 2020 2020 2041 6e79 206f 626a 6563         Any objec
-0000d240: 7420 636f 6e66 6f72 6d69 6e67 2074 6f20  t conforming to 
-0000d250: 7468 6520 504d 4441 456e 6769 6e65 2070  the PMDAEngine p
-0000d260: 726f 746f 636f 6c2e 0d0a 2020 2020 2020  rotocol...      
-0000d270: 2020 2222 220d 0a20 2020 2020 2020 206f    """..        o
-0000d280: 6c64 5f65 6e67 696e 6520 3d20 7365 6c66  ld_engine = self
-0000d290: 2e6d 6461 2e73 6574 5f65 6e67 696e 6528  .mda.set_engine(
-0000d2a0: 656e 6769 6e65 290d 0a20 2020 2020 2020  engine)..       
-0000d2b0: 2073 656c 662e 6576 656e 7473 2e6d 6461   self.events.mda
-0000d2c0: 456e 6769 6e65 5265 6769 7374 6572 6564  EngineRegistered
-0000d2d0: 2e65 6d69 7428 656e 6769 6e65 2c20 6f6c  .emit(engine, ol
-0000d2e0: 645f 656e 6769 6e65 290d 0a0d 0a20 2020  d_engine)....   
-0000d2f0: 2064 6566 2066 6978 496d 6167 6528 7365   def fixImage(se
-0000d300: 6c66 2c20 696d 673a 206e 702e 6e64 6172  lf, img: np.ndar
-0000d310: 7261 792c 206e 636f 6d70 6f6e 656e 7473  ray, ncomponents
-0000d320: 3a20 696e 7420 7c20 4e6f 6e65 203d 204e  : int | None = N
-0000d330: 6f6e 6529 202d 3e20 6e70 2e6e 6461 7272  one) -> np.ndarr
-0000d340: 6179 3a0d 0a20 2020 2020 2020 2022 2222  ay:..        """
-0000d350: 4669 7820 696d 6720 7368 6170 652f 6474  Fix img shape/dt
-0000d360: 7970 6520 6261 7365 6420 6f6e 2060 7365  ype based on `se
-0000d370: 6c66 2e67 6574 4e75 6d62 6572 4f66 436f  lf.getNumberOfCo
-0000d380: 6d70 6f6e 656e 7473 2829 602e 0d0a 0d0a  mponents()`.....
-0000d390: 2020 2020 2020 2020 3a73 7061 726b 6c65          :sparkle
-0000d3a0: 733a 202a 5468 6973 206d 6574 686f 6420  s: *This method 
-0000d3b0: 6973 206e 6577 2069 6e20 6043 4d4d 436f  is new in `CMMCo
-0000d3c0: 7265 506c 7573 602e 2a0d 0a0d 0a20 2020  rePlus`.*....   
-0000d3d0: 2020 2020 2063 6f6e 7665 7274 2069 6d61       convert ima
-0000d3e0: 6765 7320 7769 7468 206e 5f63 6f6d 706f  ges with n_compo
-0000d3f0: 6e65 6e74 7320 3e20 310d 0a20 2020 2020  nents > 1..     
-0000d400: 2020 2074 6f20 6120 7368 6170 6520 2877     to a shape (w
-0000d410: 2c20 682c 206e 756d 5f63 6f6d 706f 6e65  , h, num_compone
-0000d420: 6e74 7329 2061 6e64 2064 7479 7065 2060  nts) and dtype `
-0000d430: 696d 672e 6474 7970 652e 6974 656d 7369  img.dtype.itemsi
-0000d440: 7a65 2f2f 6e63 6f6d 7060 0d0a 0d0a 2020  ze//ncomp`....  
-0000d450: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000d460: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-0000d470: 2d2d 2d2d 0d0a 2020 2020 2020 2020 696d  ----..        im
-0000d480: 6720 3a20 6e70 2e6e 6461 7272 6179 0d0a  g : np.ndarray..
-0000d490: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-0000d4a0: 7420 696d 6167 650d 0a20 2020 2020 2020  t image..       
-0000d4b0: 206e 636f 6d70 6f6e 656e 7473 203a 2069   ncomponents : i
-0000d4c0: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
-0000d4d0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-0000d4e0: 206f 6620 636f 6d70 6f6e 656e 7473 2069   of components i
-0000d4f0: 6e20 7468 6520 696d 6167 652c 2062 7920  n the image, by 
-0000d500: 6465 6661 756c 7420 6073 656c 662e 6765  default `self.ge
-0000d510: 744e 756d 6265 724f 6643 6f6d 706f 6e65  tNumberOfCompone
-0000d520: 6e74 7328 2960 0d0a 0d0a 2020 2020 2020  nts()`....      
-0000d530: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
-0000d540: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-0000d550: 2020 2020 6e70 2e6e 6461 7272 6179 0d0a      np.ndarray..
-0000d560: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-0000d570: 7574 2069 6d61 6765 2028 706f 7373 6962  ut image (possib
-0000d580: 6c79 206e 6577 2073 6861 7065 2061 6e64  ly new shape and
-0000d590: 2064 7479 7065 290d 0a20 2020 2020 2020   dtype)..       
-0000d5a0: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
-0000d5b0: 206e 636f 6d70 6f6e 656e 7473 2069 7320   ncomponents is 
-0000d5c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000d5d0: 2020 206e 636f 6d70 6f6e 656e 7473 203d     ncomponents =
-0000d5e0: 2073 656c 662e 6765 744e 756d 6265 724f   self.getNumberO
-0000d5f0: 6643 6f6d 706f 6e65 6e74 7328 290d 0a20  fComponents().. 
-0000d600: 2020 2020 2020 2069 6620 6e63 6f6d 706f         if ncompo
-0000d610: 6e65 6e74 7320 3d3d 2034 3a0d 0a20 2020  nents == 4:..   
-0000d620: 2020 2020 2020 2020 206e 6577 5f73 6861           new_sha
-0000d630: 7065 203d 2028 2a69 6d67 2e73 6861 7065  pe = (*img.shape
-0000d640: 2c20 3429 0d0a 2020 2020 2020 2020 2020  , 4)..          
-0000d650: 2020 696d 6720 3d20 696d 672e 7669 6577    img = img.view
-0000d660: 2864 7479 7065 3d66 2275 7b69 6d67 2e64  (dtype=f"u{img.d
-0000d670: 7479 7065 2e69 7465 6d73 697a 652f 2f34  type.itemsize//4
-0000d680: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
-0000d690: 2069 6d67 203d 2069 6d67 2e72 6573 6861   img = img.resha
-0000d6a0: 7065 286e 6577 5f73 6861 7065 295b 3a2c  pe(new_shape)[:,
-0000d6b0: 203a 2c20 2832 2c20 312c 2030 2c20 3329   :, (2, 1, 0, 3)
-0000d6c0: 5d20 2023 206d 6d63 6f72 6520 6769 7665  ]  # mmcore give
-0000d6d0: 7320 6267 7261 0d0a 2020 2020 2020 2020  s bgra..        
-0000d6e0: 7265 7475 726e 2069 6d67 0d0a 0d0a 2020  return img....  
-0000d6f0: 2020 6465 6620 736e 6170 2873 656c 662c    def snap(self,
-0000d700: 206e 756d 4368 616e 6e65 6c3a 2069 6e74   numChannel: int
-0000d710: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c20   | None = None, 
-0000d720: 2a2c 2066 6978 3a20 626f 6f6c 203d 2054  *, fix: bool = T
-0000d730: 7275 6529 202d 3e20 6e70 2e6e 6461 7272  rue) -> np.ndarr
-0000d740: 6179 3a0d 0a20 2020 2020 2020 2022 2222  ay:..        """
-0000d750: 536e 6170 2061 6e64 2072 6574 7572 6e20  Snap and return 
-0000d760: 616e 2069 6d61 6765 2e0d 0a0d 0a20 2020  an image.....   
-0000d770: 2020 2020 203a 7370 6172 6b6c 6573 3a20       :sparkles: 
-0000d780: 2a54 6869 7320 6d65 7468 6f64 2069 7320  *This method is 
-0000d790: 6e65 7720 696e 2060 434d 4d43 6f72 6550  new in `CMMCoreP
-0000d7a0: 6c75 7360 2e2a 0d0a 0d0a 2020 2020 2020  lus`.*....      
-0000d7b0: 2020 436f 6e76 656e 6965 6e63 6520 666f    Convenience fo
-0000d7c0: 7220 6361 6c6c 696e 6720 6073 656c 662e  r calling `self.
-0000d7d0: 736e 6170 496d 6167 6528 2960 2066 6f6c  snapImage()` fol
-0000d7e0: 6c6f 7765 6420 6279 2072 6574 7572 6e69  lowed by returni
-0000d7f0: 6e67 2074 6865 2076 616c 7565 0d0a 2020  ng the value..  
-0000d800: 2020 2020 2020 6f66 2060 7365 6c66 2e67        of `self.g
-0000d810: 6574 496d 6167 6528 2960 2e0d 0a0d 0a20  etImage()`..... 
-0000d820: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000d830: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-0000d840: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 206e  -----..        n
-0000d850: 756d 4368 616e 6e65 6c20 3a20 696e 742c  umChannel : int,
-0000d860: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-0000d870: 2020 2020 2020 2054 6865 2063 616d 6572         The camer
-0000d880: 6120 6368 616e 6e65 6c20 746f 2067 6574  a channel to get
-0000d890: 2074 6865 2069 6d61 6765 2066 726f 6d2e   the image from.
-0000d8a0: 2020 4966 204e 6f6e 652c 2028 7468 6520    If None, (the 
-0000d8b0: 6465 6661 756c 7429 2c20 7468 656e 0d0a  default), then..
-0000d8c0: 2020 2020 2020 2020 2020 2020 4d75 6c74              Mult
-0000d8d0: 692d 4368 616e 6e65 6c20 6361 6d65 7261  i-Channel camera
-0000d8e0: 7320 7769 6c6c 2072 6574 7572 6e20 7468  s will return th
-0000d8f0: 6520 636f 6e74 656e 7420 6f66 2074 6865  e content of the
-0000d900: 2066 6972 7374 2063 6861 6e6e 656c 2e0d   first channel..
-0000d910: 0a20 2020 2020 2020 2066 6978 203a 2062  .        fix : b
-0000d920: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-0000d930: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-0000d940: 4966 2060 5472 7565 6020 2874 6865 2064  If `True` (the d
-0000d950: 6566 6175 6c74 292c 2074 6865 6e20 696d  efault), then im
-0000d960: 6167 6573 2077 6974 6820 6e5f 636f 6d70  ages with n_comp
-0000d970: 6f6e 656e 7473 203e 2031 2028 6c69 6b65  onents > 1 (like
-0000d980: 2052 4742 2069 6d61 6765 7329 0d0a 2020   RGB images)..  
-0000d990: 2020 2020 2020 2020 2020 7769 6c6c 2062            will b
-0000d9a0: 6520 7265 7368 6170 6564 2074 6f20 2877  e reshaped to (w
-0000d9b0: 2c20 682c 206e 5f63 6f6d 706f 6e65 6e74  , h, n_component
-0000d9c0: 7329 2075 7369 6e67 2060 6669 7849 6d61  s) using `fixIma
-0000d9d0: 6765 602e 0d0a 0d0a 2020 2020 2020 2020  ge`.....        
-0000d9e0: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
-0000d9f0: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-0000da00: 2020 696d 6720 3a20 6e70 2e6e 6461 7272    img : np.ndarr
-0000da10: 6179 0d0a 2020 2020 2020 2020 2222 220d  ay..        """.
-0000da20: 0a20 2020 2020 2020 2073 656c 662e 736e  .        self.sn
-0000da30: 6170 496d 6167 6528 290d 0a20 2020 2020  apImage()..     
-0000da40: 2020 2069 6d67 203d 2073 656c 662e 6765     img = self.ge
-0000da50: 7449 6d61 6765 286e 756d 4368 616e 6e65  tImage(numChanne
-0000da60: 6c2c 2066 6978 3d66 6978 2920 2023 2074  l, fix=fix)  # t
-0000da70: 7970 653a 2069 676e 6f72 650d 0a20 2020  ype: ignore..   
-0000da80: 2020 2020 2073 656c 662e 6576 656e 7473       self.events
-0000da90: 2e69 6d61 6765 536e 6170 7065 642e 656d  .imageSnapped.em
-0000daa0: 6974 2869 6d67 290d 0a20 2020 2020 2020  it(img)..       
-0000dab0: 2072 6574 7572 6e20 696d 670d 0a0d 0a20   return img.... 
-0000dac0: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
-0000dad0: 2020 6465 6620 6765 7449 6d61 6765 2873    def getImage(s
-0000dae0: 656c 662c 202a 2c20 6669 783a 2062 6f6f  elf, *, fix: boo
-0000daf0: 6c20 3d20 5472 7565 2920 2d3e 206e 702e  l = True) -> np.
-0000db00: 6e64 6172 7261 793a 0d0a 2020 2020 2020  ndarray:..      
-0000db10: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
-0000db20: 696e 7465 726e 616c 2069 6d61 6765 2062  internal image b
-0000db30: 7566 6665 722e 2222 220d 0a0d 0a20 2020  uffer."""....   
-0000db40: 2040 6f76 6572 6c6f 6164 0d0a 2020 2020   @overload..    
-0000db50: 6465 6620 6765 7449 6d61 6765 2873 656c  def getImage(sel
-0000db60: 662c 206e 756d 4368 616e 6e65 6c3a 2069  f, numChannel: i
-0000db70: 6e74 2c20 2a2c 2066 6978 3a20 626f 6f6c  nt, *, fix: bool
-0000db80: 203d 2054 7275 6529 202d 3e20 6e70 2e6e   = True) -> np.n
-0000db90: 6461 7272 6179 3a0d 0a20 2020 2020 2020  darray:..       
-0000dba0: 2022 2222 5265 7475 726e 2074 6865 2069   """Return the i
-0000dbb0: 6e74 6572 6e61 6c20 696d 6167 6520 6275  nternal image bu
-0000dbc0: 6666 6572 2066 6f72 2061 2067 6976 656e  ffer for a given
-0000dbd0: 2043 616d 6572 6120 4368 616e 6e65 6c22   Camera Channel"
-0000dbe0: 2222 0d0a 0d0a 2020 2020 6465 6620 6765  ""....    def ge
-0000dbf0: 7449 6d61 6765 280d 0a20 2020 2020 2020  tImage(..       
-0000dc00: 2073 656c 662c 206e 756d 4368 616e 6e65   self, numChanne
-0000dc10: 6c3a 2069 6e74 207c 204e 6f6e 6520 3d20  l: int | None = 
-0000dc20: 4e6f 6e65 2c20 2a2c 2066 6978 3a20 626f  None, *, fix: bo
-0000dc30: 6f6c 203d 2054 7275 650d 0a20 2020 2029  ol = True..    )
-0000dc40: 202d 3e20 6e70 2e6e 6461 7272 6179 3a0d   -> np.ndarray:.
-0000dc50: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000dc60: 726e 2074 6865 2069 6e74 6572 6e61 6c20  rn the internal 
-0000dc70: 696d 6167 6520 6275 6666 6572 2e0d 0a0d  image buffer....
-0000dc80: 0a20 2020 2020 2020 202a 2a57 6879 204f  .        **Why O
-0000dc90: 7665 7272 6964 653f 2a2a 2054 6f20 6669  verride?** To fi
-0000dca0: 7820 7468 6520 7368 6170 6520 6f66 2069  x the shape of i
-0000dcb0: 6d61 6765 7320 7769 7468 206e 5f63 6f6d  mages with n_com
-0000dcc0: 706f 6e65 6e74 7320 3e20 3120 286c 696b  ponents > 1 (lik
-0000dcd0: 6520 5247 420d 0a20 2020 2020 2020 2069  e RGB..        i
-0000dce0: 6d61 6765 7329 0d0a 0d0a 2020 2020 2020  mages)....      
-0000dcf0: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-0000dd00: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000dd10: 0d0a 2020 2020 2020 2020 6e75 6d43 6861  ..        numCha
-0000dd20: 6e6e 656c 203a 2069 6e74 2c20 6f70 7469  nnel : int, opti
-0000dd30: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
-0000dd40: 2020 5468 6520 6361 6d65 7261 2063 6861    The camera cha
-0000dd50: 6e6e 656c 2074 6f20 6765 7420 7468 6520  nnel to get the 
-0000dd60: 696d 6167 6520 6672 6f6d 2e20 2049 6620  image from.  If 
-0000dd70: 4e6f 6e65 2c20 2874 6865 2064 6566 6175  None, (the defau
-0000dd80: 6c74 292c 2074 6865 6e0d 0a20 2020 2020  lt), then..     
-0000dd90: 2020 2020 2020 204d 756c 7469 2d43 6861         Multi-Cha
-0000dda0: 6e6e 656c 2063 616d 6572 6173 2077 696c  nnel cameras wil
-0000ddb0: 6c20 7265 7475 726e 2074 6865 2063 6f6e  l return the con
-0000ddc0: 7465 6e74 206f 6620 7468 6520 6669 7273  tent of the firs
-0000ddd0: 7420 6368 616e 6e65 6c2e 0d0a 2020 2020  t channel...    
-0000dde0: 2020 2020 6669 7820 3a20 626f 6f6c 2c20      fix : bool, 
-0000ddf0: 6465 6661 756c 743a 2054 7275 650d 0a20  default: True.. 
-0000de00: 2020 2020 2020 2020 2020 2049 6620 6054             If `T
-0000de10: 7275 6560 2028 7468 6520 6465 6661 756c  rue` (the defaul
-0000de20: 7429 2c20 7468 656e 2069 6d61 6765 7320  t), then images 
-0000de30: 7769 7468 206e 5f63 6f6d 706f 6e65 6e74  with n_component
-0000de40: 7320 3e20 3120 286c 696b 6520 5247 4220  s > 1 (like RGB 
-0000de50: 696d 6167 6573 290d 0a20 2020 2020 2020  images)..       
-0000de60: 2020 2020 2077 696c 6c20 6265 2072 6573       will be res
-0000de70: 6861 7065 6420 746f 2028 772c 2068 2c20  haped to (w, h, 
-0000de80: 6e5f 636f 6d70 6f6e 656e 7473 2920 7573  n_components) us
-0000de90: 696e 6720 6066 6978 496d 6167 6560 2e0d  ing `fixImage`..
-0000dea0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000deb0: 2020 2020 2020 696d 6720 3d20 280d 0a20        img = (.. 
-0000dec0: 2020 2020 2020 2020 2020 2073 7570 6572             super
-0000ded0: 2829 2e67 6574 496d 6167 6528 6e75 6d43  ().getImage(numC
-0000dee0: 6861 6e6e 656c 290d 0a20 2020 2020 2020  hannel)..       
-0000def0: 2020 2020 2069 6620 6e75 6d43 6861 6e6e       if numChann
-0000df00: 656c 2069 7320 6e6f 7420 4e6f 6e65 0d0a  el is not None..
-0000df10: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000df20: 2073 7570 6572 2829 2e67 6574 496d 6167   super().getImag
-0000df30: 6528 290d 0a20 2020 2020 2020 2029 0d0a  e()..        )..
-0000df40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000df50: 656c 662e 6669 7849 6d61 6765 2869 6d67  elf.fixImage(img
-0000df60: 2920 6966 2066 6978 2065 6c73 6520 696d  ) if fix else im
-0000df70: 670d 0a0d 0a20 2020 2064 6566 2073 7461  g....    def sta
-0000df80: 7274 436f 6e74 696e 756f 7573 5365 7175  rtContinuousSequ
-0000df90: 656e 6365 4163 7175 6973 6974 696f 6e28  enceAcquisition(
-0000dfa0: 7365 6c66 2c20 696e 7465 7276 616c 4d73  self, intervalMs
-0000dfb0: 3a20 666c 6f61 7420 3d20 3029 202d 3e20  : float = 0) -> 
-0000dfc0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2022  None:..        "
-0000dfd0: 2222 5374 6172 7420 6120 436f 6e74 696e  ""Start a Contin
-0000dfe0: 756f 7573 5365 7175 656e 6365 4163 7175  uousSequenceAcqu
-0000dff0: 6973 6974 696f 6e2e 0d0a 0d0a 2020 2020  isition.....    
-0000e000: 2020 2020 2a2a 5768 7920 4f76 6572 7269      **Why Overri
-0000e010: 6465 3f2a 2a20 546f 2065 6d69 7420 6120  de?** To emit a 
-0000e020: 6073 7461 7274 436f 6e74 696e 756f 7573  `startContinuous
-0000e030: 5365 7175 656e 6365 4163 7175 6973 6974  SequenceAcquisit
-0000e040: 696f 6e60 2065 7665 6e74 2e0d 0a20 2020  ion` event...   
-0000e050: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000e060: 2020 7375 7065 7228 292e 7374 6172 7443    super().startC
-0000e070: 6f6e 7469 6e75 6f75 7353 6571 7565 6e63  ontinuousSequenc
-0000e080: 6541 6371 7569 7369 7469 6f6e 2869 6e74  eAcquisition(int
-0000e090: 6572 7661 6c4d 7329 0d0a 2020 2020 2020  ervalMs)..      
-0000e0a0: 2020 7365 6c66 2e65 7665 6e74 732e 636f    self.events.co
-0000e0b0: 6e74 696e 756f 7573 5365 7175 656e 6365  ntinuousSequence
-0000e0c0: 4163 7175 6973 6974 696f 6e53 7461 7274  AcquisitionStart
-0000e0d0: 6564 2e65 6d69 7428 290d 0a0d 0a20 2020  ed.emit()....   
-0000e0e0: 2040 6f76 6572 6c6f 6164 0d0a 2020 2020   @overload..    
-0000e0f0: 6465 6620 7374 6172 7453 6571 7565 6e63  def startSequenc
-0000e100: 6541 6371 7569 7369 7469 6f6e 280d 0a20  eAcquisition(.. 
-0000e110: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-0000e120: 2020 2020 2020 6e75 6d49 6d61 6765 733a        numImages:
-0000e130: 2069 6e74 2c0d 0a20 2020 2020 2020 2069   int,..        i
-0000e140: 6e74 6572 7661 6c4d 733a 2066 6c6f 6174  ntervalMs: float
-0000e150: 2c0d 0a20 2020 2020 2020 2073 746f 704f  ,..        stopO
-0000e160: 6e4f 7665 7266 6c6f 773a 2062 6f6f 6c2c  nOverflow: bool,
-0000e170: 0d0a 2020 2020 2920 2d3e 204e 6f6e 653a  ..    ) -> None:
-0000e180: 0d0a 2020 2020 2020 2020 2e2e 2e0d 0a0d  ..        ......
-0000e190: 0a20 2020 2040 6f76 6572 6c6f 6164 0d0a  .    @overload..
-0000e1a0: 2020 2020 6465 6620 7374 6172 7453 6571      def startSeq
-0000e1b0: 7565 6e63 6541 6371 7569 7369 7469 6f6e  uenceAcquisition
-0000e1c0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-0000e1d0: 0d0a 2020 2020 2020 2020 6361 6d65 7261  ..        camera
-0000e1e0: 4c61 6265 6c3a 2073 7472 2c0d 0a20 2020  Label: str,..   
-0000e1f0: 2020 2020 206e 756d 496d 6167 6573 3a20       numImages: 
-0000e200: 696e 742c 0d0a 2020 2020 2020 2020 696e  int,..        in
-0000e210: 7465 7276 616c 4d73 3a20 666c 6f61 742c  tervalMs: float,
-0000e220: 0d0a 2020 2020 2020 2020 7374 6f70 4f6e  ..        stopOn
-0000e230: 4f76 6572 666c 6f77 3a20 626f 6f6c 2c0d  Overflow: bool,.
-0000e240: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0d  .    ) -> None:.
-0000e250: 0a20 2020 2020 2020 202e 2e2e 0d0a 0d0a  .        .......
-0000e260: 2020 2020 6465 6620 7374 6172 7453 6571      def startSeq
-0000e270: 7565 6e63 6541 6371 7569 7369 7469 6f6e  uenceAcquisition
-0000e280: 2873 656c 662c 202a 6172 6773 3a20 416e  (self, *args: An
-0000e290: 792c 202a 2a6b 7761 7267 733a 2041 6e79  y, **kwargs: Any
-0000e2a0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-0000e2b0: 2020 2020 2222 2253 7461 7274 7320 7374      """Starts st
-0000e2c0: 7265 616d 696e 6720 6361 6d65 7261 2073  reaming camera s
-0000e2d0: 6571 7565 6e63 6520 6163 7175 6973 6974  equence acquisit
-0000e2e0: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
-0000e2f0: 5468 6973 2063 6f6d 6d61 6e64 2064 6f65  This command doe
-0000e300: 7320 6e6f 7420 626c 6f63 6b20 7468 6520  s not block the 
-0000e310: 6361 6c6c 696e 6720 7468 7265 6164 2066  calling thread f
-0000e320: 6f72 2074 6865 2064 7572 6174 696f 6e20  or the duration 
-0000e330: 6f66 2074 6865 0d0a 2020 2020 2020 2020  of the..        
-0000e340: 6163 7175 6973 6974 696f 6e2e 0d0a 0d0a  acquisition.....
-0000e350: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
-0000e360: 6572 7269 6465 3f2a 2a20 546f 2065 6d69  erride?** To emi
-0000e370: 7420 6120 6073 7461 7274 5365 7175 656e  t a `startSequen
-0000e380: 6365 4163 7175 6973 6974 696f 6e60 2065  ceAcquisition` e
-0000e390: 7665 6e74 2e0d 0a20 2020 2020 2020 2022  vent...        "
-0000e3a0: 2222 0d0a 2020 2020 2020 2020 7375 7065  ""..        supe
-0000e3b0: 7228 292e 7374 6172 7453 6571 7565 6e63  r().startSequenc
-0000e3c0: 6541 6371 7569 7369 7469 6f6e 282a 6172  eAcquisition(*ar
-0000e3d0: 6773 2c20 2a2a 6b77 6172 6773 290d 0a20  gs, **kwargs).. 
-0000e3e0: 2020 2020 2020 2069 6620 6c65 6e28 6172         if len(ar
-0000e3f0: 6773 2920 3d3d 2033 3a0d 0a20 2020 2020  gs) == 3:..     
-0000e400: 2020 2020 2020 206e 756d 496d 6167 6573         numImages
-0000e410: 2c20 696e 7465 7276 616c 4d73 2c20 7374  , intervalMs, st
-0000e420: 6f70 4f6e 4f76 6572 666c 6f77 203d 2061  opOnOverflow = a
-0000e430: 7267 730d 0a20 2020 2020 2020 2020 2020  rgs..           
-0000e440: 2063 616d 6572 614c 6162 656c 203d 2073   cameraLabel = s
-0000e450: 7570 6572 2829 2e67 6574 4361 6d65 7261  uper().getCamera
-0000e460: 4465 7669 6365 2829 0d0a 2020 2020 2020  Device()..      
-0000e470: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000e480: 2020 2020 2063 616d 6572 614c 6162 656c       cameraLabel
-0000e490: 2c20 6e75 6d49 6d61 6765 732c 2069 6e74  , numImages, int
-0000e4a0: 6572 7661 6c4d 732c 2073 746f 704f 6e4f  ervalMs, stopOnO
-0000e4b0: 7665 7266 6c6f 7720 3d20 6172 6773 0d0a  verflow = args..
-0000e4c0: 2020 2020 2020 2020 7365 6c66 2e65 7665          self.eve
-0000e4d0: 6e74 732e 7365 7175 656e 6365 4163 7175  nts.sequenceAcqu
-0000e4e0: 6973 6974 696f 6e53 7461 7274 6564 2e65  isitionStarted.e
-0000e4f0: 6d69 7428 0d0a 2020 2020 2020 2020 2020  mit(..          
-0000e500: 2020 6361 6d65 7261 4c61 6265 6c2c 206e    cameraLabel, n
-0000e510: 756d 496d 6167 6573 2c20 696e 7465 7276  umImages, interv
-0000e520: 616c 4d73 2c20 7374 6f70 4f6e 4f76 6572  alMs, stopOnOver
-0000e530: 666c 6f77 0d0a 2020 2020 2020 2020 290d  flow..        ).
-0000e540: 0a0d 0a20 2020 2064 6566 2073 746f 7053  ...    def stopS
-0000e550: 6571 7565 6e63 6541 6371 7569 7369 7469  equenceAcquisiti
-0000e560: 6f6e 2873 656c 662c 2063 616d 6572 614c  on(self, cameraL
-0000e570: 6162 656c 3a20 7374 7220 7c20 4e6f 6e65  abel: str | None
-0000e580: 203d 204e 6f6e 6529 202d 3e20 4e6f 6e65   = None) -> None
-0000e590: 3a0d 0a20 2020 2020 2020 2022 2222 5374  :..        """St
-0000e5a0: 6f70 7320 7374 7265 616d 696e 6720 6361  ops streaming ca
-0000e5b0: 6d65 7261 2073 6571 7565 6e63 6520 6163  mera sequence ac
-0000e5c0: 7175 6973 6974 696f 6e2e 0d0a 0d0a 2020  quisition.....  
-0000e5d0: 2020 2020 2020 2866 6f72 2061 2073 7065        (for a spe
-0000e5e0: 6369 6669 6564 2063 616d 6572 6120 6966  cified camera if
-0000e5f0: 2060 6361 6d65 7261 4c61 6265 6c60 2069   `cameraLabel` i
-0000e600: 7320 7072 6f76 6964 6564 2e29 0d0a 0d0a  s provided.)....
-0000e610: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
-0000e620: 6572 7269 6465 3f2a 2a20 546f 2065 6d69  erride?** To emi
-0000e630: 7420 6120 6073 746f 7053 6571 7565 6e63  t a `stopSequenc
-0000e640: 6541 6371 7569 7369 7469 6f6e 6020 6576  eAcquisition` ev
-0000e650: 656e 742e 0d0a 2020 2020 2020 2020 2222  ent...        ""
-0000e660: 220d 0a20 2020 2020 2020 2069 6620 6361  "..        if ca
-0000e670: 6d65 7261 4c61 6265 6c20 6973 204e 6f6e  meraLabel is Non
-0000e680: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000e690: 7375 7065 7228 292e 7374 6f70 5365 7175  super().stopSequ
-0000e6a0: 656e 6365 4163 7175 6973 6974 696f 6e28  enceAcquisition(
-0000e6b0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-0000e6c0: 0d0a 2020 2020 2020 2020 2020 2020 7375  ..            su
-0000e6d0: 7065 7228 292e 7374 6f70 5365 7175 656e  per().stopSequen
-0000e6e0: 6365 4163 7175 6973 6974 696f 6e28 6361  ceAcquisition(ca
-0000e6f0: 6d65 7261 4c61 6265 6c29 0d0a 2020 2020  meraLabel)..    
-0000e700: 2020 2020 6361 6d65 7261 4c61 6265 6c20      cameraLabel 
-0000e710: 3d20 6361 6d65 7261 4c61 6265 6c20 6f72  = cameraLabel or
-0000e720: 2073 7570 6572 2829 2e67 6574 4361 6d65   super().getCame
-0000e730: 7261 4465 7669 6365 2829 0d0a 2020 2020  raDevice()..    
-0000e740: 2020 2020 7365 6c66 2e65 7665 6e74 732e      self.events.
-0000e750: 7365 7175 656e 6365 4163 7175 6973 6974  sequenceAcquisit
-0000e760: 696f 6e53 746f 7070 6564 2e65 6d69 7428  ionStopped.emit(
-0000e770: 6361 6d65 7261 4c61 6265 6c29 0d0a 0d0a  cameraLabel)....
-0000e780: 2020 2020 6465 6620 7365 7441 7574 6f53      def setAutoS
-0000e790: 6875 7474 6572 2873 656c 662c 2073 7461  hutter(self, sta
-0000e7a0: 7465 3a20 626f 6f6c 2920 2d3e 204e 6f6e  te: bool) -> Non
-0000e7b0: 653a 0d0a 2020 2020 2020 2020 2222 2253  e:..        """S
-0000e7c0: 6574 2073 6875 7474 6572 2074 6f20 6175  et shutter to au
-0000e7d0: 746f 6d61 7469 6361 6c6c 7920 6f70 656e  tomatically open
-0000e7e0: 2061 6e64 2063 6c6f 7365 2077 6865 6e20   and close when 
-0000e7f0: 616e 2069 6d61 6765 2069 7320 6163 7175  an image is acqu
-0000e800: 6972 6564 2e0d 0a0d 0a20 2020 2020 2020  ired.....       
-0000e810: 202a 2a57 6879 204f 7665 7272 6964 653f   **Why Override?
-0000e820: 2a2a 2054 6f20 656d 6974 2061 6e20 6061  ** To emit an `a
-0000e830: 7574 6f53 6875 7474 6572 5365 7460 2065  utoShutterSet` e
-0000e840: 7665 6e74 2e0d 0a20 2020 2020 2020 2022  vent...        "
-0000e850: 2222 0d0a 2020 2020 2020 2020 7375 7065  ""..        supe
-0000e860: 7228 292e 7365 7441 7574 6f53 6875 7474  r().setAutoShutt
-0000e870: 6572 2873 7461 7465 290d 0a20 2020 2020  er(state)..     
-0000e880: 2020 2073 656c 662e 6576 656e 7473 2e61     self.events.a
-0000e890: 7574 6f53 6875 7474 6572 5365 742e 656d  utoShutterSet.em
-0000e8a0: 6974 2873 7461 7465 290d 0a0d 0a20 2020  it(state)....   
-0000e8b0: 2040 6f76 6572 6c6f 6164 0d0a 2020 2020   @overload..    
-0000e8c0: 6465 6620 7365 7453 6875 7474 6572 4f70  def setShutterOp
-0000e8d0: 656e 2873 656c 662c 2073 7461 7465 3a20  en(self, state: 
-0000e8e0: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0d0a  bool) -> None:..
-0000e8f0: 2020 2020 2020 2020 2e2e 2e0d 0a0d 0a20          ....... 
-0000e900: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
-0000e910: 2020 6465 6620 7365 7453 6875 7474 6572    def setShutter
-0000e920: 4f70 656e 2873 656c 662c 2073 6875 7474  Open(self, shutt
-0000e930: 6572 4c61 6265 6c3a 2073 7472 2c20 7374  erLabel: str, st
-0000e940: 6174 653a 2062 6f6f 6c29 202d 3e20 4e6f  ate: bool) -> No
-0000e950: 6e65 3a0d 0a20 2020 2020 2020 202e 2e2e  ne:..        ...
-0000e960: 0d0a 0d0a 2020 2020 6465 6620 7365 7453  ....    def setS
-0000e970: 6875 7474 6572 4f70 656e 2873 656c 662c  hutterOpen(self,
-0000e980: 202a 6172 6773 3a20 416e 792c 202a 2a6b   *args: Any, **k
-0000e990: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
-0000e9a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
-0000e9b0: 224f 7065 6e20 6f72 2063 6c6f 7365 2074  "Open or close t
-0000e9c0: 6865 2063 7572 7265 6e74 6c79 2073 656c  he currently sel
-0000e9d0: 6563 7465 6420 6f72 2060 7368 7574 7465  ected or `shutte
-0000e9e0: 724c 6162 656c 6020 7368 7574 7465 722e  rLabel` shutter.
-0000e9f0: 0d0a 0d0a 2020 2020 2020 2020 2a2a 5768  ....        **Wh
-0000ea00: 7920 4f76 6572 7269 6465 3f2a 2a20 546f  y Override?** To
-0000ea10: 2065 6d69 7420 6120 6070 726f 7065 7274   emit a `propert
-0000ea20: 7943 6861 6e67 6564 6020 6576 656e 742e  yChanged` event.
-0000ea30: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000ea40: 2020 2020 2020 2073 7570 6572 2829 2e73         super().s
-0000ea50: 6574 5368 7574 7465 724f 7065 6e28 2a61  etShutterOpen(*a
-0000ea60: 7267 732c 202a 2a6b 7761 7267 7329 0d0a  rgs, **kwargs)..
-0000ea70: 2020 2020 2020 2020 7368 7574 7465 724c          shutterL
-0000ea80: 6162 656c 2c20 7374 6174 6520 3d20 6b77  abel, state = kw
-0000ea90: 6172 6773 2e67 6574 2822 7368 7574 7465  args.get("shutte
-0000eaa0: 724c 6162 656c 2229 2c20 6b77 6172 6773  rLabel"), kwargs
-0000eab0: 2e67 6574 2822 7374 6174 6522 290d 0a20  .get("state").. 
-0000eac0: 2020 2020 2020 2069 6620 6c65 6e28 6172         if len(ar
-0000ead0: 6773 2920 3e20 313a 0d0a 2020 2020 2020  gs) > 1:..      
-0000eae0: 2020 2020 2020 7368 7574 7465 724c 6162        shutterLab
-0000eaf0: 656c 2c20 7374 6174 6520 3d20 6172 6773  el, state = args
-0000eb00: 0d0a 2020 2020 2020 2020 656c 6966 2061  ..        elif a
-0000eb10: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-0000eb20: 2020 7368 7574 7465 724c 6162 656c 203d    shutterLabel =
-0000eb30: 2073 7570 6572 2829 2e67 6574 5368 7574   super().getShut
-0000eb40: 7465 7244 6576 6963 6528 290d 0a20 2020  terDevice()..   
-0000eb50: 2020 2020 2020 2020 2073 7461 7465 203d           state =
-0000eb60: 2061 7267 730d 0a20 2020 2020 2020 2073   args..        s
-0000eb70: 656c 662e 6576 656e 7473 2e70 726f 7065  elf.events.prope
-0000eb80: 7274 7943 6861 6e67 6564 2e65 6d69 7428  rtyChanged.emit(
-0000eb90: 7368 7574 7465 724c 6162 656c 2c20 2253  shutterLabel, "S
-0000eba0: 7461 7465 222c 2073 7461 7465 290d 0a0d  tate", state)...
-0000ebb0: 0a20 2020 2040 6f76 6572 6c6f 6164 0d0a  .    @overload..
-0000ebc0: 2020 2020 6465 6620 6465 6c65 7465 436f      def deleteCo
-0000ebd0: 6e66 6967 2873 656c 662c 2067 726f 7570  nfig(self, group
-0000ebe0: 4e61 6d65 3a20 7374 722c 2063 6f6e 6669  Name: str, confi
-0000ebf0: 674e 616d 653a 2073 7472 2920 2d3e 204e  gName: str) -> N
-0000ec00: 6f6e 653a 0d0a 2020 2020 2020 2020 2e2e  one:..        ..
-0000ec10: 2e0d 0a0d 0a20 2020 2040 6f76 6572 6c6f  .....    @overlo
-0000ec20: 6164 0d0a 2020 2020 6465 6620 6465 6c65  ad..    def dele
-0000ec30: 7465 436f 6e66 6967 280d 0a20 2020 2020  teConfig(..     
-0000ec40: 2020 2073 656c 662c 2067 726f 7570 4e61     self, groupNa
-0000ec50: 6d65 3a20 7374 722c 2063 6f6e 6669 674e  me: str, configN
-0000ec60: 616d 653a 2073 7472 2c20 6465 7669 6365  ame: str, device
-0000ec70: 4c61 6265 6c3a 2073 7472 2c20 7072 6f70  Label: str, prop
-0000ec80: 4e61 6d65 3a20 7374 720d 0a20 2020 2029  Name: str..    )
-0000ec90: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-0000eca0: 2020 202e 2e2e 0d0a 0d0a 2020 2020 6465     .......    de
-0000ecb0: 6620 6465 6c65 7465 436f 6e66 6967 280d  f deleteConfig(.
-0000ecc0: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-0000ecd0: 2020 2020 2020 2020 6772 6f75 704e 616d          groupNam
-0000ece0: 653a 2073 7472 2c0d 0a20 2020 2020 2020  e: str,..       
-0000ecf0: 2063 6f6e 6669 674e 616d 653a 2073 7472   configName: str
-0000ed00: 2c0d 0a20 2020 2020 2020 2064 6576 6963  ,..        devic
-0000ed10: 654c 6162 656c 3a20 7374 7220 7c20 4e6f  eLabel: str | No
-0000ed20: 6e65 203d 204e 6f6e 652c 0d0a 2020 2020  ne = None,..    
-0000ed30: 2020 2020 7072 6f70 4e61 6d65 3a20 7374      propName: st
-0000ed40: 7220 7c20 4e6f 6e65 203d 204e 6f6e 652c  r | None = None,
-0000ed50: 0d0a 2020 2020 2920 2d3e 204e 6f6e 653a  ..    ) -> None:
-0000ed60: 0d0a 2020 2020 2020 2020 2222 2244 656c  ..        """Del
-0000ed70: 6574 6520 6063 6f6e 6669 674e 616d 6560  ete `configName`
-0000ed80: 2066 726f 6d20 6067 726f 7570 4e61 6d65   from `groupName
-0000ed90: 602e 0d0a 0d0a 2020 2020 2020 2020 2a2a  `.....        **
-0000eda0: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
-0000edb0: 546f 2065 6d69 7420 6120 6063 6f6e 6669  To emit a `confi
-0000edc0: 6744 656c 6574 6564 6020 6576 656e 742e  gDeleted` event.
-0000edd0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000ede0: 2020 2020 2020 2061 7267 733a 2074 7570         args: tup
-0000edf0: 6c65 5b73 7472 2c20 2e2e 2e5d 203d 2028  le[str, ...] = (
-0000ee00: 6772 6f75 704e 616d 652c 2063 6f6e 6669  groupName, confi
-0000ee10: 674e 616d 6529 0d0a 2020 2020 2020 2020  gName)..        
-0000ee20: 6966 2064 6576 6963 654c 6162 656c 2069  if deviceLabel i
-0000ee30: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2070  s not None and p
-0000ee40: 726f 704e 616d 6520 6973 206e 6f74 204e  ropName is not N
-0000ee50: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000ee60: 2020 6172 6773 203d 2028 2a61 7267 732c    args = (*args,
-0000ee70: 2064 6576 6963 654c 6162 656c 2c20 7072   deviceLabel, pr
-0000ee80: 6f70 4e61 6d65 290d 0a20 2020 2020 2020  opName)..       
-0000ee90: 2073 7570 6572 2829 2e64 656c 6574 6543   super().deleteC
-0000eea0: 6f6e 6669 6728 2a61 7267 7329 0d0a 2020  onfig(*args)..  
-0000eeb0: 2020 2020 2020 7365 6c66 2e65 7665 6e74        self.event
-0000eec0: 732e 636f 6e66 6967 4465 6c65 7465 642e  s.configDeleted.
-0000eed0: 656d 6974 2867 726f 7570 4e61 6d65 2c20  emit(groupName, 
-0000eee0: 636f 6e66 6967 4e61 6d65 290d 0a0d 0a20  configName).... 
-0000eef0: 2020 2064 6566 2064 656c 6574 6543 6f6e     def deleteCon
-0000ef00: 6669 6747 726f 7570 2873 656c 662c 2067  figGroup(self, g
-0000ef10: 726f 7570 3a20 7374 7229 202d 3e20 4e6f  roup: str) -> No
-0000ef20: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
-0000ef30: 4465 6c65 7465 7320 616e 2065 6e74 6972  Deletes an entir
-0000ef40: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-0000ef50: 6067 726f 7570 602e 0d0a 0d0a 2020 2020  `group`.....    
-0000ef60: 2020 2020 2a2a 5768 7920 4f76 6572 7269      **Why Overri
-0000ef70: 6465 3f2a 2a20 546f 2065 6d69 7420 6120  de?** To emit a 
-0000ef80: 6063 6f6e 6669 6747 726f 7570 4465 6c65  `configGroupDele
-0000ef90: 7465 6460 2065 7665 6e74 2e0d 0a20 2020  ted` event...   
-0000efa0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000efb0: 2020 7375 7065 7228 292e 6465 6c65 7465    super().delete
-0000efc0: 436f 6e66 6967 4772 6f75 7028 6772 6f75  ConfigGroup(grou
-0000efd0: 7029 0d0a 2020 2020 2020 2020 7365 6c66  p)..        self
-0000efe0: 2e65 7665 6e74 732e 636f 6e66 6967 4772  .events.configGr
-0000eff0: 6f75 7044 656c 6574 6564 2e65 6d69 7428  oupDeleted.emit(
-0000f000: 6772 6f75 7029 0d0a 0d0a 2020 2020 406f  group)....    @o
-0000f010: 7665 726c 6f61 640d 0a20 2020 2064 6566  verload..    def
-0000f020: 2064 6566 696e 6543 6f6e 6669 6728 7365   defineConfig(se
-0000f030: 6c66 2c20 6772 6f75 704e 616d 653a 2073  lf, groupName: s
-0000f040: 7472 2c20 636f 6e66 6967 4e61 6d65 3a20  tr, configName: 
-0000f050: 7374 7229 202d 3e20 4e6f 6e65 3a0d 0a20  str) -> None:.. 
-0000f060: 2020 2020 2020 202e 2e2e 0d0a 0d0a 2020         .......  
-0000f070: 2020 406f 7665 726c 6f61 640d 0a20 2020    @overload..   
-0000f080: 2064 6566 2064 6566 696e 6543 6f6e 6669   def defineConfi
-0000f090: 6728 0d0a 2020 2020 2020 2020 7365 6c66  g(..        self
-0000f0a0: 2c0d 0a20 2020 2020 2020 2067 726f 7570  ,..        group
-0000f0b0: 4e61 6d65 3a20 7374 722c 0d0a 2020 2020  Name: str,..    
-0000f0c0: 2020 2020 636f 6e66 6967 4e61 6d65 3a20      configName: 
-0000f0d0: 7374 722c 0d0a 2020 2020 2020 2020 6465  str,..        de
-0000f0e0: 7669 6365 4c61 6265 6c3a 2073 7472 2c0d  viceLabel: str,.
-0000f0f0: 0a20 2020 2020 2020 2070 726f 704e 616d  .        propNam
-0000f100: 653a 2073 7472 2c0d 0a20 2020 2020 2020  e: str,..       
-0000f110: 2076 616c 7565 3a20 7374 722c 0d0a 2020   value: str,..  
-0000f120: 2020 2920 2d3e 204e 6f6e 653a 0d0a 2020    ) -> None:..  
-0000f130: 2020 2020 2020 2e2e 2e0d 0a0d 0a20 2020        .......   
-0000f140: 2064 6566 2064 6566 696e 6543 6f6e 6669   def defineConfi
-0000f150: 6728 0d0a 2020 2020 2020 2020 7365 6c66  g(..        self
-0000f160: 2c0d 0a20 2020 2020 2020 2067 726f 7570  ,..        group
-0000f170: 4e61 6d65 3a20 7374 722c 0d0a 2020 2020  Name: str,..    
-0000f180: 2020 2020 636f 6e66 6967 4e61 6d65 3a20      configName: 
-0000f190: 7374 722c 0d0a 2020 2020 2020 2020 6465  str,..        de
-0000f1a0: 7669 6365 4c61 6265 6c3a 2073 7472 207c  viceLabel: str |
-0000f1b0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
-0000f1c0: 2020 2020 2020 2070 726f 704e 616d 653a         propName:
-0000f1d0: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
-0000f1e0: 6e65 2c0d 0a20 2020 2020 2020 2076 616c  ne,..        val
-0000f1f0: 7565 3a20 7374 7220 7c20 4e6f 6e65 203d  ue: str | None =
-0000f200: 204e 6f6e 652c 0d0a 2020 2020 2920 2d3e   None,..    ) ->
-0000f210: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000f220: 2222 2244 6566 696e 6573 2061 2063 6f6e  """Defines a con
-0000f230: 6669 6775 7261 7469 6f6e 2e0d 0a0d 0a20  figuration..... 
-0000f240: 2020 2020 2020 202a 2a57 6879 204f 7665         **Why Ove
-0000f250: 7272 6964 653f 2a2a 2054 6f20 656d 6974  rride?** To emit
-0000f260: 2061 2060 636f 6e66 6967 4465 6669 6e65   a `configDefine
-0000f270: 6460 2065 7665 6e74 2e20 2041 6c73 6f2c  d` event.  Also,
-0000f280: 2069 6620 6067 726f 7570 4e61 6d65 6020   if `groupName` 
-0000f290: 6973 0d0a 2020 2020 2020 2020 6e6f 7420  is..        not 
-0000f2a0: 6120 6465 6669 6e65 6420 6772 6f75 702c  a defined group,
-0000f2b0: 2074 6865 6e20 6064 6566 696e 6543 6f6e   then `defineCon
-0000f2c0: 6669 6747 726f 7570 2867 726f 7570 4e61  figGroup(groupNa
-0000f2d0: 6d65 2960 2069 7320 6361 6c6c 6564 2e0d  me)` is called..
-0000f2e0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000f2f0: 2020 2020 2020 6966 206e 6f74 2063 6f6e        if not con
-0000f300: 6669 674e 616d 653a 0d0a 2020 2020 2020  figName:..      
-0000f310: 2020 2020 2020 6964 7820 3d20 7375 6d28        idx = sum(
-0000f320: 554e 4e41 4d45 445f 5052 4553 4554 2069  UNNAMED_PRESET i
-0000f330: 6e20 7020 666f 7220 7020 696e 2073 656c  n p for p in sel
-0000f340: 662e 6765 7441 7661 696c 6162 6c65 436f  f.getAvailableCo
-0000f350: 6e66 6967 7328 6772 6f75 704e 616d 6529  nfigs(groupName)
-0000f360: 290d 0a20 2020 2020 2020 2020 2020 2063  )..            c
-0000f370: 6f6e 6669 674e 616d 6520 3d20 6622 7b55  onfigName = f"{U
-0000f380: 4e4e 414d 4544 5f50 5245 5345 547d 5f7b  NNAMED_PRESET}_{
-0000f390: 6964 787d 2220 6966 2069 6478 203e 2030  idx}" if idx > 0
-0000f3a0: 2065 6c73 6520 554e 4e41 4d45 445f 5052   else UNNAMED_PR
-0000f3b0: 4553 4554 0d0a 0d0a 2020 2020 2020 2020  ESET....        
-0000f3c0: 6966 206e 6f74 2073 656c 662e 6973 4772  if not self.isGr
-0000f3d0: 6f75 7044 6566 696e 6564 2867 726f 7570  oupDefined(group
-0000f3e0: 4e61 6d65 293a 0d0a 2020 2020 2020 2020  Name):..        
-0000f3f0: 2020 2020 2320 6e65 6564 6564 2074 6f20      # needed to 
-0000f400: 7265 6672 6573 6820 7079 6d6d 636f 7265  refresh pymmcore
-0000f410: 2027 4368 616e 6e65 6c47 726f 7570 2720   'ChannelGroup' 
-0000f420: 6f70 7469 6f6e 730d 0a20 2020 2020 2020  options..       
-0000f430: 2020 2020 2073 7570 6572 2829 2e64 6566       super().def
-0000f440: 696e 6543 6f6e 6669 6747 726f 7570 2867  ineConfigGroup(g
-0000f450: 726f 7570 4e61 6d65 290d 0a0d 0a20 2020  roupName)....   
-0000f460: 2020 2020 2069 6620 2864 6576 6963 654c       if (deviceL
-0000f470: 6162 656c 2069 7320 6e6f 7420 4e6f 6e65  abel is not None
-0000f480: 2920 616e 6420 2870 726f 704e 616d 6520  ) and (propName 
-0000f490: 6973 206e 6f74 204e 6f6e 6529 2061 6e64  is not None) and
-0000f4a0: 2028 7661 6c75 6520 6973 206e 6f74 204e   (value is not N
-0000f4b0: 6f6e 6529 3a0d 0a20 2020 2020 2020 2020  one):..         
-0000f4c0: 2020 2073 7570 6572 2829 2e64 6566 696e     super().defin
-0000f4d0: 6543 6f6e 6669 6728 6772 6f75 704e 616d  eConfig(groupNam
-0000f4e0: 652c 2063 6f6e 6669 674e 616d 652c 2064  e, configName, d
-0000f4f0: 6576 6963 654c 6162 656c 2c20 7072 6f70  eviceLabel, prop
-0000f500: 4e61 6d65 2c20 7661 6c75 6529 0d0a 2020  Name, value)..  
-0000f510: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000f520: 2020 2020 2020 2020 2064 6576 6963 654c           deviceL
-0000f530: 6162 656c 2c20 7072 6f70 4e61 6d65 2c20  abel, propName, 
-0000f540: 7661 6c75 6520 3d20 2822 222c 2022 222c  value = ("", "",
-0000f550: 2022 2229 0d0a 2020 2020 2020 2020 2020   "")..          
-0000f560: 2020 7375 7065 7228 292e 6465 6669 6e65    super().define
-0000f570: 436f 6e66 6967 2867 726f 7570 4e61 6d65  Config(groupName
-0000f580: 2c20 636f 6e66 6967 4e61 6d65 290d 0a0d  , configName)...
-0000f590: 0a20 2020 2020 2020 2073 656c 662e 6576  .        self.ev
-0000f5a0: 656e 7473 2e63 6f6e 6669 6744 6566 696e  ents.configDefin
-0000f5b0: 6564 2e65 6d69 7428 0d0a 2020 2020 2020  ed.emit(..      
-0000f5c0: 2020 2020 2020 6772 6f75 704e 616d 652c        groupName,
-0000f5d0: 2063 6f6e 6669 674e 616d 652c 2064 6576   configName, dev
-0000f5e0: 6963 654c 6162 656c 2c20 7072 6f70 4e61  iceLabel, propNa
-0000f5f0: 6d65 2c20 7661 6c75 650d 0a20 2020 2020  me, value..     
-0000f600: 2020 2029 0d0a 0d0a 2020 2020 6465 6620     )....    def 
-0000f610: 7365 7450 6978 656c 5369 7a65 556d 2873  setPixelSizeUm(s
-0000f620: 656c 662c 2072 6573 6f6c 7574 696f 6e49  elf, resolutionI
-0000f630: 443a 2073 7472 2c20 7069 7853 697a 653a  D: str, pixSize:
-0000f640: 2066 6c6f 6174 2920 2d3e 204e 6f6e 653a   float) -> None:
-0000f650: 0d0a 2020 2020 2020 2020 2222 2253 6574  ..        """Set
-0000f660: 2070 6978 656c 2073 697a 6520 696e 206d   pixel size in m
-0000f670: 6963 726f 6e73 2066 6f72 2074 6865 2073  icrons for the s
-0000f680: 7065 6369 6669 6564 2060 7265 736f 6c75  pecified `resolu
-0000f690: 7469 6f6e 4944 602e 0d0a 0d0a 2020 2020  tionID`.....    
-0000f6a0: 2020 2020 2a2a 5768 7920 4f76 6572 7269      **Why Overri
-0000f6b0: 6465 3f2a 2a20 546f 2065 6d69 7420 6120  de?** To emit a 
-0000f6c0: 6070 6978 656c 5369 7a65 4368 616e 6765  `pixelSizeChange
-0000f6d0: 6460 2065 7665 6e74 2e0d 0a20 2020 2020  d` event...     
-0000f6e0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000f6f0: 7375 7065 7228 292e 7365 7450 6978 656c  super().setPixel
-0000f700: 5369 7a65 556d 2872 6573 6f6c 7574 696f  SizeUm(resolutio
-0000f710: 6e49 442c 2070 6978 5369 7a65 290d 0a20  nID, pixSize).. 
-0000f720: 2020 2020 2020 2073 656c 662e 6576 656e         self.even
-0000f730: 7473 2e70 6978 656c 5369 7a65 4368 616e  ts.pixelSizeChan
-0000f740: 6765 642e 656d 6974 2870 6978 5369 7a65  ged.emit(pixSize
-0000f750: 290d 0a0d 0a20 2020 2064 6566 2064 656c  )....    def del
-0000f760: 6574 6550 6978 656c 5369 7a65 436f 6e66  etePixelSizeConf
-0000f770: 6967 2873 656c 662c 2072 6573 6f6c 7574  ig(self, resolut
-0000f780: 696f 6e49 443a 2073 7472 2920 2d3e 204e  ionID: str) -> N
-0000f790: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
-0000f7a0: 2244 656c 6574 6520 7468 6520 7069 7865  "Delete the pixe
-0000f7b0: 6c20 7369 7a65 2063 6f6e 6669 6775 7261  l size configura
-0000f7c0: 7469 6f6e 2066 6f72 2074 6865 2067 6976  tion for the giv
-0000f7d0: 656e 2060 7265 736f 6c75 7469 6f6e 4944  en `resolutionID
-0000f7e0: 602e 0d0a 0d0a 2020 2020 2020 2020 2a2a  `.....        **
-0000f7f0: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
-0000f800: 546f 2065 6d69 7420 6120 6070 6978 656c  To emit a `pixel
-0000f810: 5369 7a65 4368 616e 6765 6460 2065 7665  SizeChanged` eve
-0000f820: 6e74 2e0d 0a20 2020 2020 2020 2022 2222  nt...        """
-0000f830: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-0000f840: 292e 6465 6c65 7465 5069 7865 6c53 697a  ).deletePixelSiz
-0000f850: 6543 6f6e 6669 6728 7265 736f 6c75 7469  eConfig(resoluti
-0000f860: 6f6e 4944 290d 0a20 2020 2020 2020 2073  onID)..        s
-0000f870: 656c 662e 6576 656e 7473 2e70 6978 656c  elf.events.pixel
-0000f880: 5369 7a65 4368 616e 6765 642e 656d 6974  SizeChanged.emit
-0000f890: 2830 2e30 290d 0a0d 0a20 2020 2040 6f76  (0.0)....    @ov
-0000f8a0: 6572 6c6f 6164 0d0a 2020 2020 6465 6620  erload..    def 
-0000f8b0: 6465 6669 6e65 5069 7865 6c53 697a 6543  definePixelSizeC
-0000f8c0: 6f6e 6669 6728 7365 6c66 2c20 7265 736f  onfig(self, reso
-0000f8d0: 6c75 7469 6f6e 4944 3a20 7374 7229 202d  lutionID: str) -
-0000f8e0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-0000f8f0: 202e 2e2e 0d0a 0d0a 2020 2020 406f 7665   .......    @ove
-0000f900: 726c 6f61 640d 0a20 2020 2064 6566 2064  rload..    def d
-0000f910: 6566 696e 6550 6978 656c 5369 7a65 436f  efinePixelSizeCo
-0000f920: 6e66 6967 280d 0a20 2020 2020 2020 2073  nfig(..        s
-0000f930: 656c 662c 2072 6573 6f6c 7574 696f 6e49  elf, resolutionI
-0000f940: 443a 2073 7472 2c20 6465 7669 6365 4c61  D: str, deviceLa
-0000f950: 6265 6c3a 2073 7472 2c20 7072 6f70 4e61  bel: str, propNa
-0000f960: 6d65 3a20 7374 722c 2076 616c 7565 3a20  me: str, value: 
-0000f970: 7374 720d 0a20 2020 2029 202d 3e20 4e6f  str..    ) -> No
-0000f980: 6e65 3a0d 0a20 2020 2020 2020 202e 2e2e  ne:..        ...
-0000f990: 0d0a 0d0a 2020 2020 6465 6620 6465 6669  ....    def defi
-0000f9a0: 6e65 5069 7865 6c53 697a 6543 6f6e 6669  nePixelSizeConfi
-0000f9b0: 6728 7365 6c66 2c20 2a61 7267 733a 2073  g(self, *args: s
-0000f9c0: 7472 2c20 2a2a 6b77 6172 6773 3a20 7374  tr, **kwargs: st
-0000f9d0: 7229 202d 3e20 4e6f 6e65 3a0d 0a20 2020  r) -> None:..   
-0000f9e0: 2020 2020 2022 2222 4465 6669 6e65 7320       """Defines 
-0000f9f0: 616e 2065 6d70 7479 2070 6978 656c 2073  an empty pixel s
-0000fa00: 697a 6520 656e 7472 792e 0d0a 0d0a 2020  ize entry.....  
-0000fa10: 2020 2020 2020 2a2a 5768 7920 4f76 6572        **Why Over
-0000fa20: 7269 6465 3f2a 2a20 546f 2065 6d69 7420  ride?** To emit 
-0000fa30: 6120 6070 6978 656c 5369 7a65 4368 616e  a `pixelSizeChan
-0000fa40: 6765 6460 2065 7665 6e74 2e0d 0a20 2020  ged` event...   
-0000fa50: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000fa60: 2020 7375 7065 7228 292e 6465 6669 6e65    super().define
-0000fa70: 5069 7865 6c53 697a 6543 6f6e 6669 6728  PixelSizeConfig(
-0000fa80: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-0000fa90: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-0000faa0: 7665 6e74 732e 7069 7865 6c53 697a 6543  vents.pixelSizeC
-0000fab0: 6861 6e67 6564 2e65 6d69 7428 302e 3029  hanged.emit(0.0)
-0000fac0: 0d0a 0d0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
-0000fad0: 640d 0a20 2020 2064 6566 2073 6574 524f  d..    def setRO
-0000fae0: 4928 7365 6c66 2c20 783a 2069 6e74 2c20  I(self, x: int, 
-0000faf0: 793a 2069 6e74 2c20 7769 6474 683a 2069  y: int, width: i
-0000fb00: 6e74 2c20 6865 6967 6874 3a20 696e 7429  nt, height: int)
-0000fb10: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-0000fb20: 2020 202e 2e2e 0d0a 0d0a 2020 2020 406f     .......    @o
-0000fb30: 7665 726c 6f61 640d 0a20 2020 2064 6566  verload..    def
-0000fb40: 2073 6574 524f 4928 7365 6c66 2c20 6c61   setROI(self, la
-0000fb50: 6265 6c3a 2073 7472 2c20 783a 2069 6e74  bel: str, x: int
-0000fb60: 2c20 793a 2069 6e74 2c20 7769 6474 683a  , y: int, width:
-0000fb70: 2069 6e74 2c20 6865 6967 6874 3a20 696e   int, height: in
-0000fb80: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
-0000fb90: 2020 2020 202e 2e2e 0d0a 0d0a 2020 2020       .......    
-0000fba0: 6465 6620 7365 7452 4f49 2873 656c 662c  def setROI(self,
-0000fbb0: 202a 6172 6773 3a20 416e 792c 202a 2a6b   *args: Any, **k
-0000fbc0: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
-0000fbd0: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
-0000fbe0: 2253 6574 2074 6865 2063 616d 6572 6120  "Set the camera 
-0000fbf0: 5265 6769 6f6e 206f 6620 496e 7465 7265  Region of Intere
-0000fc00: 7374 2028 524f 4929 2e0d 0a0d 0a20 2020  st (ROI).....   
-0000fc10: 2020 2020 202a 2a57 6879 204f 7665 7272       **Why Overr
-0000fc20: 6964 653f 2a2a 2054 6f20 656d 6974 2061  ide?** To emit a
-0000fc30: 2060 726f 6953 6574 6020 6576 656e 742e   `roiSet` event.
-0000fc40: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000fc50: 2020 2020 2020 2073 7570 6572 2829 2e73         super().s
-0000fc60: 6574 524f 4928 2a61 7267 732c 202a 2a6b  etROI(*args, **k
-0000fc70: 7761 7267 7329 0d0a 2020 2020 2020 2020  wargs)..        
-0000fc80: 6966 206c 656e 2861 7267 7329 203d 3d20  if len(args) == 
-0000fc90: 343a 0d0a 2020 2020 2020 2020 2020 2020  4:..            
-0000fca0: 6172 6773 203d 2028 7375 7065 7228 292e  args = (super().
-0000fcb0: 6765 7443 616d 6572 6144 6576 6963 6528  getCameraDevice(
-0000fcc0: 292c 202a 6172 6773 290d 0a20 2020 2020  ), *args)..     
-0000fcd0: 2020 2073 656c 662e 6576 656e 7473 2e72     self.events.r
-0000fce0: 6f69 5365 742e 656d 6974 282a 6172 6773  oiSet.emit(*args
-0000fcf0: 290d 0a0d 0a20 2020 2064 6566 2073 6574  )....    def set
-0000fd00: 4368 616e 6e65 6c47 726f 7570 2873 656c  ChannelGroup(sel
-0000fd10: 662c 2063 6861 6e6e 656c 4772 6f75 703a  f, channelGroup:
-0000fd20: 2073 7472 2920 2d3e 204e 6f6e 653a 0d0a   str) -> None:..
-0000fd30: 2020 2020 2020 2020 2222 2253 7065 6369          """Speci
-0000fd40: 6669 6573 2074 6865 2067 726f 7570 2064  fies the group d
-0000fd50: 6574 6572 6d69 6e69 6e67 2074 6865 2063  etermining the c
-0000fd60: 6861 6e6e 656c 2073 656c 6563 7469 6f6e  hannel selection
-0000fd70: 2e0d 0a0d 0a20 2020 2020 2020 202e 2e2e  .....        ...
-0000fd80: 616e 6420 7365 6e64 2061 2063 6861 6e6e  and send a chann
-0000fd90: 656c 4772 6f75 7043 6861 6e67 6564 2073  elGroupChanged s
-0000fda0: 6967 6e61 6c2e 0d0a 2020 2020 2020 2020  ignal...        
-0000fdb0: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-0000fdc0: 7365 6c66 2e67 6574 4368 616e 6e65 6c47  self.getChannelG
-0000fdd0: 726f 7570 2829 2021 3d20 6368 616e 6e65  roup() != channe
-0000fde0: 6c47 726f 7570 3a0d 0a20 2020 2020 2020  lGroup:..       
-0000fdf0: 2020 2020 2073 7570 6572 2829 2e73 6574       super().set
-0000fe00: 4368 616e 6e65 6c47 726f 7570 2863 6861  ChannelGroup(cha
-0000fe10: 6e6e 656c 4772 6f75 7029 0d0a 2020 2020  nnelGroup)..    
-0000fe20: 2020 2020 2020 2020 7365 6c66 2e65 7665          self.eve
-0000fe30: 6e74 732e 6368 616e 6e65 6c47 726f 7570  nts.channelGroup
-0000fe40: 4368 616e 6765 642e 656d 6974 2863 6861  Changed.emit(cha
-0000fe50: 6e6e 656c 4772 6f75 7029 0d0a 0d0a 2020  nnelGroup)....  
-0000fe60: 2020 6465 6620 7365 7446 6f63 7573 4465    def setFocusDe
-0000fe70: 7669 6365 2873 656c 662c 2066 6f63 7573  vice(self, focus
-0000fe80: 4c61 6265 6c3a 2073 7472 2920 2d3e 204e  Label: str) -> N
-0000fe90: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
-0000fea0: 2253 6574 2074 6865 2063 7572 7265 6e74  "Set the current
-0000feb0: 2046 6f63 7573 2044 6576 6963 6520 616e   Focus Device an
-0000fec0: 6420 656d 6974 2061 2060 7072 6f70 6572  d emit a `proper
-0000fed0: 7479 4368 616e 6765 6460 2073 6967 6e61  tyChanged` signa
-0000fee0: 6c2e 2222 220d 0a20 2020 2020 2020 2069  l."""..        i
-0000fef0: 6620 7365 6c66 2e67 6574 466f 6375 7344  f self.getFocusD
-0000ff00: 6576 6963 6528 2920 213d 2066 6f63 7573  evice() != focus
-0000ff10: 4c61 6265 6c3a 0d0a 2020 2020 2020 2020  Label:..        
-0000ff20: 2020 2020 7375 7065 7228 292e 7365 7446      super().setF
-0000ff30: 6f63 7573 4465 7669 6365 2866 6f63 7573  ocusDevice(focus
-0000ff40: 4c61 6265 6c29 0d0a 2020 2020 2020 2020  Label)..        
-0000ff50: 2020 2020 7365 6c66 2e65 7665 6e74 732e      self.events.
-0000ff60: 7072 6f70 6572 7479 4368 616e 6765 642e  propertyChanged.
-0000ff70: 656d 6974 2822 436f 7265 222c 2022 466f  emit("Core", "Fo
-0000ff80: 6375 7322 2c20 666f 6375 734c 6162 656c  cus", focusLabel
-0000ff90: 290d 0a0d 0a20 2020 2064 6566 2073 6176  )....    def sav
-0000ffa0: 6553 7973 7465 6d43 6f6e 6669 6775 7261  eSystemConfigura
-0000ffb0: 7469 6f6e 2873 656c 662c 2066 696c 656e  tion(self, filen
-0000ffc0: 616d 653a 2073 7472 2920 2d3e 204e 6f6e  ame: str) -> Non
-0000ffd0: 653a 0d0a 2020 2020 2020 2020 2222 2253  e:..        """S
-0000ffe0: 6176 6573 2074 6865 2063 7572 7265 6e74  aves the current
-0000fff0: 2073 7973 7465 6d20 636f 6e66 6967 7572   system configur
-00010000: 6174 696f 6e20 746f 2061 2074 6578 7420  ation to a text 
-00010010: 6669 6c65 2e0d 0a0d 0a20 2020 2020 2020  file.....       
-00010020: 202a 2a57 6879 204f 7665 7272 6964 653f   **Why Override?
-00010030: 2a2a 2054 6f20 616c 736f 2073 6176 6520  ** To also save 
-00010040: 7069 7865 6c20 7369 7a65 2063 6f6e 6669  pixel size confi
-00010050: 6775 7261 7469 6f6e 732e 0d0a 2020 2020  gurations...    
-00010060: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00010070: 2073 7570 6572 2829 2e73 6176 6553 7973   super().saveSys
-00010080: 7465 6d43 6f6e 6669 6775 7261 7469 6f6e  temConfiguration
-00010090: 2866 696c 656e 616d 6529 0d0a 2020 2020  (filename)..    
-000100a0: 2020 2020 7078 5f63 6f6e 6669 6773 203d      px_configs =
-000100b0: 2073 656c 662e 6765 7441 7661 696c 6162   self.getAvailab
-000100c0: 6c65 5069 7865 6c53 697a 6543 6f6e 6669  lePixelSizeConfi
-000100d0: 6773 2829 0d0a 2020 2020 2020 2020 6966  gs()..        if
-000100e0: 206e 6f74 2070 785f 636f 6e66 6967 733a   not px_configs:
-000100f0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00010100: 7475 726e 0d0a 2020 2020 2020 2020 2320  turn..        # 
-00010110: 7361 7665 5379 7374 656d 436f 6e66 6967  saveSystemConfig
-00010120: 7572 6174 696f 6e20 646f 6573 206e 6f74  uration does not
-00010130: 2073 6176 6520 7468 6520 7069 7865 6c20   save the pixel 
-00010140: 7369 7a65 2063 6f6e 6669 6720 736f 2068  size config so h
-00010150: 6572 650d 0a20 2020 2020 2020 2023 2077  ere..        # w
-00010160: 6520 6164 6420 746f 2074 6865 2073 6176  e add to the sav
-00010170: 6564 2066 696c 6520 616c 736f 2061 6e79  ed file also any
-00010180: 2070 6978 656c 2073 697a 6520 636f 6e66   pixel size conf
-00010190: 6967 2e0d 0a20 2020 2020 2020 2077 6974  ig...        wit
-000101a0: 6820 6f70 656e 2866 696c 656e 616d 652c  h open(filename,
-000101b0: 2022 6122 2920 6173 2066 3a0d 0a20 2020   "a") as f:..   
-000101c0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-000101d0: 2822 2320 5069 7865 6c53 697a 6520 7365  ("# PixelSize se
-000101e0: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
-000101f0: 2020 2020 2020 666f 7220 7078 5f63 6f6e        for px_con
-00010200: 6669 6720 696e 2070 785f 636f 6e66 6967  fig in px_config
-00010210: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00010220: 2020 2020 6461 7461 203d 2073 656c 662e      data = self.
-00010230: 6765 7450 6978 656c 5369 7a65 436f 6e66  getPixelSizeConf
-00010240: 6967 4461 7461 2870 785f 636f 6e66 6967  igData(px_config
-00010250: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010260: 2020 206f 626a 203d 2064 6174 612e 6469     obj = data.di
-00010270: 6374 2829 5b22 4f62 6a65 6374 6976 6522  ct()["Objective"
-00010280: 5d5b 224c 6162 656c 225d 0d0a 2020 2020  ]["Label"]..    
-00010290: 2020 2020 2020 2020 2020 2020 7078 5f73              px_s
-000102a0: 697a 6520 3d20 7365 6c66 2e67 6574 5069  ize = self.getPi
-000102b0: 7865 6c53 697a 6555 6d42 7949 4428 7078  xelSizeUmByID(px
-000102c0: 5f63 6f6e 6669 6729 0d0a 2020 2020 2020  _config)..      
-000102d0: 2020 2020 2020 2020 2020 7078 5f61 6666            px_aff
-000102e0: 696e 6520 3d20 7365 6c66 2e67 6574 5069  ine = self.getPi
-000102f0: 7865 6c53 697a 6541 6666 696e 6542 7949  xelSizeAffineByI
-00010300: 4428 7078 5f63 6f6e 6669 6729 0d0a 2020  D(px_config)..  
-00010310: 2020 2020 2020 2020 2020 2020 2020 6366                cf
-00010320: 6720 3d20 280d 0a20 2020 2020 2020 2020  g = (..         
-00010330: 2020 2020 2020 2020 2020 2066 225c 6e43             f"\nC
-00010340: 6f6e 6669 6750 6978 656c 5369 7a65 2c7b  onfigPixelSize,{
-00010350: 7078 5f63 6f6e 6669 677d 2c4f 626a 6563  px_config},Objec
-00010360: 7469 7665 2c4c 6162 656c 2c7b 6f62 6a7d  tive,Label,{obj}
-00010370: 5c6e 220d 0a20 2020 2020 2020 2020 2020  \n"..           
-00010380: 2020 2020 2020 2020 2066 2250 6978 656c           f"Pixel
-00010390: 5369 7a65 5f75 6d2c 7b70 785f 636f 6e66  Size_um,{px_conf
-000103a0: 6967 7d2c 7b70 785f 7369 7a65 7d5c 6e22  ig},{px_size}\n"
-000103b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000103c0: 2020 2020 2020 6622 5069 7865 6c53 697a        f"PixelSiz
-000103d0: 6541 6666 696e 652c 7b70 785f 636f 6e66  eAffine,{px_conf
-000103e0: 6967 7d2c 7b27 2c27 2e6a 6f69 6e28 6d61  ig},{','.join(ma
-000103f0: 7028 7374 722c 2070 785f 6166 6669 6e65  p(str, px_affine
-00010400: 2929 7d22 0d0a 2020 2020 2020 2020 2020  ))}"..          
-00010410: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00010420: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00010430: 2863 6667 290d 0a0d 0a20 2020 2064 6566  (cfg)....    def
-00010440: 2064 6573 6372 6962 6528 7365 6c66 2c20   describe(self, 
-00010450: 736f 7274 3a20 7374 7220 7c20 4e6f 6e65  sort: str | None
-00010460: 203d 204e 6f6e 6529 202d 3e20 4e6f 6e65   = None) -> None
-00010470: 3a0d 0a20 2020 2020 2020 2022 2222 5072  :..        """Pr
-00010480: 696e 7420 696e 666f 726d 6174 696f 6e20  int information 
-00010490: 7461 626c 6520 7769 7468 2074 6865 2063  table with the c
-000104a0: 7572 7265 6e74 2063 6f6e 6669 6775 7261  urrent configura
-000104b0: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
-000104c0: 2049 6e74 656e 6465 6420 746f 2070 726f   Intended to pro
-000104d0: 7669 6465 2061 2071 7569 636b 206f 7665  vide a quick ove
-000104e0: 7276 6965 7720 6f66 2074 6865 206d 6963  rview of the mic
-000104f0: 726f 7363 6f70 6520 636f 6e66 6967 7572  roscope configur
-00010500: 6174 696f 6e20 6475 7269 6e67 0d0a 2020  ation during..  
-00010510: 2020 2020 2020 696e 7465 7261 6374 6976        interactiv
-00010520: 6520 7465 726d 696e 616c 2075 7361 6765  e terminal usage
-00010530: 2e0d 0a0d 0a20 2020 2020 2020 203a 7370  .....        :sp
-00010540: 6172 6b6c 6573 3a20 2a54 6869 7320 6d65  arkles: *This me
-00010550: 7468 6f64 2069 7320 6e65 7720 696e 2060  thod is new in `
-00010560: 434d 4d43 6f72 6550 6c75 7360 2e2a 0d0a  CMMCorePlus`.*..
-00010570: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00010580: 2020 2020 205f 6375 7272 656e 7420 3d20       _current = 
-00010590: 7b0d 0a20 2020 2020 2020 2020 2020 2073  {..            s
-000105a0: 656c 662e 6765 7443 616d 6572 6144 6576  elf.getCameraDev
-000105b0: 6963 6528 293a 2022 4361 6d65 7261 222c  ice(): "Camera",
-000105c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000105d0: 6c66 2e67 6574 5859 5374 6167 6544 6576  lf.getXYStageDev
-000105e0: 6963 6528 293a 2022 5859 5374 6167 6522  ice(): "XYStage"
-000105f0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00010600: 656c 662e 6765 7446 6f63 7573 4465 7669  elf.getFocusDevi
-00010610: 6365 2829 3a20 2246 6f63 7573 222c 0d0a  ce(): "Focus",..
-00010620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010630: 2e67 6574 5368 7574 7465 7244 6576 6963  .getShutterDevic
-00010640: 6528 293a 2022 5368 7574 7465 7222 2c0d  e(): "Shutter",.
-00010650: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010660: 662e 6765 7453 4c4d 4465 7669 6365 2829  f.getSLMDevice()
-00010670: 3a20 2253 4c4d 222c 0d0a 2020 2020 2020  : "SLM",..      
-00010680: 2020 2020 2020 7365 6c66 2e67 6574 4761        self.getGa
-00010690: 6c76 6f44 6576 6963 6528 293a 2022 4761  lvoDevice(): "Ga
-000106a0: 6c76 6f22 2c0d 0a20 2020 2020 2020 2020  lvo",..         
-000106b0: 2020 2073 656c 662e 6765 7441 7574 6f46     self.getAutoF
-000106c0: 6f63 7573 4465 7669 6365 2829 3a20 2241  ocusDevice(): "A
-000106d0: 7574 6f46 6f63 7573 222c 0d0a 2020 2020  utoFocus",..    
-000106e0: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-000106f0: 496d 6167 6550 726f 6365 7373 6f72 4465  ImageProcessorDe
-00010700: 7669 6365 2829 3a20 2249 6d61 6765 5072  vice(): "ImagePr
-00010710: 6f63 6573 736f 7222 2c0d 0a20 2020 2020  ocessor",..     
-00010720: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
-00010730: 6461 7461 3a20 6465 6661 756c 7464 6963  data: defaultdic
-00010740: 745b 7374 722c 206c 6973 745b 7374 725d  t[str, list[str]
-00010750: 5d20 3d20 6465 6661 756c 7464 6963 7428  ] = defaultdict(
-00010760: 6c69 7374 290d 0a20 2020 2020 2020 2066  list)..        f
-00010770: 6f72 2064 6576 6963 6520 696e 2073 656c  or device in sel
-00010780: 662e 6974 6572 4465 7669 6365 7328 293a  f.iterDevices():
-00010790: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-000107a0: 7461 5b22 4465 7669 6365 204c 6162 656c  ta["Device Label
-000107b0: 225d 2e61 7070 656e 6428 6465 7669 6365  "].append(device
-000107c0: 2e6c 6162 656c 290d 0a20 2020 2020 2020  .label)..       
-000107d0: 2020 2020 2064 6174 615b 2254 7970 6522       data["Type"
-000107e0: 5d2e 6170 7065 6e64 2873 7472 2864 6576  ].append(str(dev
-000107f0: 6963 652e 7479 7065 2829 2929 0d0a 2020  ice.type()))..  
-00010800: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
-00010810: 4375 7272 656e 7422 5d2e 6170 7065 6e64  Current"].append
-00010820: 285f 6375 7272 656e 742e 6765 7428 6465  (_current.get(de
-00010830: 7669 6365 2e6c 6162 656c 2c20 2222 2929  vice.label, ""))
-00010840: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00010850: 7461 5b22 4c69 6272 6172 793a 3a44 6576  ta["Library::Dev
-00010860: 6963 654e 616d 6522 5d2e 6170 7065 6e64  iceName"].append
-00010870: 2866 227b 6465 7669 6365 2e6c 6962 7261  (f"{device.libra
-00010880: 7279 2829 7d3a 3a7b 6465 7669 6365 2e6e  ry()}::{device.n
-00010890: 616d 6528 297d 2229 0d0a 2020 2020 2020  ame()}")..      
-000108a0: 2020 2020 2020 6461 7461 5b22 4465 7363        data["Desc
-000108b0: 7269 7074 696f 6e22 5d2e 6170 7065 6e64  ription"].append
-000108c0: 2864 6576 6963 652e 6465 7363 7269 7074  (device.descript
-000108d0: 696f 6e28 2929 0d0a 0d0a 2020 2020 2020  ion())....      
-000108e0: 2020 6966 206e 6f74 2061 6e79 2864 6174    if not any(dat
-000108f0: 615b 2243 7572 7265 6e74 225d 293a 0d0a  a["Current"]):..
-00010900: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00010910: 2e70 6f70 2822 4375 7272 656e 7422 290d  .pop("Current").
-00010920: 0a0d 0a20 2020 2020 2020 2070 7269 6e74  ...        print
-00010930: 2866 227b 7365 6c66 2e67 6574 5665 7273  (f"{self.getVers
-00010940: 696f 6e49 6e66 6f28 297d 2c20 7b73 656c  ionInfo()}, {sel
-00010950: 662e 6765 7441 5049 5665 7273 696f 6e49  f.getAPIVersionI
-00010960: 6e66 6f28 297d 2229 0d0a 2020 2020 2020  nfo()}")..      
-00010970: 2020 7072 696e 7428 2241 6461 7074 6572    print("Adapter
-00010980: 2070 6174 683a 222c 2022 2c22 2e6a 6f69   path:", ",".joi
-00010990: 6e28 7365 6c66 2e67 6574 4465 7669 6365  n(self.getDevice
-000109a0: 4164 6170 7465 7253 6561 7263 6850 6174  AdapterSearchPat
-000109b0: 6873 2829 2929 0d0a 2020 2020 2020 2020  hs()))..        
-000109c0: 7072 696e 745f 7461 6275 6c61 725f 6461  print_tabular_da
-000109d0: 7461 2864 6174 612c 2073 6f72 743d 736f  ta(data, sort=so
-000109e0: 7274 290d 0a0d 0a20 2020 2064 6566 2073  rt)....    def s
-000109f0: 7461 7465 2873 656c 662c 2065 7863 6c75  tate(self, exclu
-00010a00: 6465 3a20 4974 6572 6162 6c65 5b73 7472  de: Iterable[str
-00010a10: 5d20 3d20 2829 2920 2d3e 2053 7461 7465  ] = ()) -> State
-00010a20: 4469 6374 3a0d 0a20 2020 2020 2020 2022  Dict:..        "
-00010a30: 2222 5265 7475 726e 2060 5374 6174 6544  ""Return `StateD
-00010a40: 6963 7460 2077 6974 6820 636f 6d6d 6f6e  ict` with common
-00010a50: 6c79 2061 6363 6573 7365 6420 7374 6174  ly accessed stat
-00010a60: 6520 7661 6c75 6573 2e0d 0a0d 0a20 2020  e values.....   
-00010a70: 2020 2020 203a 7370 6172 6b6c 6573 3a20       :sparkles: 
-00010a80: 2a54 6869 7320 6d65 7468 6f64 2069 7320  *This method is 
-00010a90: 6e65 7720 696e 2060 434d 4d43 6f72 6550  new in `CMMCoreP
-00010aa0: 6c75 7360 2e20 4974 2069 7320 6120 6269  lus`. It is a bi
-00010ab0: 7420 6661 7374 6572 0d0a 2020 2020 2020  t faster..      
-00010ac0: 2020 7468 616e 205b 6067 6574 5379 7374    than [`getSyst
-00010ad0: 656d 5374 6174 6560 5d5b 7079 6d6d 636f  emState`][pymmco
-00010ae0: 7265 5f70 6c75 732e 434d 4d43 6f72 6550  re_plus.CMMCoreP
-00010af0: 6c75 732e 6765 7453 7973 7465 6d53 7461  lus.getSystemSta
-00010b00: 7465 5d2e 2a0d 0a0d 0a20 2020 2020 2020  te].*....       
-00010b10: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-00010b20: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
-00010b30: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
-00010b40: 203a 2049 7465 7261 626c 655b 7374 725d   : Iterable[str]
-00010b50: 0d0a 2020 2020 2020 2020 2020 2020 4c69  ..            Li
-00010b60: 7374 206f 6620 7072 6f70 6572 7469 6573  st of properties
-00010b70: 2074 6f20 6578 636c 7564 6520 7768 656e   to exclude when
-00010b80: 2067 6174 6865 7269 6e67 2073 7461 7465   gathering state
-00010b90: 2028 6d61 7920 7370 6565 6420 7468 696e   (may speed thin
-00010ba0: 6773 2075 7029 2e0d 0a20 2020 2020 2020  gs up)...       
-00010bb0: 2020 2020 2053 6565 205b 6053 7461 7465       See [`State
-00010bc0: 4469 6374 605d 5b70 796d 6d63 6f72 655f  Dict`][pymmcore_
-00010bd0: 706c 7573 2e63 6f72 652e 5f6d 6d63 6f72  plus.core._mmcor
-00010be0: 655f 706c 7573 2e53 7461 7465 4469 6374  e_plus.StateDict
-00010bf0: 5d20 666f 7220 6120 6c69 7374 206f 660d  ] for a list of.
-00010c00: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
-00010c10: 7320 7468 6174 2063 616e 2062 6520 6578  s that can be ex
-00010c20: 636c 7564 6564 2e0d 0a0d 0a20 2020 2020  cluded.....     
-00010c30: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00010c40: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00010c50: 2020 2020 2053 7461 7465 4469 6374 0d0a       StateDict..
-00010c60: 2020 2020 2020 2020 2020 2020 4120 6469              A di
-00010c70: 6374 696f 6e61 7279 206f 6620 636f 6d6d  ctionary of comm
-00010c80: 6f6e 6c79 2061 6363 6573 7365 6420 7374  only accessed st
-00010c90: 6174 6520 7661 6c75 6573 2e0d 0a20 2020  ate values...   
-00010ca0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00010cb0: 2020 2320 6170 7072 6f78 2072 6574 7269    # approx retri
-00010cc0: 6576 616c 2063 6f73 7420 696e 2063 6f6d  eval cost in com
-00010cd0: 6d65 6e74 2028 666f 7220 6465 6d6f 4361  ment (for demoCa
-00010ce0: 6d29 0d0a 2020 2020 2020 2020 6578 636c  m)..        excl
-00010cf0: 7564 6520 3d20 7365 7428 6578 636c 7564  ude = set(exclud
-00010d00: 6529 0d0a 2020 2020 2020 2020 7374 6174  e)..        stat
-00010d10: 653a 2064 6963 7420 3d20 7b7d 0d0a 2020  e: dict = {}..  
-00010d20: 2020 2020 2020 666f 7220 6174 7472 2069        for attr i
-00010d30: 6e20 280d 0a20 2020 2020 2020 2020 2020  n (..           
-00010d40: 2022 4175 746f 466f 6375 7344 6576 6963   "AutoFocusDevic
-00010d50: 6522 2c20 2023 2031 3530 206e 730d 0a20  e",  # 150 ns.. 
-00010d60: 2020 2020 2020 2020 2020 2022 4279 7465             "Byte
-00010d70: 7350 6572 5069 7865 6c22 2c20 2023 2031  sPerPixel",  # 1
-00010d80: 3439 206e 730d 0a20 2020 2020 2020 2020  49 ns..         
-00010d90: 2020 2022 4361 6d65 7261 4368 616e 6e65     "CameraChanne
-00010da0: 6c4e 616d 6573 222c 2020 2320 3120 c2b5  lNames",  # 1 ..
-00010db0: 730d 0a20 2020 2020 2020 2020 2020 2022  s..            "
-00010dc0: 4361 6d65 7261 4465 7669 6365 222c 2020  CameraDevice",  
-00010dd0: 2320 3135 3920 6e73 0d0a 2020 2020 2020  # 159 ns..      
-00010de0: 2020 2020 2020 2244 6174 6574 696d 6522        "Datetime"
-00010df0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00010e00: 4578 706f 7375 7265 222c 2020 2320 3732  Exposure",  # 72
-00010e10: 3620 6e73 0d0a 2020 2020 2020 2020 2020  6 ns..          
-00010e20: 2020 2246 6f63 7573 4465 7669 6365 222c    "FocusDevice",
-00010e30: 2020 2320 3131 3220 6e73 0d0a 2020 2020    # 112 ns..    
-00010e40: 2020 2020 2020 2020 2247 616c 766f 4465          "GalvoDe
-00010e50: 7669 6365 222c 2020 2320 3130 3920 6e73  vice",  # 109 ns
-00010e60: 0d0a 2020 2020 2020 2020 2020 2020 2249  ..            "I
-00010e70: 6d61 6765 4269 7444 6570 7468 222c 2020  mageBitDepth",  
-00010e80: 2320 3134 3720 6e73 0d0a 2020 2020 2020  # 147 ns..      
-00010e90: 2020 2020 2020 2249 6d61 6765 4865 6967        "ImageHeig
-00010ea0: 6874 222c 2020 2320 3136 3420 6e73 0d0a  ht",  # 164 ns..
-00010eb0: 2020 2020 2020 2020 2020 2020 2249 6d61              "Ima
-00010ec0: 6765 5072 6f63 6573 736f 7244 6576 6963  geProcessorDevic
-00010ed0: 6522 2c20 2023 2031 3130 206e 730d 0a20  e",  # 110 ns.. 
-00010ee0: 2020 2020 2020 2020 2020 2022 496d 6167             "Imag
-00010ef0: 6557 6964 7468 222c 2020 2320 3137 3220  eWidth",  # 172 
-00010f00: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
-00010f10: 2250 6978 656c 5369 7a65 556d 222c 2020  "PixelSizeUm",  
-00010f20: 2320 322e 3220 c2b5 730d 0a20 2020 2020  # 2.2 ..s..     
-00010f30: 2020 2020 2020 2022 5368 7574 7465 7244         "ShutterD
-00010f40: 6576 6963 6522 2c20 2023 2031 3532 206e  evice",  # 152 n
-00010f50: 730d 0a20 2020 2020 2020 2020 2020 2022  s..            "
-00010f60: 534c 4d44 6576 6963 6522 2c20 2023 2031  SLMDevice",  # 1
-00010f70: 3130 206e 730d 0a20 2020 2020 2020 2020  10 ns..         
-00010f80: 2020 2022 5859 506f 7369 7469 6f6e 222c     "XYPosition",
-00010f90: 2020 2320 312e 3120 c2b5 730d 0a20 2020    # 1.1 ..s..   
-00010fa0: 2020 2020 2020 2020 2022 5859 5374 6167           "XYStag
-00010fb0: 6544 6576 6963 6522 2c20 2023 2031 3536  eDevice",  # 156
-00010fc0: 206e 730d 0a20 2020 2020 2020 2020 2020   ns..           
-00010fd0: 2022 5a50 6f73 6974 696f 6e22 2c20 2023   "ZPosition",  #
-00010fe0: 2031 2e30 3320 c2b5 730d 0a20 2020 2020   1.03 ..s..     
-00010ff0: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00011000: 2020 2069 6620 6174 7472 206e 6f74 2069     if attr not i
-00011010: 6e20 6578 636c 7564 653a 0d0a 2020 2020  n exclude:..    
-00011020: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00011030: 7474 7220 3d3d 2022 4461 7465 7469 6d65  ttr == "Datetime
-00011040: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00011050: 2020 2020 2020 2020 7374 6174 655b 6174          state[at
-00011060: 7472 5d20 3d20 7374 7228 6461 7465 7469  tr] = str(dateti
-00011070: 6d65 2e6e 6f77 2829 290d 0a20 2020 2020  me.now())..     
-00011080: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00011090: 6174 7472 203d 3d20 2250 6978 656c 5369  attr == "PixelSi
-000110a0: 7a65 556d 223a 0d0a 2020 2020 2020 2020  zeUm":..        
-000110b0: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-000110c0: 655b 6174 7472 5d20 3d20 7365 6c66 2e67  e[attr] = self.g
-000110d0: 6574 5069 7865 6c53 697a 6555 6d28 5472  etPixelSizeUm(Tr
-000110e0: 7565 2920 2023 2054 7275 653d 3d63 6163  ue)  # True==cac
-000110f0: 6865 640d 0a20 2020 2020 2020 2020 2020  hed..           
-00011100: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00011130: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00011140: 6174 655b 6174 7472 5d20 3d20 6765 7461  ate[attr] = geta
-00011150: 7474 7228 7365 6c66 2c20 6622 6765 747b  ttr(self, f"get{
-00011160: 6174 7472 7d22 2928 290d 0a20 2020 2020  attr}")()..     
-00011170: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00011180: 7863 6570 7420 5275 6e74 696d 6545 7272  xcept RuntimeErr
-00011190: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-000111a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000111b0: 7469 6e75 650d 0a20 2020 2020 2020 2072  tinue..        r
-000111c0: 6574 7572 6e20 6361 7374 2822 5374 6174  eturn cast("Stat
-000111d0: 6544 6963 7422 2c20 7374 6174 6529 0d0a  eDict", state)..
-000111e0: 0d0a 2020 2020 4063 6f6e 7465 7874 6d61  ..    @contextma
-000111f0: 6e61 6765 720d 0a20 2020 2064 6566 205f  nager..    def _
-00011200: 7072 6f70 6572 7479 5f63 6861 6e67 655f  property_change_
-00011210: 656d 6973 7369 6f6e 5f65 6e73 7572 6564  emission_ensured
-00011220: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-00011230: 2064 6576 6963 653a 2073 7472 2c20 7072   device: str, pr
-00011240: 6f70 6572 7469 6573 3a20 5365 7175 656e  operties: Sequen
-00011250: 6365 5b73 7472 5d0d 0a20 2020 2029 202d  ce[str]..    ) -
-00011260: 3e20 4974 6572 6174 6f72 5b4e 6f6e 655d  > Iterator[None]
-00011270: 3a0d 0a20 2020 2020 2020 2022 2222 436f  :..        """Co
-00011280: 6e74 6578 7420 7468 6174 2065 6d69 7473  ntext that emits
-00011290: 2065 7665 6e74 7320 6966 2061 6e79 206f   events if any o
-000112a0: 6620 6070 726f 7065 7274 6965 7360 2063  f `properties` c
-000112b0: 6861 6e67 6520 6f6e 2064 6576 6963 652e  hange on device.
-000112c0: 0d0a 0d0a 2020 2020 2020 2020 4e4f 5445  ....        NOTE
-000112d0: 3a20 4465 7065 6e64 696e 6720 6f6e 2064  : Depending on d
-000112e0: 6576 6963 6520 6164 6170 7465 7220 6265  evice adapter be
-000112f0: 6861 7669 6f72 2074 6865 2073 6967 6e61  havior the signa
-00011300: 6c20 6d61 7920 6265 2065 6d69 7474 6564  l may be emitted
-00011310: 2074 7769 6365 2e0d 0a0d 0a20 2020 2020   twice.....     
-00011320: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-00011330: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00011340: 2d0d 0a20 2020 2020 2020 2064 6576 6963  -..        devic
-00011350: 6520 3a20 7374 720d 0a20 2020 2020 2020  e : str..       
-00011360: 2020 2020 2061 2064 6576 6963 6520 6c61       a device la
-00011370: 6265 6c0d 0a20 2020 2020 2020 2070 726f  bel..        pro
-00011380: 7065 7274 6965 7320 3a20 5365 7175 656e  perties : Sequen
-00011390: 6365 5b73 7472 5d0d 0a20 2020 2020 2020  ce[str]..       
-000113a0: 2020 2020 2061 2073 6571 7565 6e63 6520       a sequence 
-000113b0: 6f66 2070 726f 7065 7274 7920 6e61 6d65  of property name
-000113c0: 7320 746f 206d 6f6e 6974 6f72 0d0a 2020  s to monitor..  
-000113d0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000113e0: 2020 2023 206d 616b 6520 7375 7265 2074     # make sure t
-000113f0: 6861 7420 6368 616e 6769 6e67 2065 6974  hat changing eit
-00011400: 6865 7220 7374 6174 6520 6465 7669 6365  her state device
-00011410: 2070 726f 7065 7274 7920 656d 6974 7320   property emits 
-00011420: 626f 7468 2073 6967 6e61 6c73 0d0a 2020  both signals..  
-00011430: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-00011440: 2020 2020 2020 2020 6c65 6e28 7072 6f70          len(prop
-00011450: 6572 7469 6573 2920 3d3d 2031 0d0a 2020  erties) == 1..  
-00011460: 2020 2020 2020 2020 2020 616e 6420 7072            and pr
-00011470: 6f70 6572 7469 6573 5b30 5d20 696e 2053  operties[0] in S
-00011480: 5441 5445 5f50 524f 5053 0d0a 2020 2020  TATE_PROPS..    
-00011490: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
-000114a0: 2e67 6574 4465 7669 6365 5479 7065 2864  .getDeviceType(d
-000114b0: 6576 6963 6529 2069 7320 4465 7669 6365  evice) is Device
-000114c0: 5479 7065 2e53 7461 7465 4465 7669 6365  Type.StateDevice
-000114d0: 0d0a 2020 2020 2020 2020 293a 0d0a 2020  ..        ):..  
-000114e0: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
-000114f0: 7469 6573 203d 2053 5441 5445 5f50 524f  ties = STATE_PRO
-00011500: 5053 0d0a 0d0a 2020 2020 2020 2020 6265  PS....        be
-00011510: 666f 7265 203d 205b 7365 6c66 2e67 6574  fore = [self.get
-00011520: 5072 6f70 6572 7479 2864 6576 6963 652c  Property(device,
-00011530: 2070 2920 666f 7220 7020 696e 2070 726f   p) for p in pro
-00011540: 7065 7274 6965 735d 0d0a 2020 2020 2020  perties]..      
-00011550: 2020 7769 7468 205f 626c 6f63 6b53 6967    with _blockSig
-00011560: 6e61 6c28 7365 6c66 2e65 7665 6e74 732c  nal(self.events,
-00011570: 2073 656c 662e 6576 656e 7473 2e70 726f   self.events.pro
-00011580: 7065 7274 7943 6861 6e67 6564 293a 0d0a  pertyChanged):..
-00011590: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-000115a0: 640d 0a20 2020 2020 2020 2061 6674 6572  d..        after
-000115b0: 203d 205b 7365 6c66 2e67 6574 5072 6f70   = [self.getProp
-000115c0: 6572 7479 2864 6576 6963 652c 2070 2920  erty(device, p) 
-000115d0: 666f 7220 7020 696e 2070 726f 7065 7274  for p in propert
-000115e0: 6965 735d 0d0a 2020 2020 2020 2020 6966  ies]..        if
-000115f0: 2062 6566 6f72 6520 213d 2061 6674 6572   before != after
-00011600: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00011610: 6f72 2069 2c20 7661 6c20 696e 2065 6e75  or i, val in enu
-00011620: 6d65 7261 7465 2861 6674 6572 293a 0d0a  merate(after):..
-00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011640: 7365 6c66 2e65 7665 6e74 732e 7072 6f70  self.events.prop
-00011650: 6572 7479 4368 616e 6765 642e 656d 6974  ertyChanged.emit
-00011660: 2864 6576 6963 652c 2070 726f 7065 7274  (device, propert
-00011670: 6965 735b 695d 2c20 7661 6c29 0d0a 0d0a  ies[i], val)....
-00011680: 2020 2020 4063 6f6e 7465 7874 6d61 6e61      @contextmana
-00011690: 6765 720d 0a20 2020 2064 6566 2073 6574  ger..    def set
-000116a0: 436f 6e74 6578 7428 7365 6c66 2c20 2a2a  Context(self, **
-000116b0: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
-000116c0: 4974 6572 6174 6f72 5b4e 6f6e 655d 3a0d  Iterator[None]:.
-000116d0: 0a20 2020 2020 2020 2022 2222 5365 7420  .        """Set 
-000116e0: 636f 7265 2070 726f 7065 7274 6965 7320  core properties 
-000116f0: 696e 2061 2063 6f6e 7465 7874 2072 6573  in a context res
-00011700: 746f 7269 6e67 2074 6865 2069 6e69 7469  toring the initi
-00011710: 616c 2076 616c 7565 7320 6f6e 2065 7869  al values on exi
-00011720: 742e 0d0a 0d0a 2020 2020 2020 2020 3a73  t.....        :s
-00011730: 7061 726b 6c65 733a 202a 5468 6973 206d  parkles: *This m
-00011740: 6574 686f 6420 6973 206e 6577 2069 6e20  ethod is new in 
-00011750: 6043 4d4d 436f 7265 506c 7573 602e 2a0d  `CMMCorePlus`.*.
-00011760: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00011770: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-00011780: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00011790: 2020 202a 2a6b 7761 7267 7320 3a20 416e     **kwargs : An
-000117a0: 790d 0a20 2020 2020 2020 2020 2020 204b  y..            K
-000117b0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-000117c0: 206d 6179 2062 6520 616e 7920 604e 616d   may be any `Nam
-000117d0: 6560 2066 6f72 2077 6869 6368 2060 6765  e` for which `ge
-000117e0: 743c 4e61 6d65 3e60 2061 6e64 2060 7365  t<Name>` and `se
-000117f0: 743c 4e61 6d65 3e60 0d0a 2020 2020 2020  t<Name>`..      
-00011800: 2020 2020 2020 6d65 7468 6f64 7320 6578        methods ex
-00011810: 6973 742e 2020 466f 7220 6578 616d 706c  ist.  For exampl
-00011820: 652c 2060 7365 7443 6f6e 7465 7874 2865  e, `setContext(e
-00011830: 7870 6f73 7572 653d 3130 2960 2077 696c  xposure=10)` wil
-00011840: 6c20 6361 6c6c 0d0a 2020 2020 2020 2020  l call..        
-00011850: 2020 2020 6073 6574 4578 706f 7375 7265      `setExposure
-00011860: 2831 3029 6020 7768 656e 2065 6e74 6572  (10)` when enter
-00011870: 696e 6720 7468 6520 636f 6e74 6578 7420  ing the context 
-00011880: 616e 6420 6073 6574 4578 706f 7375 7265  and `setExposure
-00011890: 283c 696e 6974 6961 6c3e 2960 0d0a 2020  (<initial>)`..  
-000118a0: 2020 2020 2020 2020 2020 7768 656e 2065            when e
-000118b0: 7869 7469 6e67 2074 6865 2063 6f6e 7465  xiting the conte
-000118c0: 7874 2e0d 0a0d 0a20 2020 2020 2020 2045  xt.....        E
-000118d0: 7861 6d70 6c65 730d 0a20 2020 2020 2020  xamples..       
-000118e0: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
-000118f0: 2020 2060 6060 7079 7468 6f6e 0d0a 2020     ```python..  
-00011900: 2020 2020 2020 636f 7265 203d 2043 4d4d        core = CMM
-00011910: 436f 7265 506c 7573 2e69 6e73 7461 6e63  CorePlus.instanc
-00011920: 6528 290d 0a0d 0a20 2020 2020 2020 2077  e()....        w
-00011930: 6974 6820 636f 7265 2e73 6574 436f 6e74  ith core.setCont
-00011940: 6578 7428 6175 746f 5368 7574 7465 723d  ext(autoShutter=
-00011950: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
-00011960: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
-00011970: 636f 7265 2e67 6574 4175 746f 5368 7574  core.getAutoShut
-00011980: 7465 7228 290d 0a20 2020 2020 2020 2020  ter()..         
-00011990: 2020 2023 2064 6f20 6f74 6865 7220 7374     # do other st
-000119a0: 7566 660d 0a20 2020 2020 2020 2020 2020  uff..           
-000119b0: 202e 2e2e 0d0a 0d0a 2020 2020 2020 2020   .......        
-000119c0: 2320 6175 746f 5368 7574 7465 7220 6973  # autoShutter is
-000119d0: 2072 6573 746f 7265 6420 746f 2069 7473   restored to its
-000119e0: 206f 7269 6769 6e61 6c20 7661 6c75 6520   original value 
-000119f0: 7768 656e 2074 6865 2063 6f6e 7465 7874  when the context
-00011a00: 2065 7869 7473 0d0a 2020 2020 2020 2020   exits..        
-00011a10: 6173 7365 7274 2063 6f72 652e 6765 7441  assert core.getA
-00011a20: 7574 6f53 6875 7474 6572 2829 0d0a 2020  utoShutter()..  
-00011a30: 2020 2020 2020 6060 600d 0a20 2020 2020        ```..     
-00011a40: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00011a50: 6f72 6967 5f76 616c 7565 7320 3d20 7b7d  orig_values = {}
-00011a60: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00011a70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00011a80: 6e61 6d65 2c20 7620 696e 206b 7761 7267  name, v in kwarg
-00011a90: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
-00011aa0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00011ab0: 203d 206e 616d 655b 305d 2e75 7070 6572   = name[0].upper
-00011ac0: 2829 202b 206e 616d 655b 313a 5d0d 0a20  () + name[1:].. 
-00011ad0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00011ae0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00011af0: 2020 2020 2020 2020 206f 7269 675f 7661           orig_va
-00011b00: 6c75 6573 5b6e 616d 655d 203d 2067 6574  lues[name] = get
-00011b10: 6174 7472 2873 656c 662c 2066 2267 6574  attr(self, f"get
-00011b20: 7b6e 616d 657d 2229 2829 0d0a 2020 2020  {name}")()..    
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 6765 7461 7474 7228 7365 6c66 2c20 6622  getattr(self, f"
-00011b50: 7365 747b 6e61 6d65 7d22 2928 7629 0d0a  set{name}")(v)..
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b70: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
-00011b80: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-00011b90: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00011ba0: 6572 2e77 6172 6e69 6e67 2866 227b 6e61  er.warning(f"{na
-00011bb0: 6d65 7d20 6973 206e 6f74 2061 2076 616c  me} is not a val
-00011bc0: 6964 2070 726f 7065 7274 792c 2073 6b69  id property, ski
-00011bd0: 7070 696e 672e 2229 0d0a 2020 2020 2020  pping.")..      
-00011be0: 2020 2020 2020 7969 656c 640d 0a20 2020        yield..   
-00011bf0: 2020 2020 2066 696e 616c 6c79 3a0d 0a20       finally:.. 
-00011c00: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00011c10: 2c20 7620 696e 206f 7269 675f 7661 6c75  , v in orig_valu
-00011c20: 6573 2e69 7465 6d73 2829 3a0d 0a20 2020  es.items():..   
-00011c30: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-00011c40: 6820 7375 7070 7265 7373 2841 7474 7269  h suppress(Attri
-00011c50: 6275 7465 4572 726f 7229 3a0d 0a20 2020  buteError):..   
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2067 6574 6174 7472 2873 656c 662c 2066   getattr(self, f
-00011c80: 2273 6574 7b6b 7d22 2928 7629 0d0a 0d0a  "set{k}")(v)....
-00011c90: 2020 2020 6465 6620 6361 6e53 6571 7565      def canSeque
-00011ca0: 6e63 6545 7665 6e74 7328 0d0a 2020 2020  nceEvents(..    
-00011cb0: 2020 2020 7365 6c66 2c20 6531 3a20 4d44      self, e1: MD
-00011cc0: 4145 7665 6e74 2c20 6532 3a20 4d44 4145  AEvent, e2: MDAE
-00011cd0: 7665 6e74 2c20 6375 725f 6c65 6e67 7468  vent, cur_length
-00011ce0: 3a20 696e 7420 3d20 2d31 0d0a 2020 2020  : int = -1..    
-00011cf0: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
-00011d00: 2020 2020 2222 2243 6865 636b 2077 6865      """Check whe
-00011d10: 7468 6572 2074 776f 205b 6075 7365 712e  ther two [`useq.
-00011d20: 4d44 4145 7665 6e74 605d 5b5d 2061 7265  MDAEvent`][] are
-00011d30: 2073 6571 7565 6e63 6561 626c 6520 6279   sequenceable by
-00011d40: 2074 6869 7320 636f 7265 2069 6e73 7461   this core insta
-00011d50: 6e63 652e 0d0a 0d0a 2020 2020 2020 2020  nce.....        
-00011d60: 4d69 6372 6f2d 6d61 6e61 6765 7220 6361  Micro-manager ca
-00011d70: 6c6c 7320 6861 7264 7761 7265 2074 7269  lls hardware tri
-00011d80: 6767 6572 696e 6720 2273 6571 7565 6e63  ggering "sequenc
-00011d90: 696e 6722 2e20 2054 776f 2065 7665 6e74  ing".  Two event
-00011da0: 7320 6361 6e20 6265 0d0a 2020 2020 2020  s can be..      
-00011db0: 2020 7365 7175 656e 6365 6420 6966 202a    sequenced if *
-00011dc0: 616c 6c2a 2064 6576 6963 6520 7072 6f70  all* device prop
-00011dd0: 6572 7469 6573 2074 6861 7420 6172 6520  erties that are 
-00011de0: 6368 616e 6769 6e67 2062 6574 7765 656e  changing between
-00011df0: 2074 6865 2066 6972 7374 2061 6e64 0d0a   the first and..
-00011e00: 2020 2020 2020 2020 7365 636f 6e64 2065          second e
-00011e10: 7665 6e74 2073 7570 706f 7274 2073 6571  vent support seq
-00011e20: 7565 6e63 696e 672e 0d0a 0d0a 2020 2020  uencing.....    
-00011e30: 2020 2020 4966 2060 6375 725f 6c65 6e67      If `cur_leng
-00011e40: 7468 6020 6973 2070 726f 7669 6465 642c  th` is provided,
-00011e50: 2069 7420 6973 2075 7365 6420 746f 2064   it is used to d
-00011e60: 6574 6572 6d69 6e65 2069 6620 7468 6520  etermine if the 
-00011e70: 7365 7175 656e 6365 2069 730d 0a20 2020  sequence is..   
-00011e80: 2020 2020 2022 6675 6c6c 2220 2869 2e65       "full" (i.e
-00011e90: 2e20 7468 6520 7365 7175 656e 6365 2069  . the sequence i
-00011ea0: 7320 616c 7265 6164 7920 6174 2074 6865  s already at the
-00011eb0: 206d 6178 696d 756d 206c 656e 6774 6829   maximum length)
-00011ec0: 2061 7320 6465 7465 726d 696e 6564 2062   as determined b
-00011ed0: 790d 0a20 2020 2020 2020 2074 6865 2060  y..        the `
-00011ee0: 2e2e 2e53 6571 7565 6e63 654d 6178 4c65  ...SequenceMaxLe
-00011ef0: 6e67 7468 2829 6020 6d65 7468 6f64 2063  ngth()` method c
-00011f00: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
-00011f10: 7468 6520 6465 7669 6365 2070 726f 7065  the device prope
-00011f20: 7274 792e 0d0a 0d0a 2020 2020 2020 2020  rty.....        
-00011f30: 5365 653a 203c 6874 7470 733a 2f2f 6d69  See: <https://mi
-00011f40: 6372 6f2d 6d61 6e61 6765 722e 6f72 672f  cro-manager.org/
-00011f50: 4861 7264 7761 7265 2d62 6173 6564 5f53  Hardware-based_S
-00011f60: 796e 6368 726f 6e69 7a61 7469 6f6e 5f69  ynchronization_i
-00011f70: 6e5f 4d69 6372 6f2d 4d61 6e61 6765 723e  n_Micro-Manager>
-00011f80: 0d0a 0d0a 2020 2020 2020 2020 3a73 7061  ....        :spa
-00011f90: 726b 6c65 733a 202a 5468 6973 206d 6574  rkles: *This met
-00011fa0: 686f 6420 6973 206e 6577 2069 6e20 6043  hod is new in `C
-00011fb0: 4d4d 436f 7265 506c 7573 602e 2a0d 0a0d  MMCorePlus`.*...
-00011fc0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00011fd0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-00011fe0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-00011ff0: 2065 3120 3a20 4d44 4145 7665 6e74 0d0a   e1 : MDAEvent..
-00012000: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00012010: 6669 7273 7420 6576 656e 742e 0d0a 2020  first event...  
-00012020: 2020 2020 2020 6532 203a 204d 4441 4576        e2 : MDAEv
-00012030: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-00012040: 2054 6865 2073 6563 6f6e 6420 6576 656e   The second even
-00012050: 742e 0d0a 2020 2020 2020 2020 6375 725f  t...        cur_
-00012060: 6c65 6e67 7468 203a 2069 6e74 0d0a 2020  length : int..  
-00012070: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
-00012080: 7272 656e 7420 6c65 6e67 7468 206f 6620  rrent length of 
-00012090: 7468 6520 7365 7175 656e 6365 2e20 2055  the sequence.  U
-000120a0: 7365 6420 7768 656e 2063 6865 636b 696e  sed when checkin
-000120b0: 670d 0a20 2020 2020 2020 2020 2020 2060  g..            `
-000120c0: 2e67 6574 3c2e 2e2e 3e53 6571 7565 6e63  .get<...>Sequenc
-000120d0: 654d 6178 4c65 6e67 7468 6020 666f 7220  eMaxLength` for 
-000120e0: 6120 6769 7665 6e20 7072 6f70 6572 7479  a given property
-000120f0: 2e20 4966 2074 6865 2063 7572 7265 6e74  . If the current
-00012100: 206c 656e 6774 680d 0a20 2020 2020 2020   length..       
-00012110: 2020 2020 2069 7320 6772 6561 7465 7220       is greater 
-00012120: 7468 616e 2074 6865 206d 6178 206c 656e  than the max len
-00012130: 6774 682c 2074 6865 2065 7665 6e74 7320  gth, the events 
-00012140: 6361 6e6e 6f74 2062 6520 7365 7175 656e  cannot be sequen
-00012150: 6365 642e 2042 7920 6465 6661 756c 740d  ced. By default.
-00012160: 0a20 2020 2020 2020 2020 2020 202d 312c  .            -1,
-00012170: 2077 6869 6368 206d 6561 6e73 2074 6865   which means the
-00012180: 2063 7572 7265 6e74 206c 656e 6774 6820   current length 
-00012190: 6973 206e 6f74 2063 6865 636b 6564 2e0d  is not checked..
-000121a0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000121b0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-000121c0: 2d2d 2d0d 0a20 2020 2020 2020 2062 6f6f  ---..        boo
-000121d0: 6c0d 0a20 2020 2020 2020 2020 2020 2054  l..            T
-000121e0: 7275 6520 6966 2074 6865 2065 7665 6e74  rue if the event
-000121f0: 7320 6361 6e20 6265 2073 6571 7565 6e63  s can be sequenc
-00012200: 6564 2c20 4661 6c73 6520 6f74 6865 7277  ed, False otherw
-00012210: 6973 652e 0d0a 0d0a 2020 2020 2020 2020  ise.....        
-00012220: 4578 616d 706c 6573 0d0a 2020 2020 2020  Examples..      
-00012230: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
-00012240: 2020 2020 2121 2120 6e6f 7465 0d0a 0d0a      !!! note....
-00012250: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00012260: 7265 7375 6c74 7320 6865 7265 2077 696c  results here wil
-00012270: 6c20 6465 7065 6e64 206f 6e20 7468 6520  l depend on the 
-00012280: 6375 7272 656e 7420 7374 6174 6520 6f66  current state of
-00012290: 2074 6865 2063 6f72 6520 616e 6420 6465   the core and de
-000122a0: 7669 6365 732e 0d0a 0d0a 2020 2020 2020  vices.....      
-000122b0: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
-000122c0: 2020 2020 203e 3e3e 2066 726f 6d20 7573       >>> from us
-000122d0: 6571 2069 6d70 6f72 7420 4d44 4145 7665  eq import MDAEve
-000122e0: 6e74 0d0a 2020 2020 2020 2020 3e3e 3e20  nt..        >>> 
-000122f0: 636f 7265 203d 2043 4d4d 436f 7265 506c  core = CMMCorePl
-00012300: 7573 2e69 6e73 7461 6e63 6528 290d 0a20  us.instance().. 
-00012310: 2020 2020 2020 203e 3e3e 2063 6f72 652e         >>> core.
-00012320: 6c6f 6164 5379 7374 656d 436f 6e66 6967  loadSystemConfig
-00012330: 7572 6174 696f 6e28 290d 0a20 2020 2020  uration()..     
-00012340: 2020 203e 3e3e 2063 6f72 652e 6361 6e53     >>> core.canS
-00012350: 6571 7565 6e63 6545 7665 6e74 7328 4d44  equenceEvents(MD
-00012360: 4145 7665 6e74 2829 2c20 4d44 4145 7665  AEvent(), MDAEve
-00012370: 6e74 2829 290d 0a20 2020 2020 2020 2054  nt())..        T
-00012380: 7275 650d 0a20 2020 2020 2020 203e 3e3e  rue..        >>>
-00012390: 2063 6f72 652e 6361 6e53 6571 7565 6e63   core.canSequenc
-000123a0: 6545 7665 6e74 7328 4d44 4145 7665 6e74  eEvents(MDAEvent
-000123b0: 2878 5f70 6f73 3d31 292c 204d 4441 4576  (x_pos=1), MDAEv
-000123c0: 656e 7428 785f 706f 733d 3229 290d 0a20  ent(x_pos=2)).. 
-000123d0: 2020 2020 2020 2046 616c 7365 0d0a 2020         False..  
-000123e0: 2020 2020 2020 3e3e 3e20 636f 7265 2e63        >>> core.c
-000123f0: 616e 5365 7175 656e 6365 4576 656e 7473  anSequenceEvents
-00012400: 280d 0a20 2020 2020 2020 202e 2e2e 2020  (..        ...  
-00012410: 2020 204d 4441 4576 656e 7428 6368 616e     MDAEvent(chan
-00012420: 6e65 6c3d 7b27 636f 6e66 6967 273a 2027  nel={'config': '
-00012430: 4441 5049 277d 292c 0d0a 2020 2020 2020  DAPI'}),..      
-00012440: 2020 2e2e 2e20 2020 2020 4d44 4145 7665    ...     MDAEve
-00012450: 6e74 2863 6861 6e6e 656c 3d7b 2763 6f6e  nt(channel={'con
-00012460: 6669 6727 3a20 2746 4954 4327 7d29 0d0a  fig': 'FITC'})..
-00012470: 2020 2020 2020 2020 2e2e 2e20 290d 0a20          ... ).. 
-00012480: 2020 2020 2020 2046 616c 7365 0d0a 2020         False..  
-00012490: 2020 2020 2020 6060 600d 0a20 2020 2020        ```..     
-000124a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000124b0: 7265 7475 726e 2063 616e 5f73 6571 7565  return can_seque
-000124c0: 6e63 655f 6576 656e 7473 2873 656c 662c  nce_events(self,
-000124d0: 2065 312c 2065 322c 2063 7572 5f6c 656e   e1, e2, cur_len
-000124e0: 6774 6829 0d0a 0d0a 0d0a 666f 7220 6e61  gth)......for na
-000124f0: 6d65 2069 6e20 280d 0a20 2020 2022 6765  me in (..    "ge
-00012500: 7443 6f6e 6669 6744 6174 6122 2c0d 0a20  tConfigData",.. 
-00012510: 2020 2022 6765 7443 6f6e 6669 6747 726f     "getConfigGro
-00012520: 7570 5374 6174 6522 2c0d 0a20 2020 2022  upState",..    "
-00012530: 6765 7443 6f6e 6669 6747 726f 7570 5374  getConfigGroupSt
-00012540: 6174 6546 726f 6d43 6163 6865 222c 0d0a  ateFromCache",..
-00012550: 2020 2020 2267 6574 436f 6e66 6967 5374      "getConfigSt
-00012560: 6174 6522 2c0d 0a20 2020 2022 6765 7453  ate",..    "getS
-00012570: 7973 7465 6d53 7461 7465 222c 0d0a 2020  ystemState",..  
-00012580: 2020 2267 6574 5379 7374 656d 5374 6174    "getSystemStat
-00012590: 6543 6163 6865 222c 0d0a 293a 0d0a 2020  eCache",..):..  
-000125a0: 2020 6e61 7469 7665 5f64 6f63 203d 2067    native_doc = g
-000125b0: 6574 6174 7472 2870 796d 6d63 6f72 652e  etattr(pymmcore.
-000125c0: 434d 4d43 6f72 652c 206e 616d 6529 2e5f  CMMCore, name)._
-000125d0: 5f64 6f63 5f5f 0d0a 2020 2020 6765 7461  _doc__..    geta
-000125e0: 7474 7228 434d 4d43 6f72 6550 6c75 732c  ttr(CMMCorePlus,
-000125f0: 206e 616d 6529 2e5f 5f64 6f63 5f5f 202b   name).__doc__ +
-00012600: 3d20 280d 0a20 2020 2020 2020 2022 5c6e  = (..        "\n
-00012610: 220d 0a20 2020 2020 2020 202b 206e 6174  "..        + nat
-00012620: 6976 655f 646f 630d 0a20 2020 2020 2020  ive_doc..       
-00012630: 202b 2064 6564 656e 7428 0d0a 2020 2020   + dedent(..    
-00012640: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00012650: 2042 7920 6465 6661 756c 742c 2074 6869   By default, thi
-00012660: 7320 6d65 7468 6f64 2072 6574 7572 6e73  s method returns
-00012670: 2061 2060 7079 6d6d 636f 7265 5f70 6c75   a `pymmcore_plu
-00012680: 732e 436f 6e66 6967 7572 6174 696f 6e60  s.Configuration`
-00012690: 206f 626a 6563 742c 2077 6869 6368 0d0a   object, which..
-000126a0: 2020 2020 7072 6f76 6964 6573 2073 6f6d      provides som
-000126b0: 6520 636f 6e76 656e 6965 6e63 6573 206f  e conveniences o
-000126c0: 7665 7220 7468 6520 6e61 7469 7665 2060  ver the native `
-000126d0: 7079 6d6d 636f 7265 2e43 6f6e 6669 6775  pymmcore.Configu
-000126e0: 7261 7469 6f6e 6020 6f62 6a65 6374 2c20  ration` object, 
-000126f0: 686f 7765 7665 720d 0a20 2020 2074 6869  however..    thi
-00012700: 7320 6164 6473 2061 206c 6974 746c 6520  s adds a little 
-00012710: 6f76 6572 6865 6164 2e20 5573 6520 606e  overhead. Use `n
-00012720: 6174 6976 653d 5472 7565 6020 746f 2061  ative=True` to a
-00012730: 766f 6964 2074 6865 2063 6f6e 7665 7273  void the convers
-00012740: 696f 6e2e 0d0a 2020 2020 2222 220d 0a20  ion...    """.. 
-00012750: 2020 2020 2020 2029 2e73 7472 6970 2829         ).strip()
-00012760: 0d0a 2020 2020 290d 0a0d 0a0d 0a63 6c61  ..    )......cla
-00012770: 7373 205f 4d4d 4361 6c6c 6261 636b 5265  ss _MMCallbackRe
-00012780: 6c61 7928 7079 6d6d 636f 7265 2e4d 4d45  lay(pymmcore.MME
-00012790: 7665 6e74 4361 6c6c 6261 636b 293a 0d0a  ventCallback):..
-000127a0: 2020 2020 2222 2252 656c 6179 7320 4d4d      """Relays MM
-000127b0: 4576 656e 7443 616c 6c62 6163 6b20 6d65  EventCallback me
-000127c0: 7468 6f64 7320 746f 2043 4d4d 436f 7265  thods to CMMCore
-000127d0: 506c 7573 2e73 6967 6e61 6c2e 2222 220d  Plus.signal.""".
-000127e0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-000127f0: 745f 5f28 7365 6c66 2c20 656d 6974 7465  t__(self, emitte
-00012800: 723a 2043 4d4d 436f 7265 5369 676e 616c  r: CMMCoreSignal
-00012810: 6572 293a 0d0a 2020 2020 2020 2020 7365  er):..        se
-00012820: 6c66 2e5f 656d 6974 7465 7220 3d20 656d  lf._emitter = em
-00012830: 6974 7465 720d 0a20 2020 2020 2020 2073  itter..        s
-00012840: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00012850: 290d 0a0d 0a20 2020 2040 7374 6174 6963  )....    @static
-00012860: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-00012870: 5f6d 616b 655f 7265 656d 6974 7465 7228  _make_reemitter(
-00012880: 6e61 6d65 3a20 7374 7229 202d 3e20 4361  name: str) -> Ca
-00012890: 6c6c 6162 6c65 5b2e 2e2e 2c20 4e6f 6e65  llable[..., None
-000128a0: 5d3a 0d0a 2020 2020 2020 2020 7369 675f  ]:..        sig_
-000128b0: 6e61 6d65 203d 206e 616d 655b 325d 2e6c  name = name[2].l
-000128c0: 6f77 6572 2829 202b 206e 616d 655b 333a  ower() + name[3:
-000128d0: 5d0d 0a0d 0a20 2020 2020 2020 2064 6566  ]....        def
-000128e0: 2072 6565 6d69 7428 7365 6c66 3a20 5f4d   reemit(self: _M
-000128f0: 4d43 616c 6c62 6163 6b52 656c 6179 2c20  MCallbackRelay, 
-00012900: 2a61 7267 733a 2041 6e79 2920 2d3e 204e  *args: Any) -> N
-00012910: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00012920: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00012930: 2020 2020 2020 2020 6765 7461 7474 7228          getattr(
-00012940: 7365 6c66 2e5f 656d 6974 7465 722c 2073  self._emitter, s
-00012950: 6967 5f6e 616d 6529 2e65 6d69 7428 2a61  ig_name).emit(*a
-00012960: 7267 7329 0d0a 2020 2020 2020 2020 2020  rgs)..          
-00012970: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00012980: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-00012990: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-000129a0: 2e65 7272 6f72 280d 0a20 2020 2020 2020  .error(..       
-000129b0: 2020 2020 2020 2020 2020 2020 2066 2245               f"E
-000129c0: 7863 6570 7469 6f6e 206f 6363 7572 6564  xception occured
-000129d0: 2069 6e20 4d4d 436f 7265 506c 7573 2063   in MMCorePlus c
-000129e0: 616c 6c62 6163 6b20 7b73 6967 5f6e 616d  allback {sig_nam
-000129f0: 6521 727d 3a20 7b65 7d22 0d0a 2020 2020  e!r}: {e}"..    
-00012a00: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-00012a10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012a20: 7265 656d 6974 0d0a 0d0a 0d0a 4d4d 4361  reemit......MMCa
-00012a30: 6c6c 6261 636b 5265 6c61 7920 3d20 7479  llbackRelay = ty
-00012a40: 7065 280d 0a20 2020 2022 4d4d 4361 6c6c  pe(..    "MMCall
-00012a50: 6261 636b 5265 6c61 7922 2c0d 0a20 2020  backRelay",..   
-00012a60: 2028 5f4d 4d43 616c 6c62 6163 6b52 656c   (_MMCallbackRel
-00012a70: 6179 2c29 2c0d 0a20 2020 207b 0d0a 2020  ay,),..    {..  
-00012a80: 2020 2020 2020 6e3a 205f 4d4d 4361 6c6c        n: _MMCall
-00012a90: 6261 636b 5265 6c61 792e 5f6d 616b 655f  backRelay._make_
-00012aa0: 7265 656d 6974 7465 7228 6e29 0d0a 2020  reemitter(n)..  
-00012ab0: 2020 2020 2020 666f 7220 6e20 696e 2064        for n in d
-00012ac0: 6972 2870 796d 6d63 6f72 652e 4d4d 4576  ir(pymmcore.MMEv
-00012ad0: 656e 7443 616c 6c62 6163 6b29 0d0a 2020  entCallback)..  
-00012ae0: 2020 2020 2020 6966 206e 2e73 7461 7274        if n.start
-00012af0: 7377 6974 6828 226f 6e22 290d 0a20 2020  swith("on")..   
-00012b00: 207d 2c0d 0a29 0d0a                       },..)..
+00002f50: 2020 2020 2020 206d 7367 202b 3d20 280d         msg += (.
+00002f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f70: 2020 2020 2020 2020 2020 2020 2066 222e               f".
+00002f80: 2044 6576 6963 6520 6e61 6d65 207b 6465   Device name {de
+00002f90: 7669 6365 4e61 6d65 2172 7d20 6e6f 7420  viceName!r} not 
+00002fa0: 696e 2064 6576 6963 6573 2070 726f 7669  in devices provi
+00002fb0: 6465 6420 6279 2022 0d0a 2020 2020 2020  ded by "..      
+00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fd0: 2020 2020 2020 6622 6164 6170 7465 7220        f"adapter 
+00002fe0: 7b6d 6f64 756c 654e 616d 6521 727d 3a20  {moduleName!r}: 
+00002ff0: 7b64 6576 6963 6573 7d22 0d0a 2020 2020  {devices}"..    
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00003020: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+00003030: 4572 726f 7228 6d73 6729 2066 726f 6d20  Error(msg) from 
+00003040: 650d 0a0d 0a20 2020 2040 7379 6e63 6872  e....    @synchr
+00003050: 6f6e 697a 6564 285f 6c6f 636b 290d 0a20  onized(_lock).. 
+00003060: 2020 2064 6566 206c 6f61 6453 7973 7465     def loadSyste
+00003070: 6d43 6f6e 6669 6775 7261 7469 6f6e 280d  mConfiguration(.
+00003080: 0a20 2020 2020 2020 2073 656c 662c 2066  .        self, f
+00003090: 696c 654e 616d 653a 2073 7472 207c 2050  ileName: str | P
+000030a0: 6174 6820 3d20 224d 4d43 6f6e 6669 675f  ath = "MMConfig_
+000030b0: 6465 6d6f 2e63 6667 220d 0a20 2020 2029  demo.cfg"..    )
+000030c0: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+000030d0: 2020 2022 2222 4c6f 6164 2061 2073 7973     """Load a sys
+000030e0: 7465 6d20 636f 6e66 6967 2066 696c 6520  tem config file 
+000030f0: 636f 6e66 6f72 6d69 6e67 2074 6f20 7468  conforming to th
+00003100: 6520 4d4d 2060 2e63 6667 6020 666f 726d  e MM `.cfg` form
+00003110: 6174 2e0d 0a0d 0a20 2020 2020 2020 2068  at.....        h
+00003120: 7474 7073 3a2f 2f6d 6963 726f 2d6d 616e  ttps://micro-man
+00003130: 6167 6572 2e6f 7267 2f4d 6963 726f 2d4d  ager.org/Micro-M
+00003140: 616e 6167 6572 5f43 6f6e 6669 6775 7261  anager_Configura
+00003150: 7469 6f6e 5f47 7569 6465 2363 6f6e 6669  tion_Guide#confi
+00003160: 6775 7261 7469 6f6e 2d66 696c 652d 7379  guration-file-sy
+00003170: 6e74 6178 0d0a 0d0a 2020 2020 2020 2020  ntax....        
+00003180: 466f 7220 7265 6c61 7469 7665 2070 6174  For relative pat
+00003190: 6873 2c20 7468 6520 6375 7272 656e 7420  hs, the current 
+000031a0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+000031b0: 7920 6973 2066 6972 7374 2063 6865 636b  y is first check
+000031c0: 6564 2c20 7468 656e 2074 6865 0d0a 2020  ed, then the..  
+000031d0: 2020 2020 2020 7468 656e 2064 6576 6963        then devic
+000031e0: 6520 6164 6170 7465 7220 7061 7468 2069  e adapter path i
+000031f0: 7320 6368 6563 6b65 642e 0d0a 0d0a 2020  s checked.....  
+00003200: 2020 2020 2020 2a2a 5768 7920 4f76 6572        **Why Over
+00003210: 7269 6465 3f2a 2a20 5468 6973 206d 6574  ride?** This met
+00003220: 686f 6420 6f76 6572 7269 6465 7320 7468  hod overrides th
+00003230: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
+00003240: 656e 7461 7469 6f6e 2074 6f20 4129 2061  entation to A) a
+00003250: 6c6c 6f77 0d0a 2020 2020 2020 2020 6c6f  llow..        lo
+00003260: 6164 696e 6720 7468 6520 604d 4d43 6f6e  ading the `MMCon
+00003270: 6669 675f 6465 6d6f 2e63 6667 6020 6669  fig_demo.cfg` fi
+00003280: 6c65 2062 7920 6465 6661 756c 742c 2042  le by default, B
+00003290: 2920 746f 2070 726f 7669 6465 206d 6f72  ) to provide mor
+000032a0: 6520 666c 6578 6962 6c65 0d0a 2020 2020  e flexible..    
+000032b0: 2020 2020 7061 7468 2064 6563 6c61 7261      path declara
+000032c0: 7469 6f6e 7320 616e 6420 4329 2062 6574  tions and C) bet
+000032d0: 7465 7220 6572 726f 7220 6d65 7373 6167  ter error messag
+000032e0: 6573 2077 6865 6e20 7468 6520 6669 6c65  es when the file
+000032f0: 2063 616e 6e6f 7420 6265 2066 6f75 6e64   cannot be found
+00003300: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00003310: 2020 2020 2020 2020 6670 6174 6820 3d20          fpath = 
+00003320: 5061 7468 2866 696c 654e 616d 6529 2e65  Path(fileName).e
+00003330: 7870 616e 6475 7365 7228 290d 0a20 2020  xpanduser()..   
+00003340: 2020 2020 2069 6620 6e6f 7420 6670 6174       if not fpat
+00003350: 682e 6578 6973 7473 2829 2061 6e64 206e  h.exists() and n
+00003360: 6f74 2066 7061 7468 2e69 735f 6162 736f  ot fpath.is_abso
+00003370: 6c75 7465 2829 2061 6e64 2073 656c 662e  lute() and self.
+00003380: 5f6d 6d5f 7061 7468 3a0d 0a20 2020 2020  _mm_path:..     
+00003390: 2020 2020 2020 2066 7061 7468 203d 2050         fpath = P
+000033a0: 6174 6828 7365 6c66 2e5f 6d6d 5f70 6174  ath(self._mm_pat
+000033b0: 6829 202f 2066 696c 654e 616d 650d 0a20  h) / fileName.. 
+000033c0: 2020 2020 2020 2069 6620 6e6f 7420 6670         if not fp
+000033d0: 6174 682e 6578 6973 7473 2829 3a0d 0a20  ath.exists():.. 
+000033e0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000033f0: 2046 696c 654e 6f74 466f 756e 6445 7272   FileNotFoundErr
+00003400: 6f72 2866 2250 6174 6820 646f 6573 206e  or(f"Path does n
+00003410: 6f74 2065 7869 7374 3a20 7b66 7061 7468  ot exist: {fpath
+00003420: 7d22 290d 0a20 2020 2020 2020 2073 7570  }")..        sup
+00003430: 6572 2829 2e6c 6f61 6453 7973 7465 6d43  er().loadSystemC
+00003440: 6f6e 6669 6775 7261 7469 6f6e 2873 7472  onfiguration(str
+00003450: 2866 7061 7468 2e72 6573 6f6c 7665 2829  (fpath.resolve()
+00003460: 2929 0d0a 0d0a 2020 2020 6465 6620 756e  ))....    def un
+00003470: 6c6f 6164 416c 6c44 6576 6963 6573 2873  loadAllDevices(s
+00003480: 656c 6629 202d 3e20 4e6f 6e65 3a0d 0a20  elf) -> None:.. 
+00003490: 2020 2020 2020 2022 2222 556e 6c6f 6164         """Unload
+000034a0: 2061 6c6c 2064 6576 6963 6573 2066 726f   all devices fro
+000034b0: 6d20 7468 6520 636f 7265 2061 6e64 2072  m the core and r
+000034c0: 6573 6574 2061 6c6c 2063 6f6e 6669 6775  eset all configu
+000034d0: 7261 7469 6f6e 2064 6174 612e 0d0a 0d0a  ration data.....
+000034e0: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
+000034f0: 6572 7269 6465 3f2a 2a20 546f 2061 6464  erride?** To add
+00003500: 206c 6f67 6769 6e67 2e0d 0a20 2020 2020   logging...     
+00003510: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00003520: 2320 7468 6973 206c 6f67 2077 6f6e 2774  # this log won't
+00003530: 2061 7070 6561 7220 7768 656e 2065 7869   appear when exi
+00003540: 7469 6e67 2069 7079 7468 6f6e 2c20 6275  ting ipython, bu
+00003550: 7420 7468 6520 6d65 7468 6f64 2069 7320  t the method is 
+00003560: 7374 696c 6c20 6361 6c6c 6564 0d0a 2020  still called..  
+00003570: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00003580: 7567 2822 556e 6c6f 6164 696e 6720 616c  ug("Unloading al
+00003590: 6c20 6465 7669 6365 7322 290d 0a20 2020  l devices")..   
+000035a0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+000035b0: 7228 292e 756e 6c6f 6164 416c 6c44 6576  r().unloadAllDev
+000035c0: 6963 6573 2829 0d0a 0d0a 2020 2020 6465  ices()....    de
+000035d0: 6620 6765 7444 6576 6963 6554 7970 6528  f getDeviceType(
+000035e0: 7365 6c66 2c20 6c61 6265 6c3a 2073 7472  self, label: str
+000035f0: 2920 2d3e 2044 6576 6963 6554 7970 653a  ) -> DeviceType:
+00003600: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00003610: 7572 6e20 6465 7669 6365 2074 7970 6520  urn device type 
+00003620: 666f 7220 6120 6769 7665 6e20 6465 7669  for a given devi
+00003630: 6365 2e0d 0a0d 0a20 2020 2020 2020 202a  ce.....        *
+00003640: 2a57 6879 204f 7665 7272 6964 653f 2a2a  *Why Override?**
+00003650: 2054 6865 2072 6574 7572 6e65 6420 5b60   The returned [`
+00003660: 7079 6d6d 636f 7265 5f70 6c75 732e 4465  pymmcore_plus.De
+00003670: 7669 6365 605d 5b5d 2065 6e75 6d20 6973  vice`][] enum is
+00003680: 206d 6f72 650d 0a20 2020 2020 2020 2069   more..        i
+00003690: 6e74 6572 7072 6574 6162 6c65 2074 6861  nterpretable tha
+000036a0: 6e20 7468 6520 7261 7720 6069 6e74 6020  n the raw `int` 
+000036b0: 7265 7475 726e 6564 2062 7920 6070 796d  returned by `pym
+000036c0: 6d63 6f72 6560 0d0a 2020 2020 2020 2020  mcore`..        
+000036d0: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+000036e0: 7572 6e20 4465 7669 6365 5479 7065 2873  urn DeviceType(s
+000036f0: 7570 6572 2829 2e67 6574 4465 7669 6365  uper().getDevice
+00003700: 5479 7065 286c 6162 656c 2929 0d0a 0d0a  Type(label))....
+00003710: 2020 2020 6465 6620 6765 7450 726f 7065      def getPrope
+00003720: 7274 7954 7970 6528 7365 6c66 2c20 6c61  rtyType(self, la
+00003730: 6265 6c3a 2073 7472 2c20 7072 6f70 4e61  bel: str, propNa
+00003740: 6d65 3a20 7374 7229 202d 3e20 5072 6f70  me: str) -> Prop
+00003750: 6572 7479 5479 7065 3a0d 0a20 2020 2020  ertyType:..     
+00003760: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+00003770: 2069 6e74 7269 6e73 6963 2070 726f 7065   intrinsic prope
+00003780: 7274 7920 7479 7065 2066 6f72 2061 2067  rty type for a g
+00003790: 6976 656e 2064 6576 6963 6520 616e 6420  iven device and 
+000037a0: 7072 6f70 6572 7479 2e0d 0a0d 0a20 2020  property.....   
+000037b0: 2020 2020 202a 2a57 6879 204f 7665 7272       **Why Overr
+000037c0: 6964 653f 2a2a 2054 6865 2072 6574 7572  ide?** The retur
+000037d0: 6e65 6420 5b60 7079 6d6d 636f 7265 5f70  ned [`pymmcore_p
+000037e0: 6c75 732e 5072 6f70 6572 7479 5479 7065  lus.PropertyType
+000037f0: 605d 5b5d 2065 6e75 6d20 6973 206d 6f72  `][] enum is mor
+00003800: 650d 0a20 2020 2020 2020 2069 6e74 6572  e..        inter
+00003810: 7072 6574 6162 6c65 2074 6861 6e20 7468  pretable than th
+00003820: 6520 7261 7720 6069 6e74 6020 7265 7475  e raw `int` retu
+00003830: 726e 6564 2062 7920 6070 796d 6d63 6f72  rned by `pymmcor
+00003840: 6560 0d0a 2020 2020 2020 2020 2222 220d  e`..        """.
+00003850: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003860: 5072 6f70 6572 7479 5479 7065 2873 7570  PropertyType(sup
+00003870: 6572 2829 2e67 6574 5072 6f70 6572 7479  er().getProperty
+00003880: 5479 7065 286c 6162 656c 2c20 7072 6f70  Type(label, prop
+00003890: 4e61 6d65 2929 0d0a 0d0a 2020 2020 6465  Name))....    de
+000038a0: 6620 6465 7465 6374 4465 7669 6365 2873  f detectDevice(s
+000038b0: 656c 662c 2064 6576 6963 654c 6162 656c  elf, deviceLabel
+000038c0: 3a20 7374 7229 202d 3e20 4465 7669 6365  : str) -> Device
+000038d0: 4465 7465 6374 696f 6e53 7461 7475 733a  DetectionStatus:
+000038e0: 0d0a 2020 2020 2020 2020 2222 2254 7269  ..        """Tri
+000038f0: 6573 2074 6f20 636f 6d6d 756e 6963 6174  es to communicat
+00003900: 6520 746f 2061 2064 6576 6963 6520 7468  e to a device th
+00003910: 726f 7567 6820 6120 6769 7665 6e20 7365  rough a given se
+00003920: 7269 616c 2070 6f72 742e 0d0a 0d0a 2020  rial port.....  
+00003930: 2020 2020 2020 5573 6564 2074 6f20 6175        Used to au
+00003940: 746f 6d61 7465 2064 6973 636f 7665 7279  tomate discovery
+00003950: 206f 6620 636f 7272 6563 7420 7365 7269   of correct seri
+00003960: 616c 2070 6f72 742e 0d0a 2020 2020 2020  al port...      
+00003970: 2020 416c 736f 2063 6f6e 6669 6775 7265    Also configure
+00003980: 7320 7468 6520 7365 7269 616c 2070 6f72  s the serial por
+00003990: 7420 636f 7272 6563 746c 792e 0d0a 0d0a  t correctly.....
+000039a0: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
+000039b0: 6572 7269 6465 3f2a 2a20 5468 6520 7265  erride?** The re
+000039c0: 7475 726e 6564 205b 6070 796d 6d63 6f72  turned [`pymmcor
+000039d0: 655f 706c 7573 2e44 6576 6963 6544 6574  e_plus.DeviceDet
+000039e0: 6563 7469 6f6e 5374 6174 7573 605d 5b5d  ectionStatus`][]
+000039f0: 2065 6e75 6d0d 0a20 2020 2020 2020 2069   enum..        i
+00003a00: 7320 6d6f 7265 2069 6e74 6572 7072 6574  s more interpret
+00003a10: 6162 6c65 2074 6861 6e20 7468 6520 7261  able than the ra
+00003a20: 7720 6069 6e74 6020 7265 7475 726e 6564  w `int` returned
+00003a30: 2062 7920 6070 796d 6d63 6f72 6560 0d0a   by `pymmcore`..
+00003a40: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00003a50: 2020 2020 2072 6574 7572 6e20 4465 7669       return Devi
+00003a60: 6365 4465 7465 6374 696f 6e53 7461 7475  ceDetectionStatu
+00003a70: 7328 7375 7065 7228 292e 6465 7465 6374  s(super().detect
+00003a80: 4465 7669 6365 2864 6576 6963 654c 6162  Device(deviceLab
+00003a90: 656c 2929 0d0a 0d0a 2020 2020 2320 636f  el))....    # co
+00003aa0: 6e66 6967 206f 7665 7272 6964 6573 0d0a  nfig overrides..
+00003ab0: 0d0a 2020 2020 406f 7665 726c 6f61 640d  ..    @overload.
+00003ac0: 0a20 2020 2064 6566 2067 6574 436f 6e66  .    def getConf
+00003ad0: 6967 4461 7461 280d 0a20 2020 2020 2020  igData(..       
+00003ae0: 2073 656c 662c 2063 6f6e 6669 6747 726f   self, configGro
+00003af0: 7570 3a20 7374 722c 2063 6f6e 6669 674e  up: str, configN
+00003b00: 616d 653a 2073 7472 2c20 2a2c 206e 6174  ame: str, *, nat
+00003b10: 6976 653a 204c 6974 6572 616c 5b54 7275  ive: Literal[Tru
+00003b20: 655d 0d0a 2020 2020 2920 2d3e 2070 796d  e]..    ) -> pym
+00003b30: 6d63 6f72 652e 436f 6e66 6967 7572 6174  mcore.Configurat
+00003b40: 696f 6e3a 0d0a 2020 2020 2020 2020 2e2e  ion:..        ..
+00003b50: 2e0d 0a0d 0a20 2020 2040 6f76 6572 6c6f  .....    @overlo
+00003b60: 6164 0d0a 2020 2020 6465 6620 6765 7443  ad..    def getC
+00003b70: 6f6e 6669 6744 6174 6128 0d0a 2020 2020  onfigData(..    
+00003b80: 2020 2020 7365 6c66 2c20 636f 6e66 6967      self, config
+00003b90: 4772 6f75 703a 2073 7472 2c20 636f 6e66  Group: str, conf
+00003ba0: 6967 4e61 6d65 3a20 7374 722c 202a 2c20  igName: str, *, 
+00003bb0: 6e61 7469 7665 3a20 4c69 7465 7261 6c5b  native: Literal[
+00003bc0: 4661 6c73 655d 203d 2046 616c 7365 0d0a  False] = False..
+00003bd0: 2020 2020 2920 2d3e 2043 6f6e 6669 6775      ) -> Configu
+00003be0: 7261 7469 6f6e 3a0d 0a20 2020 2020 2020  ration:..       
+00003bf0: 202e 2e2e 0d0a 0d0a 2020 2020 6465 6620   .......    def 
+00003c00: 6765 7443 6f6e 6669 6744 6174 6128 0d0a  getConfigData(..
+00003c10: 2020 2020 2020 2020 7365 6c66 2c20 636f          self, co
+00003c20: 6e66 6967 4772 6f75 703a 2073 7472 2c20  nfigGroup: str, 
+00003c30: 636f 6e66 6967 4e61 6d65 3a20 7374 722c  configName: str,
+00003c40: 202a 2c20 6e61 7469 7665 3a20 626f 6f6c   *, native: bool
+00003c50: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
+00003c60: 2d3e 2043 6f6e 6669 6775 7261 7469 6f6e  -> Configuration
+00003c70: 207c 2070 796d 6d63 6f72 652e 436f 6e66   | pymmcore.Conf
+00003c80: 6967 7572 6174 696f 6e3a 0d0a 2020 2020  iguration:..    
+00003c90: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+00003ca0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00003cb0: 6f62 6a65 6374 2066 6f72 2061 2067 6976  object for a giv
+00003cc0: 656e 2060 636f 6e66 6967 4772 6f75 7060  en `configGroup`
+00003cd0: 2061 6e64 2060 636f 6e66 6967 4e61 6d65   and `configName
+00003ce0: 602e 0d0a 0d0a 2020 2020 2020 2020 2a2a  `.....        **
+00003cf0: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
+00003d00: 5468 6520 5b60 7079 6d6d 636f 7265 5f70  The [`pymmcore_p
+00003d10: 6c75 732e 436f 6e66 6967 7572 6174 696f  lus.Configuratio
+00003d20: 6e60 5d5b 5d20 6f62 6a65 6374 2072 6574  n`][] object ret
+00003d30: 7572 6e65 640d 0a20 2020 2020 2020 2077  urned..        w
+00003d40: 6865 6e20 606e 6174 6976 653d 4661 6c73  hen `native=Fals
+00003d50: 6560 2028 7468 6520 6465 6661 756c 7429  e` (the default)
+00003d60: 2070 726f 7669 6465 7320 6120 6e69 6365   provides a nice
+00003d70: 7220 604d 6170 7069 6e67 6020 696e 7465  r `Mapping` inte
+00003d80: 7266 6163 652e 2050 6173 730d 0a20 2020  rface. Pass..   
+00003d90: 2020 2020 2060 6e61 7469 7665 3d54 7275       `native=Tru
+00003da0: 6560 2074 6f20 6765 7420 7468 6520 6f72  e` to get the or
+00003db0: 6967 696e 616c 2060 7079 6d6d 636f 7265  iginal `pymmcore
+00003dc0: 2e43 6f6e 6669 6775 7261 7469 6f6e 6020  .Configuration` 
+00003dd0: 6f62 6a65 6374 2e0d 0a20 2020 2020 2020  object...       
+00003de0: 2022 2222 0d0a 2020 2020 2020 2020 6366   """..        cf
+00003df0: 6720 3d20 7375 7065 7228 292e 6765 7443  g = super().getC
+00003e00: 6f6e 6669 6744 6174 6128 636f 6e66 6967  onfigData(config
+00003e10: 4772 6f75 702c 2063 6f6e 6669 674e 616d  Group, configNam
+00003e20: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00003e30: 726e 2063 6667 2069 6620 6e61 7469 7665  rn cfg if native
+00003e40: 2065 6c73 6520 436f 6e66 6967 7572 6174   else Configurat
+00003e50: 696f 6e2e 6672 6f6d 5f63 6f6e 6669 6775  ion.from_configu
+00003e60: 7261 7469 6f6e 2863 6667 290d 0a0d 0a20  ration(cfg).... 
+00003e70: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
+00003e80: 2020 6465 6620 6765 7450 6978 656c 5369    def getPixelSi
+00003e90: 7a65 436f 6e66 6967 4461 7461 280d 0a20  zeConfigData(.. 
+00003ea0: 2020 2020 2020 2073 656c 662c 2063 6f6e         self, con
+00003eb0: 6669 674e 616d 653a 2073 7472 2c20 2a2c  figName: str, *,
+00003ec0: 206e 6174 6976 653a 204c 6974 6572 616c   native: Literal
+00003ed0: 5b54 7275 655d 0d0a 2020 2020 2920 2d3e  [True]..    ) ->
+00003ee0: 2070 796d 6d63 6f72 652e 436f 6e66 6967   pymmcore.Config
+00003ef0: 7572 6174 696f 6e3a 0d0a 2020 2020 2020  uration:..      
+00003f00: 2020 2e2e 2e0d 0a0d 0a20 2020 2040 6f76    .......    @ov
+00003f10: 6572 6c6f 6164 0d0a 2020 2020 6465 6620  erload..    def 
+00003f20: 6765 7450 6978 656c 5369 7a65 436f 6e66  getPixelSizeConf
+00003f30: 6967 4461 7461 280d 0a20 2020 2020 2020  igData(..       
+00003f40: 2073 656c 662c 2063 6f6e 6669 674e 616d   self, configNam
+00003f50: 653a 2073 7472 2c20 2a2c 206e 6174 6976  e: str, *, nativ
+00003f60: 653a 204c 6974 6572 616c 5b46 616c 7365  e: Literal[False
+00003f70: 5d20 3d20 4661 6c73 650d 0a20 2020 2029  ] = False..    )
+00003f80: 202d 3e20 436f 6e66 6967 7572 6174 696f   -> Configuratio
+00003f90: 6e3a 0d0a 2020 2020 2020 2020 2e2e 2e0d  n:..        ....
+00003fa0: 0a0d 0a20 2020 2064 6566 2067 6574 5069  ...    def getPi
+00003fb0: 7865 6c53 697a 6543 6f6e 6669 6744 6174  xelSizeConfigDat
+00003fc0: 6128 0d0a 2020 2020 2020 2020 7365 6c66  a(..        self
+00003fd0: 2c20 636f 6e66 6967 4e61 6d65 3a20 7374  , configName: st
+00003fe0: 722c 202a 2c20 6e61 7469 7665 3a20 626f  r, *, native: bo
+00003ff0: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
+00004000: 2920 2d3e 2043 6f6e 6669 6775 7261 7469  ) -> Configurati
+00004010: 6f6e 207c 2070 796d 6d63 6f72 652e 436f  on | pymmcore.Co
+00004020: 6e66 6967 7572 6174 696f 6e3a 0d0a 2020  nfiguration:..  
+00004030: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00004040: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+00004050: 6e20 6f62 6a65 6374 2066 6f72 2061 2067  n object for a g
+00004060: 6976 656e 2070 6978 656c 2073 697a 6520  iven pixel size 
+00004070: 7072 6573 6574 2060 636f 6e66 6967 4e61  preset `configNa
+00004080: 6d65 602e 0d0a 0d0a 2020 2020 2020 2020  me`.....        
+00004090: 2a2a 5768 7920 4f76 6572 7269 6465 3f2a  **Why Override?*
+000040a0: 2a20 5468 6520 5b60 7079 6d6d 636f 7265  * The [`pymmcore
+000040b0: 5f70 6c75 732e 436f 6e66 6967 7572 6174  _plus.Configurat
+000040c0: 696f 6e60 5d5b 5d20 6f62 6a65 6374 2072  ion`][] object r
+000040d0: 6574 7572 6e65 640d 0a20 2020 2020 2020  eturned..       
+000040e0: 2077 6865 6e20 606e 6174 6976 653d 4661   when `native=Fa
+000040f0: 6c73 6560 2028 7468 6520 6465 6661 756c  lse` (the defaul
+00004100: 7429 2070 726f 7669 6465 7320 6120 6e69  t) provides a ni
+00004110: 6365 7220 604d 6170 7069 6e67 6020 696e  cer `Mapping` in
+00004120: 7465 7266 6163 652e 2050 6173 730d 0a20  terface. Pass.. 
+00004130: 2020 2020 2020 2060 6e61 7469 7665 3d54         `native=T
+00004140: 7275 6560 2074 6f20 6765 7420 7468 6520  rue` to get the 
+00004150: 6f72 6967 696e 616c 2060 7079 6d6d 636f  original `pymmco
+00004160: 7265 2e43 6f6e 6669 6775 7261 7469 6f6e  re.Configuration
+00004170: 6020 6f62 6a65 6374 2e0d 0a20 2020 2020  ` object...     
+00004180: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004190: 6366 6720 3d20 7375 7065 7228 292e 6765  cfg = super().ge
+000041a0: 7450 6978 656c 5369 7a65 436f 6e66 6967  tPixelSizeConfig
+000041b0: 4461 7461 2863 6f6e 6669 674e 616d 6529  Data(configName)
+000041c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000041d0: 2063 6667 2069 6620 6e61 7469 7665 2065   cfg if native e
+000041e0: 6c73 6520 436f 6e66 6967 7572 6174 696f  lse Configuratio
+000041f0: 6e2e 6672 6f6d 5f63 6f6e 6669 6775 7261  n.from_configura
+00004200: 7469 6f6e 2863 6667 290d 0a0d 0a20 2020  tion(cfg)....   
+00004210: 2040 6f76 6572 6c6f 6164 0d0a 2020 2020   @overload..    
+00004220: 6465 6620 6765 7443 6f6e 6669 6747 726f  def getConfigGro
+00004230: 7570 5374 6174 6528 0d0a 2020 2020 2020  upState(..      
+00004240: 2020 7365 6c66 2c20 6772 6f75 703a 2073    self, group: s
+00004250: 7472 2c20 2a2c 206e 6174 6976 653a 204c  tr, *, native: L
+00004260: 6974 6572 616c 5b54 7275 655d 0d0a 2020  iteral[True]..  
+00004270: 2020 2920 2d3e 2070 796d 6d63 6f72 652e    ) -> pymmcore.
+00004280: 436f 6e66 6967 7572 6174 696f 6e3a 0d0a  Configuration:..
+00004290: 2020 2020 2020 2020 2e2e 2e0d 0a0d 0a20          ....... 
+000042a0: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
+000042b0: 2020 6465 6620 6765 7443 6f6e 6669 6747    def getConfigG
+000042c0: 726f 7570 5374 6174 6528 0d0a 2020 2020  roupState(..    
+000042d0: 2020 2020 7365 6c66 2c20 6772 6f75 703a      self, group:
+000042e0: 2073 7472 2c20 2a2c 206e 6174 6976 653a   str, *, native:
+000042f0: 204c 6974 6572 616c 5b46 616c 7365 5d20   Literal[False] 
+00004300: 3d20 4661 6c73 650d 0a20 2020 2029 202d  = False..    ) -
+00004310: 3e20 436f 6e66 6967 7572 6174 696f 6e3a  > Configuration:
+00004320: 0d0a 2020 2020 2020 2020 2e2e 2e0d 0a0d  ..        ......
+00004330: 0a20 2020 2064 6566 2067 6574 436f 6e66  .    def getConf
+00004340: 6967 4772 6f75 7053 7461 7465 280d 0a20  igGroupState(.. 
+00004350: 2020 2020 2020 2073 656c 662c 2067 726f         self, gro
+00004360: 7570 3a20 7374 722c 202a 2c20 6e61 7469  up: str, *, nati
+00004370: 7665 3a20 626f 6f6c 203d 2046 616c 7365  ve: bool = False
+00004380: 0d0a 2020 2020 2920 2d3e 2043 6f6e 6669  ..    ) -> Confi
+00004390: 6775 7261 7469 6f6e 207c 2070 796d 6d63  guration | pymmc
+000043a0: 6f72 652e 436f 6e66 6967 7572 6174 696f  ore.Configuratio
+000043b0: 6e3a 0d0a 2020 2020 2020 2020 2222 2252  n:..        """R
+000043c0: 6574 7572 6e20 7468 6520 7374 6174 6520  eturn the state 
+000043d0: 6f66 2074 6865 2064 6576 6963 6573 2069  of the devices i
+000043e0: 6e63 6c75 6465 6420 696e 2074 6865 2073  ncluded in the s
+000043f0: 7065 6369 6669 6564 2060 6772 6f75 7060  pecified `group`
+00004400: 2e0d 0a0d 0a20 2020 2020 2020 202a 2a57  .....        **W
+00004410: 6879 204f 7665 7272 6964 653f 2a2a 2054  hy Override?** T
+00004420: 6865 205b 6070 796d 6d63 6f72 655f 706c  he [`pymmcore_pl
+00004430: 7573 2e43 6f6e 6669 6775 7261 7469 6f6e  us.Configuration
+00004440: 605d 5b5d 206f 626a 6563 7420 7265 7475  `][] object retu
+00004450: 726e 6564 0d0a 2020 2020 2020 2020 7768  rned..        wh
+00004460: 656e 2060 6e61 7469 7665 3d46 616c 7365  en `native=False
+00004470: 6020 2874 6865 2064 6566 6175 6c74 2920  ` (the default) 
+00004480: 7072 6f76 6964 6573 2061 206e 6963 6572  provides a nicer
+00004490: 2060 4d61 7070 696e 6760 2069 6e74 6572   `Mapping` inter
+000044a0: 6661 6365 2e20 5061 7373 0d0a 2020 2020  face. Pass..    
+000044b0: 2020 2020 606e 6174 6976 653d 5472 7565      `native=True
+000044c0: 6020 746f 2067 6574 2074 6865 206f 7269  ` to get the ori
+000044d0: 6769 6e61 6c20 6070 796d 6d63 6f72 652e  ginal `pymmcore.
+000044e0: 436f 6e66 6967 7572 6174 696f 6e60 206f  Configuration` o
+000044f0: 626a 6563 742e 0d0a 2020 2020 2020 2020  bject...        
+00004500: 2222 220d 0a20 2020 2020 2020 2063 6667  """..        cfg
+00004510: 203d 2073 7570 6572 2829 2e67 6574 436f   = super().getCo
+00004520: 6e66 6967 4772 6f75 7053 7461 7465 2867  nfigGroupState(g
+00004530: 726f 7570 290d 0a20 2020 2020 2020 2072  roup)..        r
+00004540: 6574 7572 6e20 6366 6720 6966 206e 6174  eturn cfg if nat
+00004550: 6976 6520 656c 7365 2043 6f6e 6669 6775  ive else Configu
+00004560: 7261 7469 6f6e 2e66 726f 6d5f 636f 6e66  ration.from_conf
+00004570: 6967 7572 6174 696f 6e28 6366 6729 0d0a  iguration(cfg)..
+00004580: 0d0a 2020 2020 6465 6620 6765 7443 6f6e  ..    def getCon
+00004590: 6669 6747 726f 7570 5374 6174 6546 726f  figGroupStateFro
+000045a0: 6d43 6163 6865 280d 0a20 2020 2020 2020  mCache(..       
+000045b0: 2073 656c 662c 2067 726f 7570 3a20 7374   self, group: st
+000045c0: 722c 202a 2c20 6e61 7469 7665 3a20 626f  r, *, native: bo
+000045d0: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
+000045e0: 2920 2d3e 2043 6f6e 6669 6775 7261 7469  ) -> Configurati
+000045f0: 6f6e 207c 2070 796d 6d63 6f72 652e 436f  on | pymmcore.Co
+00004600: 6e66 6967 7572 6174 696f 6e3a 0d0a 2020  nfiguration:..  
+00004610: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00004620: 7468 6520 7374 6174 6520 6f66 2074 6865  the state of the
+00004630: 2073 7973 7465 6d20 6361 6368 652c 2066   system cache, f
+00004640: 6f72 2074 6865 2064 6576 6963 6573 2069  or the devices i
+00004650: 6e20 7468 6520 7370 6563 6966 6965 6420  n the specified 
+00004660: 6772 6f75 702e 0d0a 0d0a 2020 2020 2020  group.....      
+00004670: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
+00004680: 3f2a 2a20 5468 6520 5b60 7079 6d6d 636f  ?** The [`pymmco
+00004690: 7265 5f70 6c75 732e 436f 6e66 6967 7572  re_plus.Configur
+000046a0: 6174 696f 6e60 5d5b 5d20 6f62 6a65 6374  ation`][] object
+000046b0: 2072 6574 7572 6e65 640d 0a20 2020 2020   returned..     
+000046c0: 2020 2077 6865 6e20 606e 6174 6976 653d     when `native=
+000046d0: 4661 6c73 6560 2028 7468 6520 6465 6661  False` (the defa
+000046e0: 756c 7429 2070 726f 7669 6465 7320 6120  ult) provides a 
+000046f0: 6e69 6365 7220 604d 6170 7069 6e67 6020  nicer `Mapping` 
+00004700: 696e 7465 7266 6163 652e 2050 6173 730d  interface. Pass.
+00004710: 0a20 2020 2020 2020 2060 6e61 7469 7665  .        `native
+00004720: 3d54 7275 6560 2074 6f20 6765 7420 7468  =True` to get th
+00004730: 6520 6f72 6967 696e 616c 2060 7079 6d6d  e original `pymm
+00004740: 636f 7265 2e43 6f6e 6669 6775 7261 7469  core.Configurati
+00004750: 6f6e 6020 6f62 6a65 6374 2e0d 0a20 2020  on` object...   
+00004760: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004770: 2020 6366 6720 3d20 7375 7065 7228 292e    cfg = super().
+00004780: 6765 7443 6f6e 6669 6747 726f 7570 5374  getConfigGroupSt
+00004790: 6174 6546 726f 6d43 6163 6865 2867 726f  ateFromCache(gro
+000047a0: 7570 290d 0a20 2020 2020 2020 2072 6574  up)..        ret
+000047b0: 7572 6e20 6366 6720 6966 206e 6174 6976  urn cfg if nativ
+000047c0: 6520 656c 7365 2043 6f6e 6669 6775 7261  e else Configura
+000047d0: 7469 6f6e 2e66 726f 6d5f 636f 6e66 6967  tion.from_config
+000047e0: 7572 6174 696f 6e28 6366 6729 0d0a 0d0a  uration(cfg)....
+000047f0: 2020 2020 6465 6620 6765 7443 6f6e 6669      def getConfi
+00004800: 6753 7461 7465 280d 0a20 2020 2020 2020  gState(..       
+00004810: 2073 656c 662c 2067 726f 7570 3a20 7374   self, group: st
+00004820: 722c 2063 6f6e 6669 673a 2073 7472 2c20  r, config: str, 
+00004830: 2a2c 206e 6174 6976 653a 2062 6f6f 6c20  *, native: bool 
+00004840: 3d20 4661 6c73 650d 0a20 2020 2029 202d  = False..    ) -
+00004850: 3e20 436f 6e66 6967 7572 6174 696f 6e20  > Configuration 
+00004860: 7c20 7079 6d6d 636f 7265 2e43 6f6e 6669  | pymmcore.Confi
+00004870: 6775 7261 7469 6f6e 3a0d 0a20 2020 2020  guration:..     
+00004880: 2020 2022 2222 5265 7475 726e 2073 7461     """Return sta
+00004890: 7465 206f 6620 6465 7669 6365 7320 696e  te of devices in
+000048a0: 636c 7564 6564 2069 6e20 7468 6520 7370  cluded in the sp
+000048b0: 6563 6966 6965 6420 636f 6e66 6967 7572  ecified configur
+000048c0: 6174 696f 6e2e 0d0a 0d0a 2020 2020 2020  ation.....      
+000048d0: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
+000048e0: 3f2a 2a20 5468 6520 5b60 7079 6d6d 636f  ?** The [`pymmco
+000048f0: 7265 5f70 6c75 732e 436f 6e66 6967 7572  re_plus.Configur
+00004900: 6174 696f 6e60 5d5b 5d20 6f62 6a65 6374  ation`][] object
+00004910: 2072 6574 7572 6e65 640d 0a20 2020 2020   returned..     
+00004920: 2020 2077 6865 6e20 606e 6174 6976 653d     when `native=
+00004930: 4661 6c73 6560 2028 7468 6520 6465 6661  False` (the defa
+00004940: 756c 7429 2070 726f 7669 6465 7320 6120  ult) provides a 
+00004950: 6e69 6365 7220 604d 6170 7069 6e67 6020  nicer `Mapping` 
+00004960: 696e 7465 7266 6163 652e 2050 6173 730d  interface. Pass.
+00004970: 0a20 2020 2020 2020 2060 6e61 7469 7665  .        `native
+00004980: 3d54 7275 6560 2074 6f20 6765 7420 7468  =True` to get th
+00004990: 6520 6f72 6967 696e 616c 2060 7079 6d6d  e original `pymm
+000049a0: 636f 7265 2e43 6f6e 6669 6775 7261 7469  core.Configurati
+000049b0: 6f6e 6020 6f62 6a65 6374 2e0d 0a20 2020  on` object...   
+000049c0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000049d0: 2020 6366 6720 3d20 7375 7065 7228 292e    cfg = super().
+000049e0: 6765 7443 6f6e 6669 6753 7461 7465 2867  getConfigState(g
+000049f0: 726f 7570 2c20 636f 6e66 6967 290d 0a20  roup, config).. 
+00004a00: 2020 2020 2020 2072 6574 7572 6e20 6366         return cf
+00004a10: 6720 6966 206e 6174 6976 6520 656c 7365  g if native else
+00004a20: 2043 6f6e 6669 6775 7261 7469 6f6e 2e66   Configuration.f
+00004a30: 726f 6d5f 636f 6e66 6967 7572 6174 696f  rom_configuratio
+00004a40: 6e28 6366 6729 0d0a 0d0a 2020 2020 6465  n(cfg)....    de
+00004a50: 6620 6765 7453 7973 7465 6d53 7461 7465  f getSystemState
+00004a60: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
+00004a70: 202a 2c20 6e61 7469 7665 3a20 626f 6f6c   *, native: bool
+00004a80: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
+00004a90: 2d3e 2043 6f6e 6669 6775 7261 7469 6f6e  -> Configuration
+00004aa0: 207c 2070 796d 6d63 6f72 652e 436f 6e66   | pymmcore.Conf
+00004ab0: 6967 7572 6174 696f 6e3a 0d0a 2020 2020  iguration:..    
+00004ac0: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+00004ad0: 6520 656e 7469 7265 2073 7973 7465 6d20  e entire system 
+00004ae0: 7374 6174 652e 0d0a 0d0a 2020 2020 2020  state.....      
+00004af0: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
+00004b00: 3f2a 2a20 5468 6520 5b60 7079 6d6d 636f  ?** The [`pymmco
+00004b10: 7265 5f70 6c75 732e 436f 6e66 6967 7572  re_plus.Configur
+00004b20: 6174 696f 6e60 5d5b 5d20 6f62 6a65 6374  ation`][] object
+00004b30: 2072 6574 7572 6e65 640d 0a20 2020 2020   returned..     
+00004b40: 2020 2077 6865 6e20 606e 6174 6976 653d     when `native=
+00004b50: 4661 6c73 6560 2028 7468 6520 6465 6661  False` (the defa
+00004b60: 756c 7429 2070 726f 7669 6465 7320 6120  ult) provides a 
+00004b70: 6e69 6365 7220 604d 6170 7069 6e67 6020  nicer `Mapping` 
+00004b80: 696e 7465 7266 6163 652e 2050 6173 730d  interface. Pass.
+00004b90: 0a20 2020 2020 2020 2060 6e61 7469 7665  .        `native
+00004ba0: 3d54 7275 6560 2074 6f20 6765 7420 7468  =True` to get th
+00004bb0: 6520 6f72 6967 696e 616c 2060 7079 6d6d  e original `pymm
+00004bc0: 636f 7265 2e43 6f6e 6669 6775 7261 7469  core.Configurati
+00004bd0: 6f6e 6020 6f62 6a65 6374 2e0d 0a20 2020  on` object...   
+00004be0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004bf0: 2020 6366 6720 3d20 7375 7065 7228 292e    cfg = super().
+00004c00: 6765 7453 7973 7465 6d53 7461 7465 2829  getSystemState()
+00004c10: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00004c20: 2063 6667 2069 6620 6e61 7469 7665 2065   cfg if native e
+00004c30: 6c73 6520 436f 6e66 6967 7572 6174 696f  lse Configuratio
+00004c40: 6e2e 6672 6f6d 5f63 6f6e 6669 6775 7261  n.from_configura
+00004c50: 7469 6f6e 2863 6667 290d 0a0d 0a20 2020  tion(cfg)....   
+00004c60: 2064 6566 2067 6574 5379 7374 656d 5374   def getSystemSt
+00004c70: 6174 6543 6163 6865 280d 0a20 2020 2020  ateCache(..     
+00004c80: 2020 2073 656c 662c 202a 2c20 6e61 7469     self, *, nati
+00004c90: 7665 3a20 626f 6f6c 203d 2046 616c 7365  ve: bool = False
+00004ca0: 0d0a 2020 2020 2920 2d3e 2043 6f6e 6669  ..    ) -> Confi
+00004cb0: 6775 7261 7469 6f6e 207c 2070 796d 6d63  guration | pymmc
+00004cc0: 6f72 652e 436f 6e66 6967 7572 6174 696f  ore.Configuratio
+00004cd0: 6e3a 0d0a 2020 2020 2020 2020 2222 2252  n:..        """R
+00004ce0: 6574 7572 6e20 7468 6520 656e 7469 7265  eturn the entire
+00004cf0: 2073 7973 7465 6d20 7374 6174 6520 6672   system state fr
+00004d00: 6f6d 2063 6163 6865 2e0d 0a0d 0a20 2020  om cache.....   
+00004d10: 2020 2020 202a 2a57 6879 204f 7665 7272       **Why Overr
+00004d20: 6964 653f 2a2a 2054 6865 205b 6070 796d  ide?** The [`pym
+00004d30: 6d63 6f72 655f 706c 7573 2e43 6f6e 6669  mcore_plus.Confi
+00004d40: 6775 7261 7469 6f6e 605d 5b5d 206f 626a  guration`][] obj
+00004d50: 6563 7420 7265 7475 726e 6564 0d0a 2020  ect returned..  
+00004d60: 2020 2020 2020 7768 656e 2060 6e61 7469        when `nati
+00004d70: 7665 3d46 616c 7365 6020 2874 6865 2064  ve=False` (the d
+00004d80: 6566 6175 6c74 2920 7072 6f76 6964 6573  efault) provides
+00004d90: 2061 206e 6963 6572 2060 4d61 7070 696e   a nicer `Mappin
+00004da0: 6760 2069 6e74 6572 6661 6365 2e20 5061  g` interface. Pa
+00004db0: 7373 0d0a 2020 2020 2020 2020 606e 6174  ss..        `nat
+00004dc0: 6976 653d 5472 7565 6020 746f 2067 6574  ive=True` to get
+00004dd0: 2074 6865 206f 7269 6769 6e61 6c20 6070   the original `p
+00004de0: 796d 6d63 6f72 652e 436f 6e66 6967 7572  ymmcore.Configur
+00004df0: 6174 696f 6e60 206f 626a 6563 742e 0d0a  ation` object...
+00004e00: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004e10: 2020 2020 2063 6667 203d 2073 7570 6572       cfg = super
+00004e20: 2829 2e67 6574 5379 7374 656d 5374 6174  ().getSystemStat
+00004e30: 6543 6163 6865 2829 0d0a 2020 2020 2020  eCache()..      
+00004e40: 2020 7265 7475 726e 2063 6667 2069 6620    return cfg if 
+00004e50: 6e61 7469 7665 2065 6c73 6520 436f 6e66  native else Conf
+00004e60: 6967 7572 6174 696f 6e2e 6672 6f6d 5f63  iguration.from_c
+00004e70: 6f6e 6669 6775 7261 7469 6f6e 2863 6667  onfiguration(cfg
+00004e80: 290d 0a0d 0a20 2020 2023 206d 6574 6164  )....    # metad
+00004e90: 6174 6120 6d65 7468 6f64 7320 7468 6174  ata methods that
+00004ea0: 2064 6f6e 2774 2072 6571 7569 7265 2069   don't require i
+00004eb0: 6e73 7461 6e74 6961 7469 6e67 206d 6574  nstantiating met
+00004ec0: 6164 6174 6120 6669 7273 740d 0a0d 0a20  adata first.... 
+00004ed0: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
+00004ee0: 2020 6465 6620 6765 744c 6173 7449 6d61    def getLastIma
+00004ef0: 6765 416e 644d 4428 0d0a 2020 2020 2020  geAndMD(..      
+00004f00: 2020 7365 6c66 2c20 6368 616e 6e65 6c3a    self, channel:
+00004f10: 2069 6e74 2c20 736c 6963 653a 2069 6e74   int, slice: int
+00004f20: 2c20 2a2c 2066 6978 3a20 626f 6f6c 203d  , *, fix: bool =
+00004f30: 2054 7275 650d 0a20 2020 2029 202d 3e20   True..    ) -> 
+00004f40: 7475 706c 655b 6e70 2e6e 6461 7272 6179  tuple[np.ndarray
+00004f50: 2c20 4d65 7461 6461 7461 5d3a 0d0a 2020  , Metadata]:..  
+00004f60: 2020 2020 2020 2e2e 2e0d 0a0d 0a20 2020        .......   
+00004f70: 2040 6f76 6572 6c6f 6164 0d0a 2020 2020   @overload..    
+00004f80: 6465 6620 6765 744c 6173 7449 6d61 6765  def getLastImage
+00004f90: 416e 644d 4428 7365 6c66 2c20 2a2c 2066  AndMD(self, *, f
+00004fa0: 6978 3a20 626f 6f6c 203d 2054 7275 6529  ix: bool = True)
+00004fb0: 202d 3e20 7475 706c 655b 6e70 2e6e 6461   -> tuple[np.nda
+00004fc0: 7272 6179 2c20 4d65 7461 6461 7461 5d3a  rray, Metadata]:
+00004fd0: 0d0a 2020 2020 2020 2020 2e2e 2e0d 0a0d  ..        ......
+00004fe0: 0a20 2020 2040 7379 6e63 6872 6f6e 697a  .    @synchroniz
+00004ff0: 6564 285f 6c6f 636b 290d 0a20 2020 2064  ed(_lock)..    d
+00005000: 6566 2067 6574 4c61 7374 496d 6167 6541  ef getLastImageA
+00005010: 6e64 4d44 280d 0a20 2020 2020 2020 2073  ndMD(..        s
+00005020: 656c 662c 2063 6861 6e6e 656c 3a20 696e  elf, channel: in
+00005030: 7420 7c20 4e6f 6e65 203d 204e 6f6e 652c  t | None = None,
+00005040: 2073 6c69 6365 3a20 696e 7420 7c20 4e6f   slice: int | No
+00005050: 6e65 203d 204e 6f6e 652c 202a 2c20 6669  ne = None, *, fi
+00005060: 783a 2062 6f6f 6c20 3d20 5472 7565 0d0a  x: bool = True..
+00005070: 2020 2020 2920 2d3e 2074 7570 6c65 5b6e      ) -> tuple[n
+00005080: 702e 6e64 6172 7261 792c 204d 6574 6164  p.ndarray, Metad
+00005090: 6174 615d 3a0d 0a20 2020 2020 2020 2022  ata]:..        "
+000050a0: 2222 5265 7475 726e 206c 6173 7420 696d  ""Return last im
+000050b0: 6167 6520 6672 6f6d 2074 6865 2063 6972  age from the cir
+000050c0: 6375 6c61 7220 6275 6666 6572 2061 6c6f  cular buffer alo
+000050d0: 6e67 2077 6974 6820 6d65 7461 6461 7461  ng with metadata
+000050e0: 2e0d 0a0d 0a20 2020 2020 2020 203a 7370  .....        :sp
+000050f0: 6172 6b6c 6573 3a20 2a54 6869 7320 6d65  arkles: *This me
+00005100: 7468 6f64 2069 7320 6e65 7720 696e 2060  thod is new in `
+00005110: 434d 4d43 6f72 6550 6c75 7360 2e2a 0d0a  CMMCorePlus`.*..
+00005120: 0d0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+00005130: 7320 6120 636f 6e76 656e 6965 6e63 6520  s a convenience 
+00005140: 6d65 7468 6f64 2074 6861 7420 6973 2076  method that is v
+00005150: 6572 7920 7369 6d69 6c61 7220 746f 2060  ery similar to `
+00005160: 6765 744c 6173 7449 6d61 6765 4d44 602c  getLastImageMD`,
+00005170: 2065 7863 6570 740d 0a20 2020 2020 2020   except..       
+00005180: 2074 6861 7420 6974 2064 6f65 736e 2774   that it doesn't
+00005190: 2072 6571 7569 7265 2069 6e73 7461 6e74   require instant
+000051a0: 6961 7469 6e67 2061 2060 4d65 7461 4461  iating a `MetaDa
+000051b0: 7461 6020 6f62 6a65 6374 2066 6972 7374  ta` object first
+000051c0: 2e20 4974 2072 6574 7572 6e73 2061 0d0a  . It returns a..
+000051d0: 2020 2020 2020 2020 7475 706c 6520 636f          tuple co
+000051e0: 6e74 6169 6e69 6e67 2074 6865 2069 6d61  ntaining the ima
+000051f0: 6765 2061 6e64 2061 205b 6070 796d 6d63  ge and a [`pymmc
+00005200: 6f72 655f 706c 7573 2e4d 6574 6164 6174  ore_plus.Metadat
+00005210: 6160 5d5b 5d20 6f62 6a65 6374 2e0d 0a0d  a`][] object....
+00005220: 0a20 2020 2020 2020 2049 7420 616c 736f  .        It also
+00005230: 2061 6464 7320 6120 6066 6978 6020 7061   adds a `fix` pa
+00005240: 7261 6d65 7465 722c 2077 6869 6368 2072  rameter, which r
+00005250: 6573 6861 7065 7320 6d75 6c74 692d 636f  eshapes multi-co
+00005260: 6d70 6f6e 656e 740d 0a20 2020 2020 2020  mponent..       
+00005270: 2069 6d61 6765 7320 286c 696b 6520 5247   images (like RG
+00005280: 4220 696d 6167 6573 2920 746f 2028 772c  B images) to (w,
+00005290: 2068 2c20 6e5f 636f 6d70 6f6e 656e 7473   h, n_components
+000052a0: 2920 7573 696e 670d 0a20 2020 2020 2020  ) using..       
+000052b0: 205b 6066 6978 496d 6167 6560 5d5b 7079   [`fixImage`][py
+000052c0: 6d6d 636f 7265 5f70 6c75 732e 434d 4d43  mmcore_plus.CMMC
+000052d0: 6f72 6550 6c75 732e 6669 7849 6d61 6765  orePlus.fixImage
+000052e0: 5d20 6279 2064 6566 6175 6c74 2e0d 0a0d  ] by default....
+000052f0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00005300: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+00005310: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00005320: 2063 6861 6e6e 656c 203a 2069 6e74 2c20   channel : int, 
+00005330: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00005340: 2020 2020 2020 4368 616e 6e65 6c20 696e        Channel in
+00005350: 6465 782c 2062 7920 6465 6661 756c 7420  dex, by default 
+00005360: 4e6f 6e65 0d0a 2020 2020 2020 2020 736c  None..        sl
+00005370: 6963 6520 3a20 696e 742c 206f 7074 696f  ice : int, optio
+00005380: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+00005390: 2053 6c69 6365 2069 6e64 6578 2c20 6279   Slice index, by
+000053a0: 2064 6566 6175 6c74 204e 6f6e 650d 0a20   default None.. 
+000053b0: 2020 2020 2020 2066 6978 203a 2062 6f6f         fix : boo
+000053c0: 6c2c 2064 6566 6175 6c74 3a20 5472 7565  l, default: True
+000053d0: 0d0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+000053e0: 2060 5472 7565 6020 2874 6865 2064 6566   `True` (the def
+000053f0: 6175 6c74 292c 2074 6865 6e20 696d 6167  ault), then imag
+00005400: 6573 2077 6974 6820 6e5f 636f 6d70 6f6e  es with n_compon
+00005410: 656e 7473 203e 2031 2028 6c69 6b65 2052  ents > 1 (like R
+00005420: 4742 2069 6d61 6765 7329 0d0a 2020 2020  GB images)..    
+00005430: 2020 2020 2020 2020 7769 6c6c 2062 6520          will be 
+00005440: 7265 7368 6170 6564 2074 6f20 2877 2c20  reshaped to (w, 
+00005450: 682c 206e 5f63 6f6d 706f 6e65 6e74 7329  h, n_components)
+00005460: 2075 7369 6e67 2060 6669 7849 6d61 6765   using `fixImage
+00005470: 602e 0d0a 0d0a 2020 2020 2020 2020 5265  `.....        Re
+00005480: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+00005490: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+000054a0: 7475 706c 655b 6e70 2e6e 6461 7272 6179  tuple[np.ndarray
+000054b0: 2c20 4d65 7461 6461 7461 5d0d 0a20 2020  , Metadata]..   
+000054c0: 2020 2020 2020 2020 2049 6d61 6765 2061           Image a
+000054d0: 6e64 206d 6574 6164 6174 610d 0a20 2020  nd metadata..   
+000054e0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000054f0: 2020 6d64 203d 204d 6574 6164 6174 6128    md = Metadata(
+00005500: 290d 0a20 2020 2020 2020 2069 6620 6368  )..        if ch
+00005510: 616e 6e65 6c20 6973 206e 6f74 204e 6f6e  annel is not Non
+00005520: 6520 616e 6420 736c 6963 6520 6973 206e  e and slice is n
+00005530: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00005540: 2020 2020 2020 696d 6720 3d20 7375 7065        img = supe
+00005550: 7228 292e 6765 744c 6173 7449 6d61 6765  r().getLastImage
+00005560: 4d44 2863 6861 6e6e 656c 2c20 736c 6963  MD(channel, slic
+00005570: 652c 206d 6429 0d0a 2020 2020 2020 2020  e, md)..        
+00005580: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005590: 2020 2069 6d67 203d 2073 7570 6572 2829     img = super()
+000055a0: 2e67 6574 4c61 7374 496d 6167 654d 4428  .getLastImageMD(
+000055b0: 6d64 290d 0a20 2020 2020 2020 2072 6574  md)..        ret
+000055c0: 7572 6e20 2873 656c 662e 6669 7849 6d61  urn (self.fixIma
+000055d0: 6765 2869 6d67 2920 6966 2066 6978 2065  ge(img) if fix e
+000055e0: 6c73 6520 696d 672c 206d 6429 0d0a 0d0a  lse img, md)....
+000055f0: 2020 2020 406f 7665 726c 6f61 640d 0a20      @overload.. 
+00005600: 2020 2064 6566 2070 6f70 4e65 7874 496d     def popNextIm
+00005610: 6167 6541 6e64 4d44 2873 656c 662c 2063  ageAndMD(self, c
+00005620: 6861 6e6e 656c 3a20 696e 742c 2073 6c69  hannel: int, sli
+00005630: 6365 3a20 696e 742c 202a 2c20 6669 783a  ce: int, *, fix:
+00005640: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
+00005650: 2041 6e79 3a0d 0a20 2020 2020 2020 202e   Any:..        .
+00005660: 2e2e 0d0a 0d0a 2020 2020 406f 7665 726c  ......    @overl
+00005670: 6f61 640d 0a20 2020 2064 6566 2070 6f70  oad..    def pop
+00005680: 4e65 7874 496d 6167 6541 6e64 4d44 2873  NextImageAndMD(s
+00005690: 656c 662c 202a 2c20 6669 783a 2062 6f6f  elf, *, fix: boo
+000056a0: 6c20 3d20 5472 7565 2920 2d3e 2041 6e79  l = True) -> Any
+000056b0: 3a0d 0a20 2020 2020 2020 202e 2e2e 0d0a  :..        .....
+000056c0: 0d0a 2020 2020 4073 796e 6368 726f 6e69  ..    @synchroni
+000056d0: 7a65 6428 5f6c 6f63 6b29 0d0a 2020 2020  zed(_lock)..    
+000056e0: 6465 6620 706f 704e 6578 7449 6d61 6765  def popNextImage
+000056f0: 416e 644d 4428 0d0a 2020 2020 2020 2020  AndMD(..        
+00005700: 7365 6c66 2c20 6368 616e 6e65 6c3a 2069  self, channel: i
+00005710: 6e74 207c 204e 6f6e 6520 3d20 4e6f 6e65  nt | None = None
+00005720: 2c20 736c 6963 653a 2069 6e74 207c 204e  , slice: int | N
+00005730: 6f6e 6520 3d20 4e6f 6e65 2c20 2a2c 2066  one = None, *, f
+00005740: 6978 3a20 626f 6f6c 203d 2054 7275 650d  ix: bool = True.
+00005750: 0a20 2020 2029 202d 3e20 7475 706c 655b  .    ) -> tuple[
+00005760: 6e70 2e6e 6461 7272 6179 2c20 4d65 7461  np.ndarray, Meta
+00005770: 6461 7461 5d3a 0d0a 2020 2020 2020 2020  data]:..        
+00005780: 2222 2247 6574 7320 616e 6420 7265 6d6f  """Gets and remo
+00005790: 7665 7320 7468 6520 6e65 7874 2069 6d61  ves the next ima
+000057a0: 6765 2028 616e 6420 6d65 7461 6461 7461  ge (and metadata
+000057b0: 2920 6672 6f6d 2074 6865 2063 6972 6375  ) from the circu
+000057c0: 6c61 7220 6275 6666 6572 2e0d 0a0d 0a20  lar buffer..... 
+000057d0: 2020 2020 2020 203a 7370 6172 6b6c 6573         :sparkles
+000057e0: 3a20 2a54 6869 7320 6d65 7468 6f64 2069  : *This method i
+000057f0: 7320 6e65 7720 696e 2060 434d 4d43 6f72  s new in `CMMCor
+00005800: 6550 6c75 7360 2e2a 0d0a 0d0a 2020 2020  ePlus`.*....    
+00005810: 2020 2020 5468 6973 2069 7320 6120 636f      This is a co
+00005820: 6e76 656e 6965 6e63 6520 6d65 7468 6f64  nvenience method
+00005830: 2074 6861 7420 6973 2076 6572 7920 7369   that is very si
+00005840: 6d69 6c61 7220 746f 2060 706f 704e 6578  milar to `popNex
+00005850: 7449 6d61 6765 4d44 602c 2065 7863 6570  tImageMD`, excep
+00005860: 740d 0a20 2020 2020 2020 2074 6861 7420  t..        that 
+00005870: 6974 2064 6f65 736e 2774 2072 6571 7569  it doesn't requi
+00005880: 7265 2069 6e73 7461 6e74 6961 7469 6e67  re instantiating
+00005890: 2061 2060 4d65 7461 4461 7461 6020 6f62   a `MetaData` ob
+000058a0: 6a65 6374 2066 6972 7374 2e20 4974 2072  ject first. It r
+000058b0: 6574 7572 6e73 2061 0d0a 2020 2020 2020  eturns a..      
+000058c0: 2020 7475 706c 6520 636f 6e74 6169 6e69    tuple containi
+000058d0: 6e67 2074 6865 2069 6d61 6765 2061 6e64  ng the image and
+000058e0: 2061 205b 6070 796d 6d63 6f72 655f 706c   a [`pymmcore_pl
+000058f0: 7573 2e4d 6574 6164 6174 6160 5d5b 5d20  us.Metadata`][] 
+00005900: 6f62 6a65 6374 2e0d 0a0d 0a20 2020 2020  object.....     
+00005910: 2020 2049 7420 616c 736f 2061 6464 7320     It also adds 
+00005920: 6120 6066 6978 6020 7061 7261 6d65 7465  a `fix` paramete
+00005930: 722c 2077 6869 6368 2072 6573 6861 7065  r, which reshape
+00005940: 7320 6d75 6c74 692d 636f 6d70 6f6e 656e  s multi-componen
+00005950: 740d 0a20 2020 2020 2020 2069 6d61 6765  t..        image
+00005960: 7320 286c 696b 6520 5247 4220 696d 6167  s (like RGB imag
+00005970: 6573 2920 746f 2028 772c 2068 2c20 6e5f  es) to (w, h, n_
+00005980: 636f 6d70 6f6e 656e 7473 2920 7573 696e  components) usin
+00005990: 670d 0a20 2020 2020 2020 205b 6066 6978  g..        [`fix
+000059a0: 496d 6167 6560 5d5b 7079 6d6d 636f 7265  Image`][pymmcore
+000059b0: 5f70 6c75 732e 434d 4d43 6f72 6550 6c75  _plus.CMMCorePlu
+000059c0: 732e 6669 7849 6d61 6765 5d20 6279 2064  s.fixImage] by d
+000059d0: 6566 6175 6c74 2e0d 0a0d 0a20 2020 2020  efault.....     
+000059e0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+000059f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00005a00: 2d0d 0a20 2020 2020 2020 2063 6861 6e6e  -..        chann
+00005a10: 656c 203a 2069 6e74 2c20 6f70 7469 6f6e  el : int, option
+00005a20: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+00005a30: 4368 616e 6e65 6c20 696e 6465 782c 2062  Channel index, b
+00005a40: 7920 6465 6661 756c 7420 4e6f 6e65 0d0a  y default None..
+00005a50: 2020 2020 2020 2020 736c 6963 6520 3a20          slice : 
+00005a60: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
+00005a70: 2020 2020 2020 2020 2020 2053 6c69 6365             Slice
+00005a80: 2069 6e64 6578 2c20 6279 2064 6566 6175   index, by defau
+00005a90: 6c74 204e 6f6e 650d 0a20 2020 2020 2020  lt None..       
+00005aa0: 2066 6978 203a 2062 6f6f 6c2c 2064 6566   fix : bool, def
+00005ab0: 6175 6c74 3a20 5472 7565 0d0a 2020 2020  ault: True..    
+00005ac0: 2020 2020 2020 2020 4966 2060 5472 7565          If `True
+00005ad0: 6020 2874 6865 2064 6566 6175 6c74 292c  ` (the default),
+00005ae0: 2074 6865 6e20 696d 6167 6573 2077 6974   then images wit
+00005af0: 6820 6e5f 636f 6d70 6f6e 656e 7473 203e  h n_components >
+00005b00: 2031 2028 6c69 6b65 2052 4742 2069 6d61   1 (like RGB ima
+00005b10: 6765 7329 0d0a 2020 2020 2020 2020 2020  ges)..          
+00005b20: 2020 7769 6c6c 2062 6520 7265 7368 6170    will be reshap
+00005b30: 6564 2074 6f20 2877 2c20 682c 206e 5f63  ed to (w, h, n_c
+00005b40: 6f6d 706f 6e65 6e74 7329 2075 7369 6e67  omponents) using
+00005b50: 2060 6669 7849 6d61 6765 602e 0d0a 0d0a   `fixImage`.....
+00005b60: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
+00005b70: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00005b80: 0d0a 2020 2020 2020 2020 7475 706c 655b  ..        tuple[
+00005b90: 6e70 2e6e 6461 7272 6179 2c20 4d65 7461  np.ndarray, Meta
+00005ba0: 6461 7461 5d0d 0a20 2020 2020 2020 2020  data]..         
+00005bb0: 2020 2049 6d61 6765 2061 6e64 206d 6574     Image and met
+00005bc0: 6164 6174 610d 0a20 2020 2020 2020 2022  adata..        "
+00005bd0: 2222 0d0a 2020 2020 2020 2020 6d64 203d  ""..        md =
+00005be0: 204d 6574 6164 6174 6128 290d 0a20 2020   Metadata()..   
+00005bf0: 2020 2020 2069 6620 6368 616e 6e65 6c20       if channel 
+00005c00: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00005c10: 736c 6963 6520 6973 206e 6f74 204e 6f6e  slice is not Non
+00005c20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00005c30: 696d 6720 3d20 7375 7065 7228 292e 706f  img = super().po
+00005c40: 704e 6578 7449 6d61 6765 4d44 2863 6861  pNextImageMD(cha
+00005c50: 6e6e 656c 2c20 736c 6963 652c 206d 6429  nnel, slice, md)
+00005c60: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00005c70: 0a20 2020 2020 2020 2020 2020 2069 6d67  .            img
+00005c80: 203d 2073 7570 6572 2829 2e70 6f70 4e65   = super().popNe
+00005c90: 7874 496d 6167 654d 4428 6d64 290d 0a20  xtImageMD(md).. 
+00005ca0: 2020 2020 2020 2072 6574 7572 6e20 2873         return (s
+00005cb0: 656c 662e 6669 7849 6d61 6765 2869 6d67  elf.fixImage(img
+00005cc0: 2920 6966 2066 6978 2065 6c73 6520 696d  ) if fix else im
+00005cd0: 672c 206d 6429 0d0a 0d0a 2020 2020 4073  g, md)....    @s
+00005ce0: 796e 6368 726f 6e69 7a65 6428 5f6c 6f63  ynchronized(_loc
+00005cf0: 6b29 0d0a 2020 2020 6465 6620 706f 704e  k)..    def popN
+00005d00: 6578 7449 6d61 6765 2873 656c 662c 202a  extImage(self, *
+00005d10: 2c20 6669 783a 2062 6f6f 6c20 3d20 5472  , fix: bool = Tr
+00005d20: 7565 2920 2d3e 206e 702e 6e64 6172 7261  ue) -> np.ndarra
+00005d30: 793a 0d0a 2020 2020 2020 2020 2222 2247  y:..        """G
+00005d40: 6574 7320 616e 6420 7265 6d6f 7665 7320  ets and removes 
+00005d50: 7468 6520 6e65 7874 2069 6d61 6765 2066  the next image f
+00005d60: 726f 6d20 7468 6520 6369 7263 756c 6172  rom the circular
+00005d70: 2062 7566 6665 722e 0d0a 0d0a 2020 2020   buffer.....    
+00005d80: 2020 2020 2a2a 5768 7920 4f76 6572 7269      **Why Overri
+00005d90: 6465 3f2a 2a20 746f 2061 6464 2074 6865  de?** to add the
+00005da0: 2060 6669 7860 2070 6172 616d 6574 6572   `fix` parameter
+00005db0: 2c20 7768 6963 6820 7265 7368 6170 6573  , which reshapes
+00005dc0: 206d 756c 7469 2d63 6f6d 706f 6e65 6e74   multi-component
+00005dd0: 0d0a 2020 2020 2020 2020 696d 6167 6573  ..        images
+00005de0: 2028 6c69 6b65 2052 4742 2069 6d61 6765   (like RGB image
+00005df0: 7329 2074 6f20 2877 2c20 682c 206e 5f63  s) to (w, h, n_c
+00005e00: 6f6d 706f 6e65 6e74 7329 2075 7369 6e67  omponents) using
+00005e10: 0d0a 2020 2020 2020 2020 5b60 6669 7849  ..        [`fixI
+00005e20: 6d61 6765 605d 5b70 796d 6d63 6f72 655f  mage`][pymmcore_
+00005e30: 706c 7573 2e43 4d4d 436f 7265 506c 7573  plus.CMMCorePlus
+00005e40: 2e66 6978 496d 6167 655d 2062 7920 6465  .fixImage] by de
+00005e50: 6661 756c 742e 0d0a 0d0a 2020 2020 2020  fault.....      
+00005e60: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+00005e70: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00005e80: 0d0a 2020 2020 2020 2020 6669 7820 3a20  ..        fix : 
+00005e90: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
+00005ea0: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
+00005eb0: 2049 6620 6054 7275 6560 2028 7468 6520   If `True` (the 
+00005ec0: 6465 6661 756c 7429 2c20 7468 656e 2069  default), then i
+00005ed0: 6d61 6765 7320 7769 7468 206e 5f63 6f6d  mages with n_com
+00005ee0: 706f 6e65 6e74 7320 3e20 3120 286c 696b  ponents > 1 (lik
+00005ef0: 6520 5247 4220 696d 6167 6573 290d 0a20  e RGB images).. 
+00005f00: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
+00005f10: 6265 2072 6573 6861 7065 6420 746f 2028  be reshaped to (
+00005f20: 772c 2068 2c20 6e5f 636f 6d70 6f6e 656e  w, h, n_componen
+00005f30: 7473 2920 7573 696e 6720 6066 6978 496d  ts) using `fixIm
+00005f40: 6167 6560 2e0d 0a20 2020 2020 2020 2022  age`...        "
+00005f50: 2222 0d0a 2020 2020 2020 2020 696d 673a  ""..        img:
+00005f60: 206e 702e 6e64 6172 7261 7920 3d20 7375   np.ndarray = su
+00005f70: 7065 7228 292e 706f 704e 6578 7449 6d61  per().popNextIma
+00005f80: 6765 2829 0d0a 2020 2020 2020 2020 7265  ge()..        re
+00005f90: 7475 726e 2073 656c 662e 6669 7849 6d61  turn self.fixIma
+00005fa0: 6765 2869 6d67 2920 6966 2066 6978 2065  ge(img) if fix e
+00005fb0: 6c73 6520 696d 670d 0a0d 0a20 2020 2040  lse img....    @
+00005fc0: 7379 6e63 6872 6f6e 697a 6564 285f 6c6f  synchronized(_lo
+00005fd0: 636b 290d 0a20 2020 2064 6566 2067 6574  ck)..    def get
+00005fe0: 4e42 6566 6f72 654c 6173 7449 6d61 6765  NBeforeLastImage
+00005ff0: 416e 644d 4428 0d0a 2020 2020 2020 2020  AndMD(..        
+00006000: 7365 6c66 2c20 6e3a 2069 6e74 2c20 2a2c  self, n: int, *,
+00006010: 2066 6978 3a20 626f 6f6c 203d 2054 7275   fix: bool = Tru
+00006020: 650d 0a20 2020 2029 202d 3e20 7475 706c  e..    ) -> tupl
+00006030: 655b 6e70 2e6e 6461 7272 6179 2c20 4d65  e[np.ndarray, Me
+00006040: 7461 6461 7461 5d3a 0d0a 2020 2020 2020  tadata]:..      
+00006050: 2020 2222 2252 6574 7572 6e20 696d 6167    """Return imag
+00006060: 6520 7461 6b65 6e20 606e 6020 696d 6167  e taken `n` imag
+00006070: 6573 2061 676f 2061 6c6f 6e67 2077 6974  es ago along wit
+00006080: 6820 6173 736f 6369 6174 6564 206d 6574  h associated met
+00006090: 6164 6174 612e 0d0a 0d0a 2020 2020 2020  adata.....      
+000060a0: 2020 3a73 7061 726b 6c65 733a 202a 5468    :sparkles: *Th
+000060b0: 6973 206d 6574 686f 6420 6973 206e 6577  is method is new
+000060c0: 2069 6e20 6043 4d4d 436f 7265 506c 7573   in `CMMCorePlus
+000060d0: 602e 2a0d 0a0d 0a20 2020 2020 2020 2054  `.*....        T
+000060e0: 6869 7320 6973 2061 2063 6f6e 7665 6e69  his is a conveni
+000060f0: 656e 6365 206d 6574 686f 6420 7468 6174  ence method that
+00006100: 2069 7320 7665 7279 2073 696d 696c 6172   is very similar
+00006110: 2074 6f20 6067 6574 4e42 6566 6f72 654c   to `getNBeforeL
+00006120: 6173 7449 6d61 6765 4d44 602c 0d0a 2020  astImageMD`,..  
+00006130: 2020 2020 2020 6578 6365 7074 2074 6861        except tha
+00006140: 7420 6974 2064 6f65 736e 2774 2072 6571  t it doesn't req
+00006150: 7569 7265 2069 6e73 7461 6e74 6961 7469  uire instantiati
+00006160: 6e67 2061 2060 4d65 7461 4461 7461 6020  ng a `MetaData` 
+00006170: 6f62 6a65 6374 2066 6972 7374 2e20 4974  object first. It
+00006180: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00006190: 7320 6120 7475 706c 6520 636f 6e74 6169  s a tuple contai
+000061a0: 6e69 6e67 2074 6865 2069 6d61 6765 2061  ning the image a
+000061b0: 6e64 2061 205b 6070 796d 6d63 6f72 655f  nd a [`pymmcore_
+000061c0: 706c 7573 2e4d 6574 6164 6174 6160 5d5b  plus.Metadata`][
+000061d0: 5d20 6f62 6a65 6374 2e0d 0a0d 0a20 2020  ] object.....   
+000061e0: 2020 2020 2049 7420 616c 736f 2061 6464       It also add
+000061f0: 7320 6120 6066 6978 6020 7061 7261 6d65  s a `fix` parame
+00006200: 7465 722c 2077 6869 6368 2072 6573 6861  ter, which resha
+00006210: 7065 7320 6d75 6c74 692d 636f 6d70 6f6e  pes multi-compon
+00006220: 656e 740d 0a20 2020 2020 2020 2069 6d61  ent..        ima
+00006230: 6765 7320 286c 696b 6520 5247 4220 696d  ges (like RGB im
+00006240: 6167 6573 2920 746f 2028 772c 2068 2c20  ages) to (w, h, 
+00006250: 6e5f 636f 6d70 6f6e 656e 7473 2920 7573  n_components) us
+00006260: 696e 670d 0a20 2020 2020 2020 205b 6066  ing..        [`f
+00006270: 6978 496d 6167 6560 5d5b 7079 6d6d 636f  ixImage`][pymmco
+00006280: 7265 5f70 6c75 732e 434d 4d43 6f72 6550  re_plus.CMMCoreP
+00006290: 6c75 732e 6669 7849 6d61 6765 5d20 6279  lus.fixImage] by
+000062a0: 2064 6566 6175 6c74 2e0d 0a0d 0a20 2020   default.....   
+000062b0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+000062c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000062d0: 2d2d 2d0d 0a20 2020 2020 2020 206e 203a  ---..        n :
+000062e0: 2069 6e74 0d0a 2020 2020 2020 2020 2020   int..          
+000062f0: 2020 5468 6520 6e75 6d62 6572 206f 6620    The number of 
+00006300: 696d 6167 6573 2061 676f 2074 6f20 7265  images ago to re
+00006310: 7472 6965 7665 2e20 3020 6973 2074 6865  trieve. 0 is the
+00006320: 206c 6173 7420 696d 6167 652c 2031 2069   last image, 1 i
+00006330: 7320 7468 650d 0a20 2020 2020 2020 2020  s the..         
+00006340: 2020 2069 6d61 6765 2062 6566 6f72 6520     image before 
+00006350: 7468 6174 2c20 6574 632e 0d0a 2020 2020  that, etc...    
+00006360: 2020 2020 6669 7820 3a20 626f 6f6c 2c20      fix : bool, 
+00006370: 6465 6661 756c 743a 2054 7275 650d 0a20  default: True.. 
+00006380: 2020 2020 2020 2020 2020 2049 6620 6054             If `T
+00006390: 7275 6560 2028 7468 6520 6465 6661 756c  rue` (the defaul
+000063a0: 7429 2c20 7468 656e 2069 6d61 6765 7320  t), then images 
+000063b0: 7769 7468 206e 5f63 6f6d 706f 6e65 6e74  with n_component
+000063c0: 7320 3e20 3120 286c 696b 6520 5247 4220  s > 1 (like RGB 
+000063d0: 696d 6167 6573 290d 0a20 2020 2020 2020  images)..       
+000063e0: 2020 2020 2077 696c 6c20 6265 2072 6573       will be res
+000063f0: 6861 7065 6420 746f 2028 772c 2068 2c20  haped to (w, h, 
+00006400: 6e5f 636f 6d70 6f6e 656e 7473 2920 7573  n_components) us
+00006410: 696e 6720 6066 6978 496d 6167 6560 2e0d  ing `fixImage`..
+00006420: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00006430: 2020 2020 2020 6d64 203d 204d 6574 6164        md = Metad
+00006440: 6174 6128 290d 0a20 2020 2020 2020 2069  ata()..        i
+00006450: 6d67 203d 2073 7570 6572 2829 2e67 6574  mg = super().get
+00006460: 4e42 6566 6f72 654c 6173 7449 6d61 6765  NBeforeLastImage
+00006470: 4d44 286e 2c20 6d64 290d 0a20 2020 2020  MD(n, md)..     
+00006480: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
+00006490: 6978 496d 6167 6528 696d 6729 2069 6620  ixImage(img) if 
+000064a0: 6669 7820 656c 7365 2069 6d67 2c20 6d64  fix else img, md
+000064b0: 0d0a 0d0a 2020 2020 6465 6620 7365 7443  ....    def setC
+000064c0: 6f6e 6669 6728 7365 6c66 2c20 6772 6f75  onfig(self, grou
+000064d0: 704e 616d 653a 2073 7472 2c20 636f 6e66  pName: str, conf
+000064e0: 6967 4e61 6d65 3a20 7374 7229 202d 3e20  igName: str) -> 
+000064f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2022  None:..        "
+00006500: 2222 4170 706c 6965 7320 6120 636f 6e66  ""Applies a conf
+00006510: 6967 7572 6174 696f 6e20 746f 2061 2067  iguration to a g
+00006520: 726f 7570 2e0d 0a0d 0a20 2020 2020 2020  roup.....       
+00006530: 202a 2a57 6879 204f 7665 7272 6964 653f   **Why Override?
+00006540: 2a2a 2054 6865 206e 6174 6976 6520 606f  ** The native `o
+00006550: 6e43 6f6e 6669 6747 726f 7570 4368 616e  nConfigGroupChan
+00006560: 6765 6460 2063 616c 6c62 6163 6b20 6973  ged` callback is
+00006570: 206e 6f74 2061 6c77 6179 730d 0a20 2020   not always..   
+00006580: 2020 2020 2063 616c 6c65 6420 7768 656e       called when
+00006590: 6576 6572 2060 434d 4d43 6f72 652e 7365  ever `CMMCore.se
+000065a0: 7443 6f6e 6669 6760 2068 6173 2062 6565  tConfig` has bee
+000065b0: 6e20 6361 6c6c 6564 2e20 5765 206f 7665  n called. We ove
+000065c0: 7272 6964 6520 6865 7265 2074 6f20 656d  rride here to em
+000065d0: 6974 0d0a 2020 2020 2020 2020 6120 6063  it..        a `c
+000065e0: 6f6e 6669 6753 6574 6020 6576 656e 7420  onfigSet` event 
+000065f0: 7768 656e 6576 6572 2060 7365 7443 6f6e  whenever `setCon
+00006600: 6669 6760 2069 7320 6361 6c6c 6564 2e0d  fig` is called..
+00006610: 0a20 2020 2020 2020 2053 6565 203c 6874  .        See <ht
+00006620: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00006630: 2f6d 6963 726f 2d6d 616e 6167 6572 2f6d  /micro-manager/m
+00006640: 6d43 6f72 6541 6e64 4465 7669 6365 732f  mCoreAndDevices/
+00006650: 6973 7375 6573 2f32 353e 2066 6f72 2064  issues/25> for d
+00006660: 6574 6169 6c73 2e0d 0a20 2020 2020 2020  etails...       
+00006670: 2022 2222 0d0a 2020 2020 2020 2020 7375   """..        su
+00006680: 7065 7228 292e 7365 7443 6f6e 6669 6728  per().setConfig(
+00006690: 6772 6f75 704e 616d 652c 2063 6f6e 6669  groupName, confi
+000066a0: 674e 616d 6529 0d0a 2020 2020 2020 2020  gName)..        
+000066b0: 7365 6c66 2e65 7665 6e74 732e 636f 6e66  self.events.conf
+000066c0: 6967 5365 742e 656d 6974 2867 726f 7570  igSet.emit(group
+000066d0: 4e61 6d65 2c20 636f 6e66 6967 4e61 6d65  Name, configName
+000066e0: 290d 0a0d 0a20 2020 2023 204e 4557 206d  )....    # NEW m
+000066f0: 6574 686f 6473 0d0a 0d0a 2020 2020 406f  ethods....    @o
+00006700: 7665 726c 6f61 640d 0a20 2020 2064 6566  verload..    def
+00006710: 2069 7465 7244 6576 6963 6541 6461 7074   iterDeviceAdapt
+00006720: 6572 7328 0d0a 2020 2020 2020 2020 7365  ers(..        se
+00006730: 6c66 2c0d 0a20 2020 2020 2020 2061 6461  lf,..        ada
+00006740: 7074 6572 5f70 6174 7465 726e 3a20 7374  pter_pattern: st
+00006750: 7220 7c20 7265 2e50 6174 7465 726e 207c  r | re.Pattern |
+00006760: 204e 6f6e 6520 3d20 2e2e 2e2c 0d0a 2020   None = ...,..  
+00006770: 2020 2020 2020 2a2c 0d0a 2020 2020 2020        *,..      
+00006780: 2020 6173 5f6f 626a 6563 743a 204c 6974    as_object: Lit
+00006790: 6572 616c 5b54 7275 655d 203d 202e 2e2e  eral[True] = ...
+000067a0: 2c0d 0a20 2020 2029 202d 3e20 4974 6572  ,..    ) -> Iter
+000067b0: 6174 6f72 5b44 6576 6963 6541 6461 7074  ator[DeviceAdapt
+000067c0: 6572 5d3a 0d0a 2020 2020 2020 2020 2e2e  er]:..        ..
+000067d0: 2e0d 0a0d 0a20 2020 2040 6f76 6572 6c6f  .....    @overlo
+000067e0: 6164 0d0a 2020 2020 6465 6620 6974 6572  ad..    def iter
+000067f0: 4465 7669 6365 4164 6170 7465 7273 280d  DeviceAdapters(.
+00006800: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
+00006810: 2020 2020 2020 2020 6164 6170 7465 725f          adapter_
+00006820: 7061 7474 6572 6e3a 2073 7472 207c 2072  pattern: str | r
+00006830: 652e 5061 7474 6572 6e20 7c20 4e6f 6e65  e.Pattern | None
+00006840: 203d 202e 2e2e 2c0d 0a20 2020 2020 2020   = ...,..       
+00006850: 202a 2c0d 0a20 2020 2020 2020 2061 735f   *,..        as_
+00006860: 6f62 6a65 6374 3a20 4c69 7465 7261 6c5b  object: Literal[
+00006870: 4661 6c73 655d 2c0d 0a20 2020 2029 202d  False],..    ) -
+00006880: 3e20 4974 6572 6174 6f72 5b73 7472 5d3a  > Iterator[str]:
+00006890: 0d0a 2020 2020 2020 2020 2e2e 2e0d 0a0d  ..        ......
+000068a0: 0a20 2020 2064 6566 2069 7465 7244 6576  .    def iterDev
+000068b0: 6963 6541 6461 7074 6572 7328 0d0a 2020  iceAdapters(..  
+000068c0: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+000068d0: 2020 2020 2061 6461 7074 6572 5f70 6174       adapter_pat
+000068e0: 7465 726e 3a20 7374 7220 7c20 7265 2e50  tern: str | re.P
+000068f0: 6174 7465 726e 207c 204e 6f6e 6520 3d20  attern | None = 
+00006900: 4e6f 6e65 2c0d 0a20 2020 2020 2020 202a  None,..        *
+00006910: 2c0d 0a20 2020 2020 2020 2061 735f 6f62  ,..        as_ob
+00006920: 6a65 6374 3a20 626f 6f6c 203d 2054 7275  ject: bool = Tru
+00006930: 652c 0d0a 2020 2020 2920 2d3e 2049 7465  e,..    ) -> Ite
+00006940: 7261 746f 725b 4465 7669 6365 4164 6170  rator[DeviceAdap
+00006950: 7465 725d 207c 2049 7465 7261 746f 725b  ter] | Iterator[
+00006960: 7374 725d 3a0d 0a20 2020 2020 2020 2022  str]:..        "
+00006970: 2222 4974 6572 6174 6520 6f76 6572 2061  ""Iterate over a
+00006980: 6c6c 2061 7661 696c 6162 6c65 2064 6576  ll available dev
+00006990: 6963 6520 6164 6170 7465 7273 2e0d 0a0d  ice adapters....
+000069a0: 0a20 2020 2020 2020 203a 7370 6172 6b6c  .        :sparkl
+000069b0: 6573 3a20 2a54 6869 7320 6d65 7468 6f64  es: *This method
+000069c0: 2069 7320 6e65 7720 696e 2060 434d 4d43   is new in `CMMC
+000069d0: 6f72 6550 6c75 7360 2e2a 0d0a 0d0a 2020  orePlus`.*....  
+000069e0: 2020 2020 2020 4974 206f 6666 6572 7320        It offers 
+000069f0: 6120 636f 6e76 656e 6965 6e74 2077 6179  a convenient way
+00006a00: 2074 6f20 6974 6572 6174 6520 6f76 6572   to iterate over
+00006a10: 2061 7661 696c 6162 6c65 2064 6576 6963   available devic
+00006a20: 6520 6164 6170 746f 7220 6c69 6272 6172  e adaptor librar
+00006a30: 6965 732c 0d0a 2020 2020 2020 2020 6f70  ies,..        op
+00006a40: 7469 6f6e 616c 6c79 2066 696c 7465 7269  tionally filteri
+00006a50: 6e67 2061 6461 7074 6572 206c 6962 7261  ng adapter libra
+00006a60: 7279 206e 616d 652e 2049 7420 6361 6e20  ry name. It can 
+00006a70: 616c 736f 2079 6965 6c64 0d0a 2020 2020  also yield..    
+00006a80: 2020 2020 5b60 4164 6170 7465 7260 5d5b      [`Adapter`][
+00006a90: 7079 6d6d 636f 7265 5f70 6c75 732e 4465  pymmcore_plus.De
+00006aa0: 7669 6365 4164 6170 7465 725d 206f 626a  viceAdapter] obj
+00006ab0: 6563 7473 2069 6620 6061 735f 6f62 6a65  ects if `as_obje
+00006ac0: 6374 6020 6973 2060 5472 7565 6020 2874  ct` is `True` (t
+00006ad0: 6865 0d0a 2020 2020 2020 2020 6465 6661  he..        defa
+00006ae0: 756c 7429 0d0a 0d0a 2020 2020 2020 2020  ult)....        
+00006af0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00006b00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00006b10: 2020 2020 2020 2020 6164 6170 7465 725f          adapter_
+00006b20: 7061 7474 6572 6e20 3a20 7374 7220 7c20  pattern : str | 
+00006b30: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00006b40: 2020 4465 7669 6365 2061 6461 7074 6572    Device adapter
+00006b50: 206e 616d 6520 6f72 2070 6174 7465 726e   name or pattern
+00006b60: 2074 6f20 6669 6c74 6572 2062 792c 2062   to filter by, b
+00006b70: 7920 6465 6661 756c 7420 616c 6c20 6465  y default all de
+00006b80: 7669 6365 2061 6461 7074 6572 730d 0a20  vice adapters.. 
+00006b90: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
+00006ba0: 6265 2079 6965 6c64 6564 2e0d 0a20 2020  be yielded...   
+00006bb0: 2020 2020 2061 735f 6f62 6a65 6374 203a       as_object :
+00006bc0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
+00006bd0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+00006be0: 6054 7275 6560 2c20 6041 6461 7074 6572  `True`, `Adapter
+00006bf0: 6020 6f62 6a65 6374 7320 7769 6c6c 2062  ` objects will b
+00006c00: 6520 7969 656c 6465 6420 696e 7374 6561  e yielded instea
+00006c10: 6420 6f66 0d0a 2020 2020 2020 2020 2020  d of..          
+00006c20: 2020 6c69 6272 6172 7920 6e61 6d65 2073    library name s
+00006c30: 7472 696e 6773 2e20 4279 2064 6566 6175  trings. By defau
+00006c40: 6c74 2054 7275 650d 0a0d 0a20 2020 2020  lt True....     
+00006c50: 2020 2059 6965 6c64 730d 0a20 2020 2020     Yields..     
+00006c60: 2020 202d 2d2d 2d2d 2d0d 0a20 2020 2020     ------..     
+00006c70: 2020 2044 6576 6963 6520 7c20 7374 720d     Device | str.
+00006c80: 0a20 2020 2020 2020 2020 2020 2060 4465  .            `De
+00006c90: 7669 6365 6020 6f62 6a65 6374 7320 2869  vice` objects (i
+00006ca0: 6620 6061 735f 6f62 6a65 6374 3d3d 5472  f `as_object==Tr
+00006cb0: 7565 6029 206f 7220 6465 7669 6365 206c  ue`) or device l
+00006cc0: 6162 656c 2073 7472 696e 6773 2e0d 0a20  abel strings... 
+00006cd0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00006ce0: 2020 2020 6164 6170 7465 7273 3a20 5365      adapters: Se
+00006cf0: 7175 656e 6365 5b73 7472 5d20 3d20 7375  quence[str] = su
+00006d00: 7065 7228 292e 6765 7444 6576 6963 6541  per().getDeviceA
+00006d10: 6461 7074 6572 4e61 6d65 7328 290d 0a0d  dapterNames()...
+00006d20: 0a20 2020 2020 2020 2069 6620 6164 6170  .        if adap
+00006d30: 7465 725f 7061 7474 6572 6e3a 0d0a 2020  ter_pattern:..  
+00006d40: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00006d50: 6e73 7461 6e63 6528 6164 6170 7465 725f  nstance(adapter_
+00006d60: 7061 7474 6572 6e2c 2073 7472 293a 0d0a  pattern, str):..
+00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 7074 726e 203d 2072 652e 636f 6d70 696c  ptrn = re.compil
+00006d90: 6528 6164 6170 7465 725f 7061 7474 6572  e(adapter_patter
+00006da0: 6e2c 2072 652e 4947 4e4f 5245 4341 5345  n, re.IGNORECASE
+00006db0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00006dc0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00006dd0: 2020 2020 2020 7074 726e 203d 2061 6461        ptrn = ada
+00006de0: 7074 6572 5f70 6174 7465 726e 0d0a 2020  pter_pattern..  
+00006df0: 2020 2020 2020 2020 2020 6164 6170 7465            adapte
+00006e00: 7273 203d 205b 6420 666f 7220 6420 696e  rs = [d for d in
+00006e10: 2061 6461 7074 6572 7320 6966 2070 7472   adapters if ptr
+00006e20: 6e2e 7365 6172 6368 2864 295d 0d0a 0d0a  n.search(d)]....
+00006e30: 2020 2020 2020 2020 666f 7220 6164 6170          for adap
+00006e40: 7465 7220 696e 2061 6461 7074 6572 733a  ter in adapters:
+00006e50: 0d0a 2020 2020 2020 2020 2020 2020 7969  ..            yi
+00006e60: 656c 6420 4465 7669 6365 4164 6170 7465  eld DeviceAdapte
+00006e70: 7228 6164 6170 7465 722c 206d 6d63 6f72  r(adapter, mmcor
+00006e80: 653d 7365 6c66 2920 6966 2061 735f 6f62  e=self) if as_ob
+00006e90: 6a65 6374 2065 6c73 6520 6164 6170 7465  ject else adapte
+00006ea0: 720d 0a0d 0a20 2020 2040 6f76 6572 6c6f  r....    @overlo
+00006eb0: 6164 0d0a 2020 2020 6465 6620 6974 6572  ad..    def iter
+00006ec0: 4465 7669 6365 7328 0d0a 2020 2020 2020  Devices(..      
+00006ed0: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00006ee0: 2064 6576 6963 655f 7479 7065 3a20 696e   device_type: in
+00006ef0: 7420 7c20 4974 6572 6162 6c65 5b69 6e74  t | Iterable[int
+00006f00: 5d20 7c20 4e6f 6e65 203d 202e 2e2e 2c0d  ] | None = ...,.
+00006f10: 0a20 2020 2020 2020 2064 6576 6963 655f  .        device_
+00006f20: 6c61 6265 6c3a 2073 7472 207c 2072 652e  label: str | re.
+00006f30: 5061 7474 6572 6e20 7c20 4e6f 6e65 203d  Pattern | None =
+00006f40: 202e 2e2e 2c0d 0a20 2020 2020 2020 2064   ...,..        d
+00006f50: 6576 6963 655f 6164 6170 7465 723a 2073  evice_adapter: s
+00006f60: 7472 207c 2072 652e 5061 7474 6572 6e20  tr | re.Pattern 
+00006f70: 7c20 4e6f 6e65 203d 202e 2e2e 2c0d 0a20  | None = ...,.. 
+00006f80: 2020 2020 2020 202a 2c0d 0a20 2020 2020         *,..     
+00006f90: 2020 2061 735f 6f62 6a65 6374 3a20 4c69     as_object: Li
+00006fa0: 7465 7261 6c5b 4661 6c73 655d 2c0d 0a20  teral[False],.. 
+00006fb0: 2020 2029 202d 3e20 4974 6572 6174 6f72     ) -> Iterator
+00006fc0: 5b73 7472 5d3a 0d0a 2020 2020 2020 2020  [str]:..        
+00006fd0: 2e2e 2e0d 0a0d 0a20 2020 2040 6f76 6572  .......    @over
+00006fe0: 6c6f 6164 0d0a 2020 2020 6465 6620 6974  load..    def it
+00006ff0: 6572 4465 7669 6365 7328 0d0a 2020 2020  erDevices(..    
+00007000: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+00007010: 2020 2064 6576 6963 655f 7479 7065 3a20     device_type: 
+00007020: 696e 7420 7c20 4974 6572 6162 6c65 5b69  int | Iterable[i
+00007030: 6e74 5d20 7c20 4e6f 6e65 203d 202e 2e2e  nt] | None = ...
+00007040: 2c0d 0a20 2020 2020 2020 2064 6576 6963  ,..        devic
+00007050: 655f 6c61 6265 6c3a 2073 7472 207c 2072  e_label: str | r
+00007060: 652e 5061 7474 6572 6e20 7c20 4e6f 6e65  e.Pattern | None
+00007070: 203d 202e 2e2e 2c0d 0a20 2020 2020 2020   = ...,..       
+00007080: 2064 6576 6963 655f 6164 6170 7465 723a   device_adapter:
+00007090: 2073 7472 207c 2072 652e 5061 7474 6572   str | re.Patter
+000070a0: 6e20 7c20 4e6f 6e65 203d 202e 2e2e 2c0d  n | None = ...,.
+000070b0: 0a20 2020 2020 2020 202a 2c0d 0a20 2020  .        *,..   
+000070c0: 2020 2020 2061 735f 6f62 6a65 6374 3a20       as_object: 
+000070d0: 4c69 7465 7261 6c5b 5472 7565 5d20 3d20  Literal[True] = 
+000070e0: 2e2e 2e2c 0d0a 2020 2020 2920 2d3e 2049  ...,..    ) -> I
+000070f0: 7465 7261 746f 725b 4465 7669 6365 5d3a  terator[Device]:
+00007100: 0d0a 2020 2020 2020 2020 2e2e 2e0d 0a0d  ..        ......
+00007110: 0a20 2020 2064 6566 2069 7465 7244 6576  .    def iterDev
+00007120: 6963 6573 280d 0a20 2020 2020 2020 2073  ices(..        s
+00007130: 656c 662c 0d0a 2020 2020 2020 2020 6465  elf,..        de
+00007140: 7669 6365 5f74 7970 653a 2069 6e74 207c  vice_type: int |
+00007150: 2049 7465 7261 626c 655b 696e 745d 207c   Iterable[int] |
+00007160: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
+00007170: 2020 2020 2020 2064 6576 6963 655f 6c61         device_la
+00007180: 6265 6c3a 2073 7472 207c 2072 652e 5061  bel: str | re.Pa
+00007190: 7474 6572 6e20 7c20 4e6f 6e65 203d 204e  ttern | None = N
+000071a0: 6f6e 652c 0d0a 2020 2020 2020 2020 6465  one,..        de
+000071b0: 7669 6365 5f61 6461 7074 6572 3a20 7374  vice_adapter: st
+000071c0: 7220 7c20 7265 2e50 6174 7465 726e 207c  r | re.Pattern |
+000071d0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
+000071e0: 2020 2020 2020 202a 2c0d 0a20 2020 2020         *,..     
+000071f0: 2020 2061 735f 6f62 6a65 6374 3a20 626f     as_object: bo
+00007200: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
+00007210: 2920 2d3e 2049 7465 7261 746f 725b 4465  ) -> Iterator[De
+00007220: 7669 6365 5d20 7c20 4974 6572 6174 6f72  vice] | Iterator
+00007230: 5b73 7472 5d3a 0d0a 2020 2020 2020 2020  [str]:..        
+00007240: 2222 2249 7465 7261 7465 206f 7665 7220  """Iterate over 
+00007250: 6375 7272 656e 746c 7920 6c6f 6164 6564  currently loaded
+00007260: 2064 6576 6963 6573 2e0d 0a0d 0a20 2020   devices.....   
+00007270: 2020 2020 203a 7370 6172 6b6c 6573 3a20       :sparkles: 
+00007280: 2a54 6869 7320 6d65 7468 6f64 2069 7320  *This method is 
+00007290: 6e65 7720 696e 2060 434d 4d43 6f72 6550  new in `CMMCoreP
+000072a0: 6c75 7360 2e2a 0d0a 0d0a 2020 2020 2020  lus`.*....      
+000072b0: 2020 4974 206f 6666 6572 7320 6120 636f    It offers a co
+000072c0: 6e76 656e 6965 6e74 2077 6179 2074 6f20  nvenient way to 
+000072d0: 6974 6572 6174 6520 6f76 6572 206c 6f61  iterate over loa
+000072e0: 6465 6420 6465 7669 6365 732c 206f 7074  ded devices, opt
+000072f0: 696f 6e61 6c6c 7920 6669 6c74 6572 696e  ionally filterin
+00007300: 670d 0a20 2020 2020 2020 2062 7920 5b60  g..        by [`
+00007310: 4465 7669 6365 5479 7065 605d 5b70 796d  DeviceType`][pym
+00007320: 6d63 6f72 655f 706c 7573 2e44 6576 6963  mcore_plus.Devic
+00007330: 6554 7970 655d 2061 6e64 2f6f 7220 6465  eType] and/or de
+00007340: 7669 6365 206c 6162 656c 2e20 4974 2063  vice label. It c
+00007350: 616e 2061 6c73 6f0d 0a20 2020 2020 2020  an also..       
+00007360: 2079 6965 6c64 205b 6044 6576 6963 6560   yield [`Device`
+00007370: 5d5b 7079 6d6d 636f 7265 5f70 6c75 732e  ][pymmcore_plus.
+00007380: 4465 7669 6365 5d20 6f62 6a65 6374 7320  Device] objects 
+00007390: 6966 2060 6173 5f6f 626a 6563 7460 2069  if `as_object` i
+000073a0: 730d 0a20 2020 2020 2020 2060 5472 7565  s..        `True
+000073b0: 6020 2874 6865 2064 6566 6175 6c74 292e  ` (the default).
+000073c0: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+000073d0: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+000073e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+000073f0: 2020 2020 6465 7669 6365 5f74 7970 6520      device_type 
+00007400: 3a20 4465 7669 6365 5479 7065 207c 204e  : DeviceType | N
+00007410: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00007420: 2044 6576 6963 6554 7970 6520 746f 2066   DeviceType to f
+00007430: 696c 7465 7220 6279 2c20 6279 2064 6566  ilter by, by def
+00007440: 6175 6c74 2061 6c6c 2064 6576 6963 6520  ault all device 
+00007450: 7479 7065 7320 7769 6c6c 2062 6520 7969  types will be yi
+00007460: 656c 6465 642e 0d0a 2020 2020 2020 2020  elded...        
+00007470: 6465 7669 6365 5f6c 6162 656c 203a 2073  device_label : s
+00007480: 7472 207c 204e 6f6e 650d 0a20 2020 2020  tr | None..     
+00007490: 2020 2020 2020 2044 6576 6963 6520 6c61         Device la
+000074a0: 6265 6c20 746f 2066 696c 7465 7220 6279  bel to filter by
+000074b0: 2c20 6279 2064 6566 6175 6c74 2061 6c6c  , by default all
+000074c0: 2064 6576 6963 6520 6c61 6265 6c73 2077   device labels w
+000074d0: 696c 6c20 6265 2079 6965 6c64 6564 2e0d  ill be yielded..
+000074e0: 0a20 2020 2020 2020 2064 6576 6963 655f  .        device_
+000074f0: 6164 6170 7465 7220 3a20 7374 7220 7c20  adapter : str | 
+00007500: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00007510: 2020 4465 7669 6365 2061 6461 7074 6572    Device adapter
+00007520: 206c 6962 7261 7279 2074 6f20 6669 6c74   library to filt
+00007530: 6572 2062 792c 2062 7920 6465 6661 756c  er by, by defaul
+00007540: 7420 6465 7669 6365 7320 6672 6f6d 2061  t devices from a
+00007550: 6c6c 206c 6962 7261 7269 6573 0d0a 2020  ll libraries..  
+00007560: 2020 2020 2020 2020 2020 7769 6c6c 2062            will b
+00007570: 6520 7969 656c 6465 642e 0d0a 2020 2020  e yielded...    
+00007580: 2020 2020 6173 5f6f 626a 6563 7420 3a20      as_object : 
+00007590: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0d0a  bool, optional..
+000075a0: 2020 2020 2020 2020 2020 2020 4966 2060              If `
+000075b0: 5472 7565 602c 2060 4465 7669 6365 6020  True`, `Device` 
+000075c0: 6f62 6a65 6374 7320 7769 6c6c 2062 6520  objects will be 
+000075d0: 7969 656c 6465 6420 696e 7374 6561 6420  yielded instead 
+000075e0: 6f66 0d0a 2020 2020 2020 2020 2020 2020  of..            
+000075f0: 6465 7669 6365 206c 6162 656c 2073 7472  device label str
+00007600: 696e 6773 2e20 4279 2064 6566 6175 6c74  ings. By default
+00007610: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
+00007620: 2059 6965 6c64 730d 0a20 2020 2020 2020   Yields..       
+00007630: 202d 2d2d 2d2d 2d0d 0a20 2020 2020 2020   ------..       
+00007640: 2044 6576 6963 6520 7c20 7374 720d 0a20   Device | str.. 
+00007650: 2020 2020 2020 2020 2020 2060 4465 7669             `Devi
+00007660: 6365 6020 6f62 6a65 6374 7320 2869 6620  ce` objects (if 
+00007670: 6061 735f 6f62 6a65 6374 3d3d 5472 7565  `as_object==True
+00007680: 6029 206f 7220 6465 7669 6365 206c 6162  `) or device lab
+00007690: 656c 2073 7472 696e 6773 2e0d 0a20 2020  el strings...   
+000076a0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000076b0: 2020 6966 2064 6576 6963 655f 7479 7065    if device_type
+000076c0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+000076d0: 2020 2020 2020 2064 6576 6963 6573 3a20         devices: 
+000076e0: 5365 7175 656e 6365 5b73 7472 5d20 3d20  Sequence[str] = 
+000076f0: 7365 6c66 2e67 6574 4c6f 6164 6564 4465  self.getLoadedDe
+00007700: 7669 6365 7328 290d 0a20 2020 2020 2020  vices()..       
+00007710: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00007720: 2864 6576 6963 655f 7479 7065 2c20 696e  (device_type, in
+00007730: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
+00007740: 2064 6576 6963 6573 203d 2073 656c 662e   devices = self.
+00007750: 6765 744c 6f61 6465 6444 6576 6963 6573  getLoadedDevices
+00007760: 4f66 5479 7065 2864 6576 6963 655f 7479  OfType(device_ty
+00007770: 7065 290d 0a20 2020 2020 2020 2065 6c73  pe)..        els
+00007780: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00007790: 5f64 6576 6963 6573 3a20 7365 745b 7374  _devices: set[st
+000077a0: 725d 203d 2073 6574 2829 0d0a 2020 2020  r] = set()..    
+000077b0: 2020 2020 2020 2020 666f 7220 6474 7970          for dtyp
+000077c0: 6520 696e 2064 6576 6963 655f 7479 7065  e in device_type
+000077d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000077e0: 2020 205f 6465 7669 6365 732e 7570 6461     _devices.upda
+000077f0: 7465 2873 656c 662e 6765 744c 6f61 6465  te(self.getLoade
+00007800: 6444 6576 6963 6573 4f66 5479 7065 2864  dDevicesOfType(d
+00007810: 7479 7065 2929 0d0a 2020 2020 2020 2020  type))..        
+00007820: 2020 2020 6465 7669 6365 7320 3d20 6c69      devices = li
+00007830: 7374 285f 6465 7669 6365 7329 0d0a 0d0a  st(_devices)....
+00007840: 2020 2020 2020 2020 6966 2064 6576 6963          if devic
+00007850: 655f 6c61 6265 6c3a 0d0a 2020 2020 2020  e_label:..      
+00007860: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00007870: 6e63 6528 6465 7669 6365 5f6c 6162 656c  nce(device_label
+00007880: 2c20 7374 7229 3a0d 0a20 2020 2020 2020  , str):..       
+00007890: 2020 2020 2020 2020 2070 7472 6e20 3d20           ptrn = 
+000078a0: 7265 2e63 6f6d 7069 6c65 2864 6576 6963  re.compile(devic
+000078b0: 655f 6c61 6265 6c2c 2072 652e 4947 4e4f  e_label, re.IGNO
+000078c0: 5245 4341 5345 290d 0a20 2020 2020 2020  RECASE)..       
+000078d0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000078e0: 2020 2020 2020 2020 2020 2020 7074 726e              ptrn
+000078f0: 203d 2064 6576 6963 655f 6c61 6265 6c0d   = device_label.
+00007900: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
+00007910: 6963 6573 203d 205b 6420 666f 7220 6420  ices = [d for d 
+00007920: 696e 2064 6576 6963 6573 2069 6620 7074  in devices if pt
+00007930: 726e 2e73 6561 7263 6828 6429 5d0d 0a0d  rn.search(d)]...
+00007940: 0a20 2020 2020 2020 2069 6620 6465 7669  .        if devi
+00007950: 6365 5f61 6461 7074 6572 3a0d 0a20 2020  ce_adapter:..   
+00007960: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00007970: 7374 616e 6365 2864 6576 6963 655f 6164  stance(device_ad
+00007980: 6170 7465 722c 2073 7472 293a 0d0a 2020  apter, str):..  
+00007990: 2020 2020 2020 2020 2020 2020 2020 7074                pt
+000079a0: 726e 203d 2072 652e 636f 6d70 696c 6528  rn = re.compile(
+000079b0: 6465 7669 6365 5f61 6461 7074 6572 2c20  device_adapter, 
+000079c0: 7265 2e49 474e 4f52 4543 4153 4529 0d0a  re.IGNORECASE)..
+000079d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000079e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000079f0: 2020 2070 7472 6e20 3d20 6465 7669 6365     ptrn = device
+00007a00: 5f61 6461 7074 6572 0d0a 2020 2020 2020  _adapter..      
+00007a10: 2020 2020 2020 6465 7669 6365 7320 3d20        devices = 
+00007a20: 5b64 2066 6f72 2064 2069 6e20 6465 7669  [d for d in devi
+00007a30: 6365 7320 6966 2070 7472 6e2e 7365 6172  ces if ptrn.sear
+00007a40: 6368 2873 656c 662e 6765 7444 6576 6963  ch(self.getDevic
+00007a50: 654c 6962 7261 7279 2864 2929 5d0d 0a0d  eLibrary(d))]...
+00007a60: 0a20 2020 2020 2020 2066 6f72 2064 6576  .        for dev
+00007a70: 2069 6e20 6465 7669 6365 733a 0d0a 2020   in devices:..  
+00007a80: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+00007a90: 4465 7669 6365 2864 6576 2c20 6d6d 636f  Device(dev, mmco
+00007aa0: 7265 3d73 656c 6629 2069 6620 6173 5f6f  re=self) if as_o
+00007ab0: 626a 6563 7420 656c 7365 2064 6576 0d0a  bject else dev..
+00007ac0: 0d0a 2020 2020 406f 7665 726c 6f61 640d  ..    @overload.
+00007ad0: 0a20 2020 2064 6566 2069 7465 7250 726f  .    def iterPro
+00007ae0: 7065 7274 6965 7328 0d0a 2020 2020 2020  perties(..      
+00007af0: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00007b00: 2070 726f 7065 7274 795f 7479 7065 3a20   property_type: 
+00007b10: 696e 7420 7c20 4974 6572 6162 6c65 5b69  int | Iterable[i
+00007b20: 6e74 5d20 7c20 4e6f 6e65 203d 202e 2e2e  nt] | None = ...
+00007b30: 2c0d 0a20 2020 2020 2020 2070 726f 7065  ,..        prope
+00007b40: 7274 795f 6e61 6d65 5f70 6174 7465 726e  rty_name_pattern
+00007b50: 3a20 7374 7220 7c20 7265 2e50 6174 7465  : str | re.Patte
+00007b60: 726e 207c 204e 6f6e 6520 3d20 2e2e 2e2c  rn | None = ...,
+00007b70: 0d0a 2020 2020 2020 2020 2a2c 0d0a 2020  ..        *,..  
+00007b80: 2020 2020 2020 6465 7669 6365 5f74 7970        device_typ
+00007b90: 653a 2069 6e74 207c 2049 7465 7261 626c  e: int | Iterabl
+00007ba0: 655b 696e 745d 207c 204e 6f6e 6520 3d20  e[int] | None = 
+00007bb0: 2e2e 2e2c 0d0a 2020 2020 2020 2020 6465  ...,..        de
+00007bc0: 7669 6365 5f6c 6162 656c 3a20 7374 7220  vice_label: str 
+00007bd0: 7c20 7265 2e50 6174 7465 726e 207c 204e  | re.Pattern | N
+00007be0: 6f6e 6520 3d20 2e2e 2e2c 0d0a 2020 2020  one = ...,..    
+00007bf0: 2020 2020 6861 735f 6c69 6d69 7473 3a20      has_limits: 
+00007c00: 626f 6f6c 207c 204e 6f6e 6520 3d20 4e6f  bool | None = No
+00007c10: 6e65 2c0d 0a20 2020 2020 2020 2069 735f  ne,..        is_
+00007c20: 7265 6164 5f6f 6e6c 793a 2062 6f6f 6c20  read_only: bool 
+00007c30: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0d0a  | None = None,..
+00007c40: 2020 2020 2020 2020 6973 5f73 6571 7565          is_seque
+00007c50: 6e63 6561 626c 653a 2062 6f6f 6c20 7c20  nceable: bool | 
+00007c60: 4e6f 6e65 203d 204e 6f6e 652c 0d0a 2020  None = None,..  
+00007c70: 2020 2020 2020 6173 5f6f 626a 6563 743a        as_object:
+00007c80: 204c 6974 6572 616c 5b46 616c 7365 5d2c   Literal[False],
+00007c90: 0d0a 2020 2020 2920 2d3e 2049 7465 7261  ..    ) -> Itera
+00007ca0: 746f 725b 7475 706c 655b 7374 722c 2073  tor[tuple[str, s
+00007cb0: 7472 5d5d 3a0d 0a20 2020 2020 2020 202e  tr]]:..        .
+00007cc0: 2e2e 0d0a 0d0a 2020 2020 406f 7665 726c  ......    @overl
+00007cd0: 6f61 640d 0a20 2020 2064 6566 2069 7465  oad..    def ite
+00007ce0: 7250 726f 7065 7274 6965 7328 0d0a 2020  rProperties(..  
+00007cf0: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+00007d00: 2020 2020 2070 726f 7065 7274 795f 7479       property_ty
+00007d10: 7065 3a20 696e 7420 7c20 4974 6572 6162  pe: int | Iterab
+00007d20: 6c65 5b69 6e74 5d20 7c20 4e6f 6e65 203d  le[int] | None =
+00007d30: 202e 2e2e 2c0d 0a20 2020 2020 2020 2070   ...,..        p
+00007d40: 726f 7065 7274 795f 6e61 6d65 5f70 6174  roperty_name_pat
+00007d50: 7465 726e 3a20 7374 7220 7c20 7265 2e50  tern: str | re.P
+00007d60: 6174 7465 726e 207c 204e 6f6e 6520 3d20  attern | None = 
+00007d70: 2e2e 2e2c 0d0a 2020 2020 2020 2020 2a2c  ...,..        *,
+00007d80: 0d0a 2020 2020 2020 2020 6465 7669 6365  ..        device
+00007d90: 5f74 7970 653a 2069 6e74 207c 2049 7465  _type: int | Ite
+00007da0: 7261 626c 655b 696e 745d 207c 204e 6f6e  rable[int] | Non
+00007db0: 6520 3d20 2e2e 2e2c 0d0a 2020 2020 2020  e = ...,..      
+00007dc0: 2020 6465 7669 6365 5f6c 6162 656c 3a20    device_label: 
+00007dd0: 7374 7220 7c20 7265 2e50 6174 7465 726e  str | re.Pattern
+00007de0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0d0a   | None = ...,..
+00007df0: 2020 2020 2020 2020 6861 735f 6c69 6d69          has_limi
+00007e00: 7473 3a20 626f 6f6c 207c 204e 6f6e 6520  ts: bool | None 
+00007e10: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00007e20: 2069 735f 7265 6164 5f6f 6e6c 793a 2062   is_read_only: b
+00007e30: 6f6f 6c20 7c20 4e6f 6e65 203d 204e 6f6e  ool | None = Non
+00007e40: 652c 0d0a 2020 2020 2020 2020 6973 5f73  e,..        is_s
+00007e50: 6571 7565 6e63 6561 626c 653a 2062 6f6f  equenceable: boo
+00007e60: 6c20 7c20 4e6f 6e65 203d 204e 6f6e 652c  l | None = None,
+00007e70: 0d0a 2020 2020 2020 2020 6173 5f6f 626a  ..        as_obj
+00007e80: 6563 743a 204c 6974 6572 616c 5b54 7275  ect: Literal[Tru
+00007e90: 655d 203d 202e 2e2e 2c0d 0a20 2020 2029  e] = ...,..    )
+00007ea0: 202d 3e20 4974 6572 6174 6f72 5b44 6576   -> Iterator[Dev
+00007eb0: 6963 6550 726f 7065 7274 795d 3a0d 0a20  iceProperty]:.. 
+00007ec0: 2020 2020 2020 202e 2e2e 0d0a 0d0a 2020         .......  
+00007ed0: 2020 6465 6620 6974 6572 5072 6f70 6572    def iterProper
+00007ee0: 7469 6573 280d 0a20 2020 2020 2020 2073  ties(..        s
+00007ef0: 656c 662c 0d0a 2020 2020 2020 2020 7072  elf,..        pr
+00007f00: 6f70 6572 7479 5f74 7970 653a 2069 6e74  operty_type: int
+00007f10: 207c 2049 7465 7261 626c 655b 696e 745d   | Iterable[int]
+00007f20: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0d   | None = None,.
+00007f30: 0a20 2020 2020 2020 2070 726f 7065 7274  .        propert
+00007f40: 795f 6e61 6d65 5f70 6174 7465 726e 3a20  y_name_pattern: 
+00007f50: 7374 7220 7c20 7265 2e50 6174 7465 726e  str | re.Pattern
+00007f60: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0d   | None = None,.
+00007f70: 0a20 2020 2020 2020 202a 2c0d 0a20 2020  .        *,..   
+00007f80: 2020 2020 2064 6576 6963 655f 7479 7065       device_type
+00007f90: 3a20 696e 7420 7c20 4974 6572 6162 6c65  : int | Iterable
+00007fa0: 5b69 6e74 5d20 7c20 4e6f 6e65 203d 204e  [int] | None = N
+00007fb0: 6f6e 652c 0d0a 2020 2020 2020 2020 6465  one,..        de
+00007fc0: 7669 6365 5f6c 6162 656c 3a20 7374 7220  vice_label: str 
+00007fd0: 7c20 7265 2e50 6174 7465 726e 207c 204e  | re.Pattern | N
+00007fe0: 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20 2020  one = None,..   
+00007ff0: 2020 2020 2068 6173 5f6c 696d 6974 733a       has_limits:
+00008000: 2062 6f6f 6c20 7c20 4e6f 6e65 203d 204e   bool | None = N
+00008010: 6f6e 652c 0d0a 2020 2020 2020 2020 6973  one,..        is
+00008020: 5f72 6561 645f 6f6e 6c79 3a20 626f 6f6c  _read_only: bool
+00008030: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0d   | None = None,.
+00008040: 0a20 2020 2020 2020 2069 735f 7365 7175  .        is_sequ
+00008050: 656e 6365 6162 6c65 3a20 626f 6f6c 207c  enceable: bool |
+00008060: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
+00008070: 2020 2020 2020 2061 735f 6f62 6a65 6374         as_object
+00008080: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
+00008090: 2020 2020 2920 2d3e 2049 7465 7261 746f      ) -> Iterato
+000080a0: 725b 4465 7669 6365 5072 6f70 6572 7479  r[DeviceProperty
+000080b0: 5d20 7c20 4974 6572 6174 6f72 5b74 7570  ] | Iterator[tup
+000080c0: 6c65 5b73 7472 2c20 7374 725d 5d3a 0d0a  le[str, str]]:..
+000080d0: 2020 2020 2020 2020 2222 2249 7465 7261          """Itera
+000080e0: 7465 206f 7665 7220 6375 7272 656e 746c  te over currentl
+000080f0: 7920 6c6f 6164 6564 2028 6465 7669 6365  y loaded (device
+00008100: 5f6c 6162 656c 2c20 7072 6f70 6572 7479  _label, property
+00008110: 5f6e 616d 6529 2070 6169 7273 2e0d 0a0d  _name) pairs....
+00008120: 0a20 2020 2020 2020 203a 7370 6172 6b6c  .        :sparkl
+00008130: 6573 3a20 2a54 6869 7320 6d65 7468 6f64  es: *This method
+00008140: 2069 7320 6e65 7720 696e 2060 434d 4d43   is new in `CMMC
+00008150: 6f72 6550 6c75 7360 2e2a 0d0a 0d0a 2020  orePlus`.*....  
+00008160: 2020 2020 2020 4974 206f 6666 6572 7320        It offers 
+00008170: 6120 636f 6e76 656e 6965 6e74 2077 6179  a convenient way
+00008180: 2074 6f20 6974 6572 6174 6520 6f76 6572   to iterate over
+00008190: 206c 6f61 6465 6420 6465 7669 6365 732c   loaded devices,
+000081a0: 206f 7074 696f 6e61 6c6c 7920 6669 6c74   optionally filt
+000081b0: 6572 696e 670d 0a20 2020 2020 2020 2062  ering..        b
+000081c0: 7920 5b60 4465 7669 6365 5479 7065 605d  y [`DeviceType`]
+000081d0: 5b70 796d 6d63 6f72 655f 706c 7573 2e44  [pymmcore_plus.D
+000081e0: 6576 6963 6554 7970 655d 2061 6e64 2f6f  eviceType] and/o
+000081f0: 7220 6465 7669 6365 206c 6162 656c 2e20  r device label. 
+00008200: 4974 2063 616e 2061 6c73 6f0d 0a20 2020  It can also..   
+00008210: 2020 2020 2079 6965 6c64 7320 5b60 4465       yields [`De
+00008220: 7669 6365 5072 6f70 6572 7479 605d 5b70  viceProperty`][p
+00008230: 796d 6d63 6f72 655f 706c 7573 2e44 6576  ymmcore_plus.Dev
+00008240: 6963 6550 726f 7065 7274 795d 206f 626a  iceProperty] obj
+00008250: 6563 7473 2069 660d 0a20 2020 2020 2020  ects if..       
+00008260: 2060 6173 5f6f 626a 6563 7460 2069 7320   `as_object` is 
+00008270: 6054 7275 6560 2028 7468 6520 6465 6661  `True` (the defa
+00008280: 756c 7429 2e0d 0a0d 0a20 2020 2020 2020  ult).....       
+00008290: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+000082a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+000082b0: 0a20 2020 2020 2020 2070 726f 7065 7274  .        propert
+000082c0: 795f 7479 7065 203a 2069 6e74 207c 2053  y_type : int | S
+000082d0: 6571 7565 6e63 655b 696e 745d 207c 204e  equence[int] | N
+000082e0: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+000082f0: 2050 726f 7065 7274 7954 7970 6520 286f   PropertyType (o
+00008300: 7220 7479 7065 7329 2074 6f20 6669 6c74  r types) to filt
+00008310: 6572 2062 792c 2062 7920 6465 6661 756c  er by, by defaul
+00008320: 7420 616c 6c20 7072 6f70 6572 7479 2074  t all property t
+00008330: 7970 6573 2077 696c 6c0d 0a20 2020 2020  ypes will..     
+00008340: 2020 2020 2020 2062 6520 7969 656c 6465         be yielde
+00008350: 642e 0d0a 2020 2020 2020 2020 7072 6f70  d...        prop
+00008360: 6572 7479 5f6e 616d 655f 7061 7474 6572  erty_name_patter
+00008370: 6e20 3a20 7374 7220 7c20 7265 2e50 6174  n : str | re.Pat
+00008380: 7465 726e 207c 204e 6f6e 650d 0a20 2020  tern | None..   
+00008390: 2020 2020 2020 2020 2050 726f 7065 7274           Propert
+000083a0: 7920 6e61 6d65 2074 6f20 6669 6c74 6572  y name to filter
+000083b0: 2062 792c 2062 7920 6465 6661 756c 7420   by, by default 
+000083c0: 616c 6c20 7072 6f70 6572 7479 206e 616d  all property nam
+000083d0: 6573 2077 696c 6c20 6265 2079 6965 6c64  es will be yield
+000083e0: 6564 2e0d 0a20 2020 2020 2020 2020 2020  ed...           
+000083f0: 204d 6179 2062 6520 6120 636f 6d70 696c   May be a compil
+00008400: 6564 2072 6567 756c 6172 2065 7870 7265  ed regular expre
+00008410: 7373 696f 6e20 6f72 2061 2073 7472 696e  ssion or a strin
+00008420: 672c 2069 6e20 7768 6963 6820 6361 7365  g, in which case
+00008430: 2069 7420 7769 6c6c 2062 650d 0a20 2020   it will be..   
+00008440: 2020 2020 2020 2020 2063 6f6d 7069 6c65           compile
+00008450: 6420 7769 7468 2060 7265 2e49 474e 4f52  d with `re.IGNOR
+00008460: 4543 4153 4560 2e0d 0a20 2020 2020 2020  ECASE`...       
+00008470: 2064 6576 6963 655f 7479 7065 203a 2044   device_type : D
+00008480: 6576 6963 6554 7970 6520 7c20 4e6f 6e65  eviceType | None
+00008490: 0d0a 2020 2020 2020 2020 2020 2020 4465  ..            De
+000084a0: 7669 6365 5479 7065 2074 6f20 6669 6c74  viceType to filt
+000084b0: 6572 2062 792c 2062 7920 6465 6661 756c  er by, by defaul
+000084c0: 7420 616c 6c20 6465 7669 6365 2074 7970  t all device typ
+000084d0: 6573 2077 696c 6c20 6265 2079 6965 6c64  es will be yield
+000084e0: 6564 2e0d 0a20 2020 2020 2020 2064 6576  ed...        dev
+000084f0: 6963 655f 6c61 6265 6c20 3a20 7374 7220  ice_label : str 
+00008500: 7c20 4e6f 6e65 0d0a 2020 2020 2020 2020  | None..        
+00008510: 2020 2020 4465 7669 6365 206c 6162 656c      Device label
+00008520: 2074 6f20 6669 6c74 6572 2062 792c 2062   to filter by, b
+00008530: 7920 6465 6661 756c 7420 616c 6c20 6465  y default all de
+00008540: 7669 6365 206c 6162 656c 7320 7769 6c6c  vice labels will
+00008550: 2062 6520 7969 656c 6465 642e 0d0a 2020   be yielded...  
+00008560: 2020 2020 2020 6861 735f 6c69 6d69 7473        has_limits
+00008570: 203a 2062 6f6f 6c20 7c20 4e6f 6e65 0d0a   : bool | None..
+00008580: 2020 2020 2020 2020 2020 2020 4966 2070              If p
+00008590: 726f 7669 6465 642c 206f 6e6c 7920 7072  rovided, only pr
+000085a0: 6f70 6572 7469 6573 2077 6974 6820 6068  operties with `h
+000085b0: 6173 5072 6f70 6572 7479 4c69 6d69 7473  asPropertyLimits
+000085c0: 6020 6d61 7463 6869 6e67 2074 6869 7320  ` matching this 
+000085d0: 7661 6c75 650d 0a20 2020 2020 2020 2020  value..         
+000085e0: 2020 2077 696c 6c20 6265 2079 6965 6c64     will be yield
+000085f0: 6564 2e0d 0a20 2020 2020 2020 2069 735f  ed...        is_
+00008600: 7265 6164 5f6f 6e6c 7920 3a20 626f 6f6c  read_only : bool
+00008610: 207c 204e 6f6e 650d 0a20 2020 2020 2020   | None..       
+00008620: 2020 2020 2049 6620 7072 6f76 6964 6564       If provided
+00008630: 2c20 6f6e 6c79 2070 726f 7065 7274 6965  , only propertie
+00008640: 7320 7769 7468 2060 6973 5072 6f70 6572  s with `isProper
+00008650: 7479 5265 6164 4f6e 6c79 6020 6d61 7463  tyReadOnly` matc
+00008660: 6869 6e67 2074 6869 7320 7661 6c75 650d  hing this value.
+00008670: 0a20 2020 2020 2020 2020 2020 2077 696c  .            wil
+00008680: 6c20 6265 2079 6965 6c64 6564 2e0d 0a20  l be yielded... 
+00008690: 2020 2020 2020 2069 735f 7365 7175 656e         is_sequen
+000086a0: 6365 6162 6c65 203a 2062 6f6f 6c20 7c20  ceable : bool | 
+000086b0: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+000086c0: 2020 4966 2070 726f 7669 6465 6420 6f6e    If provided on
+000086d0: 6c79 2070 726f 7065 7274 6965 7320 7769  ly properties wi
+000086e0: 7468 2060 6973 5072 6f70 6572 7479 5365  th `isPropertySe
+000086f0: 7175 656e 6365 6162 6c65 6020 6d61 7463  quenceable` matc
+00008700: 6869 6e67 2074 6869 730d 0a20 2020 2020  hing this..     
+00008710: 2020 2020 2020 2076 616c 7565 2077 696c         value wil
+00008720: 6c20 6265 2079 6965 6c64 6564 2e0d 0a20  l be yielded... 
+00008730: 2020 2020 2020 2061 735f 6f62 6a65 6374         as_object
+00008740: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00008750: 6c0d 0a20 2020 2020 2020 2020 2020 2049  l..            I
+00008760: 6620 6054 7275 6560 2c20 6044 6576 6963  f `True`, `Devic
+00008770: 6550 726f 7065 7274 7960 206f 626a 6563  eProperty` objec
+00008780: 7473 2077 696c 6c20 6265 2079 6965 6c64  ts will be yield
+00008790: 6564 2069 6e73 7465 6164 206f 660d 0a20  ed instead of.. 
+000087a0: 2020 2020 2020 2020 2020 2060 2864 6576             `(dev
+000087b0: 6963 655f 6c61 6265 6c2c 2070 726f 7065  ice_label, prope
+000087c0: 7274 795f 6e61 6d65 2960 2074 7570 6c65  rty_name)` tuple
+000087d0: 732e 2042 7920 6465 6661 756c 7420 5472  s. By default Tr
+000087e0: 7565 0d0a 0d0a 2020 2020 2020 2020 5969  ue....        Yi
+000087f0: 656c 6473 0d0a 2020 2020 2020 2020 2d2d  elds..        --
+00008800: 2d2d 2d2d 0d0a 2020 2020 2020 2020 4465  ----..        De
+00008810: 7669 6365 5072 6f70 6572 7479 207c 2074  viceProperty | t
+00008820: 7570 6c65 5b73 7472 2c20 7374 725d 0d0a  uple[str, str]..
+00008830: 2020 2020 2020 2020 2020 2020 6044 6576              `Dev
+00008840: 6963 6550 726f 7065 7274 7960 206f 626a  iceProperty` obj
+00008850: 6563 7473 2028 6966 2060 6173 5f6f 626a  ects (if `as_obj
+00008860: 6563 743d 3d54 7275 6560 2920 6f72 2032  ect==True`) or 2
+00008870: 2d74 7570 6c65 7320 6f66 2028 6465 7669  -tuples of (devi
+00008880: 6365 5f6e 616d 652c 0d0a 2020 2020 2020  ce_name,..      
+00008890: 2020 2020 2020 7072 6f70 6572 7479 5f6e        property_n
+000088a0: 616d 6529 0d0a 2020 2020 2020 2020 2222  ame)..        ""
+000088b0: 220d 0a20 2020 2020 2020 2069 6620 7072  "..        if pr
+000088c0: 6f70 6572 7479 5f6e 616d 655f 7061 7474  operty_name_patt
+000088d0: 6572 6e3a 0d0a 2020 2020 2020 2020 2020  ern:..          
+000088e0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000088f0: 7072 6f70 6572 7479 5f6e 616d 655f 7061  property_name_pa
+00008900: 7474 6572 6e2c 2073 7472 293a 0d0a 2020  ttern, str):..  
+00008910: 2020 2020 2020 2020 2020 2020 2020 7074                pt
+00008920: 726e 203d 2072 652e 636f 6d70 696c 6528  rn = re.compile(
+00008930: 7072 6f70 6572 7479 5f6e 616d 655f 7061  property_name_pa
+00008940: 7474 6572 6e2c 2072 652e 4947 4e4f 5245  ttern, re.IGNORE
+00008950: 4341 5345 290d 0a20 2020 2020 2020 2020  CASE)..         
+00008960: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00008970: 2020 2020 2020 2020 2020 7074 726e 203d            ptrn =
+00008980: 2070 726f 7065 7274 795f 6e61 6d65 5f70   property_name_p
+00008990: 6174 7465 726e 0d0a 2020 2020 2020 2020  attern..        
+000089a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000089b0: 2020 2070 7472 6e20 3d20 4e6f 6e65 0d0a     ptrn = None..
+000089c0: 0d0a 2020 2020 2020 2020 6966 2070 726f  ..        if pro
+000089d0: 7065 7274 795f 7479 7065 2069 7320 4e6f  perty_type is No
+000089e0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000089f0: 2070 726f 7065 7274 795f 7479 7065 7320   property_types 
+00008a00: 3d20 7365 7428 290d 0a20 2020 2020 2020  = set()..       
+00008a10: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00008a20: 2870 726f 7065 7274 795f 7479 7065 2c20  (property_type, 
+00008a30: 696e 7429 3a0d 0a20 2020 2020 2020 2020  int):..         
+00008a40: 2020 2070 726f 7065 7274 795f 7479 7065     property_type
+00008a50: 7320 3d20 7b70 726f 7065 7274 795f 7479  s = {property_ty
+00008a60: 7065 7d0d 0a20 2020 2020 2020 2065 6c73  pe}..        els
+00008a70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00008a80: 7072 6f70 6572 7479 5f74 7970 6573 203d  property_types =
+00008a90: 2073 6574 2870 726f 7065 7274 795f 7479   set(property_ty
+00008aa0: 7065 290d 0a0d 0a20 2020 2020 2020 2066  pe)....        f
+00008ab0: 6f72 2064 6576 2069 6e20 7365 6c66 2e69  or dev in self.i
+00008ac0: 7465 7244 6576 6963 6573 2864 6576 6963  terDevices(devic
+00008ad0: 655f 7479 7065 2c20 6465 7669 6365 5f6c  e_type, device_l
+00008ae0: 6162 656c 2c20 6173 5f6f 626a 6563 743d  abel, as_object=
+00008af0: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00008b00: 2020 2020 2066 6f72 2070 726f 7020 696e       for prop in
+00008b10: 2073 656c 662e 6765 7444 6576 6963 6550   self.getDeviceP
+00008b20: 726f 7065 7274 794e 616d 6573 2864 6576  ropertyNames(dev
+00008b30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00008b40: 2020 2020 6966 2070 7472 6e20 616e 6420      if ptrn and 
+00008b50: 6e6f 7420 7074 726e 2e73 6561 7263 6828  not ptrn.search(
+00008b60: 7072 6f70 293a 0d0a 2020 2020 2020 2020  prop):..        
+00008b70: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00008b80: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
+00008b90: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
+00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bb0: 7072 6f70 6572 7479 5f74 7970 6520 6973  property_type is
+00008bc0: 206e 6f74 204e 6f6e 650d 0a20 2020 2020   not None..     
+00008bd0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00008be0: 6e64 2073 7570 6572 2829 2e67 6574 5072  nd super().getPr
+00008bf0: 6f70 6572 7479 5479 7065 2864 6576 2c20  opertyType(dev, 
+00008c00: 7072 6f70 2920 6e6f 7420 696e 2070 726f  prop) not in pro
+00008c10: 7065 7274 795f 7479 7065 730d 0a20 2020  perty_types..   
+00008c20: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
+00008c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c40: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+00008c50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00008c60: 6620 280d 0a20 2020 2020 2020 2020 2020  f (..           
+00008c70: 2020 2020 2020 2020 2068 6173 5f6c 696d           has_lim
+00008c80: 6974 7320 6973 206e 6f74 204e 6f6e 650d  its is not None.
+00008c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008ca0: 2020 2020 2061 6e64 2073 656c 662e 6861       and self.ha
+00008cb0: 7350 726f 7065 7274 794c 696d 6974 7328  sPropertyLimits(
+00008cc0: 6465 762c 2070 726f 7029 2021 3d20 6861  dev, prop) != ha
+00008cd0: 735f 6c69 6d69 7473 0d0a 2020 2020 2020  s_limits..      
+00008ce0: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
+00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d00: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
+00008d10: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00008d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008d30: 2020 2020 2020 6973 5f72 6561 645f 6f6e        is_read_on
+00008d40: 6c79 2069 7320 6e6f 7420 4e6f 6e65 0d0a  ly is not None..
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d60: 2020 2020 616e 6420 7365 6c66 2e69 7350      and self.isP
+00008d70: 726f 7065 7274 7952 6561 644f 6e6c 7928  ropertyReadOnly(
+00008d80: 6465 762c 2070 726f 7029 2021 3d20 6973  dev, prop) != is
+00008d90: 5f72 6561 645f 6f6e 6c79 0d0a 2020 2020  _read_only..    
+00008da0: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dc0: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00008de0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00008df0: 2020 2020 2020 2020 6973 5f73 6571 7565          is_seque
+00008e00: 6e63 6561 626c 6520 6973 206e 6f74 204e  nceable is not N
+00008e10: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00008e20: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
+00008e30: 662e 6973 5072 6f70 6572 7479 5365 7175  f.isPropertySequ
+00008e40: 656e 6365 6162 6c65 2864 6576 2c20 7072  enceable(dev, pr
+00008e50: 6f70 2920 213d 2069 735f 7365 7175 656e  op) != is_sequen
+00008e60: 6365 6162 6c65 0d0a 2020 2020 2020 2020  ceable..        
+00008e70: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
+00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e90: 636f 6e74 696e 7565 0d0a 0d0a 2020 2020  continue....    
+00008ea0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00008eb0: 6420 4465 7669 6365 5072 6f70 6572 7479  d DeviceProperty
+00008ec0: 2864 6576 2c20 7072 6f70 2c20 7365 6c66  (dev, prop, self
+00008ed0: 2920 6966 2061 735f 6f62 6a65 6374 2065  ) if as_object e
+00008ee0: 6c73 6520 2864 6576 2c20 7072 6f70 290d  lse (dev, prop).
+00008ef0: 0a0d 0a20 2020 2064 6566 2067 6574 5072  ...    def getPr
+00008f00: 6f70 6572 7479 4f62 6a65 6374 280d 0a20  opertyObject(.. 
+00008f10: 2020 2020 2020 2073 656c 662c 2064 6576         self, dev
+00008f20: 6963 655f 6c61 6265 6c3a 2073 7472 2c20  ice_label: str, 
+00008f30: 7072 6f70 6572 7479 5f6e 616d 653a 2073  property_name: s
+00008f40: 7472 0d0a 2020 2020 2920 2d3e 2044 6576  tr..    ) -> Dev
+00008f50: 6963 6550 726f 7065 7274 793a 0d0a 2020  iceProperty:..  
+00008f60: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00008f70: 6120 4465 7669 6365 5072 6f70 6572 7479  a DeviceProperty
+00008f80: 206f 626a 6563 7420 626f 756e 6420 746f   object bound to
+00008f90: 2061 2064 6576 6963 652f 7072 6f70 6572   a device/proper
+00008fa0: 7479 206f 6e20 7468 6973 2063 6f72 652e  ty on this core.
+00008fb0: 0d0a 0d0a 2020 2020 2020 2020 3a73 7061  ....        :spa
+00008fc0: 726b 6c65 733a 202a 5468 6973 206d 6574  rkles: *This met
+00008fd0: 686f 6420 6973 206e 6577 2069 6e20 6043  hod is new in `C
+00008fe0: 4d4d 436f 7265 506c 7573 602e 2a0d 0a0d  MMCorePlus`.*...
+00008ff0: 0a20 2020 2020 2020 205b 6044 6576 6963  .        [`Devic
+00009000: 6550 726f 7065 7274 7960 5d5b 7079 6d6d  eProperty`][pymm
+00009010: 636f 7265 5f70 6c75 732e 4465 7669 6365  core_plus.Device
+00009020: 5072 6f70 6572 7479 5d20 6f62 6a65 6374  Property] object
+00009030: 7320 6172 6520 6120 636f 6e76 656e 6965  s are a convenie
+00009040: 6e74 206f 626a 6563 740d 0a20 2020 2020  nt object..     
+00009050: 2020 206f 7269 656e 7465 6420 7761 7920     oriented way 
+00009060: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
+00009070: 2061 2073 7065 6369 6669 6320 6465 7669   a specific devi
+00009080: 6365 2070 726f 7065 7274 6965 732e 2054  ce properties. T
+00009090: 6865 7920 616c 6c6f 7720 796f 7520 746f  hey allow you to
+000090a0: 0d0a 2020 2020 2020 2020 6361 6c6c 2061  ..        call a
+000090b0: 6e79 206d 6574 686f 6420 6f6e 2060 434d  ny method on `CM
+000090c0: 4d43 6f72 6560 2074 6861 7420 6e6f 726d  MCore` that norm
+000090d0: 616c 6c79 2072 6571 7569 7265 7320 6120  ally requires a 
+000090e0: 6064 6576 6963 654c 6162 656c 6020 616e  `deviceLabel` an
+000090f0: 640d 0a20 2020 2020 2020 2060 7072 6f70  d..        `prop
+00009100: 6572 7479 4e61 6d65 6020 6173 2074 6865  ertyName` as the
+00009110: 2066 6972 7374 2074 776f 2061 7267 756d   first two argum
+00009120: 656e 7473 2061 7320 616e 2061 7267 756d  ents as an argum
+00009130: 656e 742d 6672 6565 206d 6574 686f 6420  ent-free method 
+00009140: 6f6e 2074 6865 0d0a 2020 2020 2020 2020  on the..        
+00009150: 6044 6576 6963 6550 726f 7065 7274 7960  `DeviceProperty`
+00009160: 206f 626a 6563 742e 0d0a 0d0a 2020 2020   object.....    
+00009170: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+00009180: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00009190: 2d2d 0d0a 2020 2020 2020 2020 6465 7669  --..        devi
+000091a0: 6365 5f6c 6162 656c 203a 2073 7472 0d0a  ce_label : str..
+000091b0: 2020 2020 2020 2020 2020 2020 4465 7669              Devi
+000091c0: 6365 206c 6162 656c 2074 6f20 6765 7420  ce label to get 
+000091d0: 6120 7072 6f70 6572 7479 206f 626a 6563  a property objec
+000091e0: 7420 666f 722e 0d0a 2020 2020 2020 2020  t for...        
+000091f0: 7072 6f70 6572 7479 5f6e 616d 6520 3a20  property_name : 
+00009200: 7374 720d 0a20 2020 2020 2020 2020 2020  str..           
+00009210: 2050 726f 7065 7274 7920 6e61 6d65 2074   Property name t
+00009220: 6f20 6765 7420 6120 7072 6f70 6572 7479  o get a property
+00009230: 206f 626a 6563 7420 666f 722e 0d0a 0d0a   object for.....
+00009240: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+00009250: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00009260: 2d2d 0d0a 2020 2020 2020 2020 3e3e 3e20  --..        >>> 
+00009270: 636f 7265 203d 2043 4d4d 436f 7265 506c  core = CMMCorePl
+00009280: 7573 2829 0d0a 2020 2020 2020 2020 3e3e  us()..        >>
+00009290: 3e20 636f 7265 2e6c 6f61 6444 6576 6963  > core.loadDevic
+000092a0: 6528 2244 656d 6f43 616d 6572 6122 2c20  e("DemoCamera", 
+000092b0: 2244 656d 6f43 616d 6572 6122 2c20 2244  "DemoCamera", "D
+000092c0: 4361 6d22 290d 0a20 2020 2020 2020 203e  Cam")..        >
+000092d0: 3e3e 2063 6f72 652e 696e 6974 6961 6c69  >> core.initiali
+000092e0: 7a65 4465 7669 6365 2822 4465 6d6f 4361  zeDevice("DemoCa
+000092f0: 6d65 7261 2229 0d0a 2020 2020 2020 2020  mera")..        
+00009300: 3e3e 3e20 636f 7265 2e73 6574 4361 6d65  >>> core.setCame
+00009310: 7261 4465 7669 6365 2822 4465 6d6f 4361  raDevice("DemoCa
+00009320: 6d65 7261 2229 0d0a 2020 2020 2020 2020  mera")..        
+00009330: 3e3e 3e20 6578 706f 7375 7265 203d 2063  >>> exposure = c
+00009340: 6f72 652e 6765 7450 726f 7065 7274 794f  ore.getPropertyO
+00009350: 626a 6563 7428 2244 656d 6f43 616d 6572  bject("DemoCamer
+00009360: 6122 2c20 2245 7870 6f73 7572 6522 290d  a", "Exposure").
+00009370: 0a20 2020 2020 2020 203e 3e3e 2065 7870  .        >>> exp
+00009380: 6f73 7572 652e 7479 7065 2829 0d0a 2020  osure.type()..  
+00009390: 2020 2020 2020 3c50 726f 7065 7274 7954        <PropertyT
+000093a0: 7970 652e 466c 6f61 743a 2032 3e0d 0a20  ype.Float: 2>.. 
+000093b0: 2020 2020 2020 203e 3e3e 2065 7870 6f73         >>> expos
+000093c0: 7572 652e 7570 7065 724c 696d 6974 2829  ure.upperLimit()
+000093d0: 0d0a 2020 2020 2020 2020 3130 3030 302e  ..        10000.
+000093e0: 300d 0a0d 0a20 2020 2020 2020 2067 6574  0....        get
+000093f0: 2f73 6574 2070 726f 7065 7274 7920 7661  /set property va
+00009400: 6c75 6573 2065 6173 696c 793a 0d0a 0d0a  lues easily:....
+00009410: 2020 2020 2020 2020 3e3e 3e20 6578 706f          >>> expo
+00009420: 7375 7265 2e76 616c 7565 0d0a 2020 2020  sure.value..    
+00009430: 2020 2020 3130 2e30 0d0a 2020 2020 2020      10.0..      
+00009440: 2020 3e3e 3e20 6578 706f 7375 7265 2e76    >>> exposure.v
+00009450: 616c 7565 203d 2035 2e30 0d0a 2020 2020  alue = 5.0..    
+00009460: 2020 2020 3e3e 3e20 6578 706f 7375 7265      >>> exposure
+00009470: 2e76 616c 7565 0d0a 2020 2020 2020 2020  .value..        
+00009480: 352e 300d 0a20 2020 2020 2020 203e 3e3e  5.0..        >>>
+00009490: 2063 6f72 652e 6765 7445 7870 6f73 7572   core.getExposur
+000094a0: 6528 2920 2023 2063 6861 6e67 6573 2072  e()  # changes r
+000094b0: 6566 6c65 6374 6564 2069 6e20 636f 7265  eflected in core
+000094c0: 0d0a 2020 2020 2020 2020 352e 300d 0a20  ..        5.0.. 
+000094d0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000094e0: 2020 2020 7265 7475 726e 2044 6576 6963      return Devic
+000094f0: 6550 726f 7065 7274 7928 6465 7669 6365  eProperty(device
+00009500: 5f6c 6162 656c 2c20 7072 6f70 6572 7479  _label, property
+00009510: 5f6e 616d 652c 2073 656c 6629 0d0a 0d0a  _name, self)....
+00009520: 2020 2020 6465 6620 6765 7441 6461 7074      def getAdapt
+00009530: 6572 4f62 6a65 6374 2873 656c 662c 206c  erObject(self, l
+00009540: 6962 7261 7279 5f6e 616d 653a 2073 7472  ibrary_name: str
+00009550: 2920 2d3e 2044 6576 6963 6541 6461 7074  ) -> DeviceAdapt
+00009560: 6572 3a0d 0a20 2020 2020 2020 2022 2222  er:..        """
+00009570: 5265 7475 726e 2061 6e20 6041 6461 7074  Return an `Adapt
+00009580: 6572 6020 6f62 6a65 6374 2062 6f75 6e64  er` object bound
+00009590: 2074 6f20 6c69 6272 6172 795f 6e61 6d65   to library_name
+000095a0: 206f 6e20 7468 6973 2063 6f72 652e 0d0a   on this core...
+000095b0: 0d0a 2020 2020 2020 2020 3a73 7061 726b  ..        :spark
+000095c0: 6c65 733a 202a 5468 6973 206d 6574 686f  les: *This metho
+000095d0: 6420 6973 206e 6577 2069 6e20 6043 4d4d  d is new in `CMM
+000095e0: 436f 7265 506c 7573 602e 2a0d 0a0d 0a20  CorePlus`.*.... 
+000095f0: 2020 2020 2020 205b 6041 6461 7074 6572         [`Adapter
+00009600: 605d 5b70 796d 6d63 6f72 655f 706c 7573  `][pymmcore_plus
+00009610: 2e44 6576 6963 6541 6461 7074 6572 5d20  .DeviceAdapter] 
+00009620: 6f62 6a65 6374 7320 6172 6520 6120 636f  objects are a co
+00009630: 6e76 656e 6965 6e74 206f 626a 6563 740d  nvenient object.
+00009640: 0a20 2020 2020 2020 206f 7269 656e 7465  .        oriente
+00009650: 6420 7761 7920 746f 2069 6e74 6572 6163  d way to interac
+00009660: 7420 7769 7468 2064 6576 6963 6520 6164  t with device ad
+00009670: 6170 7465 7273 2e20 5468 6579 2061 6c6c  apters. They all
+00009680: 6f77 2079 6f75 2074 6f20 6361 6c6c 2061  ow you to call a
+00009690: 6e79 206d 6574 686f 640d 0a20 2020 2020  ny method..     
+000096a0: 2020 206f 6e20 6043 4d4d 436f 7265 6020     on `CMMCore` 
+000096b0: 7468 6174 206e 6f72 6d61 6c6c 7920 7265  that normally re
+000096c0: 7175 6972 6573 2061 2060 6c69 6272 6172  quires a `librar
+000096d0: 795f 6e61 6d65 6020 6173 2074 6865 2066  y_name` as the f
+000096e0: 6972 7374 2061 7267 756d 656e 7420 6173  irst argument as
+000096f0: 2061 6e0d 0a20 2020 2020 2020 2061 7267   an..        arg
+00009700: 756d 656e 742d 6672 6565 206d 6574 686f  ument-free metho
+00009710: 6420 6f6e 2074 6865 2060 4164 6170 7465  d on the `Adapte
+00009720: 7260 206f 626a 6563 742e 0d0a 2020 2020  r` object...    
+00009730: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00009740: 2072 6574 7572 6e20 4465 7669 6365 4164   return DeviceAd
+00009750: 6170 7465 7228 6c69 6272 6172 795f 6e61  apter(library_na
+00009760: 6d65 2c20 6d6d 636f 7265 3d73 656c 6629  me, mmcore=self)
+00009770: 0d0a 0d0a 2020 2020 6465 6620 6765 7444  ....    def getD
+00009780: 6576 6963 654f 626a 6563 7428 7365 6c66  eviceObject(self
+00009790: 2c20 6465 7669 6365 5f6c 6162 656c 3a20  , device_label: 
+000097a0: 7374 7229 202d 3e20 4465 7669 6365 3a0d  str) -> Device:.
+000097b0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+000097c0: 726e 2061 2060 4465 7669 6365 6020 6f62  rn a `Device` ob
+000097d0: 6a65 6374 2062 6f75 6e64 2074 6f20 6465  ject bound to de
+000097e0: 7669 6365 5f6c 6162 656c 206f 6e20 7468  vice_label on th
+000097f0: 6973 2063 6f72 652e 0d0a 0d0a 2020 2020  is core.....    
+00009800: 2020 2020 3a73 7061 726b 6c65 733a 202a      :sparkles: *
+00009810: 5468 6973 206d 6574 686f 6420 6973 206e  This method is n
+00009820: 6577 2069 6e20 6043 4d4d 436f 7265 506c  ew in `CMMCorePl
+00009830: 7573 602e 2a0d 0a0d 0a20 2020 2020 2020  us`.*....       
+00009840: 205b 6044 6576 6963 6560 5d5b 7079 6d6d   [`Device`][pymm
+00009850: 636f 7265 5f70 6c75 732e 4465 7669 6365  core_plus.Device
+00009860: 5d20 6f62 6a65 6374 7320 6172 6520 6120  ] objects are a 
+00009870: 636f 6e76 656e 6965 6e74 206f 626a 6563  convenient objec
+00009880: 7420 6f72 6965 6e74 6564 2077 6179 2074  t oriented way t
+00009890: 6f0d 0a20 2020 2020 2020 2069 6e74 6572  o..        inter
+000098a0: 6163 7420 7769 7468 2064 6576 6963 6573  act with devices
+000098b0: 2e20 5468 6579 2061 6c6c 6f77 2079 6f75  . They allow you
+000098c0: 2074 6f20 6361 6c6c 2061 6e79 206d 6574   to call any met
+000098d0: 686f 6420 6f6e 2060 434d 4d43 6f72 6560  hod on `CMMCore`
+000098e0: 2074 6861 740d 0a20 2020 2020 2020 206e   that..        n
+000098f0: 6f72 6d61 6c6c 7920 7265 7175 6972 6573  ormally requires
+00009900: 2061 2060 6465 7669 6365 4c61 6265 6c60   a `deviceLabel`
+00009910: 2061 7320 7468 6520 6669 7273 7420 6172   as the first ar
+00009920: 6775 6d65 6e74 2061 7320 616e 2061 7267  gument as an arg
+00009930: 756d 656e 742d 6672 6565 0d0a 2020 2020  ument-free..    
+00009940: 2020 2020 6d65 7468 6f64 206f 6e20 7468      method on th
+00009950: 6520 6044 6576 6963 6560 206f 626a 6563  e `Device` objec
+00009960: 742e 0d0a 0d0a 2020 2020 2020 2020 5061  t.....        Pa
+00009970: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+00009980: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+00009990: 2020 2020 2020 6465 7669 6365 5f6c 6162        device_lab
+000099a0: 656c 203a 2073 7472 0d0a 2020 2020 2020  el : str..      
+000099b0: 2020 2020 2020 4465 7669 6365 206c 6162        Device lab
+000099c0: 656c 2074 6f20 6765 7420 6120 6465 7669  el to get a devi
+000099d0: 6365 206f 626a 6563 7420 666f 722e 0d0a  ce object for...
+000099e0: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+000099f0: 6573 0d0a 2020 2020 2020 2020 2d2d 2d2d  es..        ----
+00009a00: 2d2d 2d2d 0d0a 2020 2020 2020 2020 3e3e  ----..        >>
+00009a10: 3e20 636f 7265 203d 2043 4d4d 436f 7265  > core = CMMCore
+00009a20: 506c 7573 2829 0d0a 2020 2020 2020 2020  Plus()..        
+00009a30: 3e3e 3e20 6361 6d20 3d20 636f 7265 2e67  >>> cam = core.g
+00009a40: 6574 4465 7669 6365 4f62 6a65 6374 2822  etDeviceObject("
+00009a50: 4465 6d6f 4361 6d65 7261 2229 0d0a 2020  DemoCamera")..  
+00009a60: 2020 2020 2020 3e3e 3e20 6361 6d2e 6973        >>> cam.is
+00009a70: 4c6f 6164 6564 2829 0d0a 2020 2020 2020  Loaded()..      
+00009a80: 2020 4661 6c73 650d 0a20 2020 2020 2020    False..       
+00009a90: 203e 3e3e 2063 616d 2e6c 6f61 6428 2244   >>> cam.load("D
+00009aa0: 656d 6f43 616d 6572 6122 2c20 2244 4361  emoCamera", "DCa
+00009ab0: 6d22 290d 0a20 2020 2020 2020 203e 3e3e  m")..        >>>
+00009ac0: 2063 616d 2e69 734c 6f61 6465 6428 290d   cam.isLoaded().
+00009ad0: 0a20 2020 2020 2020 2054 7275 650d 0a20  .        True.. 
+00009ae0: 2020 2020 2020 203e 3e3e 2063 616d 2e69         >>> cam.i
+00009af0: 6e69 7469 616c 697a 6528 290d 0a0d 0a20  nitialize().... 
+00009b00: 2020 2020 2020 2067 6574 2074 6865 2064         get the d
+00009b10: 6576 6963 6520 7363 6865 6d61 0d0a 0d0a  evice schema....
+00009b20: 2020 2020 2020 2020 3e3e 3e20 6361 6d2e          >>> cam.
+00009b30: 7363 6865 6d61 2829 0d0a 2020 2020 2020  schema()..      
+00009b40: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00009b50: 2027 7469 746c 6527 3a20 2744 4361 6d27   'title': 'DCam'
+00009b60: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+00009b70: 6465 7363 7269 7074 696f 6e27 3a20 2744  description': 'D
+00009b80: 656d 6f20 6361 6d65 7261 272c 0d0a 2020  emo camera',..  
+00009b90: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+00009ba0: 3a20 276f 626a 6563 7427 2c0d 0a20 2020  : 'object',..   
+00009bb0: 2020 2020 2020 2020 2027 7072 6f70 6572           'proper
+00009bc0: 7469 6573 273a 207b 0d0a 2020 2020 2020  ties': {..      
+00009bd0: 2020 2020 2020 2020 2020 2748 7562 4944            'HubID
+00009be0: 273a 207b 2774 7970 6527 3a20 2773 7472  ': {'type': 'str
+00009bf0: 696e 6727 2c20 2772 6561 644f 6e6c 7927  ing', 'readOnly'
+00009c00: 3a20 5472 7565 2c20 2764 6566 6175 6c74  : True, 'default
+00009c10: 273a 2027 277d 2c0d 0a20 2020 2020 2020  ': ''},..       
+00009c20: 2020 2020 2020 2020 2027 4d61 7869 6d75           'Maximu
+00009c30: 6d45 7870 6f73 7572 654d 7327 3a20 7b27  mExposureMs': {'
+00009c40: 7479 7065 273a 2027 6e75 6d62 6572 272c  type': 'number',
+00009c50: 2027 7072 6549 6e69 7427 3a20 5472 7565   'preInit': True
+00009c60: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
+00009c70: 2020 2020 2754 7261 6e73 706f 7365 436f      'TransposeCo
+00009c80: 7272 6563 7469 6f6e 273a 207b 2774 7970  rrection': {'typ
+00009c90: 6527 3a20 2762 6f6f 6c65 616e 277d 2c0d  e': 'boolean'},.
+00009ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009cb0: 2027 5472 616e 7370 6f73 654d 6972 726f   'TransposeMirro
+00009cc0: 7258 273a 207b 2774 7970 6527 3a20 2762  rX': {'type': 'b
+00009cd0: 6f6f 6c65 616e 277d 2c0d 0a20 2020 2020  oolean'},..     
+00009ce0: 2020 2020 2020 2020 2020 2027 5472 616e             'Tran
+00009cf0: 7370 6f73 654d 6972 726f 7259 273a 207b  sposeMirrorY': {
+00009d00: 2774 7970 6527 3a20 2762 6f6f 6c65 616e  'type': 'boolean
+00009d10: 277d 2c0d 0a20 2020 2020 2020 2020 2020  '},..           
+00009d20: 2020 2020 2027 5472 616e 7370 6f73 6558       'TransposeX
+00009d30: 5927 3a20 7b27 7479 7065 273a 2027 626f  Y': {'type': 'bo
+00009d40: 6f6c 6561 6e27 7d0d 0a20 2020 2020 2020  olean'}..       
+00009d50: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+00009d60: 7d0d 0a20 2020 2020 2020 2022 2222 0d0a  }..        """..
+00009d70: 2020 2020 2020 2020 7265 7475 726e 2044          return D
+00009d80: 6576 6963 6528 6465 7669 6365 5f6c 6162  evice(device_lab
+00009d90: 656c 2c20 6d6d 636f 7265 3d73 656c 6629  el, mmcore=self)
+00009da0: 0d0a 0d0a 2020 2020 6465 6620 6765 7443  ....    def getC
+00009db0: 6f6e 6669 6747 726f 7570 4f62 6a65 6374  onfigGroupObject
+00009dc0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
+00009dd0: 2067 726f 7570 5f6e 616d 653a 2073 7472   group_name: str
+00009de0: 2c20 616c 6c6f 775f 6d69 7373 696e 673a  , allow_missing:
+00009df0: 2062 6f6f 6c20 3d20 4661 6c73 650d 0a20   bool = False.. 
+00009e00: 2020 2029 202d 3e20 436f 6e66 6967 4772     ) -> ConfigGr
+00009e10: 6f75 703a 0d0a 2020 2020 2020 2020 2222  oup:..        ""
+00009e20: 2252 6574 7572 6e20 6120 6043 6f6e 6669  "Return a `Confi
+00009e30: 6747 726f 7570 6020 6f62 6a65 6374 2062  gGroup` object b
+00009e40: 6f75 6e64 2074 6f20 6772 6f75 705f 6e61  ound to group_na
+00009e50: 6d65 206f 6e20 7468 6973 2063 6f72 652e  me on this core.
+00009e60: 0d0a 0d0a 2020 2020 2020 2020 3a73 7061  ....        :spa
+00009e70: 726b 6c65 733a 202a 5468 6973 206d 6574  rkles: *This met
+00009e80: 686f 6420 6973 206e 6577 2069 6e20 6043  hod is new in `C
+00009e90: 4d4d 436f 7265 506c 7573 602e 2a0d 0a0d  MMCorePlus`.*...
+00009ea0: 0a20 2020 2020 2020 205b 6043 6f6e 6669  .        [`Confi
+00009eb0: 6747 726f 7570 605d 5b70 796d 6d63 6f72  gGroup`][pymmcor
+00009ec0: 655f 706c 7573 2e43 6f6e 6669 6747 726f  e_plus.ConfigGro
+00009ed0: 7570 5d20 6f62 6a65 6374 7320 6172 6520  up] objects are 
+00009ee0: 6120 636f 6e76 656e 6965 6e74 206f 626a  a convenient obj
+00009ef0: 6563 740d 0a20 2020 2020 2020 206f 7269  ect..        ori
+00009f00: 656e 7465 6420 7761 7920 746f 2069 6e74  ented way to int
+00009f10: 6572 6163 7420 7769 7468 2063 6f6e 6669  eract with confi
+00009f20: 6775 7261 7469 6f6e 2067 726f 7570 7320  guration groups 
+00009f30: 2869 2e65 2e20 6772 6f75 7073 206f 660d  (i.e. groups of.
+00009f40: 0a20 2020 2020 2020 205b 436f 6e66 6967  .        [Config
+00009f50: 7572 6174 696f 6e0d 0a20 2020 2020 2020  uration..       
+00009f60: 2050 7265 7365 7473 5d28 6874 7470 733a   Presets](https:
+00009f70: 2f2f 6d69 6372 6f2d 6d61 6e61 6765 722e  //micro-manager.
+00009f80: 6f72 672f 4d69 6372 6f2d 4d61 6e61 6765  org/Micro-Manage
+00009f90: 725f 436f 6e66 6967 7572 6174 696f 6e5f  r_Configuration_
+00009fa0: 4775 6964 6523 636f 6e66 6967 7572 6174  Guide#configurat
+00009fb0: 696f 6e2d 7072 6573 6574 7329 0d0a 2020  ion-presets)..  
+00009fc0: 2020 2020 2020 696e 204d 6963 726f 2d4d        in Micro-M
+00009fd0: 616e 6167 6572 292e 2054 6865 7920 616c  anager). They al
+00009fe0: 6c6f 7720 796f 7520 746f 2063 616c 6c20  low you to call 
+00009ff0: 616e 7920 6d65 7468 6f64 206f 6e20 6043  any method on `C
+0000a000: 4d4d 436f 7265 6020 7468 6174 206e 6f72  MMCore` that nor
+0000a010: 6d61 6c6c 790d 0a20 2020 2020 2020 2072  mally..        r
+0000a020: 6571 7569 7265 7320 6120 6067 726f 7570  equires a `group
+0000a030: 4e61 6d65 6020 6173 2074 6865 2066 6972  Name` as the fir
+0000a040: 7374 2061 7267 756d 656e 7420 6173 2061  st argument as a
+0000a050: 6e20 6172 6775 6d65 6e74 2d66 7265 6520  n argument-free 
+0000a060: 6d65 7468 6f64 206f 6e20 7468 650d 0a20  method on the.. 
+0000a070: 2020 2020 2020 2060 436f 6e66 6967 4772         `ConfigGr
+0000a080: 6f75 7060 206f 626a 6563 742e 0d0a 0d0a  oup` object.....
+0000a090: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000a0a0: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+0000a0b0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0000a0c0: 6772 6f75 705f 6e61 6d65 203a 2073 7472  group_name : str
+0000a0d0: 0d0a 2020 2020 2020 2020 2020 2020 436f  ..            Co
+0000a0e0: 6e66 6967 7572 6174 696f 6e20 6772 6f75  nfiguration grou
+0000a0f0: 7020 6e61 6d65 2074 6f20 6765 7420 6120  p name to get a 
+0000a100: 636f 6e66 6967 2067 726f 7570 206f 626a  config group obj
+0000a110: 6563 7420 666f 722e 0d0a 2020 2020 2020  ect for...      
+0000a120: 2020 616c 6c6f 775f 6d69 7373 696e 6720    allow_missing 
+0000a130: 3a20 626f 6f6c 0d0a 2020 2020 2020 2020  : bool..        
+0000a140: 2020 2020 4966 2060 4661 6c73 6560 2061      If `False` a
+0000a150: 6e64 2074 6865 2060 436f 6e66 6967 4772  nd the `ConfigGr
+0000a160: 6f75 7060 2064 6f65 7320 6e6f 7420 6578  oup` does not ex
+0000a170: 6973 742c 2061 2060 4b65 7945 7272 6f72  ist, a `KeyError
+0000a180: 6020 7769 6c6c 2062 650d 0a20 2020 2020  ` will be..     
+0000a190: 2020 2020 2020 2072 6169 7365 642e 2042         raised. B
+0000a1a0: 7920 6465 6661 756c 7420 4661 6c73 652e  y default False.
+0000a1b0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 5265  ......        Re
+0000a1c0: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+0000a1d0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0000a1e0: 436f 6e66 6967 4772 6f75 700d 0a20 2020  ConfigGroup..   
+0000a1f0: 2020 2020 2020 2020 205b 6043 6f6e 6669           [`Confi
+0000a200: 6747 726f 7570 605d 5b70 796d 6d63 6f72  gGroup`][pymmcor
+0000a210: 655f 706c 7573 2e43 6f6e 6669 6747 726f  e_plus.ConfigGro
+0000a220: 7570 5d20 6f62 6a65 6374 2062 6f75 6e64  up] object bound
+0000a230: 2074 6f20 6067 726f 7570 5f6e 616d 6560   to `group_name`
+0000a240: 0d0a 2020 2020 2020 2020 2020 2020 6f6e  ..            on
+0000a250: 2074 6869 7320 636f 7265 2e0d 0a20 2020   this core...   
+0000a260: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000a270: 2020 6772 6f75 7020 3d20 436f 6e66 6967    group = Config
+0000a280: 4772 6f75 7028 6772 6f75 705f 6e61 6d65  Group(group_name
+0000a290: 2c20 6d6d 636f 7265 3d73 656c 6629 0d0a  , mmcore=self)..
+0000a2a0: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
+0000a2b0: 6c6c 6f77 5f6d 6973 7369 6e67 2061 6e64  llow_missing and
+0000a2c0: 206e 6f74 2067 726f 7570 2e65 7869 7374   not group.exist
+0000a2d0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+0000a2e0: 2020 7261 6973 6520 4b65 7945 7272 6f72    raise KeyError
+0000a2f0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0000a300: 2020 2066 2243 6f6e 6669 6775 7261 7469     f"Configurati
+0000a310: 6f6e 2067 726f 7570 207b 6772 6f75 705f  on group {group_
+0000a320: 6e61 6d65 2172 7d20 646f 6573 206e 6f74  name!r} does not
+0000a330: 2065 7869 7374 2e20 220d 0a20 2020 2020   exist. "..     
+0000a340: 2020 2020 2020 2020 2020 2022 5573 6520             "Use 
+0000a350: 6061 6c6c 6f77 5f6d 6973 7369 6e67 3d54  `allow_missing=T
+0000a360: 7275 6560 2074 6f20 6372 6561 7465 2063  rue` to create c
+0000a370: 7265 6174 6520 6e6f 6e2d 6578 6973 7465  reate non-existe
+0000a380: 6e74 2063 6f6e 6669 6720 6772 6f75 7073  nt config groups
+0000a390: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
+0000a3a0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0000a3b0: 6e20 6772 6f75 700d 0a0d 0a20 2020 2064  n group....    d
+0000a3c0: 6566 2069 7465 7243 6f6e 6669 6747 726f  ef iterConfigGro
+0000a3d0: 7570 7328 7365 6c66 2920 2d3e 2049 7465  ups(self) -> Ite
+0000a3e0: 7261 746f 725b 436f 6e66 6967 4772 6f75  rator[ConfigGrou
+0000a3f0: 705d 3a0d 0a20 2020 2020 2020 2022 2222  p]:..        """
+0000a400: 4974 6572 6174 6520 6043 6f6e 6669 6747  Iterate `ConfigG
+0000a410: 726f 7570 6020 6f62 6a65 6374 7320 666f  roup` objects fo
+0000a420: 7220 616c 6c20 636f 6e66 6967 732e 0d0a  r all configs...
+0000a430: 0d0a 2020 2020 2020 2020 3a73 7061 726b  ..        :spark
+0000a440: 6c65 733a 202a 5468 6973 206d 6574 686f  les: *This metho
+0000a450: 6420 6973 206e 6577 2069 6e20 6043 4d4d  d is new in `CMM
+0000a460: 436f 7265 506c 7573 602e 2a0d 0a0d 0a20  CorePlus`.*.... 
+0000a470: 2020 2020 2020 2059 6965 6c64 730d 0a20         Yields.. 
+0000a480: 2020 2020 2020 202d 2d2d 2d2d 2d0d 0a20         ------.. 
+0000a490: 2020 2020 2020 2043 6f6e 6669 6747 726f         ConfigGro
+0000a4a0: 7570 0d0a 2020 2020 2020 2020 2020 2020  up..            
+0000a4b0: 6043 6f6e 6669 6747 726f 7570 6020 6f62  `ConfigGroup` ob
+0000a4c0: 6a65 6374 730d 0a20 2020 2020 2020 2022  jects..        "
+0000a4d0: 2222 0d0a 2020 2020 2020 2020 666f 7220  ""..        for 
+0000a4e0: 6772 6f75 7020 696e 2073 656c 662e 6765  group in self.ge
+0000a4f0: 7441 7661 696c 6162 6c65 436f 6e66 6967  tAvailableConfig
+0000a500: 4772 6f75 7073 2829 3a0d 0a20 2020 2020  Groups():..     
+0000a510: 2020 2020 2020 2079 6965 6c64 2043 6f6e         yield Con
+0000a520: 6669 6747 726f 7570 2867 726f 7570 2c20  figGroup(group, 
+0000a530: 6d6d 636f 7265 3d73 656c 6629 0d0a 0d0a  mmcore=self)....
+0000a540: 2020 2020 6465 6620 6765 7444 6576 6963      def getDevic
+0000a550: 6553 6368 656d 6128 7365 6c66 2c20 6465  eSchema(self, de
+0000a560: 7669 6365 5f6c 6162 656c 3a20 7374 7229  vice_label: str)
+0000a570: 202d 3e20 4465 7669 6365 5363 6865 6d61   -> DeviceSchema
+0000a580: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+0000a590: 7475 726e 204a 534f 4e2d 7363 6865 6d61  turn JSON-schema
+0000a5a0: 2064 6573 6372 6962 696e 6720 6465 7669   describing devi
+0000a5b0: 6365 2060 6465 7669 6365 5f6c 6162 656c  ce `device_label
+0000a5c0: 6020 616e 6420 6974 7320 7072 6f70 6572  ` and its proper
+0000a5d0: 7469 6573 2e0d 0a0d 0a20 2020 2020 2020  ties.....       
+0000a5e0: 203a 7370 6172 6b6c 6573 3a20 2a54 6869   :sparkles: *Thi
+0000a5f0: 7320 6d65 7468 6f64 2069 7320 6e65 7720  s method is new 
+0000a600: 696e 2060 434d 4d43 6f72 6550 6c75 7360  in `CMMCorePlus`
+0000a610: 2e20 4974 2070 726f 7669 6465 7320 6120  . It provides a 
+0000a620: 636f 6e76 656e 6965 6e74 2077 6179 2074  convenient way t
+0000a630: 6f0d 0a20 2020 2020 2020 2067 6574 2061  o..        get a
+0000a640: 6c6c 206f 6620 7468 6520 696e 666f 726d  ll of the inform
+0000a650: 6174 696f 6e20 6162 6f75 7420 6120 6465  ation about a de
+0000a660: 7669 6365 2069 6e20 6120 7369 6e67 6c65  vice in a single
+0000a670: 2063 616c 6c2e 2a0d 0a0d 0a20 2020 2020   call.*....     
+0000a680: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+0000a690: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+0000a6a0: 2020 2020 2044 6576 6963 6553 6368 656d       DeviceSchem
+0000a6b0: 610d 0a20 2020 2020 2020 2020 2020 204a  a..            J
+0000a6c0: 534f 4e2d 7363 6865 6d61 2064 6573 6372  SON-schema descr
+0000a6d0: 6962 696e 6720 6465 7669 6365 2060 6465  ibing device `de
+0000a6e0: 7669 6365 5f6c 6162 656c 6020 616e 6420  vice_label` and 
+0000a6f0: 6974 7320 7072 6f70 6572 7469 6573 2e0d  its properties..
+0000a700: 0a0d 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+0000a710: 6c65 730d 0a20 2020 2020 2020 202d 2d2d  les..        ---
+0000a720: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 203e  -----..        >
+0000a730: 3e3e 2063 6f72 6520 3d20 434d 4d43 6f72  >> core = CMMCor
+0000a740: 6550 6c75 7328 290d 0a20 2020 2020 2020  ePlus()..       
+0000a750: 203e 3e3e 2063 6f72 652e 6c6f 6164 4465   >>> core.loadDe
+0000a760: 7669 6365 2822 4465 6d6f 4361 6d65 7261  vice("DemoCamera
+0000a770: 222c 2022 4465 6d6f 4361 6d65 7261 222c  ", "DemoCamera",
+0000a780: 2022 4443 616d 2229 0d0a 2020 2020 2020   "DCam")..      
+0000a790: 2020 3e3e 3e20 636f 7265 2e67 6574 4465    >>> core.getDe
+0000a7a0: 7669 6365 5363 6865 6d61 2822 4465 6d6f  viceSchema("Demo
+0000a7b0: 4361 6d65 7261 2229 0d0a 2020 2020 2020  Camera")..      
+0000a7c0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+0000a7d0: 2027 7469 746c 6527 3a20 2744 4361 6d27   'title': 'DCam'
+0000a7e0: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+0000a7f0: 6465 7363 7269 7074 696f 6e27 3a20 2744  description': 'D
+0000a800: 656d 6f20 6361 6d65 7261 272c 0d0a 2020  emo camera',..  
+0000a810: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+0000a820: 3a20 276f 626a 6563 7427 2c0d 0a20 2020  : 'object',..   
+0000a830: 2020 2020 2020 2020 2027 7072 6f70 6572           'proper
+0000a840: 7469 6573 273a 207b 0d0a 2020 2020 2020  ties': {..      
+0000a850: 2020 2020 2020 2020 2020 2748 7562 4944            'HubID
+0000a860: 273a 207b 2774 7970 6527 3a20 2773 7472  ': {'type': 'str
+0000a870: 696e 6727 2c20 2772 6561 644f 6e6c 7927  ing', 'readOnly'
+0000a880: 3a20 5472 7565 2c20 2764 6566 6175 6c74  : True, 'default
+0000a890: 273a 2027 277d 2c0d 0a20 2020 2020 2020  ': ''},..       
+0000a8a0: 2020 2020 2020 2020 2027 4d61 7869 6d75           'Maximu
+0000a8b0: 6d45 7870 6f73 7572 654d 7327 3a20 7b27  mExposureMs': {'
+0000a8c0: 7479 7065 273a 2027 6e75 6d62 6572 272c  type': 'number',
+0000a8d0: 2027 7072 6549 6e69 7427 3a20 5472 7565   'preInit': True
+0000a8e0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
+0000a8f0: 2020 2020 2754 7261 6e73 706f 7365 436f      'TransposeCo
+0000a900: 7272 6563 7469 6f6e 273a 207b 2774 7970  rrection': {'typ
+0000a910: 6527 3a20 2762 6f6f 6c65 616e 277d 2c0d  e': 'boolean'},.
+0000a920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a930: 2027 5472 616e 7370 6f73 654d 6972 726f   'TransposeMirro
+0000a940: 7258 273a 207b 2774 7970 6527 3a20 2762  rX': {'type': 'b
+0000a950: 6f6f 6c65 616e 277d 2c0d 0a20 2020 2020  oolean'},..     
+0000a960: 2020 2020 2020 2020 2020 2027 5472 616e             'Tran
+0000a970: 7370 6f73 654d 6972 726f 7259 273a 207b  sposeMirrorY': {
+0000a980: 2774 7970 6527 3a20 2762 6f6f 6c65 616e  'type': 'boolean
+0000a990: 277d 2c0d 0a20 2020 2020 2020 2020 2020  '},..           
+0000a9a0: 2020 2020 2027 5472 616e 7370 6f73 6558       'TransposeX
+0000a9b0: 5927 3a20 7b27 7479 7065 273a 2027 626f  Y': {'type': 'bo
+0000a9c0: 6f6c 6561 6e27 7d0d 0a20 2020 2020 2020  olean'}..       
+0000a9d0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+0000a9e0: 7d0d 0a20 2020 2020 2020 2022 2222 0d0a  }..        """..
+0000a9f0: 2020 2020 2020 2020 643a 2044 6576 6963          d: Devic
+0000aa00: 6553 6368 656d 6120 3d20 7b0d 0a20 2020  eSchema = {..   
+0000aa10: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
+0000aa20: 3a20 7365 6c66 2e67 6574 4465 7669 6365  : self.getDevice
+0000aa30: 4e61 6d65 2864 6576 6963 655f 6c61 6265  Name(device_labe
+0000aa40: 6c29 2c0d 0a20 2020 2020 2020 2020 2020  l),..           
+0000aa50: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+0000aa60: 7365 6c66 2e67 6574 4465 7669 6365 4465  self.getDeviceDe
+0000aa70: 7363 7269 7074 696f 6e28 6465 7669 6365  scription(device
+0000aa80: 5f6c 6162 656c 292c 0d0a 2020 2020 2020  _label),..      
+0000aa90: 2020 2020 2020 2274 7970 6522 3a20 226f        "type": "o
+0000aaa0: 626a 6563 7422 2c0d 0a20 2020 2020 2020  bject",..       
+0000aab0: 2020 2020 2022 7072 6f70 6572 7469 6573       "properties
+0000aac0: 223a 207b 7d2c 0d0a 2020 2020 2020 2020  ": {},..        
+0000aad0: 7d0d 0a20 2020 2020 2020 2066 6f72 2070  }..        for p
+0000aae0: 726f 7020 696e 2073 656c 662e 6974 6572  rop in self.iter
+0000aaf0: 5072 6f70 6572 7469 6573 2864 6576 6963  Properties(devic
+0000ab00: 655f 6c61 6265 6c3d 6465 7669 6365 5f6c  e_label=device_l
+0000ab10: 6162 656c 2c20 6173 5f6f 626a 6563 743d  abel, as_object=
+0000ab20: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
+0000ab30: 2020 2020 703a 2050 726f 7065 7274 7953      p: PropertyS
+0000ab40: 6368 656d 610d 0a20 2020 2020 2020 2020  chema..         
+0000ab50: 2020 2064 5b22 7072 6f70 6572 7469 6573     d["properties
+0000ab60: 225d 5b70 726f 702e 6e61 6d65 5d20 3d20  "][prop.name] = 
+0000ab70: 7020 3d20 7b7d 0d0a 2020 2020 2020 2020  p = {}..        
+0000ab80: 2020 2020 6966 2070 726f 702e 7479 7065      if prop.type
+0000ab90: 2829 2e74 6f5f 6a73 6f6e 2829 2021 3d20  ().to_json() != 
+0000aba0: 226e 756c 6c22 3a0d 0a20 2020 2020 2020  "null":..       
+0000abb0: 2020 2020 2020 2020 2070 5b22 7479 7065           p["type
+0000abc0: 225d 203d 2070 726f 702e 7479 7065 2829  "] = prop.type()
+0000abd0: 2e74 6f5f 6a73 6f6e 2829 0d0a 2020 2020  .to_json()..    
+0000abe0: 2020 2020 2020 2020 6966 2070 726f 702e          if prop.
+0000abf0: 6861 734c 696d 6974 7328 293a 0d0a 2020  hasLimits():..  
+0000ac00: 2020 2020 2020 2020 2020 2020 2020 705b                p[
+0000ac10: 226d 696e 696d 756d 225d 203d 2070 726f  "minimum"] = pro
+0000ac20: 702e 6c6f 7765 724c 696d 6974 2829 0d0a  p.lowerLimit()..
+0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac40: 705b 226d 6178 696d 756d 225d 203d 2070  p["maximum"] = p
+0000ac50: 726f 702e 7570 7065 724c 696d 6974 2829  rop.upperLimit()
+0000ac60: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000ac70: 2061 6c6c 6f77 6564 203a 3d20 7072 6f70   allowed := prop
+0000ac80: 2e61 6c6c 6f77 6564 5661 6c75 6573 2829  .allowedValues()
+0000ac90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000aca0: 2020 2069 6620 7365 7428 616c 6c6f 7765     if set(allowe
+0000acb0: 6429 203d 3d20 7b22 3022 2c20 2231 227d  d) == {"0", "1"}
+0000acc0: 2061 6e64 2070 726f 702e 7479 7065 2829   and prop.type()
+0000acd0: 203d 3d20 5072 6f70 6572 7479 5479 7065   == PropertyType
+0000ace0: 2e49 6e74 6567 6572 3a0d 0a20 2020 2020  .Integer:..     
+0000acf0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000ad00: 5b22 7479 7065 225d 203d 2022 626f 6f6c  ["type"] = "bool
+0000ad10: 6561 6e22 0d0a 2020 2020 2020 2020 2020  ean"..          
+0000ad20: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad40: 2063 6c73 203d 2070 726f 702e 7479 7065   cls = prop.type
+0000ad50: 2829 2e74 6f5f 7079 7468 6f6e 2829 0d0a  ().to_python()..
+0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad70: 2020 2020 705b 2265 6e75 6d22 5d20 3d20      p["enum"] = 
+0000ad80: 5b63 6c73 2869 2920 6966 2063 6c73 2065  [cls(i) if cls e
+0000ad90: 6c73 6520 6920 666f 7220 6920 696e 2061  lse i for i in a
+0000ada0: 6c6c 6f77 6564 5d0d 0a20 2020 2020 2020  llowed]..       
+0000adb0: 2020 2020 2069 6620 7072 6f70 2e69 7352       if prop.isR
+0000adc0: 6561 644f 6e6c 7928 293a 0d0a 2020 2020  eadOnly():..    
+0000add0: 2020 2020 2020 2020 2020 2020 705b 2272              p["r
+0000ade0: 6561 644f 6e6c 7922 5d20 3d20 5472 7565  eadOnly"] = True
+0000adf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ae00: 2020 705b 2264 6566 6175 6c74 225d 203d    p["default"] =
+0000ae10: 2070 726f 702e 7661 6c75 650d 0a20 2020   prop.value..   
+0000ae20: 2020 2020 2020 2020 2069 6620 7072 6f70           if prop
+0000ae30: 2e69 7353 6571 7565 6e63 6561 626c 6528  .isSequenceable(
+0000ae40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000ae50: 2020 2020 705b 2273 6571 7565 6e63 6561      p["sequencea
+0000ae60: 626c 6522 5d20 3d20 5472 7565 0d0a 2020  ble"] = True..  
+0000ae70: 2020 2020 2020 2020 2020 2020 2020 705b                p[
+0000ae80: 2273 6571 7565 6e63 654d 6178 4c65 6e67  "sequenceMaxLeng
+0000ae90: 7468 225d 203d 2070 726f 702e 7365 7175  th"] = prop.sequ
+0000aea0: 656e 6365 4d61 784c 656e 6774 6828 290d  enceMaxLength().
+0000aeb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000aec0: 7072 6f70 2e69 7350 7265 496e 6974 2829  prop.isPreInit()
+0000aed0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000aee0: 2020 2070 5b22 7072 6549 6e69 7422 5d20     p["preInit"] 
+0000aef0: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+0000af00: 7265 7475 726e 2064 0d0a 0d0a 2020 2020  return d....    
+0000af10: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+0000af20: 6566 206f 626a 6563 7469 7665 5f64 6576  ef objective_dev
+0000af30: 6963 655f 7061 7474 6572 6e28 7365 6c66  ice_pattern(self
+0000af40: 2920 2d3e 2050 6174 7465 726e 3a0d 0a20  ) -> Pattern:.. 
+0000af50: 2020 2020 2020 2022 2222 5061 7474 6572         """Patter
+0000af60: 6e20 7573 6564 2074 6f20 6775 6573 7320  n used to guess 
+0000af70: 6f62 6a65 6374 6976 6520 6465 7669 6365  objective device
+0000af80: 206c 6162 656c 732e 0d0a 0d0a 2020 2020   labels.....    
+0000af90: 2020 2020 3a73 7061 726b 6c65 733a 202a      :sparkles: *
+0000afa0: 5468 6973 2070 726f 7065 7274 7920 6973  This property is
+0000afb0: 206e 6577 2069 6e20 6043 4d4d 436f 7265   new in `CMMCore
+0000afc0: 506c 7573 602e 0d0a 0d0a 2020 2020 2020  Plus`.....      
+0000afd0: 2020 4974 2069 7320 7468 6520 7265 6765    It is the rege
+0000afe0: 7820 7573 6564 2062 790d 0a20 2020 2020  x used by..     
+0000aff0: 2020 205b 6067 7565 7373 4f62 6a65 6374     [`guessObject
+0000b000: 6976 6544 6576 6963 6573 605d 5b70 796d  iveDevices`][pym
+0000b010: 6d63 6f72 655f 706c 7573 2e43 4d4d 436f  mcore_plus.CMMCo
+0000b020: 7265 506c 7573 2e67 7565 7373 4f62 6a65  rePlus.guessObje
+0000b030: 6374 6976 6544 6576 6963 6573 5d20 746f  ctiveDevices] to
+0000b040: 0d0a 2020 2020 2020 2020 6669 6e64 2061  ..        find a
+0000b050: 6e79 2064 6576 6963 6573 2074 6861 7420  ny devices that 
+0000b060: 6172 6520 6c69 6b65 6c79 2074 6f20 6265  are likely to be
+0000b070: 206f 626a 6563 7469 7665 2064 6576 6963   objective devic
+0000b080: 6573 2e0d 0a0d 0a20 2020 2020 2020 2042  es.....        B
+0000b090: 7920 6465 6661 756c 743a 0d0a 0d0a 2020  y default:....  
+0000b0a0: 2020 2020 2020 2020 2020 7265 2e63 6f6d            re.com
+0000b0b0: 7069 6c65 2822 282e 2b29 3f28 6e6f 7365  pile("(.+)?(nose
+0000b0c0: 7069 6563 657c 6f62 6a28 6563 7469 7665  piece|obj(ective
+0000b0d0: 293f 2928 7475 7272 6574 293f 733f 222c  )?)(turret)?s?",
+0000b0e0: 2072 652e 4947 4e4f 5245 4341 5345 290d   re.IGNORECASE).
+0000b0f0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000b100: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000b110: 662e 5f6f 626a 6563 7469 7665 5f72 6567  f._objective_reg
+0000b120: 6578 0d0a 0d0a 2020 2020 406f 626a 6563  ex....    @objec
+0000b130: 7469 7665 5f64 6576 6963 655f 7061 7474  tive_device_patt
+0000b140: 6572 6e2e 7365 7474 6572 0d0a 2020 2020  ern.setter..    
+0000b150: 6465 6620 6f62 6a65 6374 6976 655f 6465  def objective_de
+0000b160: 7669 6365 5f70 6174 7465 726e 2873 656c  vice_pattern(sel
+0000b170: 662c 2076 616c 7565 3a20 5061 7474 6572  f, value: Patter
+0000b180: 6e20 7c20 7374 7229 202d 3e20 4e6f 6e65  n | str) -> None
+0000b190: 3a0d 0a20 2020 2020 2020 2069 6620 6973  :..        if is
+0000b1a0: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
+0000b1b0: 7374 7229 3a0d 0a20 2020 2020 2020 2020  str):..         
+0000b1c0: 2020 2076 616c 7565 203d 2072 652e 636f     value = re.co
+0000b1d0: 6d70 696c 6528 7661 6c75 652c 2072 652e  mpile(value, re.
+0000b1e0: 4947 4e4f 5245 4341 5345 290d 0a20 2020  IGNORECASE)..   
+0000b1f0: 2020 2020 2065 6c69 6620 6e6f 7420 6973       elif not is
+0000b200: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
+0000b210: 5061 7474 6572 6e29 3a0d 0a20 2020 2020  Pattern):..     
+0000b220: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0000b230: 6545 7272 6f72 280d 0a20 2020 2020 2020  eError(..       
+0000b240: 2020 2020 2020 2020 2022 4f62 6a65 6374           "Object
+0000b250: 6976 6520 5061 7474 6572 6e20 6d75 7374  ive Pattern must
+0000b260: 2062 6520 6120 7374 7269 6e67 206f 7220   be a string or 
+0000b270: 636f 6d70 696c 6564 2072 6567 6578 220d  compiled regex".
+0000b280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b290: 2066 2220 6275 7420 6973 2074 7970 6520   f" but is type 
+0000b2a0: 7b74 7970 6528 7661 6c75 6529 7d22 0d0a  {type(value)}"..
+0000b2b0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0000b2c0: 2020 2020 2020 2073 656c 662e 5f6f 626a         self._obj
+0000b2d0: 6563 7469 7665 5f72 6567 6578 203d 2076  ective_regex = v
+0000b2e0: 616c 7565 0d0a 0d0a 2020 2020 4070 726f  alue....    @pro
+0000b2f0: 7065 7274 790d 0a20 2020 2064 6566 2063  perty..    def c
+0000b300: 6861 6e6e 656c 4772 6f75 705f 7061 7474  hannelGroup_patt
+0000b310: 6572 6e28 7365 6c66 2920 2d3e 2050 6174  ern(self) -> Pat
+0000b320: 7465 726e 3a0d 0a20 2020 2020 2020 2022  tern:..        "
+0000b330: 2222 5468 6520 7265 6765 7820 7061 7474  ""The regex patt
+0000b340: 6572 6e20 7573 6564 2074 6f20 6964 656e  ern used to iden
+0000b350: 7469 6679 2063 6861 6e6e 656c 2067 726f  tify channel gro
+0000b360: 7570 732e 0d0a 0d0a 2020 2020 2020 2020  ups.....        
+0000b370: 3a73 7061 726b 6c65 733a 202a 5468 6973  :sparkles: *This
+0000b380: 2070 726f 7065 7274 7920 6973 206e 6577   property is new
+0000b390: 2069 6e20 6043 4d4d 436f 7265 506c 7573   in `CMMCorePlus
+0000b3a0: 602e 0d0a 0d0a 2020 2020 2020 2020 4974  `.....        It
+0000b3b0: 2069 7320 7468 6520 7265 6765 7820 7573   is the regex us
+0000b3c0: 6564 2062 790d 0a20 2020 2020 2020 205b  ed by..        [
+0000b3d0: 6067 6574 4f72 4775 6573 7343 6861 6e6e  `getOrGuessChann
+0000b3e0: 656c 4772 6f75 7060 5d5b 7079 6d6d 636f  elGroup`][pymmco
+0000b3f0: 7265 5f70 6c75 732e 434d 4d43 6f72 6550  re_plus.CMMCoreP
+0000b400: 6c75 732e 6765 744f 7247 7565 7373 4368  lus.getOrGuessCh
+0000b410: 616e 6e65 6c47 726f 7570 5d20 746f 0d0a  annelGroup] to..
+0000b420: 2020 2020 2020 2020 6669 6e64 2061 2063          find a c
+0000b430: 6f6e 6669 6720 6772 6f75 7020 6c69 6b65  onfig group like
+0000b440: 6c79 2074 6f20 6265 2061 2063 6861 6e6e  ly to be a chann
+0000b450: 656c 2067 726f 7570 2069 6e20 6067 6574  el group in `get
+0000b460: 4176 6169 6c61 626c 6543 6f6e 6669 6747  AvailableConfigG
+0000b470: 726f 7570 7360 0d0a 2020 2020 2020 2020  roups`..        
+0000b480: 6966 2060 6765 7443 6861 6e6e 656c 4772  if `getChannelGr
+0000b490: 6f75 7060 2072 6574 7572 6e73 2060 4e6f  oup` returns `No
+0000b4a0: 6e65 602e 0d0a 0d0a 2020 2020 2020 2020  ne`.....        
+0000b4b0: 4279 2064 6566 6175 6c74 3a0d 0a0d 0a20  By default:.... 
+0000b4c0: 2020 2020 2020 2020 2020 2072 652e 636f             re.co
+0000b4d0: 6d70 696c 6528 2228 6368 616e 7b31 2c32  mpile("(chan{1,2
+0000b4e0: 7d28 656c 293f 7c66 696c 7428 6572 293f  }(el)?|filt(er)?
+0000b4f0: 2973 3f22 2c20 7265 2e49 474e 4f52 4543  )s?", re.IGNOREC
+0000b500: 4153 4529 0d0a 2020 2020 2020 2020 2222  ASE)..        ""
+0000b510: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000b520: 6e20 7365 6c66 2e5f 6368 616e 6e65 6c5f  n self._channel_
+0000b530: 6772 6f75 705f 7265 6765 780d 0a0d 0a20  group_regex.... 
+0000b540: 2020 2040 6368 616e 6e65 6c47 726f 7570     @channelGroup
+0000b550: 5f70 6174 7465 726e 2e73 6574 7465 720d  _pattern.setter.
+0000b560: 0a20 2020 2064 6566 2063 6861 6e6e 656c  .    def channel
+0000b570: 4772 6f75 705f 7061 7474 6572 6e28 7365  Group_pattern(se
+0000b580: 6c66 2c20 7661 6c75 653a 2050 6174 7465  lf, value: Patte
+0000b590: 726e 207c 2073 7472 2920 2d3e 204e 6f6e  rn | str) -> Non
+0000b5a0: 653a 0d0a 2020 2020 2020 2020 6966 2069  e:..        if i
+0000b5b0: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
+0000b5c0: 2073 7472 293a 0d0a 2020 2020 2020 2020   str):..        
+0000b5d0: 2020 2020 7661 6c75 6520 3d20 7265 2e63      value = re.c
+0000b5e0: 6f6d 7069 6c65 2876 616c 7565 2c20 7265  ompile(value, re
+0000b5f0: 2e49 474e 4f52 4543 4153 4529 0d0a 2020  .IGNORECASE)..  
+0000b600: 2020 2020 2020 656c 6966 206e 6f74 2069        elif not i
+0000b610: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
+0000b620: 2050 6174 7465 726e 293a 0d0a 2020 2020   Pattern):..    
+0000b630: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+0000b640: 7065 4572 726f 7228 0d0a 2020 2020 2020  peError(..      
+0000b650: 2020 2020 2020 2020 2020 2263 6861 6e6e            "chann
+0000b660: 656c 4772 6f75 7020 5061 7474 6572 6e20  elGroup Pattern 
+0000b670: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
+0000b680: 206f 7220 636f 6d70 696c 6564 2072 6567   or compiled reg
+0000b690: 6578 220d 0a20 2020 2020 2020 2020 2020  ex"..           
+0000b6a0: 2020 2020 2066 2262 7574 2069 7320 7479       f"but is ty
+0000b6b0: 7065 207b 7479 7065 2876 616c 7565 297d  pe {type(value)}
+0000b6c0: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
+0000b6d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0000b6e0: 6368 616e 6e65 6c5f 6772 6f75 705f 7265  channel_group_re
+0000b6f0: 6765 7820 3d20 7661 6c75 650d 0a0d 0a20  gex = value.... 
+0000b700: 2020 2064 6566 2067 7565 7373 4f62 6a65     def guessObje
+0000b710: 6374 6976 6544 6576 6963 6573 2873 656c  ctiveDevices(sel
+0000b720: 6629 202d 3e20 6c69 7374 5b73 7472 5d3a  f) -> list[str]:
+0000b730: 0d0a 2020 2020 2020 2020 2222 2246 696e  ..        """Fin
+0000b740: 6420 616e 7920 6c6f 6164 6564 2064 6576  d any loaded dev
+0000b750: 6963 6573 2074 6861 7420 6172 6520 6c69  ices that are li
+0000b760: 6b65 6c79 2074 6f20 6265 2061 6e20 4f62  kely to be an Ob
+0000b770: 6a65 6374 6976 652f 4e6f 7365 7069 6563  jective/Nosepiec
+0000b780: 652e 0d0a 0d0a 2020 2020 2020 2020 3a73  e.....        :s
+0000b790: 7061 726b 6c65 733a 202a 5468 6973 206d  parkles: *This m
+0000b7a0: 6574 686f 6420 6973 206e 6577 2069 6e20  ethod is new in 
+0000b7b0: 6043 4d4d 436f 7265 506c 7573 602e 2a0d  `CMMCorePlus`.*.
+0000b7c0: 0a0d 0a20 2020 2020 2020 204c 696b 656c  ...        Likel
+0000b7d0: 7920 6d61 7463 6865 7320 6172 6520 6c6f  y matches are lo
+0000b7e0: 6164 6564 2053 7461 7465 4465 7669 6365  aded StateDevice
+0000b7f0: 7320 7769 7468 206e 616d 6573 2074 6861  s with names tha
+0000b800: 7420 6d61 7463 6820 7468 6973 206f 626a  t match this obj
+0000b810: 6563 7427 730d 0a20 2020 2020 2020 2060  ect's..        `
+0000b820: 6f62 6a65 6374 6976 655f 6465 7669 6365  objective_device
+0000b830: 5f70 6174 7465 726e 6020 7072 6f70 6572  _pattern` proper
+0000b840: 7479 2e20 5468 6973 2069 7320 6120 7365  ty. This is a se
+0000b850: 7474 6162 6c65 2070 726f 7065 7274 790d  ttable property.
+0000b860: 0a20 2020 2020 2020 2077 6974 6820 6120  .        with a 
+0000b870: 6465 6661 756c 7420 7661 6c75 6520 6f66  default value of
+0000b880: 3a3a 0d0a 0d0a 2020 2020 2020 2020 2020  ::....          
+0000b890: 2020 7265 2e63 6f6d 7069 6c65 2822 282e    re.compile("(.
+0000b8a0: 2b29 3f28 6e6f 7365 7069 6563 657c 6f62  +)?(nosepiece|ob
+0000b8b0: 6a28 6563 7469 7665 293f 2928 7475 7272  j(ective)?)(turr
+0000b8c0: 6574 293f 733f 222c 2072 652e 4947 4e4f  et)?s?", re.IGNO
+0000b8d0: 5245 4341 5345 290d 0a20 2020 2020 2020  RECASE)..       
+0000b8e0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+0000b8f0: 7475 726e 205b 0d0a 2020 2020 2020 2020  turn [..        
+0000b900: 2020 2020 6465 7669 6365 0d0a 2020 2020      device..    
+0000b910: 2020 2020 2020 2020 666f 7220 6465 7669          for devi
+0000b920: 6365 2069 6e20 7365 6c66 2e67 6574 4c6f  ce in self.getLo
+0000b930: 6164 6564 4465 7669 6365 734f 6654 7970  adedDevicesOfTyp
+0000b940: 6528 4465 7669 6365 5479 7065 2e53 7461  e(DeviceType.Sta
+0000b950: 7465 4465 7669 6365 290d 0a20 2020 2020  teDevice)..     
+0000b960: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000b970: 6f62 6a65 6374 6976 655f 7265 6765 782e  objective_regex.
+0000b980: 6d61 7463 6828 6465 7669 6365 290d 0a20  match(device).. 
+0000b990: 2020 2020 2020 205d 0d0a 0d0a 2020 2020         ]....    
+0000b9a0: 6465 6620 6765 744f 7247 7565 7373 4368  def getOrGuessCh
+0000b9b0: 616e 6e65 6c47 726f 7570 2873 656c 6629  annelGroup(self)
+0000b9c0: 202d 3e20 6c69 7374 5b73 7472 5d3a 0d0a   -> list[str]:..
+0000b9d0: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+0000b9e0: 6865 2063 6861 6e6e 656c 4772 6f75 7020  he channelGroup 
+0000b9f0: 6f72 2066 696e 6420 6120 6c69 6b65 6c79  or find a likely
+0000ba00: 2073 6574 206f 6620 6361 6e64 6964 6174   set of candidat
+0000ba10: 6573 2e0d 0a0d 0a20 2020 2020 2020 203a  es.....        :
+0000ba20: 7370 6172 6b6c 6573 3a20 2a54 6869 7320  sparkles: *This 
+0000ba30: 6d65 7468 6f64 2069 7320 6e65 7720 696e  method is new in
+0000ba40: 2060 434d 4d43 6f72 6550 6c75 7360 2e2a   `CMMCorePlus`.*
+0000ba50: 0d0a 0d0a 2020 2020 2020 2020 4966 2074  ....        If t
+0000ba60: 6865 2067 726f 7570 2069 7320 6e6f 7420  he group is not 
+0000ba70: 6465 6669 6e65 6420 7669 6120 602e 6765  defined via `.ge
+0000ba80: 7443 6861 6e6e 656c 4772 6f75 7060 2074  tChannelGroup` t
+0000ba90: 6865 6e20 6c69 6b65 6c79 2063 616e 6469  hen likely candi
+0000baa0: 6461 7465 730d 0a20 2020 2020 2020 2077  dates..        w
+0000bab0: 696c 6c20 6265 2066 6f75 6e64 2062 7920  ill be found by 
+0000bac0: 7365 6172 6368 696e 6720 666f 7220 636f  searching for co
+0000bad0: 6e66 6967 2067 726f 7570 7320 7769 7468  nfig groups with
+0000bae0: 206e 616d 6573 2074 6861 7420 6d61 7463   names that matc
+0000baf0: 6820 7468 6973 0d0a 2020 2020 2020 2020  h this..        
+0000bb00: 6f62 6a65 6374 2773 2060 6368 616e 6e65  object's `channe
+0000bb10: 6c47 726f 7570 5f70 6174 7465 726e 6020  lGroup_pattern` 
+0000bb20: 7072 6f70 6572 7479 2e20 5468 6973 2069  property. This i
+0000bb30: 7320 6120 7365 7474 6162 6c65 2070 726f  s a settable pro
+0000bb40: 7065 7274 790d 0a20 2020 2020 2020 2077  perty..        w
+0000bb50: 6974 6820 6120 6465 6661 756c 7420 7661  ith a default va
+0000bb60: 6c75 6520 6f66 3a0d 0a0d 0a20 2020 2020  lue of:....     
+0000bb70: 2020 2020 2020 2072 6567 203d 2072 652e         reg = re.
+0000bb80: 636f 6d70 696c 6528 2228 6368 616e 7b31  compile("(chan{1
+0000bb90: 2c32 7d28 656c 293f 7c66 696c 7428 6572  ,2}(el)?|filt(er
+0000bba0: 293f 2973 3f22 2c20 7265 2e49 474e 4f52  )?)s?", re.IGNOR
+0000bbb0: 4543 4153 4529 0d0a 0d0a 2020 2020 2020  ECASE)....      
+0000bbc0: 2020 2222 220d 0a20 2020 2020 2020 2023    """..        #
+0000bbd0: 2073 6f75 7263 6572 7920 736b 6970 3a20   sourcery skip: 
+0000bbe0: 7573 652d 6e61 6d65 642d 6578 7072 6573  use-named-expres
+0000bbf0: 7369 6f6e 0d0a 2020 2020 2020 2020 6368  sion..        ch
+0000bc00: 616e 5f67 726f 7570 203d 2073 656c 662e  an_group = self.
+0000bc10: 6765 7443 6861 6e6e 656c 4772 6f75 7028  getChannelGroup(
+0000bc20: 290d 0a20 2020 2020 2020 2069 6620 6368  )..        if ch
+0000bc30: 616e 5f67 726f 7570 3a0d 0a20 2020 2020  an_group:..     
+0000bc40: 2020 2020 2020 2072 6574 7572 6e20 5b63         return [c
+0000bc50: 6861 6e5f 6772 6f75 705d 0d0a 2020 2020  han_group]..    
+0000bc60: 2020 2020 2320 6e6f 7420 7365 7420 696e      # not set in
+0000bc70: 2063 6f72 652e 2054 7279 2022 4368 616e   core. Try "Chan
+0000bc80: 6e65 6c22 2061 6e64 206f 7468 6572 2076  nel" and other v
+0000bc90: 6172 6961 7469 6f6e 7320 6173 2066 616c  ariations as fal
+0000bca0: 6c62 6163 6b73 0d0a 2020 2020 2020 2020  lbacks..        
+0000bcb0: 7265 7475 726e 205b 0d0a 2020 2020 2020  return [..      
+0000bcc0: 2020 2020 2020 6772 6f75 700d 0a20 2020        group..   
+0000bcd0: 2020 2020 2020 2020 2066 6f72 2067 726f           for gro
+0000bce0: 7570 2069 6e20 7365 6c66 2e67 6574 4176  up in self.getAv
+0000bcf0: 6169 6c61 626c 6543 6f6e 6669 6747 726f  ailableConfigGro
+0000bd00: 7570 7328 290d 0a20 2020 2020 2020 2020  ups()..         
+0000bd10: 2020 2069 6620 7365 6c66 2e5f 6368 616e     if self._chan
+0000bd20: 6e65 6c5f 6772 6f75 705f 7265 6765 782e  nel_group_regex.
+0000bd30: 6d61 7463 6828 6772 6f75 7029 0d0a 2020  match(group)..  
+0000bd40: 2020 2020 2020 5d0d 0a0d 0a20 2020 2064        ]....    d
+0000bd50: 6566 2073 6574 5265 6c61 7469 7665 5859  ef setRelativeXY
+0000bd60: 5a50 6f73 6974 696f 6e28 0d0a 2020 2020  ZPosition(..    
+0000bd70: 2020 2020 7365 6c66 2c20 6478 3a20 666c      self, dx: fl
+0000bd80: 6f61 7420 3d20 302c 2064 793a 2066 6c6f  oat = 0, dy: flo
+0000bd90: 6174 203d 2030 2c20 647a 3a20 666c 6f61  at = 0, dz: floa
+0000bda0: 7420 3d20 300d 0a20 2020 2029 202d 3e20  t = 0..    ) -> 
+0000bdb0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2022  None:..        "
+0000bdc0: 2222 5365 7473 2074 6865 2072 656c 6174  ""Sets the relat
+0000bdd0: 6976 6520 5859 5a20 706f 7369 7469 6f6e  ive XYZ position
+0000bde0: 2069 6e20 6d69 6372 6f6e 732e 0d0a 0d0a   in microns.....
+0000bdf0: 2020 2020 2020 2020 3a73 7061 726b 6c65          :sparkle
+0000be00: 733a 202a 5468 6973 206d 6574 686f 6420  s: *This method 
+0000be10: 6973 206e 6577 2069 6e20 6043 4d4d 436f  is new in `CMMCo
+0000be20: 7265 506c 7573 602e 2a0d 0a0d 0a20 2020  rePlus`.*....   
+0000be30: 2020 2020 2054 6869 7320 6973 2061 2063       This is a c
+0000be40: 6f6e 7665 6e69 656e 6365 206d 6574 686f  onvenience metho
+0000be50: 6420 7468 6174 2063 616c 6c73 2060 7365  d that calls `se
+0000be60: 7458 5950 6f73 6974 696f 6e60 2061 6e64  tXYPosition` and
+0000be70: 2060 7365 745a 506f 7369 7469 6f6e 600d   `setZPosition`.
+0000be80: 0a20 2020 2020 2020 2077 6974 6820 7468  .        with th
+0000be90: 6520 6375 7272 656e 7420 706f 7369 7469  e current positi
+0000bea0: 6f6e 2061 7320 7468 6520 7374 6172 7469  on as the starti
+0000beb0: 6e67 2070 6f69 6e74 2e0d 0a0d 0a20 2020  ng point.....   
+0000bec0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+0000bed0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000bee0: 2d2d 2d0d 0a20 2020 2020 2020 2064 7820  ---..        dx 
+0000bef0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
+0000bf00: 6c0d 0a20 2020 2020 2020 2020 2020 2054  l..            T
+0000bf10: 6865 2072 656c 6174 6976 6520 6368 616e  he relative chan
+0000bf20: 6765 2069 6e20 5820 706f 7369 7469 6f6e  ge in X position
+0000bf30: 2c20 6279 2064 6566 6175 6c74 2030 0d0a  , by default 0..
+0000bf40: 2020 2020 2020 2020 6479 203a 2066 6c6f          dy : flo
+0000bf50: 6174 2c20 6f70 7469 6f6e 616c 0d0a 2020  at, optional..  
+0000bf60: 2020 2020 2020 2020 2020 5468 6520 7265            The re
+0000bf70: 6c61 7469 7665 2063 6861 6e67 6520 696e  lative change in
+0000bf80: 2059 2070 6f73 6974 696f 6e2c 2062 7920   Y position, by 
+0000bf90: 6465 6661 756c 7420 300d 0a20 2020 2020  default 0..     
+0000bfa0: 2020 2064 7a20 3a20 666c 6f61 742c 206f     dz : float, o
+0000bfb0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0000bfc0: 2020 2020 2054 6865 2072 656c 6174 6976       The relativ
+0000bfd0: 6520 6368 616e 6765 2069 6e20 5a20 706f  e change in Z po
+0000bfe0: 7369 7469 6f6e 2c20 6279 2064 6566 6175  sition, by defau
+0000bff0: 6c74 2030 0d0a 2020 2020 2020 2020 2222  lt 0..        ""
+0000c000: 220d 0a20 2020 2020 2020 2069 6620 6478  "..        if dx
+0000c010: 206f 7220 6479 3a0d 0a20 2020 2020 2020   or dy:..       
+0000c020: 2020 2020 2078 2c20 7920 3d20 7365 6c66       x, y = self
+0000c030: 2e67 6574 5850 6f73 6974 696f 6e28 292c  .getXPosition(),
+0000c040: 2073 656c 662e 6765 7459 506f 7369 7469   self.getYPositi
+0000c050: 6f6e 2829 0d0a 2020 2020 2020 2020 2020  on()..          
+0000c060: 2020 7365 6c66 2e73 6574 5859 506f 7369    self.setXYPosi
+0000c070: 7469 6f6e 2878 202b 2064 782c 2079 202b  tion(x + dx, y +
+0000c080: 2064 7929 0d0a 2020 2020 2020 2020 6966   dy)..        if
+0000c090: 2064 7a3a 0d0a 2020 2020 2020 2020 2020   dz:..          
+0000c0a0: 2020 7a20 3d20 7365 6c66 2e67 6574 506f    z = self.getPo
+0000c0b0: 7369 7469 6f6e 2873 656c 662e 6765 7446  sition(self.getF
+0000c0c0: 6f63 7573 4465 7669 6365 2829 290d 0a20  ocusDevice()).. 
+0000c0d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c0e0: 7365 745a 506f 7369 7469 6f6e 287a 202b  setZPosition(z +
+0000c0f0: 2064 7a29 0d0a 2020 2020 2020 2020 7365   dz)..        se
+0000c100: 6c66 2e77 6169 7446 6f72 4465 7669 6365  lf.waitForDevice
+0000c110: 2873 656c 662e 6765 7458 5953 7461 6765  (self.getXYStage
+0000c120: 4465 7669 6365 2829 290d 0a20 2020 2020  Device())..     
+0000c130: 2020 2073 656c 662e 7761 6974 466f 7244     self.waitForD
+0000c140: 6576 6963 6528 7365 6c66 2e67 6574 466f  evice(self.getFo
+0000c150: 6375 7344 6576 6963 6528 2929 0d0a 0d0a  cusDevice())....
+0000c160: 2020 2020 6465 6620 6765 745a 506f 7369      def getZPosi
+0000c170: 7469 6f6e 2873 656c 6629 202d 3e20 666c  tion(self) -> fl
+0000c180: 6f61 743a 0d0a 2020 2020 2020 2020 2222  oat:..        ""
+0000c190: 224f 6274 6169 6e73 2074 6865 2063 7572  "Obtains the cur
+0000c1a0: 7265 6e74 2070 6f73 6974 696f 6e20 6f66  rent position of
+0000c1b0: 2074 6865 205a 2061 7869 7320 6f66 2074   the Z axis of t
+0000c1c0: 6865 205a 2073 7461 6765 2069 6e20 6d69  he Z stage in mi
+0000c1d0: 6372 6f6e 732e 0d0a 0d0a 2020 2020 2020  crons.....      
+0000c1e0: 2020 3a73 7061 726b 6c65 733a 202a 5468    :sparkles: *Th
+0000c1f0: 6973 206d 6574 686f 6420 6973 206e 6577  is method is new
+0000c200: 2069 6e20 6043 4d4d 436f 7265 506c 7573   in `CMMCorePlus
+0000c210: 603a 0d0a 2020 2020 2020 2020 6164 6465  `:..        adde
+0000c220: 6420 746f 2063 6f6d 706c 656d 656e 7420  d to complement 
+0000c230: 6067 6574 5850 6f73 6974 696f 6e60 2061  `getXPosition` a
+0000c240: 6e64 2060 6765 7459 506f 7369 7469 6f6e  nd `getYPosition
+0000c250: 602a 0d0a 2020 2020 2020 2020 2222 220d  `*..        """.
+0000c260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c270: 7365 6c66 2e67 6574 506f 7369 7469 6f6e  self.getPosition
+0000c280: 2873 656c 662e 6765 7446 6f63 7573 4465  (self.getFocusDe
+0000c290: 7669 6365 2829 290d 0a0d 0a20 2020 2064  vice())....    d
+0000c2a0: 6566 2073 6574 5a50 6f73 6974 696f 6e28  ef setZPosition(
+0000c2b0: 7365 6c66 2c20 7661 6c3a 2066 6c6f 6174  self, val: float
+0000c2c0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+0000c2d0: 2020 2020 2222 2253 6574 2074 6865 2070      """Set the p
+0000c2e0: 6f73 6974 696f 6e20 6f66 2074 6865 2063  osition of the c
+0000c2f0: 7572 7265 6e74 2066 6f63 7573 2064 6576  urrent focus dev
+0000c300: 6963 6520 696e 206d 6963 726f 6e73 2e0d  ice in microns..
+0000c310: 0a0d 0a20 2020 2020 2020 203a 7370 6172  ...        :spar
+0000c320: 6b6c 6573 3a20 2a54 6869 7320 6d65 7468  kles: *This meth
+0000c330: 6f64 2069 7320 6e65 7720 696e 2060 434d  od is new in `CM
+0000c340: 4d43 6f72 6550 6c75 7360 3a0d 0a20 2020  MCorePlus`:..   
+0000c350: 2020 2020 2061 6464 6564 2074 6f20 636f       added to co
+0000c360: 6d70 6c65 6d65 6e74 2060 7365 7458 5950  mplement `setXYP
+0000c370: 6f73 6974 696f 6e60 2a0d 0a20 2020 2020  osition`*..     
+0000c380: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000c390: 7265 7475 726e 2073 656c 662e 7365 7450  return self.setP
+0000c3a0: 6f73 6974 696f 6e28 7365 6c66 2e67 6574  osition(self.get
+0000c3b0: 466f 6375 7344 6576 6963 6528 292c 2076  FocusDevice(), v
+0000c3c0: 616c 290d 0a0d 0a20 2020 2040 6f76 6572  al)....    @over
+0000c3d0: 6c6f 6164 0d0a 2020 2020 6465 6620 7365  load..    def se
+0000c3e0: 7450 6f73 6974 696f 6e28 7365 6c66 2c20  tPosition(self, 
+0000c3f0: 706f 7369 7469 6f6e 3a20 666c 6f61 7429  position: float)
+0000c400: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+0000c410: 2020 202e 2e2e 0d0a 0d0a 2020 2020 406f     .......    @o
+0000c420: 7665 726c 6f61 640d 0a20 2020 2064 6566  verload..    def
+0000c430: 2073 6574 506f 7369 7469 6f6e 2873 656c   setPosition(sel
+0000c440: 662c 2073 7461 6765 4c61 6265 6c3a 2073  f, stageLabel: s
+0000c450: 7472 2c20 706f 7369 7469 6f6e 3a20 666c  tr, position: fl
+0000c460: 6f61 7429 202d 3e20 4e6f 6e65 3a0d 0a20  oat) -> None:.. 
+0000c470: 2020 2020 2020 202e 2e2e 0d0a 0d0a 2020         .......  
+0000c480: 2020 4073 796e 6368 726f 6e69 7a65 6428    @synchronized(
+0000c490: 5f6c 6f63 6b29 0d0a 2020 2020 6465 6620  _lock)..    def 
+0000c4a0: 7365 7450 6f73 6974 696f 6e28 7365 6c66  setPosition(self
+0000c4b0: 2c20 2a61 7267 733a 2041 6e79 2c20 2a2a  , *args: Any, **
+0000c4c0: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
+0000c4d0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2022  None:..        "
+0000c4e0: 2222 5365 7420 706f 7369 7469 6f6e 206f  ""Set position o
+0000c4f0: 6620 7468 6520 7374 6167 6520 696e 206d  f the stage in m
+0000c500: 6963 726f 6e73 2e0d 0a0d 0a20 2020 2020  icrons.....     
+0000c510: 2020 202a 2a57 6879 204f 7665 7272 6964     **Why Overrid
+0000c520: 653f 2a2a 2054 6f20 6164 6420 6120 6c6f  e?** To add a lo
+0000c530: 636b 2074 6f20 7072 6576 656e 7420 636f  ck to prevent co
+0000c540: 6e63 7572 7265 6e74 2063 616c 6c73 2061  ncurrent calls a
+0000c550: 6372 6f73 7320 7468 7265 6164 732e 0d0a  cross threads...
+0000c560: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0000c570: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+0000c580: 7228 292e 7365 7450 6f73 6974 696f 6e28  r().setPosition(
+0000c590: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+0000c5a0: 0d0a 0d0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
+0000c5b0: 640d 0a20 2020 2064 6566 2073 6574 5859  d..    def setXY
+0000c5c0: 506f 7369 7469 6f6e 2873 656c 662c 2078  Position(self, x
+0000c5d0: 3a20 666c 6f61 742c 2079 3a20 666c 6f61  : float, y: floa
+0000c5e0: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
+0000c5f0: 2020 2020 202e 2e2e 0d0a 0d0a 2020 2020       .......    
+0000c600: 406f 7665 726c 6f61 640d 0a20 2020 2064  @overload..    d
+0000c610: 6566 2073 6574 5859 506f 7369 7469 6f6e  ef setXYPosition
+0000c620: 2873 656c 662c 2078 7953 7461 6765 4c61  (self, xyStageLa
+0000c630: 6265 6c3a 2073 7472 2c20 783a 2066 6c6f  bel: str, x: flo
+0000c640: 6174 2c20 793a 2066 6c6f 6174 2920 2d3e  at, y: float) ->
+0000c650: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000c660: 2e2e 2e0d 0a0d 0a20 2020 2040 7379 6e63  .......    @sync
+0000c670: 6872 6f6e 697a 6564 285f 6c6f 636b 290d  hronized(_lock).
+0000c680: 0a20 2020 2064 6566 2073 6574 5859 506f  .    def setXYPo
+0000c690: 7369 7469 6f6e 2873 656c 662c 202a 6172  sition(self, *ar
+0000c6a0: 6773 3a20 416e 792c 202a 2a6b 7761 7267  gs: Any, **kwarg
+0000c6b0: 733a 2041 6e79 2920 2d3e 204e 6f6e 653a  s: Any) -> None:
+0000c6c0: 0d0a 2020 2020 2020 2020 2222 2253 6574  ..        """Set
+0000c6d0: 7320 7468 6520 706f 7369 7469 6f6e 206f  s the position o
+0000c6e0: 6620 7468 6520 5859 2073 7461 6765 2069  f the XY stage i
+0000c6f0: 6e20 6d69 6372 6f6e 732e 0d0a 0d0a 2020  n microns.....  
+0000c700: 2020 2020 2020 2a2a 5768 7920 4f76 6572        **Why Over
+0000c710: 7269 6465 3f2a 2a20 546f 2061 6464 2061  ride?** To add a
+0000c720: 206c 6f63 6b20 746f 2070 7265 7665 6e74   lock to prevent
+0000c730: 2063 6f6e 6375 7272 656e 7420 6361 6c6c   concurrent call
+0000c740: 7320 6163 726f 7373 2074 6872 6561 6473  s across threads
+0000c750: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+0000c760: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000c770: 7570 6572 2829 2e73 6574 5859 506f 7369  uper().setXYPosi
+0000c780: 7469 6f6e 282a 6172 6773 2c20 2a2a 6b77  tion(*args, **kw
+0000c790: 6172 6773 290d 0a0d 0a20 2020 2040 7379  args)....    @sy
+0000c7a0: 6e63 6872 6f6e 697a 6564 285f 6c6f 636b  nchronized(_lock
+0000c7b0: 290d 0a20 2020 2064 6566 2067 6574 4361  )..    def getCa
+0000c7c0: 6d65 7261 4368 616e 6e65 6c4e 616d 6573  meraChannelNames
+0000c7d0: 2873 656c 6629 202d 3e20 7475 706c 655b  (self) -> tuple[
+0000c7e0: 7374 722c 202e 2e2e 5d3a 0d0a 2020 2020  str, ...]:..    
+0000c7f0: 2020 2020 2222 2243 6f6e 7665 6e69 656e      """Convenien
+0000c800: 6365 206d 6574 686f 6420 746f 2063 616c  ce method to cal
+0000c810: 6c20 6067 6574 4361 6d65 7261 4368 616e  l `getCameraChan
+0000c820: 6e65 6c4e 616d 6560 2066 6f72 2061 6c6c  nelName` for all
+0000c830: 2063 616d 6572 6120 6368 616e 6e65 6c73   camera channels
+0000c840: 2e0d 0a0d 0a20 2020 2020 2020 203a 7370  .....        :sp
+0000c850: 6172 6b6c 6573 3a20 2a54 6869 7320 6d65  arkles: *This me
+0000c860: 7468 6f64 2069 7320 6e65 7720 696e 2060  thod is new in `
+0000c870: 434d 4d43 6f72 6550 6c75 7360 2e2a 0d0a  CMMCorePlus`.*..
+0000c880: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0000c890: 2020 2020 2072 6574 7572 6e20 7475 706c       return tupl
+0000c8a0: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+0000c8b0: 7365 6c66 2e67 6574 4361 6d65 7261 4368  self.getCameraCh
+0000c8c0: 616e 6e65 6c4e 616d 6528 6929 0d0a 2020  annelName(i)..  
+0000c8d0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+0000c8e0: 696e 2072 616e 6765 2873 656c 662e 6765  in range(self.ge
+0000c8f0: 744e 756d 6265 724f 6643 616d 6572 6143  tNumberOfCameraC
+0000c900: 6861 6e6e 656c 7328 2929 0d0a 2020 2020  hannels())..    
+0000c910: 2020 2020 290d 0a0d 0a20 2020 2040 7379      )....    @sy
+0000c920: 6e63 6872 6f6e 697a 6564 285f 6c6f 636b  nchronized(_lock
+0000c930: 290d 0a20 2020 2064 6566 2073 6e61 7049  )..    def snapI
+0000c940: 6d61 6765 2873 656c 6629 202d 3e20 4e6f  mage(self) -> No
+0000c950: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
+0000c960: 4163 7175 6972 6573 2061 2073 696e 676c  Acquires a singl
+0000c970: 6520 696d 6167 6520 7769 7468 2063 7572  e image with cur
+0000c980: 7265 6e74 2073 6574 7469 6e67 732e 0d0a  rent settings...
+0000c990: 0d0a 2020 2020 2020 2020 2a2a 5768 7920  ..        **Why 
+0000c9a0: 4f76 6572 7269 6465 3f2a 2a20 546f 2061  Override?** To a
+0000c9b0: 6464 2061 206c 6f63 6b20 746f 2070 7265  dd a lock to pre
+0000c9c0: 7665 6e74 2063 6f6e 6375 7272 656e 7420  vent concurrent 
+0000c9d0: 6361 6c6c 7320 6163 726f 7373 2074 6872  calls across thr
+0000c9e0: 6561 6473 2e0d 0a20 2020 2020 2020 2022  eads...        "
+0000c9f0: 2222 0d0a 2020 2020 2020 2020 6175 746f  ""..        auto
+0000ca00: 7368 7574 7465 7220 3d20 7365 6c66 2e67  shutter = self.g
+0000ca10: 6574 4175 746f 5368 7574 7465 7228 290d  etAutoShutter().
+0000ca20: 0a20 2020 2020 2020 2069 6620 6175 746f  .        if auto
+0000ca30: 7368 7574 7465 723a 0d0a 2020 2020 2020  shutter:..      
+0000ca40: 2020 2020 2020 7365 6c66 2e65 7665 6e74        self.event
+0000ca50: 732e 7072 6f70 6572 7479 4368 616e 6765  s.propertyChange
+0000ca60: 642e 656d 6974 2873 656c 662e 6765 7453  d.emit(self.getS
+0000ca70: 6875 7474 6572 4465 7669 6365 2829 2c20  hutterDevice(), 
+0000ca80: 2253 7461 7465 222c 2054 7275 6529 0d0a  "State", True)..
+0000ca90: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+0000caa0: 2020 2020 2020 2020 2020 7375 7065 7228            super(
+0000cab0: 292e 736e 6170 496d 6167 6528 290d 0a20  ).snapImage().. 
+0000cac0: 2020 2020 2020 2066 696e 616c 6c79 3a0d         finally:.
+0000cad0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000cae0: 6175 746f 7368 7574 7465 723a 0d0a 2020  autoshutter:..  
+0000caf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cb00: 6c66 2e65 7665 6e74 732e 7072 6f70 6572  lf.events.proper
+0000cb10: 7479 4368 616e 6765 642e 656d 6974 280d  tyChanged.emit(.
+0000cb20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cb30: 2020 2020 2073 656c 662e 6765 7453 6875       self.getShu
+0000cb40: 7474 6572 4465 7669 6365 2829 2c20 2253  tterDevice(), "S
+0000cb50: 7461 7465 222c 2046 616c 7365 0d0a 2020  tate", False..  
+0000cb60: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0000cb70: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+0000cb80: 0d0a 2020 2020 6465 6620 6d64 6128 7365  ..    def mda(se
+0000cb90: 6c66 2920 2d3e 204d 4441 5275 6e6e 6572  lf) -> MDARunner
+0000cba0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+0000cbb0: 7475 726e 2074 6865 2060 4d44 4152 756e  turn the `MDARun
+0000cbc0: 6e65 7260 2066 6f72 2074 6869 7320 6043  ner` for this `C
+0000cbd0: 4d4d 436f 7265 506c 7573 6020 696e 7374  MMCorePlus` inst
+0000cbe0: 616e 6365 2e0d 0a0d 0a20 2020 2020 2020  ance.....       
+0000cbf0: 203a 7370 6172 6b6c 6573 3a20 2a54 6869   :sparkles: *Thi
+0000cc00: 7320 6d65 7468 6f64 2069 7320 6e65 7720  s method is new 
+0000cc10: 696e 2060 434d 4d43 6f72 6550 6c75 7360  in `CMMCorePlus`
+0000cc20: 2e2a 0d0a 2020 2020 2020 2020 2222 220d  .*..        """.
+0000cc30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cc40: 7365 6c66 2e5f 6d64 615f 7275 6e6e 6572  self._mda_runner
+0000cc50: 0d0a 0d0a 2020 2020 6465 6620 7275 6e5f  ....    def run_
+0000cc60: 6d64 6128 7365 6c66 2c20 6576 656e 7473  mda(self, events
+0000cc70: 3a20 4974 6572 6162 6c65 5b4d 4441 4576  : Iterable[MDAEv
+0000cc80: 656e 745d 2c20 626c 6f63 6b3a 2062 6f6f  ent], block: boo
+0000cc90: 6c20 3d20 4661 6c73 6529 202d 3e20 5468  l = False) -> Th
+0000cca0: 7265 6164 3a0d 0a20 2020 2020 2020 2022  read:..        "
+0000ccb0: 2222 5275 6e20 6120 7365 7175 656e 6365  ""Run a sequence
+0000ccc0: 206f 6620 5b75 7365 712e 4d44 4145 7665   of [useq.MDAEve
+0000ccd0: 6e74 5d5b 5d20 6f6e 2061 206e 6577 2074  nt][] on a new t
+0000cce0: 6872 6561 642e 0d0a 0d0a 2020 2020 2020  hread.....      
+0000ccf0: 2020 3a73 7061 726b 6c65 733a 202a 5468    :sparkles: *Th
+0000cd00: 6973 206d 6574 686f 6420 6973 206e 6577  is method is new
+0000cd10: 2069 6e20 6043 4d4d 436f 7265 506c 7573   in `CMMCorePlus
+0000cd20: 602e 2a0d 0a0d 0a20 2020 2020 2020 2054  `.*....        T
+0000cd30: 6865 2063 7572 7265 6e74 6c79 2072 6567  he currently reg
+0000cd40: 6973 7465 7265 6420 4d44 4145 6e67 696e  istered MDAEngin
+0000cd50: 6520 2860 636f 7265 2e6d 6461 2e65 6e67  e (`core.mda.eng
+0000cd60: 696e 6560 2920 7769 6c6c 2062 6520 7265  ine`) will be re
+0000cd70: 7370 6f6e 7369 626c 6520 666f 720d 0a20  sponsible for.. 
+0000cd80: 2020 2020 2020 2065 7865 6375 7469 6e67         executing
+0000cd90: 2074 6865 2061 6371 7569 7369 7469 6f6e   the acquisition
+0000cda0: 2e0d 0a0d 0a20 2020 2020 2020 2041 6674  .....        Aft
+0000cdb0: 6572 2073 7461 7274 696e 6720 7468 6520  er starting the 
+0000cdc0: 7365 7175 656e 6365 2079 6f75 2063 616e  sequence you can
+0000cdd0: 2070 6175 7365 206f 7220 6361 6e63 656c   pause or cancel
+0000cde0: 2077 6974 6820 7468 6520 6d64 6120 7769   with the mda wi
+0000cdf0: 7468 0d0a 2020 2020 2020 2020 7468 6520  th..        the 
+0000ce00: 6d64 6120 6f62 6a65 6374 2773 2060 746f  mda object's `to
+0000ce10: 6767 6c65 5f70 6175 7365 6020 616e 6420  ggle_pause` and 
+0000ce20: 6063 616e 6365 6c60 206d 6574 686f 6473  `cancel` methods
+0000ce30: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+0000ce40: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+0000ce50: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+0000ce60: 2020 2020 2065 7665 6e74 7320 3a20 4974       events : It
+0000ce70: 6572 6162 6c65 5b75 7365 712e 4d44 4145  erable[useq.MDAE
+0000ce80: 7665 6e74 5d0d 0a20 2020 2020 2020 2020  vent]..         
+0000ce90: 2020 2041 6e20 6974 6572 6162 6c65 206f     An iterable o
+0000cea0: 6620 5b75 7365 712e 4d44 4145 7665 6e74  f [useq.MDAEvent
+0000ceb0: 5d5b 5d20 746f 2065 7865 6375 7465 2e20  ][] to execute. 
+0000cec0: 2054 6869 7320 6d61 7920 6265 2061 6e20   This may be an 
+0000ced0: 696e 7374 616e 6365 0d0a 2020 2020 2020  instance..      
+0000cee0: 2020 2020 2020 6f66 205b 7573 6571 2e4d        of [useq.M
+0000cef0: 4441 5365 7175 656e 6365 5d5b 5d2c 206f  DASequence][], o
+0000cf00: 7220 616e 7920 6f74 6865 7220 6974 6572  r any other iter
+0000cf10: 6162 6c65 206f 6620 5b75 7365 712e 4d44  able of [useq.MD
+0000cf20: 4145 7665 6e74 5d5b 5d2e 0d0a 2020 2020  AEvent][]...    
+0000cf30: 2020 2020 626c 6f63 6b20 3a20 626f 6f6c      block : bool
+0000cf40: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+0000cf50: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+0000cf60: 2062 6c6f 636b 2075 6e74 696c 2074 6865   block until the
+0000cf70: 2073 6571 7565 6e63 6520 6973 2063 6f6d   sequence is com
+0000cf80: 706c 6574 652c 2062 7920 6465 6661 756c  plete, by defaul
+0000cf90: 7420 4661 6c73 652e 0d0a 0d0a 2020 2020  t False.....    
+0000cfa0: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+0000cfb0: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+0000cfc0: 2020 2020 2020 5468 7265 6164 0d0a 2020        Thread..  
+0000cfd0: 2020 2020 2020 2020 2020 5468 6520 7468            The th
+0000cfe0: 7265 6164 2074 6865 2073 6571 7565 6e63  read the sequenc
+0000cff0: 6520 6973 2072 756e 6e69 6e67 206f 6e2e  e is running on.
+0000d000: 2020 5573 6520 6074 6872 6561 642e 6a6f    Use `thread.jo
+0000d010: 696e 2829 6020 746f 2062 6c6f 636b 2075  in()` to block u
+0000d020: 6e74 696c 0d0a 2020 2020 2020 2020 2020  ntil..          
+0000d030: 2020 646f 6e65 2c20 6f72 2060 7468 7265    done, or `thre
+0000d040: 6164 2e69 735f 616c 6976 6528 2960 2074  ad.is_alive()` t
+0000d050: 6f20 6368 6563 6b20 6966 2074 6865 2073  o check if the s
+0000d060: 6571 7565 6e63 6520 6973 2063 6f6d 706c  equence is compl
+0000d070: 6574 652e 0d0a 2020 2020 2020 2020 2222  ete...        ""
+0000d080: 220d 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+0000d090: 6c66 2e6d 6461 2e69 735f 7275 6e6e 696e  lf.mda.is_runnin
+0000d0a0: 6728 293a 0d0a 2020 2020 2020 2020 2020  g():..          
+0000d0b0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000d0c0: 6f72 280d 0a20 2020 2020 2020 2020 2020  or(..           
+0000d0d0: 2020 2020 2022 4361 6e6e 6f74 2073 7461       "Cannot sta
+0000d0e0: 7274 2061 6e20 4d44 4120 7768 696c 6520  rt an MDA while 
+0000d0f0: 7468 6520 7072 6576 696f 7573 204d 4441  the previous MDA
+0000d100: 2069 7320 7374 696c 6c20 7275 6e6e 696e   is still runnin
+0000d110: 672e 220d 0a20 2020 2020 2020 2020 2020  g."..           
+0000d120: 2029 0d0a 2020 2020 2020 2020 7468 203d   )..        th =
+0000d130: 2054 6872 6561 6428 7461 7267 6574 3d73   Thread(target=s
+0000d140: 656c 662e 6d64 612e 7275 6e2c 2061 7267  elf.mda.run, arg
+0000d150: 733d 2865 7665 6e74 732c 2929 0d0a 2020  s=(events,))..  
+0000d160: 2020 2020 2020 7468 2e73 7461 7274 2829        th.start()
+0000d170: 0d0a 2020 2020 2020 2020 6966 2062 6c6f  ..        if blo
+0000d180: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000d190: 2074 682e 6a6f 696e 2829 0d0a 2020 2020   th.join()..    
+0000d1a0: 2020 2020 7265 7475 726e 2074 680d 0a0d      return th...
+0000d1b0: 0a20 2020 2064 6566 2072 6567 6973 7465  .    def registe
+0000d1c0: 725f 6d64 615f 656e 6769 6e65 2873 656c  r_mda_engine(sel
+0000d1d0: 662c 2065 6e67 696e 653a 2050 4d44 4145  f, engine: PMDAE
+0000d1e0: 6e67 696e 6529 202d 3e20 4e6f 6e65 3a0d  ngine) -> None:.
+0000d1f0: 0a20 2020 2020 2020 2022 2222 5365 7420  .        """Set 
+0000d200: 7468 6520 4d44 4120 456e 6769 6e65 2074  the MDA Engine t
+0000d210: 6f20 6265 2075 7365 6420 6f6e 2060 7275  o be used on `ru
+0000d220: 6e5f 6d64 6160 2e0d 0a0d 0a20 2020 2020  n_mda`.....     
+0000d230: 2020 203a 7370 6172 6b6c 6573 3a20 2a54     :sparkles: *T
+0000d240: 6869 7320 6d65 7468 6f64 2069 7320 6e65  his method is ne
+0000d250: 7720 696e 2060 434d 4d43 6f72 6550 6c75  w in `CMMCorePlu
+0000d260: 7360 2e2a 0d0a 0d0a 2020 2020 2020 2020  s`.*....        
+0000d270: 5468 6973 2077 696c 6c20 756e 7265 6769  This will unregi
+0000d280: 7374 6572 2074 6865 2070 7265 7669 6f75  ster the previou
+0000d290: 7320 656e 6769 6e65 2061 6e64 2065 6d69  s engine and emi
+0000d2a0: 7420 616e 2060 6d64 6145 6e67 696e 6552  t an `mdaEngineR
+0000d2b0: 6567 6973 7465 7265 6460 0d0a 2020 2020  egistered`..    
+0000d2c0: 2020 2020 7369 676e 616c 2e20 5468 6520      signal. The 
+0000d2d0: 6375 7272 656e 7420 456e 6769 6e65 206d  current Engine m
+0000d2e0: 7573 7420 6e6f 7420 6265 2072 756e 6e69  ust not be runni
+0000d2f0: 6e67 2061 6e20 4d44 4120 696e 206f 7264  ng an MDA in ord
+0000d300: 6572 2074 6f20 7265 6769 7374 6572 2061  er to register a
+0000d310: 206e 6577 0d0a 2020 2020 2020 2020 656e   new..        en
+0000d320: 6769 6e65 2e0d 0a0d 0a20 2020 2020 2020  gine.....       
+0000d330: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+0000d340: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+0000d350: 0a20 2020 2020 2020 2065 6e67 696e 6520  .        engine 
+0000d360: 3a20 504d 4441 456e 6769 6e65 0d0a 2020  : PMDAEngine..  
+0000d370: 2020 2020 2020 2020 2020 416e 7920 6f62            Any ob
+0000d380: 6a65 6374 2063 6f6e 666f 726d 696e 6720  ject conforming 
+0000d390: 746f 2074 6865 2050 4d44 4145 6e67 696e  to the PMDAEngin
+0000d3a0: 6520 7072 6f74 6f63 6f6c 2e0d 0a20 2020  e protocol...   
+0000d3b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000d3c0: 2020 6f6c 645f 656e 6769 6e65 203d 2073    old_engine = s
+0000d3d0: 656c 662e 6d64 612e 7365 745f 656e 6769  elf.mda.set_engi
+0000d3e0: 6e65 2865 6e67 696e 6529 0d0a 2020 2020  ne(engine)..    
+0000d3f0: 2020 2020 7365 6c66 2e65 7665 6e74 732e      self.events.
+0000d400: 6d64 6145 6e67 696e 6552 6567 6973 7465  mdaEngineRegiste
+0000d410: 7265 642e 656d 6974 2865 6e67 696e 652c  red.emit(engine,
+0000d420: 206f 6c64 5f65 6e67 696e 6529 0d0a 0d0a   old_engine)....
+0000d430: 2020 2020 6465 6620 6669 7849 6d61 6765      def fixImage
+0000d440: 2873 656c 662c 2069 6d67 3a20 6e70 2e6e  (self, img: np.n
+0000d450: 6461 7272 6179 2c20 6e63 6f6d 706f 6e65  darray, ncompone
+0000d460: 6e74 733a 2069 6e74 207c 204e 6f6e 6520  nts: int | None 
+0000d470: 3d20 4e6f 6e65 2920 2d3e 206e 702e 6e64  = None) -> np.nd
+0000d480: 6172 7261 793a 0d0a 2020 2020 2020 2020  array:..        
+0000d490: 2222 2246 6978 2069 6d67 2073 6861 7065  """Fix img shape
+0000d4a0: 2f64 7479 7065 2062 6173 6564 206f 6e20  /dtype based on 
+0000d4b0: 6073 656c 662e 6765 744e 756d 6265 724f  `self.getNumberO
+0000d4c0: 6643 6f6d 706f 6e65 6e74 7328 2960 2e0d  fComponents()`..
+0000d4d0: 0a0d 0a20 2020 2020 2020 203a 7370 6172  ...        :spar
+0000d4e0: 6b6c 6573 3a20 2a54 6869 7320 6d65 7468  kles: *This meth
+0000d4f0: 6f64 2069 7320 6e65 7720 696e 2060 434d  od is new in `CM
+0000d500: 4d43 6f72 6550 6c75 7360 2e2a 0d0a 0d0a  MCorePlus`.*....
+0000d510: 2020 2020 2020 2020 636f 6e76 6572 7420          convert 
+0000d520: 696d 6167 6573 2077 6974 6820 6e5f 636f  images with n_co
+0000d530: 6d70 6f6e 656e 7473 203e 2031 0d0a 2020  mponents > 1..  
+0000d540: 2020 2020 2020 746f 2061 2073 6861 7065        to a shape
+0000d550: 2028 772c 2068 2c20 6e75 6d5f 636f 6d70   (w, h, num_comp
+0000d560: 6f6e 656e 7473 2920 616e 6420 6474 7970  onents) and dtyp
+0000d570: 6520 6069 6d67 2e64 7479 7065 2e69 7465  e `img.dtype.ite
+0000d580: 6d73 697a 652f 2f6e 636f 6d70 600d 0a0d  msize//ncomp`...
+0000d590: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000d5a0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+0000d5b0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+0000d5c0: 2069 6d67 203a 206e 702e 6e64 6172 7261   img : np.ndarra
+0000d5d0: 790d 0a20 2020 2020 2020 2020 2020 2069  y..            i
+0000d5e0: 6e70 7574 2069 6d61 6765 0d0a 2020 2020  nput image..    
+0000d5f0: 2020 2020 6e63 6f6d 706f 6e65 6e74 7320      ncomponents 
+0000d600: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
+0000d610: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+0000d620: 6265 7220 6f66 2063 6f6d 706f 6e65 6e74  ber of component
+0000d630: 7320 696e 2074 6865 2069 6d61 6765 2c20  s in the image, 
+0000d640: 6279 2064 6566 6175 6c74 2060 7365 6c66  by default `self
+0000d650: 2e67 6574 4e75 6d62 6572 4f66 436f 6d70  .getNumberOfComp
+0000d660: 6f6e 656e 7473 2829 600d 0a0d 0a20 2020  onents()`....   
+0000d670: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+0000d680: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+0000d690: 2020 2020 2020 206e 702e 6e64 6172 7261         np.ndarra
+0000d6a0: 790d 0a20 2020 2020 2020 2020 2020 206f  y..            o
+0000d6b0: 7574 7075 7420 696d 6167 6520 2870 6f73  utput image (pos
+0000d6c0: 7369 626c 7920 6e65 7720 7368 6170 6520  sibly new shape 
+0000d6d0: 616e 6420 6474 7970 6529 0d0a 2020 2020  and dtype)..    
+0000d6e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000d6f0: 2069 6620 6e63 6f6d 706f 6e65 6e74 7320   if ncomponents 
+0000d700: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+0000d710: 2020 2020 2020 6e63 6f6d 706f 6e65 6e74        ncomponent
+0000d720: 7320 3d20 7365 6c66 2e67 6574 4e75 6d62  s = self.getNumb
+0000d730: 6572 4f66 436f 6d70 6f6e 656e 7473 2829  erOfComponents()
+0000d740: 0d0a 2020 2020 2020 2020 6966 206e 636f  ..        if nco
+0000d750: 6d70 6f6e 656e 7473 203d 3d20 343a 0d0a  mponents == 4:..
+0000d760: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000d770: 7368 6170 6520 3d20 282a 696d 672e 7368  shape = (*img.sh
+0000d780: 6170 652c 2034 290d 0a20 2020 2020 2020  ape, 4)..       
+0000d790: 2020 2020 2069 6d67 203d 2069 6d67 2e76       img = img.v
+0000d7a0: 6965 7728 6474 7970 653d 6622 757b 696d  iew(dtype=f"u{im
+0000d7b0: 672e 6474 7970 652e 6974 656d 7369 7a65  g.dtype.itemsize
+0000d7c0: 2f2f 347d 2229 0d0a 2020 2020 2020 2020  //4}")..        
+0000d7d0: 2020 2020 696d 6720 3d20 696d 672e 7265      img = img.re
+0000d7e0: 7368 6170 6528 6e65 775f 7368 6170 6529  shape(new_shape)
+0000d7f0: 5b3a 2c20 3a2c 2028 322c 2031 2c20 302c  [:, :, (2, 1, 0,
+0000d800: 2033 295d 2020 2320 6d6d 636f 7265 2067   3)]  # mmcore g
+0000d810: 6976 6573 2062 6772 610d 0a20 2020 2020  ives bgra..     
+0000d820: 2020 2072 6574 7572 6e20 696d 670d 0a0d     return img...
+0000d830: 0a20 2020 2064 6566 2073 6e61 7028 7365  .    def snap(se
+0000d840: 6c66 2c20 6e75 6d43 6861 6e6e 656c 3a20  lf, numChannel: 
+0000d850: 696e 7420 7c20 4e6f 6e65 203d 204e 6f6e  int | None = Non
+0000d860: 652c 202a 2c20 6669 783a 2062 6f6f 6c20  e, *, fix: bool 
+0000d870: 3d20 5472 7565 2920 2d3e 206e 702e 6e64  = True) -> np.nd
+0000d880: 6172 7261 793a 0d0a 2020 2020 2020 2020  array:..        
+0000d890: 2222 2253 6e61 7020 616e 6420 7265 7475  """Snap and retu
+0000d8a0: 726e 2061 6e20 696d 6167 652e 0d0a 0d0a  rn an image.....
+0000d8b0: 2020 2020 2020 2020 3a73 7061 726b 6c65          :sparkle
+0000d8c0: 733a 202a 5468 6973 206d 6574 686f 6420  s: *This method 
+0000d8d0: 6973 206e 6577 2069 6e20 6043 4d4d 436f  is new in `CMMCo
+0000d8e0: 7265 506c 7573 602e 2a0d 0a0d 0a20 2020  rePlus`.*....   
+0000d8f0: 2020 2020 2043 6f6e 7665 6e69 656e 6365       Convenience
+0000d900: 2066 6f72 2063 616c 6c69 6e67 2060 7365   for calling `se
+0000d910: 6c66 2e73 6e61 7049 6d61 6765 2829 6020  lf.snapImage()` 
+0000d920: 666f 6c6c 6f77 6564 2062 7920 7265 7475  followed by retu
+0000d930: 726e 696e 6720 7468 6520 7661 6c75 650d  rning the value.
+0000d940: 0a20 2020 2020 2020 206f 6620 6073 656c  .        of `sel
+0000d950: 662e 6765 7449 6d61 6765 2829 602e 0d0a  f.getImage()`...
+0000d960: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000d970: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+0000d980: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+0000d990: 2020 6e75 6d43 6861 6e6e 656c 203a 2069    numChannel : i
+0000d9a0: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+0000d9b0: 2020 2020 2020 2020 2020 5468 6520 6361            The ca
+0000d9c0: 6d65 7261 2063 6861 6e6e 656c 2074 6f20  mera channel to 
+0000d9d0: 6765 7420 7468 6520 696d 6167 6520 6672  get the image fr
+0000d9e0: 6f6d 2e20 2049 6620 4e6f 6e65 2c20 2874  om.  If None, (t
+0000d9f0: 6865 2064 6566 6175 6c74 292c 2074 6865  he default), the
+0000da00: 6e0d 0a20 2020 2020 2020 2020 2020 204d  n..            M
+0000da10: 756c 7469 2d43 6861 6e6e 656c 2063 616d  ulti-Channel cam
+0000da20: 6572 6173 2077 696c 6c20 7265 7475 726e  eras will return
+0000da30: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
+0000da40: 7468 6520 6669 7273 7420 6368 616e 6e65  the first channe
+0000da50: 6c2e 0d0a 2020 2020 2020 2020 6669 7820  l...        fix 
+0000da60: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
+0000da70: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+0000da80: 2020 2049 6620 6054 7275 6560 2028 7468     If `True` (th
+0000da90: 6520 6465 6661 756c 7429 2c20 7468 656e  e default), then
+0000daa0: 2069 6d61 6765 7320 7769 7468 206e 5f63   images with n_c
+0000dab0: 6f6d 706f 6e65 6e74 7320 3e20 3120 286c  omponents > 1 (l
+0000dac0: 696b 6520 5247 4220 696d 6167 6573 290d  ike RGB images).
+0000dad0: 0a20 2020 2020 2020 2020 2020 2077 696c  .            wil
+0000dae0: 6c20 6265 2072 6573 6861 7065 6420 746f  l be reshaped to
+0000daf0: 2028 772c 2068 2c20 6e5f 636f 6d70 6f6e   (w, h, n_compon
+0000db00: 656e 7473 2920 7573 696e 6720 6066 6978  ents) using `fix
+0000db10: 496d 6167 6560 2e0d 0a0d 0a20 2020 2020  Image`.....     
+0000db20: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+0000db30: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+0000db40: 2020 2020 2069 6d67 203a 206e 702e 6e64       img : np.nd
+0000db50: 6172 7261 790d 0a20 2020 2020 2020 2022  array..        "
+0000db60: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+0000db70: 2e73 6e61 7049 6d61 6765 2829 0d0a 2020  .snapImage()..  
+0000db80: 2020 2020 2020 696d 6720 3d20 7365 6c66        img = self
+0000db90: 2e67 6574 496d 6167 6528 6e75 6d43 6861  .getImage(numCha
+0000dba0: 6e6e 656c 2c20 6669 783d 6669 7829 2020  nnel, fix=fix)  
+0000dbb0: 2320 7479 7065 3a20 6967 6e6f 7265 0d0a  # type: ignore..
+0000dbc0: 2020 2020 2020 2020 7365 6c66 2e65 7665          self.eve
+0000dbd0: 6e74 732e 696d 6167 6553 6e61 7070 6564  nts.imageSnapped
+0000dbe0: 2e65 6d69 7428 696d 6729 0d0a 2020 2020  .emit(img)..    
+0000dbf0: 2020 2020 7265 7475 726e 2069 6d67 0d0a      return img..
+0000dc00: 0d0a 2020 2020 406f 7665 726c 6f61 640d  ..    @overload.
+0000dc10: 0a20 2020 2064 6566 2067 6574 496d 6167  .    def getImag
+0000dc20: 6528 7365 6c66 2c20 2a2c 2066 6978 3a20  e(self, *, fix: 
+0000dc30: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
+0000dc40: 6e70 2e6e 6461 7272 6179 3a20 2023 206e  np.ndarray:  # n
+0000dc50: 6f71 613a 2044 3431 380d 0a20 2020 2020  oqa: D418..     
+0000dc60: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+0000dc70: 2069 6e74 6572 6e61 6c20 696d 6167 6520   internal image 
+0000dc80: 6275 6666 6572 2e22 2222 0d0a 0d0a 2020  buffer."""....  
+0000dc90: 2020 406f 7665 726c 6f61 640d 0a20 2020    @overload..   
+0000dca0: 2064 6566 2067 6574 496d 6167 6528 7365   def getImage(se
+0000dcb0: 6c66 2c20 6e75 6d43 6861 6e6e 656c 3a20  lf, numChannel: 
+0000dcc0: 696e 742c 202a 2c20 6669 783a 2062 6f6f  int, *, fix: boo
+0000dcd0: 6c20 3d20 5472 7565 2920 2d3e 206e 702e  l = True) -> np.
+0000dce0: 6e64 6172 7261 793a 2020 2320 6e6f 7161  ndarray:  # noqa
+0000dcf0: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+0000dd00: 7572 6e20 7468 6520 696e 7465 726e 616c  urn the internal
+0000dd10: 2069 6d61 6765 2062 7566 6665 7220 666f   image buffer fo
+0000dd20: 7220 6120 6769 7665 6e20 4361 6d65 7261  r a given Camera
+0000dd30: 2043 6861 6e6e 656c 2e22 2222 0d0a 0d0a   Channel."""....
+0000dd40: 2020 2020 6465 6620 6765 7449 6d61 6765      def getImage
+0000dd50: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
+0000dd60: 206e 756d 4368 616e 6e65 6c3a 2069 6e74   numChannel: int
+0000dd70: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c20   | None = None, 
+0000dd80: 2a2c 2066 6978 3a20 626f 6f6c 203d 2054  *, fix: bool = T
+0000dd90: 7275 650d 0a20 2020 2029 202d 3e20 6e70  rue..    ) -> np
+0000dda0: 2e6e 6461 7272 6179 3a0d 0a20 2020 2020  .ndarray:..     
+0000ddb0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+0000ddc0: 2069 6e74 6572 6e61 6c20 696d 6167 6520   internal image 
+0000ddd0: 6275 6666 6572 2e0d 0a0d 0a20 2020 2020  buffer.....     
+0000dde0: 2020 202a 2a57 6879 204f 7665 7272 6964     **Why Overrid
+0000ddf0: 653f 2a2a 2054 6f20 6669 7820 7468 6520  e?** To fix the 
+0000de00: 7368 6170 6520 6f66 2069 6d61 6765 7320  shape of images 
+0000de10: 7769 7468 206e 5f63 6f6d 706f 6e65 6e74  with n_component
+0000de20: 7320 3e20 3120 286c 696b 6520 5247 420d  s > 1 (like RGB.
+0000de30: 0a20 2020 2020 2020 2069 6d61 6765 7329  .        images)
+0000de40: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+0000de50: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+0000de60: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+0000de70: 2020 2020 6e75 6d43 6861 6e6e 656c 203a      numChannel :
+0000de80: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
+0000de90: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000dea0: 6361 6d65 7261 2063 6861 6e6e 656c 2074  camera channel t
+0000deb0: 6f20 6765 7420 7468 6520 696d 6167 6520  o get the image 
+0000dec0: 6672 6f6d 2e20 2049 6620 4e6f 6e65 2c20  from.  If None, 
+0000ded0: 2874 6865 2064 6566 6175 6c74 292c 2074  (the default), t
+0000dee0: 6865 6e0d 0a20 2020 2020 2020 2020 2020  hen..           
+0000def0: 204d 756c 7469 2d43 6861 6e6e 656c 2063   Multi-Channel c
+0000df00: 616d 6572 6173 2077 696c 6c20 7265 7475  ameras will retu
+0000df10: 726e 2074 6865 2063 6f6e 7465 6e74 206f  rn the content o
+0000df20: 6620 7468 6520 6669 7273 7420 6368 616e  f the first chan
+0000df30: 6e65 6c2e 0d0a 2020 2020 2020 2020 6669  nel...        fi
+0000df40: 7820 3a20 626f 6f6c 2c20 6465 6661 756c  x : bool, defaul
+0000df50: 743a 2054 7275 650d 0a20 2020 2020 2020  t: True..       
+0000df60: 2020 2020 2049 6620 6054 7275 6560 2028       If `True` (
+0000df70: 7468 6520 6465 6661 756c 7429 2c20 7468  the default), th
+0000df80: 656e 2069 6d61 6765 7320 7769 7468 206e  en images with n
+0000df90: 5f63 6f6d 706f 6e65 6e74 7320 3e20 3120  _components > 1 
+0000dfa0: 286c 696b 6520 5247 4220 696d 6167 6573  (like RGB images
+0000dfb0: 290d 0a20 2020 2020 2020 2020 2020 2077  )..            w
+0000dfc0: 696c 6c20 6265 2072 6573 6861 7065 6420  ill be reshaped 
+0000dfd0: 746f 2028 772c 2068 2c20 6e5f 636f 6d70  to (w, h, n_comp
+0000dfe0: 6f6e 656e 7473 2920 7573 696e 6720 6066  onents) using `f
+0000dff0: 6978 496d 6167 6560 2e0d 0a20 2020 2020  ixImage`...     
+0000e000: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000e010: 696d 6720 3d20 280d 0a20 2020 2020 2020  img = (..       
+0000e020: 2020 2020 2073 7570 6572 2829 2e67 6574       super().get
+0000e030: 496d 6167 6528 6e75 6d43 6861 6e6e 656c  Image(numChannel
+0000e040: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000e050: 6620 6e75 6d43 6861 6e6e 656c 2069 7320  f numChannel is 
+0000e060: 6e6f 7420 4e6f 6e65 0d0a 2020 2020 2020  not None..      
+0000e070: 2020 2020 2020 656c 7365 2073 7570 6572        else super
+0000e080: 2829 2e67 6574 496d 6167 6528 290d 0a20  ().getImage().. 
+0000e090: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000e0a0: 2020 7265 7475 726e 2073 656c 662e 6669    return self.fi
+0000e0b0: 7849 6d61 6765 2869 6d67 2920 6966 2066  xImage(img) if f
+0000e0c0: 6978 2065 6c73 6520 696d 670d 0a0d 0a20  ix else img.... 
+0000e0d0: 2020 2064 6566 2073 7461 7274 436f 6e74     def startCont
+0000e0e0: 696e 756f 7573 5365 7175 656e 6365 4163  inuousSequenceAc
+0000e0f0: 7175 6973 6974 696f 6e28 7365 6c66 2c20  quisition(self, 
+0000e100: 696e 7465 7276 616c 4d73 3a20 666c 6f61  intervalMs: floa
+0000e110: 7420 3d20 3029 202d 3e20 4e6f 6e65 3a0d  t = 0) -> None:.
+0000e120: 0a20 2020 2020 2020 2022 2222 5374 6172  .        """Star
+0000e130: 7420 6120 436f 6e74 696e 756f 7573 5365  t a ContinuousSe
+0000e140: 7175 656e 6365 4163 7175 6973 6974 696f  quenceAcquisitio
+0000e150: 6e2e 0d0a 0d0a 2020 2020 2020 2020 2a2a  n.....        **
+0000e160: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
+0000e170: 546f 2065 6d69 7420 6120 6073 7461 7274  To emit a `start
+0000e180: 436f 6e74 696e 756f 7573 5365 7175 656e  ContinuousSequen
+0000e190: 6365 4163 7175 6973 6974 696f 6e60 2065  ceAcquisition` e
+0000e1a0: 7665 6e74 2e0d 0a20 2020 2020 2020 2022  vent...        "
+0000e1b0: 2222 0d0a 2020 2020 2020 2020 7375 7065  ""..        supe
+0000e1c0: 7228 292e 7374 6172 7443 6f6e 7469 6e75  r().startContinu
+0000e1d0: 6f75 7353 6571 7565 6e63 6541 6371 7569  ousSequenceAcqui
+0000e1e0: 7369 7469 6f6e 2869 6e74 6572 7661 6c4d  sition(intervalM
+0000e1f0: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
+0000e200: 2e65 7665 6e74 732e 636f 6e74 696e 756f  .events.continuo
+0000e210: 7573 5365 7175 656e 6365 4163 7175 6973  usSequenceAcquis
+0000e220: 6974 696f 6e53 7461 7274 6564 2e65 6d69  itionStarted.emi
+0000e230: 7428 290d 0a0d 0a20 2020 2040 6f76 6572  t()....    @over
+0000e240: 6c6f 6164 0d0a 2020 2020 6465 6620 7374  load..    def st
+0000e250: 6172 7453 6571 7565 6e63 6541 6371 7569  artSequenceAcqui
+0000e260: 7369 7469 6f6e 280d 0a20 2020 2020 2020  sition(..       
+0000e270: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+0000e280: 6e75 6d49 6d61 6765 733a 2069 6e74 2c0d  numImages: int,.
+0000e290: 0a20 2020 2020 2020 2069 6e74 6572 7661  .        interva
+0000e2a0: 6c4d 733a 2066 6c6f 6174 2c0d 0a20 2020  lMs: float,..   
+0000e2b0: 2020 2020 2073 746f 704f 6e4f 7665 7266       stopOnOverf
+0000e2c0: 6c6f 773a 2062 6f6f 6c2c 0d0a 2020 2020  low: bool,..    
+0000e2d0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+0000e2e0: 2020 2020 2e2e 2e0d 0a0d 0a20 2020 2040      .......    @
+0000e2f0: 6f76 6572 6c6f 6164 0d0a 2020 2020 6465  overload..    de
+0000e300: 6620 7374 6172 7453 6571 7565 6e63 6541  f startSequenceA
+0000e310: 6371 7569 7369 7469 6f6e 280d 0a20 2020  cquisition(..   
+0000e320: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+0000e330: 2020 2020 6361 6d65 7261 4c61 6265 6c3a      cameraLabel:
+0000e340: 2073 7472 2c0d 0a20 2020 2020 2020 206e   str,..        n
+0000e350: 756d 496d 6167 6573 3a20 696e 742c 0d0a  umImages: int,..
+0000e360: 2020 2020 2020 2020 696e 7465 7276 616c          interval
+0000e370: 4d73 3a20 666c 6f61 742c 0d0a 2020 2020  Ms: float,..    
+0000e380: 2020 2020 7374 6f70 4f6e 4f76 6572 666c      stopOnOverfl
+0000e390: 6f77 3a20 626f 6f6c 2c0d 0a20 2020 2029  ow: bool,..    )
+0000e3a0: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+0000e3b0: 2020 202e 2e2e 0d0a 0d0a 2020 2020 6465     .......    de
+0000e3c0: 6620 7374 6172 7453 6571 7565 6e63 6541  f startSequenceA
+0000e3d0: 6371 7569 7369 7469 6f6e 2873 656c 662c  cquisition(self,
+0000e3e0: 202a 6172 6773 3a20 416e 792c 202a 2a6b   *args: Any, **k
+0000e3f0: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
+0000e400: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
+0000e410: 2253 7461 7274 7320 7374 7265 616d 696e  "Starts streamin
+0000e420: 6720 6361 6d65 7261 2073 6571 7565 6e63  g camera sequenc
+0000e430: 6520 6163 7175 6973 6974 696f 6e2e 0d0a  e acquisition...
+0000e440: 0d0a 2020 2020 2020 2020 5468 6973 2063  ..        This c
+0000e450: 6f6d 6d61 6e64 2064 6f65 7320 6e6f 7420  ommand does not 
+0000e460: 626c 6f63 6b20 7468 6520 6361 6c6c 696e  block the callin
+0000e470: 6720 7468 7265 6164 2066 6f72 2074 6865  g thread for the
+0000e480: 2064 7572 6174 696f 6e20 6f66 2074 6865   duration of the
+0000e490: 0d0a 2020 2020 2020 2020 6163 7175 6973  ..        acquis
+0000e4a0: 6974 696f 6e2e 0d0a 0d0a 2020 2020 2020  ition.....      
+0000e4b0: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
+0000e4c0: 3f2a 2a20 546f 2065 6d69 7420 6120 6073  ?** To emit a `s
+0000e4d0: 7461 7274 5365 7175 656e 6365 4163 7175  tartSequenceAcqu
+0000e4e0: 6973 6974 696f 6e60 2065 7665 6e74 2e0d  isition` event..
+0000e4f0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000e500: 2020 2020 2020 7375 7065 7228 292e 7374        super().st
+0000e510: 6172 7453 6571 7565 6e63 6541 6371 7569  artSequenceAcqui
+0000e520: 7369 7469 6f6e 282a 6172 6773 2c20 2a2a  sition(*args, **
+0000e530: 6b77 6172 6773 290d 0a20 2020 2020 2020  kwargs)..       
+0000e540: 2069 6620 6c65 6e28 6172 6773 2920 3d3d   if len(args) ==
+0000e550: 2033 3a0d 0a20 2020 2020 2020 2020 2020   3:..           
+0000e560: 206e 756d 496d 6167 6573 2c20 696e 7465   numImages, inte
+0000e570: 7276 616c 4d73 2c20 7374 6f70 4f6e 4f76  rvalMs, stopOnOv
+0000e580: 6572 666c 6f77 203d 2061 7267 730d 0a20  erflow = args.. 
+0000e590: 2020 2020 2020 2020 2020 2063 616d 6572             camer
+0000e5a0: 614c 6162 656c 203d 2073 7570 6572 2829  aLabel = super()
+0000e5b0: 2e67 6574 4361 6d65 7261 4465 7669 6365  .getCameraDevice
+0000e5c0: 2829 0d0a 2020 2020 2020 2020 656c 7365  ()..        else
+0000e5d0: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+0000e5e0: 616d 6572 614c 6162 656c 2c20 6e75 6d49  ameraLabel, numI
+0000e5f0: 6d61 6765 732c 2069 6e74 6572 7661 6c4d  mages, intervalM
+0000e600: 732c 2073 746f 704f 6e4f 7665 7266 6c6f  s, stopOnOverflo
+0000e610: 7720 3d20 6172 6773 0d0a 2020 2020 2020  w = args..      
+0000e620: 2020 7365 6c66 2e65 7665 6e74 732e 7365    self.events.se
+0000e630: 7175 656e 6365 4163 7175 6973 6974 696f  quenceAcquisitio
+0000e640: 6e53 7461 7274 6564 2e65 6d69 7428 0d0a  nStarted.emit(..
+0000e650: 2020 2020 2020 2020 2020 2020 6361 6d65              came
+0000e660: 7261 4c61 6265 6c2c 206e 756d 496d 6167  raLabel, numImag
+0000e670: 6573 2c20 696e 7465 7276 616c 4d73 2c20  es, intervalMs, 
+0000e680: 7374 6f70 4f6e 4f76 6572 666c 6f77 0d0a  stopOnOverflow..
+0000e690: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+0000e6a0: 2064 6566 2073 746f 7053 6571 7565 6e63   def stopSequenc
+0000e6b0: 6541 6371 7569 7369 7469 6f6e 2873 656c  eAcquisition(sel
+0000e6c0: 662c 2063 616d 6572 614c 6162 656c 3a20  f, cameraLabel: 
+0000e6d0: 7374 7220 7c20 4e6f 6e65 203d 204e 6f6e  str | None = Non
+0000e6e0: 6529 202d 3e20 4e6f 6e65 3a0d 0a20 2020  e) -> None:..   
+0000e6f0: 2020 2020 2022 2222 5374 6f70 7320 7374       """Stops st
+0000e700: 7265 616d 696e 6720 6361 6d65 7261 2073  reaming camera s
+0000e710: 6571 7565 6e63 6520 6163 7175 6973 6974  equence acquisit
+0000e720: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
+0000e730: 2866 6f72 2061 2073 7065 6369 6669 6564  (for a specified
+0000e740: 2063 616d 6572 6120 6966 2060 6361 6d65   camera if `came
+0000e750: 7261 4c61 6265 6c60 2069 7320 7072 6f76  raLabel` is prov
+0000e760: 6964 6564 2e29 0d0a 0d0a 2020 2020 2020  ided.)....      
+0000e770: 2020 2a2a 5768 7920 4f76 6572 7269 6465    **Why Override
+0000e780: 3f2a 2a20 546f 2065 6d69 7420 6120 6073  ?** To emit a `s
+0000e790: 746f 7053 6571 7565 6e63 6541 6371 7569  topSequenceAcqui
+0000e7a0: 7369 7469 6f6e 6020 6576 656e 742e 0d0a  sition` event...
+0000e7b0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0000e7c0: 2020 2020 2069 6620 6361 6d65 7261 4c61       if cameraLa
+0000e7d0: 6265 6c20 6973 204e 6f6e 653a 0d0a 2020  bel is None:..  
+0000e7e0: 2020 2020 2020 2020 2020 7375 7065 7228            super(
+0000e7f0: 292e 7374 6f70 5365 7175 656e 6365 4163  ).stopSequenceAc
+0000e800: 7175 6973 6974 696f 6e28 290d 0a20 2020  quisition()..   
+0000e810: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000e820: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+0000e830: 7374 6f70 5365 7175 656e 6365 4163 7175  stopSequenceAcqu
+0000e840: 6973 6974 696f 6e28 6361 6d65 7261 4c61  isition(cameraLa
+0000e850: 6265 6c29 0d0a 2020 2020 2020 2020 6361  bel)..        ca
+0000e860: 6d65 7261 4c61 6265 6c20 3d20 6361 6d65  meraLabel = came
+0000e870: 7261 4c61 6265 6c20 6f72 2073 7570 6572  raLabel or super
+0000e880: 2829 2e67 6574 4361 6d65 7261 4465 7669  ().getCameraDevi
+0000e890: 6365 2829 0d0a 2020 2020 2020 2020 7365  ce()..        se
+0000e8a0: 6c66 2e65 7665 6e74 732e 7365 7175 656e  lf.events.sequen
+0000e8b0: 6365 4163 7175 6973 6974 696f 6e53 746f  ceAcquisitionSto
+0000e8c0: 7070 6564 2e65 6d69 7428 6361 6d65 7261  pped.emit(camera
+0000e8d0: 4c61 6265 6c29 0d0a 0d0a 2020 2020 6465  Label)....    de
+0000e8e0: 6620 7365 7441 7574 6f53 6875 7474 6572  f setAutoShutter
+0000e8f0: 2873 656c 662c 2073 7461 7465 3a20 626f  (self, state: bo
+0000e900: 6f6c 2920 2d3e 204e 6f6e 653a 0d0a 2020  ol) -> None:..  
+0000e910: 2020 2020 2020 2222 2253 6574 2073 6875        """Set shu
+0000e920: 7474 6572 2074 6f20 6175 746f 6d61 7469  tter to automati
+0000e930: 6361 6c6c 7920 6f70 656e 2061 6e64 2063  cally open and c
+0000e940: 6c6f 7365 2077 6865 6e20 616e 2069 6d61  lose when an ima
+0000e950: 6765 2069 7320 6163 7175 6972 6564 2e0d  ge is acquired..
+0000e960: 0a0d 0a20 2020 2020 2020 202a 2a57 6879  ...        **Why
+0000e970: 204f 7665 7272 6964 653f 2a2a 2054 6f20   Override?** To 
+0000e980: 656d 6974 2061 6e20 6061 7574 6f53 6875  emit an `autoShu
+0000e990: 7474 6572 5365 7460 2065 7665 6e74 2e0d  tterSet` event..
+0000e9a0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000e9b0: 2020 2020 2020 7375 7065 7228 292e 7365        super().se
+0000e9c0: 7441 7574 6f53 6875 7474 6572 2873 7461  tAutoShutter(sta
+0000e9d0: 7465 290d 0a20 2020 2020 2020 2073 656c  te)..        sel
+0000e9e0: 662e 6576 656e 7473 2e61 7574 6f53 6875  f.events.autoShu
+0000e9f0: 7474 6572 5365 742e 656d 6974 2873 7461  tterSet.emit(sta
+0000ea00: 7465 290d 0a0d 0a20 2020 2040 6f76 6572  te)....    @over
+0000ea10: 6c6f 6164 0d0a 2020 2020 6465 6620 7365  load..    def se
+0000ea20: 7453 6875 7474 6572 4f70 656e 2873 656c  tShutterOpen(sel
+0000ea30: 662c 2073 7461 7465 3a20 626f 6f6c 2920  f, state: bool) 
+0000ea40: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+0000ea50: 2020 2e2e 2e0d 0a0d 0a20 2020 2040 6f76    .......    @ov
+0000ea60: 6572 6c6f 6164 0d0a 2020 2020 6465 6620  erload..    def 
+0000ea70: 7365 7453 6875 7474 6572 4f70 656e 2873  setShutterOpen(s
+0000ea80: 656c 662c 2073 6875 7474 6572 4c61 6265  elf, shutterLabe
+0000ea90: 6c3a 2073 7472 2c20 7374 6174 653a 2062  l: str, state: b
+0000eaa0: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0d 0a20  ool) -> None:.. 
+0000eab0: 2020 2020 2020 202e 2e2e 0d0a 0d0a 2020         .......  
+0000eac0: 2020 6465 6620 7365 7453 6875 7474 6572    def setShutter
+0000ead0: 4f70 656e 2873 656c 662c 202a 6172 6773  Open(self, *args
+0000eae0: 3a20 416e 792c 202a 2a6b 7761 7267 733a  : Any, **kwargs:
+0000eaf0: 2041 6e79 2920 2d3e 204e 6f6e 653a 0d0a   Any) -> None:..
+0000eb00: 2020 2020 2020 2020 2222 224f 7065 6e20          """Open 
+0000eb10: 6f72 2063 6c6f 7365 2074 6865 2063 7572  or close the cur
+0000eb20: 7265 6e74 6c79 2073 656c 6563 7465 6420  rently selected 
+0000eb30: 6f72 2060 7368 7574 7465 724c 6162 656c  or `shutterLabel
+0000eb40: 6020 7368 7574 7465 722e 0d0a 0d0a 2020  ` shutter.....  
+0000eb50: 2020 2020 2020 2a2a 5768 7920 4f76 6572        **Why Over
+0000eb60: 7269 6465 3f2a 2a20 546f 2065 6d69 7420  ride?** To emit 
+0000eb70: 6120 6070 726f 7065 7274 7943 6861 6e67  a `propertyChang
+0000eb80: 6564 6020 6576 656e 742e 0d0a 2020 2020  ed` event...    
+0000eb90: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000eba0: 2073 7570 6572 2829 2e73 6574 5368 7574   super().setShut
+0000ebb0: 7465 724f 7065 6e28 2a61 7267 732c 202a  terOpen(*args, *
+0000ebc0: 2a6b 7761 7267 7329 0d0a 2020 2020 2020  *kwargs)..      
+0000ebd0: 2020 7368 7574 7465 724c 6162 656c 2c20    shutterLabel, 
+0000ebe0: 7374 6174 6520 3d20 6b77 6172 6773 2e67  state = kwargs.g
+0000ebf0: 6574 2822 7368 7574 7465 724c 6162 656c  et("shutterLabel
+0000ec00: 2229 2c20 6b77 6172 6773 2e67 6574 2822  "), kwargs.get("
+0000ec10: 7374 6174 6522 290d 0a20 2020 2020 2020  state")..       
+0000ec20: 2069 6620 6c65 6e28 6172 6773 2920 3e20   if len(args) > 
+0000ec30: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+0000ec40: 7368 7574 7465 724c 6162 656c 2c20 7374  shutterLabel, st
+0000ec50: 6174 6520 3d20 6172 6773 0d0a 2020 2020  ate = args..    
+0000ec60: 2020 2020 656c 6966 2061 7267 733a 0d0a      elif args:..
+0000ec70: 2020 2020 2020 2020 2020 2020 7368 7574              shut
+0000ec80: 7465 724c 6162 656c 203d 2073 7570 6572  terLabel = super
+0000ec90: 2829 2e67 6574 5368 7574 7465 7244 6576  ().getShutterDev
+0000eca0: 6963 6528 290d 0a20 2020 2020 2020 2020  ice()..         
+0000ecb0: 2020 2073 7461 7465 203d 2061 7267 730d     state = args.
+0000ecc0: 0a20 2020 2020 2020 2073 656c 662e 6576  .        self.ev
+0000ecd0: 656e 7473 2e70 726f 7065 7274 7943 6861  ents.propertyCha
+0000ece0: 6e67 6564 2e65 6d69 7428 7368 7574 7465  nged.emit(shutte
+0000ecf0: 724c 6162 656c 2c20 2253 7461 7465 222c  rLabel, "State",
+0000ed00: 2073 7461 7465 290d 0a0d 0a20 2020 2040   state)....    @
+0000ed10: 6f76 6572 6c6f 6164 0d0a 2020 2020 6465  overload..    de
+0000ed20: 6620 6465 6c65 7465 436f 6e66 6967 2873  f deleteConfig(s
+0000ed30: 656c 662c 2067 726f 7570 4e61 6d65 3a20  elf, groupName: 
+0000ed40: 7374 722c 2063 6f6e 6669 674e 616d 653a  str, configName:
+0000ed50: 2073 7472 2920 2d3e 204e 6f6e 653a 0d0a   str) -> None:..
+0000ed60: 2020 2020 2020 2020 2e2e 2e0d 0a0d 0a20          ....... 
+0000ed70: 2020 2040 6f76 6572 6c6f 6164 0d0a 2020     @overload..  
+0000ed80: 2020 6465 6620 6465 6c65 7465 436f 6e66    def deleteConf
+0000ed90: 6967 280d 0a20 2020 2020 2020 2073 656c  ig(..        sel
+0000eda0: 662c 2067 726f 7570 4e61 6d65 3a20 7374  f, groupName: st
+0000edb0: 722c 2063 6f6e 6669 674e 616d 653a 2073  r, configName: s
+0000edc0: 7472 2c20 6465 7669 6365 4c61 6265 6c3a  tr, deviceLabel:
+0000edd0: 2073 7472 2c20 7072 6f70 4e61 6d65 3a20   str, propName: 
+0000ede0: 7374 720d 0a20 2020 2029 202d 3e20 4e6f  str..    ) -> No
+0000edf0: 6e65 3a0d 0a20 2020 2020 2020 202e 2e2e  ne:..        ...
+0000ee00: 0d0a 0d0a 2020 2020 6465 6620 6465 6c65  ....    def dele
+0000ee10: 7465 436f 6e66 6967 280d 0a20 2020 2020  teConfig(..     
+0000ee20: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
+0000ee30: 2020 6772 6f75 704e 616d 653a 2073 7472    groupName: str
+0000ee40: 2c0d 0a20 2020 2020 2020 2063 6f6e 6669  ,..        confi
+0000ee50: 674e 616d 653a 2073 7472 2c0d 0a20 2020  gName: str,..   
+0000ee60: 2020 2020 2064 6576 6963 654c 6162 656c       deviceLabel
+0000ee70: 3a20 7374 7220 7c20 4e6f 6e65 203d 204e  : str | None = N
+0000ee80: 6f6e 652c 0d0a 2020 2020 2020 2020 7072  one,..        pr
+0000ee90: 6f70 4e61 6d65 3a20 7374 7220 7c20 4e6f  opName: str | No
+0000eea0: 6e65 203d 204e 6f6e 652c 0d0a 2020 2020  ne = None,..    
+0000eeb0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+0000eec0: 2020 2020 2222 2244 656c 6574 6520 6063      """Delete `c
+0000eed0: 6f6e 6669 674e 616d 6560 2066 726f 6d20  onfigName` from 
+0000eee0: 6067 726f 7570 4e61 6d65 602e 0d0a 0d0a  `groupName`.....
+0000eef0: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
+0000ef00: 6572 7269 6465 3f2a 2a20 546f 2065 6d69  erride?** To emi
+0000ef10: 7420 6120 6063 6f6e 6669 6744 656c 6574  t a `configDelet
+0000ef20: 6564 6020 6576 656e 742e 0d0a 2020 2020  ed` event...    
+0000ef30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000ef40: 2061 7267 733a 2074 7570 6c65 5b73 7472   args: tuple[str
+0000ef50: 2c20 2e2e 2e5d 203d 2028 6772 6f75 704e  , ...] = (groupN
+0000ef60: 616d 652c 2063 6f6e 6669 674e 616d 6529  ame, configName)
+0000ef70: 0d0a 2020 2020 2020 2020 6966 2064 6576  ..        if dev
+0000ef80: 6963 654c 6162 656c 2069 7320 6e6f 7420  iceLabel is not 
+0000ef90: 4e6f 6e65 2061 6e64 2070 726f 704e 616d  None and propNam
+0000efa0: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+0000efb0: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0000efc0: 203d 2028 2a61 7267 732c 2064 6576 6963   = (*args, devic
+0000efd0: 654c 6162 656c 2c20 7072 6f70 4e61 6d65  eLabel, propName
+0000efe0: 290d 0a20 2020 2020 2020 2073 7570 6572  )..        super
+0000eff0: 2829 2e64 656c 6574 6543 6f6e 6669 6728  ().deleteConfig(
+0000f000: 2a61 7267 7329 0d0a 2020 2020 2020 2020  *args)..        
+0000f010: 7365 6c66 2e65 7665 6e74 732e 636f 6e66  self.events.conf
+0000f020: 6967 4465 6c65 7465 642e 656d 6974 2867  igDeleted.emit(g
+0000f030: 726f 7570 4e61 6d65 2c20 636f 6e66 6967  roupName, config
+0000f040: 4e61 6d65 290d 0a0d 0a20 2020 2064 6566  Name)....    def
+0000f050: 2064 656c 6574 6543 6f6e 6669 6747 726f   deleteConfigGro
+0000f060: 7570 2873 656c 662c 2067 726f 7570 3a20  up(self, group: 
+0000f070: 7374 7229 202d 3e20 4e6f 6e65 3a0d 0a20  str) -> None:.. 
+0000f080: 2020 2020 2020 2022 2222 4465 6c65 7465         """Delete
+0000f090: 7320 616e 2065 6e74 6972 6520 636f 6e66  s an entire conf
+0000f0a0: 6967 7572 6174 696f 6e20 6067 726f 7570  iguration `group
+0000f0b0: 602e 0d0a 0d0a 2020 2020 2020 2020 2a2a  `.....        **
+0000f0c0: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
+0000f0d0: 546f 2065 6d69 7420 6120 6063 6f6e 6669  To emit a `confi
+0000f0e0: 6747 726f 7570 4465 6c65 7465 6460 2065  gGroupDeleted` e
+0000f0f0: 7665 6e74 2e0d 0a20 2020 2020 2020 2022  vent...        "
+0000f100: 2222 0d0a 2020 2020 2020 2020 7375 7065  ""..        supe
+0000f110: 7228 292e 6465 6c65 7465 436f 6e66 6967  r().deleteConfig
+0000f120: 4772 6f75 7028 6772 6f75 7029 0d0a 2020  Group(group)..  
+0000f130: 2020 2020 2020 7365 6c66 2e65 7665 6e74        self.event
+0000f140: 732e 636f 6e66 6967 4772 6f75 7044 656c  s.configGroupDel
+0000f150: 6574 6564 2e65 6d69 7428 6772 6f75 7029  eted.emit(group)
+0000f160: 0d0a 0d0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
+0000f170: 640d 0a20 2020 2064 6566 2064 6566 696e  d..    def defin
+0000f180: 6543 6f6e 6669 6728 7365 6c66 2c20 6772  eConfig(self, gr
+0000f190: 6f75 704e 616d 653a 2073 7472 2c20 636f  oupName: str, co
+0000f1a0: 6e66 6967 4e61 6d65 3a20 7374 7229 202d  nfigName: str) -
+0000f1b0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+0000f1c0: 202e 2e2e 0d0a 0d0a 2020 2020 406f 7665   .......    @ove
+0000f1d0: 726c 6f61 640d 0a20 2020 2064 6566 2064  rload..    def d
+0000f1e0: 6566 696e 6543 6f6e 6669 6728 0d0a 2020  efineConfig(..  
+0000f1f0: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+0000f200: 2020 2020 2067 726f 7570 4e61 6d65 3a20       groupName: 
+0000f210: 7374 722c 0d0a 2020 2020 2020 2020 636f  str,..        co
+0000f220: 6e66 6967 4e61 6d65 3a20 7374 722c 0d0a  nfigName: str,..
+0000f230: 2020 2020 2020 2020 6465 7669 6365 4c61          deviceLa
+0000f240: 6265 6c3a 2073 7472 2c0d 0a20 2020 2020  bel: str,..     
+0000f250: 2020 2070 726f 704e 616d 653a 2073 7472     propName: str
+0000f260: 2c0d 0a20 2020 2020 2020 2076 616c 7565  ,..        value
+0000f270: 3a20 7374 722c 0d0a 2020 2020 2920 2d3e  : str,..    ) ->
+0000f280: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000f290: 2e2e 2e0d 0a0d 0a20 2020 2064 6566 2064  .......    def d
+0000f2a0: 6566 696e 6543 6f6e 6669 6728 0d0a 2020  efineConfig(..  
+0000f2b0: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+0000f2c0: 2020 2020 2067 726f 7570 4e61 6d65 3a20       groupName: 
+0000f2d0: 7374 722c 0d0a 2020 2020 2020 2020 636f  str,..        co
+0000f2e0: 6e66 6967 4e61 6d65 3a20 7374 722c 0d0a  nfigName: str,..
+0000f2f0: 2020 2020 2020 2020 6465 7669 6365 4c61          deviceLa
+0000f300: 6265 6c3a 2073 7472 207c 204e 6f6e 6520  bel: str | None 
+0000f310: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+0000f320: 2070 726f 704e 616d 653a 2073 7472 207c   propName: str |
+0000f330: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
+0000f340: 2020 2020 2020 2076 616c 7565 3a20 7374         value: st
+0000f350: 7220 7c20 4e6f 6e65 203d 204e 6f6e 652c  r | None = None,
+0000f360: 0d0a 2020 2020 2920 2d3e 204e 6f6e 653a  ..    ) -> None:
+0000f370: 0d0a 2020 2020 2020 2020 2222 2244 6566  ..        """Def
+0000f380: 696e 6573 2061 2063 6f6e 6669 6775 7261  ines a configura
+0000f390: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
+0000f3a0: 202a 2a57 6879 204f 7665 7272 6964 653f   **Why Override?
+0000f3b0: 2a2a 2054 6f20 656d 6974 2061 2060 636f  ** To emit a `co
+0000f3c0: 6e66 6967 4465 6669 6e65 6460 2065 7665  nfigDefined` eve
+0000f3d0: 6e74 2e20 2041 6c73 6f2c 2069 6620 6067  nt.  Also, if `g
+0000f3e0: 726f 7570 4e61 6d65 6020 6973 0d0a 2020  roupName` is..  
+0000f3f0: 2020 2020 2020 6e6f 7420 6120 6465 6669        not a defi
+0000f400: 6e65 6420 6772 6f75 702c 2074 6865 6e20  ned group, then 
+0000f410: 6064 6566 696e 6543 6f6e 6669 6747 726f  `defineConfigGro
+0000f420: 7570 2867 726f 7570 4e61 6d65 2960 2069  up(groupName)` i
+0000f430: 7320 6361 6c6c 6564 2e0d 0a20 2020 2020  s called...     
+0000f440: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000f450: 6966 206e 6f74 2063 6f6e 6669 674e 616d  if not configNam
+0000f460: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000f470: 6964 7820 3d20 7375 6d28 554e 4e41 4d45  idx = sum(UNNAME
+0000f480: 445f 5052 4553 4554 2069 6e20 7020 666f  D_PRESET in p fo
+0000f490: 7220 7020 696e 2073 656c 662e 6765 7441  r p in self.getA
+0000f4a0: 7661 696c 6162 6c65 436f 6e66 6967 7328  vailableConfigs(
+0000f4b0: 6772 6f75 704e 616d 6529 290d 0a20 2020  groupName))..   
+0000f4c0: 2020 2020 2020 2020 2063 6f6e 6669 674e           configN
+0000f4d0: 616d 6520 3d20 6622 7b55 4e4e 414d 4544  ame = f"{UNNAMED
+0000f4e0: 5f50 5245 5345 547d 5f7b 6964 787d 2220  _PRESET}_{idx}" 
+0000f4f0: 6966 2069 6478 203e 2030 2065 6c73 6520  if idx > 0 else 
+0000f500: 554e 4e41 4d45 445f 5052 4553 4554 0d0a  UNNAMED_PRESET..
+0000f510: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+0000f520: 2073 656c 662e 6973 4772 6f75 7044 6566   self.isGroupDef
+0000f530: 696e 6564 2867 726f 7570 4e61 6d65 293a  ined(groupName):
+0000f540: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000f550: 6e65 6564 6564 2074 6f20 7265 6672 6573  needed to refres
+0000f560: 6820 7079 6d6d 636f 7265 2027 4368 616e  h pymmcore 'Chan
+0000f570: 6e65 6c47 726f 7570 2720 6f70 7469 6f6e  nelGroup' option
+0000f580: 730d 0a20 2020 2020 2020 2020 2020 2073  s..            s
+0000f590: 7570 6572 2829 2e64 6566 696e 6543 6f6e  uper().defineCon
+0000f5a0: 6669 6747 726f 7570 2867 726f 7570 4e61  figGroup(groupNa
+0000f5b0: 6d65 290d 0a0d 0a20 2020 2020 2020 2069  me)....        i
+0000f5c0: 6620 2864 6576 6963 654c 6162 656c 2069  f (deviceLabel i
+0000f5d0: 7320 6e6f 7420 4e6f 6e65 2920 616e 6420  s not None) and 
+0000f5e0: 2870 726f 704e 616d 6520 6973 206e 6f74  (propName is not
+0000f5f0: 204e 6f6e 6529 2061 6e64 2028 7661 6c75   None) and (valu
+0000f600: 6520 6973 206e 6f74 204e 6f6e 6529 3a0d  e is not None):.
+0000f610: 0a20 2020 2020 2020 2020 2020 2073 7570  .            sup
+0000f620: 6572 2829 2e64 6566 696e 6543 6f6e 6669  er().defineConfi
+0000f630: 6728 6772 6f75 704e 616d 652c 2063 6f6e  g(groupName, con
+0000f640: 6669 674e 616d 652c 2064 6576 6963 654c  figName, deviceL
+0000f650: 6162 656c 2c20 7072 6f70 4e61 6d65 2c20  abel, propName, 
+0000f660: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
+0000f670: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000f680: 2020 2064 6576 6963 654c 6162 656c 2c20     deviceLabel, 
+0000f690: 7072 6f70 4e61 6d65 2c20 7661 6c75 6520  propName, value 
+0000f6a0: 3d20 2822 222c 2022 222c 2022 2229 0d0a  = ("", "", "")..
+0000f6b0: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+0000f6c0: 7228 292e 6465 6669 6e65 436f 6e66 6967  r().defineConfig
+0000f6d0: 2867 726f 7570 4e61 6d65 2c20 636f 6e66  (groupName, conf
+0000f6e0: 6967 4e61 6d65 290d 0a0d 0a20 2020 2020  igName)....     
+0000f6f0: 2020 2073 656c 662e 6576 656e 7473 2e63     self.events.c
+0000f700: 6f6e 6669 6744 6566 696e 6564 2e65 6d69  onfigDefined.emi
+0000f710: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+0000f720: 6772 6f75 704e 616d 652c 2063 6f6e 6669  groupName, confi
+0000f730: 674e 616d 652c 2064 6576 6963 654c 6162  gName, deviceLab
+0000f740: 656c 2c20 7072 6f70 4e61 6d65 2c20 7661  el, propName, va
+0000f750: 6c75 650d 0a20 2020 2020 2020 2029 0d0a  lue..        )..
+0000f760: 0d0a 2020 2020 6465 6620 7365 7450 6978  ..    def setPix
+0000f770: 656c 5369 7a65 556d 2873 656c 662c 2072  elSizeUm(self, r
+0000f780: 6573 6f6c 7574 696f 6e49 443a 2073 7472  esolutionID: str
+0000f790: 2c20 7069 7853 697a 653a 2066 6c6f 6174  , pixSize: float
+0000f7a0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+0000f7b0: 2020 2020 2222 2253 6574 2070 6978 656c      """Set pixel
+0000f7c0: 2073 697a 6520 696e 206d 6963 726f 6e73   size in microns
+0000f7d0: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
+0000f7e0: 6564 2060 7265 736f 6c75 7469 6f6e 4944  ed `resolutionID
+0000f7f0: 602e 0d0a 0d0a 2020 2020 2020 2020 2a2a  `.....        **
+0000f800: 5768 7920 4f76 6572 7269 6465 3f2a 2a20  Why Override?** 
+0000f810: 546f 2065 6d69 7420 6120 6070 6978 656c  To emit a `pixel
+0000f820: 5369 7a65 4368 616e 6765 6460 2065 7665  SizeChanged` eve
+0000f830: 6e74 2e0d 0a20 2020 2020 2020 2022 2222  nt...        """
+0000f840: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+0000f850: 292e 7365 7450 6978 656c 5369 7a65 556d  ).setPixelSizeUm
+0000f860: 2872 6573 6f6c 7574 696f 6e49 442c 2070  (resolutionID, p
+0000f870: 6978 5369 7a65 290d 0a20 2020 2020 2020  ixSize)..       
+0000f880: 2073 656c 662e 6576 656e 7473 2e70 6978   self.events.pix
+0000f890: 656c 5369 7a65 4368 616e 6765 642e 656d  elSizeChanged.em
+0000f8a0: 6974 2870 6978 5369 7a65 290d 0a0d 0a20  it(pixSize).... 
+0000f8b0: 2020 2064 6566 2064 656c 6574 6550 6978     def deletePix
+0000f8c0: 656c 5369 7a65 436f 6e66 6967 2873 656c  elSizeConfig(sel
+0000f8d0: 662c 2072 6573 6f6c 7574 696f 6e49 443a  f, resolutionID:
+0000f8e0: 2073 7472 2920 2d3e 204e 6f6e 653a 0d0a   str) -> None:..
+0000f8f0: 2020 2020 2020 2020 2222 2244 656c 6574          """Delet
+0000f900: 6520 7468 6520 7069 7865 6c20 7369 7a65  e the pixel size
+0000f910: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+0000f920: 6f72 2074 6865 2067 6976 656e 2060 7265  or the given `re
+0000f930: 736f 6c75 7469 6f6e 4944 602e 0d0a 0d0a  solutionID`.....
+0000f940: 2020 2020 2020 2020 2a2a 5768 7920 4f76          **Why Ov
+0000f950: 6572 7269 6465 3f2a 2a20 546f 2065 6d69  erride?** To emi
+0000f960: 7420 6120 6070 6978 656c 5369 7a65 4368  t a `pixelSizeCh
+0000f970: 616e 6765 6460 2065 7665 6e74 2e0d 0a20  anged` event... 
+0000f980: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0000f990: 2020 2020 7375 7065 7228 292e 6465 6c65      super().dele
+0000f9a0: 7465 5069 7865 6c53 697a 6543 6f6e 6669  tePixelSizeConfi
+0000f9b0: 6728 7265 736f 6c75 7469 6f6e 4944 290d  g(resolutionID).
+0000f9c0: 0a20 2020 2020 2020 2073 656c 662e 6576  .        self.ev
+0000f9d0: 656e 7473 2e70 6978 656c 5369 7a65 4368  ents.pixelSizeCh
+0000f9e0: 616e 6765 642e 656d 6974 2830 2e30 290d  anged.emit(0.0).
+0000f9f0: 0a0d 0a20 2020 2040 6f76 6572 6c6f 6164  ...    @overload
+0000fa00: 0d0a 2020 2020 6465 6620 6465 6669 6e65  ..    def define
+0000fa10: 5069 7865 6c53 697a 6543 6f6e 6669 6728  PixelSizeConfig(
+0000fa20: 7365 6c66 2c20 7265 736f 6c75 7469 6f6e  self, resolution
+0000fa30: 4944 3a20 7374 7229 202d 3e20 4e6f 6e65  ID: str) -> None
+0000fa40: 3a0d 0a20 2020 2020 2020 202e 2e2e 0d0a  :..        .....
+0000fa50: 0d0a 2020 2020 406f 7665 726c 6f61 640d  ..    @overload.
+0000fa60: 0a20 2020 2064 6566 2064 6566 696e 6550  .    def defineP
+0000fa70: 6978 656c 5369 7a65 436f 6e66 6967 280d  ixelSizeConfig(.
+0000fa80: 0a20 2020 2020 2020 2073 656c 662c 2072  .        self, r
+0000fa90: 6573 6f6c 7574 696f 6e49 443a 2073 7472  esolutionID: str
+0000faa0: 2c20 6465 7669 6365 4c61 6265 6c3a 2073  , deviceLabel: s
+0000fab0: 7472 2c20 7072 6f70 4e61 6d65 3a20 7374  tr, propName: st
+0000fac0: 722c 2076 616c 7565 3a20 7374 720d 0a20  r, value: str.. 
+0000fad0: 2020 2029 202d 3e20 4e6f 6e65 3a0d 0a20     ) -> None:.. 
+0000fae0: 2020 2020 2020 202e 2e2e 0d0a 0d0a 2020         .......  
+0000faf0: 2020 6465 6620 6465 6669 6e65 5069 7865    def definePixe
+0000fb00: 6c53 697a 6543 6f6e 6669 6728 7365 6c66  lSizeConfig(self
+0000fb10: 2c20 2a61 7267 733a 2073 7472 2c20 2a2a  , *args: str, **
+0000fb20: 6b77 6172 6773 3a20 7374 7229 202d 3e20  kwargs: str) -> 
+0000fb30: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2022  None:..        "
+0000fb40: 2222 4465 6669 6e65 7320 616e 2065 6d70  ""Defines an emp
+0000fb50: 7479 2070 6978 656c 2073 697a 6520 656e  ty pixel size en
+0000fb60: 7472 792e 0d0a 0d0a 2020 2020 2020 2020  try.....        
+0000fb70: 2a2a 5768 7920 4f76 6572 7269 6465 3f2a  **Why Override?*
+0000fb80: 2a20 546f 2065 6d69 7420 6120 6070 6978  * To emit a `pix
+0000fb90: 656c 5369 7a65 4368 616e 6765 6460 2065  elSizeChanged` e
+0000fba0: 7665 6e74 2e0d 0a20 2020 2020 2020 2022  vent...        "
+0000fbb0: 2222 0d0a 2020 2020 2020 2020 7375 7065  ""..        supe
+0000fbc0: 7228 292e 6465 6669 6e65 5069 7865 6c53  r().definePixelS
+0000fbd0: 697a 6543 6f6e 6669 6728 2a61 7267 732c  izeConfig(*args,
+0000fbe0: 202a 2a6b 7761 7267 7329 0d0a 2020 2020   **kwargs)..    
+0000fbf0: 2020 2020 7365 6c66 2e65 7665 6e74 732e      self.events.
+0000fc00: 7069 7865 6c53 697a 6543 6861 6e67 6564  pixelSizeChanged
+0000fc10: 2e65 6d69 7428 302e 3029 0d0a 0d0a 2020  .emit(0.0)....  
+0000fc20: 2020 406f 7665 726c 6f61 640d 0a20 2020    @overload..   
+0000fc30: 2064 6566 2073 6574 524f 4928 7365 6c66   def setROI(self
+0000fc40: 2c20 783a 2069 6e74 2c20 793a 2069 6e74  , x: int, y: int
+0000fc50: 2c20 7769 6474 683a 2069 6e74 2c20 6865  , width: int, he
+0000fc60: 6967 6874 3a20 696e 7429 202d 3e20 4e6f  ight: int) -> No
+0000fc70: 6e65 3a0d 0a20 2020 2020 2020 202e 2e2e  ne:..        ...
+0000fc80: 0d0a 0d0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
+0000fc90: 640d 0a20 2020 2064 6566 2073 6574 524f  d..    def setRO
+0000fca0: 4928 7365 6c66 2c20 6c61 6265 6c3a 2073  I(self, label: s
+0000fcb0: 7472 2c20 783a 2069 6e74 2c20 793a 2069  tr, x: int, y: i
+0000fcc0: 6e74 2c20 7769 6474 683a 2069 6e74 2c20  nt, width: int, 
+0000fcd0: 6865 6967 6874 3a20 696e 7429 202d 3e20  height: int) -> 
+0000fce0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 202e  None:..        .
+0000fcf0: 2e2e 0d0a 0d0a 2020 2020 6465 6620 7365  ......    def se
+0000fd00: 7452 4f49 2873 656c 662c 202a 6172 6773  tROI(self, *args
+0000fd10: 3a20 416e 792c 202a 2a6b 7761 7267 733a  : Any, **kwargs:
+0000fd20: 2041 6e79 2920 2d3e 204e 6f6e 653a 0d0a   Any) -> None:..
+0000fd30: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
+0000fd40: 6865 2063 616d 6572 6120 5265 6769 6f6e  he camera Region
+0000fd50: 206f 6620 496e 7465 7265 7374 2028 524f   of Interest (RO
+0000fd60: 4929 2e0d 0a0d 0a20 2020 2020 2020 202a  I).....        *
+0000fd70: 2a57 6879 204f 7665 7272 6964 653f 2a2a  *Why Override?**
+0000fd80: 2054 6f20 656d 6974 2061 2060 726f 6953   To emit a `roiS
+0000fd90: 6574 6020 6576 656e 742e 0d0a 2020 2020  et` event...    
+0000fda0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000fdb0: 2073 7570 6572 2829 2e73 6574 524f 4928   super().setROI(
+0000fdc0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+0000fdd0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0000fde0: 2861 7267 7329 203d 3d20 343a 0d0a 2020  (args) == 4:..  
+0000fdf0: 2020 2020 2020 2020 2020 6172 6773 203d            args =
+0000fe00: 2028 7375 7065 7228 292e 6765 7443 616d   (super().getCam
+0000fe10: 6572 6144 6576 6963 6528 292c 202a 6172  eraDevice(), *ar
+0000fe20: 6773 290d 0a20 2020 2020 2020 2073 656c  gs)..        sel
+0000fe30: 662e 6576 656e 7473 2e72 6f69 5365 742e  f.events.roiSet.
+0000fe40: 656d 6974 282a 6172 6773 290d 0a0d 0a20  emit(*args).... 
+0000fe50: 2020 2064 6566 2073 6574 4368 616e 6e65     def setChanne
+0000fe60: 6c47 726f 7570 2873 656c 662c 2063 6861  lGroup(self, cha
+0000fe70: 6e6e 656c 4772 6f75 703a 2073 7472 2920  nnelGroup: str) 
+0000fe80: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+0000fe90: 2020 2222 2253 7065 6369 6669 6573 2074    """Specifies t
+0000fea0: 6865 2067 726f 7570 2064 6574 6572 6d69  he group determi
+0000feb0: 6e69 6e67 2074 6865 2063 6861 6e6e 656c  ning the channel
+0000fec0: 2073 656c 6563 7469 6f6e 2e0d 0a0d 0a20   selection..... 
+0000fed0: 2020 2020 2020 202e 2e2e 616e 6420 7365         ...and se
+0000fee0: 6e64 2061 2063 6861 6e6e 656c 4772 6f75  nd a channelGrou
+0000fef0: 7043 6861 6e67 6564 2073 6967 6e61 6c2e  pChanged signal.
+0000ff00: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000ff10: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
+0000ff20: 6574 4368 616e 6e65 6c47 726f 7570 2829  etChannelGroup()
+0000ff30: 2021 3d20 6368 616e 6e65 6c47 726f 7570   != channelGroup
+0000ff40: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0000ff50: 7570 6572 2829 2e73 6574 4368 616e 6e65  uper().setChanne
+0000ff60: 6c47 726f 7570 2863 6861 6e6e 656c 4772  lGroup(channelGr
+0000ff70: 6f75 7029 0d0a 2020 2020 2020 2020 2020  oup)..          
+0000ff80: 2020 7365 6c66 2e65 7665 6e74 732e 6368    self.events.ch
+0000ff90: 616e 6e65 6c47 726f 7570 4368 616e 6765  annelGroupChange
+0000ffa0: 642e 656d 6974 2863 6861 6e6e 656c 4772  d.emit(channelGr
+0000ffb0: 6f75 7029 0d0a 0d0a 2020 2020 6465 6620  oup)....    def 
+0000ffc0: 7365 7446 6f63 7573 4465 7669 6365 2873  setFocusDevice(s
+0000ffd0: 656c 662c 2066 6f63 7573 4c61 6265 6c3a  elf, focusLabel:
+0000ffe0: 2073 7472 2920 2d3e 204e 6f6e 653a 0d0a   str) -> None:..
+0000fff0: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
+00010000: 6865 2063 7572 7265 6e74 2046 6f63 7573  he current Focus
+00010010: 2044 6576 6963 6520 616e 6420 656d 6974   Device and emit
+00010020: 2061 2060 7072 6f70 6572 7479 4368 616e   a `propertyChan
+00010030: 6765 6460 2073 6967 6e61 6c2e 2222 220d  ged` signal.""".
+00010040: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00010050: 2e67 6574 466f 6375 7344 6576 6963 6528  .getFocusDevice(
+00010060: 2920 213d 2066 6f63 7573 4c61 6265 6c3a  ) != focusLabel:
+00010070: 0d0a 2020 2020 2020 2020 2020 2020 7375  ..            su
+00010080: 7065 7228 292e 7365 7446 6f63 7573 4465  per().setFocusDe
+00010090: 7669 6365 2866 6f63 7573 4c61 6265 6c29  vice(focusLabel)
+000100a0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000100b0: 6c66 2e65 7665 6e74 732e 7072 6f70 6572  lf.events.proper
+000100c0: 7479 4368 616e 6765 642e 656d 6974 2822  tyChanged.emit("
+000100d0: 436f 7265 222c 2022 466f 6375 7322 2c20  Core", "Focus", 
+000100e0: 666f 6375 734c 6162 656c 290d 0a0d 0a20  focusLabel).... 
+000100f0: 2020 2064 6566 2073 6176 6553 7973 7465     def saveSyste
+00010100: 6d43 6f6e 6669 6775 7261 7469 6f6e 2873  mConfiguration(s
+00010110: 656c 662c 2066 696c 656e 616d 653a 2073  elf, filename: s
+00010120: 7472 2920 2d3e 204e 6f6e 653a 0d0a 2020  tr) -> None:..  
+00010130: 2020 2020 2020 2222 2253 6176 6573 2074        """Saves t
+00010140: 6865 2063 7572 7265 6e74 2073 7973 7465  he current syste
+00010150: 6d20 636f 6e66 6967 7572 6174 696f 6e20  m configuration 
+00010160: 746f 2061 2074 6578 7420 6669 6c65 2e0d  to a text file..
+00010170: 0a0d 0a20 2020 2020 2020 202a 2a57 6879  ...        **Why
+00010180: 204f 7665 7272 6964 653f 2a2a 2054 6f20   Override?** To 
+00010190: 616c 736f 2073 6176 6520 7069 7865 6c20  also save pixel 
+000101a0: 7369 7a65 2063 6f6e 6669 6775 7261 7469  size configurati
+000101b0: 6f6e 732e 0d0a 2020 2020 2020 2020 2222  ons...        ""
+000101c0: 220d 0a20 2020 2020 2020 2073 7570 6572  "..        super
+000101d0: 2829 2e73 6176 6553 7973 7465 6d43 6f6e  ().saveSystemCon
+000101e0: 6669 6775 7261 7469 6f6e 2866 696c 656e  figuration(filen
+000101f0: 616d 6529 0d0a 2020 2020 2020 2020 7078  ame)..        px
+00010200: 5f63 6f6e 6669 6773 203d 2073 656c 662e  _configs = self.
+00010210: 6765 7441 7661 696c 6162 6c65 5069 7865  getAvailablePixe
+00010220: 6c53 697a 6543 6f6e 6669 6773 2829 0d0a  lSizeConfigs()..
+00010230: 2020 2020 2020 2020 6966 206e 6f74 2070          if not p
+00010240: 785f 636f 6e66 6967 733a 0d0a 2020 2020  x_configs:..    
+00010250: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00010260: 2020 2020 2020 2020 2320 7361 7665 5379          # saveSy
+00010270: 7374 656d 436f 6e66 6967 7572 6174 696f  stemConfiguratio
+00010280: 6e20 646f 6573 206e 6f74 2073 6176 6520  n does not save 
+00010290: 7468 6520 7069 7865 6c20 7369 7a65 2063  the pixel size c
+000102a0: 6f6e 6669 6720 736f 2068 6572 650d 0a20  onfig so here.. 
+000102b0: 2020 2020 2020 2023 2077 6520 6164 6420         # we add 
+000102c0: 746f 2074 6865 2073 6176 6564 2066 696c  to the saved fil
+000102d0: 6520 616c 736f 2061 6e79 2070 6978 656c  e also any pixel
+000102e0: 2073 697a 6520 636f 6e66 6967 2e0d 0a20   size config... 
+000102f0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00010300: 2866 696c 656e 616d 652c 2022 6122 2920  (filename, "a") 
+00010310: 6173 2066 3a0d 0a20 2020 2020 2020 2020  as f:..         
+00010320: 2020 2066 2e77 7269 7465 2822 2320 5069     f.write("# Pi
+00010330: 7865 6c53 697a 6520 7365 7474 696e 6773  xelSize settings
+00010340: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00010350: 666f 7220 7078 5f63 6f6e 6669 6720 696e  for px_config in
+00010360: 2070 785f 636f 6e66 6967 733a 0d0a 2020   px_configs:..  
+00010370: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00010380: 7461 203d 2073 656c 662e 6765 7450 6978  ta = self.getPix
+00010390: 656c 5369 7a65 436f 6e66 6967 4461 7461  elSizeConfigData
+000103a0: 2870 785f 636f 6e66 6967 290d 0a20 2020  (px_config)..   
+000103b0: 2020 2020 2020 2020 2020 2020 206f 626a               obj
+000103c0: 203d 2064 6174 612e 6469 6374 2829 5b22   = data.dict()["
+000103d0: 4f62 6a65 6374 6976 6522 5d5b 224c 6162  Objective"]["Lab
+000103e0: 656c 225d 0d0a 2020 2020 2020 2020 2020  el"]..          
+000103f0: 2020 2020 2020 7078 5f73 697a 6520 3d20        px_size = 
+00010400: 7365 6c66 2e67 6574 5069 7865 6c53 697a  self.getPixelSiz
+00010410: 6555 6d42 7949 4428 7078 5f63 6f6e 6669  eUmByID(px_confi
+00010420: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
+00010430: 2020 2020 7078 5f61 6666 696e 6520 3d20      px_affine = 
+00010440: 7365 6c66 2e67 6574 5069 7865 6c53 697a  self.getPixelSiz
+00010450: 6541 6666 696e 6542 7949 4428 7078 5f63  eAffineByID(px_c
+00010460: 6f6e 6669 6729 0d0a 2020 2020 2020 2020  onfig)..        
+00010470: 2020 2020 2020 2020 6366 6720 3d20 280d          cfg = (.
+00010480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010490: 2020 2020 2066 225c 6e43 6f6e 6669 6750       f"\nConfigP
+000104a0: 6978 656c 5369 7a65 2c7b 7078 5f63 6f6e  ixelSize,{px_con
+000104b0: 6669 677d 2c4f 626a 6563 7469 7665 2c4c  fig},Objective,L
+000104c0: 6162 656c 2c7b 6f62 6a7d 5c6e 220d 0a20  abel,{obj}\n".. 
+000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104e0: 2020 2066 2250 6978 656c 5369 7a65 5f75     f"PixelSize_u
+000104f0: 6d2c 7b70 785f 636f 6e66 6967 7d2c 7b70  m,{px_config},{p
+00010500: 785f 7369 7a65 7d5c 6e22 0d0a 2020 2020  x_size}\n"..    
+00010510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010520: 6622 5069 7865 6c53 697a 6541 6666 696e  f"PixelSizeAffin
+00010530: 652c 7b70 785f 636f 6e66 6967 7d2c 7b27  e,{px_config},{'
+00010540: 2c27 2e6a 6f69 6e28 6d61 7028 7374 722c  ,'.join(map(str,
+00010550: 2070 785f 6166 6669 6e65 2929 7d22 0d0a   px_affine))}"..
+00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010580: 2020 2066 2e77 7269 7465 2863 6667 290d     f.write(cfg).
+00010590: 0a0d 0a20 2020 2064 6566 2064 6573 6372  ...    def descr
+000105a0: 6962 6528 7365 6c66 2c20 736f 7274 3a20  ibe(self, sort: 
+000105b0: 7374 7220 7c20 4e6f 6e65 203d 204e 6f6e  str | None = Non
+000105c0: 6529 202d 3e20 4e6f 6e65 3a0d 0a20 2020  e) -> None:..   
+000105d0: 2020 2020 2022 2222 5072 696e 7420 696e       """Print in
+000105e0: 666f 726d 6174 696f 6e20 7461 626c 6520  formation table 
+000105f0: 7769 7468 2074 6865 2063 7572 7265 6e74  with the current
+00010600: 2063 6f6e 6669 6775 7261 7469 6f6e 2e0d   configuration..
+00010610: 0a0d 0a20 2020 2020 2020 2049 6e74 656e  ...        Inten
+00010620: 6465 6420 746f 2070 726f 7669 6465 2061  ded to provide a
+00010630: 2071 7569 636b 206f 7665 7276 6965 7720   quick overview 
+00010640: 6f66 2074 6865 206d 6963 726f 7363 6f70  of the microscop
+00010650: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00010660: 6475 7269 6e67 0d0a 2020 2020 2020 2020  during..        
+00010670: 696e 7465 7261 6374 6976 6520 7465 726d  interactive term
+00010680: 696e 616c 2075 7361 6765 2e0d 0a0d 0a20  inal usage..... 
+00010690: 2020 2020 2020 203a 7370 6172 6b6c 6573         :sparkles
+000106a0: 3a20 2a54 6869 7320 6d65 7468 6f64 2069  : *This method i
+000106b0: 7320 6e65 7720 696e 2060 434d 4d43 6f72  s new in `CMMCor
+000106c0: 6550 6c75 7360 2e2a 0d0a 2020 2020 2020  ePlus`.*..      
+000106d0: 2020 2222 220d 0a20 2020 2020 2020 205f    """..        _
+000106e0: 6375 7272 656e 7420 3d20 7b0d 0a20 2020  current = {..   
+000106f0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+00010700: 7443 616d 6572 6144 6576 6963 6528 293a  tCameraDevice():
+00010710: 2022 4361 6d65 7261 222c 0d0a 2020 2020   "Camera",..    
+00010720: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
+00010730: 5859 5374 6167 6544 6576 6963 6528 293a  XYStageDevice():
+00010740: 2022 5859 5374 6167 6522 2c0d 0a20 2020   "XYStage",..   
+00010750: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+00010760: 7446 6f63 7573 4465 7669 6365 2829 3a20  tFocusDevice(): 
+00010770: 2246 6f63 7573 222c 0d0a 2020 2020 2020  "Focus",..      
+00010780: 2020 2020 2020 7365 6c66 2e67 6574 5368        self.getSh
+00010790: 7574 7465 7244 6576 6963 6528 293a 2022  utterDevice(): "
+000107a0: 5368 7574 7465 7222 2c0d 0a20 2020 2020  Shutter",..     
+000107b0: 2020 2020 2020 2073 656c 662e 6765 7453         self.getS
+000107c0: 4c4d 4465 7669 6365 2829 3a20 2253 4c4d  LMDevice(): "SLM
+000107d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000107e0: 7365 6c66 2e67 6574 4761 6c76 6f44 6576  self.getGalvoDev
+000107f0: 6963 6528 293a 2022 4761 6c76 6f22 2c0d  ice(): "Galvo",.
+00010800: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010810: 662e 6765 7441 7574 6f46 6f63 7573 4465  f.getAutoFocusDe
+00010820: 7669 6365 2829 3a20 2241 7574 6f46 6f63  vice(): "AutoFoc
+00010830: 7573 222c 0d0a 2020 2020 2020 2020 2020  us",..          
+00010840: 2020 7365 6c66 2e67 6574 496d 6167 6550    self.getImageP
+00010850: 726f 6365 7373 6f72 4465 7669 6365 2829  rocessorDevice()
+00010860: 3a20 2249 6d61 6765 5072 6f63 6573 736f  : "ImageProcesso
+00010870: 7222 2c0d 0a20 2020 2020 2020 207d 0d0a  r",..        }..
+00010880: 0d0a 2020 2020 2020 2020 6461 7461 3a20  ..        data: 
+00010890: 6465 6661 756c 7464 6963 745b 7374 722c  defaultdict[str,
+000108a0: 206c 6973 745b 7374 725d 5d20 3d20 6465   list[str]] = de
+000108b0: 6661 756c 7464 6963 7428 6c69 7374 290d  faultdict(list).
+000108c0: 0a20 2020 2020 2020 2066 6f72 2064 6576  .        for dev
+000108d0: 6963 6520 696e 2073 656c 662e 6974 6572  ice in self.iter
+000108e0: 4465 7669 6365 7328 293a 0d0a 2020 2020  Devices():..    
+000108f0: 2020 2020 2020 2020 6461 7461 5b22 4465          data["De
+00010900: 7669 6365 204c 6162 656c 225d 2e61 7070  vice Label"].app
+00010910: 656e 6428 6465 7669 6365 2e6c 6162 656c  end(device.label
+00010920: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00010930: 6174 615b 2254 7970 6522 5d2e 6170 7065  ata["Type"].appe
+00010940: 6e64 2873 7472 2864 6576 6963 652e 7479  nd(str(device.ty
+00010950: 7065 2829 2929 0d0a 2020 2020 2020 2020  pe()))..        
+00010960: 2020 2020 6461 7461 5b22 4375 7272 656e      data["Curren
+00010970: 7422 5d2e 6170 7065 6e64 285f 6375 7272  t"].append(_curr
+00010980: 656e 742e 6765 7428 6465 7669 6365 2e6c  ent.get(device.l
+00010990: 6162 656c 2c20 2222 2929 0d0a 2020 2020  abel, ""))..    
+000109a0: 2020 2020 2020 2020 6461 7461 5b22 4c69          data["Li
+000109b0: 6272 6172 793a 3a44 6576 6963 654e 616d  brary::DeviceNam
+000109c0: 6522 5d2e 6170 7065 6e64 2866 227b 6465  e"].append(f"{de
+000109d0: 7669 6365 2e6c 6962 7261 7279 2829 7d3a  vice.library()}:
+000109e0: 3a7b 6465 7669 6365 2e6e 616d 6528 297d  :{device.name()}
+000109f0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00010a00: 6461 7461 5b22 4465 7363 7269 7074 696f  data["Descriptio
+00010a10: 6e22 5d2e 6170 7065 6e64 2864 6576 6963  n"].append(devic
+00010a20: 652e 6465 7363 7269 7074 696f 6e28 2929  e.description())
+00010a30: 0d0a 0d0a 2020 2020 2020 2020 6966 206e  ....        if n
+00010a40: 6f74 2061 6e79 2864 6174 615b 2243 7572  ot any(data["Cur
+00010a50: 7265 6e74 225d 293a 0d0a 2020 2020 2020  rent"]):..      
+00010a60: 2020 2020 2020 6461 7461 2e70 6f70 2822        data.pop("
+00010a70: 4375 7272 656e 7422 290d 0a0d 0a20 2020  Current")....   
+00010a80: 2020 2020 2070 7269 6e74 2866 227b 7365       print(f"{se
+00010a90: 6c66 2e67 6574 5665 7273 696f 6e49 6e66  lf.getVersionInf
+00010aa0: 6f28 297d 2c20 7b73 656c 662e 6765 7441  o()}, {self.getA
+00010ab0: 5049 5665 7273 696f 6e49 6e66 6f28 297d  PIVersionInfo()}
+00010ac0: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+00010ad0: 7428 2241 6461 7074 6572 2070 6174 683a  t("Adapter path:
+00010ae0: 222c 2022 2c22 2e6a 6f69 6e28 7365 6c66  ", ",".join(self
+00010af0: 2e67 6574 4465 7669 6365 4164 6170 7465  .getDeviceAdapte
+00010b00: 7253 6561 7263 6850 6174 6873 2829 2929  rSearchPaths()))
+00010b10: 0d0a 2020 2020 2020 2020 7072 696e 745f  ..        print_
+00010b20: 7461 6275 6c61 725f 6461 7461 2864 6174  tabular_data(dat
+00010b30: 612c 2073 6f72 743d 736f 7274 290d 0a0d  a, sort=sort)...
+00010b40: 0a20 2020 2064 6566 2073 7461 7465 2873  .    def state(s
+00010b50: 656c 662c 2065 7863 6c75 6465 3a20 4974  elf, exclude: It
+00010b60: 6572 6162 6c65 5b73 7472 5d20 3d20 2829  erable[str] = ()
+00010b70: 2920 2d3e 2053 7461 7465 4469 6374 3a0d  ) -> StateDict:.
+00010b80: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00010b90: 726e 2060 5374 6174 6544 6963 7460 2077  rn `StateDict` w
+00010ba0: 6974 6820 636f 6d6d 6f6e 6c79 2061 6363  ith commonly acc
+00010bb0: 6573 7365 6420 7374 6174 6520 7661 6c75  essed state valu
+00010bc0: 6573 2e0d 0a0d 0a20 2020 2020 2020 203a  es.....        :
+00010bd0: 7370 6172 6b6c 6573 3a20 2a54 6869 7320  sparkles: *This 
+00010be0: 6d65 7468 6f64 2069 7320 6e65 7720 696e  method is new in
+00010bf0: 2060 434d 4d43 6f72 6550 6c75 7360 2e20   `CMMCorePlus`. 
+00010c00: 4974 2069 7320 6120 6269 7420 6661 7374  It is a bit fast
+00010c10: 6572 0d0a 2020 2020 2020 2020 7468 616e  er..        than
+00010c20: 205b 6067 6574 5379 7374 656d 5374 6174   [`getSystemStat
+00010c30: 6560 5d5b 7079 6d6d 636f 7265 5f70 6c75  e`][pymmcore_plu
+00010c40: 732e 434d 4d43 6f72 6550 6c75 732e 6765  s.CMMCorePlus.ge
+00010c50: 7453 7973 7465 6d53 7461 7465 5d2e 2a0d  tSystemState].*.
+00010c60: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00010c70: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+00010c80: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+00010c90: 2020 2065 7863 6c75 6465 203a 2049 7465     exclude : Ite
+00010ca0: 7261 626c 655b 7374 725d 0d0a 2020 2020  rable[str]..    
+00010cb0: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
+00010cc0: 7072 6f70 6572 7469 6573 2074 6f20 6578  properties to ex
+00010cd0: 636c 7564 6520 7768 656e 2067 6174 6865  clude when gathe
+00010ce0: 7269 6e67 2073 7461 7465 2028 6d61 7920  ring state (may 
+00010cf0: 7370 6565 6420 7468 696e 6773 2075 7029  speed things up)
+00010d00: 2e0d 0a20 2020 2020 2020 2020 2020 2053  ...            S
+00010d10: 6565 205b 6053 7461 7465 4469 6374 605d  ee [`StateDict`]
+00010d20: 5b70 796d 6d63 6f72 655f 706c 7573 2e63  [pymmcore_plus.c
+00010d30: 6f72 652e 5f6d 6d63 6f72 655f 706c 7573  ore._mmcore_plus
+00010d40: 2e53 7461 7465 4469 6374 5d20 666f 7220  .StateDict] for 
+00010d50: 6120 6c69 7374 206f 660d 0a20 2020 2020  a list of..     
+00010d60: 2020 2020 2020 206b 6579 7320 7468 6174         keys that
+00010d70: 2063 616e 2062 6520 6578 636c 7564 6564   can be excluded
+00010d80: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00010d90: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+00010da0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2053  -----..        S
+00010db0: 7461 7465 4469 6374 0d0a 2020 2020 2020  tateDict..      
+00010dc0: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
+00010dd0: 7279 206f 6620 636f 6d6d 6f6e 6c79 2061  ry of commonly a
+00010de0: 6363 6573 7365 6420 7374 6174 6520 7661  ccessed state va
+00010df0: 6c75 6573 2e0d 0a20 2020 2020 2020 2022  lues...        "
+00010e00: 2222 0d0a 2020 2020 2020 2020 2320 6170  ""..        # ap
+00010e10: 7072 6f78 2072 6574 7269 6576 616c 2063  prox retrieval c
+00010e20: 6f73 7420 696e 2063 6f6d 6d65 6e74 2028  ost in comment (
+00010e30: 666f 7220 6465 6d6f 4361 6d29 0d0a 2020  for demoCam)..  
+00010e40: 2020 2020 2020 6578 636c 7564 6520 3d20        exclude = 
+00010e50: 7365 7428 6578 636c 7564 6529 0d0a 2020  set(exclude)..  
+00010e60: 2020 2020 2020 7374 6174 653a 2064 6963        state: dic
+00010e70: 7420 3d20 7b7d 0d0a 2020 2020 2020 2020  t = {}..        
+00010e80: 666f 7220 6174 7472 2069 6e20 280d 0a20  for attr in (.. 
+00010e90: 2020 2020 2020 2020 2020 2022 4175 746f             "Auto
+00010ea0: 466f 6375 7344 6576 6963 6522 2c20 2023  FocusDevice",  #
+00010eb0: 2031 3530 206e 730d 0a20 2020 2020 2020   150 ns..       
+00010ec0: 2020 2020 2022 4279 7465 7350 6572 5069       "BytesPerPi
+00010ed0: 7865 6c22 2c20 2023 2031 3439 206e 730d  xel",  # 149 ns.
+00010ee0: 0a20 2020 2020 2020 2020 2020 2022 4361  .            "Ca
+00010ef0: 6d65 7261 4368 616e 6e65 6c4e 616d 6573  meraChannelNames
+00010f00: 222c 2020 2320 3120 c2b5 730d 0a20 2020  ",  # 1 ..s..   
+00010f10: 2020 2020 2020 2020 2022 4361 6d65 7261           "Camera
+00010f20: 4465 7669 6365 222c 2020 2320 3135 3920  Device",  # 159 
+00010f30: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
+00010f40: 2244 6174 6574 696d 6522 2c0d 0a20 2020  "Datetime",..   
+00010f50: 2020 2020 2020 2020 2022 4578 706f 7375           "Exposu
+00010f60: 7265 222c 2020 2320 3732 3620 6e73 0d0a  re",  # 726 ns..
+00010f70: 2020 2020 2020 2020 2020 2020 2246 6f63              "Foc
+00010f80: 7573 4465 7669 6365 222c 2020 2320 3131  usDevice",  # 11
+00010f90: 3220 6e73 0d0a 2020 2020 2020 2020 2020  2 ns..          
+00010fa0: 2020 2247 616c 766f 4465 7669 6365 222c    "GalvoDevice",
+00010fb0: 2020 2320 3130 3920 6e73 0d0a 2020 2020    # 109 ns..    
+00010fc0: 2020 2020 2020 2020 2249 6d61 6765 4269          "ImageBi
+00010fd0: 7444 6570 7468 222c 2020 2320 3134 3720  tDepth",  # 147 
+00010fe0: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
+00010ff0: 2249 6d61 6765 4865 6967 6874 222c 2020  "ImageHeight",  
+00011000: 2320 3136 3420 6e73 0d0a 2020 2020 2020  # 164 ns..      
+00011010: 2020 2020 2020 2249 6d61 6765 5072 6f63        "ImageProc
+00011020: 6573 736f 7244 6576 6963 6522 2c20 2023  essorDevice",  #
+00011030: 2031 3130 206e 730d 0a20 2020 2020 2020   110 ns..       
+00011040: 2020 2020 2022 496d 6167 6557 6964 7468       "ImageWidth
+00011050: 222c 2020 2320 3137 3220 6e73 0d0a 2020  ",  # 172 ns..  
+00011060: 2020 2020 2020 2020 2020 2250 6978 656c            "Pixel
+00011070: 5369 7a65 556d 222c 2020 2320 322e 3220  SizeUm",  # 2.2 
+00011080: c2b5 730d 0a20 2020 2020 2020 2020 2020  ..s..           
+00011090: 2022 5368 7574 7465 7244 6576 6963 6522   "ShutterDevice"
+000110a0: 2c20 2023 2031 3532 206e 730d 0a20 2020  ,  # 152 ns..   
+000110b0: 2020 2020 2020 2020 2022 534c 4d44 6576           "SLMDev
+000110c0: 6963 6522 2c20 2023 2031 3130 206e 730d  ice",  # 110 ns.
+000110d0: 0a20 2020 2020 2020 2020 2020 2022 5859  .            "XY
+000110e0: 506f 7369 7469 6f6e 222c 2020 2320 312e  Position",  # 1.
+000110f0: 3120 c2b5 730d 0a20 2020 2020 2020 2020  1 ..s..         
+00011100: 2020 2022 5859 5374 6167 6544 6576 6963     "XYStageDevic
+00011110: 6522 2c20 2023 2031 3536 206e 730d 0a20  e",  # 156 ns.. 
+00011120: 2020 2020 2020 2020 2020 2022 5a50 6f73             "ZPos
+00011130: 6974 696f 6e22 2c20 2023 2031 2e30 3320  ition",  # 1.03 
+00011140: c2b5 730d 0a20 2020 2020 2020 2029 3a0d  ..s..        ):.
+00011150: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011160: 6174 7472 206e 6f74 2069 6e20 6578 636c  attr not in excl
+00011170: 7564 653a 0d0a 2020 2020 2020 2020 2020  ude:..          
+00011180: 2020 2020 2020 6966 2061 7474 7220 3d3d        if attr ==
+00011190: 2022 4461 7465 7469 6d65 223a 0d0a 2020   "Datetime":..  
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111b0: 2020 7374 6174 655b 6174 7472 5d20 3d20    state[attr] = 
+000111c0: 7374 7228 6461 7465 7469 6d65 2e6e 6f77  str(datetime.now
+000111d0: 2829 290d 0a20 2020 2020 2020 2020 2020  ())..           
+000111e0: 2020 2020 2065 6c69 6620 6174 7472 203d       elif attr =
+000111f0: 3d20 2250 6978 656c 5369 7a65 556d 223a  = "PixelSizeUm":
+00011200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011210: 2020 2020 2020 7374 6174 655b 6174 7472        state[attr
+00011220: 5d20 3d20 7365 6c66 2e67 6574 5069 7865  ] = self.getPixe
+00011230: 6c53 697a 6555 6d28 5472 7565 2920 2023  lSizeUm(True)  #
+00011240: 2054 7275 653d 3d63 6163 6865 640d 0a20   True==cached.. 
+00011250: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011260: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00011270: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011290: 2020 2020 2020 2020 7374 6174 655b 6174          state[at
+000112a0: 7472 5d20 3d20 6765 7461 7474 7228 7365  tr] = getattr(se
+000112b0: 6c66 2c20 6622 6765 747b 6174 7472 7d22  lf, f"get{attr}"
+000112c0: 2928 290d 0a20 2020 2020 2020 2020 2020  )()..           
+000112d0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+000112e0: 5275 6e74 696d 6545 7272 6f72 3a0d 0a20  RuntimeError:.. 
+000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011300: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00011310: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011320: 6361 7374 2822 5374 6174 6544 6963 7422  cast("StateDict"
+00011330: 2c20 7374 6174 6529 0d0a 0d0a 2020 2020  , state)....    
+00011340: 4063 6f6e 7465 7874 6d61 6e61 6765 720d  @contextmanager.
+00011350: 0a20 2020 2064 6566 205f 7072 6f70 6572  .    def _proper
+00011360: 7479 5f63 6861 6e67 655f 656d 6973 7369  ty_change_emissi
+00011370: 6f6e 5f65 6e73 7572 6564 280d 0a20 2020  on_ensured(..   
+00011380: 2020 2020 2073 656c 662c 2064 6576 6963       self, devic
+00011390: 653a 2073 7472 2c20 7072 6f70 6572 7469  e: str, properti
+000113a0: 6573 3a20 5365 7175 656e 6365 5b73 7472  es: Sequence[str
+000113b0: 5d0d 0a20 2020 2029 202d 3e20 4974 6572  ]..    ) -> Iter
+000113c0: 6174 6f72 5b4e 6f6e 655d 3a0d 0a20 2020  ator[None]:..   
+000113d0: 2020 2020 2022 2222 436f 6e74 6578 7420       """Context 
+000113e0: 7468 6174 2065 6d69 7473 2065 7665 6e74  that emits event
+000113f0: 7320 6966 2061 6e79 206f 6620 6070 726f  s if any of `pro
+00011400: 7065 7274 6965 7360 2063 6861 6e67 6520  perties` change 
+00011410: 6f6e 2064 6576 6963 652e 0d0a 0d0a 2020  on device.....  
+00011420: 2020 2020 2020 4e4f 5445 3a20 4465 7065        NOTE: Depe
+00011430: 6e64 696e 6720 6f6e 2064 6576 6963 6520  nding on device 
+00011440: 6164 6170 7465 7220 6265 6861 7669 6f72  adapter behavior
+00011450: 2074 6865 2073 6967 6e61 6c20 6d61 7920   the signal may 
+00011460: 6265 2065 6d69 7474 6564 2074 7769 6365  be emitted twice
+00011470: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00011480: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+00011490: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+000114a0: 2020 2020 2064 6576 6963 6520 3a20 7374       device : st
+000114b0: 720d 0a20 2020 2020 2020 2020 2020 2061  r..            a
+000114c0: 2064 6576 6963 6520 6c61 6265 6c0d 0a20   device label.. 
+000114d0: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
+000114e0: 7320 3a20 5365 7175 656e 6365 5b73 7472  s : Sequence[str
+000114f0: 5d0d 0a20 2020 2020 2020 2020 2020 2061  ]..            a
+00011500: 2073 6571 7565 6e63 6520 6f66 2070 726f   sequence of pro
+00011510: 7065 7274 7920 6e61 6d65 7320 746f 206d  perty names to m
+00011520: 6f6e 6974 6f72 0d0a 2020 2020 2020 2020  onitor..        
+00011530: 2222 220d 0a20 2020 2020 2020 2023 206d  """..        # m
+00011540: 616b 6520 7375 7265 2074 6861 7420 6368  ake sure that ch
+00011550: 616e 6769 6e67 2065 6974 6865 7220 7374  anging either st
+00011560: 6174 6520 6465 7669 6365 2070 726f 7065  ate device prope
+00011570: 7274 7920 656d 6974 7320 626f 7468 2073  rty emits both s
+00011580: 6967 6e61 6c73 0d0a 2020 2020 2020 2020  ignals..        
+00011590: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
+000115a0: 2020 6c65 6e28 7072 6f70 6572 7469 6573    len(properties
+000115b0: 2920 3d3d 2031 0d0a 2020 2020 2020 2020  ) == 1..        
+000115c0: 2020 2020 616e 6420 7072 6f70 6572 7469      and properti
+000115d0: 6573 5b30 5d20 696e 2053 5441 5445 5f50  es[0] in STATE_P
+000115e0: 524f 5053 0d0a 2020 2020 2020 2020 2020  ROPS..          
+000115f0: 2020 616e 6420 7365 6c66 2e67 6574 4465    and self.getDe
+00011600: 7669 6365 5479 7065 2864 6576 6963 6529  viceType(device)
+00011610: 2069 7320 4465 7669 6365 5479 7065 2e53   is DeviceType.S
+00011620: 7461 7465 4465 7669 6365 0d0a 2020 2020  tateDevice..    
+00011630: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+00011640: 2020 2020 7072 6f70 6572 7469 6573 203d      properties =
+00011650: 2053 5441 5445 5f50 524f 5053 0d0a 0d0a   STATE_PROPS....
+00011660: 2020 2020 2020 2020 6265 666f 7265 203d          before =
+00011670: 205b 7365 6c66 2e67 6574 5072 6f70 6572   [self.getProper
+00011680: 7479 2864 6576 6963 652c 2070 2920 666f  ty(device, p) fo
+00011690: 7220 7020 696e 2070 726f 7065 7274 6965  r p in propertie
+000116a0: 735d 0d0a 2020 2020 2020 2020 7769 7468  s]..        with
+000116b0: 205f 626c 6f63 6b53 6967 6e61 6c28 7365   _blockSignal(se
+000116c0: 6c66 2e65 7665 6e74 732c 2073 656c 662e  lf.events, self.
+000116d0: 6576 656e 7473 2e70 726f 7065 7274 7943  events.propertyC
+000116e0: 6861 6e67 6564 293a 0d0a 2020 2020 2020  hanged):..      
+000116f0: 2020 2020 2020 7969 656c 640d 0a20 2020        yield..   
+00011700: 2020 2020 2061 6674 6572 203d 205b 7365       after = [se
+00011710: 6c66 2e67 6574 5072 6f70 6572 7479 2864  lf.getProperty(d
+00011720: 6576 6963 652c 2070 2920 666f 7220 7020  evice, p) for p 
+00011730: 696e 2070 726f 7065 7274 6965 735d 0d0a  in properties]..
+00011740: 2020 2020 2020 2020 6966 2062 6566 6f72          if befor
+00011750: 6520 213d 2061 6674 6572 3a0d 0a20 2020  e != after:..   
+00011760: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
+00011770: 7661 6c20 696e 2065 6e75 6d65 7261 7465  val in enumerate
+00011780: 2861 6674 6572 293a 0d0a 2020 2020 2020  (after):..      
+00011790: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+000117a0: 7665 6e74 732e 7072 6f70 6572 7479 4368  vents.propertyCh
+000117b0: 616e 6765 642e 656d 6974 2864 6576 6963  anged.emit(devic
+000117c0: 652c 2070 726f 7065 7274 6965 735b 695d  e, properties[i]
+000117d0: 2c20 7661 6c29 0d0a 0d0a 2020 2020 4063  , val)....    @c
+000117e0: 6f6e 7465 7874 6d61 6e61 6765 720d 0a20  ontextmanager.. 
+000117f0: 2020 2064 6566 2073 6574 436f 6e74 6578     def setContex
+00011800: 7428 7365 6c66 2c20 2a2a 6b77 6172 6773  t(self, **kwargs
+00011810: 3a20 416e 7929 202d 3e20 4974 6572 6174  : Any) -> Iterat
+00011820: 6f72 5b4e 6f6e 655d 3a0d 0a20 2020 2020  or[None]:..     
+00011830: 2020 2022 2222 5365 7420 636f 7265 2070     """Set core p
+00011840: 726f 7065 7274 6965 7320 696e 2061 2063  roperties in a c
+00011850: 6f6e 7465 7874 2072 6573 746f 7269 6e67  ontext restoring
+00011860: 2074 6865 2069 6e69 7469 616c 2076 616c   the initial val
+00011870: 7565 7320 6f6e 2065 7869 742e 0d0a 0d0a  ues on exit.....
+00011880: 2020 2020 2020 2020 3a73 7061 726b 6c65          :sparkle
+00011890: 733a 202a 5468 6973 206d 6574 686f 6420  s: *This method 
+000118a0: 6973 206e 6577 2069 6e20 6043 4d4d 436f  is new in `CMMCo
+000118b0: 7265 506c 7573 602e 2a0d 0a0d 0a20 2020  rePlus`.*....   
+000118c0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+000118d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000118e0: 2d2d 2d0d 0a20 2020 2020 2020 202a 2a6b  ---..        **k
+000118f0: 7761 7267 7320 3a20 416e 790d 0a20 2020  wargs : Any..   
+00011900: 2020 2020 2020 2020 204b 6579 776f 7264           Keyword
+00011910: 2061 7267 756d 656e 7473 206d 6179 2062   arguments may b
+00011920: 6520 616e 7920 604e 616d 6560 2066 6f72  e any `Name` for
+00011930: 2077 6869 6368 2060 6765 743c 4e61 6d65   which `get<Name
+00011940: 3e60 2061 6e64 2060 7365 743c 4e61 6d65  >` and `set<Name
+00011950: 3e60 0d0a 2020 2020 2020 2020 2020 2020  >`..            
+00011960: 6d65 7468 6f64 7320 6578 6973 742e 2020  methods exist.  
+00011970: 466f 7220 6578 616d 706c 652c 2060 7365  For example, `se
+00011980: 7443 6f6e 7465 7874 2865 7870 6f73 7572  tContext(exposur
+00011990: 653d 3130 2960 2077 696c 6c20 6361 6c6c  e=10)` will call
+000119a0: 0d0a 2020 2020 2020 2020 2020 2020 6073  ..            `s
+000119b0: 6574 4578 706f 7375 7265 2831 3029 6020  etExposure(10)` 
+000119c0: 7768 656e 2065 6e74 6572 696e 6720 7468  when entering th
+000119d0: 6520 636f 6e74 6578 7420 616e 6420 6073  e context and `s
+000119e0: 6574 4578 706f 7375 7265 283c 696e 6974  etExposure(<init
+000119f0: 6961 6c3e 2960 0d0a 2020 2020 2020 2020  ial>)`..        
+00011a00: 2020 2020 7768 656e 2065 7869 7469 6e67      when exiting
+00011a10: 2074 6865 2063 6f6e 7465 7874 2e0d 0a0d   the context....
+00011a20: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+00011a30: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00011a40: 2d2d 2d0d 0a20 2020 2020 2020 2060 6060  ---..        ```
+00011a50: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
+00011a60: 636f 7265 203d 2043 4d4d 436f 7265 506c  core = CMMCorePl
+00011a70: 7573 2e69 6e73 7461 6e63 6528 290d 0a0d  us.instance()...
+00011a80: 0a20 2020 2020 2020 2077 6974 6820 636f  .        with co
+00011a90: 7265 2e73 6574 436f 6e74 6578 7428 6175  re.setContext(au
+00011aa0: 746f 5368 7574 7465 723d 4661 6c73 6529  toShutter=False)
+00011ab0: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
+00011ac0: 7373 6572 7420 6e6f 7420 636f 7265 2e67  ssert not core.g
+00011ad0: 6574 4175 746f 5368 7574 7465 7228 290d  etAutoShutter().
+00011ae0: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
+00011af0: 6f20 6f74 6865 7220 7374 7566 660d 0a20  o other stuff.. 
+00011b00: 2020 2020 2020 2020 2020 202e 2e2e 0d0a             .....
+00011b10: 0d0a 2020 2020 2020 2020 2320 6175 746f  ..        # auto
+00011b20: 5368 7574 7465 7220 6973 2072 6573 746f  Shutter is resto
+00011b30: 7265 6420 746f 2069 7473 206f 7269 6769  red to its origi
+00011b40: 6e61 6c20 7661 6c75 6520 7768 656e 2074  nal value when t
+00011b50: 6865 2063 6f6e 7465 7874 2065 7869 7473  he context exits
+00011b60: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00011b70: 2063 6f72 652e 6765 7441 7574 6f53 6875   core.getAutoShu
+00011b80: 7474 6572 2829 0d0a 2020 2020 2020 2020  tter()..        
+00011b90: 6060 600d 0a20 2020 2020 2020 2022 2222  ```..        """
+00011ba0: 0d0a 2020 2020 2020 2020 6f72 6967 5f76  ..        orig_v
+00011bb0: 616c 7565 7320 3d20 7b7d 0d0a 2020 2020  alues = {}..    
+00011bc0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00011bd0: 2020 2020 2020 666f 7220 6e61 6d65 2c20        for name, 
+00011be0: 7620 696e 206b 7761 7267 732e 6974 656d  v in kwargs.item
+00011bf0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00011c00: 2020 2020 2020 6e61 6d65 203d 206e 616d        name = nam
+00011c10: 655b 305d 2e75 7070 6572 2829 202b 206e  e[0].upper() + n
+00011c20: 616d 655b 313a 5d0d 0a20 2020 2020 2020  ame[1:]..       
+00011c30: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c50: 2020 206f 7269 675f 7661 6c75 6573 5b6e     orig_values[n
+00011c60: 616d 655d 203d 2067 6574 6174 7472 2873  ame] = getattr(s
+00011c70: 656c 662c 2066 2267 6574 7b6e 616d 657d  elf, f"get{name}
+00011c80: 2229 2829 0d0a 2020 2020 2020 2020 2020  ")()..          
+00011c90: 2020 2020 2020 2020 2020 6765 7461 7474            getatt
+00011ca0: 7228 7365 6c66 2c20 6622 7365 747b 6e61  r(self, f"set{na
+00011cb0: 6d65 7d22 2928 7629 0d0a 2020 2020 2020  me}")(v)..      
+00011cc0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00011cd0: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
+00011ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011cf0: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+00011d00: 6e69 6e67 2866 227b 6e61 6d65 7d20 6973  ning(f"{name} is
+00011d10: 206e 6f74 2061 2076 616c 6964 2070 726f   not a valid pro
+00011d20: 7065 7274 792c 2073 6b69 7070 696e 672e  perty, skipping.
+00011d30: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00011d40: 7969 656c 640d 0a20 2020 2020 2020 2066  yield..        f
+00011d50: 696e 616c 6c79 3a0d 0a20 2020 2020 2020  inally:..       
+00011d60: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
+00011d70: 206f 7269 675f 7661 6c75 6573 2e69 7465   orig_values.ite
+00011d80: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00011d90: 2020 2020 2020 2077 6974 6820 7375 7070         with supp
+00011da0: 7265 7373 2841 7474 7269 6275 7465 4572  ress(AttributeEr
+00011db0: 726f 7229 3a0d 0a20 2020 2020 2020 2020  ror):..         
+00011dc0: 2020 2020 2020 2020 2020 2067 6574 6174             getat
+00011dd0: 7472 2873 656c 662c 2066 2273 6574 7b6b  tr(self, f"set{k
+00011de0: 7d22 2928 7629 0d0a 0d0a 2020 2020 6465  }")(v)....    de
+00011df0: 6620 6361 6e53 6571 7565 6e63 6545 7665  f canSequenceEve
+00011e00: 6e74 7328 0d0a 2020 2020 2020 2020 7365  nts(..        se
+00011e10: 6c66 2c20 6531 3a20 4d44 4145 7665 6e74  lf, e1: MDAEvent
+00011e20: 2c20 6532 3a20 4d44 4145 7665 6e74 2c20  , e2: MDAEvent, 
+00011e30: 6375 725f 6c65 6e67 7468 3a20 696e 7420  cur_length: int 
+00011e40: 3d20 2d31 0d0a 2020 2020 2920 2d3e 2062  = -1..    ) -> b
+00011e50: 6f6f 6c3a 0d0a 2020 2020 2020 2020 2222  ool:..        ""
+00011e60: 2243 6865 636b 2077 6865 7468 6572 2074  "Check whether t
+00011e70: 776f 205b 6075 7365 712e 4d44 4145 7665  wo [`useq.MDAEve
+00011e80: 6e74 605d 5b5d 2061 7265 2073 6571 7565  nt`][] are seque
+00011e90: 6e63 6561 626c 6520 6279 2074 6869 7320  nceable by this 
+00011ea0: 636f 7265 2069 6e73 7461 6e63 652e 0d0a  core instance...
+00011eb0: 0d0a 2020 2020 2020 2020 4d69 6372 6f2d  ..        Micro-
+00011ec0: 6d61 6e61 6765 7220 6361 6c6c 7320 6861  manager calls ha
+00011ed0: 7264 7761 7265 2074 7269 6767 6572 696e  rdware triggerin
+00011ee0: 6720 2273 6571 7565 6e63 696e 6722 2e20  g "sequencing". 
+00011ef0: 2054 776f 2065 7665 6e74 7320 6361 6e20   Two events can 
+00011f00: 6265 0d0a 2020 2020 2020 2020 7365 7175  be..        sequ
+00011f10: 656e 6365 6420 6966 202a 616c 6c2a 2064  enced if *all* d
+00011f20: 6576 6963 6520 7072 6f70 6572 7469 6573  evice properties
+00011f30: 2074 6861 7420 6172 6520 6368 616e 6769   that are changi
+00011f40: 6e67 2062 6574 7765 656e 2074 6865 2066  ng between the f
+00011f50: 6972 7374 2061 6e64 0d0a 2020 2020 2020  irst and..      
+00011f60: 2020 7365 636f 6e64 2065 7665 6e74 2073    second event s
+00011f70: 7570 706f 7274 2073 6571 7565 6e63 696e  upport sequencin
+00011f80: 672e 0d0a 0d0a 2020 2020 2020 2020 4966  g.....        If
+00011f90: 2060 6375 725f 6c65 6e67 7468 6020 6973   `cur_length` is
+00011fa0: 2070 726f 7669 6465 642c 2069 7420 6973   provided, it is
+00011fb0: 2075 7365 6420 746f 2064 6574 6572 6d69   used to determi
+00011fc0: 6e65 2069 6620 7468 6520 7365 7175 656e  ne if the sequen
+00011fd0: 6365 2069 730d 0a20 2020 2020 2020 2022  ce is..        "
+00011fe0: 6675 6c6c 2220 2869 2e65 2e20 7468 6520  full" (i.e. the 
+00011ff0: 7365 7175 656e 6365 2069 7320 616c 7265  sequence is alre
+00012000: 6164 7920 6174 2074 6865 206d 6178 696d  ady at the maxim
+00012010: 756d 206c 656e 6774 6829 2061 7320 6465  um length) as de
+00012020: 7465 726d 696e 6564 2062 790d 0a20 2020  termined by..   
+00012030: 2020 2020 2074 6865 2060 2e2e 2e53 6571       the `...Seq
+00012040: 7565 6e63 654d 6178 4c65 6e67 7468 2829  uenceMaxLength()
+00012050: 6020 6d65 7468 6f64 2063 6f72 7265 7370  ` method corresp
+00012060: 6f6e 6469 6e67 2074 6f20 7468 6520 6465  onding to the de
+00012070: 7669 6365 2070 726f 7065 7274 792e 0d0a  vice property...
+00012080: 0d0a 2020 2020 2020 2020 5365 653a 203c  ..        See: <
+00012090: 6874 7470 733a 2f2f 6d69 6372 6f2d 6d61  https://micro-ma
+000120a0: 6e61 6765 722e 6f72 672f 4861 7264 7761  nager.org/Hardwa
+000120b0: 7265 2d62 6173 6564 5f53 796e 6368 726f  re-based_Synchro
+000120c0: 6e69 7a61 7469 6f6e 5f69 6e5f 4d69 6372  nization_in_Micr
+000120d0: 6f2d 4d61 6e61 6765 723e 0d0a 0d0a 2020  o-Manager>....  
+000120e0: 2020 2020 2020 3a73 7061 726b 6c65 733a        :sparkles:
+000120f0: 202a 5468 6973 206d 6574 686f 6420 6973   *This method is
+00012100: 206e 6577 2069 6e20 6043 4d4d 436f 7265   new in `CMMCore
+00012110: 506c 7573 602e 2a0d 0a0d 0a20 2020 2020  Plus`.*....     
+00012120: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+00012130: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00012140: 2d0d 0a20 2020 2020 2020 2065 3120 3a20  -..        e1 : 
+00012150: 4d44 4145 7665 6e74 0d0a 2020 2020 2020  MDAEvent..      
+00012160: 2020 2020 2020 5468 6520 6669 7273 7420        The first 
+00012170: 6576 656e 742e 0d0a 2020 2020 2020 2020  event...        
+00012180: 6532 203a 204d 4441 4576 656e 740d 0a20  e2 : MDAEvent.. 
+00012190: 2020 2020 2020 2020 2020 2054 6865 2073             The s
+000121a0: 6563 6f6e 6420 6576 656e 742e 0d0a 2020  econd event...  
+000121b0: 2020 2020 2020 6375 725f 6c65 6e67 7468        cur_length
+000121c0: 203a 2069 6e74 0d0a 2020 2020 2020 2020   : int..        
+000121d0: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
+000121e0: 6c65 6e67 7468 206f 6620 7468 6520 7365  length of the se
+000121f0: 7175 656e 6365 2e20 2055 7365 6420 7768  quence.  Used wh
+00012200: 656e 2063 6865 636b 696e 670d 0a20 2020  en checking..   
+00012210: 2020 2020 2020 2020 2060 2e67 6574 3c2e           `.get<.
+00012220: 2e2e 3e53 6571 7565 6e63 654d 6178 4c65  ..>SequenceMaxLe
+00012230: 6e67 7468 6020 666f 7220 6120 6769 7665  ngth` for a give
+00012240: 6e20 7072 6f70 6572 7479 2e20 4966 2074  n property. If t
+00012250: 6865 2063 7572 7265 6e74 206c 656e 6774  he current lengt
+00012260: 680d 0a20 2020 2020 2020 2020 2020 2069  h..            i
+00012270: 7320 6772 6561 7465 7220 7468 616e 2074  s greater than t
+00012280: 6865 206d 6178 206c 656e 6774 682c 2074  he max length, t
+00012290: 6865 2065 7665 6e74 7320 6361 6e6e 6f74  he events cannot
+000122a0: 2062 6520 7365 7175 656e 6365 642e 2042   be sequenced. B
+000122b0: 7920 6465 6661 756c 740d 0a20 2020 2020  y default..     
+000122c0: 2020 2020 2020 202d 312c 2077 6869 6368         -1, which
+000122d0: 206d 6561 6e73 2074 6865 2063 7572 7265   means the curre
+000122e0: 6e74 206c 656e 6774 6820 6973 206e 6f74  nt length is not
+000122f0: 2063 6865 636b 6564 2e0d 0a0d 0a20 2020   checked.....   
+00012300: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+00012310: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+00012320: 2020 2020 2020 2062 6f6f 6c0d 0a20 2020         bool..   
+00012330: 2020 2020 2020 2020 2054 7275 6520 6966           True if
+00012340: 2074 6865 2065 7665 6e74 7320 6361 6e20   the events can 
+00012350: 6265 2073 6571 7565 6e63 6564 2c20 4661  be sequenced, Fa
+00012360: 6c73 6520 6f74 6865 7277 6973 652e 0d0a  lse otherwise...
+00012370: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+00012380: 6573 0d0a 2020 2020 2020 2020 2d2d 2d2d  es..        ----
+00012390: 2d2d 2d2d 0d0a 2020 2020 2020 2020 2121  ----..        !!
+000123a0: 2120 6e6f 7465 0d0a 0d0a 2020 2020 2020  ! note....      
+000123b0: 2020 2020 2020 5468 6520 7265 7375 6c74        The result
+000123c0: 7320 6865 7265 2077 696c 6c20 6465 7065  s here will depe
+000123d0: 6e64 206f 6e20 7468 6520 6375 7272 656e  nd on the curren
+000123e0: 7420 7374 6174 6520 6f66 2074 6865 2063  t state of the c
+000123f0: 6f72 6520 616e 6420 6465 7669 6365 732e  ore and devices.
+00012400: 0d0a 0d0a 2020 2020 2020 2020 6060 6070  ....        ```p
+00012410: 7974 686f 6e0d 0a20 2020 2020 2020 203e  ython..        >
+00012420: 3e3e 2066 726f 6d20 7573 6571 2069 6d70  >> from useq imp
+00012430: 6f72 7420 4d44 4145 7665 6e74 0d0a 2020  ort MDAEvent..  
+00012440: 2020 2020 2020 3e3e 3e20 636f 7265 203d        >>> core =
+00012450: 2043 4d4d 436f 7265 506c 7573 2e69 6e73   CMMCorePlus.ins
+00012460: 7461 6e63 6528 290d 0a20 2020 2020 2020  tance()..       
+00012470: 203e 3e3e 2063 6f72 652e 6c6f 6164 5379   >>> core.loadSy
+00012480: 7374 656d 436f 6e66 6967 7572 6174 696f  stemConfiguratio
+00012490: 6e28 290d 0a20 2020 2020 2020 203e 3e3e  n()..        >>>
+000124a0: 2063 6f72 652e 6361 6e53 6571 7565 6e63   core.canSequenc
+000124b0: 6545 7665 6e74 7328 4d44 4145 7665 6e74  eEvents(MDAEvent
+000124c0: 2829 2c20 4d44 4145 7665 6e74 2829 290d  (), MDAEvent()).
+000124d0: 0a20 2020 2020 2020 2054 7275 650d 0a20  .        True.. 
+000124e0: 2020 2020 2020 203e 3e3e 2063 6f72 652e         >>> core.
+000124f0: 6361 6e53 6571 7565 6e63 6545 7665 6e74  canSequenceEvent
+00012500: 7328 4d44 4145 7665 6e74 2878 5f70 6f73  s(MDAEvent(x_pos
+00012510: 3d31 292c 204d 4441 4576 656e 7428 785f  =1), MDAEvent(x_
+00012520: 706f 733d 3229 290d 0a20 2020 2020 2020  pos=2))..       
+00012530: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00012540: 3e3e 3e20 636f 7265 2e63 616e 5365 7175  >>> core.canSequ
+00012550: 656e 6365 4576 656e 7473 280d 0a20 2020  enceEvents(..   
+00012560: 2020 2020 202e 2e2e 2020 2020 204d 4441       ...     MDA
+00012570: 4576 656e 7428 6368 616e 6e65 6c3d 7b27  Event(channel={'
+00012580: 636f 6e66 6967 273a 2027 4441 5049 277d  config': 'DAPI'}
+00012590: 292c 0d0a 2020 2020 2020 2020 2e2e 2e20  ),..        ... 
+000125a0: 2020 2020 4d44 4145 7665 6e74 2863 6861      MDAEvent(cha
+000125b0: 6e6e 656c 3d7b 2763 6f6e 6669 6727 3a20  nnel={'config': 
+000125c0: 2746 4954 4327 7d29 0d0a 2020 2020 2020  'FITC'})..      
+000125d0: 2020 2e2e 2e20 290d 0a20 2020 2020 2020    ... )..       
+000125e0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+000125f0: 6060 600d 0a20 2020 2020 2020 2022 2222  ```..        """
+00012600: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00012610: 2063 616e 5f73 6571 7565 6e63 655f 6576   can_sequence_ev
+00012620: 656e 7473 2873 656c 662c 2065 312c 2065  ents(self, e1, e
+00012630: 322c 2063 7572 5f6c 656e 6774 6829 0d0a  2, cur_length)..
+00012640: 0d0a 0d0a 666f 7220 6e61 6d65 2069 6e20  ....for name in 
+00012650: 280d 0a20 2020 2022 6765 7443 6f6e 6669  (..    "getConfi
+00012660: 6744 6174 6122 2c0d 0a20 2020 2022 6765  gData",..    "ge
+00012670: 7443 6f6e 6669 6747 726f 7570 5374 6174  tConfigGroupStat
+00012680: 6522 2c0d 0a20 2020 2022 6765 7443 6f6e  e",..    "getCon
+00012690: 6669 6747 726f 7570 5374 6174 6546 726f  figGroupStateFro
+000126a0: 6d43 6163 6865 222c 0d0a 2020 2020 2267  mCache",..    "g
+000126b0: 6574 436f 6e66 6967 5374 6174 6522 2c0d  etConfigState",.
+000126c0: 0a20 2020 2022 6765 7453 7973 7465 6d53  .    "getSystemS
+000126d0: 7461 7465 222c 0d0a 2020 2020 2267 6574  tate",..    "get
+000126e0: 5379 7374 656d 5374 6174 6543 6163 6865  SystemStateCache
+000126f0: 222c 0d0a 293a 0d0a 2020 2020 6e61 7469  ",..):..    nati
+00012700: 7665 5f64 6f63 203d 2067 6574 6174 7472  ve_doc = getattr
+00012710: 2870 796d 6d63 6f72 652e 434d 4d43 6f72  (pymmcore.CMMCor
+00012720: 652c 206e 616d 6529 2e5f 5f64 6f63 5f5f  e, name).__doc__
+00012730: 0d0a 2020 2020 6765 7461 7474 7228 434d  ..    getattr(CM
+00012740: 4d43 6f72 6550 6c75 732c 206e 616d 6529  MCorePlus, name)
+00012750: 2e5f 5f64 6f63 5f5f 202b 3d20 280d 0a20  .__doc__ += (.. 
+00012760: 2020 2020 2020 2022 5c6e 220d 0a20 2020         "\n"..   
+00012770: 2020 2020 202b 206e 6174 6976 655f 646f       + native_do
+00012780: 630d 0a20 2020 2020 2020 202b 2064 6564  c..        + ded
+00012790: 656e 7428 0d0a 2020 2020 2020 2020 2020  ent(..          
+000127a0: 2020 2222 220d 0a20 2020 2042 7920 6465    """..    By de
+000127b0: 6661 756c 742c 2074 6869 7320 6d65 7468  fault, this meth
+000127c0: 6f64 2072 6574 7572 6e73 2061 2060 7079  od returns a `py
+000127d0: 6d6d 636f 7265 5f70 6c75 732e 436f 6e66  mmcore_plus.Conf
+000127e0: 6967 7572 6174 696f 6e60 206f 626a 6563  iguration` objec
+000127f0: 742c 2077 6869 6368 0d0a 2020 2020 7072  t, which..    pr
+00012800: 6f76 6964 6573 2073 6f6d 6520 636f 6e76  ovides some conv
+00012810: 656e 6965 6e63 6573 206f 7665 7220 7468  eniences over th
+00012820: 6520 6e61 7469 7665 2060 7079 6d6d 636f  e native `pymmco
+00012830: 7265 2e43 6f6e 6669 6775 7261 7469 6f6e  re.Configuration
+00012840: 6020 6f62 6a65 6374 2c20 686f 7765 7665  ` object, howeve
+00012850: 720d 0a20 2020 2074 6869 7320 6164 6473  r..    this adds
+00012860: 2061 206c 6974 746c 6520 6f76 6572 6865   a little overhe
+00012870: 6164 2e20 5573 6520 606e 6174 6976 653d  ad. Use `native=
+00012880: 5472 7565 6020 746f 2061 766f 6964 2074  True` to avoid t
+00012890: 6865 2063 6f6e 7665 7273 696f 6e2e 0d0a  he conversion...
+000128a0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000128b0: 2029 2e73 7472 6970 2829 0d0a 2020 2020   ).strip()..    
+000128c0: 290d 0a0d 0a0d 0a63 6c61 7373 205f 4d4d  )......class _MM
+000128d0: 4361 6c6c 6261 636b 5265 6c61 7928 7079  CallbackRelay(py
+000128e0: 6d6d 636f 7265 2e4d 4d45 7665 6e74 4361  mmcore.MMEventCa
+000128f0: 6c6c 6261 636b 293a 0d0a 2020 2020 2222  llback):..    ""
+00012900: 2252 656c 6179 7320 4d4d 4576 656e 7443  "Relays MMEventC
+00012910: 616c 6c62 6163 6b20 6d65 7468 6f64 7320  allback methods 
+00012920: 746f 2043 4d4d 436f 7265 506c 7573 2e73  to CMMCorePlus.s
+00012930: 6967 6e61 6c2e 2222 220d 0a0d 0a20 2020  ignal."""....   
+00012940: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00012950: 6c66 2c20 656d 6974 7465 723a 2043 4d4d  lf, emitter: CMM
+00012960: 436f 7265 5369 676e 616c 6572 293a 0d0a  CoreSignaler):..
+00012970: 2020 2020 2020 2020 7365 6c66 2e5f 656d          self._em
+00012980: 6974 7465 7220 3d20 656d 6974 7465 720d  itter = emitter.
+00012990: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+000129a0: 2e5f 5f69 6e69 745f 5f28 290d 0a0d 0a20  .__init__().... 
+000129b0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+000129c0: 0d0a 2020 2020 6465 6620 5f6d 616b 655f  ..    def _make_
+000129d0: 7265 656d 6974 7465 7228 6e61 6d65 3a20  reemitter(name: 
+000129e0: 7374 7229 202d 3e20 4361 6c6c 6162 6c65  str) -> Callable
+000129f0: 5b2e 2e2e 2c20 4e6f 6e65 5d3a 0d0a 2020  [..., None]:..  
+00012a00: 2020 2020 2020 7369 675f 6e61 6d65 203d        sig_name =
+00012a10: 206e 616d 655b 325d 2e6c 6f77 6572 2829   name[2].lower()
+00012a20: 202b 206e 616d 655b 333a 5d0d 0a0d 0a20   + name[3:].... 
+00012a30: 2020 2020 2020 2064 6566 2072 6565 6d69         def reemi
+00012a40: 7428 7365 6c66 3a20 5f4d 4d43 616c 6c62  t(self: _MMCallb
+00012a50: 6163 6b52 656c 6179 2c20 2a61 7267 733a  ackRelay, *args:
+00012a60: 2041 6e79 2920 2d3e 204e 6f6e 653a 0d0a   Any) -> None:..
+00012a70: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00012a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012a90: 2020 6765 7461 7474 7228 7365 6c66 2e5f    getattr(self._
+00012aa0: 656d 6974 7465 722c 2073 6967 5f6e 616d  emitter, sig_nam
+00012ab0: 6529 2e65 6d69 7428 2a61 7267 7329 0d0a  e).emit(*args)..
+00012ac0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00012ad0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00012ae0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00012af0: 2020 2020 6c6f 6767 6572 2e65 7272 6f72      logger.error
+00012b00: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00012b10: 2020 2020 2020 2066 2245 7863 6570 7469         f"Excepti
+00012b20: 6f6e 206f 6363 7572 7265 6420 696e 204d  on occurred in M
+00012b30: 4d43 6f72 6550 6c75 7320 6361 6c6c 6261  MCorePlus callba
+00012b40: 636b 207b 7369 675f 6e61 6d65 2172 7d3a  ck {sig_name!r}:
+00012b50: 207b 657d 220d 0a20 2020 2020 2020 2020   {e}"..         
+00012b60: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00012b70: 2020 2020 7265 7475 726e 2072 6565 6d69      return reemi
+00012b80: 740d 0a0d 0a0d 0a4d 4d43 616c 6c62 6163  t......MMCallbac
+00012b90: 6b52 656c 6179 203d 2074 7970 6528 0d0a  kRelay = type(..
+00012ba0: 2020 2020 224d 4d43 616c 6c62 6163 6b52      "MMCallbackR
+00012bb0: 656c 6179 222c 0d0a 2020 2020 285f 4d4d  elay",..    (_MM
+00012bc0: 4361 6c6c 6261 636b 5265 6c61 792c 292c  CallbackRelay,),
+00012bd0: 0d0a 2020 2020 7b0d 0a20 2020 2020 2020  ..    {..       
+00012be0: 206e 3a20 5f4d 4d43 616c 6c62 6163 6b52   n: _MMCallbackR
+00012bf0: 656c 6179 2e5f 6d61 6b65 5f72 6565 6d69  elay._make_reemi
+00012c00: 7474 6572 286e 290d 0a20 2020 2020 2020  tter(n)..       
+00012c10: 2066 6f72 206e 2069 6e20 6469 7228 7079   for n in dir(py
+00012c20: 6d6d 636f 7265 2e4d 4d45 7665 6e74 4361  mmcore.MMEventCa
+00012c30: 6c6c 6261 636b 290d 0a20 2020 2020 2020  llback)..       
+00012c40: 2069 6620 6e2e 7374 6172 7473 7769 7468   if n.startswith
+00012c50: 2822 6f6e 2229 0d0a 2020 2020 7d2c 0d0a  ("on")..    },..
+00012c60: 290d 0a                                  )..
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_property.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_property.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_sequencing.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/_sequencing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from itertools import product
 from typing import TYPE_CHECKING, Literal, Sequence, Tuple, overload
 
-from pydantic import root_validator
 from useq import MDAEvent
 
 from pymmcore_plus.core._constants import DeviceType
 
 if TYPE_CHECKING:
     from pymmcore_plus import CMMCorePlus
 
@@ -15,20 +14,20 @@
 class SequencedEvent(MDAEvent):
     """Subclass of MDAEvent that represents a sequence of triggered events.
 
     Prefer instantiating this class via the `create` classmethod, which will
     calculate sequences for x, y, z, and exposure based on an a sequence of events.
     """
 
-    events: Tuple[MDAEvent, ...]  # noqa: UP
+    events: Tuple[MDAEvent, ...]  # noqa: UP006
 
-    exposure_sequence: Tuple[float, ...]  # noqa: UP
-    x_sequence: Tuple[float, ...]  # noqa: UP
-    y_sequence: Tuple[float, ...]  # noqa: UP
-    z_sequence: Tuple[float, ...]  # noqa: UP
+    exposure_sequence: Tuple[float, ...]  # noqa: UP006
+    x_sequence: Tuple[float, ...]  # noqa: UP006
+    y_sequence: Tuple[float, ...]  # noqa: UP006
+    z_sequence: Tuple[float, ...]  # noqa: UP006
 
     # technically this is more like a field, but it requires a core instance
     # to getConfigData for channels, so we leave it as a method.
     def property_sequences(self, core: CMMCorePlus) -> dict[tuple[str, str], list[str]]:
         """Return a dict of all sequenceable properties and their sequences.
 
         Returns
@@ -68,33 +67,35 @@
 
         data: dict[str, list] = {a: [] for a in ("z_pos", "x_pos", "y_pos", "exposure")}
         for event, attr in product(_events, list(data)):
             # do we need to check if not None?
             # the only problem might occur if some are None and some are not
             data[attr].append(getattr(event, attr))
 
+        x_seq = data["x_pos"] if len(set(data["x_pos"])) > 1 else ()
+        y_seq = data["y_pos"] if len(set(data["y_pos"])) > 1 else ()
+        if len(x_seq) != len(y_seq):  # pragma: no cover
+            raise ValueError(
+                "X and Y sequences must be the same length: "
+                f"{len(x_seq)=}, {len(y_seq)=}"
+            )
+
+        e0 = _events[0]
         return cls(
             events=_events,
             exposure_sequence=(
                 data["exposure"] if len(set(data["exposure"])) > 1 else ()
             ),
-            x_sequence=data["x_pos"] if len(set(data["x_pos"])) > 1 else (),
-            y_sequence=data["y_pos"] if len(set(data["y_pos"])) > 1 else (),
+            x_sequence=x_seq,
+            y_sequence=y_seq,
             z_sequence=data["z_pos"] if len(set(data["z_pos"])) > 1 else (),
             # use the first event to provide all other values like min_start_time, etc.
-            **_events[0].dict(),
+            **(e0.model_dump() if hasattr(e0, "model_dump") else e0.dict()),
         )
 
-    @root_validator()
-    @classmethod
-    def _validate_root(cls, value: dict) -> dict:
-        if len(value.get("x_sequence", ())) != len(value.get("y_sequence", ())):
-            raise ValueError("x_sequence and y_sequence must be the same length")
-        return value
-
 
 def get_all_sequenceable(core: CMMCorePlus) -> dict[tuple[str | DeviceType, str], int]:
     """Return all sequenceable devices in `core`.
 
     This is just a convenience function to help determine which devices can be
     sequenced on a given configuration.
 
@@ -224,42 +225,41 @@
     ```
     """
 
     def _nope(reason: str) -> tuple[bool, str] | bool:
         return (False, reason) if return_reason else False
 
     # channel
-    if e1.channel and e2.channel and (e1.channel != e2.channel):
-        if e1.channel.group != e2.channel.group:
+    if e1.channel and e1.channel != e2.channel:
+        if not e2.channel or e1.channel.group != e2.channel.group:
+            e2_channel_group = getattr(e2.channel, "group", None)
             return _nope(
                 "Cannot sequence across config groups: "
-                f"{e1.channel.group=}, {e2.channel.group=}"
+                f"{e1.channel.group=}, {e2_channel_group=}"
             )
         cfg = core.getConfigData(e1.channel.group, e1.channel.config)
         for dev, prop, _ in cfg:
             # note: we don't need _ here, so can perhaps speed up with native=True
             if not core.isPropertySequenceable(dev, prop):
                 return _nope(f"'{dev}-{prop}' is not sequenceable")
             max_len = core.getPropertySequenceMaxLength(dev, prop)
             if cur_length >= max_len:  # pragma: no cover
                 return _nope(f"'{dev}-{prop}' {max_len=} < {cur_length=}")
 
     # Z
-    if (e1.z_pos or e2.z_pos) and (e1.z_pos != e2.z_pos):
+    if e1.z_pos != e2.z_pos:
         focus_dev = core.getFocusDevice()
         if not core.isStageSequenceable(focus_dev):
             return _nope(f"Focus device {focus_dev!r} is not sequenceable")
         max_len = core.getStageSequenceMaxLength(focus_dev)
         if cur_length >= max_len:  # pragma: no cover
             return _nope(f"Focus device {focus_dev!r} {max_len=} < {cur_length=}")
 
     # XY
-    if ((e1.x_pos or e2.x_pos) and (e1.x_pos != e2.x_pos)) or (
-        (e1.y_pos or e2.y_pos) and (e1.y_pos != e2.y_pos)
-    ):
+    if e1.x_pos != e2.x_pos or e1.y_pos != e2.y_pos:
         stage = core.getXYStageDevice()
         if not core.isXYStageSequenceable(stage):
             return _nope(f"XYStage {stage!r} is not sequenceable")
         max_len = core.getXYStageSequenceMaxLength(stage)
         if cur_length >= max_len:  # pragma: no cover
             return _nope(f"XYStage {stage!r} {max_len=} < {cur_length=}")
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/__init__.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import TYPE_CHECKING, Any, List, Type
 
-from ..._util import _qt_app_is_running
+from pymmcore_plus._util import _qt_app_is_running
+
 from ._protocol import PCoreSignaler
 from ._psygnal import CMMCoreSignaler
 
 if TYPE_CHECKING:
-    from ._qsignals import QCoreSignaler
+    from ._qsignals import QCoreSignaler  # noqa: TCH004
+
 
 __all__ = [
     "CMMCoreSignaler",
     "QCoreSignaler",
     "PCoreSignaler",
     "_get_auto_core_callback_class",
     "_denormalize_slot",
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_device_signal_view.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_device_signal_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
-    from .. import CMMCorePlus
+    from pymmcore_plus.core import CMMCorePlus
 
 from ._prop_event_mixin import _C
 
 
 class _DevicePropValueSignal:
     def __init__(
         self, device_label: str, property_name: Optional[str], mmcore: "CMMCorePlus"
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_norm_slot.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_norm_slot.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_prop_event_mixin.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_prop_event_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,41 +47,42 @@
         """
         slot = normalize_slot(callback)
         key = (self._device, self._property, slot)
 
         def _wrapper(dev: str, prop: str, new_value: Any) -> None:
             cb = denormalize_slot(slot)
             if cb is None:
-                self._events._prop_callbacks.pop(key, None)
+                self._events.property_callbacks.pop(key, None)
                 return
             if dev == self._device:
                 if self._property:
                     if prop == self._property:
                         cb(new_value)
                 else:
                     cb(prop, new_value)
 
-        self._events._prop_callbacks[key] = _wrapper
+        self._events.property_callbacks[key] = _wrapper
         self._events.propertyChanged.connect(_wrapper)
         return callback
 
     def disconnect(self, callback: Callable) -> None:
         """Disconnect `callback` from this device and/or property."""
         key = (self._device, self._property, normalize_slot(callback))
-        cb = self._events._prop_callbacks.pop(key, None)
+        cb = self._events.property_callbacks.pop(key, None)
         if cb is None:
             raise ValueError("callback not connected")
         self._events.propertyChanged.disconnect(cb)
 
     def emit(self, *args: Any) -> Any:
         raise NotImplementedError("emit not implemented for _PropertySignal")
 
 
 class _DevicePropertyEventMixin(PCoreSignaler):
-    _prop_callbacks: ClassVar[PropKeyDict] = {}
+    # dict used above by _PropertySignal
+    property_callbacks: ClassVar[PropKeyDict] = {}
 
     def devicePropertyChanged(
         self, device: str, property: str | None = None
     ) -> _PropertySignal:
         """Return object to connect/disconnect to device/property-specific changes.
 
         Note that the callback provided to `.connect()` must take *two* parameters
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_protocol.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_psygnal.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_psygnal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from psygnal import Signal, SignalInstance
 
-from ...mda import MDAEngine
+from pymmcore_plus.mda import MDAEngine
+
 from ._prop_event_mixin import _DevicePropertyEventMixin
 
 
 class CMMCoreSignaler(_DevicePropertyEventMixin):
     """Signals that will be emitted from CMMCorePlus objects."""
 
     # native MMCore callback events
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_qsignals.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/core/events/_qsignals.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     configDeleted = Signal(str, str)
     configDefined = Signal(str, str, str, str, str)
     roiSet = Signal(str, int, int, int, int)
 
     # can't use _DevicePropertyEventMixin due to metaclass conflict
     def __init__(self) -> None:
         super().__init__()
-        self._prop_callbacks: PropKeyDict = {}
+        self.property_callbacks: PropKeyDict = {}
 
     def devicePropertyChanged(
         self, device: str, property: Optional[str] = None
     ) -> _PropertySignal:
         """Return object to connect/disconnect to device/property-specific changes.
 
         Note that the callback provided to `.connect()` must take *two* parameters
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_engine.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/mda/_runner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,278 +1,314 @@
 from __future__ import annotations
 
+import contextlib
 import time
-from typing import TYPE_CHECKING, Iterable, Iterator, NamedTuple, Sequence, cast
+import warnings
+from typing import TYPE_CHECKING, Iterable, Iterator
 
-import useq
-from useq import MDAEvent, MDASequence
+from psygnal import EmitLoopError
+from useq import MDASequence
 
 from pymmcore_plus._logger import logger
-from pymmcore_plus._util import retry
-from pymmcore_plus.core._sequencing import SequencedEvent
 
 from ._protocol import PMDAEngine
+from .events import PMDASignaler, _get_auto_MDA_callback_class
 
 if TYPE_CHECKING:
-    import numpy as np
-    from useq import HardwareAutofocus
+    from useq import MDAEvent
 
-    from ..core import CMMCorePlus
+    from ._engine import MDAEngine
 
-HardwareAFType = getattr(useq, "HardwareAutofocus", ())  # useq v0.3.0+
+MSG = (
+    "This sequence is a placeholder for a generator of events with unknown "
+    "length & shape. Iterating over it has no effect."
+)
 
 
-class MDAEngine(PMDAEngine):
-    """The default MDAengine that ships with pymmcore-plus.
+class GeneratorMDASequence(MDASequence):
+    axis_order: str = ""
 
-    This implements the [`PMDAEngine`][pymmcore_plus.mda.PMDAEngine] protocol, and
-    uses a [`CMMCorePlus`][pymmcore_plus.CMMCorePlus] instance to control the hardware.
+    @property
+    def sizes(self) -> dict[str, int]:  # pragma: no cover
+        warnings.warn(MSG, stacklevel=2)
+        return {}
+
+    def iter_axis(self, axis: str) -> Iterator:  # pragma: no cover
+        warnings.warn(MSG, stacklevel=2)
+        yield from []
+
+    def __str__(self) -> str:
+        return "GeneratorMDASequence()"
+
+
+class MDARunner:
+    """Object that executes a multi-dimensional experiment using an MDAEngine.
+
+    This object is available at [`CMMCorePlus.mda`][pymmcore_plus.CMMCorePlus.mda].
+
+    This is the main object that runs a multi-dimensional experiment; it does so by
+    driving an acquisition engine that implements the
+    [`PMDAEngine`][pymmcore_plus.mda.PMDAEngine] protocol.  It emits signals at specific
+    times during the experiment (see
+    [`PMDASignaler`][pymmcore_plus.mda.events.PMDASignaler] for details on the signals
+    that are available to connect to and when they are emitted).
     """
 
-    def __init__(self, mmc: CMMCorePlus) -> None:
-        self._mmc = mmc
+    def __init__(self) -> None:
+        self._engine: PMDAEngine | None = None
+        self._signals = _get_auto_MDA_callback_class()()
+        self._running = False
+        self._paused = False
+        self._paused_time: float = 0
+        self._pause_interval: float = 0.1  # sec to wait between checking pause state
+
+        self._canceled = False
+        self._sequence: MDASequence | None = None
+        self._reset_timer()
+
+    def set_engine(self, engine: PMDAEngine) -> PMDAEngine | None:
+        """Set the [`PMDAEngine`][pymmcore_plus.mda.PMDAEngine] to use for the MDA run."""  # noqa: E501
+        if not isinstance(engine, PMDAEngine):
+            raise TypeError("Engine does not conform to the Engine protocol.")
+
+        if self.is_running():
+            raise RuntimeError(
+                "Cannot register a new engine when the current engine is running "
+                "an acquistion. Please cancel the current engine's acquistion "
+                "before registering"
+            )
+
+        old_engine, self._engine = self._engine, engine
+        return old_engine
 
-        # used for one_shot autofocus to store the z correction for each position index.
-        # map of {position_index: z_correction}
-        self._z_correction: dict[int | None, float] = {}
+    # NOTE:
+    # this return annotation is a lie, since the user can set it to their own engine.
+    # but in MOST cases, this is the engine that will be used by default, so it's
+    # convenient for IDEs to point to this rather than the abstract protocol.
+    @property
+    def engine(self) -> MDAEngine | None:
+        """The [`PMDAEngine`][pymmcore_plus.mda.PMDAEngine] that is currently being used."""  # noqa: E501
+        return self._engine  # type: ignore
+
+    @property
+    def events(self) -> PMDASignaler:
+        """Signals that are emitted during the MDA run.
 
-    # ===================== SETUP =====================
+        See [`PMDASignaler`][pymmcore_plus.mda.PMDASignaler] for details on the
+        signals that are available to connect to.
+        """
+        return self._signals
 
-    def setup_sequence(self, sequence: MDASequence) -> None:
-        """Setup the hardware for the entire sequence.
+    def is_running(self) -> bool:
+        """Return True if an acquistion is currently underway.
 
-        (currently, this does nothing but get the global `CMMCorePlus` singleton
-        if one is not already provided).
+        This will return True at any point between the emission of the
+        [`sequenceStarted`][pymmcore_plus.mda.PMDASignaler.sequenceStarted] and
+        [`sequenceFinished`][pymmcore_plus.mda.PMDASignaler.sequenceFinished] signals,
+        including when the acquisition is currently paused.
+
+        Returns
+        -------
+        bool
+            Whether an acquistion is underway.
         """
-        from ..core import CMMCorePlus
+        return self._running
 
-        self._mmc = self._mmc or CMMCorePlus.instance()
+    def is_paused(self) -> bool:
+        """Return True if the acquistion is currently paused.
 
-        # set sequence fov size for grid plans
-        if hasattr(sequence, "set_fov_size"):
-            if px := self._mmc.getPixelSizeUm():
-                _, _, width, height = self._mmc.getROI()
-
-                # set fov to main sequence
-                sequence.set_fov_size((width * px, height * px))
-
-                # set fov to any stage positions sequences
-                if sequence.stage_positions is not None:
-                    for p in sequence.stage_positions:
-                        if p.sequence is not None:
-                            p.sequence.set_fov_size((width * px, height * px))
+        Use `toggle_pause` to change the paused state.
 
-    def setup_event(self, event: MDAEvent) -> None:
-        """Set the system hardware (XY, Z, channel, exposure) as defined in the event.
+        Returns
+        -------
+        bool
+            Whether the current acquistion is paused.
+        """
+        return self._paused
 
-        Parameters
-        ----------
-        event : MDAEvent
-            The event to use for the Hardware config
+    def cancel(self) -> None:
+        """Cancel the currently running acquisition.
+
+        This is a no-op if no acquisition is currently running.
+        If an acquisition is running then this will cancel the acquistion and
+        a sequenceCanceled signal, followed by a sequenceFinished signal will
+        be emitted.
         """
-        if isinstance(event, SequencedEvent):
-            self.setup_sequenced_event(event)
-        else:
-            self.setup_single_event(event)
-        self._mmc.waitForSystem()
-
-    def setup_sequenced_event(self, event: SequencedEvent) -> None:
-        """Setup hardware for a sequenced (triggered) event.
-
-        This method is not part of the PMDAEngine protocol (it is called by
-        `setup_event`, which *is* part of the protocol), but it is made public
-        in case a user wants to subclass this engine and override this method.
+        self._canceled = True
+        self._paused_time = 0
+
+    def toggle_pause(self) -> None:
+        """Toggle the paused state of the current acquisition.
+
+        To get whether the acquisition is currently paused use the
+        [`is_paused`][pymmcore_plus.mda.MDARunner.is_paused] method. This method is a
+        no-op if no acquistion is currently underway.
         """
-        core = self._mmc
-        cam_device = self._mmc.getCameraDevice()
+        if self.is_running():
+            self._paused = not self._paused
+            self._signals.sequencePauseToggled.emit(self._paused)
+
+    def run(self, events: Iterable[MDAEvent]) -> None:
+        """Run the multi-dimensional acquistion defined by `sequence`.
+
+        Most users should not use this directly as it will block further
+        execution. Instead, use the
+        [`CMMCorePlus.run_mda`][pymmcore_plus.CMMCorePlus.run_mda] method which will
+        run on a thread.
 
-        if event.exposure_sequence:
-            core.loadExposureSequence(cam_device, event.exposure_sequence)
-        if event.x_sequence:  # y_sequence is implied and will be the same length
-            stage = core.getXYStageDevice()
-            core.loadXYStageSequence(stage, event.x_sequence, event.y_sequence)
-        if event.z_sequence:
-            zstage = core.getFocusDevice()
-            core.loadStageSequence(zstage, event.z_sequence)
-        if prop_seqs := event.property_sequences(core):
-            for (dev, prop), value_sequence in prop_seqs.items():
-                core.loadPropertySequence(dev, prop, value_sequence)
-
-        # TODO: SLM
-        core.prepareSequenceAcquisition(cam_device)
-
-        # start sequences or set non-sequenced values
-        if event.x_sequence:
-            core.startXYStageSequence(stage)
-        elif event.x_pos is not None or event.y_pos is not None:
-            self._set_event_position(event)
-
-        if event.z_sequence:
-            core.startStageSequence(zstage)
-        elif event.z_pos is not None:
-            self._set_event_z(event)
-
-        if event.exposure_sequence:
-            core.startExposureSequence(cam_device)
-        elif event.exposure is not None:
-            core.setExposure(event.exposure)
-
-        if prop_seqs:
-            for dev, prop in prop_seqs:
-                core.startPropertySequence(dev, prop)
-        elif event.channel is not None:
-            core.setConfig(event.channel.group, event.channel.config)
-
-    def setup_single_event(self, event: MDAEvent) -> None:
-        """Setup hardware for a single (non-sequenced) event.
-
-        This method is not part of the PMDAEngine protocol (it is called by
-        `setup_event`, which *is* part of the protocol), but it is made public
-        in case a user wants to subclass this engine and override this method.
+        Parameters
+        ----------
+        events : Iterable[MDAEvent]
+            An iterable of `useq.MDAEvents` objects to execute.
         """
-        if event.x_pos is not None or event.y_pos is not None:
-            self._set_event_position(event)
-        if event.z_pos is not None:
-            self._set_event_z(event)
-
-        if event.channel is not None:
-            self._mmc.setConfig(event.channel.group, event.channel.config)
-        if event.exposure is not None:
-            self._mmc.setExposure(event.exposure)
-
-    # ===================== EXEC =====================
-
-    def exec_event(self, event: MDAEvent) -> EventPayload | None:
-        """Execute an individual event and return the image data."""
-        action = getattr(event, "action", None)
-        if isinstance(action, HardwareAFType) and event.z_pos is not None:
-            try:
-                # execute hardware autofocus
-                new_correction = self._execute_autofocus(action)  # type: ignore
-            except RuntimeError as e:
-                logger.warning("Hardware autofocus failed. {}", e)
-            else:
-                # store correction for this position index
-                p_idx = event.index.get("p", None)
-                self._z_correction[p_idx] = new_correction
-            return None
-
-        if isinstance(event, SequencedEvent):
-            return self.exec_sequenced_event(event)
-        else:
-            return self.exec_single_event(event)
-
-    def exec_sequenced_event(self, event: SequencedEvent) -> EventPayload:
-        """Execute a sequenced (triggered) event and return the image data.
-
-        This method is not part of the PMDAEngine protocol (it is called by
-        `exec_event`, which *is* part of the protocol), but it is made public
-        in case a user wants to subclass this engine and override this method.
+        error = None
+        sequence = events if isinstance(events, MDASequence) else GeneratorMDASequence()
+        try:
+            engine = self._prepare_to_run(sequence)
+            self._run(engine, events)
+        except Exception as e:
+            error = e
+        with contextlib.suppress(Exception):
+            self._finish_run(sequence)
+        if error is not None:
+            raise error
+
+    def _run(self, engine: PMDAEngine, events: Iterable[MDAEvent]) -> None:
+        """Main execution of events, inside the try/except block of `run`."""
+        teardown_event = getattr(engine, "teardown_event", lambda e: None)
+        event_iterator = getattr(engine, "event_iterator", iter)
+        _events: Iterator[MDAEvent] = event_iterator(events)
+
+        for event in _events:
+            # If cancelled break out of the loop
+            if self._wait_until_event(event) or not self._running:
+                break
+
+            logger.info(event)
+            engine.setup_event(event)
+
+            output = engine.exec_event(event)
+
+            if (img := getattr(output, "image", None)) is not None:
+                with contextlib.suppress(EmitLoopError):
+                    self._signals.frameReady.emit(img, event)
+
+            # FIXME: this is here to make tests pass with sequenced events for now,
+            # but we might not want to do this for sequences for performance reasons.s
+            if (imgs := getattr(output, "image_sequence", None)) is not None:
+                with contextlib.suppress(EmitLoopError):
+                    for img, sub_event in imgs:
+                        self._signals.frameReady.emit(img, sub_event)
+
+            teardown_event(event)
+
+    def _prepare_to_run(self, sequence: MDASequence) -> PMDAEngine:
+        """Set up for the MDA run.
+
+        Parameters
+        ----------
+        sequence : MDASequence
+            The sequence of events to run.
         """
-        # TODO: add support for multiple camera devices
-        n_events = len(event.events)
+        if not self._engine:
+            raise RuntimeError("No MDAEngine set.")
 
-        # Start sequence
-        # Note that the overload of startSequenceAcquisition that takes a camera
-        # label does NOT automatically initialize a circular buffer.  So if this call
-        # is changed to accept the camera in the future, that should be kept in mind.
-        self._mmc.startSequenceAcquisition(
-            n_events,
-            0,  # intervalMS  # TODO: add support for this
-            True,  # stopOnOverflow
-        )
-
-        # block until the sequence is done, popping images in the meantime
-        images = []
-        while self._mmc.isSequenceRunning():
-            if self._mmc.getRemainingImageCount():
-                images.append(self._mmc.popNextImage())
-            else:
-                time.sleep(0.001)
-
-        if self._mmc.isBufferOverflowed():
-            raise MemoryError("Buffer overflowed")
-
-        while self._mmc.getRemainingImageCount():
-            images.append(self._mmc.popNextImage())
-
-        if len(images) != n_events:
-            logger.warning(
-                "Unexpected number of images returned from sequence. "
-                "Expected {}, got {}",
-                n_events,
-                len(images),
-            )
+        self._running = True
+        self._paused = False
+        self._paused_time = 0.0
+        self._sequence = sequence
+
+        self._engine.setup_sequence(sequence)
+        logger.info("MDA Started: {}", sequence)
+
+        self._signals.sequenceStarted.emit(sequence)
+        self._reset_timer()
+        return self._engine
 
-        return EventPayload(image_sequence=images)
+    def _reset_timer(self) -> None:
+        self._t0 = time.perf_counter()  # reference time, in seconds
 
-    def exec_single_event(self, event: MDAEvent) -> EventPayload | None:
-        """Execute a single (non-triggered) event and return the image data.
+    def _time_elapsed(self) -> float:
+        return time.perf_counter() - self._t0
 
-        This method is not part of the PMDAEngine protocol (it is called by
-        `exec_event`, which *is* part of the protocol), but it is made public
-        in case a user wants to subclass this engine and override this method.
+    def _check_canceled(self) -> bool:
+        """Return True if the cancel method has been called and emit relevant signals.
+
+        If cancelled, this relies on the `self._sequence` being the current sequence
+        in order to emit a `sequenceCanceled` signal.
+
+        Returns
+        -------
+        bool
+            Whether the MDA has been canceled.
         """
-        self._mmc.snapImage()
-        return EventPayload(image=self._mmc.getImage())
+        if self._canceled:
+            logger.warning("MDA Canceled: {}", self._sequence)
+            self._signals.sequenceCanceled.emit(self._sequence)
+            self._canceled = False
+            return True
+        return False
 
-    # ===================== EXTRA =====================
+    def _wait_until_event(self, event: MDAEvent) -> bool:
+        """Wait until the event's min start time, checking for pauses cancellations.
 
-    def event_iterator(self, events: Iterable[MDAEvent]) -> Iterator[MDAEvent]:
-        """Event iterator that merges events for hardware sequencing if possible.
+        Parameters
+        ----------
+        event : MDAEvent
+            The event to wait for.
 
-        This wraps `for event in events: ...` inside `MDARunner.run()` and combines
-        sequenceable events into an instance of `SequencedEvent`.
+        Returns
+        -------
+        bool
+            Whether the MDA was cancelled while waiting.
         """
-        seq: list[MDAEvent] = []
-        for event in events:
-            # if the sequence is empty or the current event can be sequenced with the
-            # previous event, add it to the sequence
-            if not seq or self._mmc.canSequenceEvents(seq[-1], event, len(seq)):
-                seq.append(event)
-            else:
-                # otherwise, yield a SequencedEvent if the sequence has accumulated
-                # more than one event, otherwise yield the single event
-                yield seq[0] if len(seq) == 1 else SequencedEvent.create(seq)
-                # add this current event and start a new sequence
-                seq = [event]
-        # yield any remaining events
-        if seq:
-            yield seq[0] if len(seq) == 1 else SequencedEvent.create(seq)
+        if not self.is_running():
+            return False
+        if self._check_canceled():
+            return True
+        while self.is_paused() and not self._canceled:
+            self._paused_time += self._pause_interval  # fixme: be more precise
+            time.sleep(self._pause_interval)
+
+            if self._check_canceled():
+                return True
+
+        # FIXME: this is actually the only place where the runner assumes our event is
+        # an MDAevent.  For everything else, the engine is technically the only thing
+        # that cares about the event time.
+        # So this whole method could potentially be moved to the engine.
+        if event.min_start_time:
+            go_at = event.min_start_time + self._paused_time
+            # We need to enter a loop here checking paused and canceled.
+            # otherwise you'll potentially wait a long time to cancel
+            to_go = go_at - self._time_elapsed()
+            while to_go > 0:
+                while self._paused and not self._canceled:
+                    self._paused_time += self._pause_interval  # fixme: be more precise
+                    to_go += self._pause_interval
+                    time.sleep(self._pause_interval)
+
+                if self._canceled:
+                    break
+                time.sleep(min(to_go, 0.5))
+                to_go = go_at - self._time_elapsed()
+
+        # check canceled again in case it was canceled
+        # during the waiting loop
+        return self._check_canceled()
 
-    def _execute_autofocus(self, action: HardwareAutofocus) -> float:
-        """Perform the hardware autofocus.
+    def _finish_run(self, sequence: MDASequence) -> None:
+        """To be called at the end of an acquisition.
 
-        Returns the change in ZPosition that occurred during the autofocus event.
+        Parameters
+        ----------
+        sequence : MDASequence
+            The sequence that was finished.
         """
-        # switch off autofocus device if it is on
-        self._mmc.enableContinuousFocus(False)
+        self._running = False
+        self._canceled = False
+
+        if hasattr(self._engine, "teardown_sequence"):
+            self._engine.teardown_sequence(sequence)  # type: ignore
 
-        # setup the autofocus device
-        self._mmc.setPosition(
-            action.autofocus_device_name,
-            action.autofocus_motor_offset,
-        )
-        self._mmc.waitForSystem()
-
-        @retry(exceptions=RuntimeError, tries=action.max_retries, logger=logger.warning)
-        def _perform_full_focus(previous_z: float) -> float:
-            self._mmc.fullFocus()
-            self._mmc.waitForSystem()
-            return self._mmc.getZPosition() - previous_z
-
-        return _perform_full_focus(self._mmc.getZPosition())
-
-    def _set_event_position(self, event: MDAEvent) -> None:
-        x = event.x_pos if event.x_pos is not None else self._mmc.getXPosition()
-        y = event.y_pos if event.y_pos is not None else self._mmc.getYPosition()
-        self._mmc.setXYPosition(x, y)
-
-    def _set_event_z(self, event: MDAEvent) -> None:
-        p_idx = event.index.get("p", None)
-        correction = self._z_correction.setdefault(p_idx, 0.0)
-        self._mmc.setZPosition(cast("float", event.z_pos) + correction)
-
-
-class EventPayload(NamedTuple):
-    image: np.ndarray | None = None
-    image_sequence: Sequence[np.ndarray] | None = None
+        logger.info("MDA Finished: {}", sequence)
+        self._signals.sequenceFinished.emit(sequence)
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_protocol.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/mda/_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Protocol, runtime_checkable
 
 if TYPE_CHECKING:
-    from typing import TYPE_CHECKING, Iterable, Iterator
+    from typing import Iterable, Iterator
 
     from useq import MDAEvent, MDASequence
 
 
 # NOTE: This whole thing could potentially go in useq-schema
 # as it makes no assumptions about pymmcore-plus
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/__init__.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/mda/events/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from ..._util import _qt_app_is_running
+from pymmcore_plus._util import _qt_app_is_running
+
 from ._protocol import PMDASignaler
 from ._psygnal import MDASignaler
 
 if TYPE_CHECKING:
-    from ._qsignals import QMDASignaler
+    from ._qsignals import QMDASignaler  # noqa: TCH004
 
 
 __all__ = [
     "PMDASignaler",
     "MDASignaler",
     "QMDASignaler",
     "_get_auto_MDA_callback_class",
```

### Comparing `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_protocol.py` & `pymmcore_plus-0.8.0/src/pymmcore_plus/mda/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/conftest.py` & `pymmcore_plus-0.8.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
 from unittest.mock import patch
 
 import pymmcore_plus
 import pytest
-from _pytest.logging import LogCaptureFixture
 from pymmcore_plus._logger import logger
 from pymmcore_plus.core.events import CMMCoreSignaler, QCoreSignaler
 from pymmcore_plus.mda.events import MDASignaler, QMDASignaler
 
+if TYPE_CHECKING:
+    from _pytest.logging import LogCaptureFixture
+
 
 @pytest.fixture(params=["QSignal", "psygnal"], scope="function")
 def core(request):
     core = pymmcore_plus.CMMCorePlus()
     if request.param == "psygnal":
         core._events = CMMCoreSignaler()
-        core.mda._events = MDASignaler()
+        core.mda._signals = MDASignaler()
     else:
         core._events = QCoreSignaler()
-        core.mda._events = QMDASignaler()
+        core.mda._signals = QMDASignaler()
     core._callback_relay = pymmcore_plus.core._mmcore_plus.MMCallbackRelay(core.events)
     core.registerCallback(core._callback_relay)
     if not core.getDeviceAdapterSearchPaths():
         pytest.fail("To run tests, please install MM with `mmcore install`")
     core.loadSystemConfiguration()
     return core
```

### Comparing `pymmcore_plus-0.7.1/tests/local_config.cfg` & `pymmcore_plus-0.8.0/tests/local_config.cfg`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/test_adapter_class.py` & `pymmcore_plus-0.8.0/tests/test_adapter_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/test_cli.py` & `pymmcore_plus-0.8.0/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 import json
 import os
 import shutil
 import subprocess
 import time
 from multiprocessing import Process, Queue
-from pathlib import Path
 from time import sleep
-from typing import Any, Callable, cast
+from typing import TYPE_CHECKING, Any, Callable, cast
 from unittest.mock import patch
 
 import pytest
 from pymmcore_plus import CMMCorePlus, __version__, _cli, _logger, install
 from pymmcore_plus._cli import app
 from typer.testing import CliRunner
 from useq import MDASequence
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 runner = CliRunner()
 subrun = subprocess.run
 
 
 def _mock_urlretrieve(url: str, filename: str, reporthook=None) -> None:
     """fake urlretrieve that writes a fake file."""
     with open(filename, "w") as f:
@@ -157,26 +159,30 @@
             metadata={"test": "test"},
         )
         useq_file = tmp_path / "test.json"
         useq_file.write_text(seq.json())
         cmd.append(str(useq_file))
 
         for field_name, val in args.items():
-            field = MDASequence.__fields__[field_name]
+            try:
+                valid_field = getattr(MDASequence(**{field_name: val}), field_name)
+            except TypeError:
+                valid_field = None
             # when the args are a complete field on their own
             # it will replace the whole field
-            if isinstance(val, str) or field.validate(val, {}, loc="")[0]:
+            if isinstance(val, str) or valid_field:
                 seq = seq.replace(**{field_name: val})
             # otherwise it updates the existing
             else:
-                sub_field = cast(dict, seq.dict()[field_name])
+                _data = seq.model_dump() if hasattr(seq, "model_dump") else seq.dict()
+                sub_field = cast(dict, _data[field_name])
                 sub_field.update(**val)
-                newval = field.validate(sub_field, {}, loc="")[0]
+                newval = getattr(MDASequence(**{field_name: sub_field}), field_name)
                 seq = seq.replace(**{field_name: newval})
-        expected = seq.copy()
+        expected = seq.model_copy() if hasattr(seq, "model_copy") else seq.copy()
     else:
         expected = MDASequence(**args)
 
     with patch("pymmcore_plus.core._mmcore_plus._instance") as mock:
         result = runner.invoke(app, cmd)
 
     assert result.exit_code == 0
```

### Comparing `pymmcore_plus-0.7.1/tests/test_config_group_class.py` & `pymmcore_plus-0.8.0/tests/test_config_group_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/test_core.py` & `pymmcore_plus-0.8.0/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     # using this to avoid our setProperty override... which would immediately
     # raise the exception (we want it to be raised deeper)
     if isinstance(core.events, CMMCoreSignaler):
         pymmcore.CMMCore.setProperty(core, "Camera", "Binning", 2)
         msg = caplog.records[0].message
         assert msg.startswith(
-            "Exception occured in MMCorePlus callback 'propertyChanged'"
+            "Exception occurred in MMCorePlus callback 'propertyChanged'"
         )
     else:
         with qtbot.capture_exceptions() as exceptions:
             with qtbot.waitSignal(core.events.propertyChanged):
                 pymmcore.CMMCore.setProperty(core, "Camera", "Binning", 2)
         assert len(exceptions) == 1
         assert str(exceptions[0][1]) == "Boom"
@@ -128,22 +128,22 @@
     fr_mock = MagicMock()
     ss_mock = MagicMock()
     sf_mock = MagicMock()
     xystage_mock = MagicMock()
     stage_mock = MagicMock()
     exp_mock = MagicMock()
 
-    core.mda._events.frameReady.connect(fr_mock)
-    core.mda._events.sequenceStarted.connect(ss_mock)
-    core.mda._events.sequenceFinished.connect(sf_mock)
+    core.mda._signals.frameReady.connect(fr_mock)
+    core.mda._signals.sequenceStarted.connect(ss_mock)
+    core.mda._signals.sequenceFinished.connect(sf_mock)
     core.events.XYStagePositionChanged.connect(xystage_mock)
     core.events.stagePositionChanged.connect(stage_mock)
     core.events.exposureChanged.connect(exp_mock)
 
-    with qtbot.waitSignal(core.mda._events.sequenceFinished):
+    with qtbot.waitSignal(core.mda._signals.sequenceFinished):
         core.run_mda(mda)
     assert fr_mock.call_count == len(list(mda))
     for event, _call in zip(mda, fr_mock.call_args_list):
         assert isinstance(_call.args[0], np.ndarray)
         assert _call.args[1] == event
 
     ss_mock.assert_called_once_with(mda)
@@ -174,34 +174,34 @@
     )
 
     pause_mock = MagicMock()
     cancel_mock = MagicMock()
     sf_mock = MagicMock()
     ss_mock = MagicMock()
 
-    core.mda._events.sequenceStarted.connect(ss_mock)
-    core.mda._events.sequencePauseToggled.connect(pause_mock)
-    core.mda._events.sequenceCanceled.connect(cancel_mock)
-    core.mda._events.sequenceFinished.connect(sf_mock)
+    core.mda._signals.sequenceStarted.connect(ss_mock)
+    core.mda._signals.sequencePauseToggled.connect(pause_mock)
+    core.mda._signals.sequenceCanceled.connect(cancel_mock)
+    core.mda._signals.sequenceFinished.connect(sf_mock)
 
     _fcount = 0
 
-    @core.mda._events.frameReady.connect
+    @core.mda._signals.frameReady.connect
     def _onframe(frame, event):
         nonlocal _fcount
         _fcount += 1
         if _fcount == 1:
             core.mda.toggle_pause()
             pause_mock.assert_called_with(True)
             core.mda.toggle_pause()
             pause_mock.assert_called_with(False)
         elif _fcount == 2:
             core.mda.cancel()
 
-    with qtbot.waitSignal(core.mda._events.sequenceFinished):
+    with qtbot.waitSignal(core.mda._signals.sequenceFinished):
         core.run_mda(mda)
 
     ss_mock.assert_called_once_with(mda)
     cancel_mock.assert_called_once_with(mda)
     assert _fcount < len(list(mda))
     sf_mock.assert_called_once_with(mda)
 
@@ -444,23 +444,23 @@
 
     th = Thread(target=trigger_cb)
     with qtbot.waitSignal(core.events.XYStagePositionChanged):
         th.start()
     assert got_lock
     got_lock = False
 
-    core.mda._events.frameReady.connect(cb)
+    core.mda._signals.frameReady.connect(cb)
     mda = MDASequence(
         time_plan={"interval": 0.1, "loops": 2},
         stage_positions=[(1, 1, 1)],
         z_plan={"range": 3, "step": 1},
         channels=[{"config": "DAPI", "exposure": 1}],
     )
 
-    with qtbot.waitSignal(core.mda._events.sequenceFinished):
+    with qtbot.waitSignal(core.mda._signals.sequenceFinished):
         core.run_mda(mda)
     assert got_lock
 
 
 def test_single_instance():
     core1 = CMMCorePlus.instance()
     core2 = CMMCorePlus.instance()
```

### Comparing `pymmcore_plus-0.7.1/tests/test_device_class.py` & `pymmcore_plus-0.8.0/tests/test_device_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/test_events.py` & `pymmcore_plus-0.8.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/test_misc.py` & `pymmcore_plus-0.8.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/test_property_class.py` & `pymmcore_plus-0.8.0/tests/test_property_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/tests/test_sequencing.py` & `pymmcore_plus-0.8.0/tests/test_sequencing.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         time_plan=useq.TIntervalLoops(interval=0, loops=NLOOPS),
     )
     EXPECTED_SEQUENCES = 4  # timeseries at each of 2 positions, 2 channels
 
     core_mock = cast("CMMCorePlus", MagicMock(wraps=core))  # so we can spy on all_calls
     engine = MDAEngine(mmc=core_mock)
 
+    engine.use_hardware_sequencing = False
+    assert len(list(engine.event_iterator(mda))) == NLOOPS * 2 * 2
+
+    engine.use_hardware_sequencing = True
     events = list(engine.event_iterator(mda))
     assert len(events) == EXPECTED_SEQUENCES
 
     runner = MDARunner()
     runner.set_engine(engine)
 
     runner.run(mda)
@@ -53,14 +57,15 @@
 
 def test_sequenced_mda_with_zero_values() -> None:
     # just testing a bug I found where if z, x, or y are 0, they accidentally
     # get sequenced
     mda = useq.MDASequence(z_plan=useq.ZRangeAround(range=3.0, step=0.5))
     core = CMMCorePlus()
     core.loadSystemConfiguration()
+    core.mda.engine.use_hardware_sequencing = True
     core.mda.run(mda)
 
 
 def test_fully_sequenceable_core():
     mda = useq.MDASequence(
         stage_positions=[(0, 0, 0), (1, 1, 1)],
         z_plan=useq.ZRangeAround(range=3, step=1),
@@ -80,15 +85,15 @@
     core_mock.isBufferOverflowed.return_value = False
     core_mock.getCameraDevice.return_value = CAM
     core_mock.getXYStageDevice.return_value = XYSTAGE
     core_mock.getFocusDevice.return_value = FOCUS
     core_mock.getFocusDevice.return_value = FOCUS
     core_mock.getPixelSizeUm.return_value = None
 
-    engine = MDAEngine(mmc=core_mock)
+    engine = MDAEngine(mmc=core_mock, use_hardware_sequencing=True)
 
     combined_events = list(engine.event_iterator(mda))
     assert len(combined_events) == 1
     seq_event = combined_events[0]
     assert isinstance(seq_event, SequencedEvent)
 
     runner = MDARunner()
@@ -109,8 +114,9 @@
     core.initializeCircularBuffer()
     core.setCircularBufferMemoryFootprint(20)
     max_imgs = core.getBufferFreeCapacity()
     mda = useq.MDASequence(
         channels=["DAPI"],
         time_plan=useq.TIntervalLoops(interval=0, loops=max_imgs * 2),
     )
+    core.mda.engine.use_hardware_sequencing = True
     core.mda.run(mda)
```

### Comparing `pymmcore_plus-0.7.1/.gitignore` & `pymmcore_plus-0.8.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -133,14 +133,13 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
-src/pymmcore_plus/_version.py
 Micro-Manager-*
 .vscode
 
 docs/_includes/_cmmcore_members.md
 docs/_includes/_cmmcore_table.md
 docs/_includes/_cmmcoreplus_members.md
```

### Comparing `pymmcore_plus-0.7.1/LICENSE` & `pymmcore_plus-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.1/README.md` & `pymmcore_plus-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pymmcore-plus
 
 [![License](https://img.shields.io/pypi/l/pymmcore-plus.svg?color=green)](https://github.com/pymmcore-plus/pymmcore-plus/raw/master/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymmcore-plus)](https://pypi.org/project/pymmcore-plus)
 [![PyPI](https://img.shields.io/pypi/v/pymmcore-plus.svg?color=green)](https://pypi.org/project/pymmcore-plus)
-[![Python
-Version](https://img.shields.io/pypi/pyversions/pymmcore-plus.svg?color=green)](https://python.org)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/pymmcore-plus)](https://anaconda.org/conda-forge/pymmcore-plus)
 [![CI](https://github.com/pymmcore-plus/pymmcore-plus/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/pymmcore-plus/pymmcore-plus/actions/workflows/test_and_deploy.yml)
+[![docs](https://github.com/pymmcore-plus/pymmcore-plus/actions/workflows/docs.yml/badge.svg)](https://pymmcore-plus.github.io/pymmcore-plus/)
 [![codecov](https://codecov.io/gh/pymmcore-plus/pymmcore-plus/branch/main/graph/badge.svg)](https://codecov.io/gh/pymmcore-plus/pymmcore-plus)
 
 `pymmcore-plus` extends [pymmcore](https://github.com/micro-manager/pymmcore)
 (python bindings for the C++ [micro-manager
 core](https://github.com/micro-manager/mmCoreAndDevices/)) with a number of
 features designed to facilitate working with **Micro-manager in pure python/C
 environments**.
@@ -25,26 +26,26 @@
   experiments. It accepts an
   [MDASequence](https://pymmcore-plus.github.io/useq-schema/schema/sequence/)
   from [useq-schema](https://pymmcore-plus.github.io/useq-schema/) for
   experiment design/declaration.
 - Adds a [callback
   system](https://pymmcore-plus.github.io/pymmcore-plus/api/events/) that adapts
   the CMMCore callback object to an existing python event loop (such as Qt, or
-  perhaps asyncio/etc...).  The `CMMCorePlus` class also fixes a number of
+  perhaps asyncio/etc...). The `CMMCorePlus` class also fixes a number of
   "missed" events that are not currently emitted by the CMMCore API.
 
 ## Documentation
 
 https://pymmcore-plus.github.io/pymmcore-plus/
 
 ## Why not just use `pymmcore` directly?
 
 [pymmcore](https://github.com/micro-manager/pymmcore) is (and should probably
 remain) a thin SWIG wrapper for the C++ code at the core of the
-[Micro-Manager](https://github.com/micro-manager/mmCoreAndDevices/) project.  It
+[Micro-Manager](https://github.com/micro-manager/mmCoreAndDevices/) project. It
 is sufficient to control micromanager via python, but lacks some "niceties" that
 python users are accustomed to. This library:
 
 - extends the `pymmcore.CMMCore` object with [additional
   methods](https://pymmcore-plus.github.io/pymmcore-plus/api/cmmcoreplus/)
 - fixes emission of a number of events in `MMCore`.
 - provide proper python interfaces for various objects like
@@ -53,23 +54,23 @@
 - provides an [object-oriented
   API](https://pymmcore-plus.github.io/pymmcore-plus/api/device/) for Devices
   and their properties.
 - uses more interpretable `Enums` rather than `int` for [various
   constants](https://pymmcore-plus.github.io/pymmcore-plus/api/constants/)
 - improves docstrings and type annotations.
 - generally feel more pythonic (note however, `camelCase` method names from the
-  CMMCore API are *not* substituted with `snake_case`).
+  CMMCore API are _not_ substituted with `snake_case`).
 
 ## What about `Pycro-Manager`?
 
 [Pycro-Manager](https://github.com/micro-manager/pycro-manager) is a library
 designed to make it easier to work with and control the **Java** Micro-manager
-application using python.  As such, it requires Java to be installed and running
+application using python. As such, it requires Java to be installed and running
 in the background (either via the micro-manager GUI application directly, or via
-a headless process).  The python half communicates with the Java half using
+a headless process). The python half communicates with the Java half using
 ZeroMQ messaging.
 
 **In brief**: while `Pycro-Manager` provides a python API to control the Java
 Micro-manager application (which in turn controls the C++ core), `pymmcore-plus`
 provides a python API to control the C++ core directly, without the need for
 Java in the loop.
 
@@ -91,15 +92,15 @@
 Usually, you'll then want to install the device adapters (though
 you can also download these manually from [micro-manager.org](https://micro-manager.org/Micro-Manager_Nightly_Builds)):
 
 ```sh
 mmcore install
 ```
 
-*See [installation documentation ](https://pymmcore-plus.github.io/pymmcore-plus/install/) for more details.*
+_See [installation documentation ](https://pymmcore-plus.github.io/pymmcore-plus/install/) for more details._
 
 ### Usage
 
 Then use the core object as you would `pymmcore.CMMCore`...
 but with [more features](https://pymmcore-plus.github.io/pymmcore-plus/api/cmmcoreplus/) :smile:
 
 ```python
@@ -115,8 +116,8 @@
 documentation](http://pymmcore-plus.github.io/pymmcore-plus/examples/mda/).
 
 You can find some basic python scripts in the [examples](examples) directory of
 this repository
 
 ## Contributing
 
-Contributions are welcome!  See [contributing guide](http://pymmcore-plus.github.io/pymmcore-plus/contributing/).
+Contributions are welcome! See [contributing guide](http://pymmcore-plus.github.io/pymmcore-plus/contributing/).
```

### Comparing `pymmcore_plus-0.7.1/pyproject.toml` & `pymmcore_plus-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     "Topic :: System :: Hardware",
     "Topic :: System :: Hardware :: Hardware Drivers",
     "Topic :: Utilities",
 ]
 dynamic = ["version"]
 dependencies = [
     "appdirs",
-    "loguru",
+    "loguru >=0.5.0",
     "numpy",
-    "psygnal>=0.4.2",
-    "pymmcore>=10.1.1.70.4",
-    "rich",
-    "typer",
+    "psygnal >=0.4.2",
+    "pymmcore >=10.1.1.70.4",
+    "rich >=10.2.0",
+    "typer >=0.4.2",
     "typing-extensions",
-    "useq-schema >=0.3.1",
+    "useq-schema >=0.4.0",
     "wrapt",
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 docs = [
@@ -81,69 +81,69 @@
 # https://hatch.pypa.io/latest/config/metadata/
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
-[tool.hatch.build.hooks.vcs]
-version-file = "src/pymmcore_plus/_version.py"
-
 # https://hatch.pypa.io/latest/config/build/#file-selection
-# [tool.hatch.build.targets.sdist]
-# include = ["/src", "/tests"]
+[tool.hatch.build.targets.sdist]
+include = ["/src", "/tests"]
 
+[tool.hatch.build.targets.wheel]
+only-include = ["src"]
+sources = ["src"]
 
-# https://github.com/charliermarsh/ruff
+# https://beta.ruff.rs/docs/rules/
 [tool.ruff]
 line-length = 88
 target-version = "py38"
-extend-select = [
-    "E",  # style errors
-    "F",  # flakes
-    "D",  # pydocstyle
-    "I",  # isort
-    "UP", # pyupgrade
-    # "N",  # pep8-naming
-    # "S",  # bandit
-    "C",    # flake8-comprehensions
+select = [
+    "E",    # style errors
+    "F",    # flakes
+    "W",    # warnings
+    "D",    # pydocstyle
+    "I",    # isort
+    "UP",   # pyupgrade
+    "C4",   # flake8-comprehensions
     "B",    # flake8-bugbear
     "A001", # flake8-builtins
     "RUF",  # ruff-specific rules
+    "TID",  # tidy
+    "TCH",  # typecheck
+    "SLF",  # private-access
 ]
-extend-ignore = [
+ignore = [
     "D100", # Missing docstring in public module
     "D104", # Missing docstring in public package
     "D107", # Missing docstring in __init__
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D213", # Multi-line docstring summary should start at the second line
     "D400", # First line should end with a period
     "D401", # First line should be in imperative mood
     "D413", # Missing blank line after last section
     "D416", # Section name should end with a colon
-    "C901", # Function is too complex
 ]
 
 [tool.ruff.per-file-ignores]
-"tests/*.py" = ["D"]
+"tests/*.py" = ["D", "SLF"]
 "examples/*.py" = ["D"]
 "_cli.py" = ["B008"]
-"_mmcore_plus*.py" = ["D4"]
 "docs/*.py" = ["A", "D"]
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = ["error"]
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
-files = "src/**/*/*.py"
+files = "src/**"
 strict = true
 disallow_any_generics = false
 disallow_subclassing_any = false
 show_error_codes = true
 pretty = true
 plugins = "pydantic.mypy"
 
@@ -155,15 +155,15 @@
     "@overload",
     "except ImportError",
     "raise AssertionError",
     "if __name__ == .__main__.:",
     "raise NotImplementedError",
 ]
 [tool.coverage.run]
-source = ['src/pymmcore_plus']
+source = ['pymmcore_plus']
 
 # https://github.com/mgedmin/check-manifest#configuration
 [tool.check-manifest]
 ignore = [
     ".github_changelog_generator",
     ".pre-commit-config.yaml",
     ".ruff_cache/**/*",
```

### Comparing `pymmcore_plus-0.7.1/PKG-INFO` & `pymmcore_plus-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmcore-plus
-Version: 0.7.1
+Version: 0.8.0
 Summary: pymmcore superset providing improved APIs, event connection, and a pure python acquisition engine
 Project-URL: Source, https://github.com/pymmcore-plus/pymmcore-plus
 Project-URL: Tracker, https://github.com/pymmcore-plus/pymmcore-plus/issues
 Project-URL: Documentation, https://pymmcore-plus.github.io/pymmcore-plus
 Author-email: Talley Lambert <talley.lambert@gmail.com>, Federico Gasparoli <federico.gasparoli@gmail.com>, Ian Hunt-Isaak <ianhuntisaak@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -21,22 +21,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Requires-Dist: appdirs
-Requires-Dist: loguru
+Requires-Dist: loguru>=0.5.0
 Requires-Dist: numpy
 Requires-Dist: psygnal>=0.4.2
 Requires-Dist: pymmcore>=10.1.1.70.4
-Requires-Dist: rich
-Requires-Dist: typer
+Requires-Dist: rich>=10.2.0
+Requires-Dist: typer>=0.4.2
 Requires-Dist: typing-extensions
-Requires-Dist: useq-schema>=0.3.1
+Requires-Dist: useq-schema>=0.4.0
 Requires-Dist: wrapt
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
@@ -57,18 +57,19 @@
 Requires-Dist: pytest-qt; extra == 'testing'
 Requires-Dist: qtpy; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # pymmcore-plus
 
 [![License](https://img.shields.io/pypi/l/pymmcore-plus.svg?color=green)](https://github.com/pymmcore-plus/pymmcore-plus/raw/master/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymmcore-plus)](https://pypi.org/project/pymmcore-plus)
 [![PyPI](https://img.shields.io/pypi/v/pymmcore-plus.svg?color=green)](https://pypi.org/project/pymmcore-plus)
-[![Python
-Version](https://img.shields.io/pypi/pyversions/pymmcore-plus.svg?color=green)](https://python.org)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/pymmcore-plus)](https://anaconda.org/conda-forge/pymmcore-plus)
 [![CI](https://github.com/pymmcore-plus/pymmcore-plus/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/pymmcore-plus/pymmcore-plus/actions/workflows/test_and_deploy.yml)
+[![docs](https://github.com/pymmcore-plus/pymmcore-plus/actions/workflows/docs.yml/badge.svg)](https://pymmcore-plus.github.io/pymmcore-plus/)
 [![codecov](https://codecov.io/gh/pymmcore-plus/pymmcore-plus/branch/main/graph/badge.svg)](https://codecov.io/gh/pymmcore-plus/pymmcore-plus)
 
 `pymmcore-plus` extends [pymmcore](https://github.com/micro-manager/pymmcore)
 (python bindings for the C++ [micro-manager
 core](https://github.com/micro-manager/mmCoreAndDevices/)) with a number of
 features designed to facilitate working with **Micro-manager in pure python/C
 environments**.
@@ -85,26 +86,26 @@
   experiments. It accepts an
   [MDASequence](https://pymmcore-plus.github.io/useq-schema/schema/sequence/)
   from [useq-schema](https://pymmcore-plus.github.io/useq-schema/) for
   experiment design/declaration.
 - Adds a [callback
   system](https://pymmcore-plus.github.io/pymmcore-plus/api/events/) that adapts
   the CMMCore callback object to an existing python event loop (such as Qt, or
-  perhaps asyncio/etc...).  The `CMMCorePlus` class also fixes a number of
+  perhaps asyncio/etc...). The `CMMCorePlus` class also fixes a number of
   "missed" events that are not currently emitted by the CMMCore API.
 
 ## Documentation
 
 https://pymmcore-plus.github.io/pymmcore-plus/
 
 ## Why not just use `pymmcore` directly?
 
 [pymmcore](https://github.com/micro-manager/pymmcore) is (and should probably
 remain) a thin SWIG wrapper for the C++ code at the core of the
-[Micro-Manager](https://github.com/micro-manager/mmCoreAndDevices/) project.  It
+[Micro-Manager](https://github.com/micro-manager/mmCoreAndDevices/) project. It
 is sufficient to control micromanager via python, but lacks some "niceties" that
 python users are accustomed to. This library:
 
 - extends the `pymmcore.CMMCore` object with [additional
   methods](https://pymmcore-plus.github.io/pymmcore-plus/api/cmmcoreplus/)
 - fixes emission of a number of events in `MMCore`.
 - provide proper python interfaces for various objects like
@@ -113,23 +114,23 @@
 - provides an [object-oriented
   API](https://pymmcore-plus.github.io/pymmcore-plus/api/device/) for Devices
   and their properties.
 - uses more interpretable `Enums` rather than `int` for [various
   constants](https://pymmcore-plus.github.io/pymmcore-plus/api/constants/)
 - improves docstrings and type annotations.
 - generally feel more pythonic (note however, `camelCase` method names from the
-  CMMCore API are *not* substituted with `snake_case`).
+  CMMCore API are _not_ substituted with `snake_case`).
 
 ## What about `Pycro-Manager`?
 
 [Pycro-Manager](https://github.com/micro-manager/pycro-manager) is a library
 designed to make it easier to work with and control the **Java** Micro-manager
-application using python.  As such, it requires Java to be installed and running
+application using python. As such, it requires Java to be installed and running
 in the background (either via the micro-manager GUI application directly, or via
-a headless process).  The python half communicates with the Java half using
+a headless process). The python half communicates with the Java half using
 ZeroMQ messaging.
 
 **In brief**: while `Pycro-Manager` provides a python API to control the Java
 Micro-manager application (which in turn controls the C++ core), `pymmcore-plus`
 provides a python API to control the C++ core directly, without the need for
 Java in the loop.
 
@@ -151,15 +152,15 @@
 Usually, you'll then want to install the device adapters (though
 you can also download these manually from [micro-manager.org](https://micro-manager.org/Micro-Manager_Nightly_Builds)):
 
 ```sh
 mmcore install
 ```
 
-*See [installation documentation ](https://pymmcore-plus.github.io/pymmcore-plus/install/) for more details.*
+_See [installation documentation ](https://pymmcore-plus.github.io/pymmcore-plus/install/) for more details._
 
 ### Usage
 
 Then use the core object as you would `pymmcore.CMMCore`...
 but with [more features](https://pymmcore-plus.github.io/pymmcore-plus/api/cmmcoreplus/) :smile:
 
 ```python
@@ -175,8 +176,8 @@
 documentation](http://pymmcore-plus.github.io/pymmcore-plus/examples/mda/).
 
 You can find some basic python scripts in the [examples](examples) directory of
 this repository
 
 ## Contributing
 
-Contributions are welcome!  See [contributing guide](http://pymmcore-plus.github.io/pymmcore-plus/contributing/).
+Contributions are welcome! See [contributing guide](http://pymmcore-plus.github.io/pymmcore-plus/contributing/).
```

