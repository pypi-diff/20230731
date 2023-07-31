# Comparing `tmp/mlflow_knative-0.3.0.tar.gz` & `tmp/mlflow_knative-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_knative-0.3.0.tar", max compression
+gzip compressed data, was "mlflow_knative-0.4.1.tar", max compression
```

## Comparing `mlflow_knative-0.3.0.tar` & `mlflow_knative-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1085 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     5315 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/README.md
--rw-r--r--   0        0        0      526 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/__init__.py
--rw-r--r--   0        0        0    15767 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/deployment_client.py
--rw-r--r--   0        0        0     6330 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/knative.py
--rw-r--r--   0        0        0     2232 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/mlflow_docker.py
--rw-r--r--   0        0        0      808 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/service.yaml
--rw-r--r--   0        0        0     1089 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/templating.py
--rw-r--r--   0        0        0     1616 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6158 1970-01-01 00:00:00.000000 mlflow_knative-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     5794 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/README.md
+-rw-r--r--   0        0        0      526 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/mlflow_knative/__init__.py
+-rw-r--r--   0        0        0    17635 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/mlflow_knative/deployment_client.py
+-rw-r--r--   0        0        0     6330 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/mlflow_knative/knative.py
+-rw-r--r--   0        0        0     2232 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/mlflow_knative/mlflow_docker.py
+-rw-r--r--   0        0        0      808 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/mlflow_knative/service.yaml
+-rw-r--r--   0        0        0     1089 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/mlflow_knative/templating.py
+-rw-r--r--   0        0        0     1616 2023-07-31 15:28:21.000000 mlflow_knative-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6637 1970-01-01 00:00:00.000000 mlflow_knative-0.4.1/PKG-INFO
```

### Comparing `mlflow_knative-0.3.0/LICENSE.md` & `mlflow_knative-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.3.0/README.md` & `mlflow_knative-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 pip install mlflow-knative
 ```
 
 
 Getting Started
 ---------------
 
-A Kubernetes context is required to define the Knative target.  
+The plugin adds support for a `knative` target scheme to the [`mlflow deployments` CLI](https://mlflow.org/docs/latest/cli.html#mlflow-deployments).
+
+A [Kubernetes context](https://kubernetes.io/docs/tasks/access-application-cluster/configure-access-multiple-clusters/) is used to define the Knative target as `knative:/<context>`.  
 You can list available contexts with `kubectl config get-contexts`.
 
-Make sure Docker is running locally if you intend create or update a deployment, as this is required to build an image from the MLflow model.
+**Note:** Passing only the base `knative:/` (*context* omitted) as target lets the Kubernetes client pick a default configuration, which may be in-cluster. [Kubernetes *RBAC*](https://kubernetes.io/docs/reference/access-authn-authz/rbac/) must be configured to allow the pod running this deployment client to create, list, update and delete Knative services.
 
-The plugin adds support for a `knative` target scheme to the [`mlflow deployments` CLI](https://mlflow.org/docs/latest/cli.html#mlflow-deployments).
+Make sure Docker is running locally if you intend create or update a deployment, as this is required to build an image from the MLflow model.
 
 Setting the `image_repository` config key is required to make the Docker image of the model available for deployment by Knative. Additionally you may also provide an image tag with the `image_tag` config key (defaults to `latest`).
 
 ```console
 mlflow deployments create \
   --target knative:/<context> \
   --name <deployment-name> \
```

### Comparing `mlflow_knative-0.3.0/mlflow_knative/__init__.py` & `mlflow_knative-0.4.1/mlflow_knative/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.3.0/mlflow_knative/deployment_client.py` & `mlflow_knative-0.4.1/mlflow_knative/deployment_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """MLflow Knative Deployment Plugin.
 
 The plugin implements a MLflow deployment client for Knative targets
 as well as helper functions.
 
 Implementing: https://mlflow.org/docs/latest/_modules/mlflow/deployments/base.html
 """
+import importlib
 import logging
 import warnings
 from http import HTTPStatus
 
 import docker
 import kubernetes
 import mlflow
@@ -23,20 +24,26 @@
 IMAGE_REPOSITORY_CONFIG_KEY = "image_repository"
 IMAGE_TAG_CONFIG_KEY = "image_tag"
 DEFAULT_IMAGE_TAG = "latest"
 
 NAMESPACE_CONFIG_KEY = "namespace"
 DEFAULT_NAMESPACE = "default"
 RUN_ID_ANNOTATION = "knative.deployments.mlflow.org/run-id"
+MANAGED_BY_LABEL = "app.kubernetes.io/managed-by"
+DISTRIBUTION_NAME = importlib.metadata.distribution(__package__).name
 
 TEMPLATE_PATH_CONFIG_KEY = "service_template"
 
 logger = logging.getLogger(__package__)
 
 
+def _is_managed(service: dict) -> bool:
+    return service["metadata"]["labels"].get(MANAGED_BY_LABEL) == DISTRIBUTION_NAME
+
+
 class EndpointArgumentNotSupported(mlflow.exceptions.MlflowException):
     """Raised when the unsupported 'endpoint' argument is used."""
 
     def __init__(self):
         super().__init__(
             "'endpoint' argument not supported by Knative deployment plugin."
         )
@@ -44,16 +51,24 @@
 
 class KnativeDeploymentClient(mlflow.deployments.BaseDeploymentClient):
     """Knative Deployment Client for MLflow."""
 
     def __init__(self, uri: str):
         super().__init__(target_uri=uri)
         self._docker_client = docker.from_env()
-        self._kubernetes_client = kubernetes.config.new_client_from_config(
-            context=uri.removeprefix("knative:/")
+
+        # Use `load_config` to allow the client to fall back to in-cluster config
+        kubernetes_client_config = type.__call__(kubernetes.client.Configuration)
+        kubernetes.config.load_config(
+            client_configuration=kubernetes_client_config,
+            # Defaulting to `None` ensures `load_config` falls back to default behavior
+            context=uri.removeprefix("knative:/") or None,
+        )
+        self._kubernetes_client = kubernetes.client.ApiClient(
+            configuration=kubernetes_client_config
         )
 
     def create_deployment(
         self,
         name: str,
         model_uri: str,
         flavor: str | None = None,
@@ -94,16 +109,24 @@
             try:
                 body = get_service_body(
                     namespace=namespace,
                     name=name,
                     image=image,
                     template_path=config.get(TEMPLATE_PATH_CONFIG_KEY),
                 )
+
+                # Annotate the service with the MLflow run ID (used as cache key)
                 annotations = body["metadata"].setdefault("annotations", {})
                 annotations[RUN_ID_ANNOTATION] = model_info.run_id
+
+                # Label the service as managed by this plugin,
+                # which is meant to ignore unmanaged services.
+                labels = body["metadata"].setdefault("labels", {})
+                labels[MANAGED_BY_LABEL] = DISTRIBUTION_NAME
+
                 service = knative_api.create_namespaced_service(
                     namespace=namespace,
                     body=body,
                 )
             except kubernetes.client.rest.ApiException as error:
                 if error.status == HTTPStatus.CONFLICT:
                     raise mlflow.exceptions.MlflowException(
@@ -152,14 +175,21 @@
         with self._kubernetes_client as kubernetes_client:
             knative_api = KnativeServingV1Api(kubernetes_client)
             namespace = config.get(NAMESPACE_CONFIG_KEY, DEFAULT_NAMESPACE)
             try:
                 service = knative_api.get_namespaced_service(
                     namespace=namespace, name=name
                 )
+
+                if not _is_managed(service):
+                    raise mlflow.exceptions.MlflowException(
+                        f"deployment with name '{name}' in namespace '{namespace}' "
+                        f"is not managed by {DISTRIBUTION_NAME}, aborting."
+                    )
+
                 image = get_model_as_image(
                     self._docker_client,
                     model_uri,
                     repository=config[IMAGE_REPOSITORY_CONFIG_KEY],
                     tag=config.get(IMAGE_TAG_CONFIG_KEY, DEFAULT_IMAGE_TAG),
                     # Force image repository if the run ID doesn't match
                     force_update=service["metadata"]["annotations"].get(
@@ -211,14 +241,24 @@
 
         config = config if config is not None else {}
 
         with self._kubernetes_client as kubernetes_client:
             knative_api = KnativeServingV1Api(kubernetes_client)
             namespace = config.get(NAMESPACE_CONFIG_KEY, DEFAULT_NAMESPACE)
             try:
+                service = knative_api.get_namespaced_service(
+                    namespace=namespace, name=name
+                )
+
+                if not _is_managed(service):
+                    raise mlflow.exceptions.MlflowException(
+                        f"deployment with name '{name}' in namespace '{namespace}' "
+                        f"is not managed by {DISTRIBUTION_NAME}, aborting."
+                    )
+
                 knative_api.delete_namespaced_service(namespace=namespace, name=name)
             except kubernetes.client.rest.ApiException as error:
                 if error.status == HTTPStatus.NOT_FOUND:
                     raise mlflow.exceptions.MlflowException(
                         f"no deployment with name '{name}' "
                         f"found in namespace '{namespace}'."
                     )
@@ -247,14 +287,15 @@
                             RUN_ID_ANNOTATION
                         ),
                     }
                     for namespace in core_api.list_namespace().items
                     for service in knative_api.list_namespaced_service(
                         namespace=namespace.metadata.name
                     )["items"]
+                    if _is_managed(service)
                 ]
             except kubernetes.client.rest.ApiException as error:
                 raise mlflow.exceptions.MlflowException(
                     f"Kubernetes API error ({error.status})"
                 ) from error
 
     def get_deployment(self, name: str, endpoint: str | None = None) -> dict[str, str]:
@@ -274,28 +315,29 @@
 
             deployments = []
             for namespace in core_api.list_namespace().items:
                 try:
                     service = knative_api.get_namespaced_service(
                         namespace=namespace.metadata.name, name=name
                     )
-                    deployments.append(
-                        {
-                            "name": service["metadata"]["name"],
-                            "namespace": service["metadata"]["namespace"],
-                            "url": service["status"]["url"],
-                            "generation": service["metadata"]["generation"],
-                            "creation_timestamp": service["metadata"][
-                                "creationTimestamp"
-                            ],
-                            "run_id": service["metadata"]["annotations"].get(
-                                RUN_ID_ANNOTATION
-                            ),
-                        }
-                    )
+                    if _is_managed(service):
+                        deployments.append(
+                            {
+                                "name": service["metadata"]["name"],
+                                "namespace": service["metadata"]["namespace"],
+                                "url": service["status"]["url"],
+                                "generation": service["metadata"]["generation"],
+                                "creation_timestamp": service["metadata"][
+                                    "creationTimestamp"
+                                ],
+                                "run_id": service["metadata"]["annotations"].get(
+                                    RUN_ID_ANNOTATION
+                                ),
+                            }
+                        )
                 except kubernetes.client.rest.ApiException as error:
                     if error.status == HTTPStatus.NOT_FOUND:
                         pass
                     else:
                         raise mlflow.exceptions.MlflowException(
                             f"Kubernetes API error ({error.status})"
                         ) from error
```

### Comparing `mlflow_knative-0.3.0/mlflow_knative/knative.py` & `mlflow_knative-0.4.1/mlflow_knative/knative.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.3.0/mlflow_knative/mlflow_docker.py` & `mlflow_knative-0.4.1/mlflow_knative/mlflow_docker.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.3.0/mlflow_knative/service.yaml` & `mlflow_knative-0.4.1/mlflow_knative/service.yaml`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.3.0/mlflow_knative/templating.py` & `mlflow_knative-0.4.1/mlflow_knative/templating.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.3.0/pyproject.toml` & `mlflow_knative-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-knative"
-version = "0.3.0"
+version = "0.4.1"
 description = "MLflow plugin adding a Knative deployment target"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "deployment", "deployments", "knative", "kubernetes", "kn", "k8s"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
```

### Comparing `mlflow_knative-0.3.0/PKG-INFO` & `mlflow_knative-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-knative
-Version: 0.3.0
+Version: 0.4.1
 Summary: MLflow plugin adding a Knative deployment target
 Home-page: https://gitlab.com/lzinsou/mlflow-knative
 Keywords: mlflow,plugin,mlops,deployment,deployments,knative,kubernetes,kn,k8s
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -44,20 +44,22 @@
 pip install mlflow-knative
 ```
 
 
 Getting Started
 ---------------
 
-A Kubernetes context is required to define the Knative target.  
+The plugin adds support for a `knative` target scheme to the [`mlflow deployments` CLI](https://mlflow.org/docs/latest/cli.html#mlflow-deployments).
+
+A [Kubernetes context](https://kubernetes.io/docs/tasks/access-application-cluster/configure-access-multiple-clusters/) is used to define the Knative target as `knative:/<context>`.  
 You can list available contexts with `kubectl config get-contexts`.
 
-Make sure Docker is running locally if you intend create or update a deployment, as this is required to build an image from the MLflow model.
+**Note:** Passing only the base `knative:/` (*context* omitted) as target lets the Kubernetes client pick a default configuration, which may be in-cluster. [Kubernetes *RBAC*](https://kubernetes.io/docs/reference/access-authn-authz/rbac/) must be configured to allow the pod running this deployment client to create, list, update and delete Knative services.
 
-The plugin adds support for a `knative` target scheme to the [`mlflow deployments` CLI](https://mlflow.org/docs/latest/cli.html#mlflow-deployments).
+Make sure Docker is running locally if you intend create or update a deployment, as this is required to build an image from the MLflow model.
 
 Setting the `image_repository` config key is required to make the Docker image of the model available for deployment by Knative. Additionally you may also provide an image tag with the `image_tag` config key (defaults to `latest`).
 
 ```console
 mlflow deployments create \
   --target knative:/<context> \
   --name <deployment-name> \
```

