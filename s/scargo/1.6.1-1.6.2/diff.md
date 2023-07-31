# Comparing `tmp/scargo-1.6.1.tar.gz` & `tmp/scargo-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.6.1.tar", last modified: Wed Jul 19 10:03:34 2023, max compression
+gzip compressed data, was "scargo-1.6.2.tar", last modified: Mon Jul 31 11:57:05 2023, max compression
```

## Comparing `scargo-1.6.1.tar` & `scargo-1.6.2.tar`

### file list

```diff
@@ -1,96 +1,103 @@
--rw-r--r--   0        0        0     4508 2023-07-19 10:03:29.503412 scargo-1.6.1/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-07-19 10:03:29.503412 scargo-1.6.1/LICENSE
--rw-r--r--   0        0        0     2494 2023-07-19 10:03:29.503412 scargo-1.6.1/README.md
--rw-r--r--   0        0        0     2748 2023-07-19 10:03:29.515412 scargo-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/__init__.py
--rwxr-xr-x   0        0        0    19734 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     5226 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      698 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/clang_utils.py
--rw-r--r--   0        0        0    12830 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1767 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/build.py
--rw-r--r--   0        0        0    12319 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/check.py
--rw-r--r--   0        0        0     1142 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/clean.py
--rw-r--r--   0        0        0     4168 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/debug.py
--rw-r--r--   0        0        0     3402 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/doc.py
--rw-r--r--   0        0        0     3918 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/fix.py
--rw-r--r--   0        0        0     3835 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/flash.py
--rw-r--r--   0        0        0     6677 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/gen.py
--rw-r--r--   0        0        0     2857 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/new.py
--rw-r--r--   0        0        0     3405 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/publish.py
--rw-r--r--   0        0        0     1688 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/run.py
--rw-r--r--   0        0        0     3651 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/test.py
--rw-r--r--   0        0        0     4553 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/version.py
--rw-r--r--   0        0        0     6707 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/config.py
--rw-r--r--   0        0        0     2255 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/config_utils.py
--rw-r--r--   0        0        0     2290 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/docker_utils.py
--rw-r--r--   0        0        0       86 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1658 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0      441 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0       86 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/__init__.py
--rw-r--r--   0        0        0     2251 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/data_classes.py
--rw-r--r--   0        0        0     1197 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/header_parser.py
--rw-r--r--   0        0        0     2385 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/params_extractor.py
--rw-r--r--   0        0        0      395 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0      940 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     2468 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3186 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     1607 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0      454 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0     4834 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1067 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4275 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     1865 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1464 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0     2192 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/conan/profile.j2
--rw-r--r--   0        0        0      150 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     2423 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      886 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      159 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2128 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0      754 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0       49 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2363 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      158 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0     1000 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/stm32.cfg.j2
--rw-r--r--   0        0        0      294 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/esp32.cmake.j2
--rw-r--r--   0        0        0       39 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0      594 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0      835 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0      470 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/project.cmake.j2
--rw-r--r--   0        0        0     2228 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0      227 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/stm32.cmake.j2
--rw-r--r--   0        0        0       91 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1079 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      716 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0      213 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/x86.cmake.j2
--rw-r--r--   0        0        0     1597 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      550 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     5357 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0      629 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/global_values.py
--rw-r--r--   0        0        0     2044 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/logger.py
--rw-r--r--   0        0        0     1137 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/LICENSE
--rw-r--r--   0        0        0      519 2023-07-19 10:03:29.519412 scargo-1.6.1/setup.cfg
--rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 scargo-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-07-31 11:56:59.364710 scargo-1.6.2/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-07-31 11:56:59.364710 scargo-1.6.2/LICENSE
+-rw-r--r--   0        0        0     2494 2023-07-31 11:56:59.364710 scargo-1.6.2/README.md
+-rw-r--r--   0        0        0     2748 2023-07-31 11:56:59.380711 scargo-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19734 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     4629 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      698 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12896 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     1854 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/build.py
+-rw-r--r--   0        0        0    12319 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/check.py
+-rw-r--r--   0        0        0     1142 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4168 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3402 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3872 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3835 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6677 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/gen.py
+-rw-r--r--   0        0        0     2996 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/new.py
+-rw-r--r--   0        0        0     3649 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/run.py
+-rw-r--r--   0        0        0     3651 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/test.py
+-rw-r--r--   0        0        0     4553 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/version.py
+-rw-r--r--   0        0        0     7288 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/config.py
+-rw-r--r--   0        0        0     2255 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/config_utils.py
+-rw-r--r--   0        0        0     2290 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1658 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2385 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0     2049 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2602 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4834 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1221 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     2232 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1539 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      287 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile.j2
+-rw-r--r--   0        0        0     1079 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile_esp32.j2
+-rw-r--r--   0        0        0     1545 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile_stm32.j2
+-rw-r--r--   0        0        0     1244 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile_x86.j2
+-rw-r--r--   0        0        0      280 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/stm32_gcc_toolchain_wrapper.cmake.j2
+-rw-r--r--   0        0        0      342 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/test_package/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      749 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/test_package/conanfile.py.j2
+-rw-r--r--   0        0        0       59 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/test_package/example.cpp.j2
+-rw-r--r--   0        0        0      150 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     3031 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      879 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      124 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2126 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0      754 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0       49 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2376 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      684 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1105 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      697 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      371 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2228 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      227 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      716 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0       33 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1597 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      550 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      629 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/logger.py
+-rw-r--r--   0        0        0     1137 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      519 2023-07-31 11:56:59.384711 scargo-1.6.2/setup.cfg
+-rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 scargo-1.6.2/PKG-INFO
```

### Comparing `scargo-1.6.1/CODE-OF-CONDUCT.md` & `scargo-1.6.2/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/LICENSE` & `scargo-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/README.md` & `scargo-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/pyproject.toml` & `scargo-1.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/certs/certGen.sh` & `scargo-1.6.2/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/certs/generateAllCertificates.sh` & `scargo-1.6.2/scargo/certs/generateAllCertificates.sh`

 * *Files 12% similar despite different names*

```diff
@@ -83,46 +83,31 @@
     exit
     fi
 
 
 mkdir -p ${OUTPUT_DIR}
 
 #Download CA certificate for IoT Hub
-BALTIMORE_CERT=${OUTPUT_DIR}/baltimore.pem
 DIGIROOT_CERT=${OUTPUT_DIR}/digiroot.pem
 CA_PEM=${OUTPUT_DIR}/ca.pem
 
-rm -f ${OUTPUT_DIR}/ca.pem
-
-if [ -f "$BALTIMORE_CERT" ]; then
-    echo "$BALTIMORE_CERT already exists."
-else
-    wget https://cacerts.digicert.com/BaltimoreCyberTrustRoot.crt.pem -O ${OUTPUT_DIR}/baltimore.pem
-    if [ $? -ne 0 ]; then
-        echo -e "${RED} Failed to download Baltimore certificate" >&2
-        rm ${OUTPUT_DIR}/baltimore.pem
-        exit 1
-    fi
-fi
+rm -f ${CA_PEM}
 
 if [ -f "$DIGIROOT_CERT" ]; then
     echo "$DIGIROOT_CERT already exists."
 else
-    wget https://cacerts.digicert.com/DigiCertGlobalRootG2.crt.pem -O ${OUTPUT_DIR}/digiroot.pem
+    wget https://cacerts.digicert.com/DigiCertGlobalRootG2.crt.pem -O ${DIGIROOT_CERT}
     if [ $? -ne 0 ]; then
         echo -e "${RED} Failed to download Digiroot certificate" >&2
-        rm ${OUTPUT_DIR}/digiroot.pem
+        rm ${DIGIROOT_CERT}
         exit 1
     fi
 fi
 
-cat ${OUTPUT_DIR}/baltimore.pem >> ${OUTPUT_DIR}/ca_temp.pem
-cat ${OUTPUT_DIR}/digiroot.pem >> ${OUTPUT_DIR}/ca_temp.pem
-grep . ${OUTPUT_DIR}/ca_temp.pem > ${OUTPUT_DIR}/ca.pem
-rm -f ${OUTPUT_DIR}/ca_temp.pem
+cp ${DIGIROOT_CERT} ${CA_PEM}
 
 if [ ${MODE} == "Device-certificate" ]; then
     #Generate only device cert
     CERT_DIR=${INPUT_DIR:="/workspace/build/certs"}
     ${SCRIPT_DIR}/certGen.sh --create_device_certificate_from_intermediate ${DEVICE_NAME} ${CERT_DIR} \
         --output ${OUTPUT_DIR} \
         --password ${PASSWD}
```

### Comparing `scargo-1.6.1/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.6.2/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/certs/openssl_root_ca.cnf` & `scargo-1.6.2/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/clang_utils.py` & `scargo-1.6.2/scargo/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/cli.py` & `scargo-1.6.2/scargo/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,20 +361,21 @@
 
 ###############################################################################
 
 
 @cli.command()
 def publish(
     repo: str = Option("", "--repo", "-r", help="Repo name"),
+    profile: str = Option("Release", "--profile", "-p"),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
     """Upload conan pkg to repo"""
     if base_dir:
         os.chdir(base_dir)
-    scargo_publish(repo)
+    scargo_publish(repo, profile)
 
 
 ###############################################################################
 
 
 @cli.command()
 def run(
```

### Comparing `scargo-1.6.1/scargo/commands/build.py` & `scargo-1.6.2/scargo/commands/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,18 +53,24 @@
                 ".",
                 "-if",
                 build_dir,
                 "-pr:b",
                 "default",
                 "-pr:h",
                 f"./.conan/profiles/{config.project.target.family}_{profile}",
+                "-b",
+                "missing",
             ],
             cwd=project_dir,
         )
         subprocess.check_call(
-            ["conan", "build", ".", "-if", build_dir, "-bf", build_dir],
-            cwd=project_dir,
+            [
+                "conan",
+                "build",
+                f"{project_dir}",
+            ],
+            cwd=build_dir,
         )
 
     except subprocess.CalledProcessError:
         logger.error("Unable to build exec file")
         sys.exit(1)
```

### Comparing `scargo-1.6.1/scargo/commands/check.py` & `scargo-1.6.2/scargo/commands/check.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/clean.py` & `scargo-1.6.2/scargo/commands/clean.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/debug.py` & `scargo-1.6.2/scargo/commands/debug.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/doc.py` & `scargo-1.6.2/scargo/commands/doc.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/docker.py` & `scargo-1.6.2/scargo/commands/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,17 @@
     Build docker
 
     :param docker_opts: additional docker options
     :param project_root
     :raises CalledProcessError: if docker build fail
     """
     logger.debug("Build docker environment.")
-    print(docker_opts)
     if not project_root:
         project_root = get_scargo_config_or_exit().project_root
     docker_path = _get_docker_path(project_root)
-    print(docker_path)
 
     cmd = get_docker_compose_command()
     cmd.extend(["build", *docker_opts])
 
     try:
         subprocess.run(cmd, cwd=docker_path, check=True)
         logger.info("Initialize docker environment.")
```

### Comparing `scargo-1.6.1/scargo/commands/fix.py` & `scargo-1.6.2/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/flash.py` & `scargo-1.6.2/scargo/commands/flash.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/gen.py` & `scargo-1.6.2/scargo/commands/gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/new.py` & `scargo-1.6.2/scargo/commands/new.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import sys
 from pathlib import Path
 from typing import Optional
 
 from scargo import __version__
 from scargo.config import Target
 from scargo.config_utils import get_scargo_config_or_exit
+from scargo.file_generators.conan_gen import generate_test_package
 from scargo.file_generators.cpp_gen import generate_cpp
 from scargo.file_generators.toml_gen import generate_toml
 from scargo.global_values import SCARGO_DEFAULT_CONFIG_FILE, SCARGO_DOCKER_ENV
 from scargo.logger import get_logger
 
 logger = get_logger()
 
@@ -73,14 +74,16 @@
         docker_image_tag=f"{name.lower()}-dev:1.0",
         lib_name=lib_name,
         bin_name=bin_name,
     )
 
     config = get_scargo_config_or_exit(toml_path)
     generate_cpp(config)
+    if lib_name and not bin_name:
+        generate_test_package(config)
 
     test_dir = project_dir / "tests"
     Path(test_dir, "mocks").mkdir(parents=True)
     Path(test_dir, "ut").mkdir(parents=True)
     Path(test_dir, "it").mkdir(parents=True)
 
     if git:
```

### Comparing `scargo-1.6.1/scargo/commands/publish.py` & `scargo-1.6.2/scargo/commands/publish.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,49 +12,58 @@
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 
 logger = get_logger()
 
 
-def scargo_publish(repo: str) -> None:
+def scargo_publish(repo: str, profile: str = "Release") -> None:
     """
     Publish conan package
 
     :param str repo: repository name
     :return: None
     """
     config = prepare_config()
     project_path = config.project_root
     project_config = config.project
     project_name = project_config.name
-    version = project_config.version
 
     conan_clean_remote()
     conan_add_remote(project_path, config)
     conan_add_conancenter()
 
     # Export package
     try:
         subprocess.check_call(
-            "conan export-pkg . -f",
+            [
+                "conan",
+                "create",
+                ".",
+                "-pr:b",
+                "default",
+                "-pr:h",
+                f"./.conan/profiles/{config.project.target.family}_{profile}",
+                "-b",
+                "missing",
+            ],
             cwd=project_path,
-            shell=True,
         )
     except subprocess.CalledProcessError:
         logger.error("Unable to create package")
+        sys.exit(1)
 
     # Upload package to artifactory
     conan_repo = ["-r", repo] if repo else []
     try:
         subprocess.check_call(
             [
                 "conan",
                 "upload",
-                f"{project_name}/{version}",
+                f"{project_name}",
                 *conan_repo,
                 "--all",
                 "--confirm",
             ],
             cwd=project_path,
         )
     except subprocess.CalledProcessError:
```

### Comparing `scargo-1.6.1/scargo/commands/run.py` & `scargo-1.6.2/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/test.py` & `scargo-1.6.2/scargo/commands/test.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/commands/update.py` & `scargo-1.6.2/scargo/commands/update.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/config.py` & `scargo-1.6.2/scargo/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     )
     project_root: Path
 
     @property
     def source_dir_path(self) -> Path:
         return self.project_root / self.project.target.source_dir
 
+    @property
+    def include_dir_path(self) -> Path:
+        return self.project_root / self.project.target.include_dir
+
     def get_stm32_config(self) -> "Stm32Config":
         if not self.stm32:
             raise ConfigError("No [stm32] section in config")
         return self.stm32
 
     def get_esp32_config(self) -> "Esp32Config":
         if not self.esp32:
@@ -100,42 +104,65 @@
         return None
 
 
 class Target(BaseModel):
     id: str
     family: str
     source_dir: str
+    include_dir: str
     cc: Optional[str] = None
     cxx: Optional[str] = None
 
     @classmethod
     def get_target_by_id(cls, target_id: str) -> "Target":
         return TARGETS[target_id]
 
 
 TARGETS = {
-    "x86": Target(id="x86", family="x86", source_dir="src", cc="gcc", cxx="g++"),
-    "stm32": Target(id="stm32", family="stm32", source_dir="src"),
-    "esp32": Target(id="esp32", family="esp32", source_dir="main"),
-    "esp32s2": Target(id="esp32s2", family="esp32", source_dir="main"),
-    "esp32s3": Target(id="esp32s3", family="esp32", source_dir="main"),
-    "esp32c2": Target(id="esp32c2", family="esp32", source_dir="main"),
-    "esp32c3": Target(id="esp32c3", family="esp32", source_dir="main"),
+    "x86": Target(
+        id="x86",
+        family="x86",
+        source_dir="src",
+        include_dir="include",
+        cc="gcc",
+        cxx="g++",
+    ),
+    "stm32": Target(
+        id="stm32", family="stm32", source_dir="src", include_dir="include"
+    ),
+    "esp32": Target(
+        id="esp32", family="esp32", source_dir="main", include_dir="include"
+    ),
+    "esp32s2": Target(
+        id="esp32s2", family="esp32", source_dir="main", include_dir="include"
+    ),
+    "esp32s3": Target(
+        id="esp32s3", family="esp32", source_dir="main", include_dir="include"
+    ),
+    "esp32c2": Target(
+        id="esp32c2", family="esp32", source_dir="main", include_dir="include"
+    ),
+    "esp32c3": Target(
+        id="esp32c3", family="esp32", source_dir="main", include_dir="include"
+    ),
 }
 
 
 # for typer
 ScargoTargets = Enum(  # type: ignore[misc]
     "ScargoTargets", {target.id: target.id for target in TARGETS.values()}
 )
 
 
 class ProfileConfig(BaseModel, extra=Extra.allow):
     cflags: Optional[str]
     cxxflags: Optional[str]
+    cc: Optional[str] = None
+    cxx: Optional[str] = None
+    cmake_build_type: Optional[str] = Field("Debug", alias="cmake-build-type")
 
     @property
     def extras(self) -> Dict[str, Any]:
         return {
             key: value
             for key, value in dict(self).items()
             if key not in self.__fields__
```

### Comparing `scargo-1.6.1/scargo/config_utils.py` & `scargo-1.6.2/scargo/config_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/docker_utils.py` & `scargo-1.6.2/scargo/docker_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/base_gen.py` & `scargo-1.6.2/scargo/file_generators/base_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/clang_parser/data_classes.py` & `scargo-1.6.2/scargo/file_generators/clang_parser/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/clang_parser/header_parser.py` & `scargo-1.6.2/scargo/file_generators/clang_parser/header_parser.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/clang_parser/params_extractor.py` & `scargo-1.6.2/scargo/file_generators/clang_parser/params_extractor.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/cpp_gen.py` & `scargo-1.6.2/scargo/file_generators/cpp_gen.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
     This class is a container cpp files creation with multilayer approach
     """
 
     def __init__(self, config: Config) -> None:
         self._config = config
         self._src_dir = config.source_dir_path
+        self._inc_dir = config.include_dir_path
 
     def _generate_bin(self, bin_name: str) -> None:
         """Function which creates main.cpp file using jinja"""
         self._create_file_from_template(
             "cpp/main.cpp.j2",
             f"{bin_name.lower()}.cpp",
             template_params={
@@ -29,23 +30,25 @@
 
     def _generate_lib(self, lib_name: str) -> None:
         """Function which creates a lib files using jinja"""
 
         lib_name = lib_name.lower()
         class_name = "".join(lib_name.replace("_", " ").title().split())
 
-        self._create_file_from_template(
+        create_file_from_template(
             "cpp/lib.cpp.j2",
-            f"{lib_name}.cpp",
+            self._src_dir / f"{lib_name}.cpp",
             template_params={"class_name": class_name, "lib_name": lib_name},
+            config=self._config,
         )
-        self._create_file_from_template(
+        create_file_from_template(
             "cpp/lib.h.j2",
-            f"{lib_name}.h",
+            self._inc_dir / f"{lib_name}.h",
             template_params={"class_name": class_name},
+            config=self._config,
         )
 
     def _generate_cmake(self) -> None:
         self._create_file_from_template(
             f"cpp/cmake-src-{self._config.project.target.family}.j2",
             "CMakeLists.txt",
             template_params={"config": self._config},
```

### Comparing `scargo-1.6.1/scargo/file_generators/docker_gen.py` & `scargo-1.6.2/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/env_gen.py` & `scargo-1.6.2/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/mock_gen.py` & `scargo-1.6.2/scargo/file_generators/mock_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-1.6.2/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-1.6.2/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files 18% similar despite different names*

```diff
@@ -2,42 +2,40 @@
 # Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 #
 # DO NOT EDIT THIS FILE!
 # This file is generated by `scargo update`.
 #
-{% if config.project.target.family == "esp32" %}
-cmake_minimum_required(VERSION 3.14)
-{% else %}
-cmake_minimum_required(VERSION 3.16)
+cmake_minimum_required(VERSION 3.22)
+
+list(APPEND CMAKE_PREFIX_PATH "${CMAKE_BINARY_DIR}/generators/")
+{% if config.project.target.family != 'esp32' %}
+set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
 {% endif %}
+set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
 {% if config.project.target.family == 'stm32' %}
 {% include 'stm32.cmake.j2' %}
 {% elif config.project.target.family == 'x86' %}
 {% include 'x86.cmake.j2' %}
+{% elif config.project.target.family == "esp32" %}
+{% include 'esp32.cmake.j2' %}
 {% endif %}
 
-set(CMAKE_CXX_STANDARD {{ config.project.cxxstandard }})
-
 {% for key, value in config.project.cmake_variables.items() %}
 set({{ key }} "{{ value }}")
 {% endfor %}
-
 {% for profile_name, profile in config.profiles.items() %}
     {% if profile.extras %}
 # {{ profile_name }}
 IF("${CMAKE_BUILD_TYPE}" STREQUAL "{{ profile_name }}")
         {% for key, value in profile.extras.items() %}
     SET({{ key }} {{ value }})
         {% endfor %}
 ENDIF()
     {% endif %}
-
 {% endfor %}
 
-{% if config.project.target.family == "esp32" %}
-{% include 'esp32.cmake.j2' %}
-{% else %}
-add_subdirectory(src)
+{% if config.project.target.family != "esp32" %}
+add_subdirectory({{ config.source_dir_path.relative_to(config.project_root) }})
 {% endif %}
```

### Comparing `scargo-1.6.1/scargo/file_generators/templates/README.md.j2` & `scargo-1.6.2/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-1.6.2/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,28 @@
+#
+# DO NOT EDIT THIS FILE!
+# This file is generated by `scargo update`.
+#
+
 from conan import ConanFile
-from conan.tools.cmake import CMakeToolchain, CMake
-from conans import tools  # type: ignore[misc, no-any-unimported]
+from conan.tools.cmake import CMakeToolchain, CMake, cmake_layout
+
+{% if config.project.target.family == "stm32" %}
+from conans import tools
+{% endif %}
 
 class {{ config.project.name|capitalize|replace("-", "") }}Conan(ConanFile):  # type: ignore[misc, no-any-unimported]
     name = "{{ config.project.name }}"
     version = "{{ config.project.version }}"
-    settings = "os", "compiler", "build_type", "arch"
+    license = "MIT"
     description = "{{ config.project.description }}"
+    settings = "os", "compiler", "build_type", "arch"
     url = "{{ config.project.homepage_url }}"
     generators = "CMakeDeps"
-    exports_sources = "src/*", "CMakeLists.txt"
-
-    def generate(self):
-        tc = CMakeToolchain(self)
-        tc.generate()
-
-    def package(self) -> None:
-        self.copy("*", src='build/Debug/bin/', dst='bin', keep_path=False)
-        self.copy("*", src='build/Debug/lib/', dst='lib', keep_path=False)
-
-    def package_info(self) -> None:
-        self.cpp_info.libs = tools.collect_libs(self)
-
-    def build(self) -> None:
-        cmake = CMake(self)
-        cmake.configure()
-        cmake.build()
-
-    def source(self) -> None:
-        {% if config.project.target.family == "stm32" %}
-        git = tools.Git(folder="third-party/stm32-cmake")
-        git.clone("https://github.com/ObKo/stm32-cmake.git", "master")
-        {% else %}
-        pass
-        {% endif %}
+    exports_sources = ["{{ config.source_dir_path.relative_to(config.project_root) }}/*", "CMakeLists.txt", "include/*", "config/*"]
 
     {% if config.dependencies.build or config.dependencies.tool %}
     def build_requirements(self) -> None:
         {% for dep in config.dependencies.build %}
         self.requires("{{ dep }}")
         {% endfor %}
         {% for tool_dep in config.dependencies.tool %}
@@ -47,7 +32,44 @@
     {% endif %}
     {% if config.dependencies.general %}
     def requirements(self) -> None:
         {% for dep in config.dependencies.general %}
         self.requires("{{ dep }}")
         {% endfor %}
     {% endif %}
+
+    {% if config.project.target.family == "stm32" %}
+    def source(self) -> None:
+        git = tools.Git(folder="third-party/stm32-cmake")
+        git.clone("https://github.com/ObKo/stm32-cmake.git", "master")
+    {% endif %}
+
+    def layout(self):
+        cmake_layout(self)
+
+    def generate(self):
+        tc = CMakeToolchain(self)
+        tc.generate()
+
+    def build(self) -> None:
+        cmake = CMake(self)
+        cmake.configure()
+        cmake.build()
+
+    def package(self) -> None:
+        {% if config.project.lib_name %}
+        cmake = CMake(self)
+        cmake.install()
+        {% endif %}
+        {% if config.project.bin_name %}
+        self.copy("*.bin")
+        self.copy("*.elf")
+        {% endif %}
+
+    {% if config.project.lib_name %}
+    def package_info(self) -> None:
+        self.cpp_info.libs = ["{{ config.project.name }}"]
+    {% endif %}
+
+  
+
+
```

### Comparing `scargo-1.6.1/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-1.6.2/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#
+# DO NOT EDIT THIS FILE!
+# This file is generated by `scargo update`.
+#
+
 from conans import CMake, ConanFile, tools  # type: ignore[import]
 
 
 class {{ config.project.name|capitalize|replace("-", "") }}TestConan(ConanFile):  # type: ignore[misc, no-any-unimported]
     name = "{{ config.project.name }}_test"
     version = "{{ config.project.version }}"
     settings = "os", "compiler", "build_type", "arch"
```

### Comparing `scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files 24% similar despite different names*

```diff
@@ -16,17 +16,23 @@
 
 
 {% if  config.project.bin_name %}
 add_executable(${PROJECT_NAME}
      {{ config.project.bin_name|lower }}.cpp
 )
 {% elif config.project.lib_name%}
-add_library(${PROJECT_NAME}
-     {{ config.project.lib_name|lower }}.cpp
-     {{ config.project.lib_name|lower }}.h
+add_library(${PROJECT_NAME} STATIC
+    ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.include_dir_path.relative_to(config.project_root) }}/{{ config.project.lib_name|lower }}.h
+)
+
+target_include_directories(${PROJECT_NAME}
+    PUBLIC
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.include_dir_path.relative_to(config.project_root) }}
+    PRIVATE
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.source_dir_path.relative_to(config.project_root) }}
 )
 {% endif %}
 
 target_link_libraries(${PROJECT_NAME}
     CMSIS::STM32::${STM32_DEVICE}
     # HAL::STM32::${STM32_FAMILY}
     STM32::NoSys
@@ -63,7 +69,11 @@
     TARGET ${PROJECT_NAME}
     POST_BUILD
     COMMAND ${CMAKE_OBJCOPY} -O ihex $<TARGET_FILE:${PROJECT_NAME}> ${CMAKE_RUNTIME_OUTPUT_DIRECTORY}/${PROJECT_NAME}.hex
     BYPRODUCTS ${PROJECT_NAME}.hex
     COMMENT "Generating hex file ${CMAKE_PROJECT_NAME}.hex"
 )
 {% endif %}
+{% if config.project.lib_name %}
+install(TARGETS ${PROJECT_NAME} DESTINATION lib)
+install(DIRECTORY {{ config.include_dir_path.relative_to(config.project_root) }}/ DESTINATION {{ config.include_dir_path.relative_to(config.project_root) }})
+{% endif %}
```

### Comparing `scargo-1.6.1/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-1.6.2/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 ARG ESPRESSIF_IDF_TAG="v4.4.3"
 ARG ESPRESSIF_IDF_VERSION="${ESPRESSIF_IDF_TAG}"
 ARG ESPRESSIF_IDF_PATH="/opt/esp-idf"
 ARG ESPRESSIF_IDF_REPO_URL="https://github.com/espressif/esp-idf.git"
 ARG ESPRESSIF_TOOLS_PATH="/root/.espressif"
 ARG RUN_CLANG_TIDY_SCRIPT_URL="https://raw.githubusercontent.com/llvm/llvm-project/llvmorg-16.0.0/clang-tools-extra/clang-tidy/tool/run-clang-tidy.py"
-ENV  IDF_TOOLS_PATH ${ESPRESSIF_IDF_PATH}
-ENV  IDF_PATH ${ESPRESSIF_IDF_PATH}
+ENV IDF_TOOLS_PATH ${ESPRESSIF_IDF_PATH}
+ENV IDF_PATH ${ESPRESSIF_IDF_PATH}
 
 WORKDIR /opt
 
 RUN umask 0002 && git clone --single-branch --branch ${ESPRESSIF_IDF_VERSION} --recursive ${ESPRESSIF_IDF_REPO_URL} ${ESPRESSIF_IDF_PATH}
 RUN umask 0002 && ${ESPRESSIF_IDF_PATH}/install.sh
 RUN umask 0002 && ${ESPRESSIF_IDF_PATH}/tools/idf_tools.py install xtensa-clang
```

### Comparing `scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-stm32.j2` & `scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     apt -y install sudo && \
     rm -rf /var/lib/apt/lists/* && \
     update-alternatives --install /usr/bin/python python /usr/bin/python3 1
 
 FROM base AS cpp
 
 RUN apt update --fix-missing && apt -y --no-install-recommends install cppcheck lib32z1 \
-    make cmake clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev gdb && \
+    make cmake clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev gdb screen && \
     rm -rf /var/lib/apt/lists/*
 
 FROM cpp AS {{ project.target.family }}
 {% include 'docker/Dockerfile-' + project.target.family + '.j2' %}
 
 WORKDIR /opt
 
@@ -31,17 +31,17 @@
 FROM custom_{{ project.name }} AS {{ project.name }}_dev
 
 ARG USER_NAME=user
 ARG USER_PASSWORD=user
 ARG UID_NUMBER=1000
 ARG GID_NUMBER=1000
 ARG SSH_PORT=2000
+ARG CONAN_LOGIN_USERNAME=""
+ARG CONAN_PASSWORD=""
 
-ARG CONAN_LOGIN_USERNAME
-ARG CONAN_PASSWORD
 ENV CONAN_LOGIN_USERNAME=${CONAN_LOGIN_USERNAME}
 ENV CONAN_PASSWORD=${CONAN_PASSWORD}
 
 WORKDIR /opt
 
 # configure ssh
 RUN apt update --fix-missing && apt install -y --no-install-recommends openssh-server && \
```

### Comparing `scargo-1.6.1/scargo/file_generators/templates/mock/class_interface.h.j2` & `scargo-1.6.2/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.cpp.j2` & `scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/scargo.toml.j2` & `scargo-1.6.2/scargo/file_generators/templates/scargo.toml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-1.6.2/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-1.6.2/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-1.6.2/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/tests_gen.py` & `scargo-1.6.2/scargo/file_generators/tests_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/toml_gen.py` & `scargo-1.6.2/scargo/file_generators/toml_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/file_generators/ut_gen.py` & `scargo-1.6.2/scargo/file_generators/ut_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/global_values.py` & `scargo-1.6.2/scargo/global_values.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/logger.py` & `scargo-1.6.2/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/path_utils.py` & `scargo-1.6.2/scargo/path_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/templates/.clang-format` & `scargo-1.6.2/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/templates/.clang-tidy` & `scargo-1.6.2/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/templates/.gitignore` & `scargo-1.6.2/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/scargo/templates/LICENSE` & `scargo-1.6.2/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/setup.cfg` & `scargo-1.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-1.6.1/PKG-INFO` & `scargo-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.6.1
+Version: 1.6.2
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

