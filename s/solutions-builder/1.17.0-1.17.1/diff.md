# Comparing `tmp/solutions_builder-1.17.0.tar.gz` & `tmp/solutions_builder-1.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solutions_builder-1.17.0.tar", max compression
+gzip compressed data, was "solutions_builder-1.17.1.tar", max compression
```

## Comparing `solutions_builder-1.17.0.tar` & `solutions_builder-1.17.1.tar`

### file list

```diff
@@ -1,202 +1,202 @@
--rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.17.0/LICENSE
--rw-r--r--   0        0        0     4828 2023-07-30 22:22:19.607467 solutions_builder-1.17.0/README.md
--rw-r--r--   0        0        0     1143 2023-07-30 23:50:00.289366 solutions_builder-1.17.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.883150 solutions_builder-1.17.0/solutions_builder/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 14:30:18.509259 solutions_builder-1.17.0/solutions_builder/cli/__init__.py
--rw-r--r--   0        0        0     6576 2023-07-30 22:21:18.189632 solutions_builder-1.17.0/solutions_builder/cli/cli.py
--rw-r--r--   0        0        0     4630 2023-07-30 19:01:45.254364 solutions_builder-1.17.0/solutions_builder/cli/cli_utils.py
--rw-r--r--   0        0        0     6488 2023-07-24 23:55:03.708526 solutions_builder-1.17.0/solutions_builder/cli/component.py
--rw-r--r--   0        0        0     5883 2023-06-20 16:37:06.248359 solutions_builder-1.17.0/solutions_builder/cli/infra.py
--rw-r--r--   0        0        0     2313 2023-07-30 19:01:45.254891 solutions_builder-1.17.0/solutions_builder/cli/set.py
--rw-r--r--   0        0        0     1416 2023-07-30 19:36:49.163334 solutions_builder-1.17.0/solutions_builder/cli/template.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.884916 solutions_builder-1.17.0/solutions_builder/copier_extensions/__init__.py
--rw-r--r--   0        0        0     4617 2023-07-30 19:01:45.255561 solutions_builder-1.17.0/solutions_builder/copier_extensions/st_helpers.py
--rw-r--r--   0        0        0      101 2023-06-27 16:32:20.329504 solutions_builder-1.17.0/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
--rw-r--r--   0        0        0      766 2023-06-27 16:32:20.329809 solutions_builder-1.17.0/solutions_builder/module_template/README.md
--rw-r--r--   0        0        0      865 2023-06-27 16:32:20.330046 solutions_builder-1.17.0/solutions_builder/module_template/copier.yaml
--rw-r--r--   0        0        0       89 2023-06-27 16:32:20.330491 solutions_builder-1.17.0/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
--rw-r--r--   0        0        0     1135 2023-06-27 16:32:20.330828 solutions_builder-1.17.0/solutions_builder/module_template/template_copier.yaml
--rw-r--r--   0        0        0     3878 2023-06-27 16:32:20.331156 solutions_builder-1.17.0/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
--rw-r--r--   0        0        0      566 2023-06-27 16:32:20.331543 solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
--rw-r--r--   0        0        0      109 2023-07-17 17:37:48.428293 solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
--rw-r--r--   0        0        0     3204 2023-07-24 17:56:25.067234 solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
--rw-r--r--   0        0        0      590 2023-06-27 16:32:20.332297 solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
--rw-r--r--   0        0        0       81 2023-06-27 16:32:20.332629 solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
--rw-r--r--   0        0        0      736 2023-06-27 16:32:20.332955 solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
--rw-r--r--   0        0        0      636 2023-06-27 16:32:20.333135 solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
--rw-r--r--   0        0        0      836 2023-06-27 16:32:20.333605 solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
--rw-r--r--   0        0        0      777 2023-06-27 16:32:20.333871 solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
--rw-r--r--   0        0        0      858 2023-06-27 16:32:20.334058 solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
--rw-r--r--   0        0        0       80 2023-06-15 16:31:59.885841 solutions_builder-1.17.0/solutions_builder/modules/restful_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1363 2023-06-27 16:32:20.334262 solutions_builder-1.17.0/solutions_builder/modules/restful_service/README.md
--rw-r--r--   0        0        0      545 2023-06-15 16:31:59.886671 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1257 2023-07-30 22:21:18.055965 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
--rw-r--r--   0        0        0      215 2023-06-15 16:31:59.887289 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-06-15 16:31:59.887400 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0       98 2023-07-19 19:21:44.171995 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     2974 2023-07-24 17:56:25.068032 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      863 2023-06-15 16:31:59.888227 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1711 2023-07-19 19:21:44.172458 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1664 2023-06-21 14:30:18.511495 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.889165 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3876 2023-06-21 14:30:18.511914 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
--rw-r--r--   0        0        0     1222 2023-06-21 14:30:18.512138 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.890086 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0     1232 2023-07-30 19:01:45.257085 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-06-15 16:31:59.891124 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2023-06-15 16:31:59.891325 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-06-15 16:31:59.891641 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-06-15 16:31:59.891935 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-06-15 16:31:59.892130 solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2305 2023-06-27 16:32:20.334559 solutions_builder-1.17.0/solutions_builder/modules/restful_service/copier.yaml
--rw-r--r--   0        0        0      120 2023-06-27 16:32:20.334922 solutions_builder-1.17.0/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-06-15 16:31:59.892900 solutions_builder-1.17.0/solutions_builder/modules/restful_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      263 2023-06-15 16:31:59.893286 solutions_builder-1.17.0/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
--rw-r--r--   0        0        0     3223 2023-06-22 05:56:48.856502 solutions_builder-1.17.0/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
--rw-r--r--   0        0        0     3269 2023-06-27 16:32:20.335275 solutions_builder-1.17.0/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-07-24 17:56:25.068742 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1572 2023-07-24 17:56:25.068959 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/README.md
--rw-r--r--   0        0        0      545 2023-07-24 17:56:25.069278 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0      215 2023-07-24 17:56:25.069954 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-07-24 17:56:25.070170 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      143 2023-07-24 17:56:25.071143 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3193 2023-07-24 17:56:25.071427 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      942 2023-07-24 17:56:25.071750 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1751 2023-07-24 17:56:25.072069 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1550 2023-07-24 17:56:25.072329 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
--rw-r--r--   0        0        0        0 2023-07-24 17:56:25.072391 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     5195 2023-07-24 17:56:25.072863 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
--rw-r--r--   0        0        0     1196 2023-07-24 17:56:25.073140 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
--rw-r--r--   0        0        0        0 2023-07-24 17:56:25.073249 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 17:56:25.073377 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
--rw-r--r--   0        0        0      430 2023-07-24 17:56:25.073672 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
--rw-r--r--   0        0        0     1348 2023-07-24 17:56:25.074022 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
--rw-r--r--   0        0        0     1138 2023-07-24 17:56:25.074230 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
--rw-r--r--   0        0        0     1232 2023-07-30 19:01:45.257414 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-07-24 17:56:25.074827 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       97 2023-07-24 17:56:25.075036 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-07-24 17:56:25.075389 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-07-24 17:56:25.075817 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-07-24 17:56:25.076190 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2667 2023-07-24 17:56:25.076875 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/copier.yaml
--rw-r--r--   0        0        0       71 2023-07-24 17:56:25.077448 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-07-24 17:56:25.077814 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      719 2023-07-24 17:56:25.078410 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
--rw-r--r--   0        0        0     2693 2023-07-24 17:56:25.078755 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
--rw-r--r--   0        0        0      930 2023-07-24 17:56:25.079130 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
--rw-r--r--   0        0        0     1280 2023-07-24 17:56:25.079504 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
--rw-r--r--   0        0        0     2076 2023-07-24 17:56:25.079902 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
--rw-r--r--   0        0        0     3851 2023-07-24 17:56:25.080437 solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-06-21 14:30:18.513363 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1369 2023-07-24 21:15:52.513805 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/copier.yaml
--rw-r--r--   0        0        0      794 2023-06-27 16:32:20.335672 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       63 2023-06-21 14:30:18.514649 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/skaffold.yaml.patch
--rw-r--r--   0        0        0      701 2023-06-15 16:31:59.895524 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf
--rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.895667 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf
--rw-r--r--   0        0        0     2486 2023-06-21 14:30:18.514915 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf
--rw-r--r--   0        0        0     1783 2023-06-15 16:31:59.895957 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf
--rw-r--r--   0        0        0      268 2023-06-21 14:30:18.515245 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
--rw-r--r--   0        0        0     1553 2023-06-21 14:30:18.515555 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf
--rw-r--r--   0        0        0       80 2023-06-21 14:30:18.515897 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     2186 2023-07-24 17:56:25.081230 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/copier.yaml
--rw-r--r--   0        0        0      180 2023-06-21 14:30:18.516469 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
--rw-r--r--   0        0        0      658 2023-06-21 14:30:18.516847 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
--rw-r--r--   0        0        0      145 2023-06-21 14:30:18.517055 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
--rw-r--r--   0        0        0      185 2023-06-21 14:30:18.517271 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
--rw-r--r--   0        0        0      378 2023-06-21 14:30:18.517461 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
--rw-r--r--   0        0        0       59 2023-06-21 14:30:18.517746 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
--rw-r--r--   0        0        0     2420 2023-06-21 14:30:18.518147 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
--rw-r--r--   0        0        0      670 2023-06-21 14:30:18.518796 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
--rw-r--r--   0        0        0     1264 2023-06-21 14:30:18.519004 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
--rw-r--r--   0        0        0      709 2023-06-21 14:30:18.519311 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
--rw-r--r--   0        0        0     1568 2023-06-21 14:30:18.519782 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
--rw-r--r--   0        0        0     1695 2023-06-21 14:30:18.520002 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
--rw-r--r--   0        0        0     1877 2023-06-21 14:30:18.520187 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
--rw-r--r--   0        0        0      480 2023-06-21 14:30:18.520341 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
--rw-r--r--   0        0        0     1802 2023-06-21 14:30:18.520745 solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
--rw-r--r--   0        0        0       80 2023-06-21 14:30:18.521191 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1048 2023-07-24 17:56:25.081536 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
--rw-r--r--   0        0        0      834 2023-06-15 16:31:59.898543 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
--rw-r--r--   0        0        0     2760 2023-06-15 16:31:59.898838 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
--rw-r--r--   0        0        0      671 2023-06-15 16:31:59.899283 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
--rw-r--r--   0        0        0     1298 2023-06-15 16:31:59.899651 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
--rw-r--r--   0        0        0       81 2023-06-15 16:31:59.899785 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
--rw-r--r--   0        0        0      196 2023-06-15 16:31:59.899968 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
--rw-r--r--   0        0        0     1967 2023-06-15 16:31:59.900160 solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
--rw-r--r--   0        0        0       90 2023-06-27 16:32:20.335915 solutions_builder-1.17.0/solutions_builder/requirements.txt
--rw-r--r--   0        0        0    68957 2023-06-15 16:31:59.901015 solutions_builder-1.17.0/solutions_builder/template_root/.github/assets/setup_local.png
--rw-r--r--   0        0        0   239307 2023-06-15 16:31:59.902244 solutions_builder-1.17.0/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
--rw-r--r--   0        0        0     2639 2023-06-15 16:31:59.902916 solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
--rw-r--r--   0        0        0     2690 2023-06-15 16:31:59.903239 solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
--rw-r--r--   0        0        0     5786 2023-06-15 16:31:59.905439 solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
--rw-r--r--   0        0        0     8049 2023-06-15 16:31:59.912323 solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
--rw-r--r--   0        0        0     3131 2023-06-15 16:31:59.916647 solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
--rw-r--r--   0        0        0      471 2023-06-15 16:31:59.917181 solutions_builder-1.17.0/solutions_builder/template_root/.gitignore
--rw-r--r--   0        0        0    14552 2023-06-15 16:31:59.919314 solutions_builder-1.17.0/solutions_builder/template_root/.pylintrc
--rw-r--r--   0        0        0      711 2023-07-30 19:36:40.143918 solutions_builder-1.17.0/solutions_builder/template_root/README.md
--rw-r--r--   0        0        0      398 2023-06-27 16:32:20.336295 solutions_builder-1.17.0/solutions_builder/template_root/components/README.md
--rw-r--r--   0        0        0      211 2023-07-30 19:01:45.257591 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
--rw-r--r--   0        0        0      395 2023-07-30 19:01:45.257720 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
--rw-r--r--   0        0        0       77 2023-07-30 19:01:45.257853 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
--rw-r--r--   0        0        0      131 2023-07-30 19:01:45.257982 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
--rw-r--r--   0        0        0      571 2023-07-30 19:01:45.258119 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
--rw-r--r--   0        0        0        0 2023-07-30 19:01:45.258192 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
--rw-r--r--   0        0        0      832 2023-07-30 19:01:45.258388 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
--rw-r--r--   0        0        0      696 2023-07-30 19:01:45.258527 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
--rw-r--r--   0        0        0       35 2023-07-30 19:01:45.258667 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
--rw-r--r--   0        0        0       91 2023-07-30 19:01:45.258836 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
--rw-r--r--   0        0        0     1377 2023-07-30 19:01:45.259011 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
--rw-r--r--   0        0        0        0 2023-07-30 19:01:45.259066 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
--rw-r--r--   0        0        0      755 2023-07-30 19:01:45.259218 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
--rw-r--r--   0        0        0     1007 2023-07-30 19:01:45.259348 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
--rw-r--r--   0        0        0     2244 2023-07-30 19:01:45.259501 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
--rw-r--r--   0        0        0        0 2023-07-30 19:01:45.259554 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
--rw-r--r--   0        0        0     1003 2023-07-30 19:01:45.259707 solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
--rw-r--r--   0        0        0     2130 2023-07-30 19:01:45.260182 solutions_builder-1.17.0/solutions_builder/template_root/copier.yaml
--rw-r--r--   0        0        0       97 2023-06-15 16:31:59.924976 solutions_builder-1.17.0/solutions_builder/template_root/firebase.json
--rw-r--r--   0        0        0       98 2023-06-15 16:31:59.925120 solutions_builder-1.17.0/solutions_builder/template_root/setup.cfg
--rw-r--r--   0        0        0      215 2023-07-30 19:01:45.260563 solutions_builder-1.17.0/solutions_builder/template_root/skaffold.yaml
--rw-r--r--   0        0        0      359 2023-07-30 19:36:40.143927 solutions_builder-1.17.0/solutions_builder/template_root/st.yaml
--rw-r--r--   0        0        0      921 2023-06-15 16:31:59.925959 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
--rw-r--r--   0        0        0      730 2023-06-15 16:31:59.926143 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
--rw-r--r--   0        0        0     3585 2023-06-15 16:31:59.926376 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
--rw-r--r--   0        0        0     1178 2023-06-15 16:31:59.926551 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
--rw-r--r--   0        0        0     5024 2023-06-15 16:31:59.927017 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
--rw-r--r--   0        0        0      190 2023-06-15 16:31:59.927289 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
--rw-r--r--   0        0        0     1185 2023-06-15 16:31:59.927608 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
--rw-r--r--   0        0        0     1601 2023-06-15 16:31:59.927810 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
--rw-r--r--   0        0        0     2364 2023-06-15 16:31:59.927994 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/firebase/main.tf
--rw-r--r--   0        0        0     1194 2023-06-15 16:31:59.928358 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/firebase/variables.tf
--rw-r--r--   0        0        0     3860 2023-07-24 21:15:52.514400 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/gke/main.tf
--rw-r--r--   0        0        0      832 2023-06-15 16:31:59.928824 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/gke/outputs.tf
--rw-r--r--   0        0        0     3386 2023-07-24 21:15:52.514752 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/gke/variables.tf
--rw-r--r--   0        0        0     2926 2023-06-15 16:31:59.930393 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
--rw-r--r--   0        0        0      692 2023-06-15 16:31:59.930656 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
--rw-r--r--   0        0        0     1087 2023-06-15 16:31:59.931016 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
--rw-r--r--   0        0        0      827 2023-06-15 16:31:59.931291 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/project_services/main.tf
--rw-r--r--   0        0        0      773 2023-06-15 16:31:59.931538 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/project_services/variables.tf
--rw-r--r--   0        0        0      953 2023-06-15 16:31:59.931934 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/service_account/main.tf
--rw-r--r--   0        0        0     1037 2023-06-15 16:31:59.932426 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/service_account/variables.tf
--rw-r--r--   0        0        0     1529 2023-06-15 16:31:59.932733 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
--rw-r--r--   0        0        0      677 2023-06-15 16:31:59.933018 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
--rw-r--r--   0        0        0     1333 2023-06-15 16:31:59.933248 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
--rw-r--r--   0        0        0     1269 2023-06-15 16:31:59.933426 solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
--rw-r--r--   0        0        0     2193 2023-06-15 16:31:59.933834 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
--rw-r--r--   0        0        0      730 2023-06-15 16:31:59.934084 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
--rw-r--r--   0        0        0       66 2023-06-15 16:31:59.934377 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
--rw-r--r--   0        0        0     1071 2023-06-15 16:31:59.934790 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
--rw-r--r--   0        0        0      826 2023-06-15 16:31:59.935095 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
--rw-r--r--   0        0        0      517 2023-06-15 16:31:59.935395 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
--rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.935538 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
--rw-r--r--   0        0        0     4400 2023-07-24 17:56:25.082298 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
--rw-r--r--   0        0        0      997 2023-06-15 16:31:59.935925 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
--rw-r--r--   0        0        0      835 2023-06-15 16:31:59.936181 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
--rw-r--r--   0        0        0      606 2023-06-15 16:31:59.936549 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
--rw-r--r--   0        0        0     2546 2023-06-15 16:31:59.936876 solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.937992 solutions_builder-1.17.0/solutions_builder/template_root/tests/__init__.py
--rw-r--r--   0        0        0      825 2023-06-15 16:31:59.938319 solutions_builder-1.17.0/solutions_builder/template_root/tests/e2e/e2e_utils.py
--rwxr-xr-x   0        0        0      364 2023-06-15 16:31:59.938529 solutions_builder-1.17.0/solutions_builder/template_root/utils/disable_org_policies.sh
--rwxr-xr-x   0        0        0     1094 2023-07-30 22:21:18.148228 solutions_builder-1.17.0/solutions_builder/template_root/utils/init_env_vars.sh
--rw-r--r--   0        0        0       81 2023-06-15 16:31:59.939607 solutions_builder-1.17.0/solutions_builder/template_root/{{_copier_conf.answers_file}}
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.939700 solutions_builder-1.17.0/solutions_builder/tests/__init__.py
--rw-r--r--   0        0        0     5935 1970-01-01 00:00:00.000000 solutions_builder-1.17.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.17.1/LICENSE
+-rw-r--r--   0        0        0     4828 2023-07-31 15:22:50.618546 solutions_builder-1.17.1/README.md
+-rw-r--r--   0        0        0     1150 2023-07-31 19:04:38.966647 solutions_builder-1.17.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622568 solutions_builder-1.17.1/solutions_builder/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622645 solutions_builder-1.17.1/solutions_builder/cli/__init__.py
+-rw-r--r--   0        0        0     6576 2023-07-31 18:15:08.854346 solutions_builder-1.17.1/solutions_builder/cli/cli.py
+-rw-r--r--   0        0        0     4630 2023-07-31 18:15:08.854833 solutions_builder-1.17.1/solutions_builder/cli/cli_utils.py
+-rw-r--r--   0        0        0     6488 2023-07-31 18:15:08.855383 solutions_builder-1.17.1/solutions_builder/cli/component.py
+-rw-r--r--   0        0        0     5883 2023-07-31 18:15:08.855940 solutions_builder-1.17.1/solutions_builder/cli/infra.py
+-rw-r--r--   0        0        0     2313 2023-07-31 18:15:08.856262 solutions_builder-1.17.1/solutions_builder/cli/set.py
+-rw-r--r--   0        0        0     1416 2023-07-31 18:15:08.856690 solutions_builder-1.17.1/solutions_builder/cli/template.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.624032 solutions_builder-1.17.1/solutions_builder/copier_extensions/__init__.py
+-rw-r--r--   0        0        0     4617 2023-07-31 18:15:08.857361 solutions_builder-1.17.1/solutions_builder/copier_extensions/st_helpers.py
+-rw-r--r--   0        0        0      101 2023-07-31 15:22:50.624510 solutions_builder-1.17.1/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
+-rw-r--r--   0        0        0      766 2023-07-31 15:22:50.624649 solutions_builder-1.17.1/solutions_builder/module_template/README.md
+-rw-r--r--   0        0        0      865 2023-07-31 15:22:50.624799 solutions_builder-1.17.1/solutions_builder/module_template/copier.yaml
+-rw-r--r--   0        0        0       89 2023-07-31 15:22:50.625018 solutions_builder-1.17.1/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
+-rw-r--r--   0        0        0     1135 2023-07-31 15:22:50.625172 solutions_builder-1.17.1/solutions_builder/module_template/template_copier.yaml
+-rw-r--r--   0        0        0     3878 2023-07-31 18:15:08.857842 solutions_builder-1.17.1/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
+-rw-r--r--   0        0        0      566 2023-07-31 15:22:50.625671 solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
+-rw-r--r--   0        0        0      109 2023-07-31 15:22:50.625798 solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
+-rw-r--r--   0        0        0     3204 2023-07-31 15:22:50.625960 solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
+-rw-r--r--   0        0        0      590 2023-07-31 18:15:08.858360 solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.626261 solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
+-rw-r--r--   0        0        0      736 2023-07-31 18:15:08.858809 solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
+-rw-r--r--   0        0        0      636 2023-07-31 18:15:08.859174 solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
+-rw-r--r--   0        0        0      836 2023-07-31 18:15:08.859431 solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
+-rw-r--r--   0        0        0      777 2023-07-31 18:15:08.860677 solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
+-rw-r--r--   0        0        0      858 2023-07-31 18:15:08.861114 solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.627394 solutions_builder-1.17.1/solutions_builder/modules/restful_service/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1363 2023-07-31 15:22:50.627536 solutions_builder-1.17.1/solutions_builder/modules/restful_service/README.md
+-rw-r--r--   0        0        0      545 2023-07-31 15:22:50.627695 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1257 2023-07-31 15:22:50.628306 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.628605 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.628881 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0       98 2023-07-31 15:22:50.629046 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     2974 2023-07-31 15:22:50.629209 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      862 2023-07-31 18:15:08.861667 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1711 2023-07-31 18:15:08.861913 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1664 2023-07-31 18:15:08.862151 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.629799 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     3876 2023-07-31 18:15:08.863155 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
+-rw-r--r--   0        0        0     1222 2023-07-31 18:15:08.863993 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.630283 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.630545 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-07-31 15:22:50.630703 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2023-07-31 15:22:50.630849 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-07-31 15:22:50.630997 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-07-31 15:22:50.631183 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-07-31 15:22:50.631328 solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2305 2023-07-31 15:22:50.631452 solutions_builder-1.17.1/solutions_builder/modules/restful_service/copier.yaml
+-rw-r--r--   0        0        0      120 2023-07-31 15:22:50.631626 solutions_builder-1.17.1/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2023-07-31 15:22:50.631734 solutions_builder-1.17.1/solutions_builder/modules/restful_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      263 2023-07-31 15:22:50.631945 solutions_builder-1.17.1/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
+-rw-r--r--   0        0        0     3223 2023-07-31 15:22:50.632152 solutions_builder-1.17.1/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
+-rw-r--r--   0        0        0     3269 2023-07-31 15:22:50.632352 solutions_builder-1.17.1/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.632549 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1572 2023-07-31 15:22:50.632676 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/README.md
+-rw-r--r--   0        0        0      545 2023-07-31 15:22:50.632822 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.632992 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.633061 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0      143 2023-07-31 15:22:50.633183 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     3193 2023-07-31 15:22:50.633333 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      942 2023-07-31 18:15:08.864488 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1751 2023-07-31 18:15:08.864850 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1550 2023-07-31 18:15:08.865404 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.633781 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     5195 2023-07-31 18:15:08.866038 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
+-rw-r--r--   0        0        0     1196 2023-07-31 18:15:08.866510 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634163 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634237 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-31 15:22:50.634359 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
+-rw-r--r--   0        0        0     1348 2023-07-31 15:22:50.634473 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
+-rw-r--r--   0        0        0     1138 2023-07-31 15:22:50.634593 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
+-rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.634791 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-07-31 15:22:50.634913 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       97 2023-07-31 15:22:50.635030 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-07-31 15:22:50.635163 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-07-31 15:22:50.635357 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-07-31 15:22:50.635506 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2667 2023-07-31 15:22:50.635659 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/copier.yaml
+-rw-r--r--   0        0        0       71 2023-07-31 15:22:50.635866 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2023-07-31 15:22:50.635986 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      719 2023-07-31 18:15:08.867078 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
+-rw-r--r--   0        0        0     2693 2023-07-31 18:15:08.867595 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
+-rw-r--r--   0        0        0      930 2023-07-31 18:15:08.868573 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
+-rw-r--r--   0        0        0     1280 2023-07-31 18:15:08.869038 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
+-rw-r--r--   0        0        0     2076 2023-07-31 18:15:08.869331 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
+-rw-r--r--   0        0        0     3851 2023-07-31 18:15:08.869640 solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.637527 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1369 2023-07-31 15:22:50.637698 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/copier.yaml
+-rw-r--r--   0        0        0      794 2023-07-31 15:22:50.637941 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       63 2023-07-31 15:22:50.638097 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/skaffold.yaml.patch
+-rw-r--r--   0        0        0      701 2023-07-31 18:15:08.870023 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 18:15:08.870356 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf
+-rw-r--r--   0        0        0     2486 2023-07-31 18:15:08.870677 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf
+-rw-r--r--   0        0        0     1783 2023-07-31 18:15:08.871043 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf
+-rw-r--r--   0        0        0      268 2023-07-31 15:22:50.639380 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
+-rw-r--r--   0        0        0     1553 2023-07-31 18:15:08.871438 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.641148 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     2186 2023-07-31 15:22:50.641453 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/copier.yaml
+-rw-r--r--   0        0        0      180 2023-07-31 15:22:50.641792 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
+-rw-r--r--   0        0        0      658 2023-07-31 15:22:50.641933 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
+-rw-r--r--   0        0        0      145 2023-07-31 15:22:50.642056 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
+-rw-r--r--   0        0        0      185 2023-07-31 15:22:50.642172 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
+-rw-r--r--   0        0        0      378 2023-07-31 15:22:50.642293 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
+-rw-r--r--   0        0        0       59 2023-07-31 15:22:50.642402 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
+-rw-r--r--   0        0        0     2420 2023-07-31 18:15:08.871703 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
+-rw-r--r--   0        0        0      670 2023-07-31 18:15:08.872051 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
+-rw-r--r--   0        0        0     1264 2023-07-31 18:15:08.872364 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
+-rw-r--r--   0        0        0      709 2023-07-31 18:15:08.872682 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 18:15:08.872908 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
+-rw-r--r--   0        0        0     1695 2023-07-31 18:15:08.873182 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
+-rw-r--r--   0        0        0     1877 2023-07-31 18:15:08.873452 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
+-rw-r--r--   0        0        0      480 2023-07-31 15:22:50.643659 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
+-rw-r--r--   0        0        0     1802 2023-07-31 18:15:08.873897 solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.644034 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1048 2023-07-31 15:22:50.644166 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
+-rw-r--r--   0        0        0      834 2023-07-31 18:15:08.874208 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
+-rw-r--r--   0        0        0     2760 2023-07-31 15:22:50.644547 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
+-rw-r--r--   0        0        0      670 2023-07-31 18:15:08.874591 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
+-rw-r--r--   0        0        0     1298 2023-07-31 18:15:08.874979 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.644903 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
+-rw-r--r--   0        0        0      196 2023-07-31 15:22:50.645021 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
+-rw-r--r--   0        0        0     1984 2023-07-31 18:15:08.875232 solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
+-rw-r--r--   0        0        0       90 2023-07-31 15:22:50.645285 solutions_builder-1.17.1/solutions_builder/requirements.txt
+-rw-r--r--   0        0        0    68957 2023-07-31 15:22:50.645771 solutions_builder-1.17.1/solutions_builder/template_root/.github/assets/setup_local.png
+-rw-r--r--   0        0        0   239307 2023-07-31 15:22:50.647206 solutions_builder-1.17.1/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
+-rw-r--r--   0        0        0     2639 2023-07-31 15:22:50.647454 solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
+-rw-r--r--   0        0        0     2690 2023-07-31 15:22:50.647592 solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
+-rw-r--r--   0        0        0     5786 2023-07-31 15:22:50.648204 solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
+-rw-r--r--   0        0        0     8049 2023-07-31 15:22:50.648360 solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
+-rw-r--r--   0        0        0     3131 2023-07-31 15:22:50.648490 solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
+-rw-r--r--   0        0        0      471 2023-07-31 15:22:50.648622 solutions_builder-1.17.1/solutions_builder/template_root/.gitignore
+-rw-r--r--   0        0        0    14552 2023-07-31 15:22:50.648747 solutions_builder-1.17.1/solutions_builder/template_root/.pylintrc
+-rw-r--r--   0        0        0      711 2023-07-31 15:22:50.649129 solutions_builder-1.17.1/solutions_builder/template_root/README.md
+-rw-r--r--   0        0        0      398 2023-07-31 15:22:50.649329 solutions_builder-1.17.1/solutions_builder/template_root/components/README.md
+-rw-r--r--   0        0        0      211 2023-07-31 15:22:50.649479 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
+-rw-r--r--   0        0        0      395 2023-07-31 15:22:50.649633 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.649720 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
+-rw-r--r--   0        0        0      131 2023-07-31 15:22:50.649904 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
+-rw-r--r--   0        0        0      571 2023-07-31 15:22:50.650164 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.650248 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
+-rw-r--r--   0        0        0      831 2023-07-31 18:15:08.875632 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
+-rw-r--r--   0        0        0      695 2023-07-31 18:15:08.876536 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
+-rw-r--r--   0        0        0       35 2023-07-31 15:22:50.650730 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
+-rw-r--r--   0        0        0       91 2023-07-31 15:22:50.650873 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
+-rw-r--r--   0        0        0     1376 2023-07-31 18:15:08.876835 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651072 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
+-rw-r--r--   0        0        0      754 2023-07-31 18:15:08.877104 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
+-rw-r--r--   0        0        0     1006 2023-07-31 18:15:08.877464 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
+-rw-r--r--   0        0        0     2243 2023-07-31 18:15:08.877823 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651579 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-31 18:15:08.878095 solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
+-rw-r--r--   0        0        0     2130 2023-07-31 15:22:50.651893 solutions_builder-1.17.1/solutions_builder/template_root/copier.yaml
+-rw-r--r--   0        0        0       97 2023-07-31 15:22:50.652011 solutions_builder-1.17.1/solutions_builder/template_root/firebase.json
+-rw-r--r--   0        0        0       98 2023-07-31 15:22:50.652089 solutions_builder-1.17.1/solutions_builder/template_root/setup.cfg
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.652207 solutions_builder-1.17.1/solutions_builder/template_root/skaffold.yaml
+-rw-r--r--   0        0        0      359 2023-07-31 15:22:50.652564 solutions_builder-1.17.1/solutions_builder/template_root/st.yaml
+-rw-r--r--   0        0        0      921 2023-07-31 18:15:08.878359 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
+-rw-r--r--   0        0        0      730 2023-07-31 18:15:08.878713 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
+-rw-r--r--   0        0        0     3585 2023-07-31 18:15:08.879095 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
+-rw-r--r--   0        0        0     1178 2023-07-31 18:15:08.879619 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
+-rw-r--r--   0        0        0     5024 2023-07-31 18:15:08.879881 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
+-rw-r--r--   0        0        0      190 2023-07-31 15:22:50.653603 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
+-rw-r--r--   0        0        0     1186 2023-07-31 18:15:08.880381 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
+-rw-r--r--   0        0        0     1601 2023-07-31 18:15:08.880648 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
+-rw-r--r--   0        0        0     2364 2023-07-31 18:15:08.880910 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/firebase/main.tf
+-rw-r--r--   0        0        0     1194 2023-07-31 18:15:08.881457 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/firebase/variables.tf
+-rw-r--r--   0        0        0     3860 2023-07-31 18:15:08.881824 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/gke/main.tf
+-rw-r--r--   0        0        0      832 2023-07-31 18:15:08.882060 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/gke/outputs.tf
+-rw-r--r--   0        0        0     3386 2023-07-31 18:15:08.882381 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/gke/variables.tf
+-rw-r--r--   0        0        0     2926 2023-07-31 18:15:08.882728 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
+-rw-r--r--   0        0        0      692 2023-07-31 18:15:08.882988 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
+-rw-r--r--   0        0        0     1087 2023-07-31 18:15:08.883243 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
+-rw-r--r--   0        0        0      827 2023-07-31 18:15:08.883600 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/project_services/main.tf
+-rw-r--r--   0        0        0      774 2023-07-31 18:15:08.883935 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/project_services/variables.tf
+-rw-r--r--   0        0        0      953 2023-07-31 18:15:08.884177 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/service_account/main.tf
+-rw-r--r--   0        0        0     1037 2023-07-31 18:15:08.884389 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/service_account/variables.tf
+-rw-r--r--   0        0        0     1529 2023-07-31 18:15:08.884649 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
+-rw-r--r--   0        0        0      678 2023-07-31 18:15:08.885002 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
+-rw-r--r--   0        0        0     1333 2023-07-31 18:15:08.885363 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
+-rw-r--r--   0        0        0     1269 2023-07-31 18:15:08.885688 solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
+-rw-r--r--   0        0        0     2193 2023-07-31 15:22:50.656401 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
+-rw-r--r--   0        0        0      730 2023-07-31 18:15:08.886192 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
+-rw-r--r--   0        0        0       66 2023-07-31 15:22:50.656645 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
+-rw-r--r--   0        0        0     1071 2023-07-31 18:15:08.886491 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
+-rw-r--r--   0        0        0      826 2023-07-31 18:15:08.886753 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
+-rw-r--r--   0        0        0      517 2023-07-31 15:22:50.657065 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 18:15:08.887003 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
+-rw-r--r--   0        0        0     4400 2023-07-31 18:15:08.887546 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
+-rw-r--r--   0        0        0      991 2023-07-31 18:15:08.887983 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
+-rw-r--r--   0        0        0      835 2023-07-31 18:15:08.888294 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
+-rw-r--r--   0        0        0      606 2023-07-31 15:22:50.657649 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
+-rw-r--r--   0        0        0     2546 2023-07-31 18:15:08.888624 solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.657846 solutions_builder-1.17.1/solutions_builder/template_root/tests/__init__.py
+-rw-r--r--   0        0        0      825 2023-07-31 15:22:50.658012 solutions_builder-1.17.1/solutions_builder/template_root/tests/e2e/e2e_utils.py
+-rwxr-xr-x   0        0        0      364 2023-07-31 15:22:50.658190 solutions_builder-1.17.1/solutions_builder/template_root/utils/disable_org_policies.sh
+-rwxr-xr-x   0        0        0      990 2023-07-31 18:15:08.888898 solutions_builder-1.17.1/solutions_builder/template_root/utils/init_env_vars.sh
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.658645 solutions_builder-1.17.1/solutions_builder/template_root/{{_copier_conf.answers_file}}
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.658746 solutions_builder-1.17.1/solutions_builder/tests/__init__.py
+-rw-r--r--   0        0        0     5942 1970-01-01 00:00:00.000000 solutions_builder-1.17.1/PKG-INFO
```

### Comparing `solutions_builder-1.17.0/LICENSE` & `solutions_builder-1.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/README.md` & `solutions_builder-1.17.1/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/pyproject.toml` & `solutions_builder-1.17.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solutions-builder"
-version = "1.17.0"
+version = "1.17.1"
 description = "A solution framework to generate a project with built-in structure and modules"
 authors = ["Jon Chen <jonchen@google.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/GoogleCloudPlatform/solutions-builder"
 repository = "https://github.com/GoogleCloudPlatform/solutions-builder"
 packages = [
@@ -24,15 +24,15 @@
 pyyaml = "^6.0"
 typer = "^0.9.0"
 jinja2-time = "^0.2.0"
 copier-templates-extensions = "^0.3.0"
 pathlib = "^1.0.1"
 jinja2 = "^3.1.2"
 jinja2-strcase = "^0.0.2"
-pydantic = "<2"
+pydantic = "<=1.10.12"
 
 [tool.poetry.group.dev.dependencies]
 python = ">=3.8,<4.0"
 copier-templates-extensions = "^0.3.0"
 copier = "^7.2.0"
 PyYAML = "^6.0"
 jinja2-time = "^0.2.0"
```

### Comparing `solutions_builder-1.17.0/solutions_builder/cli/cli.py` & `solutions_builder-1.17.1/solutions_builder/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/cli/cli_utils.py` & `solutions_builder-1.17.1/solutions_builder/cli/cli_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/cli/component.py` & `solutions_builder-1.17.1/solutions_builder/cli/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/cli/infra.py` & `solutions_builder-1.17.1/solutions_builder/cli/infra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/cli/set.py` & `solutions_builder-1.17.1/solutions_builder/cli/set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/cli/template.py` & `solutions_builder-1.17.1/solutions_builder/cli/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/copier_extensions/st_helpers.py` & `solutions_builder-1.17.1/solutions_builder/copier_extensions/st_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/README.md` & `solutions_builder-1.17.1/solutions_builder/module_template/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/copier.yaml` & `solutions_builder-1.17.1/solutions_builder/module_template/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/template_copier.yaml` & `solutions_builder-1.17.1/solutions_builder/module_template/template_copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml` & `solutions_builder-1.17.1/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+"""
+DB Client fixture for re-use in testing
+"""
+
+import pytest
+from google.cloud.bigquery import Client
+
+client = Client()
+
 
-# TODO: Add main code below.
+@pytest.fixture(scope="module")
+def client_fixture():
+  yield client
```

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -13,11 +13,11 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 terraform {
   backend "gcs" {
-    bucket = {% raw %}"{{project_id}}-tfstate"{% endraw %}
-    prefix = "stage/{{terraform_stage}}"
+    bucket = "{{project_id}}-tfstate"
+    prefix = "stage/3-gke-ingress"
   }
 }
```

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/README.md` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/README.md` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 """
   Sample Service config file
 """
 import os
 
 PORT = os.environ["PORT"] if os.environ.get("PORT") is not None else 80
 PROJECT_ID = os.environ.get("PROJECT_ID") or \
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/copier.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/README.md` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/copier.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/copier.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/copier.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -11,10 +11,14 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-output "ingress_ip_address" {
-  value = local.global_static_ip_name
+output "project_id" {
+  value = var.project_id
+}
+
+output "tfstate-bucket" {
+  value = google_storage_bucket.tfstate-bucket.name
 }
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -13,11 +13,11 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 terraform {
   backend "gcs" {
-    bucket = "{{project_id}}-tfstate"
-    prefix = "stage/3-gke-ingress"
+    bucket = {% raw %}"{{project_id}}-tfstate"{% endraw %}
+    prefix = "stage/{{terraform_stage}}"
   }
 }
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -12,9 +12,9 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 output "lb_https_ip_address" {
-  value =  module.lb-http.external_ip
+  value = module.lb-http.external_ip
 }
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -32,25 +32,25 @@
   validation {
     condition     = length(var.region) > 0
     error_message = "The region value must be an non-empty string."
   }
 }
 
 variable "loadbalancer_name" {
-  type = string
+  type    = string
   default = "http-lb"
 }
 
 variable "domains" {
-  type = string
+  type        = string
   description = "List of domains attached to the LB, comma-separated."
 }
 
 variable "cloudrun_services" {
-  type = string
+  type        = string
   description = "List of Cloud Run service names, comma-separated."
 }
 
 variable "security_policy" {
   description = "The resource URL for the security policy to associate with the backend service"
   type        = string
   default     = null
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.github/assets/setup_local.png` & `solutions_builder-1.17.1/solutions_builder/template_root/.github/assets/setup_local.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png` & `solutions_builder-1.17.1/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml` & `solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml` & `solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml` & `solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml` & `solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml` & `solutions_builder-1.17.1/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/.pylintrc` & `solutions_builder-1.17.1/solutions_builder/template_root/.pylintrc`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/README.md` & `solutions_builder-1.17.1/solutions_builder/template_root/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 """
 Config module to setup common environment
 """
 
 import os
 
 PROJECT_ID = os.environ.get("PROJECT_ID", "")
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 """
   File for reusing db clients
 """
 from google.cloud import bigquery
 
 client = bigquery.Client()
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 """
 Data model for example list.
 """
 
 import os
 
 from firedantic import Model
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/project_services/main.tf`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-"""
-Copyright 2022 Google LLC
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    https://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-"""
-DB Client fixture for re-use in testing
-"""
-
-import pytest
-from google.cloud.bigquery import Client
-
-client = Client()
-
-
-@pytest.fixture(scope="module")
-def client_fixture():
-  yield client
+/**
+ * Copyright 2023 Google LLC
+ *
+ * Licensed under the Apache License, Version 2.0 (the "License");
+ * you may not use this file except in compliance with the License.
+ * You may obtain a copy of the License at
+ *
+ *     https://www.apache.org/licenses/LICENSE-2.0
+ *
+ * Unless required by applicable law or agreed to in writing, software
+ * distributed under the License is distributed on an "AS IS" BASIS,
+ * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+ * See the License for the specific language governing permissions and
+ * limitations under the License.
+ *
+ */
+
+resource "google_project_service" "project-apis" {
+  for_each                   = toset(var.services)
+  project                    = var.project_id
+  service                    = each.value
+  disable_dependent_services = true
+}
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 """
   Pytest Fixture for getting testclient from fastapi
 """
 
 # disabling pylint rules that conflict with pytest fixtures
 # pylint: disable=unused-argument,redefined-outer-name,unused-import
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 """
   Pytest Fixture for getting firestore emulator
 """
 import os
 import signal
 import subprocess
 import time
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py` & `solutions_builder-1.17.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-Copyright 2022 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 """class and methods for logs handling."""
 
 import logging
 
 logging.basicConfig(level=logging.INFO)
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/copier.yaml` & `solutions_builder-1.17.1/solutions_builder/template_root/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -15,11 +15,7 @@
  *
  */
 
 variable "project_id" {
   type        = string
   description = "project ID"
 }
-
-variable "storage_multiregion" {
-  type = string
-}
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudrun/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/cloudrun/main.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/compute_backend/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/compute_backend/main.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
@@ -36,8 +36,8 @@
     module_name = "blueprints/terraform/terraform-google-lb-http:serverless_negs/v9.0.0"
   }
 
   provider_meta "google-beta" {
     module_name = "blueprints/terraform/terraform-google-lb-http:serverless_negs/v9.0.0"
   }
 
-}
+}
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/firebase/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/firebase/main.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/firebase/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/firebase/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/gke/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/gke/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/gke/outputs.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/gke/outputs.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/gke/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/gke/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/project_services/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/project_services/variables.tf`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -11,13 +11,16 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-resource "google_project_service" "project-apis" {
-  for_each                   = toset(var.services)
-  project                    = var.project_id
-  service                    = each.value
-  disable_dependent_services = true
-}
+variable "project_id" {
+  type        = string
+  description = "project ID"
+}
+
+variable "services" {
+  type        = list(any)
+  description = "List of services to enable"
+}
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/project_services/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/service_account/main.tf`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -11,16 +11,17 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-variable "project_id" {
-  type        = string
-  description = "project ID"
+module "service_accounts" {
+  source        = "terraform-google-modules/service-accounts/google"
+  version       = "~> 3.0"
+  project_id    = var.project_id
+  names         = ["${var.name}"]
+  display_name  = var.display_name
+  description   = var.description
+  project_roles = [for i in var.roles : "${var.project_id}=>${i}"]
+  generate_keys = false
 }
-
-variable "services" {
-  type        = list(any)
-  description = "List of services to enable"
-}
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/service_account/main.tf` & `solutions_builder-1.17.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -11,17 +11,10 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-module "service_accounts" {
-  source        = "terraform-google-modules/service-accounts/google"
-  version       = "~> 3.0"
-  project_id    = var.project_id
-  names         = ["${var.name}"]
-  display_name  = var.display_name
-  description   = var.description
-  project_roles = [for i in var.roles : "${var.project_id}=>${i}"]
-  generate_keys = false
+output "ingress_ip_address" {
+  value = local.global_static_ip_name
 }
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/service_account/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/service_account/variables.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf` & `solutions_builder-1.17.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-/**
- * Copyright 2022 Google LLC
- *
- * Licensed under the Apache License, Version 2.0 (the "License");
- * you may not use this file except in compliance with the License.
- * You may obtain a copy of the License at
- *
- *     https://www.apache.org/licenses/LICENSE-2.0
- *
- * Unless required by applicable law or agreed to in writing, software
- * distributed under the License is distributed on an "AS IS" BASIS,
- * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
- * See the License for the specific language governing permissions and
- * limitations under the License.
- *
- */
+"""
+Copyright 2023 Google LLC
 
-variable "project_id" {
-  type        = string
-  description = "project ID"
-}
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    https://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+# TODO: Add main code below.
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/vpc_network/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/vpc_network/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
@@ -11,14 +11,30 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-output "project_id" {
-  value = var.project_id
+output "vpc_network" {
+  value = var.vpc_network
 }
 
-output "tfstate-bucket" {
-  value = google_storage_bucket.tfstate-bucket.name
+output "vpc_subnetwork" {
+  value = var.vpc_subnetwork
+}
+
+output "ip_cidr_range" {
+  value = var.ip_cidr_range
+}
+
+output "master_ipv4_cidr_block" {
+  value = var.master_ipv4_cidr_block
+}
+
+output "secondary_ranges_pods" {
+  value = var.secondary_ranges_pods
+}
+
+output "secondary_ranges_services" {
+  value = var.secondary_ranges_services
 }
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/main.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/main.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf` & `solutions_builder-1.17.1/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright 2022 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     https://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/tests/e2e/e2e_utils.py` & `solutions_builder-1.17.1/solutions_builder/template_root/tests/e2e/e2e_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.0/solutions_builder/template_root/utils/init_env_vars.sh` & `solutions_builder-1.17.1/solutions_builder/template_root/utils/init_env_vars.sh`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #!/bin/bash
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# This script automates all the setup steps after creating code skeleton using
-# the Solutions Builder and set up all components to a brand-new Google Cloud
-# project.
+#!/bin/bash
+
+set -f
 
-export PROJECT_ID="{{project_id}}"
-export REGION="{{gcp_region}}"
+# Hardcoded the project ID for all local development.
+declare -a EnvVars=(
+  "SA_EMAIL"
+)
+for variable in "${EnvVars[@]}"; do
+  if [[ -z "${!variable}" ]]; then
+    printf "$variable is not set.\n"
+    exit 1
+  fi
+done
 
-{% if deploy_with_gke == true -%}
-export CLUSTER_NAME=main-cluster
-{%- endif %}
+mkdir -p .tmp
+gcloud iam service-accounts keys create .tmp/sa-key.json --iam-account=$SA_EMAIL
 
-# # Terraform impersonate service account
-# export TF_RUNNER_SA_EMAIL="terraform-runner@$PROJECT_ID.iam.gserviceaccount.com"
-# export GOOGLE_IMPERSONATE_SERVICE_ACCOUNT=$TF_RUNNER_SA_EMAIL
+gcloud auth activate-service-account --key-file=.tmp/sa-key.json
```

### Comparing `solutions_builder-1.17.0/PKG-INFO` & `solutions_builder-1.17.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solutions-builder
-Version: 1.17.0
+Version: 1.17.1
 Summary: A solution framework to generate a project with built-in structure and modules
 Home-page: https://github.com/GoogleCloudPlatform/solutions-builder
 License: Apache
 Author: Jon Chen
 Author-email: jonchen@google.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: copier (>=7.2.0,<8.0.0)
 Requires-Dist: copier-templates-extensions (>=0.3.0,<0.4.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jinja2-strcase (>=0.0.2,<0.0.3)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
-Requires-Dist: pydantic (<2)
+Requires-Dist: pydantic (<=1.10.12)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/GoogleCloudPlatform/solutions-builder
 Description-Content-Type: text/markdown
 
 # Google Cloud Solutions Builder
```

