# Comparing `tmp/jupyter_events-0.6.3.tar.gz` & `tmp/jupyter_events-0.7.0.tar.gz`

## Comparing `jupyter_events-0.6.3.tar` & `jupyter_events-0.7.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/CHANGELOG.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/RELEASE.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/codecov.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/.github/dependabot.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/Makefile
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/conf.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/index.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/make.bat
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/demo/demo-notebook.ipynb
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/demo/index.md
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/application.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/configure.md
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/defining-schema.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/event-schemas.md
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/first-event.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/index.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/listeners.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/docs/user_guide/modifiers.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/_version.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/cli.py
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/py.typed
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/pytest_plugin.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/schema.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/schema_registry.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/traits.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/validators.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/yaml.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/schemas/event-core-schema.yml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/schemas/event-metaschema.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/jupyter_events/schemas/property-metaschema.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/conftest.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/test_cli.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/test_listeners.py
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/test_logger.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/test_modifiers.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/test_schema.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/test_traits.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/utils.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/bad/bad-id.yaml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/bad/invalid.yaml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/bad/nested-reserved-property.yaml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/bad/reserved-property.yaml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/good/array.yaml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/good/basic.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/good/basic.yaml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/good/nested-array.yaml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/tests/schemas/good/user.yaml
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/COPYING.md
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/README.md
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jupyter_events-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/RELEASE.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/index.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/demo/demo-notebook.ipynb
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/demo/index.md
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/application.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/configure.md
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/defining-schema.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/event-schemas.md
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/first-event.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/index.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/listeners.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/docs/user_guide/modifiers.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/_version.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/cli.py
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/py.typed
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/pytest_plugin.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/schema.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/schema_registry.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/traits.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/validators.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/yaml.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/schemas/event-core-schema.yml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/schemas/event-metaschema.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/jupyter_events/schemas/property-metaschema.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/test_cli.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/test_listeners.py
+-rw-r--r--   0        0        0    14400 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/test_logger.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/test_modifiers.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/test_schema.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/test_traits.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/utils.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/bad/bad-id.yaml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/bad/invalid.yaml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/bad/nested-reserved-property.yaml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/bad/reserved-property.yaml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/good/array.yaml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/good/basic.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/good/basic.yaml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/good/nested-array.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/tests/schemas/good/user.yaml
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/README.md
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 jupyter_events-0.7.0/PKG-INFO
```

### Comparing `jupyter_events-0.6.3/.pre-commit-config.yaml` & `jupyter_events-0.7.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,26 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.19.2
+    rev: 0.23.2
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.194
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.276
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyter_events-0.6.3/CHANGELOG.md` & `jupyter_events-0.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.7.0
+
+([Full Changelog](https://github.com/jupyter/jupyter_events/compare/v0.6.3...56e7d2660b59632765a85859217cddc7304e82f8))
+
+### Enhancements made
+
+- allow a 'message' field in an event schema [#72](https://github.com/jupyter/jupyter_events/pull/72) ([@Zsailer](https://github.com/Zsailer))
+
+### Bugs fixed
+
+- Improve usability of jp_read_emitted_events fixture [#74](https://github.com/jupyter/jupyter_events/pull/74) ([@kevin-bates](https://github.com/kevin-bates))
+
+### Maintenance and upkeep improvements
+
+- Migrate RefResolver to referencing.Registry [#80](https://github.com/jupyter/jupyter_events/pull/80) ([@hbcarlos](https://github.com/hbcarlos))
+- Use local coverage [#73](https://github.com/jupyter/jupyter_events/pull/73) ([@blink1073](https://github.com/blink1073))
+- Clean up license [#67](https://github.com/jupyter/jupyter_events/pull/67) ([@dcsaba89](https://github.com/dcsaba89))
+- Add more linting [#65](https://github.com/jupyter/jupyter_events/pull/65) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/jupyter_events/graphs/contributors?from=2023-01-12&to=2023-07-31&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_events+involves%3Ablink1073+updated%3A2023-01-12..2023-07-31&type=Issues) | [@dcsaba89](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_events+involves%3Adcsaba89+updated%3A2023-01-12..2023-07-31&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_events+involves%3Ahbcarlos+updated%3A2023-01-12..2023-07-31&type=Issues) | [@kevin-bates](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_events+involves%3Akevin-bates+updated%3A2023-01-12..2023-07-31&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_events+involves%3Apre-commit-ci+updated%3A2023-01-12..2023-07-31&type=Issues) | [@Zsailer](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_events+involves%3AZsailer+updated%3A2023-01-12..2023-07-31&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.6.3
 
 ([Full Changelog](https://github.com/jupyter/jupyter_events/compare/v0.6.2...ac65980322317f1f30bc07150c9e14afaad03d40))
 
 ### Maintenance and upkeep improvements
 
 - Clean up typing [#64](https://github.com/jupyter/jupyter_events/pull/64) ([@blink1073](https://github.com/blink1073))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/jupyter_events/graphs/contributors?from=2023-01-10&to=2023-01-12&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_events+involves%3Ablink1073+updated%3A2023-01-10..2023-01-12&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.6.2
 
 ([Full Changelog](https://github.com/jupyter/jupyter_events/compare/v0.6.1...a00859944090df5277f263fcfe72ae48b8cc2382))
 
 ### Maintenance and upkeep improvements
 
 - Decrease pyyaml dependency floor to increase compatibility [#63](https://github.com/jupyter/jupyter_events/pull/63) ([@kevin-bates](https://github.com/kevin-bates))
```

### Comparing `jupyter_events-0.6.3/RELEASE.md` & `jupyter_events-0.7.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/.github/workflows/prep-release.yml` & `jupyter_events-0.7.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/.github/workflows/publish-release.yml` & `jupyter_events-0.7.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/.github/workflows/python-tests.yml` & `jupyter_events-0.7.0/.github/workflows/python-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,31 +14,38 @@
   build:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ["3.7", "3.11"]
+        python-version: ["3.8", "3.12"]
         include:
           - os: windows-latest
             python-version: "3.9"
           - os: ubuntu-latest
             python-version: "pypy-3.8"
           - os: ubuntu-latest
             python-version: "3.10"
           - os: macos-latest
-            python-version: "3.8"
+            python-version: "3.11"
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Run Tests
         run: hatch run cov:test
-      - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
+
+  coverage:
+    runs-on: ubuntu-latest
+    needs:
+      - build
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
 
   docs:
     runs-on: windows-latest
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - run: hatch run docs:build
@@ -146,15 +153,15 @@
         with:
           version_spec: 100.100.100
           token: ${{ secrets.GITHUB_TOKEN }}
 
   tests_check: # This job does nothing and is only used for the branch protection
     if: always()
     needs:
-      - build
+      - coverage
       - docs
       - test_lint
       - check_release
       - test_minimum_versions
       - test_prereleases
       - jupyter_server_downstream
       - test_sdist
```

### Comparing `jupyter_events-0.6.3/docs/Makefile` & `jupyter_events-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/conf.py` & `jupyter_events-0.7.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 from typing import List
 
 project = "jupyter_events"
-copyright = "2019, Project Jupyter"
+copyright = "2019, Project Jupyter"  # noqa
 author = "Project Jupyter"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `jupyter_events-0.6.3/docs/index.md` & `jupyter_events-0.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/make.bat` & `jupyter_events-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/_static/jupyter_logo.png` & `jupyter_events-0.7.0/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/demo/demo-notebook.ipynb` & `jupyter_events-0.7.0/docs/demo/demo-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/user_guide/application.md` & `jupyter_events-0.7.0/docs/user_guide/application.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/user_guide/configure.md` & `jupyter_events-0.7.0/docs/user_guide/configure.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/user_guide/defining-schema.md` & `jupyter_events-0.7.0/docs/user_guide/defining-schema.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/user_guide/event-schemas.md` & `jupyter_events-0.7.0/docs/user_guide/event-schemas.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/user_guide/first-event.md` & `jupyter_events-0.7.0/docs/user_guide/first-event.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/user_guide/listeners.md` & `jupyter_events-0.7.0/docs/user_guide/listeners.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/docs/user_guide/modifiers.md` & `jupyter_events-0.7.0/docs/user_guide/modifiers.md`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/jupyter_events/cli.py` & `jupyter_events-0.7.0/jupyter_events/cli.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/jupyter_events/logger.py` & `jupyter_events-0.7.0/jupyter_events/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 """
 import asyncio
 import copy
 import inspect
 import json
 import logging
 import warnings
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import Any, Callable, Coroutine, Optional, Union
 
 from jsonschema import ValidationError
-from pythonjsonlogger import jsonlogger  # type:ignore
+from pythonjsonlogger import jsonlogger
 from traitlets import Dict, Instance, Set, default
 from traitlets.config import Config, LoggingConfigurable
 
 from .schema import SchemaType
 from .schema_registry import SchemaRegistry
 from .traits import Handlers
 from .validators import JUPYTER_EVENTS_CORE_VALIDATOR
@@ -59,15 +59,15 @@
     Event schemas must be registered with the
     EventLogger using the `register_schema` or
     `register_schema_file` methods. Every schema
     will be validated against Jupyter Event's metaschema.
     """
 
     handlers = Handlers(
-        default_value=[],
+        default_value=None,
         allow_none=True,
         help="""A list of logging.Handler instances to send events to.
 
         When set to None (the default), all events are discarded.
         """,
     ).tag(config=True)
 
@@ -145,24 +145,29 @@
 
     def register_handler(self, handler: logging.Handler) -> None:
         """Register a new logging handler to the Event Logger.
 
         All outgoing messages will be formatted as a JSON string.
         """
 
-        def _skip_message(record, **kwargs):
+        def _handle_message_field(record, **kwargs):
+            """Python's logger always emits the "message" field with
+            the value as "null" unless it's present in the schema/data.
+            Message happens to be a common field for event logs,
+            so special case it here and only emit it if "message"
+            is found the in the schema's property list.
             """
-            Remove 'message' from log record.
-            It is always emitted with 'null', and we do not want it,
-            since we are always emitting events only
-            """
-            del record["message"]
+            schema = self.schemas.get(record["__schema__"])
+            if "message" not in schema.properties:
+                del record["message"]
             return json.dumps(record, **kwargs)
 
-        formatter = jsonlogger.JsonFormatter(json_serializer=_skip_message)
+        formatter = jsonlogger.JsonFormatter(
+            json_serializer=_handle_message_field,
+        )
         handler.setFormatter(formatter)
         self._logger.addHandler(handler)
         if handler not in self.handlers:
             self.handlers.append(handler)
 
     def remove_handler(self, handler: logging.Handler) -> None:
         """Remove a logging handler from the logger and list of handlers."""
@@ -204,17 +209,17 @@
         # Assert this signature or raise an exception
         if signature == expected_signature:
             # If the schema ID and version is given, only add
             # this modifier to that schema
             if schema_id:
                 self._modifiers[schema_id].add(modifier)
                 return
-            for id in self._modifiers:
-                if schema_id is None or id == schema_id:
-                    self._modifiers[id].add(modifier)
+            for id_ in self._modifiers:
+                if schema_id is None or id_ == schema_id:
+                    self._modifiers[id_].add(modifier)
         else:
             msg = (
                 "Modifiers are required to follow an exact function/method "
                 "signature. The signature should look like:"
                 f"\n\n\tdef my_modifier{expected_signature}:\n\n"
                 "Check that you are using type annotations for each argument "
                 "and the return value."
@@ -279,18 +284,18 @@
             # If the schema ID and version is given, only add
             # this modifier to that schema
             if schema_id:
                 if modified:
                     self._modified_listeners[schema_id].add(listener)
                     return
                 self._unmodified_listeners[schema_id].add(listener)
-            for id in self.schemas.schema_ids:
-                if schema_id is None or id == schema_id:
+            for id_ in self.schemas.schema_ids:
+                if schema_id is None or id_ == schema_id:
                     if modified:
-                        self._modified_listeners[id].add(listener)
+                        self._modified_listeners[id_].add(listener)
                     else:
                         self._unmodified_listeners[schema_id].add(listener)
         else:
             msg = (
                 "Listeners are required to follow an exact function/method "
                 "signature. The signature should look like:"
                 f"\n\n\tasync def my_listener{expected_signature}:\n\n"
@@ -359,14 +364,15 @@
         # this was intended.
         if schema_id not in self.schemas:
             warnings.warn(
                 f"{schema_id} has not been registered yet. If "
                 "this was not intentional, please register the schema using the "
                 "`register_event_schema` method.",
                 SchemaNotRegistered,
+                stacklevel=2,
             )
             return None
 
         schema = self.schemas.get(schema_id)
 
         # Deep copy the data and modify the copy.
         modified_data = copy.deepcopy(data)
@@ -377,18 +383,17 @@
             # Process this event, i.e. validate and modify (in place)
             self.schemas.validate_event(schema_id, data)
 
         # Validate the modified data.
         self.schemas.validate_event(schema_id, modified_data)
 
         # Generate the empty event capsule.
-        if timestamp_override is None:
-            timestamp = datetime.utcnow()
-        else:
-            timestamp = timestamp_override
+        timestamp = (
+            datetime.now(tz=timezone.utc) if timestamp_override is None else timestamp_override
+        )
         capsule = {
             "__timestamp__": timestamp.isoformat() + "Z",
             "__schema__": schema_id,
             "__schema_version__": schema.version,
             "__metadata_version__": EVENTS_METADATA_VERSION,
         }
         try:
```

### Comparing `jupyter_events-0.6.3/jupyter_events/pytest_plugin.py` & `jupyter_events-0.7.0/jupyter_events/pytest_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 @pytest.fixture
 def jp_read_emitted_events(jp_event_handler, jp_event_sink):
     """Reads list of events since last time it was called."""
 
     def _read():
         jp_event_handler.flush()
-        lines = jp_event_sink.getvalue().strip().split("\n")
-        output = [json.loads(item) for item in lines]
+        event_buf = jp_event_sink.getvalue().strip()
+        output = [json.loads(item) for item in event_buf.split("\n")] if event_buf else None
         # Clear the sink.
         jp_event_sink.truncate(0)
         jp_event_sink.seek(0)
         return output
 
     return _read
```

### Comparing `jupyter_events-0.6.3/jupyter_events/schema.py` & `jupyter_events-0.7.0/jupyter_events/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Event schema objects."""
 import json
 from pathlib import Path, PurePath
 from typing import Optional, Type, Union
 
-from jsonschema import FormatChecker, RefResolver, validators
+from jsonschema import FormatChecker, validators
+from referencing import Registry
+from referencing.jsonschema import DRAFT7
 
 try:
     from jsonschema.protocols import Validator
 except ImportError:
     from typing import Any
 
     Validator = Any  # type:ignore
@@ -51,31 +53,35 @@
     validator_class: jsonschema.validators
         The validator class from jsonschema used to validate instances
         of this event schema. The schema itself will be validated
         against Jupyter Event's metaschema to ensure that
         any schema registered here follows the expected form
         of Jupyter Events.
 
-    resolver:
-        RefResolver for nested JSON schema references.
+    registry:
+        Registry for nested JSON schema references.
     """
 
     def __init__(
         self,
         schema: SchemaType,
         validator_class: Type[Validator] = validators.Draft7Validator,  # type:ignore[assignment]
         format_checker: FormatChecker = draft7_format_checker,
-        resolver: Optional[RefResolver] = None,
+        registry: Optional[Registry] = None,
     ):
         """Initialize an event schema."""
         _schema = self._load_schema(schema)
         # Validate the schema against Jupyter Events metaschema.
         validate_schema(_schema)
+
+        if registry is None:
+            registry = DRAFT7.create_resource(_schema) @ Registry()
+
         # Create a validator for this schema
-        self._validator = validator_class(_schema, resolver=resolver, format_checker=format_checker)
+        self._validator = validator_class(_schema, registry=registry, format_checker=format_checker)  # type: ignore
         self._schema = _schema
 
     def __repr__(self):
         """A string repr for an event schema."""
         return json.dumps(self._schema, indent=2)
 
     @staticmethod
@@ -131,19 +137,23 @@
             EventSchema._ensure_yaml_loaded(loaded_schema, was_str=True)
             return loaded_schema
 
         msg = f"Expected a dictionary, string, or PurePath, but instead received {schema.__class__.__name__}."
         raise EventSchemaUnrecognized(msg)
 
     @property
-    def id(self) -> str:
+    def id(self) -> str:  # noqa
         """Schema $id field."""
         return self._schema["$id"]
 
     @property
     def version(self) -> int:
         """Schema's version."""
         return self._schema["version"]
 
+    @property
+    def properties(self) -> dict:
+        return self._schema["properties"]
+
     def validate(self, data: dict) -> None:
         """Validate an incoming instance of this event schema."""
         self._validator.validate(data)
```

### Comparing `jupyter_events-0.6.3/jupyter_events/schema_registry.py` & `jupyter_events-0.7.0/jupyter_events/schema_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,39 +43,39 @@
         found here:
         """
         if not isinstance(schema, EventSchema):
             schema = EventSchema(schema)
         self._add(schema)
         return schema
 
-    def get(self, id: str) -> EventSchema:
+    def get(self, id_: str) -> EventSchema:
         """Fetch a given schema. If the schema is not found,
         this will raise a KeyError.
         """
         try:
-            return self._schemas[id]
+            return self._schemas[id_]
         except KeyError:
             msg = (
-                f"The requested schema, {id}, was not found in the "
+                f"The requested schema, {id_}, was not found in the "
                 "schema registry. Are you sure it was previously registered?"
             )
             raise KeyError(msg) from None
 
-    def remove(self, id: str) -> None:
+    def remove(self, id_: str) -> None:
         """Remove a given schema. If the schema is not found,
         this will raise a KeyError.
         """
         try:
-            del self._schemas[id]
+            del self._schemas[id_]
         except KeyError:
             msg = (
-                f"The requested schema, {id}, was not found in the "
+                f"The requested schema, {id_}, was not found in the "
                 "schema registry. Are you sure it was previously registered?"
             )
             raise KeyError(msg) from None
 
-    def validate_event(self, id: str, data: dict) -> None:
+    def validate_event(self, id_: str, data: dict) -> None:
         """Validate an event against a schema within this
         registry.
         """
-        schema = self.get(id)
+        schema = self.get(id_)
         schema.validate(data)
```

### Comparing `jupyter_events-0.6.3/jupyter_events/traits.py` & `jupyter_events-0.7.0/jupyter_events/traits.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/jupyter_events/validators.py` & `jupyter_events-0.7.0/jupyter_events/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Event validators."""
 import pathlib
 
 import jsonschema
-from jsonschema import Draft7Validator, RefResolver, ValidationError
+from jsonschema import Draft7Validator, ValidationError
+from referencing import Registry
+from referencing.jsonschema import DRAFT7
+
+from . import yaml
 
 draft7_format_checker = (
     Draft7Validator.FORMAT_CHECKER
     if hasattr(Draft7Validator, "FORMAT_CHECKER")
     else jsonschema.draft7_format_checker
 )
 
-from . import yaml
 
 METASCHEMA_PATH = pathlib.Path(__file__).parent.joinpath("schemas")
 
 EVENT_METASCHEMA_FILEPATH = METASCHEMA_PATH.joinpath("event-metaschema.yml")
 EVENT_METASCHEMA = yaml.load(EVENT_METASCHEMA_FILEPATH)
 
 EVENT_CORE_SCHEMA_FILEPATH = METASCHEMA_PATH.joinpath("event-core-schema.yml")
@@ -25,27 +28,29 @@
 
 SCHEMA_STORE = {
     EVENT_METASCHEMA["$id"]: EVENT_METASCHEMA,
     PROPERTY_METASCHEMA["$id"]: PROPERTY_METASCHEMA,
     EVENT_CORE_SCHEMA["$id"]: EVENT_CORE_SCHEMA,
 }
 
-METASCHEMA_RESOLVER = RefResolver(
-    base_uri=EVENT_METASCHEMA["$id"], referrer=EVENT_METASCHEMA, store=SCHEMA_STORE
-)
+resources = [
+    DRAFT7.create_resource(each)
+    for each in (EVENT_METASCHEMA, PROPERTY_METASCHEMA, EVENT_CORE_SCHEMA)
+]
+METASCHEMA_REGISTRY: Registry = resources @ Registry()
 
-JUPYTER_EVENTS_SCHEMA_VALIDATOR = Draft7Validator(
+JUPYTER_EVENTS_SCHEMA_VALIDATOR = Draft7Validator(  # type: ignore
     schema=EVENT_METASCHEMA,
-    resolver=METASCHEMA_RESOLVER,
+    registry=METASCHEMA_REGISTRY,
     format_checker=draft7_format_checker,
 )
 
-JUPYTER_EVENTS_CORE_VALIDATOR = Draft7Validator(
+JUPYTER_EVENTS_CORE_VALIDATOR = Draft7Validator(  # type: ignore
     schema=EVENT_CORE_SCHEMA,
-    resolver=METASCHEMA_RESOLVER,
+    registry=METASCHEMA_REGISTRY,
     format_checker=draft7_format_checker,
 )
 
 
 def validate_schema(schema: dict) -> None:
     """Validate a schema dict."""
     try:
```

### Comparing `jupyter_events-0.6.3/jupyter_events/yaml.py` & `jupyter_events-0.7.0/jupyter_events/yaml.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/jupyter_events/schemas/event-core-schema.yml` & `jupyter_events-0.7.0/jupyter_events/schemas/event-core-schema.yml`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/jupyter_events/schemas/event-metaschema.yml` & `jupyter_events-0.7.0/jupyter_events/schemas/event-metaschema.yml`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/jupyter_events/schemas/property-metaschema.yml` & `jupyter_events-0.7.0/jupyter_events/schemas/property-metaschema.yml`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/test_cli.py` & `jupyter_events-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/test_listeners.py` & `jupyter_events-0.7.0/tests/test_listeners.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/test_logger.py` & `jupyter_events-0.7.0/tests/test_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 import json
 import logging
-from datetime import datetime, timedelta
+import sys
+from datetime import datetime, timedelta, timezone
 from unittest.mock import MagicMock
 
 import jsonschema
 import pytest
 from jsonschema.exceptions import ValidationError
 from traitlets import TraitError
 from traitlets.config.loader import PyFileConfigLoader
@@ -109,15 +110,15 @@
     }
 
     output = io.StringIO()
     handler = logging.StreamHandler(output)
     el = EventLogger(handlers=[handler])
     el.register_event_schema(schema)
 
-    timestamp_override = datetime.utcnow() - timedelta(days=1)
+    timestamp_override = datetime.now(tz=timezone.utc) - timedelta(days=1)
 
     el.emit(
         schema_id="http://test/test",
         data={"something": "blah"},
         timestamp_override=timestamp_override,
     )
     handler.flush()
@@ -132,15 +133,15 @@
     schema = {
         "$id": "http://test/test",
         "version": 1,
         "properties": {
             "something": {
                 "type": "string",
                 "title": "test",
-            },
+            }
         },
     }
 
     output = io.StringIO()
     handler = logging.StreamHandler(output)
     el = EventLogger(handlers=[handler])
     el.register_event_schema(schema)
@@ -154,20 +155,120 @@
     handler.flush()
 
     event_capsule = json.loads(output.getvalue())
 
     assert "__timestamp__" in event_capsule
     # Remove timestamp from capsule when checking equality, since it is gonna vary
     del event_capsule["__timestamp__"]
-    assert event_capsule == {
+    expected = {
         "__schema__": "http://test/test",
         "__schema_version__": 1,
         "__metadata_version__": 1,
         "something": "blah",
     }
+    if sys.version_info >= (3, 12):
+        expected["taskName"] = None
+    assert event_capsule == expected
+
+
+def test_message_field():
+    """
+    Simple test for emitting an event with
+    the literal property "message".
+    """
+    schema = {
+        "$id": "http://test/test",
+        "version": 1,
+        "properties": {
+            "something": {
+                "type": "string",
+                "title": "test",
+            },
+            "message": {
+                "type": "string",
+                "title": "test",
+            },
+        },
+    }
+
+    output = io.StringIO()
+    handler = logging.StreamHandler(output)
+    el = EventLogger(handlers=[handler])
+    el.register_event_schema(schema)
+
+    el.emit(
+        schema_id="http://test/test",
+        data={"something": "blah", "message": "a message was seen"},
+    )
+    handler.flush()
+
+    event_capsule = json.loads(output.getvalue())
+
+    assert "__timestamp__" in event_capsule
+    # Remove timestamp from capsule when checking equality, since it is gonna vary
+    del event_capsule["__timestamp__"]
+    expected = {
+        "__schema__": "http://test/test",
+        "__schema_version__": 1,
+        "__metadata_version__": 1,
+        "something": "blah",
+        "message": "a message was seen",
+    }
+    if sys.version_info >= (3, 12):
+        expected["taskName"] = None
+    assert event_capsule == expected
+
+
+def test_nested_message_field():
+    """
+    Simple test for emitting an event with
+    the literal property "message".
+    """
+    schema = {
+        "$id": "http://test/test",
+        "version": 1,
+        "properties": {
+            "thing": {
+                "type": "object",
+                "title": "thing",
+                "properties": {
+                    "message": {
+                        "type": "string",
+                        "title": "message",
+                    },
+                },
+            },
+        },
+    }
+
+    output = io.StringIO()
+    handler = logging.StreamHandler(output)
+    el = EventLogger(handlers=[handler])
+    el.register_event_schema(schema)
+
+    el.emit(
+        schema_id="http://test/test",
+        data={"thing": {"message": "a nested message was seen"}},
+    )
+    handler.flush()
+
+    event_capsule = json.loads(output.getvalue())
+
+    assert "__timestamp__" in event_capsule
+    # Remove timestamp from capsule when checking equality, since it is gonna vary
+    del event_capsule["__timestamp__"]
+    expected = {
+        "__schema__": "http://test/test",
+        "__schema_version__": 1,
+        "__metadata_version__": 1,
+        "thing": {"message": "a nested message was seen"},
+    }
+    if sys.version_info >= (3, 12):
+        expected["taskName"] = None
+    assert event_capsule == expected
 
 
 def test_register_event_schema(tmp_path):
     """
     Register schema from a file
     """
     schema = {
@@ -316,32 +417,38 @@
     handler1.flush()
 
     event_capsule0 = json.loads(output0.getvalue())
 
     assert "__timestamp__" in event_capsule0
     # Remove timestamp from capsule when checking equality, since it is gonna vary
     del event_capsule0["__timestamp__"]
-    assert event_capsule0 == {
+    expected = {
         "__schema__": "http://test/test0",
         "__schema_version__": 1,
         "__metadata_version__": 1,
         "something": "blah",
     }
+    if sys.version_info >= (3, 12):
+        expected["taskName"] = None
+    assert event_capsule0 == expected
 
     event_capsule1 = json.loads(output1.getvalue())
 
     assert "__timestamp__" in event_capsule1
     # Remove timestamp from capsule when checking equality, since it is gonna vary
     del event_capsule1["__timestamp__"]
-    assert event_capsule1 == {
+    expected = {
         "__schema__": "http://test/test1",
         "__schema_version__": 1,
         "__metadata_version__": 1,
         "something": "blah",
     }
+    if sys.version_info >= (3, 12):
+        expected["taskName"] = None
+    assert event_capsule1 == expected
 
 
 def test_register_duplicate_schemas():
     schema0 = {
         "$id": "http://test/test",
         "version": 1,
         "type": "object",
```

### Comparing `jupyter_events-0.6.3/tests/test_modifiers.py` & `jupyter_events-0.7.0/tests/test_modifiers.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/test_schema.py` & `jupyter_events-0.7.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/test_traits.py` & `jupyter_events-0.7.0/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/utils.py` & `jupyter_events-0.7.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/schemas/bad/nested-reserved-property.yaml` & `jupyter_events-0.7.0/tests/schemas/bad/nested-reserved-property.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/tests/schemas/good/nested-array.yaml` & `jupyter_events-0.7.0/tests/schemas/good/nested-array.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_events-0.6.3/.gitignore` & `jupyter_events-0.7.0/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -101,7 +101,10 @@
 /site
 
 # mypy
 .mypy_cache/
 
 .DS_Store
 .vscode/
+
+# pycharm
+.idea/
```

### Comparing `jupyter_events-0.6.3/pyproject.toml` & `jupyter_events-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling>=1.5"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter-events"
 description = "Jupyter Event System library"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
     { name = "Jupyter Development Team", email = "jupyter@googlegroups.com" },
 ]
 keywords = [
     "Jupyter",
     "JupyterLab",
 ]
@@ -19,30 +19,31 @@
     "Intended Audience :: Science/Research",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "jsonschema[format-nongpl,format_nongpl]>=3.2.0",
+    "referencing",
+    "jsonschema[format-nongpl,format_nongpl]>=4.18.0",
     "python-json-logger>=2.0.4",
     "pyyaml>=5.3",
     "traitlets>=5.3",
     # The following are necessary to address an issue where pyproject.toml normalizes extra dependencies
     # such that 'format_nongpl' is normalized to 'format-nongpl' which prevents these two validators from
     # from being installed when jsonschema is <= 4.9 because jsonschema uses 'format_nongpl' in those releases.
     "rfc3339-validator",
     "rfc3986-validator>=0.1.1",
 ]
 dynamic = [
     "version",
 ]
 
 [project.license]
-file = 'COPYING.md'
+file = 'LICENSE'
 
 [project.urls]
 Homepage = "http://jupyter.org"
 
 [project.scripts]
 jupyter-events = "jupyter_events.cli:main"
 
@@ -50,19 +51,17 @@
 docs = [
     "jupyterlite-sphinx",
     "myst_parser",
     "pydata_sphinx_theme",
     "sphinxcontrib-spelling",
 ]
 test = [
-    "coverage",
     "pre-commit",
     "pytest-asyncio>=0.19.0",
     "pytest-console-scripts",
-    "pytest-cov",
     "pytest>=7.0",
     # [cli]
     "click",
     "rich",
 ]
 cli = [
     "click",
@@ -81,27 +80,27 @@
 features = ["test"]
 [tool.hatch.envs.test.scripts]
 test = "python -m pytest -vv {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.cov]
 features = ["test"]
-dependencies = ["coverage", "pytest-cov"]
+dependencies = ["coverage[toml]", "pytest-cov"]
 [tool.hatch.envs.cov.scripts]
-test = "python -m pytest -vv --cov jupyter_events --cov-branch --cov-report term-missing:skip-covered --cov-fail-under 80 {args}"
+test = "python -m pytest -vv --cov jupyter_events --cov-branch --cov-report term-missing:skip-covered {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.typing]
 features = ["test"]
 dependencies = ["mypy>=0.990"]
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:.}"
 
 [tool.hatch.envs.lint]
-dependencies = ["black[jupyter]==22.12.0", "mdformat>0.7", "ruff==0.0.194"]
+dependencies = ["black[jupyter]==23.3.0", "mdformat>0.7", "ruff==0.0.270"]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
 ]
@@ -129,14 +128,18 @@
   "raise NotImplementedError",
   "if 0:",
   "if __name__ == .__main__.:",
   "class .*\bProtocol\\):",
 "@(abc\\.)?abstractmethod",
 ]
 
+[tool.coverage.run]
+relative_files = true
+source = ["jupyter_events"]
+
 [tool.mypy]
 check_untyped_defs = true
 disallow_incomplete_defs = true
 no_implicit_optional = true
 pretty = true
 show_error_context = true
 show_error_codes = true
@@ -152,50 +155,27 @@
 skip-string-normalization = true
 target-version = ["py37"]
 
 [tool.ruff]
 target-version = "py37"
 line-length = 100
 select = [
-  "A", "B", "C", "E", "EM", "F", "FBT", "I", "N", "Q", "RUF", "S", "T",
-  "UP", "W", "YTT",
+  "A", "B", "C", "DTZ", "E", "EM", "F", "FBT", "I", "ICN", "ISC", "N",
+  "PLC", "PLE", "PLR", "PLW", "Q", "RUF", "S", "SIM", "T", "TID", "UP",
+  "W", "YTT",
 ]
 ignore = [
-  # Allow non-abstract empty methods in abstract base classes
-  "B027",
-  # Ignore McCabe complexity
-  "C901",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Use of `assert` detected
-  "S101",
-  # Line too long
-  "E501",
-  # Relative imports are banned
-  "TID252",
-  # Boolean ... in function definition
-  "FBT001", "FBT002",
-  # Module level import not at top of file
-  "E402",
-  # A001/A002/A003 .. is shadowing a python builtin
-  "A001", "A002", "A003",
-  # Possible hardcoded password
-  "S105", "S106",
   # Q000 Single quotes found but double quotes preferred
   "Q000",
-  # N806 Variable `B` in function should be lowercase
-  "N806",
-  # T201 `print` found
-  "T201",
-  # N802 Function name `CreateWellKnownSid` should be lowercase
-  "N802", "N803",
-  # C408 Unnecessary `dict` call (rewrite as a literal)
-  "C408",
-  # N801 Class name `directional_link` should use CapWords convention
-  "N801",
+  # FBT001 Boolean positional arg in function definition
+  "FBT001", "FBT002", "FBT003",
+  # E501 Line too long (158 > 100 characters)
+  "E501",
+  # SIM105 Use `contextlib.suppress(...)`
+  "SIM105",
 ]
 unfixable = [
   # Don't touch print statements
   "T201",
   # Don't touch noqa lines
   "RUF100",
 ]
@@ -205,15 +185,19 @@
 # F841 local variable 'foo' is assigned to but never used
 # C408 Unnecessary `dict` call
 # E402 Module level import not at top of file
 # T201 `print` found
 # B007 Loop control variable `i` not used within the loop body.
 # N802 Function name `assertIn` should be lowercase
 # F841 Local variable `t` is assigned to but never used
-"tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "F841"]
+# S101 Use of `assert` detected
+"tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "F841", "S101"]
+# C901 Function is too complex
+"jupyter_events/logger.py" = ["C901"] # `emit` is too complex (12 > 10)
+
 
 [tool.interrogate]
 ignore-init-module=true
 ignore-private=true
 ignore-semiprivate=true
 ignore-property-decorators=true
 ignore-nested-functions=true
```

### Comparing `jupyter_events-0.6.3/PKG-INFO` & `jupyter_events-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,79 @@
 Metadata-Version: 2.1
 Name: jupyter-events
-Version: 0.6.3
+Version: 0.7.0
 Summary: Jupyter Event System library
 Project-URL: Homepage, http://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
-License: # Licensing terms
+License: BSD 3-Clause License
         
-        This project is licensed under the terms of the Modified BSD License
-        (also known as New or Revised or 3-Clause BSD), as follows:
-        
-        - Copyright (c) 2022-, Jupyter Development Team
+        Copyright (c) 2022-, Jupyter Development Team
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
-        Redistributions of source code must retain the above copyright notice, this
-        list of conditions and the following disclaimer.
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
         
-        Redistributions in binary form must reproduce the above copyright notice, this
-        list of conditions and the following disclaimer in the documentation and/or
-        other materials provided with the distribution.
-        
-        Neither the name of the Jupyter Development Team nor the names of its
-        contributors may be used to endorse or promote products derived from this
-        software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-        ## About the Jupyter Development Team
-        
-        The Jupyter Development Team is the set of all contributors to the Jupyter project.
-        This includes all of the Jupyter subprojects.
-        
-        The core team that coordinates development on GitHub can be found here:
-        https://github.com/jupyter/.
-        
-        ## Our Copyright Policy
-        
-        Jupyter uses a shared copyright model. Each contributor maintains copyright
-        over their contributions to Jupyter. But, it is important to note that these
-        contributions are typically only changes to the repositories. Thus, the Jupyter
-        source code, in its entirety is not the copyright of any single person or
-        institution. Instead, it is the collective copyright of the entire Jupyter
-        Development Team. If individual contributors want to maintain a record of what
-        changes/contributions they have specific copyright on, they should indicate
-        their copyright in the commit message of the change, when they commit the
-        change to one of the Jupyter repositories.
-        
-        With this in mind, the following banner should be used in any source code file
-        to indicate the copyright and license terms:
-        
-        ```
-        # Copyright (c) Jupyter Development Team.
-        # Distributed under the terms of the Modified BSD License.
-        ```
-License-File: COPYING.md
+License-File: LICENSE
 Keywords: Jupyter,JupyterLab
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: jsonschema[format-nongpl]>=3.2.0
+Requires-Python: >=3.8
+Requires-Dist: jsonschema[format-nongpl]>=4.18.0
 Requires-Dist: python-json-logger>=2.0.4
 Requires-Dist: pyyaml>=5.3
+Requires-Dist: referencing
 Requires-Dist: rfc3339-validator
 Requires-Dist: rfc3986-validator>=0.1.1
 Requires-Dist: traitlets>=5.3
 Provides-Extra: cli
 Requires-Dist: click; extra == 'cli'
 Requires-Dist: rich; extra == 'cli'
 Provides-Extra: docs
 Requires-Dist: jupyterlite-sphinx; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: click; extra == 'test'
-Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-console-scripts; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: rich; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Jupyter Events
 
 [![Build Status](https://github.com/jupyter/jupyter_events/actions/workflows/python-tests.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter/jupyter_events/actions/workflows/python-tests.yml/badge.svg?query=branch%3Amain++)
-[![codecov](https://codecov.io/gh/jupyter/jupyter_events/branch/main/graph/badge.svg?token=S9WiBg2iL0)](https://codecov.io/gh/jupyter/jupyter_events)
 [![Documentation Status](https://readthedocs.org/projects/jupyter-events/badge/?version=latest)](http://jupyter-events.readthedocs.io/en/latest/?badge=latest)
 
 _An event system for Jupyter Applications and extensions._
 
 Jupyter Events enables Jupyter Python Applications (e.g. Jupyter Server, JupyterLab Server, JupyterHub, etc.) to emit **events**—structured data describing things happening inside the application. Other software (e.g. client applications like JupyterLab) can _listen_ and respond to these events.
 
 ## Install
@@ -122,7 +89,35 @@
 ```
 conda install -c conda-forge jupyter_events
 ```
 
 ## Documentation
 
 Documentation is available at [jupyter-events.readthedocs.io](https://jupyter-events.readthedocs.io).
+
+## About the Jupyter Development Team
+
+The Jupyter Development Team is the set of all contributors to the Jupyter project.
+This includes all of the Jupyter subprojects.
+
+The core team that coordinates development on GitHub can be found here:
+https://github.com/jupyter/.
+
+## Our Copyright Policy
+
+Jupyter uses a shared copyright model. Each contributor maintains copyright
+over their contributions to Jupyter. But, it is important to note that these
+contributions are typically only changes to the repositories. Thus, the Jupyter
+source code, in its entirety is not the copyright of any single person or
+institution. Instead, it is the collective copyright of the entire Jupyter
+Development Team. If individual contributors want to maintain a record of what
+changes/contributions they have specific copyright on, they should indicate
+their copyright in the commit message of the change, when they commit the
+change to one of the Jupyter repositories.
+
+With this in mind, the following banner should be used in any source code file
+to indicate the copyright and license terms:
+
+```
+# Copyright (c) Jupyter Development Team.
+# Distributed under the terms of the Modified BSD License.
+```
```

