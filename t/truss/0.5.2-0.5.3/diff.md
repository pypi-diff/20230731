# Comparing `tmp/truss-0.5.2.tar.gz` & `tmp/truss-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.5.2.tar", max compression
+gzip compressed data, was "truss-0.5.3.tar", max compression
```

## Comparing `truss-0.5.2.tar` & `truss-0.5.3.tar`

### file list

```diff
@@ -1,217 +1,222 @@
--rw-r--r--   0        0        0     5483 2023-07-28 22:19:05.925630 truss-0.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2418 2023-07-28 22:19:05.925630 truss-0.5.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-07-28 22:19:05.925630 truss-0.5.2/LICENSE
--rw-r--r--   0        0        0     3518 2023-07-28 22:19:05.925630 truss-0.5.2/README.md
--rw-r--r--   0        0        0      933 2023-07-28 22:19:05.925630 truss-0.5.2/context_builder.Dockerfile
--rw-r--r--   0        0        0     2546 2023-07-28 22:19:06.033645 truss-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      330 2023-07-28 22:19:06.033645 truss-0.5.2/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-07-28 22:19:06.033645 truss-0.5.2/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-07-28 22:19:06.033645 truss-0.5.2/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-07-28 22:19:06.033645 truss-0.5.2/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13068 2023-07-28 22:19:06.033645 truss-0.5.2/truss/build.py
--rw-r--r--   0        0        0    11216 2023-07-28 22:19:06.033645 truss-0.5.2/truss/cli.py
--rw-r--r--   0        0        0     2873 2023-07-28 22:19:06.033645 truss-0.5.2/truss/constants.py
--rw-r--r--   0        0        0      338 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/cache_warmer.py
--rw-r--r--   0        0        0     1294 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     7028 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1893 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2120 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     1072 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/truss_file_syncer.py
--rw-r--r--   0        0        0     5801 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-07-28 22:19:06.033645 truss-0.5.2/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-07-28 22:19:06.033645 truss-0.5.2/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-07-28 22:19:06.033645 truss-0.5.2/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-07-28 22:19:06.033645 truss-0.5.2/truss/errors.py
--rw-r--r--   0        0        0      824 2023-07-28 22:19:06.033645 truss-0.5.2/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-07-28 22:19:06.033645 truss-0.5.2/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1230 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2403 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1225 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     5425 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-07-28 22:19:06.033645 truss-0.5.2/truss/notebook.py
--rw-r--r--   0        0        0    15420 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      139 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/constants.py
--rw-r--r--   0        0        0      774 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/hash.py
--rw-r--r--   0        0        0     2930 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/local_truss_patch_applier.py
--rw-r--r--   0        0        0      468 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/signature.py
--rw-r--r--   0        0        0     3075 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      937 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-07-28 22:19:06.033645 truss-0.5.2/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-07-28 22:19:06.033645 truss-0.5.2/truss/readme_generator.py
--rw-r--r--   0        0        0      176 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/__init__.py
--rw-r--r--   0        0        0     4919 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/api.py
--rw-r--r--   0        0        0      752 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/auth.py
--rw-r--r--   0        0        0     3616 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/core.py
--rw-r--r--   0        0        0      943 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/error.py
--rw-r--r--   0        0        0     4741 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/remote.py
--rw-r--r--   0        0        0     1156 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/service.py
--rw-r--r--   0        0        0     2001 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/utils/tar.py
--rw-r--r--   0        0        0      985 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/utils/transfer.py
--rw-r--r--   0        0        0     1407 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/remote_cli.py
--rw-r--r--   0        0        0     4219 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/remote_factory.py
--rw-r--r--   0        0        0     5970 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/truss_remote.py
--rw-r--r--   0        0        0     2482 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/__init__.py
--rw-r--r--   0        0        0     1967 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     3819 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     5103 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     6317 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     4026 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2652 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0      998 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1842 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     7386 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     5930 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     2319 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      144 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     2382 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     2340 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/termination_handler_middleware.py
--rw-r--r--   0        0        0    12328 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      727 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0    11624 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      274 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     3279 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/logging.py
--rw-r--r--   0        0        0     1430 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0     3318 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/serialization.py
--rw-r--r--   0        0        0     1863 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/util.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0      739 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1550 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      739 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_async_truss/config.yaml
--rw-r--r--   0        0        0      646 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_async_truss/model/model.py
--rw-r--r--   0        0        0       34 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_concurrency_truss/config.yaml
--rw-r--r--   0        0        0      547 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_concurrency_truss/model/model.py
--rw-r--r--   0        0        0      739 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/config.yaml
--rw-r--r--   0        0        0      521 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/model/model.py
--rw-r--r--   0        0        0      773 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_truss/config.yaml
--rw-r--r--   0        0        0      568 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        6 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/packages/test_package/test.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/__init__.py
--rw-r--r--   0        0        0    22226 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    18726 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     1929 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0     2073 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/baseten/test_api.py
--rw-r--r--   0        0        0      580 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/baseten/test_auth.py
--rw-r--r--   0        0        0      835 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/baseten/test_core.py
--rw-r--r--   0        0        0     4316 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/test_remote_factory.py
--rw-r--r--   0        0        0     2394 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/test_truss_remote.py
--rw-r--r--   0        0        0    10415 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     6081 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     7513 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0     8326 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/test_server_integration.py
--rw-r--r--   0        0        0     1560 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/core/server/common/test_truss_server.py
--rw-r--r--   0        0        0      821 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2605 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/server/common/test_termination_handler_middleware.py
--rw-r--r--   0        0        0     2252 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_build.py
--rw-r--r--   0        0        0     8657 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0    14982 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_control_truss_patching.py
--rw-r--r--   0        0        0      517 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_docker.py
--rw-r--r--   0        0        0    12242 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    30057 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0     1865 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_validation.py
--rw-r--r--   0        0        0     4974 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/util/test_path.py
--rw-r--r--   0        0        0    15256 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_config.py
--rw-r--r--   0        0        0     2698 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41143 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_spec.py
--rw-r--r--   0        0        0     2782 2023-07-28 22:19:06.041646 truss-0.5.2/truss/types.py
--rw-r--r--   0        0        0     3121 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/.truss_ignore
--rw-r--r--   0        0        0      379 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/data_structures.py
--rw-r--r--   0        0        0     2552 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/download.py
--rw-r--r--   0        0        0      553 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/jinja.py
--rw-r--r--   0        0        0     6040 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-07-28 22:19:06.041646 truss-0.5.2/truss/validation.py
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 truss-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-07-31 20:34:42.276205 truss-0.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2418 2023-07-31 20:34:42.276205 truss-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-07-31 20:34:42.276205 truss-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3518 2023-07-31 20:34:42.276205 truss-0.5.3/README.md
+-rw-r--r--   0        0        0      933 2023-07-31 20:34:42.276205 truss-0.5.3/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2546 2023-07-31 20:34:42.388206 truss-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-07-31 20:34:42.388206 truss-0.5.3/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-31 20:34:42.388206 truss-0.5.3/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-07-31 20:34:42.388206 truss-0.5.3/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-07-31 20:34:42.388206 truss-0.5.3/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13363 2023-07-31 20:34:42.388206 truss-0.5.3/truss/build.py
+-rw-r--r--   0        0        0       51 2023-07-31 20:34:42.388206 truss-0.5.3/truss/cli/__init__.py
+-rw-r--r--   0        0        0    11384 2023-07-31 20:34:42.388206 truss-0.5.3/truss/cli/cli.py
+-rw-r--r--   0        0        0     1015 2023-07-31 20:34:42.388206 truss-0.5.3/truss/cli/create.py
+-rw-r--r--   0        0        0     2873 2023-07-31 20:34:42.388206 truss-0.5.3/truss/constants.py
+-rw-r--r--   0        0        0      338 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/cache_warmer.py
+-rw-r--r--   0        0        0     1294 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     8321 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1893 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2120 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     1072 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/truss_file_syncer.py
+-rw-r--r--   0        0        0     5801 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-07-31 20:34:42.388206 truss-0.5.3/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-07-31 20:34:42.388206 truss-0.5.3/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-07-31 20:34:42.388206 truss-0.5.3/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-07-31 20:34:42.388206 truss-0.5.3/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-07-31 20:34:42.388206 truss-0.5.3/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-07-31 20:34:42.388206 truss-0.5.3/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1230 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2403 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1225 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     5425 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-07-31 20:34:42.388206 truss-0.5.3/truss/notebook.py
+-rw-r--r--   0        0        0    15420 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      139 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/constants.py
+-rw-r--r--   0        0        0      774 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/hash.py
+-rw-r--r--   0        0        0     2930 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      468 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/signature.py
+-rw-r--r--   0        0        0     3075 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      937 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-07-31 20:34:42.388206 truss-0.5.3/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-07-31 20:34:42.388206 truss-0.5.3/truss/readme_generator.py
+-rw-r--r--   0        0        0      176 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/__init__.py
+-rw-r--r--   0        0        0     4919 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/api.py
+-rw-r--r--   0        0        0      752 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/auth.py
+-rw-r--r--   0        0        0     3616 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/core.py
+-rw-r--r--   0        0        0      943 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/error.py
+-rw-r--r--   0        0        0     4741 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/remote.py
+-rw-r--r--   0        0        0     1156 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/service.py
+-rw-r--r--   0        0        0     2001 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/utils/tar.py
+-rw-r--r--   0        0        0      985 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/utils/transfer.py
+-rw-r--r--   0        0        0     1407 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/remote_cli.py
+-rw-r--r--   0        0        0     4219 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/remote_factory.py
+-rw-r--r--   0        0        0     5970 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/truss_remote.py
+-rw-r--r--   0        0        0     2482 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1967 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     3819 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     5103 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     6317 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     4026 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2652 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0      998 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1842 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     7386 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     5930 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     2319 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      144 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     2340 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/termination_handler_middleware.py
+-rw-r--r--   0        0        0    12328 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0    11624 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      274 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     3279 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     1430 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     1863 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/util.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0      521 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/tgi/proxy.conf
+-rw-r--r--   0        0        0      491 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/tgi/supervisord.conf.jinja
+-rw-r--r--   0        0        0      586 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/tgi/tgi.Dockerfile.jinja
+-rw-r--r--   0        0        0     3400 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0      739 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_async_truss/config.yaml
+-rw-r--r--   0        0        0      646 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_async_truss/model/model.py
+-rw-r--r--   0        0        0       34 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_concurrency_truss/config.yaml
+-rw-r--r--   0        0        0      547 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_concurrency_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/config.yaml
+-rw-r--r--   0        0        0      521 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/model/model.py
+-rw-r--r--   0        0        0      773 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_truss/config.yaml
+-rw-r--r--   0        0        0      568 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        6 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/packages/test_package/test.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/__init__.py
+-rw-r--r--   0        0        0    22226 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    18726 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     1929 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0     2073 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/baseten/test_api.py
+-rw-r--r--   0        0        0      580 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/baseten/test_auth.py
+-rw-r--r--   0        0        0      835 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/baseten/test_core.py
+-rw-r--r--   0        0        0     4316 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/test_remote_factory.py
+-rw-r--r--   0        0        0     2394 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/test_truss_remote.py
+-rw-r--r--   0        0        0    10415 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     6081 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7513 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0     8326 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/test_server_integration.py
+-rw-r--r--   0        0        0     1560 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/core/server/common/test_truss_server.py
+-rw-r--r--   0        0        0      821 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2605 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/server/common/test_termination_handler_middleware.py
+-rw-r--r--   0        0        0     2252 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_build.py
+-rw-r--r--   0        0        0     8657 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    14982 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_docker.py
+-rw-r--r--   0        0        0    12242 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    30057 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0     1865 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     4974 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/util/test_path.py
+-rw-r--r--   0        0        0    15932 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_config.py
+-rw-r--r--   0        0        0     2698 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41143 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_spec.py
+-rw-r--r--   0        0        0     2782 2023-07-31 20:34:42.400206 truss-0.5.3/truss/types.py
+-rw-r--r--   0        0        0     3121 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/.truss_ignore
+-rw-r--r--   0        0        0      379 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/data_structures.py
+-rw-r--r--   0        0        0     2552 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/download.py
+-rw-r--r--   0        0        0      553 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/jinja.py
+-rw-r--r--   0        0        0     6040 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-07-31 20:34:42.400206 truss-0.5.3/truss/validation.py
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 truss-0.5.3/PKG-INFO
```

### Comparing `truss-0.5.2/CODE_OF_CONDUCT.md` & `truss-0.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/CONTRIBUTING.md` & `truss-0.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/LICENSE` & `truss-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/README.md` & `truss-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/context_builder.Dockerfile` & `truss-0.5.3/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/pyproject.toml` & `truss-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.5.2"
+version = "0.5.3"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.5.2/truss/blob/blob_backend_registry.py` & `truss-0.5.3/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/blob/http_public_blob_backend.py` & `truss-0.5.3/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/build.py` & `truss-0.5.3/truss/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from truss.constants import CONFIG_FILE, TEMPLATES_DIR, TRUSS
 from truss.docker import kill_containers
 from truss.environment_inference.requirements_inference import infer_deps
 from truss.errors import FrameworkNotSupportedError
 from truss.model_frameworks import MODEL_FRAMEWORKS_BY_TYPE, model_framework_from_model
 from truss.model_inference import infer_python_version, map_to_supported_python_version
 from truss.notebook import is_notebook_or_ipython
-from truss.truss_config import TrussConfig
+from truss.truss_config import Build, ModelServer, TrussConfig
 from truss.truss_handle import TrussHandle
 from truss.types import ModelFrameworkType
 from truss.util.gpu import get_gpu_memory
 from truss.util.path import build_truss_target_directory, copy_tree_path
 
 logger: logging.Logger = logging.getLogger(__name__)
 
@@ -27,33 +27,35 @@
     logger.addHandler(logging.StreamHandler(sys.stdout))
 
 
 def populate_target_directory(
     config: TrussConfig,
     target_directory_path: Optional[str] = None,
     template: str = "custom",
+    populate_dirs: bool = True,
 ) -> Path:
     target_directory_path_typed = None
     if target_directory_path is None:
         target_directory_path_typed = build_truss_target_directory(template)
     else:
         target_directory_path_typed = Path(target_directory_path)
         target_directory_path_typed.mkdir(parents=True, exist_ok=True)
 
-    # Create data dir
-    (target_directory_path_typed / config.data_dir).mkdir()
-
-    # Create bundled packages dir
-    # TODO: Drop by default
-    (target_directory_path_typed / config.bundled_packages_dir).mkdir()
-
-    # Create model module dir
-    model_dir = target_directory_path_typed / config.model_module_dir
-    template_path = TEMPLATES_DIR / template
-    copy_tree_path(template_path / "model", model_dir)
+    if populate_dirs:
+        # Create data dir
+        (target_directory_path_typed / config.data_dir).mkdir()
+
+        # Create bundled packages dir
+        # TODO: Drop by default
+        (target_directory_path_typed / config.bundled_packages_dir).mkdir()
+
+        # Create model module dir
+        model_dir = target_directory_path_typed / config.model_module_dir
+        template_path = TEMPLATES_DIR / template
+        copy_tree_path(template_path / "model", model_dir)
 
     # Write config
     with (target_directory_path_typed / CONFIG_FILE).open("w") as config_file:
         yaml.dump(config.to_dict(verbose=False), config_file)
 
     return target_directory_path_typed
 
@@ -211,14 +213,15 @@
 
 def init(
     target_directory: str,
     data_files: Optional[List[str]] = None,
     requirements_file: Optional[str] = None,
     bundled_packages: Optional[List[str]] = None,
     trainable: bool = False,
+    build_config: Optional[Build] = None,
 ) -> TrussHandle:
     """
     Initialize an empty placeholder Truss. A Truss is a build context designed
     to be built as a container locally or uploaded into a baseten serving
     environment. This placeholder structure can be filled to represent ML
     models.
 
@@ -226,19 +229,24 @@
         target_directory: Absolute or relative path of the directory to create
                           Truss in. The directory is created if it doesn't exist.
     """
     config = TrussConfig(
         python_version=map_to_supported_python_version(infer_python_version()),
     )
 
+    if build_config:
+        config.build = build_config
+
     if trainable:
         config.train.resources.use_gpu = True
 
     target_directory_path = populate_target_directory(
-        config=config, target_directory_path=target_directory
+        config=config,
+        target_directory_path=target_directory,
+        populate_dirs=config.build.model_server is ModelServer.TrussServer,
     )
 
     if trainable:
         _populate_default_training_code(
             config, target_directory_path=Path(target_directory)
         )
```

### Comparing `truss-0.5.2/truss/cli.py` & `truss-0.5.3/truss/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import wraps
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 import rich
 import rich_click as click
 import truss
+from truss.cli.create import select_server_backend
 from truss.remote.remote_cli import inquire_model_name, inquire_remote_name
 from truss.remote.remote_factory import RemoteFactory
 
 logging.basicConfig(level=logging.INFO)
 
 
 click.rich_click.COMMAND_GROUPS = {
@@ -101,16 +102,21 @@
 @error_handling
 def init(target_directory, skip_confirm, trainable) -> None:
     """Create a new truss.
 
     TARGET_DIRECTORY: A Truss is created in this directory
     """
     tr_path = Path(target_directory)
+    build_config = select_server_backend()
     if skip_confirm or click.confirm(f"A Truss will be created at {tr_path}"):
-        truss.init(target_directory=target_directory, trainable=trainable)
+        truss.init(
+            target_directory=target_directory,
+            trainable=trainable,
+            build_config=build_config,
+        )
         click.echo(f"Truss was created in {tr_path}")
 
 
 @image.command()  # type: ignore
 @click.argument("build_dir")
 @click.argument("target_directory", required=False)
 @error_handling
```

### Comparing `truss-0.5.2/truss/constants.py` & `truss-0.5.3/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/image_builder/image_builder.py` & `truss-0.5.3/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.5.3/truss/contexts/image_builder/serving_image_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,28 +22,57 @@
     file_is_not_empty,
     to_dotted_python_version,
     truss_base_image_name,
     truss_base_image_tag,
 )
 from truss.contexts.truss_context import TrussContext
 from truss.patch.hash import directory_content_hash
+from truss.truss_config import Build, ModelServer, TrussConfig
 from truss.truss_spec import TrussSpec
 from truss.util.download import download_external_data
 from truss.util.jinja import read_template_from_fs
 from truss.util.path import (
     build_truss_target_directory,
+    copy_file_path,
     copy_tree_or_file,
     copy_tree_path,
 )
 
 BUILD_SERVER_DIR_NAME = "server"
 BUILD_CONTROL_SERVER_DIR_NAME = "control"
 
 CONFIG_FILE = "config.yaml"
 
+HF_ACCESS_TOKEN_SECRET_NAME = "hf_access_token"
+
+
+def create_tgi_build_dir(config: TrussConfig, build_dir: Path):
+    if not build_dir.exists():
+        build_dir.mkdir(parents=True)
+
+    build_config: Build = config.build
+    hf_access_token = config.secrets.get(HF_ACCESS_TOKEN_SECRET_NAME)
+    dockerfile_template = read_template_from_fs(
+        TEMPLATES_DIR, "tgi/tgi.Dockerfile.jinja"
+    )
+    dockerfile_content = dockerfile_template.render(hf_access_token=hf_access_token)
+    dockerfile_filepath = build_dir / "Dockerfile"
+    dockerfile_filepath.write_text(dockerfile_content)
+
+    copy_file_path(TEMPLATES_DIR / "tgi" / "proxy.conf", build_dir / "proxy.conf")
+    args = " ".join(
+        [f"--{k.replace('_', '-')}={v}" for k, v in build_config.arguments.items()]
+    )
+    supervisord_template = read_template_from_fs(
+        TEMPLATES_DIR, "tgi/supervisord.conf.jinja"
+    )
+    supervisord_contents = supervisord_template.render(extra_args=args)
+    supervisord_filepath = build_dir / "supervisord.conf"
+    supervisord_filepath.write_text(supervisord_contents)
+
 
 class ServingImageBuilderContext(TrussContext):
     @staticmethod
     def run(truss_dir: Path):
         return ServingImageBuilder(truss_dir)
 
 
@@ -64,14 +93,18 @@
         spec = self._spec
         config = spec.config
         model_framework_name = spec.model_framework_name
         if build_dir is None:
             # TODO(pankaj) We probably don't need model framework specific directory.
             build_dir = build_truss_target_directory(model_framework_name)
 
+        if config.build.model_server is ModelServer.TGI:
+            create_tgi_build_dir(config, build_dir)
+            return
+
         data_dir = build_dir / config.data_dir  # type: ignore[operator]
 
         def copy_into_build_dir(from_path: Path, path_in_build_dir: str):
             copy_tree_or_file(from_path, build_dir / path_in_build_dir)  # type: ignore[operator]
 
         # Copy over truss
         copy_tree_path(truss_dir, build_dir)
```

### Comparing `truss-0.5.2/truss/contexts/image_builder/training_image_builder.py` & `truss-0.5.3/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/image_builder/util.py` & `truss-0.5.3/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.5.3/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/local_loader/load_model_local.py` & `truss-0.5.3/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/local_loader/train_local.py` & `truss-0.5.3/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/local_loader/truss_file_syncer.py` & `truss-0.5.3/truss/contexts/local_loader/truss_file_syncer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.5.3/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/contexts/local_loader/utils.py` & `truss-0.5.3/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/docker.py` & `truss-0.5.3/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/environment_inference/requirements_inference.py` & `truss-0.5.3/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/errors.py` & `truss-0.5.3/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/local/local_config.py` & `truss-0.5.3/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/local/local_config_handler.py` & `truss-0.5.3/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_framework.py` & `truss-0.5.3/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/__init__.py` & `truss-0.5.3/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/huggingface_transformer.py` & `truss-0.5.3/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/keras.py` & `truss-0.5.3/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/lightgbm.py` & `truss-0.5.3/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/mlflow.py` & `truss-0.5.3/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/pytorch.py` & `truss-0.5.3/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/sklearn.py` & `truss-0.5.3/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_frameworks/xgboost.py` & `truss-0.5.3/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/model_inference.py` & `truss-0.5.3/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/patch/calc_patch.py` & `truss-0.5.3/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/patch/dir_signature.py` & `truss-0.5.3/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/patch/hash.py` & `truss-0.5.3/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/patch/local_truss_patch_applier.py` & `truss-0.5.3/truss/patch/local_truss_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/patch/truss_dir_patch_applier.py` & `truss-0.5.3/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/patch/types.py` & `truss-0.5.3/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/readme_generator.py` & `truss-0.5.3/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/api.py` & `truss-0.5.3/truss/remote/baseten/api.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/auth.py` & `truss-0.5.3/truss/remote/baseten/auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/core.py` & `truss-0.5.3/truss/remote/baseten/core.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/error.py` & `truss-0.5.3/truss/remote/baseten/error.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/remote.py` & `truss-0.5.3/truss/remote/baseten/remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/service.py` & `truss-0.5.3/truss/remote/baseten/service.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/utils/tar.py` & `truss-0.5.3/truss/remote/baseten/utils/tar.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/baseten/utils/transfer.py` & `truss-0.5.3/truss/remote/baseten/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/remote_cli.py` & `truss-0.5.3/truss/remote/remote_cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/remote_factory.py` & `truss-0.5.3/truss/remote/remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/remote/truss_remote.py` & `truss-0.5.3/truss/remote/truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/README.md.jinja` & `truss-0.5.3/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/base.Dockerfile.jinja` & `truss-0.5.3/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/application.py` & `truss-0.5.3/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/endpoints.py` & `truss-0.5.3/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/errors.py` & `truss-0.5.3/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.5.3/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.5.3/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.5.3/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/helpers/types.py` & `truss-0.5.3/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/control/control/server.py` & `truss-0.5.3/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/custom/model/model.py` & `truss-0.5.3/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/huggingface_transformer/model/model.py` & `truss-0.5.3/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/keras/model/model.py` & `truss-0.5.3/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/lightgbm/model/model.py` & `truss-0.5.3/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/mlflow/model/model.py` & `truss-0.5.3/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/pytorch/model/model.py` & `truss-0.5.3/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/common/errors.py` & `truss-0.5.3/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.5.3/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/common/patches.py` & `truss-0.5.3/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/common/retry.py` & `truss-0.5.3/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/common/termination_handler_middleware.py` & `truss-0.5.3/truss/templates/server/common/termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/common/truss_server.py` & `truss-0.5.3/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/inference_server.py` & `truss-0.5.3/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server/model_wrapper.py` & `truss-0.5.3/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/server.Dockerfile.jinja` & `truss-0.5.3/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/shared/logging.py` & `truss-0.5.3/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/shared/secrets_resolver.py` & `truss-0.5.3/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/shared/serialization.py` & `truss-0.5.3/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/shared/util.py` & `truss-0.5.3/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/sklearn/model/model.py` & `truss-0.5.3/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/training/job.py` & `truss-0.5.3/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/templates/xgboost/model/model.py` & `truss-0.5.3/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/auto-mpg.data` & `truss-0.5.3/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/happy.ipynb` & `truss-0.5.3/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/model_load_failure_test/config.yaml` & `truss-0.5.3/truss/test_data/model_load_failure_test/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.5.3/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/patch_ping_test_server/app.py` & `truss-0.5.3/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/pima-indians-diabetes.csv` & `truss-0.5.3/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/readme_int_example.md` & `truss-0.5.3/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/readme_no_example.md` & `truss-0.5.3/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/readme_str_example.md` & `truss-0.5.3/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/server.Dockerfile` & `truss-0.5.3/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.5.3/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.5.3/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_async_truss/config.yaml` & `truss-0.5.3/truss/test_data/test_async_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_async_truss/model/model.py` & `truss-0.5.3/truss/test_data/test_async_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_concurrency_truss/model/model.py` & `truss-0.5.3/truss/test_data/test_concurrency_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/config.yaml` & `truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/model/model.py` & `truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_streaming_truss/config.yaml` & `truss-0.5.3/truss/test_data/test_streaming_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_streaming_truss/model/model.py` & `truss-0.5.3/truss/test_data/test_streaming_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_truss/config.yaml` & `truss-0.5.3/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/test_data/test_truss/model/model.py` & `truss-0.5.3/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/conftest.py` & `truss-0.5.3/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.5.3/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.5.3/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.5.3/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.5.3/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/local/test_local_config_handler.py` & `truss-0.5.3/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.5.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.5.3/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.5.3/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.5.3/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.5.3/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.5.3/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/patch/test_calc_patch.py` & `truss-0.5.3/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/patch/test_hash.py` & `truss-0.5.3/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.5.3/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/remote/baseten/test_api.py` & `truss-0.5.3/truss/tests/remote/baseten/test_api.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/remote/baseten/test_auth.py` & `truss-0.5.3/truss/tests/remote/baseten/test_auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/remote/baseten/test_core.py` & `truss-0.5.3/truss/tests/remote/baseten/test_core.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/remote/test_remote_factory.py` & `truss-0.5.3/truss/tests/remote/test_remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/remote/test_truss_remote.py` & `truss-0.5.3/truss/tests/remote/test_truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/samples.py` & `truss-0.5.3/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.5.3/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.5.3/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/control/control/test_server.py` & `truss-0.5.3/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/control/control/test_server_integration.py` & `truss-0.5.3/truss/tests/templates/control/control/test_server_integration.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/core/server/common/test_truss_server.py` & `truss-0.5.3/truss/tests/templates/core/server/common/test_truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/core/server/common/test_util.py` & `truss-0.5.3/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.5.3/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/server/common/test_retry.py` & `truss-0.5.3/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/server/common/test_termination_handler_middleware.py` & `truss-0.5.3/truss/tests/templates/server/common/test_termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.5.3/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_backward.py` & `truss-0.5.3/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_build.py` & `truss-0.5.3/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_config.py` & `truss-0.5.3/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_context_builder_image.py` & `truss-0.5.3/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_control_truss_patching.py` & `truss-0.5.3/truss/tests/test_control_truss_patching.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_docker.py` & `truss-0.5.3/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_model_inference.py` & `truss-0.5.3/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_notebooks.py` & `truss-0.5.3/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.5.3/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_truss_gatherer.py` & `truss-0.5.3/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_truss_handle.py` & `truss-0.5.3/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/test_validation.py` & `truss-0.5.3/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/tests/util/test_path.py` & `truss-0.5.3/truss/tests/util/test_path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/truss_config.py` & `truss-0.5.3/truss/truss_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,39 @@
 
     def to_dict(self):
         return {
             "predict_concurrency": self.predict_concurrency,
         }
 
 
+class ModelServer(Enum):
+    TrussServer = "TrussServer"
+    TGI = "TGI"
+    VLLM = "VLLM"
+
+
+@dataclass
+class Build:
+    model_server: ModelServer = ModelServer.TrussServer
+    arguments: Dict = field(default_factory=dict)
+
+    @staticmethod
+    def from_dict(d):
+        model_server = ModelServer[d.get("model_server", "TrussServer")]
+        arguments = d.get("arguments", {})
+
+        return Build(
+            model_server=model_server,
+            arguments=arguments,
+        )
+
+    def to_dict(self):
+        return obj_to_dict(self)
+
+
 @dataclass
 class Resources:
     cpu: str = DEFAULT_CPU
     memory: str = DEFAULT_MEMORY
     use_gpu: bool = DEFAULT_USE_GPU
     accelerator: AcceleratorSpec = field(default_factory=AcceleratorSpec)
 
@@ -298,14 +323,15 @@
     input_type: str = DEFAULT_MODEL_INPUT_TYPE
     model_metadata: Dict[str, Any] = field(default_factory=dict)
     requirements: List[str] = field(default_factory=list)
     system_packages: List[str] = field(default_factory=list)
     environment_variables: Dict[str, str] = field(default_factory=dict)
     resources: Resources = field(default_factory=Resources)
     runtime: Runtime = field(default_factory=Runtime)
+    build: Build = field(default_factory=Build)
     python_version: str = DEFAULT_PYTHON_VERSION
     examples_filename: str = DEFAULT_EXAMPLES_FILENAME
     secrets: Dict[str, str] = field(default_factory=dict)
     description: Optional[str] = None
     bundled_packages_dir: str = DEFAULT_BUNDLED_PACKAGES_DIR
     external_package_dirs: List[str] = field(default_factory=list)
     live_reload: bool = False
@@ -342,14 +368,15 @@
             input_type=d.get("input_type", DEFAULT_MODEL_INPUT_TYPE),
             model_metadata=d.get("model_metadata", {}),
             requirements=d.get("requirements", []),
             system_packages=d.get("system_packages", []),
             environment_variables=d.get("environment_variables", {}),
             resources=Resources.from_dict(d.get("resources", {})),
             runtime=Runtime.from_dict(d.get("runtime", {})),
+            build=Build.from_dict(d.get("build", {})),
             python_version=d.get("python_version", DEFAULT_PYTHON_VERSION),
             model_name=d.get("model_name", None),
             examples_filename=d.get("examples_filename", DEFAULT_EXAMPLES_FILENAME),
             secrets=d.get("secrets", {}),
             description=d.get("description", None),
             bundled_packages_dir=d.get(
                 "bundled_packages_dir", DEFAULT_BUNDLED_PACKAGES_DIR
@@ -388,14 +415,15 @@
             validate_secret_name(secret_name)
 
 
 DATACLASS_TO_REQ_KEYS_MAP = {
     Train: {"variables"},
     Resources: {"accelerator", "cpu", "memory", "use_gpu"},
     Runtime: {"predict_concurrency"},
+    Build: {"model_server"},
     TrussConfig: {
         "environment_variables",
         "external_package_dirs",
         "model_metadata",
         "model_name",
         "python_version",
         "requirements",
```

### Comparing `truss-0.5.2/truss/truss_gatherer.py` & `truss-0.5.3/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/truss_handle.py` & `truss-0.5.3/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/truss_spec.py` & `truss-0.5.3/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/types.py` & `truss-0.5.3/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/util/.truss_ignore` & `truss-0.5.3/truss/util/.truss_ignore`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/util/download.py` & `truss-0.5.3/truss/util/download.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/util/gpu.py` & `truss-0.5.3/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/util/path.py` & `truss-0.5.3/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/truss/validation.py` & `truss-0.5.3/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.2/PKG-INFO` & `truss-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.5.2
+Version: 0.5.3
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
```

