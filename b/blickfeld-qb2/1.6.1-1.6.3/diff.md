# Comparing `tmp/blickfeld_qb2-1.6.1.tar.gz` & `tmp/blickfeld_qb2-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blickfeld_qb2-1.6.1.tar", last modified: Tue Jul  4 14:50:04 2023, max compression
+gzip compressed data, was "blickfeld_qb2-1.6.3.tar", last modified: Wed Jul 26 06:27:17 2023, max compression
```

## Comparing `blickfeld_qb2-1.6.1.tar` & `blickfeld_qb2-1.6.3.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2023-07-04 14:49:59.000000 blickfeld_qb2-1.6.1/LICENSE.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/PKG-INFO
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      312 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4372 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2420 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/geometry/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2943 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/geometry/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3682 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/channel.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/device_ca_cert.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      796 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1045 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4181 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    55060 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/_types.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/_version.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/casing.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/importing.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/naming.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_client.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_server.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/async_channel.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/__main__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/compiler.py
--rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/main.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)    28668 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/models.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7461 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/parser.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1515 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    12345 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    16869 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      746 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4015 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      985 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1935 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5067 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      699 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3487 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      635 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3881 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10016 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3024 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    26328 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6137 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    16640 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      755 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10428 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2919 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2328 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    15032 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10089 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4591 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    27697 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/PKG-INFO
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3168 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/SOURCES.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/dependency_links.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/requires.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/top_level.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/setup.cfg
--rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/setup.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2023-07-26 06:27:10.000000 blickfeld_qb2-1.6.3/LICENSE.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/PKG-INFO
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      312 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/base/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4372 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/base/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/base/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2420 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/base/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/base/geometry/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2943 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/base/geometry/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/base/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/base/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3682 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/base/grpc/channel.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/base/grpc/device_ca_cert.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      796 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1045 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4181 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    55060 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/_types.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/_version.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/casing.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/compile/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/compile/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/compile/importing.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/compile/naming.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/grpclib_client.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/grpclib_server.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/util/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/util/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/util/async_channel.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/protobuf/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/__main__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/compiler.py
+-rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/main.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    28668 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/models.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7461 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/parser.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1515 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    12345 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    16869 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/detector/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/detector/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/detector/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      746 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/detector/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/detector/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4015 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/detector/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      985 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1935 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5067 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      699 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3487 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/laser/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/laser/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/laser/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      635 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/laser/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/laser/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3881 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/laser/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10016 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3024 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    26328 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6137 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    16640 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      755 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10428 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/push/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/push/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/push/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2919 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/push/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/push/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2328 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/push/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/push/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    15032 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/push/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/system/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/system/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/system/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10089 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/system/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/system/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4591 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/system/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/blickfeld_qb2/system/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    27697 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/blickfeld_qb2/system/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-26 06:27:17.657166 blickfeld_qb2-1.6.3/blickfeld_qb2.egg-info/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-07-26 06:27:17.000000 blickfeld_qb2-1.6.3/blickfeld_qb2.egg-info/PKG-INFO
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3168 2023-07-26 06:27:17.000000 blickfeld_qb2-1.6.3/blickfeld_qb2.egg-info/SOURCES.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2023-07-26 06:27:17.000000 blickfeld_qb2-1.6.3/blickfeld_qb2.egg-info/dependency_links.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2023-07-26 06:27:17.000000 blickfeld_qb2-1.6.3/blickfeld_qb2.egg-info/requires.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2023-07-26 06:27:17.000000 blickfeld_qb2-1.6.3/blickfeld_qb2.egg-info/top_level.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2023-07-26 06:27:17.661167 blickfeld_qb2-1.6.3/setup.cfg
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2023-07-26 06:27:16.000000 blickfeld_qb2-1.6.3/setup.py
```

### Comparing `blickfeld_qb2-1.6.1/LICENSE.txt` & `blickfeld_qb2-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/base/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/base/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/base/geometry/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/base/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/channel.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/base/grpc/channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/device_ca_cert.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/base/grpc/device_ca_cert.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/config/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/beam_deflection_control/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/casing.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/casing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/importing.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_client.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_server.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/async_channel.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/compiler.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/main.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/models.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/models.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/parser.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/betterproto/plugin/parser.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/config/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/core_processing/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/detector/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/detector/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/detector/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/detector/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/config/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/diagnostics/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/config/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/hardware/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/laser/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/laser/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/laser/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/laser/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/config/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/percept_pipeline/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/percept_processing/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/percept_toolkit/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/push/config/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/push/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/push/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/push/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/push/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/push/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/system/config/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/system/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/system/data/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/system/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2/system/services/__init__.py` & `blickfeld_qb2-1.6.3/blickfeld_qb2/system/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/SOURCES.txt` & `blickfeld_qb2-1.6.3/blickfeld_qb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.6.1/setup.py` & `blickfeld_qb2-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="blickfeld_qb2",
-    version="1.6.1",
+    version="1.6.3",
     author="Blickfeld GmbH",
     author_email="opensource@blickfeld.com",
     url="https://github.com/Blickfeld/blickfeld-qb2",
     description="Python package to communicate securely with Qb2 LiDAR devices of the Blickfeld GmbH",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

