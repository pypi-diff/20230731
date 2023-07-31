# Comparing `tmp/azure-quantum-0.28.291393b1.tar.gz` & `tmp/azure-quantum-0.28.291394.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-quantum-0.28.291393b1.tar", last modified: Fri Jul 28 04:52:22 2023, max compression
+gzip compressed data, was "azure-quantum-0.28.291394.tar", last modified: Fri Jul 28 04:45:19 2023, max compression
```

## Comparing `azure-quantum-0.28.291393b1.tar` & `azure-quantum-0.28.291394.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/
--rw-rw-rw-   0        0        0     5398 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/PKG-INFO
--rw-rw-rw-   0        0        0     4891 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.393275 azure-quantum-0.28.291393b1/azure/
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.423967 azure-quantum-0.28.291393b1/azure/quantum/
--rw-rw-rw-   0        0        0      414 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.423967 azure-quantum-0.28.291393b1/azure/quantum/_authentication/
--rw-rw-rw-   0        0        0      236 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/__init__.py
--rw-rw-rw-   0        0        0     5047 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/_chained.py
--rw-rw-rw-   0        0        0    10502 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/_default.py
--rw-rw-rw-   0        0        0     3570 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/
--rw-rw-rw-   0        0        0      896 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/__init__.py
--rw-rw-rw-   0        0        0     5854 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_client.py
--rw-rw-rw-   0        0        0     4444 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_configuration.py
--rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_patch.py
--rw-rw-rw-   0        0        0    80832 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_serialization.py
--rw-rw-rw-   0        0        0      996 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_vendor.py
--rw-rw-rw-   0        0        0      503 2023-07-28 04:52:21.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/
--rw-rw-rw-   0        0        0      840 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/__init__.py
--rw-rw-rw-   0        0        0     6010 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_client.py
--rw-rw-rw-   0        0        0     4487 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_configuration.py
--rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_patch.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/
--rw-rw-rw-   0        0        0     1154 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/__init__.py
--rw-rw-rw-   0        0        0    54215 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_patch.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/models/
--rw-rw-rw-   0        0        0     2100 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/__init__.py
--rw-rw-rw-   0        0        0     2977 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/_enums.py
--rw-rw-rw-   0        0        0    41802 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/_models.py
--rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/_patch.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/
--rw-rw-rw-   0        0        0     1154 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/__init__.py
--rw-rw-rw-   0        0        0    75919 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_patch.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/
--rw-rw-rw-   0        0        0      360 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/
--rw-rw-rw-   0        0        0      236 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/__init__.py
--rw-rw-rw-   0        0        0     4647 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_chained.py
--rw-rw-rw-   0        0        0    10430 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_default.py
--rw-rw-rw-   0        0        0     3632 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/job/
--rw-rw-rw-   0        0        0       43 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/job/__init__.py
--rw-rw-rw-   0        0        0    11565 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/job/base_job.py
--rw-rw-rw-   0        0        0     3728 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/job/job.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/
--rw-rw-rw-   0        0        0      287 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/__init__.py
--rw-rw-rw-   0        0        0      560 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/online_problem.py
--rw-rw-rw-   0        0        0     3638 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/problem.py
--rw-rw-rw-   0        0        0    10536 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/streaming_problem.py
--rw-rw-rw-   0        0        0    12953 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/aio/target/
--rw-rw-rw-   0        0        0      521 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/ionq.py
--rw-rw-rw-   0        0        0     1413 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/quantinuum.py
--rw-rw-rw-   0        0        0     3311 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/solvers.py
--rw-rw-rw-   0        0        0     2366 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/target.py
--rw-rw-rw-   0        0        0     2449 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/target_factory.py
--rw-rw-rw-   0        0        0      249 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/toshiba.py
--rw-rw-rw-   0        0        0    13507 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/workspace.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/argument_types/
--rw-rw-rw-   0        0        0      213 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/argument_types/__init__.py
--rw-rw-rw-   0        0        0      721 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/argument_types/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/chemistry/
--rw-rw-rw-   0        0        0      351 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/chemistry/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/cirq/
--rw-rw-rw-   0        0        0      125 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/__init__.py
--rw-rw-rw-   0        0        0     2773 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/job.py
--rw-rw-rw-   0        0        0     8039 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/service.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/
--rw-rw-rw-   0        0        0      502 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/__init__.py
--rw-rw-rw-   0        0        0     6804 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/ionq.py
--rw-rw-rw-   0        0        0     4541 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/quantinuum.py
--rw-rw-rw-   0        0        0     2184 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/target.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/job/
--rw-rw-rw-   0        0        0      372 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/__init__.py
--rw-rw-rw-   0        0        0    11987 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/base_job.py
--rw-rw-rw-   0        0        0     1683 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/filtered_job.py
--rw-rw-rw-   0        0        0     4505 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/job.py
--rw-rw-rw-   0        0        0    11936 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/session.py
--rw-rw-rw-   0        0        0     1198 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item.py
--rw-rw-rw-   0        0        0     1200 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item_factory.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/optimization/
--rw-rw-rw-   0        0        0      276 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/__init__.py
--rw-rw-rw-   0        0        0      636 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/online_problem.py
--rw-rw-rw-   0        0        0    13570 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/problem.py
--rw-rw-rw-   0        0        0      319 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/solvers.py
--rw-rw-rw-   0        0        0    13650 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/streaming_problem.py
--rw-rw-rw-   0        0        0     5983 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/term.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/optimization/toshiba/
--rw-rw-rw-   0        0        0      302 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/toshiba/__init__.py
--rw-rw-rw-   0        0        0      374 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/toshiba/solvers.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/qiskit/
--rw-rw-rw-   0        0        0      273 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.502097 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/
--rw-rw-rw-   0        0        0      965 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/__init__.py
--rw-rw-rw-   0        0        0    16467 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/backend.py
--rw-rw-rw-   0        0        0    12920 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/ionq.py
--rw-rw-rw-   0        0        0     3441 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/microsoft.py
--rw-rw-rw-   0        0        0     3884 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/qci.py
--rw-rw-rw-   0        0        0    13278 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/quantinuum.py
--rw-rw-rw-   0        0        0     4081 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/rigetti.py
--rw-rw-rw-   0        0        0    14829 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/job.py
--rw-rw-rw-   0        0        0     9974 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/provider.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.502097 azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/
--rw-rw-rw-   0        0        0        0 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/__init__.py
--rw-rw-rw-   0        0        0      814 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/resource_estimator.py
--rw-rw-rw-   0        0        0    12536 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/
--rw-rw-rw-   0        0        0      507 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/__init__.py
--rw-rw-rw-   0        0        0     7212 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/ionq.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/
--rw-rw-rw-   0        0        0      502 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/__init__.py
--rw-rw-rw-   0        0        0     1005 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/job.py
--rw-rw-rw-   0        0        0    13896 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/result.py
--rw-rw-rw-   0        0        0    15889 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/target.py
--rw-rw-rw-   0        0        0     8976 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/params.py
--rw-rw-rw-   0        0        0     7250 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/quantinuum.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/
--rw-rw-rw-   0        0        0      378 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/result.py
--rw-rw-rw-   0        0        0     5916 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/target.py
--rw-rw-rw-   0        0        0    14807 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/solvers.py
--rw-rw-rw-   0        0        0     8933 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/target.py
--rw-rw-rw-   0        0        0     5322 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/target_factory.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/
--rw-rw-rw-   0        0        0      146 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/__init__.py
--rw-rw-rw-   0        0        0     5722 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/solvers.py
--rw-rw-rw-   0        0        0      243 2023-07-28 04:52:21.000000 azure-quantum-0.28.291393b1/azure/quantum/version.py
--rw-rw-rw-   0        0        0    19134 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/workspace.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure_quantum.egg-info/
--rw-rw-rw-   0        0        0     5398 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4242 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      782 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       46 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-cirq.txt
--rw-rw-rw-   0        0        0       94 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-dev.txt
--rw-rw-rw-   0        0        0      248 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-qiskit.txt
--rw-rw-rw-   0        0        0       19 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-qsharp.txt
--rw-rw-rw-   0        0        0      275 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-quil.txt
--rw-rw-rw-   0        0        0      246 2023-07-28 04:52:17.000000 azure-quantum-0.28.291393b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/setup.cfg
--rw-rw-rw-   0        0        0     3770 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.846238 azure-quantum-0.28.291394/
+-rw-rw-rw-   0        0        0     5396 2023-07-28 04:45:19.846238 azure-quantum-0.28.291394/PKG-INFO
+-rw-rw-rw-   0        0        0     4891 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.768115 azure-quantum-0.28.291394/azure/
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.783737 azure-quantum-0.28.291394/azure/quantum/
+-rw-rw-rw-   0        0        0      414 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.783737 azure-quantum-0.28.291394/azure/quantum/_authentication/
+-rw-rw-rw-   0        0        0      236 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     5047 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_authentication/_chained.py
+-rw-rw-rw-   0        0        0    10502 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3570 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.783737 azure-quantum-0.28.291394/azure/quantum/_client/
+-rw-rw-rw-   0        0        0      896 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/__init__.py
+-rw-rw-rw-   0        0        0     5854 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/_client.py
+-rw-rw-rw-   0        0        0     4444 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/_configuration.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/_patch.py
+-rw-rw-rw-   0        0        0    80832 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/_serialization.py
+-rw-rw-rw-   0        0        0      996 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/_vendor.py
+-rw-rw-rw-   0        0        0      501 2023-07-28 04:45:19.000000 azure-quantum-0.28.291394/azure/quantum/_client/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/_client/aio/
+-rw-rw-rw-   0        0        0      840 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/aio/__init__.py
+-rw-rw-rw-   0        0        0     6010 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/aio/_client.py
+-rw-rw-rw-   0        0        0     4487 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/aio/_configuration.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/aio/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/_client/aio/operations/
+-rw-rw-rw-   0        0        0     1154 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/aio/operations/__init__.py
+-rw-rw-rw-   0        0        0    54215 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/aio/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/aio/operations/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/_client/models/
+-rw-rw-rw-   0        0        0     2100 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/models/__init__.py
+-rw-rw-rw-   0        0        0     2977 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/models/_enums.py
+-rw-rw-rw-   0        0        0    41802 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/models/_models.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/models/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/_client/operations/
+-rw-rw-rw-   0        0        0     1154 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/operations/__init__.py
+-rw-rw-rw-   0        0        0    75919 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/_client/operations/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/aio/
+-rw-rw-rw-   0        0        0      360 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/aio/_authentication/
+-rw-rw-rw-   0        0        0      236 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     4647 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/_authentication/_chained.py
+-rw-rw-rw-   0        0        0    10430 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3632 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/aio/job/
+-rw-rw-rw-   0        0        0       43 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/job/__init__.py
+-rw-rw-rw-   0        0        0    11565 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/job/base_job.py
+-rw-rw-rw-   0        0        0     3728 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/job/job.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.799364 azure-quantum-0.28.291394/azure/quantum/aio/optimization/
+-rw-rw-rw-   0        0        0      287 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/optimization/__init__.py
+-rw-rw-rw-   0        0        0      560 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/optimization/online_problem.py
+-rw-rw-rw-   0        0        0     3638 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/optimization/problem.py
+-rw-rw-rw-   0        0        0    10536 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/optimization/streaming_problem.py
+-rw-rw-rw-   0        0        0    12953 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.814988 azure-quantum-0.28.291394/azure/quantum/aio/target/
+-rw-rw-rw-   0        0        0      521 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/target/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/target/ionq.py
+-rw-rw-rw-   0        0        0     1413 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/target/quantinuum.py
+-rw-rw-rw-   0        0        0     3311 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/target/solvers.py
+-rw-rw-rw-   0        0        0     2366 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/target/target.py
+-rw-rw-rw-   0        0        0     2449 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/target/target_factory.py
+-rw-rw-rw-   0        0        0      249 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/target/toshiba.py
+-rw-rw-rw-   0        0        0    13507 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/aio/workspace.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.814988 azure-quantum-0.28.291394/azure/quantum/argument_types/
+-rw-rw-rw-   0        0        0      213 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/argument_types/__init__.py
+-rw-rw-rw-   0        0        0      721 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/argument_types/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.814988 azure-quantum-0.28.291394/azure/quantum/chemistry/
+-rw-rw-rw-   0        0        0      351 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/chemistry/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.814988 azure-quantum-0.28.291394/azure/quantum/cirq/
+-rw-rw-rw-   0        0        0      125 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/cirq/__init__.py
+-rw-rw-rw-   0        0        0     2773 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/cirq/job.py
+-rw-rw-rw-   0        0        0     8039 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/cirq/service.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.814988 azure-quantum-0.28.291394/azure/quantum/cirq/targets/
+-rw-rw-rw-   0        0        0      502 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/cirq/targets/__init__.py
+-rw-rw-rw-   0        0        0     6804 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/cirq/targets/ionq.py
+-rw-rw-rw-   0        0        0     4541 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/cirq/targets/quantinuum.py
+-rw-rw-rw-   0        0        0     2184 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/cirq/targets/target.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.814988 azure-quantum-0.28.291394/azure/quantum/job/
+-rw-rw-rw-   0        0        0      372 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/job/__init__.py
+-rw-rw-rw-   0        0        0    11987 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/job/base_job.py
+-rw-rw-rw-   0        0        0     1683 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/job/filtered_job.py
+-rw-rw-rw-   0        0        0     4505 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/job/job.py
+-rw-rw-rw-   0        0        0    11936 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/job/session.py
+-rw-rw-rw-   0        0        0     1198 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/job/workspace_item.py
+-rw-rw-rw-   0        0        0     1200 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/job/workspace_item_factory.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.814988 azure-quantum-0.28.291394/azure/quantum/optimization/
+-rw-rw-rw-   0        0        0      276 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/__init__.py
+-rw-rw-rw-   0        0        0      636 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/online_problem.py
+-rw-rw-rw-   0        0        0    13570 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/problem.py
+-rw-rw-rw-   0        0        0      319 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/solvers.py
+-rw-rw-rw-   0        0        0    13650 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/streaming_problem.py
+-rw-rw-rw-   0        0        0     5983 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/term.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/optimization/toshiba/
+-rw-rw-rw-   0        0        0      302 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/toshiba/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/optimization/toshiba/solvers.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/qiskit/
+-rw-rw-rw-   0        0        0      273 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/
+-rw-rw-rw-   0        0        0      965 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/__init__.py
+-rw-rw-rw-   0        0        0    16467 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/backend.py
+-rw-rw-rw-   0        0        0    12920 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/ionq.py
+-rw-rw-rw-   0        0        0     3441 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/microsoft.py
+-rw-rw-rw-   0        0        0     3884 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/qci.py
+-rw-rw-rw-   0        0        0    13278 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/quantinuum.py
+-rw-rw-rw-   0        0        0     4081 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/backends/rigetti.py
+-rw-rw-rw-   0        0        0    14829 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/job.py
+-rw-rw-rw-   0        0        0     9974 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/provider.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/qiskit/results/
+-rw-rw-rw-   0        0        0        0 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/results/__init__.py
+-rw-rw-rw-   0        0        0      814 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/qiskit/results/resource_estimator.py
+-rw-rw-rw-   0        0        0    12536 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/target/
+-rw-rw-rw-   0        0        0      507 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/__init__.py
+-rw-rw-rw-   0        0        0     7212 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/ionq.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/target/microsoft/
+-rw-rw-rw-   0        0        0      502 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/microsoft/__init__.py
+-rw-rw-rw-   0        0        0     1005 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/microsoft/job.py
+-rw-rw-rw-   0        0        0    13896 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/microsoft/result.py
+-rw-rw-rw-   0        0        0    15889 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/microsoft/target.py
+-rw-rw-rw-   0        0        0     8976 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/params.py
+-rw-rw-rw-   0        0        0     7250 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/quantinuum.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/target/rigetti/
+-rw-rw-rw-   0        0        0      378 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/rigetti/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/rigetti/result.py
+-rw-rw-rw-   0        0        0     5916 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/rigetti/target.py
+-rw-rw-rw-   0        0        0    14807 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/solvers.py
+-rw-rw-rw-   0        0        0     8933 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/target.py
+-rw-rw-rw-   0        0        0     5322 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/target_factory.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.830613 azure-quantum-0.28.291394/azure/quantum/target/toshiba/
+-rw-rw-rw-   0        0        0      146 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/toshiba/__init__.py
+-rw-rw-rw-   0        0        0     5722 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/target/toshiba/solvers.py
+-rw-rw-rw-   0        0        0      241 2023-07-28 04:45:19.000000 azure-quantum-0.28.291394/azure/quantum/version.py
+-rw-rw-rw-   0        0        0    19134 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/azure/quantum/workspace.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:45:19.846238 azure-quantum-0.28.291394/azure_quantum.egg-info/
+-rw-rw-rw-   0        0        0     5396 2023-07-28 04:45:19.000000 azure-quantum-0.28.291394/azure_quantum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4242 2023-07-28 04:45:19.000000 azure-quantum-0.28.291394/azure_quantum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:45:19.000000 azure-quantum-0.28.291394/azure_quantum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      782 2023-07-28 04:45:19.000000 azure-quantum-0.28.291394/azure_quantum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 04:45:19.000000 azure-quantum-0.28.291394/azure_quantum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       46 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/requirements-cirq.txt
+-rw-rw-rw-   0        0        0       94 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/requirements-dev.txt
+-rw-rw-rw-   0        0        0      248 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/requirements-qiskit.txt
+-rw-rw-rw-   0        0        0       19 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/requirements-qsharp.txt
+-rw-rw-rw-   0        0        0      275 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/requirements-quil.txt
+-rw-rw-rw-   0        0        0      246 2023-07-28 04:45:16.000000 azure-quantum-0.28.291394/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:45:19.846238 azure-quantum-0.28.291394/setup.cfg
+-rw-rw-rw-   0        0        0     3770 2023-07-28 04:27:17.000000 azure-quantum-0.28.291394/setup.py
```

### Comparing `azure-quantum-0.28.291393b1/PKG-INFO` & `azure-quantum-0.28.291394/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 0.28.291393b1
+Version: 0.28.291394
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/qdk-python
 Author: Microsoft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `azure-quantum-0.28.291393b1/README.md` & `azure-quantum-0.28.291394/README.md`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_authentication/_chained.py` & `azure-quantum-0.28.291394/azure/quantum/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_authentication/_default.py` & `azure-quantum-0.28.291394/azure/quantum/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_authentication/_token.py` & `azure-quantum-0.28.291394/azure/quantum/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/__init__.py` & `azure-quantum-0.28.291394/azure/quantum/_client/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/_client.py` & `azure-quantum-0.28.291394/azure/quantum/_client/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/_configuration.py` & `azure-quantum-0.28.291394/azure/quantum/_client/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/_patch.py` & `azure-quantum-0.28.291394/azure/quantum/_client/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/_serialization.py` & `azure-quantum-0.28.291394/azure/quantum/_client/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/_vendor.py` & `azure-quantum-0.28.291394/azure/quantum/_client/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/__init__.py` & `azure-quantum-0.28.291394/azure/quantum/_client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_client.py` & `azure-quantum-0.28.291394/azure/quantum/_client/aio/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_configuration.py` & `azure-quantum-0.28.291394/azure/quantum/_client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_patch.py` & `azure-quantum-0.28.291394/azure/quantum/_client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/__init__.py` & `azure-quantum-0.28.291394/azure/quantum/_client/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_operations.py` & `azure-quantum-0.28.291394/azure/quantum/_client/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_patch.py` & `azure-quantum-0.28.291394/azure/quantum/_client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/models/__init__.py` & `azure-quantum-0.28.291394/azure/quantum/_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/models/_enums.py` & `azure-quantum-0.28.291394/azure/quantum/_client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/models/_models.py` & `azure-quantum-0.28.291394/azure/quantum/_client/models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/models/_patch.py` & `azure-quantum-0.28.291394/azure/quantum/_client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/operations/__init__.py` & `azure-quantum-0.28.291394/azure/quantum/_client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_operations.py` & `azure-quantum-0.28.291394/azure/quantum/_client/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_patch.py` & `azure-quantum-0.28.291394/azure/quantum/_client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_chained.py` & `azure-quantum-0.28.291394/azure/quantum/aio/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_default.py` & `azure-quantum-0.28.291394/azure/quantum/aio/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_token.py` & `azure-quantum-0.28.291394/azure/quantum/aio/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/job/base_job.py` & `azure-quantum-0.28.291394/azure/quantum/aio/job/base_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/job/job.py` & `azure-quantum-0.28.291394/azure/quantum/aio/job/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/online_problem.py` & `azure-quantum-0.28.291394/azure/quantum/aio/optimization/online_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/problem.py` & `azure-quantum-0.28.291394/azure/quantum/aio/optimization/problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/streaming_problem.py` & `azure-quantum-0.28.291394/azure/quantum/aio/optimization/streaming_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/storage.py` & `azure-quantum-0.28.291394/azure/quantum/aio/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/target/__init__.py` & `azure-quantum-0.28.291394/azure/quantum/aio/target/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/target/ionq.py` & `azure-quantum-0.28.291394/azure/quantum/aio/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/target/quantinuum.py` & `azure-quantum-0.28.291394/azure/quantum/aio/target/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/target/solvers.py` & `azure-quantum-0.28.291394/azure/quantum/aio/target/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/target/target.py` & `azure-quantum-0.28.291394/azure/quantum/aio/target/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/target/target_factory.py` & `azure-quantum-0.28.291394/azure/quantum/aio/target/target_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/aio/workspace.py` & `azure-quantum-0.28.291394/azure/quantum/aio/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/argument_types/types.py` & `azure-quantum-0.28.291394/azure/quantum/argument_types/types.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/cirq/job.py` & `azure-quantum-0.28.291394/azure/quantum/cirq/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/cirq/service.py` & `azure-quantum-0.28.291394/azure/quantum/cirq/service.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/ionq.py` & `azure-quantum-0.28.291394/azure/quantum/cirq/targets/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/quantinuum.py` & `azure-quantum-0.28.291394/azure/quantum/cirq/targets/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/target.py` & `azure-quantum-0.28.291394/azure/quantum/cirq/targets/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/job/base_job.py` & `azure-quantum-0.28.291394/azure/quantum/job/base_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/job/filtered_job.py` & `azure-quantum-0.28.291394/azure/quantum/job/filtered_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/job/job.py` & `azure-quantum-0.28.291394/azure/quantum/job/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/job/session.py` & `azure-quantum-0.28.291394/azure/quantum/job/session.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item.py` & `azure-quantum-0.28.291394/azure/quantum/job/workspace_item.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item_factory.py` & `azure-quantum-0.28.291394/azure/quantum/job/workspace_item_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/optimization/online_problem.py` & `azure-quantum-0.28.291394/azure/quantum/optimization/online_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/optimization/problem.py` & `azure-quantum-0.28.291394/azure/quantum/optimization/problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/optimization/streaming_problem.py` & `azure-quantum-0.28.291394/azure/quantum/optimization/streaming_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/optimization/term.py` & `azure-quantum-0.28.291394/azure/quantum/optimization/term.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/__init__.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/backend.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/backends/backend.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/ionq.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/microsoft.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/backends/microsoft.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/qci.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/backends/qci.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/quantinuum.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/backends/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/rigetti.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/backends/rigetti.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/job.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/provider.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/resource_estimator.py` & `azure-quantum-0.28.291394/azure/quantum/qiskit/results/resource_estimator.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/storage.py` & `azure-quantum-0.28.291394/azure/quantum/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/ionq.py` & `azure-quantum-0.28.291394/azure/quantum/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/job.py` & `azure-quantum-0.28.291394/azure/quantum/target/microsoft/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/result.py` & `azure-quantum-0.28.291394/azure/quantum/target/microsoft/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/target.py` & `azure-quantum-0.28.291394/azure/quantum/target/microsoft/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/params.py` & `azure-quantum-0.28.291394/azure/quantum/target/params.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/quantinuum.py` & `azure-quantum-0.28.291394/azure/quantum/target/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/result.py` & `azure-quantum-0.28.291394/azure/quantum/target/rigetti/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/target.py` & `azure-quantum-0.28.291394/azure/quantum/target/rigetti/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/solvers.py` & `azure-quantum-0.28.291394/azure/quantum/target/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/target.py` & `azure-quantum-0.28.291394/azure/quantum/target/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/target_factory.py` & `azure-quantum-0.28.291394/azure/quantum/target/target_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/solvers.py` & `azure-quantum-0.28.291394/azure/quantum/target/toshiba/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure/quantum/workspace.py` & `azure-quantum-0.28.291394/azure/quantum/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure_quantum.egg-info/PKG-INFO` & `azure-quantum-0.28.291394/azure_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 0.28.291393b1
+Version: 0.28.291394
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/qdk-python
 Author: Microsoft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `azure-quantum-0.28.291393b1/azure_quantum.egg-info/SOURCES.txt` & `azure-quantum-0.28.291394/azure_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/azure_quantum.egg-info/requires.txt` & `azure-quantum-0.28.291394/azure_quantum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.291393b1/setup.py` & `azure-quantum-0.28.291394/setup.py`

 * *Files identical despite different names*

