# Comparing `tmp/solutions_builder-1.17.5.tar.gz` & `tmp/solutions_builder-1.17.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solutions_builder-1.17.5.tar", max compression
+gzip compressed data, was "solutions_builder-1.17.6.tar", max compression
```

## Comparing `solutions_builder-1.17.5.tar` & `solutions_builder-1.17.6.tar`

### file list

```diff
@@ -1,202 +1,202 @@
--rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.17.5/LICENSE
--rw-r--r--   0        0        0     4828 2023-07-31 15:22:50.618546 solutions_builder-1.17.5/README.md
--rw-r--r--   0        0        0     1150 2023-07-31 21:28:11.830879 solutions_builder-1.17.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622568 solutions_builder-1.17.5/solutions_builder/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622645 solutions_builder-1.17.5/solutions_builder/cli/__init__.py
--rw-r--r--   0        0        0     6551 2023-07-31 21:20:56.712072 solutions_builder-1.17.5/solutions_builder/cli/cli.py
--rw-r--r--   0        0        0     4630 2023-07-31 19:26:47.632344 solutions_builder-1.17.5/solutions_builder/cli/cli_utils.py
--rw-r--r--   0        0        0     6527 2023-07-31 21:28:04.069345 solutions_builder-1.17.5/solutions_builder/cli/component.py
--rw-r--r--   0        0        0     5883 2023-07-31 19:26:47.633561 solutions_builder-1.17.5/solutions_builder/cli/infra.py
--rw-r--r--   0        0        0     2313 2023-07-31 19:26:47.634344 solutions_builder-1.17.5/solutions_builder/cli/set.py
--rw-r--r--   0        0        0     1416 2023-07-31 19:26:06.133259 solutions_builder-1.17.5/solutions_builder/cli/template.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.624032 solutions_builder-1.17.5/solutions_builder/copier_extensions/__init__.py
--rw-r--r--   0        0        0     4617 2023-07-31 19:26:47.636088 solutions_builder-1.17.5/solutions_builder/copier_extensions/st_helpers.py
--rw-r--r--   0        0        0      101 2023-07-31 15:22:50.624510 solutions_builder-1.17.5/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
--rw-r--r--   0        0        0      766 2023-07-31 15:22:50.624649 solutions_builder-1.17.5/solutions_builder/module_template/README.md
--rw-r--r--   0        0        0      865 2023-07-31 15:22:50.624799 solutions_builder-1.17.5/solutions_builder/module_template/copier.yaml
--rw-r--r--   0        0        0       89 2023-07-31 15:22:50.625018 solutions_builder-1.17.5/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
--rw-r--r--   0        0        0     1135 2023-07-31 15:22:50.625172 solutions_builder-1.17.5/solutions_builder/module_template/template_copier.yaml
--rw-r--r--   0        0        0     3878 2023-07-31 19:26:06.134447 solutions_builder-1.17.5/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
--rw-r--r--   0        0        0      566 2023-07-31 15:22:50.625671 solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
--rw-r--r--   0        0        0      109 2023-07-31 15:22:50.625798 solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
--rw-r--r--   0        0        0     3204 2023-07-31 15:22:50.625960 solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
--rw-r--r--   0        0        0      590 2023-07-31 19:26:06.135288 solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.626261 solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
--rw-r--r--   0        0        0      736 2023-07-31 19:26:06.135779 solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
--rw-r--r--   0        0        0      636 2023-07-31 19:26:06.136084 solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
--rw-r--r--   0        0        0      836 2023-07-31 19:26:06.136404 solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
--rw-r--r--   0        0        0      777 2023-07-31 19:26:06.137072 solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
--rw-r--r--   0        0        0      858 2023-07-31 19:26:06.137649 solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.627394 solutions_builder-1.17.5/solutions_builder/modules/restful_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1363 2023-07-31 15:22:50.627536 solutions_builder-1.17.5/solutions_builder/modules/restful_service/README.md
--rw-r--r--   0        0        0      545 2023-07-31 15:22:50.627695 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1257 2023-07-31 15:22:50.628306 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.628605 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.628881 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0       98 2023-07-31 15:22:50.629046 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     2974 2023-07-31 15:22:50.629209 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      862 2023-07-31 19:26:06.138139 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1711 2023-07-31 19:26:06.138427 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1664 2023-07-31 19:26:06.138760 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.629799 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3876 2023-07-31 19:26:06.139176 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
--rw-r--r--   0        0        0     1222 2023-07-31 19:26:06.139854 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.630283 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.630545 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-07-31 15:22:50.630703 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2023-07-31 15:22:50.630849 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-07-31 15:22:50.630997 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-07-31 15:22:50.631183 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-07-31 15:22:50.631328 solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2305 2023-07-31 19:26:47.637120 solutions_builder-1.17.5/solutions_builder/modules/restful_service/copier.yaml
--rw-r--r--   0        0        0      120 2023-07-31 15:22:50.631626 solutions_builder-1.17.5/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-07-31 15:22:50.631734 solutions_builder-1.17.5/solutions_builder/modules/restful_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      263 2023-07-31 15:22:50.631945 solutions_builder-1.17.5/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
--rw-r--r--   0        0        0     3223 2023-07-31 15:22:50.632152 solutions_builder-1.17.5/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
--rw-r--r--   0        0        0     3269 2023-07-31 15:22:50.632352 solutions_builder-1.17.5/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.632549 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1572 2023-07-31 15:22:50.632676 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/README.md
--rw-r--r--   0        0        0      545 2023-07-31 15:22:50.632822 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.632992 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.633061 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      143 2023-07-31 15:22:50.633183 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3193 2023-07-31 15:22:50.633333 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      942 2023-07-31 19:26:06.140161 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1751 2023-07-31 19:26:06.140436 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1550 2023-07-31 19:26:06.140868 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.633781 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     5195 2023-07-31 19:26:06.141312 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
--rw-r--r--   0        0        0     1196 2023-07-31 19:26:06.141730 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634163 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634237 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
--rw-r--r--   0        0        0      430 2023-07-31 15:22:50.634359 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
--rw-r--r--   0        0        0     1348 2023-07-31 15:22:50.634473 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
--rw-r--r--   0        0        0     1138 2023-07-31 15:22:50.634593 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
--rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.634791 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-07-31 15:22:50.634913 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       97 2023-07-31 15:22:50.635030 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-07-31 15:22:50.635163 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-07-31 15:22:50.635357 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-07-31 15:22:50.635506 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2667 2023-07-31 15:22:50.635659 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/copier.yaml
--rw-r--r--   0        0        0       71 2023-07-31 15:22:50.635866 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-07-31 15:22:50.635986 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      719 2023-07-31 19:26:06.142418 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
--rw-r--r--   0        0        0     2693 2023-07-31 19:26:06.142972 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
--rw-r--r--   0        0        0      930 2023-07-31 19:26:06.143419 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
--rw-r--r--   0        0        0     1280 2023-07-31 19:26:06.143751 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
--rw-r--r--   0        0        0     2076 2023-07-31 19:26:06.144059 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
--rw-r--r--   0        0        0     3851 2023-07-31 19:26:06.144531 solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.637527 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1398 2023-07-31 21:24:12.019665 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/copier.yaml
--rw-r--r--   0        0        0      794 2023-07-31 15:22:50.637941 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       63 2023-07-31 15:22:50.638097 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/skaffold.yaml.patch
--rw-r--r--   0        0        0      701 2023-07-31 19:26:06.144964 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.145601 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf
--rw-r--r--   0        0        0     2486 2023-07-31 19:26:06.145978 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf
--rw-r--r--   0        0        0     1783 2023-07-31 19:26:06.146393 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf
--rw-r--r--   0        0        0      268 2023-07-31 15:22:50.639380 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
--rw-r--r--   0        0        0     1553 2023-07-31 19:26:06.146871 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.641148 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     2186 2023-07-31 19:26:47.638488 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/copier.yaml
--rw-r--r--   0        0        0      180 2023-07-31 15:22:50.641792 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
--rw-r--r--   0        0        0      658 2023-07-31 15:22:50.641933 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
--rw-r--r--   0        0        0      145 2023-07-31 15:22:50.642056 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
--rw-r--r--   0        0        0      185 2023-07-31 15:22:50.642172 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
--rw-r--r--   0        0        0      378 2023-07-31 15:22:50.642293 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
--rw-r--r--   0        0        0       59 2023-07-31 15:22:50.642402 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
--rw-r--r--   0        0        0     2420 2023-07-31 19:26:06.147317 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
--rw-r--r--   0        0        0      670 2023-07-31 19:26:06.147738 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
--rw-r--r--   0        0        0     1264 2023-07-31 19:26:06.148024 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
--rw-r--r--   0        0        0      709 2023-07-31 19:26:06.148386 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.148713 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
--rw-r--r--   0        0        0     1695 2023-07-31 19:26:06.149003 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
--rw-r--r--   0        0        0     1877 2023-07-31 19:26:06.149312 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
--rw-r--r--   0        0        0      480 2023-07-31 15:22:50.643659 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
--rw-r--r--   0        0        0     1802 2023-07-31 19:26:06.149801 solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.644034 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1048 2023-07-31 19:26:47.639062 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
--rw-r--r--   0        0        0      834 2023-07-31 19:26:06.150138 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
--rw-r--r--   0        0        0     2760 2023-07-31 15:22:50.644547 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
--rw-r--r--   0        0        0      670 2023-07-31 19:26:06.150553 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
--rw-r--r--   0        0        0     1298 2023-07-31 19:26:06.151001 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.644903 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
--rw-r--r--   0        0        0      196 2023-07-31 15:22:50.645021 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
--rw-r--r--   0        0        0     1984 2023-07-31 19:26:06.151475 solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
--rw-r--r--   0        0        0       90 2023-07-31 15:22:50.645285 solutions_builder-1.17.5/solutions_builder/requirements.txt
--rw-r--r--   0        0        0    68957 2023-07-31 15:22:50.645771 solutions_builder-1.17.5/solutions_builder/template_root/.github/assets/setup_local.png
--rw-r--r--   0        0        0   239307 2023-07-31 15:22:50.647206 solutions_builder-1.17.5/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
--rw-r--r--   0        0        0     2639 2023-07-31 15:22:50.647454 solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
--rw-r--r--   0        0        0     2690 2023-07-31 15:22:50.647592 solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
--rw-r--r--   0        0        0     5786 2023-07-31 19:26:47.639716 solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
--rw-r--r--   0        0        0     8049 2023-07-31 19:26:47.640169 solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
--rw-r--r--   0        0        0     3131 2023-07-31 15:22:50.648490 solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
--rw-r--r--   0        0        0      471 2023-07-31 15:22:50.648622 solutions_builder-1.17.5/solutions_builder/template_root/.gitignore
--rw-r--r--   0        0        0    14552 2023-07-31 15:22:50.648747 solutions_builder-1.17.5/solutions_builder/template_root/.pylintrc
--rw-r--r--   0        0        0      711 2023-07-31 15:22:50.649129 solutions_builder-1.17.5/solutions_builder/template_root/README.md
--rw-r--r--   0        0        0      398 2023-07-31 15:22:50.649329 solutions_builder-1.17.5/solutions_builder/template_root/components/README.md
--rw-r--r--   0        0        0      211 2023-07-31 15:22:50.649479 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
--rw-r--r--   0        0        0      395 2023-07-31 15:22:50.649633 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.649720 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
--rw-r--r--   0        0        0      131 2023-07-31 15:22:50.649904 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
--rw-r--r--   0        0        0      571 2023-07-31 15:22:50.650164 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.650248 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
--rw-r--r--   0        0        0      831 2023-07-31 19:26:06.151862 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
--rw-r--r--   0        0        0      695 2023-07-31 19:26:06.153743 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
--rw-r--r--   0        0        0       35 2023-07-31 15:22:50.650730 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
--rw-r--r--   0        0        0       91 2023-07-31 15:22:50.650873 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
--rw-r--r--   0        0        0     1376 2023-07-31 19:26:06.154070 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651072 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
--rw-r--r--   0        0        0      754 2023-07-31 19:26:06.154613 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
--rw-r--r--   0        0        0     1006 2023-07-31 19:26:06.155093 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
--rw-r--r--   0        0        0     2243 2023-07-31 19:26:06.155755 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651579 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
--rw-r--r--   0        0        0     1002 2023-07-31 19:26:06.156062 solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
--rw-r--r--   0        0        0     2130 2023-07-31 15:22:50.651893 solutions_builder-1.17.5/solutions_builder/template_root/copier.yaml
--rw-r--r--   0        0        0       97 2023-07-31 15:22:50.652011 solutions_builder-1.17.5/solutions_builder/template_root/firebase.json
--rw-r--r--   0        0        0       98 2023-07-31 15:22:50.652089 solutions_builder-1.17.5/solutions_builder/template_root/setup.cfg
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.652207 solutions_builder-1.17.5/solutions_builder/template_root/skaffold.yaml
--rw-r--r--   0        0        0      359 2023-07-31 15:22:50.652564 solutions_builder-1.17.5/solutions_builder/template_root/st.yaml
--rw-r--r--   0        0        0      921 2023-07-31 19:26:06.156495 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
--rw-r--r--   0        0        0      730 2023-07-31 19:26:06.157029 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
--rw-r--r--   0        0        0     3585 2023-07-31 19:26:06.157569 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
--rw-r--r--   0        0        0     1178 2023-07-31 19:26:06.158072 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
--rw-r--r--   0        0        0     5024 2023-07-31 19:26:06.158367 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
--rw-r--r--   0        0        0      190 2023-07-31 15:22:50.653603 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
--rw-r--r--   0        0        0     1186 2023-07-31 19:26:06.158842 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
--rw-r--r--   0        0        0     1601 2023-07-31 19:26:06.159185 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
--rw-r--r--   0        0        0     2364 2023-07-31 19:26:06.159491 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/firebase/main.tf
--rw-r--r--   0        0        0     1194 2023-07-31 19:26:06.160029 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/firebase/variables.tf
--rw-r--r--   0        0        0     3860 2023-07-31 19:26:06.160499 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/gke/main.tf
--rw-r--r--   0        0        0      832 2023-07-31 19:26:06.160786 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/gke/outputs.tf
--rw-r--r--   0        0        0     3386 2023-07-31 19:26:06.161064 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/gke/variables.tf
--rw-r--r--   0        0        0     2926 2023-07-31 19:26:06.161342 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
--rw-r--r--   0        0        0      692 2023-07-31 19:26:06.161609 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
--rw-r--r--   0        0        0     1087 2023-07-31 19:26:06.161883 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
--rw-r--r--   0        0        0      827 2023-07-31 19:26:06.162157 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/project_services/main.tf
--rw-r--r--   0        0        0      774 2023-07-31 19:26:06.162534 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/project_services/variables.tf
--rw-r--r--   0        0        0      953 2023-07-31 19:26:06.162825 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/service_account/main.tf
--rw-r--r--   0        0        0     1037 2023-07-31 19:26:06.163149 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/service_account/variables.tf
--rw-r--r--   0        0        0     1529 2023-07-31 19:26:06.163558 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
--rw-r--r--   0        0        0      678 2023-07-31 19:26:06.163969 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
--rw-r--r--   0        0        0     1333 2023-07-31 19:26:06.164360 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
--rw-r--r--   0        0        0     1269 2023-07-31 19:26:06.164825 solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
--rw-r--r--   0        0        0     2306 2023-07-31 19:39:45.308006 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
--rw-r--r--   0        0        0      730 2023-07-31 19:26:06.165370 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
--rw-r--r--   0        0        0       66 2023-07-31 15:22:50.656645 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
--rw-r--r--   0        0        0     1071 2023-07-31 19:26:06.165664 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
--rw-r--r--   0        0        0      826 2023-07-31 19:26:06.166236 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
--rw-r--r--   0        0        0      517 2023-07-31 15:22:50.657065 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.166512 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
--rw-r--r--   0        0        0     4400 2023-07-31 19:26:06.167078 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
--rw-r--r--   0        0        0      991 2023-07-31 19:26:06.167766 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
--rw-r--r--   0        0        0      835 2023-07-31 19:26:06.168129 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
--rw-r--r--   0        0        0      606 2023-07-31 15:22:50.657649 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
--rw-r--r--   0        0        0     2546 2023-07-31 19:26:06.168711 solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.657846 solutions_builder-1.17.5/solutions_builder/template_root/tests/__init__.py
--rw-r--r--   0        0        0      825 2023-07-31 15:22:50.658012 solutions_builder-1.17.5/solutions_builder/template_root/tests/e2e/e2e_utils.py
--rwxr-xr-x   0        0        0      364 2023-07-31 15:22:50.658190 solutions_builder-1.17.5/solutions_builder/template_root/utils/disable_org_policies.sh
--rwxr-xr-x   0        0        0      990 2023-07-31 19:26:06.169251 solutions_builder-1.17.5/solutions_builder/template_root/utils/init_env_vars.sh
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.658645 solutions_builder-1.17.5/solutions_builder/template_root/{{_copier_conf.answers_file}}
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.658746 solutions_builder-1.17.5/solutions_builder/tests/__init__.py
--rw-r--r--   0        0        0     5942 1970-01-01 00:00:00.000000 solutions_builder-1.17.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.17.6/LICENSE
+-rw-r--r--   0        0        0     4828 2023-07-31 15:22:50.618546 solutions_builder-1.17.6/README.md
+-rw-r--r--   0        0        0     1150 2023-07-31 21:38:15.340949 solutions_builder-1.17.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622568 solutions_builder-1.17.6/solutions_builder/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622645 solutions_builder-1.17.6/solutions_builder/cli/__init__.py
+-rw-r--r--   0        0        0     6551 2023-07-31 21:20:56.712072 solutions_builder-1.17.6/solutions_builder/cli/cli.py
+-rw-r--r--   0        0        0     4630 2023-07-31 19:26:47.632344 solutions_builder-1.17.6/solutions_builder/cli/cli_utils.py
+-rw-r--r--   0        0        0     6527 2023-07-31 21:28:04.069345 solutions_builder-1.17.6/solutions_builder/cli/component.py
+-rw-r--r--   0        0        0     5883 2023-07-31 19:26:47.633561 solutions_builder-1.17.6/solutions_builder/cli/infra.py
+-rw-r--r--   0        0        0     2313 2023-07-31 19:26:47.634344 solutions_builder-1.17.6/solutions_builder/cli/set.py
+-rw-r--r--   0        0        0     1416 2023-07-31 19:26:06.133259 solutions_builder-1.17.6/solutions_builder/cli/template.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.624032 solutions_builder-1.17.6/solutions_builder/copier_extensions/__init__.py
+-rw-r--r--   0        0        0     4617 2023-07-31 19:26:47.636088 solutions_builder-1.17.6/solutions_builder/copier_extensions/st_helpers.py
+-rw-r--r--   0        0        0      101 2023-07-31 15:22:50.624510 solutions_builder-1.17.6/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
+-rw-r--r--   0        0        0      766 2023-07-31 15:22:50.624649 solutions_builder-1.17.6/solutions_builder/module_template/README.md
+-rw-r--r--   0        0        0      865 2023-07-31 15:22:50.624799 solutions_builder-1.17.6/solutions_builder/module_template/copier.yaml
+-rw-r--r--   0        0        0       89 2023-07-31 15:22:50.625018 solutions_builder-1.17.6/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
+-rw-r--r--   0        0        0     1135 2023-07-31 15:22:50.625172 solutions_builder-1.17.6/solutions_builder/module_template/template_copier.yaml
+-rw-r--r--   0        0        0     3878 2023-07-31 19:26:06.134447 solutions_builder-1.17.6/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
+-rw-r--r--   0        0        0      566 2023-07-31 15:22:50.625671 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
+-rw-r--r--   0        0        0      109 2023-07-31 15:22:50.625798 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
+-rw-r--r--   0        0        0     3204 2023-07-31 15:22:50.625960 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
+-rw-r--r--   0        0        0      590 2023-07-31 19:26:06.135288 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.626261 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
+-rw-r--r--   0        0        0      736 2023-07-31 19:26:06.135779 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
+-rw-r--r--   0        0        0      636 2023-07-31 19:26:06.136084 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
+-rw-r--r--   0        0        0      836 2023-07-31 19:26:06.136404 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
+-rw-r--r--   0        0        0      777 2023-07-31 19:26:06.137072 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
+-rw-r--r--   0        0        0      858 2023-07-31 19:26:06.137649 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.627394 solutions_builder-1.17.6/solutions_builder/modules/restful_service/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1363 2023-07-31 15:22:50.627536 solutions_builder-1.17.6/solutions_builder/modules/restful_service/README.md
+-rw-r--r--   0        0        0      545 2023-07-31 15:22:50.627695 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1257 2023-07-31 15:22:50.628306 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.628605 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.628881 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0       98 2023-07-31 15:22:50.629046 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     2974 2023-07-31 15:22:50.629209 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      862 2023-07-31 19:26:06.138139 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1711 2023-07-31 19:26:06.138427 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1664 2023-07-31 19:26:06.138760 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.629799 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     3876 2023-07-31 19:26:06.139176 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
+-rw-r--r--   0        0        0     1222 2023-07-31 19:26:06.139854 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.630283 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.630545 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-07-31 15:22:50.630703 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2023-07-31 15:22:50.630849 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-07-31 15:22:50.630997 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-07-31 15:22:50.631183 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-07-31 15:22:50.631328 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2305 2023-07-31 19:26:47.637120 solutions_builder-1.17.6/solutions_builder/modules/restful_service/copier.yaml
+-rw-r--r--   0        0        0      120 2023-07-31 15:22:50.631626 solutions_builder-1.17.6/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2023-07-31 15:22:50.631734 solutions_builder-1.17.6/solutions_builder/modules/restful_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      263 2023-07-31 15:22:50.631945 solutions_builder-1.17.6/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
+-rw-r--r--   0        0        0     3223 2023-07-31 15:22:50.632152 solutions_builder-1.17.6/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
+-rw-r--r--   0        0        0     3269 2023-07-31 15:22:50.632352 solutions_builder-1.17.6/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.632549 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1572 2023-07-31 15:22:50.632676 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/README.md
+-rw-r--r--   0        0        0      545 2023-07-31 15:22:50.632822 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.632992 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.633061 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0      143 2023-07-31 15:22:50.633183 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     3193 2023-07-31 15:22:50.633333 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      942 2023-07-31 19:26:06.140161 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1751 2023-07-31 19:26:06.140436 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1550 2023-07-31 19:26:06.140868 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.633781 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     5195 2023-07-31 19:26:06.141312 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
+-rw-r--r--   0        0        0     1196 2023-07-31 19:26:06.141730 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634163 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634237 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-31 15:22:50.634359 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
+-rw-r--r--   0        0        0     1348 2023-07-31 15:22:50.634473 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
+-rw-r--r--   0        0        0     1138 2023-07-31 15:22:50.634593 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
+-rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.634791 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-07-31 15:22:50.634913 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       97 2023-07-31 15:22:50.635030 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-07-31 15:22:50.635163 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-07-31 15:22:50.635357 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-07-31 15:22:50.635506 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2667 2023-07-31 15:22:50.635659 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/copier.yaml
+-rw-r--r--   0        0        0       71 2023-07-31 15:22:50.635866 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2023-07-31 15:22:50.635986 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      719 2023-07-31 19:26:06.142418 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
+-rw-r--r--   0        0        0     2693 2023-07-31 19:26:06.142972 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
+-rw-r--r--   0        0        0      930 2023-07-31 19:26:06.143419 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
+-rw-r--r--   0        0        0     1280 2023-07-31 19:26:06.143751 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
+-rw-r--r--   0        0        0     2076 2023-07-31 19:26:06.144059 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
+-rw-r--r--   0        0        0     3851 2023-07-31 19:26:06.144531 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.637527 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1398 2023-07-31 21:24:12.019665 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/copier.yaml
+-rw-r--r--   0        0        0      794 2023-07-31 15:22:50.637941 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       59 2023-07-31 21:38:07.061173 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/skaffold.yaml.patch
+-rw-r--r--   0        0        0      701 2023-07-31 19:26:06.144964 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.145601 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf
+-rw-r--r--   0        0        0     2486 2023-07-31 19:26:06.145978 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf
+-rw-r--r--   0        0        0     1783 2023-07-31 19:26:06.146393 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf
+-rw-r--r--   0        0        0      268 2023-07-31 15:22:50.639380 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
+-rw-r--r--   0        0        0     1553 2023-07-31 19:26:06.146871 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.641148 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     2186 2023-07-31 19:26:47.638488 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/copier.yaml
+-rw-r--r--   0        0        0      180 2023-07-31 15:22:50.641792 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
+-rw-r--r--   0        0        0      658 2023-07-31 15:22:50.641933 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
+-rw-r--r--   0        0        0      145 2023-07-31 15:22:50.642056 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
+-rw-r--r--   0        0        0      185 2023-07-31 15:22:50.642172 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
+-rw-r--r--   0        0        0      378 2023-07-31 15:22:50.642293 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
+-rw-r--r--   0        0        0       59 2023-07-31 15:22:50.642402 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
+-rw-r--r--   0        0        0     2420 2023-07-31 19:26:06.147317 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
+-rw-r--r--   0        0        0      670 2023-07-31 19:26:06.147738 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
+-rw-r--r--   0        0        0     1264 2023-07-31 19:26:06.148024 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
+-rw-r--r--   0        0        0      709 2023-07-31 19:26:06.148386 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.148713 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
+-rw-r--r--   0        0        0     1695 2023-07-31 19:26:06.149003 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
+-rw-r--r--   0        0        0     1877 2023-07-31 19:26:06.149312 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
+-rw-r--r--   0        0        0      480 2023-07-31 15:22:50.643659 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
+-rw-r--r--   0        0        0     1802 2023-07-31 19:26:06.149801 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.644034 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1048 2023-07-31 19:26:47.639062 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
+-rw-r--r--   0        0        0      834 2023-07-31 19:26:06.150138 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
+-rw-r--r--   0        0        0     2760 2023-07-31 15:22:50.644547 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
+-rw-r--r--   0        0        0      670 2023-07-31 19:26:06.150553 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
+-rw-r--r--   0        0        0     1298 2023-07-31 19:26:06.151001 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.644903 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
+-rw-r--r--   0        0        0      196 2023-07-31 15:22:50.645021 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
+-rw-r--r--   0        0        0     1984 2023-07-31 19:26:06.151475 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
+-rw-r--r--   0        0        0       90 2023-07-31 15:22:50.645285 solutions_builder-1.17.6/solutions_builder/requirements.txt
+-rw-r--r--   0        0        0    68957 2023-07-31 15:22:50.645771 solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/setup_local.png
+-rw-r--r--   0        0        0   239307 2023-07-31 15:22:50.647206 solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
+-rw-r--r--   0        0        0     2639 2023-07-31 15:22:50.647454 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
+-rw-r--r--   0        0        0     2690 2023-07-31 15:22:50.647592 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
+-rw-r--r--   0        0        0     5786 2023-07-31 19:26:47.639716 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
+-rw-r--r--   0        0        0     8049 2023-07-31 19:26:47.640169 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
+-rw-r--r--   0        0        0     3131 2023-07-31 15:22:50.648490 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
+-rw-r--r--   0        0        0      471 2023-07-31 15:22:50.648622 solutions_builder-1.17.6/solutions_builder/template_root/.gitignore
+-rw-r--r--   0        0        0    14552 2023-07-31 15:22:50.648747 solutions_builder-1.17.6/solutions_builder/template_root/.pylintrc
+-rw-r--r--   0        0        0      711 2023-07-31 15:22:50.649129 solutions_builder-1.17.6/solutions_builder/template_root/README.md
+-rw-r--r--   0        0        0      398 2023-07-31 15:22:50.649329 solutions_builder-1.17.6/solutions_builder/template_root/components/README.md
+-rw-r--r--   0        0        0      211 2023-07-31 15:22:50.649479 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
+-rw-r--r--   0        0        0      395 2023-07-31 15:22:50.649633 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.649720 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
+-rw-r--r--   0        0        0      131 2023-07-31 15:22:50.649904 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
+-rw-r--r--   0        0        0      571 2023-07-31 15:22:50.650164 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.650248 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
+-rw-r--r--   0        0        0      831 2023-07-31 19:26:06.151862 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
+-rw-r--r--   0        0        0      695 2023-07-31 19:26:06.153743 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
+-rw-r--r--   0        0        0       35 2023-07-31 15:22:50.650730 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
+-rw-r--r--   0        0        0       91 2023-07-31 15:22:50.650873 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
+-rw-r--r--   0        0        0     1376 2023-07-31 19:26:06.154070 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651072 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
+-rw-r--r--   0        0        0      754 2023-07-31 19:26:06.154613 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
+-rw-r--r--   0        0        0     1006 2023-07-31 19:26:06.155093 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
+-rw-r--r--   0        0        0     2243 2023-07-31 19:26:06.155755 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651579 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-31 19:26:06.156062 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
+-rw-r--r--   0        0        0     2130 2023-07-31 15:22:50.651893 solutions_builder-1.17.6/solutions_builder/template_root/copier.yaml
+-rw-r--r--   0        0        0       97 2023-07-31 15:22:50.652011 solutions_builder-1.17.6/solutions_builder/template_root/firebase.json
+-rw-r--r--   0        0        0       98 2023-07-31 15:22:50.652089 solutions_builder-1.17.6/solutions_builder/template_root/setup.cfg
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.652207 solutions_builder-1.17.6/solutions_builder/template_root/skaffold.yaml
+-rw-r--r--   0        0        0      359 2023-07-31 15:22:50.652564 solutions_builder-1.17.6/solutions_builder/template_root/st.yaml
+-rw-r--r--   0        0        0      921 2023-07-31 19:26:06.156495 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
+-rw-r--r--   0        0        0      730 2023-07-31 19:26:06.157029 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
+-rw-r--r--   0        0        0     3585 2023-07-31 19:26:06.157569 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
+-rw-r--r--   0        0        0     1178 2023-07-31 19:26:06.158072 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
+-rw-r--r--   0        0        0     5024 2023-07-31 19:26:06.158367 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
+-rw-r--r--   0        0        0      190 2023-07-31 15:22:50.653603 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
+-rw-r--r--   0        0        0     1186 2023-07-31 19:26:06.158842 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
+-rw-r--r--   0        0        0     1601 2023-07-31 19:26:06.159185 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
+-rw-r--r--   0        0        0     2364 2023-07-31 19:26:06.159491 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/main.tf
+-rw-r--r--   0        0        0     1194 2023-07-31 19:26:06.160029 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/variables.tf
+-rw-r--r--   0        0        0     3860 2023-07-31 19:26:06.160499 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/main.tf
+-rw-r--r--   0        0        0      832 2023-07-31 19:26:06.160786 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/outputs.tf
+-rw-r--r--   0        0        0     3386 2023-07-31 19:26:06.161064 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/variables.tf
+-rw-r--r--   0        0        0     2926 2023-07-31 19:26:06.161342 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
+-rw-r--r--   0        0        0      692 2023-07-31 19:26:06.161609 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
+-rw-r--r--   0        0        0     1087 2023-07-31 19:26:06.161883 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
+-rw-r--r--   0        0        0      827 2023-07-31 19:26:06.162157 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/main.tf
+-rw-r--r--   0        0        0      774 2023-07-31 19:26:06.162534 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/variables.tf
+-rw-r--r--   0        0        0      953 2023-07-31 19:26:06.162825 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/main.tf
+-rw-r--r--   0        0        0     1037 2023-07-31 19:26:06.163149 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/variables.tf
+-rw-r--r--   0        0        0     1529 2023-07-31 19:26:06.163558 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
+-rw-r--r--   0        0        0      678 2023-07-31 19:26:06.163969 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
+-rw-r--r--   0        0        0     1333 2023-07-31 19:26:06.164360 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
+-rw-r--r--   0        0        0     1269 2023-07-31 19:26:06.164825 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
+-rw-r--r--   0        0        0     2306 2023-07-31 19:39:45.308006 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
+-rw-r--r--   0        0        0      730 2023-07-31 19:26:06.165370 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
+-rw-r--r--   0        0        0       66 2023-07-31 15:22:50.656645 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
+-rw-r--r--   0        0        0     1071 2023-07-31 19:26:06.165664 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
+-rw-r--r--   0        0        0      826 2023-07-31 19:26:06.166236 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
+-rw-r--r--   0        0        0      517 2023-07-31 15:22:50.657065 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.166512 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
+-rw-r--r--   0        0        0     4400 2023-07-31 19:26:06.167078 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
+-rw-r--r--   0        0        0      991 2023-07-31 19:26:06.167766 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
+-rw-r--r--   0        0        0      835 2023-07-31 19:26:06.168129 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
+-rw-r--r--   0        0        0      606 2023-07-31 15:22:50.657649 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
+-rw-r--r--   0        0        0     2546 2023-07-31 19:26:06.168711 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.657846 solutions_builder-1.17.6/solutions_builder/template_root/tests/__init__.py
+-rw-r--r--   0        0        0      825 2023-07-31 15:22:50.658012 solutions_builder-1.17.6/solutions_builder/template_root/tests/e2e/e2e_utils.py
+-rwxr-xr-x   0        0        0      364 2023-07-31 15:22:50.658190 solutions_builder-1.17.6/solutions_builder/template_root/utils/disable_org_policies.sh
+-rwxr-xr-x   0        0        0      990 2023-07-31 19:26:06.169251 solutions_builder-1.17.6/solutions_builder/template_root/utils/init_env_vars.sh
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.658645 solutions_builder-1.17.6/solutions_builder/template_root/{{_copier_conf.answers_file}}
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.658746 solutions_builder-1.17.6/solutions_builder/tests/__init__.py
+-rw-r--r--   0        0        0     5942 1970-01-01 00:00:00.000000 solutions_builder-1.17.6/PKG-INFO
```

### Comparing `solutions_builder-1.17.5/LICENSE` & `solutions_builder-1.17.6/LICENSE`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/README.md` & `solutions_builder-1.17.6/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/pyproject.toml` & `solutions_builder-1.17.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solutions-builder"
-version = "1.17.5"
+version = "1.17.6"
 description = "A solution framework to generate a project with built-in structure and modules"
 authors = ["Jon Chen <jonchen@google.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/GoogleCloudPlatform/solutions-builder"
 repository = "https://github.com/GoogleCloudPlatform/solutions-builder"
 packages = [
```

### Comparing `solutions_builder-1.17.5/solutions_builder/cli/cli.py` & `solutions_builder-1.17.6/solutions_builder/cli/cli.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/cli/cli_utils.py` & `solutions_builder-1.17.6/solutions_builder/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/cli/component.py` & `solutions_builder-1.17.6/solutions_builder/cli/component.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/cli/infra.py` & `solutions_builder-1.17.6/solutions_builder/cli/infra.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/cli/set.py` & `solutions_builder-1.17.6/solutions_builder/cli/set.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/cli/template.py` & `solutions_builder-1.17.6/solutions_builder/cli/template.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/copier_extensions/st_helpers.py` & `solutions_builder-1.17.6/solutions_builder/copier_extensions/st_helpers.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/README.md` & `solutions_builder-1.17.6/solutions_builder/module_template/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/copier.yaml` & `solutions_builder-1.17.6/solutions_builder/module_template/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/template_copier.yaml` & `solutions_builder-1.17.6/solutions_builder/module_template/template_copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml` & `solutions_builder-1.17.6/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf` & `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/README.md` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/README.md` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/copier.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/README.md` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/copier.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/copier.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/copier.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf` & `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.github/assets/setup_local.png` & `solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/setup_local.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png` & `solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml` & `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml` & `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml` & `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml` & `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml` & `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/.pylintrc` & `solutions_builder-1.17.6/solutions_builder/template_root/.pylintrc`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/README.md` & `solutions_builder-1.17.6/solutions_builder/template_root/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py` & `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/copier.yaml` & `solutions_builder-1.17.6/solutions_builder/template_root/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudrun/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/compute_backend/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/firebase/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/firebase/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/gke/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/gke/outputs.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/gke/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/project_services/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/project_services/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/service_account/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/service_account/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/vpc_network/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/main.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf` & `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/tests/e2e/e2e_utils.py` & `solutions_builder-1.17.6/solutions_builder/template_root/tests/e2e/e2e_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/solutions_builder/template_root/utils/init_env_vars.sh` & `solutions_builder-1.17.6/solutions_builder/template_root/utils/init_env_vars.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.5/PKG-INFO` & `solutions_builder-1.17.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solutions-builder
-Version: 1.17.5
+Version: 1.17.6
 Summary: A solution framework to generate a project with built-in structure and modules
 Home-page: https://github.com/GoogleCloudPlatform/solutions-builder
 License: Apache
 Author: Jon Chen
 Author-email: jonchen@google.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

