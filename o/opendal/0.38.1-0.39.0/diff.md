# Comparing `tmp/opendal-0.38.1.tar.gz` & `tmp/opendal-0.39.0.tar.gz`

## Comparing `opendal-0.38.1.tar` & `opendal-0.39.0.tar`

### file list

```diff
@@ -1,340 +1,367 @@
--rw-r--r--   0        0        0     6878 1970-01-01 00:00:00.000000 opendal-0.38.1/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    95565 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1114 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6290 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5554 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2987 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1290 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     6142 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123     1040 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10880 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     3172 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
--rw-r--r--   0     1001      123     2687 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
--rw-r--r--   0     1001      123     2576 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md
--rw-r--r--   0     1001      123     6055 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2602_object_versioning.md
--rw-r--r--   0     1001      123     4748 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    26469 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6622 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    32922 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9949 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    17725 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    14214 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    53997 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13488 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    30012 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    14264 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2376 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    13222 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    23560 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    38577 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    11611 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/throttle.rs
--rw-r--r--   0     1001      123    14179 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/timeout.rs
--rw-r--r--   0     1001      123    12198 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3644 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3571 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    18865 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123    12928 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1020 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1566 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     5407 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
--rw-r--r--   0     1001      123    12938 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
--rw-r--r--   0     1001      123     1067 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
--rw-r--r--   0     1001      123     1934 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     5941 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5735 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3415 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    11165 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2159 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123    35575 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/multipart.rs
--rw-r--r--   0     1001      123     2962 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11712 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1976 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     3018 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/append.rs
--rw-r--r--   0     1001      123     9438 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3670 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15410 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4154 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     2842 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_reader.rs
--rw-r--r--   0     1001      123     1473 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_stream.rs
--rw-r--r--   0     1001      123     1070 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/mod.rs
--rw-r--r--   0     1001      123     4579 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2181 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10637 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     2132 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/stream.rs
--rw-r--r--   0     1001      123     9158 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5739 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     3953 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    13103 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/ops.rs
--rw-r--r--   0     1001      123    11651 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6507 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123     4514 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/appender.rs
--rw-r--r--   0     1001      123    32011 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123     5544 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    16985 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     2304 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/docs.md
--rw-r--r--   0     1001      123     5870 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      927 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2346 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    14348 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123    10123 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     1960 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/docs.md
--rw-r--r--   0     1001      123     3519 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2909 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     4216 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cacache/backend.rs
--rw-r--r--   0     1001      123      657 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cacache/docs.md
--rw-r--r--   0     1001      123      860 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cacache/mod.rs
--rw-r--r--   0     1001      123     5727 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/appender.rs
--rw-r--r--   0     1001      123    13691 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/backend.rs
--rw-r--r--   0     1001      123     9182 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/core.rs
--rw-r--r--   0     1001      123     1314 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/docs.md
--rw-r--r--   0     1001      123     3492 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/error.rs
--rw-r--r--   0     1001      123      910 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/mod.rs
--rw-r--r--   0     1001      123     5963 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/pager.rs
--rw-r--r--   0     1001      123     2324 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/writer.rs
--rw-r--r--   0     1001      123     3972 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      186 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/docs.md
--rw-r--r--   0     1001      123      859 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    10414 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/backend.rs
--rw-r--r--   0     1001      123     8274 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/builder.rs
--rw-r--r--   0     1001      123    14868 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/core.rs
--rw-r--r--   0     1001      123     3219 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/error.rs
--rw-r--r--   0     1001      123      906 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/mod.rs
--rw-r--r--   0     1001      123     2160 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/writer.rs
--rw-r--r--   0     1001      123     1409 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/appender.rs
--rw-r--r--   0     1001      123    23196 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123      869 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/docs.md
--rw-r--r--   0     1001      123     1424 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      898 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3541 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    15921 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123      737 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/docs.md
--rw-r--r--   0     1001      123     1808 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4208 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     2098 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    23950 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    17061 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3512 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10592 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6539 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123     3361 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/backend.rs
--rw-r--r--   0     1001      123     4276 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/builder.rs
--rw-r--r--   0     1001      123     7046 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/core.rs
--rw-r--r--   0     1001      123     1743 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/error.rs
--rw-r--r--   0     1001      123      904 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/mod.rs
--rw-r--r--   0     1001      123     2154 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/writer.rs
--rw-r--r--   0     1001      123    20868 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2573 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    13208 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     3048 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/docs.md
--rw-r--r--   0     1001      123     1497 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2659 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    16276 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    15931 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123      867 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/docs.md
--rw-r--r--   0     1001      123     1871 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     9056 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123      186 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/docs.md
--rw-r--r--   0     1001      123     2790 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1951 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     5712 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9058 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4405 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      511 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memory/docs.md
--rw-r--r--   0     1001      123      857 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     6599 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/backend.rs
--rw-r--r--   0     1001      123      861 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/mod.rs
--rw-r--r--   0     1001      123     4625 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     8174 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123     4710 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/appender.rs
--rw-r--r--   0     1001      123    15662 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     9415 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3492 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      910 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2324 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    12480 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/backend.rs
--rw-r--r--   0     1001      123     4177 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/builder.rs
--rw-r--r--   0     1001      123     1743 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/error.rs
--rw-r--r--   0     1001      123     9228 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/graph_model.rs
--rw-r--r--   0     1001      123      926 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/mod.rs
--rw-r--r--   0     1001      123     4874 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/pager.rs
--rw-r--r--   0     1001      123     6426 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/writer.rs
--rw-r--r--   0     1001      123     4869 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/appender.rs
--rw-r--r--   0     1001      123    22015 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    25314 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     1842 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/docs.md
--rw-r--r--   0     1001      123     3407 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      910 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123     6613 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redb/backend.rs
--rw-r--r--   0     1001      123      677 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redb/docs.md
--rw-r--r--   0     1001      123      854 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redb/mod.rs
--rw-r--r--   0     1001      123     9658 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      856 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redis/docs.md
--rw-r--r--   0     1001      123      855 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     4241 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123     1263 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/docs.md
--rw-r--r--   0     1001      123      859 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    41263 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     4183 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28667 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     7050 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/docs.md
--rw-r--r--   0     1001      123     4805 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7387 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7720 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123    16132 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/backend.rs
--rw-r--r--   0     1001      123     1076 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/docs.md
--rw-r--r--   0     1001      123     2587 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/error.rs
--rw-r--r--   0     1001      123      899 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/mod.rs
--rw-r--r--   0     1001      123     2420 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/pager.rs
--rw-r--r--   0     1001      123     3641 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/utils.rs
--rw-r--r--   0     1001      123     1958 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/writer.rs
--rw-r--r--   0     1001      123     5813 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      642 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sled/docs.md
--rw-r--r--   0     1001      123      854 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123     9779 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/backend.rs
--rw-r--r--   0     1001      123     8021 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/core.rs
--rw-r--r--   0     1001      123     2952 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/error.rs
--rw-r--r--   0     1001      123      894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/mod.rs
--rw-r--r--   0     1001      123     2555 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/writer.rs
--rw-r--r--   0     1001      123     4551 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
--rw-r--r--   0     1001      123     3636 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
--rw-r--r--   0     1001      123     1743 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
--rw-r--r--   0     1001      123      912 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
--rw-r--r--   0     1001      123     2228 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
--rw-r--r--   0     1001      123    39653 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29752 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     4779 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2223 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    21005 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1851 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      990 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123      892 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123    18302 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2337 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19002 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     1864 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/docs.md
--rw-r--r--   0     1001      123     4224 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     7373 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     4859 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2249 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     8596 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/appender.rs
--rw-r--r--   0     1001      123     2649 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6975 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    12174 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     7417 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    17930 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1614 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    27602 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123    13888 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3073 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1153 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    50360 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123     3428 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_functions.rs
--rw-r--r--   0     1001      123    18181 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_futures.rs
--rw-r--r--   0     1001      123     9547 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     7375 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    13822 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 opendal-0.38.1/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-07-15 04:02:43.000000 opendal-0.38.1/.gitignore
--rw-r--r--   0     1001      123     2213 2023-07-15 04:02:43.000000 opendal-0.38.1/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1084 2023-07-15 04:02:43.000000 opendal-0.38.1/README.md
--rw-r--r--   0     1001      123      765 2023-07-15 04:02:43.000000 opendal-0.38.1/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-07-15 04:02:43.000000 opendal-0.38.1/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-07-15 04:02:43.000000 opendal-0.38.1/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-07-15 04:02:43.000000 opendal-0.38.1/examples/object.ipynb
--rw-r--r--   0     1001      123     1660 2023-07-15 04:02:43.000000 opendal-0.38.1/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-07-15 04:02:43.000000 opendal-0.38.1/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-07-15 04:02:43.000000 opendal-0.38.1/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123      405 2023-07-15 04:02:43.000000 opendal-0.38.1/python/opendal/layers.pyi
--rw-r--r--   0     1001      123    11963 2023-07-15 04:02:43.000000 opendal-0.38.1/src/asyncio.rs
--rw-r--r--   0     1001      123     3074 2023-07-15 04:02:43.000000 opendal-0.38.1/src/layers.rs
--rw-r--r--   0     1001      123    12218 2023-07-15 04:02:43.000000 opendal-0.38.1/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-07-15 04:02:43.000000 opendal-0.38.1/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-07-15 04:02:43.000000 opendal-0.38.1/tests/steps/binding.py
--rw-r--r--   0     1001      123   140798 2023-07-15 04:02:43.000000 opendal-0.38.1/Cargo.lock
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 opendal-0.38.1/PKG-INFO
+-rw-r--r--   0        0        0     7449 1970-01-01 00:00:00.000000 opendal-0.39.0/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123   101503 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1114 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6389 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5554 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2987 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1290 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123     1202 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10880 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     2687 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
+-rw-r--r--   0     1001      123     2576 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md
+-rw-r--r--   0     1001      123     6055 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2602_object_versioning.md
+-rw-r--r--   0     1001      123     4748 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    27247 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     5197 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/await_tree.rs
+-rw-r--r--   0     1001      123     6622 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    32923 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9949 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17725 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    14214 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    53997 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13488 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    30012 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    14225 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2549 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13222 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    23560 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    45436 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    11611 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/throttle.rs
+-rw-r--r--   0     1001      123    14179 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/timeout.rs
+-rw-r--r--   0     1001      123    12198 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3644 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3571 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    18865 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123    12928 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1020 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1566 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     5407 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
+-rw-r--r--   0     1001      123    12938 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
+-rw-r--r--   0     1001      123     1067 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     5941 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5669 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     2360 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    11165 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2136 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123    35546 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/multipart.rs
+-rw-r--r--   0     1001      123     2962 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11712 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1636 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     3018 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/append/api.rs
+-rw-r--r--   0     1001      123      827 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/append/mod.rs
+-rw-r--r--   0     1001      123     9438 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     1317 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3519 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/page/api.rs
+-rw-r--r--   0     1001      123     9150 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/page/into_flat_page.rs
+-rw-r--r--   0     1001      123     6884 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/page/into_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     1153 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/page/mod.rs
+-rw-r--r--   0     1001      123    11015 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/api.rs
+-rw-r--r--   0     1001      123     6660 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/into_read_from_file.rs
+-rw-r--r--   0     1001      123    15694 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/into_seekable_read_by_range.rs
+-rw-r--r--   0     1001      123     4555 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/into_streamable_read.rs
+-rw-r--r--   0     1001      123     1365 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/mod.rs
+-rw-r--r--   0     1001      123     2132 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/stream/api.rs
+-rw-r--r--   0     1001      123     1437 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/stream/into_stream.rs
+-rw-r--r--   0     1001      123     2842 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/stream/into_stream_from_reader.rs
+-rw-r--r--   0     1001      123      995 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/stream/mod.rs
+-rw-r--r--   0     1001      123     5739 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/write/api.rs
+-rw-r--r--   0     1001      123     1129 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/write/mod.rs
+-rw-r--r--   0     1001      123     8364 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/oio/write/multipart_upload_write.rs
+-rw-r--r--   0     1001      123     3953 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    13606 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/ops.rs
+-rw-r--r--   0     1001      123    11651 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6507 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123     4514 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/appender.rs
+-rw-r--r--   0     1001      123    32011 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123     5544 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    16985 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     2304 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/docs.md
+-rw-r--r--   0     1001      123     5876 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      927 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2346 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    14348 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123    10123 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     1960 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/docs.md
+-rw-r--r--   0     1001      123     3524 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2909 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     4216 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cacache/backend.rs
+-rw-r--r--   0     1001      123      657 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cacache/docs.md
+-rw-r--r--   0     1001      123      860 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cacache/mod.rs
+-rw-r--r--   0     1001      123     5727 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/appender.rs
+-rw-r--r--   0     1001      123    14730 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/backend.rs
+-rw-r--r--   0     1001      123    14597 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/core.rs
+-rw-r--r--   0     1001      123     1314 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/docs.md
+-rw-r--r--   0     1001      123     3496 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/error.rs
+-rw-r--r--   0     1001      123      910 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/mod.rs
+-rw-r--r--   0     1001      123     5963 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/pager.rs
+-rw-r--r--   0     1001      123     5355 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/cos/writer.rs
+-rw-r--r--   0     1001      123     3972 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      186 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dashmap/docs.md
+-rw-r--r--   0     1001      123      859 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    10414 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/backend.rs
+-rw-r--r--   0     1001      123     8274 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/builder.rs
+-rw-r--r--   0     1001      123    14868 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/core.rs
+-rw-r--r--   0     1001      123     3091 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/error.rs
+-rw-r--r--   0     1001      123      906 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/mod.rs
+-rw-r--r--   0     1001      123     2160 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/writer.rs
+-rw-r--r--   0     1001      123     9314 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/backend.rs
+-rw-r--r--   0     1001      123      988 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/docs.md
+-rwxr-xr-x   0     1001      123     1675 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/ca-key.pem
+-rwxr-xr-x   0     1001      123     1338 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/ca.pem
+-rwxr-xr-x   0     1001      123      227 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/client-key.pem
+-rwxr-xr-x   0     1001      123     1123 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/client.pem
+-rwxr-xr-x   0     1001      123      227 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/etcd1/etcd-key.pem
+-rwxr-xr-x   0     1001      123     1184 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/etcd1/etcd.pem
+-rwxr-xr-x   0     1001      123      227 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/etcd2/etcd-key.pem
+-rwxr-xr-x   0     1001      123     1184 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/etcd2/etcd.pem
+-rwxr-xr-x   0     1001      123      227 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/etcd3/etcd-key.pem
+-rwxr-xr-x   0     1001      123     1184 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/etcd3/etcd.pem
+-rwxr-xr-x   0     1001      123      227 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/server-key.pem
+-rwxr-xr-x   0     1001      123     1176 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/fixtures/server.pem
+-rw-r--r--   0     1001      123      853 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/etcd/mod.rs
+-rw-r--r--   0     1001      123     1409 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/fs/appender.rs
+-rw-r--r--   0     1001      123    23198 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123      869 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/fs/docs.md
+-rw-r--r--   0     1001      123     1424 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      898 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3541 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    15921 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123      737 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ftp/docs.md
+-rw-r--r--   0     1001      123     1808 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4208 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     2098 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    23950 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    17061 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3517 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10592 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6539 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123     3361 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/backend.rs
+-rw-r--r--   0     1001      123     4276 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/builder.rs
+-rw-r--r--   0     1001      123     7046 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/core.rs
+-rw-r--r--   0     1001      123     1767 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/error.rs
+-rw-r--r--   0     1001      123      904 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/mod.rs
+-rw-r--r--   0     1001      123     2154 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/writer.rs
+-rw-r--r--   0     1001      123    20868 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1932 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2573 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123     1463 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/appender.rs
+-rw-r--r--   0     1001      123    15256 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     3241 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/docs.md
+-rw-r--r--   0     1001      123     1497 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      902 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2659 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    16276 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1899 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    15931 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123      867 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/docs.md
+-rw-r--r--   0     1001      123     1895 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     9056 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123      186 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/docs.md
+-rw-r--r--   0     1001      123     2795 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1951 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     5712 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9058 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4405 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      511 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/memory/docs.md
+-rw-r--r--   0     1001      123      857 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     6599 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/mini_moka/backend.rs
+-rw-r--r--   0     1001      123      861 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/mini_moka/mod.rs
+-rw-r--r--   0     1001      123     4945 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     8174 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123     4710 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/obs/appender.rs
+-rw-r--r--   0     1001      123    16647 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123    14394 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3497 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      910 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     7641 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    12480 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/backend.rs
+-rw-r--r--   0     1001      123     4177 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/builder.rs
+-rw-r--r--   0     1001      123     1767 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/error.rs
+-rw-r--r--   0     1001      123     9228 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs
+-rw-r--r--   0     1001      123      926 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/mod.rs
+-rw-r--r--   0     1001      123     4874 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/pager.rs
+-rw-r--r--   0     1001      123     6426 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/writer.rs
+-rw-r--r--   0     1001      123     4869 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/appender.rs
+-rw-r--r--   0     1001      123    22098 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    25640 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     1842 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/docs.md
+-rw-r--r--   0     1001      123     3412 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      910 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     5349 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123     7677 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/persy/backend.rs
+-rw-r--r--   0     1001      123      834 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/persy/docs.md
+-rw-r--r--   0     1001      123      856 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/persy/mod.rs
+-rw-r--r--   0     1001      123     6613 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/redb/backend.rs
+-rw-r--r--   0     1001      123      677 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/redb/docs.md
+-rw-r--r--   0     1001      123      854 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/redb/mod.rs
+-rw-r--r--   0     1001      123    10018 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      856 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/redis/docs.md
+-rw-r--r--   0     1001      123      855 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     4241 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123     1263 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/rocksdb/docs.md
+-rw-r--r--   0     1001      123      859 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    42506 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     4183 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28571 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     7050 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/docs.md
+-rw-r--r--   0     1001      123     4677 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7387 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     5342 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123    16132 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sftp/backend.rs
+-rw-r--r--   0     1001      123     1076 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sftp/docs.md
+-rw-r--r--   0     1001      123     2587 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sftp/error.rs
+-rw-r--r--   0     1001      123      899 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sftp/mod.rs
+-rw-r--r--   0     1001      123     2420 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sftp/pager.rs
+-rw-r--r--   0     1001      123     3639 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sftp/utils.rs
+-rw-r--r--   0     1001      123     1958 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sftp/writer.rs
+-rw-r--r--   0     1001      123     5813 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      642 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sled/docs.md
+-rw-r--r--   0     1001      123      854 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123     9779 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/supabase/backend.rs
+-rw-r--r--   0     1001      123     8021 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/supabase/core.rs
+-rw-r--r--   0     1001      123     2957 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/supabase/error.rs
+-rw-r--r--   0     1001      123      894 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/supabase/mod.rs
+-rw-r--r--   0     1001      123     2555 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/supabase/writer.rs
+-rw-r--r--   0     1001      123     7331 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/tikv/backend.rs
+-rw-r--r--   0     1001      123      863 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/tikv/docs.md
+-rw-r--r--   0     1001      123      848 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/tikv/fixtures/pd.toml
+-rw-r--r--   0     1001      123     1120 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/tikv/fixtures/tikv.toml
+-rw-r--r--   0     1001      123      854 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/tikv/mod.rs
+-rw-r--r--   0     1001      123     5665 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
+-rw-r--r--   0     1001      123     3636 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
+-rw-r--r--   0     1001      123     1767 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
+-rw-r--r--   0     1001      123      912 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
+-rw-r--r--   0     1001      123     2228 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
+-rw-r--r--   0     1001      123    39529 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29766 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     4784 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2223 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    21005 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1945 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      990 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      892 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123    18302 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2337 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19002 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     1864 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/docs.md
+-rw-r--r--   0     1001      123     4144 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     7373 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     4859 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2249 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     8596 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/appender.rs
+-rw-r--r--   0     1001      123     2649 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     7110 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12242 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     7417 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    17930 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1614 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    27615 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123    14137 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3073 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1153 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    50360 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123     3428 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/operator/operator_functions.rs
+-rw-r--r--   0     1001      123    19070 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/operator/operator_futures.rs
+-rw-r--r--   0     1001      123     9545 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     7768 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    13711 2023-07-31 11:06:45.000000 opendal-0.39.0/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 opendal-0.39.0/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-07-31 11:06:45.000000 opendal-0.39.0/.gitignore
+-rw-r--r--   0     1001      123     2213 2023-07-31 11:06:45.000000 opendal-0.39.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1084 2023-07-31 11:06:45.000000 opendal-0.39.0/README.md
+-rw-r--r--   0     1001      123      765 2023-07-31 11:06:45.000000 opendal-0.39.0/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-07-31 11:06:45.000000 opendal-0.39.0/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-07-31 11:06:45.000000 opendal-0.39.0/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-07-31 11:06:45.000000 opendal-0.39.0/examples/object.ipynb
+-rw-r--r--   0     1001      123     1660 2023-07-31 11:06:45.000000 opendal-0.39.0/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-07-31 11:06:45.000000 opendal-0.39.0/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-07-31 11:06:45.000000 opendal-0.39.0/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123     1191 2023-07-31 11:06:45.000000 opendal-0.39.0/python/opendal/layers.pyi
+-rw-r--r--   0     1001      123    11963 2023-07-31 11:06:45.000000 opendal-0.39.0/src/asyncio.rs
+-rw-r--r--   0     1001      123     3074 2023-07-31 11:06:45.000000 opendal-0.39.0/src/layers.rs
+-rw-r--r--   0     1001      123    12218 2023-07-31 11:06:45.000000 opendal-0.39.0/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-07-31 11:06:45.000000 opendal-0.39.0/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-07-31 11:06:45.000000 opendal-0.39.0/tests/steps/binding.py
+-rw-r--r--   0     1001      123   152962 2023-07-31 11:06:45.000000 opendal-0.39.0/Cargo.lock
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 opendal-0.39.0/PKG-INFO
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/Cargo.toml` & `opendal-0.39.0/local_dependencies/opendal/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.38.1"
+version= "0.39.0"
 resolver = "2"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
@@ -73,14 +73,15 @@
 layers-all = [
   "layers-chaos",
   "layers-metrics",
   "layers-prometheus",
   "layers-tracing",
   "layers-minitrace",
   "layers-throttle",
+  "layers-await-tree",
 ]
 # Enable layers chaos support
 layers-chaos = ["dep:rand"]
 # Enable layers metrics support
 layers-metrics = ["dep:metrics"]
 # Enable layers prometheus support
 layers-prometheus = ["dep:prometheus"]
@@ -90,14 +91,16 @@
 layers-minitrace = ["dep:minitrace"]
 # Enable layers tracing support.
 layers-tracing = ["dep:tracing"]
 # Enable layers oteltrace support.
 layers-otel-trace = ["dep:opentelemetry"]
 # Enable layers throttle support.
 layers-throttle = ["dep:governor"]
+# Enable layers await-tree support.
+layers-await-tree = ["dep:await-tree"]
 
 services-azblob = [
   "dep:sha2",
   "dep:reqsign",
   "reqsign?/services-azblob",
   "reqsign?/reqwest_request",
 ]
@@ -110,14 +113,15 @@
 services-cos = [
   "dep:reqsign",
   "reqsign?/services-tencent",
   "reqsign?/reqwest_request",
 ]
 services-dashmap = ["dep:dashmap"]
 services-dropbox = []
+services-etcd = ["dep:etcd-client"]
 services-fs = ["tokio/fs"]
 services-ftp = ["dep:suppaftp", "dep:lazy-regex", "dep:bb8", "dep:async-tls"]
 services-gcs = [
   "dep:reqsign",
   "reqsign?/services-google",
   "reqsign?/reqwest_request",
 ]
@@ -138,25 +142,29 @@
 ]
 services-onedrive = []
 services-oss = [
   "dep:reqsign",
   "reqsign?/services-aliyun",
   "reqsign?/reqwest_request",
 ]
+services-persy = ["dep:persy"]
 services-redb = ["dep:redb"]
 services-redis = ["dep:redis"]
+services-redis-native-tls = ["services-redis", "redis?/tokio-native-tls-comp"]
+services-redis-rustls = ["services-redis", "redis?/tokio-rustls-comp"]
 services-rocksdb = ["dep:rocksdb"]
 services-s3 = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-sftp = ["dep:openssh", "dep:openssh-sftp-client", "dep:dirs"]
 services-sled = ["dep:sled"]
 services-supabase = []
+services-tikv = ["tikv-client"]
 services-vercel-artifacts = []
 services-wasabi = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-webdav = []
@@ -175,67 +183,71 @@
 path = "tests/behavior/main.rs"
 
 [dependencies]
 anyhow = { version = "1.0.30", features = ["std"] }
 async-compat = "0.2"
 async-tls = { version = "0.11", optional = true }
 async-trait = "0.1.68"
+await-tree = { version = "0.1.1", optional = true }
 backon = "0.4.0"
 base64 = "0.21"
 bb8 = { version = "0.8", optional = true }
 bytes = "1.2"
 cacache = { version = "11.6", default-features = false, features = [
   "tokio-runtime",
   "mmap",
 ], optional = true }
 chrono = "0.4.26"
 dashmap = { version = "5.4", optional = true }
 dirs = { version = "5.0.1", optional = true }
+etcd-client = { version = "0.11", optional = true, features = ["tls"] }
 flagset = "0.4"
 futures = { version = "0.3", default-features = false, features = ["std"] }
 governor = { version = "0.5", optional = true, features = ["std"] }
-hdrs = { version = "0.2", optional = true, features = ["async_file"] }
+hdrs = { version = "0.3.0", optional = true, features = ["async_file"] }
 http = "0.2.5"
 hyper = "0.14"
 lazy-regex = { version = "2.5.0", optional = true }
 log = "0.4"
 madsim = { version = "0.2.21", optional = true }
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
 mini-moka = { version = "0.10", optional = true }
-minitrace = { version = "0.4.1", optional = true }
+minitrace = { version = "0.5", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
 openssh = { version = "0.9.9", optional = true }
 openssh-sftp-client = { version = "0.13.5", optional = true, features = [
   "openssh",
   "tracing",
 ] }
 opentelemetry = { version = "0.19.0", optional = true }
 parking_lot = "0.12"
 percent-encoding = "2"
+persy = { version = "1.4.4", optional = true }
 pin-project = "1"
 prometheus = { version = "0.13", features = ["process"], optional = true }
 prost = { version = "0.11", optional = true }
-quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
+quick-xml = { version = "0.29", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
 redb = { version = "1.0.0", optional = true }
 redis = { version = "0.23", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
-reqsign = { version = "0.13.0", default-features = false, optional = true }
+reqsign = { version = "0.14.0", default-features = false, optional = true }
 reqwest = { version = "0.11.18", features = [
   "stream",
 ], default-features = false }
 rocksdb = { version = "0.21.0", default-features = false, optional = true }
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
 sha2 = { version = "0.10", optional = true }
 sled = { version = "0.34.7", optional = true }
 suppaftp = { version = "4.5", default-features = false, features = [
   "async-secure",
   "async-rustls",
 ], optional = true }
+tikv-client = { version = "0.2.0", optional = true }
 tokio = "1.27"
 tracing = { version = "0.1", optional = true }
 uuid = { version = "1", features = ["serde", "v4"] }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.39.0/local_dependencies/opendal/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,74 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.39.0] - 2023-07-31
+
+### Added
+* feat: add a behaviour test for InvalidInput by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2644
+* feat(services/persy): add a basic persy service impl by @PsiACE in https://github.com/apache/incubator-opendal/pull/2648
+* feat(services/vercel_artifacts): Impl `stat` by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2649
+* feat(test): add fuzz test for range_reader by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2609
+* feat(core/http_util): Remove sensitive header like Set-Cookie by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2664
+* feat: Add RetryInterceptor support for RetryLayer by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2666
+* feat: support kerberos for hdfs service by @zuston in https://github.com/apache/incubator-opendal/pull/2668
+* feat: support append for hdfs by @zuston in https://github.com/apache/incubator-opendal/pull/2671
+* feat(s3): Use us-east-1 while head bucket returns 403 without X-Amz-Bucket-Region by @john8628 in https://github.com/apache/incubator-opendal/pull/2677
+* feat(oay): Add webdav basic read impl by @Young-Flash in https://github.com/apache/incubator-opendal/pull/2658
+* feat(services/redis): enable TLS by @Stormshield-robinc in https://github.com/apache/incubator-opendal/pull/2670
+* feat(services/etcd): introduce new service backend etcd by @G-XD in https://github.com/apache/incubator-opendal/pull/2672
+* feat(service/obs):add multipart upload function support by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2685
+* feat(services/s3): Add assume role support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2687
+* feat(services/tikv): introduce new service backend tikv by @oowl in https://github.com/apache/incubator-opendal/pull/2565
+* feat(service/cos): add multipart upload function support by @ArmandoZ in https://github.com/apache/incubator-opendal/pull/2697
+* feat(oio): Add MultipartUploadWrite to easier the work for Writer by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2699
+* feat(test): add fuzz target for writer by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2706
+* feat: cos multipart uploads write by @parkma99 in https://github.com/apache/incubator-opendal/pull/2712
+* feat(layers): support await_tree instrument by @oowl in https://github.com/apache/incubator-opendal/pull/2623
+* feat(tests): Extract fuzz test of #2717 by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2720
+* feat: oss multipart uploads write by @parkma99 in https://github.com/apache/incubator-opendal/pull/2723
+* feat: add override_content_type by @G-XD in https://github.com/apache/incubator-opendal/pull/2734
+### Changed
+* refactor(services/redis): Polish features of redis by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2681
+* refactor(services/s3): Check header first for region detect by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2691
+* refactor(raw/oio): Reorganize to allow adding more features by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2698
+* refactor: Polish fuzz build time by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2721
+### Fixed
+* fix(services/cos): fix cos service comments by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2656
+* fix(test): profile setting warning by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2657
+* fix(bindings/C): fix the memory found in valgrind. by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2673
+* fix: owncloud test sometimes fail by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2684
+* fix(services/obs): remove content-length check in backend by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2686
+* fix: fix `HADOOP_CONF_DIR` setting in guidance document by @wcy-fdu in https://github.com/apache/incubator-opendal/pull/2713
+* fix: Seek before the start of file should be invalid by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2718
+* fix(layer/minitrace): fix doctest by @andylokandy in https://github.com/apache/incubator-opendal/pull/2728
+### Docs
+* docs: add instructions to fix wrong vote mail and uploads by @ClSlaid in https://github.com/apache/incubator-opendal/pull/2682
+* doc(services/tikv): add tikv service backend to readme by @oowl in https://github.com/apache/incubator-opendal/pull/2711
+* docs(bindings/java): improve safety doc for get_current_env by @tisonkun in https://github.com/apache/incubator-opendal/pull/2733
+### CI
+* ci(services/webdav): Setup integration test for owncloud by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2659
+* ci: Fix unexpected error in owncloud by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2663
+* ci: upgrade hawkeye action by @tisonkun in https://github.com/apache/incubator-opendal/pull/2665
+* ci: Make owncloud happy by reduce the concurrency by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2667
+* ci: Setup protoc in rust builder by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2674
+* ci: Fix Cargo.lock not updated by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2680
+* ci: Add services fuzz test for read/write/range_read by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2710
+### Chore
+* chore: Update CODEOWNERS by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2676
+* chore(bindings/python): upgrade pyo3 to 0.19 by @messense in https://github.com/apache/incubator-opendal/pull/2694
+* chore: upgrade quick-xml to 0.29 by @messense in https://github.com/apache/incubator-opendal/pull/2696
+* chore(download): update version 0.38.1 by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2714
+* chore(service/minitrace): update to v0.5.0 by @andylokandy in https://github.com/apache/incubator-opendal/pull/2725
+
+
 ## [v0.38.1] - 2023-07-14
 
 ### Added
 
 - feat(binding/lua): add rename and create_dir operator function by @oowl in https://github.com/apache/incubator-opendal/pull/2564
 - feat(services/azblob): support sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2574
 - feat(services/gcs): support sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2576
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.39.0/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/README.md` & `opendal-0.39.0/local_dependencies/opendal/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,18 +63,20 @@
 
 <details>
 <summary>Key-Value Storage Service (like rocksdb, sled)</summary>
 
 - cacache: [cacache](https://crates.io/crates/cacache) backend
 - dashmap: [dashmap](https://github.com/xacrimon/dashmap) backend
 - memory: In memory backend
+- persy: [persy](https://crates.io/crates/persy) backend
 - redis: [Redis](https://redis.io/) services
 - rocksdb: [RocksDB](http://rocksdb.org/) services
 - sled: [sled](https://crates.io/crates/sled) backend
 - redb: [redb](https://crates.io/crates/redb) backend
+- tikv: [tikv](https://tikv.org/) backend
 
 </details>
 
 <details>
 <summary>Cache Storage Service (like memcached, moka)</summary>
 
 - ghac: [Github Action Cache](https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows) Service
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.39.0/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.39.0/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.39.0/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.39.0/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.39.0/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.39.0/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/features.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/features.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 - `services-dashmap`: Enable dashmap service support.
 - `services-ftp`: Enable ftp service support.
 - `services-hdfs`: Enable hdfs service support.
 - `services-memcached`: Enable memcached service support.
 - `services-mini-moka`: Enable mini-moka service support.
 - `services-moka`: Enable moka service support.
 - `services-ipfs`: Enable ipfs service support.
-- `services-redis`: Enable redis service support.
+- `services-redis`: Enable redis service support without TLS.
+- `services-redis-rustls`: Enable redis service support with `rustls`.
+- `services-redis-native-tls`: Enable redis service support with `native-tls`.
 - `services-rocksdb`: Enable rocksdb service support.
 - `services-sled`: Enable sled service support.
 
 ## Dependencies Features
 
 - `rustls`: Enable TLS functionality provided by `rustls`, enabled by default
 - `native-tls`: Enable TLS functionality provided by `native-tls`
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.39.0/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2602_object_versioning.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/2602_object_versioning.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.39.0/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# Upgrade to v0.39
+
+## Public API
+
+### Service S3 Role Arn Behavior
+
+In PR #2687, OpenDAL changed the behavior when `role_arn` has been specified.
+
+OpenDAL used to override role_arn simply. But since this version, OpenDAL will make sure to use assume_role with specified `role_arn` and `external_id` (if supplied).
+
+### RetryLayer supports RetryInterceptor
+
+In PR #2666, `RetryLayer` supports `RetryInterceptor`. To implement this change, `RetryLayer` changed it's in-memory layout by adding a new generic parameter `I` to `RetryLayer<I>`.
+
+Users who stores `RetryLayer` in struct or enum will need to change the type if they don't want to use default behavior.
+
+## Raw API
+
+In PR #2698, OpenDAL re-org the internal structure of `opendal::raw::oio` and changed some APIs name.
+
 # Upgrade to v0.38
 
 There are no public API changes.
 
 ## Raw API
 
 OpenDAL add the `Write::sink` API to enable streaming writing. This is a breaking change for users who depend on the raw API.
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/complete.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 use std::sync::Arc;
 use std::task::Context;
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 
-use crate::raw::oio::into_reader::RangeReader;
-use crate::raw::oio::to_flat_pager;
-use crate::raw::oio::to_hierarchy_pager;
+use crate::raw::oio::into_flat_page;
+use crate::raw::oio::into_hierarchy_page;
+use crate::raw::oio::ByRangeSeekableReader;
 use crate::raw::oio::Entry;
-use crate::raw::oio::IntoStreamableReader;
-use crate::raw::oio::ToFlatPager;
-use crate::raw::oio::ToHierarchyPager;
+use crate::raw::oio::FlatPager;
+use crate::raw::oio::HierarchyPager;
+use crate::raw::oio::StreamableReader;
 use crate::raw::*;
 use crate::*;
 
 /// Complete underlying services features so that users can use them in
 /// the same way.
 ///
 /// # Notes
@@ -168,15 +168,15 @@
         let range = args.range();
         let (rp, r) = self.inner.read(path, args).await?;
         let content_length = rp.metadata().content_length();
 
         match (seekable, streamable) {
             (true, true) => Ok((rp, CompleteReader::AlreadyComplete(r))),
             (true, false) => {
-                let r = oio::into_streamable_reader(r, 256 * 1024);
+                let r = oio::into_streamable_read(r, 256 * 1024);
                 Ok((rp, CompleteReader::NeedStreamable(r)))
             }
             _ => {
                 let (offset, size) = match (range.offset(), range.size()) {
                     (Some(offset), _) => (offset, content_length),
                     (None, None) => (0, content_length),
                     (None, Some(size)) => {
@@ -189,20 +189,20 @@
                         } else {
                             (total_size - size, size)
                         };
 
                         (offset, size)
                     }
                 };
-                let r = oio::into_reader::by_range(self.inner.clone(), path, r, offset, size);
+                let r = oio::into_seekable_read_by_range(self.inner.clone(), path, r, offset, size);
 
                 if streamable {
                     Ok((rp, CompleteReader::NeedSeekable(r)))
                 } else {
-                    let r = oio::into_streamable_reader(r, 256 * 1024);
+                    let r = oio::into_streamable_read(r, 256 * 1024);
                     Ok((rp, CompleteReader::NeedBoth(r)))
                 }
             }
         }
     }
 
     fn complete_blocking_reader(
@@ -219,15 +219,15 @@
         let streamable = capability.read_can_next;
 
         let (rp, r) = self.inner.blocking_read(path, args)?;
 
         match (seekable, streamable) {
             (true, true) => Ok((rp, CompleteReader::AlreadyComplete(r))),
             (true, false) => {
-                let r = oio::into_streamable_reader(r, 256 * 1024);
+                let r = oio::into_streamable_read(r, 256 * 1024);
                 Ok((rp, CompleteReader::NeedStreamable(r)))
             }
             (false, _) => Err(Error::new(
                 ErrorKind::Unsupported,
                 "non seekable blocking reader is not supported",
             )),
         }
@@ -250,30 +250,30 @@
         let delimiter = args.delimiter();
 
         if delimiter.is_empty() {
             return if cap.list_without_delimiter {
                 let (rp, p) = self.inner.list(path, args).await?;
                 Ok((rp, CompletePager::AlreadyComplete(p)))
             } else {
-                let p = to_flat_pager(
+                let p = into_flat_page(
                     self.inner.clone(),
                     path,
                     args.with_delimiter("/").limit().unwrap_or(1000),
                 );
                 Ok((RpList::default(), CompletePager::NeedFlat(p)))
             };
         }
 
         if delimiter == "/" {
             return if cap.list_with_delimiter_slash {
                 let (rp, p) = self.inner.list(path, args).await?;
                 Ok((rp, CompletePager::AlreadyComplete(p)))
             } else {
                 let (_, p) = self.inner.list(path, args.with_delimiter("")).await?;
-                let p = to_hierarchy_pager(p, path);
+                let p = into_hierarchy_page(p, path);
                 Ok((RpList::default(), CompletePager::NeedHierarchy(p)))
             };
         }
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "list with other delimiter is not supported",
@@ -299,31 +299,31 @@
         let delimiter = args.delimiter();
 
         if delimiter.is_empty() {
             return if cap.list_without_delimiter {
                 let (rp, p) = self.inner.blocking_list(path, args)?;
                 Ok((rp, CompletePager::AlreadyComplete(p)))
             } else {
-                let p = to_flat_pager(
+                let p = into_flat_page(
                     self.inner.clone(),
                     path,
                     args.with_delimiter("/").limit().unwrap_or(1000),
                 );
                 Ok((RpList::default(), CompletePager::NeedFlat(p)))
             };
         }
 
         if delimiter == "/" {
             return if cap.list_with_delimiter_slash {
                 let (rp, p) = self.inner.blocking_list(path, args)?;
                 Ok((rp, CompletePager::AlreadyComplete(p)))
             } else {
                 let (_, p) = self.inner.blocking_list(path, args.with_delimiter(""))?;
-                let p: ToHierarchyPager<<A as Accessor>::BlockingPager> =
-                    to_hierarchy_pager(p, path);
+                let p: HierarchyPager<<A as Accessor>::BlockingPager> =
+                    into_hierarchy_page(p, path);
                 Ok((RpList::default(), CompletePager::NeedHierarchy(p)))
             };
         }
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "list with other delimiter is not supported",
@@ -528,17 +528,17 @@
 
         self.inner().batch(args).await
     }
 }
 
 pub enum CompleteReader<A: Accessor, R> {
     AlreadyComplete(R),
-    NeedSeekable(RangeReader<A>),
-    NeedStreamable(IntoStreamableReader<R>),
-    NeedBoth(IntoStreamableReader<RangeReader<A>>),
+    NeedSeekable(ByRangeSeekableReader<A>),
+    NeedStreamable(StreamableReader<R>),
+    NeedBoth(StreamableReader<ByRangeSeekableReader<A>>),
 }
 
 impl<A, R> oio::Read for CompleteReader<A, R>
 where
     A: Accessor<Reader = R>,
     R: oio::Read,
 {
@@ -610,16 +610,16 @@
             _ => unreachable!("not supported types of complete reader"),
         }
     }
 }
 
 pub enum CompletePager<A: Accessor, P> {
     AlreadyComplete(P),
-    NeedFlat(ToFlatPager<Arc<A>, P>),
-    NeedHierarchy(ToHierarchyPager<P>),
+    NeedFlat(FlatPager<Arc<A>, P>),
+    NeedHierarchy(HierarchyPager<P>),
 }
 
 #[async_trait]
 impl<A, P> oio::Page for CompletePager<A, P>
 where
     A: Accessor<Pager = P>,
     P: oio::Page,
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/logging.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files 2% similar despite different names*

```diff
@@ -53,64 +53,69 @@
 /// ## Real usage
 ///
 /// ```no_run
 /// use std::error::Error;
 ///
 /// use anyhow::Result;
 /// use futures::executor::block_on;
+/// use minitrace::collector::Config;
+/// use minitrace::prelude::*;
 /// use opendal::layers::MinitraceLayer;
 /// use opendal::services;
 /// use opendal::Operator;
 ///
 /// fn main() -> Result<(), Box<dyn Error + Send + Sync + 'static>> {
-///     let collector = {
-///         let (span, collector) = minitrace::Span::root("op");
+///     let reporter =
+///         minitrace_jaeger::JaegerReporter::new("127.0.0.1:6831".parse().unwrap(), "opendal")
+///             .unwrap();
+///     minitrace::set_reporter(reporter, Config::default());
+///
+///     {
+///         let root = Span::root("op", SpanContext::random());
 ///         let runtime = tokio::runtime::Runtime::new()?;
 ///         runtime.block_on(
 ///             async {
 ///                 let _ = dotenvy::dotenv();
-///                 let op = Operator::from_env::<services::Memory>()
+///                 let op = Operator::new(services::Memory::default())
 ///                     .expect("init operator must succeed")
 ///                     .layer(MinitraceLayer)
 ///                     .finish();
 ///                 op.write("test", "0".repeat(16 * 1024 * 1024).into_bytes())
 ///                     .await
 ///                     .expect("must succeed");
 ///                 op.stat("test").await.expect("must succeed");
 ///                 op.read("test").await.expect("must succeed");
 ///             }
-///             .in_span(Span::enter_with_parent("test", &span)),
+///             .in_span(Span::enter_with_parent("test", &root)),
 ///         );
-///         collector
-///     };
-///     let spans = block_on(collector.collect());
-///     let bytes =
-///         minitrace_jaeger::encode("opendal".to_owned(), rand::random(), 0, 0, &spans).unwrap();
-///     minitrace_jaeger::report_blocking("127.0.0.1:6831".parse().unwrap(), &bytes)
-///         .expect("report error");
+///     }
+///
+///     minitrace::flush();
+///
 ///     Ok(())
 /// }
 /// ```
 ///
 /// # Output
 ///
 /// OpenDAL is using [`minitrace`](https://docs.rs/minitrace/latest/minitrace/) for tracing internally.
 ///
 /// To enable minitrace output, please init one of the reporter that `minitrace` supports.
 ///
 /// For example:
 ///
-/// ```ignore
+/// ```no_run
 /// extern crate minitrace_jaeger;
 ///
-/// let spans = block_on(collector.collect());
+/// use minitrace::collector::Config;
 ///
-/// let bytes =
-///     minitrace_jaeger::encode("opendal".to_owned(), rand::random(), 0, 0, &spans).unwrap();
-/// minitrace_jaeger::report_blocking("127.0.0.1:6831".parse().unwrap(), &bytes).expect("report error");
+/// let reporter =
+///     minitrace_jaeger::JaegerReporter::new("127.0.0.1:6831".parse().unwrap(), "opendal")
+///         .unwrap();
+/// minitrace::set_reporter(reporter, Config::default());
 /// ```
 ///
 /// For real-world usage, please take a look at [`minitrace-datadog`](https://crates.io/crates/minitrace-datadog) or [`minitrace-jaeger`](https://crates.io/crates/minitrace-jaeger) .
 pub struct MinitraceLayer;
 
 impl<A: Accessor> Layer<A> for MinitraceLayer {
     type LayeredAccessor = MinitraceAccessor<A>;
@@ -141,15 +146,15 @@
     }
 
     #[trace]
     fn metadata(&self) -> AccessorInfo {
         self.inner.info()
     }
 
-    #[trace("create", enter_on_poll = true)]
+    #[trace(name = "create", enter_on_poll = true)]
     async fn create_dir(&self, path: &str, args: OpCreateDir) -> Result<RpCreateDir> {
         self.inner.create_dir(path, args).await
     }
 
     #[trace(enter_on_poll = true)]
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         self.inner
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 #[cfg(feature = "layers-prometheus")]
 mod prometheus;
 #[cfg(feature = "layers-prometheus")]
 pub use self::prometheus::PrometheusLayer;
 
 mod retry;
+pub use self::retry::RetryInterceptor;
 pub use self::retry::RetryLayer;
 
 #[cfg(feature = "layers-tracing")]
 mod tracing;
 #[cfg(feature = "layers-tracing")]
 pub use self::tracing::TracingLayer;
 
@@ -79,7 +80,11 @@
 
 #[cfg(feature = "layers-throttle")]
 mod throttle;
 #[cfg(feature = "layers-otel-trace")]
 pub use self::oteltrace::OtelTraceLayer;
 #[cfg(feature = "layers-throttle")]
 pub use self::throttle::ThrottleLayer;
+#[cfg(feature = "layers-await-tree")]
+mod await_tree;
+#[cfg(feature = "layers-await-tree")]
+pub use self::await_tree::AwaitTreeLayer;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::io;
 use std::pin::Pin;
+use std::sync::Arc;
 use std::task::ready;
 use std::task::Context;
 use std::task::Poll;
 use std::time::Duration;
 
 use async_trait::async_trait;
 use backon::BackoffBuilder;
@@ -61,16 +62,66 @@
 /// use opendal::Scheme;
 ///
 /// let _ = Operator::new(services::Memory::default())
 ///     .expect("must init")
 ///     .layer(RetryLayer::new())
 ///     .finish();
 /// ```
-#[derive(Default, Clone)]
-pub struct RetryLayer(ExponentialBuilder);
+///
+/// ## Customize retry interceptor
+///
+/// RetryLayer accepts [`RetryInterceptor`] to allow users to customize
+/// their own retry interceptor logic.
+///
+/// ```
+/// use std::time::Duration;
+///
+/// use anyhow::Result;
+/// use opendal::layers::RetryInterceptor;
+/// use opendal::layers::RetryLayer;
+/// use opendal::services;
+/// use opendal::Error;
+/// use opendal::Operator;
+/// use opendal::Scheme;
+///
+/// struct MyRetryInterceptor;
+///
+/// impl RetryInterceptor for MyRetryInterceptor {
+///     fn intercept(&self, err: &Error, dur: Duration, ctx: &[(&str, &str)]) {
+///         // do something
+///     }
+/// }
+///
+/// let _ = Operator::new(services::Memory::default())
+///     .expect("must init")
+///     .layer(RetryLayer::new().with_notify(MyRetryInterceptor))
+///     .finish();
+/// ```
+pub struct RetryLayer<I = DefaultRetryInterceptor> {
+    builder: ExponentialBuilder,
+    notify: Arc<I>,
+}
+
+impl<I> Clone for RetryLayer<I> {
+    fn clone(&self) -> Self {
+        Self {
+            builder: self.builder.clone(),
+            notify: self.notify.clone(),
+        }
+    }
+}
+
+impl Default for RetryLayer {
+    fn default() -> Self {
+        Self {
+            builder: ExponentialBuilder::default(),
+            notify: Arc::new(DefaultRetryInterceptor),
+        }
+    }
+}
 
 impl RetryLayer {
     /// Create a new retry layer.
     /// # Examples
     ///
     /// ```
     /// use anyhow::Result;
@@ -83,233 +134,351 @@
     ///     .expect("must init")
     ///     .layer(RetryLayer::new());
     /// ```
     pub fn new() -> Self {
         Self::default()
     }
 
+    /// Set the retry interceptor as new notify.
+    ///
+    /// ```
+    /// use std::time::Duration;
+    ///
+    /// use anyhow::Result;
+    /// use opendal::layers::RetryInterceptor;
+    /// use opendal::layers::RetryLayer;
+    /// use opendal::services;
+    /// use opendal::Error;
+    /// use opendal::Operator;
+    /// use opendal::Scheme;
+    ///
+    /// struct MyRetryInterceptor;
+    ///
+    /// impl RetryInterceptor for MyRetryInterceptor {
+    ///     fn intercept(&self, err: &Error, dur: Duration, ctx: &[(&str, &str)]) {
+    ///         // do something
+    ///     }
+    /// }
+    ///
+    /// let _ = Operator::new(services::Memory::default())
+    ///     .expect("must init")
+    ///     .layer(RetryLayer::new().with_notify(MyRetryInterceptor))
+    ///     .finish();
+    /// ```
+    pub fn with_notify<I: RetryInterceptor>(self, notify: I) -> RetryLayer<I> {
+        RetryLayer {
+            builder: self.builder,
+            notify: Arc::new(notify),
+        }
+    }
+
     /// Set jitter of current backoff.
     ///
     /// If jitter is enabled, ExponentialBackoff will add a random jitter in `[0, min_delay)
     /// to current delay.
     pub fn with_jitter(mut self) -> Self {
-        self.0 = self.0.with_jitter();
+        self.builder = self.builder.with_jitter();
         self
     }
 
     /// Set factor of current backoff.
     ///
     /// # Panics
     ///
     /// This function will panic if input factor smaller than `1.0`.
     pub fn with_factor(mut self, factor: f32) -> Self {
-        self.0 = self.0.with_factor(factor);
+        self.builder = self.builder.with_factor(factor);
         self
     }
 
     /// Set min_delay of current backoff.
     pub fn with_min_delay(mut self, min_delay: Duration) -> Self {
-        self.0 = self.0.with_min_delay(min_delay);
+        self.builder = self.builder.with_min_delay(min_delay);
         self
     }
 
     /// Set max_delay of current backoff.
     ///
     /// Delay will not increasing if current delay is larger than max_delay.
     pub fn with_max_delay(mut self, max_delay: Duration) -> Self {
-        self.0 = self.0.with_max_delay(max_delay);
+        self.builder = self.builder.with_max_delay(max_delay);
         self
     }
 
     /// Set max_times of current backoff.
     ///
     /// Backoff will return `None` if max times is reaching.
     pub fn with_max_times(mut self, max_times: usize) -> Self {
-        self.0 = self.0.with_max_times(max_times);
+        self.builder = self.builder.with_max_times(max_times);
         self
     }
 }
 
-impl<A: Accessor> Layer<A> for RetryLayer {
-    type LayeredAccessor = RetryAccessor<A>;
+impl<A: Accessor, I: RetryInterceptor> Layer<A> for RetryLayer<I> {
+    type LayeredAccessor = RetryAccessor<A, I>;
 
     fn layer(&self, inner: A) -> Self::LayeredAccessor {
         RetryAccessor {
             inner,
-            builder: self.0.clone(),
+            builder: self.builder.clone(),
+            notify: self.notify.clone(),
         }
     }
 }
 
-#[derive(Clone)]
-pub struct RetryAccessor<A: Accessor> {
+/// RetryInterceptor is used to intercept while retry happened.
+pub trait RetryInterceptor: Send + Sync + 'static {
+    /// Everytime RetryLayer is retrying, this function will be called.
+    ///
+    /// # Timing
+    ///
+    /// just before the retry sleep.
+    ///
+    /// # Inputs
+    ///
+    /// - err: The error that caused the current retry.
+    /// - dur: The duration that will sleep before next retry.
+    /// - ctx: The context (`name`, `value`) of current operation, like `operation` and `path`.
+    ///
+    /// # Notes
+    ///
+    /// The intercept must be quick and non-blocking. No heavy IO is
+    /// allowed. Otherwise the retry will be blocked.
+    fn intercept(&self, err: &Error, dur: Duration, ctx: &[(&str, &str)]);
+}
+
+/// The DefaultRetryInterceptor will log the retry error in warning level.
+pub struct DefaultRetryInterceptor;
+
+impl RetryInterceptor for DefaultRetryInterceptor {
+    fn intercept(&self, err: &Error, dur: Duration, ctx: &[(&str, &str)]) {
+        let context = ctx
+            .iter()
+            .map(|(k, v)| format!("{}={}", k, v))
+            .collect::<Vec<_>>()
+            .join(" ");
+
+        warn!(
+            target: "opendal::service",
+            "{} -> retry after {}s: error={:?}",
+            context, dur.as_secs_f64(), err)
+    }
+}
+
+pub struct RetryAccessor<A: Accessor, I: RetryInterceptor> {
     inner: A,
     builder: ExponentialBuilder,
+    notify: Arc<I>,
 }
 
-impl<A: Accessor> Debug for RetryAccessor<A> {
+impl<A: Accessor, I: RetryInterceptor> Debug for RetryAccessor<A, I> {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("RetryAccessor")
             .field("inner", &self.inner)
             .finish_non_exhaustive()
     }
 }
 
 #[async_trait]
-impl<A: Accessor> LayeredAccessor for RetryAccessor<A> {
+impl<A: Accessor, I: RetryInterceptor> LayeredAccessor for RetryAccessor<A, I> {
     type Inner = A;
-    type Reader = RetryWrapper<A::Reader>;
-    type BlockingReader = RetryWrapper<A::BlockingReader>;
-    type Writer = RetryWrapper<A::Writer>;
-    type BlockingWriter = RetryWrapper<A::BlockingWriter>;
-    type Appender = RetryWrapper<A::Appender>;
-    type Pager = RetryWrapper<A::Pager>;
-    type BlockingPager = RetryWrapper<A::BlockingPager>;
+    type Reader = RetryWrapper<A::Reader, I>;
+    type BlockingReader = RetryWrapper<A::BlockingReader, I>;
+    type Writer = RetryWrapper<A::Writer, I>;
+    type BlockingWriter = RetryWrapper<A::BlockingWriter, I>;
+    type Appender = RetryWrapper<A::Appender, I>;
+    type Pager = RetryWrapper<A::Pager, I>;
+    type BlockingPager = RetryWrapper<A::BlockingPager, I>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
     async fn create_dir(&self, path: &str, args: OpCreateDir) -> Result<RpCreateDir> {
         { || self.inner.create_dir(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
-            .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::CreateDir, dur.as_secs_f64(), err)
+            .notify(|err, dur: Duration| {
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::CreateDir.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .map(|v| v.map_err(|e| e.set_persistent()))
             .await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         { || self.inner.read(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::Read, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[("operation", Operation::Read.into_static()), ("path", path)],
+                )
             })
             .map(|v| {
-                v.map(|(rp, r)| (rp, RetryWrapper::new(r, path, self.builder.clone())))
-                    .map_err(|e| e.set_persistent())
+                v.map(|(rp, r)| {
+                    (
+                        rp,
+                        RetryWrapper::new(r, self.notify.clone(), path, self.builder.clone()),
+                    )
+                })
+                .map_err(|e| e.set_persistent())
             })
             .await
     }
 
     /// Return `Interrupted` Error even after retry.
     ///
     /// Allowing users to retry the write request from upper logic.
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         { || self.inner.write(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::Write, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::Write.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .map(|v| {
-                v.map(|(rp, r)| (rp, RetryWrapper::new(r, path, self.builder.clone())))
-                    .map_err(|e| e.set_persistent())
+                v.map(|(rp, r)| {
+                    (
+                        rp,
+                        RetryWrapper::new(r, self.notify.clone(), path, self.builder.clone()),
+                    )
+                })
+                .map_err(|e| e.set_persistent())
             })
             .await
     }
 
     async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
         { || self.inner.append(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::Append, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::Append.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .map(|v| {
-                v.map(|(rp, r)| (rp, RetryWrapper::new(r, path, self.builder.clone())))
-                    .map_err(|e| e.set_persistent())
+                v.map(|(rp, r)| {
+                    (
+                        rp,
+                        RetryWrapper::new(r, self.notify.clone(), path, self.builder.clone()),
+                    )
+                })
+                .map_err(|e| e.set_persistent())
             })
             .await
     }
 
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         { || self.inner.stat(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::Stat, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[("operation", Operation::Stat.into_static()), ("path", path)],
+                )
             })
             .map(|v| v.map_err(|e| e.set_persistent()))
             .await
     }
 
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         { || self.inner.delete(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::Delete, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::Delete.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .map(|v| v.map_err(|e| e.set_persistent()))
             .await
     }
 
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         { || self.inner.copy(from, to, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::Copy, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::Copy.into_static()),
+                        ("from", from),
+                        ("to", to),
+                    ],
+                )
             })
             .map(|v| v.map_err(|e| e.set_persistent()))
             .await
     }
 
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         { || self.inner.rename(from, to, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::Rename, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::Rename.into_static()),
+                        ("from", from),
+                        ("to", to),
+                    ],
+                )
             })
             .map(|v| v.map_err(|e| e.set_persistent()))
             .await
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         { || self.inner.list(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::List, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[("operation", Operation::List.into_static()), ("path", path)],
+                )
             })
             .map(|v| {
                 v.map(|(l, p)| {
-                    let pager = RetryWrapper::new(p, path, self.builder.clone());
+                    let pager =
+                        RetryWrapper::new(p, self.notify.clone(), path, self.builder.clone());
                     (l, pager)
                 })
                 .map_err(|e| e.set_persistent())
             })
             .await
     }
 
@@ -324,135 +493,177 @@
                 }
                 Ok(RpBatch::new(nrp))
             }
         }
         .retry(&self.builder)
         .when(|e: &Error| e.is_temporary())
         .notify(|err, dur| {
-            warn!(
-                target: "opendal::service",
-                "operation={} -> retry after {}s: error={:?}",
-                Operation::Batch, dur.as_secs_f64(), err)
+            self.notify.intercept(
+                err,
+                dur,
+                &[
+                    ("operation", Operation::Batch.into_static()),
+                    ("count", &args.operation().len().to_string()),
+                ],
+            )
         })
         .await
         .map_err(|e| e.set_persistent())
     }
 
     fn blocking_create_dir(&self, path: &str, args: OpCreateDir) -> Result<RpCreateDir> {
         { || self.inner.blocking_create_dir(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::BlockingCreateDir, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::BlockingCreateDir.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         { || self.inner.blocking_read(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::BlockingRead, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::BlockingRead.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .call()
-            .map(|(rp, r)| (rp, RetryWrapper::new(r, path, self.builder.clone())))
+            .map(|(rp, r)| {
+                (
+                    rp,
+                    RetryWrapper::new(r, self.notify.clone(), path, self.builder.clone()),
+                )
+            })
             .map_err(|e| e.set_persistent())
     }
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         { || self.inner.blocking_write(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::BlockingWrite, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::BlockingWrite.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .call()
-            .map(|(rp, r)| (rp, RetryWrapper::new(r, path, self.builder.clone())))
+            .map(|(rp, r)| {
+                (
+                    rp,
+                    RetryWrapper::new(r, self.notify.clone(), path, self.builder.clone()),
+                )
+            })
             .map_err(|e| e.set_persistent())
     }
 
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         { || self.inner.blocking_stat(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::BlockingStat, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::BlockingStat.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         { || self.inner.blocking_delete(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::BlockingDelete, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::BlockingDelete.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
         { || self.inner.blocking_list(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
-                warn!(
-                    target: "opendal::service",
-                    "operation={} -> retry after {}s: error={:?}",
-                    Operation::BlockingList, dur.as_secs_f64(), err)
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", Operation::BlockingList.into_static()),
+                        ("path", path),
+                    ],
+                )
             })
             .call()
             .map(|(rp, p)| {
-                let p = RetryWrapper::new(p, path, self.builder.clone());
+                let p = RetryWrapper::new(p, self.notify.clone(), path, self.builder.clone());
                 (rp, p)
             })
             .map_err(|e| e.set_persistent())
     }
 }
 
-pub struct RetryWrapper<R> {
+pub struct RetryWrapper<R, I> {
     inner: R,
+    notify: Arc<I>,
+
     path: String,
     builder: ExponentialBuilder,
     current_backoff: Option<ExponentialBackoff>,
     sleep: Option<Pin<Box<tokio::time::Sleep>>>,
 }
 
-impl<R> RetryWrapper<R> {
-    fn new(inner: R, path: &str, backoff: ExponentialBuilder) -> Self {
+impl<R, I> RetryWrapper<R, I> {
+    fn new(inner: R, notify: Arc<I>, path: &str, backoff: ExponentialBuilder) -> Self {
         Self {
             inner,
+            notify,
+
             path: path.to_string(),
             builder: backoff,
             current_backoff: None,
             sleep: None,
         }
     }
 }
 
-impl<R: oio::Read> oio::Read for RetryWrapper<R> {
+impl<R: oio::Read, I: RetryInterceptor> oio::Read for RetryWrapper<R, I> {
     fn poll_read(&mut self, cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
         if let Some(sleep) = self.sleep.as_mut() {
             ready!(sleep.poll_unpin(cx));
             self.sleep = None;
         }
 
         match ready!(self.inner.poll_read(cx, buf)) {
@@ -475,18 +686,22 @@
 
                 match backoff.next() {
                     None => {
                         self.current_backoff = None;
                         Poll::Ready(Err(err))
                     }
                     Some(dur) => {
-                        warn!(
-                            target: "opendal::service",
-                            "operation={} path={} -> retry after {}s: error={:?}",
-                            ReadOperation::Read, self.path, dur.as_secs_f64(), err);
+                        self.notify.intercept(
+                            &err,
+                            dur,
+                            &[
+                                ("operation", ReadOperation::Read.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         self.sleep = Some(Box::pin(tokio::time::sleep(dur)));
                         self.poll_read(cx, buf)
                     }
                 }
             }
         }
     }
@@ -517,18 +732,22 @@
 
                 match backoff.next() {
                     None => {
                         self.current_backoff = None;
                         Poll::Ready(Err(err))
                     }
                     Some(dur) => {
-                        warn!(
-                            target: "opendal::service",
-                            "operation={} path={} -> retry after {}s: error={:?}",
-                             ReadOperation::Seek, self.path, dur.as_secs_f64(), err);
+                        self.notify.intercept(
+                            &err,
+                            dur,
+                            &[
+                                ("operation", ReadOperation::Seek.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         self.sleep = Some(Box::pin(tokio::time::sleep(dur)));
                         self.poll_seek(cx, pos)
                     }
                 }
             }
         }
     }
@@ -563,87 +782,108 @@
 
                 match backoff.next() {
                     None => {
                         self.current_backoff = None;
                         Poll::Ready(Some(Err(err)))
                     }
                     Some(dur) => {
-                        warn!(
-                            target: "opendal::service",
-                            "operation={} path={} -> retry after {}s: error={:?}",
-                            ReadOperation::Next, self.path, dur.as_secs_f64(), err);
+                        self.notify.intercept(
+                            &err,
+                            dur,
+                            &[
+                                ("operation", ReadOperation::Next.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         self.sleep = Some(Box::pin(tokio::time::sleep(dur)));
                         self.poll_next(cx)
                     }
                 }
             }
         }
     }
 }
 
-impl<R: oio::BlockingRead> oio::BlockingRead for RetryWrapper<R> {
+impl<R: oio::BlockingRead, I: RetryInterceptor> oio::BlockingRead for RetryWrapper<R, I> {
     fn read(&mut self, buf: &mut [u8]) -> Result<usize> {
         { || self.inner.read(buf) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
-            .notify(move |err, dur| {
-                warn!(
-                target: "opendal::service",
-                "operation={} -> pager retry after {}s: error={:?}",
-                ReadOperation::BlockingRead, dur.as_secs_f64(), err)
+            .notify(|err, dur| {
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", ReadOperation::BlockingRead.into_static()),
+                        ("path", &self.path),
+                    ],
+                );
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
     fn seek(&mut self, pos: io::SeekFrom) -> Result<u64> {
         { || self.inner.seek(pos) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
-            .notify(move |err, dur| {
-                warn!(
-                target: "opendal::service",
-                "operation={} -> pager retry after {}s: error={:?}",
-                ReadOperation::BlockingSeek, dur.as_secs_f64(), err)
+            .notify(|err, dur| {
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", ReadOperation::BlockingSeek.into_static()),
+                        ("path", &self.path),
+                    ],
+                );
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
     fn next(&mut self) -> Option<Result<Bytes>> {
         { || self.inner.next().transpose() }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
-            .notify(move |err, dur| {
-                warn!(
-                target: "opendal::service",
-                "operation={} -> pager retry after {}s: error={:?}",
-                ReadOperation::BlockingNext, dur.as_secs_f64(), err)
+            .notify(|err, dur| {
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", ReadOperation::BlockingNext.into_static()),
+                        ("path", &self.path),
+                    ],
+                );
             })
             .call()
             .map_err(|e| e.set_persistent())
             .transpose()
     }
 }
 
 #[async_trait]
-impl<R: oio::Write> oio::Write for RetryWrapper<R> {
+impl<R: oio::Write, I: RetryInterceptor> oio::Write for RetryWrapper<R, I> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let mut backoff = self.builder.build();
 
         loop {
             match self.inner.write(bs.clone()).await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
                 Err(e) => match backoff.next() {
                     None => return Err(e),
                     Some(dur) => {
-                        warn!(target: "opendal::service",
-                              "operation={} path={} -> pager retry after {}s: error={:?}",
-                              WriteOperation::Write, self.path, dur.as_secs_f64(), e);
+                        self.notify.intercept(
+                            &e,
+                            dur,
+                            &[
+                                ("operation", WriteOperation::Write.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         tokio::time::sleep(dur).await;
                         continue;
                     }
                 },
             }
         }
     }
@@ -659,17 +899,22 @@
         loop {
             match self.inner.abort().await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
                 Err(e) => match backoff.next() {
                     None => return Err(e),
                     Some(dur) => {
-                        warn!(target: "opendal::service",
-                              "operation={} path={} -> pager retry after {}s: error={:?}",
-                              WriteOperation::Abort, self.path, dur.as_secs_f64(), e);
+                        self.notify.intercept(
+                            &e,
+                            dur,
+                            &[
+                                ("operation", WriteOperation::Abort.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         tokio::time::sleep(dur).await;
                         continue;
                     }
                 },
             }
         }
     }
@@ -680,71 +925,89 @@
         loop {
             match self.inner.close().await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
                 Err(e) => match backoff.next() {
                     None => return Err(e),
                     Some(dur) => {
-                        warn!(target: "opendal::service",
-                              "operation={} path={} -> pager retry after {}s: error={:?}",
-                              WriteOperation::Close, self.path, dur.as_secs_f64(), e);
+                        self.notify.intercept(
+                            &e,
+                            dur,
+                            &[
+                                ("operation", WriteOperation::Close.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         tokio::time::sleep(dur).await;
                         continue;
                     }
                 },
             }
         }
     }
 }
 
-impl<R: oio::BlockingWrite> oio::BlockingWrite for RetryWrapper<R> {
+impl<R: oio::BlockingWrite, I: RetryInterceptor> oio::BlockingWrite for RetryWrapper<R, I> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
         { || self.inner.write(bs.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
-            .notify(move |err, dur| {
-                warn!(
-                target: "opendal::service",
-                "operation={} -> pager retry after {}s: error={:?}",
-                WriteOperation::BlockingWrite, dur.as_secs_f64(), err)
+            .notify(|err, dur| {
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", WriteOperation::BlockingWrite.into_static()),
+                        ("path", &self.path),
+                    ],
+                );
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
     fn close(&mut self) -> Result<()> {
         { || self.inner.close() }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
-            .notify(move |err, dur| {
-                warn!(
-                target: "opendal::service",
-                "operation={} -> pager retry after {}s: error={:?}",
-               WriteOperation::BlockingClose, dur.as_secs_f64(), err)
+            .notify(|err, dur| {
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", WriteOperation::BlockingClose.into_static()),
+                        ("path", &self.path),
+                    ],
+                );
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 }
 
 #[async_trait]
-impl<A: oio::Append> oio::Append for RetryWrapper<A> {
+impl<A: oio::Append, I: RetryInterceptor> oio::Append for RetryWrapper<A, I> {
     async fn append(&mut self, bs: Bytes) -> Result<()> {
         let mut backoff = self.builder.build();
 
         loop {
             match self.inner.append(bs.clone()).await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
                 Err(e) => match backoff.next() {
                     None => return Err(e),
                     Some(dur) => {
-                        warn!(target: "opendal::service",
-                              "operation={} path={} -> appender retry after {}s: error={:?}",
-                              AppendOperation::Append, self.path, dur.as_secs_f64(), e);
+                        self.notify.intercept(
+                            &e,
+                            dur,
+                            &[
+                                ("operation", AppendOperation::Append.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         tokio::time::sleep(dur).await;
                         continue;
                     }
                 },
             }
         }
     }
@@ -755,60 +1018,74 @@
         loop {
             match self.inner.close().await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
                 Err(e) => match backoff.next() {
                     None => return Err(e),
                     Some(dur) => {
-                        warn!(target: "opendal::service",
-                              "operation={} path={} -> appender retry after {}s: error={:?}",
-                              AppendOperation::Close, self.path, dur.as_secs_f64(), e);
+                        self.notify.intercept(
+                            &e,
+                            dur,
+                            &[
+                                ("operation", AppendOperation::Close.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         tokio::time::sleep(dur).await;
                         continue;
                     }
                 },
             }
         }
     }
 }
 
 #[async_trait]
-impl<P: oio::Page> oio::Page for RetryWrapper<P> {
+impl<P: oio::Page, I: RetryInterceptor> oio::Page for RetryWrapper<P, I> {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         let mut backoff = self.builder.build();
 
         loop {
             match self.inner.next().await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
                 Err(e) => match backoff.next() {
                     None => return Err(e),
                     Some(dur) => {
-                        warn!(target: "opendal::service",
-                              "operation={} path={} -> pager retry after {}s: error={:?}",
-                              PageOperation::Next, self.path, dur.as_secs_f64(), e);
+                        self.notify.intercept(
+                            &e,
+                            dur,
+                            &[
+                                ("operation", PageOperation::Next.into_static()),
+                                ("path", &self.path),
+                            ],
+                        );
                         tokio::time::sleep(dur).await;
                         continue;
                     }
                 },
             }
         }
     }
 }
 
-impl<P: oio::BlockingPage> oio::BlockingPage for RetryWrapper<P> {
+impl<P: oio::BlockingPage, I: RetryInterceptor> oio::BlockingPage for RetryWrapper<P, I> {
     fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         { || self.inner.next() }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
-            .notify(move |err, dur| {
-                warn!(
-                target: "opendal::service",
-                "operation={} -> pager retry after {}s: error={:?}",
-                PageOperation::BlockingNext, dur.as_secs_f64(), err)
+            .notify(|err, dur| {
+                self.notify.intercept(
+                    err,
+                    dur,
+                    &[
+                        ("operation", PageOperation::BlockingNext.into_static()),
+                        ("path", &self.path),
+                    ],
+                );
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 }
 
 #[cfg(test)]
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/throttle.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/throttle.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/timeout.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/timeout.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.39.0/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/lib.rs` & `opendal-0.39.0/local_dependencies/opendal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 use futures::TryStreamExt;
 use http::Request;
 use http::Response;
 
 use super::body::IncomingAsyncBody;
 use super::parse_content_length;
 use super::AsyncBody;
-use crate::raw::oio::into_stream;
+use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
 /// HttpClient that used across opendal.
 #[derive(Clone)]
 pub struct HttpClient {
@@ -146,17 +146,14 @@
             // it to interrupt so we can retry it.
             Error::new(ErrorKind::Unexpected, "read data from http stream")
                 .map(|v| if err.is_body() { v.set_temporary() } else { v })
                 .with_context("url", uri.to_string())
                 .set_source(err)
         });
 
-        let body = IncomingAsyncBody::new(
-            Box::new(into_stream::from_futures_stream(stream)),
-            content_length,
-        );
+        let body = IncomingAsyncBody::new(Box::new(oio::into_stream(stream)), content_length);
 
         let resp = hr.body(body).expect("response must build succeed");
 
         Ok(resp)
     }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -47,16 +47,15 @@
 mod uri;
 pub use uri::percent_encode_path;
 
 mod error;
 pub use error::new_request_build_error;
 pub use error::new_request_credential_error;
 pub use error::new_request_sign_error;
-pub use error::parse_error_response;
-pub use error::ErrorResponse;
+pub use error::with_error_response_context;
 
 mod bytes_range;
 pub use bytes_range::BytesRange;
 
 mod bytes_content_range;
 pub use bytes_content_range::BytesContentRange;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/multipart.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/multipart.rs`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 use http::StatusCode;
 use http::Uri;
 use http::Version;
 
 use super::new_request_build_error;
 use super::AsyncBody;
 use super::IncomingAsyncBody;
-use crate::raw::oio::into_stream;
+use crate::raw::oio;
 use crate::*;
 
 /// Multipart is a builder for multipart/form-data.
 #[derive(Debug)]
 pub struct Multipart<T: Part> {
     boundary: String,
     parts: Vec<T>,
@@ -316,15 +316,15 @@
         builder = builder.version(self.version);
         // Swap headers directly instead of copy the entire map.
         mem::swap(builder.headers_mut().unwrap(), &mut self.headers);
 
         let bs: Bytes = self.content;
         let length = bs.len();
         let body = IncomingAsyncBody::new(
-            Box::new(into_stream::from_futures_stream(stream::iter(vec![Ok(bs)]))),
+            Box::new(oio::into_stream(stream::iter(vec![Ok(bs)]))),
             Some(length as u64),
         );
 
         builder
             .body(body)
             .expect("mixed part must be valid response")
     }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/mod.rs`

 * *Files 19% similar despite different names*

```diff
@@ -23,36 +23,24 @@
 //!   access raw APIs.
 //! - Raw APIs should only be accessed via `opendal::raw::Xxxx`, any public
 //!   API should never expose raw API directly.
 //! - Raw APIs are far more less stable than public API, please don't rely on
 //!   them whenever possible.
 
 mod accessor;
-pub use accessor::Accessor;
-pub use accessor::AccessorInfo;
-pub use accessor::FusedAccessor;
+pub use accessor::*;
 
 mod layer;
-pub use layer::Layer;
-pub use layer::LayeredAccessor;
-
-pub mod oio;
+pub use layer::*;
 
 mod path;
-pub use path::build_abs_path;
-pub use path::build_rel_path;
-pub use path::build_rooted_abs_path;
-pub use path::get_basename;
-pub use path::get_parent;
-pub use path::normalize_path;
-pub use path::normalize_root;
-pub use path::validate_path;
+pub use path::*;
 
 mod operation;
-pub use operation::Operation;
+pub use operation::*;
 
 mod version;
 pub use version::VERSION;
 
 mod rps;
 pub use rps::*;
 
@@ -66,7 +54,8 @@
 pub use serde_util::*;
 
 mod chrono_util;
 pub use chrono_util::*;
 
 // Expose as a pub mod to avoid confusing.
 pub mod adapters;
+pub mod oio;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/append.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/append/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! into_blocking_reader will provide different implementations to convert
-//! into [`oio::BlockingRead`][crate::raw::oio::BlockingRead]
+mod backend;
+pub use backend::HdfsBuilder as Hdfs;
 
-mod from_fd;
-pub use from_fd::from_fd;
-pub use from_fd::FdReader;
+mod appender;
+mod error;
+mod pager;
+mod writer;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/into_seekable_read_by_range.rs`

 * *Files 2% similar despite different names*

```diff
@@ -28,39 +28,47 @@
 use tokio::io::ReadBuf;
 
 use crate::raw::*;
 use crate::*;
 
 /// Convert given reader into [`oio::Reader`] by range.
 ///
+/// # Input
+///
+/// The input is an Accessor will may return a non-seekable reader.
+///
+/// # Output
+///
+/// The output is a reader that can be seek by range.
+///
 /// # Notes
 ///
 /// This operation is not zero cost. If the accessor already returns a
 /// seekable reader, please don't use this.
-pub fn by_range<A: Accessor>(
+pub fn into_seekable_read_by_range<A: Accessor>(
     acc: Arc<A>,
     path: &str,
     reader: A::Reader,
     offset: u64,
     size: u64,
-) -> RangeReader<A> {
-    RangeReader {
+) -> ByRangeSeekableReader<A> {
+    ByRangeSeekableReader {
         acc,
         path: path.to_string(),
         offset,
         size,
         cur: 0,
         state: State::Reading(reader),
         last_seek_pos: None,
         sink: Vec::new(),
     }
 }
 
-/// RangeReader that can do seek on non-seekable reader.
-pub struct RangeReader<A: Accessor> {
+/// ByRangeReader that can do seek on non-seekable reader.
+pub struct ByRangeSeekableReader<A: Accessor> {
     acc: Arc<A>,
     path: String,
 
     offset: u64,
     size: u64,
     cur: u64,
     state: State<A::Reader>,
@@ -80,15 +88,15 @@
     Sending(BoxFuture<'static, Result<(RpRead, R)>>),
     Reading(R),
 }
 
 /// Safety: State will only be accessed under &mut.
 unsafe impl<R: oio::Read> Sync for State<R> {}
 
-impl<A: Accessor> RangeReader<A> {
+impl<A: Accessor> ByRangeSeekableReader<A> {
     fn read_future(&self) -> BoxFuture<'static, Result<(RpRead, A::Reader)>> {
         let acc = self.acc.clone();
         let path = self.path.clone();
         let op = OpRead::default().with_range(BytesRange::new(
             Some(self.offset + self.cur),
             Some(self.size - self.cur),
         ));
@@ -119,15 +127,15 @@
                 ))
             }
         };
         Ok(n)
     }
 }
 
-impl<A: Accessor> oio::Read for RangeReader<A> {
+impl<A: Accessor> oio::Read for ByRangeSeekableReader<A> {
     fn poll_read(&mut self, cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
         match &mut self.state {
             State::Idle => {
                 if self.cur >= self.size {
                     return Poll::Ready(Ok(0));
                 }
 
@@ -383,15 +391,16 @@
     async fn test_read_all() -> anyhow::Result<()> {
         let (bs, _) = gen_bytes();
         let acc = Arc::new(MockReadService::new(bs.clone()));
 
         let r = MockReader {
             inner: futures::io::Cursor::new(bs.to_vec()),
         };
-        let mut r = Box::new(by_range(acc, "x", r, 0, bs.len() as u64)) as oio::Reader;
+        let mut r =
+            Box::new(into_seekable_read_by_range(acc, "x", r, 0, bs.len() as u64)) as oio::Reader;
 
         let mut buf = Vec::new();
         r.read_to_end(&mut buf).await?;
         assert_eq!(bs.len(), buf.len(), "read size");
         assert_eq!(
             format!("{:x}", Sha256::digest(&bs)),
             format!("{:x}", Sha256::digest(&buf)),
@@ -417,15 +426,15 @@
     async fn test_read_part() -> anyhow::Result<()> {
         let (bs, _) = gen_bytes();
         let acc = Arc::new(MockReadService::new(bs.clone()));
 
         let r = MockReader {
             inner: futures::io::Cursor::new(bs[4096..4096 + 4096].to_vec()),
         };
-        let mut r = Box::new(by_range(acc, "x", r, 4096, 4096)) as oio::Reader;
+        let mut r = Box::new(into_seekable_read_by_range(acc, "x", r, 4096, 4096)) as oio::Reader;
 
         let mut buf = Vec::new();
         r.read_to_end(&mut buf).await?;
         assert_eq!(4096, buf.len(), "read size");
         assert_eq!(
             format!("{:x}", Sha256::digest(&bs[4096..4096 + 4096])),
             format!("{:x}", Sha256::digest(&buf)),
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files 21% similar despite different names*

```diff
@@ -11,112 +11,109 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::cmp;
-use std::io::SeekFrom;
+use std::io;
 use std::pin::Pin;
 use std::task::ready;
 use std::task::Context;
 use std::task::Poll;
 
+use bb8::PooledConnection;
+use futures::future::BoxFuture;
 use futures::AsyncRead;
-use futures::AsyncSeek;
+use futures::FutureExt;
+use suppaftp::Status;
 
+use super::backend::Manager;
 use crate::raw::*;
 use crate::*;
 
-/// Convert given fd into [`oio::Reader`].
-pub fn from_fd<R>(fd: R, start: u64, end: u64) -> FdReader<R>
-where
-    R: AsyncRead + AsyncSeek + Unpin + Send + Sync,
-{
-    FdReader {
-        inner: fd,
-        start,
-        end,
-        offset: 0,
-    }
+/// Wrapper for ftp data stream and command stream.
+pub struct FtpReader {
+    reader: Box<dyn AsyncRead + Send + Unpin>,
+    state: State,
 }
 
-/// FdReader is a wrapper of input fd to implement [`oio::Read`].
-pub struct FdReader<R: AsyncRead + AsyncSeek + Unpin + Send + Sync> {
-    inner: R,
-
-    start: u64,
-    end: u64,
-    offset: u64,
+unsafe impl Sync for FtpReader {}
+
+pub enum State {
+    Reading(Option<PooledConnection<'static, Manager>>),
+    Finalize(BoxFuture<'static, Result<()>>),
 }
 
-impl<R> FdReader<R>
-where
-    R: AsyncRead + AsyncSeek + Unpin + Send + Sync,
-{
-    pub(crate) fn current_size(&self) -> i64 {
-        debug_assert!(self.offset >= self.start, "offset must in range");
-        self.end as i64 - self.offset as i64
+impl FtpReader {
+    /// Create an instance of FtpReader.
+    pub fn new(
+        r: Box<dyn AsyncRead + Send + Unpin>,
+        c: PooledConnection<'static, Manager>,
+    ) -> Self {
+        Self {
+            reader: r,
+            state: State::Reading(Some(c)),
+        }
     }
 }
 
-impl<R> oio::Read for FdReader<R>
-where
-    R: AsyncRead + AsyncSeek + Unpin + Send + Sync,
-{
+impl oio::Read for FtpReader {
     fn poll_read(&mut self, cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
-        if self.current_size() <= 0 {
-            return Poll::Ready(Ok(0));
-        }
+        let data = Pin::new(&mut self.reader).poll_read(cx, buf);
+
+        match &mut self.state {
+            // Reading state, try to poll some data.
+            State::Reading(stream) => {
+                match stream {
+                    Some(_) => {
+                        // when hit Err or EOF, consume ftpstream, change state to Finalize and send fut.
+                        if let Poll::Ready(Err(_)) | Poll::Ready(Ok(0)) = data {
+                            let mut ft = stream.take().unwrap();
+
+                            let fut = async move {
+                                ft.read_response_in(&[
+                                    Status::ClosingDataConnection,
+                                    Status::RequestedFileActionOk,
+                                ])
+                                .await?;
+
+                                Ok(())
+                            };
+                            self.state = State::Finalize(Box::pin(fut));
+                        } else {
+                            // Otherwise, exit and return data.
+                            return data.map_err(|err| {
+                                Error::new(ErrorKind::Unexpected, "read data from ftp data stream")
+                                    .set_source(err)
+                            });
+                        }
+
+                        self.poll_read(cx, buf)
+                    }
+                    // We could never reach this branch because we will change to Finalize state once we consume ftp stream.
+                    None => unreachable!(),
+                }
+            }
 
-        let max = cmp::min(buf.len() as u64, self.current_size() as u64) as usize;
-        // TODO: we can use pread instead.
-        let n =
-            ready!(Pin::new(&mut self.inner).poll_read(cx, &mut buf[..max])).map_err(|err| {
-                Error::new(ErrorKind::Unexpected, "read data from FdReader")
-                    .with_context("source", "FdReader")
-                    .set_source(err)
-            })?;
-        self.offset += n as u64;
-        Poll::Ready(Ok(n))
+            // Finalize state, wait for finalization of stream.
+            State::Finalize(fut) => match ready!(Pin::new(fut).poll_unpin(cx)) {
+                Ok(_) => Poll::Ready(Ok(0)),
+                Err(e) => Poll::Ready(Err(e)),
+            },
+        }
     }
 
-    /// TODO: maybe we don't need to do seek really, just call pread instead.
-    ///
-    /// We need to wait for tokio's pread support.
-    fn poll_seek(&mut self, cx: &mut Context<'_>, pos: SeekFrom) -> Poll<Result<u64>> {
-        let (base, offset) = match pos {
-            SeekFrom::Start(n) => (self.start as i64, n as i64),
-            SeekFrom::End(n) => (self.end as i64, n),
-            SeekFrom::Current(n) => (self.offset as i64, n),
-        };
-
-        match base.checked_add(offset) {
-            Some(n) if n < 0 => Poll::Ready(Err(Error::new(
-                ErrorKind::InvalidInput,
-                "invalid seek to a negative or overflowing position",
-            ))),
-            Some(n) => {
-                let cur =
-                    ready!(Pin::new(&mut self.inner).poll_seek(cx, SeekFrom::Start(n as u64)))
-                        .map_err(|err| {
-                            Error::new(ErrorKind::Unexpected, "seek data from FdReader")
-                                .with_context("source", "FdReader")
-                                .set_source(err)
-                        })?;
+    fn poll_seek(&mut self, cx: &mut Context<'_>, pos: io::SeekFrom) -> Poll<Result<u64>> {
+        let (_, _) = (cx, pos);
 
-                self.offset = cur;
-                Poll::Ready(Ok(self.offset - self.start))
-            }
-            None => Poll::Ready(Err(Error::new(
-                ErrorKind::InvalidInput,
-                "invalid seek to a negative or overflowing position",
-            ))),
-        }
+        Poll::Ready(Err(Error::new(
+            ErrorKind::Unsupported,
+            "output reader doesn't support seeking",
+        )))
     }
 
     fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<bytes::Bytes>>> {
         let _ = cx;
 
         Poll::Ready(Some(Err(Error::new(
             ErrorKind::Unsupported,
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_reader.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/stream/into_stream_from_reader.rs`

 * *Files 18% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 use crate::raw::*;
 use crate::*;
 
 // TODO: 64KiB is picked based on experiences, should be configurable
 const DEFAULT_CAPACITY: usize = 64 * 1024;
 
 /// Convert given futures reader into [`oio::Stream`].
-pub fn from_futures_reader<R>(r: R) -> FromFuturesReader<R>
+pub fn into_stream_from_reader<R>(r: R) -> FromReaderStream<R>
 where
     R: AsyncRead + Send + Sync + Unpin,
 {
-    FromFuturesReader {
+    FromReaderStream {
         inner: Some(r),
         buf: BytesMut::new(),
     }
 }
 
-pub struct FromFuturesReader<R> {
+pub struct FromReaderStream<R> {
     inner: Option<R>,
     buf: BytesMut,
 }
 
-impl<S> oio::Stream for FromFuturesReader<S>
+impl<S> oio::Stream for FromReaderStream<S>
 where
     S: AsyncRead + Send + Sync + Unpin,
 {
     fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<Bytes>>> {
         let reader = match self.inner.as_mut() {
             Some(r) => r,
             None => return Poll::Ready(None),
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_stream.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/stream/into_stream.rs`

 * *Files 14% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 use bytes::Bytes;
 use futures::TryStreamExt;
 
 use crate::raw::*;
 use crate::*;
 
 /// Convert given futures stream into [`oio::Stream`].
-pub fn from_futures_stream<S>(stream: S) -> FromFuturesStream<S>
+pub fn into_stream<S>(stream: S) -> IntoStream<S>
 where
     S: futures::Stream<Item = Result<Bytes>> + Send + Sync + Unpin,
 {
-    FromFuturesStream { inner: stream }
+    IntoStream { inner: stream }
 }
 
-pub struct FromFuturesStream<S> {
+pub struct IntoStream<S> {
     inner: S,
 }
 
-impl<S> oio::Stream for FromFuturesStream<S>
+impl<S> oio::Stream for IntoStream<S>
 where
     S: futures::Stream<Item = Result<Bytes>> + Send + Sync + Unpin,
 {
     fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<Bytes>>> {
         self.inner.try_poll_next_unpin(cx)
     }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,12 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! into_stream will provide different implementations to convert into
-//! [`oio::Stream`][crate::raw::oio::Stream]
+mod backend;
+pub use backend::GhacBuilder as Ghac;
 
-mod from_futures_stream;
-pub use from_futures_stream::from_futures_stream;
-
-mod from_futures_reader;
-pub use from_futures_reader::from_futures_reader;
+mod error;
+mod writer;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/into_streamable_read.rs`

 * *Files 4% similar despite different names*

```diff
@@ -22,31 +22,31 @@
 
 use bytes::Bytes;
 use tokio::io::ReadBuf;
 
 use crate::raw::*;
 use crate::*;
 
-/// as_streamable is used to make [`oio::Read`] or [`oio::BlockingRead`] streamable.
-pub fn into_streamable_reader<R>(r: R, capacity: usize) -> IntoStreamableReader<R> {
-    IntoStreamableReader {
+/// into_streamable is used to make [`oio::Read`] or [`oio::BlockingRead`] streamable.
+pub fn into_streamable_read<R>(r: R, capacity: usize) -> StreamableReader<R> {
+    StreamableReader {
         r,
         cap: capacity,
         buf: Vec::with_capacity(capacity),
     }
 }
 
 /// Make given read streamable.
-pub struct IntoStreamableReader<R> {
+pub struct StreamableReader<R> {
     r: R,
     cap: usize,
     buf: Vec<u8>,
 }
 
-impl<R: oio::Read> oio::Read for IntoStreamableReader<R> {
+impl<R: oio::Read> oio::Read for StreamableReader<R> {
     fn poll_read(&mut self, cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
         self.r.poll_read(cx, buf)
     }
 
     fn poll_seek(&mut self, cx: &mut Context<'_>, pos: SeekFrom) -> Poll<Result<u64>> {
         self.r.poll_seek(cx, pos)
     }
@@ -63,15 +63,15 @@
                 buf.set_filled(n);
                 Poll::Ready(Some(Ok(Bytes::from(buf.filled().to_vec()))))
             }
         }
     }
 }
 
-impl<R: oio::BlockingRead> oio::BlockingRead for IntoStreamableReader<R> {
+impl<R: oio::BlockingRead> oio::BlockingRead for StreamableReader<R> {
     fn read(&mut self, buf: &mut [u8]) -> Result<usize> {
         self.r.read(buf)
     }
 
     fn seek(&mut self, pos: SeekFrom) -> Result<u64> {
         self.r.seek(pos)
     }
@@ -109,15 +109,15 @@
         let size = rng.gen_range(1..16 * 1024 * 1024);
         let mut content = vec![0; size];
         rng.fill_bytes(&mut content);
         // Generate cap between 1B..1MB;
         let cap = rng.gen_range(1..1024 * 1024);
 
         let r = oio::Cursor::from(content.clone());
-        let mut s = into_streamable_reader(Box::new(r) as oio::Reader, cap);
+        let mut s = into_streamable_read(Box::new(r) as oio::Reader, cap);
 
         let mut bs = BytesMut::new();
         while let Some(b) = s.next().await {
             let b = b.expect("read must success");
             bs.put_slice(&b);
         }
         assert_eq!(bs.freeze().to_vec(), content)
@@ -132,15 +132,15 @@
         let size = rng.gen_range(1..16 * 1024 * 1024);
         let mut content = vec![0; size];
         rng.fill_bytes(&mut content);
         // Generate cap between 1B..1MB;
         let cap = rng.gen_range(1..1024 * 1024);
 
         let r = oio::Cursor::from(content.clone());
-        let mut s = into_streamable_reader(Box::new(r) as oio::BlockingReader, cap);
+        let mut s = into_streamable_read(Box::new(r) as oio::BlockingReader, cap);
 
         let mut bs = BytesMut::new();
         while let Some(b) = s.next() {
             let b = b.expect("read must success");
             bs.put_slice(&b);
         }
         assert_eq!(bs.freeze().to_vec(), content)
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/mod.rs`

 * *Files 25% similar despite different names*

```diff
@@ -11,68 +11,53 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! `oio` provides OpenDAL's raw traits and types that opendal returns as
-//! output.
-//!
-//! Those types should only be used internally and we don't want users to
-//! depend on them. So we should also implement trait like `AsyncRead` for
-//! our `output` traits.
-
-mod read;
-pub use read::BlockingRead;
-pub use read::BlockingReader;
-pub use read::Read;
-pub use read::ReadExt;
-pub use read::ReadOperation;
-pub use read::Reader;
-
-pub mod into_blocking_reader;
-pub mod into_reader;
-
-mod write;
-pub use write::BlockingWrite;
-pub use write::BlockingWriter;
-pub use write::Write;
-pub use write::WriteOperation;
-pub use write::Writer;
-
-mod append;
-pub use append::Append;
-pub use append::AppendOperation;
-pub use append::Appender;
-
-mod stream;
-pub use stream::Stream;
-pub use stream::Streamer;
-
-pub mod into_stream;
-
-mod cursor;
-pub use cursor::Cursor;
-pub use cursor::VectorCursor;
-
-mod into_streamable;
-pub use into_streamable::into_streamable_reader;
-pub use into_streamable::IntoStreamableReader;
+mod mode;
+pub use mode::EntryMode;
 
 mod entry;
 pub use entry::Entry;
 
-mod page;
-pub use page::BlockingPage;
-pub use page::BlockingPager;
-pub use page::Page;
-pub use page::PageOperation;
-pub use page::Pager;
-
-mod to_flat_pager;
-pub use to_flat_pager::to_flat_pager;
-pub use to_flat_pager::ToFlatPager;
-
-mod to_hierarchy_pager;
-pub use to_hierarchy_pager::to_hierarchy_pager;
-pub use to_hierarchy_pager::ToHierarchyPager;
+mod metadata;
+pub use metadata::Metadata;
+pub use metadata::Metakey;
+
+mod reader;
+pub use reader::BlockingReader;
+pub use reader::Reader;
+
+mod writer;
+pub use writer::BlockingWriter;
+pub use writer::Writer;
+
+mod appender;
+pub use appender::Appender;
+
+mod list;
+pub use list::BlockingLister;
+pub use list::Lister;
+
+mod operator;
+pub use operator::operator_functions;
+pub use operator::operator_futures;
+pub use operator::BlockingOperator;
+pub use operator::Operator;
+pub use operator::OperatorBuilder;
+pub use operator::OperatorInfo;
+
+mod builder;
+pub use builder::Builder;
+
+mod error;
+pub use error::Error;
+pub use error::ErrorKind;
+pub use error::Result;
+
+mod scheme;
+pub use scheme::Scheme;
+
+mod capability;
+pub use capability::Capability;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/page/api.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 // under the License.
 
 use std::fmt::Display;
 use std::fmt::Formatter;
 
 use async_trait::async_trait;
 
-use super::Entry;
+use crate::raw::oio::Entry;
 use crate::*;
 
 /// PageOperation is the name for APIs of pager.
 #[derive(Debug, Copy, Clone, Hash, Eq, PartialEq)]
 #[non_exhaustive]
 pub enum PageOperation {
     /// Operation for [`Page::next`]
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/read/api.rs`

 * *Files 6% similar despite different names*

```diff
@@ -152,28 +152,26 @@
 impl futures::AsyncRead for dyn Read {
     fn poll_read(
         mut self: Pin<&mut Self>,
         cx: &mut Context<'_>,
         buf: &mut [u8],
     ) -> Poll<io::Result<usize>> {
         let this: &mut dyn Read = &mut *self;
-        this.poll_read(cx, buf)
-            .map_err(|err| io::Error::new(io::ErrorKind::Interrupted, err))
+        this.poll_read(cx, buf).map_err(format_io_error)
     }
 }
 
 impl futures::AsyncSeek for dyn Read {
     fn poll_seek(
         mut self: Pin<&mut Self>,
         cx: &mut Context<'_>,
         pos: io::SeekFrom,
     ) -> Poll<io::Result<u64>> {
         let this: &mut dyn Read = &mut *self;
-        this.poll_seek(cx, pos)
-            .map_err(|err| io::Error::new(io::ErrorKind::Interrupted, err))
+        this.poll_seek(cx, pos).map_err(format_io_error)
     }
 }
 
 impl futures::Stream for dyn Read {
     type Item = Result<Bytes>;
 
     fn poll_next(mut self: Pin<&mut Self>, cx: &mut Context<'_>) -> Poll<Option<Self::Item>> {
@@ -346,30 +344,45 @@
     }
 }
 
 impl io::Read for dyn BlockingRead {
     #[inline]
     fn read(&mut self, buf: &mut [u8]) -> io::Result<usize> {
         let this: &mut dyn BlockingRead = &mut *self;
-        this.read(buf)
-            .map_err(|err| io::Error::new(io::ErrorKind::Interrupted, err))
+        this.read(buf).map_err(format_io_error)
     }
 }
 
 impl io::Seek for dyn BlockingRead {
     #[inline]
     fn seek(&mut self, pos: io::SeekFrom) -> io::Result<u64> {
         let this: &mut dyn BlockingRead = &mut *self;
-        this.seek(pos)
-            .map_err(|err| io::Error::new(io::ErrorKind::Interrupted, err))
+        this.seek(pos).map_err(format_io_error)
     }
 }
 
 impl Iterator for dyn BlockingRead {
     type Item = Result<Bytes>;
 
     #[inline]
     fn next(&mut self) -> Option<Self::Item> {
         let this: &mut dyn BlockingRead = &mut *self;
         this.next()
     }
 }
+
+/// helper functions to format `Error` into `io::Error`.
+///
+/// This function is added privately by design and only valid in current
+/// context (i.e. `oio` crate). We don't want to expose this function to
+/// users.
+#[inline]
+fn format_io_error(err: Error) -> io::Error {
+    let kind = match err.kind() {
+        ErrorKind::NotFound => io::ErrorKind::NotFound,
+        ErrorKind::PermissionDenied => io::ErrorKind::PermissionDenied,
+        ErrorKind::InvalidInput => io::ErrorKind::InvalidInput,
+        _ => io::ErrorKind::Interrupted,
+    };
+
+    io::Error::new(kind, err)
+}
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/stream.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/stream/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/page/into_flat_page.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
 use async_trait::async_trait;
 
 use crate::raw::*;
 use crate::*;
 
 /// to_flat_pager is used to make a hierarchy pager flat.
-pub fn to_flat_pager<A: Accessor, P>(acc: A, path: &str, size: usize) -> ToFlatPager<A, P> {
+pub fn into_flat_page<A: Accessor, P>(acc: A, path: &str, size: usize) -> FlatPager<A, P> {
     #[cfg(debug_assertions)]
     {
         let meta = acc.info();
         debug_assert!(
             meta.capability().list_with_delimiter_slash,
             "service doesn't support list hierarchy, it must be a bug"
         );
     }
 
-    ToFlatPager {
+    FlatPager {
         acc,
         size,
         root: path.to_string(),
         dirs: VecDeque::from([oio::Entry::new(path, Metadata::new(EntryMode::DIR))]),
         pagers: vec![],
         res: Vec::with_capacity(size),
     }
@@ -76,25 +76,25 @@
 ///
 /// There is no guarantee about the order between files and dirs at the same level.
 /// We only make sure the nested dirs will show up before parent dirs.
 ///
 /// Especially, for storage services that can't return dirs first, ToFlatPager
 /// may output parent dirs' files before nested dirs, this is expected because files
 /// always output directly while listing.
-pub struct ToFlatPager<A: Accessor, P> {
+pub struct FlatPager<A: Accessor, P> {
     acc: A,
     size: usize,
     root: String,
     dirs: VecDeque<oio::Entry>,
     pagers: Vec<(P, oio::Entry, Vec<oio::Entry>)>,
     res: Vec<oio::Entry>,
 }
 
 #[async_trait]
-impl<A, P> oio::Page for ToFlatPager<A, P>
+impl<A, P> oio::Page for FlatPager<A, P>
 where
     A: Accessor<Pager = P>,
     P: oio::Page,
 {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         loop {
             if let Some(de) = self.dirs.pop_back() {
@@ -146,15 +146,15 @@
             if self.res.len() >= self.size {
                 return Ok(Some(mem::take(&mut self.res)));
             }
         }
     }
 }
 
-impl<A, P> oio::BlockingPage for ToFlatPager<A, P>
+impl<A, P> oio::BlockingPage for FlatPager<A, P>
 where
     A: Accessor<BlockingPager = P>,
     P: oio::BlockingPage,
 {
     fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         loop {
             if let Some(de) = self.dirs.pop_back() {
@@ -295,15 +295,15 @@
     }
 
     #[test]
     fn test_blocking_list() -> Result<()> {
         let _ = tracing_subscriber::fmt().with_test_writer().try_init();
 
         let acc = MockService::new();
-        let mut pager = to_flat_pager(acc, "x/", 10);
+        let mut pager = into_flat_page(acc, "x/", 10);
 
         let mut entries = Vec::default();
 
         while let Some(e) = pager.next()? {
             entries.extend_from_slice(&e)
         }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/page/into_hierarchy_pager.rs`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
 use async_trait::async_trait;
 
 use crate::raw::*;
 use crate::*;
 
 /// to_hierarchy_pager is used to make a hierarchy pager flat.
-pub fn to_hierarchy_pager<P>(pager: P, path: &str) -> ToHierarchyPager<P> {
+pub fn into_hierarchy_page<P>(pager: P, path: &str) -> HierarchyPager<P> {
     let path = if path == "/" {
         "".to_string()
     } else {
         path.to_string()
     };
 
-    ToHierarchyPager {
+    HierarchyPager {
         pager,
         path,
         visited: HashSet::default(),
     }
 }
 
 /// ToHierarchyPager will convert a flat page to hierarchy by filter
@@ -43,21 +43,21 @@
 /// # Notes
 ///
 /// ToHierarchyPager filter entries after fetch entries. So it's possible
 /// to return an empty vec. It doesn't mean the all pages have been
 /// returned.
 ///
 /// Please keep calling next_page until we returned `Ok(None)`
-pub struct ToHierarchyPager<P> {
+pub struct HierarchyPager<P> {
     pager: P,
     path: String,
     visited: HashSet<String>,
 }
 
-impl<P> ToHierarchyPager<P> {
+impl<P> HierarchyPager<P> {
     /// TODO: use retain_mut instead after we bump MSRV to 1.61.
     fn filter_entries(&mut self, entries: Vec<oio::Entry>) -> Vec<oio::Entry> {
         entries
             .into_iter()
             .filter_map(|mut e| {
                 // If path is not started with prefix, drop it.
                 //
@@ -113,15 +113,15 @@
                 None
             })
             .collect()
     }
 }
 
 #[async_trait]
-impl<P: oio::Page> oio::Page for ToHierarchyPager<P> {
+impl<P: oio::Page> oio::Page for HierarchyPager<P> {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         let page = self.pager.next().await?;
 
         let entries = if let Some(entries) = page {
             entries
         } else {
             return Ok(None);
@@ -129,15 +129,15 @@
 
         let entries = self.filter_entries(entries);
 
         Ok(Some(entries))
     }
 }
 
-impl<P: oio::BlockingPage> oio::BlockingPage for ToHierarchyPager<P> {
+impl<P: oio::BlockingPage> oio::BlockingPage for HierarchyPager<P> {
     fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         let page = self.pager.next()?;
 
         let entries = if let Some(entries) = page {
             entries
         } else {
             return Ok(None);
@@ -197,15 +197,15 @@
     }
 
     #[test]
     fn test_blocking_list() -> Result<()> {
         let _ = tracing_subscriber::fmt().with_test_writer().try_init();
 
         let pager = MockPager::new(&["x/x/", "x/y/", "y/", "x/x/x", "y/y", "xy/", "z", "y/a"]);
-        let mut pager = to_hierarchy_pager(pager, "");
+        let mut pager = into_hierarchy_page(pager, "");
 
         let mut entries = Vec::default();
 
         let mut set = HashSet::new();
         while let Some(e) = pager.next()? {
             for i in &e {
                 debug!("got path {}", i.path());
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/write/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/ops.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/ops.rs`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 
 /// Args for `read` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpRead {
     br: BytesRange,
     if_match: Option<String>,
     if_none_match: Option<String>,
+    override_content_type: Option<String>,
     override_cache_control: Option<String>,
     override_content_disposition: Option<String>,
     version: Option<String>,
 }
 
 impl OpRead {
     /// Create a default `OpRead` which will read whole content of path.
@@ -283,14 +284,25 @@
     }
 
     /// Returns the cache-control header that should be send back by the remote read operation.
     pub fn override_cache_control(&self) -> Option<&str> {
         self.override_cache_control.as_deref()
     }
 
+    /// Sets the content-type header that should be send back by the remote read operation.
+    pub fn with_override_content_type(mut self, content_type: &str) -> Self {
+        self.override_content_type = Some(content_type.into());
+        self
+    }
+
+    /// Returns the content-type header that should be send back by the remote read operation.
+    pub fn override_content_type(&self) -> Option<&str> {
+        self.override_content_type.as_deref()
+    }
+
     /// Set the If-Match of the option
     pub fn with_if_match(mut self, if_match: &str) -> Self {
         self.if_match = Some(if_match.to_string());
         self
     }
 
     /// Get If-Match from option
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/appender.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         _ => (ErrorKind::Unexpected, false),
     };
 
     let mut message = match de::from_reader::<_, AzblobError>(bs.clone().reader()) {
         Ok(azblob_err) => format!("{azblob_err:?}"),
         Err(_) => String::from_utf8_lossy(&bs).into_owned(),
     };
+
     // If there is no body here, fill with error code.
     if message.is_empty() {
         if let Some(v) = parts.headers.get("x-ms-error-code") {
             if let Ok(code) = v.to_str() {
                 message = format!(
                     "{:?}",
                     AzblobError {
@@ -115,15 +116,17 @@
                         ..Default::default()
                     }
                 )
             }
         }
     }
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,17 @@
                         ..Default::default()
                     }
                 )
             }
         }
     }
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cacache/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/cacache/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cacache/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/cacache/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cacache/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/cacache/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/appender.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/cos/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/cos/backend.rs`

 * *Files 5% similar despite different names*

```diff
@@ -31,25 +31,31 @@
 use super::error::parse_error;
 use super::pager::CosPager;
 use super::writer::CosWriter;
 use crate::raw::*;
 use crate::services::cos::appender::CosAppender;
 use crate::*;
 
-/// Huawei Cloud COS services support.
+const DEFAULT_WRITE_MIN_SIZE: usize = 1024 * 1024;
+
+/// Tencent-Cloud COS services support.
 #[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct CosBuilder {
     root: Option<String>,
     endpoint: Option<String>,
     secret_id: Option<String>,
     secret_key: Option<String>,
     bucket: Option<String>,
     http_client: Option<HttpClient>,
 
+    /// the part size of cos multipart upload, which should be 1 MB to 5 GB.
+    /// There is no minimum size limit on the last part of your multipart upload
+    write_min_size: Option<usize>,
+
     disable_config_load: bool,
 }
 
 impl Debug for CosBuilder {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Builder")
             .field("root", &self.root)
@@ -116,14 +122,22 @@
         if !bucket.is_empty() {
             self.bucket = Some(bucket.to_string());
         }
 
         self
     }
 
+    /// set the minimum size of unsized write, it should be greater than 1 MB.
+    /// Reference: [Upload Part | Tencent Cloud](https://www.tencentcloud.com/document/product/436/7750)
+    pub fn write_min_size(&mut self, write_min_size: usize) -> &mut Self {
+        self.write_min_size = Some(write_min_size);
+
+        self
+    }
+
     /// Disable config load so that opendal will not load config from
     /// environment.
     ///
     /// For examples:
     ///
     /// - envs like `TENCENTCLOUD_SECRET_ID`
     pub fn disable_config_load(&mut self) -> &mut Self {
@@ -151,14 +165,16 @@
         let mut builder = CosBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("secret_id").map(|v| builder.secret_id(v));
         map.get("secret_key").map(|v| builder.secret_key(v));
+        map.get("write_min_size")
+            .map(|v| builder.write_min_size(v.parse().expect("input must be a number")));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", &self);
 
@@ -214,40 +230,49 @@
         if let Some(v) = self.secret_key.take() {
             cfg.secret_key = Some(v);
         }
 
         let cred_loader = TencentCosCredentialLoader::new(client.client(), cfg);
 
         let signer = TencentCosSigner::new();
+        let write_min_size = self.write_min_size.unwrap_or(DEFAULT_WRITE_MIN_SIZE);
+        if write_min_size < 1024 * 1024 {
+            return Err(Error::new(
+                ErrorKind::ConfigInvalid,
+                "The write minimum buffer size is misconfigured",
+            )
+            .with_context("service", Scheme::Cos));
+        }
 
         debug!("backend build finished");
         Ok(CosBackend {
             core: Arc::new(CosCore {
                 bucket: bucket.clone(),
                 root,
                 endpoint: format!("{}://{}.{}", &scheme, &bucket, &endpoint),
                 signer,
                 loader: cred_loader,
                 client,
+                write_min_size,
             }),
         })
     }
 }
 
-/// Backend for Huaweicloud COS services.
+/// Backend for Tencent-Cloud COS services.
 #[derive(Debug, Clone)]
 pub struct CosBackend {
     core: Arc<CosCore>,
 }
 
 #[async_trait]
 impl Accessor for CosBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
-    type Writer = CosWriter;
+    type Writer = oio::MultipartUploadWriter<CosWriter>;
     type BlockingWriter = ();
     type Appender = CosAppender;
     type Pager = CosPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
@@ -265,14 +290,16 @@
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
                 write_can_sink: true,
                 write_with_content_type: true,
                 write_with_cache_control: true,
+                write_with_content_disposition: true,
+                write_without_content_length: true,
 
                 append: true,
                 append_with_cache_control: true,
                 append_with_content_disposition: true,
                 append_with_content_type: true,
 
                 delete: true,
@@ -293,15 +320,15 @@
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
         let mut req =
             self.core
-                .cos_put_object_request(path, Some(0), None, None, AsyncBody::Empty)?;
+                .cos_put_object_request(path, Some(0), None, None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
@@ -328,24 +355,17 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.content_length().is_none() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "write without content length is not supported",
-            ));
-        }
-
         Ok((
             RpWrite::default(),
-            CosWriter::new(self.core.clone(), args, path.to_string()),
+            CosWriter::new(self.core.clone(), path, args),
         ))
     }
 
     async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
         Ok((
             RpAppend::default(),
             CosAppender::new(self.core.clone(), path, args),
@@ -414,14 +434,15 @@
                 v.if_match(),
                 v.if_none_match(),
             )?,
             PresignOperation::Write(v) => self.core.cos_put_object_request(
                 path,
                 None,
                 v.content_type(),
+                v.content_disposition(),
                 v.cache_control(),
                 AsyncBody::Empty,
             )?,
         };
         self.core.sign_query(&mut req, args.expire()).await?;
 
         // We don't need this request anymore, consume it directly.
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/supabase/core.rs`

 * *Files 27% similar despite different names*

```diff
@@ -12,316 +12,259 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
-use std::fmt::Formatter;
-use std::time::Duration;
 
-use http::header::CACHE_CONTROL;
-use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
-use http::header::IF_MATCH;
-use http::header::IF_NONE_MATCH;
+use http::HeaderValue;
 use http::Request;
 use http::Response;
-use reqsign::TencentCosCredential;
-use reqsign::TencentCosCredentialLoader;
-use reqsign::TencentCosSigner;
 
 use crate::raw::*;
 use crate::*;
 
-pub struct CosCore {
-    pub bucket: String,
+pub struct SupabaseCore {
     pub root: String,
+    pub bucket: String,
     pub endpoint: String,
 
-    pub signer: TencentCosSigner,
-    pub loader: TencentCosCredentialLoader,
-    pub client: HttpClient,
+    /// The key used for authorization
+    /// If loaded, the read operation will always access the nonpublic resources.
+    /// If you want to read the public resources, please do not set the key.
+    pub key: Option<String>,
+
+    pub http_client: HttpClient,
 }
 
-impl Debug for CosCore {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("Backend")
+impl Debug for SupabaseCore {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        f.debug_struct("SupabaseCore")
             .field("root", &self.root)
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .finish_non_exhaustive()
     }
 }
 
-impl CosCore {
-    async fn load_credential(&self) -> Result<Option<TencentCosCredential>> {
-        let cred = self
-            .loader
-            .load()
-            .await
-            .map_err(new_request_credential_error)?;
-
-        if let Some(cred) = cred {
-            Ok(Some(cred))
-        } else {
-            Ok(None)
+impl SupabaseCore {
+    pub fn new(
+        root: &str,
+        bucket: &str,
+        endpoint: &str,
+        key: Option<String>,
+        client: HttpClient,
+    ) -> Self {
+        Self {
+            root: root.to_string(),
+            bucket: bucket.to_string(),
+            endpoint: endpoint.to_string(),
+            key,
+            http_client: client,
         }
     }
 
-    pub async fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
-        let cred = if let Some(cred) = self.load_credential().await? {
-            cred
-        } else {
-            return Ok(());
-        };
-
-        self.signer.sign(req, &cred).map_err(new_request_sign_error)
-    }
-
-    pub async fn sign_query<T>(&self, req: &mut Request<T>, duration: Duration) -> Result<()> {
-        let cred = if let Some(cred) = self.load_credential().await? {
-            cred
-        } else {
-            return Ok(());
-        };
-
-        self.signer
-            .sign_query(req, duration, &cred)
-            .map_err(new_request_sign_error)
-    }
-
-    #[inline]
-    pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
-        self.client.send(req).await
-    }
-}
-
-impl CosCore {
-    pub async fn cos_get_object(
-        &self,
-        path: &str,
-        range: BytesRange,
-        if_match: Option<&str>,
-        if_none_match: Option<&str>,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.cos_get_object_request(path, range, if_match, if_none_match)?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
-
-    pub fn cos_get_object_request(
-        &self,
-        path: &str,
-        range: BytesRange,
-        if_match: Option<&str>,
-        if_none_match: Option<&str>,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::get(&url);
-
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
-        }
-
-        if !range.is_full() {
-            req = req.header(http::header::RANGE, range.to_header())
-        }
-
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
+    /// Add authorization header to the request if the key is set. Otherwise leave
+    /// the request as-is.
+    pub fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
+        if let Some(k) = &self.key {
+            let v = HeaderValue::from_str(&format!("Bearer {}", k)).unwrap();
+            req.headers_mut().insert(http::header::AUTHORIZATION, v);
         }
-
-        let req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        Ok(req)
+        Ok(())
     }
+}
 
-    pub fn cos_put_object_request(
+// requests
+impl SupabaseCore {
+    pub fn supabase_upload_object_request(
         &self,
         path: &str,
-        size: Option<u64>,
+        size: Option<usize>,
         content_type: Option<&str>,
-        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/storage/v1/object/{}/{}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
+        );
 
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::put(&url);
+        let mut req = Request::post(&url);
 
         if let Some(size) = size {
             req = req.header(CONTENT_LENGTH, size)
         }
-        if let Some(cache_control) = cache_control {
-            req = req.header(CACHE_CONTROL, cache_control)
-        }
 
         if let Some(mime) = content_type {
             req = req.header(CONTENT_TYPE, mime)
         }
 
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn cos_head_object(
+    pub fn supabase_delete_object_request(&self, path: &str) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/storage/v1/object/{}/{}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
+        );
+
+        Request::delete(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)
+    }
+
+    pub fn supabase_get_object_public_request(
         &self,
         path: &str,
-        if_match: Option<&str>,
-        if_none_match: Option<&str>,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.cos_head_object_request(path, if_match, if_none_match)?;
+        _: BytesRange,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/storage/v1/object/public/{}/{}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
+        );
 
-        self.sign(&mut req).await?;
+        let req = Request::get(&url);
 
-        self.send(req).await
+        req.body(AsyncBody::Empty).map_err(new_request_build_error)
     }
 
-    pub fn cos_head_object_request(
+    pub fn supabase_get_object_auth_request(
         &self,
         path: &str,
-        if_match: Option<&str>,
-        if_none_match: Option<&str>,
+        _: BytesRange,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/storage/v1/object/authenticated/{}/{}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
+        );
 
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::head(&url);
+        let req = Request::get(&url);
 
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
-        }
+        req.body(AsyncBody::Empty).map_err(new_request_build_error)
+    }
 
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
-        }
+    pub fn supabase_head_object_public_request(&self, path: &str) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/storage/v1/object/public/{}/{}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
+        );
 
-        let req = req
+        Request::head(&url)
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        Ok(req)
+            .map_err(new_request_build_error)
     }
 
-    pub async fn cos_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub fn supabase_head_object_auth_request(&self, path: &str) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/storage/v1/object/authenticated/{}/{}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
+        );
 
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let req = Request::delete(&url);
-
-        let mut req = req
+        Request::head(&url)
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
+            .map_err(new_request_build_error)
     }
 
-    pub fn cos_append_object_request(
+    pub fn supabase_get_object_info_public_request(
         &self,
         path: &str,
-        position: u64,
-        size: usize,
-        args: &OpAppend,
-        body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let url = format!(
-            "{}/{}?append&position={}",
+            "{}/storage/v1/object/info/public/{}/{}",
             self.endpoint,
-            percent_encode_path(&p),
-            position
+            self.bucket,
+            percent_encode_path(&p)
         );
 
-        let mut req = Request::post(&url);
-
-        req = req.header(CONTENT_LENGTH, size);
-
-        if let Some(mime) = args.content_type() {
-            req = req.header(CONTENT_TYPE, mime);
-        }
+        Request::get(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)
+    }
 
-        if let Some(pos) = args.content_disposition() {
-            req = req.header(CONTENT_DISPOSITION, pos);
-        }
+    pub fn supabase_get_object_info_auth_request(&self, path: &str) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/storage/v1/object/info/authenticated/{}/{}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
+        );
 
-        if let Some(cache_control) = args.cache_control() {
-            req = req.header(CACHE_CONTROL, cache_control)
-        }
+        Request::get(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)
+    }
+}
 
-        let req = req.body(body).map_err(new_request_build_error)?;
-        Ok(req)
+// core utils
+impl SupabaseCore {
+    pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
+        self.http_client.send(req).await
     }
 
-    pub async fn cos_copy_object(
+    pub async fn supabase_get_object(
         &self,
-        from: &str,
-        to: &str,
+        path: &str,
+        range: BytesRange,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let source = build_abs_path(&self.root, from);
-        let target = build_abs_path(&self.root, to);
-
-        let source = format!("/{}/{}", self.bucket, percent_encode_path(&source));
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&target));
-
-        let mut req = Request::put(&url)
-            .header("x-cos-copy-source", percent_encode_path(&source))
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
+        let mut req = if self.key.is_some() {
+            self.supabase_get_object_auth_request(path, range)?
+        } else {
+            self.supabase_get_object_public_request(path, range)?
+        };
+        self.sign(&mut req)?;
+        self.send(req).await
+    }
 
+    pub async fn supabase_head_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = if self.key.is_some() {
+            self.supabase_head_object_auth_request(path)?
+        } else {
+            self.supabase_head_object_public_request(path)?
+        };
+        self.sign(&mut req)?;
         self.send(req).await
     }
 
-    pub async fn cos_list_objects(
+    pub async fn supabase_get_object_info(
         &self,
         path: &str,
-        next_marker: &str,
-        delimiter: &str,
-        limit: Option<usize>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let mut queries = vec![];
-        if !path.is_empty() {
-            queries.push(format!("prefix={}", percent_encode_path(&p)));
-        }
-        if !delimiter.is_empty() {
-            queries.push(format!("delimiter={delimiter}"));
-        }
-        if let Some(limit) = limit {
-            queries.push(format!("max-keys={limit}"));
-        }
-        if !next_marker.is_empty() {
-            queries.push(format!("marker={next_marker}"));
-        }
-
-        let url = if queries.is_empty() {
-            self.endpoint.to_string()
+        let mut req = if self.key.is_some() {
+            self.supabase_get_object_info_auth_request(path)?
         } else {
-            format!("{}?{}", self.endpoint, queries.join("&"))
+            self.supabase_get_object_info_public_request(path)?
         };
+        self.sign(&mut req)?;
+        self.send(req).await
+    }
 
-        let mut req = Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-
+    pub async fn supabase_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.supabase_delete_object_request(path)?;
+        self.sign(&mut req)?;
         self.send(req).await
     }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/cos/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/cos/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -59,20 +59,21 @@
     };
 
     let message = match de::from_reader::<_, CosError>(bs.clone().reader()) {
         Ok(cos_error) => format!("{cos_error:?}"),
         Err(_) => String::from_utf8_lossy(&bs).into_owned(),
     };
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
-
     Ok(err)
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/cos/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/cos/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/cos/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 9% similar despite different names*

```diff
@@ -11,64 +11,61 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::CosCore;
+use super::backend::WebdavBackend;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct CosWriter {
-    core: Arc<CosCore>,
+pub struct WebdavWriter {
+    backend: WebdavBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl CosWriter {
-    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
-        CosWriter { core, op, path }
+impl WebdavWriter {
+    pub fn new(backend: WebdavBackend, op: OpWrite, path: String) -> Self {
+        WebdavWriter { backend, op, path }
     }
 
-    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
-        let mut req = self.core.cos_put_object_request(
-            &self.path,
-            Some(size),
-            self.op.content_type(),
-            self.op.cache_control(),
-            body,
-        )?;
-
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
+    async fn write_oneshot(&mut self, size: u64, body: AsyncBody) -> Result<()> {
+        let resp = self
+            .backend
+            .webdav_put(
+                &self.path,
+                Some(size),
+                self.op.content_type(),
+                self.op.content_disposition(),
+                body,
+            )
+            .await?;
 
         let status = resp.status();
 
         match status {
-            StatusCode::CREATED | StatusCode::OK => {
+            StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 }
 
 #[async_trait]
-impl oio::Write for CosWriter {
+impl oio::Write for WebdavWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
             .await
     }
 
     async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
         self.write_oneshot(size, AsyncBody::Stream(s)).await
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/builder.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/error.rs`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use http::Response;
 use http::StatusCode;
-use http::Uri;
 use serde::Deserialize;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
@@ -51,24 +50,22 @@
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
     if let Some(dropbox_err) = dropbox_err {
         (kind, retryable) =
             parse_dropbox_error_summary(&dropbox_err.error_summary).unwrap_or((kind, retryable));
     }
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
-    if let Some(uri) = parts.extensions.get::<Uri>() {
-        err = err.with_context("uri", uri.to_string());
-    }
-
     Ok(err)
 }
 
 /// We cannot get the error type from the response header when the status code is 409.
 /// Because Dropbox API v2 will put error summary in the response body,
 /// we need to parse it to get the correct error type and then error kind.
 ///
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/dropbox/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/fs/appender.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/fs/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,16 @@
 
         Ok(p)
     }
 }
 
 #[async_trait]
 impl Accessor for FsBackend {
-    type Reader = oio::into_reader::FdReader<Compat<tokio::fs::File>>;
-    type BlockingReader = oio::into_blocking_reader::FdReader<std::fs::File>;
+    type Reader = oio::FromFileReader<Compat<tokio::fs::File>>;
+    type BlockingReader = oio::FromFileReader<std::fs::File>;
     type Writer = FsWriter<tokio::fs::File>;
     type BlockingWriter = FsWriter<std::fs::File>;
     type Appender = FsAppender<tokio::fs::File>;
     type Pager = Option<FsPager<tokio::fs::ReadDir>>;
     type BlockingPager = Option<FsPager<std::fs::ReadDir>>;
 
     fn info(&self) -> AccessorInfo {
@@ -354,15 +354,15 @@
                 },
                 total_length,
             ),
             // Read the whole file.
             (None, None) => (0, total_length),
         };
 
-        let mut r = oio::into_reader::from_fd(f, start, end);
+        let mut r = oio::into_read_from_file(f, start, end);
 
         // Rewind to make sure we are on the correct offset.
         r.seek(SeekFrom::Start(0)).await?;
 
         Ok((RpRead::new(end - start), r))
     }
 
@@ -554,15 +554,15 @@
                 },
                 total_length,
             ),
             // Read the whole file.
             (None, None) => (0, total_length),
         };
 
-        let mut r = oio::into_blocking_reader::from_fd(f, start, end);
+        let mut r: oio::FromFileReader<std::fs::File> = oio::into_read_from_file(f, start, end);
 
         // Rewind to make sure we are on the correct offset.
         r.seek(SeekFrom::Start(0))?;
 
         Ok((RpRead::new(end - start), r))
     }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/fs/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/fs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/ftp/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files 26% similar despite different names*

```diff
@@ -11,113 +11,137 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::io;
-use std::pin::Pin;
-use std::task::ready;
-use std::task::Context;
-use std::task::Poll;
-
-use bb8::PooledConnection;
-use futures::future::BoxFuture;
-use futures::AsyncRead;
-use futures::FutureExt;
-use suppaftp::Status;
+use std::collections::HashMap;
+use std::fmt::Debug;
+use std::fmt::Formatter;
+use std::sync::Arc;
 
-use super::backend::Manager;
-use crate::raw::*;
+use async_trait::async_trait;
+use rocksdb::DB;
+
+use crate::raw::adapters::kv;
+use crate::Result;
 use crate::*;
 
-/// Wrapper for ftp data stream and command stream.
-pub struct FtpReader {
-    reader: Box<dyn AsyncRead + Send + Unpin>,
-    state: State,
-}
-
-unsafe impl Sync for FtpReader {}
-
-pub enum State {
-    Reading(Option<PooledConnection<'static, Manager>>),
-    Finalize(BoxFuture<'static, Result<()>>),
-}
-
-impl FtpReader {
-    /// Create an instance of FtpReader.
-    pub fn new(
-        r: Box<dyn AsyncRead + Send + Unpin>,
-        c: PooledConnection<'static, Manager>,
-    ) -> Self {
-        Self {
-            reader: r,
-            state: State::Reading(Some(c)),
+/// RocksDB service support.
+#[doc = include_str!("docs.md")]
+#[derive(Clone, Default, Debug)]
+pub struct RocksdbBuilder {
+    /// The path to the rocksdb data directory.
+    datadir: Option<String>,
+    /// the working directory of the service. Can be "/path/to/dir"
+    ///
+    /// default is "/"
+    root: Option<String>,
+}
+
+impl RocksdbBuilder {
+    /// Set the path to the rocksdb data directory. Will create if not exists.
+    pub fn datadir(&mut self, path: &str) -> &mut Self {
+        self.datadir = Some(path.into());
+        self
+    }
+
+    /// set the working directory, all operations will be performed under it.
+    ///
+    /// default: "/"
+    pub fn root(&mut self, root: &str) -> &mut Self {
+        if !root.is_empty() {
+            self.root = Some(root.to_owned());
         }
+        self
     }
 }
 
-impl oio::Read for FtpReader {
-    fn poll_read(&mut self, cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
-        let data = Pin::new(&mut self.reader).poll_read(cx, buf);
-
-        match &mut self.state {
-            // Reading state, try to poll some data.
-            State::Reading(stream) => {
-                match stream {
-                    Some(_) => {
-                        // when hit Err or EOF, consume ftpstream, change state to Finalize and send fut.
-                        if let Poll::Ready(Err(_)) | Poll::Ready(Ok(0)) = data {
-                            let mut ft = stream.take().unwrap();
-
-                            let fut = async move {
-                                ft.read_response_in(&[
-                                    Status::ClosingDataConnection,
-                                    Status::RequestedFileActionOk,
-                                ])
-                                .await?;
-
-                                Ok(())
-                            };
-                            self.state = State::Finalize(Box::pin(fut));
-                        } else {
-                            // Otherwise, exit and return data.
-                            return data.map_err(|err| {
-                                Error::new(ErrorKind::Unexpected, "read data from ftp data stream")
-                                    .set_source(err)
-                            });
-                        }
-
-                        self.poll_read(cx, buf)
-                    }
-                    // We could never reach this branch because we will change to Finalize state once we consume ftp stream.
-                    None => unreachable!(),
-                }
-            }
-
-            // Finalize state, wait for finalization of stream.
-            State::Finalize(fut) => match ready!(Pin::new(fut).poll_unpin(cx)) {
-                Ok(_) => Poll::Ready(Ok(0)),
-                Err(e) => Poll::Ready(Err(e)),
+impl Builder for RocksdbBuilder {
+    const SCHEME: Scheme = Scheme::Rocksdb;
+    type Accessor = RocksdbBackend;
+
+    fn from_map(map: HashMap<String, String>) -> Self {
+        let mut builder = RocksdbBuilder::default();
+
+        map.get("datadir").map(|v| builder.datadir(v));
+
+        builder
+    }
+
+    fn build(&mut self) -> Result<Self::Accessor> {
+        let path = self.datadir.take().ok_or_else(|| {
+            Error::new(ErrorKind::ConfigInvalid, "datadir is required but not set")
+                .with_context("service", Scheme::Rocksdb)
+        })?;
+        let db = DB::open_default(&path).map_err(|e| {
+            Error::new(ErrorKind::ConfigInvalid, "open default transaction db")
+                .with_context("service", Scheme::Rocksdb)
+                .with_context("datadir", path)
+                .set_source(e)
+        })?;
+
+        Ok(RocksdbBackend::new(Adapter { db: Arc::new(db) }))
+    }
+}
+
+/// Backend for rocksdb services.
+pub type RocksdbBackend = kv::Backend<Adapter>;
+
+#[derive(Clone)]
+pub struct Adapter {
+    db: Arc<DB>,
+}
+
+impl Debug for Adapter {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        let mut ds = f.debug_struct("Adapter");
+        ds.field("path", &self.db.path());
+        ds.finish()
+    }
+}
+
+#[async_trait]
+impl kv::Adapter for Adapter {
+    fn metadata(&self) -> kv::Metadata {
+        kv::Metadata::new(
+            Scheme::Rocksdb,
+            &self.db.path().to_string_lossy(),
+            Capability {
+                read: true,
+                write: true,
+                ..Default::default()
             },
-        }
+        )
+    }
+
+    async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
+        self.blocking_get(path)
+    }
+
+    fn blocking_get(&self, path: &str) -> Result<Option<Vec<u8>>> {
+        Ok(self.db.get(path)?)
     }
 
-    fn poll_seek(&mut self, cx: &mut Context<'_>, pos: io::SeekFrom) -> Poll<Result<u64>> {
-        let (_, _) = (cx, pos);
+    async fn set(&self, path: &str, value: &[u8]) -> Result<()> {
+        self.blocking_set(path, value)
+    }
+
+    fn blocking_set(&self, path: &str, value: &[u8]) -> Result<()> {
+        Ok(self.db.put(path, value)?)
+    }
+
+    async fn delete(&self, path: &str) -> Result<()> {
+        self.blocking_delete(path)
+    }
+
+    fn blocking_delete(&self, path: &str) -> Result<()> {
+        Ok(self.db.delete(path)?)
+    }
+}
 
-        Poll::Ready(Err(Error::new(
-            ErrorKind::Unsupported,
-            "output reader doesn't support seeking",
-        )))
-    }
-
-    fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<bytes::Bytes>>> {
-        let _ = cx;
-
-        Poll::Ready(Some(Err(Error::new(
-            ErrorKind::Unsupported,
-            "output reader doesn't support seeking",
-        ))))
+impl From<rocksdb::Error> for Error {
+    fn from(e: rocksdb::Error) -> Self {
+        Error::new(ErrorKind::Unexpected, "got rocksdb error").set_source(e)
     }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,17 @@
     };
 
     let message = match de::from_slice::<GcsErrorResponse>(&bs) {
         Ok(gcs_err) => format!("{gcs_err:?}"),
         Err(_) => String::from_utf8_lossy(&bs).into_owned(),
     };
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/builder.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/http/error.rs`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,29 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-        .with_context("response", format!("{parts:?}"));
+    let message = String::from_utf8_lossy(&bs);
+
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,19 @@
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
     let bs = body.bytes().await?;
-    let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-        .with_context("response", format!("{parts:?}"));
+    let message = String::from_utf8_lossy(&bs);
+
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::GhacBuilder as Ghac;
+pub use backend::IpfsBuilder as Ipfs;
 
 mod error;
-mod writer;
+mod ipld;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 10% similar despite different names*

```diff
@@ -22,26 +22,29 @@
 use std::io::SeekFrom;
 use std::path::PathBuf;
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use log::debug;
 
+use super::appender::HdfsAppender;
 use super::error::parse_io_error;
 use super::pager::HdfsPager;
 use super::writer::HdfsWriter;
 use crate::raw::*;
 use crate::*;
 
 /// [Hadoop Distributed File System (HDFS™)](https://hadoop.apache.org/) support.
 #[doc = include_str!("docs.md")]
 #[derive(Debug, Default)]
 pub struct HdfsBuilder {
     root: Option<String>,
     name_node: Option<String>,
+    kerberos_ticket_cache_path: Option<String>,
+    user: Option<String>,
 }
 
 impl HdfsBuilder {
     /// Set root of this backend.
     ///
     /// All operations will happen under this root.
     pub fn root(&mut self, root: &str) -> &mut Self {
@@ -64,25 +67,46 @@
         if !name_node.is_empty() {
             // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
             self.name_node = Some(name_node.trim_end_matches('/').to_string())
         }
 
         self
     }
+
+    /// Set kerberos_ticket_cache_path of this backend
+    ///
+    /// This should be configured when kerberos is enabled.
+    pub fn kerberos_ticket_cache_path(&mut self, kerberos_ticket_cache_path: &str) -> &mut Self {
+        if !kerberos_ticket_cache_path.is_empty() {
+            self.kerberos_ticket_cache_path = Some(kerberos_ticket_cache_path.to_string())
+        }
+        self
+    }
+
+    /// Set user of this backend
+    pub fn user(&mut self, user: &str) -> &mut Self {
+        if !user.is_empty() {
+            self.user = Some(user.to_string())
+        }
+        self
+    }
 }
 
 impl Builder for HdfsBuilder {
     const SCHEME: Scheme = Scheme::Hdfs;
     type Accessor = HdfsBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
         let mut builder = HdfsBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("name_node").map(|v| builder.name_node(v));
+        map.get("kerberos_ticket_cache_path")
+            .map(|v| builder.kerberos_ticket_cache_path(v));
+        map.get("user").map(|v| builder.user(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", &self);
 
@@ -93,15 +117,23 @@
                     .with_context("service", Scheme::Hdfs))
             }
         };
 
         let root = normalize_root(&self.root.take().unwrap_or_default());
         debug!("backend use root {}", root);
 
-        let client = hdrs::Client::connect(name_node).map_err(parse_io_error)?;
+        let mut builder = hdrs::ClientBuilder::new(name_node);
+        if let Some(ticket_cache_path) = &self.kerberos_ticket_cache_path {
+            builder = builder.with_kerberos_ticket_cache_path(ticket_cache_path.as_str());
+        }
+        if let Some(user) = &self.user {
+            builder = builder.with_user(user.as_str());
+        }
+
+        let client = builder.connect().map_err(parse_io_error)?;
 
         // Create root dir if not exist.
         if let Err(e) = client.metadata(&root) {
             if e.kind() == io::ErrorKind::NotFound {
                 debug!("root {} is not exist, creating now", root);
 
                 client.create_dir(&root).map_err(parse_io_error)?
@@ -125,19 +157,19 @@
 
 /// hdrs::Client is thread-safe.
 unsafe impl Send for HdfsBackend {}
 unsafe impl Sync for HdfsBackend {}
 
 #[async_trait]
 impl Accessor for HdfsBackend {
-    type Reader = oio::into_reader::FdReader<hdrs::AsyncFile>;
-    type BlockingReader = oio::into_blocking_reader::FdReader<hdrs::File>;
+    type Reader = oio::FromFileReader<hdrs::AsyncFile>;
+    type BlockingReader = oio::FromFileReader<hdrs::File>;
     type Writer = HdfsWriter<hdrs::AsyncFile>;
     type BlockingWriter = HdfsWriter<hdrs::File>;
-    type Appender = ();
+    type Appender = HdfsAppender<hdrs::AsyncFile>;
     type Pager = Option<HdfsPager>;
     type BlockingPager = Option<HdfsPager>;
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Hdfs)
             .set_root(&self.root)
@@ -195,21 +227,50 @@
             (Some(offset), None) => (offset, meta.len()),
             // Read the last size bytes.
             (None, Some(size)) => (meta.len() - size, meta.len()),
             // Read the whole file.
             (None, None) => (0, meta.len()),
         };
 
-        let mut r = oio::into_reader::from_fd(f, start, end);
+        let mut r = oio::into_read_from_file(f, start, end);
         // Rewind to make sure we are on the correct offset.
         r.seek(SeekFrom::Start(0)).await?;
 
         Ok((RpRead::new(end - start), r))
     }
 
+    async fn append(&self, path: &str, _: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        let p = build_rooted_abs_path(&self.root, path);
+
+        let parent = PathBuf::from(&p)
+            .parent()
+            .ok_or_else(|| {
+                Error::new(
+                    ErrorKind::Unexpected,
+                    "path should have parent but not, it must be malformed",
+                )
+                .with_context("input", &p)
+            })?
+            .to_path_buf();
+        self.client
+            .create_dir(&parent.to_string_lossy())
+            .map_err(parse_io_error)?;
+
+        let f = self
+            .client
+            .open_file()
+            .create(true)
+            .append(true)
+            .async_open(&p)
+            .await
+            .map_err(parse_io_error)?;
+
+        Ok((RpAppend::new(), HdfsAppender::new(f)))
+    }
+
     async fn write(&self, path: &str, _: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let parent = PathBuf::from(&p)
             .parent()
             .ok_or_else(|| {
                 Error::new(
@@ -332,15 +393,15 @@
             (Some(offset), None) => (offset, meta.len()),
             // Read the last size bytes.
             (None, Some(size)) => (meta.len() - size, meta.len()),
             // Read the whole file.
             (None, None) => (0, meta.len()),
         };
 
-        let mut r = oio::into_blocking_reader::from_fd(f, start, end);
+        let mut r = oio::into_read_from_file(f, start, end);
         // Rewind to make sure we are on the correct offset.
         r.seek(SeekFrom::Start(0))?;
 
         Ok((RpRead::new(end - start), r))
     }
 
     fn blocking_write(&self, path: &str, _: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/docs.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 - [x] delete
 - [ ] copy
 - [ ] rename
 - [x] list
 - [ ] ~~scan~~
 - [ ] ~~presign~~
 - [x] blocking
+- [x] append
 
 ## Differences with webhdfs
 
 [Webhdfs][crate::services::Webhdfs] is powered by hdfs's RESTful HTTP API.
 
 ## Features
 
 HDFS support needs to enable feature `services-hdfs`.
 
 ## Configuration
 
 - `root`: Set the work dir for backend.
 - `name_node`: Set the name node for backend.
+- `kerberos_ticket_cache_path`: Set the kerberos ticket cache path for backend, this should be gotten by `klist` after `kinit`
+- `user`: Set the user for backend
 
 Refer to [`HdfsBuilder`]'s public API docs for more information.
 
 ## Environment
 
 HDFS needs some environment set correctly.
 
@@ -71,15 +74,15 @@
 1. Obtain the entire HDFS config folder (usually located at HADOOP_HOME/etc/hadoop).
 2. Set the environment variable HADOOP_CONF_DIR to the path of this folder.
 ```shell
 export HADOOP_CONF_DIR=<path of the config folder>
 ```
 3. Append the HADOOP_CONF_DIR to the `CLASSPATH`
 ```shell
-export CLASSPATH=$CLASSPATH:$HADOOP_CONF_DIR
+export CLASSPATH=$HADOOP_CONF_DIR:$HADOOP_CLASSPATH:$CLASSPATH
 ```
 4. Use the `cluster_name` specified in the `core-site.xml` file (located in the HADOOP_CONF_DIR folder) to replace namenode:port.
 
 ```rust
 builder.name_node("hdfs://cluster_name");
 ```
 ## Example
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::HdfsBuilder as Hdfs;
+pub use backend::WasabiBuilder as Wasabi;
 
+mod core;
 mod error;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -27,26 +27,28 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
-            (ErrorKind::ConditionNotMatch, false)
-        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
-        | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
+        | StatusCode::GATEWAY_TIMEOUT
+        // IPFS Gateway will return `408 REQUEST_TIMEOUT` while `ipfs resolve -r` failed.
+        | StatusCode::REQUEST_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-        .with_context("response", format!("{parts:?}"));
+    let message = String::from_utf8_lossy(&bs);
+
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files 17% similar despite different names*

```diff
@@ -26,26 +26,30 @@
 /// Parse error response into Error.
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
-        StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        // Some services (like owncloud) return 403 while file locked.
+        StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, true),
+        // Allowing retry for resource locked.
+        StatusCode::LOCKED => (ErrorKind::Unexpected, true),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
-        | StatusCode::GATEWAY_TIMEOUT
-        // IPFS Gateway will return `408 REQUEST_TIMEOUT` while `ipfs resolve -r` failed.
-        | StatusCode::REQUEST_TIMEOUT => (ErrorKind::Unexpected, true),
+        | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-        .with_context("response", format!("{parts:?}"));
+    let message = String::from_utf8_lossy(&bs);
+
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,11 +12,10 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::IpfsBuilder as Ipfs;
+pub use backend::MemcachedBuilder as Memcached;
 
-mod error;
-mod ipld;
+mod ascii;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,17 @@
     };
 
     let message = match ipfs_error {
         Some(ipfs_error) => format!("{ipfs_error:?}"),
         None => String::from_utf8_lossy(&bs).into_owned(),
     };
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -12,10 +12,8 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::MemcachedBuilder as Memcached;
-
-mod ascii;
+pub use backend::MemoryBuilder as Memory;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::MemoryBuilder as Memory;
+pub use backend::RocksdbBuilder as Rocksdb;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/mini_moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/mini_moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 pub use cos::Cos;
 
 #[cfg(feature = "services-dashmap")]
 mod dashmap;
 #[cfg(feature = "services-dashmap")]
 pub use self::dashmap::Dashmap;
 
+#[cfg(feature = "services-etcd")]
+mod etcd;
+#[cfg(feature = "services-etcd")]
+pub use self::etcd::Etcd;
+
 #[cfg(feature = "services-fs")]
 mod fs;
 #[cfg(feature = "services-fs")]
 pub use fs::Fs;
 
 #[cfg(feature = "services-ftp")]
 mod ftp;
@@ -110,14 +115,19 @@
 pub use oss::Oss;
 
 #[cfg(feature = "services-cacache")]
 mod cacache;
 #[cfg(feature = "services-cacache")]
 pub use self::cacache::Cacache;
 
+#[cfg(feature = "services-persy")]
+mod persy;
+#[cfg(feature = "services-persy")]
+pub use self::persy::Persy;
+
 #[cfg(feature = "services-redis")]
 mod redis;
 #[cfg(feature = "services-redis")]
 pub use self::redis::Redis;
 
 #[cfg(feature = "services-rocksdb")]
 mod rocksdb;
@@ -179,7 +189,12 @@
 #[cfg(feature = "services-vercel-artifacts")]
 pub use vercel_artifacts::VercelArtifacts;
 
 #[cfg(feature = "services-redb")]
 mod redb;
 #[cfg(feature = "services-redb")]
 pub use self::redb::Redb;
+
+#[cfg(feature = "services-tikv")]
+mod tikv;
+#[cfg(feature = "services-tikv")]
+pub use self::tikv::Tikv;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/obs/appender.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/obs/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -88,22 +88,29 @@
 ///     builder.secret_access_key("secret_access_key");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
 ///
 ///     Ok(())
 /// }
 /// ```
+
+const DEFAULT_WRITE_MIN_SIZE: usize = 100 * 1024;
+
+/// Huawei-Cloud Object Storage Service (OBS) support
 #[derive(Default, Clone)]
 pub struct ObsBuilder {
     root: Option<String>,
     endpoint: Option<String>,
     access_key_id: Option<String>,
     secret_access_key: Option<String>,
     bucket: Option<String>,
     http_client: Option<HttpClient>,
+    /// the part size of obs multipart upload, which should be 100 KiB to 5 GiB.
+    /// There is no minimum size limit on the last part of your multipart upload
+    write_min_size: Option<usize>,
 }
 
 impl Debug for ObsBuilder {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Builder")
             .field("root", &self.root)
             .field("endpoint", &self.endpoint)
@@ -180,14 +187,22 @@
     ///
     /// This API is part of OpenDAL's Raw API. `HttpClient` could be changed
     /// during minor updates.
     pub fn http_client(&mut self, client: HttpClient) -> &mut Self {
         self.http_client = Some(client);
         self
     }
+
+    /// set the minimum size of unsized write, it should be greater than 100 KB.
+    /// Reference: [Huawei Obs multipart upload limits](https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0099.html)
+    pub fn write_min_size(&mut self, write_min_size: usize) -> &mut Self {
+        self.write_min_size = Some(write_min_size);
+
+        self
+    }
 }
 
 impl Builder for ObsBuilder {
     const SCHEME: Scheme = Scheme::Obs;
     type Accessor = ObsBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
@@ -195,14 +210,16 @@
 
         map.get("root").map(|v| builder.root(v));
         map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("access_key_id").map(|v| builder.access_key_id(v));
         map.get("secret_access_key")
             .map(|v| builder.secret_access_key(v));
+        map.get("write_min_size")
+            .map(|v| builder.write_min_size(v.parse().expect("input must be a number")));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", &self);
 
@@ -270,24 +287,33 @@
         let signer = HuaweicloudObsSigner::new({
             if is_obs_default {
                 &bucket
             } else {
                 &endpoint
             }
         });
+        let write_min_size = self.write_min_size.unwrap_or(DEFAULT_WRITE_MIN_SIZE);
+        if write_min_size < 100 * 1024 {
+            return Err(Error::new(
+                ErrorKind::ConfigInvalid,
+                "The write minimum buffer size is misconfigured",
+            )
+            .with_context("service", Scheme::Obs));
+        }
 
         debug!("backend build finished");
         Ok(ObsBackend {
             core: Arc::new(ObsCore {
                 bucket,
                 root,
                 endpoint: format!("{}://{}", &scheme, &endpoint),
                 signer,
                 loader: cred_loader,
                 client,
+                write_min_size,
             }),
         })
     }
 }
 
 /// Backend for Huaweicloud OBS services.
 #[derive(Debug, Clone)]
@@ -321,14 +347,15 @@
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
                 write_can_sink: true,
                 write_with_content_type: true,
                 write_with_cache_control: true,
+                write_without_content_length: true,
 
                 append: true,
                 append_with_cache_control: true,
                 append_with_content_type: true,
                 append_with_content_disposition: true,
 
                 delete: true,
@@ -416,24 +443,17 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.content_length().is_none() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "write without content length is not supported",
-            ));
-        }
-
         Ok((
             RpWrite::default(),
-            ObsWriter::new(self.core.clone(), args, path.to_string()),
+            ObsWriter::new(self.core.clone(), path, args),
         ))
     }
 
     async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
         Ok((
             RpAppend::default(),
             ObsAppender::new(self.core.clone(), path, args),
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files 24% similar despite different names*

```diff
@@ -15,37 +15,41 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::time::Duration;
 
+use bytes::Bytes;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use reqsign::HuaweicloudObsCredential;
 use reqsign::HuaweicloudObsCredentialLoader;
 use reqsign::HuaweicloudObsSigner;
+use serde::Deserialize;
+use serde::Serialize;
 
 use crate::raw::*;
 use crate::*;
 
 pub struct ObsCore {
     pub bucket: String,
     pub root: String,
     pub endpoint: String,
 
     pub signer: HuaweicloudObsSigner,
     pub loader: HuaweicloudObsCredentialLoader,
     pub client: HttpClient,
+    pub write_min_size: usize,
 }
 
 impl Debug for ObsCore {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Backend")
             .field("root", &self.root)
             .field("bucket", &self.bucket)
@@ -323,8 +327,166 @@
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
+    pub async fn obs_initiate_multipart_upload(
+        &self,
+        path: &str,
+        content_type: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}?uploads", self.endpoint, percent_encode_path(&p));
+        let mut req = Request::post(&url);
+
+        if let Some(mime) = content_type {
+            req = req.header(CONTENT_TYPE, mime)
+        }
+        let mut req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+    pub async fn obs_upload_part_request(
+        &self,
+        path: &str,
+        upload_id: &str,
+        part_number: usize,
+        size: Option<u64>,
+        body: AsyncBody,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!(
+            "{}/{}?partNumber={}&uploadId={}",
+            self.endpoint,
+            percent_encode_path(&p),
+            part_number,
+            percent_encode_path(upload_id)
+        );
+
+        let mut req = Request::put(&url);
+
+        if let Some(size) = size {
+            req = req.header(CONTENT_LENGTH, size);
+        }
+
+        // Set body
+        let mut req = req.body(body).map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub async fn obs_complete_multipart_upload(
+        &self,
+        path: &str,
+        upload_id: &str,
+        parts: &[CompleteMultipartUploadRequestPart],
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/{}?uploadId={}",
+            self.endpoint,
+            percent_encode_path(&p),
+            percent_encode_path(upload_id)
+        );
+
+        let req = Request::post(&url);
+
+        let content = quick_xml::se::to_string(&CompleteMultipartUploadRequest {
+            part: parts.to_vec(),
+        })
+        .map_err(new_xml_deserialize_error)?;
+        // Make sure content length has been set to avoid post with chunked encoding.
+        let req = req.header(CONTENT_LENGTH, content.len());
+        // Set content-type to `application/xml` to avoid mixed with form post.
+        let req = req.header(CONTENT_TYPE, "application/xml");
+
+        let mut req = req
+            .body(AsyncBody::Bytes(Bytes::from(content)))
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
+
+    /// Abort an on-going multipart upload.
+    pub async fn obs_abort_multipart_upload(
+        &self,
+        path: &str,
+        upload_id: &str,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!(
+            "{}/{}?uploadId={}",
+            self.endpoint,
+            percent_encode_path(&p),
+            percent_encode_path(upload_id)
+        );
+
+        let mut req = Request::delete(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
+}
+/// Result of CreateMultipartUpload
+#[derive(Default, Debug, Deserialize)]
+#[serde(default, rename_all = "PascalCase")]
+pub struct InitiateMultipartUploadResult {
+    pub upload_id: String,
+}
+
+/// Request of CompleteMultipartUploadRequest
+#[derive(Default, Debug, Serialize)]
+#[serde(default, rename = "CompleteMultipartUpload", rename_all = "PascalCase")]
+pub struct CompleteMultipartUploadRequest {
+    pub part: Vec<CompleteMultipartUploadRequestPart>,
+}
+
+#[derive(Clone, Default, Debug, Serialize)]
+#[serde(default, rename_all = "PascalCase")]
+pub struct CompleteMultipartUploadRequestPart {
+    #[serde(rename = "PartNumber")]
+    pub part_number: usize,
+    ///
+    ///
+    /// quick-xml will do escape on `"` which leads to our serialized output is
+    /// not the same as aws s3's example.
+    ///
+    /// Ideally, we could use `serialize_with` to address this (buf failed)
+    ///
+    /// ```ignore
+    /// #[derive(Default, Debug, Serialize)]
+    /// #[serde(default, rename_all = "PascalCase")]
+    /// struct CompleteMultipartUploadRequestPart {
+    ///     #[serde(rename = "PartNumber")]
+    ///     part_number: usize,
+    ///     #[serde(rename = "ETag", serialize_with = "partial_escape")]
+    ///     etag: String,
+    /// }
+    ///
+    /// fn partial_escape<S>(s: &str, ser: S) -> std::result::Result<S::Ok, S::Error>
+    /// where
+    ///     S: serde::Serializer,
+    /// {
+    ///     ser.serialize_str(&String::from_utf8_lossy(
+    ///         &quick_xml::escape::partial_escape(s.as_bytes()),
+    ///     ))
+    /// }
+    /// ```
+    ///
+    /// ref: <https://github.com/tafia/quick-xml/issues/362>
+    #[serde(rename = "ETag")]
+    pub etag: String,
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     };
 
     let message = match de::from_reader::<_, ObsError>(bs.clone().reader()) {
         Ok(obs_error) => format!("{obs_error:?}"),
         Err(_) => String::from_utf8_lossy(&bs).into_owned(),
     };
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -11,71 +11,66 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::ObsCore;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct ObsWriter {
-    core: Arc<ObsCore>,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl ObsWriter {
-    pub fn new(core: Arc<ObsCore>, op: OpWrite, path: String) -> Self {
-        ObsWriter { core, op, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
+}
 
-    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
-        let mut req = self.core.obs_put_object_request(
-            &self.path,
-            Some(size),
-            self.op.content_type(),
-            self.op.cache_control(),
-            body,
-        )?;
-
-        self.core.sign(&mut req).await?;
+#[async_trait]
+impl oio::Write for WebhdfsWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        let req = self
+            .backend
+            .webhdfs_create_object_request(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
-        let resp = self.core.send(req).await?;
+        let resp = self.backend.client.send(req).await?;
 
         let status = resp.status();
-
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
-}
-
-#[async_trait]
-impl oio::Write for ObsWriter {
-    async fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
-            .await
-    }
 
-    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
-        self.write_oneshot(size, AsyncBody::Stream(s)).await
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
     }
 
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/builder.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/gdrive/error.rs`

 * *Files 11% similar despite different names*

```diff
@@ -34,16 +34,19 @@
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-        .with_context("response", format!("{parts:?}"));
+    let message = String::from_utf8_lossy(&bs);
+
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/graph_model.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/appender.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/oss/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 use super::pager::OssPager;
 use super::writer::OssWriter;
 use crate::raw::*;
 use crate::*;
 
 const DEFAULT_WRITE_MIN_SIZE: usize = 8 * 1024 * 1024;
 const DEFAULT_BATCH_MAX_OPERATIONS: usize = 1000;
+
 /// Aliyun Object Storage Service (OSS) support
 #[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct OssBuilder {
     root: Option<String>,
 
     endpoint: Option<String>,
@@ -381,15 +382,15 @@
     core: Arc<OssCore>,
 }
 
 #[async_trait]
 impl Accessor for OssBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
-    type Writer = OssWriter;
+    type Writer = oio::MultipartUploadWriter<OssWriter>;
     type BlockingWriter = ();
     type Appender = OssAppender;
     type Pager = OssPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
@@ -407,14 +408,15 @@
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
                 write_can_sink: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
+                write_with_content_disposition: true,
                 write_without_content_length: true,
                 delete: true,
                 create_dir: true,
                 copy: true,
 
                 append: true,
                 append_with_cache_control: true,
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 5% similar despite different names*

```diff
@@ -485,89 +485,74 @@
             &self.endpoint
         }
     }
 
     pub async fn oss_initiate_upload(
         &self,
         path: &str,
-        args: &OpWrite,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let cache_control = args.cache_control();
-        let req = self
-            .oss_initiate_upload_request(path, None, None, cache_control, AsyncBody::Empty, false)
-            .await?;
-        self.send(req).await
-    }
-
-    /// Creates a request that initiates multipart upload
-    async fn oss_initiate_upload_request(
-        &self,
-        path: &str,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
-        body: AsyncBody,
         is_presign: bool,
-    ) -> Result<Request<AsyncBody>> {
+    ) -> Result<Response<IncomingAsyncBody>> {
         let path = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
         let url = format!("{}/{}?uploads", endpoint, percent_encode_path(&path));
         let mut req = Request::post(&url);
         if let Some(mime) = content_type {
             req = req.header(CONTENT_TYPE, mime);
         }
         if let Some(disposition) = content_disposition {
             req = req.header(CONTENT_DISPOSITION, disposition);
         }
         if let Some(cache_control) = cache_control {
             req = req.header(CACHE_CONTROL, cache_control);
         }
         req = self.insert_sse_headers(req);
-        let mut req = req.body(body).map_err(new_request_build_error)?;
+        let mut req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
-        Ok(req)
+        self.send(req).await
     }
 
     /// Creates a request to upload a part
     pub async fn oss_upload_part_request(
         &self,
         path: &str,
         upload_id: &str,
         part_number: usize,
         is_presign: bool,
-        size: Option<u64>,
+        size: u64,
         body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
+    ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
 
         let url = format!(
             "{}/{}?partNumber={}&uploadId={}",
             endpoint,
             percent_encode_path(&p),
             part_number,
             percent_encode_path(upload_id)
         );
 
         let mut req = Request::put(&url);
-
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size);
-        }
+        req = req.header(CONTENT_LENGTH, size);
         let mut req = req.body(body).map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
-        Ok(req)
+        self.send(req).await
     }
 
     pub async fn oss_complete_multipart_upload_request(
         &self,
         path: &str,
         upload_id: &str,
         is_presign: bool,
-        parts: &[MultipartUploadPart],
+        parts: Vec<MultipartUploadPart>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
         let url = format!(
             "{}/{}?uploadId={}",
             endpoint,
             percent_encode_path(&p),
@@ -588,14 +573,37 @@
         let mut req = req
             .body(AsyncBody::Bytes(Bytes::from(content)))
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
+
+    /// Abort an on-going multipart upload.
+    /// reference docs https://www.alibabacloud.com/help/zh/oss/developer-reference/abortmultipartupload
+    pub async fn oss_abort_multipart_upload(
+        &self,
+        path: &str,
+        upload_id: &str,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!(
+            "{}/{}?uploadId={}",
+            self.endpoint,
+            percent_encode_path(&p),
+            percent_encode_path(upload_id)
+        );
+
+        let mut req = Request::delete(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
 }
 
 /// Request of DeleteObjects.
 #[derive(Default, Debug, Serialize)]
 #[serde(default, rename = "Delete", rename_all = "PascalCase")]
 pub struct DeleteObjectsRequest {
     pub object: Vec<DeleteObjectsRequestObject>,
@@ -768,17 +776,18 @@
                     part_number: 8,
                     etag: "\"8C315065167132444177411FDA14****\"".to_string(),
                 },
             ],
         };
 
         // quick_xml::se::to_string()
-        let mut serializer = quick_xml::se::Serializer::new(String::new());
+        let mut serialized = String::new();
+        let mut serializer = quick_xml::se::Serializer::new(&mut serialized);
         serializer.indent(' ', 4);
-        let serialized = req.serialize(serializer).unwrap();
+        req.serialize(serializer).unwrap();
         pretty_assertions::assert_eq!(
             serialized,
             r#"<CompleteMultipartUpload>
     <Part>
         <PartNumber>1</PartNumber>
         <ETag>"3349DC700140D7F86A0784842780****"</ETag>
     </Part>
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/oss/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,17 @@
     };
 
     let message = match de::from_reader::<_, OssError>(bs.clone().reader()) {
         Ok(oss_err) => format!("{oss_err:?}"),
         Err(_) => String::from_utf8_lossy(&bs).into_owned(),
     };
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -23,50 +23,48 @@
 use http::StatusCode;
 
 use super::core::*;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct OssWriter {
-    core: Arc<OssCore>,
+pub struct ObsWriter {
+    core: Arc<ObsCore>,
 
     op: OpWrite,
     path: String,
     upload_id: Option<String>,
 
-    parts: Vec<MultipartUploadPart>,
+    parts: Vec<CompleteMultipartUploadRequestPart>,
     buffer: oio::VectorCursor,
     buffer_size: usize,
 }
 
-impl OssWriter {
-    pub fn new(core: Arc<OssCore>, path: &str, op: OpWrite) -> Self {
+impl ObsWriter {
+    pub fn new(core: Arc<ObsCore>, path: &str, op: OpWrite) -> Self {
         let buffer_size = core.write_min_size;
-        OssWriter {
+        ObsWriter {
             core,
             path: path.to_string(),
             op,
 
             upload_id: None,
             parts: vec![],
             buffer: oio::VectorCursor::new(),
             buffer_size,
         }
     }
 
     async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
-        let mut req = self.core.oss_put_object_request(
+        let mut req = self.core.obs_put_object_request(
             &self.path,
             Some(size),
             self.op.content_type(),
-            self.op.content_disposition(),
             self.op.cache_control(),
             body,
-            false,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
@@ -77,64 +75,77 @@
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn initiate_upload(&self) -> Result<String> {
-        let resp = self.core.oss_initiate_upload(&self.path, &self.op).await?;
-        match resp.status() {
+        let resp = self
+            .core
+            .obs_initiate_multipart_upload(&self.path, self.op.content_type())
+            .await?;
+
+        let status = resp.status();
+
+        match status {
             StatusCode::OK => {
                 let bs = resp.into_body().bytes().await?;
+
                 let result: InitiateMultipartUploadResult =
                     quick_xml::de::from_reader(bs.reader()).map_err(new_xml_deserialize_error)?;
+
                 Ok(result.upload_id)
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn write_part(&self, upload_id: &str, bs: Bytes) -> Result<MultipartUploadPart> {
-        // Aliyun OSS requires part number must between [1..=10000]
+    async fn write_part(
+        &self,
+        upload_id: &str,
+        bs: Bytes,
+    ) -> Result<CompleteMultipartUploadRequestPart> {
+        // Obs service requires part number must between [1..=10000]
         let part_number = self.parts.len() + 1;
-        let mut req = self
+
+        let resp = self
             .core
-            .oss_upload_part_request(
+            .obs_upload_part_request(
                 &self.path,
                 upload_id,
                 part_number,
-                false,
                 Some(bs.len() as u64),
                 AsyncBody::Bytes(bs),
             )
             .await?;
 
-        self.core.sign(&mut req).await?;
+        let status = resp.status();
 
-        let resp = self.core.send(req).await?;
-        match resp.status() {
+        match status {
             StatusCode::OK => {
                 let etag = parse_etag(resp.headers())?
                     .ok_or_else(|| {
                         Error::new(
                             ErrorKind::Unexpected,
                             "ETag not present in returning response",
                         )
                     })?
                     .to_string();
+
                 resp.into_body().consume().await?;
-                Ok(MultipartUploadPart { part_number, etag })
+
+                Ok(CompleteMultipartUploadRequestPart { part_number, etag })
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 }
 
 #[async_trait]
-impl oio::Write for OssWriter {
+impl oio::Write for ObsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let upload_id = match &self.upload_id {
             Some(upload_id) => upload_id,
             None => {
                 if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
                     return self
                         .write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
@@ -173,23 +184,44 @@
                 self.buffer.pop();
                 Err(e)
             }
         }
     }
 
     async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
-        self.write_oneshot(size, AsyncBody::Stream(s)).await
+        if self.op.content_length().unwrap_or_default() == size {
+            return self.write_oneshot(size, AsyncBody::Stream(s)).await;
+        } else {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "Obs does not support streaming multipart upload",
+            ));
+        }
     }
 
-    // TODO: we can cancel the upload by sending an abort request.
     async fn abort(&mut self) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support abort",
-        ))
+        let upload_id = if let Some(upload_id) = &self.upload_id {
+            upload_id
+        } else {
+            return Ok(());
+        };
+
+        let resp = self
+            .core
+            .obs_abort_multipart_upload(&self.path, upload_id)
+            .await?;
+        match resp.status() {
+            // Obs returns code 204 No Content if abort succeeds.
+            // Reference: https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0103.html
+            StatusCode::NO_CONTENT => {
+                resp.into_body().consume().await?;
+                Ok(())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
     }
 
     async fn close(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
             return Ok(());
@@ -208,17 +240,20 @@
                     return Err(e);
                 }
             }
         }
 
         let resp = self
             .core
-            .oss_complete_multipart_upload_request(&self.path, upload_id, false, &self.parts)
+            .obs_complete_multipart_upload(&self.path, upload_id, &self.parts)
             .await?;
-        match resp.status() {
+
+        let status = resp.status();
+
+        match status {
             StatusCode::OK => {
                 resp.into_body().consume().await?;
 
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/redb/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/redb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/redb/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/redb/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/redb/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/redb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files 7% similar despite different names*

```diff
@@ -181,15 +181,26 @@
                 let host = ep_url
                     .host()
                     .map(|h| h.to_string())
                     .unwrap_or_else(|| "127.0.0.1".to_string());
                 let port = ep_url.port_u16().unwrap_or(DEFAULT_REDIS_PORT);
                 ConnectionAddr::Tcp(host, port)
             }
-            // TODO: wait for upstream to support `rustls` based TLS connection.
+            Some("rediss") => {
+                let host = ep_url
+                    .host()
+                    .map(|h| h.to_string())
+                    .unwrap_or_else(|| "127.0.0.1".to_string());
+                let port = ep_url.port_u16().unwrap_or(DEFAULT_REDIS_PORT);
+                ConnectionAddr::TcpTls {
+                    host,
+                    port,
+                    insecure: false,
+                }
+            }
             Some("unix") | Some("redis+unix") => {
                 let path = PathBuf::from(ep_url.path());
                 ConnectionAddr::Unix(path)
             }
             Some(s) => {
                 return Err(
                     Error::new(ErrorKind::ConfigInvalid, "invalid or unsupported scheme")
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/redis/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/redis/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/rocksdb/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/persy/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::RocksdbBuilder as Rocksdb;
+
+pub use backend::PersyBuilder as Persy;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 use bytes::Buf;
 use http::StatusCode;
 use log::debug;
 use log::warn;
 use md5::Digest;
 use md5::Md5;
 use once_cell::sync::Lazy;
+use reqsign::AwsAssumeRoleLoader;
 use reqsign::AwsConfig;
 use reqsign::AwsCredentialLoad;
-use reqsign::AwsLoader;
+use reqsign::AwsDefaultLoader;
 use reqsign::AwsV4Signer;
 
 use super::core::*;
 use super::error::parse_error;
 use super::error::parse_s3_error_code;
 use super::pager::S3Pager;
 use super::writer::S3Writer;
@@ -65,41 +66,42 @@
 #[derive(Default)]
 pub struct S3Builder {
     root: Option<String>,
 
     bucket: String,
     endpoint: Option<String>,
     region: Option<String>,
-    role_arn: Option<String>,
-    external_id: Option<String>,
+
+    // Credentials related values.
     access_key_id: Option<String>,
     secret_access_key: Option<String>,
+    security_token: Option<String>,
+    role_arn: Option<String>,
+    external_id: Option<String>,
+    disable_config_load: bool,
+    disable_ec2_metadata: bool,
+    allow_anonymous: bool,
+    customed_credential_load: Option<Box<dyn AwsCredentialLoad>>,
+
+    // S3 features flags
     server_side_encryption: Option<String>,
     server_side_encryption_aws_kms_key_id: Option<String>,
     server_side_encryption_customer_algorithm: Option<String>,
     server_side_encryption_customer_key: Option<String>,
     server_side_encryption_customer_key_md5: Option<String>,
     default_storage_class: Option<String>,
-
-    /// temporary credentials, check the official [doc](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp.html) for detail
-    security_token: Option<String>,
-
-    disable_config_load: bool,
-    disable_ec2_metadata: bool,
-    allow_anonymous: bool,
     enable_virtual_host_style: bool,
 
-    http_client: Option<HttpClient>,
-    customed_credential_load: Option<Box<dyn AwsCredentialLoad>>,
-
     /// the part size of s3 multipart upload, which should be 5 MiB to 5 GiB.
     /// There is no minimum size limit on the last part of your multipart upload
     write_min_size: Option<usize>,
     /// batch_max_operations
     batch_max_operations: Option<usize>,
+
+    http_client: Option<HttpClient>,
 }
 
 impl Debug for S3Builder {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut d = f.debug_struct("Builder");
 
         d.field("root", &self.root)
@@ -187,14 +189,17 @@
             self.secret_access_key = Some(v.to_string())
         }
 
         self
     }
 
     /// Set role_arn for this backend.
+    ///
+    /// If `role_arn` is set, we will use already known config as source
+    /// credential to assume role with `role_arn`.
     pub fn role_arn(&mut self, v: &str) -> &mut Self {
         if !v.is_empty() {
             self.role_arn = Some(v.to_string())
         }
 
         self
     }
@@ -428,14 +433,17 @@
     /// - Enabled, opendal will send API to `https://bucket_name.s3.us-east-1.amazonaws.com`
     pub fn enable_virtual_host_style(&mut self) -> &mut Self {
         self.enable_virtual_host_style = true;
         self
     }
 
     /// Adding a customed credential load for service.
+    ///
+    /// If customed_credential_load has been set, we will ignore all other
+    /// credential load methods.
     pub fn customed_credential_load(&mut self, cred: Box<dyn AwsCredentialLoad>) -> &mut Self {
         self.customed_credential_load = Some(cred);
         self
     }
 
     /// Specify the http client that used by this service.
     ///
@@ -544,23 +552,22 @@
     ///
     /// # Examples
     ///
     /// ```no_run
     /// use opendal::services::S3;
     ///
     /// # async fn example() {
-    /// let builder = S3::default();
-    /// let region: Option<String> = builder.detect_region("https://s3.amazonaws.com", "example").await;
+    /// let region: Option<String> = S3::detect_region("https://s3.amazonaws.com", "example").await;
     /// # }
     /// ```
     ///
     /// # Reference
     ///
     /// - [Amazon S3 HeadBucket API](https://docs.aws.amazon.com/zh_cn/AmazonS3/latest/API/API_HeadBucket.html)
-    pub async fn detect_region(&self, endpoint: &str, bucket: &str) -> Option<String> {
+    pub async fn detect_region(endpoint: &str, bucket: &str) -> Option<String> {
         let mut endpoint = if endpoint.starts_with("http") {
             endpoint.to_string()
         } else {
             // Prefix https if endpoint doesn't start with scheme.
             format!("https://{}", endpoint)
         };
 
@@ -612,26 +619,27 @@
 
         debug!(
             "auto detect region got response: status {:?}, header: {:?}",
             res.status(),
             res.headers()
         );
 
-        match res.status() {
-            StatusCode::OK | StatusCode::FORBIDDEN | StatusCode::MOVED_PERMANENTLY => {
-                let region = res.headers().get("x-amz-bucket-region")?;
-                if let Ok(regin) = region.to_str() {
-                    Some(regin.to_string())
-                } else {
-                    None
-                }
-            }
-            // Unexpected status code
-            _ => None,
+        // Get region from response header no matter status code.
+        let region = res.headers().get("x-amz-bucket-region")?;
+        if let Ok(regin) = region.to_str() {
+            return Some(regin.to_string());
         }
+
+        // Status code is 403 or 200 means we already visit the correct
+        // region, we can use the default region directly.
+        if res.status() == StatusCode::FORBIDDEN || res.status() == StatusCode::OK {
+            return Some("us-east-1".to_string());
+        }
+
+        None
     }
 }
 
 impl Builder for S3Builder {
     const SCHEME: Scheme = Scheme::S3;
     type Accessor = S3Backend;
 
@@ -749,40 +757,24 @@
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
                     .with_context("service", Scheme::S3)
             })?
         };
 
+        // This is our current config.
         let mut cfg = AwsConfig::default();
         if !self.disable_config_load {
             cfg = cfg.from_profile();
             cfg = cfg.from_env();
         }
 
-        // Setting all value from user input if available.
         if let Some(v) = self.region.take() {
             cfg.region = Some(v);
         }
-        if let Some(v) = self.access_key_id.take() {
-            cfg.access_key_id = Some(v)
-        }
-        if let Some(v) = self.secret_access_key.take() {
-            cfg.secret_access_key = Some(v)
-        }
-        if let Some(v) = self.security_token.take() {
-            cfg.session_token = Some(v)
-        }
-        if let Some(v) = self.role_arn.take() {
-            cfg.role_arn = Some(v)
-        }
-        if let Some(v) = self.external_id.take() {
-            cfg.external_id = Some(v)
-        }
-
         if cfg.region.is_none() {
             // AWS S3 requires region to be set.
             if self.endpoint.is_none()
                 || self.endpoint.as_deref() == Some("https://s3.amazonaws.com")
             {
                 return Err(Error::new(ErrorKind::ConfigInvalid, "region is missing")
                     .with_operation("Builder::build")
@@ -798,23 +790,74 @@
         let region = cfg.region.to_owned().unwrap();
         debug!("backend use region: {region}");
 
         // Building endpoint.
         let endpoint = self.build_endpoint(&region);
         debug!("backend use endpoint: {endpoint}");
 
-        let mut loader = AwsLoader::new(client.client(), cfg);
-        if self.disable_ec2_metadata {
-            loader = loader.with_disable_ec2_metadata();
+        // Setting all value from user input if available.
+        if let Some(v) = self.access_key_id.take() {
+            cfg.access_key_id = Some(v)
+        }
+        if let Some(v) = self.secret_access_key.take() {
+            cfg.secret_access_key = Some(v)
+        }
+        if let Some(v) = self.security_token.take() {
+            cfg.session_token = Some(v)
         }
+
+        let mut loader: Option<Box<dyn AwsCredentialLoad>> = None;
+        // If customed_credential_load is set, we will use it.
         if let Some(v) = self.customed_credential_load.take() {
-            loader = loader.with_customed_credential_loader(v);
+            loader = Some(v);
         }
 
+        // If role_arn is set, we must use AssumeRoleLoad.
+        if let Some(role_arn) = self.role_arn.take() {
+            // use current env as source credential loader.
+            let default_loader = AwsDefaultLoader::new(client.client(), cfg.clone());
+
+            // Build the config for assume role.
+            let assume_role_cfg = AwsConfig {
+                region: Some(region.clone()),
+                role_arn: Some(role_arn),
+                external_id: self.external_id.clone(),
+                sts_regional_endpoints: "regional".to_string(),
+                ..Default::default()
+            };
+            let assume_role_loader = AwsAssumeRoleLoader::new(
+                client.client(),
+                assume_role_cfg,
+                Box::new(default_loader),
+            )
+            .map_err(|err| {
+                Error::new(
+                    ErrorKind::ConfigInvalid,
+                    "The assume_role_loader is misconfigured",
+                )
+                .with_context("service", Scheme::S3)
+                .set_source(err)
+            })?;
+            loader = Some(Box::new(assume_role_loader));
+        }
+        // If loader is not set, we will use default loader.
+        let loader = match loader {
+            Some(v) => v,
+            None => {
+                let mut default_loader = AwsDefaultLoader::new(client.client(), cfg);
+                if self.disable_ec2_metadata {
+                    default_loader = default_loader.with_disable_ec2_metadata();
+                }
+
+                Box::new(default_loader)
+            }
+        };
+
         let signer = AwsV4Signer::new("s3", &region);
+
         let write_min_size = self.write_min_size.unwrap_or(DEFAULT_WRITE_MIN_SIZE);
         if write_min_size < 5 * 1024 * 1024 {
             return Err(Error::new(
                 ErrorKind::ConfigInvalid,
                 "The write minimum buffer size is misconfigured",
             )
             .with_context("service", Scheme::S3));
@@ -851,15 +894,15 @@
     core: Arc<S3Core>,
 }
 
 #[async_trait]
 impl Accessor for S3Backend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
-    type Writer = S3Writer;
+    type Writer = oio::MultipartUploadWriter<S3Writer>;
     type BlockingWriter = ();
     type Appender = ();
     type Pager = S3Pager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
@@ -874,14 +917,15 @@
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
                 read_with_override_cache_control: true,
                 read_with_override_content_disposition: true,
+                read_with_override_content_type: true,
 
                 write: true,
                 write_can_sink: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
                 create_dir: true,
@@ -925,24 +969,15 @@
                 Ok(RpCreateDir::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self
-            .core
-            .s3_get_object(
-                path,
-                args.range(),
-                args.if_none_match(),
-                args.if_match(),
-                args.override_content_disposition(),
-            )
-            .await?;
+        let resp = self.core.s3_get_object(path, args).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
@@ -1024,22 +1059,15 @@
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
                 self.core
                     .s3_head_object_request(path, v.if_none_match(), v.if_match())?
             }
-            PresignOperation::Read(v) => self.core.s3_get_object_request(
-                path,
-                v.range(),
-                v.override_content_disposition(),
-                v.override_cache_control(),
-                v.if_none_match(),
-                v.if_match(),
-            )?,
+            PresignOperation::Read(v) => self.core.s3_get_object_request(path, v.clone())?,
             PresignOperation::Write(_) => {
                 self.core
                     .s3_put_object_request(path, None, None, None, None, AsyncBody::Empty)?
             }
         };
 
         self.core.sign_query(&mut req, args.expire()).await?;
@@ -1199,15 +1227,13 @@
                 "invalid service",
                 "https://opendal.apache.org",
                 "example",
                 None,
             ),
         ];
 
-        let b = S3Builder::default();
-
         for (name, endpoint, bucket, expected) in cases {
-            let region = b.detect_region(endpoint, bucket).await;
+            let region = S3Builder::detect_region(endpoint, bucket).await;
             assert_eq!(region.as_deref(), expected, "{}", name);
         }
     }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,19 @@
 
 use bytes::Bytes;
 use http::header::HeaderName;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
-use http::header::IF_MATCH;
-use http::header::IF_NONE_MATCH;
 use http::HeaderValue;
 use http::Request;
 use http::Response;
 use reqsign::AwsCredential;
-use reqsign::AwsLoader;
+use reqsign::AwsDefaultLoader;
 use reqsign::AwsV4Signer;
 use serde::Deserialize;
 use serde::Serialize;
 
 use crate::raw::*;
 use crate::*;
 
@@ -51,68 +49,68 @@
         "x-amz-server-side-encryption-customer-key";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-server-side-encryption-customer-key-md5";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_AWS_KMS_KEY_ID: &str =
         "x-amz-server-side-encryption-aws-kms-key-id";
     pub const X_AMZ_STORAGE_CLASS: &str = "x-amz-storage-class";
 
+    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_ALGORITHM: &str =
         "x-amz-copy-source-server-side-encryption-customer-algorithm";
+    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY: &str =
         "x-amz-copy-source-server-side-encryption-customer-key";
+    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-copy-source-server-side-encryption-customer-key-md5";
 
     pub const RESPONSE_CONTENT_DISPOSITION: &str = "response-content-disposition";
     pub const RESPONSE_CACHE_CONTROL: &str = "response-cache-control";
+
+    pub const DESTINATION: &str = "Destination";
+    pub const OVERWRITE: &str = "Overwrite";
 }
 
-pub struct S3Core {
+pub struct WasabiCore {
     pub bucket: String,
     pub endpoint: String,
     pub root: String,
     pub server_side_encryption: Option<HeaderValue>,
     pub server_side_encryption_aws_kms_key_id: Option<HeaderValue>,
     pub server_side_encryption_customer_algorithm: Option<HeaderValue>,
     pub server_side_encryption_customer_key: Option<HeaderValue>,
     pub server_side_encryption_customer_key_md5: Option<HeaderValue>,
     pub default_storage_class: Option<HeaderValue>,
-    pub allow_anonymous: bool,
 
     pub signer: AwsV4Signer,
-    pub loader: AwsLoader,
+    pub loader: AwsDefaultLoader,
     pub client: HttpClient,
-    pub write_min_size: usize,
-    pub batch_max_operations: usize,
 }
 
-impl Debug for S3Core {
+impl Debug for WasabiCore {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
-        f.debug_struct("S3Core")
+        f.debug_struct("WasabiCore")
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .field("root", &self.root)
             .finish_non_exhaustive()
     }
 }
 
-impl S3Core {
+impl WasabiCore {
     /// If credential is not found, we will not sign the request.
     async fn load_credential(&self) -> Result<Option<AwsCredential>> {
         let cred = self
             .loader
             .load()
             .await
             .map_err(new_request_credential_error)?;
 
         if let Some(cred) = cred {
             Ok(Some(cred))
-        } else if self.allow_anonymous {
-            // If allow_anonymous has been set, we will not sign the request.
-            Ok(None)
         } else {
             // Mark this error as temporary since it could be caused by AWS STS.
             Err(Error::new(
                 ErrorKind::PermissionDenied,
                 "no valid credential found, please check configuration or try again",
             )
             .set_temporary())
@@ -204,52 +202,46 @@
             )
         }
 
         req
     }
 }
 
-impl S3Core {
-    pub fn s3_head_object_request(
-        &self,
-        path: &str,
-        if_none_match: Option<&str>,
-        if_match: Option<&str>,
-    ) -> Result<Request<AsyncBody>> {
+impl WasabiCore {
+    pub fn head_object_request(&self, path: &str, args: &OpStat) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
         req = self.insert_sse_headers(req, false);
 
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
+        if let Some(v) = args.if_match() {
+            req = req.header(http::header::IF_MATCH, v);
         }
 
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
+        if let Some(v) = args.if_none_match() {
+            req = req.header(http::header::IF_NONE_MATCH, v);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub fn s3_get_object_request(
+    pub fn get_object_request(
         &self,
         path: &str,
         range: BytesRange,
         override_content_disposition: Option<&str>,
         override_cache_control: Option<&str>,
         if_none_match: Option<&str>,
-        if_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         // Construct headers to add to the request
         let mut url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         // Add query arguments to the URL based on response overrides
@@ -275,57 +267,45 @@
         let mut req = Request::get(&url);
 
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header());
         }
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
+            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
         }
 
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
-        }
         // Set SSE headers.
         // TODO: how will this work with presign?
         req = self.insert_sse_headers(req, false);
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn s3_get_object(
+    pub async fn get_object(
         &self,
         path: &str,
         range: BytesRange,
         if_none_match: Option<&str>,
-        if_match: Option<&str>,
-        override_content_disposition: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.s3_get_object_request(
-            path,
-            range,
-            override_content_disposition,
-            None,
-            if_none_match,
-            if_match,
-        )?;
+        let mut req = self.get_object_request(path, range, None, None, if_none_match)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn s3_put_object_request(
+    pub fn put_object_request(
         &self,
         path: &str,
-        size: Option<u64>,
+        size: Option<usize>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
@@ -359,46 +339,41 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn s3_head_object(
+    pub async fn head_object(
         &self,
         path: &str,
-        if_none_match: Option<&str>,
-        if_match: Option<&str>,
+        args: &OpStat,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.s3_head_object_request(path, if_none_match, if_match)?;
+        let mut req = self.head_object_request(path, args)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn s3_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn s3_copy_object(
-        &self,
-        from: &str,
-        to: &str,
-    ) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn copy_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
         let from = build_abs_path(&self.root, from);
         let to = build_abs_path(&self.root, to);
 
         let source = format!("{}/{}", self.bucket, percent_encode_path(&from));
         let target = format!("{}/{}", self.endpoint, percent_encode_path(&to));
 
         let mut req = Request::put(&target);
@@ -448,40 +423,33 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn s3_list_objects(
+    /// Make this functions as `pub(suber)` because `DirStream` depends
+    /// on this.
+    pub async fn list_objects(
         &self,
         path: &str,
         continuation_token: &str,
         delimiter: &str,
         limit: Option<usize>,
-        start_after: Option<String>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let mut url = format!("{}?list-type=2", self.endpoint);
-        if !p.is_empty() {
-            write!(url, "&prefix={}", percent_encode_path(&p))
-                .expect("write into string must succeed");
-        }
-        if !delimiter.is_empty() {
-            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
-        }
+        let mut url = format!(
+            "{}?list-type=2&delimiter={delimiter}&prefix={}",
+            self.endpoint,
+            percent_encode_path(&p)
+        );
         if let Some(limit) = limit {
             write!(url, "&max-keys={limit}").expect("write into string must succeed");
         }
-        if let Some(start_after) = start_after {
-            let start_after = build_abs_path(&self.root, &start_after);
-            write!(url, "&start-after={}", percent_encode_path(&start_after))
-                .expect("write into string must succeed");
-        }
         if !continuation_token.is_empty() {
             // AWS S3 could return continuation-token that contains `=`
             // which could lead `reqsign` parse query wrongly.
             // URL encode continuation-token before starting signing so that
             // our signer will not be confused.
             write!(
                 url,
@@ -496,15 +464,15 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn s3_initiate_multipart_upload(
+    pub async fn initiate_multipart_upload(
         &self,
         path: &str,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
@@ -538,15 +506,15 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn s3_upload_part_request(
+    pub fn upload_part_request(
         &self,
         path: &str,
         upload_id: &str,
         part_number: usize,
         size: Option<u64>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
@@ -571,15 +539,15 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn s3_complete_multipart_upload(
+    pub async fn complete_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
         parts: &[CompleteMultipartUploadRequestPart],
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
@@ -610,15 +578,15 @@
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     /// Abort an on-going multipart upload.
-    pub async fn s3_abort_multipart_upload(
+    pub async fn abort_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
@@ -631,18 +599,15 @@
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn s3_delete_objects(
-        &self,
-        paths: Vec<String>,
-    ) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn delete_objects(&self, paths: Vec<String>) -> Result<Response<IncomingAsyncBody>> {
         let url = format!("{}/?delete", self.endpoint);
 
         let req = Request::post(&url);
 
         let content = quick_xml::se::to_string(&DeleteObjectsRequest {
             object: paths
                 .into_iter()
@@ -664,14 +629,90 @@
             .body(AsyncBody::Bytes(Bytes::from(content)))
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
+
+    pub async fn put_object(
+        &self,
+        path: &str,
+        size: Option<usize>,
+        content_type: Option<&str>,
+        content_disposition: Option<&str>,
+        cache_control: Option<&str>,
+        body: AsyncBody,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.put_object_request(
+            path,
+            size,
+            content_type,
+            content_disposition,
+            cache_control,
+            body,
+        )?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub async fn rename_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
+        let from = percent_encode_path(build_abs_path(&self.root, from).as_str());
+        let to = percent_encode_path(build_abs_path(&self.root, to).as_str());
+
+        let url = format!("{}/{}", self.endpoint, from);
+
+        let mut req = Request::builder().method("MOVE").uri(url);
+
+        // Set SSE headers.
+        req = self.insert_sse_headers(req, true);
+
+        let mut req = req
+            .header(constants::DESTINATION, to)
+            .header(constants::OVERWRITE, "true")
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub async fn append_object(
+        &self,
+        path: &str,
+        size: Option<usize>,
+        body: AsyncBody,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}?append", self.endpoint, percent_encode_path(&p));
+
+        let mut req = Request::put(&url);
+
+        if let Some(size) = size {
+            req = req.header(CONTENT_LENGTH, size)
+        }
+
+        // Set storage class header
+        if let Some(v) = &self.default_storage_class {
+            req = req.header(HeaderName::from_static(constants::X_AMZ_STORAGE_CLASS), v);
+        }
+
+        // Set SSE headers.
+        req = self.insert_sse_headers(req, true);
+
+        let mut req = req.body(body).map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
 }
 
 /// Result of CreateMultipartUpload
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
 pub struct InitiateMultipartUploadResult {
     pub upload_id: String,
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/s3/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use bytes::Buf;
 use http::Response;
-use http::Uri;
 use quick_xml::de;
 use serde::Deserialize;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
@@ -56,24 +55,22 @@
         .map(|s3_err| (format!("{s3_err:?}"), Some(s3_err)))
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
     if let Some(s3_err) = s3_err {
         (kind, retryable) = parse_s3_error_code(s3_err.code.as_str()).unwrap_or((kind, retryable));
     }
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
-    if let Some(uri) = parts.extensions.get::<Uri>() {
-        err = err.with_context("uri", uri.to_string());
-    }
-
     Ok(err)
 }
 
 /// Returns the `Error kind` of this code and whether the error is retryable.
 /// All possible error code: <https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#ErrorCodeList>
 pub fn parse_s3_error_code(code: &str) -> Option<(ErrorKind, bool)> {
     match code {
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/write/multipart_upload_write.rs`

 * *Files 18% similar despite different names*

```diff
@@ -11,161 +11,147 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
-use bytes::Buf;
 use bytes::Bytes;
-use http::StatusCode;
 
-use super::core::*;
-use super::error::parse_error;
-use crate::raw::*;
-use crate::*;
+use crate::{raw::*, *};
 
-pub struct S3Writer {
-    core: Arc<S3Core>,
+const DEFAULT_WRITE_MIN_SIZE: usize = 8 * 1024 * 1024;
 
-    op: OpWrite,
-    path: String,
-    upload_id: Option<String>,
+/// MultipartUploadWrite is used to implement [`Write`] based on multipart
+/// uploads. By implementing MultipartUploadWrite, services don't need to
+/// care about the details of buffering and uploading parts.
+///
+/// The layout after adopting [`MultipartUploadWrite`]:
+///
+/// - Services impl `MultipartUploadWrite`
+/// - `MultipartUploadWriter` impl `Write`
+/// - Expose `MultipartUploadWriter` as `Accessor::Writer`
+#[async_trait]
+pub trait MultipartUploadWrite: Send + Sync + Unpin {
+    /// write_once write all data at once.
+    ///
+    /// MultipartUploadWriter will call this API when the size of data is
+    /// already known.
+    async fn write_once(&self, size: u64, body: AsyncBody) -> Result<()>;
+
+    /// initiate_part will call start a multipart upload and return the upload id.
+    ///
+    /// MultipartUploadWriter will call this when:
+    ///
+    /// - the total size of data is unknown.
+    /// - the total size of data is known, but the size of current write
+    /// is less then the total size.
+    async fn initiate_part(&self) -> Result<String>;
+
+    /// write_part will write a part of the data and returns the result
+    /// [`MultipartUploadPart`].
+    ///
+    /// MultipartUploadWriter will call this API and stores the result in
+    /// order.
+    ///
+    /// - part_number is the index of the part, starting from 0.
+    async fn write_part(
+        &self,
+        upload_id: &str,
+        part_number: usize,
+        size: u64,
+        body: AsyncBody,
+    ) -> Result<MultipartUploadPart>;
+
+    /// complete_part will complete the multipart upload to build the final
+    /// file.
+    async fn complete_part(&self, upload_id: &str, parts: &[MultipartUploadPart]) -> Result<()>;
+
+    /// abort_part will cancel the multipart upload and purge all data.
+    async fn abort_part(&self, upload_id: &str) -> Result<()>;
+}
 
-    parts: Vec<CompleteMultipartUploadRequestPart>,
+/// The result of [`MultipartUploadWrite::write_part`].
+///
+/// services implement should convert MultipartUploadPart to their own represents.
+///
+/// - `part_number` is the index of the part, starting from 0.
+/// - `etag` is the `ETag` of the part.
+pub struct MultipartUploadPart {
+    /// The number of the part, starting from 0.
+    pub part_number: usize,
+    /// The etag of the part.
+    pub etag: String,
+}
+
+/// MultipartUploadWriter will implements [`Write`] based on multipart
+/// uploads.
+///
+/// ## TODO
+///
+/// - Add threshold for `write_once` to avoid unnecessary multipart uploads.
+/// - Allow users to switch to un-buffered mode if users write 16MiB every time.
+pub struct MultipartUploadWriter<W: MultipartUploadWrite> {
+    inner: W,
+    total_size: Option<u64>,
+
+    upload_id: Option<String>,
+    parts: Vec<MultipartUploadPart>,
     buffer: oio::VectorCursor,
     buffer_size: usize,
 }
 
-impl S3Writer {
-    pub fn new(core: Arc<S3Core>, path: &str, op: OpWrite) -> Self {
-        let buffer_size = core.write_min_size;
-        S3Writer {
-            core,
-            path: path.to_string(),
-            op,
+impl<W: MultipartUploadWrite> MultipartUploadWriter<W> {
+    /// Create a new MultipartUploadWriter.
+    pub fn new(inner: W, total_size: Option<u64>) -> Self {
+        Self {
+            inner,
+            total_size,
 
             upload_id: None,
-            parts: vec![],
+            parts: Vec::new(),
             buffer: oio::VectorCursor::new(),
-            buffer_size,
-        }
-    }
-
-    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
-        let mut req = self.core.s3_put_object_request(
-            &self.path,
-            Some(size),
-            self.op.content_type(),
-            self.op.content_disposition(),
-            self.op.cache_control(),
-            body,
-        )?;
-
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
-
-        let status = resp.status();
-
-        match status {
-            StatusCode::CREATED | StatusCode::OK => {
-                resp.into_body().consume().await?;
-                Ok(())
-            }
-            _ => Err(parse_error(resp).await?),
+            buffer_size: DEFAULT_WRITE_MIN_SIZE,
         }
     }
 
-    async fn initiate_upload(&self) -> Result<String> {
-        let resp = self
-            .core
-            .s3_initiate_multipart_upload(
-                &self.path,
-                self.op.content_type(),
-                self.op.content_disposition(),
-                self.op.cache_control(),
-            )
-            .await?;
-
-        let status = resp.status();
-
-        match status {
-            StatusCode::OK => {
-                let bs = resp.into_body().bytes().await?;
-
-                let result: InitiateMultipartUploadResult =
-                    quick_xml::de::from_reader(bs.reader()).map_err(new_xml_deserialize_error)?;
-
-                Ok(result.upload_id)
-            }
-            _ => Err(parse_error(resp).await?),
-        }
-    }
-
-    async fn write_part(
-        &self,
-        upload_id: &str,
-        bs: Bytes,
-    ) -> Result<CompleteMultipartUploadRequestPart> {
-        // AWS S3 requires part number must between [1..=10000]
-        let part_number = self.parts.len() + 1;
-
-        let mut req = self.core.s3_upload_part_request(
-            &self.path,
-            upload_id,
-            part_number,
-            Some(bs.len() as u64),
-            AsyncBody::Bytes(bs),
-        )?;
-
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
-
-        let status = resp.status();
-
-        match status {
-            StatusCode::OK => {
-                let etag = parse_etag(resp.headers())?
-                    .ok_or_else(|| {
-                        Error::new(
-                            ErrorKind::Unexpected,
-                            "ETag not present in returning response",
-                        )
-                    })?
-                    .to_string();
-
-                resp.into_body().consume().await?;
-
-                Ok(CompleteMultipartUploadRequestPart { part_number, etag })
-            }
-            _ => Err(parse_error(resp).await?),
-        }
+    /// Configure the write_min_size.
+    ///
+    /// write_min_size is used to control the size of internal buffer.
+    ///
+    /// MultipartUploadWriter will flush the buffer to upload a part when
+    /// the size of buffer is larger than write_min_size.
+    ///
+    /// This value is default to 8 MiB (as recommended by AWS).
+    pub fn with_write_min_size(mut self, v: usize) -> Self {
+        self.buffer_size = v;
+        self
     }
 }
 
 #[async_trait]
-impl oio::Write for S3Writer {
+impl<W> oio::Write for MultipartUploadWriter<W>
+where
+    W: MultipartUploadWrite,
+{
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let upload_id = match &self.upload_id {
             Some(upload_id) => upload_id,
             None => {
-                if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
+                if self.total_size.unwrap_or_default() == bs.len() as u64 {
                     return self
-                        .write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+                        .inner
+                        .write_once(bs.len() as u64, AsyncBody::Bytes(bs))
                         .await;
-                } else {
-                    let upload_id = self.initiate_upload().await?;
-                    self.upload_id = Some(upload_id);
-                    self.upload_id.as_deref().unwrap()
                 }
+
+                let upload_id = self.inner.initiate_part().await?;
+                self.upload_id = Some(upload_id);
+                self.upload_id.as_deref().unwrap()
             }
         };
 
         // Ignore empty bytes
         if bs.is_empty() {
             return Ok(());
         }
@@ -175,15 +161,24 @@
         if self.buffer.len() <= self.buffer_size {
             return Ok(());
         }
 
         let bs = self.buffer.peak_at_least(self.buffer_size);
         let size = bs.len();
 
-        match self.write_part(upload_id, bs).await {
+        match self
+            .inner
+            .write_part(
+                upload_id,
+                self.parts.len(),
+                size as u64,
+                AsyncBody::Bytes(bs),
+            )
+            .await
+        {
             Ok(part) => {
                 self.buffer.take(size);
                 self.parts.push(part);
                 Ok(())
             }
             Err(e) => {
                 // If the upload fails, we should pop the given bs to make sure
@@ -191,77 +186,80 @@
                 self.buffer.pop();
                 Err(e)
             }
         }
     }
 
     async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
-        if self.op.content_length().unwrap_or_default() == size {
-            return self.write_oneshot(size, AsyncBody::Stream(s)).await;
-        } else {
+        if !self.buffer.is_empty() {
             return Err(Error::new(
-                ErrorKind::Unsupported,
-                "S3 does not support streaming multipart upload",
+                ErrorKind::InvalidInput,
+                "Writer::sink should not be used mixed with existing buffer",
             ));
         }
-    }
 
-    async fn abort(&mut self) -> Result<()> {
-        let upload_id = if let Some(upload_id) = &self.upload_id {
-            upload_id
-        } else {
-            return Ok(());
+        let upload_id = match &self.upload_id {
+            Some(upload_id) => upload_id,
+            None => {
+                if self.total_size.unwrap_or_default() == size {
+                    return self.inner.write_once(size, AsyncBody::Stream(s)).await;
+                }
+
+                let upload_id = self.inner.initiate_part().await?;
+                self.upload_id = Some(upload_id);
+                self.upload_id.as_deref().unwrap()
+            }
         };
 
-        let resp = self
-            .core
-            .s3_abort_multipart_upload(&self.path, upload_id)
+        let part = self
+            .inner
+            .write_part(upload_id, self.parts.len(), size, AsyncBody::Stream(s))
             .await?;
-        match resp.status() {
-            // s3 returns code 204 if abort succeeds.
-            StatusCode::NO_CONTENT => {
-                resp.into_body().consume().await?;
-                Ok(())
-            }
-            _ => Err(parse_error(resp).await?),
-        }
+        self.parts.push(part);
+
+        Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
             return Ok(());
         };
 
         // Make sure internal buffer has been flushed.
         if !self.buffer.is_empty() {
             let bs = self.buffer.peak_exact(self.buffer.len());
 
-            match self.write_part(upload_id, bs).await {
+            match self
+                .inner
+                .write_part(
+                    upload_id,
+                    self.parts.len(),
+                    bs.len() as u64,
+                    AsyncBody::Bytes(bs),
+                )
+                .await
+            {
                 Ok(part) => {
                     self.buffer.clear();
                     self.parts.push(part);
                 }
                 Err(e) => {
                     return Err(e);
                 }
             }
         }
 
-        let resp = self
-            .core
-            .s3_complete_multipart_upload(&self.path, upload_id, &self.parts)
-            .await?;
-
-        let status = resp.status();
+        self.inner.complete_part(upload_id, &self.parts).await
+    }
 
-        match status {
-            StatusCode::OK => {
-                resp.into_body().consume().await?;
+    async fn abort(&mut self) -> Result<()> {
+        let upload_id = if let Some(upload_id) = &self.upload_id {
+            upload_id
+        } else {
+            return Ok(());
+        };
 
-                Ok(())
-            }
-            _ => Err(parse_error(resp).await?),
-        }
+        self.inner.abort_part(upload_id).await
     }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sftp/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/sftp/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sftp/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/utils.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sftp/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -25,39 +25,39 @@
 use futures::AsyncRead;
 use futures::AsyncSeek;
 use openssh_sftp_client::file::File;
 use openssh_sftp_client::file::TokioCompatFile;
 use openssh_sftp_client::metadata::MetaData as SftpMeta;
 
 use crate::raw::oio;
-use crate::raw::oio::into_reader::FdReader;
+use crate::raw::oio::FromFileReader;
 use crate::raw::oio::ReadExt;
 use crate::EntryMode;
 use crate::Metadata;
 use crate::Result;
 
 pub struct SftpReaderInner {
     file: Pin<Box<Compat<TokioCompatFile>>>,
 }
-pub type SftpReader = FdReader<SftpReaderInner>;
+pub type SftpReader = FromFileReader<SftpReaderInner>;
 
 impl SftpReaderInner {
     pub async fn new(file: File) -> Self {
         let file = Compat::new(file.into());
         Self {
             file: Box::pin(file),
         }
     }
 }
 
 impl SftpReader {
     /// Create a new reader from a file, starting at the given offset and ending at the given offset.
     pub async fn new(file: File, start: u64, end: u64) -> Result<Self> {
         let file = SftpReaderInner::new(file).await;
-        let mut r = oio::into_reader::from_fd(file, start, end);
+        let mut r = oio::into_read_from_file(file, start, end);
         r.seek(SeekFrom::Start(0)).await?;
         Ok(r)
     }
 }
 
 impl AsyncRead for SftpReaderInner {
     fn poll_read(
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sled/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/sled/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/supabase/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/supabase/error.rs`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,17 @@
     let (message, _) = from_slice::<SupabaseError>(&bs)
         .map(|sb_err| {
             (kind, retryable) = parse_supabase_error(&sb_err);
             (format!("{sb_err:?}"), Some(sb_err))
         })
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/supabase/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/supabase/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs`

 * *Files 20% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::VercelArtifacts)
             .set_capability(Capability {
+                stat: true,
+
                 read: true,
                 read_can_next: true,
 
                 write: true,
 
                 ..Default::default()
             });
@@ -91,23 +93,45 @@
         }
 
         Ok((
             RpWrite::default(),
             VercelArtifactsWriter::new(self.clone(), args, path.to_string()),
         ))
     }
+
+    async fn stat(&self, path: &str, _args: OpStat) -> Result<RpStat> {
+        if (path == "/") || (path.ends_with('/')) {
+            return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
+        }
+
+        let res = self.vercel_artifacts_stat(path).await?;
+
+        let status = res.status();
+
+        match status {
+            StatusCode::OK => {
+                let meta = parse_into_metadata(path, res.headers())?;
+                Ok(RpStat::new(meta))
+            }
+
+            _ => Err(parse_error(res).await?),
+        }
+    }
 }
 
 impl VercelArtifactsBackend {
     async fn vercel_artifacts_get(
         &self,
-        path: &str,
+        hash: &str,
         args: OpRead,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let url: String = format!("https://api.vercel.com/v8/artifacts/{}", path);
+        let url: String = format!(
+            "https://api.vercel.com/v8/artifacts/{}",
+            percent_encode_path(hash)
+        );
 
         let mut req = Request::get(&url);
 
         if !args.range().is_full() {
             req = req.header(header::RANGE, args.range().to_header());
         }
 
@@ -123,22 +147,43 @@
 
     pub async fn vercel_artifacts_put(
         &self,
         hash: &str,
         size: u64,
         body: AsyncBody,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let url = format!("https://api.vercel.com/v8/artifacts/{}", hash);
+        let url = format!(
+            "https://api.vercel.com/v8/artifacts/{}",
+            percent_encode_path(hash)
+        );
 
         let mut req = Request::put(&url);
 
         let auth_header_content = format!("Bearer {}", self.access_token);
-        // Borrowed from [vercel/remote-cache](https://github.com/vercel/remote-cache/blob/46cbc71346c84ec6c3022ec660ade52a25a20013/packages/remote/src/artifact-request.ts#LL41C34-L41C58)
         req = req.header(header::CONTENT_TYPE, "application/octet-stream");
         req = req.header(header::AUTHORIZATION, auth_header_content);
         req = req.header(header::CONTENT_LENGTH, size);
 
         let req = req.body(body).map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
+
+    pub async fn vercel_artifacts_stat(&self, hash: &str) -> Result<Response<IncomingAsyncBody>> {
+        let url = format!(
+            "https://api.vercel.com/v8/artifacts/{}",
+            percent_encode_path(hash)
+        );
+
+        let mut req = Request::head(&url);
+
+        let auth_header_content = format!("Bearer {}", self.access_token);
+        req = req.header(header::AUTHORIZATION, auth_header_content);
+        req = req.header(header::CONTENT_LENGTH, 0);
+
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.client.send(req).await
+    }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/onedrive/error.rs`

 * *Files 11% similar despite different names*

```diff
@@ -34,16 +34,19 @@
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-        .with_context("response", format!("{parts:?}"));
+    let message = String::from_utf8_lossy(&bs);
+
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 use http::StatusCode;
 use log::debug;
 use md5::Digest;
 use md5::Md5;
 use once_cell::sync::Lazy;
 use reqsign::AwsConfig;
 use reqsign::AwsCredentialLoad;
-use reqsign::AwsLoader;
+use reqsign::AwsDefaultLoader;
 use reqsign::AwsV4Signer;
 
 use super::core::*;
 use super::error::parse_error;
 use super::error::parse_wasabi_error_code;
 use super::pager::WasabiPager;
 use super::writer::WasabiWriter;
@@ -850,21 +850,18 @@
         let region = cfg.region.to_owned().unwrap();
         debug!("backend use region: {region}");
 
         // Building endpoint.
         let endpoint = self.build_endpoint(&region);
         debug!("backend use endpoint: {endpoint}");
 
-        let mut loader = AwsLoader::new(client.client(), cfg);
+        let mut loader = AwsDefaultLoader::new(client.client(), cfg);
         if self.disable_ec2_metadata {
             loader = loader.with_disable_ec2_metadata();
         }
-        if let Some(v) = self.customed_credential_load.take() {
-            loader = loader.with_customed_credential_loader(v);
-        }
 
         let signer = AwsV4Signer::new("s3", &region);
 
         debug!("backend build finished");
         Ok(WasabiBackend {
             core: Arc::new(WasabiCore {
                 bucket: bucket.to_string(),
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 
 use bytes::Bytes;
 use http::header::HeaderName;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::header::IF_MATCH;
+use http::header::IF_NONE_MATCH;
 use http::HeaderValue;
 use http::Request;
 use http::Response;
 use reqsign::AwsCredential;
-use reqsign::AwsLoader;
+use reqsign::AwsCredentialLoad;
 use reqsign::AwsV4Signer;
 use serde::Deserialize;
 use serde::Serialize;
 
 use crate::raw::*;
 use crate::*;
 
@@ -49,68 +51,69 @@
         "x-amz-server-side-encryption-customer-key";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-server-side-encryption-customer-key-md5";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_AWS_KMS_KEY_ID: &str =
         "x-amz-server-side-encryption-aws-kms-key-id";
     pub const X_AMZ_STORAGE_CLASS: &str = "x-amz-storage-class";
 
-    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_ALGORITHM: &str =
         "x-amz-copy-source-server-side-encryption-customer-algorithm";
-    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY: &str =
         "x-amz-copy-source-server-side-encryption-customer-key";
-    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-copy-source-server-side-encryption-customer-key-md5";
 
     pub const RESPONSE_CONTENT_DISPOSITION: &str = "response-content-disposition";
+    pub const RESPONSE_CONTENT_TYPE: &str = "response-content-type";
     pub const RESPONSE_CACHE_CONTROL: &str = "response-cache-control";
-
-    pub const DESTINATION: &str = "Destination";
-    pub const OVERWRITE: &str = "Overwrite";
 }
 
-pub struct WasabiCore {
+pub struct S3Core {
     pub bucket: String,
     pub endpoint: String,
     pub root: String,
     pub server_side_encryption: Option<HeaderValue>,
     pub server_side_encryption_aws_kms_key_id: Option<HeaderValue>,
     pub server_side_encryption_customer_algorithm: Option<HeaderValue>,
     pub server_side_encryption_customer_key: Option<HeaderValue>,
     pub server_side_encryption_customer_key_md5: Option<HeaderValue>,
     pub default_storage_class: Option<HeaderValue>,
+    pub allow_anonymous: bool,
 
     pub signer: AwsV4Signer,
-    pub loader: AwsLoader,
+    pub loader: Box<dyn AwsCredentialLoad>,
     pub client: HttpClient,
+    pub write_min_size: usize,
+    pub batch_max_operations: usize,
 }
 
-impl Debug for WasabiCore {
+impl Debug for S3Core {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
-        f.debug_struct("WasabiCore")
+        f.debug_struct("S3Core")
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .field("root", &self.root)
             .finish_non_exhaustive()
     }
 }
 
-impl WasabiCore {
+impl S3Core {
     /// If credential is not found, we will not sign the request.
     async fn load_credential(&self) -> Result<Option<AwsCredential>> {
         let cred = self
             .loader
-            .load()
+            .load_credential(self.client.client())
             .await
             .map_err(new_request_credential_error)?;
 
         if let Some(cred) = cred {
             Ok(Some(cred))
+        } else if self.allow_anonymous {
+            // If allow_anonymous has been set, we will not sign the request.
+            Ok(None)
         } else {
             // Mark this error as temporary since it could be caused by AWS STS.
             Err(Error::new(
                 ErrorKind::PermissionDenied,
                 "no valid credential found, please check configuration or try again",
             )
             .set_temporary())
@@ -202,110 +205,118 @@
             )
         }
 
         req
     }
 }
 
-impl WasabiCore {
-    pub fn head_object_request(&self, path: &str, args: &OpStat) -> Result<Request<AsyncBody>> {
+impl S3Core {
+    pub fn s3_head_object_request(
+        &self,
+        path: &str,
+        if_none_match: Option<&str>,
+        if_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
         req = self.insert_sse_headers(req, false);
 
-        if let Some(v) = args.if_match() {
-            req = req.header(http::header::IF_MATCH, v);
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
-        if let Some(v) = args.if_none_match() {
-            req = req.header(http::header::IF_NONE_MATCH, v);
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub fn get_object_request(
-        &self,
-        path: &str,
-        range: BytesRange,
-        override_content_disposition: Option<&str>,
-        override_cache_control: Option<&str>,
-        if_none_match: Option<&str>,
-    ) -> Result<Request<AsyncBody>> {
+    pub fn s3_get_object_request(&self, path: &str, args: OpRead) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         // Construct headers to add to the request
         let mut url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         // Add query arguments to the URL based on response overrides
         let mut query_args = Vec::new();
-        if let Some(override_content_disposition) = override_content_disposition {
+        if let Some(override_content_disposition) = args.override_content_disposition() {
             query_args.push(format!(
                 "{}={}",
                 constants::RESPONSE_CONTENT_DISPOSITION,
                 percent_encode_path(override_content_disposition)
             ))
         }
-        if let Some(override_cache_control) = override_cache_control {
+        if let Some(override_content_type) = args.override_content_type() {
+            query_args.push(format!(
+                "{}={}",
+                constants::RESPONSE_CONTENT_TYPE,
+                percent_encode_path(override_content_type)
+            ))
+        }
+        if let Some(override_cache_control) = args.override_cache_control() {
             query_args.push(format!(
                 "{}={}",
                 constants::RESPONSE_CACHE_CONTROL,
                 percent_encode_path(override_cache_control)
             ))
         }
         if !query_args.is_empty() {
             url.push_str(&format!("?{}", query_args.join("&")));
         }
 
         let mut req = Request::get(&url);
 
+        let range = args.range();
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header());
         }
 
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
+        if let Some(if_none_match) = args.if_none_match() {
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
+        if let Some(if_match) = args.if_match() {
+            req = req.header(IF_MATCH, if_match);
+        }
         // Set SSE headers.
         // TODO: how will this work with presign?
         req = self.insert_sse_headers(req, false);
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn get_object(
+    pub async fn s3_get_object(
         &self,
         path: &str,
-        range: BytesRange,
-        if_none_match: Option<&str>,
+        args: OpRead,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.get_object_request(path, range, None, None, if_none_match)?;
+        let mut req = self.s3_get_object_request(path, args)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn put_object_request(
+    pub fn s3_put_object_request(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
@@ -339,41 +350,46 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn head_object(
+    pub async fn s3_head_object(
         &self,
         path: &str,
-        args: &OpStat,
+        if_none_match: Option<&str>,
+        if_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.head_object_request(path, args)?;
+        let mut req = self.s3_head_object_request(path, if_none_match, if_match)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn s3_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn copy_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn s3_copy_object(
+        &self,
+        from: &str,
+        to: &str,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let from = build_abs_path(&self.root, from);
         let to = build_abs_path(&self.root, to);
 
         let source = format!("{}/{}", self.bucket, percent_encode_path(&from));
         let target = format!("{}/{}", self.endpoint, percent_encode_path(&to));
 
         let mut req = Request::put(&target);
@@ -423,33 +439,40 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    /// Make this functions as `pub(suber)` because `DirStream` depends
-    /// on this.
-    pub async fn list_objects(
+    pub async fn s3_list_objects(
         &self,
         path: &str,
         continuation_token: &str,
         delimiter: &str,
         limit: Option<usize>,
+        start_after: Option<String>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let mut url = format!(
-            "{}?list-type=2&delimiter={delimiter}&prefix={}",
-            self.endpoint,
-            percent_encode_path(&p)
-        );
+        let mut url = format!("{}?list-type=2", self.endpoint);
+        if !p.is_empty() {
+            write!(url, "&prefix={}", percent_encode_path(&p))
+                .expect("write into string must succeed");
+        }
+        if !delimiter.is_empty() {
+            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
+        }
         if let Some(limit) = limit {
             write!(url, "&max-keys={limit}").expect("write into string must succeed");
         }
+        if let Some(start_after) = start_after {
+            let start_after = build_abs_path(&self.root, &start_after);
+            write!(url, "&start-after={}", percent_encode_path(&start_after))
+                .expect("write into string must succeed");
+        }
         if !continuation_token.is_empty() {
             // AWS S3 could return continuation-token that contains `=`
             // which could lead `reqsign` parse query wrongly.
             // URL encode continuation-token before starting signing so that
             // our signer will not be confused.
             write!(
                 url,
@@ -464,15 +487,15 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn initiate_multipart_upload(
+    pub async fn s3_initiate_multipart_upload(
         &self,
         path: &str,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
@@ -506,52 +529,50 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn upload_part_request(
+    pub fn s3_upload_part_request(
         &self,
         path: &str,
         upload_id: &str,
         part_number: usize,
-        size: Option<u64>,
+        size: u64,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/{}?partNumber={}&uploadId={}",
             self.endpoint,
             percent_encode_path(&p),
             part_number,
             percent_encode_path(upload_id)
         );
 
         let mut req = Request::put(&url);
 
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size);
-        }
+        req = req.header(CONTENT_LENGTH, size);
 
         // Set SSE headers.
         req = self.insert_sse_headers(req, true);
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn complete_multipart_upload(
+    pub async fn s3_complete_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
-        parts: &[CompleteMultipartUploadRequestPart],
+        parts: Vec<CompleteMultipartUploadRequestPart>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/{}?uploadId={}",
             self.endpoint,
             percent_encode_path(&p),
@@ -559,18 +580,16 @@
         );
 
         let req = Request::post(&url);
 
         // Set SSE headers.
         let req = self.insert_sse_headers(req, true);
 
-        let content = quick_xml::se::to_string(&CompleteMultipartUploadRequest {
-            part: parts.to_vec(),
-        })
-        .map_err(new_xml_deserialize_error)?;
+        let content = quick_xml::se::to_string(&CompleteMultipartUploadRequest { part: parts })
+            .map_err(new_xml_deserialize_error)?;
         // Make sure content length has been set to avoid post with chunked encoding.
         let req = req.header(CONTENT_LENGTH, content.len());
         // Set content-type to `application/xml` to avoid mixed with form post.
         let req = req.header(CONTENT_TYPE, "application/xml");
 
         let mut req = req
             .body(AsyncBody::Bytes(Bytes::from(content)))
@@ -578,15 +597,15 @@
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     /// Abort an on-going multipart upload.
-    pub async fn abort_multipart_upload(
+    pub async fn s3_abort_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
@@ -599,15 +618,18 @@
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn delete_objects(&self, paths: Vec<String>) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn s3_delete_objects(
+        &self,
+        paths: Vec<String>,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let url = format!("{}/?delete", self.endpoint);
 
         let req = Request::post(&url);
 
         let content = quick_xml::se::to_string(&DeleteObjectsRequest {
             object: paths
                 .into_iter()
@@ -629,90 +651,14 @@
             .body(AsyncBody::Bytes(Bytes::from(content)))
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
-
-    pub async fn put_object(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        content_disposition: Option<&str>,
-        cache_control: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.put_object_request(
-            path,
-            size,
-            content_type,
-            content_disposition,
-            cache_control,
-            body,
-        )?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
-
-    pub async fn rename_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
-        let from = percent_encode_path(build_abs_path(&self.root, from).as_str());
-        let to = percent_encode_path(build_abs_path(&self.root, to).as_str());
-
-        let url = format!("{}/{}", self.endpoint, from);
-
-        let mut req = Request::builder().method("MOVE").uri(url);
-
-        // Set SSE headers.
-        req = self.insert_sse_headers(req, true);
-
-        let mut req = req
-            .header(constants::DESTINATION, to)
-            .header(constants::OVERWRITE, "true")
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
-
-    pub async fn append_object(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        body: AsyncBody,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}?append", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::put(&url);
-
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
-        }
-
-        // Set storage class header
-        if let Some(v) = &self.default_storage_class {
-            req = req.header(HeaderName::from_static(constants::X_AMZ_STORAGE_CLASS), v);
-        }
-
-        // Set SSE headers.
-        req = self.insert_sse_headers(req, true);
-
-        let mut req = req.body(body).map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
 }
 
 /// Result of CreateMultipartUpload
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
 pub struct InitiateMultipartUploadResult {
     pub upload_id: String,
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         .map(|err| (format!("{err:?}"), Some(err)))
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
     if let Some(wasabi_err) = wasabi_err {
         (kind, retryable) = parse_wasabi_error_code(&wasabi_err.code).unwrap_or((kind, retryable));
     }
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::WasabiBuilder as Wasabi;
+pub use backend::WebhdfsBuilder as Webhdfs;
 
-mod core;
 mod error;
+mod message;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs`

 * *Files 15% similar despite different names*

```diff
@@ -27,25 +27,26 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        // Allowing retry for resource locked.
-        StatusCode::LOCKED => (ErrorKind::Unexpected, true),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-        .with_context("response", format!("{parts:?}"));
+    let message = String::from_utf8_lossy(&bs);
+
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.39.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.39.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/docs.md` & `opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     };
 
     let message = match serde_json::from_str::<WebHdfsErrorWrapper>(body) {
         Ok(wh_error) => format!("{:?}", wh_error.remote_exception),
         Err(_) => body.to_owned(),
     };
 
-    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+    let mut err = Error::new(kind, &message);
+
+    err = with_error_response_context(err, parts);
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
@@ -77,15 +79,14 @@
 #[cfg(test)]
 mod tests {
     use bytes::Buf;
     use futures::stream;
     use serde_json::from_reader;
 
     use super::*;
-    use crate::raw::oio::into_stream;
 
     /// Error response example from https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Error%20Responses
     #[tokio::test]
     async fn test_parse_error() -> Result<()> {
         let ill_args = bytes::Bytes::from(
             r#"
 {
@@ -95,17 +96,15 @@
     "javaClassName": "java.lang.IllegalArgumentException",
     "message"      : "Invalid value for webhdfs parameter \"permission\": ..."
   }
 }
     "#,
         );
         let body = IncomingAsyncBody::new(
-            Box::new(into_stream::from_futures_stream(stream::iter(vec![Ok(
-                ill_args.clone(),
-            )]))),
+            Box::new(oio::into_stream(stream::iter(vec![Ok(ill_args.clone())]))),
             None,
         );
         let resp = Response::builder()
             .status(StatusCode::BAD_REQUEST)
             .body(body)
             .unwrap();
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/append/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,9 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-mod backend;
-pub use backend::WebhdfsBuilder as Webhdfs;
-
-mod error;
-mod message;
-mod pager;
-mod writer;
+mod api;
+pub use api::*;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.39.0/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/appender.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/capability.rs`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     pub read_with_if_match: bool,
     /// If operator supports read with if none match natively, it will be true.
     pub read_with_if_none_match: bool,
     /// if operator supports read with override cache control natively, it will be true.
     pub read_with_override_cache_control: bool,
     /// if operator supports read with override content disposition natively, it will be true.
     pub read_with_override_content_disposition: bool,
+    /// if operator supports read with override content type natively, it will be true.
+    pub read_with_override_content_type: bool,
 
     /// If operator supports write natively, it will be true.
     pub write: bool,
     /// If operator supports write by sink a stream into, it will be true.
     pub write_can_sink: bool,
     /// If operator supports write with without content length, it will
     /// be true.
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/error.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/error.rs`

 * *Files 1% similar despite different names*

```diff
@@ -343,14 +343,15 @@
 }
 
 impl From<Error> for io::Error {
     fn from(err: Error) -> Self {
         let kind = match err.kind() {
             ErrorKind::NotFound => io::ErrorKind::NotFound,
             ErrorKind::PermissionDenied => io::ErrorKind::PermissionDenied,
+            ErrorKind::InvalidInput => io::ErrorKind::InvalidInput,
             _ => io::ErrorKind::Other,
         };
 
         io::Error::new(kind, err)
     }
 }
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/list.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files 25% similar despite different names*

```diff
@@ -11,53 +11,24 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-mod mode;
-pub use mode::EntryMode;
-
-mod entry;
-pub use entry::Entry;
-
-mod metadata;
-pub use metadata::Metadata;
-pub use metadata::Metakey;
-
-mod reader;
-pub use reader::BlockingReader;
-pub use reader::Reader;
-
-mod writer;
-pub use writer::BlockingWriter;
-pub use writer::Writer;
-
-mod appender;
-pub use appender::Appender;
-
-mod list;
-pub use list::BlockingLister;
-pub use list::Lister;
+//! Operator's API will be split into different mods.
 
+#[allow(clippy::module_inception)]
 mod operator;
-pub use operator::operator_functions;
-pub use operator::operator_futures;
-pub use operator::BlockingOperator;
 pub use operator::Operator;
-pub use operator::OperatorBuilder;
-pub use operator::OperatorInfo;
 
-mod builder;
-pub use builder::Builder;
+mod blocking_operator;
+pub use blocking_operator::BlockingOperator;
 
-mod error;
-pub use error::Error;
-pub use error::ErrorKind;
-pub use error::Result;
+mod builder;
+pub use builder::OperatorBuilder;
 
-mod scheme;
-pub use scheme::Scheme;
+mod metadata;
+pub use metadata::OperatorInfo;
 
-mod capability;
-pub use capability::Capability;
+pub mod operator_functions;
+pub mod operator_futures;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,16 @@
     /// ```no_run
     /// # use anyhow::Result;
     /// # use futures::io;
     /// # use opendal::BlockingOperator;
     /// # fn test(op: BlockingOperator) -> Result<()> {
     /// let _ = op
     ///     .delete_with("path/to/file")
-    ///     .version("example_version").call()?;
+    ///     .version("example_version")
+    ///     .call()?;
     /// # Ok(())
     /// # }
     /// ```
     pub fn delete_with(&self, path: &str) -> FunctionDelete {
         let path = normalize_path(path);
 
         FunctionDelete(OperatorFunction::new(
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,16 @@
             Scheme::Azdfs => Self::from_map::<services::Azdfs>(map)?.finish(),
             #[cfg(feature = "services-cacache")]
             Scheme::Cacache => Self::from_map::<services::Cacache>(map)?.finish(),
             #[cfg(feature = "services-cos")]
             Scheme::Cos => Self::from_map::<services::Cos>(map)?.finish(),
             #[cfg(feature = "services-dashmap")]
             Scheme::Dashmap => Self::from_map::<services::Dashmap>(map)?.finish(),
+            #[cfg(feature = "services-etcd")]
+            Scheme::Etcd => Self::from_map::<services::Etcd>(map)?.finish(),
             #[cfg(feature = "services-fs")]
             Scheme::Fs => Self::from_map::<services::Fs>(map)?.finish(),
             #[cfg(feature = "services-ftp")]
             Scheme::Ftp => Self::from_map::<services::Ftp>(map)?.finish(),
             #[cfg(feature = "services-gcs")]
             Scheme::Gcs => Self::from_map::<services::Gcs>(map)?.finish(),
             #[cfg(feature = "services-ghac")]
@@ -191,14 +193,16 @@
             Scheme::Obs => Self::from_map::<services::Obs>(map)?.finish(),
             #[cfg(feature = "services-onedrive")]
             Scheme::Onedrive => Self::from_map::<services::Onedrive>(map)?.finish(),
             #[cfg(feature = "services-gdrive")]
             Scheme::Gdrive => Self::from_map::<services::Gdrive>(map)?.finish(),
             #[cfg(feature = "services-oss")]
             Scheme::Oss => Self::from_map::<services::Oss>(map)?.finish(),
+            #[cfg(feature = "services-persy")]
+            Scheme::Persy => Self::from_map::<services::Persy>(map)?.finish(),
             #[cfg(feature = "services-redis")]
             Scheme::Redis => Self::from_map::<services::Redis>(map)?.finish(),
             #[cfg(feature = "services-rocksdb")]
             Scheme::Rocksdb => Self::from_map::<services::Rocksdb>(map)?.finish(),
             #[cfg(feature = "services-s3")]
             Scheme::S3 => Self::from_map::<services::S3>(map)?.finish(),
             #[cfg(feature = "services-sftp")]
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.39.0/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -11,24 +11,35 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! Operator's API will be split into different mods.
+//! `oio` provides OpenDAL's raw traits and types that opendal returns as
+//! output.
+//!
+//! Those types should only be used internally and we don't want users to
+//! depend on them. So we should also implement trait like `AsyncRead` for
+//! our `output` traits.
+
+mod read;
+pub use read::*;
+
+mod write;
+pub use write::*;
+
+mod append;
+pub use append::*;
+
+mod stream;
+pub use stream::*;
+
+mod page;
+pub use page::*;
+
+mod cursor;
+pub use cursor::Cursor;
+pub use cursor::VectorCursor;
 
-#[allow(clippy::module_inception)]
-mod operator;
-pub use operator::Operator;
-
-mod blocking_operator;
-pub use blocking_operator::BlockingOperator;
-
-mod builder;
-pub use builder::OperatorBuilder;
-
-mod metadata;
-pub use metadata::OperatorInfo;
-
-pub mod operator_functions;
-pub mod operator_futures;
+mod entry;
+pub use entry::Entry;
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_functions.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/operator/operator_functions.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_futures.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/operator/operator_futures.rs`

 * *Files 3% similar despite different names*

```diff
@@ -247,14 +247,22 @@
     pub fn override_cache_control(mut self, v: &str) -> Self {
         self.0 = self
             .0
             .map_args(|(args, dur)| (args.with_override_cache_control(v), dur));
         self
     }
 
+    /// Sets the content-type header that should be send back by the remote read operation.
+    pub fn override_content_type(mut self, v: &str) -> Self {
+        self.0 = self
+            .0
+            .map_args(|(args, dur)| (args.with_override_content_type(v), dur));
+        self
+    }
+
     /// Set the If-Match of the option
     pub fn if_match(mut self, v: &str) -> Self {
         self.0 = self.0.map_args(|(args, dur)| (args.with_if_match(v), dur));
         self
     }
 
     /// Set the If-None-Match of the option
@@ -348,14 +356,22 @@
     pub fn override_cache_control(mut self, cache_control: &str) -> Self {
         self.0 = self
             .0
             .map_args(|args| args.with_override_cache_control(cache_control));
         self
     }
 
+    /// Sets the content-type header that should be send back by the remote read operation.
+    pub fn override_content_type(mut self, content_type: &str) -> Self {
+        self.0 = self
+            .0
+            .map_args(|args| args.with_override_content_type(content_type));
+        self
+    }
+
     /// Set the If-Match for this operation.
     pub fn if_match(mut self, v: &str) -> Self {
         self.0 = self.0.map_args(|args| args.with_if_match(v));
         self
     }
 
     /// Set the If-None-Match for this operation.
@@ -403,14 +419,22 @@
     pub fn override_cache_control(mut self, cache_control: &str) -> Self {
         self.0 = self
             .0
             .map_args(|args| args.with_override_cache_control(cache_control));
         self
     }
 
+    /// Sets the content-type header that should be send back by the remote read operation.
+    pub fn override_content_type(mut self, content_type: &str) -> Self {
+        self.0 = self
+            .0
+            .map_args(|args| args.with_override_content_type(content_type));
+        self
+    }
+
     /// Set the If-Match for this operation.
     pub fn if_match(mut self, v: &str) -> Self {
         self.0 = self.0.map_args(|args| args.with_if_match(v));
         self
     }
 
     /// Set the If-None-Match for this operation.
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

```diff
@@ -204,15 +204,15 @@
             ));
         };
 
         let r = if acc_meta.capability().read_can_next {
             r
         } else {
             // Make this capacity configurable.
-            Box::new(oio::into_streamable_reader(r, 256 * 1024))
+            Box::new(oio::into_streamable_read(r, 256 * 1024))
         };
 
         Ok(BlockingReader { inner: r })
     }
 }
 
 impl oio::BlockingRead for BlockingReader {
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/scheme.rs`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     Azdfs,
     /// [cacache][crate::services::Cacache]: cacache backend support.
     Cacache,
     /// [cos][crate::services::Cos]: Tencent Cloud Object Storage services.
     Cos,
     /// [dashmap][crate::services::Dashmap]: dashmap backend support.
     Dashmap,
+    /// [etcd][crate::services::Etcd]: Etcd Services
+    Etcd,
     /// [fs][crate::services::Fs]: POSIX alike file system.
     Fs,
     /// [ftp][crate::services::Ftp]: FTP backend.
     Ftp,
     /// [gcs][crate::services::Gcs]: Google Cloud Storage backend.
     Gcs,
     /// [ghac][crate::services::Ghac]: GitHub Action Cache services.
@@ -72,14 +74,16 @@
     Onedrive,
     /// [gdrive][crate::services::Gdrive]: GoogleDrive services.
     Gdrive,
     /// [dropbox][crate::services::Dropbox]: Dropbox services.
     Dropbox,
     /// [oss][crate::services::Oss]: Aliyun Object Storage Services
     Oss,
+    /// [persy][crate::services::Persy]: persy backend support.
+    Persy,
     /// [redis][crate::services::Redis]: Redis services
     Redis,
     /// [rocksdb][crate::services::Rocksdb]: RocksDB services
     Rocksdb,
     /// [s3][crate::services::S3]: AWS S3 alike services.
     S3,
     /// [sftp][crate::services::Sftp]: SFTP services
@@ -94,14 +98,16 @@
     Wasabi,
     /// [webdav][crate::services::Webdav]: WebDAV support.
     Webdav,
     /// [webhdfs][crate::services::Webhdfs]: WebHDFS RESTful API Services
     Webhdfs,
     /// [redb][crate::services::Redb]: Redb Services
     Redb,
+    /// [tikv][crate::services::tikv]: Tikv Services
+    Tikv,
     /// Custom that allow users to implement services outside of OpenDAL.
     ///
     /// # NOTE
     ///
     /// - Custom must not overwrite any existing services name.
     /// - Custom must be lowed cases.
     Custom(&'static str),
@@ -133,27 +139,29 @@
         let s = s.to_lowercase();
         match s.as_str() {
             "azblob" => Ok(Scheme::Azblob),
             "azdfs" => Ok(Scheme::Azdfs),
             "cacache" => Ok(Scheme::Cacache),
             "cos" => Ok(Scheme::Cos),
             "dashmap" => Ok(Scheme::Dashmap),
+            "etcd" => Ok(Scheme::Etcd),
             "fs" => Ok(Scheme::Fs),
             "gcs" => Ok(Scheme::Gcs),
             "ghac" => Ok(Scheme::Ghac),
             "hdfs" => Ok(Scheme::Hdfs),
             "http" | "https" => Ok(Scheme::Http),
             "ftp" | "ftps" => Ok(Scheme::Ftp),
             "ipfs" | "ipns" => Ok(Scheme::Ipfs),
             "ipmfs" => Ok(Scheme::Ipmfs),
             "memcached" => Ok(Scheme::Memcached),
             "memory" => Ok(Scheme::Memory),
             "mini_moka" => Ok(Scheme::MiniMoka),
             "moka" => Ok(Scheme::Moka),
             "obs" => Ok(Scheme::Obs),
+            "persy" => Ok(Scheme::Persy),
             "redis" => Ok(Scheme::Redis),
             "rocksdb" => Ok(Scheme::Rocksdb),
             "s3" => Ok(Scheme::S3),
             "sled" => Ok(Scheme::Sled),
             "supabase" => Ok(Scheme::Supabase),
             "oss" => Ok(Scheme::Oss),
             "vercel_artifacts" => Ok(Scheme::VercelArtifacts),
@@ -169,42 +177,45 @@
     fn from(v: Scheme) -> Self {
         match v {
             Scheme::Azblob => "azblob",
             Scheme::Azdfs => "azdfs",
             Scheme::Cacache => "cacache",
             Scheme::Cos => "cos",
             Scheme::Dashmap => "dashmap",
+            Scheme::Etcd => "etcd",
             Scheme::Fs => "fs",
             Scheme::Gcs => "gcs",
             Scheme::Ghac => "ghac",
             Scheme::Hdfs => "hdfs",
             Scheme::Http => "http",
             Scheme::Ftp => "ftp",
             Scheme::Ipfs => "ipfs",
             Scheme::Ipmfs => "ipmfs",
             Scheme::Memcached => "memcached",
             Scheme::Memory => "memory",
             Scheme::MiniMoka => "mini_moka",
             Scheme::Moka => "moka",
             Scheme::Obs => "obs",
             Scheme::Onedrive => "onedrive",
+            Scheme::Persy => "persy",
             Scheme::Gdrive => "gdrive",
             Scheme::Dropbox => "dropbox",
             Scheme::Redis => "redis",
             Scheme::Rocksdb => "rocksdb",
             Scheme::S3 => "s3",
             Scheme::Sftp => "sftp",
             Scheme::Sled => "sled",
             Scheme::Supabase => "supabase",
             Scheme::VercelArtifacts => "vercel_artifacts",
             Scheme::Oss => "oss",
             Scheme::Wasabi => "wasabi",
             Scheme::Webdav => "webdav",
             Scheme::Webhdfs => "webhdfs",
             Scheme::Redb => "redb",
+            Scheme::Tikv => "tikv",
             Scheme::Custom(v) => v,
         }
     }
 }
 
 impl From<Scheme> for String {
     fn from(v: Scheme) -> Self {
```

### Comparing `opendal-0.38.1/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.39.0/local_dependencies/opendal/src/types/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,15 @@
     /// ```
     pub async fn sink<S, T>(&mut self, size: u64, sink_from: S) -> Result<()>
     where
         S: futures::Stream<Item = Result<T>> + Send + Sync + Unpin + 'static,
         T: Into<Bytes>,
     {
         if let State::Idle(Some(w)) = &mut self.state {
-            let s = Box::new(oio::into_stream::from_futures_stream(
-                sink_from.map_ok(|v| v.into()),
-            ));
+            let s = Box::new(oio::into_stream(sink_from.map_ok(|v| v.into())));
             w.sink(size, s).await
         } else {
             unreachable!(
                 "writer state invalid while sink, expect Idle, actual {}",
                 self.state
             );
         }
@@ -153,37 +151,34 @@
     ///
     /// # Examples
     ///
     /// ```no_run
     /// use std::io::Result;
     ///
     /// use bytes::Bytes;
+    /// use futures::io::Cursor;
     /// use futures::stream;
     /// use futures::StreamExt;
     /// use opendal::Operator;
-    /// use futures::io::Cursor;
     ///
     /// #[tokio::main]
     /// async fn copy_example(op: Operator) -> Result<()> {
-    ///     let mut w = op
-    ///         .writer_with("path/to/file")
-    ///         .content_length(4096)
-    ///         .await?;
-    ///     let reader = Cursor::new(vec![0;4096]);
+    ///     let mut w = op.writer_with("path/to/file").content_length(4096).await?;
+    ///     let reader = Cursor::new(vec![0; 4096]);
     ///     w.copy(4096, reader).await?;
     ///     w.close().await?;
     ///     Ok(())
     /// }
     /// ```
     pub async fn copy<R>(&mut self, size: u64, read_from: R) -> Result<()>
     where
         R: futures::AsyncRead + Send + Sync + Unpin + 'static,
     {
         if let State::Idle(Some(w)) = &mut self.state {
-            let s = Box::new(oio::into_stream::from_futures_reader(read_from));
+            let s = Box::new(oio::into_stream_from_reader(read_from));
             w.sink(size, s).await
         } else {
             unreachable!(
                 "writer state invalid while copy, expect Idle, actual {}",
                 self.state
             );
         }
```

### Comparing `opendal-0.38.1/Cargo.toml` & `opendal-0.39.0/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.38.1"
+version= "0.39.0"
 resolver = "2"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 futures = "0.3.28"
 opendal.path = "local_dependencies/opendal"
-pyo3 = { version = "0.18", features = ["abi3-py37"] }
-pyo3-asyncio = { version = "0.18", features = ["tokio-runtime"] }
+pyo3 = { version = "0.19", features = ["abi3-py37"] }
+pyo3-asyncio = { version = "0.19", features = ["tokio-runtime"] }
 tokio = "1"
```

### Comparing `opendal-0.38.1/.gitignore` & `opendal-0.39.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/CONTRIBUTING.md` & `opendal-0.39.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/README.md` & `opendal-0.39.0/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/benchmark/README.md` & `opendal-0.39.0/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/benchmark/async_opendal_benchmark.py` & `opendal-0.39.0/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.39.0/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/examples/object.ipynb` & `opendal-0.39.0/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/pyproject.toml` & `opendal-0.39.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/python/opendal/__init__.py` & `opendal-0.39.0/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/python/opendal/__init__.pyi` & `opendal-0.39.0/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/src/asyncio.rs` & `opendal-0.39.0/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/src/layers.rs` & `opendal-0.39.0/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/src/lib.rs` & `opendal-0.39.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/tests/binding.feature` & `opendal-0.39.0/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/tests/steps/binding.py` & `opendal-0.39.0/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.1/Cargo.lock` & `opendal-0.39.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,40 @@
 dependencies = [
  "getrandom 0.2.10",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
+name = "ahash"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+ "version_check",
+]
+
+[[package]]
 name = "aho-corasick"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -110,14 +127,23 @@
 [[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
+name = "arbitrary"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2d098ff73c1ca148721f37baad5ea6a465a13f9573aba8641fbbbae8164a54e"
+dependencies = [
+ "derive_arbitrary",
+]
+
+[[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "assert-json-diff"
@@ -223,14 +249,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa24f727524730b077666307f2734b4a1a1c57acb79193127dcc8914d5242dd7"
 dependencies = [
  "event-listener",
 ]
 
 [[package]]
+name = "async-recursion"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d7d78656ba01f1b93024b7c3a0467f1608e4be67d725749fdcd7d2c7678fd7a2"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "async-std"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62565bb4402e926b29953c785397c6dc0391b7b446e45008b0049eb43cec6f5d"
 dependencies = [
  "async-channel",
  "async-global-executor",
@@ -324,14 +361,31 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "await-tree"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "325bcfc4b87d4aa36f1319b806bacc40fcefcaf43a12bd85a5a2f44fc14ce9de"
+dependencies = [
+ "coarsetime",
+ "derive_builder",
+ "flexstr",
+ "indextree",
+ "itertools",
+ "parking_lot 0.12.1",
+ "pin-project",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
 name = "awaitable"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "70af449c9a763cb655c6a1e5338b42d99c67190824ff90658c1e30be844c0775"
 dependencies = [
  "awaitable-error",
  "cfg-if",
@@ -487,15 +541,15 @@
 dependencies = [
  "bitflags 1.3.2",
  "cexpr",
  "clang-sys",
  "lazy_static",
  "lazycell",
  "peeking_take_while",
- "prettyplease",
+ "prettyplease 0.2.9",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
  "syn 2.0.23",
 ]
@@ -821,14 +875,26 @@
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
+name = "coarsetime"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a90d114103adbc625300f346d4d09dfb4ab1c4a8df6868435dd903392ecf4354"
+dependencies = [
+ "libc",
+ "once_cell",
+ "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "combine"
@@ -923,14 +989,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "crc"
+version = "3.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86ec7a15cbe22e59248fc7eadb1907dab5ba09372595da4d73dd805ed4417dfe"
+dependencies = [
+ "crc-catalog",
+]
+
+[[package]]
+name = "crc-catalog"
+version = "2.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9cace84e55f07e7301bae1c519df89cdad8cc3cd868413d3fdbdeca9ff3db484"
+
+[[package]]
 name = "crc32fast"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
@@ -999,15 +1080,15 @@
 version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.9.0",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1103,14 +1184,45 @@
 [[package]]
 name = "data-encoding"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
 
 [[package]]
+name = "dav-server"
+version = "0.5.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1c1b3c57ea8b45dc1303de4653b12e3a2742ff023a469083716feea98abfdbe"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "headers",
+ "htmlescape",
+ "http",
+ "http-body",
+ "lazy_static",
+ "libc",
+ "log",
+ "lru",
+ "mime_guess",
+ "parking_lot 0.12.1",
+ "percent-encoding",
+ "pin-project",
+ "pin-utils",
+ "regex",
+ "time 0.3.22",
+ "tokio",
+ "url",
+ "uuid",
+ "xml-rs",
+ "xmltree",
+]
+
+[[package]]
 name = "deadpool"
 version = "0.9.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "421fe0f90f2ab22016f32a9881be5134fdd71c65298917084b0c7477cbc3856e"
 dependencies = [
  "async-trait",
  "deadpool-runtime",
@@ -1122,25 +1234,84 @@
 [[package]]
 name = "deadpool-runtime"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eaa37046cc0f6c3cc6090fbdbf73ef0b8ef4cfcc37f6befc0020f63e8cf121e1"
 
 [[package]]
+name = "defer"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "647605a6345d5e89c3950a36a638c56478af9b414c55c6f2477c73b115f9acde"
+
+[[package]]
 name = "der"
 version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c7ed52955ce76b1554f509074bb357d3fb8ac9b51288a65a3fd480d1dfba946"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
+name = "derive-new"
+version = "0.5.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3418329ca0ad70234b9735dc4ceed10af4df60eff9c8e7b06cb5e520d92c3535"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "derive_arbitrary"
+version = "1.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53e0efad4403bfc52dc201159c4b842a246a14b98c64b55dfd0f2d89729dfeb8"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.23",
+]
+
+[[package]]
+name = "derive_builder"
+version = "0.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
+dependencies = [
+ "derive_builder_macro",
+]
+
+[[package]]
+name = "derive_builder_core"
+version = "0.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c11bdc11a0c47bc7d37d582b5285da6849c96681023680b906673c5707af7b0f"
+dependencies = [
+ "darling",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "derive_builder_macro"
+version = "0.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ebcda35c7a396850a55ffeac740804b40ffec779b98fffbb1738f4033f0ee79e"
+dependencies = [
+ "derive_builder_core",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "derive_destructure2"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35cb7e5875e1028a73e551747d6d0118f25c3d6dbba2dadf97cc0f4d0c53f2f5"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -1283,25 +1454,14 @@
 name = "equivalent"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88bffebc5d80432c9b140ee17875ff173a8ab62faad5b257da912bd2f6c1c0a1"
 
 [[package]]
 name = "errno"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys 0.48.0",
@@ -1323,35 +1483,77 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d2f06b9cac1506ece98fe3231e3cc9c4410ec3d5b1f24ae1c8946f0742cdefc"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
+name = "etcd-client"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4b0ea5ef6dc2388a4b1669fa32097249bc03a15417b97cb75e38afb309e4a89"
+dependencies = [
+ "http",
+ "prost",
+ "tokio",
+ "tokio-stream",
+ "tonic",
+ "tonic-build",
+ "tower",
+ "tower-service",
+]
+
+[[package]]
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
+name = "fail"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3be3c61c59fdc91f5dbc3ea31ee8623122ce80057058be560654c5d410d181a6"
+dependencies = [
+ "lazy_static",
+ "log",
+ "rand 0.7.3",
+]
+
+[[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
+name = "fixedbitset"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
+
+[[package]]
 name = "flagset"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cda653ca797810c02f7ca4b804b40b8b95ae046eb989d356bce17919a8c25499"
 
 [[package]]
+name = "flexstr"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4d50aef14619d336a54fca5a592d952eb39037b1a1e7e6afd9f91c892ac7ef65"
+dependencies = [
+ "static_assertions",
+]
+
+[[package]]
 name = "float-cmp"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
 dependencies = [
  "num-traits",
 ]
@@ -1627,40 +1829,68 @@
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 
 [[package]]
 name = "hashbrown"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+dependencies = [
+ "ahash 0.8.3",
+ "allocator-api2",
+]
 
 [[package]]
 name = "hdfs-sys"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73dcfda0dbca0569e98b8bfb87028d83d2f07705587bac1fddea7dc9ee1eca13"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "hdrs"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70a8d6dab41a27fd3825810f6413f16f15733c84114504e41955516e4156676c"
+checksum = "dd139e8f6c58950322dc73060b8c23b80be07d235dd2eaf5c7c821c1d91eb469"
 dependencies = [
- "async-lock",
  "blocking",
- "errno 0.2.8",
+ "errno",
  "futures",
  "hdfs-sys",
  "libc",
  "log",
 ]
 
 [[package]]
+name = "headers"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f3e372db8e5c0d213e0cd0b9be18be2aca3d44cf2fe30a9d46a65581cd454584"
+dependencies = [
+ "base64 0.13.1",
+ "bitflags 1.3.2",
+ "bytes",
+ "headers-core",
+ "http",
+ "httpdate",
+ "mime",
+ "sha1",
+]
+
+[[package]]
+name = "headers-core"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7f66481bfee273957b1f20485a4ff3362987f85b2c236580d81b4eb7a326429"
+dependencies = [
+ "http",
+]
+
+[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
@@ -1709,14 +1939,20 @@
 dependencies = [
  "libc",
  "match_cfg",
  "winapi",
 ]
 
 [[package]]
+name = "htmlescape"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e9025058dae765dee5070ec375f591e2ba14638c63feff74f13805a72e523163"
+
+[[package]]
 name = "http"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
@@ -1813,14 +2049,26 @@
  "hyper",
  "rustls 0.21.2",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
+name = "hyper-timeout"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bbb958482e8c7be4bc3cf272a766a2b0bf1a6755e7a6ae777f017a31d11b13b1"
+dependencies = [
+ "hyper",
+ "pin-project-lite",
+ "tokio",
+ "tokio-io-timeout",
+]
+
+[[package]]
 name = "hyper-tls"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
 dependencies = [
  "bytes",
  "hyper",
@@ -1896,14 +2144,20 @@
 checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.0",
 ]
 
 [[package]]
+name = "indextree"
+version = "4.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c40411d0e5c63ef1323c3d09ce5ec6d84d71531e18daed0743fccea279d7deb6"
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "infer"
@@ -2085,14 +2339,25 @@
 [[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
+name = "libfuzzer-sys"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "beb09950ae85a0a94b27676cccf37da5ff13f27076aa1adbc6545dd0d0e1bd4e"
+dependencies = [
+ "arbitrary",
+ "cc",
+ "once_cell",
+]
+
+[[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
  "cfg-if",
  "winapi",
@@ -2180,14 +2445,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 dependencies = [
  "value-bag",
 ]
 
 [[package]]
+name = "lru"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eedb2bdbad7e0634f83989bf596f497b070130daaa398ab22d84c39e266deec5"
+dependencies = [
+ "hashbrown 0.14.0",
+]
+
+[[package]]
 name = "lru-cache"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e24f1ad8321ca0e8a1e0ac13f23cb668e6f5466c2c57319f6a5cf1cc8e3b1c"
 dependencies = [
  "linked-hash-map",
 ]
@@ -2212,15 +2486,15 @@
 
 [[package]]
 name = "madsim"
 version = "0.2.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7777a8bc4e68878b6e5433ac7b9bc196d9ccdfeef1f7cb3d23193cb997a520c9"
 dependencies = [
- "ahash",
+ "ahash 0.7.6",
  "async-channel",
  "async-stream",
  "async-task",
  "bincode",
  "bytes",
  "downcast-rs",
  "futures-util",
@@ -2325,37 +2599,28 @@
 checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "metrics"
 version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b9b8653cec6897f73b519a43fba5ee3d50f62fe9af80b428accdcc093b4a849"
 dependencies = [
- "ahash",
+ "ahash 0.7.6",
  "metrics-macros",
  "portable-atomic 0.3.20",
 ]
 
 [[package]]
 name = "metrics-macros"
 version = "0.6.0"
@@ -2393,14 +2658,24 @@
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
+name = "mime_guess"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
+dependencies = [
+ "mime",
+ "unicase",
+]
+
+[[package]]
 name = "mini-moka"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cafc5ec7807288595f9c20c86e6ce6d262b722f61e0547fe7e6e6e6451b58d5"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-utils",
@@ -2415,31 +2690,44 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "minitrace"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "317e28b8c337ada2fd437611c241ce053d5b7f5480b79e945597996b87b1de96"
+checksum = "5bdc5c5a697f93f25a109f36988a60ce534c05b944afb8ef3c1498e131638133"
 dependencies = [
+ "defer",
  "futures",
  "minitrace-macro",
  "minstant",
  "once_cell",
  "parking_lot 0.12.1",
  "pin-project",
+ "rand 0.8.5",
+]
+
+[[package]]
+name = "minitrace-jaeger"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f3d0fff56ac16fb4acb2f64e84f36879a2cacd87553c689ef2baec02a9097da6"
+dependencies = [
+ "log",
+ "minitrace",
+ "thrift_codec",
 ]
 
 [[package]]
 name = "minitrace-macro"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77814d165883613a1846517efdc50b88fabd9c210b7ff4d3745b38b99d539652"
+checksum = "f2277f13e7d585f02062590b3496cc0ca862aefadd24888efa01d50843605b79"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
@@ -2523,14 +2811,20 @@
  "tagptr",
  "thiserror",
  "triomphe",
  "uuid",
 ]
 
 [[package]]
+name = "multimap"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
+
+[[package]]
 name = "naive-timer"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "034a0ad7deebf0c2abcf2435950a6666c3c15ea9d8fad0c0f48efa8a7f843fed"
 
 [[package]]
 name = "napi"
@@ -2724,24 +3018,26 @@
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "anyhow",
  "axum",
+ "bytes",
  "chrono",
  "clap 4.3.10",
+ "dav-server",
  "dirs 5.0.1",
  "futures",
  "opendal",
- "quick-xml 0.27.1",
+ "quick-xml",
  "serde",
  "tokio",
  "toml 0.7.5",
  "tower",
  "tower-http",
  "tracing",
  "tracing-subscriber",
@@ -2776,27 +3072,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.3.10",
  "dirs 5.0.1",
  "env_logger",
  "futures",
@@ -2819,105 +3115,126 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
+ "await-tree",
  "backon",
  "base64 0.21.2",
  "bb8",
  "bytes",
  "cacache",
  "chrono",
  "criterion",
  "dashmap",
  "dirs 5.0.1",
  "dotenvy",
+ "etcd-client",
  "flagset",
  "futures",
  "governor",
  "hdrs",
  "http",
  "hyper",
  "lazy-regex",
  "libtest-mimic",
  "log",
  "madsim",
  "md-5",
  "metrics",
  "mini-moka",
  "minitrace",
+ "minitrace-jaeger",
  "moka",
  "once_cell",
  "openssh",
  "openssh-sftp-client",
  "opentelemetry 0.19.0",
  "opentelemetry-jaeger",
  "parking_lot 0.12.1",
  "paste",
  "percent-encoding",
+ "persy",
  "pin-project",
  "pretty_assertions",
  "prometheus",
  "prost",
- "quick-xml 0.27.1",
+ "quick-xml",
  "rand 0.8.5",
  "redb",
  "redis",
  "reqsign",
  "reqwest",
  "rocksdb",
  "serde",
  "serde_json",
  "sha2",
  "size",
  "sled",
  "suppaftp",
+ "tikv-client",
  "tokio",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
  "uuid",
  "wiremock",
 ]
 
 [[package]]
 name = "opendal-c"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "bytes",
  "cbindgen",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-dotnet"
 version = "0.1.0"
 dependencies = [
  "opendal",
 ]
 
 [[package]]
+name = "opendal-fuzz"
+version = "0.0.0"
+dependencies = [
+ "anyhow",
+ "arbitrary",
+ "bytes",
+ "dotenvy",
+ "libfuzzer-sys",
+ "opendal",
+ "rand 0.8.5",
+ "sha2",
+ "tokio",
+ "uuid",
+]
+
+[[package]]
 name = "opendal-hs"
 version = "0.1.0"
 dependencies = [
  "chrono",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-java"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "anyhow",
  "jni",
  "num_cpus",
  "once_cell",
  "opendal",
  "tokio",
@@ -2929,26 +3246,26 @@
 dependencies = [
  "mlua",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.38.1"
+version = "0.39.0"
 dependencies = [
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
 ]
@@ -3337,14 +3654,40 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
+name = "persy"
+version = "1.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3712821f12453814409ec149071bd4832a8ec458e648579c104aee30ed70b300"
+dependencies = [
+ "crc",
+ "data-encoding",
+ "fs2",
+ "linked-hash-map",
+ "rand 0.8.5",
+ "thiserror",
+ "unsigned-varint",
+ "zigzag",
+]
+
+[[package]]
+name = "petgraph"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
+dependencies = [
+ "fixedbitset",
+ "indexmap 1.9.3",
+]
+
+[[package]]
 name = "pin-project"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
@@ -3505,14 +3848,24 @@
  "diff",
  "output_vt100",
  "yansi",
 ]
 
 [[package]]
 name = "prettyplease"
+version = "0.1.25"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c8646e95016a7a6c4adea95bafa8a16baab64b583356217f2c85db4a39d9a86"
+dependencies = [
+ "proc-macro2",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "prettyplease"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9825a04601d60621feed79c4e6b56d65db77cdca55cef43b46b0de1096d1c282"
 dependencies = [
  "proc-macro2",
  "syn 2.0.23",
 ]
@@ -3579,41 +3932,73 @@
  "fnv",
  "lazy_static",
  "libc",
  "memchr",
  "parking_lot 0.12.1",
  "procfs",
  "protobuf",
+ "reqwest",
  "thiserror",
 ]
 
 [[package]]
 name = "prost"
 version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
+name = "prost-build"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "119533552c9a7ffacc21e099c24a0ac8bb19c2a2a3f363de84cd9b844feab270"
+dependencies = [
+ "bytes",
+ "heck",
+ "itertools",
+ "lazy_static",
+ "log",
+ "multimap",
+ "petgraph",
+ "prettyplease 0.1.25",
+ "prost",
+ "prost-types",
+ "regex",
+ "syn 1.0.109",
+ "tempfile",
+ "which",
+]
+
+[[package]]
 name = "prost-derive"
 version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
  "itertools",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "prost-types"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "213622a1460818959ac1181aaeb2dc9c7f63df720db7d788b3e24eacd1983e13"
+dependencies = [
+ "prost",
+]
+
+[[package]]
 name = "protobuf"
 version = "2.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "106dd99e98437432fed6519dedecfade6a06a73bb7b2a1e019fdd2bee5778d94"
 
 [[package]]
 name = "pulldown-cmark"
@@ -3624,89 +4009,79 @@
  "bitflags 1.3.2",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.8.0",
+ "memoffset",
  "parking_lot 0.12.1",
- "pyo3-build-config 0.18.3",
+ "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-asyncio"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3564762e37035cfc486228e10b0528460fa026d681b5763873c693aa0d5c260"
+checksum = "a2cc34c1f907ca090d7add03dc523acdd91f3a4dab12286604951e2f5152edad"
 dependencies = [
  "futures",
  "once_cell",
  "pin-project-lite",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
-dependencies = [
- "once_cell",
- "target-lexicon",
-]
-
-[[package]]
-name = "pyo3-build-config"
 version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
- "pyo3-build-config 0.18.3",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -3745,27 +4120,17 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quick-xml"
-version = "0.27.1"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffc053f057dd768a56f62cd7e434c42c831d296968997e9ac1f76ea7c2d14c41"
-dependencies = [
- "memchr",
- "serde",
-]
-
-[[package]]
-name = "quick-xml"
-version = "0.28.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
+checksum = "81b9228215d82c7b61490fec1de287136b5de6f5700f6e58ea9ad61a7964ca51"
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quote"
@@ -3920,15 +4285,15 @@
 [[package]]
 name = "redb"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b48b6e8001eaa7ac3793fbfc7444ade76fc51efa3629dee8c66629425d39595"
 dependencies = [
  "libc",
- "pyo3-build-config 0.19.1",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "redis"
 version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3ea8c51b5dc1d8e5fd3350ec8167f464ec0995e79f2e90a075b63371500d557f"
@@ -3936,19 +4301,24 @@
  "arc-swap",
  "async-trait",
  "bytes",
  "combine",
  "futures",
  "futures-util",
  "itoa",
+ "native-tls",
  "percent-encoding",
  "pin-project-lite",
+ "rustls 0.21.2",
+ "rustls-native-certs",
  "ryu",
  "sha1_smol",
  "tokio",
+ "tokio-native-tls",
+ "tokio-rustls",
  "tokio-util",
  "url",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -4018,32 +4388,32 @@
 name = "regex-syntax"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "reqsign"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6cb65eb3405f9c2de5c18bfc37338d6bbdb2c35eb8eb0e946208cbb564e4833"
+checksum = "f88838c22f5c35c2e8d5552842427a425b34d0693189091a3607d24949894414"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "chrono",
  "form_urlencoded",
  "hex",
  "hmac",
  "home",
  "http",
  "jsonwebtoken",
  "log",
  "once_cell",
  "percent-encoding",
- "quick-xml 0.28.2",
+ "quick-xml",
  "rand 0.8.5",
  "reqwest",
  "rsa",
  "rust-ini",
  "serde",
  "serde_json",
  "sha1",
@@ -4193,43 +4563,43 @@
 [[package]]
 name = "rustix"
 version = "0.36.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14e4d67015953998ad0eb82887a0eb0129e18a7e2f3b7b0f6c422fddcd503d62"
 dependencies = [
  "bitflags 1.3.2",
- "errno 0.3.1",
+ "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys 0.1.4",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "rustix"
 version = "0.37.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8818fa822adcc98b18fedbb3632a6a33213c070556b5aa7c4c8cc21cff565c4c"
 dependencies = [
  "bitflags 1.3.2",
- "errno 0.3.1",
+ "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys 0.3.8",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustix"
 version = "0.38.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aabcb0461ebd01d6b79945797c27f8529082226cb630a9865a71870ff63532a4"
 dependencies = [
  "bitflags 2.3.3",
- "errno 0.3.1",
+ "errno",
  "libc",
  "linux-raw-sys 0.4.3",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustls"
@@ -4713,14 +5083,20 @@
 [[package]]
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
+name = "static_assertions"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
+
+[[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "subtle"
@@ -4873,14 +5249,54 @@
  "integer-encoding",
  "log",
  "ordered-float",
  "threadpool",
 ]
 
 [[package]]
+name = "thrift_codec"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fce3200b189fd4733eb2bb22235755c8aa0361ba1c66b67db54893144d147279"
+dependencies = [
+ "byteorder",
+ "trackable",
+]
+
+[[package]]
+name = "tikv-client"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e9a500ec7c937fe18b1d08720406e63f3c7e2de1d7c58d460d3dc21a6656a3b"
+dependencies = [
+ "async-recursion",
+ "async-trait",
+ "derive-new",
+ "either",
+ "fail",
+ "futures",
+ "glob",
+ "lazy_static",
+ "log",
+ "pin-project",
+ "prometheus",
+ "prost",
+ "rand 0.8.5",
+ "regex",
+ "semver",
+ "serde",
+ "serde_derive",
+ "thiserror",
+ "tokio",
+ "tonic",
+ "tonic-build",
+ "tonic-disable-doctest",
+]
+
+[[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
 dependencies = [
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
@@ -4965,14 +5381,24 @@
  "signal-hook-registry",
  "socket2 0.4.9",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "tokio-io-timeout"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30b74022ada614a1b4834de765f9bb43877f910cc8ce4be40e89042c9223a8bf"
+dependencies = [
+ "pin-project-lite",
+ "tokio",
+]
+
+[[package]]
 name = "tokio-io-utility"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d672654d175710e52c7c41f6aec77c62b3c0954e2a7ebce9049d1e94ed7c263"
 dependencies = [
  "bytes",
  "tokio",
@@ -5084,24 +5510,83 @@
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tonic"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3082666a3a6433f7f511c7192923fa1fe07c69332d3c6a2e6bb040b569199d5a"
+dependencies = [
+ "async-stream",
+ "async-trait",
+ "axum",
+ "base64 0.21.2",
+ "bytes",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-timeout",
+ "percent-encoding",
+ "pin-project",
+ "prost",
+ "rustls-pemfile",
+ "tokio",
+ "tokio-rustls",
+ "tokio-stream",
+ "tower",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "tonic-build"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6fdaae4c2c638bb70fe42803a26fbd6fc6ac8c72f5c59f67ecc2a2dcabf4b07"
+dependencies = [
+ "prettyplease 0.1.25",
+ "proc-macro2",
+ "prost-build",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "tonic-disable-doctest"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "322be90b9db8035feae8d5b26d04dd9146dc4b0eaa6dec32fc9cf68d1a29e806"
+dependencies = [
+ "convert_case",
+ "itertools",
+ "tonic-build",
+]
+
+[[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
  "futures-core",
  "futures-util",
+ "indexmap 1.9.3",
  "pin-project",
  "pin-project-lite",
+ "rand 0.8.5",
+ "slab",
  "tokio",
+ "tokio-util",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "tower-http"
@@ -5208,14 +5693,33 @@
  "thread_local",
  "tracing",
  "tracing-core",
  "tracing-log",
 ]
 
 [[package]]
+name = "trackable"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b15bd114abb99ef8cee977e517c8f37aee63f184f2d08e3e6ceca092373369ae"
+dependencies = [
+ "trackable_derive",
+]
+
+[[package]]
+name = "trackable_derive"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ebeb235c5847e2f82cfe0f07eb971d1e5f6804b18dac2ae16349cc604380f82f"
+dependencies = [
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "triomphe"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1ee9bd9239c339d714d657fac840c6d2a4f9c45f4f9ec7b0975113458be78db"
 dependencies = [
  "arc-swap",
  "serde",
@@ -5324,14 +5828,20 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "unsigned-varint"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d86a8dc7f45e4c1b0d30e43038c38f274e77af056aa5f74b93c2cf9eb3c1c836"
+
+[[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
 name = "url"
@@ -5565,14 +6075,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aabe153544e473b775453675851ecc86863d2a81d786d741f6b76778f2a48940"
 dependencies = [
  "webpki",
 ]
 
 [[package]]
+name = "which"
+version = "4.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
+dependencies = [
+ "either",
+ "libc",
+ "once_cell",
+]
+
+[[package]]
 name = "widestring"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "653f141f39ec16bba3c5abe400a0c60da7468261cc2cbf36805022876bc721a8"
 
 [[package]]
 name = "winapi"
@@ -5793,14 +6314,29 @@
  "regex",
  "serde",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
+name = "xml-rs"
+version = "0.8.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "47430998a7b5d499ccee752b41567bc3afc57e1327dc855b1a2aa44ce29b5fa1"
+
+[[package]]
+name = "xmltree"
+version = "0.10.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d7d8a75eaf6557bb84a65ace8609883db44a29951042ada9b393151532e41fcb"
+dependencies = [
+ "xml-rs",
+]
+
+[[package]]
 name = "xxhash-rust"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "735a71d46c4d68d71d4b24d03fdc2b98e38cea81730595801db779c04fe80d70"
 
 [[package]]
 name = "yansi"
@@ -5809,7 +6345,16 @@
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
 [[package]]
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
+
+[[package]]
+name = "zigzag"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "70b40401a28d86ce16a330b863b86fd7dbee4d7c940587ab09ab8c019f9e3fdf"
+dependencies = [
+ "num-traits",
+]
```

### Comparing `opendal-0.38.1/PKG-INFO` & `opendal-0.39.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.38.1
+Version: 0.39.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: gevent ; extra == 'benchmark'
 Requires-Dist: greenify ; extra == 'benchmark'
 Requires-Dist: greenlet ; extra == 'benchmark'
 Requires-Dist: boto3 ; extra == 'benchmark'
```

