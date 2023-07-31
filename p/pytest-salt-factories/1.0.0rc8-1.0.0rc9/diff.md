# Comparing `tmp/pytest-salt-factories-1.0.0rc8.tar.gz` & `tmp/pytest-salt-factories-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Mar 12 10:13:21 2022, max compression
+gzip compressed data, last modified: Sun Mar 20 12:34:55 2022, max compression
```

## Comparing `pytest-salt-factories-1.0.0rc8.tar` & `pytest-salt-factories-1.0.0rc9.tar`

### file list

```diff
@@ -1,325 +1,326 @@
--rw-r--r--   0 root         (0) root         (0)     4151 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.codecov.yml
--rw-r--r--   0 root         (0) root         (0)      745 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.coveragerc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.github/
--rw-r--r--   0 root         (0) root         (0)      429 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.github/CODEOWNERS
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      638 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)    30500 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.github/workflows/testing.yml
--rw-r--r--   0 root         (0) root         (0)     1426 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4482 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4472 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)      506 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)     1644 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)    13608 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      548 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)     8796 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)    11339 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3410 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2033 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/changelog/
--rw-r--r--   0 root         (0) root         (0)       12 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/changelog/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/css/
--rw-r--r--   0 root         (0) root         (0)      425 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/css/inline-include.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/img/
--rw-r--r--   0 root         (0) root         (0)    10359 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/img/SaltProject_Logomark_teal.png
--rw-r--r--   0 root         (0) root         (0)     9591 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/img/SaltProject_altlogo_teal.png
--rw-r--r--   0 root         (0) root         (0)    12539 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/img/complicated.svg
--rw-r--r--   0 root         (0) root         (0)     2241 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/_static/img/simple.svg
--rw-r--r--   0 root         (0) root         (0)       30 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     8259 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      314 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      563 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/
--rw-r--r--   0 root         (0) root         (0)      143 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/bases.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/
--rw-r--r--   0 root         (0) root         (0)      162 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/call.rst
--rw-r--r--   0 root         (0) root         (0)      166 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/cloud.rst
--rw-r--r--   0 root         (0) root         (0)      154 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/cp.rst
--rw-r--r--   0 root         (0) root         (0)      158 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/key.rst
--rw-r--r--   0 root         (0) root         (0)      158 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/run.rst
--rw-r--r--   0 root         (0) root         (0)      147 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/salt.rst
--rw-r--r--   0 root         (0) root         (0)      143 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/spm.rst
--rw-r--r--   0 root         (0) root         (0)      158 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli/ssh.rst
--rw-r--r--   0 root         (0) root         (0)      560 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli.rst
--rw-r--r--   0 root         (0) root         (0)      157 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/client.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/daemons/
--rw-r--r--   0 root         (0) root         (0)      161 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/daemons/api.rst
--rw-r--r--   0 root         (0) root         (0)      162 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/daemons/container.rst
--rw-r--r--   0 root         (0) root         (0)      174 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/daemons/master.rst
--rw-r--r--   0 root         (0) root         (0)      174 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/daemons/minion.rst
--rw-r--r--   0 root         (0) root         (0)      170 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/daemons/proxy.rst
--rw-r--r--   0 root         (0) root         (0)      150 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/daemons/sshd.rst
--rw-r--r--   0 root         (0) root         (0)      155 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/exceptions.rst
--rw-r--r--   0 root         (0) root         (0)      472 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/index.rst
--rw-r--r--   0 root         (0) root         (0)      188 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/manager.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/
--rw-r--r--   0 root         (0) root         (0)      164 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/event_listener.rst
--rw-r--r--   0 root         (0) root         (0)      175 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/factories.rst
--rw-r--r--   0 root         (0) root         (0)      117 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/index.rst
--rw-r--r--   0 root         (0) root         (0)      140 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/loader.rst
--rw-r--r--   0 root         (0) root         (0)       72 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/log_server.rst
--rw-r--r--   0 root         (0) root         (0)     1502 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/markers.rst
--rw-r--r--   0 root         (0) root         (0)       85 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/sysinfo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/
--rw-r--r--   0 root         (0) root         (0)      193 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/cli_scripts.rst
--rw-r--r--   0 root         (0) root         (0)      190 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/functional.rst
--rw-r--r--   0 root         (0) root         (0)      182 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/index.rst
--rw-r--r--   0 root         (0) root         (0)      178 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/loader.rst
--rw-r--r--   0 root         (0) root         (0)      191 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/markers.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/saltext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)      185 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/saltext/engines/pytest_engine.rst
--rw-r--r--   0 root         (0) root         (0)      229 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/saltext/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/saltext/log_handlers/
--rw-r--r--   0 root         (0) root         (0)      205 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/saltext/log_handlers/pytest_log_handler.rst
--rw-r--r--   0 root         (0) root         (0)      179 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/utils/tempfiles.rst
--rw-r--r--   0 root         (0) root         (0)      273 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/sitevars.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/topics/
--rw-r--r--   0 root         (0) root         (0)      779 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/topics/fixtures.rst
--rw-r--r--   0 root         (0) root         (0)     1032 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/topics/install.rst
--rw-r--r--   0 root         (0) root         (0)     1540 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/docs/topics/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/
--rw-r--r--   0 root         (0) root         (0)    11344 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/LICENSE
--rw-r--r--   0 root         (0) root         (0)      117 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/README.md
--rw-r--r--   0 root         (0) root         (0)      307 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/requirements/
--rw-r--r--   0 root         (0) root         (0)       13 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     1662 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      132 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/
--rw-r--r--   0 root         (0) root         (0)      863 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/__init__.py
--rw-r--r--   0 root         (0) root         (0)      506 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      551 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/modules/echo_mod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/states/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/states/__init__.py
--rw-r--r--   0 root         (0) root         (0)      796 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/states/echo_mod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      768 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      445 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      502 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/modules/test_echo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/states/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/states/__init__.py
--rw-r--r--   0 root         (0) root         (0)      539 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/states/test_echo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      506 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/modules/test_echo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/states/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/states/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1078 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/states/test_echo.py
--rw-r--r--   0 root         (0) root         (0)    20519 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     1238 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      348 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/requirements/
--rw-r--r--   0 root         (0) root         (0)      211 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      144 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      150 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/requirements/lint.txt
--rw-r--r--   0 root         (0) root         (0)      109 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     3282 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      111 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3410 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9637 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      531 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      626 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/
--rw-r--r--   0 root         (0) root         (0)     1799 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/__main__.py
--rw-r--r--   0 root         (0) root         (0)    25738 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/bases.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/
--rw-r--r--   0 root         (0) root         (0)      147 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      743 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/call.py
--rw-r--r--   0 root         (0) root         (0)     3306 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/cloud.py
--rw-r--r--   0 root         (0) root         (0)      607 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/cp.py
--rw-r--r--   0 root         (0) root         (0)     1413 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/key.py
--rw-r--r--   0 root         (0) root         (0)      770 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     1309 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/salt.py
--rw-r--r--   0 root         (0) root         (0)      413 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/spm.py
--rw-r--r--   0 root         (0) root         (0)     1269 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/ssh.py
--rw-r--r--   0 root         (0) root         (0)     3433 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/
--rw-r--r--   0 root         (0) root         (0)      144 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/api.py
--rw-r--r--   0 root         (0) root         (0)    24222 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/container.py
--rw-r--r--   0 root         (0) root         (0)    21359 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/master.py
--rw-r--r--   0 root         (0) root         (0)    10511 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/minion.py
--rw-r--r--   0 root         (0) root         (0)    11620 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/proxy.py
--rw-r--r--   0 root         (0) root         (0)     8150 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/sshd.py
--rw-r--r--   0 root         (0) root         (0)     5781 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/syndic.py
--rw-r--r--   0 root         (0) root         (0)      159 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    26033 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/
--rw-r--r--   0 root         (0) root         (0)     2726 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18958 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/event_listener.py
--rw-r--r--   0 root         (0) root         (0)     2045 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/factories.py
--rw-r--r--   0 root         (0) root         (0)     3397 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/loader.py
--rw-r--r--   0 root         (0) root         (0)     9297 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/log_server.py
--rw-r--r--   0 root         (0) root         (0)     1635 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/markers.py
--rw-r--r--   0 root         (0) root         (0)     5440 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/sysinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/
--rw-r--r--   0 root         (0) root         (0)     3917 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8265 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/cli_scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/coverage/
--rw-r--r--   0 root         (0) root         (0)       86 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/coverage/sitecustomize.py
--rw-r--r--   0 root         (0) root         (0)    17655 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/functional.py
--rw-r--r--   0 root         (0) root         (0)     7186 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/loader.py
--rw-r--r--   0 root         (0) root         (0)     5594 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/markers.py
--rw-r--r--   0 root         (0) root         (0)      350 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/ports.py
--rw-r--r--   0 root         (0) root         (0)       43 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/ports.pyi
--rw-r--r--   0 root         (0) root         (0)      362 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/processes.py
--rw-r--r--   0 root         (0) root         (0)       47 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/processes.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)     6166 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/engines/pytest_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/log_handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/log_handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13370 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/log_handlers/pytest_log_handler.py
--rw-r--r--   0 root         (0) root         (0)    14429 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/tempfiles.py
--rw-r--r--   0 root         (0) root         (0)     7303 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/virtualenv.py
--rw-r--r--   0 root         (0) root         (0)       46 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/src/saltfactories/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4978 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/base/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2159 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/base/test_salt_daemon_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      973 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/conftest.py
--rw-r--r--   0 root         (0) root         (0)      548 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_call.py
--rw-r--r--   0 root         (0) root         (0)      322 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_cloud.py
--rw-r--r--   0 root         (0) root         (0)      316 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_cp.py
--rw-r--r--   0 root         (0) root         (0)      318 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_key.py
--rw-r--r--   0 root         (0) root         (0)      318 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_run.py
--rw-r--r--   0 root         (0) root         (0)      310 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_salt.py
--rw-r--r--   0 root         (0) root         (0)      313 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_spm.py
--rw-r--r--   0 root         (0) root         (0)      318 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3856 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_master_factory.py
--rw-r--r--   0 root         (0) root         (0)     4614 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_minion_factory.py
--rw-r--r--   0 root         (0) root         (0)     3591 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_proxy_minion_factory.py
--rw-r--r--   0 root         (0) root         (0)     5207 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_syndic_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/loader/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/loader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1592 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/loader/test_fixture_deps.py
--rw-r--r--   0 root         (0) root         (0)     5348 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/loader/test_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/markers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/markers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4664 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/markers/test_requires_salt_modules.py
--rw-r--r--   0 root         (0) root         (0)     4803 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/markers/test_requires_salt_states.py
--rw-r--r--   0 root         (0) root         (0)     1405 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     1089 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/test_sys_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/processes/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/processes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/processes/bases/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/processes/bases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/saltext/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11703 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/saltext/test_log_handlers.py
--rw-r--r--   0 root         (0) root         (0)     6823 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/functional/utils/test_tempfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/cli/conftest.py
--rw-r--r--   0 root         (0) root         (0)      993 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/cli/test_salt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      609 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/api/test_api.py
--rw-r--r--   0 root         (0) root         (0)      787 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/api/test_restarts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/container/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2461 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/container/test_container_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/master/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/master/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3994 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/master/test_master.py
--rw-r--r--   0 root         (0) root         (0)      600 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/master/test_restarts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1647 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/test_event_forwarder_engine.py
--rw-r--r--   0 root         (0) root         (0)     2007 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/test_minion.py
--rw-r--r--   0 root         (0) root         (0)      655 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/test_restarts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/proxy/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/proxy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2355 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/proxy/test_proxy_minion.py
--rw-r--r--   0 root         (0) root         (0)      813 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/proxy/test_restarts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/ssh/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1697 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/ssh/test_salt_ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/sshd/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/sshd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1196 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/sshd/test_sshd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/syndic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/syndic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5526 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/syndic/test_syndic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/utils/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/utils/saltext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1069 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/integration/utils/saltext/test_log_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/scenarios/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/scenarios/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/scenarios/examples/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/scenarios/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1336 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/scenarios/examples/conftest.py
--rw-r--r--   0 root         (0) root         (0)      332 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/scenarios/examples/test_echoext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/base/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22623 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/base/test_salt_cli_factory.py
--rw-r--r--   0 root         (0) root         (0)     3125 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/base/test_salt_daemon_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1948 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/cli/test_salt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/daemons/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/daemons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1092 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/daemons/test_api.py
--rw-r--r--   0 root         (0) root         (0)      956 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/factories/daemons/test_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/markers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/markers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/saltext/__init__.py
--rw-r--r--   0 root         (0) root         (0)      665 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/saltext/test_log_handlers.py
--rw-r--r--   0 root         (0) root         (0)    20747 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/test_cli_scripts.py
--rw-r--r--   0 root         (0) root         (0)      279 2022-03-12 10:13:21.000000 pytest-salt-factories-1.0.0rc8/tests/unit/utils/test_random_string.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      745 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.github/
+-rw-r--r--   0 root         (0) root         (0)      429 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.github/CODEOWNERS
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      638 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)    30500 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.github/workflows/testing.yml
+-rw-r--r--   0 root         (0) root         (0)     1426 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4482 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4472 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)      506 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)    13608 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      548 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)     9013 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)    11339 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3410 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2033 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/changelog/
+-rw-r--r--   0 root         (0) root         (0)       12 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/changelog/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/css/
+-rw-r--r--   0 root         (0) root         (0)      425 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/css/inline-include.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/img/
+-rw-r--r--   0 root         (0) root         (0)    10359 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/img/SaltProject_Logomark_teal.png
+-rw-r--r--   0 root         (0) root         (0)     9591 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/img/SaltProject_altlogo_teal.png
+-rw-r--r--   0 root         (0) root         (0)    12539 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/img/complicated.svg
+-rw-r--r--   0 root         (0) root         (0)     2241 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/_static/img/simple.svg
+-rw-r--r--   0 root         (0) root         (0)       30 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     8259 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      314 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      563 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/
+-rw-r--r--   0 root         (0) root         (0)      143 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/bases.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/
+-rw-r--r--   0 root         (0) root         (0)      162 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/call.rst
+-rw-r--r--   0 root         (0) root         (0)      166 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/cloud.rst
+-rw-r--r--   0 root         (0) root         (0)      154 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/cp.rst
+-rw-r--r--   0 root         (0) root         (0)      158 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/key.rst
+-rw-r--r--   0 root         (0) root         (0)      158 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/run.rst
+-rw-r--r--   0 root         (0) root         (0)      147 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/salt.rst
+-rw-r--r--   0 root         (0) root         (0)      143 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/spm.rst
+-rw-r--r--   0 root         (0) root         (0)      158 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli/ssh.rst
+-rw-r--r--   0 root         (0) root         (0)      560 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli.rst
+-rw-r--r--   0 root         (0) root         (0)      157 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/client.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/daemons/
+-rw-r--r--   0 root         (0) root         (0)      161 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/daemons/api.rst
+-rw-r--r--   0 root         (0) root         (0)      162 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/daemons/container.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/daemons/master.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/daemons/minion.rst
+-rw-r--r--   0 root         (0) root         (0)      170 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/daemons/proxy.rst
+-rw-r--r--   0 root         (0) root         (0)      150 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/daemons/sshd.rst
+-rw-r--r--   0 root         (0) root         (0)      155 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/exceptions.rst
+-rw-r--r--   0 root         (0) root         (0)      472 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/index.rst
+-rw-r--r--   0 root         (0) root         (0)      188 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/manager.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/
+-rw-r--r--   0 root         (0) root         (0)      164 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/event_listener.rst
+-rw-r--r--   0 root         (0) root         (0)      175 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/factories.rst
+-rw-r--r--   0 root         (0) root         (0)      117 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/index.rst
+-rw-r--r--   0 root         (0) root         (0)      140 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/loader.rst
+-rw-r--r--   0 root         (0) root         (0)       72 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/log_server.rst
+-rw-r--r--   0 root         (0) root         (0)     1502 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/markers.rst
+-rw-r--r--   0 root         (0) root         (0)       85 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/sysinfo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/
+-rw-r--r--   0 root         (0) root         (0)      193 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/cli_scripts.rst
+-rw-r--r--   0 root         (0) root         (0)      190 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/functional.rst
+-rw-r--r--   0 root         (0) root         (0)      182 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/index.rst
+-rw-r--r--   0 root         (0) root         (0)      178 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/loader.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/markers.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/saltext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)      185 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/saltext/engines/pytest_engine.rst
+-rw-r--r--   0 root         (0) root         (0)      229 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/saltext/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/saltext/log_handlers/
+-rw-r--r--   0 root         (0) root         (0)      205 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/saltext/log_handlers/pytest_log_handler.rst
+-rw-r--r--   0 root         (0) root         (0)      179 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/utils/tempfiles.rst
+-rw-r--r--   0 root         (0) root         (0)      273 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/sitevars.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/topics/
+-rw-r--r--   0 root         (0) root         (0)      779 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/topics/fixtures.rst
+-rw-r--r--   0 root         (0) root         (0)     1032 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/topics/install.rst
+-rw-r--r--   0 root         (0) root         (0)     1540 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/docs/topics/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/
+-rw-r--r--   0 root         (0) root         (0)    11344 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      117 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/README.md
+-rw-r--r--   0 root         (0) root         (0)      307 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/requirements/
+-rw-r--r--   0 root         (0) root         (0)       13 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      132 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/
+-rw-r--r--   0 root         (0) root         (0)      863 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      506 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      551 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/modules/echo_mod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/states/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      796 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/states/echo_mod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      768 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      445 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      502 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/modules/test_echo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/states/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      539 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/states/test_echo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      506 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/modules/test_echo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/states/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/states/test_echo.py
+-rw-r--r--   0 root         (0) root         (0)    20519 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      348 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/requirements/
+-rw-r--r--   0 root         (0) root         (0)      211 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/requirements/lint.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)     3374 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      111 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3410 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9689 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      616 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      626 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/
+-rw-r--r--   0 root         (0) root         (0)     1799 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    25738 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/bases.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/
+-rw-r--r--   0 root         (0) root         (0)      147 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      743 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/call.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/cloud.py
+-rw-r--r--   0 root         (0) root         (0)      607 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/cp.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/key.py
+-rw-r--r--   0 root         (0) root         (0)      770 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/salt.py
+-rw-r--r--   0 root         (0) root         (0)      413 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/spm.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/
+-rw-r--r--   0 root         (0) root         (0)      144 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/api.py
+-rw-r--r--   0 root         (0) root         (0)    24222 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/container.py
+-rw-r--r--   0 root         (0) root         (0)    21359 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/master.py
+-rw-r--r--   0 root         (0) root         (0)    10511 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/minion.py
+-rw-r--r--   0 root         (0) root         (0)    11620 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     8150 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/sshd.py
+-rw-r--r--   0 root         (0) root         (0)     5781 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/syndic.py
+-rw-r--r--   0 root         (0) root         (0)      159 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    26033 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/
+-rw-r--r--   0 root         (0) root         (0)     2726 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18958 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/event_listener.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/factories.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/loader.py
+-rw-r--r--   0 root         (0) root         (0)     9297 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/log_server.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/markers.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/sysinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/
+-rw-r--r--   0 root         (0) root         (0)     3917 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8265 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/cli_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/coverage/
+-rw-r--r--   0 root         (0) root         (0)       86 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/coverage/sitecustomize.py
+-rw-r--r--   0 root         (0) root         (0)    17655 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/functional.py
+-rw-r--r--   0 root         (0) root         (0)     7186 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/loader.py
+-rw-r--r--   0 root         (0) root         (0)     5594 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/markers.py
+-rw-r--r--   0 root         (0) root         (0)      350 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/ports.py
+-rw-r--r--   0 root         (0) root         (0)       43 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/ports.pyi
+-rw-r--r--   0 root         (0) root         (0)      362 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/processes.py
+-rw-r--r--   0 root         (0) root         (0)       47 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/processes.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/
+-rw-r--r--   0 root         (0) root         (0)      400 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6409 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/engines/pytest_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/log_handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/log_handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13498 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/log_handlers/pytest_log_handler.py
+-rw-r--r--   0 root         (0) root         (0)    14429 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/tempfiles.py
+-rw-r--r--   0 root         (0) root         (0)     7303 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/virtualenv.py
+-rw-r--r--   0 root         (0) root         (0)       46 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/src/saltfactories/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/base/test_salt_daemon_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      973 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      548 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_call.py
+-rw-r--r--   0 root         (0) root         (0)      322 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_cloud.py
+-rw-r--r--   0 root         (0) root         (0)      316 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_cp.py
+-rw-r--r--   0 root         (0) root         (0)      318 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_key.py
+-rw-r--r--   0 root         (0) root         (0)      318 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_run.py
+-rw-r--r--   0 root         (0) root         (0)      310 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_salt.py
+-rw-r--r--   0 root         (0) root         (0)      313 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_spm.py
+-rw-r--r--   0 root         (0) root         (0)      318 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_master_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4614 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_minion_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_proxy_minion_factory.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_syndic_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/loader/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/loader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/loader/test_fixture_deps.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/loader/test_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/markers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/markers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/markers/test_requires_salt_modules.py
+-rw-r--r--   0 root         (0) root         (0)     4803 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/markers/test_requires_salt_states.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/test_sys_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/processes/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/processes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/processes/bases/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/processes/bases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/saltext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/saltext/test_log_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/functional/utils/test_tempfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/cli/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      993 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/cli/test_salt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      609 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/api/test_api.py
+-rw-r--r--   0 root         (0) root         (0)      787 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/api/test_restarts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/container/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/container/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/container/test_container_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/master/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/master/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/master/test_master.py
+-rw-r--r--   0 root         (0) root         (0)      600 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/master/test_restarts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/test_event_forwarder_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/test_minion.py
+-rw-r--r--   0 root         (0) root         (0)      655 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/test_restarts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/proxy/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/proxy/test_proxy_minion.py
+-rw-r--r--   0 root         (0) root         (0)      813 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/proxy/test_restarts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/ssh/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/ssh/test_salt_ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/sshd/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/sshd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/sshd/test_sshd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/syndic/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/syndic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/syndic/test_syndic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/utils/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/utils/saltext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/integration/utils/saltext/test_log_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/scenarios/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/scenarios/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/scenarios/examples/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/scenarios/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/scenarios/examples/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      332 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/scenarios/examples/test_echoext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22623 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/base/test_salt_cli_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/base/test_salt_daemon_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/cli/test_salt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/daemons/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/daemons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/daemons/test_api.py
+-rw-r--r--   0 root         (0) root         (0)      956 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/factories/daemons/test_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/markers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/markers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/saltext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      665 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/saltext/test_log_handlers.py
+-rw-r--r--   0 root         (0) root         (0)    20747 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/test_cli_scripts.py
+-rw-r--r--   0 root         (0) root         (0)      279 2022-03-20 12:34:55.000000 pytest-salt-factories-1.0.0rc9/tests/unit/utils/test_random_string.py
```

### Comparing `pytest-salt-factories-1.0.0rc8/.codecov.yml` & `pytest-salt-factories-1.0.0rc9/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.coveragerc` & `pytest-salt-factories-1.0.0rc9/.coveragerc`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.github/workflows/release.yml` & `pytest-salt-factories-1.0.0rc9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.github/workflows/testing.yml` & `pytest-salt-factories-1.0.0rc9/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.gitignore` & `pytest-salt-factories-1.0.0rc9/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.pre-commit-config.yaml` & `pytest-salt-factories-1.0.0rc9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.pre-commit-hooks/check-changelog-entries.py` & `pytest-salt-factories-1.0.0rc9/.pre-commit-hooks/check-changelog-entries.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.pylint-spelling-words` & `pytest-salt-factories-1.0.0rc9/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.pylintrc` & `pytest-salt-factories-1.0.0rc9/.pylintrc`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/.readthedocs.yaml` & `pytest-salt-factories-1.0.0rc9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/CHANGELOG.rst` & `pytest-salt-factories-1.0.0rc9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,23 @@
    no changelog was kept. Please refer to the git history for details.
 
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
+1.0.0rc9 (2022-03-20)
+=====================
+
+Improvements
+------------
+
+- Use old-style Salt entrypoints for improved backwards compatibility. (`#98 <https://github.com/saltstack/pytest-salt-factories/issues/98>`_)
+
+
 1.0.0rc8 (2022-03-12)
 =====================
 
 Bug Fixes
 ---------
 
 - Instead of just removing `saltfactories.utils.ports` and `saltfactories.utils.processes`, redirect the imports to the right library and show a deprecation warning. (`#106 <https://github.com/saltstack/pytest-salt-factories/issues/106>`_)
```

### Comparing `pytest-salt-factories-1.0.0rc8/LICENSE` & `pytest-salt-factories-1.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/PKG-INFO` & `pytest-salt-factories-1.0.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-salt-factories
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Pytest Salt Plugin
 Home-page: https://github.com/saltstack/pytest-salt-factories
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/saltstack/pytest-salt-factories
 Project-URL: Tracker, https://github.com/saltstack/pytest-salt-factories/issues
```

### Comparing `pytest-salt-factories-1.0.0rc8/README.rst` & `pytest-salt-factories-1.0.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/Makefile` & `pytest-salt-factories-1.0.0rc9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/_static/img/SaltProject_Logomark_teal.png` & `pytest-salt-factories-1.0.0rc9/docs/_static/img/SaltProject_Logomark_teal.png`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/_static/img/SaltProject_altlogo_teal.png` & `pytest-salt-factories-1.0.0rc9/docs/_static/img/SaltProject_altlogo_teal.png`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/_static/img/complicated.svg` & `pytest-salt-factories-1.0.0rc9/docs/_static/img/complicated.svg`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/_static/img/simple.svg` & `pytest-salt-factories-1.0.0rc9/docs/_static/img/simple.svg`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/conf.py` & `pytest-salt-factories-1.0.0rc9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/index.rst` & `pytest-salt-factories-1.0.0rc9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/make.bat` & `pytest-salt-factories-1.0.0rc9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/cli.rst` & `pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/cli.rst`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/ref/saltfactories/plugins/markers.rst` & `pytest-salt-factories-1.0.0rc9/docs/ref/saltfactories/plugins/markers.rst`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/topics/fixtures.rst` & `pytest-salt-factories-1.0.0rc9/docs/topics/fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/topics/install.rst` & `pytest-salt-factories-1.0.0rc9/docs/topics/install.rst`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/docs/topics/usage.rst` & `pytest-salt-factories-1.0.0rc9/docs/topics/usage.rst`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/LICENSE` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/setup.cfg` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/__init__.py` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/modules/echo_mod.py` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/modules/echo_mod.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/src/echoext/states/echo_mod.py` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/src/echoext/states/echo_mod.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/conftest.py` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/integration/states/test_echo.py` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/integration/states/test_echo.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/examples/echo-extension/tests/unit/states/test_echo.py` & `pytest-salt-factories-1.0.0rc9/examples/echo-extension/tests/unit/states/test_echo.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/noxfile.py` & `pytest-salt-factories-1.0.0rc9/noxfile.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/pyproject.toml` & `pytest-salt-factories-1.0.0rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/setup.cfg` & `pytest-salt-factories-1.0.0rc9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,16 @@
 	salt-factories-factories = saltfactories.plugins.factories
 	salt-factories-markers = saltfactories.plugins.markers
 	salt-factories-sysinfo = saltfactories.plugins.sysinfo
 	salt-factories-event-listener = saltfactories.plugins.event_listener
 	salt-factories-log-server = saltfactories.plugins.log_server
 	salt-factories-loader-mock = saltfactories.plugins.loader
 salt.loader = 
-	salt-factories = saltfactories.utils.saltext
+	engines_dirs      = saltfactories.utils.saltext:get_engines_dirs
+	log_handlers_dirs =  saltfactories.utils.saltext:get_log_handlers_dirs
 
 [bdist_wheel]
 universal = false
 
 [sdist]
 owner = root
 group = root
```

### Comparing `pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/PKG-INFO` & `pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-salt-factories
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Pytest Salt Plugin
 Home-page: https://github.com/saltstack/pytest-salt-factories
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/saltstack/pytest-salt-factories
 Project-URL: Tracker, https://github.com/saltstack/pytest-salt-factories/issues
```

### Comparing `pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/SOURCES.txt` & `pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
 src/saltfactories/utils/ports.pyi
 src/saltfactories/utils/processes.py
 src/saltfactories/utils/processes.pyi
 src/saltfactories/utils/tempfiles.py
 src/saltfactories/utils/virtualenv.py
 src/saltfactories/utils/coverage/sitecustomize.py
 src/saltfactories/utils/saltext/__init__.py
+src/saltfactories/utils/saltext/engines/__init__.py
 src/saltfactories/utils/saltext/engines/pytest_engine.py
 src/saltfactories/utils/saltext/log_handlers/__init__.py
 src/saltfactories/utils/saltext/log_handlers/pytest_log_handler.py
 tests/__init__.py
 tests/conftest.py
 tests/functional/__init__.py
 tests/functional/test_cli.py
```

### Comparing `pytest-salt-factories-1.0.0rc8/src/pytest_salt_factories.egg-info/requires.txt` & `pytest-salt-factories-1.0.0rc9/src/pytest_salt_factories.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/__init__.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/__main__.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/__main__.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/bases.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/bases.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/call.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/call.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/cloud.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/cloud.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/cp.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/cp.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/key.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/key.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/run.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/run.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/salt.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/salt.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/cli/ssh.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/cli/ssh.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/client.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/client.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/api.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/api.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/container.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/container.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/master.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/master.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/minion.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/minion.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/proxy.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/proxy.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/sshd.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/sshd.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/daemons/syndic.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/daemons/syndic.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/manager.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/manager.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/__init__.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/event_listener.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/event_listener.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/factories.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/loader.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/loader.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/log_server.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/log_server.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/markers.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/markers.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/plugins/sysinfo.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/plugins/sysinfo.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/__init__.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/cli_scripts.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/functional.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/functional.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/loader.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/loader.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/markers.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/markers.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/engines/pytest_engine.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/engines/pytest_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 Simple salt engine which will setup a socket to accept connections allowing us to know
 when a daemon is up and running
 """
 import atexit
 import datetime
 import logging
 import threading
+from collections.abc import MutableMapping
 
-import zmq
-
-try:
-    from collections.abc import MutableMapping
-except ImportError:
-    # Py2 compat
-    from collections import MutableMapping
 try:
     import msgpack
 
     HAS_MSGPACK = True
-except ImportError:
+except ImportError:  # pragma: no cover
     HAS_MSGPACK = False
+try:
+    import zmq
+
+    HAS_ZMQ = True
+except ImportError:  # pragma: no cover
+    HAS_ZMQ = False
+
 
 import salt.utils.event
 
 try:
     import salt.utils.immutabletypes as immutabletypes
 except ImportError:
     immutabletypes = None
@@ -38,24 +39,28 @@
 
 log = logging.getLogger(__name__)
 
 __virtualname__ = "pytest"
 
 
 def __virtual__():
+    if HAS_MSGPACK is False:
+        return False, "msgpack was not importable. Please install msgpack."
+    if HAS_ZMQ is False:
+        return False, "zmq was not importable. Please install pyzmq."
+    if "__role" not in __opts__:
+        return False, "The required '__role' key could not be found in the options dictionary"
     role = __opts__["__role"]
     pytest_key = "pytest-{}".format(role)
     if pytest_key not in __opts__:
         return False, "No '{}' key in opts dictionary".format(pytest_key)
 
     pytest_config = __opts__[pytest_key]
     if "returner_address" not in pytest_config:
         return False, "No 'returner_address' key in opts['{}'] dictionary".format(pytest_key)
-    if HAS_MSGPACK is False:
-        return False, "msgpack was not importable. Please install msgpack."
     return True
 
 
 def start():
     """
     Method to start the engine.
     """
```

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/saltext/log_handlers/pytest_log_handler.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/saltext/log_handlers/pytest_log_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 
 __virtualname__ = "pytest_log_handler"
 
 log = logging.getLogger(__name__)
 
 
 def __virtual__():
+    if HAS_MSGPACK is False:
+        return False, "msgpack was not importable. Please install msgpack."
+    if HAS_ZMQ is False:
+        return False, "zmq was not importable. Please install pyzmq."
+    if "__role" not in __opts__:
+        return False, "The required '__role' key could not be found in the options dictionary"
     role = __opts__["__role"]
     pytest_key = "pytest-{}".format(role)
 
     if pytest_key not in __opts__ and "pytest" not in __opts__:
         return False, "Neither '{}' nor 'pytest' keys in opts dictionary".format(pytest_key)
 
     if pytest_key not in __opts__:
@@ -61,18 +67,14 @@
     if "port" not in log_opts:
         return (
             False,
             "No 'port' key in opts['pytest']['log'] or opts['pytest'][{}]['log']".format(
                 __opts__["role"]
             ),
         )
-    if HAS_MSGPACK is False:
-        return False, "msgpack was not importable. Please install msgpack."
-    if HAS_ZMQ is False:
-        return False, "zmq was not importable. Please install pyzmq."
     return True
 
 
 def setup_handlers():
     """
     Setup the handlers.
     """
```

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/tempfiles.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/tempfiles.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/src/saltfactories/utils/virtualenv.py` & `pytest-salt-factories-1.0.0rc9/src/saltfactories/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/conftest.py` & `pytest-salt-factories-1.0.0rc9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/factories/base/test_salt_daemon_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/factories/base/test_salt_daemon_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/conftest.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/factories/cli/test_call.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/factories/cli/test_call.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_master_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_master_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_minion_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_minion_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_proxy_minion_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_proxy_minion_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/factories/daemons/test_syndic_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/factories/daemons/test_syndic_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/loader/test_fixture_deps.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/loader/test_fixture_deps.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/loader/test_loader.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/markers/test_requires_salt_modules.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/markers/test_requires_salt_modules.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/markers/test_requires_salt_states.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/markers/test_requires_salt_states.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/test_cli.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/test_sys_info.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/test_sys_info.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/utils/saltext/test_log_handlers.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/utils/saltext/test_log_handlers.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/functional/utils/test_tempfiles.py` & `pytest-salt-factories-1.0.0rc9/tests/functional/utils/test_tempfiles.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/cli/conftest.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/cli/test_salt.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/cli/test_salt.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/api/test_api.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/api/test_api.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/api/test_restarts.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/api/test_restarts.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/container/test_container_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/container/test_container_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/master/test_master.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/master/test_master.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/master/test_restarts.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/master/test_restarts.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/test_event_forwarder_engine.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/test_event_forwarder_engine.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/test_minion.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/test_minion.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/minion/test_restarts.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/minion/test_restarts.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/proxy/test_proxy_minion.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/proxy/test_proxy_minion.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/proxy/test_restarts.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/proxy/test_restarts.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/ssh/test_salt_ssh.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/ssh/test_salt_ssh.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/sshd/test_sshd.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/sshd/test_sshd.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/factories/daemons/syndic/test_syndic.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/factories/daemons/syndic/test_syndic.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/integration/utils/saltext/test_log_handlers.py` & `pytest-salt-factories-1.0.0rc9/tests/integration/utils/saltext/test_log_handlers.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/scenarios/examples/conftest.py` & `pytest-salt-factories-1.0.0rc9/tests/scenarios/examples/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/unit/factories/base/test_salt_cli_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/unit/factories/base/test_salt_cli_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/unit/factories/base/test_salt_daemon_factory.py` & `pytest-salt-factories-1.0.0rc9/tests/unit/factories/base/test_salt_daemon_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/unit/factories/cli/test_salt.py` & `pytest-salt-factories-1.0.0rc9/tests/unit/factories/cli/test_salt.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/unit/factories/daemons/test_api.py` & `pytest-salt-factories-1.0.0rc9/tests/unit/factories/daemons/test_api.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/unit/factories/daemons/test_container.py` & `pytest-salt-factories-1.0.0rc9/tests/unit/factories/daemons/test_container.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/unit/utils/saltext/test_log_handlers.py` & `pytest-salt-factories-1.0.0rc9/tests/unit/utils/saltext/test_log_handlers.py`

 * *Files identical despite different names*

### Comparing `pytest-salt-factories-1.0.0rc8/tests/unit/utils/test_cli_scripts.py` & `pytest-salt-factories-1.0.0rc9/tests/unit/utils/test_cli_scripts.py`

 * *Files identical despite different names*

