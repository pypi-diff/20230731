# Comparing `tmp/pdm-2.8.1.tar.gz` & `tmp/pdm-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.8.1.tar", last modified: Wed Jul 26 05:34:15 2023, max compression
+gzip compressed data, was "pdm-2.8.2.tar", last modified: Mon Jul 31 06:41:35 2023, max compression
```

## Comparing `pdm-2.8.1.tar` & `pdm-2.8.2.tar`

### file list

```diff
@@ -1,281 +1,281 @@
--rw-r--r--   0        0        0   129793 2023-07-26 05:34:05.032076 pdm-2.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-07-26 05:34:05.032076 pdm-2.8.1/LICENSE
--rw-r--r--   0        0        0     1075 2023-07-26 05:34:05.032076 pdm-2.8.1/LICENSE
--rw-r--r--   0        0        0     7937 2023-07-26 05:34:05.032076 pdm-2.8.1/README.md
--rw-r--r--   0        0        0     7937 2023-07-26 05:34:05.032076 pdm-2.8.1/README.md
--rw-r--r--   0        0        0     4715 2023-07-26 05:34:15.188673 pdm-2.8.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/__version__.py
--rw-r--r--   0        0        0     3413 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11906 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1791 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    16569 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     7084 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2871 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6542 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1275 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     7537 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     3066 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     3679 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0    10561 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3982 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15754 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2645 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8112 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     4284 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15489 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2437 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9371 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     7276 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     6484 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1720 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2427 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6149 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2156 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      820 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2196 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1280 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2652 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5168 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    50740 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18666 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25535 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10529 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/options.py
--rw-r--r--   0        0        0     6539 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/__init__.py
--rw-r--r--   0        0        0     3102 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/.gitignore
--rw-r--r--   0        0        0       18 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/README.md
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/__init__.py
--rw-r--r--   0        0        0      278 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/src/example_package/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/tests/__init__.py
--rw-r--r--   0        0        0    26365 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2373 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/compat.py
--rw-r--r--   0        0        0    10620 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     9734 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/base.py
--rw-r--r--   0        0        0     4255 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1362 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2614 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7513 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1367 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/core.py
--rw-r--r--   0        0        0    11127 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2092 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18219 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    11150 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        6 2023-07-26 05:34:15.160672 pdm-2.8.1/src/pdm/models/VERSION
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4916 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/backends.py
--rw-r--r--   0        0        0    12115 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26687 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/environment.py
--rw-r--r--   0        0        0     2114 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6323 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2202 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    22707 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18772 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/search.py
--rw-r--r--   0        0        0     3292 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16725 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2858 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    17114 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/config.py
--rw-r--r--   0        0        0    26872 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/core.py
--rw-r--r--   0        0        0     2194 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/py.typed
--rw-r--r--   0        0        0    20073 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     2001 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13381 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1577 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/termui.py
--rw-r--r--   0        0        0    14109 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-07-26 05:34:05.044077 pdm-2.8.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12362 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_add.py
--rw-r--r--   0        0        0     5795 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4950 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_init.py
--rw-r--r--   0        0        0    11242 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_list.py
--rw-r--r--   0        0        0     6975 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3888 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29463 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     2778 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_template.py
--rw-r--r--   0        0        0     8876 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_update.py
--rw-r--r--   0        0        0     2997 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_use.py
--rw-r--r--   0        0        0    10808 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    94569 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-07-26 05:34:05.056078 pdm-2.8.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-07-26 05:34:05.056078 pdm-2.8.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       13 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    13807 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      572 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      726 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      344 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo/pyproject.toml
--rw-r--r--   0        0        0       26 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_backends.py
--rw-r--r--   0        0        0    13397 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_marker.py
--rw-r--r--   0        0        0     2936 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2556 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3590 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7704 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_plugin.py
--rw-r--r--   0        0        0    12085 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_signals.py
--rw-r--r--   0        0        0     4409 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_utils.py
--rw-r--r--   0        0        0    10122 1970-01-01 00:00:00.000000 pdm-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0   130128 2023-07-31 06:41:27.688008 pdm-2.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-07-31 06:41:27.688008 pdm-2.8.2/LICENSE
+-rw-r--r--   0        0        0     1075 2023-07-31 06:41:27.688008 pdm-2.8.2/LICENSE
+-rw-r--r--   0        0        0     7937 2023-07-31 06:41:27.688008 pdm-2.8.2/README.md
+-rw-r--r--   0        0        0     7937 2023-07-31 06:41:27.688008 pdm-2.8.2/README.md
+-rw-r--r--   0        0        0     4715 2023-07-31 06:41:35.744149 pdm-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3413 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11924 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1791 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    16569 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7084 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2871 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1275 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     7537 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3679 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0    10561 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3982 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15754 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2645 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8112 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6954 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4284 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15489 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2437 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9371 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     7276 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6484 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1720 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2427 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2156 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      820 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2196 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1280 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2652 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5168 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    50740 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18666 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25535 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10529 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/options.py
+-rw-r--r--   0        0        0     6539 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/templates/__init__.py
+-rw-r--r--   0        0        0     3102 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/templates/default/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/templates/default/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/templates/default/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/templates/default/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/templates/default/src/example_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.692008 pdm-2.8.2/src/pdm/cli/templates/default/tests/__init__.py
+-rw-r--r--   0        0        0    26365 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2373 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/compat.py
+-rw-r--r--   0        0        0    10620 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     9734 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     4255 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2614 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7513 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    11127 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2092 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18219 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    11150 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        6 2023-07-31 06:41:35.724148 pdm-2.8.2/src/pdm/models/VERSION
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4916 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    12115 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26687 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     2114 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6323 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2202 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    22741 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18772 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/search.py
+-rw-r--r--   0        0        0     3292 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16725 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2858 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    17114 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26872 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2194 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/py.typed
+-rw-r--r--   0        0        0    20073 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     2001 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13381 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1577 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/termui.py
+-rw-r--r--   0        0        0    14109 2023-07-31 06:41:27.696008 pdm-2.8.2/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12362 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5795 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4950 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11242 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6975 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3888 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29463 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     2778 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_template.py
+-rw-r--r--   0        0        0     8876 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10808 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-07-31 06:41:27.700008 pdm-2.8.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    94569 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-07-31 06:41:27.704008 pdm-2.8.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-07-31 06:41:27.708008 pdm-2.8.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-07-31 06:41:27.712008 pdm-2.8.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       13 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    13807 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      572 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      726 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      344 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13397 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2936 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2556 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3590 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7704 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/test_signals.py
+-rw-r--r--   0        0        0     4409 2023-07-31 06:41:27.716009 pdm-2.8.2/tests/test_utils.py
+-rw-r--r--   0        0        0    10122 1970-01-01 00:00:00.000000 pdm-2.8.2/PKG-INFO
```

### Comparing `pdm-2.8.1/CHANGELOG.md` & `pdm-2.8.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Release v2.8.2 (2023-07-31)
+---------------------------
+
+### Features & Improvements
+
+- Allow setting username and password in URL for publish command [#2140](https://github.com/pdm-project/pdm/issues/2140)
+
+### Bug Fixes
+
+- Use UTF-8 encoding when writing `sitecustomize.py`. [#2139](https://github.com/pdm-project/pdm/issues/2139)
+
+
 Release v2.8.1 (2023-07-26)
 ---------------------------
 
 ### Features & Improvements
 
 - Add `keyring`, `copier`, `cookiecutter`, `template`, `truststore` dependency groups. [#2109](https://github.com/pdm-project/pdm/issues/2109)
 - Ignore wheels for python versions not in range. [#2113](https://github.com/pdm-project/pdm/issues/2113)
```

### Comparing `pdm-2.8.1/LICENSE` & `pdm-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/README.md` & `pdm-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/pyproject.toml` & `pdm-2.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.8.1"
+version = "2.8.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.8.1/src/pdm/_types.py` & `pdm-2.8.2/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/builders/base.py` & `pdm-2.8.2/src/pdm/builders/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             self.bin_dirs.append(paths["scripts"])
             self.lib_dirs.extend([paths["platlib"], paths["purelib"]])
         self.site_dir = os.path.join(overlay, "site")
         if os.path.isdir(self.site_dir):
             # Clear existing site dir as .pyc may be cached.
             shutil.rmtree(self.site_dir)
         os.makedirs(self.site_dir)
-        with open(os.path.join(self.site_dir, "sitecustomize.py"), "w") as fp:
+        with open(os.path.join(self.site_dir, "sitecustomize.py"), "w", encoding="utf-8") as fp:
             fp.write(
                 textwrap.dedent(
                     f"""
                 import sys, os, site
 
                 original_sys_path = sys.path[:]
                 known_paths = set()
```

### Comparing `pdm-2.8.1/src/pdm/builders/editable.py` & `pdm-2.8.2/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/builders/sdist.py` & `pdm-2.8.2/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/builders/wheel.py` & `pdm-2.8.2/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/actions.py` & `pdm-2.8.2/src/pdm/cli/actions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/add.py` & `pdm-2.8.2/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/base.py` & `pdm-2.8.2/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/build.py` & `pdm-2.8.2/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/cache.py` & `pdm-2.8.2/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/completion.py` & `pdm-2.8.2/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/config.py` & `pdm-2.8.2/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/export.py` & `pdm-2.8.2/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.8.2/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.8.2/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/import_cmd.py` & `pdm-2.8.2/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/info.py` & `pdm-2.8.2/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/init.py` & `pdm-2.8.2/src/pdm/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/install.py` & `pdm-2.8.2/src/pdm/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/list.py` & `pdm-2.8.2/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/lock.py` & `pdm-2.8.2/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.8.2/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/publish/package.py` & `pdm-2.8.2/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/publish/repository.py` & `pdm-2.8.2/src/pdm/cli/commands/publish/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,19 +39,22 @@
         username, password = self._ensure_credentials(username, password)
         self.session.auth = (username, password)
         weakref.finalize(self, self.session.close)
 
     def _ensure_credentials(self, username: str | None, password: str | None) -> tuple[str, str]:
         from pdm.models.auth import keyring
 
-        netloc = urlparse(self.url).netloc
+        parsed_url = urlparse(self.url)
+        netloc = parsed_url.netloc
         if username and password:
             return username, password
         if password:
             return "__token__", password
+        if parsed_url.username is not None and parsed_url.password is not None:
+            return parsed_url.username, parsed_url.password
         if keyring.enabled:
             auth = keyring.get_auth_info(self.url, username)
             if auth is not None:
                 return auth
         token = self._get_pypi_token_via_oidc()
         if token is not None:
             return "__token__", token
```

### Comparing `pdm-2.8.1/src/pdm/cli/commands/remove.py` & `pdm-2.8.2/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/run.py` & `pdm-2.8.2/src/pdm/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/search.py` & `pdm-2.8.2/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/self_cmd.py` & `pdm-2.8.2/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/show.py` & `pdm-2.8.2/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/sync.py` & `pdm-2.8.2/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/update.py` & `pdm-2.8.2/src/pdm/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/use.py` & `pdm-2.8.2/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/activate.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/backends.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/create.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/list.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/purge.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/remove.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/commands/venv/utils.py` & `pdm-2.8.2/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/completions/pdm.bash` & `pdm-2.8.2/src/pdm/cli/completions/pdm.bash`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/completions/pdm.fish` & `pdm-2.8.2/src/pdm/cli/completions/pdm.fish`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/completions/pdm.ps1` & `pdm-2.8.2/src/pdm/cli/completions/pdm.ps1`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/completions/pdm.zsh` & `pdm-2.8.2/src/pdm/cli/completions/pdm.zsh`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/filters.py` & `pdm-2.8.2/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/hooks.py` & `pdm-2.8.2/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/options.py` & `pdm-2.8.2/src/pdm/cli/options.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/templates/__init__.py` & `pdm-2.8.2/src/pdm/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/templates/default/.gitignore` & `pdm-2.8.2/src/pdm/cli/templates/default/.gitignore`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/cli/utils.py` & `pdm-2.8.2/src/pdm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/compat.py` & `pdm-2.8.2/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/core.py` & `pdm-2.8.2/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/environments/__init__.py` & `pdm-2.8.2/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/environments/base.py` & `pdm-2.8.2/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/environments/local.py` & `pdm-2.8.2/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/environments/python.py` & `pdm-2.8.2/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/exceptions.py` & `pdm-2.8.2/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/formats/__init__.py` & `pdm-2.8.2/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/formats/base.py` & `pdm-2.8.2/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/formats/flit.py` & `pdm-2.8.2/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/formats/pipfile.py` & `pdm-2.8.2/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/formats/poetry.py` & `pdm-2.8.2/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/formats/requirements.py` & `pdm-2.8.2/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/formats/setup_py.py` & `pdm-2.8.2/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/installers/core.py` & `pdm-2.8.2/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/installers/installers.py` & `pdm-2.8.2/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/installers/manager.py` & `pdm-2.8.2/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/installers/packages.py` & `pdm-2.8.2/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/installers/synchronizers.py` & `pdm-2.8.2/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/installers/uninstallers.py` & `pdm-2.8.2/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/auth.py` & `pdm-2.8.2/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/backends.py` & `pdm-2.8.2/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/caches.py` & `pdm-2.8.2/src/pdm/models/caches.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/candidates.py` & `pdm-2.8.2/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/in_process/__init__.py` & `pdm-2.8.2/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.8.2/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/in_process/parse_setup.py` & `pdm-2.8.2/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/in_process/pep508.py` & `pdm-2.8.2/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.8.2/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/markers.py` & `pdm-2.8.2/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/project_info.py` & `pdm-2.8.2/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/python.py` & `pdm-2.8.2/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/repositories.py` & `pdm-2.8.2/src/pdm/models/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,11 +529,12 @@
             if not PySpecSet(info[1]).contains(str(self.environment.interpreter.version), True):
                 continue
             can = self.packages[key]
             can.requires_python = info[1]
             if not requirement.name:
                 # make sure can.identify() won't return a randomly-generated name
                 requirement.name = can.name
+            can.req = requirement
             yield can
 
     def get_hashes(self, candidate: Candidate) -> list[FileHash]:
         return candidate.hashes
```

### Comparing `pdm-2.8.1/src/pdm/models/requirements.py` & `pdm-2.8.2/src/pdm/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/search.py` & `pdm-2.8.2/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/session.py` & `pdm-2.8.2/src/pdm/models/session.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/setup.py` & `pdm-2.8.2/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/specifiers.py` & `pdm-2.8.2/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/venv.py` & `pdm-2.8.2/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/versions.py` & `pdm-2.8.2/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/models/working_set.py` & `pdm-2.8.2/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/pep582/sitecustomize.py` & `pdm-2.8.2/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/project/config.py` & `pdm-2.8.2/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/project/core.py` & `pdm-2.8.2/src/pdm/project/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/project/lockfile.py` & `pdm-2.8.2/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/project/project_file.py` & `pdm-2.8.2/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/project/toml_file.py` & `pdm-2.8.2/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/pytest.py` & `pdm-2.8.2/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/resolver/core.py` & `pdm-2.8.2/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/resolver/providers.py` & `pdm-2.8.2/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/resolver/python.py` & `pdm-2.8.2/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/resolver/reporters.py` & `pdm-2.8.2/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/signals.py` & `pdm-2.8.2/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/termui.py` & `pdm-2.8.2/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/src/pdm/utils.py` & `pdm-2.8.2/src/pdm/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/conftest.py` & `pdm-2.8.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_add.py` & `pdm-2.8.2/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_build.py` & `pdm-2.8.2/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_cache.py` & `pdm-2.8.2/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_config.py` & `pdm-2.8.2/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_fix.py` & `pdm-2.8.2/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_hooks.py` & `pdm-2.8.2/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_init.py` & `pdm-2.8.2/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_install.py` & `pdm-2.8.2/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_list.py` & `pdm-2.8.2/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_lock.py` & `pdm-2.8.2/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_others.py` & `pdm-2.8.2/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_publish.py` & `pdm-2.8.2/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_remove.py` & `pdm-2.8.2/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_run.py` & `pdm-2.8.2/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_self_command.py` & `pdm-2.8.2/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_template.py` & `pdm-2.8.2/tests/cli/test_template.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_update.py` & `pdm-2.8.2/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_use.py` & `pdm-2.8.2/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/cli/test_venv.py` & `pdm-2.8.2/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/conftest.py` & `pdm-2.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.8.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.8.2/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.8.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.8.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.8.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.8.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.8.2/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.8.2/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.8.2/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     --hash=sha256:0fbeb6180d383a9186d0d6ed954e0042ad9f18e0e8de088b2b419d526927d196 \
     --hash=sha256:c34f04500f2cbbea882b1acb02002ad6fe6b7ffa64a6164577995657f50aed22
 itsdangerous==1.1.0 \
     --hash=sha256:321b033d07f2a4136d3ec762eac9f16a10ccd60f53c0c91af90217ace7ba1f19 \
     --hash=sha256:72a1252c0b2cc2bcc351acf2cfe2ec0159d8578c54767d5c2aa67fd869346e55 \
     --hash=sha256:ac4c9f590d59c36b7d2953f97fda415f2461280e5279650aafe1e593f129c4f7 \
     --hash=sha256:b12271b2047cb23eeb98c8b5622e2e5c5e9abd9784a153e9d8ef9cb4dd09d749
-jinja2==2.11.3 \
+Jinja2==2.11.3 \
     --hash=sha256:03e47ad063331dd6a3f04a43eddca8a966a26ba0c5b7207a9a9e4e08f1b29419 \
     --hash=sha256:a6d58433de0ae800347cab1fa3043cebbabe8baa9d29e668f1c768cb87a333c6
-markupsafe==1.1.1 \
+MarkupSafe==1.1.1 \
     --hash=sha256:00bc623926325b26bb9605ae9eae8a215691f33cae5df11ca5424f06f2d1f473 \
     --hash=sha256:09027a7803a62ca78792ad89403b1b7a73a01c8cb65909cd876f7fcebd79b161 \
     --hash=sha256:09c4b7f37d6c648cb13f9230d847adf22f8171b1ccc4d5682398e77f40309235 \
     --hash=sha256:0db2ff381c2218c1ba7192f75e5c5cf180efa023ddfc6914ffe9a38b2bd303dd \
     --hash=sha256:1027c282dad077d0bae18be6794e6b6b8c91d58ed8a8d89a89d59693b9131db5 \
     --hash=sha256:13d3144e1e340870b25e7b10b98d779608c02016d5184cfb9927a9f10c689f42 \
     --hash=sha256:195d7d2c4fbb0ee8139a6cf67194f3973a6b3042d742ebe0a9ed36d8b6f0c07f \
@@ -86,11 +86,11 @@
     --hash=sha256:d73a845f227b0bfe8a7455ee623525ee656a9e2e749e4742706d80a6065d5e2c \
     --hash=sha256:d9be0ba6c527163cbed5e0857c451fcd092ce83947944d6c14bc95441203f032 \
     --hash=sha256:dbc6ee2241abe4f518685f603e427a94ceb73c08b6d15d85c6c5c4a71bde9c3e \
     --hash=sha256:de603df0d005177f7ef7faa56578d2d47fc93aaef165cdef91d64959176edb15 \
     --hash=sha256:e249096428b3ae81b08327a63a485ad0878de3fb939049038579ac0ef61e17e7 \
     --hash=sha256:e8313f01ba26fbbe36c7be1966a7b7424942f670f38e666995b88d012765b9be \
     --hash=sha256:feb7b34d6325451ef96bc0e36e1a6c0c1c64bc1fbec4b854f4529e51887b1621
-werkzeug==1.0.1 \
+Werkzeug==1.0.1 \
     --hash=sha256:2de2a5db0baeae7b2d2664949077c2ac63fbd16d98da0ff71837f7d1dea3fd43 \
     --hash=sha256:6c80b1e5ad3665290ea39320b91e1be1e0d5f60652b964a3070216de83d2e47c
 --extra-index-url https://test.pypi.org/simple
```

### Comparing `pdm-2.8.1/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.8.2/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.8.2/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.8.2/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/pypi.json` & `pdm-2.8.2/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/fixtures/pyproject.toml` & `pdm-2.8.2/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/models/test_backends.py` & `pdm-2.8.2/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/models/test_candidates.py` & `pdm-2.8.2/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/models/test_marker.py` & `pdm-2.8.2/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/models/test_requirements.py` & `pdm-2.8.2/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/models/test_setup_parsing.py` & `pdm-2.8.2/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/models/test_specifiers.py` & `pdm-2.8.2/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/models/test_versions.py` & `pdm-2.8.2/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/resolver/test_resolve.py` & `pdm-2.8.2/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/test_formats.py` & `pdm-2.8.2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/test_installer.py` & `pdm-2.8.2/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/test_integration.py` & `pdm-2.8.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/test_plugin.py` & `pdm-2.8.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/test_project.py` & `pdm-2.8.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/test_signals.py` & `pdm-2.8.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/tests/test_utils.py` & `pdm-2.8.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.1/PKG-INFO` & `pdm-2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.8.1
+Version: 2.8.2
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.8.1 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.8.2 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

