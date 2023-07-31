# Comparing `tmp/astro_provider_databricks-0.1.4.tar.gz` & `tmp/astro_provider_databricks-0.1.5.tar.gz`

## Comparing `astro_provider_databricks-0.1.4.tar` & `astro_provider_databricks-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.deepsource.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/CHANGELOG.rst
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/Tiltfile
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/codecov.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/mlc-config.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/noxfile.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/yamllint-config.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/ci-test-connections.yaml
--rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/scripts/verify_tag_and_version.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/astro-deploy.yml
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/mlc_config.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/.dockerignore
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/Dockerfile
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/docker-compose.yaml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/packages.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/requirements.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/.astro/config.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/Makefile
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/conf.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/contributing.rst
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/make.bat
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/requirements.txt
--rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/banner.png
--rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/dbt_dag.png
--rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/dbt_task_group.png
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/logo-dark.png
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/logo-light.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/css/custom.css
--rw-r--r--   0        0        0   212922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/screenshots/workflow_1_airflow.png
--rw-r--r--   0        0        0   763410 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/screenshots/workflow_1_databricks.png
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/assets/images/dbutils-notebook-success.png
--rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/assets/images/repair-all-failed.png
--rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/assets/images/repair-single-failed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/.airflowignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/__init__.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/example_databricks_notebook.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/example_databricks_workflow.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/example_task_group.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/quickstart/astro-cli.md
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/quickstart/without-astro-cli.md
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/operators/__init__.py
--rw-r--r--   0        0        0    14553 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/operators/notebook.py
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/operators/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/plugins/__init__.py
--rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/plugins/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/pytest.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/test_example_dags.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/__init__.py
--rw-r--r--   0        0        0    14882 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/test_notebook.py
--rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/test_plugin.py
--rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/test_workflow.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/LICENSE
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.deepsource.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/CHANGELOG.rst
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/Tiltfile
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/codecov.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/mlc-config.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/noxfile.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/yamllint-config.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.github/ci-test-connections.yaml
+-rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.github/scripts/verify_tag_and_version.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.github/workflows/mlc_config.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/dev/.dockerignore
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/dev/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/dev/Dockerfile
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/dev/docker-compose.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/dev/packages.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/dev/requirements.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/dev/.astro/config.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/Makefile
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/conf.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/contributing.rst
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/make.bat
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/requirements.txt
+-rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/banner.png
+-rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/dbt_dag.png
+-rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/dbt_task_group.png
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/logo-light.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/css/custom.css
+-rw-r--r--   0        0        0   212922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/screenshots/workflow_1_airflow.png
+-rw-r--r--   0        0        0   763410 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/_static/screenshots/workflow_1_databricks.png
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/assets/images/dbutils-notebook-success.png
+-rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/assets/images/repair-all-failed.png
+-rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/docs/assets/images/repair-single-failed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/example_dags/.airflowignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/example_dags/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/example_dags/example_databricks_notebook.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/example_dags/example_databricks_workflow.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/example_dags/example_task_group.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/quickstart/astro-cli.md
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/quickstart/without-astro-cli.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/operators/__init__.py
+-rw-r--r--   0        0        0    13312 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/operators/common.py
+-rw-r--r--   0        0        0    14757 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/operators/notebook.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/operators/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/plugins/__init__.py
+-rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/astro_databricks/plugins/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/pytest.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/test_example_dags.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/databricks/__init__.py
+-rw-r--r--   0        0        0    14764 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/databricks/test_common.py
+-rw-r--r--   0        0        0    14882 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/databricks/test_notebook.py
+-rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/databricks/test_plugin.py
+-rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/tests/databricks/test_workflow.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/README.md
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.5/PKG-INFO
```

### Comparing `astro_provider_databricks-0.1.4/.pre-commit-config.yaml` & `astro_provider_databricks-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/CHANGELOG.rst` & `astro_provider_databricks-0.1.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/CODE_OF_CONDUCT.md` & `astro_provider_databricks-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/Tiltfile` & `astro_provider_databricks-0.1.5/Tiltfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/noxfile.py` & `astro_provider_databricks-0.1.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/.github/scripts/verify_tag_and_version.py` & `astro_provider_databricks-0.1.5/.github/scripts/verify_tag_and_version.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/.github/workflows/ci.yml` & `astro_provider_databricks-0.1.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/.github/workflows/docs.yml` & `astro_provider_databricks-0.1.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/dev/Dockerfile` & `astro_provider_databricks-0.1.5/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/dev/docker-compose.yaml` & `astro_provider_databricks-0.1.5/dev/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/Makefile` & `astro_provider_databricks-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/conf.py` & `astro_provider_databricks-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/contributing.rst` & `astro_provider_databricks-0.1.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/index.rst` & `astro_provider_databricks-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/make.bat` & `astro_provider_databricks-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/_static/banner.png` & `astro_provider_databricks-0.1.5/docs/_static/banner.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/_static/dbt_dag.png` & `astro_provider_databricks-0.1.5/docs/_static/dbt_dag.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/_static/dbt_task_group.png` & `astro_provider_databricks-0.1.5/docs/_static/dbt_task_group.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/_static/logo-dark.png` & `astro_provider_databricks-0.1.5/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/_static/logo-light.png` & `astro_provider_databricks-0.1.5/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/_static/screenshots/workflow_1_airflow.png` & `astro_provider_databricks-0.1.5/docs/_static/screenshots/workflow_1_airflow.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/_static/screenshots/workflow_1_databricks.png` & `astro_provider_databricks-0.1.5/docs/_static/screenshots/workflow_1_databricks.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/assets/images/dbutils-notebook-success.png` & `astro_provider_databricks-0.1.5/docs/assets/images/dbutils-notebook-success.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/assets/images/repair-all-failed.png` & `astro_provider_databricks-0.1.5/docs/assets/images/repair-all-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/docs/assets/images/repair-single-failed.png` & `astro_provider_databricks-0.1.5/docs/assets/images/repair-single-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/example_dags/example_databricks_notebook.py` & `astro_provider_databricks-0.1.5/example_dags/example_databricks_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/example_dags/example_databricks_workflow.py` & `astro_provider_databricks-0.1.5/example_dags/example_databricks_workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/example_dags/example_task_group.py` & `astro_provider_databricks-0.1.5/example_dags/example_task_group.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/quickstart/astro-cli.md` & `astro_provider_databricks-0.1.5/quickstart/astro-cli.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/quickstart/without-astro-cli.md` & `astro_provider_databricks-0.1.5/quickstart/without-astro-cli.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/astro_databricks/operators/notebook.py` & `astro_provider_databricks-0.1.5/astro_databricks/operators/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,19 @@
         notebook_params: dict | None = None,
         notebook_packages: list[dict[str, Any]] = None,
         job_cluster_key: str | None = None,
         new_cluster: dict | None = None,
         existing_cluster_id: str | None = None,
         **kwargs,
     ):
+        if new_cluster and existing_cluster_id:
+            raise ValueError(
+                "Both new_cluster and existing_cluster_id are set. Only one can be set."
+            )
+
         self.notebook_path = notebook_path
         self.source = source
         self.notebook_params = notebook_params or {}
         self.notebook_packages = notebook_packages or []
         self.databricks_conn_id = databricks_conn_id
         self.databricks_run_id = ""
         self.databricks_metadata: dict | None = None
@@ -172,15 +177,17 @@
         Convert the operator to a Databricks workflow task that can be a task in a workflow
         """
         if airflow.__version__ in ("2.2.4", "2.2.5"):
             databricks_task_group = self.find_parent_databricks_workflow_task_group()
         else:
             databricks_task_group = self.databricks_task_group
 
-        if databricks_task_group and hasattr(databricks_task_group, "notebook_packages"):
+        if databricks_task_group and hasattr(
+            databricks_task_group, "notebook_packages"
+        ):
             self.merge_notebook_packages(databricks_task_group)
 
         if databricks_task_group and hasattr(databricks_task_group, "notebook_params"):
             self.notebook_params = {
                 **self.notebook_params,
                 **databricks_task_group.notebook_params,
             }
```

### Comparing `astro_provider_databricks-0.1.4/astro_databricks/operators/workflow.py` & `astro_provider_databricks-0.1.5/astro_databricks/operators/workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/astro_databricks/plugins/plugin.py` & `astro_provider_databricks-0.1.5/astro_databricks/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/tests/conftest.py` & `astro_provider_databricks-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/tests/test_example_dags.py` & `astro_provider_databricks-0.1.5/tests/test_example_dags.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/tests/utils.py` & `astro_provider_databricks-0.1.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/tests/databricks/test_notebook.py` & `astro_provider_databricks-0.1.5/tests/databricks/test_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/tests/databricks/test_plugin.py` & `astro_provider_databricks-0.1.5/tests/databricks/test_plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/tests/databricks/test_workflow.py` & `astro_provider_databricks-0.1.5/tests/databricks/test_workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/.gitignore` & `astro_provider_databricks-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/LICENSE` & `astro_provider_databricks-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/README.md` & `astro_provider_databricks-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.4/pyproject.toml` & `astro_provider_databricks-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "apache-airflow>=2.2.4",
     "databricks-sql-connector>=2.0.4;python_version>='3.10'",
     "databricks-cli>=0.17.7",
     "apache-airflow-providers-databricks>=2.2.0",
-    "mergedeep"
+    "mergedeep",
+    "pydantic>=1.10.0,<2.0.0", # Airflow & Pydantic issue: https://github.com/apache/airflow/issues/32311
 ]
 
 [project.optional-dependencies]
 docs =[
     "pydata_sphinx_theme",
     "sphinx",
     "sphinx-autobuild",
```

### Comparing `astro_provider_databricks-0.1.4/PKG-INFO` & `astro_provider_databricks-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-provider-databricks
-Version: 0.1.4
+Version: 0.1.5
 Summary: Affordable Databricks Workflows in Apache Airflow
 Project-URL: Homepage, https://github.com/astronomer/astro-provider-databricks/
 Project-URL: Documentation, https://github.com/astronomer/astro-provider-databricks/
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Requires-Dist: apache-airflow-providers-databricks>=2.2.0
 Requires-Dist: apache-airflow>=2.2.4
 Requires-Dist: databricks-cli>=0.17.7
 Requires-Dist: databricks-sql-connector>=2.0.4; python_version >= '3.10'
 Requires-Dist: mergedeep
+Requires-Dist: pydantic<2.0.0,>=1.10.0
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-tabs; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: mypy; extra == 'tests'
```

