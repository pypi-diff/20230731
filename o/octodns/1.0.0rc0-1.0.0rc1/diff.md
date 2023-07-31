# Comparing `tmp/octodns-1.0.0rc0.tar.gz` & `tmp/octodns-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-1.0.0rc0.tar", last modified: Wed May 17 16:58:26 2023, max compression
+gzip compressed data, was "octodns-1.0.0rc1.tar", last modified: Wed Jul 26 16:44:58 2023, max compression
```

## Comparing `octodns-1.0.0rc0.tar` & `octodns-1.0.0rc1.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/
--rw-r--r--   0 neo       (1000) neo       (1000)    26907 2023-05-17 16:57:30.000000 octodns-1.0.0rc0/CHANGELOG.md
--rw-r--r--   0 neo       (1000) neo       (1000)     3229 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/CODE_OF_CONDUCT.md
--rw-r--r--   0 neo       (1000) neo       (1000)     3761 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/CONTRIBUTING.md
--rw-r--r--   0 neo       (1000) neo       (1000)     1056 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/LICENSE
--rw-r--r--   0 neo       (1000) neo       (1000)      292 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/MANIFEST.in
--rw-r--r--   0 neo       (1000) neo       (1000)    26279 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)    26000 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/README.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.530521 octodns-1.0.0rc0/docs/
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.530521 octodns-1.0.0rc0/docs/assets/
--rw-r--r--   0 neo       (1000) neo       (1000)    82371 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/assets/deploy.png
--rw-r--r--   0 neo       (1000) neo       (1000)    75814 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/assets/noop.png
--rw-r--r--   0 neo       (1000) neo       (1000)   212872 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/assets/pr.png
--rw-r--r--   0 neo       (1000) neo       (1000)     2917 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/docs/auto_arpa.md
--rw-r--r--   0 neo       (1000) neo       (1000)     7482 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/docs/dynamic_records.md
--rw-r--r--   0 neo       (1000) neo       (1000)     3427 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/geo_records.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.530521 octodns-1.0.0rc0/docs/logos/
--rw-r--r--   0 neo       (1000) neo       (1000)     3983 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/logos/octodns-logo.png
--rw-r--r--   0 neo       (1000) neo       (1000)     7720 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/docs/records.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.533854 octodns-1.0.0rc0/octodns/
--rw-r--r--   0 neo       (1000) neo       (1000)      101 2023-05-17 16:57:30.000000 octodns-1.0.0rc0/octodns/__init__.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.533854 octodns-1.0.0rc0/octodns/cmds/
--rw-r--r--   0 neo       (1000) neo       (1000)        6 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/__init__.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3786 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/cmds/args.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1423 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/cmds/compare.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1536 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/dump.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)     3360 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/cmds/report.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1544 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/sync.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)      517 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/validate.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)      444 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/versions.py
--rw-r--r--   0 neo       (1000) neo       (1000)      717 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/equality.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2373 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/idna.py
--rw-r--r--   0 neo       (1000) neo       (1000)    32891 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/manager.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.537188 octodns-1.0.0rc0/octodns/processor/
--rw-r--r--   0 neo       (1000) neo       (1000)        6 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/__init__.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1824 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/acme.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2153 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/processor/arpa.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2960 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/base.py
--rw-r--r--   0 neo       (1000) neo       (1000)     5052 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/processor/filter.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3664 2023-05-16 17:41:42.000000 octodns-1.0.0rc0/octodns/processor/ownership.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2276 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/restrict.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3803 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/processor/spf.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.537188 octodns-1.0.0rc0/octodns/provider/
--rw-r--r--   0 neo       (1000) neo       (1000)      108 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/provider/__init__.py
--rw-r--r--   0 neo       (1000) neo       (1000)    12356 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/provider/base.py
--rw-r--r--   0 neo       (1000) neo       (1000)    11096 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/provider/plan.py
--rw-r--r--   0 neo       (1000) neo       (1000)    12103 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/provider/yaml.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.543854 octodns-1.0.0rc0/octodns/record/
--rw-r--r--   0 neo       (1000) neo       (1000)     1471 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/__init__.py
--rw-r--r--   0 neo       (1000) neo       (1000)      412 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/a.py
--rw-r--r--   0 neo       (1000) neo       (1000)      423 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/aaaa.py
--rw-r--r--   0 neo       (1000) neo       (1000)      488 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/alias.py
--rw-r--r--   0 neo       (1000) neo       (1000)    10392 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/base.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2342 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/caa.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1407 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/change.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1495 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/chunked.py
--rw-r--r--   0 neo       (1000) neo       (1000)      534 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/cname.py
--rw-r--r--   0 neo       (1000) neo       (1000)      296 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/dname.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3442 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ds.py
--rw-r--r--   0 neo       (1000) neo       (1000)    15080 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/record/dynamic.py
--rw-r--r--   0 neo       (1000) neo       (1000)      450 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/exception.py
--rw-r--r--   0 neo       (1000) neo       (1000)     5311 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/geo.py
--rw-r--r--   0 neo       (1000) neo       (1000)    13426 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/octodns/record/geo_data.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1385 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ip.py
--rw-r--r--   0 neo       (1000) neo       (1000)    10626 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/loc.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3328 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/mx.py
--rw-r--r--   0 neo       (1000) neo       (1000)     4382 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/naptr.py
--rw-r--r--   0 neo       (1000) neo       (1000)      235 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ns.py
--rw-r--r--   0 neo       (1000) neo       (1000)      412 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ptr.py
--rw-r--r--   0 neo       (1000) neo       (1000)      644 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/rr.py
--rw-r--r--   0 neo       (1000) neo       (1000)      220 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/spf.py
--rw-r--r--   0 neo       (1000) neo       (1000)     4223 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/srv.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3491 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/sshfp.py
--rw-r--r--   0 neo       (1000) neo       (1000)      465 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/record/subnet.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2000 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/target.py
--rw-r--r--   0 neo       (1000) neo       (1000)     4987 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/tlsa.py
--rw-r--r--   0 neo       (1000) neo       (1000)      257 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/txt.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3263 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/urlfwd.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.543854 octodns-1.0.0rc0/octodns/source/
--rw-r--r--   0 neo       (1000) neo       (1000)        6 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/source/__init__.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1713 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/source/base.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3280 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/source/envvar.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)     8240 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/source/tinydns.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2194 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/yaml.py
--rw-r--r--   0 neo       (1000) neo       (1000)    10479 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/zone.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.533854 octodns-1.0.0rc0/octodns.egg-info/
--rw-r--r--   0 neo       (1000) neo       (1000)    26279 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)     6243 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/SOURCES.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/dependency_links.txt
--rw-r--r--   0 neo       (1000) neo       (1000)      272 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/entry_points.txt
--rw-r--r--   0 neo       (1000) neo       (1000)      292 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/requires.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        8 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/top_level.txt
--rw-r--r--   0 neo       (1000) neo       (1000)      209 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/pyproject.toml
--rw-r--r--   0 neo       (1000) neo       (1000)      943 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/requirements-dev.txt
--rw-r--r--   0 neo       (1000) neo       (1000)      179 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/requirements.txt
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.547188 octodns-1.0.0rc0/script/
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1273 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/bootstrap
--rwxr-xr-x   0 neo       (1000) neo       (1000)      177 2021-10-12 19:58:05.000000 octodns-1.0.0rc0/script/changelog
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1085 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/cibuild
--rwxr-xr-x   0 neo       (1000) neo       (1000)      796 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/cibuild-setup-py
--rwxr-xr-x   0 neo       (1000) neo       (1000)      998 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/script/coverage
--rwxr-xr-x   0 neo       (1000) neo       (1000)      184 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/format
--rwxr-xr-x   0 neo       (1000) neo       (1000)     2486 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/generate-geo-data
--rwxr-xr-x   0 neo       (1000) neo       (1000)      387 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/lint
--rwxr-xr-x   0 neo       (1000) neo       (1000)      738 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/script/release
--rwxr-xr-x   0 neo       (1000) neo       (1000)      283 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/script/sdist
--rwxr-xr-x   0 neo       (1000) neo       (1000)      662 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/script/test
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1705 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/test-module
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1940 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/update-requirements
--rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/setup.cfg
--rw-r--r--   0 neo       (1000) neo       (1000)     2907 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/setup.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.553855 octodns-1.0.0rc0/tests/
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/
--rw-r--r--   0 neo       (1000) neo       (1000)      363 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/alias-zone-loop.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      447 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/always-dry-run.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      129 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-plan-output-config.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       63 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-plan-output-missing-class.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       81 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-provider-class-module.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       59 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-provider-class-no-module.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       67 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-provider-class.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)     4749 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/tests/config/dynamic.tests.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)        4 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/empty.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       32 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-provider-class.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       75 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-provider-config.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      121 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-provider-env.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       44 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-sources.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      235 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/no-dump.yaml
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/override/
--rw-r--r--   0 neo       (1000) neo       (1000)      167 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/override/dynamic.tests.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      115 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/plan-output-filehandle.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      389 2021-06-25 17:49:24.000000 octodns-1.0.0rc0/tests/config/processors-missing-class.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      493 2021-06-25 17:49:24.000000 octodns-1.0.0rc0/tests/config/processors-wants-config.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      940 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/processors.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      461 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/provider-problems.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      400 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/simple-alias-zone.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      626 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/simple-arpa.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      841 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/simple-split.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      216 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/simple-validate.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)     1016 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/simple.yaml
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.527188 octodns-1.0.0rc0/tests/config/split/
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/
--rw-r--r--   0 neo       (1000) neo       (1000)      749 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/a.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      993 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/aaaa.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      785 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/cname.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)     1689 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/real-ish-a.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      277 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/simple-weighted.yaml
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/
--rw-r--r--   0 neo       (1000) neo       (1000)       38 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/12.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       36 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/2.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       37 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/test.yaml
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.567188 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/
--rw-r--r--   0 neo       (1000) neo       (1000)      640 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/$unit.tests.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      198 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/_srv._tcp.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       81 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/aaaa.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/cname.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/dname.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       85 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/excluded.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       69 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/ignored.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       85 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/included.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      248 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/mx.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      313 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/naptr.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-08-20 18:14:19.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/ptr.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       71 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/spf.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       56 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/sub.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      166 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/txt.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      241 2021-07-27 03:02:31.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/urlfwd.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       51 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/www.sub.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       47 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/www.yaml
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.567188 octodns-1.0.0rc0/tests/config/split/unordered.tst/
--rw-r--r--   0 neo       (1000) neo       (1000)       36 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unordered.tst/abc.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unordered.tst/xyz.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)        4 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/config/sub.txt.unit.tests.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       99 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/subzone.unit.tests.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)     3328 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/config/unit.tests.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      307 2021-06-25 17:49:24.000000 octodns-1.0.0rc0/tests/config/unknown-processor.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      217 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/unknown-provider.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)      328 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/unknown-source-zone.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)       89 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/unordered.yaml
--rw-r--r--   0 neo       (1000) neo       (1000)     2874 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/helpers.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1579 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_equality.py
--rw-r--r--   0 neo       (1000) neo       (1000)     4690 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_idna.py
--rw-r--r--   0 neo       (1000) neo       (1000)    38035 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_manager.py
--rw-r--r--   0 neo       (1000) neo       (1000)     9527 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_plan.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3135 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_processor_acme.py
--rw-r--r--   0 neo       (1000) neo       (1000)     7812 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_processor_arpa.py
--rw-r--r--   0 neo       (1000) neo       (1000)     6302 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_processor_filter.py
--rw-r--r--   0 neo       (1000) neo       (1000)     5156 2023-05-16 17:41:42.000000 octodns-1.0.0rc0/tests/test_octodns_processor_ownership.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3653 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_processor_restrict.py
--rw-r--r--   0 neo       (1000) neo       (1000)    12859 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_processor_spf.py
--rw-r--r--   0 neo       (1000) neo       (1000)    33602 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/tests/test_octodns_provider_base.py
--rw-r--r--   0 neo       (1000) neo       (1000)    22494 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_provider_yaml.py
--rw-r--r--   0 neo       (1000) neo       (1000)    17628 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record.py
--rw-r--r--   0 neo       (1000) neo       (1000)     6241 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_a.py
--rw-r--r--   0 neo       (1000) neo       (1000)     7294 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_aaaa.py
--rw-r--r--   0 neo       (1000) neo       (1000)     3468 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_alias.py
--rw-r--r--   0 neo       (1000) neo       (1000)     8813 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_caa.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2926 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_change.py
--rw-r--r--   0 neo       (1000) neo       (1000)      952 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_chunked.py
--rw-r--r--   0 neo       (1000) neo       (1000)     4291 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_cname.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2879 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_dname.py
--rw-r--r--   0 neo       (1000) neo       (1000)     6371 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ds.py
--rw-r--r--   0 neo       (1000) neo       (1000)    53366 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/tests/test_octodns_record_dynamic.py
--rw-r--r--   0 neo       (1000) neo       (1000)     9241 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_geo.py
--rw-r--r--   0 neo       (1000) neo       (1000)      681 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ip.py
--rw-r--r--   0 neo       (1000) neo       (1000)    23625 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_loc.py
--rw-r--r--   0 neo       (1000) neo       (1000)     8611 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_mx.py
--rw-r--r--   0 neo       (1000) neo       (1000)    12946 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_naptr.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2537 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ns.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2802 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ptr.py
--rw-r--r--   0 neo       (1000) neo       (1000)     2166 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_spf.py
--rw-r--r--   0 neo       (1000) neo       (1000)    13678 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_srv.py
--rw-r--r--   0 neo       (1000) neo       (1000)    10648 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_sshfp.py
--rw-r--r--   0 neo       (1000) neo       (1000)      738 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_target.py
--rw-r--r--   0 neo       (1000) neo       (1000)    14105 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_tlsa.py
--rw-r--r--   0 neo       (1000) neo       (1000)     5264 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_txt.py
--rw-r--r--   0 neo       (1000) neo       (1000)    12418 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_urlfwd.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1419 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_source_envvar.py
--rw-r--r--   0 neo       (1000) neo       (1000)     6080 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_source_tinydns.py
--rw-r--r--   0 neo       (1000) neo       (1000)     1402 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_yaml.py
--rw-r--r--   0 neo       (1000) neo       (1000)    18104 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_zone.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/tests/zones/
--rw-r--r--   0 neo       (1000) neo       (1000)      599 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/zones/2.0.192.in-addr.arpa.
--rw-r--r--   0 neo       (1000) neo       (1000)      474 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/ext.unit.tests.extension
--rw-r--r--   0 neo       (1000) neo       (1000)     1541 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/invalid.records.tst
--rw-r--r--   0 neo       (1000) neo       (1000)      362 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/invalid.zone.tst
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/tests/zones/tinydns/
--rw-r--r--   0 neo       (1000) neo       (1000)     1024 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/tinydns/.is-needed-for-tests
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1345 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/zones/tinydns/example.com
--rw-r--r--   0 neo       (1000) neo       (1000)      166 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/tinydns/other.foo
--rw-r--r--   0 neo       (1000) neo       (1000)     1769 2022-01-14 22:24:33.000000 octodns-1.0.0rc0/tests/zones/unit.tests.
--rw-r--r--   0 neo       (1000) neo       (1000)     1932 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/zones/unit.tests.tst
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.652312 octodns-1.0.0rc1/
+-rw-r--r--   0 ross       (501) staff       (20)    27486 2023-07-26 16:44:25.000000 octodns-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0 ross       (501) staff       (20)     3229 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ross       (501) staff       (20)     3761 2022-09-27 14:17:03.000000 octodns-1.0.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 ross       (501) staff       (20)     1056 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)      292 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 ross       (501) staff       (20)    26279 2023-07-26 16:44:58.651893 octodns-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)    26000 2023-04-06 23:34:30.000000 octodns-1.0.0rc1/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.535249 octodns-1.0.0rc1/docs/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.541467 octodns-1.0.0rc1/docs/assets/
+-rw-r--r--   0 ross       (501) staff       (20)    82371 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/docs/assets/deploy.png
+-rw-r--r--   0 ross       (501) staff       (20)    75814 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/docs/assets/noop.png
+-rw-r--r--   0 ross       (501) staff       (20)   212872 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/docs/assets/pr.png
+-rw-r--r--   0 ross       (501) staff       (20)     2917 2023-02-27 17:58:31.000000 octodns-1.0.0rc1/docs/auto_arpa.md
+-rw-r--r--   0 ross       (501) staff       (20)     7451 2023-06-28 20:20:17.000000 octodns-1.0.0rc1/docs/dynamic_records.md
+-rw-r--r--   0 ross       (501) staff       (20)     3427 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/docs/geo_records.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.545086 octodns-1.0.0rc1/docs/logos/
+-rw-r--r--   0 ross       (501) staff       (20)     3983 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/docs/logos/octodns-logo.png
+-rw-r--r--   0 ross       (501) staff       (20)     7720 2022-07-22 22:56:06.000000 octodns-1.0.0rc1/docs/records.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.550966 octodns-1.0.0rc1/octodns/
+-rw-r--r--   0 ross       (501) staff       (20)      100 2023-07-26 16:44:25.000000 octodns-1.0.0rc1/octodns/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.556761 octodns-1.0.0rc1/octodns/cmds/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/cmds/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     3786 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/octodns/cmds/args.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     1423 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/octodns/cmds/compare.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     1536 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/cmds/dump.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     3554 2023-06-25 04:24:05.000000 octodns-1.0.0rc1/octodns/cmds/report.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     1544 2022-09-29 21:34:41.000000 octodns-1.0.0rc1/octodns/cmds/sync.py
+-rwxr-xr-x   0 ross       (501) staff       (20)      517 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/cmds/validate.py
+-rwxr-xr-x   0 ross       (501) staff       (20)      444 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/cmds/versions.py
+-rw-r--r--   0 ross       (501) staff       (20)      717 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/equality.py
+-rw-r--r--   0 ross       (501) staff       (20)     2373 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/octodns/idna.py
+-rw-r--r--   0 ross       (501) staff       (20)    32890 2023-07-26 16:26:11.000000 octodns-1.0.0rc1/octodns/manager.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.561414 octodns-1.0.0rc1/octodns/processor/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/processor/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     1824 2022-09-29 21:34:52.000000 octodns-1.0.0rc1/octodns/processor/acme.py
+-rw-r--r--   0 ross       (501) staff       (20)     2286 2023-06-20 14:38:33.000000 octodns-1.0.0rc1/octodns/processor/arpa.py
+-rw-r--r--   0 ross       (501) staff       (20)     2960 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/processor/base.py
+-rw-r--r--   0 ross       (501) staff       (20)     5052 2023-01-22 16:25:39.000000 octodns-1.0.0rc1/octodns/processor/filter.py
+-rw-r--r--   0 ross       (501) staff       (20)     3836 2023-06-25 04:24:05.000000 octodns-1.0.0rc1/octodns/processor/ownership.py
+-rw-r--r--   0 ross       (501) staff       (20)     2276 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/processor/restrict.py
+-rw-r--r--   0 ross       (501) staff       (20)     3803 2023-02-20 21:03:39.000000 octodns-1.0.0rc1/octodns/processor/spf.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.564393 octodns-1.0.0rc1/octodns/provider/
+-rw-r--r--   0 ross       (501) staff       (20)      108 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/provider/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    12356 2023-05-19 16:41:48.000000 octodns-1.0.0rc1/octodns/provider/base.py
+-rw-r--r--   0 ross       (501) staff       (20)    11255 2023-06-25 04:24:05.000000 octodns-1.0.0rc1/octodns/provider/plan.py
+-rw-r--r--   0 ross       (501) staff       (20)    12103 2023-07-26 16:26:11.000000 octodns-1.0.0rc1/octodns/provider/yaml.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.581976 octodns-1.0.0rc1/octodns/record/
+-rw-r--r--   0 ross       (501) staff       (20)     1471 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/octodns/record/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)      412 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/a.py
+-rw-r--r--   0 ross       (501) staff       (20)      423 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/aaaa.py
+-rw-r--r--   0 ross       (501) staff       (20)      488 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/alias.py
+-rw-r--r--   0 ross       (501) staff       (20)    10633 2023-07-18 23:53:10.000000 octodns-1.0.0rc1/octodns/record/base.py
+-rw-r--r--   0 ross       (501) staff       (20)     2342 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/caa.py
+-rw-r--r--   0 ross       (501) staff       (20)     1407 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/change.py
+-rw-r--r--   0 ross       (501) staff       (20)     1495 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/octodns/record/chunked.py
+-rw-r--r--   0 ross       (501) staff       (20)      534 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/cname.py
+-rw-r--r--   0 ross       (501) staff       (20)      296 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/dname.py
+-rw-r--r--   0 ross       (501) staff       (20)     3442 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/ds.py
+-rw-r--r--   0 ross       (501) staff       (20)    15080 2023-05-19 16:41:48.000000 octodns-1.0.0rc1/octodns/record/dynamic.py
+-rw-r--r--   0 ross       (501) staff       (20)      452 2023-05-19 19:16:44.000000 octodns-1.0.0rc1/octodns/record/exception.py
+-rw-r--r--   0 ross       (501) staff       (20)     5311 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/octodns/record/geo.py
+-rw-r--r--   0 ross       (501) staff       (20)    13426 2023-04-05 21:50:25.000000 octodns-1.0.0rc1/octodns/record/geo_data.py
+-rw-r--r--   0 ross       (501) staff       (20)     1385 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/ip.py
+-rw-r--r--   0 ross       (501) staff       (20)    10626 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/loc.py
+-rw-r--r--   0 ross       (501) staff       (20)     3328 2023-07-26 16:26:49.000000 octodns-1.0.0rc1/octodns/record/mx.py
+-rw-r--r--   0 ross       (501) staff       (20)     4382 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/naptr.py
+-rw-r--r--   0 ross       (501) staff       (20)      235 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/ns.py
+-rw-r--r--   0 ross       (501) staff       (20)      412 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/ptr.py
+-rw-r--r--   0 ross       (501) staff       (20)      644 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/rr.py
+-rw-r--r--   0 ross       (501) staff       (20)      220 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/spf.py
+-rw-r--r--   0 ross       (501) staff       (20)     4223 2023-07-26 16:26:49.000000 octodns-1.0.0rc1/octodns/record/srv.py
+-rw-r--r--   0 ross       (501) staff       (20)     3491 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/sshfp.py
+-rw-r--r--   0 ross       (501) staff       (20)      465 2023-05-19 16:41:48.000000 octodns-1.0.0rc1/octodns/record/subnet.py
+-rw-r--r--   0 ross       (501) staff       (20)     2000 2023-07-26 16:26:49.000000 octodns-1.0.0rc1/octodns/record/target.py
+-rw-r--r--   0 ross       (501) staff       (20)     4987 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/tlsa.py
+-rw-r--r--   0 ross       (501) staff       (20)      257 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/txt.py
+-rw-r--r--   0 ross       (501) staff       (20)     3263 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/octodns/record/urlfwd.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.583595 octodns-1.0.0rc1/octodns/source/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/octodns/source/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     1712 2023-05-23 20:27:03.000000 octodns-1.0.0rc1/octodns/source/base.py
+-rw-r--r--   0 ross       (501) staff       (20)     3280 2022-09-29 21:34:52.000000 octodns-1.0.0rc1/octodns/source/envvar.py
+-rwxr-xr-x   0 ross       (501) staff       (20)    15823 2023-07-17 16:02:15.000000 octodns-1.0.0rc1/octodns/source/tinydns.py
+-rw-r--r--   0 ross       (501) staff       (20)     2194 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/octodns/yaml.py
+-rw-r--r--   0 ross       (501) staff       (20)    11392 2023-07-17 16:02:15.000000 octodns-1.0.0rc1/octodns/zone.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.553553 octodns-1.0.0rc1/octodns.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)    26279 2023-07-26 16:44:58.000000 octodns-1.0.0rc1/octodns.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     6243 2023-07-26 16:44:58.000000 octodns-1.0.0rc1/octodns.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-07-26 16:44:58.000000 octodns-1.0.0rc1/octodns.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      272 2023-07-26 16:44:58.000000 octodns-1.0.0rc1/octodns.egg-info/entry_points.txt
+-rw-r--r--   0 ross       (501) staff       (20)      300 2023-07-26 16:44:58.000000 octodns-1.0.0rc1/octodns.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)        8 2023-07-26 16:44:58.000000 octodns-1.0.0rc1/octodns.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      209 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)      910 2023-06-28 23:41:11.000000 octodns-1.0.0rc1/requirements-dev.txt
+-rw-r--r--   0 ross       (501) staff       (20)      179 2023-06-28 23:41:11.000000 octodns-1.0.0rc1/requirements.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.589341 octodns-1.0.0rc1/script/
+-rwxr-xr-x   0 ross       (501) staff       (20)     1273 2022-09-12 21:53:38.000000 octodns-1.0.0rc1/script/bootstrap
+-rwxr-xr-x   0 ross       (501) staff       (20)      177 2022-12-09 16:20:31.000000 octodns-1.0.0rc1/script/changelog
+-rwxr-xr-x   0 ross       (501) staff       (20)     1085 2022-08-09 14:56:52.000000 octodns-1.0.0rc1/script/cibuild
+-rwxr-xr-x   0 ross       (501) staff       (20)      796 2022-03-28 19:32:48.000000 octodns-1.0.0rc1/script/cibuild-setup-py
+-rwxr-xr-x   0 ross       (501) staff       (20)      998 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/script/coverage
+-rwxr-xr-x   0 ross       (501) staff       (20)      184 2023-04-06 23:34:30.000000 octodns-1.0.0rc1/script/format
+-rwxr-xr-x   0 ross       (501) staff       (20)     2486 2023-04-06 23:34:41.000000 octodns-1.0.0rc1/script/generate-geo-data
+-rwxr-xr-x   0 ross       (501) staff       (20)      387 2023-04-06 23:34:30.000000 octodns-1.0.0rc1/script/lint
+-rwxr-xr-x   0 ross       (501) staff       (20)      984 2023-06-28 20:20:17.000000 octodns-1.0.0rc1/script/release
+-rwxr-xr-x   0 ross       (501) staff       (20)      283 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/script/sdist
+-rwxr-xr-x   0 ross       (501) staff       (20)      662 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/script/test
+-rwxr-xr-x   0 ross       (501) staff       (20)     1705 2023-01-22 16:25:39.000000 octodns-1.0.0rc1/script/test-module
+-rwxr-xr-x   0 ross       (501) staff       (20)     1940 2023-04-06 23:34:30.000000 octodns-1.0.0rc1/script/update-requirements
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-07-26 16:44:58.652417 octodns-1.0.0rc1/setup.cfg
+-rw-r--r--   0 ross       (501) staff       (20)     3231 2023-06-28 23:41:11.000000 octodns-1.0.0rc1/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.612686 octodns-1.0.0rc1/tests/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.627932 octodns-1.0.0rc1/tests/config/
+-rw-r--r--   0 ross       (501) staff       (20)      363 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/alias-zone-loop.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      447 2023-01-22 16:25:39.000000 octodns-1.0.0rc1/tests/config/always-dry-run.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      129 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/bad-plan-output-config.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       63 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/bad-plan-output-missing-class.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       81 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/bad-provider-class-module.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       59 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/bad-provider-class-no-module.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       67 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/bad-provider-class.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     4749 2023-04-05 21:50:25.000000 octodns-1.0.0rc1/tests/config/dynamic.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)        4 2022-02-16 22:41:06.000000 octodns-1.0.0rc1/tests/config/empty.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       32 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/missing-provider-class.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       75 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/missing-provider-config.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      121 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/missing-provider-env.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       44 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/missing-sources.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      235 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/no-dump.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.628205 octodns-1.0.0rc1/tests/config/override/
+-rw-r--r--   0 ross       (501) staff       (20)      167 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/override/dynamic.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      115 2021-04-27 01:16:58.000000 octodns-1.0.0rc1/tests/config/plan-output-filehandle.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      389 2021-07-18 20:43:40.000000 octodns-1.0.0rc1/tests/config/processors-missing-class.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      493 2021-07-18 20:43:40.000000 octodns-1.0.0rc1/tests/config/processors-wants-config.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      940 2023-07-26 16:26:11.000000 octodns-1.0.0rc1/tests/config/processors.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      461 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/provider-problems.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      400 2023-01-22 16:25:39.000000 octodns-1.0.0rc1/tests/config/simple-alias-zone.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      626 2023-02-20 21:03:39.000000 octodns-1.0.0rc1/tests/config/simple-arpa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      841 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/simple-split.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      216 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/simple-validate.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     1016 2023-01-22 16:25:39.000000 octodns-1.0.0rc1/tests/config/simple.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.519861 octodns-1.0.0rc1/tests/config/split/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.630059 octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/
+-rw-r--r--   0 ross       (501) staff       (20)      749 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/a.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      993 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/aaaa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      785 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/cname.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     1689 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/real-ish-a.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      277 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/simple-weighted.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.632335 octodns-1.0.0rc1/tests/config/split/subzone.unit.tests.tst/
+-rw-r--r--   0 ross       (501) staff       (20)       38 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/subzone.unit.tests.tst/12.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       36 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/subzone.unit.tests.tst/2.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       37 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/subzone.unit.tests.tst/test.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.640432 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/
+-rw-r--r--   0 ross       (501) staff       (20)      640 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/$unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      198 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/_srv._tcp.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       81 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/aaaa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/cname.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/dname.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       85 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/excluded.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       69 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/ignored.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       85 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/included.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      248 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/mx.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      313 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/naptr.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2021-08-19 21:09:32.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/ptr.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       71 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/spf.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       56 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/sub.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      166 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/txt.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      241 2021-08-01 18:46:05.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/urlfwd.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       51 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/www.sub.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       47 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unit.tests.tst/www.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.641290 octodns-1.0.0rc1/tests/config/split/unordered.tst/
+-rw-r--r--   0 ross       (501) staff       (20)       36 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unordered.tst/abc.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/split/unordered.tst/xyz.yaml
+-rw-r--r--   0 ross       (501) staff       (20)        4 2022-08-09 14:56:52.000000 octodns-1.0.0rc1/tests/config/sub.txt.unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       99 2022-02-16 22:41:32.000000 octodns-1.0.0rc1/tests/config/subzone.unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     3328 2022-09-07 01:07:32.000000 octodns-1.0.0rc1/tests/config/unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      307 2021-07-18 20:43:40.000000 octodns-1.0.0rc1/tests/config/unknown-processor.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      217 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/unknown-provider.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      328 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/unknown-source-zone.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       89 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/config/unordered.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     2874 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/helpers.py
+-rw-r--r--   0 ross       (501) staff       (20)     1579 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/tests/test_octodns_equality.py
+-rw-r--r--   0 ross       (501) staff       (20)     4690 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/tests/test_octodns_idna.py
+-rw-r--r--   0 ross       (501) staff       (20)    38035 2023-07-21 20:04:31.000000 octodns-1.0.0rc1/tests/test_octodns_manager.py
+-rw-r--r--   0 ross       (501) staff       (20)     9527 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_plan.py
+-rw-r--r--   0 ross       (501) staff       (20)     3135 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/tests/test_octodns_processor_acme.py
+-rw-r--r--   0 ross       (501) staff       (20)     9011 2023-06-20 14:38:33.000000 octodns-1.0.0rc1/tests/test_octodns_processor_arpa.py
+-rw-r--r--   0 ross       (501) staff       (20)     6302 2023-01-22 16:25:39.000000 octodns-1.0.0rc1/tests/test_octodns_processor_filter.py
+-rw-r--r--   0 ross       (501) staff       (20)     5156 2023-05-19 16:41:48.000000 octodns-1.0.0rc1/tests/test_octodns_processor_ownership.py
+-rw-r--r--   0 ross       (501) staff       (20)     3653 2022-09-21 16:37:15.000000 octodns-1.0.0rc1/tests/test_octodns_processor_restrict.py
+-rw-r--r--   0 ross       (501) staff       (20)    12859 2023-02-20 21:03:39.000000 octodns-1.0.0rc1/tests/test_octodns_processor_spf.py
+-rw-r--r--   0 ross       (501) staff       (20)    33602 2023-05-19 16:41:48.000000 octodns-1.0.0rc1/tests/test_octodns_provider_base.py
+-rw-r--r--   0 ross       (501) staff       (20)    22494 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_provider_yaml.py
+-rw-r--r--   0 ross       (501) staff       (20)    18809 2023-07-17 16:02:15.000000 octodns-1.0.0rc1/tests/test_octodns_record.py
+-rw-r--r--   0 ross       (501) staff       (20)     6241 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_a.py
+-rw-r--r--   0 ross       (501) staff       (20)     7294 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/tests/test_octodns_record_aaaa.py
+-rw-r--r--   0 ross       (501) staff       (20)     3468 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_alias.py
+-rw-r--r--   0 ross       (501) staff       (20)     8813 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_caa.py
+-rw-r--r--   0 ross       (501) staff       (20)     2926 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/tests/test_octodns_record_change.py
+-rw-r--r--   0 ross       (501) staff       (20)      952 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/tests/test_octodns_record_chunked.py
+-rw-r--r--   0 ross       (501) staff       (20)     4291 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_cname.py
+-rw-r--r--   0 ross       (501) staff       (20)     2879 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_dname.py
+-rw-r--r--   0 ross       (501) staff       (20)     6371 2023-01-22 16:26:20.000000 octodns-1.0.0rc1/tests/test_octodns_record_ds.py
+-rw-r--r--   0 ross       (501) staff       (20)    53366 2023-05-19 16:41:48.000000 octodns-1.0.0rc1/tests/test_octodns_record_dynamic.py
+-rw-r--r--   0 ross       (501) staff       (20)     9241 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_geo.py
+-rw-r--r--   0 ross       (501) staff       (20)      680 2023-05-23 20:27:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_ip.py
+-rw-r--r--   0 ross       (501) staff       (20)    23625 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_loc.py
+-rw-r--r--   0 ross       (501) staff       (20)     8610 2023-07-26 16:26:49.000000 octodns-1.0.0rc1/tests/test_octodns_record_mx.py
+-rw-r--r--   0 ross       (501) staff       (20)    12946 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_naptr.py
+-rw-r--r--   0 ross       (501) staff       (20)     2537 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_ns.py
+-rw-r--r--   0 ross       (501) staff       (20)     2801 2023-05-23 20:27:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_ptr.py
+-rw-r--r--   0 ross       (501) staff       (20)     2166 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_spf.py
+-rw-r--r--   0 ross       (501) staff       (20)    13677 2023-07-26 16:26:49.000000 octodns-1.0.0rc1/tests/test_octodns_record_srv.py
+-rw-r--r--   0 ross       (501) staff       (20)    10647 2023-05-23 20:27:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_sshfp.py
+-rw-r--r--   0 ross       (501) staff       (20)      737 2023-07-26 16:26:49.000000 octodns-1.0.0rc1/tests/test_octodns_record_target.py
+-rw-r--r--   0 ross       (501) staff       (20)    14104 2023-05-23 20:27:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_tlsa.py
+-rw-r--r--   0 ross       (501) staff       (20)     5264 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_txt.py
+-rw-r--r--   0 ross       (501) staff       (20)    12418 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_record_urlfwd.py
+-rw-r--r--   0 ross       (501) staff       (20)     1419 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_source_envvar.py
+-rw-r--r--   0 ross       (501) staff       (20)     9293 2023-07-17 16:02:15.000000 octodns-1.0.0rc1/tests/test_octodns_source_tinydns.py
+-rw-r--r--   0 ross       (501) staff       (20)     1402 2023-02-04 16:25:03.000000 octodns-1.0.0rc1/tests/test_octodns_yaml.py
+-rw-r--r--   0 ross       (501) staff       (20)    19346 2023-07-17 16:02:15.000000 octodns-1.0.0rc1/tests/test_octodns_zone.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.648276 octodns-1.0.0rc1/tests/zones/
+-rw-r--r--   0 ross       (501) staff       (20)      599 2022-08-09 14:56:52.000000 octodns-1.0.0rc1/tests/zones/2.0.192.in-addr.arpa.
+-rw-r--r--   0 ross       (501) staff       (20)      474 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/zones/ext.unit.tests.extension
+-rw-r--r--   0 ross       (501) staff       (20)     1541 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/zones/invalid.records.tst
+-rw-r--r--   0 ross       (501) staff       (20)      362 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/zones/invalid.zone.tst
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-07-26 16:44:58.651357 octodns-1.0.0rc1/tests/zones/tinydns/
+-rw-r--r--   0 ross       (501) staff       (20)     1024 2021-03-18 00:02:34.000000 octodns-1.0.0rc1/tests/zones/tinydns/.is-needed-for-tests
+-rwxr-xr-x   0 ross       (501) staff       (20)     2305 2023-07-17 16:02:15.000000 octodns-1.0.0rc1/tests/zones/tinydns/example.com
+-rw-r--r--   0 ross       (501) staff       (20)      207 2023-07-17 16:02:15.000000 octodns-1.0.0rc1/tests/zones/tinydns/other.foo
+-rw-r--r--   0 ross       (501) staff       (20)     1932 2022-10-10 20:14:11.000000 octodns-1.0.0rc1/tests/zones/unit.tests.
+-rw-r--r--   0 ross       (501) staff       (20)     1932 2022-07-22 22:56:06.000000 octodns-1.0.0rc1/tests/zones/unit.tests.tst
```

### Comparing `octodns-1.0.0rc0/CHANGELOG.md` & `octodns-1.0.0rc1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## v1.0.0.rc1 - 2023-07-20 - The last one before the 1s
+
+* Record and Zone validation now ensures there's no whitespace in names
+* OwnershipProcessor managed records always add w/lenient=True, this allows
+  ownership to be marked in the same zone for delegation NS records.
+* octodns-report access --lenient flag to allow running reports with records
+  sourced from providers with non-compliant record data.
+* Correctly handle FQDNs in TinyDNS config files that end with trailing .'s
+* Complete rewrite of TinyDnsBaseSource to fully implement the spec and the ipv6
+  extensions
+
 ## v1.0.0.rc0 - 2023-05-16 - First of the ones
 
 #### Noteworthy changes
 
 * 1.x Deprecation removals
    * Provider, Source, and Processor shims removed, they've been warnings for >
      1yr.  Everything should be using and referring to provider-specific
```

### Comparing `octodns-1.0.0rc0/CODE_OF_CONDUCT.md` & `octodns-1.0.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/CONTRIBUTING.md` & `octodns-1.0.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/LICENSE` & `octodns-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/PKG-INFO` & `octodns-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: OctoDNS: DNS as code - Tools for managing DNS across multiple providers
 Home-page: https://github.com/octodns/octodns
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `octodns-1.0.0rc0/README.md` & `octodns-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/docs/assets/deploy.png` & `octodns-1.0.0rc1/docs/assets/deploy.png`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/docs/assets/noop.png` & `octodns-1.0.0rc1/docs/assets/noop.png`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/docs/assets/pr.png` & `octodns-1.0.0rc1/docs/assets/pr.png`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/docs/auto_arpa.md` & `octodns-1.0.0rc1/docs/auto_arpa.md`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/docs/dynamic_records.md` & `octodns-1.0.0rc1/docs/dynamic_records.md`

 * *Files 2% similar despite different names*

```diff
@@ -199,12 +199,11 @@
           status: up
         - value: 3.4.5.6
           # defaults to status: obey
   ...
 ```
 
 Support matrix:
-* NS1 supports all 3 flag values
-* Azure DNS supports only `obey` and `down`
+* NS1 and Azure DNS support all 3 flag values
 * All other dynamic-capable providers only support the default `obey`
 
 See "Health Check Options" in individual provider documentation for customization support.
```

### Comparing `octodns-1.0.0rc0/docs/geo_records.md` & `octodns-1.0.0rc1/docs/geo_records.md`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/docs/logos/octodns-logo.png` & `octodns-1.0.0rc1/docs/logos/octodns-logo.png`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/docs/records.md` & `octodns-1.0.0rc1/docs/records.md`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/cmds/args.py` & `octodns-1.0.0rc1/octodns/cmds/args.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/cmds/compare.py` & `octodns-1.0.0rc1/octodns/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/cmds/dump.py` & `octodns-1.0.0rc1/octodns/cmds/dump.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/cmds/report.py` & `octodns-1.0.0rc1/octodns/cmds/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     )
     parser.add_argument(
         '--num-workers', default=4, help='Number of background workers'
     )
     parser.add_argument(
         '--timeout', default=1, help='Number seconds to wait for an answer'
     )
+    parser.add_argument(
+        '--lenient',
+        action='store_true',
+        default=False,
+        help='Ignore record validations and do a best effort dump',
+    )
     parser.add_argument('server', nargs='+', help='Servers to query')
 
     args = parser.parse_args()
 
     manager = Manager(args.config_file)
 
     log = getLogger('report')
@@ -57,15 +63,15 @@
     try:
         sources = [manager.providers[source] for source in args.source]
     except KeyError as e:
         raise Exception(f'Unknown source: {e.args[0]}')
 
     zone = manager.get_zone(args.zone)
     for source in sources:
-        source.populate(zone)
+        source.populate(zone, lenient=args.lenient)
 
     servers = ','.join(args.server)
     print(f'name,type,ttl,{servers},consistent')
     resolvers = []
     ip_addr_re = re.compile(r'^[\d\.]+$')
     for server in args.server:
         resolver = AsyncResolver(
```

### Comparing `octodns-1.0.0rc0/octodns/cmds/sync.py` & `octodns-1.0.0rc1/octodns/cmds/sync.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/cmds/validate.py` & `octodns-1.0.0rc1/octodns/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/equality.py` & `octodns-1.0.0rc1/octodns/equality.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/idna.py` & `octodns-1.0.0rc1/octodns/idna.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/manager.py` & `octodns-1.0.0rc1/octodns/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,14 @@
         eligible_zones=[],
         eligible_sources=[],
         eligible_targets=[],
         dry_run=True,
         force=False,
         plan_output_fh=stdout,
     ):
-
         self.log.info(
             'sync: eligible_zones=%s, eligible_targets=%s, dry_run=%s, '
             'force=%s, plan_output_fh=%s',
             eligible_zones,
             eligible_targets,
             dry_run,
             force,
```

### Comparing `octodns-1.0.0rc0/octodns/processor/acme.py` & `octodns-1.0.0rc1/octodns/processor/acme.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/processor/arpa.py` & `octodns-1.0.0rc1/octodns/processor/arpa.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,13 +57,18 @@
             if arpa.endswith(f'.{zone_name}'):
                 name = arpa[:-n]
                 fqdns = sorted(fqdns)
                 record = Record.new(
                     zone,
                     name,
                     {'ttl': self.ttl, 'type': 'PTR', 'values': fqdns},
+                    lenient=lenient,
+                )
+                zone.add_record(
+                    record,
+                    replace=self.populate_should_replace,
+                    lenient=lenient,
                 )
-                zone.add_record(record, replace=self.populate_should_replace)
 
         self.log.info(
             'populate:   found %s records', len(zone.records) - before
         )
```

### Comparing `octodns-1.0.0rc0/octodns/processor/base.py` & `octodns-1.0.0rc1/octodns/processor/base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/processor/filter.py` & `octodns-1.0.0rc1/octodns/processor/filter.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/processor/ownership.py` & `octodns-1.0.0rc1/octodns/processor/ownership.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,17 @@
             else:
                 name = f'{self.txt_name}.{record._type}'
             txt = Record.new(
                 desired,
                 name,
                 {'type': 'TXT', 'ttl': 60, 'value': self.txt_value},
             )
-            desired.add_record(txt)
+            # add these w/lenient to cover the case when the ownership record
+            # for a NS delegation record should technically live in the subzone
+            desired.add_record(txt, lenient=True)
 
         return desired
 
     def _is_ownership(self, record):
         return (
             record._type == 'TXT'
             and record.name.startswith(self.txt_name)
```

### Comparing `octodns-1.0.0rc0/octodns/processor/restrict.py` & `octodns-1.0.0rc1/octodns/processor/restrict.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/processor/spf.py` & `octodns-1.0.0rc1/octodns/processor/spf.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/provider/base.py` & `octodns-1.0.0rc1/octodns/provider/base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/provider/plan.py` & `octodns-1.0.0rc1/octodns/provider/plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,24 @@
 class RootNsChange(UnsafePlan):
     def __init__(self):
         super().__init__('Root NS record change, force required')
 
 
 class TooMuchChange(UnsafePlan):
     def __init__(
-        self, why, update_pcent, update_threshold, change_count, existing_count
+        self,
+        why,
+        update_pcent,
+        update_threshold,
+        change_count,
+        existing_count,
+        name,
     ):
         msg = (
-            f'{why}, {update_pcent:.2f}% is over {update_threshold:.2f}% '
+            f'[{name}] {why}, {update_pcent:.2f}% is over {update_threshold:.2f}% '
             f'({change_count}/{existing_count}), force required'
         )
         super().__init__(msg)
 
 
 class Plan(object):
     log = getLogger('Plan')
@@ -74,15 +80,14 @@
 
     def raise_if_unsafe(self):
         # TODO: what is safe really?
         if (
             self.existing
             and len(self.existing.records) >= self.MIN_EXISTING_RECORDS
         ):
-
             existing_record_count = len(self.existing.records)
             if existing_record_count > 0:
                 update_pcent = (
                     self.change_counts['Update'] / existing_record_count
                 )
                 delete_pcent = (
                     self.change_counts['Delete'] / existing_record_count
@@ -94,22 +99,24 @@
             if update_pcent > self.update_pcent_threshold:
                 raise TooMuchChange(
                     'Too many updates',
                     update_pcent * 100,
                     self.update_pcent_threshold * 100,
                     self.change_counts['Update'],
                     existing_record_count,
+                    self.existing.decoded_name,
                 )
             if delete_pcent > self.delete_pcent_threshold:
                 raise TooMuchChange(
                     'Too many deletes',
                     delete_pcent * 100,
                     self.delete_pcent_threshold * 100,
                     self.change_counts['Delete'],
                     existing_record_count,
+                    self.existing.decoded_name,
                 )
 
         # If we have any changes of the root NS record for the zone it's a huge
         # deal and force should always be required for extra care
         if self.exists and any(
             c
             for c in self.changes
```

### Comparing `octodns-1.0.0rc0/octodns/provider/yaml.py` & `octodns-1.0.0rc1/octodns/provider/yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/__init__.py` & `octodns-1.0.0rc1/octodns/record/__init__.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/base.py` & `octodns-1.0.0rc1/octodns/record/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
         reasons = []
         try:
             name = idna_encode(str(name))
         except IdnaError as e:
             # convert the error into a reason
             reasons.append(str(e))
             name = str(name)
+
+        if ' ' in name or '\t' in name:
+            reasons.append('invalid record, whitespace is not allowed')
+
         fqdn = f'{name}.{zone.name}' if name else zone.name
         try:
             _type = data['type']
         except KeyError:
             raise Exception(f'Invalid record {idna_decode(fqdn)}, missing type')
         try:
             _class = cls._CLASSES[_type]
@@ -115,14 +119,18 @@
             _class = cls._CLASSES[rr._type]
             data = _class.data_from_rrs(rrs)
             record = Record.new(zone, name, data, lenient=lenient)
             records.append(record)
 
         return records
 
+    @classmethod
+    def parse_rdata_texts(cls, rdatas):
+        return [cls._value_type.parse_rdata_text(r) for r in rdatas]
+
     def __init__(self, zone, name, data, source=None):
         self.zone = zone
         if name:
             # internally everything is idna
             self.name = idna_encode(str(name))
             # we'll keep a decoded version around for logs and errors
             self.decoded_name = idna_decode(self.name)
```

### Comparing `octodns-1.0.0rc0/octodns/record/caa.py` & `octodns-1.0.0rc1/octodns/record/caa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/change.py` & `octodns-1.0.0rc1/octodns/record/change.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/chunked.py` & `octodns-1.0.0rc1/octodns/record/chunked.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/cname.py` & `octodns-1.0.0rc1/octodns/record/cname.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/ds.py` & `octodns-1.0.0rc1/octodns/record/ds.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/dynamic.py` & `octodns-1.0.0rc1/octodns/record/dynamic.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/geo.py` & `octodns-1.0.0rc1/octodns/record/geo.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/geo_data.py` & `octodns-1.0.0rc1/octodns/record/geo_data.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/ip.py` & `octodns-1.0.0rc1/octodns/record/ip.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/loc.py` & `octodns-1.0.0rc1/octodns/record/loc.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/mx.py` & `octodns-1.0.0rc1/octodns/record/mx.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/naptr.py` & `octodns-1.0.0rc1/octodns/record/naptr.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/rr.py` & `octodns-1.0.0rc1/octodns/record/rr.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/srv.py` & `octodns-1.0.0rc1/octodns/record/srv.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/sshfp.py` & `octodns-1.0.0rc1/octodns/record/sshfp.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/target.py` & `octodns-1.0.0rc1/octodns/record/target.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/tlsa.py` & `octodns-1.0.0rc1/octodns/record/tlsa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/record/urlfwd.py` & `octodns-1.0.0rc1/octodns/record/urlfwd.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/source/base.py` & `octodns-1.0.0rc1/octodns/source/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #
 #
 #
 
 
 class BaseSource(object):
-
     SUPPORTS_MULTIVALUE_PTR = False
     SUPPORTS_POOL_VALUE_STATUS = False
     SUPPORTS_ROOT_NS = False
     SUPPORTS_DYNAMIC_SUBNETS = False
 
     def __init__(self, id):
         self.id = id
```

### Comparing `octodns-1.0.0rc0/octodns/source/envvar.py` & `octodns-1.0.0rc1/octodns/source/envvar.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/yaml.py` & `octodns-1.0.0rc1/octodns/yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/octodns/zone.py` & `octodns-1.0.0rc1/octodns/zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 class Zone(object):
     log = getLogger('Zone')
 
     def __init__(self, name, sub_zones):
         if not name[-1] == '.':
             raise Exception(f'Invalid zone name {name}, missing ending dot')
+        elif ' ' in name or '\t' in name:
+            raise Exception(f'Invalid zone name {name}, whitespace not allowed')
+
         # internally everything is idna
         self.name = idna_encode(str(name)) if name else name
         # we'll keep a decoded version around for logs and errors
         self.decoded_name = idna_decode(self.name)
         self.sub_zones = sub_zones
         # We're grouping by node, it allows us to efficiently search for
         # duplicates and detect when CNAMEs co-exist with other records. Also
@@ -68,14 +71,40 @@
             fqdn.encode('ascii')
             # it's non-idna or idna encoded
             return self._idna_name_re.sub('', idna_encode(fqdn))
         except UnicodeEncodeError:
             # it has utf8 chars
             return self._utf8_name_re.sub('', fqdn)
 
+    def owns(self, _type, fqdn):
+        if fqdn[-1] != '.':
+            fqdn = f'{fqdn}.'
+
+        # if we exactly match the zone name we own it
+        if fqdn == self.name:
+            return True
+
+        # if we don't end with the zone's name on a boundary we aren't owned
+        if not fqdn.endswith(f'.{self.name}'):
+            return False
+
+        hostname = self.hostname_from_fqdn(fqdn)
+        if hostname in self.sub_zones:
+            # if our hostname matches a sub-zone exactly we have to be a NS
+            # record
+            return _type == 'NS'
+
+        for sub_zone in self.sub_zones:
+            if hostname.endswith(f'.{sub_zone}'):
+                # this belongs under a sub-zone
+                return False
+
+        # otherwise we own it
+        return True
+
     def add_record(self, record, replace=False, lenient=False):
         if self._origin:
             self.hydrate()
 
         name = record.name
 
         if not lenient:
```

### Comparing `octodns-1.0.0rc0/octodns.egg-info/PKG-INFO` & `octodns-1.0.0rc1/octodns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: OctoDNS: DNS as code - Tools for managing DNS across multiple providers
 Home-page: https://github.com/octodns/octodns
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `octodns-1.0.0rc0/octodns.egg-info/SOURCES.txt` & `octodns-1.0.0rc1/octodns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/requirements-dev.txt` & `octodns-1.0.0rc1/requirements-dev.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # DO NOT EDIT THIS FILE DIRECTLY - use ./script/update-requirements to update
-Pygments==2.13.0
-attrs==22.1.0
-black==22.10.0
-bleach==5.0.1
-build==0.9.0
-certifi==2022.12.7
+Pygments==2.15.1
+black==23.3.0
+bleach==6.0.0
+build==0.10.0
+certifi==2023.5.7
 cffi==1.15.1
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
 click==8.1.3
 cmarkgfm==2022.10.27
-commonmark==0.9.1
-coverage==6.5.0
-docutils==0.19
-exceptiongroup==1.0.0
-importlib-metadata==5.0.0
-iniconfig==1.1.1
-isort==5.11.4
+coverage==7.2.7
+docutils==0.20.1
+exceptiongroup==1.1.1
+importlib-metadata==6.7.0
+iniconfig==2.0.0
+isort==5.12.0
 jaraco.classes==3.2.3
-keyring==23.9.3
-more-itertools==9.0.0
-mypy-extensions==0.4.3
-packaging==21.3
-pathspec==0.10.1
-pep517==0.13.0
-pkginfo==1.8.3
-platformdirs==2.5.2
-pluggy==1.0.0
+keyring==24.2.0
+markdown-it-py==3.0.0
+mdurl==0.1.2
+more-itertools==9.1.0
+mypy-extensions==1.0.0
+packaging==23.1
+pathspec==0.11.1
+pkginfo==1.9.6
+platformdirs==3.8.0
+pluggy==1.2.0
 pprintpp==0.4.0
 pycountry-convert==0.7.2
 pycountry==22.3.5
 pycparser==2.21
-pyflakes==2.5.0
-pyparsing==3.0.9
-pytest-cov==4.0.0
-pytest-mock==3.10.0
+pyflakes==3.0.1
+pyproject_hooks==1.0.0
+pytest-cov==4.1.0
+pytest-mock==3.11.1
 pytest-network==0.0.1
-pytest==7.2.0
-readme-renderer==37.3
+pytest==7.4.0
+readme-renderer==40.0
 repoze.lru==0.7
-requests-toolbelt==0.10.1
-requests==2.28.1
+requests-toolbelt==1.0.0
+requests==2.31.0
 rfc3986==2.0.0
-rich==12.6.0
+rich==13.4.2
 tomli==2.0.1
-twine==4.0.1
-typing_extensions==4.4.0
-urllib3==1.26.12
+twine==4.0.2
+urllib3==2.0.3
 webencodings==0.5.1
-zipp==3.10.0
+zipp==3.15.0
```

### Comparing `octodns-1.0.0rc0/script/bootstrap` & `octodns-1.0.0rc1/script/bootstrap`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/script/cibuild` & `octodns-1.0.0rc1/script/cibuild`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/script/cibuild-setup-py` & `octodns-1.0.0rc1/script/cibuild-setup-py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/script/coverage` & `octodns-1.0.0rc1/script/coverage`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/script/generate-geo-data` & `octodns-1.0.0rc1/script/generate-geo-data`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/script/release` & `octodns-1.0.0rc1/script/release`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,27 @@
 cd "$(dirname "$0")"/..
 ROOT=$(pwd)
 
 if [ -z "$VENV_NAME" ]; then
     VENV_NAME="env"
 fi
 
+PYPYRC="$HOME/.pypirc"
+if [ ! -e "$PYPYRC" ]; then
+    cat << EndOfMessage >&2
+$PYPYRC does not exist, please create it with the following contents
+
+[pypi]
+  username = __token__
+  password = [secret-token-goes-here]
+
+EndOfMessage
+    exit 1
+fi
+
 ACTIVATE="$VENV_NAME/bin/activate"
 if [ ! -f "$ACTIVATE" ]; then
     echo "$ACTIVATE does not exist, run ./script/bootstrap" >&2
     exit 1
 fi
 . "$ACTIVATE"
```

### Comparing `octodns-1.0.0rc0/script/test` & `octodns-1.0.0rc1/script/test`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/script/test-module` & `octodns-1.0.0rc1/script/test-module`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/script/update-requirements` & `octodns-1.0.0rc1/script/update-requirements`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/setup.py` & `octodns-1.0.0rc1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -68,17 +68,21 @@
     author='Ross McFarland',
     author_email='rwmcfa1@gmail.com',
     description=octodns.__doc__,
     entry_points={'console_scripts': console_scripts},
     extras_require={
         'dev': tests_require
         + (
-            'black>=22.3.0',
+            # we need to manually/explicitely bump major versions as they're
+            # likely to result in formatting changes that should happen in their
+            # own PR. This will basically happen yearly
+            # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
+            'black>=23.1.0,<24.0.0',
             'build>=0.7.0',
-            'isort>=5.11.4',
+            'isort>=5.11.5',
             'pycountry>=19.8.18',
             'pycountry-convert>=0.7.2',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         )
     },
```

### Comparing `octodns-1.0.0rc0/tests/config/dynamic.tests.yaml` & `octodns-1.0.0rc1/tests/config/dynamic.tests.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/processors.yaml` & `octodns-1.0.0rc1/tests/config/processors.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/simple-arpa.yaml` & `octodns-1.0.0rc1/tests/config/simple-arpa.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/simple-split.yaml` & `octodns-1.0.0rc1/tests/config/simple-split.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/simple.yaml` & `octodns-1.0.0rc1/tests/config/simple.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/a.yaml` & `octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/a.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/aaaa.yaml` & `octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/aaaa.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/cname.yaml` & `octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/cname.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/real-ish-a.yaml` & `octodns-1.0.0rc1/tests/config/split/dynamic.tests.tst/real-ish-a.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/split/unit.tests.tst/$unit.tests.yaml` & `octodns-1.0.0rc1/tests/config/split/unit.tests.tst/$unit.tests.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/config/unit.tests.yaml` & `octodns-1.0.0rc1/tests/config/unit.tests.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/helpers.py` & `octodns-1.0.0rc1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_equality.py` & `octodns-1.0.0rc1/tests/test_octodns_equality.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_idna.py` & `octodns-1.0.0rc1/tests/test_octodns_idna.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_manager.py` & `octodns-1.0.0rc1/tests/test_octodns_manager.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_plan.py` & `octodns-1.0.0rc1/tests/test_octodns_plan.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_processor_acme.py` & `octodns-1.0.0rc1/tests/test_octodns_processor_acme.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_processor_arpa.py` & `octodns-1.0.0rc1/tests/test_octodns_processor_arpa.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 #
 
 from unittest import TestCase
 
 from octodns.processor.arpa import AutoArpa
 from octodns.record import Record
+from octodns.record.exception import ValidationError
 from octodns.zone import Zone
 
 
 class TestAutoArpa(TestCase):
     def test_empty_zone(self):
-
         # empty zone no records
         zone = Zone('unit.tests.', [])
         aa = AutoArpa('auto-arpa')
         aa.process_source_zone(zone, [])
         self.assertFalse(aa._records)
 
     def test_single_value_A(self):
@@ -223,7 +223,43 @@
         self.assertEqual(record.fqdn, ptr.value)
         self.assertEqual(3600, ptr.ttl)
 
         # non-matching boundary edge case
         arpa = Zone('0.10.in-addr.arpa.', [])
         aa.populate(arpa)
         self.assertEqual(0, len(arpa.records))
+
+    def test_single_value_A_with_space(self):
+        zone = Zone('unit.tests.', [])
+
+        # invalid record without lenient
+        with self.assertRaises(ValidationError):
+            Record.new(
+                zone,
+                'a with spaces',
+                {'ttl': 32, 'type': 'A', 'value': '1.2.3.4'},
+            )
+
+        # invalid record with lenient
+        lenient = True
+        record = Record.new(
+            zone,
+            'a with spaces',
+            {'ttl': 32, 'type': 'A', 'value': '1.2.3.4'},
+            lenient=lenient,
+        )
+        zone.add_record(record)
+        aa = AutoArpa('auto-arpa')
+        aa.process_source_zone(zone, [])
+        self.assertEqual(
+            {'4.3.2.1.in-addr.arpa.': {'a with spaces.unit.tests.'}},
+            aa._records,
+        )
+
+        # matching zone
+        arpa = Zone('3.2.1.in-addr.arpa.', [])
+        aa.populate(arpa, lenient=lenient)
+        self.assertEqual(1, len(arpa.records))
+        (ptr,) = arpa.records
+        self.assertEqual('4.3.2.1.in-addr.arpa.', ptr.fqdn)
+        self.assertEqual(record.fqdn, ptr.value)
+        self.assertEqual(3600, ptr.ttl)
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_processor_filter.py` & `octodns-1.0.0rc1/tests/test_octodns_processor_filter.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_processor_ownership.py` & `octodns-1.0.0rc1/tests/test_octodns_processor_ownership.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_processor_restrict.py` & `octodns-1.0.0rc1/tests/test_octodns_processor_restrict.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_processor_spf.py` & `octodns-1.0.0rc1/tests/test_octodns_processor_spf.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_provider_base.py` & `octodns-1.0.0rc1/tests/test_octodns_provider_base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_provider_yaml.py` & `octodns-1.0.0rc1/tests/test_octodns_provider_yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record.py` & `octodns-1.0.0rc1/tests/test_octodns_record.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from unittest import TestCase
 
 from octodns.idna import idna_encode
 from octodns.record import (
     AliasRecord,
     ARecord,
+    CnameRecord,
     Create,
     Delete,
     MxValue,
     NsValue,
     Record,
     RecordException,
     Rr,
@@ -172,14 +173,28 @@
         self.assertEqual(['fc00::3'], record.values)
         record = records[('CNAME', 'cname')]
         self.assertEqual(46, record.ttl)
         self.assertEqual('target.unit.tests.', record.value)
         # make sure there's nothing extra
         self.assertEqual(5, len(records))
 
+    def test_parse_rdata_texts(self):
+        self.assertEqual(['2.3.4.5'], ARecord.parse_rdata_texts(['2.3.4.5']))
+        self.assertEqual(
+            ['2.3.4.6', '3.4.5.7'],
+            ARecord.parse_rdata_texts(['2.3.4.6', '3.4.5.7']),
+        )
+        self.assertEqual(
+            ['some.target.'], CnameRecord.parse_rdata_texts(['some.target.'])
+        )
+        self.assertEqual(
+            ['some.target.', 'other.target.'],
+            CnameRecord.parse_rdata_texts(['some.target.', 'other.target.']),
+        )
+
     def test_values_mixin_data(self):
         # no values, no value or values in data
         a = ARecord(self.zone, '', {'type': 'A', 'ttl': 600, 'values': []})
         self.assertNotIn('values', a.data)
 
         # empty value, no value or values in data
         b = ARecord(self.zone, '', {'type': 'A', 'ttl': 600, 'values': ['']})
@@ -394,14 +409,36 @@
         )
 
 
 class TestRecordValidation(TestCase):
     zone = Zone('unit.tests.', [])
 
     def test_base(self):
+        # no spaces
+        for name in (
+            ' ',
+            ' leading',
+            'trailing ',
+            'in the middle',
+            '\t',
+            '\tleading',
+            'trailing\t',
+            'in\tthe\tmiddle',
+        ):
+            with self.assertRaises(ValidationError) as ctx:
+                Record.new(
+                    self.zone,
+                    name,
+                    {'ttl': 300, 'type': 'A', 'value': '1.2.3.4'},
+                )
+            reason = ctx.exception.reasons[0]
+            self.assertEqual(
+                'invalid record, whitespace is not allowed', reason
+            )
+
         # name = '@'
         with self.assertRaises(ValidationError) as ctx:
             name = '@'
             Record.new(
                 self.zone, name, {'ttl': 300, 'type': 'A', 'value': '1.2.3.4'}
             )
         reason = ctx.exception.reasons[0]
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_a.py` & `octodns-1.0.0rc1/tests/test_octodns_record_a.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_aaaa.py` & `octodns-1.0.0rc1/tests/test_octodns_record_aaaa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_alias.py` & `octodns-1.0.0rc1/tests/test_octodns_record_alias.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_caa.py` & `octodns-1.0.0rc1/tests/test_octodns_record_caa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_change.py` & `octodns-1.0.0rc1/tests/test_octodns_record_change.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_chunked.py` & `octodns-1.0.0rc1/tests/test_octodns_record_chunked.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_cname.py` & `octodns-1.0.0rc1/tests/test_octodns_record_cname.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_dname.py` & `octodns-1.0.0rc1/tests/test_octodns_record_dname.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_ds.py` & `octodns-1.0.0rc1/tests/test_octodns_record_ds.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_dynamic.py` & `octodns-1.0.0rc1/tests/test_octodns_record_dynamic.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_geo.py` & `octodns-1.0.0rc1/tests/test_octodns_record_geo.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_ip.py` & `octodns-1.0.0rc1/tests/test_octodns_record_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from octodns.record.a import ARecord, Ipv4Value
 from octodns.zone import Zone
 
 
 class TestRecordIp(TestCase):
     def test_ipv4_value_rdata_text(self):
-
         # anything goes, we're a noop
         for s in (
             None,
             '',
             'word',
             42,
             42.43,
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_loc.py` & `octodns-1.0.0rc1/tests/test_octodns_record_loc.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_mx.py` & `octodns-1.0.0rc1/tests/test_octodns_record_mx.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         self.assertEqual(change.existing, a)
         self.assertEqual(change.new, other)
 
         # __repr__ doesn't blow up
         a.__repr__()
 
     def test_mx_value_rdata_text(self):
-
         # empty string won't parse
         with self.assertRaises(RrParseError):
             MxValue.parse_rdata_text('')
 
         # single word won't parse
         with self.assertRaises(RrParseError):
             MxValue.parse_rdata_text('nope')
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_naptr.py` & `octodns-1.0.0rc1/tests/test_octodns_record_naptr.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_ns.py` & `octodns-1.0.0rc1/tests/test_octodns_record_ns.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_ptr.py` & `octodns-1.0.0rc1/tests/test_octodns_record_ptr.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
                 self.zone, '', {'type': 'PTR', 'ttl': 600, 'value': 'foo.bar'}
             )
         self.assertEqual(
             ['PTR value "foo.bar" missing trailing .'], ctx.exception.reasons
         )
 
     def test_ptr_rdata_text(self):
-
         # anything goes, we're a noop
         for s in (
             None,
             '',
             'word',
             42,
             42.43,
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_spf.py` & `octodns-1.0.0rc1/tests/test_octodns_record_spf.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_srv.py` & `octodns-1.0.0rc1/tests/test_octodns_record_srv.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         self.assertEqual(change.existing, a)
         self.assertEqual(change.new, other)
 
         # __repr__ doesn't blow up
         a.__repr__()
 
     def test_srv_value_rdata_text(self):
-
         # empty string won't parse
         with self.assertRaises(RrParseError):
             SrvValue.parse_rdata_text('')
 
         # single word won't parse
         with self.assertRaises(RrParseError):
             SrvValue.parse_rdata_text('nope')
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_sshfp.py` & `octodns-1.0.0rc1/tests/test_octodns_record_sshfp.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         self.assertEqual(change.existing, a)
         self.assertEqual(change.new, other)
 
         # __repr__ doesn't blow up
         a.__repr__()
 
     def test_sshfp_value_rdata_text(self):
-
         # empty string won't parse
         with self.assertRaises(RrParseError):
             SshfpValue.parse_rdata_text('')
 
         # single word won't parse
         with self.assertRaises(RrParseError):
             SshfpValue.parse_rdata_text('nope')
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_target.py` & `octodns-1.0.0rc1/tests/test_octodns_record_target.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from octodns.record.alias import AliasRecord
 from octodns.record.target import _TargetValue
 from octodns.zone import Zone
 
 
 class TestRecordTarget(TestCase):
     def test_target_rdata_text(self):
-
         # anything goes, we're a noop
         for s in (
             None,
             '',
             'word',
             42,
             42.43,
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_tlsa.py` & `octodns-1.0.0rc1/tests/test_octodns_record_tlsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
         self.assertEqual(change.existing, a)
         self.assertEqual(change.new, other)
 
         # __repr__ doesn't blow up
         a.__repr__()
 
     def test_tsla_value_rdata_text(self):
-
         # empty string won't parse
         with self.assertRaises(RrParseError):
             TlsaValue.parse_rdata_text('')
 
         # single word won't parse
         with self.assertRaises(RrParseError):
             TlsaValue.parse_rdata_text('nope')
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_txt.py` & `octodns-1.0.0rc1/tests/test_octodns_record_txt.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_record_urlfwd.py` & `octodns-1.0.0rc1/tests/test_octodns_record_urlfwd.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_source_envvar.py` & `octodns-1.0.0rc1/tests/test_octodns_source_envvar.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_source_tinydns.py` & `octodns-1.0.0rc1/tests/test_octodns_source_tinydns.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,25 +13,30 @@
 
 class TestTinyDnsFileSource(TestCase):
     source = TinyDnsFileSource('test', './tests/zones/tinydns')
 
     def test_populate_normal(self):
         got = Zone('example.com.', [])
         self.source.populate(got)
-        self.assertEqual(17, len(got.records))
+        self.assertEqual(30, len(got.records))
 
         expected = Zone('example.com.', [])
         for name, data in (
             ('', {'type': 'A', 'ttl': 30, 'values': ['10.2.3.4', '10.2.3.5']}),
             (
                 '',
                 {
                     'type': 'NS',
-                    'ttl': 3600,
-                    'values': ['ns1.ns.com.', 'ns2.ns.com.'],
+                    'ttl': 31,
+                    'values': [
+                        'a.ns.example.com.',
+                        'b.ns.example.com.',
+                        'ns1.ns.com.',
+                        'ns2.ns.com.',
+                    ],
                 },
             ),
             (
                 'sub',
                 {
                     'type': 'NS',
                     'ttl': 30,
@@ -40,14 +45,18 @@
             ),
             ('www', {'type': 'A', 'ttl': 3600, 'value': '10.2.3.6'}),
             (
                 'cname',
                 {'type': 'CNAME', 'ttl': 3600, 'value': 'www.example.com.'},
             ),
             (
+                'cname2',
+                {'type': 'CNAME', 'ttl': 48, 'value': 'www2.example.com.'},
+            ),
+            (
                 'some-host-abc123',
                 {'type': 'A', 'ttl': 1800, 'value': '10.2.3.7'},
             ),
             ('has-dup-def123', {'type': 'A', 'ttl': 3600, 'value': '10.2.3.8'}),
             ('www.sub', {'type': 'A', 'ttl': 3600, 'value': '1.2.3.4'}),
             ('has-dup-def456', {'type': 'A', 'ttl': 3600, 'value': '10.2.3.8'}),
             (
@@ -57,33 +66,33 @@
                     'ttl': 3600,
                     'values': [
                         {
                             'preference': 10,
                             'exchange': 'smtp-1-host.example.com.',
                         },
                         {
-                            'preference': 20,
+                            'preference': 0,
                             'exchange': 'smtp-2-host.example.com.',
                         },
                     ],
                 },
             ),
             (
                 'smtp',
                 {
                     'type': 'MX',
                     'ttl': 1800,
                     'values': [
                         {
                             'preference': 30,
-                            'exchange': 'smtp-1-host.example.com.',
+                            'exchange': 'smtp-3-host.mx.example.com.',
                         },
                         {
                             'preference': 40,
-                            'exchange': 'smtp-2-host.example.com.',
+                            'exchange': 'smtp-4-host.mx.example.com.',
                         },
                     ],
                 },
             ),
             ('', {'type': 'TXT', 'ttl': 300, 'value': 'test TXT'}),
             ('colon', {'type': 'TXT', 'ttl': 300, 'value': 'test : TXT'}),
             ('nottl', {'type': 'TXT', 'ttl': 3600, 'value': 'nottl test TXT'}),
@@ -107,14 +116,91 @@
                 'semicolon',
                 {
                     'type': 'TXT',
                     'ttl': 300,
                     'value': 'v=DKIM1\\; k=rsa\\; p=blah',
                 },
             ),
+            ('b.ns', {'type': 'A', 'ttl': 31, 'value': '43.44.45.46'}),
+            ('a.ns', {'type': 'A', 'ttl': 3600, 'value': '42.43.44.45'}),
+            (
+                'smtp-3-host.mx',
+                {'type': 'A', 'ttl': 1800, 'value': '21.22.23.24'},
+            ),
+            (
+                'smtp-4-host.mx',
+                {'type': 'A', 'ttl': 1800, 'value': '22.23.24.25'},
+            ),
+            ('ns5.ns', {'type': 'A', 'ttl': 30, 'value': '14.15.16.17'}),
+            ('ns6.ns', {'type': 'A', 'ttl': 30, 'value': '15.16.17.18'}),
+            (
+                'other',
+                {
+                    'type': 'NS',
+                    'ttl': 30,
+                    'values': ['ns5.ns.example.com.', 'ns6.ns.example.com.'],
+                },
+            ),
+            (
+                '_a._tcp',
+                {
+                    'type': 'SRV',
+                    'ttl': 43,
+                    'values': [
+                        {
+                            'priority': 0,
+                            'weight': 0,
+                            'port': 8888,
+                            'target': 'target.srv.example.com.',
+                        },
+                        {
+                            'priority': 10,
+                            'weight': 50,
+                            'port': 8080,
+                            'target': 'target.somewhere.else.',
+                        },
+                    ],
+                },
+            ),
+            ('target.srv', {'type': 'A', 'ttl': 43, 'value': '56.57.58.59'}),
+            (
+                '_b._tcp',
+                {
+                    'type': 'SRV',
+                    'ttl': 3600,
+                    'values': [
+                        {
+                            'priority': 0,
+                            'weight': 0,
+                            'port': 9999,
+                            'target': 'target.srv.example.com.',
+                        }
+                    ],
+                },
+            ),
+            (
+                'arbitrary-sshfp',
+                {
+                    'type': 'SSHFP',
+                    'ttl': 45,
+                    'values': [
+                        {
+                            'algorithm': 1,
+                            'fingerprint_type': 2,
+                            'fingerprint': '00479b27',
+                        },
+                        {
+                            'algorithm': 2,
+                            'fingerprint_type': 2,
+                            'fingerprint': '00479a28',
+                        },
+                    ],
+                },
+            ),
+            ('arbitrary-a', {'type': 'A', 'ttl': 3600, 'value': '80.81.82.83'}),
         ):
             record = Record.new(expected, name, data)
             expected.add_record(record)
 
         changes = expected.changes(got, SimpleProvider())
         self.assertEqual([], changes)
 
@@ -146,28 +232,30 @@
             record = Record.new(expected, name, data)
             expected.add_record(record)
 
         changes = expected.changes(got, SimpleProvider())
         self.assertEqual([], changes)
 
     def test_populate_in_addr_arpa(self):
-
         got = Zone('3.2.10.in-addr.arpa.', [])
         self.source.populate(got)
 
         expected = Zone('3.2.10.in-addr.arpa.', [])
         for name, data in (
             ('10', {'type': 'PTR', 'ttl': 3600, 'value': 'a-ptr.example.com.'}),
             ('11', {'type': 'PTR', 'ttl': 30, 'value': 'a-ptr-2.example.com.'}),
             (
                 '8',
                 {
                     'type': 'PTR',
                     'ttl': 3600,
-                    'value': 'has-dup-def123.example.com.',
+                    'values': [
+                        'has-dup-def123.example.com.',
+                        'has-dup-def456.example.com.',
+                    ],
                 },
             ),
             (
                 '7',
                 {
                     'type': 'PTR',
                     'ttl': 1800,
@@ -180,8 +268,9 @@
 
         changes = expected.changes(got, SimpleProvider())
         self.assertEqual([], changes)
 
     def test_ignores_subs(self):
         got = Zone('example.com.', ['sub'])
         self.source.populate(got)
-        self.assertEqual(16, len(got.records))
+        # we don't see one www.sub.example.com. record b/c it's in a sub
+        self.assertEqual(29, len(got.records))
```

### Comparing `octodns-1.0.0rc0/tests/test_octodns_yaml.py` & `octodns-1.0.0rc1/tests/test_octodns_yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/test_octodns_zone.py` & `octodns-1.0.0rc1/tests/test_octodns_zone.py`

 * *Files 9% similar despite different names*

```diff
@@ -182,16 +182,45 @@
         self.assertIsInstance(changes[0], Delete)
 
     def test_missing_dot(self):
         with self.assertRaises(Exception) as ctx:
             Zone('not.allowed', [])
         self.assertTrue('missing ending dot' in str(ctx.exception))
 
-    def test_sub_zones(self):
+    def test_whitespace(self):
+        with self.assertRaises(Exception) as ctx:
+            Zone('space not allowed.', [])
+        self.assertTrue('whitespace not allowed' in str(ctx.exception))
+
+    def test_owns(self):
+        zone = Zone('unit.tests.', set(['sub']))
+
+        self.assertTrue(zone.owns('A', 'unit.tests'))
+        self.assertTrue(zone.owns('A', 'unit.tests.'))
+        self.assertTrue(zone.owns('A', 'www.unit.tests.'))
+        self.assertTrue(zone.owns('A', 'www.unit.tests.'))
+        # we do own our direct sub's delegation NS records
+        self.assertTrue(zone.owns('NS', 'sub.unit.tests.'))
+
+        # we don't own the root of our sub
+        self.assertFalse(zone.owns('A', 'sub.unit.tests.'))
 
+        # of anything under it
+        self.assertFalse(zone.owns('A', 'www.sub.unit.tests.'))
+
+        # including subsequent delegatoin NS records
+        self.assertFalse(zone.owns('NS', 'below.sub.unit.tests.'))
+
+        # edge cases
+        # we don't own something that ends with our name, but isn't a boundary
+        self.assertFalse(zone.owns('A', 'foo-unit.tests.'))
+        # we do something that ends with the sub-zone, but isn't at a boundary
+        self.assertTrue(zone.owns('A', 'foo-sub.unit.tests.'))
+
+    def test_sub_zones(self):
         # NS for exactly the sub is allowed
         zone = Zone('unit.tests.', set(['sub', 'barred']))
         record = Record.new(
             zone,
             'sub',
             {'ttl': 3600, 'type': 'NS', 'values': ['1.2.3.4.', '2.3.4.5.']},
         )
```

### Comparing `octodns-1.0.0rc0/tests/zones/2.0.192.in-addr.arpa.` & `octodns-1.0.0rc1/tests/zones/2.0.192.in-addr.arpa.`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/zones/invalid.records.tst` & `octodns-1.0.0rc1/tests/zones/invalid.records.tst`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/zones/tinydns/.is-needed-for-tests` & `octodns-1.0.0rc1/tests/zones/tinydns/.is-needed-for-tests`

 * *Files identical despite different names*

### Comparing `octodns-1.0.0rc0/tests/zones/unit.tests.` & `octodns-1.0.0rc1/tests/zones/unit.tests.`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 ; NS Records
 @           3600  IN  NS  ns1.unit.tests.
 @           3600  IN  NS  ns2.unit.tests.
 under       3600  IN  NS  ns1.unit.tests.
 under       3600  IN  NS  ns2.unit.tests.
 
+; SSHFP Records
+@           600   IN  SSHFP 1 1 bf6b6825d2977c511a475bbefb88aad54a92ac73
+@           600   IN  SSHFP 1 1 7491973e5f8b39d5327cd4e08bc81b05f7710b49
+
 ; CAA Records
 caa         1800  IN  CAA 0 issue "ca.unit.tests"
 caa         1800  IN  CAA 0 iodef "mailto:admin@unit.tests"
 
 ; SRV Records
 _srv._tcp   600   IN  SRV 10 20 30 foo-1.unit.tests.
 _srv._tcp   600   IN  SRV 10 20 30 foo-2.unit.tests.
```

### Comparing `octodns-1.0.0rc0/tests/zones/unit.tests.tst` & `octodns-1.0.0rc1/tests/zones/unit.tests.tst`

 * *Files identical despite different names*

