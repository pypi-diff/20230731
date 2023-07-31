# Comparing `tmp/dbt-core-1.6.0rc1.tar.gz` & `tmp/dbt-core-1.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.6.0rc1.tar", last modified: Mon Jul 17 21:04:32 2023, max compression
+gzip compressed data, was "dbt-core-1.6.0rc2.tar", last modified: Fri Jul 28 23:17:11 2023, max compression
```

## Comparing `dbt-core-1.6.0rc1.tar` & `dbt-core-1.6.0rc2.tar`

### file list

```diff
@@ -1,345 +1,345 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.934350 dbt-core-1.6.0rc1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.934350 dbt-core-1.6.0rc1/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    57217 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18265 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.942350 dbt-core-1.6.0rc1/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    27182 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.942350 dbt-core-1.6.0rc1/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    60992 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.942350 dbt-core-1.6.0rc1/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55911 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    54904 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/semantic_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/semantic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    62873 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   105768 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    79543 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    30501 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/drop_relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/validate_sql.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/clone.sql
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.966350 dbt-core-1.6.0rc1/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    48426 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20475 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38427 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.966350 dbt-core-1.6.0rc1/dbt/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22958 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    19598 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.248681 dbt-core-1.6.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-28 23:17:11.244681 dbt-core-1.6.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.212681 dbt-core-1.6.0rc2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.216681 dbt-core-1.6.0rc2/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.216681 dbt-core-1.6.0rc2/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57217 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.216681 dbt-core-1.6.0rc2/dbt/adapters/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/relation_configs/config_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.216681 dbt-core-1.6.0rc2/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.216681 dbt-core-1.6.0rc2/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.220681 dbt-core-1.6.0rc2/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23444 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.220681 dbt-core-1.6.0rc2/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27182 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.220681 dbt-core-1.6.0rc2/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60992 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.220681 dbt-core-1.6.0rc2/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.224681 dbt-core-1.6.0rc2/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55911 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21703 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55230 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/semantic_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/semantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.224681 dbt-core-1.6.0rc2/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.208681 dbt-core-1.6.0rc2/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.224681 dbt-core-1.6.0rc2/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.224681 dbt-core-1.6.0rc2/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.224681 dbt-core-1.6.0rc2/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62930 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105768 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79543 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.228681 dbt-core-1.6.0rc2/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30501 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.228681 dbt-core-1.6.0rc2/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.228681 dbt-core-1.6.0rc2/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.228681 dbt-core-1.6.0rc2/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.208681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.228681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/drop_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/validate_sql.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.228681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.228681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.208681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/clone/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/clone/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.232681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.236681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.236681 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.208681 dbt-core-1.6.0rc2/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.236681 dbt-core-1.6.0rc2/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497539 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.236681 dbt-core-1.6.0rc2/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.236681 dbt-core-1.6.0rc2/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.236681 dbt-core-1.6.0rc2/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.212681 dbt-core-1.6.0rc2/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.236681 dbt-core-1.6.0rc2/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.240681 dbt-core-1.6.0rc2/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.240681 dbt-core-1.6.0rc2/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.240681 dbt-core-1.6.0rc2/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.240681 dbt-core-1.6.0rc2/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69868 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48426 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38427 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/parser/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.240681 dbt-core-1.6.0rc2/dbt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/plugins/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/plugins/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.244681 dbt-core-1.6.0rc2/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23046 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.244681 dbt-core-1.6.0rc2/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.244681 dbt-core-1.6.0rc2/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18954 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19598 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:17:11.244681 dbt-core-1.6.0rc2/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-28 23:17:11.000000 dbt-core-1.6.0rc2/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-28 23:17:11.000000 dbt-core-1.6.0rc2/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:17:11.000000 dbt-core-1.6.0rc2/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 23:17:11.000000 dbt-core-1.6.0rc2/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:17:11.000000 dbt-core-1.6.0rc2/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 23:17:11.000000 dbt-core-1.6.0rc2/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-28 23:17:11.000000 dbt-core-1.6.0rc2/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:17:11.248681 dbt-core-1.6.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-28 23:16:59.000000 dbt-core-1.6.0rc2/setup.py
```

### Comparing `dbt-core-1.6.0rc1/PKG-INFO` & `dbt-core-1.6.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0rc1
+Version: 1.6.0rc2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0rc1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0rc2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0rc1/README.md` & `dbt-core-1.6.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/__init__.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/column.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/connections.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/impl.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/meta.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/plugin.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/query_headers.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/base/relation.py` & `dbt-core-1.6.0rc2/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/cache.py` & `dbt-core-1.6.0rc2/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/factory.py` & `dbt-core-1.6.0rc2/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/protocol.py` & `dbt-core-1.6.0rc2/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/reference_keys.py` & `dbt-core-1.6.0rc2/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_base.py` & `dbt-core-1.6.0rc2/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_change.py` & `dbt-core-1.6.0rc2/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_validation.py` & `dbt-core-1.6.0rc2/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/sql/connections.py` & `dbt-core-1.6.0rc2/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/adapters/sql/impl.py` & `dbt-core-1.6.0rc2/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/cli/exceptions.py` & `dbt-core-1.6.0rc2/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/cli/flags.py` & `dbt-core-1.6.0rc2/dbt/cli/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/cli/main.py` & `dbt-core-1.6.0rc2/dbt/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 @click.pass_context
 @p.cache_selected_only
 @p.debug
 @p.deprecated_print
 @p.enable_legacy_logger
 @p.fail_fast
 @p.log_cache_events
+@p.log_file_max_bytes
 @p.log_format
 @p.log_format_file
 @p.log_level
 @p.log_level_file
 @p.log_path
 @p.macro_debugging
 @p.partial_parse
```

### Comparing `dbt-core-1.6.0rc1/dbt/cli/option_types.py` & `dbt-core-1.6.0rc2/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/cli/options.py` & `dbt-core-1.6.0rc2/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/cli/params.py` & `dbt-core-1.6.0rc2/dbt/cli/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,23 @@
 use_colors_file = click.option(
     "--use-colors-file/--no-use-colors-file",
     envvar="DBT_USE_COLORS_FILE",
     help="Specify whether log file output is colorized by overriding the default value and the general --use-colors/--no-use-colors setting.",
     default=True,
 )
 
+log_file_max_bytes = click.option(
+    "--log-file-max-bytes",
+    envvar="DBT_LOG_FILE_MAX_BYTES",
+    help="Configure the max file size in bytes for a single dbt.log file, before rolling over. 0 means no limit.",
+    default=10 * 1024 * 1024,  # 10mb
+    type=click.INT,
+    hidden=True,
+)
+
 log_path = click.option(
     "--log-path",
     envvar="DBT_LOG_PATH",
     help="Configure the 'log-path'. Only applies this setting for the current run. Overrides the 'DBT_LOG_PATH' if it is set.",
     default=None,
     type=click.Path(resolve_path=True, path_type=Path),
 )
@@ -376,17 +385,17 @@
     help="Pass SQL inline to dbt compile and show",
 )
 
 # `--select` and `--models` are analogous for most commands except `dbt list` for legacy reasons.
 # Most CLI arguments should use the combined `select` option that aliases `--models` to `--select`.
 # However, if you need to split out these separators (like `dbt ls`), use the `models` and `raw_select` options instead.
 # See https://github.com/dbt-labs/dbt-core/pull/6774#issuecomment-1408476095 for more info.
-models = click.option(*model_decls, **select_attrs)
-raw_select = click.option(*select_decls, **select_attrs)
-select = click.option(*select_decls, *model_decls, **select_attrs)
+models = click.option(*model_decls, **select_attrs)  # type: ignore[arg-type]
+raw_select = click.option(*select_decls, **select_attrs)  # type: ignore[arg-type]
+select = click.option(*select_decls, *model_decls, **select_attrs)  # type: ignore[arg-type]
 
 selector = click.option(
     "--selector",
     envvar=None,
     help="The selector name to use, as defined in selectors.yml",
 )
```

### Comparing `dbt-core-1.6.0rc1/dbt/cli/requires.py` & `dbt-core-1.6.0rc2/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/cli/resolvers.py` & `dbt-core-1.6.0rc2/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/cli/types.py` & `dbt-core-1.6.0rc2/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/_jinja_blocks.py` & `dbt-core-1.6.0rc2/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/agate_helper.py` & `dbt-core-1.6.0rc2/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/git.py` & `dbt-core-1.6.0rc2/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/jinja.py` & `dbt-core-1.6.0rc2/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/jinja_static.py` & `dbt-core-1.6.0rc2/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/registry.py` & `dbt-core-1.6.0rc2/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/system.py` & `dbt-core-1.6.0rc2/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/clients/yaml_helper.py` & `dbt-core-1.6.0rc2/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/compilation.py` & `dbt-core-1.6.0rc2/dbt/compilation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
 import json
 
 import networkx as nx  # type: ignore
 import os
 import pickle
-import sqlparse
 
 from collections import defaultdict
 from typing import List, Dict, Any, Tuple, Optional
 
 from dbt.flags import get_flags
 from dbt.adapters.factory import get_adapter
 from dbt.clients import jinja
@@ -32,14 +31,15 @@
 from dbt.events.functions import fire_event, get_invocation_id
 from dbt.events.types import FoundStats, Note, WritingInjectedSQLForNode
 from dbt.events.contextvars import get_node_info
 from dbt.node_types import NodeType, ModelLanguage
 from dbt.events.format import pluralize
 import dbt.tracking
 import dbt.task.list as list_task
+import sqlparse
 
 graph_file_name = "graph.gpickle"
 
 
 def print_compile_stats(stats):
     names = {
         NodeType.Model: "model",
@@ -374,24 +374,24 @@
 
             new_cte_name = self.add_ephemeral_prefix(cte_model.name)
             rendered_sql = cte_model._pre_injected_sql or cte_model.compiled_code
             sql = f" {new_cte_name} as (\n{rendered_sql}\n)"
 
             _add_prepended_cte(prepended_ctes, InjectedCTE(id=cte.id, sql=sql))
 
-        injected_sql = inject_ctes_into_sql(
-            model.compiled_code,
-            prepended_ctes,
-        )
         # Check again before updating for multi-threading
         if not model.extra_ctes_injected:
+            injected_sql = inject_ctes_into_sql(
+                model.compiled_code,
+                prepended_ctes,
+            )
+            model.extra_ctes_injected = True
             model._pre_injected_sql = model.compiled_code
             model.compiled_code = injected_sql
             model.extra_ctes = prepended_ctes
-            model.extra_ctes_injected = True
 
         # if model.extra_ctes is not set to prepended ctes, something went wrong
         return model, model.extra_ctes
 
     # Sets compiled_code and compiled flag in the ManifestSQLNode passed in,
     # creates a "context" dictionary for jinja rendering,
     # and then renders the "compiled_code" using the node, the
@@ -519,14 +519,20 @@
     ) -> ManifestSQLNode:
         """This is the main entry point into this code. It's called by
         CompileRunner.compile, GenericRPCRunner.compile, and
         RunTask.get_hook_sql. It calls '_compile_code' to render
         the node's raw_code into compiled_code, and then calls the
         recursive method to "prepend" the ctes.
         """
+        # Make sure Lexer for sqlparse 0.4.4 is initialized
+        from sqlparse.lexer import Lexer  # type: ignore
+
+        if hasattr(Lexer, "get_default_instance"):
+            Lexer.get_default_instance()
+
         node = self._compile_code(node, manifest, extra_context)
 
         node, _ = self._recursively_prepend_ctes(node, manifest, extra_context)
         if write:
             self._write_node(node)
         return node
```

### Comparing `dbt-core-1.6.0rc1/dbt/config/profile.py` & `dbt-core-1.6.0rc2/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/config/project.py` & `dbt-core-1.6.0rc2/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/config/renderer.py` & `dbt-core-1.6.0rc2/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/config/runtime.py` & `dbt-core-1.6.0rc2/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/config/selectors.py` & `dbt-core-1.6.0rc2/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/config/utils.py` & `dbt-core-1.6.0rc2/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/constants.py` & `dbt-core-1.6.0rc2/dbt/constants.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/base.py` & `dbt-core-1.6.0rc2/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/configured.py` & `dbt-core-1.6.0rc2/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/context_config.py` & `dbt-core-1.6.0rc2/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/docs.py` & `dbt-core-1.6.0rc2/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/exceptions_jinja.py` & `dbt-core-1.6.0rc2/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/macro_resolver.py` & `dbt-core-1.6.0rc2/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/macros.py` & `dbt-core-1.6.0rc2/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/manifest.py` & `dbt-core-1.6.0rc2/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/providers.py` & `dbt-core-1.6.0rc2/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/secret.py` & `dbt-core-1.6.0rc2/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/context/target.py` & `dbt-core-1.6.0rc2/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/connection.py` & `dbt-core-1.6.0rc2/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/files.py` & `dbt-core-1.6.0rc2/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/manifest.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/manifest_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/metrics.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/model_config.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/model_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,14 +615,16 @@
     updated_at: Optional[str] = None
     # Not using Optional because of serialization issues with a Union of str and List[str]
     check_cols: Union[str, List[str], None] = None
 
     @classmethod
     def validate(cls, data):
         super().validate(data)
+        # Note: currently you can't just set these keys in schema.yml because this validation
+        # will fail when parsing the snapshot node.
         if not data.get("strategy") or not data.get("unique_key") or not data.get("target_schema"):
             raise ValidationError(
                 "Snapshots must be configured with a 'strategy', 'unique_key', "
                 "and 'target_schema'."
             )
         if data.get("strategy") == "check":
             if not data.get("check_cols"):
@@ -645,14 +647,15 @@
                 raise ValidationError("A 'timestamp' snapshot should not have 'check_cols'")
         # If the strategy is not 'check' or 'timestamp' it's a custom strategy,
         # formerly supported with GenericSnapshotConfig
 
         if data.get("materialized") and data.get("materialized") != "snapshot":
             raise ValidationError("A snapshot must have a materialized value of 'snapshot'")
 
+    # Called by "calculate_node_config_dict" in ContextConfigGenerator
     def finalize_and_validate(self):
         data = self.to_dict(omit_none=True)
         self.validate(data)
         return self.from_dict(data)
 
 
 RESOURCE_TYPES: Dict[NodeType, Type[BaseConfig]] = {
```

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/node_args.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/node_args.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/nodes.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     SeedExceedsLimitChecksumChanged,
 )
 from dbt.events.contextvars import set_log_contextvars
 from dbt.flags import get_flags
 from dbt.node_types import ModelLanguage, NodeType, AccessType
 from dbt_semantic_interfaces.call_parameter_sets import FilterCallParameterSets
 from dbt_semantic_interfaces.references import (
+    EntityReference,
     MeasureReference,
     LinkableElementReference,
     SemanticModelReference,
     TimeDimensionReference,
 )
 from dbt_semantic_interfaces.references import MetricReference as DSIMetricReference
 from dbt_semantic_interfaces.type_enums import MetricType, TimeGranularity
@@ -1494,14 +1495,15 @@
     measures: Sequence[Measure] = field(default_factory=list)
     dimensions: Sequence[Dimension] = field(default_factory=list)
     metadata: Optional[SourceFileMetadata] = None
     depends_on: DependsOn = field(default_factory=DependsOn)
     refs: List[RefArgs] = field(default_factory=list)
     created_at: float = field(default_factory=lambda: time.time())
     config: SemanticModelConfig = field(default_factory=SemanticModelConfig)
+    primary_entity: Optional[str] = None
 
     @property
     def entity_references(self) -> List[LinkableElementReference]:
         return [entity.reference for entity in self.entities]
 
     @property
     def dimension_references(self) -> List[LinkableElementReference]:
@@ -1564,25 +1566,34 @@
             if measure.reference == measure_reference:
                 measure = measure
 
         assert (
             measure is not None
         ), f"No measure with name ({measure_reference.element_name}) in semantic_model with name ({self.name})"
 
-        if self.defaults is not None:
-            default_agg_time_dimesion = self.defaults.agg_time_dimension
+        default_agg_time_dimension = (
+            self.defaults.agg_time_dimension if self.defaults is not None else None
+        )
 
-        agg_time_dimension_name = measure.agg_time_dimension or default_agg_time_dimesion
+        agg_time_dimension_name = measure.agg_time_dimension or default_agg_time_dimension
         assert agg_time_dimension_name is not None, (
-            f"Aggregation time dimension for measure {measure.name} is not set! This should either be set directly on "
-            f"the measure specification in the model, or else defaulted to the primary time dimension in the data "
-            f"source containing the measure."
+            f"Aggregation time dimension for measure {measure.name} on semantic model {self.name} is not set! "
+            "To fix this either specify a default `agg_time_dimension` for the semantic model or define an "
+            "`agg_time_dimension` on the measure directly."
         )
         return TimeDimensionReference(element_name=agg_time_dimension_name)
 
+    @property
+    def primary_entity_reference(self) -> Optional[EntityReference]:
+        return (
+            EntityReference(element_name=self.primary_entity)
+            if self.primary_entity is not None
+            else None
+        )
+
 
 # ====================================
 # Patches
 # ====================================
 
 
 @dataclass
```

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/semantic_manifest.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/semantic_models.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/unparsed.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/unparsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,14 +724,15 @@
     name: str
     model: str  # looks like "ref(...)"
     description: Optional[str] = None
     defaults: Optional[Defaults] = None
     entities: List[UnparsedEntity] = field(default_factory=list)
     measures: List[UnparsedMeasure] = field(default_factory=list)
     dimensions: List[UnparsedDimension] = field(default_factory=list)
+    primary_entity: Optional[str] = None
 
 
 def normalize_date(d: Optional[datetime.date]) -> Optional[datetime.datetime]:
     """Convert date to datetime (at midnight), and add local time zone if naive"""
     if d is None:
         return None
```

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/graph/utils.py` & `dbt-core-1.6.0rc2/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/project.py` & `dbt-core-1.6.0rc2/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/relation.py` & `dbt-core-1.6.0rc2/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/results.py` & `dbt-core-1.6.0rc2/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/selection.py` & `dbt-core-1.6.0rc2/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/sql.py` & `dbt-core-1.6.0rc2/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/state.py` & `dbt-core-1.6.0rc2/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/contracts/util.py` & `dbt-core-1.6.0rc2/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/dataclass_schema.py` & `dbt-core-1.6.0rc2/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/deprecations.py` & `dbt-core-1.6.0rc2/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/deps/base.py` & `dbt-core-1.6.0rc2/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/deps/git.py` & `dbt-core-1.6.0rc2/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/deps/local.py` & `dbt-core-1.6.0rc2/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/deps/registry.py` & `dbt-core-1.6.0rc2/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/deps/resolver.py` & `dbt-core-1.6.0rc2/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/deps/tarball.py` & `dbt-core-1.6.0rc2/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.6.0rc2/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/docs/source/conf.py` & `dbt-core-1.6.0rc2/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/events/adapter_endpoint.py` & `dbt-core-1.6.0rc2/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/events/base_types.py` & `dbt-core-1.6.0rc2/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/events/contextvars.py` & `dbt-core-1.6.0rc2/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/events/eventmgr.py` & `dbt-core-1.6.0rc2/dbt/events/eventmgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import threading
 import traceback
 from typing import Any, Callable, List, Optional, TextIO
 from uuid import uuid4
 from dbt.events.format import timestamp_to_datetime_string
 
 from dbt.events.base_types import BaseEvent, EventLevel, msg_from_base_event, EventMsg
-
+import dbt.utils
 
 # A Filter is a function which takes a BaseEvent and returns True if the event
 # should be logged, False otherwise.
 Filter = Callable[[EventMsg], bool]
 
 
 # Default filter which logs every event
@@ -76,14 +76,15 @@
     filter: Filter = NoFilter
     scrubber: Scrubber = NoScrubber
     line_format: LineFormat = LineFormat.PlainText
     level: EventLevel = EventLevel.WARN
     use_colors: bool = False
     output_stream: Optional[TextIO] = None
     output_file_name: Optional[str] = None
+    output_file_max_bytes: Optional[int] = 10 * 1024 * 1024  # 10 mb
     logger: Optional[Any] = None
 
 
 class _Logger:
     def __init__(self, event_manager: "EventManager", config: LoggerConfig) -> None:
         self.name: str = config.name
         self.filter: Filter = config.filter
@@ -96,15 +97,15 @@
             stream_handler = logging.StreamHandler(config.output_stream)
             self._python_logger = self._get_python_log_for_handler(stream_handler)
 
         if config.output_file_name:
             file_handler = RotatingFileHandler(
                 filename=str(config.output_file_name),
                 encoding="utf8",
-                maxBytes=10 * 1024 * 1024,  # 10 mb
+                maxBytes=config.output_file_max_bytes,  # type: ignore
                 backupCount=5,
             )
             self._python_logger = self._get_python_log_for_handler(file_handler)
 
     def _get_python_log_for_handler(self, handler: logging.Handler):
         log = logging.getLogger(self.name)
         log.setLevel(_log_level_map[self.level])
@@ -171,15 +172,15 @@
 
 
 class _JsonLogger(_Logger):
     def create_line(self, msg: EventMsg) -> str:
         from dbt.events.functions import msg_to_dict
 
         msg_dict = msg_to_dict(msg)
-        raw_log_line = json.dumps(msg_dict, sort_keys=True)
+        raw_log_line = json.dumps(msg_dict, sort_keys=True, cls=dbt.utils.ForgivingJSONEncoder)
         line = self.scrubber(raw_log_line)  # type: ignore
         return line
 
 
 class EventManager:
     def __init__(self) -> None:
         self.loggers: List[_Logger] = []
```

### Comparing `dbt-core-1.6.0rc1/dbt/events/format.py` & `dbt-core-1.6.0rc2/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/events/functions.py` & `dbt-core-1.6.0rc2/dbt/events/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import json
 import os
 import sys
 from typing import Callable, Dict, List, Optional, TextIO
 import uuid
 from google.protobuf.json_format import MessageToDict
 
+import dbt.utils
 
 LOG_VERSION = 3
 metadata_vars: Optional[Dict[str, str]] = None
 
 # These are the logging events issued by the "clean" command,
 # where we can't count on having a log directory. We've removed
 # the "class" flags on the events in types.py. If necessary we
@@ -63,15 +64,19 @@
         if flags.LOG_LEVEL_FILE != "none":
             # create and add the file logger to the event manager
             log_file = os.path.join(flags.LOG_PATH, "dbt.log")
             log_file_format = _line_format_from_str(flags.LOG_FORMAT_FILE, LineFormat.DebugText)
             log_level_file = EventLevel.DEBUG if flags.DEBUG else EventLevel(flags.LOG_LEVEL_FILE)
             EVENT_MANAGER.add_logger(
                 _get_logfile_config(
-                    log_file, flags.USE_COLORS_FILE, log_file_format, log_level_file
+                    log_file,
+                    flags.USE_COLORS_FILE,
+                    log_file_format,
+                    log_level_file,
+                    flags.LOG_FILE_MAX_BYTES,
                 )
             )
 
 
 def _line_format_from_str(format_str: str, default: LineFormat) -> LineFormat:
     if format_str == "text":
         return LineFormat.PlainText
@@ -112,24 +117,29 @@
 ) -> bool:
     return (msg.info.name not in ["CacheAction", "CacheDumpGraph"] or log_cache_events) and not (
         line_format == LineFormat.Json and type(msg.data) == Formatting
     )
 
 
 def _get_logfile_config(
-    log_path: str, use_colors: bool, line_format: LineFormat, level: EventLevel
+    log_path: str,
+    use_colors: bool,
+    line_format: LineFormat,
+    level: EventLevel,
+    log_file_max_bytes: int,
 ) -> LoggerConfig:
     return LoggerConfig(
         name="file_log",
         line_format=line_format,
         use_colors=use_colors,
         level=level,  # File log is *always* debug level
         scrubber=env_scrubber,
         filter=partial(_logfile_filter, bool(get_flags().LOG_CACHE_EVENTS), line_format),
         output_file_name=log_path,
+        output_file_max_bytes=log_file_max_bytes,
     )
 
 
 def _logfile_filter(log_cache_events: bool, line_format: LineFormat, msg: EventMsg) -> bool:
     return (
         msg.info.code not in nofile_codes
         and not (msg.info.name in ["CacheAction", "CacheDumpGraph"] and not log_cache_events)
@@ -196,15 +206,15 @@
     _CAPTURE_STREAM = None
 
 
 # returns a dictionary representation of the event fields.
 # the message may contain secrets which must be scrubbed at the usage site.
 def msg_to_json(msg: EventMsg) -> str:
     msg_dict = msg_to_dict(msg)
-    raw_log_line = json.dumps(msg_dict, sort_keys=True)
+    raw_log_line = json.dumps(msg_dict, sort_keys=True, cls=dbt.utils.ForgivingJSONEncoder)
     return raw_log_line
 
 
 def msg_to_dict(msg: EventMsg) -> dict:
     msg_dict = dict()
     try:
         msg_dict = MessageToDict(
```

### Comparing `dbt-core-1.6.0rc1/dbt/events/helpers.py` & `dbt-core-1.6.0rc2/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/events/types.py` & `dbt-core-1.6.0rc2/dbt/events/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1149,18 +1149,19 @@
 
 class DeprecatedModel(WarnLevel):
     def code(self):
         return "I065"
 
     def message(self) -> str:
         version = ".v" + self.model_version if self.model_version else ""
-        return (
+        msg = (
             f"Model {self.model_name}{version} has passed its deprecation date of {self.deprecation_date}. "
             "This model should be disabled or removed."
         )
+        return warning_tag(msg)
 
 
 class UpcomingReferenceDeprecation(WarnLevel):
     def code(self):
         return "I066"
 
     def message(self) -> str:
@@ -1174,15 +1175,15 @@
             coda = (
                 f"A new version of '{self.ref_model_name}' is available. Try it out: "
                 f"{{{{ ref('{self.ref_model_package}', '{self.ref_model_name}', "
                 f"v='{self.ref_model_latest_version}') }}}}."
             )
             msg = msg + coda
 
-        return msg
+        return warning_tag(msg)
 
 
 class DeprecatedReference(WarnLevel):
     def code(self):
         return "I067"
 
     def message(self) -> str:
@@ -1196,15 +1197,15 @@
             coda = (
                 f"A new version of '{self.ref_model_name}' is available. Migrate now: "
                 f"{{{{ ref('{self.ref_model_package}', '{self.ref_model_name}', "
                 f"v='{self.ref_model_latest_version}') }}}}."
             )
             msg = msg + coda
 
-        return msg
+        return warning_tag(msg)
 
 
 class UnsupportedConstraintMaterialization(WarnLevel):
     def code(self):
         return "I068"
 
     def message(self) -> str:
```

### Comparing `dbt-core-1.6.0rc1/dbt/events/types_pb2.py` & `dbt-core-1.6.0rc2/dbt/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/exceptions.py` & `dbt-core-1.6.0rc2/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/flags.py` & `dbt-core-1.6.0rc2/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/graph/cli.py` & `dbt-core-1.6.0rc2/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/graph/graph.py` & `dbt-core-1.6.0rc2/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/graph/queue.py` & `dbt-core-1.6.0rc2/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/graph/selector.py` & `dbt-core-1.6.0rc2/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/graph/selector_methods.py` & `dbt-core-1.6.0rc2/dbt/graph/selector_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/graph/selector_spec.py` & `dbt-core-1.6.0rc2/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/helper_types.py` & `dbt-core-1.6.0rc2/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/README.md` & `dbt-core-1.6.0rc2/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/docs/overview.md` & `dbt-core-1.6.0rc2/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/drop_relation.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/drop_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/clone.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/clone/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.6.0rc2/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/index.html` & `dbt-core-1.6.0rc2/dbt/include/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -93338,286 +93338,260 @@
 0016c990: 3d5c 2761 6374 6976 655c 2720 6e67 2d73  =\'active\' ng-s
 0016c9a0: 686f 7720 3d20 2270 6172 656e 7473 4c65  how = "parentsLe
 0016c9b0: 6e67 7468 2021 3d20 3022 3e3c 6120 7569  ngth != 0"><a ui
 0016c9c0: 2d73 7265 663d 2264 6274 2e6d 6574 7269  -sref="dbt.metri
 0016c9d0: 6328 7b5c 2723 5c27 3a20 5c27 6465 7065  c({\'#\': \'depe
 0016c9e0: 6e64 735f 6f6e 5c27 7d29 223e 4465 7065  nds_on\'})">Depe
 0016c9f0: 6e64 7320 4f6e 3c2f 613e 3c2f 6c69 3e5c  nds On</a></li>\
-0016ca00: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016ca10: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
-0016ca20: 6976 653d 5c27 6163 7469 7665 5c27 3e3c  ive=\'active\'><
-0016ca30: 6120 7569 2d73 7265 663d 2264 6274 2e6d  a ui-sref="dbt.m
-0016ca40: 6574 7269 6328 7b5c 2723 5c27 3a20 5c27  etric({\'#\': \'
-0016ca50: 636f 6465 5c27 7d29 223e 5351 4c3c 2f61  code\'})">SQL</a
-0016ca60: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
-0016ca70: 2020 2020 3c2f 756c 3e5c 6e20 2020 2020      </ul>\n     
-0016ca80: 2020 203c 2f64 6976 3e5c 6e20 2020 203c     </div>\n    <
-0016ca90: 2f64 6976 3e5c 6e20 2020 203c 6469 7620  /div>\n    <div 
-0016caa0: 636c 6173 733d 2261 7070 2d64 6574 6169  class="app-detai
-0016cab0: 6c73 223e 5c6e 2020 2020 2020 2020 3c64  ls">\n        <d
-0016cac0: 6976 2063 6c61 7373 3d22 6170 702d 6672  iv class="app-fr
-0016cad0: 616d 6520 6170 702d 7061 6422 3e5c 6e5c  ame app-pad">\n\
-0016cae0: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-0016caf0: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
-0016cb00: 7469 6f6e 223e 5c6e 2020 2020 2020 2020  tion">\n        
-0016cb10: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0016cb20: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
-0016cb30: 6574 2220 6964 3d22 6465 7461 696c 7322  et" id="details"
-0016cb40: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
-0016cb50: 2020 2020 2020 2020 203c 7461 626c 652d           <table-
-0016cb60: 6465 7461 696c 7320 6d6f 6465 6c3d 226d  details model="m
-0016cb70: 6574 7269 6322 2065 7874 7261 733d 2265  etric" extras="e
-0016cb80: 7874 7261 5f74 6162 6c65 5f66 6965 6c64  xtra_table_field
-0016cb90: 7322 202f 3e5c 6e20 2020 2020 2020 2020  s" />\n         
-0016cba0: 2020 203c 2f73 6563 7469 6f6e 3e5c 6e5c     </section>\n\
-0016cbb0: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-0016cbc0: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
-0016cbd0: 7469 6f6e 223e 5c6e 2020 2020 2020 2020  tion">\n        
-0016cbe0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0016cbf0: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
-0016cc00: 6574 2220 6964 3d22 6465 7363 7269 7074  et" id="descript
-0016cc10: 696f 6e22 3e3c 2f64 6976 3e5c 6e20 2020  ion"></div>\n   
-0016cc20: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016cc30: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
-0016cc40: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
-0016cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016cc60: 3c68 363e 4465 7363 7269 7074 696f 6e3c  <h6>Description<
-0016cc70: 2f68 363e 5c6e 2020 2020 2020 2020 2020  /h6>\n          
-0016cc80: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0016cc90: 6c61 7373 3d22 7061 6e65 6c22 3e5c 6e20  lass="panel">\n 
-0016cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ccb0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016ccc0: 733d 2270 616e 656c 2d62 6f64 7922 3e5c  s="panel-body">\
-0016ccd0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016cce0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016ccf0: 7620 6e67 2d69 663d 226d 6574 7269 632e  v ng-if="metric.
-0016cd00: 6465 7363 7269 7074 696f 6e22 2063 6c61  description" cla
-0016cd10: 7373 3d22 6d6f 6465 6c2d 6d61 726b 646f  ss="model-markdo
-0016cd20: 776e 2220 6d61 726b 6564 3d22 6d65 7472  wn" marked="metr
-0016cd30: 6963 2e64 6573 6372 6970 7469 6f6e 223e  ic.description">
-0016cd40: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016cd60: 2020 2020 3c64 6976 206e 672d 6966 3d22      <div ng-if="
-0016cd70: 216d 6574 7269 632e 6465 7363 7269 7074  !metric.descript
-0016cd80: 696f 6e22 3e54 6869 7320 7b7b 206d 6574  ion">This {{ met
-0016cd90: 7269 632e 7265 736f 7572 6365 5f74 7970  ric.resource_typ
-0016cda0: 6520 7d7d 2069 7320 6e6f 7420 6375 7272  e }} is not curr
-0016cdb0: 656e 746c 7920 646f 6375 6d65 6e74 6564  ently documented
-0016cdc0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016cde0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016cdf0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0016ce00: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016ce10: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016ce20: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
-0016ce30: 6e3e 5c6e 5c6e 2020 2020 2020 2020 2020  n>\n\n          
-0016ce40: 2020 3c73 6563 7469 6f6e 2063 6c61 7373    <section class
-0016ce50: 3d22 7365 6374 696f 6e22 206e 672d 7368  ="section" ng-sh
-0016ce60: 6f77 203d 2022 7061 7265 6e74 734c 656e  ow = "parentsLen
-0016ce70: 6774 6820 213d 2030 223e 5c6e 2020 2020  gth != 0">\n    
-0016ce80: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016ce90: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-0016cea0: 7461 7267 6574 2220 6964 3d22 6465 7065  target" id="depe
-0016ceb0: 6e64 735f 6f6e 223e 3c2f 6469 763e 5c6e  nds_on"></div>\n
-0016cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ced0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-0016cee0: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
-0016cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016cf00: 2020 203c 6836 3e44 6570 656e 6473 204f     <h6>Depends O
-0016cf10: 6e3c 2f68 363e 5c6e 2020 2020 2020 2020  n</h6>\n        
-0016cf20: 2020 2020 2020 2020 2020 2020 3c72 6566              <ref
-0016cf30: 6572 656e 6365 2d6c 6973 7420 7265 6665  erence-list refe
-0016cf40: 7265 6e63 6573 3d22 7061 7265 6e74 7322  rences="parents"
-0016cf50: 206e 6f64 653d 226d 6574 7269 6322 202f   node="metric" /
-0016cf60: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016cf70: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
-0016cf80: 2020 2020 2020 203c 2f73 6563 7469 6f6e         </section
-0016cf90: 3e5c 6e5c 6e5c 6e20 2020 2020 2020 2020  >\n\n\n         
-0016cfa0: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
-0016cfb0: 733d 2273 6563 7469 6f6e 223e 5c6e 2020  s="section">\n  
-0016cfc0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0016cfd0: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
-0016cfe0: 6e2d 7461 7267 6574 2220 6964 3d22 636f  n-target" id="co
-0016cff0: 6465 223e 3c2f 6469 763e 5c6e 2020 2020  de"></div>\n    
-0016d000: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016d010: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-0016d020: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
-0016d030: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016d040: 636f 6465 2d62 6c6f 636b 2076 6572 7369  code-block versi
-0016d050: 6f6e 733d 2276 6572 7369 6f6e 7322 2064  ons="versions" d
-0016d060: 6566 6175 6c74 3d22 6465 6661 756c 745f  efault="default_
-0016d070: 7665 7273 696f 6e22 206c 616e 6775 6167  version" languag
-0016d080: 653d 226c 616e 6775 6167 6522 3e3c 2f63  e="language"></c
-0016d090: 6f64 652d 626c 6f63 6b3e 5c6e 2020 2020  ode-block>\n    
-0016d0a0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0016d0b0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016d0c0: 3c2f 7365 6374 696f 6e3e 5c6e 2020 2020  </section>\n    
-0016d0d0: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016d0e0: 3c2f 6469 763e 5c6e 3c2f 6469 763e 5c6e  </div>\n</div>\n
-0016d0f0: 2729 7d5d 292c 652e 6578 706f 7274 733d  ')}]),e.exports=
-0016d100: 6e7d 2c66 756e 6374 696f 6e28 652c 7429  n},function(e,t)
-0016d110: 7b76 6172 206e 3d22 2f64 6f63 732f 6f70  {var n="/docs/op
-0016d120: 6572 6174 696f 6e2e 6874 6d6c 223b 7769  eration.html";wi
-0016d130: 6e64 6f77 2e61 6e67 756c 6172 2e6d 6f64  ndow.angular.mod
-0016d140: 756c 6528 226e 6722 292e 7275 6e28 5b22  ule("ng").run(["
-0016d150: 2474 656d 706c 6174 6543 6163 6865 222c  $templateCache",
-0016d160: 6675 6e63 7469 6f6e 2865 297b 652e 7075  function(e){e.pu
-0016d170: 7428 6e2c 273c 7374 796c 653e 5c6e 2f2a  t(n,'<style>\n/*
-0016d180: 2054 4f44 4f20 2a2f 5c6e 2e73 6563 7469   TODO */\n.secti
-0016d190: 6f6e 2d74 6172 6765 7420 7b5c 6e20 2020  on-target {\n   
-0016d1a0: 2074 6f70 3a20 2d38 656d 3b5c 6e7d 5c6e   top: -8em;\n}\n
-0016d1b0: 5c6e 2e6e 6f66 6c65 7820 7b5c 6e20 2020  \n.noflex {\n   
-0016d1c0: 2066 6c65 783a 2030 2030 2031 3630 7078   flex: 0 0 160px
-0016d1d0: 2021 696d 706f 7274 616e 743b 5c6e 7d5c   !important;\n}\
-0016d1e0: 6e5c 6e2e 6869 6768 6c69 6768 7420 7b5c  n\n.highlight {\
-0016d1f0: 6e20 2020 2063 6f6c 6f72 3a20 2332 3432  n    color: #242
-0016d200: 3932 653b 5c6e 2020 2020 6261 636b 6772  92e;\n    backgr
-0016d210: 6f75 6e64 2d63 6f6c 6f72 3a20 7768 6974  ound-color: whit
-0016d220: 653b 5c6e 7d5c 6e5c 6e3c 2f73 7479 6c65  e;\n}\n\n</style
-0016d230: 3e5c 6e5c 6e3c 6469 7620 636c 6173 733d  >\n\n<div class=
-0016d240: 5c27 6170 702d 7363 726f 6c6c 5c27 3e5c  \'app-scroll\'>\
-0016d250: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
-0016d260: 2261 7070 2d6c 696e 6b73 2061 7070 2d73  "app-links app-s
-0016d270: 7469 636b 7922 3e5c 6e20 2020 2020 2020  ticky">\n       
-0016d280: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-0016d290: 2d74 6974 6c65 223e 5c6e 2020 2020 2020  -title">\n      
-0016d2a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016d2b0: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
-0016d2c0: 7061 6420 6170 702d 666c 7573 682d 626f  pad app-flush-bo
-0016d2d0: 7474 6f6d 223e 5c6e 2020 2020 2020 2020  ttom">\n        
-0016d2e0: 2020 2020 2020 2020 3c68 313e 5c6e 2020          <h1>\n  
-0016d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d300: 2020 3c73 7061 6e20 636c 6173 733d 2262    <span class="b
-0016d310: 7265 616b 223e 7b7b 206d 6f64 656c 2e6e  reak">{{ model.n
-0016d320: 616d 6520 7d7d 3c2f 7370 616e 3e5c 6e20  ame }}</span>\n 
-0016d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d340: 2020 203c 736d 616c 6c3e 6f70 6572 6174     <small>operat
-0016d350: 696f 6e3c 2f73 6d61 6c6c 3e5c 6e20 2020  ion</small>\n   
-0016d360: 2020 2020 2020 2020 2020 2020 203c 2f68               </h
-0016d370: 313e 5c6e 2020 2020 2020 2020 2020 2020  1>\n            
-0016d380: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016d390: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016d3a0: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
-0016d3b0: 6672 616d 6520 6170 702d 7061 642d 6822  frame app-pad-h"
-0016d3c0: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-0016d3d0: 756c 2063 6c61 7373 3d22 6e61 7620 6e61  ul class="nav na
-0016d3e0: 762d 7461 6273 223e 5c6e 2020 2020 2020  v-tabs">\n      
-0016d3f0: 2020 2020 2020 2020 2020 3c6c 6920 7569            <li ui
-0016d400: 2d73 7265 662d 6163 7469 7665 3d5c 2761  -sref-active=\'a
-0016d410: 6374 6976 655c 273e 3c61 2075 692d 7372  ctive\'><a ui-sr
-0016d420: 6566 3d22 6462 742e 6f70 6572 6174 696f  ef="dbt.operatio
-0016d430: 6e28 7b5c 2723 5c27 3a20 5c27 6465 7363  n({\'#\': \'desc
-0016d440: 7269 7074 696f 6e5c 277d 2922 3e44 6573  ription\'})">Des
-0016d450: 6372 6970 7469 6f6e 3c2f 613e 3c2f 6c69  cription</a></li
+0016ca00: 6e20 2020 2020 2020 2020 2020 203c 2f75  n            </u
+0016ca10: 6c3e 5c6e 2020 2020 2020 2020 3c2f 6469  l>\n        </di
+0016ca20: 763e 5c6e 2020 2020 3c2f 6469 763e 5c6e  v>\n    </div>\n
+0016ca30: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016ca40: 6170 702d 6465 7461 696c 7322 3e5c 6e20  app-details">\n 
+0016ca50: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016ca60: 733d 2261 7070 2d66 7261 6d65 2061 7070  s="app-frame app
+0016ca70: 2d70 6164 223e 5c6e 5c6e 2020 2020 2020  -pad">\n\n      
+0016ca80: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
+0016ca90: 6c61 7373 3d22 7365 6374 696f 6e22 3e5c  lass="section">\
+0016caa0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016cab0: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+0016cac0: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
+0016cad0: 2264 6574 6169 6c73 223e 3c2f 6469 763e  "details"></div>
+0016cae0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016caf0: 2020 3c74 6162 6c65 2d64 6574 6169 6c73    <table-details
+0016cb00: 206d 6f64 656c 3d22 6d65 7472 6963 2220   model="metric" 
+0016cb10: 6578 7472 6173 3d22 6578 7472 615f 7461  extras="extra_ta
+0016cb20: 626c 655f 6669 656c 6473 2220 2f3e 5c6e  ble_fields" />\n
+0016cb30: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
+0016cb40: 6374 696f 6e3e 5c6e 5c6e 2020 2020 2020  ction>\n\n      
+0016cb50: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
+0016cb60: 6c61 7373 3d22 7365 6374 696f 6e22 3e5c  lass="section">\
+0016cb70: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016cb80: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+0016cb90: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
+0016cba0: 2264 6573 6372 6970 7469 6f6e 223e 3c2f  "description"></
+0016cbb0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+0016cbc0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0016cbd0: 3d22 7365 6374 696f 6e2d 636f 6e74 656e  ="section-conten
+0016cbe0: 7422 3e5c 6e20 2020 2020 2020 2020 2020  t">\n           
+0016cbf0: 2020 2020 2020 2020 203c 6836 3e44 6573           <h6>Des
+0016cc00: 6372 6970 7469 6f6e 3c2f 6836 3e5c 6e20  cription</h6>\n 
+0016cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016cc20: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
+0016cc30: 616e 656c 223e 5c6e 2020 2020 2020 2020  anel">\n        
+0016cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016cc50: 3c64 6976 2063 6c61 7373 3d22 7061 6e65  <div class="pane
+0016cc60: 6c2d 626f 6479 223e 5c6e 2020 2020 2020  l-body">\n      
+0016cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016cc80: 2020 2020 2020 3c64 6976 206e 672d 6966        <div ng-if
+0016cc90: 3d22 6d65 7472 6963 2e64 6573 6372 6970  ="metric.descrip
+0016cca0: 7469 6f6e 2220 636c 6173 733d 226d 6f64  tion" class="mod
+0016ccb0: 656c 2d6d 6172 6b64 6f77 6e22 206d 6172  el-markdown" mar
+0016ccc0: 6b65 643d 226d 6574 7269 632e 6465 7363  ked="metric.desc
+0016ccd0: 7269 7074 696f 6e22 3e3c 2f64 6976 3e5c  ription"></div>\
+0016cce0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016ccf0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016cd00: 7620 6e67 2d69 663d 2221 6d65 7472 6963  v ng-if="!metric
+0016cd10: 2e64 6573 6372 6970 7469 6f6e 223e 5468  .description">Th
+0016cd20: 6973 207b 7b20 6d65 7472 6963 2e72 6573  is {{ metric.res
+0016cd30: 6f75 7263 655f 7479 7065 207d 7d20 6973  ource_type }} is
+0016cd40: 206e 6f74 2063 7572 7265 6e74 6c79 2064   not currently d
+0016cd50: 6f63 756d 656e 7465 643c 2f64 6976 3e5c  ocumented</div>\
+0016cd60: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016cd70: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+0016cd80: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016cd90: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+0016cda0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0016cdb0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016cdc0: 203c 2f73 6563 7469 6f6e 3e5c 6e5c 6e20   </section>\n\n 
+0016cdd0: 2020 2020 2020 2020 2020 203c 7365 6374             <sect
+0016cde0: 696f 6e20 636c 6173 733d 2273 6563 7469  ion class="secti
+0016cdf0: 6f6e 2220 6e67 2d73 686f 7720 3d20 2270  on" ng-show = "p
+0016ce00: 6172 656e 7473 4c65 6e67 7468 2021 3d20  arentsLength != 
+0016ce10: 3022 3e5c 6e20 2020 2020 2020 2020 2020  0">\n           
+0016ce20: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016ce30: 2273 6563 7469 6f6e 2d74 6172 6765 7422  "section-target"
+0016ce40: 2069 643d 2264 6570 656e 6473 5f6f 6e22   id="depends_on"
+0016ce50: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
+0016ce60: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016ce70: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
+0016ce80: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
+0016ce90: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
+0016cea0: 4465 7065 6e64 7320 4f6e 3c2f 6836 3e5c  Depends On</h6>\
+0016ceb0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016cec0: 2020 2020 203c 7265 6665 7265 6e63 652d       <reference-
+0016ced0: 6c69 7374 2072 6566 6572 656e 6365 733d  list references=
+0016cee0: 2270 6172 656e 7473 2220 6e6f 6465 3d22  "parents" node="
+0016cef0: 6d65 7472 6963 2220 2f3e 5c6e 2020 2020  metric" />\n    
+0016cf00: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+0016cf10: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+0016cf20: 3c2f 7365 6374 696f 6e3e 5c6e 5c6e 2020  </section>\n\n  
+0016cf30: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+0016cf40: 2020 3c2f 6469 763e 5c6e 3c2f 6469 763e    </div>\n</div>
+0016cf50: 5c6e 2729 7d5d 292c 652e 6578 706f 7274  \n')}]),e.export
+0016cf60: 733d 6e7d 2c66 756e 6374 696f 6e28 652c  s=n},function(e,
+0016cf70: 7429 7b76 6172 206e 3d22 2f64 6f63 732f  t){var n="/docs/
+0016cf80: 6f70 6572 6174 696f 6e2e 6874 6d6c 223b  operation.html";
+0016cf90: 7769 6e64 6f77 2e61 6e67 756c 6172 2e6d  window.angular.m
+0016cfa0: 6f64 756c 6528 226e 6722 292e 7275 6e28  odule("ng").run(
+0016cfb0: 5b22 2474 656d 706c 6174 6543 6163 6865  ["$templateCache
+0016cfc0: 222c 6675 6e63 7469 6f6e 2865 297b 652e  ",function(e){e.
+0016cfd0: 7075 7428 6e2c 273c 7374 796c 653e 5c6e  put(n,'<style>\n
+0016cfe0: 2f2a 2054 4f44 4f20 2a2f 5c6e 2e73 6563  /* TODO */\n.sec
+0016cff0: 7469 6f6e 2d74 6172 6765 7420 7b5c 6e20  tion-target {\n 
+0016d000: 2020 2074 6f70 3a20 2d38 656d 3b5c 6e7d     top: -8em;\n}
+0016d010: 5c6e 5c6e 2e6e 6f66 6c65 7820 7b5c 6e20  \n\n.noflex {\n 
+0016d020: 2020 2066 6c65 783a 2030 2030 2031 3630     flex: 0 0 160
+0016d030: 7078 2021 696d 706f 7274 616e 743b 5c6e  px !important;\n
+0016d040: 7d5c 6e5c 6e2e 6869 6768 6c69 6768 7420  }\n\n.highlight 
+0016d050: 7b5c 6e20 2020 2063 6f6c 6f72 3a20 2332  {\n    color: #2
+0016d060: 3432 3932 653b 5c6e 2020 2020 6261 636b  4292e;\n    back
+0016d070: 6772 6f75 6e64 2d63 6f6c 6f72 3a20 7768  ground-color: wh
+0016d080: 6974 653b 5c6e 7d5c 6e5c 6e3c 2f73 7479  ite;\n}\n\n</sty
+0016d090: 6c65 3e5c 6e5c 6e3c 6469 7620 636c 6173  le>\n\n<div clas
+0016d0a0: 733d 5c27 6170 702d 7363 726f 6c6c 5c27  s=\'app-scroll\'
+0016d0b0: 3e5c 6e20 2020 203c 6469 7620 636c 6173  >\n    <div clas
+0016d0c0: 733d 2261 7070 2d6c 696e 6b73 2061 7070  s="app-links app
+0016d0d0: 2d73 7469 636b 7922 3e5c 6e20 2020 2020  -sticky">\n     
+0016d0e0: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+0016d0f0: 7070 2d74 6974 6c65 223e 5c6e 2020 2020  pp-title">\n    
+0016d100: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016d110: 7373 3d22 6170 702d 6672 616d 6520 6170  ss="app-frame ap
+0016d120: 702d 7061 6420 6170 702d 666c 7573 682d  p-pad app-flush-
+0016d130: 626f 7474 6f6d 223e 5c6e 2020 2020 2020  bottom">\n      
+0016d140: 2020 2020 2020 2020 2020 3c68 313e 5c6e            <h1>\n
+0016d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d160: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+0016d170: 2262 7265 616b 223e 7b7b 206d 6f64 656c  "break">{{ model
+0016d180: 2e6e 616d 6520 7d7d 3c2f 7370 616e 3e5c  .name }}</span>\
+0016d190: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016d1a0: 2020 2020 203c 736d 616c 6c3e 6f70 6572       <small>oper
+0016d1b0: 6174 696f 6e3c 2f73 6d61 6c6c 3e5c 6e20  ation</small>\n 
+0016d1c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016d1d0: 2f68 313e 5c6e 2020 2020 2020 2020 2020  /h1>\n          
+0016d1e0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+0016d1f0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+0016d200: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
+0016d210: 702d 6672 616d 6520 6170 702d 7061 642d  p-frame app-pad-
+0016d220: 6822 3e5c 6e20 2020 2020 2020 2020 2020  h">\n           
+0016d230: 203c 756c 2063 6c61 7373 3d22 6e61 7620   <ul class="nav 
+0016d240: 6e61 762d 7461 6273 223e 5c6e 2020 2020  nav-tabs">\n    
+0016d250: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
+0016d260: 7569 2d73 7265 662d 6163 7469 7665 3d5c  ui-sref-active=\
+0016d270: 2761 6374 6976 655c 273e 3c61 2075 692d  'active\'><a ui-
+0016d280: 7372 6566 3d22 6462 742e 6f70 6572 6174  sref="dbt.operat
+0016d290: 696f 6e28 7b5c 2723 5c27 3a20 5c27 6465  ion({\'#\': \'de
+0016d2a0: 7363 7269 7074 696f 6e5c 277d 2922 3e44  scription\'})">D
+0016d2b0: 6573 6372 6970 7469 6f6e 3c2f 613e 3c2f  escription</a></
+0016d2c0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+0016d2d0: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
+0016d2e0: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
+0016d2f0: 5c27 206e 672d 7368 6f77 203d 2022 7061  \' ng-show = "pa
+0016d300: 7265 6e74 734c 656e 6774 6820 213d 2030  rentsLength != 0
+0016d310: 223e 3c61 2075 692d 7372 6566 3d22 6462  "><a ui-sref="db
+0016d320: 742e 6f70 6572 6174 696f 6e28 7b5c 2723  t.operation({\'#
+0016d330: 5c27 3a20 5c27 6465 7065 6e64 735f 6f6e  \': \'depends_on
+0016d340: 5c27 7d29 223e 4465 7065 6e64 7320 4f6e  \'})">Depends On
+0016d350: 3c2f 613e 3c2f 6c69 3e5c 6e20 2020 2020  </a></li>\n     
+0016d360: 2020 2020 2020 2020 2020 203c 6c69 2075             <li u
+0016d370: 692d 7372 6566 2d61 6374 6976 653d 5c27  i-sref-active=\'
+0016d380: 6163 7469 7665 5c27 3e3c 6120 7569 2d73  active\'><a ui-s
+0016d390: 7265 663d 2264 6274 2e6f 7065 7261 7469  ref="dbt.operati
+0016d3a0: 6f6e 287b 5c27 235c 273a 205c 2763 6f64  on({\'#\': \'cod
+0016d3b0: 655c 277d 2922 3e53 514c 3c2f 613e 3c2f  e\'})">SQL</a></
+0016d3c0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+0016d3d0: 203c 2f75 6c3e 5c6e 2020 2020 2020 2020   </ul>\n        
+0016d3e0: 3c2f 6469 763e 5c6e 2020 2020 3c2f 6469  </div>\n    </di
+0016d3f0: 763e 5c6e 2020 2020 3c64 6976 2063 6c61  v>\n    <div cla
+0016d400: 7373 3d22 6170 702d 6465 7461 696c 7322  ss="app-details"
+0016d410: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
+0016d420: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
+0016d430: 2061 7070 2d70 6164 223e 5c6e 2020 2020   app-pad">\n    
+0016d440: 2020 2020 2020 2020 3c73 6563 7469 6f6e          <section
+0016d450: 2063 6c61 7373 3d22 7365 6374 696f 6e22   class="section"
 0016d460: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016d470: 2020 203c 6c69 2075 692d 7372 6566 2d61     <li ui-sref-a
-0016d480: 6374 6976 653d 5c27 6163 7469 7665 5c27  ctive=\'active\'
-0016d490: 206e 672d 7368 6f77 203d 2022 7061 7265   ng-show = "pare
-0016d4a0: 6e74 734c 656e 6774 6820 213d 2030 223e  ntsLength != 0">
-0016d4b0: 3c61 2075 692d 7372 6566 3d22 6462 742e  <a ui-sref="dbt.
-0016d4c0: 6f70 6572 6174 696f 6e28 7b5c 2723 5c27  operation({\'#\'
-0016d4d0: 3a20 5c27 6465 7065 6e64 735f 6f6e 5c27  : \'depends_on\'
-0016d4e0: 7d29 223e 4465 7065 6e64 7320 4f6e 3c2f  })">Depends On</
-0016d4f0: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
-0016d500: 2020 2020 2020 2020 203c 6c69 2075 692d           <li ui-
-0016d510: 7372 6566 2d61 6374 6976 653d 5c27 6163  sref-active=\'ac
-0016d520: 7469 7665 5c27 3e3c 6120 7569 2d73 7265  tive\'><a ui-sre
-0016d530: 663d 2264 6274 2e6f 7065 7261 7469 6f6e  f="dbt.operation
-0016d540: 287b 5c27 235c 273a 205c 2763 6f64 655c  ({\'#\': \'code\
-0016d550: 277d 2922 3e53 514c 3c2f 613e 3c2f 6c69  '})">SQL</a></li
-0016d560: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-0016d570: 2f75 6c3e 5c6e 2020 2020 2020 2020 3c2f  /ul>\n        </
-0016d580: 6469 763e 5c6e 2020 2020 3c2f 6469 763e  div>\n    </div>
-0016d590: 5c6e 2020 2020 3c64 6976 2063 6c61 7373  \n    <div class
-0016d5a0: 3d22 6170 702d 6465 7461 696c 7322 3e5c  ="app-details">\
-0016d5b0: 6e20 2020 2020 2020 203c 6469 7620 636c  n        <div cl
-0016d5c0: 6173 733d 2261 7070 2d66 7261 6d65 2061  ass="app-frame a
-0016d5d0: 7070 2d70 6164 223e 5c6e 2020 2020 2020  pp-pad">\n      
-0016d5e0: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
-0016d5f0: 6c61 7373 3d22 7365 6374 696f 6e22 3e5c  lass="section">\
-0016d600: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016d610: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
-0016d620: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
-0016d630: 2264 6573 6372 6970 7469 6f6e 223e 3c2f  "description"></
-0016d640: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-0016d650: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016d660: 3d22 7365 6374 696f 6e2d 636f 6e74 656e  ="section-conten
-0016d670: 7422 3e5c 6e20 2020 2020 2020 2020 2020  t">\n           
-0016d680: 2020 2020 2020 2020 203c 6836 3e44 6573           <h6>Des
-0016d690: 6372 6970 7469 6f6e 3c2f 6836 3e5c 6e20  cription</h6>\n 
-0016d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d6b0: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
-0016d6c0: 616e 656c 223e 5c6e 2020 2020 2020 2020  anel">\n        
-0016d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d6e0: 3c64 6976 2063 6c61 7373 3d22 7061 6e65  <div class="pane
-0016d6f0: 6c2d 626f 6479 223e 5c6e 2020 2020 2020  l-body">\n      
-0016d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d710: 2020 2020 2020 3c64 6976 206e 672d 6966        <div ng-if
-0016d720: 3d22 6d6f 6465 6c2e 6465 7363 7269 7074  ="model.descript
-0016d730: 696f 6e22 2063 6c61 7373 3d22 6d6f 6465  ion" class="mode
-0016d740: 6c2d 6d61 726b 646f 776e 2220 6d61 726b  l-markdown" mark
-0016d750: 6564 3d22 6d6f 6465 6c2e 6465 7363 7269  ed="model.descri
-0016d760: 7074 696f 6e22 3e3c 2f64 6976 3e5c 6e20  ption"></div>\n 
-0016d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d780: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016d790: 6e67 2d69 663d 2221 6d6f 6465 6c2e 6465  ng-if="!model.de
-0016d7a0: 7363 7269 7074 696f 6e22 3e54 6869 7320  scription">This 
-0016d7b0: 7b7b 206d 6f64 656c 2e72 6573 6f75 7263  {{ model.resourc
-0016d7c0: 655f 7479 7065 207d 7d20 6973 206e 6f74  e_type }} is not
-0016d7d0: 2063 7572 7265 6e74 6c79 2064 6f63 756d   currently docum
-0016d7e0: 656e 7465 643c 2f64 6976 3e5c 6e20 2020  ented</div>\n   
-0016d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d800: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
-0016d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d820: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
-0016d830: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0016d840: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
-0016d850: 6563 7469 6f6e 3e5c 6e5c 6e20 2020 2020  ection>\n\n     
-0016d860: 2020 2020 2020 203c 7365 6374 696f 6e20         <section 
-0016d870: 636c 6173 733d 2273 6563 7469 6f6e 2220  class="section" 
-0016d880: 6e67 2d73 686f 7720 3d20 2270 6172 656e  ng-show = "paren
-0016d890: 7473 4c65 6e67 7468 2021 3d20 3022 3e5c  tsLength != 0">\
-0016d8a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016d8b0: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
-0016d8c0: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
-0016d8d0: 2264 6570 656e 6473 5f6f 6e22 3e3c 2f64  "depends_on"></d
-0016d8e0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016d8f0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016d900: 2273 6563 7469 6f6e 2d63 6f6e 7465 6e74  "section-content
-0016d910: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016d920: 2020 2020 2020 2020 3c68 363e 4465 7065          <h6>Depe
-0016d930: 6e64 7320 4f6e 3c2f 6836 3e5c 6e20 2020  nds On</h6>\n   
-0016d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d950: 203c 7265 6665 7265 6e63 652d 6c69 7374   <reference-list
-0016d960: 2072 6566 6572 656e 6365 733d 2270 6172   references="par
-0016d970: 656e 7473 2220 6e6f 6465 3d22 6d6f 6465  ents" node="mode
-0016d980: 6c22 202f 3e5c 6e20 2020 2020 2020 2020  l" />\n         
-0016d990: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-0016d9a0: 2020 2020 2020 2020 2020 203c 2f73 6563             </sec
-0016d9b0: 7469 6f6e 3e5c 6e5c 6e20 2020 2020 2020  tion>\n\n       
-0016d9c0: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
-0016d9d0: 6173 733d 2273 6563 7469 6f6e 223e 5c6e  ass="section">\n
-0016d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d9f0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-0016da00: 696f 6e2d 7461 7267 6574 2220 6964 3d22  ion-target" id="
-0016da10: 636f 6465 223e 3c2f 6469 763e 5c6e 2020  code"></div>\n  
-0016da20: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0016da30: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
-0016da40: 6e2d 636f 6e74 656e 7422 3e5c 6e20 2020  n-content">\n   
-0016da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016da60: 203c 636f 6465 2d62 6c6f 636b 2076 6572   <code-block ver
-0016da70: 7369 6f6e 733d 2276 6572 7369 6f6e 7322  sions="versions"
-0016da80: 2064 6566 6175 6c74 3d22 6465 6661 756c   default="defaul
-0016da90: 745f 7665 7273 696f 6e22 206c 616e 6775  t_version" langu
-0016daa0: 6167 653d 226c 616e 6775 6167 6522 3e3c  age="language"><
-0016dab0: 2f63 6f64 652d 626c 6f63 6b3e 5c6e 2020  /code-block>\n  
-0016dac0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0016dad0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-0016dae0: 2020 3c2f 7365 6374 696f 6e3e 5c6e 2020    </section>\n  
-0016daf0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-0016db00: 2020 3c2f 6469 763e 5c6e 3c2f 6469 763e    </div>\n</div>
-0016db10: 5c6e 2729 7d5d 292c 652e 6578 706f 7274  \n')}]),e.export
-0016db20: 733d 6e7d 5d29 3b0a 2f2f 2320 736f 7572  s=n}]);.//# sour
-0016db30: 6365 4d61 7070 696e 6755 524c 3d6d 6169  ceMappingURL=mai
-0016db40: 6e2e 6a73 2e6d 6170 3c2f 7363 7269 7074  n.js.map</script
-0016db50: 3e3c 2f62 6f64 793e 0a3c 2f68 746d 6c3e  ></body>.</html>
-0016db60: 0a                                       .
+0016d470: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
+0016d480: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
+0016d490: 643d 2264 6573 6372 6970 7469 6f6e 223e  d="description">
+0016d4a0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016d4b0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016d4c0: 7373 3d22 7365 6374 696f 6e2d 636f 6e74  ss="section-cont
+0016d4d0: 656e 7422 3e5c 6e20 2020 2020 2020 2020  ent">\n         
+0016d4e0: 2020 2020 2020 2020 2020 203c 6836 3e44             <h6>D
+0016d4f0: 6573 6372 6970 7469 6f6e 3c2f 6836 3e5c  escription</h6>\
+0016d500: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016d510: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016d520: 2270 616e 656c 223e 5c6e 2020 2020 2020  "panel">\n      
+0016d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d540: 2020 3c64 6976 2063 6c61 7373 3d22 7061    <div class="pa
+0016d550: 6e65 6c2d 626f 6479 223e 5c6e 2020 2020  nel-body">\n    
+0016d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d570: 2020 2020 2020 2020 3c64 6976 206e 672d          <div ng-
+0016d580: 6966 3d22 6d6f 6465 6c2e 6465 7363 7269  if="model.descri
+0016d590: 7074 696f 6e22 2063 6c61 7373 3d22 6d6f  ption" class="mo
+0016d5a0: 6465 6c2d 6d61 726b 646f 776e 2220 6d61  del-markdown" ma
+0016d5b0: 726b 6564 3d22 6d6f 6465 6c2e 6465 7363  rked="model.desc
+0016d5c0: 7269 7074 696f 6e22 3e3c 2f64 6976 3e5c  ription"></div>\
+0016d5d0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016d5e0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016d5f0: 7620 6e67 2d69 663d 2221 6d6f 6465 6c2e  v ng-if="!model.
+0016d600: 6465 7363 7269 7074 696f 6e22 3e54 6869  description">Thi
+0016d610: 7320 7b7b 206d 6f64 656c 2e72 6573 6f75  s {{ model.resou
+0016d620: 7263 655f 7479 7065 207d 7d20 6973 206e  rce_type }} is n
+0016d630: 6f74 2063 7572 7265 6e74 6c79 2064 6f63  ot currently doc
+0016d640: 756d 656e 7465 643c 2f64 6976 3e5c 6e20  umented</div>\n 
+0016d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d660: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d680: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
+0016d690: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0016d6a0: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+0016d6b0: 2f73 6563 7469 6f6e 3e5c 6e5c 6e20 2020  /section>\n\n   
+0016d6c0: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
+0016d6d0: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
+0016d6e0: 2220 6e67 2d73 686f 7720 3d20 2270 6172  " ng-show = "par
+0016d6f0: 656e 7473 4c65 6e67 7468 2021 3d20 3022  entsLength != 0"
+0016d700: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016d710: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
+0016d720: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
+0016d730: 643d 2264 6570 656e 6473 5f6f 6e22 3e3c  d="depends_on"><
+0016d740: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+0016d750: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016d760: 733d 2273 6563 7469 6f6e 2d63 6f6e 7465  s="section-conte
+0016d770: 6e74 223e 5c6e 2020 2020 2020 2020 2020  nt">\n          
+0016d780: 2020 2020 2020 2020 2020 3c68 363e 4465            <h6>De
+0016d790: 7065 6e64 7320 4f6e 3c2f 6836 3e5c 6e20  pends On</h6>\n 
+0016d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d7b0: 2020 203c 7265 6665 7265 6e63 652d 6c69     <reference-li
+0016d7c0: 7374 2072 6566 6572 656e 6365 733d 2270  st references="p
+0016d7d0: 6172 656e 7473 2220 6e6f 6465 3d22 6d6f  arents" node="mo
+0016d7e0: 6465 6c22 202f 3e5c 6e20 2020 2020 2020  del" />\n       
+0016d7f0: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+0016d800: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
+0016d810: 6563 7469 6f6e 3e5c 6e5c 6e20 2020 2020  ection>\n\n     
+0016d820: 2020 2020 2020 203c 7365 6374 696f 6e20         <section 
+0016d830: 636c 6173 733d 2273 6563 7469 6f6e 223e  class="section">
+0016d840: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016d850: 2020 3c64 6976 2063 6c61 7373 3d22 7365    <div class="se
+0016d860: 6374 696f 6e2d 7461 7267 6574 2220 6964  ction-target" id
+0016d870: 3d22 636f 6465 223e 3c2f 6469 763e 5c6e  ="code"></div>\n
+0016d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d890: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+0016d8a0: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
+0016d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d8c0: 2020 203c 636f 6465 2d62 6c6f 636b 2076     <code-block v
+0016d8d0: 6572 7369 6f6e 733d 2276 6572 7369 6f6e  ersions="version
+0016d8e0: 7322 2064 6566 6175 6c74 3d22 6465 6661  s" default="defa
+0016d8f0: 756c 745f 7665 7273 696f 6e22 206c 616e  ult_version" lan
+0016d900: 6775 6167 653d 226c 616e 6775 6167 6522  guage="language"
+0016d910: 3e3c 2f63 6f64 652d 626c 6f63 6b3e 5c6e  ></code-block>\n
+0016d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d930: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016d940: 2020 2020 3c2f 7365 6374 696f 6e3e 5c6e      </section>\n
+0016d950: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+0016d960: 2020 2020 3c2f 6469 763e 5c6e 3c2f 6469      </div>\n</di
+0016d970: 763e 5c6e 2729 7d5d 292c 652e 6578 706f  v>\n')}]),e.expo
+0016d980: 7274 733d 6e7d 5d29 3b0a 2f2f 2320 736f  rts=n}]);.//# so
+0016d990: 7572 6365 4d61 7070 696e 6755 524c 3d6d  urceMappingURL=m
+0016d9a0: 6169 6e2e 6a73 2e6d 6170 3c2f 7363 7269  ain.js.map</scri
+0016d9b0: 7074 3e3c 2f62 6f64 793e 0a3c 2f68 746d  pt></body>.</htm
+0016d9c0: 6c3e 0a                                  l>.
```

### Comparing `dbt-core-1.6.0rc1/dbt/include/starter_project/README.md` & `dbt-core-1.6.0rc2/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.6.0rc2/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/internal_deprecations.py` & `dbt-core-1.6.0rc2/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/logger.py` & `dbt-core-1.6.0rc2/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/node_types.py` & `dbt-core-1.6.0rc2/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/__init__.py` & `dbt-core-1.6.0rc2/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/analysis.py` & `dbt-core-1.6.0rc2/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/base.py` & `dbt-core-1.6.0rc2/dbt/parser/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,15 @@
                 package_updaters[package_macro.package_name] = MacroGenerator(
                     package_macro, imported_macro_context
                 )
 
         self.package_updaters = package_updaters
         self.component = component
 
-    def __call__(self, parsed_node: Any, config_dict: Dict[str, Any]) -> None:
-        override = config_dict.get(self.component)
+    def __call__(self, parsed_node: Any, override: Optional[str]) -> None:
         if parsed_node.package_name in self.package_updaters:
             new_value = self.package_updaters[parsed_node.package_name](override, parsed_node)
         else:
             new_value = self.default_updater(override, parsed_node)
 
         if isinstance(new_value, str):
             new_value = new_value.strip()
@@ -276,17 +275,27 @@
         # re-mangle hooks, in case we got new ones
         self._mangle_hooks(final_config_dict)
         parsed_node.config = parsed_node.config.from_dict(final_config_dict)
 
     def update_parsed_node_relation_names(
         self, parsed_node: IntermediateNode, config_dict: Dict[str, Any]
     ) -> None:
-        self._update_node_database(parsed_node, config_dict)
-        self._update_node_schema(parsed_node, config_dict)
-        self._update_node_alias(parsed_node, config_dict)
+
+        # These call the RelationUpdate callable to go through generate_name macros
+        self._update_node_database(parsed_node, config_dict.get("database"))
+        self._update_node_schema(parsed_node, config_dict.get("schema"))
+        self._update_node_alias(parsed_node, config_dict.get("alias"))
+
+        # Snapshot nodes use special "target_database" and "target_schema" fields for some reason
+        if parsed_node.resource_type == NodeType.Snapshot:
+            if "target_database" in config_dict and config_dict["target_database"]:
+                parsed_node.database = config_dict["target_database"]
+            if "target_schema" in config_dict and config_dict["target_schema"]:
+                parsed_node.schema = config_dict["target_schema"]
+
         self._update_node_relation_name(parsed_node)
 
     def update_parsed_node_config(
         self,
         parsed_node: IntermediateNode,
         config: ContextConfig,
         context=None,
@@ -345,15 +354,15 @@
         )
 
         parsed_node.config_call_dict = config._config_call_dict
 
         # do this once before we parse the node database/schema/alias, so
         # parsed_node.config is what it would be if they did nothing
         self.update_parsed_node_config_dict(parsed_node, config_dict)
-        # This updates the node database/schema/alias
+        # This updates the node database/schema/alias/relation_name
         self.update_parsed_node_relation_names(parsed_node, config_dict)
 
         # tests don't have hooks
         if parsed_node.resource_type == NodeType.Test:
             return
 
         # at this point, we've collected our hooks. Use the node context to
```

### Comparing `dbt-core-1.6.0rc1/dbt/parser/common.py` & `dbt-core-1.6.0rc2/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/docs.py` & `dbt-core-1.6.0rc2/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/generic_test.py` & `dbt-core-1.6.0rc2/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/generic_test_builders.py` & `dbt-core-1.6.0rc2/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/hooks.py` & `dbt-core-1.6.0rc2/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/macros.py` & `dbt-core-1.6.0rc2/dbt/parser/macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
             if not macro.name.startswith(MACRO_PREFIX):
                 continue
 
             name: str = macro.name.replace(MACRO_PREFIX, "")
             node = self.parse_macro(block, base_node, name)
             # get supported_languages for materialization macro
-            if "materialization" in name:
+            if block.block_type_name == "materialization":
                 node.supported_languages = jinja.get_supported_languages(macro)
             yield node
 
     def parse_file(self, block: FileBlock):
         assert isinstance(block.file, SourceFile)
         source_file = block.file
         assert isinstance(source_file.contents, str)
```

### Comparing `dbt-core-1.6.0rc1/dbt/parser/manifest.py` & `dbt-core-1.6.0rc2/dbt/parser/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
     def check_for_model_deprecations(self):
         for node in self.manifest.nodes.values():
             if isinstance(node, ModelNode):
                 if (
                     node.deprecation_date
                     and node.deprecation_date < datetime.datetime.now().astimezone()
                 ):
-                    fire_event(
+                    warn_or_error(
                         DeprecatedModel(
                             model_name=node.name,
                             model_version=version_to_str(node.version),
                             deprecation_date=node.deprecation_date.isoformat(),
                         )
                     )
 
@@ -577,15 +577,15 @@
                     if resolved_ref.deprecation_date:
 
                         if resolved_ref.deprecation_date < datetime.datetime.now().astimezone():
                             event_cls = DeprecatedReference
                         else:
                             event_cls = UpcomingReferenceDeprecation
 
-                        fire_event(
+                        warn_or_error(
                             event_cls(
                                 model_name=node.name,
                                 ref_model_package=resolved_ref.package_name,
                                 ref_model_name=resolved_ref.name,
                                 ref_model_version=version_to_str(resolved_ref.version),
                                 ref_model_latest_version=str(resolved_ref.latest_version),
                                 ref_model_deprecation_date=resolved_ref.deprecation_date.isoformat(),
```

### Comparing `dbt-core-1.6.0rc1/dbt/parser/models.py` & `dbt-core-1.6.0rc2/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/partial.py` & `dbt-core-1.6.0rc2/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/read_files.py` & `dbt-core-1.6.0rc2/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/schema_generic_tests.py` & `dbt-core-1.6.0rc2/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/schema_renderer.py` & `dbt-core-1.6.0rc2/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/schema_yaml_readers.py` & `dbt-core-1.6.0rc2/dbt/parser/schema_yaml_readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,15 @@
             path=path,
             resource_type=NodeType.SemanticModel,
             unique_id=unique_id,
             entities=self._get_entities(unparsed.entities),
             measures=self._get_measures(unparsed.measures),
             dimensions=self._get_dimensions(unparsed.dimensions),
             defaults=unparsed.defaults,
+            primary_entity=unparsed.primary_entity,
         )
 
         ctx = generate_parse_semantic_models(
             parsed,
             self.root_project,
             self.schema_parser.manifest,
             package_name,
```

### Comparing `dbt-core-1.6.0rc1/dbt/parser/schemas.py` & `dbt-core-1.6.0rc2/dbt/parser/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/search.py` & `dbt-core-1.6.0rc2/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/seeds.py` & `dbt-core-1.6.0rc2/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/singular_test.py` & `dbt-core-1.6.0rc2/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/snapshots.py` & `dbt-core-1.6.0rc2/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/sources.py` & `dbt-core-1.6.0rc2/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/parser/sql.py` & `dbt-core-1.6.0rc2/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/plugins/__init__.py` & `dbt-core-1.6.0rc2/dbt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/plugins/manager.py` & `dbt-core-1.6.0rc2/dbt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/plugins/manifest.py` & `dbt-core-1.6.0rc2/dbt/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/semver.py` & `dbt-core-1.6.0rc2/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/base.py` & `dbt-core-1.6.0rc2/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/build.py` & `dbt-core-1.6.0rc2/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/clean.py` & `dbt-core-1.6.0rc2/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/clone.py` & `dbt-core-1.6.0rc2/dbt/task/clone.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/compile.py` & `dbt-core-1.6.0rc2/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/debug.py` & `dbt-core-1.6.0rc2/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/deps.py` & `dbt-core-1.6.0rc2/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/freshness.py` & `dbt-core-1.6.0rc2/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/generate.py` & `dbt-core-1.6.0rc2/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/init.py` & `dbt-core-1.6.0rc2/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/list.py` & `dbt-core-1.6.0rc2/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/printer.py` & `dbt-core-1.6.0rc2/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/retry.py` & `dbt-core-1.6.0rc2/dbt/task/retry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/run.py` & `dbt-core-1.6.0rc2/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/run_operation.py` & `dbt-core-1.6.0rc2/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/runnable.py` & `dbt-core-1.6.0rc2/dbt/task/runnable.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,23 +371,25 @@
             for r in self._flattened_nodes:
                 if r.unique_id not in executed_node_ids:
                     self.node_results.append(
                         RunResult.from_node(r, RunStatus.Skipped, "Skipping due to fail_fast")
                     )
 
             print_run_result_error(failure.result)
-            raise
+            # ensure information about all nodes is propagated to run results when failing fast
+            return self.node_results
         except KeyboardInterrupt:
             self._cancel_connections(pool)
             print_run_end_messages(self.node_results, keyboard_interrupt=True)
             raise
-        finally:
-            pool.close()
-            pool.join()
-            return self.node_results
+
+        pool.close()
+        pool.join()
+
+        return self.node_results
 
     def _mark_dependent_errors(self, node_id, result, cause):
         if self.graph is None:
             raise DbtInternalError("graph is None in _mark_dependent_errors")
         for dep_node_id in self.graph.get_dependent_nodes(node_id):
             self._skipped_children[dep_node_id] = cause
```

### Comparing `dbt-core-1.6.0rc1/dbt/task/seed.py` & `dbt-core-1.6.0rc2/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/serve.py` & `dbt-core-1.6.0rc2/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/show.py` & `dbt-core-1.6.0rc2/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/snapshot.py` & `dbt-core-1.6.0rc2/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/sql.py` & `dbt-core-1.6.0rc2/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/task/test.py` & `dbt-core-1.6.0rc2/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/tests/fixtures/project.py` & `dbt-core-1.6.0rc2/dbt/tests/fixtures/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,14 +498,15 @@
         USE_COLORS=False,
         USE_COLORS_FILE=False,
         LOG_LEVEL="info",
         LOG_LEVEL_FILE="debug",
         DEBUG=False,
         LOG_CACHE_EVENTS=False,
         QUIET=False,
+        LOG_FILE_MAX_BYTES=1000000,
     )
     setup_event_logger(log_flags)
     orig_cwd = os.getcwd()
     os.chdir(project_root)
     # Return whatever is needed later in tests but can only come from fixtures, so we can keep
     # the signatures in the test signature to a minimum.
     project = TestProjInfo(
```

### Comparing `dbt-core-1.6.0rc1/dbt/tests/util.py` & `dbt-core-1.6.0rc2/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/tracking.py` & `dbt-core-1.6.0rc2/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/ui.py` & `dbt-core-1.6.0rc2/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/dbt/utils.py` & `dbt-core-1.6.0rc2/dbt/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 import requests
 import sys
 from tarfile import ReadError
 import time
 from pathlib import PosixPath, WindowsPath
 
 from contextlib import contextmanager
-from dbt.exceptions import ConnectionError, DuplicateAliasError
-from dbt.events.functions import fire_event
 from dbt.events.types import RetryExternalCall, RecordRetryException
+from dbt.helper_types import WarnErrorOptions
 from dbt import flags
 from enum import Enum
 from typing_extensions import Protocol
 from typing import (
     Tuple,
     Type,
     Any,
@@ -36,14 +35,15 @@
     Mapping,
     Iterable,
     AbstractSet,
     Set,
     Sequence,
 )
 
+import dbt.events.functions
 import dbt.exceptions
 
 DECIMALS: Tuple[Type[Any], ...]
 try:
     import cdecimal  # typing: ignore
 except ImportError:
     DECIMALS = (decimal.Decimal,)
@@ -333,23 +333,26 @@
     handles `Decimal`s and `Undefined`s. Decimals can lose precision because
     they get converted to floats. Undefined's are serialized to an empty string
     """
 
     def default(self, obj):
         if isinstance(obj, DECIMALS):
             return float(obj)
-        if isinstance(obj, (datetime.datetime, datetime.date, datetime.time)):
+        elif isinstance(obj, (datetime.datetime, datetime.date, datetime.time)):
             return obj.isoformat()
-        if isinstance(obj, jinja2.Undefined):
+        elif isinstance(obj, jinja2.Undefined):
             return ""
-        if hasattr(obj, "to_dict"):
+        elif isinstance(obj, Exception):
+            return repr(obj)
+        elif hasattr(obj, "to_dict"):
             # if we have a to_dict we should try to serialize the result of
             # that!
             return obj.to_dict(omit_none=True)
-        return super().default(obj)
+        else:
+            return super().default(obj)
 
 
 class ForgivingJSONEncoder(JSONEncoder):
     def default(self, obj):
         # let dbt's default JSON encoder handle it if possible, fallback to
         # str()
         try:
@@ -365,15 +368,15 @@
 
     def translate_mapping(self, kwargs: Mapping[str, Any]) -> Dict[str, Any]:
         result: Dict[str, Any] = {}
 
         for key, value in kwargs.items():
             canonical_key = self.aliases.get(key, key)
             if canonical_key in result:
-                raise DuplicateAliasError(kwargs, self.aliases, canonical_key)
+                raise dbt.exceptions.DuplicateAliasError(kwargs, self.aliases, canonical_key)
             result[canonical_key] = self.translate_value(value)
         return result
 
     def translate_sequence(self, value: Sequence[Any]) -> List[Any]:
         return [self.translate_value(v) for v in value]
 
     def translate_value(self, value: Any) -> Any:
@@ -385,17 +388,15 @@
         return value
 
     def translate(self, value: Mapping[str, Any]) -> Dict[str, Any]:
         try:
             return self.translate_mapping(value)
         except RuntimeError as exc:
             if "maximum recursion depth exceeded" in str(exc):
-                raise dbt.exceptions.RecursionError(
-                    "Cycle detected in a value passed to translate!"
-                )
+                raise RecursionError("Cycle detected in a value passed to translate!")
             raise
 
 
 def translate_aliases(
     kwargs: Dict[str, Any],
     aliases: Dict[str, str],
     recurse: bool = False,
@@ -599,20 +600,22 @@
     try:
         return fn()
     except (
         requests.exceptions.RequestException,
         ReadError,
     ) as exc:
         if attempt <= max_attempts - 1:
-            fire_event(RecordRetryException(exc=str(exc)))
-            fire_event(RetryExternalCall(attempt=attempt, max=max_attempts))
+            dbt.events.functions.fire_event(RecordRetryException(exc=str(exc)))
+            dbt.events.functions.fire_event(RetryExternalCall(attempt=attempt, max=max_attempts))
             time.sleep(1)
             return _connection_exception_retry(fn, max_attempts, attempt + 1)
         else:
-            raise ConnectionError("External connection exception occurred: " + str(exc))
+            raise dbt.exceptions.ConnectionError(
+                "External connection exception occurred: " + str(exc)
+            )
 
 
 # This is used to serialize the args in the run_results and in the logs.
 # We do this separately because there are a few fields that don't serialize,
 # i.e. PosixPath, WindowsPath, and types. It also includes args from both
 # cli args and flags, which is more complete than just the cli args.
 # If new args are added that are false by default (particularly in the
@@ -648,14 +651,17 @@
         if key in default_false_keys and var_args[key] is False:
             continue
         if key in default_empty_yaml_dict_keys and var_args[key] == "{}":
             continue
         # this was required for a test case
         if isinstance(var_args[key], PosixPath) or isinstance(var_args[key], WindowsPath):
             var_args[key] = str(var_args[key])
+        if isinstance(var_args[key], WarnErrorOptions):
+            var_args[key] = var_args[key].to_dict()
+
         dict_args[key] = var_args[key]
     return dict_args
 
 
 # This is useful for proto generated classes in particular, since
 # the default for protobuf for strings is the empty string, so
 # Optional[str] types don't work for generated Python classes.
```

### Comparing `dbt-core-1.6.0rc1/dbt/version.py` & `dbt-core-1.6.0rc2/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.6.0rc1"
+__version__ = "1.6.0rc2"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.6.0rc1/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.6.0rc2/dbt_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0rc1
+Version: 1.6.0rc2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0rc1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0rc2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0rc1/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.6.0rc2/dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0rc1/setup.py` & `dbt-core-1.6.0rc2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.6.0rc1"
+package_version = "1.6.0rc2"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -55,34 +55,31 @@
         # ----
         # Legacy: This package has not been updated since 2019, and it is unused in dbt's logging system (since v1.0)
         # The dependency here will be removed along with the removal of 'legacy logging', in a future release of dbt-core
         "logbook>=1.5,<1.6",
         # ----
         # dbt-core uses these packages in standard ways. Pin to the major version, and check compatibility
         # with major versions in each new minor version of dbt-core.
-        # temporarily pinning click for mypy failures: https://github.com/pallets/click/issues/2558
-        "click>=8.1.1,<8.1.4",
+        "click<9",
         "networkx>=2.3,<4",
         # ----
         # These packages are major-version-0. Keep upper bounds on upcoming minor versions (which could have breaking changes)
         # and check compatibility / bump in each new minor version of dbt-core.
         "colorama>=0.3.9,<0.5",
         "pathspec>=0.9,<0.12",
         "isodate>=0.6,<0.7",
         # ----
-        # There was a pin to below 0.4.4 for a while due to a bug in Ubuntu/sqlparse 0.4.4
-        "sqlparse>=0.2.3",
+        "sqlparse>=0.2.3,<0.5",
         # ----
         # These are major-version-0 packages also maintained by dbt-labs. Accept patches.
         "dbt-extractor~=0.4.1",
         "hologram~=0.0.16",  # includes transitive dependencies on python-dateutil and jsonschema
         "minimal-snowplow-tracker~=0.0.2",
         # DSI is under active development, so we're pinning to specific dev versions for now.
-        # TODO: Before RC/final release, update to use ~= pinning.
-        "dbt-semantic-interfaces~=0.1.0rc1",
+        "dbt-semantic-interfaces~=0.2.0",
         # ----
         # Expect compatibility with all new versions of these packages, so lower bounds only.
         "packaging>20.9",
         "protobuf>=4.0.0",
         "pytz>=2015.7",
         "pyyaml>=6.0",
         "typing-extensions>=3.7.4",
```

