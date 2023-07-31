# Comparing `tmp/git_co_evg_base-3.0.6.tar.gz` & `tmp/git_co_evg_base-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_co_evg_base-3.0.6.tar", max compression
+gzip compressed data, was "git_co_evg_base-4.0.0.tar", max compression
```

## Comparing `git_co_evg_base-3.0.6.tar` & `git_co_evg_base-4.0.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     9753 2022-11-08 13:14:37.656843 git_co_evg_base-3.0.6/README.md
--rw-r--r--   0        0        0     1730 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/__init__.py
--rw-r--r--   0        0        0     3814 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/build_checker.py
--rw-r--r--   0        0        0        0 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/clients/__init__.py
--rw-r--r--   0        0        0      998 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/clients/evg_cli_proxy.py
--rw-r--r--   0        0        0    20224 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/goodbase_cli.py
--rw-r--r--   0        0        0     2148 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/goodbase_options.py
--rw-r--r--   0        0        0        0 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/models/__init__.py
--rw-r--r--   0        0        0     1060 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/models/build_status.py
--rw-r--r--   0        0        0        0 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/services/__init__.py
--rw-r--r--   0        0        0     3919 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/services/config_service.py
--rw-r--r--   0        0        0     3350 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/services/criteria_service.py
--rw-r--r--   0        0        0     6276 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/services/evg_service.py
--rw-r--r--   0        0        0     1029 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/services/file_service.py
--rw-r--r--   0        0        0     3558 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/services/git_service.py
--rw-r--r--   0        0        0     2886 2022-11-08 13:14:37.688843 git_co_evg_base-3.0.6/src/goodbase/services/search_service.py
--rw-r--r--   0        0        0    11132 1970-01-01 00:00:00.000000 git_co_evg_base-3.0.6/setup.py
--rw-r--r--   0        0        0    10734 1970-01-01 00:00:00.000000 git_co_evg_base-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0    10256 2023-07-31 10:10:10.932276 git_co_evg_base-4.0.0/README.md
+-rw-r--r--   0        0        0     1769 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/__init__.py
+-rw-r--r--   0        0        0     4161 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/build_checker.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/clients/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/clients/evg_cli_proxy.py
+-rw-r--r--   0        0        0    20859 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/goodbase_cli.py
+-rw-r--r--   0        0        0     2148 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/goodbase_options.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/models/__init__.py
+-rw-r--r--   0        0        0     1060 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/models/build_status.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/services/__init__.py
+-rw-r--r--   0        0        0     4112 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/services/config_service.py
+-rw-r--r--   0        0        0     3350 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/services/criteria_service.py
+-rw-r--r--   0        0        0     6315 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/services/evg_service.py
+-rw-r--r--   0        0        0     1029 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/services/file_service.py
+-rw-r--r--   0        0        0     3558 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/services/git_service.py
+-rw-r--r--   0        0        0     2886 2023-07-31 10:10:10.984288 git_co_evg_base-4.0.0/src/goodbase/services/search_service.py
+-rw-r--r--   0        0        0    11237 1970-01-01 00:00:00.000000 git_co_evg_base-4.0.0/PKG-INFO
```

### Comparing `git_co_evg_base-3.0.6/README.md` & `git_co_evg_base-4.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -125,68 +125,72 @@
 
   If you have any evergreen modules with local checkouts in the location specified in your
   project's evergreen.yml configuration file. They will automatically be checked out to the
   revision that was run in Evergreen with the revision of the base project.
 
   Examples
 
-  Working on a fix for a task 'replica_sets' on the build variants 'enterprise-rhel-80-64-bit' and
-  'enterprise-windows', to ensure the task has been run on those build variants:
+  Working on a fix for a task 'replica_sets_jscore_passthrough' on the build variants '! Amazon
+  Linux 2 arm64 (all feature flags)' and '! Enterprise Windows (all feature flags)', to ensure the
+  task has been run on those build variants:
 
-      git co-evg-base --run-task replica_sets --build-variant enterprise-rhel-80-64-bit --build-variant enterprise-windows
+      git co-evg-base --run-task replica_sets_jscore_passthrough --display-variant-name "^! Amazon Linux 2 arm64 (all feature flags)$" --display-variant-name "^! Enterprise Windows (all feature flags)$"
 
   Starting a new change, to ensure that there are no systemic failures on the base commit:
 
       git co-evg-base --pass-threshold 0.98
 
 Options:
   --passing-task TEXT             Specify a task that needs to be passing (can be specified
                                   multiple times).
   --run-task TEXT                 Specify a task that needs to be run (can be specified multiple
                                   times).
   --run-threshold FLOAT           Specify the percentage of tasks that need to be run.
   --pass-threshold FLOAT          Specify the percentage of tasks that need to be successful.
   --fail-threshold FLOAT          Specify the percentage of tasks that need to be failed.
-  --evg-config-file PATH          File containing evergreen authentication information
-                                  [default=~/.evergreen.yml].
-  --evg-project TEXT              Evergreen project to query against [default=mongodb-mongo-
-                                  master].
+  --evg-config-file PATH          File containing evergreen authentication information.  [default:
+                                  /Users/<username>/.evergreen.yml]
+  --evg-project TEXT              Evergreen project to query against.  [default: mongodb-mongo-
+                                  master]
   --build-variant TEXT            Regex of Build variants to check (can be specified multiple
-                                  times) [default=.*-required$].
-  --commit-lookback INTEGER       Number of commits to check before giving up [default=50].
+                                  times).
+  --display-variant-name TEXT     Regex of Build variant display names to check (can be specified
+                                  multiple times).  [default: .*]
+  --commit-lookback INTEGER       Number of commits to check before giving up.  [default: 50]
   --timeout-secs INTEGER          Number of seconds to search for before giving up.
   --commit-limit TEXT             Oldest commit to check before giving up.
   --git-operation [checkout|rebase|merge|none]
-                                  Git operations to perform with found commit [default=none].
-  -b, --branch TEXT               Name of branch to create on checkout.
+                                  Git operations to perform with found commit.  [default: none]
+  -b, --branch TEXT               Name of branch to create on checkout. When specified, git-
+                                  operation is set to checkout by default.
   --save-criteria TEXT            Save the specified criteria rules under the specified name for
                                   future use.
   --use-criteria TEXT             Use previously save criteria rules.
   --list-criteria                 Display saved criteria.
   --override                      Override saved conflicting save criteria rules.
   --export-criteria TEXT          Specify saved criteria to export to a file.
   --export-file PATH              File to write exported rules to.
   --import-criteria PATH          Import previously exported criteria.
   --output-format [plaintext|yaml|json]
-                                  Format of the command output [default=plaintext].
+                                  Format of the command output.  [default: plaintext]
   --verbose                       Enable debug logging.
   --help                          Show this message and exit.
 ```
 
 Checkout using the default criteria:
 
 ```bash
 $ git co-evg-base
 ```
 
-Checkout with successful tasks 'auth' and 'auth_audit' on builds 'enterprise-windows' and
-'enterprise-rhel-80-64-bit' and 95% of the tasks are passing.
+Checkout with successful tasks 'auth' and 'auth_audit' on builds '! Enterprise Windows (all feature flags)'
+and '! Amazon Linux 2 arm64 (all feature flags)' and 95% of the tasks are passing.
 
 ```bash
-$ git co-evg-base --passing-task auth --passing-task auth_audit --run-threshold 0.95 --build-variant enterprise-windows --build-variant enterprise-rhel-80-64-bit
+$ git co-evg-base --passing-task auth --passing-task auth_audit --run-threshold 0.95 --display-variant-name "^! Enterprise Windows (all feature flags)$" --display-variant-name "^! Amazon Linux 2 arm64 (all feature flags)$"
 ```
 
 ## Contributor's Guide
 
 ### Setting up a local development environment
 
 This project uses [poetry](https://python-poetry.org/) for setting up a local environment.
```

### Comparing `git_co_evg_base-3.0.6/pyproject.toml` & `git_co_evg_base-4.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-co-evg-base"
-version = "3.0.6"
+version = "4.0.0"
 description = "Find a good commit to base your work on"
 authors = ["David Bradford <david.bradford@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/evergreen-ci/git-co-evg-base"
 packages = [
     { include = "goodbase", from = "src"},
 ]
@@ -20,28 +20,30 @@
 Inject = "^4.3.1"
 structlog = "^21.1.0"
 PyYAML = "^5.4.1"
 xdg = "^5.1.1"
 pydantic = "^1.8.2"
 rich = "^10.9.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.0"
 black = "^22.3.0"
 pytest-black = "^0.3"
 pytest-cov = "^2.8"
 pytest-flake8 = "^1.0"
-pytest-mypy = "^0.8"
+pytest-mypy = "^0.10"
 mypy = "^0.910"
-pytest-pydocstyle = "^2.0"
+pytest-pydocstyle = "^2.3"
 pre-commit = "^2.6"
 pytest-isort = "^2.0"
 flake8-bugbear = "^21.4"
 types-PyYAML = "^5.4.10"
 types-requests = "^2.27.7"
+flake8 = "3.9.2"
+py = "^1.11.0"
 
 [tool.black]
 line-length = 100
 target-version = ['py39']
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `git_co_evg_base-3.0.6/src/goodbase/build_checker.py` & `git_co_evg_base-4.0.0/src/goodbase/build_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,45 +11,50 @@
 
 
 class BuildChecks(BaseModel):
     """
     Set of checks to perform to check build criteria.
 
     build_variant_regex: List of build variant regexes to which checks should apply.
+    display_name_regex: List of build variant display name regexes to which checks should apply.
     success_threshold: Percentage of tasks that need to pass to use the build.
     failure_threshold: Percentage of tasks that need to fail to use the build.
     run_threshold: Percentage of tasks that need to have run to use the build.
     successful_tasks: Set of tasks that need to have passed to use the build.
     active_tasks: Set of tasks that need to have run to use the build.
     """
 
     build_variant_regex: List[str]
+    display_name_regex: List[str]
     success_threshold: Optional[float] = None
     failure_threshold: Optional[float] = None
     run_threshold: Optional[float] = None
     successful_tasks: Optional[Set[str]] = None
     active_tasks: Optional[Set[str]] = None
 
-    def should_apply(self, build_variant: str) -> bool:
+    def should_apply(self, build_variant: str, display_name: str) -> bool:
         """
         Check if the given build variant should apply to these checks.
 
         :param build_variant: Name of build variant to check.
+        :param display_name: Display name of build variant to check.
         :return: True if these checks apply to the given build variant.
         """
-        return any(re.match(bv_regex, build_variant) for bv_regex in self.build_variant_regex)
+        return any(
+            re.match(bv_regex, build_variant) for bv_regex in self.build_variant_regex
+        ) or any(re.match(dn_regex, display_name) for dn_regex in self.display_name_regex)
 
     def check(self, build_status: BuildStatus) -> bool:
         """
         Check if the given build stats meet the specified criteria.
 
         :param build_status: Status of build to check.
         :return: True if the build matches the criteria.
         """
-        if not self.should_apply(build_status.build_variant):
+        if not self.should_apply(build_status.build_variant, build_status.build_name):
             return True
 
         if self.success_threshold and build_status.success_pct() < self.success_threshold:
             LOGGER.debug(
                 "Unmet criteria, success_threshold",
                 build=build_status.build_name,
                 expected_success=self.success_threshold,
```

### Comparing `git_co_evg_base-3.0.6/src/goodbase/clients/evg_cli_proxy.py` & `git_co_evg_base-4.0.0/src/goodbase/clients/evg_cli_proxy.py`

 * *Files identical despite different names*

### Comparing `git_co_evg_base-3.0.6/src/goodbase/goodbase_cli.py` & `git_co_evg_base-4.0.0/src/goodbase/goodbase_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from typing import Dict, List, NamedTuple, Optional
 
 import click
 import inject
 import structlog
 import yaml
+from click.core import ParameterSource
 from evergreen import EvergreenApi, RetryingEvergreenApi
 from plumbum import ProcessExecutionError
 from rich.console import Console
 from rich.table import Table
 from structlog.stdlib import LoggerFactory
 
 from goodbase.build_checker import BuildChecks
@@ -33,15 +34,15 @@
 MAX_LOOKBACK = 50
 DEFAULT_THRESHOLD = 0.95
 EXTERNAL_LOGGERS = [
     "evergreen",
     "inject",
     "urllib3",
 ]
-PROJECT_REGEX_TO_DEFAULT_BUILD_VARIANTS = {"mongodb-mongo-.*": [".*-required$"]}
+PROJECT_REGEX_TO_DEFAULT_DISPLAY_VARIANT_NAME_REGEXES = {"mongodb-mongo-.*": ["^! .*"]}
 
 
 class RevisionInformation(NamedTuple):
     """
     Details about what revision(s) were found.
 
     revision: Revision of base project.
@@ -194,22 +195,24 @@
         self.criteria_service.import_criteria(import_file)
 
     def display_criteria(self) -> None:
         """Display saved criteria."""
         for group in self.criteria_service.get_all_criteria():
             table = Table(title=group.name, show_lines=True)
             table.add_column("Build Variant Regexes")
+            table.add_column("Display Name Regexes")
             table.add_column("Success %")
             table.add_column("Run %")
             table.add_column("Successful Tasks")
             table.add_column("Run Tasks")
 
             for rule in group.rules:
                 table.add_row(
                     "\n".join(rule.build_variant_regex),
+                    "\n".join(rule.display_name_regex),
                     f"{rule.success_threshold}" if rule.success_threshold else "",
                     f"{rule.run_threshold}" if rule.run_threshold else "",
                     "\n".join(rule.successful_tasks) if rule.successful_tasks else "",
                     "\n".join(rule.active_tasks) if rule.active_tasks else "",
                 )
 
             self.console.print(table)
@@ -228,15 +231,16 @@
         level=level,
         stream=sys.stderr,
     )
     for log_name in EXTERNAL_LOGGERS:
         logging.getLogger(log_name).setLevel(logging.WARNING)
 
 
-@click.command(context_settings=dict(max_content_width=100))
+@click.command(context_settings=dict(max_content_width=100, show_default=True))
+@click.pass_context
 @click.option(
     "--passing-task",
     type=str,
     multiple=True,
     help="Specify a task that needs to be passing (can be specified multiple times).",
 )
 @click.option(
@@ -258,43 +262,49 @@
     type=float,
     help="Specify the percentage of tasks that need to be failed.",
 )
 @click.option(
     "--evg-config-file",
     default=DEFAULT_EVG_CONFIG,
     type=click.Path(exists=True),
-    help=f"File containing evergreen authentication information [default={DEFAULT_EVG_CONFIG}].",
+    help="File containing evergreen authentication information.",
 )
 @click.option(
     "--evg-project",
     default=DEFAULT_EVG_PROJECT,
-    help=f"Evergreen project to query against [default={DEFAULT_EVG_PROJECT}].",
+    help="Evergreen project to query against.",
 )
 @click.option(
     "--build-variant",
     multiple=True,
-    help="Regex of Build variants to check (can be specified multiple times) [default=.*].",
+    help="Regex of Build variants to check (can be specified multiple times).",
+)
+@click.option(
+    "--display-variant-name",
+    default=[".*"],
+    multiple=True,
+    help="Regex of Build variant display names to check (can be specified multiple times).",
 )
 @click.option(
     "--commit-lookback",
     type=int,
     default=MAX_LOOKBACK,
-    help=f"Number of commits to check before giving up [default={MAX_LOOKBACK}].",
+    help="Number of commits to check before giving up.",
 )
 @click.option("--timeout-secs", type=int, help="Number of seconds to search for before giving up.")
 @click.option(
     "--commit-limit",
     type=str,
     help="Oldest commit to check before giving up.",
 )
 @click.option(
     "--git-operation",
     type=click.Choice([a.value for a in GitAction]),
-    default=GitAction.NONE,
-    help="Git operations to perform with found commit [default=none].",
+    default=GitAction.NONE.value,
+    help="Git operations to perform with found commit.",
 )
 @click.option(
     "-b",
     "--branch",
     help="Name of branch to create on checkout. When specified, git-operation is set to checkout by default.",
 )
 @click.option(
@@ -316,27 +326,29 @@
 @click.option("--export-file", type=click.Path(), help="File to write exported rules to.")
 @click.option(
     "--import-criteria", type=click.Path(exists=True), help="Import previously exported criteria."
 )
 @click.option(
     "--output-format",
     type=click.Choice([f.value for f in OutputFormat]),
-    default=OutputFormat.PLAINTEXT,
-    help="Format of the command output [default=plaintext].",
+    default=OutputFormat.PLAINTEXT.value,
+    help="Format of the command output.",
 )
 @click.option("--verbose", is_flag=True, default=False, help="Enable debug logging.")
 def main(
+    ctx: click.Context,
     passing_task: List[str],
     run_task: List[str],
     run_threshold: float,
     pass_threshold: float,
     fail_threshold: float,
     evg_config_file: str,
     evg_project: str,
     build_variant: List[str],
+    display_variant_name: List[str],
     commit_lookback: int,
     commit_limit: Optional[str],
     timeout_secs: Optional[int],
     git_operation: GitAction,
     branch: Optional[str],
     save_criteria: Optional[str],
     use_criteria: Optional[str],
@@ -379,19 +391,20 @@
 
     If you have any evergreen modules with local checkouts in the location specified in your
     project's evergreen.yml configuration file. They will automatically be checked out to the
     revision that was run in Evergreen with the revision of the base project.
 
     Examples
 
-    Working on a fix for a task 'replica_sets' on the build variants 'enterprise-rhel-80-64-bit' and
-    'enterprise-windows', to ensure the task has been run on those build variants:
+    Working on a fix for a task 'replica_sets_jscore_passthrough' on the build variants
+    '! Amazon Linux 2 arm64 (all feature flags)' and '! Enterprise Windows (all feature flags)',
+    to ensure the task has been run on those build variants:
 
       \b
-      git co-evg-base --run-task replica_sets --build-variant enterprise-rhel-80-64-bit --build-variant enterprise-windows
+      git co-evg-base --run-task replica_sets_jscore_passthrough --display-variant-name "^! Amazon Linux 2 arm64 (all feature flags)$" --display-variant-name "^! Enterprise Windows (all feature flags)$"
 
     Starting a new change, to ensure that there are no systemic failures on the base commit:
 
       \b
       git co-evg-base --pass-threshold 0.98
 
     """
@@ -424,33 +437,33 @@
         operation=git_operation,
         override_criteria=override,
         timeout_secs=timeout_secs,
         branch_name=branch,
         output_format=output_format,
     )
 
-    build_variant_checks = [".*"]
+    display_variant_name_checks = display_variant_name
 
-    if build_variant:
-        build_variant_checks = build_variant
-    else:
+    if ctx.get_parameter_source("display_variant_name") == ParameterSource.DEFAULT:
         for (
             project_regex,
-            default_build_variants,
-        ) in PROJECT_REGEX_TO_DEFAULT_BUILD_VARIANTS.items():
+            default_display_variant_name_regexes,
+        ) in PROJECT_REGEX_TO_DEFAULT_DISPLAY_VARIANT_NAME_REGEXES.items():
             if re.match(project_regex, evg_project):
                 LOGGER.debug(
-                    "Found default build variants for evg project",
-                    evg_project=project_regex,
-                    default_build_variants=default_build_variants,
+                    "Found default build variant display name regexes for evg project",
+                    evg_project_regex=project_regex,
+                    default_display_variant_name_regexes=default_display_variant_name_regexes,
                 )
-                build_variant_checks = default_build_variants
+                display_variant_name_checks = default_display_variant_name_regexes
                 break
 
-    build_checks = BuildChecks(build_variant_regex=build_variant_checks)
+    build_checks = BuildChecks(
+        build_variant_regex=build_variant, display_name_regex=display_variant_name_checks
+    )
     if pass_threshold is not None:
         build_checks.success_threshold = pass_threshold
 
     if fail_threshold is not None:
         build_checks.failure_threshold = fail_threshold
 
     if run_threshold is not None:
```

### Comparing `git_co_evg_base-3.0.6/src/goodbase/goodbase_options.py` & `git_co_evg_base-4.0.0/src/goodbase/goodbase_options.py`

 * *Files identical despite different names*

### Comparing `git_co_evg_base-3.0.6/src/goodbase/models/build_status.py` & `git_co_evg_base-4.0.0/src/goodbase/models/build_status.py`

 * *Files identical despite different names*

### Comparing `git_co_evg_base-3.0.6/src/goodbase/services/config_service.py` & `git_co_evg_base-4.0.0/src/goodbase/services/config_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,24 @@
         """
         Add the given build checks to this criteria group.
 
         :param build_checks: checks to add.
         :param override: Overwrite checks if they already exist.
         """
         existing_rules = [
-            bc for bc in self.rules if bc.build_variant_regex == build_checks.build_variant_regex
+            bc
+            for bc in self.rules
+            if bc.build_variant_regex == build_checks.build_variant_regex
+            and bc.display_name_regex == build_checks.display_name_regex
         ]
         other_rules = [
-            bc for bc in self.rules if bc.build_variant_regex != build_checks.build_variant_regex
+            bc
+            for bc in self.rules
+            if bc.build_variant_regex != build_checks.build_variant_regex
+            or bc.display_name_regex != build_checks.display_name_regex
         ]
         if existing_rules and not override:
             raise ValueError("Rule already exists, use `--override` to override it.")
         self.rules = other_rules
         self.rules.append(build_checks)
```

### Comparing `git_co_evg_base-3.0.6/src/goodbase/services/criteria_service.py` & `git_co_evg_base-4.0.0/src/goodbase/services/criteria_service.py`

 * *Files identical despite different names*

### Comparing `git_co_evg_base-3.0.6/src/goodbase/services/evg_service.py` & `git_co_evg_base-4.0.0/src/goodbase/services/evg_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from concurrent.futures import ThreadPoolExecutor as Executor
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import inject
 import structlog
 import yaml
-from evergreen import EvergreenApi, Version
+from evergreen import Build, EvergreenApi, Version
 from requests.exceptions import HTTPError
 
 from goodbase.build_checker import BuildChecks
 from goodbase.clients.evg_cli_proxy import EvgCliProxy
 from goodbase.models.build_status import BuildStatus
 
 N_THREADS = 16
@@ -28,29 +28,29 @@
 
         :param evg_api: Evergreen API client.
         :param evg_cli_proxy: Proxy for evergreen cli.
         """
         self.evg_api = evg_api
         self.evg_cli_proxy = evg_cli_proxy
 
-    def analyze_build(self, build_id: str) -> Optional[BuildStatus]:
+    @staticmethod
+    def analyze_build(build: Build) -> Optional[BuildStatus]:
         """
         Get a summary of results for the given build.
 
-        :param build_id: ID of build to analyze.
+        :param build: Evergreen build to analyze.
         :return: Summary of build.
         """
         try:
-            build = self.evg_api.build_by_id(build_id)
             tasks = build.get_tasks()
         except HTTPError as err:
             LOGGER.debug(
                 "Could not get data from Evergreen for a build",
                 status_code=err.response.status_code,
-                build_id=build_id,
+                build_id=build.id,
                 exc_info=True,
             )
             return None
 
         successful_tasks = {task.display_name for task in tasks if task.is_success()}
         inactive_tasks = {task.display_name for task in tasks if task.is_undispatched()}
         all_tasks = {task.display_name for task in tasks}
@@ -99,19 +99,22 @@
 
         :param evg_version: Evergreen version to check.
         :param build_checks: Build criteria to use.
         :return: List of build statuses.
         """
         if not evg_version.build_variants_status or len(evg_version.build_variants_status) == 0:
             return None
+        builds = evg_version.get_builds()
         with Executor(max_workers=N_THREADS) as exe:
             jobs = [
-                exe.submit(self.analyze_build, build_id)
-                for bv, build_id in evg_version.build_variants_map.items()
-                if any(bc.should_apply(bv) for bc in build_checks)
+                exe.submit(self.analyze_build, build)
+                for build in builds
+                if any(
+                    bc.should_apply(build.build_variant, build.display_name) for bc in build_checks
+                )
             ]
 
         results = []
         for j in jobs:
             result = j.result()
             if result is not None:
                 results.append(result)
```

### Comparing `git_co_evg_base-3.0.6/src/goodbase/services/file_service.py` & `git_co_evg_base-4.0.0/src/goodbase/services/file_service.py`

 * *Files identical despite different names*

### Comparing `git_co_evg_base-3.0.6/src/goodbase/services/git_service.py` & `git_co_evg_base-4.0.0/src/goodbase/services/git_service.py`

 * *Files identical despite different names*

### Comparing `git_co_evg_base-3.0.6/src/goodbase/services/search_service.py` & `git_co_evg_base-4.0.0/src/goodbase/services/search_service.py`

 * *Files identical despite different names*

### Comparing `git_co_evg_base-3.0.6/setup.py` & `git_co_evg_base-4.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,273 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: git-co-evg-base
+Version: 4.0.0
+Summary: Find a good commit to base your work on
+Home-page: https://github.com/evergreen-ci/git-co-evg-base
+Author: David Bradford
+Author-email: david.bradford@mongodb.com
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Inject (>=4.3.1,<5.0.0)
+Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: click (>=8,<9)
+Requires-Dist: evergreen.py (>=3.2.7,<4.0.0)
+Requires-Dist: plumbum (>=1.7.0,<2.0.0)
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: rich (>=10.9.0,<11.0.0)
+Requires-Dist: structlog (>=21.1.0,<22.0.0)
+Requires-Dist: xdg (>=5.1.1,<6.0.0)
+Project-URL: Repository, https://github.com/evergreen-ci/git-co-evg-base
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# git-co-evg-base
 
-packages = \
-['goodbase', 'goodbase.clients', 'goodbase.models', 'goodbase.services']
+Find and perform git actions on a recent commit that matches the specified criteria.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Inject>=4.3.1,<5.0.0',
- 'PyYAML>=5.4.1,<6.0.0',
- 'click>=8,<9',
- 'evergreen.py>=3.2.7,<4.0.0',
- 'plumbum>=1.7.0,<2.0.0',
- 'pydantic>=1.8.2,<2.0.0',
- 'rich>=10.9.0,<11.0.0',
- 'structlog>=21.1.0,<22.0.0',
- 'xdg>=5.1.1,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['git-co-evg-base = goodbase.goodbase_cli:main']}
-
-setup_kwargs = {
-    'name': 'git-co-evg-base',
-    'version': '3.0.6',
-    'description': 'Find a good commit to base your work on',
-    'long_description': "# git-co-evg-base\n\nFind and perform git actions on a recent commit that matches the specified criteria.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/git-co-evg-base) [![PyPI](https://img.shields.io/pypi/v/git-co-evg-base.svg)](https://pypi.org/project/git-co-evg-base/) [![Upload Python Package](https://github.com/evergreen-ci/git-co-evg-base/actions/workflows/deploy.yml/badge.svg)](https://github.com/evergreen-ci/git-co-evg-base/actions/workflows/deploy.yml) [![Documentation](https://img.shields.io/badge/Docs-Available-green)](https://evergreen-ci.github.io/git-co-evg-base/)\n\n## Table of contents\n\n- [git-co-evg-base](#git-co-evg-base)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Documentation](#documentation)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor's Guide](#contributors-guide)\n    - [Setting up a local development environment](#setting-up-a-local-development-environment)\n    - [linting/formatting](#lintingformatting)\n    - [Running tests](#running-tests)\n    - [Automatically running checks on commit](#automatically-running-checks-on-commit)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n  - [Resources](#resources)\n\n## Description\n\nWhen running an Evergreen patch build, it can be useful that base your\nchanges on a commit in which the tests in Evergreen have already been run.\nThis way if you encounter any failures in your patch build, you can easily\ncompare the failure with what was seen in the base commit to understand if\nyour changes may have introduced the failure.\n\nThis command allows you to specify criteria to use to find a\ngit commit to start work from.\n\n## Documentation\n\nDocumentation can be found [here](https://evergreen-ci.github.io/git-co-evg-base/).\n\n## Dependencies\n\n* Python 3.7 or later\n* git\n* [Evergreen config file](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool)\n* [Evergreen CLI](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool)\n\n## Installation\n\nWe strongly recommend using a tool like [pipx](https://pypa.github.io/pipx/) to install\nthis tool. This will isolate the dependencies and ensure they don't conflict with other tools.\n\n```bash\n$ pipx install git-co-evg-base\n```\n\n### Debugging installation issues\n\nA common issue that arises during installation is pipx failing to install git-co-evg-base and printing out the following error:\n```bash\n$ pipx install git-co-evg-base\nFatal error from pip prevented installation. Full pip output in file:\n    /home/ubuntu/.local/pipx/logs/cmd_2022-03-31_13.24.42_pip_errors.log\n\nSome possibly relevant errors from pip install:\n    ERROR: Could not find a version that satisfies the requirement git-co-evg-base (from versions: none)\n    ERROR: No matching distribution found for git-co-evg-base\n\nError installing git-co-evg-base.\n```\n\nThis error indicates that pipx could not find a version of git-co-evg-base that was built to support the version of Python installed on your machine.\nMake sure to check that your version of Python matches the requirements called out in the [Dependencies](#dependencies) section. You\ncan check the version of Python that is on your computer by running\n```bash\n$ python --version\n```\n\nIf you are running into the issue above but are sure that the correct version of Python is installed on your computer,\nyou can explicitly specify a path to the correct Python version during installation.\n\n```bash\n$ which python3.9\n/usr/bin/python3.9\n$ pipx install git-co-evg-base --python /usr/bin/python3.9\n```\n\n## Usage\n\nDetailed usage documentation can be found [here](https://github.com/evergreen-ci/git-co-evg-base/tree/main/docs/usage.md).\n\n```\nUsage: git-co-evg-base [OPTIONS]\n\n  Find and perform git actions on a recent commit that matches the specified criteria.\n\n  When running an Evergreen patch build, it can be useful that base your changes on a commit in\n  which the tests in Evergreen have already been run. This way if you encounter any failures in\n  your patch build, you can easily compare the failure with what was seen in the base commit to\n  understand if your changes may have introduced the failure.\n\n  This command allows you to specify criteria to use to find a git commit to start work from.\n\n  Criteria\n\n  There are 5 criteria that can be specified:\n\n  * The percentage of tasks that have passed in each build.\n\n  * The percentage of tasks that have failed in each build.\n\n  * The percentage of tasks that have run in each build.\n\n  * Specific tasks that must have passed in each build (if they are part of that build).\n\n  * Specific tasks that must have run in each build (if they are part of that build).\n\n  If no criteria are specified, a success threshold of 0.95 will be used and the other 4 above\n  options will be null.\n\n  Additionally, you can specify which build variants the criteria should be checked against. By\n  default, all build variants will be checked.\n\n  Notes\n\n  If you have any evergreen modules with local checkouts in the location specified in your\n  project's evergreen.yml configuration file. They will automatically be checked out to the\n  revision that was run in Evergreen with the revision of the base project.\n\n  Examples\n\n  Working on a fix for a task 'replica_sets' on the build variants 'enterprise-rhel-80-64-bit' and\n  'enterprise-windows', to ensure the task has been run on those build variants:\n\n      git co-evg-base --run-task replica_sets --build-variant enterprise-rhel-80-64-bit --build-variant enterprise-windows\n\n  Starting a new change, to ensure that there are no systemic failures on the base commit:\n\n      git co-evg-base --pass-threshold 0.98\n\nOptions:\n  --passing-task TEXT             Specify a task that needs to be passing (can be specified\n                                  multiple times).\n  --run-task TEXT                 Specify a task that needs to be run (can be specified multiple\n                                  times).\n  --run-threshold FLOAT           Specify the percentage of tasks that need to be run.\n  --pass-threshold FLOAT          Specify the percentage of tasks that need to be successful.\n  --fail-threshold FLOAT          Specify the percentage of tasks that need to be failed.\n  --evg-config-file PATH          File containing evergreen authentication information\n                                  [default=~/.evergreen.yml].\n  --evg-project TEXT              Evergreen project to query against [default=mongodb-mongo-\n                                  master].\n  --build-variant TEXT            Regex of Build variants to check (can be specified multiple\n                                  times) [default=.*-required$].\n  --commit-lookback INTEGER       Number of commits to check before giving up [default=50].\n  --timeout-secs INTEGER          Number of seconds to search for before giving up.\n  --commit-limit TEXT             Oldest commit to check before giving up.\n  --git-operation [checkout|rebase|merge|none]\n                                  Git operations to perform with found commit [default=none].\n  -b, --branch TEXT               Name of branch to create on checkout.\n  --save-criteria TEXT            Save the specified criteria rules under the specified name for\n                                  future use.\n  --use-criteria TEXT             Use previously save criteria rules.\n  --list-criteria                 Display saved criteria.\n  --override                      Override saved conflicting save criteria rules.\n  --export-criteria TEXT          Specify saved criteria to export to a file.\n  --export-file PATH              File to write exported rules to.\n  --import-criteria PATH          Import previously exported criteria.\n  --output-format [plaintext|yaml|json]\n                                  Format of the command output [default=plaintext].\n  --verbose                       Enable debug logging.\n  --help                          Show this message and exit.\n```\n\nCheckout using the default criteria:\n\n```bash\n$ git co-evg-base\n```\n\nCheckout with successful tasks 'auth' and 'auth_audit' on builds 'enterprise-windows' and\n'enterprise-rhel-80-64-bit' and 95% of the tasks are passing.\n\n```bash\n$ git co-evg-base --passing-task auth --passing-task auth_audit --run-threshold 0.95 --build-variant enterprise-windows --build-variant enterprise-rhel-80-64-bit\n```\n\n## Contributor's Guide\n\n### Setting up a local development environment\n\nThis project uses [poetry](https://python-poetry.org/) for setting up a local environment.\n\n```bash\ngit clone ...\ncd ...\npoetry install\n```\n\n### linting/formatting\n\nThis project uses [black](https://black.readthedocs.io/en/stable/) and\n[isort](https://pycqa.github.io/isort/) for formatting.\n\n```bash\npoetry run black src tests\npoetry run isort src tests\n```\n\n### Running tests\n\nThis project uses [pytest](https://docs.pytest.org/en/6.2.x/) for testing.\n\n```bash\npoetry run pytest\n```\n\n### Automatically running checks on commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time. To enable pre-commit on your local repository run:\n\n```bash\npoetry run pre-commit install\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\n\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a Github Pull Request for code review.\n\n### Deployment\n\nDeployment to pypi is automatically triggered on merges to main.\n\n## Resources\n\n* [Evergreen REST documentation](https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage)\n",
-    'author': 'David Bradford',
-    'author_email': 'david.bradford@mongodb.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/evergreen-ci/git-co-evg-base',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/git-co-evg-base) [![PyPI](https://img.shields.io/pypi/v/git-co-evg-base.svg)](https://pypi.org/project/git-co-evg-base/) [![Upload Python Package](https://github.com/evergreen-ci/git-co-evg-base/actions/workflows/deploy.yml/badge.svg)](https://github.com/evergreen-ci/git-co-evg-base/actions/workflows/deploy.yml) [![Documentation](https://img.shields.io/badge/Docs-Available-green)](https://evergreen-ci.github.io/git-co-evg-base/)
 
+## Table of contents
+
+- [git-co-evg-base](#git-co-evg-base)
+  - [Table of contents](#table-of-contents)
+  - [Description](#description)
+  - [Documentation](#documentation)
+  - [Dependencies](#dependencies)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Contributor's Guide](#contributors-guide)
+    - [Setting up a local development environment](#setting-up-a-local-development-environment)
+    - [linting/formatting](#lintingformatting)
+    - [Running tests](#running-tests)
+    - [Automatically running checks on commit](#automatically-running-checks-on-commit)
+    - [Versioning](#versioning)
+    - [Code Review](#code-review)
+    - [Deployment](#deployment)
+  - [Resources](#resources)
+
+## Description
+
+When running an Evergreen patch build, it can be useful that base your
+changes on a commit in which the tests in Evergreen have already been run.
+This way if you encounter any failures in your patch build, you can easily
+compare the failure with what was seen in the base commit to understand if
+your changes may have introduced the failure.
+
+This command allows you to specify criteria to use to find a
+git commit to start work from.
+
+## Documentation
+
+Documentation can be found [here](https://evergreen-ci.github.io/git-co-evg-base/).
+
+## Dependencies
+
+* Python 3.7 or later
+* git
+* [Evergreen config file](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool)
+* [Evergreen CLI](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool)
+
+## Installation
+
+We strongly recommend using a tool like [pipx](https://pypa.github.io/pipx/) to install
+this tool. This will isolate the dependencies and ensure they don't conflict with other tools.
+
+```bash
+$ pipx install git-co-evg-base
+```
+
+### Debugging installation issues
+
+A common issue that arises during installation is pipx failing to install git-co-evg-base and printing out the following error:
+```bash
+$ pipx install git-co-evg-base
+Fatal error from pip prevented installation. Full pip output in file:
+    /home/ubuntu/.local/pipx/logs/cmd_2022-03-31_13.24.42_pip_errors.log
+
+Some possibly relevant errors from pip install:
+    ERROR: Could not find a version that satisfies the requirement git-co-evg-base (from versions: none)
+    ERROR: No matching distribution found for git-co-evg-base
+
+Error installing git-co-evg-base.
+```
+
+This error indicates that pipx could not find a version of git-co-evg-base that was built to support the version of Python installed on your machine.
+Make sure to check that your version of Python matches the requirements called out in the [Dependencies](#dependencies) section. You
+can check the version of Python that is on your computer by running
+```bash
+$ python --version
+```
+
+If you are running into the issue above but are sure that the correct version of Python is installed on your computer,
+you can explicitly specify a path to the correct Python version during installation.
+
+```bash
+$ which python3.9
+/usr/bin/python3.9
+$ pipx install git-co-evg-base --python /usr/bin/python3.9
+```
+
+## Usage
+
+Detailed usage documentation can be found [here](https://github.com/evergreen-ci/git-co-evg-base/tree/main/docs/usage.md).
+
+```
+Usage: git-co-evg-base [OPTIONS]
+
+  Find and perform git actions on a recent commit that matches the specified criteria.
+
+  When running an Evergreen patch build, it can be useful that base your changes on a commit in
+  which the tests in Evergreen have already been run. This way if you encounter any failures in
+  your patch build, you can easily compare the failure with what was seen in the base commit to
+  understand if your changes may have introduced the failure.
+
+  This command allows you to specify criteria to use to find a git commit to start work from.
+
+  Criteria
+
+  There are 5 criteria that can be specified:
+
+  * The percentage of tasks that have passed in each build.
+
+  * The percentage of tasks that have failed in each build.
+
+  * The percentage of tasks that have run in each build.
+
+  * Specific tasks that must have passed in each build (if they are part of that build).
+
+  * Specific tasks that must have run in each build (if they are part of that build).
+
+  If no criteria are specified, a success threshold of 0.95 will be used and the other 4 above
+  options will be null.
+
+  Additionally, you can specify which build variants the criteria should be checked against. By
+  default, all build variants will be checked.
+
+  Notes
+
+  If you have any evergreen modules with local checkouts in the location specified in your
+  project's evergreen.yml configuration file. They will automatically be checked out to the
+  revision that was run in Evergreen with the revision of the base project.
+
+  Examples
+
+  Working on a fix for a task 'replica_sets_jscore_passthrough' on the build variants '! Amazon
+  Linux 2 arm64 (all feature flags)' and '! Enterprise Windows (all feature flags)', to ensure the
+  task has been run on those build variants:
+
+      git co-evg-base --run-task replica_sets_jscore_passthrough --display-variant-name "^! Amazon Linux 2 arm64 (all feature flags)$" --display-variant-name "^! Enterprise Windows (all feature flags)$"
+
+  Starting a new change, to ensure that there are no systemic failures on the base commit:
+
+      git co-evg-base --pass-threshold 0.98
+
+Options:
+  --passing-task TEXT             Specify a task that needs to be passing (can be specified
+                                  multiple times).
+  --run-task TEXT                 Specify a task that needs to be run (can be specified multiple
+                                  times).
+  --run-threshold FLOAT           Specify the percentage of tasks that need to be run.
+  --pass-threshold FLOAT          Specify the percentage of tasks that need to be successful.
+  --fail-threshold FLOAT          Specify the percentage of tasks that need to be failed.
+  --evg-config-file PATH          File containing evergreen authentication information.  [default:
+                                  /Users/<username>/.evergreen.yml]
+  --evg-project TEXT              Evergreen project to query against.  [default: mongodb-mongo-
+                                  master]
+  --build-variant TEXT            Regex of Build variants to check (can be specified multiple
+                                  times).
+  --display-variant-name TEXT     Regex of Build variant display names to check (can be specified
+                                  multiple times).  [default: .*]
+  --commit-lookback INTEGER       Number of commits to check before giving up.  [default: 50]
+  --timeout-secs INTEGER          Number of seconds to search for before giving up.
+  --commit-limit TEXT             Oldest commit to check before giving up.
+  --git-operation [checkout|rebase|merge|none]
+                                  Git operations to perform with found commit.  [default: none]
+  -b, --branch TEXT               Name of branch to create on checkout. When specified, git-
+                                  operation is set to checkout by default.
+  --save-criteria TEXT            Save the specified criteria rules under the specified name for
+                                  future use.
+  --use-criteria TEXT             Use previously save criteria rules.
+  --list-criteria                 Display saved criteria.
+  --override                      Override saved conflicting save criteria rules.
+  --export-criteria TEXT          Specify saved criteria to export to a file.
+  --export-file PATH              File to write exported rules to.
+  --import-criteria PATH          Import previously exported criteria.
+  --output-format [plaintext|yaml|json]
+                                  Format of the command output.  [default: plaintext]
+  --verbose                       Enable debug logging.
+  --help                          Show this message and exit.
+```
+
+Checkout using the default criteria:
+
+```bash
+$ git co-evg-base
+```
+
+Checkout with successful tasks 'auth' and 'auth_audit' on builds '! Enterprise Windows (all feature flags)'
+and '! Amazon Linux 2 arm64 (all feature flags)' and 95% of the tasks are passing.
+
+```bash
+$ git co-evg-base --passing-task auth --passing-task auth_audit --run-threshold 0.95 --display-variant-name "^! Enterprise Windows (all feature flags)$" --display-variant-name "^! Amazon Linux 2 arm64 (all feature flags)$"
+```
+
+## Contributor's Guide
+
+### Setting up a local development environment
+
+This project uses [poetry](https://python-poetry.org/) for setting up a local environment.
+
+```bash
+git clone ...
+cd ...
+poetry install
+```
+
+### linting/formatting
+
+This project uses [black](https://black.readthedocs.io/en/stable/) and
+[isort](https://pycqa.github.io/isort/) for formatting.
+
+```bash
+poetry run black src tests
+poetry run isort src tests
+```
+
+### Running tests
+
+This project uses [pytest](https://docs.pytest.org/en/6.2.x/) for testing.
+
+```bash
+poetry run pytest
+```
+
+### Automatically running checks on commit
+
+This project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run
+configured checks at git commit time. To enable pre-commit on your local repository run:
+
+```bash
+poetry run pre-commit install
+```
+
+### Versioning
+
+This project uses [semver](https://semver.org/) for versioning.
+
+Please include a description what is added for each new version in `CHANGELOG.md`.
+
+### Code Review
+
+Please open a Github Pull Request for code review.
+
+### Deployment
+
+Deployment to pypi is automatically triggered on merges to main.
+
+## Resources
+
+* [Evergreen REST documentation](https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage)
 
-setup(**setup_kwargs)
```

