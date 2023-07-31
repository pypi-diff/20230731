# Comparing `tmp/cryo_python-0.1.0.tar.gz` & `tmp/cryo_python-0.1.1.tar.gz`

## Comparing `cryo_python-0.1.0.tar` & `cryo_python-0.1.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/Cargo.toml
--rw-rw-r--   0     1001     1002      646 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/collect.rs
--rw-rw-r--   0     1001     1002     1556 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs
--rw-rw-r--   0     1001     1002    15170 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/blocks.rs
--rw-rw-r--   0     1001     1002     2834 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/blocks_and_transactions.rs
--rw-rw-r--   0     1001     1002     1541 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs
--rw-rw-r--   0     1001     1002     8279 2023-07-26 21:22:52.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/logs.rs
--rw-rw-r--   0     1001     1002      184 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/mod.rs
--rw-rw-r--   0     1001     1002     1546 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs
--rw-rw-r--   0     1001     1002    20155 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs
--rw-rw-r--   0     1001     1002     1618 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs
--rw-rw-r--   0     1001     1002    20921 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/traces.rs
--rw-rw-r--   0     1001     1002     2510 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/transactions.rs
--rw-rw-r--   0     1001     1002     7794 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs
--rw-rw-r--   0     1001     1002     5620 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/freeze.rs
--rw-rw-r--   0     1001     1002      428 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/lib.rs
--rw-rw-r--   0     1001     1002     1192 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs
--rw-rw-r--   0     1001     1002     1222 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs
--rw-rw-r--   0     1001     1002     1999 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs
--rw-rw-r--   0     1001     1002      260 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/mod.rs
--rw-rw-r--   0     1001     1002     3216 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs
--rw-rw-r--   0     1001     1002     1809 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs
--rw-rw-r--   0     1001     1002     1516 2023-07-26 18:58:33.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/conversions.rs
--rw-rw-r--   0     1001     1002      770 2023-07-26 18:25:02.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs
--rw-rw-r--   0     1001     1002     2755 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/dataframes/export.rs
--rw-rw-r--   0     1001     1002      117 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/dataframes/mod.rs
--rw-rw-r--   0     1001     1002      505 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/dataframes/sort.rs
--rw-rw-r--   0     1001     1002       61 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/datatypes/mod.rs
--rw-rw-r--   0     1001     1002     3609 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs
--rw-rw-r--   0     1001     1002     4013 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs
--rw-rw-r--   0     1001     1002     2584 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/errors.rs
--rw-rw-r--   0     1001     1002     1556 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/files.rs
--rw-rw-r--   0     1001     1002     1113 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/mod.rs
--rw-rw-r--   0     1001     1002     1583 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/queries.rs
--rw-rw-r--   0     1001     1002     4713 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/schemas.rs
--rw-rw-r--   0     1001     1002     3611 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/sources.rs
--rw-rw-r--   0     1001     1002     2002 2023-07-26 18:58:33.000000 cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/summaries.rs
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/Cargo.toml
--rw-rw-r--   0     1001     1002     8308 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/args.rs
--rw-rw-r--   0     1001     1002      456 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/lib.rs
--rw-rw-r--   0     1001     1002      380 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/main.rs
--rw-rw-r--   0     1001     1002      509 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/args.rs
--rw-rw-r--   0     1001     1002     7031 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/blocks.rs
--rw-rw-r--   0     1001     1002     4845 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/file_output.rs
--rw-rw-r--   0     1001     1002      156 2023-07-26 18:00:26.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/mod.rs
--rw-rw-r--   0     1001     1002     5425 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/query.rs
--rw-rw-r--   0     1001     1002     1999 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/source.rs
--rw-rw-r--   0     1001     1002     1281 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/run.rs
--rw-rw-r--   0     1001     1002     6307 2023-07-26 19:03:06.000000 cryo_python-0.1.0/local_dependencies/cryo_cli/src/summaries.rs
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 cryo_python-0.1.0/Cargo.toml
--rw-rw-r--   0     1001     1002     3124 2023-07-26 18:00:26.000000 cryo_python-0.1.0/.github/workflows/CI.yml
--rw-rw-r--   0     1001     1002      685 2023-07-26 18:00:26.000000 cryo_python-0.1.0/.gitignore
--rw-rw-r--   0     1001     1002      518 2023-07-26 18:00:26.000000 cryo_python-0.1.0/pyproject.toml
--rw-rw-r--   0     1001     1002      171 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python/cryo/__init__.py
--rw-rw-r--   0     1001     1002     1034 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python/cryo/_args.py
--rw-rw-r--   0     1001     1002     1461 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python/cryo/_collect.py
--rw-rw-r--   0     1001     1002     1002 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python/cryo/_freeze.py
--rw-rw-r--   0     1001     1002     1592 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python/cryo/_spec.py
--rw-rw-r--   0     1001     1002      180 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python_tests/test_chunks.py
--rw-rw-r--   0     1001     1002      189 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python_tests/test_columns.py
--rw-rw-r--   0     1001     1002     1190 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python_tests/test_datatypes.py
--rw-rw-r--   0     1001     1002     1433 2023-07-26 18:00:26.000000 cryo_python-0.1.0/python_tests/test_output_formats.py
--rw-rw-r--   0     1001     1002     3336 2023-07-26 19:03:06.000000 cryo_python-0.1.0/src/collect_adapter.rs
--rw-rw-r--   0     1001     1002     3820 2023-07-26 19:03:06.000000 cryo_python-0.1.0/src/freeze_adapter.rs
--rw-rw-r--   0     1001     1002      594 2023-07-26 18:00:26.000000 cryo_python-0.1.0/src/lib.rs
--rw-rw-r--   0     1001     1002   121425 2023-07-26 18:00:26.000000 cryo_python-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 cryo_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/Cargo.toml
+-rw-r--r--   0      502       20     8308 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/args.rs
+-rw-r--r--   0      502       20      456 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/lib.rs
+-rw-r--r--   0      502       20      380 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/main.rs
+-rw-r--r--   0      502       20      509 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/args.rs
+-rw-r--r--   0      502       20     7031 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/blocks.rs
+-rw-r--r--   0      502       20     4845 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/file_output.rs
+-rw-r--r--   0      502       20      156 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/mod.rs
+-rw-r--r--   0      502       20     5425 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/query.rs
+-rw-r--r--   0      502       20     1999 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/source.rs
+-rw-r--r--   0      502       20     1281 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/run.rs
+-rw-r--r--   0      502       20     6307 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/summaries.rs
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/Cargo.toml
+-rw-r--r--   0      502       20      646 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/collect.rs
+-rw-r--r--   0      502       20     1556 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs
+-rw-r--r--   0      502       20    15170 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/blocks.rs
+-rw-r--r--   0      502       20     2834 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/blocks_and_transactions.rs
+-rw-r--r--   0      502       20     1541 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs
+-rw-r--r--   0      502       20     8279 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/logs.rs
+-rw-r--r--   0      502       20      184 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/mod.rs
+-rw-r--r--   0      502       20     1546 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs
+-rw-r--r--   0      502       20    20155 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs
+-rw-r--r--   0      502       20     1618 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs
+-rw-r--r--   0      502       20    20921 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/traces.rs
+-rw-r--r--   0      502       20     2510 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/transactions.rs
+-rw-r--r--   0      502       20     7794 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs
+-rw-r--r--   0      502       20     5620 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/freeze.rs
+-rw-r--r--   0      502       20      428 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/lib.rs
+-rw-r--r--   0      502       20     1192 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs
+-rw-r--r--   0      502       20     1222 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs
+-rw-r--r--   0      502       20     1999 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs
+-rw-r--r--   0      502       20      260 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/mod.rs
+-rw-r--r--   0      502       20     3216 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs
+-rw-r--r--   0      502       20     1809 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs
+-rw-r--r--   0      502       20     1516 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/conversions.rs
+-rw-r--r--   0      502       20      770 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs
+-rw-r--r--   0      502       20     2755 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/export.rs
+-rw-r--r--   0      502       20      117 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/mod.rs
+-rw-r--r--   0      502       20      505 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/sort.rs
+-rw-r--r--   0      502       20       61 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/mod.rs
+-rw-r--r--   0      502       20     3609 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs
+-rw-r--r--   0      502       20     4013 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs
+-rw-r--r--   0      502       20     2584 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/errors.rs
+-rw-r--r--   0      502       20     1556 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/files.rs
+-rw-r--r--   0      502       20     1113 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/mod.rs
+-rw-r--r--   0      502       20     1583 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/queries.rs
+-rw-r--r--   0      502       20     4713 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/schemas.rs
+-rw-r--r--   0      502       20     3611 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/sources.rs
+-rw-r--r--   0      502       20     2002 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/summaries.rs
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 cryo_python-0.1.1/Cargo.toml
+-rw-r--r--   0      502       20     3124 2023-07-29 00:55:34.000000 cryo_python-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0      502       20      685 2023-07-29 00:55:34.000000 cryo_python-0.1.1/.gitignore
+-rw-r--r--   0      502       20       71 2023-07-31 06:19:43.000000 cryo_python-0.1.1/build.rs
+-rw-r--r--   0      502       20      518 2023-07-29 00:55:34.000000 cryo_python-0.1.1/pyproject.toml
+-rw-r--r--   0      502       20      171 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/__init__.py
+-rw-r--r--   0      502       20     1034 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_args.py
+-rw-r--r--   0      502       20     1461 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_collect.py
+-rw-r--r--   0      502       20     1002 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_freeze.py
+-rw-r--r--   0      502       20     1592 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_spec.py
+-rw-r--r--   0      502       20      180 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_chunks.py
+-rw-r--r--   0      502       20      189 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_columns.py
+-rw-r--r--   0      502       20     1190 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_datatypes.py
+-rw-r--r--   0      502       20     1433 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_output_formats.py
+-rw-r--r--   0      502       20     3336 2023-07-29 00:55:34.000000 cryo_python-0.1.1/src/collect_adapter.rs
+-rw-r--r--   0      502       20     3820 2023-07-29 00:55:34.000000 cryo_python-0.1.1/src/freeze_adapter.rs
+-rw-r--r--   0      502       20      594 2023-07-29 00:55:34.000000 cryo_python-0.1.1/src/lib.rs
+-rw-r--r--   0      502       20   121447 2023-07-31 21:49:21.000000 cryo_python-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 cryo_python-0.1.1/PKG-INFO
```

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/Cargo.toml` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/collect.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/collect.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/blocks.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/blocks.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/blocks_and_transactions.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/blocks_and_transactions.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/logs.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/logs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/traces.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/traces.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/transactions.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/transactions.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/freeze.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/freeze.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/conversions.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/conversions.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/dataframes/export.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/export.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/errors.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/errors.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/files.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/files.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/mod.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/queries.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/queries.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/schemas.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/schemas.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/sources.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/sources.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_freeze/src/types/summaries.rs` & `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/summaries.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/Cargo.toml` & `cryo_python-0.1.1/local_dependencies/cryo_cli/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/src/args.rs` & `cryo_python-0.1.1/local_dependencies/cryo_cli/src/args.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/blocks.rs` & `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/blocks.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/file_output.rs` & `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/file_output.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/query.rs` & `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/query.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/src/parse/source.rs` & `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/source.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/src/run.rs` & `cryo_python-0.1.1/local_dependencies/cryo_cli/src/run.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/local_dependencies/cryo_cli/src/summaries.rs` & `cryo_python-0.1.1/local_dependencies/cryo_cli/src/summaries.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/Cargo.toml` & `cryo_python-0.1.1/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 [package]
 name = "cryo_python"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
+build = "build.rs"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "cryo"
 crate-type = ["cdylib"]
 
 [dependencies]
 cryo_cli = { version = "0.1.0", path = "local_dependencies/cryo_cli" }
 cryo_freeze = { version = "0.1.0", path = "local_dependencies/cryo_freeze" }
 polars = { version = "0.30.0", features = ["parquet", "string_encoding", "polars-lazy", "lazy", "binary_encoding", "json", "dtype-struct"] }
 pyo3 = { version = "0.18.0", features = ["extension-module"] }
 pyo3-asyncio = { version = "0.18.0", features = ["tokio-runtime"] }
 pyo3-polars = "0.4.0"
 tokio = "1.29.0"
+
+[build-dependencies]
+pyo3-build-config = "0.18.0"
+
```

### Comparing `cryo_python-0.1.0/.github/workflows/CI.yml` & `cryo_python-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/.gitignore` & `cryo_python-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/pyproject.toml` & `cryo_python-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/python/cryo/_args.py` & `cryo_python-0.1.1/python/cryo/_args.py`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/python/cryo/_collect.py` & `cryo_python-0.1.1/python/cryo/_collect.py`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/python/cryo/_freeze.py` & `cryo_python-0.1.1/python/cryo/_freeze.py`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/python/cryo/_spec.py` & `cryo_python-0.1.1/python/cryo/_spec.py`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/python_tests/test_datatypes.py` & `cryo_python-0.1.1/python_tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/python_tests/test_output_formats.py` & `cryo_python-0.1.1/python_tests/test_output_formats.py`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/src/collect_adapter.rs` & `cryo_python-0.1.1/src/collect_adapter.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/src/freeze_adapter.rs` & `cryo_python-0.1.1/src/freeze_adapter.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/src/lib.rs` & `cryo_python-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.0/Cargo.lock` & `cryo_python-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -876,21 +876,22 @@
  "prefix-hex",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "cryo_python"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "cryo_cli",
  "cryo_freeze",
  "polars",
  "pyo3",
  "pyo3-asyncio",
+ "pyo3-build-config",
  "pyo3-polars",
  "tokio",
 ]
 
 [[package]]
 name = "crypto-bigint"
 version = "0.5.2"
```

