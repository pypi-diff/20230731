# Comparing `tmp/easyecs-0.1.1.tar.gz` & `tmp/easyecs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.1.1.tar", max compression
+gzip compressed data, was "easyecs-0.1.2.tar", max compression
```

## Comparing `easyecs-0.1.1.tar` & `easyecs-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     2230 2023-07-31 17:03:44.840777 easyecs-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8473 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0     3390 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0     3511 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     8098 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0      488 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/template/verify.py
--rw-r--r--   0        0        0    12565 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1530 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2043 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2285 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/signal.py
--rw-r--r--   0        0        0      485 2023-07-31 17:03:44.860777 easyecs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 easyecs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-07-31 19:57:56.318579 easyecs-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     8375 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0     3390 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0     3511 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     7949 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/template/verify.py
+-rw-r--r--   0        0        0    12418 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1459 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2043 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     2360 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     1672 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      505 2023-07-31 19:57:56.346580 easyecs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.1.2/PKG-INFO
```

### Comparing `easyecs-0.1.1/README.md` & `easyecs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.1/easyecs/cli.py` & `easyecs-0.1.2/easyecs/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!python
 
 import time
 import inotify.adapters
-import os
 import boto3
 import click
 from easyecs.cloudformation.template import create_template
 from easyecs.cloudformation.fetch import (
     fetch_containers,
     fetch_is_stack_created,
 )
@@ -38,16 +37,16 @@
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
     vpc_id = cache_settings["vpc_id"]
     subnet_ids = cache_settings["subnet_ids"]
     azs = cache_settings["azs"]
 
     ecs_manifest = read_ecs_file()
-    app_name = ecs_manifest["metadata"]["appname"]
-    user = ecs_manifest["metadata"].get("user", os.environ["USER"])
+    app_name = ecs_manifest.metadata.appname
+    user = ecs_manifest.metadata.user
     stack_name = f"{user}-{app_name}"
 
     verify_ecs_manifest(ecs_manifest)
 
     print()
 
     loader_import = Loader(
@@ -126,16 +125,16 @@
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
     vpc_id = cache_settings["vpc_id"]
     subnet_ids = cache_settings["subnet_ids"]
     azs = cache_settings["azs"]
 
     ecs_manifest = read_ecs_file()
-    app_name = ecs_manifest["metadata"]["appname"]
-    user = ecs_manifest["metadata"].get("user", os.environ["USER"])
+    app_name = ecs_manifest.metadata.appname
+    user = ecs_manifest.metadata.user
     stack_name = f"{user}-{app_name}"
 
     verify_ecs_manifest(ecs_manifest)
 
     print()
 
     loader_import = Loader(
@@ -224,16 +223,16 @@
         thread.stop()
 
     exit(0)
 
 
 def action_delete():
     ecs_manifest = read_ecs_file()
-    app_name = ecs_manifest["metadata"]["appname"]
-    user = ecs_manifest["metadata"].get("user", os.environ["USER"])
+    app_name = ecs_manifest.metadata.appname
+    user = ecs_manifest.metadata.user
     stack_name = f"{user}-{app_name}"
     delete_stack(stack_name)
 
 
 def action_debug():
     sync_events = set(["IN_CLOSE_WRITE"])
     i = inotify.adapters.Inotify()
@@ -315,13 +314,13 @@
     show_default=True,
     help=(
         "If used, and only when there's no update on the cloudformation stack, easyecs"
         " will force a new deployment of the task."
     ),
 )
 @click.pass_context
-def click_delete(ctx):
+def click_delete(ctx, force_redeployment):
     action_delete()
 
 
 if __name__ == "__main__":
     entrypoint()
```

### Comparing `easyecs-0.1.1/easyecs/cloudformation/fetch.py` & `easyecs-0.1.2/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.1/easyecs/cloudformation/stack/__init__.py` & `easyecs-0.1.2/easyecs/cloudformation/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.1/easyecs/cloudformation/template/__init__.py` & `easyecs-0.1.2/easyecs/cloudformation/template/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,27 +58,27 @@
         ServicePrincipal,
         Role,
     )
 
     role_name = f"{service_name}-task-role"
     policy_name = f"{service_name}-task-role-policy"
     assumed_by = ServicePrincipal("ecs-tasks.amazonaws.com")
-    managed_policies_raw = ecs_manifest["role"]["managed_policies"]
+    managed_policies_raw = ecs_manifest.role.managed_policies
     managed_policies = [
         ManagedPolicy.from_aws_managed_policy_name(managed_policy)
         for managed_policy in managed_policies_raw
     ]
-    policy_statements_raw = ecs_manifest["role"]["statements"]
+    policy_statements_raw = ecs_manifest.role.statements
     policy_statements = [
         PolicyStatement(
-            sid=policy_statement["sid"],
-            actions=policy_statement["actions"],
-            resources=policy_statement["resources"],
+            sid=policy_statement.sid,
+            actions=policy_statement.actions,
+            resources=policy_statement.resources,
             effect=(
-                Effect.ALLOW if policy_statement["effect"] == "Allow" else Effect.DENY
+                Effect.ALLOW if policy_statement.effect == "Allow" else Effect.DENY
             ),
         )
         for policy_statement in policy_statements_raw
     ]
     inline_policies = PolicyDocument(statements=policy_statements)
     role: Role = Role(
         stack,
@@ -100,27 +100,27 @@
         ServicePrincipal,
         Role,
     )
 
     role_name = f"{service_name}-execution-task-role"
     policy_name = f"{service_name}-execution-task-role-policy"
     assumed_by = ServicePrincipal("ecs-tasks.amazonaws.com")
-    managed_policies_raw = ecs_manifest["execution_role"]["managed_policies"]
+    managed_policies_raw = ecs_manifest.execution_role.managed_policies
     managed_policies = [
         ManagedPolicy.from_aws_managed_policy_name(managed_policy)
         for managed_policy in managed_policies_raw
     ]
-    policy_statements_raw = ecs_manifest["execution_role"]["statements"]
+    policy_statements_raw = ecs_manifest.execution_role.statements
     policy_statements = [
         PolicyStatement(
-            sid=policy_statement["sid"],
-            actions=policy_statement["actions"],
-            resources=policy_statement["resources"],
+            sid=policy_statement.sid,
+            actions=policy_statement.actions,
+            resources=policy_statement.resources,
             effect=(
-                Effect.ALLOW if policy_statement["effect"] == "Allow" else Effect.DENY
+                Effect.ALLOW if policy_statement.effect == "Allow" else Effect.DENY
             ),
         )
         for policy_statement in policy_statements_raw
     ]
     inline_policies = PolicyDocument(statements=policy_statements)
     role: Role = Role(
         stack,
@@ -169,49 +169,49 @@
         ContainerImage,
         LogDriver,
         FargateTaskDefinition,
         Secret as ECSSecret,
     )
 
     task_definition_name = f"{service_name}-task-definition"
-    resource_limits = ecs_data["task_definition"]["resources"]["limits"]
-    cpu_limit = resource_limits["cpu"] * 1024
-    memory_limit = resource_limits["memory"]
+    resource_limits = ecs_data.task_definition.resources.limits
+    cpu_limit = resource_limits.cpu * 1024
+    memory_limit = resource_limits.memory
     task_definition: FargateTaskDefinition = FargateTaskDefinition(
         stack,
         task_definition_name,
         task_role=task_role,
         execution_role=execution_role,
         cpu=cpu_limit,
         memory_limit_mib=memory_limit,
     )
-    container_definitions = ecs_data["task_definition"]["containers"]
+    container_definitions = ecs_data.task_definition.containers
     log_configuration = LogDriver.aws_logs(stream_prefix="ecs", log_group=log_group)
     for container_definition in container_definitions:
-        name = container_definition["name"]
-        image = container_definition["image"]
-        user = container_definition.get("user", "root")
-        resource_limits = container_definition["resources"]["limits"]
-        cpu = resource_limits["cpu"] * 1024
-        memory = resource_limits["memory"]
-        command = container_definition.get("command", None).split(" ")
+        name = container_definition.name
+        image = container_definition.image
+        user = container_definition.user
+        resource_limits = container_definition.resources.limits
+        cpu = resource_limits.cpu * 1024
+        memory = resource_limits.memory
+        command = container_definition.command.split(" ")
         if not run:
             command = ["sleep", "infinity"]
         environment = {}
-        for env_definition in container_definition["env"]:
-            env_name = env_definition["name"]
-            env_value = env_definition["value"]
-            env_active = env_definition.get("active", True)
+        for env_definition in container_definition.env:
+            env_name = env_definition.name
+            env_value = env_definition.value
+            env_active = env_definition.active
             if env_active:
                 environment[env_name] = env_value
         secrets = {}
-        for secret_definition in container_definition["secrets"]:
-            secret_name = secret_definition["name"]
-            secret_field = secret_definition["field"]
-            secret_arn = secret_definition["arn"]
+        for secret_definition in container_definition.secrets:
+            secret_name = secret_definition.name
+            secret_field = secret_definition.field
+            secret_arn = secret_definition.arn
             secret = Secret.from_secret_complete_arn(
                 stack, f"{secret_name}_{name}", secret_arn
             )
             ecs_secret = ECSSecret.from_secrets_manager(secret, secret_field)
             secrets[secret_name] = ecs_secret
         task_definition.add_container(
             id=name,
```

### Comparing `easyecs-0.1.1/easyecs/command/__init__.py` & `easyecs-0.1.2/easyecs/command/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 port_forward_pids = []
 threads = []
 popen_procs_port_forward = []
 popen_procs_exec_command = []
 
 
 def create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers):
-    containers = ecs_manifest["task_definition"]["containers"]
+    containers = ecs_manifest.task_definition.containers
     for container in containers:
-        container_name = container["name"]
-        container_ports = container.get("port_forward", [])
+        container_name = container.name
+        container_ports = container.port_forward
         for container_port in container_ports:
             from_port = container_port.split(":")[0]
             to_port = container_port.split(":")[1]
             loader = Loader(
                 f"Creating port forward on {container_name} container from"
                 f" {from_port} to {to_port}:",
                 f"Creating port forward on {container_name} container from"
@@ -150,23 +150,21 @@
                         start_new_session=True,
                         input=proc_tar_local.stdout,
                         stdout=subprocess.DEVNULL,
                     )
 
 
 def run_sync_thread(parsed_containers, ecs_manifest):
-    containers = ecs_manifest["task_definition"]["containers"]
+    containers = ecs_manifest.task_definition.containers
     for container in containers:
-        synchronize = container.get("synchronize", None)
+        synchronize = container.synchronize
         if synchronize:
-            container_name = container["name"]
-            root = synchronize["root"]
-            exclude = [
-                ["--exclude", filename] for filename in synchronize.get("exclude", [])
-            ]
+            container_name = container.name
+            root = synchronize.root
+            exclude = [["--exclude", filename] for filename in synchronize.exclude]
             port = parsed_containers[container_name].get("netcat_port", None)
             if port:
                 cmd_tar_local = ["tar"]
                 for file in exclude:
                     cmd_tar_local += file
                 cmd_tar_local += [
                     "-cvzf",
@@ -188,25 +186,25 @@
                 )
                 t = StoppableThread(port, root, exclude)
                 threads.append(t)
                 t.start()
 
 
 def execute_command(ecs_manifest, parsed_containers, aws_region, aws_account):
-    containers = ecs_manifest["task_definition"]["containers"]
+    containers = ecs_manifest.task_definition.containers
     catchable_sigs = set(signal.Signals) - {signal.SIGKILL, signal.SIGSTOP}
     ssm_client = boto3.client("ssm")
     found_tty = False
     tty_cmd = ""
     for container in containers:
-        command = container.get("command", None)
+        command = container.command
         if command:
-            tty = container.get("tty", False)
-            container_name = container["name"]
-            container_command = container["command"]
+            tty = container.tty
+            container_name = container.name
+            container_command = container.command
             target = parsed_containers.get(container_name)["ssm_target"]
             parameters_nc_server = {"command": [container_command]}
             ssm_container = ssm_client.start_session(
                 Target=target,
                 DocumentName="AWS-StartInteractiveCommand",
                 Parameters=parameters_nc_server,
             )
@@ -301,19 +299,19 @@
         "https://ssm.eu-west-1.amazonaws.com",
     ]
     output = subprocess.check_output(cmd_nc_server, start_new_session=True)
     return "/nc" in output.decode("utf8").split("\n")[2]
 
 
 def run_nc_commands(parsed_containers, aws_region, aws_account, ecs_manifest):
-    containers = ecs_manifest["task_definition"]["containers"]
+    containers = ecs_manifest.task_definition.containers
     for container in containers:
-        synchronize = container.get("synchronize", None)
+        synchronize = container.synchronize
         if synchronize:
-            container_name = container["name"]
+            container_name = container.name
             parsed_container = parsed_containers.get(container_name)
             ssm_target = parsed_container["ssm_target"]
             loader = Loader(
                 f"Running netcat command on container {container_name} for"
                 " synchronization:",
                 f"Running netcat command on container {container_name} for"
                 " synchronization: \u2705",
```

### Comparing `easyecs-0.1.1/easyecs/docker/__init__.py` & `easyecs-0.1.2/easyecs/docker/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import subprocess
 from easyecs.helpers.common import parse_dict_with_env_var
 
 
 def build_docker_image(ecs_manifest):
-    containers = ecs_manifest["task_definition"]["containers"]
+    containers = ecs_manifest.task_definition.containers
     for container in containers:
-        image_name = container.get("image")
-        build = container.get("build", None)
+        image_name = container.image
+        build = container.build
         if build:
-            dockerfile = build.get("dockerfile", "Dockerfile")
+            dockerfile = build.dockerfile
             if dockerfile:
                 dockerfile = f"-f {dockerfile}"
-            target = build.get("target", None)
+            target = build.target
             if target:
                 target = f"--target {target}"
-            build_args = build.get("args", {})
+            build_args = build.args
             build_args = parse_dict_with_env_var(build_args)
             build_args_str = " ".join(
                 [f'--build-arg {key}="{value}"' for key, value in build_args.items()]
             )
             build_cmd = (
                 f"docker build -t {image_name} {dockerfile} {target} {build_args_str} ."
             )
```

### Comparing `easyecs-0.1.1/easyecs/helpers/common.py` & `easyecs-0.1.2/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.1/easyecs/helpers/loader.py` & `easyecs-0.1.2/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.1/easyecs/helpers/selector.py` & `easyecs-0.1.2/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.1/easyecs/helpers/settings.py` & `easyecs-0.1.2/easyecs/helpers/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,21 @@
     fetch_account_id,
     fetch_availability_zones,
     fetch_container_subnet_ids,
     fetch_region,
     fetch_vpc_id,
 )
 from easyecs.helpers.color import Color
+from easyecs.model.ecs import EcsFileModel
 
 
-def read_ecs_file():
+def read_ecs_file() -> EcsFileModel:
     with open("./ecs.yml") as f:
         data = yaml.load(f, Loader=SafeLoader)
-    return data
+    return EcsFileModel(**data)
 
 
 def load_settings(aws_account):
     try:
         os.makedirs(".tmp", exist_ok=True)
         with open(".tmp/easyecs.tmp", "r") as f:
             cache_configuration = json.load(f)
```

### Comparing `easyecs-0.1.1/PKG-INFO` & `easyecs-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-cdk-lib (>=2.89.0,<3.0.0)
 Requires-Dist: boto3 (>=1.28.14,<2.0.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: inotify (>=0.2.10,<0.3.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # EasyECS
 
 EasyECS is an innovative container deployment tool designed to streamline the process of launching containers within the Amazon Web Services (AWS) Elastic Container Service (ECS) Fargate. With its user-friendly interface and automated workflows, EasyECS empowers developers to efficiently manage containerized applications on the AWS cloud platform. This tool is similar to what skaffold can be in Kubernetes environment.
```

